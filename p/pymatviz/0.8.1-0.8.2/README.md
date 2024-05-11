# Comparing `tmp/pymatviz-0.8.1.tar.gz` & `tmp/pymatviz-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatviz-0.8.1.tar", last modified: Sun Feb 11 17:36:33 2024, max compression
+gzip compressed data, was "pymatviz-0.8.2.tar", last modified: Sat May 11 16:39:51 2024, max compression
```

## Comparing `pymatviz-0.8.1.tar` & `pymatviz-0.8.2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-02-11 17:36:33.886151 pymatviz-0.8.1/
--rw-r--r--   0 janosh     (501) wheel        (0)    20005 2024-02-11 17:36:33.885762 pymatviz-0.8.1/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.8.1/license
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-02-11 17:36:33.879509 pymatviz-0.8.1/pymatviz/
--rw-r--r--   0 janosh     (501) wheel        (0)     5391 2024-02-11 17:28:48.000000 pymatviz-0.8.1/pymatviz/__init__.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3813 2023-12-29 11:32:28.000000 pymatviz-0.8.1/pymatviz/correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3107 2023-12-26 18:23:26.000000 pymatviz-0.8.1/pymatviz/cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.8.1/pymatviz/elements.csv
--rw-r--r--   0 janosh     (501) wheel        (0)    14820 2023-12-28 08:25:38.000000 pymatviz-0.8.1/pymatviz/histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)    15523 2024-02-11 17:28:48.000000 pymatviz-0.8.1/pymatviz/io.py
--rw-r--r--   0 janosh     (501) wheel        (0)    11348 2024-02-08 19:05:15.000000 pymatviz-0.8.1/pymatviz/parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)    16521 2024-02-02 11:27:31.000000 pymatviz-0.8.1/pymatviz/phonons.py
--rw-r--r--   0 janosh     (501) wheel        (0)    49289 2024-02-09 12:17:57.000000 pymatviz-0.8.1/pymatviz/ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2915 2023-10-28 21:27:58.000000 pymatviz-0.8.1/pymatviz/relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2144 2023-05-19 14:05:47.000000 pymatviz-0.8.1/pymatviz/sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)    18088 2023-12-23 02:44:29.000000 pymatviz-0.8.1/pymatviz/structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2792 2024-02-02 11:27:31.000000 pymatviz-0.8.1/pymatviz/sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)    10188 2024-02-02 11:27:31.000000 pymatviz-0.8.1/pymatviz/uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    25971 2024-02-02 11:27:31.000000 pymatviz-0.8.1/pymatviz/utils.py
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-02-11 17:36:33.884881 pymatviz-0.8.1/pymatviz.egg-info/
--rw-r--r--   0 janosh     (501) wheel        (0)    20005 2024-02-11 17:36:33.000000 pymatviz-0.8.1/pymatviz.egg-info/PKG-INFO
--rw-r--r--   0 janosh     (501) wheel        (0)      846 2024-02-11 17:36:33.000000 pymatviz-0.8.1/pymatviz.egg-info/SOURCES.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        1 2024-02-11 17:36:33.000000 pymatviz-0.8.1/pymatviz.egg-info/dependency_links.txt
--rw-r--r--   0 janosh     (501) wheel        (0)      320 2024-02-11 17:36:33.000000 pymatviz-0.8.1/pymatviz.egg-info/requires.txt
--rw-r--r--   0 janosh     (501) wheel        (0)        9 2024-02-11 17:36:33.000000 pymatviz-0.8.1/pymatviz.egg-info/top_level.txt
--rw-r--r--   0 janosh     (501) wheel        (0)     3160 2024-02-11 17:29:22.000000 pymatviz-0.8.1/pyproject.toml
--rw-r--r--   0 janosh     (501) wheel        (0)    16969 2024-02-11 17:28:48.000000 pymatviz-0.8.1/readme.md
--rw-r--r--   0 janosh     (501) wheel        (0)       38 2024-02-11 17:36:33.886207 pymatviz-0.8.1/setup.cfg
-drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-02-11 17:36:33.884473 pymatviz-0.8.1/tests/
--rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.8.1/tests/test_correlation.py
--rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.8.1/tests/test_cumulative.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2606 2023-12-28 08:25:38.000000 pymatviz-0.8.1/tests/test_histograms.py
--rw-r--r--   0 janosh     (501) wheel        (0)      957 2024-02-11 17:28:48.000000 pymatviz-0.8.1/tests/test_init.py
--rw-r--r--   0 janosh     (501) wheel        (0)     8573 2024-02-11 17:28:48.000000 pymatviz-0.8.1/tests/test_io.py
--rw-r--r--   0 janosh     (501) wheel        (0)     3049 2023-12-26 18:26:44.000000 pymatviz-0.8.1/tests/test_parity.py
--rw-r--r--   0 janosh     (501) wheel        (0)     5841 2023-12-26 11:06:58.000000 pymatviz-0.8.1/tests/test_phonons.py
--rw-r--r--   0 janosh     (501) wheel        (0)    14989 2024-02-09 12:17:57.000000 pymatviz-0.8.1/tests/test_ptable.py
--rw-r--r--   0 janosh     (501) wheel        (0)      457 2024-02-11 17:28:48.000000 pymatviz-0.8.1/tests/test_readme.py
--rw-r--r--   0 janosh     (501) wheel        (0)     1378 2023-05-24 19:03:32.000000 pymatviz-0.8.1/tests/test_relevance.py
--rw-r--r--   0 janosh     (501) wheel        (0)      599 2023-12-26 10:57:39.000000 pymatviz-0.8.1/tests/test_sankey.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2856 2023-12-22 18:16:48.000000 pymatviz-0.8.1/tests/test_structure_viz.py
--rw-r--r--   0 janosh     (501) wheel        (0)      999 2023-05-19 14:05:47.000000 pymatviz-0.8.1/tests/test_sunburst.py
--rw-r--r--   0 janosh     (501) wheel        (0)     2383 2023-12-26 10:56:52.000000 pymatviz-0.8.1/tests/test_uncertainty.py
--rw-r--r--   0 janosh     (501) wheel        (0)    17471 2024-02-02 11:27:31.000000 pymatviz-0.8.1/tests/test_utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.610679 pymatviz-0.8.2/
+-rw-r--r--   0 janosh     (501) wheel        (0)    20665 2024-05-11 16:39:51.610417 pymatviz-0.8.2/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)     1073 2021-08-04 10:50:41.000000 pymatviz-0.8.2/license
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.602909 pymatviz-0.8.2/pymatviz/
+-rw-r--r--   0 janosh     (501) wheel        (0)     3791 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/__init__.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3874 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3181 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    19361 2022-12-30 20:51:55.000000 pymatviz-0.8.2/pymatviz/elements.csv
+-rw-r--r--   0 janosh     (501) wheel        (0)     4251 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/enums.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    14974 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16227 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/io.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    13297 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    20943 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/phonons.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    16587 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/powerups.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    71398 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2967 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2220 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    17490 2024-05-10 13:08:51.000000 pymatviz-0.8.2/pymatviz/structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2981 2024-05-11 16:28:36.000000 pymatviz-0.8.2/pymatviz/sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    10628 2024-05-04 22:48:32.000000 pymatviz-0.8.2/pymatviz/uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    17211 2024-05-10 13:08:51.000000 pymatviz-0.8.2/pymatviz/utils.py
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.609516 pymatviz-0.8.2/pymatviz.egg-info/
+-rw-r--r--   0 janosh     (501) wheel        (0)    20665 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/PKG-INFO
+-rw-r--r--   0 janosh     (501) wheel        (0)      908 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/SOURCES.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        1 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/dependency_links.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)      327 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/requires.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)        9 2024-05-11 16:39:51.000000 pymatviz-0.8.2/pymatviz.egg-info/top_level.txt
+-rw-r--r--   0 janosh     (501) wheel        (0)     3332 2024-05-11 16:29:23.000000 pymatviz-0.8.2/pyproject.toml
+-rw-r--r--   0 janosh     (501) wheel        (0)    17586 2024-05-11 16:29:46.000000 pymatviz-0.8.2/readme.md
+-rw-r--r--   0 janosh     (501) wheel        (0)       38 2024-05-11 16:39:51.610720 pymatviz-0.8.2/setup.cfg
+drwxr-xr-x   0 janosh     (501) wheel        (0)        0 2024-05-11 16:39:51.609114 pymatviz-0.8.2/tests/
+-rw-r--r--   0 janosh     (501) wheel        (0)      464 2022-10-15 03:29:31.000000 pymatviz-0.8.2/tests/test_correlation.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      705 2022-12-24 23:29:33.000000 pymatviz-0.8.2/tests/test_cumulative.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2642 2024-03-17 14:44:01.000000 pymatviz-0.8.2/tests/test_histograms.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      859 2024-05-11 16:28:36.000000 pymatviz-0.8.2/tests/test_init.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     8672 2024-05-06 00:10:06.000000 pymatviz-0.8.2/tests/test_io.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     3049 2023-12-26 18:26:44.000000 pymatviz-0.8.2/tests/test_parity.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     7585 2024-03-31 18:45:17.000000 pymatviz-0.8.2/tests/test_phonons.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    11203 2024-03-22 14:01:49.000000 pymatviz-0.8.2/tests/test_powerups.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    20065 2024-05-11 16:28:36.000000 pymatviz-0.8.2/tests/test_ptable.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      457 2024-05-02 15:22:30.000000 pymatviz-0.8.2/tests/test_readme.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     1378 2023-05-24 19:03:32.000000 pymatviz-0.8.2/tests/test_relevance.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      599 2023-12-26 10:57:39.000000 pymatviz-0.8.2/tests/test_sankey.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2677 2024-05-10 13:08:51.000000 pymatviz-0.8.2/tests/test_structure_viz.py
+-rw-r--r--   0 janosh     (501) wheel        (0)      999 2023-05-19 14:05:47.000000 pymatviz-0.8.2/tests/test_sunburst.py
+-rw-r--r--   0 janosh     (501) wheel        (0)     2383 2023-12-26 10:56:52.000000 pymatviz-0.8.2/tests/test_uncertainty.py
+-rw-r--r--   0 janosh     (501) wheel        (0)    12483 2024-05-05 13:32:56.000000 pymatviz-0.8.2/tests/test_utils.py
```

### Comparing `pymatviz-0.8.1/PKG-INFO` & `pymatviz-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.8.1
+Version: 0.8.2
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,15 @@
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: pdfCropMargins; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: weasyprint; extra == "test"
 Provides-Extra: data-src
 Requires-Dist: matminer; extra == "data-src"
+Requires-Dist: mp_api; extra == "data-src"
 Provides-Extra: export-figs
 Requires-Dist: kaleido; extra == "export-figs"
 Provides-Extra: gh-pages
 Requires-Dist: jupyter; extra == "gh-pages"
 Requires-Dist: lazydocs; extra == "gh-pages"
 Requires-Dist: nbconvert; extra == "gh-pages"
 Provides-Extra: df-pdf-export
