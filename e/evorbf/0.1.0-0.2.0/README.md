# Comparing `tmp/evorbf-0.1.0.tar.gz` & `tmp/evorbf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evorbf-0.1.0.tar", last modified: Tue May  7 16:58:57 2024, max compression
+gzip compressed data, was "evorbf-0.2.0.tar", last modified: Sat May 11 03:18:42 2024, max compression
```

## Comparing `evorbf-0.1.0.tar` & `evorbf-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:57.026266 evorbf-0.1.0/
--rw-rw-rw-   0        0        0     3433 2020-08-04 06:14:52.000000 evorbf-0.1.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1458 2024-05-07 16:04:28.000000 evorbf-0.1.0/ChangeLog.md
--rw-rw-rw-   0        0        0    35823 2023-07-27 04:10:18.000000 evorbf-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       71 2024-05-07 16:04:28.000000 evorbf-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    10272 2024-05-07 16:58:57.026266 evorbf-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6321 2024-05-07 16:49:13.000000 evorbf-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.912381 evorbf-0.1.0/drafts/
--rw-rw-rw-   0        0        0      320 2023-08-15 09:38:29.000000 evorbf-0.1.0/drafts/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-11-22 03:09:10.000000 evorbf-0.1.0/drafts/activation.py
--rw-rw-rw-   0        0        0    20273 2023-12-01 14:40:29.000000 evorbf-0.1.0/drafts/base_rbf_numpy.py
--rw-rw-rw-   0        0        0     8888 2023-09-23 04:13:31.000000 evorbf-0.1.0/drafts/base_rbf_torch.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.925710 evorbf-0.1.0/drafts/examples/
--rw-rw-rw-   0        0        0      243 2023-08-14 15:29:51.000000 evorbf-0.1.0/drafts/examples/__init__.py
--rw-rw-rw-   0        0        0     2588 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/exam_classification.py
--rw-rw-rw-   0        0        0     2920 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/exam_gridsearch.py
--rw-rw-rw-   0        0        0     2979 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/exam_knn_vs_elm_multi_class.py
--rw-rw-rw-   0        0        0     1315 2023-09-20 12:41:32.000000 evorbf-0.1.0/drafts/examples/exam_regression.py
--rw-rw-rw-   0        0        0     1847 2023-09-20 12:42:57.000000 evorbf-0.1.0/drafts/examples/exam_standard_elm_binary_class.py
--rw-rw-rw-   0        0        0     1283 2023-09-20 12:42:41.000000 evorbf-0.1.0/drafts/examples/exam_standard_elm_regression.py
--rw-rw-rw-   0        0        0     1989 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/exam_svc_vs_elm_binary_class.py
--rw-rw-rw-   0        0        0     2084 2023-09-20 12:41:32.000000 evorbf-0.1.0/drafts/examples/exam_svr_vs_elm_regression.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.932690 evorbf-0.1.0/drafts/examples/utils/
--rw-rw-rw-   0        0        0      320 2023-08-14 15:29:51.000000 evorbf-0.1.0/drafts/examples/utils/__init__.py
--rw-rw-rw-   0        0        0      550 2023-09-20 12:23:49.000000 evorbf-0.1.0/drafts/examples/utils/exam_data_loader.py
--rw-rw-rw-   0        0        0     1359 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/utils/exam_get_weights.py
--rw-rw-rw-   0        0        0     1752 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/utils/exam_save_load_model.py
--rw-rw-rw-   0        0        0     1499 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/utils/exam_save_results.py
--rw-rw-rw-   0        0        0     1533 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/examples/utils/exam_save_y_predicted.py
--rw-rw-rw-   0        0        0     1747 2023-09-20 12:23:49.000000 evorbf-0.1.0/drafts/examples/utils/exam_scaler.py
--rw-rw-rw-   0        0        0     7268 2023-09-22 10:04:28.000000 evorbf-0.1.0/drafts/haha.py
--rw-rw-rw-   0        0        0     2514 2023-09-21 07:55:15.000000 evorbf-0.1.0/drafts/haha01.py
--rw-rw-rw-   0        0        0     2759 2023-09-21 06:40:34.000000 evorbf-0.1.0/drafts/haha02.py
--rw-rw-rw-   0        0        0     2970 2023-09-21 08:16:04.000000 evorbf-0.1.0/drafts/haha03.py
--rw-rw-rw-   0        0        0     3109 2023-09-21 09:20:46.000000 evorbf-0.1.0/drafts/haha04.py
--rw-rw-rw-   0        0        0     3034 2023-09-21 09:27:36.000000 evorbf-0.1.0/drafts/haha05.py
--rw-rw-rw-   0        0        0     2786 2023-09-21 09:28:55.000000 evorbf-0.1.0/drafts/haha06.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.955746 evorbf-0.1.0/drafts/model/
--rw-rw-rw-   0        0        0      320 2023-09-22 10:04:28.000000 evorbf-0.1.0/drafts/model/__init__.py
--rw-rw-rw-   0        0        0     7656 2023-12-01 14:44:41.000000 evorbf-0.1.0/drafts/model/mha_rbf.py
--rw-rw-rw-   0        0        0     9800 2023-12-01 14:44:41.000000 evorbf-0.1.0/drafts/model/standard_rbf.py
--rw-rw-rw-   0        0        0      809 2023-09-20 12:42:57.000000 evorbf-0.1.0/drafts/test_ElmClassifier.py
--rw-rw-rw-   0        0        0      891 2023-09-20 12:42:41.000000 evorbf-0.1.0/drafts/test_ElmRegressor.py
--rw-rw-rw-   0        0        0      886 2023-09-20 12:41:47.000000 evorbf-0.1.0/drafts/test_MhaElmClassifier.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.955746 evorbf-0.1.0/evorbf/
--rw-rw-rw-   0        0        0      493 2024-05-07 16:04:28.000000 evorbf-0.1.0/evorbf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.988460 evorbf-0.1.0/evorbf/core/
--rw-rw-rw-   0        0        0      320 2024-05-07 08:45:39.000000 evorbf-0.1.0/evorbf/core/__init__.py
--rw-rw-rw-   0        0        0    20057 2024-05-07 15:50:24.000000 evorbf-0.1.0/evorbf/core/base_rbf.py
--rw-rw-rw-   0        0        0     7654 2024-05-07 15:50:24.000000 evorbf-0.1.0/evorbf/core/ina_rbf.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:57.025733 evorbf-0.1.0/evorbf/helpers/
--rw-rw-rw-   0        0        0      320 2023-08-10 12:25:40.000000 evorbf-0.1.0/evorbf/helpers/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-08-10 12:25:40.000000 evorbf-0.1.0/evorbf/helpers/metrics.py
--rw-rw-rw-   0        0        0     7841 2024-05-07 08:47:57.000000 evorbf-0.1.0/evorbf/helpers/preprocessor.py
--rw-rw-rw-   0        0        0     7807 2023-11-22 03:06:59.000000 evorbf-0.1.0/evorbf/helpers/scaler.py
--rw-rw-rw-   0        0        0     3660 2023-08-10 12:25:40.000000 evorbf-0.1.0/evorbf/helpers/validator.py
-drwxrwxrwx   0        0        0        0 2024-05-07 16:58:56.984170 evorbf-0.1.0/evorbf.egg-info/
--rw-rw-rw-   0        0        0    10272 2024-05-07 16:58:56.000000 evorbf-0.1.0/evorbf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2024-05-07 16:58:56.000000 evorbf-0.1.0/evorbf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 16:58:56.000000 evorbf-0.1.0/evorbf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-07 16:58:56.000000 evorbf-0.1.0/evorbf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-07 16:58:56.000000 evorbf-0.1.0/evorbf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 16:58:57.026266 evorbf-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4015 2024-05-07 16:25:59.000000 evorbf-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.843928 evorbf-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-11 03:17:58.000000 evorbf-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 03:17:58.000000 evorbf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 03:17:58.000000 evorbf-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-11 03:18:42.843928 evorbf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-11 03:17:58.000000 evorbf-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.839928 evorbf-0.2.0/evorbf/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.839928 evorbf-0.2.0/evorbf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/core/base_rbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/core/ina_rbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/core/standard_rbf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.839928 evorbf-0.2.0/evorbf/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/helpers/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/helpers/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/helpers/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-11 03:17:58.000000 evorbf-0.2.0/evorbf/helpers/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.839928 evorbf-0.2.0/evorbf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-11 03:18:42.000000 evorbf-0.2.0/evorbf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-11 03:18:42.000000 evorbf-0.2.0/evorbf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:18:42.000000 evorbf-0.2.0/evorbf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-11 03:18:42.000000 evorbf-0.2.0/evorbf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 03:18:42.000000 evorbf-0.2.0/evorbf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:18:42.843928 evorbf-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-11 03:17:58.000000 evorbf-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:18:42.839928 evorbf-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-11 03:17:58.000000 evorbf-0.2.0/tests/test_InaRbfClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-11 03:17:58.000000 evorbf-0.2.0/tests/test_InaRbfRegressor.py
```

### Comparing `evorbf-0.1.0/CODE_OF_CONDUCT.md` & `evorbf-0.2.0/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-In the interest of fostering an open and welcoming environment, we as
-contributors and maintainers pledge to making participation in our project and
-our community a harassment-free experience for everyone, regardless of age, body
-size, disability, ethnicity, sex characteristics, gender identity and expression,
-level of experience, education, socio-economic status, nationality, personal
-appearance, race, religion, or sexual identity and orientation.
-
-## Our Standards
-
-Examples of behavior that contributes to creating a positive environment
-include:
-
-* Using welcoming and inclusive language
-* Being respectful of differing viewpoints and experiences
-* Gracefully accepting constructive criticism
-* Focusing on what is best for the community
-* Showing empathy towards other community members
-
-Examples of unacceptable behavior by participants include:
-
-* The use of sexualized language or imagery and unwelcome sexual attention or
- advances
-* Trolling, insulting/derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or electronic
- address, without explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
- professional setting
-
-## Our Responsibilities
-
-Project maintainers are responsible for clarifying the standards of acceptable
-behavior and are expected to take appropriate and fair corrective action in
-response to any instances of unacceptable behavior.
-
-Project maintainers have the right and responsibility to remove, edit, or
-reject comments, commits, code, wiki edits, issues, and other contributions
-that are not aligned to this Code of Conduct, or to ban temporarily or
-permanently any contributor for other behaviors that they deem inappropriate,
-threatening, offensive, or harmful.
-
-## Scope
-
-This Code of Conduct applies both within project spaces and in public spaces
-when an individual is representing the project or its community. Examples of
-representing a project or community include using an official project e-mail
-address, posting via an official social media account, or acting as an appointed
-representative at an online or offline event. Representation of a project may be
-further defined and clarified by project maintainers.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behavior may be
-reported by contacting the project team at nguyenthieu2102@gmail.com. All
-complaints will be reviewed and investigated and will result in a response that
-is deemed necessary and appropriate to the circumstances. The project team is
-obligated to maintain confidentiality with regard to the reporter of an incident.
-Further details of specific enforcement policies may be posted separately.
-
-Project maintainers who do not follow or enforce the Code of Conduct in good
-faith may face temporary or permanent repercussions as determined by other
-members of the project's leadership.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
-available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
-
-[homepage]: https://www.contributor-covenant.org
-
-For answers to common questions about this code of conduct, see
-https://www.contributor-covenant.org/faq
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+In the interest of fostering an open and welcoming environment, we as
+contributors and maintainers pledge to making participation in our project and
+our community a harassment-free experience for everyone, regardless of age, body
+size, disability, ethnicity, sex characteristics, gender identity and expression,
+level of experience, education, socio-economic status, nationality, personal
+appearance, race, religion, or sexual identity and orientation.
+
+## Our Standards
+
+Examples of behavior that contributes to creating a positive environment
+include:
+
+* Using welcoming and inclusive language
+* Being respectful of differing viewpoints and experiences
+* Gracefully accepting constructive criticism
+* Focusing on what is best for the community
+* Showing empathy towards other community members
+
+Examples of unacceptable behavior by participants include:
+
+* The use of sexualized language or imagery and unwelcome sexual attention or
+ advances
+* Trolling, insulting/derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or electronic
+ address, without explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+ professional setting
+
+## Our Responsibilities
+
+Project maintainers are responsible for clarifying the standards of acceptable
+behavior and are expected to take appropriate and fair corrective action in
+response to any instances of unacceptable behavior.
+
+Project maintainers have the right and responsibility to remove, edit, or
+reject comments, commits, code, wiki edits, issues, and other contributions
+that are not aligned to this Code of Conduct, or to ban temporarily or
+permanently any contributor for other behaviors that they deem inappropriate,
+threatening, offensive, or harmful.
+
+## Scope
+
+This Code of Conduct applies both within project spaces and in public spaces
+when an individual is representing the project or its community. Examples of
+representing a project or community include using an official project e-mail
+address, posting via an official social media account, or acting as an appointed
+representative at an online or offline event. Representation of a project may be
+further defined and clarified by project maintainers.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behavior may be
+reported by contacting the project team at nguyenthieu2102@gmail.com. All
+complaints will be reviewed and investigated and will result in a response that
+is deemed necessary and appropriate to the circumstances. The project team is
+obligated to maintain confidentiality with regard to the reporter of an incident.
+Further details of specific enforcement policies may be posted separately.
+
+Project maintainers who do not follow or enforce the Code of Conduct in good
+faith may face temporary or permanent repercussions as determined by other
+members of the project's leadership.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
+available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html
+
+[homepage]: https://www.contributor-covenant.org
+
+For answers to common questions about this code of conduct, see
+https://www.contributor-covenant.org/faq
```

### Comparing `evorbf-0.1.0/LICENSE` & `evorbf-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `evorbf-0.1.0/README.md` & `evorbf-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,130 +1,153 @@
-
-<p align="center">
-<img style="max-width:100%;" src="https://thieu1995.github.io/post/2023-08/evorbf1.png" alt="EvoRBF"/>
-</p>
-
----
-
-
-[![GitHub release](https://img.shields.io/badge/release-0.1.0-yellow.svg)](https://github.com/thieu1995/evorbf/releases)
-[![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/evorbf) 
-[![PyPI version](https://badge.fury.io/py/evorbf.svg)](https://badge.fury.io/py/evorbf)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evorbf.svg)
-![PyPI - Status](https://img.shields.io/pypi/status/evorbf.svg)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/evorbf.svg)
-[![Downloads](https://static.pepy.tech/badge/evorbf)](https://pepy.tech/project/evorbf)
-[![Tests & Publishes to PyPI](https://github.com/thieu1995/evorbf/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/evorbf/actions/workflows/publish-package.yaml)
-![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/evorbf.svg)
-[![Documentation Status](https://readthedocs.org/projects/evorbf/badge/?version=latest)](https://evorbf.readthedocs.io/en/latest/?badge=latest)
-[![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
-![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/evorbf.svg)
-[![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8249045.svg)](https://doi.org/10.5281/zenodo.8249045)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-
-
-EvoRBF (Evolving Radial Basis Function Network) is a Python library that implements a framework 
-for training Radial Basis Function (RBF) networks using Intelligence Nature-inspired Algorithms (INAs). It provides a 
-comparable alternative to the traditional RBF network and is compatible with the Scikit-Learn library. With EvoRBF, you can 
-perform searches and hyperparameter tuning using the functionalities provided by the Scikit-Learn library.
-
-* **Free software:** GNU General Public License (GPL) V3 license
-* **Provided Estimator**: RbfRegressor, RbfClassifier, InaRbfRegressor, InaRbfClassifier
-* **Total InaRBf models**: > 400 Models
-* **Supported performance metrics**: >= 67 (47 regressions and 20 classifications)
-* **Supported loss functions**: >= 61 (45 regressions and 16 classifications)
-* **Documentation:** https://evorbf.readthedocs.io/en/latest/
-* **Python versions:** >= 3.7.x
-* **Dependencies:** numpy, scipy, scikit-learn, pandas, mealpy, permetrics
-
-
-# Citation Request 
-
-If you want to understand how Intelligence Nature-inspired Algorithms is applied to Radial Basis Function Network, you 
-need to read the paper titled "Application of artificial intelligence in estimating mining capital expenditure using radial basis function neural network optimized by metaheuristic algorithms". 
-The paper can be accessed at the following [this link](https://doi.org/10.1016/B978-0-443-18764-3.00015-1)
-
-
-# Usage
-
-* Install the [current PyPI release](https://pypi.python.org/pypi/evorbf):
-```sh 
-$ pip install evorbf
-```
-
-After installation, you can check EvoRBF version:
-
-```sh
-$ python
->>> import evorbf
->>> evorbf.__version__
-```
-
-In this section, we will explore the usage of the EvoRBF model with the assistance of a dataset. While all the 
-preprocessing steps mentioned below can be replicated using Scikit-Learn, we have implemented some utility functions 
-to provide users with convenience and faster usage.  
-
-```python
-import numpy as np
-from evorbf import Data, InaRbfRegressor
-from sklearn.datasets import load_diabetes
-
-## Load data object
-# total samples = 442, total features = 10
-X, y = load_diabetes(return_X_y=True)
-data = Data(X, y)
-
-## Split train and test
-data.split_train_test(test_size=0.2, random_state=2)
-print(data.X_train.shape, data.X_test.shape)
-
-## Scaling dataset
-data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard"))
-data.X_test = scaler_X.transform(data.X_test)
-
-data.y_train, scaler_y = data.scale(data.y_train, scaling_methods=("standard", ))
-data.y_test = scaler_y.transform(np.reshape(data.y_test, (-1, 1)))
-
-## Create model
-opt_paras = {"name": "WOA", "epoch": 500, "pop_size": 20}
-model = InaRbfRegressor(size_hidden=25, center_finder="kmean", regularization=False, lamda=0.5, obj_name="MSE",
-                        optimizer="BaseGA", optimizer_paras=opt_paras, verbose=True, seed=42)
-
-## Train the model
-model.fit(data.X_train, data.y_train, lb=-1., ub=2.)
-
-## Test the model
-y_pred = model.predict(data.X_test)
-
-print(model.optimizer.g_best.solution)
-## Calculate some metrics
-print(model.score(X=data.X_test, y=data.y_test, method="RMSE"))
-print(model.scores(X=data.X_test, y=data.y_test, list_methods=["R2", "R", "KGE", "MAPE"]))
-print(model.evaluate(y_true=data.y_test, y_pred=y_pred, list_metrics=["MSE", "RMSE", "R2S", "NSE", "KGE", "MAPE"]))
-```
-
-A real-world dataset contains features that vary in magnitudes, units, and range. We would suggest performing 
-normalization when the scale of a feature is irrelevant or misleading. Feature Scaling basically helps to normalize 
-the data within a particular range.
-
-
-# Support (questions, problems)
-
-### Official Links 
-
-* Official source code repo: https://github.com/thieu1995/evorbf
-* Official document: https://evorbf.readthedocs.io/
-* Download releases: https://pypi.org/project/evorbf/
-* Issue tracker: https://github.com/thieu1995/evorbf/issues
-* Notable changes log: https://github.com/thieu1995/evorbf/blob/master/ChangeLog.md
-* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
-
-* This project also related to our another projects which are "optimization" and "machine learning", check it here:
-    * https://github.com/thieu1995/mealpy
-    * https://github.com/thieu1995/metaheuristics
-    * https://github.com/thieu1995/opfunu
-    * https://github.com/thieu1995/enoppy
-    * https://github.com/thieu1995/permetrics
-    * https://github.com/thieu1995/MetaCluster
-    * https://github.com/thieu1995/pfevaluator
-    * https://github.com/aiir-team
+
+<p align="center">
+<img style="max-width:100%;" src="https://thieu1995.github.io/post/2023-08/evorbf1.png" alt="EvoRBF"/>
+</p>
+
+---
+
+
+[![GitHub release](https://img.shields.io/badge/release-0.2.0-yellow.svg)](https://github.com/thieu1995/evorbf/releases)
+[![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/evorbf) 
+[![PyPI version](https://badge.fury.io/py/evorbf.svg)](https://badge.fury.io/py/evorbf)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evorbf.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/evorbf.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/evorbf.svg)
+[![Downloads](https://static.pepy.tech/badge/evorbf)](https://pepy.tech/project/evorbf)
+[![Tests & Publishes to PyPI](https://github.com/thieu1995/evorbf/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/evorbf/actions/workflows/publish-package.yaml)
+![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/evorbf.svg)
+[![Documentation Status](https://readthedocs.org/projects/evorbf/badge/?version=latest)](https://evorbf.readthedocs.io/en/latest/?badge=latest)
+[![Chat](https://img.shields.io/badge/Chat-on%20Telegram-blue)](https://t.me/+fRVCJGuGJg1mNDg1)
+![GitHub contributors](https://img.shields.io/github/contributors/thieu1995/evorbf.svg)
+[![GitTutorial](https://img.shields.io/badge/PR-Welcome-%23FF8300.svg?)](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11136007.svg)](https://doi.org/10.5281/zenodo.11136007)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+
+
+**EvoRBF** is a Python library that implements a framework 
+for training Radial Basis Function (RBF) networks using `Intelligence Nature-inspired Algorithms (INAs)`. It provides a 
+comparable alternative to the traditional RBF network and is compatible with the Scikit-Learn library. With EvoRBF, you can 
+perform searches and hyperparameter tuning using the functionalities provided by the Scikit-Learn library.
+
+| **EvoRBF**                           | **Evolving Radial Basis Function Network**                     |
+|--------------------------------------|----------------------------------------------------------------|
+| **Free software**                    | GNU General Public License (GPL) V3 license                    |
+| **Provided Estimator**               | RbfRegressor, RbfClassifier, InaRbfRegressor, InaRbfClassifier |
+| **Provided machine learning models** | \> 400 Models                                                  |
+| **Supported performance metrics**    | \>= 67 (47 regressions and 20 classifications)                 |
+| **Supported loss functions**         | \>= 61 (45 regressions and 16 classifications)                 |
+| **Documentation**                    | https://evorbf.readthedocs.io                                  | 
+| **Python versions**                  | \>= 3.8.x                                                      |  
+| **Dependencies**                     | numpy, scipy, scikit-learn, pandas, mealpy, permetrics         |
+
+
+# Citation Request 
+
+If you want to understand how Intelligence Nature-inspired Algorithms is applied to Radial Basis Function Network, you 
+need to read the paper titled "Application of artificial intelligence in estimating mining capital expenditure using radial basis function neural network optimized by metaheuristic algorithms". 
+The paper can be accessed at the following [this link](https://doi.org/10.1016/B978-0-443-18764-3.00015-1)
+
+
+```bibtex
+@software{thieu_2024_11136008,
+  author       = {Nguyen Van Thieu},
+  title        = {EvoRBF: Evolving Radial Basis Function Network by Intelligent Nature-inspired Algorithms},
+  month        = may,
+  year         = 2024,
+  publisher    = {Zenodo},
+  doi          = {10.5281/zenodo.11136007},
+  url          = {https://doi.org/10.5281/zenodo.11136007}
+}
+
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier},
+  doi={10.1016/j.sysarc.2023.102871}
+}
+```
+
+
+# Usage
+
+* Install the [current PyPI release](https://pypi.python.org/pypi/evorbf):
+```sh 
+$ pip install evorbf
+```
+
+After installation, you can check EvoRBF version:
+
+```sh
+$ python
+>>> import evorbf
+>>> evorbf.__version__
+```
+
+In this example below, we will use Whale Optimization Algorithm to optimize the Signma and Weights of hidden layer 
+in RBF network (WOA-RBF model) for Diabetes prediction problem.
+
+```python
+import numpy as np
+from evorbf import Data, InaRbfRegressor
+from sklearn.datasets import load_diabetes
+
+## Load data object
+# total samples = 442, total features = 10
+X, y = load_diabetes(return_X_y=True)
+data = Data(X, y)
+
+## Split train and test
+data.split_train_test(test_size=0.2, random_state=2)
+print(data.X_train.shape, data.X_test.shape)
+
+## Scaling dataset
+data.X_train, scaler_X = data.scale(data.X_train, scaling_methods=("standard"))
+data.X_test = scaler_X.transform(data.X_test)
+
+data.y_train, scaler_y = data.scale(data.y_train, scaling_methods=("standard", ))
+data.y_test = scaler_y.transform(np.reshape(data.y_test, (-1, 1)))
+
+## Create model
+opt_paras = {"name": "WOA", "epoch": 500, "pop_size": 20}
+model = InaRbfRegressor(size_hidden=25, center_finder="kmean", regularization=False, lamda=0.5, obj_name="MSE",
+                        optimizer="BaseGA", optimizer_paras=opt_paras, verbose=True, seed=42)
+
+## Train the model
+model.fit(data.X_train, data.y_train, lb=-1., ub=2.)
+
+## Test the model
+y_pred = model.predict(data.X_test)
+
+print(model.optimizer.g_best.solution)
+## Calculate some metrics
+print(model.score(X=data.X_test, y=data.y_test, method="RMSE"))
+print(model.scores(X=data.X_test, y=data.y_test, list_methods=["R2", "R", "KGE", "MAPE"]))
+print(model.evaluate(y_true=data.y_test, y_pred=y_pred, list_metrics=["MSE", "RMSE", "R2S", "NSE", "KGE", "MAPE"]))
+```
+
+A real-world dataset contains features that vary in magnitudes, units, and range. We would suggest performing 
+normalization when the scale of a feature is irrelevant or misleading. Feature Scaling basically helps to normalize 
+the data within a particular range.
+
+
+# Support (questions, problems)
+
+### Official Links 
+
+* Official source code repo: https://github.com/thieu1995/evorbf
+* Official document: https://evorbf.readthedocs.io/
+* Download releases: https://pypi.org/project/evorbf/
+* Issue tracker: https://github.com/thieu1995/evorbf/issues
+* Notable changes log: https://github.com/thieu1995/evorbf/blob/master/ChangeLog.md
+* Official chat group: https://t.me/+fRVCJGuGJg1mNDg1
+
+* This project also related to our another projects which are "optimization" and "machine learning", check it here:
+    * https://github.com/thieu1995/mealpy
+    * https://github.com/thieu1995/metaheuristics
+    * https://github.com/thieu1995/opfunu
+    * https://github.com/thieu1995/enoppy
+    * https://github.com/thieu1995/permetrics
+    * https://github.com/thieu1995/MetaCluster
+    * https://github.com/thieu1995/pfevaluator
+    * https://github.com/aiir-team
```