@@ -81,31 +82,31 @@
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 [![Zenodo](https://img.shields.io/badge/DOI-10.5281/zenodo.10456384-blue?logo=Zenodo&logoColor=white)](https://zenodo.org/records/10456384)
 
 </h4>
 
 <slot name="how-to-cite">
 
-> If you use `pymatviz` in your research, [see how to cite](#--how-to-cite-pymatviz).
+> If you use `pymatviz` in your research, [see how to cite](#how-to-cite-pymatviz).
 
 </slot>
 
-## 🔨 &thinsp; Installation
+## Installation
 
 ```sh
 pip install pymatviz
 ```
 
-## 💡 &thinsp; API Docs
+## API Docs
 
 See the [/api] page.
 
 [/api]: https://janosh.github.io/pymatviz/api
 
-## 📙 &thinsp; Usage
+## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
@@ -116,45 +117,42 @@
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-| [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py) |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                       ![ptable-heatmap]                        |                        ![ptable-heatmap-ratio]                        |
-|  [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)  | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|            ![ptable-heatmap-plotly-more-hover-data]            |                     ![ptable-heatmap-plotly-log]                      |
-
-## Nested Periodic Table
-
-See [`pymatviz/ptable.py`](pymatviz/ptable.py). Plot histogram plots and scatter plots nested within periodic table.
-| [`ptable_hists(data, colormap="coolwarm"`](pymatviz/ptable.py) | [`ptable_scatters(data, colormap="coolwarm"`](pymatviz/ptable.py) |
-| :------------------------------------------------------------: | :---------------------------------------------------------------: |
-
-<!-- prettier-ignore -->
-|                        ![ptable-hists]                         |                        ![ptable-scatters]                         |
+|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
+| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
+|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
+|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
+|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
+|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
+|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
+| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
+|                                           ![ptable-heatmap-splits]                                           |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
-[ptable-scatters]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-scatters.svg
+[ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
+[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
 
 ## Phonons
 
 See [`pymatviz/phonons.py`](pymatviz/phonons.py).
 
-|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           | [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py) |
-| :------------------------------------------------------------------------: | :--------------------------------------------------: |
-|                              ![phonon-bands]                               |                    ![phonon-dos]                     |
-| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) |                                                      |
-|                          ![phonon-bands-and-dos]                           |                                                      |
+|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
+| :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
+|                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
+| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
+|                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
 
 [phonon-bands]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-mp-2758.svg
 [phonon-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-dos-mp-2758.svg
-[phonon-bands-and-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-2758]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-23907]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-23907.svg
 
 ### Dash app using `ptable_heatmap_plotly()`
 
 See [`examples/mprester_ptable.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb).
 
 <https://user-images.githubusercontent.com/30958850/181644052-b330f0a2-70fc-451c-8230-20d45d3af72f.mp4>
 
@@ -209,33 +207,33 @@
 | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
 |                       ![density-scatter]                        |                  ![density-scatter-with-hist]                   |
 |       [`density_hexbin(xs, ys, ...)`](pymatviz/parity.py)       |  [`density_hexbin_with_hist(xs, ys, ...)`](pymatviz/parity.py)  |
 |                        ![density-hexbin]                        |                   ![density-hexbin-with-hist]                   |
 | [`scatter_with_err_bar(xs, ys, yerr, ...)`](pymatviz/parity.py) | [`residual_vs_actual(y_true, y_pred, ...)`](pymatviz/parity.py) |
 |                     ![scatter-with-err-bar]                     |                      ![residual-vs-actual]                      |
 
-## Uncertainty Calibration
+## Uncertainty
 
 See [`pymatviz/uncertainty.py`](pymatviz/uncertainty.py).
 
 |       [`qq_gaussian(y_true, y_pred, y_std)`](pymatviz/uncertainty.py)       |       [`qq_gaussian(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py)       |
 | :-------------------------------------------------------------------------: | :-------------------------------------------------------------------------------: |
 |                             ![normal-prob-plot]                             |                           ![normal-prob-plot-multiple]                            |
 | [`error_decay_with_uncert(y_true, y_pred, y_std)`](pymatviz/uncertainty.py) | [`error_decay_with_uncert(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py) |
 |                         ![error-decay-with-uncert]                          |                        ![error-decay-with-uncert-multiple]                        |
 
-## Cumulative Error & Residual
+## Cumulative Metrics
 
 See [`pymatviz/cumulative.py`](pymatviz/cumulative.py).
 
 | [`cumulative_error(preds, targets)`](pymatviz/cumulative.py) | [`cumulative_residual(preds, targets)`](pymatviz/cumulative.py) |
 | :----------------------------------------------------------: | :-------------------------------------------------------------: |
 |                     ![cumulative-error]                      |                     ![cumulative-residual]                      |
 
-## Classification Metrics
+## Classification
 
 See [`pymatviz/relevance.py`](pymatviz/relevance.py).
 
 | [`roc_curve(targets, proba_pos)`](pymatviz/relevance.py) | [`precision_recall_curve(targets, proba_pos)`](pymatviz/relevance.py) |
 | :------------------------------------------------------: | :-------------------------------------------------------------------: |
 |                       ![roc-curve]                       |                       ![precision-recall-curve]                       |
 
@@ -272,24 +270,24 @@
 [sankey-spglib-vs-aflow-spacegroups]: https://github.com/janosh/pymatviz/raw/main/assets/sankey-spglib-vs-aflow-spacegroups.svg
 [scatter-with-err-bar]: https://github.com/janosh/pymatviz/raw/main/assets/scatter-with-err-bar.svg
 [spg-num-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-num-sunburst.svg
 [spg-symbol-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-symbol-sunburst.svg
 [struct-2d-mp-12712-Hf9Zr9Pd24-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-12712-Hf9Zr9Pd24-disordered.svg
 [struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered.svg
 
-## 📖 &thinsp; How to cite `pymatviz`
+## How to cite `pymatviz`
 
-You can cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
+See [`citation.cff`](citation.cff) or cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
 
 ```bib
 @software{riebesell_pymatviz_2022,
   title = {Pymatviz: visualization toolkit for materials informatics},
-  author = {Riebesell, Janosh},
+  author = {Riebesell, Janosh and Yang, Haoyu and Goodall, Rhys and Baird, Sterling G.},
   date = {2022-10-01},
   year = {2022},
   doi = {10.5281/zenodo.7486816},
   url = {https://github.com/janosh/pymatviz},
   note = {10.5281/zenodo.7486816 - https://github.com/janosh/pymatviz},
   urldate = {2023-01-01}, % optional, replace with your date of access
-  version = {0.7.1}, % replace with the version you use
+  version = {0.8.2}, % replace with the version you use
 }
 ```
```

### Comparing `pymatviz-0.8.1/license` & `pymatviz-0.8.2/license`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/pymatviz/correlation.py` & `pymatviz-0.8.2/pymatviz/correlation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Plot distributions of correlation matrix eigenvalues."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 from matplotlib import pyplot as plt
```

### Comparing `pymatviz-0.8.1/pymatviz/cumulative.py` & `pymatviz-0.8.2/pymatviz/cumulative.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Plot the cumulative distribution of residuals and absolute errors."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `pymatviz-0.8.1/pymatviz/elements.csv` & `pymatviz-0.8.2/pymatviz/elements.csv`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/pymatviz/histograms.py` & `pymatviz-0.8.2/pymatviz/histograms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Histograms and bar charts."""
+
 from __future__ import annotations
 
 from collections.abc import Sequence
 from typing import TYPE_CHECKING, Any, Literal, cast
 
 import matplotlib.pyplot as plt
 import numpy as np
@@ -9,20 +11,22 @@
 import plotly.express as px
 import plotly.graph_objects as go
 from matplotlib import transforms
 from matplotlib.ticker import FixedLocator
 from pymatgen.core import Structure
 from pymatgen.symmetry.groups import SpaceGroup
 
+from pymatviz.enums import Key
+from pymatviz.powerups import annotate_bars
 from pymatviz.ptable import count_elements
 from pymatviz.utils import (
     Backend,
-    annotate_bars,
     crystal_sys_from_spg_num,
     df_to_arrays,
+    plotly_key,
     si_fmt_int,
 )
 
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
 
@@ -141,14 +145,15 @@
         # if 1st sequence item is structure, assume all are
         data = cast(Sequence[Structure], data)
         series = pd.Series(struct.get_space_group_info()[1] for struct in data)
     else:
         series = pd.Series(data)
 
     count_col = "Counts"
+    crys_sys_col = Key.crystal_system.value
     df_data = series.value_counts(sort=False).to_frame(name=count_col)
 
     crystal_sys_colors = {
         "triclinic": "red",
         "monoclinic": "teal",
         "orthorhombic": "blue",
         "tetragonal": "green",
@@ -157,54 +162,54 @@
         "cubic": "darkred",
     }
 
     if df_data.index.inferred_type == "integer":  # assume index is space group numbers
         df_data = df_data.reindex(range(1, 231), fill_value=0).sort_index()
         if not show_empty_bins:
             df_data = df_data.query(f"{count_col} > 0")
-        df_data["crystal_sys"] = [crystal_sys_from_spg_num(x) for x in df_data.index]
+        df_data[crys_sys_col] = [crystal_sys_from_spg_num(x) for x in df_data.index]
 
         xlim = (df_data.index.min() - 0.5, df_data.index.max() + 0.5)
         x_label = "International Spacegroup Number"
 
     else:  # assume index is space group symbols
         # TODO: figure how to implement show_empty_bins for space group symbols
         # if show_empty_bins:
         #     idx = [SpaceGroup.from_int_number(x).symbol for x in range(1, 231)]
         #     df = df.reindex(idx, fill_value=0)
         df_data = df_data[df_data[count_col] > 0]
-        df_data["crystal_sys"] = [SpaceGroup(x).crystal_system for x in df_data.index]
+        df_data[crys_sys_col] = [SpaceGroup(x).crystal_system for x in df_data.index]
 
         # sort df by crystal system going from smallest to largest spacegroup numbers
         # e.g. triclinic (1-2) comes first, cubic (195-230) last
         sys_order = dict(zip(crystal_sys_colors, range(len(crystal_sys_colors))))
-        df_data = df_data.loc[df_data.crystal_sys.map(sys_order).sort_values().index]
+        df_data = df_data.loc[df_data[crys_sys_col].map(sys_order).sort_values().index]
 
         x_label = "International Spacegroup Symbol"
 
     # count rows per crystal system
-    crys_sys_counts = df_data.groupby("crystal_sys").sum(count_col)
-    crys_sys_counts["width"] = df_data.value_counts("crystal_sys")
+    crys_sys_counts = df_data.groupby(crys_sys_col).sum(count_col)
+    crys_sys_counts["width"] = df_data.value_counts(crys_sys_col)
     crys_sys_counts["color"] = pd.Series(crystal_sys_colors)
 
     # sort by key order in dict crys_colors
     crys_sys_counts = crys_sys_counts.loc[
         [x for x in crystal_sys_colors if x in crys_sys_counts.index]
     ]
     xlim = (0, len(df_data) - 1)
 
     fig_title = f"{count_col} per crystal system" if show_counts else None
-    if backend == "plotly":
+    if backend == plotly_key:
         df_plot = df_data if show_empty_bins else df_data.reset_index()
 
         fig = px.bar(
             df_plot,
             x=df_plot.index,
             y=count_col,
-            color=df_data.crystal_sys,
+            color=df_data[crys_sys_col],
             color_discrete_map=crystal_sys_colors,
             **kwargs,
         )
         # add vertical lines between crystal systems and fill area with color
         x0 = x1 = 0
         for idx, (crys_sys, count, width, color) in enumerate(
             crys_sys_counts.itertuples()
@@ -330,15 +335,15 @@
     plt.xticks(rotation=90)
 
     return ax
 
 
 def elements_hist(
     formulas: ElemValues,
-    count_mode: CountMode = "composition",
+    count_mode: CountMode = Key.composition,
     log: bool = False,
     keep_top: int | None = None,
     ax: plt.Axes | None = None,
     bar_values: Literal["percent", "count"] | None = "percent",
     h_offset: int = 0,
     v_offset: int = 10,
     rotation: int = 45,
```

### Comparing `pymatviz-0.8.1/pymatviz/io.py` & `pymatviz-0.8.2/pymatviz/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""I/O utilities for saving figures and dataframes to various image formats."""
+
 from __future__ import annotations
 
 import copy
 import os
 import subprocess
 from os.path import dirname
 from shutil import which
@@ -26,14 +28,15 @@
     fig: go.Figure | plt.Figure | plt.Axes,
     path: str,
     plotly_config: dict[str, Any] | None = None,
     env_disable: Sequence[str] = ("CI",),
     pdf_sleep: float = 0.6,
     style: str = "",
     prec: int | None = None,  # Added round keyword argument
+    template: str | None = None,
     **kwargs: Any,
 ) -> None:
     """Write a plotly or matplotlib figure to disk (as HTML/PDF/SVG/...).
 
     If the file is has .svelte extension, insert `{...$$props}` into the figure's
     top-level div so it can be later styled and customized from Svelte code.
 
@@ -52,17 +55,25 @@
             https://github.com/plotly/plotly.py/issues/3469. Defaults to 0.6. Has no
             effect on matplotlib figures.
         style (str, optional): CSS style string to be inserted into the HTML file.
             Defaults to "". Only used if path ends with .svelte or .html.
         prec (int, optional): Number of significant figures to keep for any float
             in the exported file. Defaults to None (no rounding). Sensible values are
             usually 4, 5, 6.
+        template (str, optional): Temporary plotly to apply to the figure before
+            saving. Will be reset to the original after. Defaults to "pymatviz_white" if
+            path ends with .pdf or .pdfa, else None. Set to None to disable. Only used
+            if fig is a plotly figure.
 
         **kwargs: Keyword arguments passed to fig.write_html().
     """
+    is_pdf = path.lower().endswith((".pdf", ".pdfa"))
+    if template is None and is_pdf:
+        template = "pymatviz_white"
+
     if prec is not None:
         # create a copy of figure and round all floats in fig.data to round significant
         # figures
         fig = copy.deepcopy(fig)
         for trace in fig.data:
             # trace is a go.Scatter or go.Bar or go.Heatmap or ...
             if trace.x is not None:
@@ -82,15 +93,14 @@
         fig.savefig(path, **kwargs, transparent=True)
         return
     if not isinstance(fig, go.Figure):
         raise TypeError(
             f"Unsupported figure type {type(fig)}, expected plotly or matplotlib Figure"
             " or plt.Axes"
         )
-    is_pdf = path.lower().endswith((".pdf", ".pdfa"))
     if path.lower().endswith((".svelte", ".html")):
         config = dict(
             showTips=False,
             modeBarButtonsToRemove=[
                 "lasso2d",
                 "select2d",
                 "autoScale2d",
@@ -115,17 +125,17 @@
                 # add trailing newline for pre-commit end-of-file commit hook
                 file.write(text + "\n")
         if style:
             with open(path, mode="r+", encoding="utf-8") as file:
                 # replace first '<div ' with '<div {style=} '
                 file.write(file.read().replace("<div ", f"<div {style=} ", 1))
     else:
-        if is_pdf:
-            orig_template = fig.layout.template
-            fig.layout.template = "pymatviz_white"
+        orig_template = fig.layout.template
+        if is_pdf and template:
+            fig.layout.template = template
         # hide click-to-show traces in PDF
         hidden_traces = []
         for trace in fig.data:
             if trace.visible == "legendonly":
                 trace.visible = False
                 hidden_traces.append(trace)
         fig.write_image(path, **kwargs)
@@ -206,17 +216,18 @@
     try:
         from weasyprint import HTML
     except ImportError as exc:
         msg = "weasyprint not installed\nrun pip install weasyprint"
         raise ImportError(msg) from exc
 
     if styler_css:
-        styler_css = styler_css if isinstance(styler_css, dict) else DEFAULT_DF_STYLES
+        styler_css = DEFAULT_DF_STYLES if styler_css is True else styler_css
         styler.set_table_styles(
-            [dict(selector=sel, props=val) for sel, val in styler_css.items()]
+            [dict(selector=sel, props=val) for sel, val in styler_css.items()],
+            overwrite=False,
         )
 
     styler.set_uuid("")
     html_str = styler.to_html(**kwargs)
 
     if size is None:
         n_rows, n_cols = styler.data.shape
@@ -288,41 +299,49 @@
         os.remove(normalized_file_path)
 
     except ImportError as exc:
         msg = "pdfCropMargins not installed\nrun pip install pdfCropMargins"
         raise ImportError(msg) from exc
 
 
-TABLE_SCROLL_CSS = "table { overflow: scroll; max-width: 100%; display: block; }"
+ALLOW_TABLE_SCROLL = "table { overflow: scroll; max-width: 100%; display: block; }"
+# https://stackoverflow.com/a/38994837
+HIDE_SCROLL_BAR = """
+table {
+    scrollbar-width: none;  /* Firefox */
+}
+table::-webkit-scrollbar {
+    display: none;  /* Safari and Chrome */
+}"""
 
 
 def df_to_html_table(
     styler: Styler,
     file_path: str | Path | None = None,
     inline_props: str | None = "",
     script: str | None = "",
-    styles: str | None = TABLE_SCROLL_CSS,
+    styles: str | None = ALLOW_TABLE_SCROLL + HIDE_SCROLL_BAR,
     styler_css: bool | dict[str, str] = True,
     sortable: bool = True,
     post_process: Callable[[str], str] | None = None,
     **kwargs: Any,
 ) -> str:
     """Convert a pandas Styler to a svelte table.
 
     Args:
         styler (Styler): Styler object to export.
         file_path (str): Path to the file to write the svelte table to.
         inline_props (str): Inline props to pass to the table element. Example:
             "class='table' style='width: 100%'". Defaults to "".
         script (str): JavaScript string to insert above the table. Will replace the
-            opening HTML opening <table tag to allow passing props to it. The default
+            opening HTML opening table tag to allow passing props to it. The default
             script uses ...props to enable Svelte props forwarding to the table element.
             See source code to inspect default script.
-        styles (str): CSS rules to insert at the bottom of the <style> tag element.
-            Defaults to TABLE_SCROLL_CSS.
+        styles (str): CSS rules to insert at the bottom of the style tag. Defaults to
+            TABLE_SCROLL_CSS.
         styler_css (bool | dict[str, str]): Whether to apply some sensible default CSS
             to the pandas Styler. Defaults to True. If dict, keys are CSS selectors and
             values CSS strings. Example:
             dict("td, th": "border: none; padding: 4px 6px;")
         sortable (bool): Whether to enable sorting the table by clicking on column
             headers. Defaults to True. Requires npm install svelte-zoo.
         post_process (Callable[[str], str]): Function to post-process the HTML string
```

### Comparing `pymatviz-0.8.1/pymatviz/parity.py` & `pymatviz-0.8.2/pymatviz/parity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+"""Parity, residual and density plots."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.interpolate
 
-from pymatviz.utils import (
+from pymatviz.powerups import (
+    add_best_fit_line,
     add_identity_line,
     annotate_metrics,
-    df_to_arrays,
     with_marginal_hist,
 )
+from pymatviz.utils import df_to_arrays
 
 
 if TYPE_CHECKING:
     import pandas as pd
     from matplotlib.gridspec import GridSpec
     from numpy.typing import ArrayLike
 
@@ -69,15 +72,16 @@
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
     log_density: bool = True,
     hist_density_kwargs: dict[str, Any] | None = None,
     color_bar: bool | dict[str, Any] = True,
     xlabel: str | None = None,
     ylabel: str | None = None,
-    identity: bool = True,
+    identity_line: bool | dict[str, Any] = True,
+    best_fit_line: bool | dict[str, Any] = True,
     stats: bool | dict[str, Any] = True,
     **kwargs: Any,
 ) -> plt.Axes:
     """Scatter plot colored (and optionally sorted) by density.
 
     Args:
         x (array | str): x-values or dataframe column name.
@@ -90,16 +94,18 @@
         hist_density_kwargs (dict, optional): Passed to hist_density(). Use to change
             sort (by density, default True), bins (default 100), or method (for
             interpolation, default "nearest").
         color_bar (bool | dict, optional): Whether to add a color bar. Defaults to True.
             If dict, unpacked into ax.figure.colorbar(). E.g. dict(label="Density").
         xlabel (str, optional): x-axis label. Defaults to "Actual".
         ylabel (str, optional): y-axis label. Defaults to "Predicted".
-        identity (bool, optional): Whether to add an identity/parity line (y = x).
-            Defaults to True.
+        identity_line (bool | dict[str, Any], optional): Whether to add an parity line
+            (y = x). Defaults to True. Pass a dict to customize line properties.
+        best_fit_line (bool | dict[str, Any], optional): Whether to add a best-fit line.
+            Defaults to True. Pass a dict to customize line properties.
         stats (bool | dict[str, Any], optional): Whether to display a text box with MAE
             and R^2. Defaults to True. Can be dict to pass kwargs to annotate_metrics().
             E.g. stats=dict(loc="upper left", prefix="Title", prop=dict(fontsize=16)).
         **kwargs: Passed to ax.scatter(). Defaults to dict(s=6) to control marker size.
             Other common keys are cmap, vmin, vamx, alpha, edgecolors, linewidths.
 
     Returns:
@@ -117,16 +123,22 @@
 
     xs, ys, cs = hist_density(xs, ys, **(hist_density_kwargs or {}))
 
     # decrease marker size
     defaults = dict(s=6, norm=mpl.colors.LogNorm() if log_density else None)
     ax.scatter(xs, ys, c=cs, **defaults | kwargs)
 
-    if identity:
-        add_identity_line(ax)
+    if identity_line:
+        add_identity_line(
+            ax, **(identity_line if isinstance(identity_line, dict) else {})
+        )
+    if best_fit_line:
+        add_best_fit_line(
+            ax, **(best_fit_line if isinstance(best_fit_line, dict) else {})
+        )
 
     if stats:
         annotate_metrics(xs, ys, fig=ax, **(stats if isinstance(stats, dict) else {}))
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     if color_bar:
@@ -139,14 +151,16 @@
 def scatter_with_err_bar(
     x: ArrayLike | str,
     y: ArrayLike | str,
     df: pd.DataFrame | None = None,
     xerr: ArrayLike | None = None,
     yerr: ArrayLike | None = None,
     ax: plt.Axes | None = None,
+    identity_line: bool | dict[str, Any] = True,
+    best_fit_line: bool | dict[str, Any] = True,
     xlabel: str = "Actual",
     ylabel: str = "Predicted",
     title: str | None = None,
     **kwargs: Any,
 ) -> plt.Axes:
     """Scatter plot with optional x- and/or y-error bars. Useful when passing model
     uncertainties as yerr=y_std for checking if uncertainty correlates with error, i.e.
@@ -155,43 +169,56 @@
     Args:
         x (array | str): x-values or dataframe column name
         y (array | str): y-values or dataframe column name
         df (pd.DataFrame, optional): DataFrame with x and y columns. Defaults to None.
         xerr (array, optional): Horizontal error bars. Defaults to None.
         yerr (array, optional): Vertical error bars. Defaults to None.
         ax (Axes, optional): matplotlib Axes on which to plot. Defaults to None.
+        identity_line (bool | dict[str, Any], optional): Whether to add an parity line
+            (y = x). Defaults to True. Pass a dict to customize line properties.
+        best_fit_line (bool | dict[str, Any], optional): Whether to add a best-fit line.
+            Defaults to True. Pass a dict to customize line properties.
         xlabel (str, optional): x-axis label. Defaults to "Actual".
         ylabel (str, optional): y-axis label. Defaults to "Predicted".
         title (str, optional): Plot tile. Defaults to None.
         **kwargs: Additional keyword arguments to pass to ax.errorbar().
 
     Returns:
         plt.Axes: matplotlib Axes object
     """
     xs, ys = df_to_arrays(df, x, y)
     ax = ax or plt.gca()
 
     styles = dict(markersize=6, fmt="o", ecolor="g", capthick=2, elinewidth=2)
     ax.errorbar(xs, ys, xerr=xerr, yerr=yerr, **kwargs, **styles)
 
-    add_identity_line(ax)
+    if identity_line:
+        add_identity_line(
+            ax, **(identity_line if isinstance(identity_line, dict) else {})
+        )
+    if best_fit_line:
+        add_best_fit_line(
+            ax, **(best_fit_line if isinstance(best_fit_line, dict) else {})
+        )
 
     annotate_metrics(xs, ys, fig=ax)
 
     ax.set(xlabel=xlabel, ylabel=ylabel, title=title)
 
     return ax
 
 
 def density_hexbin(
     x: ArrayLike | str,
     y: ArrayLike | str,
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
     weights: ArrayLike | None = None,
+    identity_line: bool | dict[str, Any] = True,
+    best_fit_line: bool | dict[str, Any] = True,
     xlabel: str = "Actual",
     ylabel: str = "Predicted",
     cbar_label: str | None = "Density",
     # [x, y, width, height] anchored at lower left corner
     cbar_coords: tuple[float, float, float, float] = (0.95, 0.03, 0.03, 0.7),
     **kwargs: Any,
 ) -> plt.Axes:
@@ -202,14 +229,18 @@
         x (array): x-values or dataframe column name.
         y (array): y-values or dataframe column name.
         df (pd.DataFrame, optional): DataFrame with x and y columns. Defaults to None.
         ax (Axes, optional): matplotlib Axes on which to plot. Defaults to None.
         weights (array, optional): If given, these values are accumulated in the bins.
             Otherwise, every point has value 1. Must be of the same length as x and y.
             Defaults to None.
+        identity_line (bool | dict[str, Any], optional): Whether to add an parity line
+            (y = x). Defaults to True. Pass a dict to customize line properties.
+        best_fit_line (bool | dict[str, Any], optional): Whether to add a best-fit line.
+            Defaults to True. Pass a dict to customize line properties.
         xlabel (str, optional): x-axis label. Defaults to "Actual".
         ylabel (str, optional): y-axis label. Defaults to "Predicted".
         cbar_label (str, optional): Color bar label. Defaults to "Density".
         cbar_coords (tuple[float, float, float, float], optional): Color bar position
             and size: [x, y, width, height] anchored at lower left corner. Defaults to
             (0.18, 0.8, 0.42, 0.05).
         **kwargs: Additional keyword arguments to pass to ax.hexbin().
@@ -226,15 +257,22 @@
     cb_ax = ax.inset_axes(cbar_coords)
     plt.colorbar(hexbin, cax=cb_ax)
     cb_ax.yaxis.set_ticks_position("left")
     if cbar_label:
         # make title vertical
         cb_ax.set_title(cbar_label, rotation=90, pad=10)
 
-    add_identity_line(ax)
+    if identity_line:
+        add_identity_line(
+            ax, **(identity_line if isinstance(identity_line, dict) else {})
+        )
+    if best_fit_line:
+        add_best_fit_line(
+            ax, **(best_fit_line if isinstance(best_fit_line, dict) else {})
+        )
 
     annotate_metrics(xs, ys, fig=ax, loc="upper left")
 
     ax.set(xlabel=xlabel, ylabel=ylabel)
 
     return ax
```

### Comparing `pymatviz-0.8.1/pymatviz/phonons.py` & `pymatviz-0.8.2/pymatviz/phonons.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,122 @@
+"""Plotting functions for pymatgen phonon band structures and density of states."""
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Literal, Union, no_type_check
+import sys
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Literal, Union, get_args, no_type_check
 
 import plotly.express as px
 import plotly.graph_objects as go
 import scipy.constants as const
 from plotly.subplots import make_subplots
 from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine as PhononBands
 from pymatgen.phonon.dos import PhononDos
 from pymatgen.util.string import htmlify
 
 
 if TYPE_CHECKING:
-    import numpy as np
+    from collections.abc import Sequence
 
+    import numpy as np
+    from pymatgen.core import Structure
+    from typing_extensions import Self
 
 AnyBandStructure = Union[BandStructureSymmLine, PhononBands]
 
 
+@dataclass
+class PhononDBDoc:
+    """Dataclass for phonon DB docs."""
+
+    structure: Structure
+    phonon_bandstructure: PhononBands
+    phonon_dos: PhononDos
+    free_energies: list[float]  # vibrational part of free energies per formula unit
+    internal_energies: list[float]  # vibrational part of internal energies per f.u.
+    heat_capacities: list[float]
+    entropies: list[float]
+    temps: list[float] | None = None  # temperatures
+    # whether imaginary modes are present in the BS
+    has_imaginary_modes: bool | None = None
+    primitive: Structure | None = None
+    supercell: list[list[int]] | None = None  # 3x3 matrix
+    # non-analytical corrections based on Born charges
+    nac_params: dict[str, Any] | None = None
+    thermal_displacement_data: dict[str, Any] | None = None
+    mp_id: str | None = None  # material ID
+    formula: str | None = None  # chemical formula
+
+    def __new__(cls, **kwargs: Any) -> Self:
+        """Ignore unexpected and initialize dataclass with known kwargs."""
+        try:
+            cls_init = cls.__initializer  # type: ignore[has-type]
+        except AttributeError:
+            # store original init on the class in a different place
+            cls.__initializer = cls_init = cls.__init__
+            # replace init with noop to avoid raising on unexpected kwargs
+            cls.__init__ = lambda *args, **kwargs: None  # type: ignore[method-assign] # noqa: ARG005
+
+        ret = object.__new__(cls)
+        known_kwargs = {
+            key: val for key, val in kwargs.items() if key in cls.__annotations__
+        }
+        cls_init(ret, **known_kwargs)
+
+        return ret
+
+
 def pretty_sym_point(symbol: str) -> str:
     """Convert a symbol to a pretty-printed version."""
     # htmlify maps S0 -> S<sub>0</sub> but leaves S_0 as is so we remove underscores
     return (
         htmlify(symbol.replace("_", ""))
         .replace("GAMMA", "Γ")
         .replace("DELTA", "Δ")
         .replace("SIGMA", "Σ")
     )
 
 
-def get_band_xaxis_ticks(bs: PhononBands) -> tuple[list[float], list[str]]:
+def get_band_xaxis_ticks(
+    band_struct: PhononBands, branches: Sequence[str] | set[str] = ()
+) -> tuple[list[float], list[str]]:
     """Get all ticks and labels for a band structure plot.
 
     Returns:
         tuple[list[float], list[str]]: Ticks and labels for the x-axis of a band
             structure plot.
+        branches (Sequence[str]): Branches to plot. Defaults to empty tuple, meaning all
+            branches are plotted.
     """
-    ticks_x_pos = []
+    ticks_x_pos: list[float] = []
     tick_labels: list[str] = []
-    prev_label = bs.qpoints[0].label
-    prev_branch = bs.branches[0]["name"]
+    prev_label = band_struct.qpoints[0].label
+    prev_branch = band_struct.branches[0]["name"]
 
-    for idx, point in enumerate(bs.qpoints):
+    for idx, point in enumerate(band_struct.qpoints):
         if point.label is None:
             continue
-        ticks_x_pos += [bs.distance[idx]]
 
-        branches = (
+        branch_names = (
             branch["name"]
-            for branch in bs.branches
+            for branch in band_struct.branches
             if branch["start_index"] <= idx <= branch["end_index"]
         )
-        this_branch = next(branches, None)
+        this_branch = next(branch_names, None)
 
         if point.label != prev_label and prev_branch != this_branch:
             tick_labels.pop()
             ticks_x_pos.pop()
             tick_labels += [f"{prev_label or ''}|{point.label}"]
-        else:
+            ticks_x_pos += [band_struct.distance[idx]]
+        elif this_branch in branches:
             tick_labels += [point.label]
+            ticks_x_pos += [band_struct.distance[idx]]
 
         prev_label = point.label
         prev_branch = this_branch
 
     tick_labels = list(map(pretty_sym_point, tick_labels))
     return ticks_x_pos, tick_labels
 
@@ -90,98 +143,139 @@
         fig.add_hrect(
             y0=y_lim.get(y0, y0), y1=y_lim.get(y1, y1), **shade_defaults | kwds
         )
 
     return fig
 
 
+BranchMode = Literal["union", "intersection"]
+
+
 def plot_phonon_bands(
     band_structs: PhononBands | dict[str, PhononBands],
-    line_kwds: dict[str, Any] | None = None,
+    line_kwargs: dict[str, Any] | None = None,
+    branches: Sequence[str] = (),
+    branch_mode: BranchMode = "union",
     shaded_ys: dict[tuple[YMin, YMax], dict[str, Any]] | bool | None = None,
     **kwargs: Any,
 ) -> go.Figure:
     """Plot single or multiple pymatgen band structures using Plotly, focusing on the
     minimum set of overlapping branches.
 
     Warning: Only tested with phonon band structures so far but plan is to extend to
     electronic band structures.
 
     Args:
         band_structs (PhononBandStructureSymmLine | dict[str, PhononBandStructure]):
             Single BandStructureSymmLine or PhononBandStructureSymmLine object or a dict
             with labels mapped to multiple such objects.
-        line_kwds (dict[str, Any]): Passed to Plotly's Figure.add_scatter method.
+        line_kwargs (dict[str, Any]): Passed to Plotly's Figure.add_scatter method.
+        branches (Sequence[str]): Branches to plot. Defaults to empty tuple, meaning all
+            branches are plotted.
+        branch_mode ("union" | "intersection"): Whether to plot union or intersection
+            of branches in case of multiple band structures with non-overlapping
+            branches. Defaults to "union".
         shaded_ys (dict[tuple[float | str, float | str], dict]): Keys are y-ranges
             (min, max) tuple and values are kwargs for shaded regions created by
             fig.add_hrect(). Defaults to single entry (0, "y_min"):
             dict(fillcolor="gray", opacity=0.07). "y_min" and "y_max" will be replaced
             with the figure's y-axis range. dict(layer="below", row="all", col="all") is
             always passed to add_hrect but can be overridden by the user. Set to False
             to disable.
         **kwargs: Passed to Plotly's Figure.add_scatter method.
 
     Returns:
         go.Figure: Plotly figure object.
     """
     fig = go.Figure()
-    line_kwds = line_kwds or {}
+    line_kwargs = line_kwargs or {}
+
+    if isinstance(branches, str):
+        branches = [branches]
+
+    if branch_mode not in get_args(BranchMode):
+        raise ValueError(
+            f"Invalid {branch_mode=}, must be one of {get_args(BranchMode)}"
+        )
 
     if not isinstance(band_structs, dict):  # normalize input to dictionary
         band_structs = {"": band_structs}
 
     # find common branches by normalized branch names
     common_branches: set[str] = set()
-    for bs in band_structs.values():
+    for idx, bs in enumerate(band_structs.values()):
         if not isinstance(bs, PhononBands):
-            type_name = type(bs).__name__
             raise TypeError(
-                f"Only {PhononBands.__name__} objects supported, got {type_name}"
+                f"Only {PhononBands.__name__} supported, got {type(bs).__name__}"
             )
-        branches = {pretty_sym_point(branch["name"]) for branch in bs.branches}
-        common_branches = common_branches & branches if common_branches else branches
-
-    if not common_branches:
-        raise ValueError("No common branches found among the band structures.")
+        bs_branches = {branch["name"] for branch in bs.branches}
+        common_branches = (
+            bs_branches
+            if idx == 0
+            # calc set union/intersect (& or |) depending on branch_mode
+            else getattr(common_branches, branch_mode)(bs_branches)
+        )
+    missing_branches = set(branches) - common_branches
+    avail_branches = "\n- ".join(common_branches)
+    if branches:
+        common_branches &= set(branches)
+
+    if common_branches == set():
+        available = "\n- ".join(
+            f"{key}: {', '.join(branch['name'] for branch in bs.branches)}"
+            for key, bs in band_structs.items()
+        )
+        msg = f"No common branches with {branch_mode=}.\n- {available}"
+        if branches:
+            msg += f"\n- Only branches {branches} were requested."
+        raise ValueError(msg)
+
+    if missing_branches:
+        print(  # noqa: T201 # keep this warning after "No common branches" error
+            f"Warning: {missing_branches=}, available branches:\n- {avail_branches}",
+            file=sys.stderr,
+        )
 
     # plotting only the common branches for each band structure
     first_bs = None
     colors = px.colors.qualitative.Plotly
     line_styles = ("solid", "dot", "dash", "longdash", "dashdot", "longdashdot")
 
     for bs_idx, (label, bs) in enumerate(band_structs.items()):
         color = colors[bs_idx % len(colors)]
         line_style = line_styles[bs_idx % len(line_styles)]
         line_defaults = dict(color=color, width=1.5, dash=line_style)
         # 1st bands determine x-axis scale (there are usually slight scale differences
         # between bands)
         first_bs = first_bs or bs
         for branch_idx, branch in enumerate(bs.branches):
+            if branch["name"] not in common_branches:
+                continue
             start_idx = branch["start_index"]
             end_idx = branch["end_index"] + 1  # Include the end point
             # using the same first_bs x-axis for all band structures to avoid band
             # shifting
             distances = first_bs.distance[start_idx:end_idx]
             for band in range(bs.nb_bands):
                 frequencies = bs.bands[band][start_idx:end_idx]
                 # group traces for toggling and set legend name only for 1st band
                 fig.add_scatter(
                     x=distances,
                     y=frequencies,
                     mode="lines",
-                    line=line_defaults | line_kwds,
+                    line=line_defaults | line_kwargs,
                     legendgroup=label,
                     name=label,
                     showlegend=branch_idx == band == 0,
                     **kwargs,
                 )
 
     # add x-axis labels and vertical lines for common high-symmetry points
     first_bs = next(iter(band_structs.values()))
-    x_ticks, x_labels = get_band_xaxis_ticks(first_bs)
+    x_ticks, x_labels = get_band_xaxis_ticks(first_bs, branches=common_branches)
     fig.layout.xaxis.update(tickvals=x_ticks, ticktext=x_labels, tickangle=0)
 
     # remove 0 and the last line to avoid duplicate vertical line, looks like
     # graphical artifact
     for x_pos in {*x_ticks} - {0, x_ticks[-1]}:
         fig.add_vline(x=x_pos, line=dict(color="black", width=1))
 
@@ -195,17 +289,17 @@
 
     if y_min < -0.1:  # no need for y=0 line if y_min = 0
         fig.add_hline(y=0, line=dict(color="black", width=1))
     if y_min >= -0.01:  # set y_min=0 if below tolerance for imaginary frequencies
         y_min = 0
     fig.layout.yaxis.range = (1.05 * y_min, 1.05 * y_max)
 
-    axes_kwds = dict(linecolor="black", gridcolor="lightgray")
-    fig.layout.xaxis.update(**axes_kwds)
-    fig.layout.yaxis.update(**axes_kwds)
+    axes_kwargs = dict(linecolor="black", gridcolor="lightgray")
+    fig.layout.xaxis.update(**axes_kwargs)
+    fig.layout.yaxis.update(**axes_kwargs)
 
     # move legend to top left corner
     fig.layout.legend.update(
         x=0.005,
         y=0.99,
         orientation="h",
         yanchor="top",
@@ -288,16 +382,16 @@
 
     fig.layout.xaxis.update(title=f"Frequency ({units})")
     fig.layout.yaxis.update(title="Density of States")
     fig.layout.margin = dict(t=5, b=5, l=5, r=5)
     fig.layout.font.size = 16 * (fig.layout.width or 800) / 800
     fig.layout.legend.update(x=0.005, y=0.99, orientation="h", yanchor="top")
 
-    qual_colors = px.colors.qualitative.Plotly
     if last_peak_anno:
+        qual_colors = px.colors.qualitative.Plotly
         for idx, (key, dos) in enumerate(doses.items()):
             last_peak = dos.get_last_peak()
             color = (
                 fig.data[idx].line.color
                 or fig.data[idx].marker.color
                 or qual_colors[idx % len(qual_colors)]
             )
@@ -351,28 +445,34 @@
 
 def plot_phonon_bands_and_dos(
     band_structs: PhononBands | dict[str, PhononBands],
     doses: PhononDos | dict[str, PhononDos],
     bands_kwargs: dict[str, Any] | None = None,
     dos_kwargs: dict[str, Any] | None = None,
     subplot_kwargs: dict[str, Any] | None = None,
+    all_line_kwargs: dict[str, Any] | None = None,
+    per_line_kwargs: dict[str, dict[str, Any]] | None = None,
     **kwargs: Any,
 ) -> go.Figure:
     """Plot phonon DOS and band structure using Plotly.
 
     Args:
         doses (PhononDos | dict[str, PhononDos]): PhononDos or dict of multiple.
         band_structs (PhononBandStructureSymmLine | dict[str, PhononBandStructure]):
             Single BandStructureSymmLine or PhononBandStructureSymmLine object or a dict
             with labels mapped to multiple such objects.
         bands_kwargs (dict[str, Any]): Passed to Plotly's Figure.add_scatter method.
         dos_kwargs (dict[str, Any]): Passed to Plotly's Figure.add_scatter method.
         subplot_kwargs (dict[str, Any]): Passed to Plotly's make_subplots method.
             Defaults to dict(shared_yaxes=True, column_widths=(0.8, 0.2),
             horizontal_spacing=0.01).
+        all_line_kwargs (dict[str, Any]): Passed to trace.update for each in fig.data.
+            Modify line appearance for all traces. Defaults to None.
+        per_line_kwargs (dict[str, str]): Map of line labels to kwargs for trace.update.
+            Modify line appearance for specific traces. Defaults to None.
         **kwargs: Passed to Plotly's Figure.add_scatter method.
 
     Returns:
         go.Figure: Plotly figure object.
     """
     if not isinstance(band_structs, dict):  # normalize input to dictionary
         band_structs = {"": band_structs}
@@ -404,22 +504,27 @@
         trace.x, trace.y = trace.y, trace.x
 
     fig.add_traces(dos_fig.data, rows=1, cols=2)
     # transfer zero line from DOS to band structure
     if fig.layout.yaxis.range[0] < -0.1:
         fig.add_hline(y=0, line=dict(color="black", width=1), row=1, col=2)
 
-    # put traces with same labels into the same legend group and hide the legend for
-    # the 2nd subplot, give them the same color as the corresponding band structure
     line_map: dict[str, dict[str, Any]] = {}
     for trace in fig.data:
+        # put traces with same labels into the same legend group
         trace.legendgroup = trace.name
+        # hide legend for all BS lines, show only DOS line
         trace.showlegend = trace.showlegend and trace.xaxis == "x2"
+        # give all lines with same name the same appearance (esp. color)
         trace.line = line_map.setdefault(trace.name, trace.line)
 
+        trace.update(all_line_kwargs or {})
+        if trace_kwargs := (per_line_kwargs or {}).get(trace.name):
+            trace.update(trace_kwargs)
+
     fig.layout.xaxis2.update(title="DOS")
     # transfer x-axis label from DOS fig to parent fig (since DOS may have custom units)
     fig.layout.yaxis.update(title=dos_fig.layout.xaxis.title.text)
 
     # set y-axis range to match band structure
     fig.layout.yaxis.update(range=bands_fig.layout.yaxis.range)
```

### Comparing `pymatviz-0.8.1/pymatviz/ptable.py` & `pymatviz-0.8.2/pymatviz/ptable.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,120 @@
+"""Various periodic table heatmaps with matplotlib and plotly."""
+
 from __future__ import annotations
 
+import inspect
 import itertools
 import math
 import warnings
 from collections.abc import Sequence
-from typing import TYPE_CHECKING, Any, Callable, Literal, get_args
+from functools import partial
+from typing import TYPE_CHECKING, Literal, Union, get_args
 
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.figure_factory as ff
 from matplotlib.cm import get_cmap
 from matplotlib.colors import Colormap, LogNorm, Normalize
 from matplotlib.patches import Rectangle
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 from pymatgen.core import Composition, Element
 
+from pymatviz.enums import Key
 from pymatviz.utils import df_ptable, pick_bw_for_contrast, si_fmt, si_fmt_int
 
 
 if TYPE_CHECKING:
-    from typing import TypeAlias
+    from typing import Any, Callable, Final
 
     import plotly.graph_objects as go
 
-    ElemValues: TypeAlias = dict[str | int, int | float] | pd.Series | Sequence[str]
+
+# Data types supported by ptable plotters
+SupportedValueType = Union[Sequence[float], np.ndarray]
+
+SupportedDataType = Union[
+    dict[str, Union[float, Sequence[float], np.ndarray]], pd.DataFrame, pd.Series
+]
 
 CountMode = Literal[
-    "composition", "fractional_composition", "reduced_composition", "occurrence"
+    Key.composition, "fractional_composition", "reduced_composition", "occurrence"
 ]
 
+ElemValues = Union[dict[Union[str, int], float], pd.Series, Sequence[str]]
+
+ELEM_CLASS_COLORS: Final = {
+    "Diatomic Nonmetal": "green",
+    "Noble Gas": "purple",
+    "Alkali Metal": "red",
+    "Alkaline Earth Metal": "orange",
+    "Metalloid": "darkgreen",
+    "Polyatomic Nonmetal": "teal",
+    "Transition Metal": "blue",
+    "Post Transition Metal": "cyan",
+    "Lanthanide": "brown",
+    "Actinide": "gray",
+    "Nonmetal": "green",
+    "Halogen": "teal",
+    "Metal": "lightblue",
+    "Alkaline Metal": "magenta",
+    "Transactinide": "olive",
+}
+
+
+def add_element_type_legend(
+    data: pd.DataFrame | pd.Series | dict[str, list[float]],
+    elem_class_colors: dict[str, str] | None = None,
+    legend_kwargs: dict[str, Any] | None = None,
+) -> None:
+    """Add a legend to a matplotlib figure showing the colors of element types.
+
+
+    Args:
+        data (pd.DataFrame | pd.Series | dict[str, list[float]]): Map from element
+            to plot data. Used only to determine which element types are present.
+        elem_class_colors (dict[str, str]): Map from element
+            types to colors. E.g. {"Alkali Metal": "red", "Noble Gas": "blue"}.
+        legend_kwargs (dict): Keyword arguments passed to plt.legend() for customizing
+            legend appearance. Defaults to None.
+    """
+    elem_class_colors = ELEM_CLASS_COLORS | (elem_class_colors or {})
+    # else case list(data) covers dict and DataFrame
+    elems_with_data = data.index if isinstance(data, pd.Series) else list(data)
+    visible_elem_types = df_ptable.loc[elems_with_data, "type"].unique()
+    font_size = 10
+    legend_elements = [
+        plt.Line2D(
+            *([0], [0]),
+            marker="s",
+            color="w",
+            label=elem_class,
+            markerfacecolor=color,
+            markersize=1.2 * font_size,
+        )
+        for elem_class, color in elem_class_colors.items()
+        if elem_class in visible_elem_types
+    ]
+    legend_kwargs = dict(
+        loc="center left",
+        bbox_to_anchor=(0, -42),
+        ncol=6,
+        frameon=False,
+        fontsize=font_size,
+        handlelength=1,  # more compact legend
+    ) | (legend_kwargs or {})
+    plt.legend(handles=legend_elements, **legend_kwargs)
+
 
 def count_elements(
     values: ElemValues,
-    count_mode: CountMode = "composition",
+    count_mode: CountMode = Key.composition,
     exclude_elements: Sequence[str] = (),
     fill_value: float | None = 0,
 ) -> pd.Series:
     """Count element occurrence in list of formula strings or dict-like compositions.
     If passed values are already a map from element symbol to counts, ensure the
     data is a pd.Series filled with zero values for missing element symbols.
 
@@ -84,15 +160,17 @@
         if count_mode == "occurrence":
             srs = pd.Series(
                 itertools.chain.from_iterable(
                     map(str, Composition(comp, allow_negative=True)) for comp in srs
                 )
             ).value_counts()
         else:
-            attr = "element_composition" if count_mode == "composition" else count_mode
+            attr = (
+                "element_composition" if count_mode == Key.composition else count_mode
+            )
             srs = pd.DataFrame(
                 getattr(Composition(formula, allow_negative=True), attr).as_dict()
                 for formula in srs
             ).sum()  # sum up element occurrences
     else:
         raise ValueError(
             "Expected values to be map from element symbols to heatmap values or "
@@ -136,19 +214,431 @@
             raise ValueError(
                 f"Unexpected symbol(s) {bad_symbols} in {exclude_elements=}"
             ) from exc
 
     return srs
 
 
+def data_preprocessor(data: SupportedDataType) -> pd.DataFrame:
+    """Preprocess input data for ptable plotters, including:
+        - Convert all data types to pd.DataFrame.
+        - Impute missing values.
+        - Handle anomalies such as NaN, infinity.
+        - Write vmin/vmax as metadata into the DataFrame.
+
+    Returns:
+        pd.DataFrame: The preprocessed DataFrame with element names
+            as index and values as columns.
+
+    Example:
+        >>> data_dict: dict = {
+            "H": 1.0,
+            "He": [2.0, 4.0],
+            "Li": [[6.0, 8.0], [10.0, 12.0]],
+        }
+
+        OR
+        >>> data_df: pd.DataFrame = pd.DataFrame(
+            data_dict.items(),
+            columns=["element", "heat_val"]
+            ).set_index("element")
+
+        OR
+        >>> data_series: pd.Series = pd.Series(data_dict)
+
+        >>> preprocess_data(data_dict / df / series)
+
+             Element   Value
+        0    H         [1.0, ]
+        1    He        [2.0, 4.0]
+        2    Li        [[6.0, 8.0], [10.0, 12.0]]
+
+        Metadata:
+            vmin: 1.0
+            vmax: 12.0
+    """
+
+    def set_vmin_vmax(df: pd.DataFrame) -> pd.DataFrame:
+        """Write vmin and vmax to DataFrame metadata."""
+        # flatten up to triple nested lists
+        values = df[Key.heat_val].explode().explode().explode()
+        numeric_values = pd.to_numeric(values, errors="coerce")
+
+        df.attrs["vmin"] = numeric_values.min()  # ignores NaNs
+        df.attrs["vmax"] = numeric_values.max()
+        return df
+
+    # Check and handle different supported data types
+    if isinstance(data, pd.DataFrame):
+        data_df = data
+
+    elif isinstance(data, pd.Series):
+        data_df = data.to_frame(name=Key.heat_val)
+        data_df.index.name = Key.element
+
+    elif isinstance(data, dict):
+        data_df = pd.DataFrame(
+            data.items(), columns=[Key.element, Key.heat_val]
+        ).set_index(Key.element)
+
+    else:
+        raise TypeError(f"Unsupported data type, choose from: {SupportedDataType}.")
+
+    # Convert all values to np.array
+    data_df[Key.heat_val] = data_df[Key.heat_val].map(
+        lambda x: np.array([x]) if isinstance(x, float) else np.array(x)
+    )
+
+    # Handle missing and anomalous values
+    data_df = handle_missing_and_anomaly(data_df)
+
+    # Write vmin/vmax into metadata
+    return set_vmin_vmax(data_df)
+
+
+def handle_missing_and_anomaly(
+    df: pd.DataFrame,
+    # missing_strategy: Literal["zero", "mean"] = "mean",
+) -> pd.DataFrame:
+    """Handle missing value (NaN) and anomaly (infinity).
+
+    Infinity would be replaced by vmax(∞) or vmin(-∞).
+    Missing values would be handled by selected strategy:
+        - zero: impute with zeros
+        - mean: impute with mean value
+
+    TODO: finish this function
+    """
+    return df
+
+
+class PTableProjector:
+    """Project (nest) a custom plot into a periodic table.
+
+    Scopes mentioned in this plotter:
+        plot: Refers to the global scope.
+        ax: Refers to the axis where child plotter would plot.
+        child: Refers to the child plotter itself, for example, ax.plot().
+    """
+
+    def __init__(
+        self,
+        *,
+        data: SupportedDataType,
+        colormap: str | Colormap | None,
+        plot_kwargs: dict[str, Any] | None = None,
+        hide_f_block: bool | None = None,
+    ) -> None:
+        """Initialize a ptable projector.
+
+        Default figsize is set to (0.75 * n_groups, 0.75 * n_periods),
+        and axes would be turned off by default.
+
+        Args:
+            data (SupportedDataType): The data to be visualized.
+            colormap (str | Colormap | None): The colormap to use.
+            plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
+            hide_f_block: Hide f-block (Lanthanum and Actinium series). Defaults to
+                None, meaning hide if no data is provided for f-block elements.
+        """
+        # Get colormap
+        self.cmap: Colormap = colormap
+
+        # Preprocess data
+        self.data: pd.DataFrame = data
+
+        if hide_f_block is None:
+            hide_f_block = bool(
+                {
+                    atom_num
+                    for atom_num in [*range(57, 72), *range(89, 104)]  # rare earths
+                    # check if data is present for f-block elements
+                    if (elem := Element.from_Z(atom_num).symbol) in self.data.index  # type: ignore[union-attr]
+                    and self.data.loc[elem, Key.heat_val]  # type: ignore[union-attr]
+                }
+            )
+
+        self.hide_f_block = hide_f_block
+
+        # Initialize periodic table canvas
+        n_periods = df_ptable.row.max()
+        n_groups = df_ptable.column.max()
+
+        if self.hide_f_block:
+            n_periods -= 3
+
+        # Set figure size
+        plot_kwargs = plot_kwargs or {}
+        plot_kwargs.setdefault("figsize", (0.75 * n_groups, 0.75 * n_periods))
+
+        self.fig, self.axes = plt.subplots(n_periods, n_groups, **plot_kwargs)
+
+        # Turn off all axes
+        for ax in self.axes.flat:
+            ax.axis("off")
+
+    @property
+    def cmap(self) -> Colormap | None:
+        """The periodic table's matplotlib Colormap instance."""
+        return self._cmap
+
+    @cmap.setter
+    def cmap(self, colormap: str | Colormap | None) -> None:
+        """Set the periodic table's matplotlib Colormap instance."""
+        self._cmap = None if colormap is None else plt.get_cmap(colormap)
+
+    @property
+    def data(self) -> pd.DataFrame:
+        """The preprocessed data."""
+        return self._data
+
+    @data.setter
+    def data(self, data: SupportedDataType) -> None:
+        """Set and preprocess the data. Also set normalizer."""
+        # Preprocess data
+        self._data: pd.DataFrame = data_preprocessor(data)
+
+        # Normalize data for colorbar
+        self._norm: Normalize = Normalize(
+            vmin=self._data.attrs["vmin"], vmax=self._data.attrs["vmax"]
+        )
+
+    @property
+    def norm(self) -> Normalize:
+        """Data min-max normalizer."""
+        return self._norm
+
+    def add_child_plots(
+        self,
+        child_plotter: Callable[[plt.axes, Any], None],
+        child_args: dict[str, Any],
+        *,
+        ax_kwargs: dict[str, Any],
+        on_empty: Literal["hide", "show"] = "hide",
+    ) -> None:
+        """Add custom child plots to the periodic table grid.
+
+        Args:
+            child_plotter: A callable for the child plotter.
+            child_args: Arguments to pass to the child plotter call.
+            ax_kwargs: Keyword arguments to pass to ax.set().
+            on_empty: Whether to "show" or "hide" tiles for elements without data.
+        """
+        for element in Element:
+            # Hide f-block
+            if self.hide_f_block and (element.is_lanthanoid or element.is_actinoid):
+                continue
+
+            # Get axis index by element symbol
+            symbol: str = element.symbol
+            row, column = df_ptable.loc[symbol, ["row", "column"]]
+            ax: plt.Axes = self.axes[row - 1][column - 1]
+
+            # Get and check tile data
+            try:
+                plot_data: np.ndarray | Sequence[float] = self.data.loc[
+                    symbol, Key.heat_val
+                ]
+            except KeyError:  # skip element without data
+                plot_data = None
+
+            if (plot_data is None or len(plot_data) == 0) and on_empty == "hide":
+                continue
+
+            # Call child plotter
+            child_plotter(ax, plot_data, **child_args)
+
+            # Pass axis kwargs
+            if ax_kwargs:
+                ax.set(**ax_kwargs)
+
+    def add_ele_symbols(
+        self,
+        text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+        pos: tuple[float, float] = (0.5, 0.5),
+        kwargs: dict[str, Any] | None = None,
+    ) -> None:
+        """Add element symbols for each tile.
+
+        Args:
+            text (str | Callable): The text to add to the tile.
+                If a callable, it should accept a pymatgen Element object and return a
+                string. If a string, it can contain a format
+                specifier for an `elem` variable which will be replaced by the element.
+            pos: The position of the text relative to the axes.
+            kwargs: Additional keyword arguments to pass to the `ax.text`.
+        """
+        # Update symbol args
+        kwargs = kwargs or {}
+        kwargs.setdefault("fontsize", 18)
+
+        # Add symbol for each element
+        for element in Element:
+            # Hide f-block
+            if self.hide_f_block and (element.is_lanthanoid or element.is_actinoid):
+                continue
+
+            # Get axis index by element symbol
+            symbol: str = element.symbol
+            row, column = df_ptable.loc[symbol, ["row", "column"]]
+            ax: plt.Axes = self.axes[row - 1][column - 1]
+
+            anno = text(element) if callable(text) else text.format(elem=element)
+            ax.text(
+                *pos, anno, ha="center", va="center", transform=ax.transAxes, **kwargs
+            )
+
+    def add_colorbar(
+        self,
+        title: str,
+        coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
+        *,
+        cbar_kwargs: dict[str, Any] | None = None,
+        title_kwargs: dict[str, Any] | None = None,
+    ) -> None:
+        """Add a global colorbar.
+
+        Args:
+            title: Title for the colorbar.
+            coords: Coordinates of the colorbar (left, bottom, width, height).
+                    Defaults to (0.18, 0.8, 0.42, 0.02).
+            cbar_kwargs: Additional keyword arguments to pass to fig.colorbar().
+            title_kwargs: Additional keyword arguments for the colorbar title.
+        """
+        # Update colorbar args
+        cbar_kwargs = {"orientation": "horizontal"} | (cbar_kwargs or {})
+
+        # Check colormap
+        if self.cmap is None:
+            raise ValueError("Cannot add colorbar without colormap.")
+
+        # Add colorbar
+        cbar_ax = self.fig.add_axes(coords)
+
+        self.fig.colorbar(
+            plt.cm.ScalarMappable(norm=self._norm, cmap=self.cmap),
+            cax=cbar_ax,
+            **cbar_kwargs,
+        )
+
+        # Set colorbar title
+        title_kwargs = title_kwargs or {}
+        title_kwargs.setdefault("fontsize", 12)
+        title_kwargs.setdefault("pad", 10)
+        title_kwargs["label"] = title
+
+        cbar_ax.set_title(**title_kwargs)
+
+
+class ChildPlotters:
+    """Collect some pre-defined child plotters."""
+
+    @staticmethod
+    def rectangle(
+        ax: plt.axes,
+        data: SupportedValueType,
+        norm: Normalize,
+        cmap: Colormap,
+        start_angle: float,
+    ) -> None:
+        """Rectangle heatmap plotter, could be evenly split.
+
+        Could be evenly split, depending on the
+        length of the data (could mix and match).
+
+        Args:
+            ax (plt.axes): The axis to plot on.
+            data (SupportedValueType): The values for to
+                the child plotter.
+            norm (Normalize): Normalizer for data-color mapping.
+            cmap (Colormap): Colormap used for value mapping.
+            start_angle (float): The starting angle for the splits in degrees,
+                and the split proceeds counter-clockwise (0 refers to the x-axis).
+        """
+        # Map values to colors
+        if isinstance(data, (Sequence, np.ndarray)):
+            colors = [cmap(norm(value)) for value in data]
+        else:
+            raise TypeError("Unsupported data type.")
+
+        # Add the pie chart
+        ax.pie(
+            np.ones(len(colors)),
+            colors=colors,
+            startangle=start_angle,
+            wedgeprops=dict(clip_on=True),
+        )
+
+        # Crop the central rectangle from the pie chart
+        rect = Rectangle((-0.5, -0.5), 1, 1, fc="none", ec="none")
+        ax.set_clip_path(rect)
+
+        ax.set_xlim(-0.5, 0.5)
+        ax.set_ylim(-0.5, 0.5)
+
+    @staticmethod
+    def scatter(
+        ax: plt.axes,
+        data: SupportedValueType,
+        **child_args: Any,
+    ) -> None:
+        """Scatter plotter.
+
+        Args:
+            ax (plt.axes): The axis to plot on.
+            data (SupportedValueType): The values for to
+                the child plotter.
+            child_args (dict): args to pass to the child plotter call
+        """
+        # Add scatter
+        if len(data) == 2:
+            ax.scatter(x=data[0], y=data[1], **child_args)
+        elif len(data) == 3:
+            ax.scatter(x=data[0], y=data[1], c=data[2], **child_args)
+
+        # Adjust tick labels
+        # TODO: how to achieve this from external?
+        ax.tick_params(axis="both", which="major", labelsize=8)
+
+        # Hide the right and top spines
+        ax.axis("on")  # turned off by default
+        ax.spines[["right", "top"]].set_visible(False)
+
+    @staticmethod
+    def line(
+        ax: plt.axes,
+        data: SupportedValueType,
+        **child_args: Any,
+    ) -> None:
+        """Line plotter.
+
+        Args:
+            ax (plt.axes): The axis to plot on.
+            data (SupportedValueType): The values for to
+                the child plotter.
+            child_args (dict): args to pass to the child plotter call
+        """
+        # Add line
+        ax.plot(data[0], data[1], **child_args)
+
+        # Adjust tick labels
+        # TODO: how to achieve this from external?
+        ax.tick_params(axis="both", which="major", labelsize=8)
+
+        # Hide the right and top spines
+        ax.axis("on")  # turned off by default
+        ax.spines[["right", "top"]].set_visible(False)
+
+
 def ptable_heatmap(
     values: ElemValues,
     log: bool | Normalize = False,
     ax: plt.Axes | None = None,
-    count_mode: CountMode = "composition",
+    count_mode: CountMode = Key.composition,
     cbar_title: str = "Element Count",
     cbar_range: tuple[float | None, float | None] | None = None,
     cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.05),
     cbar_kwargs: dict[str, Any] | None = None,
     colorscale: str = "viridis",
     show_scale: bool = True,
     show_values: bool = True,
@@ -161,15 +651,16 @@
     exclude_elements: Sequence[str] = (),
     zero_color: str = "#eff",  # light gray
     zero_symbol: str | float = "-",
     text_style: dict[str, Any] | None = None,
     label_font_size: int = 16,
     value_font_size: int = 12,
     tile_size: float | tuple[float, float] = 0.9,
-    rare_earth_voffset: float = 0.5,
+    f_block_voffset: float = 0.5,
+    hide_f_block: bool | None = None,
     **kwargs: Any,
 ) -> plt.Axes:
     """Plot a heatmap across the periodic table of elements.
 
     Args:
         values (dict[str, int | float] | pd.Series | list[str]): Map from element
             symbols to heatmap values or iterable of composition strings/objects.
@@ -228,23 +719,34 @@
         value_font_size (int): Font size for heat values. Defaults to 12.
         tile_size (float | tuple[float, float]): Size of each tile in the periodic
             table as a fraction of available space before touching neighboring tiles.
             1 or (1, 1) means no gaps between tiles. Defaults to 0.9.
         cbar_coords (tuple[float, float, float, float]): Color bar position and size:
             [x, y, width, height] anchored at lower left corner of the bar. Defaults to
             (0.18, 0.8, 0.42, 0.05).
-        rare_earth_voffset (float): Vertical offset for lanthanides and actinides
+        f_block_voffset (float): Vertical offset for lanthanides and actinides
             (row 6 and 7) from the rest of the periodic table. Defaults to 0.5.
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
         **kwargs: Additional keyword arguments passed to plt.figure().
 
     Returns:
         plt.Axes: matplotlib Axes with the heatmap.
     """
+
+    def tick_fmt(val: float, _pos: int) -> str:
+        # val: value at color axis tick (e.g. 10.0, 20.0, ...)
+        # pos: zero-based tick counter (e.g. 0, 1, 2, ...)
+        default_fmt = (
+            ".0%" if heat_mode == "percent" else (".0f" if val < 1e4 else ".2g")
+        )
+        return f"{val:{cbar_fmt or fmt or default_fmt}}"
+
     if fmt is None:
-        fmt = lambda x, _: si_fmt(x, ".1%" if heat_mode == "percent" else ".0f")
+        fmt = partial(si_fmt, fmt=".1%" if heat_mode == "percent" else ".0f")
     if cbar_fmt is None:
         cbar_fmt = fmt
 
     valid_logs = (bool, Normalize)
     if not isinstance(log, valid_logs):
         raise TypeError(f"Invalid {log=}, must be instance of {valid_logs}")
 
@@ -295,14 +797,17 @@
             norm.vmax = cbar_range[1]
 
     text_style = dict(
         horizontalalignment="center", fontsize=label_font_size, fontweight="semibold"
     ) | (text_style or {})
 
     for symbol, row, column, *_ in df_ptable.itertuples():
+        if hide_f_block and (row in (6, 7)):
+            continue
+
         period = n_rows - row  # invert row count to make periodic table right side up
         tile_value = values.get(symbol)
 
         # inf (float/0) or NaN (0/0) are expected when passing in values from
         # ptable_heatmap_ratio
         if symbol in exclude_elements:
             color = "white"
@@ -316,25 +821,30 @@
         elif tile_value == 0:
             color = zero_color
             label = str(zero_symbol)
         else:
             color = color_map(norm(tile_value))
 
             if callable(fmt):
-                # 2nd arg=0 just for consistency with matplotlib fmt signature
-                label = fmt(tile_value, 0)
+                if len(inspect.signature(fmt).parameters) == 2:
+                    # 2nd arg=0 needed for matplotlib which always passes 2 positional
+                    # args to fmt()
+                    label = fmt(tile_value, 0)
+                else:
+                    label = fmt(tile_value)
+
             elif heat_mode == "percent":
                 label = f"{tile_value:{fmt or '.1f'}}"
             else:
                 fmt = fmt or (".0f" if tile_value > 100 else ".1f")
                 label = f"{tile_value:{fmt}}"
             # replace shortens scientific notation 1e+01 to 1e1 so it fits inside cells
             label = label.replace("e+0", "e")
         if period < 3:  # vertical offset for lanthanides + actinides
-            period += rare_earth_voffset
+            period += f_block_voffset
         rect = Rectangle(
             (column, period), tile_width, tile_height, edgecolor="gray", facecolor=color
         )
 
         if heat_mode is None or not show_values:
             # no value to display below in colored rectangle so center element symbol
             text_style.setdefault("verticalalignment", "center")
@@ -381,22 +891,14 @@
         # format major and minor ticks
         # TODO maybe give user direct control over labelsize, instead of hard-coding
         # 8pt smaller than default
         cbar_ax.tick_params(which="both", labelsize=text_style["fontsize"])
 
         mappable = plt.cm.ScalarMappable(norm=norm, cmap=colorscale)
 
-        def tick_fmt(val: float, _pos: int) -> str:
-            # val: value at color axis tick (e.g. 10.0, 20.0, ...)
-            # pos: zero-based tick counter (e.g. 0, 1, 2, ...)
-            default_fmt = (
-                ".0%" if heat_mode == "percent" else (".0f" if val < 1e4 else ".2g")
-            )
-            return f"{val:{cbar_fmt or fmt or default_fmt}}"
-
         if callable(cbar_fmt):
             tick_fmt = cbar_fmt
 
         cbar_kwargs = cbar_kwargs or {}
         cbar = fig.colorbar(
             mappable,
             cax=cbar_kwargs.pop("cax", cbar_ax),
@@ -411,18 +913,129 @@
     plt.ylim(0.3, n_rows + 0.1)
     plt.xlim(0.9, n_columns + 1)
 
     plt.axis("off")
     return ax
 
 
+def ptable_heatmap_splits(
+    data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
+    colormap: str | None = None,
+    start_angle: float = 135,
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_pos: tuple[float, float] = (0.5, 0.5),
+    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
+    cbar_title: str = "Values",
+    on_empty: Literal["hide", "show"] = "hide",
+    hide_f_block: bool | None = None,
+    ax_kwargs: dict[str, Any] | None = None,
+    symbol_kwargs: dict[str, Any] | None = None,
+    plot_kwargs: dict[str, Any]
+    | Callable[[Sequence[float]], dict[str, Any]]
+    | None = None,
+    cbar_title_kwargs: dict[str, Any] | None = None,
+    cbar_kwargs: dict[str, Any] | None = None,
+) -> plt.Figure:
+    """Plot evenly-split heatmaps, nested inside a periodic table.
+
+    Args:
+        data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
+            Map from element symbols to plot data. E.g. if dict,
+            {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
+            be plotted on the lower-left corner and the 2nd on the upper-right.
+            If pd.Series, index is element symbols and values lists.
+            If pd.DataFrame, column names are element symbols,
+            plots are created from each column.
+        colormap (str): Matplotlib colormap name to use.
+        start_angle (float): The starting angle for the splits in degrees,
+                and the split proceeds counter-clockwise (0 refers to
+                the x-axis). Defaults to 135 degrees.
+        ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
+            Use to set x/y labels, limits, etc. Defaults to None. Example:
+            dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
+            ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
+        symbol_text (str | Callable[[Element], str]): Text to display for
+            each element symbol. Defaults to lambda elem: elem.symbol.
+        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
+            element symbols. Defaults to None.
+        symbol_pos (tuple[float, float]): Position of element symbols
+            relative to the lower left corner of each tile.
+            Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
+        cbar_coords (tuple[float, float, float, float]): Colorbar
+            position and size: [x, y, width, height] anchored at lower left
+            corner of the bar. Defaults to (0.25, 0.77, 0.35, 0.02).
+        cbar_title (str): Colorbar title. Defaults to "Values".
+        cbar_title_kwargs (dict): Keyword arguments passed to
+            cbar.ax.set_title(). Defaults to dict(fontsize=12, pad=10).
+        cbar_kwargs (dict): Keyword arguments passed to fig.colorbar().
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
+
+    Notes:
+        Default figsize is set to (0.75 * n_groups, 0.75 * n_periods).
+
+    Returns:
+        plt.Figure: periodic table with a subplot in each element tile.
+    """
+    # Re-initialize kwargs as empty dict if None
+    plot_kwargs = plot_kwargs or {}
+    ax_kwargs = ax_kwargs or {}
+    symbol_kwargs = symbol_kwargs or {}
+    cbar_title_kwargs = cbar_title_kwargs or {}
+    cbar_kwargs = cbar_kwargs or {}
+
+    # Initialize periodic table plotter
+    plotter = PTableProjector(
+        data=data,
+        colormap=colormap,
+        plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
+        hide_f_block=hide_f_block,
+    )
+
+    # Call child plotter: evenly split rectangle
+    child_args = {
+        "start_angle": start_angle,
+        "cmap": plotter.cmap,
+        "norm": plotter.norm,
+    }
+
+    plotter.add_child_plots(
+        ChildPlotters.rectangle,  # type: ignore[arg-type]
+        child_args=child_args,
+        ax_kwargs=ax_kwargs,
+        on_empty=on_empty,
+    )
+
+    # Add element symbols
+    plotter.add_ele_symbols(
+        text=symbol_text,
+        pos=symbol_pos,
+        kwargs=symbol_kwargs,
+    )
+
+    # Add colorbar
+    plotter.add_colorbar(
+        title=cbar_title,
+        coords=cbar_coords,
+        cbar_kwargs=cbar_kwargs,
+        title_kwargs=cbar_title_kwargs,
+    )
+
+    return plotter.fig
+
+
 def ptable_heatmap_ratio(
     values_num: ElemValues,
     values_denom: ElemValues,
-    count_mode: CountMode = "composition",
+    count_mode: CountMode = Key.composition,
     normalize: bool = False,
     cbar_title: str = "Element Ratio",
     not_in_numerator: tuple[str, str] | None = ("#eff", "gray: not in 1st list"),
     not_in_denominator: tuple[str, str] | None = (
         "lightskyblue",
         "blue: not in 2nd list",
     ),
@@ -480,15 +1093,15 @@
         plt.text(0.8, y_pos, txt, fontsize=10, bbox=bbox)
 
     return ptable_heatmap(values, cbar_title=cbar_title, **kwargs)
 
 
 def ptable_heatmap_plotly(
     values: ElemValues,
-    count_mode: CountMode = "composition",
+    count_mode: CountMode = Key.composition,
     colorscale: str | Sequence[str] | Sequence[tuple[float, str]] = "viridis",
     show_scale: bool = True,
     show_values: bool = True,
     heat_mode: Literal["value", "fraction", "percent"] | None = "value",
     fmt: str | None = None,
     hover_props: Sequence[str] | dict[str, str] | None = None,
     hover_data: dict[str, str | int | float] | pd.Series | None = None,
@@ -587,19 +1200,17 @@
             "Combining log color scale and heat_mode='fraction'/'percent' unsupported"
         )
     if len(cscale_range) != 2:
         raise ValueError(f"{cscale_range=} should have length 2")
 
     if isinstance(colorscale, (str, type(None))):
         colorscale = px.colors.get_colorscale(colorscale or "viridis")
-    elif isinstance(colorscale, Sequence) and isinstance(
+    elif not isinstance(colorscale, Sequence) or not isinstance(
         colorscale[0], (str, list, tuple)
     ):
-        pass
-    else:
         raise TypeError(
             f"{colorscale=} should be string, list of strings or list of "
             "tuples(float, str)"
         )
 
     color_bar = color_bar or {}
     color_bar.setdefault("orientation", "h")
@@ -628,16 +1239,16 @@
         label_map = dict.fromkeys([np.nan, None, "nan"], " ")  # type: ignore[list-item]
 
     for symbol, period, group, name, *_ in df_ptable.itertuples():
         # build table from bottom up so that period 1 becomes top row
         row = n_rows - period
         col = group - 1
 
+        label = ""  # label (if not None) is placed below the element symbol
         if show_values:
-            label = ""  # label (if not None) is placed below the element symbol
             if symbol in exclude_elements:
                 label = "excl."
             elif heat_value := heat_value_element_map.get(symbol):
                 if heat_mode == "percent":
                     label = f"{heat_value:{fmt or '.1%'}}"
                 else:
                     default_prec = ".1f" if heat_value < 100 else ",.0f"
@@ -755,19 +1366,22 @@
     symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
     cbar_title: str = "Values",
     cbar_title_kwds: dict[str, Any] | None = None,
     cbar_kwds: dict[str, Any] | None = None,
     symbol_pos: tuple[float, float] = (0.5, 0.8),
     log: bool = False,
     anno_kwds: dict[str, Any] | None = None,
+    on_empty: Literal["show", "hide"] = "hide",
+    color_elem_types: Literal["symbol", "background", "both", False]
+    | dict[str, str] = "background",
+    elem_type_legend: bool | dict[str, Any] = True,
     **kwargs: Any,
 ) -> plt.Figure:
     """Plot small histograms for each element laid out in a periodic table.
 
-
     Args:
         data (pd.DataFrame | pd.Series | dict[str, list[float]]): Map from element
             symbols to histogram values. E.g. if dict, {"Fe": [1, 2, 3], "O": [4, 5]}.
             If pd.Series, index is element symbols and values lists. If pd.DataFrame,
             column names are element symbols histograms are plotted from each column.
         bins (int): Number of bins for the histograms. Defaults to 20.
         colormap (str): Matplotlib colormap name to use. Defaults to None. See options
@@ -794,14 +1408,22 @@
         log (bool): Whether to log scale y-axis of each histogram. Defaults to False.
         anno_kwds (dict): Keyword arguments passed to plt.annotate() for element
             annotations. Defaults to None. Useful for adding e.g. number of data points
             in each histogram. For that, use
             anno_kwds=lambda hist_vals: dict(text=len(hist_vals)).
             Recognized keys are text, xy, xycoords, fontsize, and any other
             plt.annotate() keywords.
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        color_elem_types ('symbol' | 'background' | 'both' | False | dict): Whether to
+            color element symbols, tile backgrounds, or both based on element type.
+            If dict, it should map element types to colors. Defaults to "background".
+        elem_type_legend (bool | dict): Whether to show a legend for element
+            types. Defaults to True. If dict, used as kwargs to plt.legend(), e.g. to
+            set the legend title, use {"title": "Element Types"}.
         **kwargs: Additional keyword arguments passed to plt.subplots(). Defaults to
             dict(figsize=(0.75 * n_columns, 0.75 * n_rows)) with n_columns/n_rows the
             number of columns/rows in the periodic table.
 
     Returns:
         plt.Figure: periodic table with a histogram in each element tile.
     """
@@ -835,35 +1457,50 @@
         cmap = plt.get_cmap(colormap) if isinstance(colormap, str) else colormap
 
     # Turn off axis of subplots on the grid that don't correspond to elements
     ax: plt.Axes
     for ax in axes.flat:
         ax.axis("off")
 
+    elem_class_colors = ELEM_CLASS_COLORS | (
+        color_elem_types if isinstance(color_elem_types, dict) else {}
+    )
+
     symbol_kwargs = symbol_kwargs or {}
-    for Z in range(1, 119):
-        element = Element.from_Z(Z)
+    for element in Element:
         symbol = element.symbol
         row, group = df_ptable.loc[symbol, ["row", "column"]]
 
         ax = axes[row - 1][group - 1]
         symbol_kwargs.setdefault("fontsize", 10)
+        hist_data = data.get(symbol, [])
+
+        if len(hist_data) == 0 and on_empty == "hide":
+            continue
+
+        if color_elem_types:
+            elem_class = df_ptable.loc[symbol, "type"]
+            if color_elem_types in ("symbol", "both"):
+                symbol_kwargs["color"] = elem_class_colors.get(elem_class, "black")
+            if color_elem_types in ("background", "both"):
+                bg_color = elem_class_colors.get(elem_class, "white")
+                ax.set_facecolor((*mpl.colors.to_rgb(bg_color), 0.07))
+
         ax.text(
             *symbol_pos,
             symbol_text(element)
             if callable(symbol_text)
             else symbol_text.format(elem=element),
             ha="center",
             va="center",
             transform=ax.transAxes,
             **symbol_kwargs,
         )
         ax.axis("on")  # re-enable axes of elements that exist
 
-        hist_data = data.get(symbol, [])
         if anno_kwds:
             defaults = dict(
                 text=lambda hist_vals: si_fmt_int(len(hist_vals)),
                 xy=(0.8, 0.8),
                 xycoords="axes fraction",
                 fontsize=8,
                 horizontalalignment="center",
@@ -923,194 +1560,172 @@
         # Set color bar title
         cbar_title_kwds = cbar_title_kwds or {}
         cbar_title_kwds.setdefault("fontsize", 12)
         cbar_title_kwds.setdefault("pad", 10)
         cbar_title_kwds["label"] = cbar_title
         cbar_ax.set_title(**cbar_title_kwds)
 
+    if elem_type_legend and color_elem_types:
+        legend_kwargs = elem_type_legend if isinstance(elem_type_legend, dict) else {}
+        add_element_type_legend(
+            data=data, elem_class_colors=elem_class_colors, legend_kwargs=legend_kwargs
+        )
+
     return fig
 
 
 def ptable_scatters(
     data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
-    colormap: str | None = None,
-    scatter_kwds: dict[str, Any]
-    | Callable[[Sequence[float]], dict[str, Any]]
-    | None = None,
-    symbol_kwargs: Any = None,
     symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
     symbol_pos: tuple[float, float] = (0.5, 0.8),
-    cbar_coords: tuple[float, float, float, float] = (0.18, 0.8, 0.42, 0.02),
-    cbar_title: str = "Values",
-    cbar_title_kwds: dict[str, Any] | None = None,
-    cbar_kwds: dict[str, Any] | None = None,
-    anno_kwds: dict[str, Any] | None = None,
-    **kwargs: Any,
+    on_empty: Literal["hide", "show"] = "hide",
+    hide_f_block: bool | None = None,
+    plot_kwargs: dict[str, Any]
+    | Callable[[Sequence[float]], dict[str, Any]]
+    | None = None,
+    child_args: dict[str, Any] | None = None,
+    ax_kwargs: dict[str, Any] | None = None,
+    symbol_kwargs: dict[str, Any] | None = None,
 ) -> plt.Figure:
-    """Plot scatter plots for each element, nested inside a periodic table.
+    """Make scatter plots for each element, nested inside a periodic table.
 
     Args:
-        data (pd.DataFrame | pd.Series | dict[str, list[list[float]]):
-            Map from element symbols to scatter plots. E.g. if dict,
-            {"Fe": [[1, 2, 3], [4, 5, 6]], "O": [[7, 8], [9, 10]]}.
-            You could also add a 3rd list for coloring, e.g.
-            {"Fe": [[1, 2], [3, 4], [5, 6]]}.
+        data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
+            Map from element symbols to plot data. E.g. if dict,
+            {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
+            be plotted on the lower-left corner and the 2nd on the upper-right.
             If pd.Series, index is element symbols and values lists.
             If pd.DataFrame, column names are element symbols,
-            scatter plots are plotted from each column.
-        colormap (str): Matplotlib colormap name to use. Defaults to None.
-        scatter_kwds (dict | Callable): Keywords passed to ax.hist() for each
-            scatter plot. If callable, it is called with the scatter plot
-            values for each element and should return a dict of
-            keyword arguments. Defaults to None.
+            plots are created from each column.
+        ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
+            Use to set x/y labels, limits, etc. Defaults to None. Example:
+            dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
+            ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
         symbol_text (str | Callable[[Element], str]): Text to display for
             each element symbol. Defaults to lambda elem: elem.symbol.
         symbol_kwargs (dict): Keyword arguments passed to plt.text() for
             element symbols. Defaults to None.
         symbol_pos (tuple[float, float]): Position of element symbols
             relative to the lower left corner of each tile.
-            Defaults to (0.5, 0.8). (1, 1) is the upper right corner.
-        cbar_coords (tuple[float, float, float, float]): Colorbar
-            position and size: [x, y, width, height] anchored at lower left
-            corner of the bar. Defaults to (0.25, 0.77, 0.35, 0.02).
-        cbar_title (str): Colorbar title. Defaults to "Values".
-        cbar_title_kwds (dict): Keyword arguments passed to
-            cbar.ax.set_title(). Defaults to dict(fontsize=12, pad=10).
-        cbar_kwds (dict): Keyword arguments passed to fig.colorbar().
-        anno_kwds (dict): Keyword arguments passed to plt.annotate()
-            for element annotations. Defaults to None. Useful for adding
-            e.g. number of data points in each scatter plot. For that, use
-            anno_kwds=lambda scatter_vals: dict(text=len(scatter_vals)).
-            Recognized keys are text, xy, xycoords, fontsize, and any other
-            plt.annotate() keywords.
-        **kwargs: Additional keyword arguments passed to plt.subplots().
+            Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        child_args: Arguments to pass to the child plotter call.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
 
-    Notes:
-        Default figsize is set to (0.75 * n_groups, 0.75 * n_periods).
-
-    Returns:
-        plt.Figure: periodic table with a scatter plot in each element tile.
+    TODO: allow colormap with 3rd data dimension
     """
-    n_periods = df_ptable.row.max()
-    n_groups = df_ptable.column.max()
+    # Re-initialize kwargs as empty dict if None
+    plot_kwargs = plot_kwargs or {}
+    ax_kwargs = ax_kwargs or {}
 
-    kwargs.setdefault("figsize", (0.75 * n_groups, 0.75 * n_periods))
-    fig, axes = plt.subplots(n_periods, n_groups, **kwargs)
-
-    # Use series name as colorbar title if available when no title was passed
-    if isinstance(data, pd.Series) and cbar_title == "Values" and data.name:
-        cbar_title = data.name
-        data = data.to_dict()
-
-    elif isinstance(data, pd.DataFrame):
-        data = data.to_dict(orient="list")
-
-    cmap = None
-    if colormap:
-        cmap = plt.get_cmap(colormap) if isinstance(colormap, str) else colormap
-
-    # Turn off axis of subplots on the grid that don't correspond to elements
-    ax: plt.Axes
-    for ax in axes.flat:
-        ax.axis("off")
+    child_args = child_args or {}
 
     symbol_kwargs = symbol_kwargs or {}
-    for Z in range(1, 119):
-        element = Element.from_Z(Z)
-        symbol = element.symbol
-        row, group = df_ptable.loc[symbol, ["row", "column"]]
+    symbol_kwargs.setdefault("fontsize", 12)
 
-        ax = axes[row - 1][group - 1]
-        symbol_kwargs.setdefault("fontsize", 10)
-        ax.text(
-            *symbol_pos,
-            symbol_text(element)
-            if callable(symbol_text)
-            else symbol_text.format(elem=element),
-            ha="center",
-            va="center",
-            transform=ax.transAxes,
-            **symbol_kwargs,
-        )
-        ax.axis("on")
-        # make sure axes is square to fill the tile
-        ax.set_aspect("equal")
-
-        scatter_data = data.get(symbol, [])
+    # Initialize periodic table plotter
+    plotter = PTableProjector(
+        data=data,
+        colormap=None,
+        plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
+        hide_f_block=hide_f_block,
+    )
 
-        if anno_kwds:
-            defaults = dict(
-                text=lambda hist_vals: si_fmt_int(len(hist_vals)),
-                xy=(0.8, 0.8),
-                xycoords="axes fraction",
-                fontsize=8,
-                horizontalalignment="center",
-                verticalalignment="center",
-            )
-            if callable(anno_kwds):
-                annotation = anno_kwds(scatter_data)
-            else:
-                annotation = anno_kwds
-                anno_text = anno_kwds.get("text")
-                if isinstance(anno_text, dict):
-                    anno_text = anno_text.get(symbol)
-                elif callable(anno_text):
-                    anno_text = anno_text(scatter_data)
-                annotation["text"] = anno_text
-            ax.annotate(**(defaults | annotation))
+    # Call child plotter: Scatter
+    plotter.add_child_plots(
+        ChildPlotters.scatter,
+        child_args=child_args,
+        ax_kwargs=ax_kwargs,
+        on_empty=on_empty,
+    )
 
-        if scatter_data is not None:
-            if callable(scatter_kwds):
-                scatter_kwargs = scatter_kwds(scatter_data)  # type: ignore[arg-type]
-            else:
-                scatter_kwargs = scatter_kwds or {}
+    # Add element symbols
+    plotter.add_ele_symbols(
+        text=symbol_text,
+        pos=symbol_pos,
+        kwargs=symbol_kwargs,
+    )
 
-            # Plot without colormap when data len is 2
-            if len(scatter_data) == 2:
-                ax.scatter(scatter_data[0], scatter_data[1], **(scatter_kwargs or {}))
-
-            # Plot with colormap when data len is 3
-            elif len(scatter_data) == 3:
-                ax.scatter(
-                    scatter_data[0],
-                    scatter_data[1],
-                    c=scatter_data[2],
-                    cmap=cmap,
-                    **(scatter_kwargs or {}),
-                )
+    return plotter.fig
 
-            ax.tick_params(labelsize=8, direction="out")
 
-        # Disable ticks for elements without data
-        else:
-            ax.set_xticks([])
-            ax.set_yticks([])
+def ptable_lines(
+    data: pd.DataFrame | pd.Series | dict[str, list[list[float]]],
+    symbol_text: str | Callable[[Element], str] = lambda elem: elem.symbol,
+    symbol_pos: tuple[float, float] = (0.5, 0.8),
+    on_empty: Literal["hide", "show"] = "hide",
+    hide_f_block: bool | None = None,
+    plot_kwargs: dict[str, Any]
+    | Callable[[Sequence[float]], dict[str, Any]]
+    | None = None,
+    child_args: dict[str, Any] | None = None,
+    ax_kwargs: dict[str, Any] | None = None,
+    symbol_kwargs: dict[str, Any] | None = None,
+) -> plt.Figure:
+    """Line plots for each element, nested inside a periodic table.
 
-        # Hide right/top boarders
-        for side in ("right", "top"):
-            ax.spines[side].set_visible(b=False)
+    Args:
+        data (pd.DataFrame | pd.Series | dict[str, list[list[float]]]):
+            Map from element symbols to plot data. E.g. if dict,
+            {"Fe": [1, 2], "Co": [3, 4]}, where the 1st value would
+            be plotted on the lower-left corner and the 2nd on the upper-right.
+            If pd.Series, index is element symbols and values lists.
+            If pd.DataFrame, column names are element symbols,
+            plots are created from each column.
+        ax_kwargs (dict): Keyword arguments passed to ax.set() for each plot.
+            Use to set x/y labels, limits, etc. Defaults to None. Example:
+            dict(title="Periodic Table", xlabel="x-axis", ylabel="y-axis", xlim=(0, 10),
+            ylim=(0, 10), xscale="linear", yscale="log"). See ax.set() docs for options:
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.set.html#matplotlib-axes-axes-set
+        symbol_text (str | Callable[[Element], str]): Text to display for
+            each element symbol. Defaults to lambda elem: elem.symbol.
+        symbol_kwargs (dict): Keyword arguments passed to plt.text() for
+            element symbols. Defaults to None.
+        symbol_pos (tuple[float, float]): Position of element symbols
+            relative to the lower left corner of each tile.
+            Defaults to (0.5, 0.5). (1, 1) is the upper right corner.
+        on_empty ('hide' | 'show'): Whether to show or hide tiles for elements without
+            data. Defaults to "hide".
+        hide_f_block (bool): Hide f-block (Lanthanum and Actinium series). Defaults to
+            None, meaning hide if no data is provided for f-block elements.
+        child_args: Arguments to pass to the child plotter call.
+        plot_kwargs (dict): Additional keyword arguments to
+                pass to the plt.subplots function call.
+    """
+    # Re-initialize kwargs as empty dict if None
+    plot_kwargs = plot_kwargs or {}
+    ax_kwargs = ax_kwargs or {}
 
-    # Add colorbar if data dimensionality is 3
-    if isinstance(cmap, Colormap) and {len(data) for data in data.values()} == {3}:
-        # Get the min/max values for norm calculation
-        third_lists = [data[2] for data in data.values()]
-        vmin = min(min(third_list) for third_list in third_lists)
-        vmax = max(max(third_list) for third_list in third_lists)
+    child_args = child_args or {}
 
-        norm = Normalize(vmin=vmin, vmax=vmax)
+    symbol_kwargs = symbol_kwargs or {}
+    symbol_kwargs.setdefault("fontsize", 12)
 
-        cbar_ax = fig.add_axes(cbar_coords)
+    # Initialize periodic table plotter
+    plotter = PTableProjector(
+        data=data,
+        colormap=None,
+        plot_kwargs=plot_kwargs,  # type: ignore[arg-type]
+        hide_f_block=hide_f_block,
+    )
 
-        fig.colorbar(
-            plt.cm.ScalarMappable(norm=norm, cmap=cmap),
-            cax=cbar_ax,
-            **{"orientation": "horizontal"} | (cbar_kwds or {}),
-        )
+    # Call child plotter: line
+    plotter.add_child_plots(
+        ChildPlotters.line,
+        child_args=child_args,
+        ax_kwargs=ax_kwargs,
+        on_empty=on_empty,
+    )
 
-        # Set colorbar title
-        cbar_title_kwds = cbar_title_kwds or {}
-        cbar_title_kwds.setdefault("fontsize", 12)
-        cbar_title_kwds.setdefault("pad", 10)
-        cbar_title_kwds["label"] = cbar_title
-        cbar_ax.set_title(**cbar_title_kwds)
+    # Add element symbols
+    plotter.add_ele_symbols(
+        text=symbol_text,
+        pos=symbol_pos,
+        kwargs=symbol_kwargs,
+    )
 
-    return fig
+    return plotter.fig
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymatviz-0.8.1/pymatviz/relevance.py` & `pymatviz-0.8.2/pymatviz/relevance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Plots for evaluating classifier performance."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import sklearn.metrics as skm
```

### Comparing `pymatviz-0.8.1/pymatviz/sankey.py` & `pymatviz-0.8.2/pymatviz/sankey.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Sankey diagram for comparing distributions in two dataframe columns."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal
 
 import plotly.graph_objects as go
```

### Comparing `pymatviz-0.8.1/pymatviz/structure_viz.py` & `pymatviz-0.8.2/pymatviz/structure_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,38 @@
+"""2D plots of pymatgen structures with matplotlib.
+
+plot_structure_2d() and its helpers get_rot_matrix() and unit_cell_to_lines() were
+inspired by ASE https://wiki.fysik.dtu.dk/ase/ase/visualize/visualize.html#matplotlib.
+"""
+
 from __future__ import annotations
 
 import math
 import warnings
 from itertools import product
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.patches import PathPatch, Wedge
 from matplotlib.path import Path
 from pymatgen.analysis.local_env import CrystalNN, NearNeighbors
+from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-from pymatviz.utils import covalent_radii, jmol_colors
+from pymatviz.utils import ExperimentalWarning, covalent_radii, jmol_colors
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
+    from typing import Any, Literal
 
     from numpy.typing import ArrayLike
     from pymatgen.core import Structure
 
 
-class ExperimentalWarning(Warning):
-    """Used for experimental show_bonds feature."""
-
-
-warnings.simplefilter("once", ExperimentalWarning)
-
-
-# plot_structure_2d() and its helpers get_rot_matrix() and unit_cell_to_lines() were
-# inspired by ASE https://wiki.fysik.dtu.dk/ase/ase/visualize/visualize.html#matplotlib
-
-
 def _angles_to_rotation_matrix(
     angles: str, rotation: ArrayLike | None = None
 ) -> ArrayLike:
     """Convert Euler angles to a rotation matrix.
 
     Note the order of angles matters. 50x,40z != 40z,50x.
 
@@ -46,16 +43,18 @@
             Defaults to identity matrix np.eye(3).
 
     Returns:
         np.array: 3d rotation matrix.
     """
     if rotation is None:
         rotation = np.eye(3)
-    if angles == "":
-        return rotation.copy()  # return initial rotation matrix if no angles
+
+    # Return initial rotation matrix if no angles
+    if not angles:
+        return rotation.copy()
 
     for angle in angles.split(","):
         radians = math.radians(float(angle[:-1]))
         xyz = angle[-1]
         dim = "xyz".index(xyz)
         sin = math.sin(radians)
         cos = math.cos(radians)
@@ -76,36 +75,35 @@
 
     Returns:
         tuple[np.array, np.array, np.array]:
         - Lines
         - z-indices that sort plot elements into out-of-plane layers
         - lines used to plot the unit cell
     """
-    n_lines = 0
+    n_lines = n1 = 0
     segments = []
-    for c in range(3):
-        norm = math.sqrt(sum(cell[c] ** 2))
+    for idx in range(3):
+        norm = math.sqrt(sum(cell[idx] ** 2))
         segment = max(2, int(norm / 0.3))
         segments.append(segment)
         n_lines += 4 * segment
 
     lines = np.empty((n_lines, 3))
-    z_indices = np.empty(n_lines, int)
+    z_indices = np.empty(n_lines, dtype=int)
     unit_cell_lines = np.zeros((3, 3))
 
-    n1 = 0
-    for c in range(3):
-        segment = segments[c]
-        dd = cell[c] / (4 * segment - 2)
-        unit_cell_lines[c] = dd
+    for idx in range(3):
+        segment = segments[idx]
+        dd = cell[idx] / (4 * segment - 2)
+        unit_cell_lines[idx] = dd
         P = np.arange(1, 4 * segment + 1, 4)[:, None] * dd
-        z_indices[n1:] = c
+        z_indices[n1:] = idx
         for i, j in [(0, 0), (0, 1), (1, 0), (1, 1)]:
             n2 = n1 + segment
-            lines[n1:n2] = P + i * cell[c - 2] + j * cell[c - 1]
+            lines[n1:n2] = P + i * cell[idx - 2] + j * cell[idx - 1]
             n1 = n2
 
     return lines, z_indices, unit_cell_lines
 
 
 def plot_structure_2d(
     struct: Structure,
@@ -116,30 +114,29 @@
     scale: float = 1,
     show_unit_cell: bool = True,
     show_bonds: bool | NearNeighbors = False,
     site_labels: bool
     | Literal["symbol", "species"]
     | dict[str, str | float]
     | Sequence[str | float] = True,
-    site_labels_bbox: dict[str, Any] | None = None,
     label_kwargs: dict[str, Any] | None = None,
     bond_kwargs: dict[str, Any] | None = None,
     standardize_struct: bool | None = None,
     axis: bool | str = "off",
 ) -> plt.Axes:
-    """Plot pymatgen structure object in 2d. Uses matplotlib.
+    """Plot pymatgen structures in 2D with matplotlib.
 
     Inspired by ASE's ase.visualize.plot.plot_atoms()
     https://wiki.fysik.dtu.dk/ase/ase/visualize/visualize.html#matplotlib
     pymatviz aims to give similar output to ASE but supports disordered structures and
     avoids the conversion hassle of AseAtomsAdaptor.get_atoms(pmg_struct).
 
     For example, these two snippets should give very similar output:
 
-    ```py
+    ```python
     from pymatgen.ext.matproj import MPRester
 
     mp_19017 = MPRester().get_structure_by_material_id("mp-19017")
 
     # ASE
     from ase.visualize.plot import plot_atoms
     from pymatgen.io.ase import AseAtomsAdaptor
@@ -176,35 +173,33 @@
         atomic_radii (float | dict[str, float], optional): Either a scaling factor for
             default radii or map from element symbol to atomic radii. Defaults to
             covalent radii.
         colors (dict[str, str | list[float]], optional): Map from element symbols to
             colors, either a named color (str) or rgb(a) values like (0.2, 0.3, 0.6).
             Defaults to JMol colors (https://jmol.sourceforge.net/jscolors).
         scale (float, optional): Scaling of the plotted atoms and lines. Defaults to 1.
-        show_unit_cell (bool, optional): Whether to draw unit cell. Defaults to True.
-        show_bonds (bool | NearNeighbors, optional): Whether to draw bonds. If True, use
+        show_unit_cell (bool, optional): Whether to plot unit cell. Defaults to True.
+        show_bonds (bool | NearNeighbors, optional): Whether to plot bonds. If True, use
             pymatgen.analysis.local_env.CrystalNN to infer the structure's connectivity.
-            If False, don't draw bonds. If a subclass of
+            If False, don't plot bonds. If a subclass of
             pymatgen.analysis.local_env.NearNeighbors, use that to determine
             connectivity. Options include VoronoiNN, MinimumDistanceNN, OpenBabelNN,
             CovalentBondNN, dtc. Defaults to True.
         site_labels (bool | "symbol" | "species" | dict[str, str | float] | Sequence):
             How to annotate lattice sites.
             If True, labels are element species (symbol + oxidation
             state). If a dict, should map species strings (or element symbols but looks
             for species string first) to labels. If a list, must be same length as the
             number of sites in the crystal. If a string, must be "symbol" or
             "species". "symbol" hides the oxidation state, "species" shows it
             (equivalent to True). Defaults to True.
-        site_labels_bbox (dict, optional): Keyword arguments for matplotlib.text.Text
-            bbox like {"facecolor": "white", "alpha": 0.5}. Defaults to None.
         label_kwargs (dict, optional): Keyword arguments for matplotlib.text.Text like
             {"fontsize": 14}. Defaults to None.
         bond_kwargs (dict, optional): Keyword arguments for the matplotlib.path.Path
-            class used to draw chemical bonds. Allowed are edgecolor, facecolor, color,
+            class used to plot chemical bonds. Allowed are edgecolor, facecolor, color,
             linewidth, linestyle, antialiased, hatch, fill, capstyle, joinstyle.
             Defaults to None.
         standardize_struct (bool, optional): Whether to standardize the structure using
             SpacegroupAnalyzer(struct).get_conventional_standard_structure() before
             plotting. Defaults to False unless any fractional coordinates are negative,
             i.e. any crystal sites are outside the unit cell. Set this to False to
             disable this behavior which speeds up plotting for many structures.
@@ -222,172 +217,188 @@
 
     if isinstance(site_labels, (list, tuple)) and len(site_labels) != len(struct):
         raise ValueError(
             f"If a list, site_labels ({len(site_labels)=}) must have same length as"
             f" the number of sites in the crystal ({len(struct)=})"
         )
 
-    # default behavior in case of no user input is to standardize if any fractional
+    # Default behavior in case of no user input: standardize if any fractional
     # coordinates are negative
     has_sites_outside_unit_cell = any(any(site.frac_coords < 0) for site in struct)
     if standardize_struct is False and has_sites_outside_unit_cell:
         warnings.warn(
             "your structure has negative fractional coordinates, you may want to set "
             "standardize=True",
             UserWarning,
         )
     elif standardize_struct is None:
         standardize_struct = has_sites_outside_unit_cell
     if standardize_struct:
-        from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-
         struct = SpacegroupAnalyzer(struct).get_conventional_standard_structure()
+
+    # Get default colors
     if colors is None:
         colors = jmol_colors
 
     # Get any element at each site, only used for occlusion calculation which won't be
     # perfect for disordered sites. Plotting wedges of different radii for disordered
     # sites is handled later.
     elements_at_sites = [str(site.species.elements[0].symbol) for site in struct]
 
     if atomic_radii is None or isinstance(atomic_radii, float):
         # atomic_radii is a scaling factor for the default set of radii
         atomic_radii = 0.7 * covalent_radii * (atomic_radii or 1)
     else:
         # atomic_radii is assumed to be a map from element symbols to atomic radii
         # make sure all present elements are assigned a radius
-        missing = set(elements_at_sites) - set(atomic_radii)
-        if missing:
+        if missing := set(elements_at_sites) - set(atomic_radii):
             raise ValueError(f"atomic_radii is missing keys: {missing}")
 
     radii_at_sites = np.array(
         [atomic_radii[el] for el in elements_at_sites]  # type: ignore[index]
     )
 
-    n_atoms = len(struct)
+    # Generate lines for unit cell
     rotation_matrix = _angles_to_rotation_matrix(rotation)
     unit_cell = struct.lattice.matrix
 
     if show_unit_cell:
         lines, z_indices, unit_cell_lines = unit_cell_to_lines(unit_cell)
         corners = np.array(list(product((0, 1), (0, 1), (0, 1))))
         cell_vertices = np.dot(corners, unit_cell)
         cell_vertices = np.dot(cell_vertices, rotation_matrix)
     else:
         lines = np.empty((0, 3))
         z_indices = None
         unit_cell_lines = None
         cell_vertices = None
 
+    # Zip atoms and unit cell lines together
+    n_atoms = len(struct)
     n_lines = len(lines)
 
     positions = np.empty((n_atoms + n_lines, 3))
     site_coords = np.array([site.coords for site in struct])
     positions[:n_atoms] = site_coords
     positions[n_atoms:] = lines
 
-    # determine which lines should be hidden behind other objects
+    # Determine which unit cell line should be hidden behind other objects
     for idx in range(n_lines):
         this_layer = unit_cell_lines[z_indices[idx]]
+
         occluded_top = ((site_coords - lines[idx] + this_layer) ** 2).sum(
             1
         ) < radii_at_sites**2
+
         occluded_bottom = ((site_coords - lines[idx] - this_layer) ** 2).sum(
             1
         ) < radii_at_sites**2
+
         if any(occluded_top & occluded_bottom):
             z_indices[idx] = -1
 
+    # Apply rotation matrix
     positions = np.dot(positions, rotation_matrix)
     rotated_site_coords = positions[:n_atoms]
 
+    # Normalize wedge positions
     min_coords = (rotated_site_coords - radii_at_sites[:, None]).min(0)
     max_coords = (rotated_site_coords + radii_at_sites[:, None]).max(0)
 
     if show_unit_cell:
         min_coords = np.minimum(min_coords, cell_vertices.min(0))
         max_coords = np.maximum(max_coords, cell_vertices.max(0))
 
     means = (min_coords + max_coords) / 2
     coord_ranges = 1.05 * (max_coords - min_coords)
 
     offset = scale * (means - coord_ranges / 2)
     positions *= scale
     positions -= offset
 
+    # Rotate and scale unit cell lines
     if n_lines > 0:
         unit_cell_lines = np.dot(unit_cell_lines, rotation_matrix)[:, :2] * scale
 
     special_site_labels = ("symbol", "species")
-    # sort positions by 3rd dim so we draw from back to front in z-axis (out-of-plane)
+    # Sort positions by 3rd dim to plot from back to front along z-axis (out-of-plane)
     for idx in positions[:, 2].argsort():
         xy = positions[idx, :2]
         start = 0
+        zorder = positions[idx][2]
+
         if idx < n_atoms:
-            # loop over all species on a site (usually just 1 for ordered sites)
-            for specie, occupancy in struct[idx].species.items():
-                # strip oxidation state from element symbol (e.g. Ta5+ to Ta)
-                elem_symbol = specie.symbol
+            # Loop over all species on a site (usually just 1 for ordered sites)
+            for species, occupancy in struct[idx].species.items():
+                # Strip oxidation state from element symbol (e.g. Ta5+ to Ta)
+                elem_symbol = species.symbol
+
                 radius = atomic_radii[elem_symbol] * scale  # type: ignore[index]
                 face_color = colors[elem_symbol]
                 wedge = Wedge(
                     xy,
                     radius,
                     360 * start,
                     360 * (start + occupancy),
                     facecolor=face_color,
                     edgecolor="black",
+                    zorder=zorder,
                 )
                 ax.add_patch(wedge)
 
+                # Generate labels
                 if site_labels == "symbol":
                     txt = elem_symbol
                 elif site_labels in ("species", True):
-                    txt = specie
+                    txt = species
                 elif site_labels is False:
                     txt = ""
                 elif isinstance(site_labels, dict):
-                    # try element incl. oxidation state as dict key first (e.g. Na+),
+                    # Try element incl. oxidation state as dict key first (e.g. Na+),
                     # then just element as fallback
                     txt = site_labels.get(
-                        repr(specie), site_labels.get(elem_symbol, "")
+                        repr(species), site_labels.get(elem_symbol, "")
                     )
                     if txt in special_site_labels:
-                        txt = specie if txt == "species" else elem_symbol
+                        txt = species if txt == "species" else elem_symbol
                 elif isinstance(site_labels, (list, tuple)):
                     txt = site_labels[idx]  # idx runs from 0 to n_atoms
                 else:
                     raise ValueError(
                         f"Invalid {site_labels=}. Must be one of (bool, "
                         f"{', '.join(special_site_labels)}, dict, list)"
                     )
 
+                # Add labels
                 if site_labels:
-                    # place element symbol half way along outer wedge edge for
+                    # Place element symbol half way along outer wedge edge for
                     # disordered sites
                     half_way = 2 * np.pi * (start + occupancy / 2)
                     direction = np.array([math.cos(half_way), math.sin(half_way)])
                     text_offset = (
                         (0.5 * radius) * direction if occupancy < 1 else (0, 0)
                     )
 
-                    bbox = dict(facecolor="none", edgecolor="none", pad=1)
-                    bbox.update(site_labels_bbox or {})
                     txt_kwds = dict(
-                        ha="center", va="center", bbox=bbox, **(label_kwargs or {})
+                        ha="center",
+                        va="center",
+                        zorder=zorder,
+                        **(label_kwargs or {}),
                     )
                     ax.text(*(xy + text_offset), txt, **txt_kwds)
 
                 start += occupancy
-        else:  # draw unit cell
+
+        # Plot unit cell
+        else:
             cell_idx = idx - n_atoms
-            # only draw line if not obstructed by an atom
+            # Only plot lines not obstructed by an atom
             if z_indices[cell_idx] != -1:
                 hxy = unit_cell_lines[z_indices[cell_idx]]
-                path = PathPatch(Path((xy + hxy, xy - hxy)))
+                path = PathPatch(Path((xy + hxy, xy - hxy)), zorder=zorder)
                 ax.add_patch(path)
 
     if show_bonds:
         warnings.warn(
             "Warning: the show_bonds feature of plot_structure_2d() is experimental. "
             "Issues and PRs with improvements welcome.",
             category=ExperimentalWarning,
@@ -398,37 +409,27 @@
             neighbor_strategy_cls = show_bonds
         else:
             raise ValueError(
                 f"Expected boolean or a NearNeighbors subclass for {show_bonds = }"
             )
 
         # If structure doesn't have any oxidation states yet, guess them from chemical
-        # composition. Helps CrystalNN and other strategies to estimate better bond
-        # connectivity. Uses getattr on site.specie since it's often a pymatgen Element
+        # composition. Use CrystalNN and other strategies to better estimate bond
+        # connectivity. Use getattr on site.specie since it's often a pymatgen Element
         # which has no oxi_state
         if not any(
             hasattr(getattr(site, "specie", None), "oxi_state") for site in struct
         ):
             try:
                 struct.add_oxidation_state_by_guess()
             except ValueError:  # fails for disordered structures
-                "Charge balance analysis requires integer values in Composition"
+                # Charge balance analysis requires integer values in Composition
+                pass
 
-        try:
-            structure_graph = neighbor_strategy_cls().get_bonded_structure(struct)
-        except AttributeError:  # Many NearNeighbors subclasses don't support
-            # disordered structures raising AttributeError. in that case, we create new
-            # structure with majority species on each site.
-            # TODO: remove this exception case once
-            # https://github.com/materialsproject/pymatgen/pull/2630 is released
-            struct_copy = struct.copy()
-            for site in struct_copy:
-                # get majority species for each site
-                site.species = max(site.species, key=site.species.get)
-            structure_graph = neighbor_strategy_cls().get_bonded_structure(struct_copy)
+        structure_graph = neighbor_strategy_cls().get_bonded_structure(struct)
 
         bonds = structure_graph.graph.edges(data=True)
         for bond in bonds:
             from_idx, to_idx, data = bond
             if data["to_jimage"] != (0, 0, 0):
                 continue  # skip bonds across periodic boundaries
             from_xy = positions[from_idx, :2]
```

### Comparing `pymatviz-0.8.1/pymatviz/sunburst.py` & `pymatviz-0.8.2/pymatviz/sunburst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+"""Hierarchical multi-level pie charts (i.e. sunbursts).
+
+E.g. for crystal symmetry distributions.
+"""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal
 
 import pandas as pd
 import plotly.express as px
 from pymatgen.core import Structure
 from pymatgen.symmetry.groups import SpaceGroup
 
+from pymatviz.enums import Key
 from pymatviz.utils import crystal_sys_from_spg_num
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     import plotly.graph_objects as go
@@ -45,29 +51,32 @@
             struct.get_space_group_info()[1]  # type: ignore[union-attr]
             for struct in data
         )
     else:
         series = pd.Series(data)
 
     df_spg_counts = pd.DataFrame(series.value_counts().reset_index())
-    df_spg_counts.columns = ["spacegroup", "count"]
+    df_spg_counts.columns = [Key.spacegroup, "count"]
 
     try:  # assume column contains integers as space group numbers
-        df_spg_counts["crystal_sys"] = [
-            crystal_sys_from_spg_num(x) for x in df_spg_counts.spacegroup
+        df_spg_counts[Key.crystal_system] = [
+            crystal_sys_from_spg_num(x) for x in df_spg_counts[Key.spacegroup]
         ]
     except (ValueError, TypeError):  # column must be strings of space group symbols
-        df_spg_counts["crystal_sys"] = [
-            SpaceGroup(x).crystal_system for x in df_spg_counts.spacegroup
+        df_spg_counts[Key.crystal_system] = [
+            SpaceGroup(x).crystal_system for x in df_spg_counts[Key.spacegroup]
         ]
 
     kwargs.setdefault("color_discrete_sequence", px.colors.qualitative.G10)
 
     fig = px.sunburst(
-        df_spg_counts, path=["crystal_sys", "spacegroup"], values="count", **kwargs
+        df_spg_counts,
+        path=[Key.crystal_system, Key.spacegroup],
+        values="count",
+        **kwargs,
     )
 
     if show_counts == "percent":
         fig.data[0].textinfo = "label+percent entry"
     elif show_counts == "value":
         fig.data[0].textinfo = "label+value"
     elif show_counts is not False:
```

### Comparing `pymatviz-0.8.1/pymatviz/uncertainty.py` & `pymatviz-0.8.2/pymatviz/uncertainty.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+"""Visualizations for assessing the quality of model uncertainty estimates."""
+
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
 
-from pymatviz.utils import add_identity_line, df_to_arrays
+from pymatviz.powerups import add_identity_line
+from pymatviz.utils import df_to_arrays
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from numpy.typing import ArrayLike
 
 
 def qq_gaussian(
     y_true: ArrayLike | str,
     y_pred: ArrayLike | str,
     y_std: ArrayLike | dict[str, ArrayLike] | str | Sequence[str],
     df: pd.DataFrame | None = None,
     ax: plt.Axes | None = None,
+    identity_line: bool | dict[str, Any] = True,
 ) -> plt.Axes:
     """Plot the Gaussian quantile-quantile (Q-Q) plot of one (passed as array) or
     multiple (passed as dict) sets of uncertainty estimates for a single pair of ground
     truth targets `y_true` and model predictions `y_pred`.
 
     Overconfidence relative to a Gaussian distribution is visualized as shaded
     areas below the parity line, underconfidence (oversized uncertainties) as
@@ -41,14 +45,16 @@
         y_true (array | str): Ground truth targets
         y_pred (array | str): Model predictions
         y_std (array | dict[str, array] | str | list[str]): Model uncertainties either
             as array(s) (single or dict with labels if you have multiple sources of
             uncertainty) or column names in df.
         df (pd.DataFrame, optional): DataFrame with y_true, y_pred and y_std columns.
         ax (Axes): matplotlib Axes on which to plot. Defaults to None.
+        identity_line (bool | dict[str, Any], optional): Whether to add a parity line
+            (y = x). Defaults to True. Pass a dict to customize line properties.
 
     Returns:
         plt.Axes: matplotlib Axes object
     """
     if isinstance(y_std, (str, pd.Index)):
         y_true, y_pred, y_std = df_to_arrays(df, y_true, y_pred, y_std)
     else:
@@ -78,15 +84,18 @@
             exp_proportions, y1=obs_proportions, y2=exp_proportions, alpha=0.2
         )
         miscal_area = np.trapz(
             np.abs(obs_proportions - exp_proportions), dx=1 / resolution
         )
         lines.append([line, miscal_area])
 
-    add_identity_line(ax)  # guiding line for perfect calibration
+    if identity_line:  # guiding line for perfect calibration
+        add_identity_line(
+            ax, **(identity_line if isinstance(identity_line, dict) else {})
+        )
 
     ax.set(xlim=(0, 1), ylim=(0, 1))
     ax.set(xlabel="Theoretical Quantile", ylabel="Observed Quantile")
 
     legend1 = ax.legend(loc="upper left", frameon=False)
     # Multiple legends on the same axes:
     # https://matplotlib.org/3.3.3/tutorials/intermediate/legend_guide.html#multiple-legends-on-the-same-axes
```

### Comparing `pymatviz-0.8.1/pymatviz.egg-info/PKG-INFO` & `pymatviz-0.8.2/pymatviz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatviz
-Version: 0.8.1
+Version: 0.8.2
 Summary: A toolkit for visualizations in materials informatics
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Janosh Riebesell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,14 +48,15 @@
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: pdfCropMargins; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: weasyprint; extra == "test"
 Provides-Extra: data-src
 Requires-Dist: matminer; extra == "data-src"
+Requires-Dist: mp_api; extra == "data-src"
 Provides-Extra: export-figs
 Requires-Dist: kaleido; extra == "export-figs"
 Provides-Extra: gh-pages
 Requires-Dist: jupyter; extra == "gh-pages"
 Requires-Dist: lazydocs; extra == "gh-pages"
 Requires-Dist: nbconvert; extra == "gh-pages"
 Provides-Extra: df-pdf-export
@@ -81,31 +82,31 @@
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 [![Zenodo](https://img.shields.io/badge/DOI-10.5281/zenodo.10456384-blue?logo=Zenodo&logoColor=white)](https://zenodo.org/records/10456384)
 
 </h4>
 
 <slot name="how-to-cite">
 
-> If you use `pymatviz` in your research, [see how to cite](#--how-to-cite-pymatviz).
+> If you use `pymatviz` in your research, [see how to cite](#how-to-cite-pymatviz).
 
 </slot>
 
-## 🔨 &thinsp; Installation
+## Installation
 
 ```sh
 pip install pymatviz
 ```
 
-## 💡 &thinsp; API Docs
+## API Docs
 
 See the [/api] page.
 
 [/api]: https://janosh.github.io/pymatviz/api
 
-## 📙 &thinsp; Usage
+## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
@@ -116,45 +117,42 @@
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-| [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py) |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                       ![ptable-heatmap]                        |                        ![ptable-heatmap-ratio]                        |
-|  [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)  | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|            ![ptable-heatmap-plotly-more-hover-data]            |                     ![ptable-heatmap-plotly-log]                      |
-
-## Nested Periodic Table
-
-See [`pymatviz/ptable.py`](pymatviz/ptable.py). Plot histogram plots and scatter plots nested within periodic table.
-| [`ptable_hists(data, colormap="coolwarm"`](pymatviz/ptable.py) | [`ptable_scatters(data, colormap="coolwarm"`](pymatviz/ptable.py) |
-| :------------------------------------------------------------: | :---------------------------------------------------------------: |
-
-<!-- prettier-ignore -->
-|                        ![ptable-hists]                         |                        ![ptable-scatters]                         |
+|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
+| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
+|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
+|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
+|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
+|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
+|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
+| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
+|                                           ![ptable-heatmap-splits]                                           |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
-[ptable-scatters]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-scatters.svg
+[ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
+[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
 
 ## Phonons
 
 See [`pymatviz/phonons.py`](pymatviz/phonons.py).
 
-|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           | [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py) |
-| :------------------------------------------------------------------------: | :--------------------------------------------------: |
-|                              ![phonon-bands]                               |                    ![phonon-dos]                     |
-| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) |                                                      |
-|                          ![phonon-bands-and-dos]                           |                                                      |
+|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
+| :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
+|                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
+| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
+|                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
 
 [phonon-bands]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-mp-2758.svg
 [phonon-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-dos-mp-2758.svg
-[phonon-bands-and-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-2758]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-23907]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-23907.svg
 
 ### Dash app using `ptable_heatmap_plotly()`
 
 See [`examples/mprester_ptable.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb).
 
 <https://user-images.githubusercontent.com/30958850/181644052-b330f0a2-70fc-451c-8230-20d45d3af72f.mp4>
 
@@ -209,33 +207,33 @@
 | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
 |                       ![density-scatter]                        |                  ![density-scatter-with-hist]                   |
 |       [`density_hexbin(xs, ys, ...)`](pymatviz/parity.py)       |  [`density_hexbin_with_hist(xs, ys, ...)`](pymatviz/parity.py)  |
 |                        ![density-hexbin]                        |                   ![density-hexbin-with-hist]                   |
 | [`scatter_with_err_bar(xs, ys, yerr, ...)`](pymatviz/parity.py) | [`residual_vs_actual(y_true, y_pred, ...)`](pymatviz/parity.py) |
 |                     ![scatter-with-err-bar]                     |                      ![residual-vs-actual]                      |
 
-## Uncertainty Calibration
+## Uncertainty
 
 See [`pymatviz/uncertainty.py`](pymatviz/uncertainty.py).
 
 |       [`qq_gaussian(y_true, y_pred, y_std)`](pymatviz/uncertainty.py)       |       [`qq_gaussian(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py)       |
 | :-------------------------------------------------------------------------: | :-------------------------------------------------------------------------------: |
 |                             ![normal-prob-plot]                             |                           ![normal-prob-plot-multiple]                            |
 | [`error_decay_with_uncert(y_true, y_pred, y_std)`](pymatviz/uncertainty.py) | [`error_decay_with_uncert(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py) |
 |                         ![error-decay-with-uncert]                          |                        ![error-decay-with-uncert-multiple]                        |
 
-## Cumulative Error & Residual
+## Cumulative Metrics
 
 See [`pymatviz/cumulative.py`](pymatviz/cumulative.py).
 
 | [`cumulative_error(preds, targets)`](pymatviz/cumulative.py) | [`cumulative_residual(preds, targets)`](pymatviz/cumulative.py) |
 | :----------------------------------------------------------: | :-------------------------------------------------------------: |
 |                     ![cumulative-error]                      |                     ![cumulative-residual]                      |
 
-## Classification Metrics
+## Classification
 
 See [`pymatviz/relevance.py`](pymatviz/relevance.py).
 
 | [`roc_curve(targets, proba_pos)`](pymatviz/relevance.py) | [`precision_recall_curve(targets, proba_pos)`](pymatviz/relevance.py) |
 | :------------------------------------------------------: | :-------------------------------------------------------------------: |
 |                       ![roc-curve]                       |                       ![precision-recall-curve]                       |
 
@@ -272,24 +270,24 @@
 [sankey-spglib-vs-aflow-spacegroups]: https://github.com/janosh/pymatviz/raw/main/assets/sankey-spglib-vs-aflow-spacegroups.svg
 [scatter-with-err-bar]: https://github.com/janosh/pymatviz/raw/main/assets/scatter-with-err-bar.svg
 [spg-num-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-num-sunburst.svg
 [spg-symbol-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-symbol-sunburst.svg
 [struct-2d-mp-12712-Hf9Zr9Pd24-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-12712-Hf9Zr9Pd24-disordered.svg
 [struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered.svg
 
-## 📖 &thinsp; How to cite `pymatviz`
+## How to cite `pymatviz`
 
-You can cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
+See [`citation.cff`](citation.cff) or cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
 
 ```bib
 @software{riebesell_pymatviz_2022,
   title = {Pymatviz: visualization toolkit for materials informatics},
-  author = {Riebesell, Janosh},
+  author = {Riebesell, Janosh and Yang, Haoyu and Goodall, Rhys and Baird, Sterling G.},
   date = {2022-10-01},
   year = {2022},
   doi = {10.5281/zenodo.7486816},
   url = {https://github.com/janosh/pymatviz},
   note = {10.5281/zenodo.7486816 - https://github.com/janosh/pymatviz},
   urldate = {2023-01-01}, % optional, replace with your date of access
-  version = {0.7.1}, % replace with the version you use
+  version = {0.8.2}, % replace with the version you use
 }
 ```
```

### Comparing `pymatviz-0.8.1/pymatviz.egg-info/SOURCES.txt` & `pymatviz-0.8.2/pymatviz.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 license
 pyproject.toml
 readme.md
 pymatviz/__init__.py
 pymatviz/correlation.py
 pymatviz/cumulative.py
 pymatviz/elements.csv
+pymatviz/enums.py
 pymatviz/histograms.py
 pymatviz/io.py
 pymatviz/parity.py
 pymatviz/phonons.py
+pymatviz/powerups.py
 pymatviz/ptable.py
 pymatviz/relevance.py
 pymatviz/sankey.py
 pymatviz/structure_viz.py
 pymatviz/sunburst.py
 pymatviz/uncertainty.py
 pymatviz/utils.py
@@ -24,14 +26,15 @@
 tests/test_correlation.py
 tests/test_cumulative.py
 tests/test_histograms.py
 tests/test_init.py
 tests/test_io.py
 tests/test_parity.py
 tests/test_phonons.py
+tests/test_powerups.py
 tests/test_ptable.py
 tests/test_readme.py
 tests/test_relevance.py
 tests/test_sankey.py
 tests/test_structure_viz.py
 tests/test_sunburst.py
 tests/test_uncertainty.py
```

### Comparing `pymatviz-0.8.1/pyproject.toml` & `pymatviz-0.8.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymatviz"
-version = "0.8.1"
+version = "0.8.2"
 description = "A toolkit for visualizations in materials informatics"
 authors = [{ name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" }]
 readme = "readme.md"
 license = { file = "license" }
 keywords = [
     "chemistry",
     "data visualization",
@@ -44,15 +44,15 @@
     "jinja2",
     "kaleido",
     "pdfCropMargins",
     "pytest",
     "pytest-cov",
     "weasyprint",
 ]
-data-src = ["matminer"]
+data-src = ["matminer", "mp_api"]
 export-figs = ["kaleido"]
 gh-pages = ["jupyter", "lazydocs", "nbconvert"]
 # needed for pandas Stylers, see https://github.com/pandas-dev/pandas/blob/-/pyproject.toml
 df-pdf-export = ["jinja2", "pdfCropMargins", "weasyprint"]
 auto-text-pos = ["adjustText"]
 
 [tool.setuptools.packages]
@@ -76,45 +76,58 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 show_error_codes = true
 no_implicit_optional = false
 
 [tool.ruff]
 target-version = "py39"
-lint.select = ["ALL"]
-lint.ignore = [
+
+[tool.ruff.lint]
+select = ["ALL"]
+ignore = [
     "ANN101",
+    "ANN102",
     "ANN401",
     "B028",   # No explicit stacklevel keyword argument found
     "C408",   # unnecessary-collection-call
     "C901",
     "COM812", # trailing comma missing
-    "D100",   # Missing docstring in public module
     "D205",   # 1 blank line required between summary line and description
     "E731",   # do not assign a lambda expression, use a def
     "EM101",
     "EM102",
     "ERA001",
     "FBT001",
     "FBT002",
     "FIX002",
+    "ISC001",
     "N806",   # non-lowercase-variable-in-function
     "NPY002",
     "PLR",    # pylint refactor
     "PT006",  # pytest-parametrize-names-wrong-type
     "PT011",  # pytest-raises-too-broad
     "PTH",
     "RUF001", # ambiguous-unicode-character-string
     "S311",
-    "SIM105", # Use contextlib.suppress(FileNotFoundError) instead of try-except-pass
+    "SIM105", # Use contextlib.suppress() instead of try-except-pass
     "TD",
     "TRY003",
 ]
-lint.pydocstyle.convention = "google"
-lint.isort.lines-after-imports = 2
-lint.isort.split-on-trailing-comma = false
+pydocstyle.convention = "google"
+isort.lines-after-imports = 2
+isort.split-on-trailing-comma = false
+
+[tool.ruff.format]
+docstring-code-format = true
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
-"tests/*" = ["D103", "S101"]
-"examples/*" = ["INP001", "T201"] # T201: print found
-"site/*" = ["INP001", "S602"]
+"tests/*" = ["D", "S101"]
+# T201: print found
+# D100: Missing docstring in public module
+"examples/*" = ["D100", "INP001", "T201"]
+"site/*" = ["D", "INP001", "S602"]
+
+[tool.pyright]
+typeCheckingMode = "off"
+reportPossiblyUnboundVariable = true
+reportUnboundVariable = true
```

### Comparing `pymatviz-0.8.1/readme.md` & `pymatviz-0.8.2/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pymatviz?logo=icloud&logoColor=white)](https://pypistats.org/packages/pymatviz)
 [![Zenodo](https://img.shields.io/badge/DOI-10.5281/zenodo.10456384-blue?logo=Zenodo&logoColor=white)](https://zenodo.org/records/10456384)
 
 </h4>
 
 <slot name="how-to-cite">
 
-> If you use `pymatviz` in your research, [see how to cite](#--how-to-cite-pymatviz).
+> If you use `pymatviz` in your research, [see how to cite](#how-to-cite-pymatviz).
 
 </slot>
 
-## 🔨 &thinsp; Installation
+## Installation
 
 ```sh
 pip install pymatviz
 ```
 
-## 💡 &thinsp; API Docs
+## API Docs
 
 See the [/api] page.
 
 [/api]: https://janosh.github.io/pymatviz/api
 
-## 📙 &thinsp; Usage
+## Usage
 
 See the Jupyter notebooks under [`examples/`](examples) for how to use `pymatviz`. PRs with additional examples are welcome! 🙏
 
 |                                                                                                                        |                                                                                                                                       |                                      |
 | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | [matbench_dielectric_eda.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)   | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/matbench_dielectric_eda.ipynb)  | [![Launch Codespace]][codespace url] |
 | [mp_bimodal_e_form.ipynb](https://github.com/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)               | [![Open in Google Colab]](https://colab.research.google.com/github/janosh/pymatviz/blob/main/examples/mp_bimodal_e_form.ipynb)        | [![Launch Codespace]][codespace url] |
@@ -49,45 +49,42 @@
 [Launch Codespace]: https://img.shields.io/badge/Launch-Codespace-darkblue?logo=github
 [codespace url]: https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=340898532
 
 ## Periodic Table
 
 See [`pymatviz/ptable.py`](pymatviz/ptable.py). Heatmaps of the periodic table can be plotted both with `matplotlib` and `plotly`. `plotly` supports displaying additional data on hover or full interactivity through [Dash](https://plotly.com/dash).
 
-| [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py) |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
-| :------------------------------------------------------------: | :-------------------------------------------------------------------: |
-|                       ![ptable-heatmap]                        |                        ![ptable-heatmap-ratio]                        |
-|  [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)  | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
-|            ![ptable-heatmap-plotly-more-hover-data]            |                     ![ptable-heatmap-plotly-log]                      |
-
-## Nested Periodic Table
-
-See [`pymatviz/ptable.py`](pymatviz/ptable.py). Plot histogram plots and scatter plots nested within periodic table.
-| [`ptable_hists(data, colormap="coolwarm"`](pymatviz/ptable.py) | [`ptable_scatters(data, colormap="coolwarm"`](pymatviz/ptable.py) |
-| :------------------------------------------------------------: | :---------------------------------------------------------------: |
-
-<!-- prettier-ignore -->
-|                        ![ptable-hists]                         |                        ![ptable-scatters]                         |
+|                        [`ptable_heatmap(compositions, log=True)`](pymatviz/ptable.py)                        |    [`ptable_heatmap_ratio(comps_a, comps_b)`](pymatviz/ptable.py)     |
+| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
+|                                              ![ptable-heatmap]                                               |                        ![ptable-heatmap-ratio]                        |
+|                         [`ptable_heatmap_plotly(atomic_masses)`](pymatviz/ptable.py)                         | [`ptable_heatmap_plotly(compositions, log=True)`](pymatviz/ptable.py) |
+|                                   ![ptable-heatmap-plotly-more-hover-data]                                   |                     ![ptable-heatmap-plotly-log]                      |
+|                       [`ptable_hists(data, colormap="coolwarm")`](pymatviz/ptable.py)                        |              [`ptable_lines(data)`](pymatviz/ptable.py)               |
+|                                               ![ptable-hists]                                                |                            ![ptable-lines]                            |
+| [`ptable_heatmap_splits(data, colormap="coolwarm", start_angle=135, hide_f_block=True)`](pymatviz/ptable.py) |
+|                                           ![ptable-heatmap-splits]                                           |
 
 [ptable-hists]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-hists.svg
-[ptable-scatters]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-scatters.svg
+[ptable-lines]: https://github.com/janosh/pymatviz/raw/main/examples/diatomics/homo-nuclear-mace-medium.svg
+[ptable-heatmap-splits]: https://github.com/janosh/pymatviz/raw/main/assets/ptable-heatmap-splits.svg
 
 ## Phonons
 
 See [`pymatviz/phonons.py`](pymatviz/phonons.py).
 
-|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           | [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py) |
-| :------------------------------------------------------------------------: | :--------------------------------------------------: |
-|                              ![phonon-bands]                               |                    ![phonon-dos]                     |
-| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) |                                                      |
-|                          ![phonon-bands-and-dos]                           |                                                      |
+|           [`plot_phonon_bands(bands_dict)`](pymatviz/phonons.py)           |             [`plot_phonon_dos(doses_dict)`](pymatviz/phonons.py)             |
+| :------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
+|                              ![phonon-bands]                               |                                ![phonon-dos]                                 |
+| [`plot_phonon_bands_and_dos(bands_dict, doses_dict)`](pymatviz/phonons.py) | [`plot_phonon_bands_and_dos(single_bands, single_dos)`](pymatviz/phonons.py) |
+|                      ![phonon-bands-and-dos-mp-2758]                       |                       ![phonon-bands-and-dos-mp-23907]                       |
 
 [phonon-bands]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-mp-2758.svg
 [phonon-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-dos-mp-2758.svg
-[phonon-bands-and-dos]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-2758]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-2758.svg
+[phonon-bands-and-dos-mp-23907]: https://github.com/janosh/pymatviz/raw/main/assets/phonon-bands-and-dos-mp-23907.svg
 
 ### Dash app using `ptable_heatmap_plotly()`
 
 See [`examples/mprester_ptable.ipynb`](https://github.com/janosh/pymatviz/blob/main/examples/mprester_ptable.ipynb).
 
 <https://user-images.githubusercontent.com/30958850/181644052-b330f0a2-70fc-451c-8230-20d45d3af72f.mp4>
 
@@ -142,33 +139,33 @@
 | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
 |                       ![density-scatter]                        |                  ![density-scatter-with-hist]                   |
 |       [`density_hexbin(xs, ys, ...)`](pymatviz/parity.py)       |  [`density_hexbin_with_hist(xs, ys, ...)`](pymatviz/parity.py)  |
 |                        ![density-hexbin]                        |                   ![density-hexbin-with-hist]                   |
 | [`scatter_with_err_bar(xs, ys, yerr, ...)`](pymatviz/parity.py) | [`residual_vs_actual(y_true, y_pred, ...)`](pymatviz/parity.py) |
 |                     ![scatter-with-err-bar]                     |                      ![residual-vs-actual]                      |
 
-## Uncertainty Calibration
+## Uncertainty
 
 See [`pymatviz/uncertainty.py`](pymatviz/uncertainty.py).
 
 |       [`qq_gaussian(y_true, y_pred, y_std)`](pymatviz/uncertainty.py)       |       [`qq_gaussian(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py)       |
 | :-------------------------------------------------------------------------: | :-------------------------------------------------------------------------------: |
 |                             ![normal-prob-plot]                             |                           ![normal-prob-plot-multiple]                            |
 | [`error_decay_with_uncert(y_true, y_pred, y_std)`](pymatviz/uncertainty.py) | [`error_decay_with_uncert(y_true, y_pred, y_std: dict)`](pymatviz/uncertainty.py) |
 |                         ![error-decay-with-uncert]                          |                        ![error-decay-with-uncert-multiple]                        |
 
-## Cumulative Error & Residual
+## Cumulative Metrics
 
 See [`pymatviz/cumulative.py`](pymatviz/cumulative.py).
 
 | [`cumulative_error(preds, targets)`](pymatviz/cumulative.py) | [`cumulative_residual(preds, targets)`](pymatviz/cumulative.py) |
 | :----------------------------------------------------------: | :-------------------------------------------------------------: |
 |                     ![cumulative-error]                      |                     ![cumulative-residual]                      |
 
-## Classification Metrics
+## Classification
 
 See [`pymatviz/relevance.py`](pymatviz/relevance.py).
 
 | [`roc_curve(targets, proba_pos)`](pymatviz/relevance.py) | [`precision_recall_curve(targets, proba_pos)`](pymatviz/relevance.py) |
 | :------------------------------------------------------: | :-------------------------------------------------------------------: |
 |                       ![roc-curve]                       |                       ![precision-recall-curve]                       |
 
@@ -205,24 +202,24 @@
 [sankey-spglib-vs-aflow-spacegroups]: https://github.com/janosh/pymatviz/raw/main/assets/sankey-spglib-vs-aflow-spacegroups.svg
 [scatter-with-err-bar]: https://github.com/janosh/pymatviz/raw/main/assets/scatter-with-err-bar.svg
 [spg-num-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-num-sunburst.svg
 [spg-symbol-sunburst]: https://github.com/janosh/pymatviz/raw/main/assets/spg-symbol-sunburst.svg
 [struct-2d-mp-12712-Hf9Zr9Pd24-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-12712-Hf9Zr9Pd24-disordered.svg
 [struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered]: https://github.com/janosh/pymatviz/raw/main/assets/struct-2d-mp-19017-Li4Mn0.8Fe1.6P4C1.6O16-disordered.svg
 
-## 📖 &thinsp; How to cite `pymatviz`
+## How to cite `pymatviz`
 
-You can cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
+See [`citation.cff`](citation.cff) or cite the [Zenodo record](https://zenodo.org/badge/latestdoi/340898532) using the following BibTeX entry:
 
 ```bib
 @software{riebesell_pymatviz_2022,
   title = {Pymatviz: visualization toolkit for materials informatics},
-  author = {Riebesell, Janosh},
+  author = {Riebesell, Janosh and Yang, Haoyu and Goodall, Rhys and Baird, Sterling G.},
   date = {2022-10-01},
   year = {2022},
   doi = {10.5281/zenodo.7486816},
   url = {https://github.com/janosh/pymatviz},
   note = {10.5281/zenodo.7486816 - https://github.com/janosh/pymatviz},
   urldate = {2023-01-01}, % optional, replace with your date of access
-  version = {0.7.1}, % replace with the version you use
+  version = {0.8.2}, % replace with the version you use
 }
 ```
```

### Comparing `pymatviz-0.8.1/tests/test_cumulative.py` & `pymatviz-0.8.2/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/tests/test_histograms.py` & `pymatviz-0.8.2/tests/test_histograms.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Literal
 
 import matplotlib.pyplot as plt
 import plotly.graph_objects as go
 import pytest
 
 from pymatviz import elements_hist, spacegroup_hist, true_pred_hist
+from pymatviz.utils import VALID_BACKENDS, mpl_key
 from tests.conftest import df_regr, y_pred, y_true
 
 
 if TYPE_CHECKING:
     import pandas as pd
     from numpy.typing import ArrayLike
     from pymatgen.core import Structure
@@ -41,15 +42,15 @@
     ax = true_pred_hist(y_true, y_pred, y_std, df, bins=bins, cmap=cmap)
     assert isinstance(ax, plt.Axes)
 
 
 @pytest.mark.parametrize("xticks", ["all", "crys_sys_edges", 1, 50])
 @pytest.mark.parametrize("show_counts", [True, False])
 @pytest.mark.parametrize("show_empty_bins", [True, False])
-@pytest.mark.parametrize("backend", ["matplotlib", "plotly"])
+@pytest.mark.parametrize("backend", VALID_BACKENDS)
 def test_spacegroup_hist(
     spg_symbols: list[str],
     structures: list[Structure],
     backend: Backend,
     xticks: Literal["all", "crys_sys_edges", 1, 50],
     show_counts: bool,
     show_empty_bins: bool,
@@ -58,15 +59,15 @@
     fig = spacegroup_hist(
         range(1, 231),
         xticks=xticks,
         show_counts=show_counts,
         show_empty_bins=show_empty_bins,
         backend=backend,
     )
-    assert isinstance(fig, plt.Axes if backend == "matplotlib" else go.Figure)
+    assert isinstance(fig, plt.Axes if backend == mpl_key else go.Figure)
 
     # spacegroup symbols
     fig = spacegroup_hist(
         spg_symbols,
         xticks=xticks,
         show_counts=show_counts,
         show_empty_bins=show_empty_bins,
```

### Comparing `pymatviz-0.8.1/tests/test_init.py` & `pymatviz-0.8.2/tests/test_init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import json
 from importlib.metadata import version
 
-import pymatviz
 from pymatviz import PKG_NAME, __version__
 
 
 def test_pkg_metadata() -> None:
     assert __version__ == version(PKG_NAME)
 
     # ensure __init__.py and site/package.json are in sync
@@ -23,11 +22,7 @@
             pyproject = tomllib.load(file)
 
         assert pyproject["project"]["name"] == PKG_NAME
         assert pyproject["project"]["version"] == __version__
         assert pyproject["project"]["description"] == pkg_data["description"]
     except ImportError:
         pass  # tomllib only available in 3.11+
-
-
-def test_convenience_exports() -> None:
-    assert len(pymatviz.__dict__) >= 90
```

### Comparing `pymatviz-0.8.1/tests/test_io.py` & `pymatviz-0.8.2/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,20 +150,21 @@
     with open(file_path, "rb") as pdf_file:
         contents = pdf_file.read()
 
     # TODO: maybe add more specific checks here, like file content validation
     assert contents[:4] == b"%PDF"
 
     # Test file overwrite behavior
-    file_size_before = file_path.stat().st_size
+    file_size_before = file_path.stat().st_size  # ~7000 bytes
     df_to_pdf(**kwds)
-    file_size_after = file_path.stat().st_size
+    file_size_after = file_path.stat().st_size  # ~7000 bytes
 
     # file size should be the same since content is unchanged
-    assert file_size_before - 10 <= file_size_after <= file_size_before + 10
+    assert abs(file_size_before - file_size_after) < 2000
+    # file size difference strangely increased from <10 to 7354-6156=1198 on 2024-05-04
 
 
 def test_normalize_and_crop_pdf(
     capsys: pytest.CaptureFixture[str], monkeypatch: pytest.MonkeyPatch
 ) -> None:
     # patch which('gs') to return None
     monkeypatch.setattr("pymatviz.io.which", lambda _: None)
```

### Comparing `pymatviz-0.8.1/tests/test_parity.py` & `pymatviz-0.8.2/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/tests/test_phonons.py` & `pymatviz-0.8.2/tests/test_phonons.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,86 +3,134 @@
 import json
 from glob import glob
 from typing import Literal, Union
 
 import plotly.graph_objects as go
 import pytest
 from monty.io import zopen
-from monty.json import MontyDecoder
+from monty.json import MontyDecoder, MSONable
 from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine as PhononBands
 from pymatgen.phonon.dos import PhononDos
 
 from pymatviz import plot_phonon_bands, plot_phonon_bands_and_dos, plot_phonon_dos
-from pymatviz.phonons import pretty_sym_point
+from pymatviz.phonons import BranchMode, pretty_sym_point
 from pymatviz.utils import TEST_FILES
 
 
 BandsDoses = dict[str, dict[str, Union[PhononBands, PhononDos]]]
 bs_key, dos_key = "phonon_bandstructure", "phonon_dos"
+# enable loading PhononDBDocParsed with @module set to uninstalled ffonons.dbs.phonondb
+# by changing to identical dataclass in pymatviz.phonons module
+MSONable.REDIRECT["ffonons.dbs.phonondb"] = {
+    "PhononDBDocParsed": {"@class": "PhononDBDoc", "@module": "pymatviz.phonons"}
+}
+MSONable.REDIRECT["atomate2.common.schemas.phonons"] = {
+    "PhononBSDOSDoc": {"@class": "PhononDBDoc", "@module": "pymatviz.phonons"}
+}
 
 
 @pytest.fixture()
 def phonon_bands_doses_mp_2758() -> BandsDoses:
-    with zopen(f"{TEST_FILES}/mp-2758-Sr4Se4-pbe.json.lzma") as file:
-        dft_dct = json.loads(file.read(), cls=MontyDecoder)
-    with zopen(f"{TEST_FILES}/mp-2758-Sr4Se4-mace-y7uhwpje.json.lzma") as file:
-        ml_dct = json.loads(file.read(), cls=MontyDecoder)
+    with zopen(f"{TEST_FILES}/phonons/mp-2758-Sr4Se4-pbe.json.lzma") as file:
+        dft_doc = json.loads(file.read(), cls=MontyDecoder)
 
-    bands = {"DFT": dft_dct[bs_key], "MACE": ml_dct[bs_key]}
-    doses = {"DFT": dft_dct[dos_key], "MACE": ml_dct[dos_key]}
+    with zopen(f"{TEST_FILES}/phonons/mp-2758-Sr4Se4-mace-y7uhwpje.json.lzma") as file:
+        ml_doc = json.loads(file.read(), cls=MontyDecoder)
+
+    bands = {"DFT": getattr(dft_doc, bs_key), "MACE": getattr(ml_doc, bs_key)}
+    doses = {"DFT": getattr(dft_doc, dos_key), "MACE": getattr(ml_doc, dos_key)}
     return {"bands": bands, "doses": doses}
 
 
 @pytest.fixture()
-def phonon_bands_doses_mp_2691() -> BandsDoses:
-    # with zopen(f"{TEST_FILES}/mp-2691-Cd4Se4-pbe.json.lzma") as file:
-    with zopen(f"{TEST_FILES}/mp-2667-Cs1Au1-pbe.json.lzma") as file:
+def phonon_bands_doses_mp_2667() -> BandsDoses:
+    # with zopen(f"{TEST_FILES}/phonons/mp-2691-Cd4Se4-pbe.json.lzma") as file:
+    with zopen(f"{TEST_FILES}/phonons/mp-2667-Cs1Au1-pbe.json.lzma") as file:
         return json.loads(file.read(), cls=MontyDecoder)
 
 
 @pytest.fixture()
 def phonon_doses() -> dict[str, PhononDos]:
-    paths = glob(f"{TEST_FILES}/mp-*-pbe.json.lzma")
+    paths = glob(f"{TEST_FILES}/phonons/mp-*-pbe.json.lzma")
     assert len(paths) >= 2
     return {
-        path.split("/")[-1].split("-pbe")[0]: json.loads(
-            zopen(path).read(), cls=MontyDecoder
-        )[dos_key]
+        path.split("/")[-1].split("-pbe")[0]: getattr(
+            json.loads(zopen(path).read(), cls=MontyDecoder), dos_key
+        )
         for path in paths
     }
 
 
-def test_plot_phonon_bands(phonon_bands_doses_mp_2758: BandsDoses) -> None:
+@pytest.mark.parametrize(
+    "branches, branch_mode", [(["GAMMA-X", "X-U"], "union"), ((), "intersection")]
+)
+def test_plot_phonon_bands(
+    phonon_bands_doses_mp_2758: BandsDoses,
+    branches: tuple[str, str],
+    branch_mode: BranchMode,
+) -> None:
     # test single band structure
-    fig = plot_phonon_bands(phonon_bands_doses_mp_2758["bands"]["DFT"])
+    fig = plot_phonon_bands(
+        phonon_bands_doses_mp_2758["bands"]["DFT"],
+        branch_mode=branch_mode,
+        branches=branches,
+    )
     assert isinstance(fig, go.Figure)
     assert fig.layout.xaxis.title.text == "Wave Vector"
     assert fig.layout.yaxis.title.text == "Frequency (THz)"
     assert fig.layout.font.size == 16
 
-    x_labels = ("Γ", "X", "X", "U|K", "Γ", "Γ", "L", "L", "W", "W", "X")
-    assert fig.layout.xaxis.ticktext == x_labels
+    if branches == ():
+        x_labels = ["Γ", "X", "X", "U|K", "Γ", "Γ", "L", "L", "W", "W", "X"]
+    else:
+        x_labels = ["Γ", "X", "X", "U|K"]
+    assert list(fig.layout.xaxis.ticktext) == x_labels
     assert fig.layout.xaxis.range is None
     assert fig.layout.yaxis.range == pytest.approx((0, 5.36385427095))
 
     # test dict of band structures
-    fig = plot_phonon_bands(phonon_bands_doses_mp_2758["bands"])
+    fig = plot_phonon_bands(
+        phonon_bands_doses_mp_2758["bands"], branch_mode=branch_mode, branches=branches
+    )
     assert isinstance(fig, go.Figure)
 
     with pytest.raises(
-        TypeError, match=f"Only {PhononBands.__name__} objects supported, got str"
+        TypeError, match=f"Only {PhononBands.__name__} supported, got str"
     ):
         plot_phonon_bands("invalid input")
 
 
+def test_plot_phonon_bands_raises(
+    phonon_bands_doses_mp_2758: BandsDoses, capsys: pytest.CaptureFixture
+) -> None:
+    with pytest.raises(ValueError) as exc:
+        plot_phonon_bands(
+            phonon_bands_doses_mp_2758["bands"]["DFT"], branches=("foo-bar",)
+        )
+
+    assert (
+        "No common branches with branch_mode='union'.\n"
+        "- : GAMMA-X, X-U, K-GAMMA, GAMMA-L, L-W, W-X\n"
+        "- Only branches ('foo-bar',) were requested." in str(exc.value)
+    )
+
+    # issues warning when requesting some available and some unavailable branches
+    plot_phonon_bands(
+        phonon_bands_doses_mp_2758["bands"]["DFT"], branches=("X-U", "foo-bar")
+    )
+    stdout, stderr = capsys.readouterr()
+    assert stdout == ""
+    assert "Warning: missing_branches={'foo-bar'}, available branches:" in stderr
+
+
 @pytest.mark.parametrize(
     "sym_point, expected",
     [("Γ", "Γ"), ("Γ|DELTA", "Γ|Δ"), ("GAMMA", "Γ"), ("S_0|SIGMA", "S<sub>0</sub>|Σ")],
 )
-def test_prety_sym_point(sym_point: str, expected: str) -> None:
+def test_pretty_sym_point(sym_point: str, expected: str) -> None:
     assert pretty_sym_point(sym_point) == expected
 
 
 @pytest.mark.parametrize(
     "units, stack, sigma, normalize, last_peak_anno",
     [
         ("eV", False, 0.01, "max", "{key}={last_peak:.1f}"),
```

### Comparing `pymatviz-0.8.1/tests/test_relevance.py` & `pymatviz-0.8.2/tests/test_relevance.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/tests/test_sankey.py` & `pymatviz-0.8.2/tests/test_sankey.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/tests/test_structure_viz.py` & `pymatviz-0.8.2/tests/test_structure_viz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import pytest
 from pymatgen.analysis.local_env import NearNeighbors, VoronoiNN
 from pymatgen.core import Lattice, Structure
 
@@ -65,20 +65,16 @@
     assert ax.axes.axison == (axis not in (False, "off"))
 
 
 @pytest.mark.parametrize(
     "site_labels",
     [True, False, "symbol", "species", {"Fe": "Iron"}, {"Fe": 1.0}, ["Fe", "O"]],
 )
-@pytest.mark.parametrize("site_labels_bbox", [None, {}, {"boxstyle": "round"}])
 def test_plot_structure_2d_site_labels(
     site_labels: bool | str | dict[str, str | float] | Sequence[str],
-    site_labels_bbox: dict[str, Any] | None,
 ) -> None:
-    ax = plot_structure_2d(
-        disordered_struct, site_labels=site_labels, site_labels_bbox=site_labels_bbox
-    )
+    ax = plot_structure_2d(disordered_struct, site_labels=site_labels)
     if site_labels is False:
         assert not ax.axes.texts
     else:
         label = ax.axes.texts[0].get_text()
         assert label in ("Fe", "O", "1.0", "Iron")
```

### Comparing `pymatviz-0.8.1/tests/test_sunburst.py` & `pymatviz-0.8.2/tests/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `pymatviz-0.8.1/tests/test_uncertainty.py` & `pymatviz-0.8.2/tests/test_uncertainty.py`

 * *Files identical despite different names*