### Comparing `evorbf-0.1.0/drafts/base_rbf_numpy.py` & `evorbf-0.2.0/evorbf/core/base_rbf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,477 +1,460 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 09:48, 17/08/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import pickle
-import numpy as np
-import pandas as pd
-from pathlib import Path
-from permetrics import RegressionMetric, ClassificationMetric
-from sklearn.base import BaseEstimator
-from mealpy import get_optimizer_by_name, Optimizer, get_all_optimizers
-from sklearn.cluster import KMeans
-
-from evorbf.helpers import activation, validator
-from evorbf.helpers.metrics import get_all_regression_metrics, get_all_classification_metrics
-
-
-class RBF01:
-    """Radial Basis Function version 01
-
-    This class defines the general RBF model that:
-        + use non-linear Gaussian function
-        + use inverse matrix multiplication instead of Gradient-based
-        + have no regulation term
-
-    Parameters
-    ----------
-    size_input : int, default=5
-        The number of input nodes
-
-    size_hidden : int, default=10
-        The number of hidden nodes
-
-    size_output : int, default=1
-        The number of output nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-    """
-    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=(1.0, ), **kwargs):
-        self.size_hidden = size_hidden
-        self.center_finder = center_finder
-        self.sigmas = sigmas
-        self.centers, self.weights, self.weights_shape = None, None, None
-
-    @staticmethod
-    def calculate_centers(X, method="kmean", n_clusters=5):
-        if method == "kmean":
-            kobj = KMeans(n_clusters=n_clusters, init='random', random_state=11).fit(X)
-            return kobj.cluster_centers_
-        elif method == "random":
-            return X[np.random.choice(len(X), n_clusters, replace=False)]
-
-    @staticmethod
-    def calculate_rbf(X, c, sigmas):
-        # Calculate Radial Basis Function (Gaussian)
-        return np.exp(-np.sum((X - c)**2, axis=1) / (2 * sigmas**2))
-
-    def transform_X(self, X):
-        # Calculate RBF layer outputs
-        if self.centers is None or self.weights is None:
-            raise Exception("Model not trained.")
-        rbf_layer = np.zeros((X.shape[0], self.size_hidden))
-        for i in range(X.shape[0]):
-            rbf_layer[i] = self.calculate_rbf(X[i], self.centers, self.sigmas)
-        return rbf_layer
-
-    def fit(self, X, y):
-        """Fit the model to data matrix X and target(s) y.
-
-        Parameters
-        ----------
-        X : ndarray or sparse matrix of shape (n_samples, n_features)
-            The input data.
-
-        y : ndarray of shape (n_samples,) or (n_samples, n_outputs)
-            The target values (class labels in classification, real numbers in regression).
-
-        Returns
-        -------
-        self : object
-            Returns a trained RBF model.
-        """
-        # Initialize centers
-        self.centers = self.calculate_centers(X, self.center_finder, self.size_hidden)
-        # Calculate RBF layer outputs
-        rbf_layer = self.transform_X(X)
-        # Solve for weights using pseudo-inverse
-        self.weights = np.linalg.pinv(rbf_layer) @ y
-        return self
-
-    def predict(self, X):
-        """Predict using the Radial Basis Function model.
-
-        Parameters
-        ----------
-        X : {array-like, sparse matrix} of shape (n_samples, n_features)
-            The input data.
-
-        Returns
-        -------
-        y : ndarray of shape (n_samples, n_outputs)
-            The predicted values.
-        """
-        rbf_layer = self.transform_X(X)
-        return rbf_layer @ self.weights
-    
-    def update_parameters_by_solution(self, solution, X, y):
-        if self.centers is None:
-            self.centers = self.calculate_centers(X, self.center_finder, self.size_hidden)
-        if self.weights_shape is None:
-            if y.ndim == 1:
-                self.weights_shape = (self.size_hidden, 1)
-            else:
-                self.weights_shape = (self.size_hidden, y.shape[1])
-        self.sigmas = solution[:self.size_hidden]
-        self.weights = np.reshape(solution[self.size_hidden:], self.weights_shape)
-    
-    def get_weights(self):
-        return self.weights
-
-    def set_weights(self, weights):
-        self.weights = weights
-
-
-class RBF02(RBF01):
-    """Radial Basis Function version 02
-
-    This class defines the general RBF model that:
-        + use non-linear Gaussian function
-        + use inverse matrix multiplication instead of Gradient-based
-        + have regulation term with hyper-parameter `lamda`
-
-    Parameters
-    ----------
-    size_input : int, default=5
-        The number of input nodes
-
-    size_hidden : int, default=10
-        The number of hidden nodes
-
-    size_output : int, default=1
-        The number of output nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-    """
-    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=(1.0,), lamda=0.01, **kwargs):
-        super().__init__(size_hidden, center_finder, sigmas, **kwargs)
-        self.lamda = lamda
-
-    def fit(self, X, y):
-        # Initialize centers
-        self.centers = self.calculate_centers(X, self.center_finder, self.size_hidden)
-        # Calculate RBF layer outputs
-        rbf_layer = self.transform_X(X)
-        # Solve for weights using ridge regression (L2 regularization)
-        iden = np.identity(self.size_hidden)
-        self.weights = np.linalg.inv(rbf_layer.T @ rbf_layer + self.lamda * iden) @ rbf_layer.T @ y
-        return self
-
-
-class BaseRbf(BaseEstimator):
-    """
-    Defines the most general class for RBF network that inherits the BaseEstimator class of Scikit-Learn library.
-
-    Parameters
-    ----------
-    hidden_size : int, default=10
-        The number of hidden nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-    """
-
-    SUPPORTED_CLS_METRICS = get_all_classification_metrics()
-    SUPPORTED_REG_METRICS = get_all_regression_metrics()
-    CLS_OBJ_LOSSES = None
-
-    def __init__(self, regularization=False, size_hidden=10, center_finder="kmean", sigmas=(1.0, ), lamda=0.01):
-        super().__init__()
-        self._net_class = RBF01
-        if regularization:
-            self._net_class = RBF02
-        self.regularization = regularization
-        self.size_hidden = size_hidden
-        self.center_finder = center_finder
-        self.sigmas = sigmas
-        self.lamda = lamda
-        self.parameters = {}
-        self.network, self.obj_scaler, self.loss_train, self.n_labels = None, None, None, None
-
-    @staticmethod
-    def _check_method(method=None, list_supported_methods=None) -> str:
-        if type(method) is str:
-            return validator.check_str("method", method, list_supported_methods)
-        else:
-            raise ValueError(f"method should be a string and belongs to {list_supported_methods}")
-
-    def create_network(self, X, y):
-        return None, None
-
-    def fit(self, X, y):
-        self.network, self.obj_scaler = self.create_network(X, y)
-        y_scaled = self.obj_scaler.transform(y)
-        self.network.fit(X, y_scaled)
-        return self
-
-    def predict(self, X, return_prob=False):
-        """
-        Inherit the predict function from BaseRbf class, with 1 more parameter `return_prob`.
-
-        Parameters
-        ----------
-        X : {array-like, sparse matrix} of shape (n_samples, n_features)
-            The input data.
-
-        return_prob : bool, default=False
-            It is used for classification problem:
-
-            - If True, the returned results are the probability for each sample
-            - If False, the returned results are the predicted labels
-        """
-        pred = self.network.predict(X)
-        if return_prob:
-            return pred
-        return self.obj_scaler.inverse_transform(pred)
-
-    def __evaluate_reg(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
-        rm = RegressionMetric(y_true=y_true, y_pred=y_pred, decimal=8)
-        return rm.get_metrics_by_list_names(list_metrics)
-
-    def __evaluate_cls(self, y_true, y_pred, list_metrics=("AS", "RS")):
-        cm = ClassificationMetric(y_true, y_pred, decimal=8)
-        return cm.get_metrics_by_list_names(list_metrics)
-    
-    def __score_reg(self, X, y, method="RMSE"):
-        method = self._check_method(method, list(self.SUPPORTED_REG_METRICS.keys()))
-        y_pred = self.network.predict(X)
-        return RegressionMetric(y, y_pred, decimal=8).get_metric_by_name(method)[method]
-    
-    def __scores_reg(self, X, y, list_methods=("MSE", "MAE")):
-        y_pred = self.network.predict(X)
-        return self.__evaluate_reg(y_true=y, y_pred=y_pred, list_metrics=list_methods)
-
-    def __score_cls(self, X, y, method="AS"):
-        method = self._check_method(method, list(self.SUPPORTED_CLS_METRICS.keys()))
-        return_prob = False
-        if self.n_labels > 2:
-            if method in self.CLS_OBJ_LOSSES:
-                return_prob = True
-        y_pred = self.predict(X, return_prob=return_prob)
-        cm = ClassificationMetric(y_true=y, y_pred=y_pred, decimal=8)
-        return cm.get_metric_by_name(method)[method]
-
-    def __scores_cls(self, X, y, list_methods=("AS", "RS")):
-        list_errors = list(set(list_methods) & set(self.CLS_OBJ_LOSSES))
-        list_scores = list((set(self.SUPPORTED_CLS_METRICS.keys()) - set(self.CLS_OBJ_LOSSES)) & set(list_methods))
-        t1 = {}
-        if len(list_errors) > 0:
-            return_prob = False
-            if self.n_labels > 2:
-                return_prob = True
-            y_pred = self.predict(X, return_prob=return_prob)
-            t1 = self.__evaluate_cls(y_true=y, y_pred=y_pred, list_metrics=list_errors)
-        y_pred = self.predict(X, return_prob=False)
-        t2 = self.__evaluate_cls(y_true=y, y_pred=y_pred, list_metrics=list_scores)
-        return {**t2, **t1}
-
-    def evaluate(self, y_true, y_pred, list_metrics=None):
-        """Return the list of performance metrics of the prediction.
-
-        Parameters
-        ----------
-        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            Predicted values for `X`.
-
-        list_metrics : list
-            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        pass
-
-    def score(self, X, y, method=None):
-        """Return the metric of the prediction.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
-            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        method : str, default="RMSE"
-            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        result : float
-            The result of selected metric
-        """
-        pass
-
-    def scores(self, X, y, list_methods=None):
-        """Return the list of metrics of the prediction.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
-            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        list_methods : list, default=("MSE", "MAE")
-            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        pass
-
-    def save_loss_train(self, save_path="history", filename="loss.csv"):
-        ## Save loss train to csv file
-        Path(save_path).mkdir(parents=True, exist_ok=True)
-        if self.loss_train is None:
-            print(f"{self.__class__.__name__} model doesn't have training loss!")
-        else:
-            data = {"epoch": list(range(1, len(self.loss_train) + 1)), "loss": self.loss_train}
-            pd.DataFrame(data).to_csv(f"{save_path}/{filename}", index=False)
-
-    def save_metrics(self, y_true, y_pred, list_metrics=("RMSE", "MAE"), save_path="history", filename="metrics.csv"):
-        ## Save metrics to csv file
-        Path(save_path).mkdir(parents=True, exist_ok=True)
-        results = self.evaluate(y_true, y_pred, list_metrics)
-        df = pd.DataFrame.from_dict(results, orient='index').T
-        df.to_csv(f"{save_path}/{filename}", index=False)
-
-    def save_y_predicted(self, X, y_true, save_path="history", filename="y_predicted.csv"):
-        ## Save the predicted results to csv file
-        Path(save_path).mkdir(parents=True, exist_ok=True)
-        y_pred = self.predict(X, return_prob=False)
-        data = {"y_true": np.squeeze(np.asarray(y_true)), "y_pred": np.squeeze(np.asarray(y_pred))}
-        pd.DataFrame(data).to_csv(f"{save_path}/{filename}", index=False)
-
-    def save_model(self, save_path="history", filename="model.pkl"):
-        ## Save model to pickle file
-        Path(save_path).mkdir(parents=True, exist_ok=True)
-        if filename[-4:] != ".pkl":
-            filename += ".pkl"
-        pickle.dump(self, open(f"{save_path}/{filename}", 'wb'))
-
-    @staticmethod
-    def load_model(load_path="history", filename="model.pkl"):
-        if filename[-4:] != ".pkl":
-            filename += ".pkl"
-        return pickle.load(open(f"{load_path}/{filename}", 'rb'))
-
-
-class BaseMhaRbf(BaseRbf):
-    """
-    Defines the most general class for Metaheuristic-based RBF model that inherits the BaseELM class
-
-    Parameters
-    ----------
-    hidden_size : int, default=10
-        The number of hidden nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-
-    obj_name : None or str, default=None
-        The name of objective for the problem, also depend on the problem is classification and regression.
-
-    optimizer : str or instance of Optimizer class (from Mealpy library), default = "BaseGA"
-        The Metaheuristic Algorithm that use to solve the feature selection problem.
-        Current supported list, please check it here: https://github.com/thieu1995/mealpy.
-        If a custom optimizer is passed, make sure it is an instance of `Optimizer` class.
-
-    optimizer_paras : None or dict of parameter, default=None
-        The parameter for the `optimizer` object.
-        If `None`, the default parameters of optimizer is used (defined in https://github.com/thieu1995/mealpy.)
-        If `dict` is passed, make sure it has at least `epoch` and `pop_size` parameters.
-
-    verbose : bool, default=True
-        Whether to print progress messages to stdout.
-    """
-
-    SUPPORTED_OPTIMIZERS = list(get_all_optimizers().keys())
-    SUPPORTED_CLS_OBJECTIVES = get_all_classification_metrics()
-    SUPPORTED_REG_OBJECTIVES = get_all_regression_metrics()
-
-    def __init__(self, regularization=False, size_hidden=10, center_finder="kmean", sigmas=(1.0, ), lamda=0.01,
-                 obj_name=None, optimizer="BaseGA", optimizer_paras=None, verbose=True):
-        super().__init__(regularization=regularization, size_hidden=size_hidden,
-                         center_finder=center_finder, sigmas=sigmas, lamda=lamda)
-        self.obj_name = obj_name
-        self.optimizer_paras = optimizer_paras
-        self.optimizer = self._set_optimizer(optimizer, optimizer_paras)
-        self.verbose = verbose
-        self.network, self.obj_scaler, self.obj_weights = None, None, None
-
-    def _set_optimizer(self, optimizer=None, optimizer_paras=None):
-        if type(optimizer) is str:
-            opt_class = get_optimizer_by_name(optimizer)
-            if type(optimizer_paras) is dict:
-                return opt_class(**optimizer_paras)
-            else:
-                return opt_class(epoch=500, pop_size=50)
-        elif isinstance(optimizer, Optimizer):
-            if type(optimizer_paras) is dict:
-                return optimizer.set_parameters(optimizer_paras)
-            return optimizer
-        else:
-            raise TypeError(f"optimizer needs to set as a string and supported by Mealpy library.")
-
-    def _get_history_loss(self, optimizer=None):
-        list_global_best = optimizer.history.list_global_best
-        # 2D array / matrix 2D
-        global_obj_list = np.array([agent[1][-1] for agent in list_global_best])
-        # Make each obj_list as a element in array for drawing
-        return global_obj_list[:, 0]
-
-    def fitness_function(self, solution=None):
-        pass
-
-    def fit(self, X, y):
-        self.network, self.obj_scaler = self.create_network(X, y)
-        y_scaled = self.obj_scaler.transform(y)
-        self.X_temp, self.y_temp = X, y_scaled
-        if y_scaled.ndim == 1:
-            problem_size = self.size_hidden + self.size_hidden * 1
-        else:
-            problem_size = self.size_hidden + self.size_hidden * y_scaled.shape[1]
-        lb = [0., ]*self.size_hidden + [-1., ]*(problem_size - self.size_hidden)
-        ub = [10., ]*self.size_hidden + [1., ]*(problem_size - self.size_hidden)
-        log_to = "console" if self.verbose else "None"
-        if self.obj_name is None:
-            raise ValueError("obj_name can't be None")
-        else:
-            if self.obj_name in self.SUPPORTED_REG_OBJECTIVES.keys():
-                minmax = self.SUPPORTED_REG_OBJECTIVES[self.obj_name]
-            elif self.obj_name in self.SUPPORTED_CLS_OBJECTIVES.keys():
-                minmax = self.SUPPORTED_CLS_OBJECTIVES[self.obj_name]
-            else:
-                raise ValueError("obj_name is not supported. Please check the library: permetrics to see the supported objective function.")
-        problem = {
-            "fit_func": self.fitness_function,
-            "lb": lb,
-            "ub": ub,
-            "minmax": minmax,
-            "log_to": log_to,
-            "save_population": False,
-            "obj_weights": self.obj_weights
-        }
-        self.solution, self.best_fit = self.optimizer.solve(problem)
-        self.network.update_parameters_by_solution(self.solution, self.X_temp, self.y_temp)
-        self.loss_train = self._get_history_loss(optimizer=self.optimizer)
-        return self
+#!/usr/bin/env python
+# Created by "Thieu" at 09:48, 17/08/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import pickle
+import numpy as np
+import pandas as pd
+from pathlib import Path
+from permetrics import RegressionMetric, ClassificationMetric
+from sklearn.base import BaseEstimator
+from mealpy import get_optimizer_by_name, Optimizer, get_all_optimizers, FloatVar
+from sklearn.cluster import KMeans
+from evorbf.helpers import validator
+from evorbf.helpers.metrics import get_all_regression_metrics, get_all_classification_metrics
+
+
+class RBF:
+    """Radial Basis Function
+
+    This class defines the general RBF core that:
+        + use non-linear Gaussian function
+        + use inverse matrix multiplication instead of Gradient-based
+        + set up regulation term with hyperparameter `lamda`
+
+    Parameters
+    ----------
+    size_input : int, default=5
+        The number of input nodes
+
+    size_hidden : int, default=10
+        The number of hidden nodes
+
+    size_output : int, default=1
+        The number of output nodes
+
+    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
+        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
+        Activation function for the hidden layer.
+    """
+    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=2.0, regularization=False, lamda=0.01, seed=None):
+        self.size_hidden = size_hidden
+        self.center_finder = center_finder
+        self.sigmas = sigmas
+        self.regularization = regularization
+        self.lamda = lamda
+        self.seed = seed
+        self.centers, self.weights, self.weights_shape = None, None, None
+
+    @staticmethod
+    def calculate_centers(X, method="kmean", n_clusters=5, seed=42):
+        if method == "kmean":
+            kobj = KMeans(n_clusters=n_clusters, n_init='auto', random_state=seed).fit(X)
+            return kobj.cluster_centers_
+        elif method == "random":
+            generator = np.random.default_rng(seed)
+            return X[generator.choice(len(X), n_clusters, replace=False)]
+
+    @staticmethod
+    def calculate_rbf(X, c, sigmas):
+        # Calculate Radial Basis Function (Gaussian)
+        return np.exp(-np.sum((X - c)**2, axis=1) / (2 * sigmas**2))
+
+    def transform_X(self, X):
+        # Calculate RBF layer outputs
+        if self.centers is None:
+            raise Exception("Model is not trained yet.")
+        rbf_layer = np.zeros((X.shape[0], self.size_hidden))
+        for i in range(X.shape[0]):
+            rbf_layer[i] = self.calculate_rbf(X[i], self.centers, self.sigmas)
+        return rbf_layer
+
+    def fit(self, X, y):
+        """Fit the core to data matrix X and target(s) y.
+
+        Parameters
+        ----------
+        X : ndarray or sparse matrix of shape (n_samples, n_features)
+            The input data.
+
+        y : ndarray of shape (n_samples,) or (n_samples, n_outputs)
+            The target values (class labels in classification, real numbers in regression).
+
+        Returns
+        -------
+        self : object
+            Returns a trained RBF core.
+        """
+        # Initialize centers
+        self.centers = self.calculate_centers(X, self.center_finder, self.size_hidden, self.seed)
+        # Calculate RBF layer outputs
+        rbf_layer = self.transform_X(X)
+        if self.regularization:
+            # Solve for weights using ridge regression (L2 regularization)
+            iden = np.identity(self.size_hidden)
+            self.weights = np.linalg.inv(rbf_layer.T @ rbf_layer + self.lamda * iden) @ rbf_layer.T @ y
+        else:
+            # Solve for weights using pseudo-inverse
+            self.weights = np.linalg.pinv(rbf_layer) @ y
+        return self
+
+    def predict(self, X):
+        """Predict using the Radial Basis Function core.
+
+        Parameters
+        ----------
+        X : {array-like, sparse matrix} of shape (n_samples, n_features)
+            The input data.
+
+        Returns
+        -------
+        y : ndarray of shape (n_samples, n_outputs)
+            The predicted values.
+        """
+        rbf_layer = self.transform_X(X)
+        return rbf_layer @ self.weights
+    
+    def update_weights_from_solution(self, solution, X, y):
+        if self.centers is None:
+            self.centers = self.calculate_centers(X, self.center_finder, self.size_hidden, self.seed)
+        if self.weights_shape is None:
+            if y.ndim == 1:
+                self.weights_shape = (self.size_hidden, 1)
+            else:
+                self.weights_shape = (self.size_hidden, y.shape[1])
+        self.sigmas = solution[:self.size_hidden]
+        self.weights = np.reshape(solution[self.size_hidden:], self.weights_shape)
+    
+    def get_weights(self):
+        return self.weights
+
+    def set_weights(self, weights):
+        self.weights = weights
+
+    def get_weights_size(self):
+        return self.weights.size()
+
+
+class BaseRbf(BaseEstimator):
+    """
+    Defines the most general class for RBF network that inherits the BaseEstimator class of Scikit-Learn library.
+
+    Parameters
+    ----------
+    hidden_size : int, default=10
+        The number of hidden nodes
+
+    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
+        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
+        Activation function for the hidden layer.
+    """
+
+    SUPPORTED_CLS_METRICS = get_all_classification_metrics()
+    SUPPORTED_REG_METRICS = get_all_regression_metrics()
+    CLS_OBJ_LOSSES = None
+
+    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=2.0, regularization=False, lamda=0.01, seed=None):
+        super().__init__()
+        self._net_class = RBF
+        self.size_hidden = size_hidden
+        self.center_finder = center_finder
+        self.sigmas = sigmas
+        self.regularization = regularization
+        self.lamda = lamda
+        self.seed = seed
+        self.parameters = {}
+        self.network, self.obj_scaler, self.loss_train, self.n_labels = None, None, None, None
+
+    @staticmethod
+    def _check_method(method=None, list_supported_methods=None) -> str:
+        if type(method) is str:
+            return validator.check_str("method", method, list_supported_methods)
+        else:
+            raise ValueError(f"method should be a string and belongs to {list_supported_methods}")
+
+    def create_network(self, X, y):
+        return None, None
+
+    def fit(self, X, y):
+        self.network, self.obj_scaler = self.create_network(X, y)
+        y_scaled = self.obj_scaler.transform(y)
+        self.network.fit(X, y_scaled)
+        return self
+
+    def predict(self, X, return_prob=False):
+        """
+        Inherit the predict function from BaseRbf class, with 1 more parameter `return_prob`.
+
+        Parameters
+        ----------
+        X : {array-like, sparse matrix} of shape (n_samples, n_features)
+            The input data.
+
+        return_prob : bool, default=False
+            It is used for classification problem:
+
+            - If True, the returned results are the probability for each sample
+            - If False, the returned results are the predicted labels
+        """
+        pred = self.network.predict(X)
+        if return_prob:
+            return pred
+        return self.obj_scaler.inverse_transform(pred)
+
+    def __evaluate_reg(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
+        rm = RegressionMetric(y_true=y_true, y_pred=y_pred)
+        return rm.get_metrics_by_list_names(list_metrics)
+
+    def __evaluate_cls(self, y_true, y_pred, list_metrics=("AS", "RS")):
+        cm = ClassificationMetric(y_true, y_pred)
+        return cm.get_metrics_by_list_names(list_metrics)
+    
+    def __score_reg(self, X, y, method="RMSE"):
+        method = self._check_method(method, list(self.SUPPORTED_REG_METRICS.keys()))
+        y_pred = self.network.predict(X)
+        return RegressionMetric(y, y_pred).get_metric_by_name(method)[method]
+    
+    def __scores_reg(self, X, y, list_methods=("MSE", "MAE")):
+        y_pred = self.network.predict(X)
+        return self.__evaluate_reg(y_true=y, y_pred=y_pred, list_metrics=list_methods)
+
+    def __score_cls(self, X, y, method="AS"):
+        method = self._check_method(method, list(self.SUPPORTED_CLS_METRICS.keys()))
+        return_prob = False
+        if self.n_labels > 2:
+            if method in self.CLS_OBJ_LOSSES:
+                return_prob = True
+        y_pred = self.predict(X, return_prob=return_prob)
+        cm = ClassificationMetric(y_true=y, y_pred=y_pred)
+        return cm.get_metric_by_name(method)[method]
+
+    def __scores_cls(self, X, y, list_methods=("AS", "RS")):
+        list_errors = list(set(list_methods) & set(self.CLS_OBJ_LOSSES))
+        list_scores = list((set(self.SUPPORTED_CLS_METRICS.keys()) - set(self.CLS_OBJ_LOSSES)) & set(list_methods))
+        t1 = {}
+        if len(list_errors) > 0:
+            return_prob = False
+            if self.n_labels > 2:
+                return_prob = True
+            y_pred = self.predict(X, return_prob=return_prob)
+            t1 = self.__evaluate_cls(y_true=y, y_pred=y_pred, list_metrics=list_errors)
+        y_pred = self.predict(X, return_prob=False)
+        t2 = self.__evaluate_cls(y_true=y, y_pred=y_pred, list_metrics=list_scores)
+        return {**t2, **t1}
+
+    def evaluate(self, y_true, y_pred, list_metrics=None):
+        """Return the list of performance metrics of the prediction.
+
+        Parameters
+        ----------
+        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            Predicted values for `X`.
+
+        list_metrics : list
+            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        pass
+
+    def score(self, X, y, method=None):
+        """Return the metric of the prediction.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
+            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        method : str, default="RMSE"
+            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        result : float
+            The result of selected metric
+        """
+        pass
+
+    def scores(self, X, y, list_methods=None):
+        """Return the list of metrics of the prediction.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
+            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        list_methods : list, default=("MSE", "MAE")
+            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        pass
+
+    def save_loss_train(self, save_path="history", filename="loss.csv"):
+        ## Save loss train to csv file
+        Path(save_path).mkdir(parents=True, exist_ok=True)
+        if self.loss_train is None:
+            print(f"{self.__class__.__name__} core doesn't have training loss!")
+        else:
+            data = {"epoch": list(range(1, len(self.loss_train) + 1)), "loss": self.loss_train}
+            pd.DataFrame(data).to_csv(f"{save_path}/{filename}", index=False)
+
+    def save_metrics(self, y_true, y_pred, list_metrics=("RMSE", "MAE"), save_path="history", filename="metrics.csv"):
+        ## Save metrics to csv file
+        Path(save_path).mkdir(parents=True, exist_ok=True)
+        results = self.evaluate(y_true, y_pred, list_metrics)
+        df = pd.DataFrame.from_dict(results, orient='index').T
+        df.to_csv(f"{save_path}/{filename}", index=False)
+
+    def save_y_predicted(self, X, y_true, save_path="history", filename="y_predicted.csv"):
+        ## Save the predicted results to csv file
+        Path(save_path).mkdir(parents=True, exist_ok=True)
+        y_pred = self.predict(X, return_prob=False)
+        data = {"y_true": np.squeeze(np.asarray(y_true)), "y_pred": np.squeeze(np.asarray(y_pred))}
+        pd.DataFrame(data).to_csv(f"{save_path}/{filename}", index=False)
+
+    def save_model(self, save_path="history", filename="core.pkl"):
+        ## Save core to pickle file
+        Path(save_path).mkdir(parents=True, exist_ok=True)
+        if filename[-4:] != ".pkl":
+            filename += ".pkl"
+        pickle.dump(self, open(f"{save_path}/{filename}", 'wb'))
+
+    @staticmethod
+    def load_model(load_path="history", filename="core.pkl"):
+        if filename[-4:] != ".pkl":
+            filename += ".pkl"
+        return pickle.load(open(f"{load_path}/{filename}", 'rb'))
+
+
+class BaseInaRbf(BaseRbf):
+    """
+    Defines the most general class for Intelligence Nature-inspired Algorithm-based RBF core that inherits the BaseELM class
+
+    Parameters
+    ----------
+    hidden_size : int, default=10
+        The number of hidden nodes
+
+    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
+        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
+        Activation function for the hidden layer.
+
+    obj_name : None or str, default=None
+        The name of objective for the problem, also depend on the problem is classification and regression.
+
+    optimizer : str or instance of Optimizer class (from Mealpy library), default = "BaseGA"
+        The Metaheuristic Algorithm that use to solve the feature selection problem.
+        Current supported list, please check it here: https://github.com/thieu1995/mealpy.
+        If a custom optimizer is passed, make sure it is an instance of `Optimizer` class.
+
+    optimizer_paras : None or dict of parameter, default=None
+        The parameter for the `optimizer` object.
+        If `None`, the default parameters of optimizer is used (defined in https://github.com/thieu1995/mealpy.)
+        If `dict` is passed, make sure it has at least `epoch` and `pop_size` parameters.
+
+    verbose : bool, default=True
+        Whether to print progress messages to stdout.
+    """
+
+    SUPPORTED_OPTIMIZERS = list(get_all_optimizers().keys())
+    SUPPORTED_CLS_OBJECTIVES = get_all_classification_metrics()
+    SUPPORTED_REG_OBJECTIVES = get_all_regression_metrics()
+
+    def __init__(self, size_hidden=10, center_finder="kmean", regularization=False, lamda=0.01,
+                 obj_name=None, optimizer="BaseGA", optimizer_paras=None, verbose=True, seed=None):
+        super().__init__(size_hidden=size_hidden, center_finder=center_finder,
+                         regularization=regularization, lamda=lamda, seed=seed)
+        self.obj_name = obj_name
+        self.optimizer_paras = optimizer_paras
+        self.optimizer = self._set_optimizer(optimizer, optimizer_paras)
+        self.verbose = verbose
+        self.network, self.obj_scaler, self.obj_weights = None, None, None
+
+    def _set_optimizer(self, optimizer=None, optimizer_paras=None):
+        if type(optimizer) is str:
+            opt_class = get_optimizer_by_name(optimizer)
+            if type(optimizer_paras) is dict:
+                return opt_class(**optimizer_paras)
+            else:
+                return opt_class(epoch=500, pop_size=50)
+        elif isinstance(optimizer, Optimizer):
+            if type(optimizer_paras) is dict:
+                return optimizer.set_parameters(optimizer_paras)
+            return optimizer
+        else:
+            raise TypeError(f"optimizer needs to set as a string and supported by Mealpy library.")
+
+    def _get_history_loss(self, optimizer=None):
+        list_global_best = optimizer.history.list_global_best
+        # 2D array / matrix 2D
+        return np.array([agent.target.fitness for agent in list_global_best])
+
+    def objective_function(self, solution=None):
+        pass
+
+    def fit(self, X, y, lb=(-1.0, ), ub=(1.0, ), save_population=False):
+        self.network, self.obj_scaler = self.create_network(X, y)
+        y_scaled = self.obj_scaler.transform(y)
+        self.X_temp, self.y_temp = X, y_scaled
+        if y_scaled.ndim == 1:
+            problem_size = self.size_hidden
+        else:
+            problem_size = self.size_hidden * y_scaled.shape[1]
+        ub_sigma = [np.mean(np.max(X, axis=0)), ] * self.size_hidden
+        lb_sigma = [0.01, ] * self.size_hidden
+        if type(lb) in (list, tuple, np.ndarray) and type(ub) in (list, tuple, np.ndarray):
+            if len(lb) == len(ub):
+                if len(lb) == 1:
+                    lb = np.array(lb_sigma + list(lb) * problem_size, dtype=float)
+                    ub = np.array(ub_sigma + list(ub) * problem_size, dtype=float)
+                elif len(lb) != problem_size:
+                    raise ValueError(f"Invalid lb and ub. Their length should be equal to 1 or problem_size.")
+            else:
+                raise ValueError(f"Invalid lb and ub. They should have the same length.")
+        elif type(lb) in (int, float) and type(ub) in (int, float):
+            lb = lb_sigma + [float(lb), ] * problem_size
+            ub = ub_sigma + [float(ub), ] * problem_size
+        else:
+            raise ValueError(f"Invalid lb and ub. They should be a number of list/tuple/np.ndarray with size equal to problem_size")
+        log_to = "console" if self.verbose else "None"
+        if self.obj_name is None:
+            raise ValueError("obj_name can't be None")
+        else:
+            if self.obj_name in self.SUPPORTED_REG_OBJECTIVES.keys():
+                minmax = self.SUPPORTED_REG_OBJECTIVES[self.obj_name]
+            elif self.obj_name in self.SUPPORTED_CLS_OBJECTIVES.keys():
+                minmax = self.SUPPORTED_CLS_OBJECTIVES[self.obj_name]
+            else:
+                raise ValueError("obj_name is not supported. Please check the library: permetrics to see the supported objective function.")
+        problem = {
+            "obj_func": self.objective_function,
+            "bounds": FloatVar(lb=lb, ub=ub),
+            "minmax": minmax,
+            "log_to": log_to,
+            "save_population": save_population,
+            "obj_weights": self.obj_weights
+        }
+        self.optimizer.solve(problem, seed=self.seed)
+        self.network.update_weights_from_solution(self.optimizer.g_best.solution, X, y_scaled)
+        self.loss_train = self._get_history_loss(optimizer=self.optimizer)
+        return self
```

### Comparing `evorbf-0.1.0/drafts/model/standard_rbf.py` & `evorbf-0.2.0/evorbf/core/standard_rbf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,243 +1,255 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 09:52, 17/08/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-from sklearn.base import ClassifierMixin, RegressorMixin
-from sklearn.preprocessing import OneHotEncoder
-from evorbf.base_rbf_numpy import BaseRbf, RBF
-from evorbf.helpers.encoder import ObjectiveScaler
-
-
-class RbfRegressor(BaseRbf, RegressorMixin):
-    """
-    Defines the RBF model for Regression problems that inherit the BaseRbf and RegressorMixin classes.
-
-    Parameters
-    ----------
-    hidden_size : int, default=10
-        The number of hidden nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-
-    Examples
-    --------
-    >>> from evorbf import RbfRegressor, Data
-    >>> from sklearn.datasets import make_regression
-    >>> X, y = make_regression(n_samples=200, random_state=1)
-    >>> data = Data(X, y)
-    >>> data.split_train_test(test_size=0.2, random_state=1)
-    >>> model = RbfRegressor(hidden_size=10, act_name="elu")
-    >>> model.fit(data.X_train, data.y_train)
-    >>> pred = model.predict(data.X_test)
-    >>> print(pred)
-    """
-
-    def __init__(self, hidden_size=10, act_name="elu"):
-        super().__init__(hidden_size=hidden_size, act_name=act_name)
-
-    def create_network(self, X, y):
-        if type(y) in (list, tuple, np.ndarray):
-            y = np.squeeze(np.asarray(y))
-            if y.ndim == 1:
-                size_output = 1
-            elif y.ndim == 2:
-                size_output = y.shape[1]
-            else:
-                raise TypeError("Invalid y array shape, it should be 1D vector or 2D matrix.")
-        else:
-            raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
-        obj_scaler = ObjectiveScaler(obj_name="self", ohe_scaler=None)
-        network = RBF(size_input=X.shape[1], size_hidden=self.hidden_size, size_output=size_output, act_name=self.act_name)
-        return network, obj_scaler
-
-    def score(self, X, y, method="RMSE"):
-        """Return the metric of the prediction.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
-            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        method : str, default="RMSE"
-            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        result : float
-            The result of selected metric
-        """
-        return self._BaseRbf__score_reg(X, y, method)
-
-    def scores(self, X, y, list_methods=("MSE", "MAE")):
-        """Return the list of metrics of the prediction.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
-            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        list_methods : list, default=("MSE", "MAE")
-            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        return self._BaseRbf__scores_reg(X, y, list_methods)
-
-    def evaluate(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
-        """Return the list of performance metrics of the prediction.
-
-        Parameters
-        ----------
-        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            Predicted values for `X`.
-
-        list_metrics : list, default=("MSE", "MAE")
-            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        return self._BaseRbf__evaluate_reg(y_true, y_pred, list_metrics)
-
-
-class RbfClassifier(BaseRbf, ClassifierMixin):
-    """
-    Defines the general class of Metaheuristic-based RBF model for Classification problems that inherit the BaseRbf and ClassifierMixin classes.
-
-    Parameters
-    ----------
-    hidden_size : int, default=10
-        The number of hidden nodes
-
-    act_name : {"relu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid", "hard_sigmoid",
-        "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink", "soft_shrink", "hard_shrink" }, default='sigmoid'
-        Activation function for the hidden layer.
-
-    Examples
-    --------
-    >>> from evorbf import Data, RbfClassifier
-    >>> from sklearn.datasets import make_classification
-    >>> X, y = make_classification(n_samples=100, random_state=1)
-    >>> data = Data(X, y)
-    >>> data.split_train_test(test_size=0.2, random_state=1)
-    >>> model = RbfClassifier(hidden_size=10, act_name="elu")
-    >>> model.fit(data.X_train, data.y_train)
-    >>> pred = model.predict(data.X_test)
-    >>> print(pred)
-    array([1, 0, 1, 0, 1])
-    """
-
-    CLS_OBJ_LOSSES = ["CEL", "HL", "KLDL", "BSL"]
-
-    def __init__(self, hidden_size=10, act_name="elu"):
-        super().__init__(hidden_size=hidden_size, act_name=act_name)
-        self.return_prob = False
-        self.n_labels = None 
-
-    def create_network(self, X, y):
-        if type(y) in (list, tuple, np.ndarray):
-            y = np.squeeze(np.asarray(y))
-            if y.ndim == 1:
-                self.n_labels = len(np.unique(y))
-            else:
-                raise TypeError("Invalid y array shape, it should be 1D vector containing labels 0, 1, 2,.. and so on.")
-        else:
-            raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
-        ohe_scaler = OneHotEncoder(sparse=False)
-        ohe_scaler.fit(np.reshape(y, (-1, 1)))
-        obj_scaler = ObjectiveScaler(obj_name="softmax", ohe_scaler=ohe_scaler)
-        network = RBF(size_input=X.shape[1], size_hidden=self.hidden_size, size_output=self.n_labels, act_name=self.act_name)
-        return network, obj_scaler
-
-    def score(self, X, y, method="AS"):
-        """
-        Return the metric on the given test data and labels.
-
-        In multi-label classification, this is the subset accuracy which is a harsh metric
-        since you require for each sample that each label set be correctly predicted.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True labels for `X`.
-
-        method : str, default="AS"
-            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        result : float
-            The result of selected metric
-        """
-        return self._BaseRbf__score_cls(X, y, method)
-
-    def scores(self, X, y, list_methods=("AS", "RS")):
-        """
-        Return the list of metrics on the given test data and labels.
-
-        In multi-label classification, this is the subset accuracy which is a harsh metric
-        since you require for each sample that each label set be correctly predicted.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Test samples.
-
-        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True labels for `X`.
-
-        list_methods : list, default=("AS", "RS")
-            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        return self._BaseRbf__scores_cls(X, y, list_methods)
-
-    def evaluate(self, y_true, y_pred, list_metrics=("AS", "RS")):
-        """
-        Return the list of performance metrics on the given test data and labels.
-
-        Parameters
-        ----------
-        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            True values for `X`.
-
-        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
-            Predicted values for `X`.
-
-        list_metrics : list, default=("AS", "RS")
-            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
-
-        Returns
-        -------
-        results : dict
-            The results of the list metrics
-        """
-        return self._BaseRbf__evaluate_cls(y_true, y_pred, list_metrics)
+#!/usr/bin/env python
+# Created by "Thieu" at 18:33, 10/05/2024 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+from sklearn.base import ClassifierMixin, RegressorMixin
+from sklearn.preprocessing import OneHotEncoder
+from evorbf.core.base_rbf import BaseRbf, RBF
+from evorbf.helpers.scaler import ObjectiveScaler
+
+
+class RbfRegressor(BaseRbf, RegressorMixin):
+    """
+    Defines the RBF model for Regression problems that inherit the BaseRbf and RegressorMixin classes.
+
+    Parameters
+    ----------
+    hidden_size : int, default=10
+        The number of hidden nodes
+
+    act_name : {"relu", "leaky_relu", "celu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid",
+        "hard_sigmoid", "log_sigmoid", "silu", "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink",
+        "soft_shrink", "hard_shrink", "softmin", "softmax", "log_softmax" }, default='sigmoid'
+        Activation function for the hidden layer.
+
+    seed: int, default=None
+        Determines random number generation for weights and bias initialization.
+        Pass an int for reproducible results across multiple function calls.
+
+    Examples
+    --------
+    >>> from evorbf import RbfRegressor, Data
+    >>> from sklearn.datasets import make_regression
+    >>> X, y = make_regression(n_samples=200, random_state=1)
+    >>> data = Data(X, y)
+    >>> data.split_train_test(test_size=0.2, random_state=1)
+    >>> model = RbfRegressor(hidden_size=10, act_name="elu")
+    >>> model.fit(data.X_train, data.y_train)
+    >>> pred = model.predict(data.X_test)
+    >>> print(pred)
+    """
+
+    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=2.0, regularization=False, lamda=0.01, seed=None):
+        super().__init__(size_hidden, center_finder, sigmas, regularization, lamda, seed)
+
+    def create_network(self, X, y):
+        if type(y) in (list, tuple, np.ndarray):
+            y = np.squeeze(np.asarray(y))
+            if y.ndim == 1:
+                size_output = 1
+            elif y.ndim == 2:
+                size_output = y.shape[1]
+            else:
+                raise TypeError("Invalid y array shape, it should be 1D vector or 2D matrix.")
+        else:
+            raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
+        obj_scaler = ObjectiveScaler(obj_name="self", ohe_scaler=None)
+        network = RBF(size_hidden=self.size_hidden, center_finder=self.center_finder, sigmas=self.sigmas,
+                      regularization=self.regularization, seed=self.seed)
+        return network, obj_scaler
+
+    def score(self, X, y, method="RMSE"):
+        """Return the metric of the prediction.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
+            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        method : str, default="RMSE"
+            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        result : float
+            The result of selected metric
+        """
+        return self._BaseRbf__score_reg(X, y, method)
+
+    def scores(self, X, y, list_methods=("MSE", "MAE")):
+        """Return the list of metrics of the prediction.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples. For some estimators this may be a precomputed kernel matrix or a list of generic objects instead with shape
+            ``(n_samples, n_samples_fitted)``, where ``n_samples_fitted`` is the number of samples used in the fitting for the estimator.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        list_methods : list, default=("MSE", "MAE")
+            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        return self._BaseRbf__scores_reg(X, y, list_methods)
+
+    def evaluate(self, y_true, y_pred, list_metrics=("MSE", "MAE")):
+        """Return the list of performance metrics of the prediction.
+
+        Parameters
+        ----------
+        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            Predicted values for `X`.
+
+        list_metrics : list, default=("MSE", "MAE")
+            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        return self._BaseRbf__evaluate_reg(y_true, y_pred, list_metrics)
+
+
+class RbfClassifier(BaseRbf, ClassifierMixin):
+    """
+    Defines the general class of Metaheuristic-based RBF model for Classification problems that inherit the BaseRbf and ClassifierMixin classes.
+
+    Parameters
+    ----------
+    hidden_size : int, default=10
+        The number of hidden nodes
+
+    act_name : {"relu", "leaky_relu", "celu", "prelu", "gelu", "elu", "selu", "rrelu", "tanh", "hard_tanh", "sigmoid",
+        "hard_sigmoid", "log_sigmoid", "silu", "swish", "hard_swish", "soft_plus", "mish", "soft_sign", "tanh_shrink",
+        "soft_shrink", "hard_shrink", "softmin", "softmax", "log_softmax" }, default='sigmoid'
+        Activation function for the hidden layer.
+
+    seed: int, default=None
+        Determines random number generation for weights and bias initialization.
+        Pass an int for reproducible results across multiple function calls.
+
+    Examples
+    --------
+    >>> from evorbf import Data, RbfClassifier
+    >>> from sklearn.datasets import make_classification
+    >>> X, y = make_classification(n_samples=100, random_state=1)
+    >>> data = Data(X, y)
+    >>> data.split_train_test(test_size=0.2, random_state=1)
+    >>> model = RbfClassifier(hidden_size=10, act_name="elu")
+    >>> model.fit(data.X_train, data.y_train)
+    >>> pred = model.predict(data.X_test)
+    >>> print(pred)
+    array([1, 0, 1, 0, 1])
+    """
+
+    CLS_OBJ_LOSSES = ["CEL", "HL", "KLDL", "BSL"]
+
+    def __init__(self, size_hidden=10, center_finder="kmean", sigmas=2.0, regularization=False, lamda=0.01, seed=None):
+        super().__init__(size_hidden, center_finder, sigmas, regularization, lamda, seed)
+        self.return_prob = False
+        self.n_labels = None
+
+    def create_network(self, X, y):
+        if type(y) in (list, tuple, np.ndarray):
+            y = np.squeeze(np.asarray(y))
+            if y.ndim == 1:
+                self.n_labels = len(np.unique(y))
+            else:
+                raise TypeError("Invalid y array shape, it should be 1D vector containing labels 0, 1, 2,.. and so on.")
+        else:
+            raise TypeError("Invalid y array type, it should be list, tuple or np.ndarray")
+        ohe_scaler = OneHotEncoder(sparse_output=False)
+        ohe_scaler.fit(np.reshape(y, (-1, 1)))
+        obj_scaler = ObjectiveScaler(obj_name="softmax", ohe_scaler=ohe_scaler)
+        network = RBF(size_hidden=self.size_hidden, center_finder=self.center_finder, sigmas=self.sigmas,
+                      regularization=self.regularization, seed=self.seed)
+        return network, obj_scaler
+
+    def score(self, X, y, method="AS"):
+        """
+        Return the metric on the given test data and labels.
+
+        In multi-label classification, this is the subset accuracy which is a harsh metric
+        since you require for each sample that each label set be correctly predicted.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True labels for `X`.
+
+        method : str, default="AS"
+            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        result : float
+            The result of selected metric
+        """
+        return self._BaseRbf__score_cls(X, y, method)
+
+    def scores(self, X, y, list_methods=("AS", "RS")):
+        """
+        Return the list of metrics on the given test data and labels.
+
+        In multi-label classification, this is the subset accuracy which is a harsh metric
+        since you require for each sample that each label set be correctly predicted.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True labels for `X`.
+
+        list_methods : list, default=("AS", "RS")
+            You can get all of the metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        return self._BaseRbf__scores_cls(X, y, list_methods)
+
+    def evaluate(self, y_true, y_pred, list_metrics=("AS", "RS")):
+        """
+        Return the list of performance metrics on the given test data and labels.
+
+        Parameters
+        ----------
+        y_true : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True values for `X`.
+
+        y_pred : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            Predicted values for `X`.
+
+        list_metrics : list, default=("AS", "RS")
+            You can get metrics from Permetrics library: https://github.com/thieu1995/permetrics
+
+        Returns
+        -------
+        results : dict
+            The results of the list metrics
+        """
+        return self._BaseRbf__evaluate_cls(y_true, y_pred, list_metrics)
```

### Comparing `evorbf-0.1.0/drafts/test_MhaElmClassifier.py` & `evorbf-0.2.0/tests/test_InaRbfClassifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 15:45, 15/08/2023 ----------%
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-from evorbf import MhaRbfClassifier
-
-np.random.seed(41)
-
-
-def test_MhaElmClassifier_class():
-    X = np.random.rand(100, 6)
-    y = np.random.randint(0, 2, size=100)
-
-    opt_paras = {"name": "GA", "epoch": 10, "pop_size": 30}
-    model = MhaRbfClassifier(hidden_size=10, act_name="elu", obj_name="AS", optimizer="BaseGA", optimizer_paras=opt_paras, verbose=False)
-    model.fit(X, y)
-    pred = model.predict(X)
-    assert MhaRbfClassifier.SUPPORTED_CLS_OBJECTIVES == model.SUPPORTED_CLS_OBJECTIVES
-    assert pred[0] in (0, 1)
+#!/usr/bin/env python
+# Created by "Thieu" at 17:13, 10/05/2024 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+
+from evorbf import InaRbfClassifier
+
+
+def test_InaRbfClassifier_class():
+    X = np.random.rand(100, 6)
+    y = np.random.randint(0, 2, size=100)
+
+    opt_paras = {"name": "GA", "epoch": 10, "pop_size": 30}
+    model = InaRbfClassifier(size_hidden=25, center_finder="kmean", regularization=False, lamda=0.5, obj_name="NPV",
+                             optimizer="OriginalWOA", optimizer_paras=opt_paras, verbose=True, seed=42)
+    model.fit(X, y)
+    pred = model.predict(X)
+    assert InaRbfClassifier.SUPPORTED_CLS_OBJECTIVES == model.SUPPORTED_CLS_OBJECTIVES
+    assert pred[0] in (0, 1)
```

### Comparing `evorbf-0.1.0/evorbf/helpers/metrics.py` & `evorbf-0.2.0/evorbf/helpers/metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 06:52, 10/08/2023 ----------%
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-from sklearn.model_selection import cross_val_score
-from sklearn.model_selection import cross_val_predict
-from sklearn.model_selection import cross_validate
-from sklearn.model_selection import learning_curve
-from sklearn.model_selection import permutation_test_score
-from sklearn.model_selection import validation_curve
-from permetrics.regression import RegressionMetric
-from permetrics.classification import ClassificationMetric
-
-
-def get_metrics(problem, y_true, y_pred, metrics=None, testcase="test"):
-    if problem == "regression":
-        evaluator = RegressionMetric(y_true, y_pred)
-        paras = [{"decimal": 4}, ] * len(metrics)
-    else:
-        evaluator = ClassificationMetric(y_true, y_pred)
-        paras = [{"average": "weighted"}, ] * len(metrics)
-    if type(metrics) is dict:
-        result = evaluator.get_metrics_by_dict(metrics)
-    elif type(metrics) in (tuple, list):
-        result = evaluator.get_metrics_by_list_names(metrics, paras)
-    else:
-        raise ValueError("metrics parameter should be a list or dict")
-    final_result = {}
-    for key, value in result.items():
-        if testcase is None or testcase == "":
-            final_result[f"{key}"] = value
-        else:
-            final_result[f"{key}_{testcase}"] = value
-    return final_result
-
-
-def get_all_regression_metrics():
-    UNUSED_METRICS = ("RE", "RB", "AE", "SE", "SLE")
-    dict_results = {}
-    for key, value in RegressionMetric.SUPPORT.items():
-        if (key not in UNUSED_METRICS) and (value["type"] in ("min", "max")):
-            dict_results[key] = value["type"]
-    return dict_results
-
-
-def get_all_classification_metrics():
-    dict_results = {}
-    for key, value in ClassificationMetric.SUPPORT.items():
-        if value["type"] in ("min", "max"):
-            dict_results[key] = value["type"]
-    return dict_results
+#!/usr/bin/env python
+# Created by "Thieu" at 06:52, 10/08/2023 ----------%
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+from sklearn.model_selection import cross_val_score
+from sklearn.model_selection import cross_val_predict
+from sklearn.model_selection import cross_validate
+from sklearn.model_selection import learning_curve
+from sklearn.model_selection import permutation_test_score
+from sklearn.model_selection import validation_curve
+from permetrics.regression import RegressionMetric
+from permetrics.classification import ClassificationMetric
+
+
+def get_metrics(problem, y_true, y_pred, metrics=None, testcase="test"):
+    if problem == "regression":
+        evaluator = RegressionMetric(y_true, y_pred)
+    else:
+        evaluator = ClassificationMetric(y_true, y_pred)
+    if type(metrics) is dict:
+        result = evaluator.get_metrics_by_dict(metrics)
+    elif type(metrics) in (tuple, list):
+        result = evaluator.get_metrics_by_list_names(metrics)
+    else:
+        raise ValueError("metrics parameter should be a list or dict")
+    final_result = {}
+    for key, value in result.items():
+        if testcase is None or testcase == "":
+            final_result[f"{key}"] = value
+        else:
+            final_result[f"{key}_{testcase}"] = value
+    return final_result
+
+
+def get_all_regression_metrics():
+    UNUSED_METRICS = ("RE", "RB", "AE", "SE", "SLE")
+    dict_results = {}
+    for key, value in RegressionMetric.SUPPORT.items():
+        if (key not in UNUSED_METRICS) and (value["type"] in ("min", "max")):
+            dict_results[key] = value["type"]
+    return dict_results
+
+
+def get_all_classification_metrics():
+    dict_results = {}
+    for key, value in ClassificationMetric.SUPPORT.items():
+        if value["type"] in ("min", "max"):
+            dict_results[key] = value["type"]
+    return dict_results
```

### Comparing `evorbf-0.1.0/evorbf/helpers/preprocessor.py` & `evorbf-0.2.0/evorbf/helpers/preprocessor.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 23:33, 10/08/2023 ----------%
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import pandas as pd
-import numpy as np
-from pathlib import Path
-from evorbf.helpers.scaler import DataTransformer
-from sklearn.model_selection import train_test_split
-
-
-class LabelEncoder:
-    """
-    Encode categorical features as integer labels.
-    """
-
-    def __init__(self):
-        self.unique_labels = None
-        self.label_to_index = {}
-
-    @staticmethod
-    def check_y(y):
-        y = np.squeeze(np.asarray(y))
-        if y.ndim != 1:
-            raise ValueError("y label should have shape like 1-D vector.")
-        return y
-
-    def fit(self, y):
-        """
-        Fit label encoder to a given set of labels.
-
-        Parameters:
-        -----------
-        y : array-like
-            Labels to encode.
-        """
-        y = self.check_y(y)
-        self.unique_labels = np.unique(y)
-        self.label_to_index = {label: i for i, label in enumerate(self.unique_labels)}
-
-    def transform(self, y):
-        """
-        Transform labels to encoded integer labels.
-
-        Parameters:
-        -----------
-        y : array-like (1-D vector)
-            Labels to encode.
-
-        Returns:
-        --------
-        encoded_labels : array-like
-            Encoded integer labels.
-        """
-        y = self.check_y(y)
-        if self.unique_labels is None:
-            raise ValueError("Label encoder has not been fit yet.")
-        return np.array([self.label_to_index[label] for label in y])
-
-    def fit_transform(self, y):
-        """Fit label encoder and return encoded labels.
-
-        Parameters
-        ----------
-        y : array-like of shape (n_samples,)
-            Target values.
-
-        Returns
-        -------
-        y : array-like of shape (n_samples,)
-            Encoded labels.
-        """
-        self.fit(y)
-        return self.transform(y)
-
-    def inverse_transform(self, y):
-        """
-        Transform integer labels to original labels.
-
-        Parameters:
-        -----------
-        y : array-like
-            Encoded integer labels.
-
-        Returns:
-        --------
-        original_labels : array-like
-            Original labels.
-        """
-        y = self.check_y(y)
-        if self.unique_labels is None:
-            raise ValueError("Label encoder has not been fit yet.")
-        return np.array([self.unique_labels[i] if i in self.label_to_index.values() else "unknown" for i in y])
-
-
-class TimeSeriesDifferencer:
-
-    def __init__(self, interval=1):
-        if interval < 1:
-            raise ValueError("Interval for differencing must be at least 1.")
-        self.interval = interval
-
-    def difference(self, X):
-        self.original_data = X.copy()
-        return np.array([X[i] - X[i - self.interval] for i in range(self.interval, len(X))])
-
-    def inverse_difference(self, diff_data):
-        if self.original_data is None:
-            raise ValueError("Original data is required for inversion.")
-        return np.array([diff_data[i - self.interval] + self.original_data[i - self.interval] for i in range(self.interval, len(self.original_data))])
-
-
-class FeatureEngineering:
-    def __init__(self):
-        """
-        Initialize the FeatureEngineering class
-        """
-        # Check if the threshold is a valid number
-        pass
-
-    def create_threshold_binary_features(self, X, threshold):
-        """
-        Perform feature engineering to add binary indicator columns for values below the threshold.
-        Add each new column right after the corresponding original column.
-
-        Args:
-        X (numpy.ndarray): The input 2D matrix of shape (n_samples, n_features).
-        threshold (float): The threshold value for identifying low values.
-
-        Returns:
-        numpy.ndarray: The updated 2D matrix with binary indicator columns.
-        """
-        # Check if X is a NumPy array
-        if not isinstance(X, np.ndarray):
-            raise ValueError("Input X should be a NumPy array.")
-        # Check if the threshold is a valid number
-        if not (isinstance(threshold, int) or isinstance(threshold, float)):
-            raise ValueError("Threshold should be a numeric value.")
-
-        # Create a new matrix to hold the original and new columns
-        X_new = np.zeros((X.shape[0], X.shape[1] * 2))
-        # Iterate over each column in X
-        for idx in range(X.shape[1]):
-            feature_values = X[:, idx]
-            # Create a binary indicator column for values below the threshold
-            indicator_column = (feature_values < threshold).astype(int)
-            # Add the original column and indicator column to the new matrix
-            X_new[:, idx * 2] = feature_values
-            X_new[:, idx * 2 + 1] = indicator_column
-        return X_new
-
-
-class Data:
-    """
-    The structure of our supported Data class
-
-    Parameters
-    ----------
-    X : np.ndarray
-        The features of your data
-
-    y : np.ndarray
-        The labels of your data
-    """
-
-    SUPPORT = {
-        "scaler": list(DataTransformer.SUPPORTED_SCALERS.keys())
-    }
-
-    def __init__(self, X=None, y=None, name="Unknown"):
-        self.X = X
-        self.y = self.check_y(y)
-        self.name = name
-        self.X_train, self.y_train, self.X_test, self.y_test = None, None, None, None
-
-    @staticmethod
-    def check_y(y):
-        if y is None:
-            return y
-        y = np.squeeze(np.asarray(y))
-        if y.ndim == 1:
-            y = np.reshape(y, (-1, 1))
-        return y
-
-    @staticmethod
-    def scale(X, scaling_methods=('standard', ), list_dict_paras=None):
-        X = np.squeeze(np.asarray(X))
-        if X.ndim == 1:
-            X = np.reshape(X, (-1, 1))
-        if X.ndim >= 3:
-            raise TypeError(f"Invalid X data type. It should be array-like with shape (n samples, m features)")
-        scaler = DataTransformer(scaling_methods=scaling_methods, list_dict_paras=list_dict_paras)
-        data = scaler.fit_transform(X)
-        return data, scaler
-
-    @staticmethod
-    def encode_label(y):
-        y = np.squeeze(np.asarray(y))
-        if y.ndim != 1:
-            raise TypeError(f"Invalid y data type. It should be a vector / array-like with shape (n samples,)")
-        scaler = LabelEncoder()
-        data = scaler.fit_transform(y)
-        return data, scaler
-
-    def split_train_test(self, test_size=0.2, train_size=None,
-                         random_state=41, shuffle=True, stratify=None, inplace=True):
-        """
-        The wrapper of the split_train_test function in scikit-learn library.
-        """
-        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.X, self.y, test_size=test_size,
-                        train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
-        if not inplace:
-            return self.X_train, self.X_test, self.y_train, self.y_test
-
-    def set_train_test(self, X_train=None, y_train=None, X_test=None, y_test=None):
-        """
-        Function use to set your own X_train, y_train, X_test, y_test in case you don't want to use our split function
-
-        Parameters
-        ----------
-        X_train : np.ndarray
-        y_train : np.ndarray
-        X_test : np.ndarray
-        y_test : np.ndarray
-        """
-        self.X_train = X_train
-        self.y_train = y_train
-        self.X_test = X_test
-        self.y_test = y_test
-        return self
+#!/usr/bin/env python
+# Created by "Thieu" at 23:33, 10/08/2023 ----------%
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import pandas as pd
+import numpy as np
+from pathlib import Path
+from evorbf.helpers.scaler import DataTransformer
+from sklearn.model_selection import train_test_split
+
+
+class LabelEncoder:
+    """
+    Encode categorical features as integer labels.
+    """
+
+    def __init__(self):
+        self.unique_labels = None
+        self.label_to_index = {}
+
+    @staticmethod
+    def check_y(y):
+        y = np.squeeze(np.asarray(y))
+        if y.ndim != 1:
+            raise ValueError("y label should have shape like 1-D vector.")
+        return y
+
+    def fit(self, y):
+        """
+        Fit label encoder to a given set of labels.
+
+        Parameters:
+        -----------
+        y : array-like
+            Labels to encode.
+        """
+        y = self.check_y(y)
+        self.unique_labels = np.unique(y)
+        self.label_to_index = {label: i for i, label in enumerate(self.unique_labels)}
+
+    def transform(self, y):
+        """
+        Transform labels to encoded integer labels.
+
+        Parameters:
+        -----------
+        y : array-like (1-D vector)
+            Labels to encode.
+
+        Returns:
+        --------
+        encoded_labels : array-like
+            Encoded integer labels.
+        """
+        y = self.check_y(y)
+        if self.unique_labels is None:
+            raise ValueError("Label encoder has not been fit yet.")
+        return np.array([self.label_to_index[label] for label in y])
+
+    def fit_transform(self, y):
+        """Fit label encoder and return encoded labels.
+
+        Parameters
+        ----------
+        y : array-like of shape (n_samples,)
+            Target values.
+
+        Returns
+        -------
+        y : array-like of shape (n_samples,)
+            Encoded labels.
+        """
+        self.fit(y)
+        return self.transform(y)
+
+    def inverse_transform(self, y):
+        """
+        Transform integer labels to original labels.
+
+        Parameters:
+        -----------
+        y : array-like
+            Encoded integer labels.
+
+        Returns:
+        --------
+        original_labels : array-like
+            Original labels.
+        """
+        y = self.check_y(y)
+        if self.unique_labels is None:
+            raise ValueError("Label encoder has not been fit yet.")
+        return np.array([self.unique_labels[i] if i in self.label_to_index.values() else "unknown" for i in y])
+
+
+class TimeSeriesDifferencer:
+
+    def __init__(self, interval=1):
+        if interval < 1:
+            raise ValueError("Interval for differencing must be at least 1.")
+        self.interval = interval
+
+    def difference(self, X):
+        self.original_data = X.copy()
+        return np.array([X[i] - X[i - self.interval] for i in range(self.interval, len(X))])
+
+    def inverse_difference(self, diff_data):
+        if self.original_data is None:
+            raise ValueError("Original data is required for inversion.")
+        return np.array([diff_data[i - self.interval] + self.original_data[i - self.interval] for i in range(self.interval, len(self.original_data))])
+
+
+class FeatureEngineering:
+    def __init__(self):
+        """
+        Initialize the FeatureEngineering class
+        """
+        # Check if the threshold is a valid number
+        pass
+
+    def create_threshold_binary_features(self, X, threshold):
+        """
+        Perform feature engineering to add binary indicator columns for values below the threshold.
+        Add each new column right after the corresponding original column.
+
+        Args:
+        X (numpy.ndarray): The input 2D matrix of shape (n_samples, n_features).
+        threshold (float): The threshold value for identifying low values.
+
+        Returns:
+        numpy.ndarray: The updated 2D matrix with binary indicator columns.
+        """
+        # Check if X is a NumPy array
+        if not isinstance(X, np.ndarray):
+            raise ValueError("Input X should be a NumPy array.")
+        # Check if the threshold is a valid number
+        if not (isinstance(threshold, int) or isinstance(threshold, float)):
+            raise ValueError("Threshold should be a numeric value.")
+
+        # Create a new matrix to hold the original and new columns
+        X_new = np.zeros((X.shape[0], X.shape[1] * 2))
+        # Iterate over each column in X
+        for idx in range(X.shape[1]):
+            feature_values = X[:, idx]
+            # Create a binary indicator column for values below the threshold
+            indicator_column = (feature_values < threshold).astype(int)
+            # Add the original column and indicator column to the new matrix
+            X_new[:, idx * 2] = feature_values
+            X_new[:, idx * 2 + 1] = indicator_column
+        return X_new
+
+
+class Data:
+    """
+    The structure of our supported Data class
+
+    Parameters
+    ----------
+    X : np.ndarray
+        The features of your data
+
+    y : np.ndarray
+        The labels of your data
+    """
+
+    SUPPORT = {
+        "scaler": list(DataTransformer.SUPPORTED_SCALERS.keys())
+    }
+
+    def __init__(self, X=None, y=None, name="Unknown"):
+        self.X = X
+        self.y = self.check_y(y)
+        self.name = name
+        self.X_train, self.y_train, self.X_test, self.y_test = None, None, None, None
+
+    @staticmethod
+    def check_y(y):
+        if y is None:
+            return y
+        y = np.squeeze(np.asarray(y))
+        if y.ndim == 1:
+            y = np.reshape(y, (-1, 1))
+        return y
+
+    @staticmethod
+    def scale(X, scaling_methods=('standard', ), list_dict_paras=None):
+        X = np.squeeze(np.asarray(X))
+        if X.ndim == 1:
+            X = np.reshape(X, (-1, 1))
+        if X.ndim >= 3:
+            raise TypeError(f"Invalid X data type. It should be array-like with shape (n samples, m features)")
+        scaler = DataTransformer(scaling_methods=scaling_methods, list_dict_paras=list_dict_paras)
+        data = scaler.fit_transform(X)
+        return data, scaler
+
+    @staticmethod
+    def encode_label(y):
+        y = np.squeeze(np.asarray(y))
+        if y.ndim != 1:
+            raise TypeError(f"Invalid y data type. It should be a vector / array-like with shape (n samples,)")
+        scaler = LabelEncoder()
+        data = scaler.fit_transform(y)
+        return data, scaler
+
+    def split_train_test(self, test_size=0.2, train_size=None,
+                         random_state=41, shuffle=True, stratify=None, inplace=True):
+        """
+        The wrapper of the split_train_test function in scikit-learn library.
+        """
+        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.X, self.y, test_size=test_size,
+                        train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
+        if not inplace:
+            return self.X_train, self.X_test, self.y_train, self.y_test
+
+    def set_train_test(self, X_train=None, y_train=None, X_test=None, y_test=None):
+        """
+        Function use to set your own X_train, y_train, X_test, y_test in case you don't want to use our split function
+
+        Parameters
+        ----------
+        X_train : np.ndarray
+        y_train : np.ndarray
+        X_test : np.ndarray
+        y_test : np.ndarray
+        """
+        self.X_train = X_train
+        self.y_train = y_train
+        self.X_test = X_test
+        self.y_test = y_test
+        return self
```

### Comparing `evorbf-0.1.0/evorbf/helpers/scaler.py` & `evorbf-0.2.0/evorbf/helpers/scaler.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 12:36, 17/09/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-from scipy.stats import boxcox, yeojohnson
-from scipy.special import inv_boxcox
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
-
-
-class ObjectiveScaler:
-    """
-    For label scaler in classification (binary and multiple classification)
-    """
-    def __init__(self, obj_name="sigmoid", ohe_scaler=None):
-        """
-        ohe_scaler: Need to be an instance of One-Hot-Encoder for softmax scaler (multiple classification problem)
-        """
-        self.obj_name = obj_name
-        self.ohe_scaler = ohe_scaler
-
-    def transform(self, data):
-        if self.obj_name == "sigmoid" or self.obj_name == "self":
-            return data
-        elif self.obj_name == "hinge":
-            data = np.squeeze(np.array(data))
-            data[np.where(data == 0)] = -1
-            return data
-        elif self.obj_name == "softmax":
-            data = self.ohe_scaler.transform(np.reshape(data, (-1, 1)))
-            return data
-
-    def inverse_transform(self, data):
-        if self.obj_name == "sigmoid":
-            data = np.squeeze(np.array(data))
-            data = np.rint(data).astype(int)
-        elif self.obj_name == "hinge":
-            data = np.squeeze(np.array(data))
-            data = np.ceil(data).astype(int)
-            data[np.where(data == -1)] = 0
-        elif self.obj_name == "softmax":
-            data = np.squeeze(np.array(data))
-            data = np.argmax(data, axis=1)
-        return data
-
-
-class Log1pScaler(BaseEstimator, TransformerMixin):
-
-    def fit(self, X, y=None):
-        # LogETransformer doesn't require fitting, so we simply return self.
-        return self
-
-    def transform(self, X):
-        # Apply the natural logarithm to each element of the input data
-        return np.log1p(X)
-
-    def inverse_transform(self, X):
-        # Apply the exponential function to reverse the logarithmic transformation
-        return np.expm1(X)
-
-
-class LogeScaler(BaseEstimator, TransformerMixin):
-
-    def fit(self, X, y=None):
-        # LogETransformer doesn't require fitting, so we simply return self.
-        return self
-
-    def transform(self, X):
-        # Apply the natural logarithm (base e) to each element of the input data
-        return np.log(X)
-
-    def inverse_transform(self, X):
-        # Apply the exponential function to reverse the logarithmic transformation
-        return np.exp(X)
-
-
-class SqrtScaler(BaseEstimator, TransformerMixin):
-
-    def fit(self, X, y=None):
-        # SqrtScaler doesn't require fitting, so we simply return self.
-        return self
-
-    def transform(self, X):
-        # Apply the square root transformation to each element of the input data
-        return np.sqrt(X)
-
-    def inverse_transform(self, X):
-        # Apply the square of each element to reverse the square root transformation
-        return X ** 2
-
-
-class BoxCoxScaler(BaseEstimator, TransformerMixin):
-
-    def __init__(self, lmbda=None):
-        self.lmbda = lmbda
-
-    def fit(self, X, y=None):
-        # Estimate the lambda parameter from the data if not provided
-        if self.lmbda is None:
-            _, self.lmbda = boxcox(X.flatten())
-        return self
-
-    def transform(self, X):
-        # Apply the Box-Cox transformation to the data
-        X_new = boxcox(X.flatten(), lmbda=self.lmbda)
-        return X_new.reshape(X.shape)
-
-    def inverse_transform(self, X):
-        # Inverse transform using the original lambda parameter
-        return inv_boxcox(X, self.lmbda)
-
-
-class YeoJohnsonScaler(BaseEstimator, TransformerMixin):
-
-    def __init__(self, lmbda=None):
-        self.lmbda = lmbda
-
-    def fit(self, X, y=None):
-        # Estimate the lambda parameter from the data if not provided
-        if self.lmbda is None:
-            _, self.lmbda = yeojohnson(X.flatten())
-        return self
-
-    def transform(self, X):
-        # Apply the Yeo-Johnson transformation to the data
-        X_new = boxcox(X.flatten(), lmbda=self.lmbda)
-        return X_new.reshape(X.shape)
-
-    def inverse_transform(self, X):
-        # Inverse transform using the original lambda parameter
-        return inv_boxcox(X, self.lmbda)
-
-
-class SinhArcSinhScaler(BaseEstimator, TransformerMixin):
-    # https://stats.stackexchange.com/questions/43482/transformation-to-increase-kurtosis-and-skewness-of-normal-r-v
-    def __init__(self, epsilon=0.1, delta=1.0):
-        self.epsilon = epsilon
-        self.delta = delta
-
-    def fit(self, X, y=None):
-        return self
-
-    def transform(self, X):
-        return np.sinh(self.delta * np.arcsinh(X) - self.epsilon)
-
-    def inverse_transform(self, X):
-        return np.sinh((np.arcsinh(X) + self.epsilon) / self.delta)
-
-
-class DataTransformer(BaseEstimator, TransformerMixin):
-
-    SUPPORTED_SCALERS = {"standard": StandardScaler, "minmax": MinMaxScaler, "max-abs": MaxAbsScaler,
-                         "log1p": Log1pScaler, "loge": LogeScaler, "sqrt": SqrtScaler,
-                         "sinh-arc-sinh": SinhArcSinhScaler, "robust": RobustScaler,
-                         "box-cox": BoxCoxScaler, "yeo-johnson": YeoJohnsonScaler}
-
-    def __init__(self, scaling_methods=('standard', ), list_dict_paras=None):
-        if type(scaling_methods) is str:
-            if list_dict_paras is None:
-                self.list_dict_paras = [{}]
-            elif type(list_dict_paras) is dict:
-                self.list_dict_paras = [list_dict_paras]
-            else:
-                raise TypeError(f"You use only 1 scaling method, the list_dict_paras should be dict of parameter for that scaler.")
-            self.scaling_methods = [scaling_methods]
-        elif type(scaling_methods) in (tuple, list, np.ndarray):
-            if list_dict_paras is None:
-                self.list_dict_paras = [{}, ]*len(scaling_methods)
-            elif type(list_dict_paras) in (tuple, list, np.ndarray):
-                self.list_dict_paras = list(list_dict_paras)
-            else:
-                raise TypeError(f"Invalid type of list_dict_paras. Supported type are: tuple, list, or np.ndarray of parameter dict")
-            self.scaling_methods = list(scaling_methods)
-        else:
-            raise TypeError(f"Invalid type of scaling_methods. Supported type are: str, tuple, list, or np.ndarray")
-
-        self.scalers = [self._get_scaler(technique, paras) for (technique, paras) in zip(self.scaling_methods, self.list_dict_paras)]
-
-    def _get_scaler(self, technique, paras):
-        if technique in self.SUPPORTED_SCALERS.keys():
-            if type(paras) is not dict:
-                paras = {}
-            return self.SUPPORTED_SCALERS[technique](**paras)
-        else:
-            raise ValueError(f"Invalid scaling technique. Supported techniques are {self.SUPPORTED_SCALERS.keys()}")
-
-    def fit(self, X, y=None):
-        for idx, _ in enumerate(self.scalers):
-            X = self.scalers[idx].fit_transform(X)
-        return self
-
-    def transform(self, X):
-        for scaler in self.scalers:
-            X = scaler.transform(X)
-        return X
-
-    def inverse_transform(self, X):
-        for scaler in reversed(self.scalers):
-            X = scaler.inverse_transform(X)
-        return X
+#!/usr/bin/env python
+# Created by "Thieu" at 12:36, 17/09/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+from scipy.stats import boxcox, yeojohnson
+from scipy.special import inv_boxcox
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
+
+
+class ObjectiveScaler:
+    """
+    For label scaler in classification (binary and multiple classification)
+    """
+    def __init__(self, obj_name="sigmoid", ohe_scaler=None):
+        """
+        ohe_scaler: Need to be an instance of One-Hot-Encoder for softmax scaler (multiple classification problem)
+        """
+        self.obj_name = obj_name
+        self.ohe_scaler = ohe_scaler
+
+    def transform(self, data):
+        if self.obj_name == "sigmoid" or self.obj_name == "self":
+            return data
+        elif self.obj_name == "hinge":
+            data = np.squeeze(np.array(data))
+            data[np.where(data == 0)] = -1
+            return data
+        elif self.obj_name == "softmax":
+            data = self.ohe_scaler.transform(np.reshape(data, (-1, 1)))
+            return data
+
+    def inverse_transform(self, data):
+        if self.obj_name == "sigmoid":
+            data = np.squeeze(np.array(data))
+            data = np.rint(data).astype(int)
+        elif self.obj_name == "hinge":
+            data = np.squeeze(np.array(data))
+            data = np.ceil(data).astype(int)
+            data[np.where(data == -1)] = 0
+        elif self.obj_name == "softmax":
+            data = np.squeeze(np.array(data))
+            data = np.argmax(data, axis=1)
+        return data
+
+
+class Log1pScaler(BaseEstimator, TransformerMixin):
+
+    def fit(self, X, y=None):
+        # LogETransformer doesn't require fitting, so we simply return self.
+        return self
+
+    def transform(self, X):
+        # Apply the natural logarithm to each element of the input data
+        return np.log1p(X)
+
+    def inverse_transform(self, X):
+        # Apply the exponential function to reverse the logarithmic transformation
+        return np.expm1(X)
+
+
+class LogeScaler(BaseEstimator, TransformerMixin):
+
+    def fit(self, X, y=None):
+        # LogETransformer doesn't require fitting, so we simply return self.
+        return self
+
+    def transform(self, X):
+        # Apply the natural logarithm (base e) to each element of the input data
+        return np.log(X)
+
+    def inverse_transform(self, X):
+        # Apply the exponential function to reverse the logarithmic transformation
+        return np.exp(X)
+
+
+class SqrtScaler(BaseEstimator, TransformerMixin):
+
+    def fit(self, X, y=None):
+        # SqrtScaler doesn't require fitting, so we simply return self.
+        return self
+
+    def transform(self, X):
+        # Apply the square root transformation to each element of the input data
+        return np.sqrt(X)
+
+    def inverse_transform(self, X):
+        # Apply the square of each element to reverse the square root transformation
+        return X ** 2
+
+
+class BoxCoxScaler(BaseEstimator, TransformerMixin):
+
+    def __init__(self, lmbda=None):
+        self.lmbda = lmbda
+
+    def fit(self, X, y=None):
+        # Estimate the lambda parameter from the data if not provided
+        if self.lmbda is None:
+            _, self.lmbda = boxcox(X.flatten())
+        return self
+
+    def transform(self, X):
+        # Apply the Box-Cox transformation to the data
+        X_new = boxcox(X.flatten(), lmbda=self.lmbda)
+        return X_new.reshape(X.shape)
+
+    def inverse_transform(self, X):
+        # Inverse transform using the original lambda parameter
+        return inv_boxcox(X, self.lmbda)
+
+
+class YeoJohnsonScaler(BaseEstimator, TransformerMixin):
+
+    def __init__(self, lmbda=None):
+        self.lmbda = lmbda
+
+    def fit(self, X, y=None):
+        # Estimate the lambda parameter from the data if not provided
+        if self.lmbda is None:
+            _, self.lmbda = yeojohnson(X.flatten())
+        return self
+
+    def transform(self, X):
+        # Apply the Yeo-Johnson transformation to the data
+        X_new = boxcox(X.flatten(), lmbda=self.lmbda)
+        return X_new.reshape(X.shape)
+
+    def inverse_transform(self, X):
+        # Inverse transform using the original lambda parameter
+        return inv_boxcox(X, self.lmbda)
+
+
+class SinhArcSinhScaler(BaseEstimator, TransformerMixin):
+    # https://stats.stackexchange.com/questions/43482/transformation-to-increase-kurtosis-and-skewness-of-normal-r-v
+    def __init__(self, epsilon=0.1, delta=1.0):
+        self.epsilon = epsilon
+        self.delta = delta
+
+    def fit(self, X, y=None):
+        return self
+
+    def transform(self, X):
+        return np.sinh(self.delta * np.arcsinh(X) - self.epsilon)
+
+    def inverse_transform(self, X):
+        return np.sinh((np.arcsinh(X) + self.epsilon) / self.delta)
+
+
+class DataTransformer(BaseEstimator, TransformerMixin):
+
+    SUPPORTED_SCALERS = {"standard": StandardScaler, "minmax": MinMaxScaler, "max-abs": MaxAbsScaler,
+                         "log1p": Log1pScaler, "loge": LogeScaler, "sqrt": SqrtScaler,
+                         "sinh-arc-sinh": SinhArcSinhScaler, "robust": RobustScaler,
+                         "box-cox": BoxCoxScaler, "yeo-johnson": YeoJohnsonScaler}
+
+    def __init__(self, scaling_methods=('standard', ), list_dict_paras=None):
+        if type(scaling_methods) is str:
+            if list_dict_paras is None:
+                self.list_dict_paras = [{}]
+            elif type(list_dict_paras) is dict:
+                self.list_dict_paras = [list_dict_paras]
+            else:
+                raise TypeError(f"You use only 1 scaling method, the list_dict_paras should be dict of parameter for that scaler.")
+            self.scaling_methods = [scaling_methods]
+        elif type(scaling_methods) in (tuple, list, np.ndarray):
+            if list_dict_paras is None:
+                self.list_dict_paras = [{}, ]*len(scaling_methods)
+            elif type(list_dict_paras) in (tuple, list, np.ndarray):
+                self.list_dict_paras = list(list_dict_paras)
+            else:
+                raise TypeError(f"Invalid type of list_dict_paras. Supported type are: tuple, list, or np.ndarray of parameter dict")
+            self.scaling_methods = list(scaling_methods)
+        else:
+            raise TypeError(f"Invalid type of scaling_methods. Supported type are: str, tuple, list, or np.ndarray")
+
+        self.scalers = [self._get_scaler(technique, paras) for (technique, paras) in zip(self.scaling_methods, self.list_dict_paras)]
+
+    def _get_scaler(self, technique, paras):
+        if technique in self.SUPPORTED_SCALERS.keys():
+            if type(paras) is not dict:
+                paras = {}
+            return self.SUPPORTED_SCALERS[technique](**paras)
+        else:
+            raise ValueError(f"Invalid scaling technique. Supported techniques are {self.SUPPORTED_SCALERS.keys()}")
+
+    def fit(self, X, y=None):
+        for idx, _ in enumerate(self.scalers):
+            X = self.scalers[idx].fit_transform(X)
+        return self
+
+    def transform(self, X):
+        for scaler in self.scalers:
+            X = scaler.transform(X)
+        return X
+
+    def inverse_transform(self, X):
+        for scaler in reversed(self.scalers):
+            X = scaler.inverse_transform(X)
+        return X
```

### Comparing `evorbf-0.1.0/evorbf/helpers/validator.py` & `evorbf-0.2.0/evorbf/helpers/validator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 21:39, 10/08/2023 ----------%
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import operator
-import numpy as np
-
-
-def is_in_bound(value, bound):
-    ops = None
-    if type(bound) is tuple:
-        ops = operator.lt
-    elif type(bound) is list:
-        ops = operator.le
-    if bound[0] == float("-inf") and bound[1] == float("inf"):
-        return True
-    elif bound[0] == float("-inf") and ops(value, bound[1]):
-        return True
-    elif ops(bound[0], value) and bound[1] == float("inf"):
-        return True
-    elif ops(bound[0], value) and ops(value, bound[1]):
-        return True
-    return False
-
-
-def is_str_in_list(value: str, my_list: list):
-    if type(value) == str and my_list is not None:
-        return True if value in my_list else False
-    return False
-
-
-def check_int(name: str, value: int, bound=None):
-    if type(value) in [int, float]:
-        if bound is None:
-            return int(value)
-        elif is_in_bound(value, bound):
-            return int(value)
-    bound = "" if bound is None else f"and value should be in range: {bound}"
-    raise ValueError(f"'{name}' is an integer {bound}.")
-
-
-def check_float(name: str, value: int, bound=None):
-    if type(value) in [int, float]:
-        if bound is None:
-            return float(value)
-        elif is_in_bound(value, bound):
-            return float(value)
-    bound = "" if bound is None else f"and value should be in range: {bound}"
-    raise ValueError(f"'{name}' is a float {bound}.")
-
-
-def check_str(name: str, value: str, bound=None):
-    if type(value) is str:
-        if bound is None or is_str_in_list(value, bound):
-            return value
-    bound = "" if bound is None else f"and value should be one of this: {bound}"
-    raise ValueError(f"'{name}' is a string {bound}.")
-
-
-def check_bool(name: str, value: bool, bound=(True, False)):
-    if type(value) is bool:
-        if value in bound:
-            return value
-    bound = "" if bound is None else f"and value should be one of this: {bound}"
-    raise ValueError(f"'{name}' is a boolean {bound}.")
-
-
-def check_tuple_int(name: str, values: tuple, bounds=None):
-    if type(values) in [tuple, list] and len(values) > 1:
-        value_flag = [type(item) == int for item in values]
-        if np.all(value_flag):
-            if bounds is not None and len(bounds) == len(values):
-                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
-                if np.all(value_flag):
-                    return values
-            else:
-                return values
-    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
-    raise ValueError(f"'{name}' are integer {bounds}.")
-
-
-def check_tuple_float(name: str, values: tuple, bounds=None):
-    if type(values) in [tuple, list] and len(values) > 1:
-        value_flag = [type(item) in [int, float] for item in values]
-        if np.all(value_flag):
-            if bounds is not None and len(bounds) == len(values):
-                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
-                if np.all(value_flag):
-                    return values
-            else:
-                return values
-    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
-    raise ValueError(f"'{name}' are float {bounds}.")
+#!/usr/bin/env python
+# Created by "Thieu" at 21:39, 10/08/2023 ----------%
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import operator
+import numpy as np
+
+
+def is_in_bound(value, bound):
+    ops = None
+    if type(bound) is tuple:
+        ops = operator.lt
+    elif type(bound) is list:
+        ops = operator.le
+    if bound[0] == float("-inf") and bound[1] == float("inf"):
+        return True
+    elif bound[0] == float("-inf") and ops(value, bound[1]):
+        return True
+    elif ops(bound[0], value) and bound[1] == float("inf"):
+        return True
+    elif ops(bound[0], value) and ops(value, bound[1]):
+        return True
+    return False
+
+
+def is_str_in_list(value: str, my_list: list):
+    if type(value) == str and my_list is not None:
+        return True if value in my_list else False
+    return False
+
+
+def check_int(name: str, value: int, bound=None):
+    if type(value) in [int, float]:
+        if bound is None:
+            return int(value)
+        elif is_in_bound(value, bound):
+            return int(value)
+    bound = "" if bound is None else f"and value should be in range: {bound}"
+    raise ValueError(f"'{name}' is an integer {bound}.")
+
+
+def check_float(name: str, value: int, bound=None):
+    if type(value) in [int, float]:
+        if bound is None:
+            return float(value)
+        elif is_in_bound(value, bound):
+            return float(value)
+    bound = "" if bound is None else f"and value should be in range: {bound}"
+    raise ValueError(f"'{name}' is a float {bound}.")
+
+
+def check_str(name: str, value: str, bound=None):
+    if type(value) is str:
+        if bound is None or is_str_in_list(value, bound):
+            return value
+    bound = "" if bound is None else f"and value should be one of this: {bound}"
+    raise ValueError(f"'{name}' is a string {bound}.")
+
+
+def check_bool(name: str, value: bool, bound=(True, False)):
+    if type(value) is bool:
+        if value in bound:
+            return value
+    bound = "" if bound is None else f"and value should be one of this: {bound}"
+    raise ValueError(f"'{name}' is a boolean {bound}.")
+
+
+def check_tuple_int(name: str, values: tuple, bounds=None):
+    if type(values) in [tuple, list] and len(values) > 1:
+        value_flag = [type(item) == int for item in values]
+        if np.all(value_flag):
+            if bounds is not None and len(bounds) == len(values):
+                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
+                if np.all(value_flag):
+                    return values
+            else:
+                return values
+    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
+    raise ValueError(f"'{name}' are integer {bounds}.")
+
+
+def check_tuple_float(name: str, values: tuple, bounds=None):
+    if type(values) in [tuple, list] and len(values) > 1:
+        value_flag = [type(item) in [int, float] for item in values]
+        if np.all(value_flag):
+            if bounds is not None and len(bounds) == len(values):
+                value_flag = [is_in_bound(item, bound) for item, bound in zip(values, bounds)]
+                if np.all(value_flag):
+                    return values
+            else:
+                return values
+    bounds = "" if bounds is None else f"and values should be in range: {bounds}"
+    raise ValueError(f"'{name}' are float {bounds}.")
```

### Comparing `evorbf-0.1.0/setup.py` & `evorbf-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 13:24, 25/05/2022 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
-# --------------------------------------------------%
-
-from setuptools import setup, find_packages
-
-
-def readme():
-    with open('README.md', encoding='utf-8') as f:
-        README = f.read()
-    return README
-
-
-setup(
-    name="evorbf",
-    version="0.1.0",
-    author="Thieu",
-    author_email="nguyenthieu2102@gmail.com",
-    description="EvoRBF: Evolving Radial Basis Function Network by Intelligent Nature-inspired Algorithms",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    keywords=["radial basis function", "machine learning", "artificial intelligence",
-              " deep learning", "neural networks", "single hidden layer network", "metaheuristic-based RBF"
-              "random projection", "kernel methods", "feature extraction", "classification", "regression",
-              "supervised learning", "optimization algorithms", "Kernel RBF", "Cross-validation"
-              "Genetic algorithm (GA)", "Particle swarm optimization (PSO)", "Ant colony optimization (ACO)",
-              "Differential evolution (DE)", "Simulated annealing", "Grey wolf optimizer (GWO)", "Whale Optimization Algorithm (WOA)",
-              "confusion matrix", "recall", "precision", "accuracy", "K-Nearest Neighbors", "random forest",
-              "support vector machine", "scikit-learn models", "estimator", "Robust machine learning",
-              "shallow neural network", "nature-inspired RBF", "RBF network",
-              "Convergence analysis", "Search space exploration", "Local search", "Computational intelligence", "Robust optimization",
-              "Performance analysis", "Intelligent optimization", "Simulations"],
-    url="https://github.com/thieu1995/evorbf",
-    project_urls={
-        'Documentation': 'https://evorbf.readthedocs.io/',
-        'Source Code': 'https://github.com/thieu1995/evorbf',
-        'Bug Tracker': 'https://github.com/thieu1995/evorbf/issues',
-        'Change Log': 'https://github.com/thieu1995/evorbf/blob/master/ChangeLog.md',
-        'Forum': 'https://t.me/+fRVCJGuGJg1mNDg1',
-    },
-    packages=find_packages(exclude=['tests*', 'examples*']),
-    include_package_data=True,
-    license="GPLv3",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Information Technology",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: System :: Benchmark",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Mathematics",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Scientific/Engineering :: Visualization",
-        "Topic :: Scientific/Engineering :: Bio-Informatics",
-        "Topic :: Software Development :: Build Tools",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Utilities",
-    ],
-    install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
-                      "pandas>=1.3.5", "mealpy>=3.0.1", "permetrics>=2.0.0"],
-    extras_require={
-        "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
-    },
-    python_requires='>=3.7',
-)
+#!/usr/bin/env python
+# Created by "Thieu" at 13:24, 25/05/2022 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+
+from setuptools import setup, find_packages
+
+
+def readme():
+    with open('README.md', encoding='utf-8') as f:
+        README = f.read()
+    return README
+
+
+setup(
+    name="evorbf",
+    version="0.2.0",
+    author="Thieu",
+    author_email="nguyenthieu2102@gmail.com",
+    description="EvoRBF: Evolving Radial Basis Function Network by Intelligent Nature-inspired Algorithms",
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    keywords=["radial basis function", "machine learning", "artificial intelligence",
+              " deep learning", "neural networks", "single hidden layer network", "metaheuristic-based RBF"
+              "random projection", "kernel methods", "feature extraction", "classification", "regression",
+              "supervised learning", "optimization algorithms", "Kernel RBF", "Cross-validation"
+              "Genetic algorithm (GA)", "Particle swarm optimization (PSO)", "Ant colony optimization (ACO)",
+              "Differential evolution (DE)", "Simulated annealing", "Grey wolf optimizer (GWO)", "Whale Optimization Algorithm (WOA)",
+              "confusion matrix", "recall", "precision", "accuracy", "K-Nearest Neighbors", "random forest",
+              "support vector machine", "scikit-learn models", "estimator", "Robust machine learning",
+              "shallow neural network", "nature-inspired RBF", "RBF network",
+              "Convergence analysis", "Search space exploration", "Local search", "Computational intelligence", "Robust optimization",
+              "Performance analysis", "Intelligent optimization", "Simulations"],
+    url="https://github.com/thieu1995/evorbf",
+    project_urls={
+        'Documentation': 'https://evorbf.readthedocs.io/',
+        'Source Code': 'https://github.com/thieu1995/evorbf',
+        'Bug Tracker': 'https://github.com/thieu1995/evorbf/issues',
+        'Change Log': 'https://github.com/thieu1995/evorbf/blob/master/ChangeLog.md',
+        'Forum': 'https://t.me/+fRVCJGuGJg1mNDg1',
+    },
+    packages=find_packages(exclude=['tests*', 'examples*']),
+    include_package_data=True,
+    license="GPLv3",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Topic :: System :: Benchmark",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Mathematics",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Visualization",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        "Topic :: Software Development :: Build Tools",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Utilities",
+    ],
+    install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
+                      "pandas>=1.3.5", "mealpy>=3.0.1", "permetrics>=2.0.0"],
+    extras_require={
+        "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
+    },
+    python_requires='>=3.8',
+)
```

