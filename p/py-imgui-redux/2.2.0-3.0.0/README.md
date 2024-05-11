# Comparing `tmp/py_imgui_redux-2.2.0.tar.gz` & `tmp/py_imgui_redux-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_imgui_redux-2.2.0.tar", last modified: Tue Apr 16 03:03:36 2024, max compression
+gzip compressed data, was "py_imgui_redux-3.0.0.tar", last modified: Sat May 11 21:54:25 2024, max compression
```

## Comparing `py_imgui_redux-2.2.0.tar` & `py_imgui_redux-3.0.0.tar`

### file list

```diff
@@ -1,315 +1,434 @@
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.105074 py_imgui_redux-2.2.0/
--rw-r--r--   0 alagyn    (1000) users      (100)      610 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) users      (100)     1070 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/LICENSE
--rw-r--r--   0 alagyn    (1000) users      (100)      280 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) users      (100)     7436 2024-04-16 03:03:36.105074 py_imgui_redux-2.2.0/PKG-INFO
--rw-r--r--   0 alagyn    (1000) users      (100)     6672 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/README.md
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.088074 py_imgui_redux-2.2.0/build/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.104074 py_imgui_redux-2.2.0/build/py_imgui_redux.egg-info/
--rw-r--r--   0 alagyn    (1000) users      (100)    10713 2024-04-16 03:03:36.000000 py_imgui_redux-2.2.0/build/py_imgui_redux.egg-info/SOURCES.txt
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.090074 py_imgui_redux-2.2.0/cmake/
--rw-r--r--   0 alagyn    (1000) users      (100)     1607 2024-04-16 01:53:16.000000 py_imgui_redux-2.2.0/cmake/Findpyglad.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)     1536 2024-04-16 02:05:56.000000 py_imgui_redux-2.2.0/cmake/Findpyglfw.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)     1950 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/cmake/imgui-srcs.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)      978 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/cmake/setupPyBindLib.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)    44462 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/pybind11_stubgen.py
--rw-r--r--   0 alagyn    (1000) users      (100)    13158 2024-04-16 00:32:18.000000 py_imgui_redux-2.2.0/pyproject.toml
--rw-r--r--   0 alagyn    (1000) users      (100)       38 2024-04-16 03:03:36.105074 py_imgui_redux-2.2.0/setup.cfg
--rw-r--r--   0 alagyn    (1000) users      (100)    10373 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/setup.py
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.089074 py_imgui_redux-2.2.0/source/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.088074 py_imgui_redux-2.2.0/source/inc/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.088074 py_imgui_redux-2.2.0/source/inc/bind-imgui/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.090074 py_imgui_redux-2.2.0/source/inc/bind-imgui/imgui-core/
--rw-r--r--   0 alagyn    (1000) users      (100)      849 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/bind-imgui/imgui-core/imgui-modules.h
--rw-r--r--   0 alagyn    (1000) users      (100)      244 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/bind-imgui/imgui-core/texture.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.090074 py_imgui_redux-2.2.0/source/inc/bind-imgui/imnodes/
--rw-r--r--   0 alagyn    (1000) users      (100)      365 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/bind-imgui/imnodes/imnodes-modules.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.090074 py_imgui_redux-2.2.0/source/inc/bind-imgui/implot/
--rw-r--r--   0 alagyn    (1000) users      (100)      428 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/bind-imgui/implot/implot-modules.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/inc/binder/
--rw-r--r--   0 alagyn    (1000) users      (100)      117 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/bind-modules.h
--rw-r--r--   0 alagyn    (1000) users      (100)      798 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/enum-utility.h
--rw-r--r--   0 alagyn    (1000) users      (100)     1076 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/list-wrapper.h
--rw-r--r--   0 alagyn    (1000) users      (100)      200 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/module-utility.h
--rw-r--r--   0 alagyn    (1000) users      (100)      149 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/numpy.h
--rw-r--r--   0 alagyn    (1000) users      (100)      233 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/struct-utility.h
--rw-r--r--   0 alagyn    (1000) users      (100)     1980 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/inc/binder/wraps.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/src/
--rw-r--r--   0 alagyn    (1000) users      (100)      424 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/bind-imgui.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/src/binder/
--rw-r--r--   0 alagyn    (1000) users      (100)     1024 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/binder/enum-utility.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     4210 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/binder/wraps.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/src/imgui-core/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/src/imgui-core/bind-backends/
--rw-r--r--   0 alagyn    (1000) users      (100)     5771 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/bind-backends/glfw.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      721 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/bind-backends/opengl3.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      914 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/bind-imgui-core.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.091074 py_imgui_redux-2.2.0/source/src/imgui-core/modules/
--rw-r--r--   0 alagyn    (1000) users      (100)      902 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/cursor-layout.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1749 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/demos.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     9868 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/drawlist.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     4310 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/im-windows.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      744 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-context.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    26732 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-enums.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    15233 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-structs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2036 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/stacks.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      833 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/styles.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/
--rw-r--r--   0 alagyn    (1000) users      (100)     2291 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/colors.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     8021 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/drag-inputs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3727 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/images.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     5568 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/input.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    11667 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/main.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     6398 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/slide-inputs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1187 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tables.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      723 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tabs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1590 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/text.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1474 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tree.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/source/src/imnodes/
--rw-r--r--   0 alagyn    (1000) users      (100)      269 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imnodes/bind-imnodes.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/source/src/imnodes/modules/
--rw-r--r--   0 alagyn    (1000) users      (100)     8493 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-context.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3373 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-enums.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3062 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-structs.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/source/src/implot/
--rw-r--r--   0 alagyn    (1000) users      (100)      474 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/bind-implot.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/source/src/implot/modules/
--rw-r--r--   0 alagyn    (1000) users      (100)     2166 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-colormap.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      892 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-context.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    10156 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-enums.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1627 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-misc.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    17093 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-plotting.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3880 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-setup-funcs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3602 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-structs.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3225 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-tools.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     4508 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/source/src/implot/modules/implot-utils.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/third-party/
--rw-r--r--   0 alagyn    (1000) users      (100)     1212 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/third-party/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.092074 py_imgui_redux-2.2.0/third-party/imconfig/
--rw-r--r--   0 alagyn    (1000) users      (100)     9664 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/third-party/imconfig/bind-imconfig.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.094074 py_imgui_redux-2.2.0/third-party/imgui/
--rw-r--r--   0 alagyn    (1000) users      (100)     1063 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.editorconfig
--rw-r--r--   0 alagyn    (1000) users      (100)       45 2024-04-16 00:36:50.000000 py_imgui_redux-2.2.0/third-party/imgui/.git
--rw-r--r--   0 alagyn    (1000) users      (100)      397 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.095074 py_imgui_redux-2.2.0/third-party/imgui/.github/
--rw-r--r--   0 alagyn    (1000) users      (100)       59 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/FUNDING.yml
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.095074 py_imgui_redux-2.2.0/third-party/imgui/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 alagyn    (1000) users      (100)       28 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 alagyn    (1000) users      (100)     5065 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/ISSUE_TEMPLATE/issue_template.yml
--rw-r--r--   0 alagyn    (1000) users      (100)      233 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/pull_request_template.md
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.095074 py_imgui_redux-2.2.0/third-party/imgui/.github/workflows/
--rw-r--r--   0 alagyn    (1000) users      (100)    21144 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) users      (100)      312 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/workflows/scheduled.yml
--rw-r--r--   0 alagyn    (1000) users      (100)     1826 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.github/workflows/static-analysis.yml
--rw-r--r--   0 alagyn    (1000) users      (100)     1173 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/.gitignore
--rw-r--r--   0 alagyn    (1000) users      (100)     1083 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/LICENSE.txt
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.097074 py_imgui_redux-2.2.0/third-party/imgui/backends/
--rw-r--r--   0 alagyn    (1000) users      (100)    29589 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_allegro5.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2188 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_allegro5.h
--rw-r--r--   0 alagyn    (1000) users      (100)    16189 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_android.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2153 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_android.h
--rw-r--r--   0 alagyn    (1000) users      (100)    27386 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx10.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1473 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx10.h
--rw-r--r--   0 alagyn    (1000) users      (100)    29334 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx11.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1538 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx11.h
--rw-r--r--   0 alagyn    (1000) users      (100)    35510 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx12.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2544 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx12.h
--rw-r--r--   0 alagyn    (1000) users      (100)    18488 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx9.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1467 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx9.h
--rw-r--r--   0 alagyn    (1000) users      (100)    46787 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glfw.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     4012 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glfw.h
--rw-r--r--   0 alagyn    (1000) users      (100)    14229 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glut.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3123 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glut.h
--rw-r--r--   0 alagyn    (1000) users      (100)     3318 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_metal.h
--rw-r--r--   0 alagyn    (1000) users      (100)    27587 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_metal.mm
--rw-r--r--   0 alagyn    (1000) users      (100)    15484 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl2.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2162 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl2.h
--rw-r--r--   0 alagyn    (1000) users      (100)    47025 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3402 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3.h
--rw-r--r--   0 alagyn    (1000) users      (100)    36341 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3_loader.h
--rw-r--r--   0 alagyn    (1000) users      (100)     2399 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_osx.h
--rw-r--r--   0 alagyn    (1000) users      (100)    35849 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_osx.mm
--rw-r--r--   0 alagyn    (1000) users      (100)    36305 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl2.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2578 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl2.h
--rw-r--r--   0 alagyn    (1000) users      (100)    29721 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl3.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     2583 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl3.h
--rw-r--r--   0 alagyn    (1000) users      (100)    11797 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1979 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.h
--rw-r--r--   0 alagyn    (1000) users      (100)    11301 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1987 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.h
--rw-r--r--   0 alagyn    (1000) users      (100)    82654 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_vulkan.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    10282 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_vulkan.h
--rw-r--r--   0 alagyn    (1000) users      (100)    32620 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_wgpu.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1693 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_wgpu.h
--rw-r--r--   0 alagyn    (1000) users      (100)    46165 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_win32.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3433 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_win32.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.097074 py_imgui_redux-2.2.0/third-party/imgui/backends/vulkan/
--rwxr-xr-x   0 alagyn    (1000) users      (100)      254 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/vulkan/generate_spv.sh
--rw-r--r--   0 alagyn    (1000) users      (100)      249 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/vulkan/glsl_shader.frag
--rw-r--r--   0 alagyn    (1000) users      (100)      454 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/backends/vulkan/glsl_shader.vert
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.097074 py_imgui_redux-2.2.0/third-party/imgui/docs/
--rw-r--r--   0 alagyn    (1000) users      (100)     8898 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/BACKENDS.md
--rw-r--r--   0 alagyn    (1000) users      (100)   438005 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/CHANGELOG.txt
--rw-r--r--   0 alagyn    (1000) users      (100)    10123 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/CONTRIBUTING.md
--rw-r--r--   0 alagyn    (1000) users      (100)    12912 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/EXAMPLES.md
--rw-r--r--   0 alagyn    (1000) users      (100)    45061 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/FAQ.md
--rw-r--r--   0 alagyn    (1000) users      (100)    24285 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/FONTS.md
--rw-r--r--   0 alagyn    (1000) users      (100)    20306 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/README.md
--rw-r--r--   0 alagyn    (1000) users      (100)    33130 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/docs/TODO.txt
--rw-r--r--   0 alagyn    (1000) users      (100)    10507 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imconfig.h
--rw-r--r--   0 alagyn    (1000) users      (100)   791356 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)   327986 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui.h
--rw-r--r--   0 alagyn    (1000) users      (100)   436764 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui_demo.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)   221094 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui_draw.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)   258269 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui_internal.h
--rw-r--r--   0 alagyn    (1000) users      (100)   236180 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui_tables.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)   441238 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imgui_widgets.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    20344 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imstb_rectpack.h
--rw-r--r--   0 alagyn    (1000) users      (100)    55207 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imstb_textedit.h
--rw-r--r--   0 alagyn    (1000) users      (100)   199484 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/imstb_truetype.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.097074 py_imgui_redux-2.2.0/third-party/imgui/misc/
--rw-r--r--   0 alagyn    (1000) users      (100)      998 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/README.txt
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.098074 py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/
--rw-r--r--   0 alagyn    (1000) users      (100)      586 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/README.txt
--rw-r--r--   0 alagyn    (1000) users      (100)     3357 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/imgui_stdlib.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     1172 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/imgui_stdlib.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.098074 py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/
--rw-r--r--   0 alagyn    (1000) users      (100)      487 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/README.txt
--rw-r--r--   0 alagyn    (1000) users      (100)      555 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.gdb
--rw-r--r--   0 alagyn    (1000) users      (100)     1419 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.natstepfilter
--rw-r--r--   0 alagyn    (1000) users      (100)     1917 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.natvis
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.098074 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/
--rw-r--r--   0 alagyn    (1000) users      (100)    43912 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Cousine-Regular.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)   190044 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/DroidSans.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)    16848 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Karla-Regular.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)    41208 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/ProggyClean.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)    35656 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/ProggyTiny.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)   162588 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Roboto-Medium.ttf
--rw-r--r--   0 alagyn    (1000) users      (100)    13792 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.098074 py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/
--rw-r--r--   0 alagyn    (1000) users      (100)     2502 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/README.md
--rw-r--r--   0 alagyn    (1000) users      (100)    46376 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/imgui_freetype.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3599 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/imgui_freetype.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.098074 py_imgui_redux-2.2.0/third-party/imgui/misc/single_file/
--rw-r--r--   0 alagyn    (1000) users      (100)      994 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imgui/misc/single_file/imgui_single_file.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.099074 py_imgui_redux-2.2.0/third-party/imnodes/
--rw-r--r--   0 alagyn    (1000) users      (100)     1022 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/.clang-format
--rw-r--r--   0 alagyn    (1000) users      (100)     1400 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/.clang-tidy
--rw-r--r--   0 alagyn    (1000) users      (100)       47 2024-04-16 00:36:51.000000 py_imgui_redux-2.2.0/third-party/imnodes/.git
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.089074 py_imgui_redux-2.2.0/third-party/imnodes/.github/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.099074 py_imgui_redux-2.2.0/third-party/imnodes/.github/workflows/
--rw-r--r--   0 alagyn    (1000) users      (100)      699 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/.github/workflows/build.yaml
--rw-r--r--   0 alagyn    (1000) users      (100)     9001 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/.gitignore
--rw-r--r--   0 alagyn    (1000) users      (100)       80 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/.gitmodules
--rw-r--r--   0 alagyn    (1000) users      (100)     2180 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) users      (100)     1072 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/LICENSE.md
--rw-r--r--   0 alagyn    (1000) users      (100)     9463 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/README.md
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.099074 py_imgui_redux-2.2.0/third-party/imnodes/example/
--rw-r--r--   0 alagyn    (1000) users      (100)    24843 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/color_node_editor.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     9464 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/graph.h
--rw-r--r--   0 alagyn    (1000) users      (100)      977 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/hello.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     4164 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/main.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)     3595 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/multi_editor.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)      135 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/node_editor.h
--rw-r--r--   0 alagyn    (1000) users      (100)     5865 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/example/save_load.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.099074 py_imgui_redux-2.2.0/third-party/imnodes/img/
--rw-r--r--   0 alagyn    (1000) users      (100)  1517285 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/img/imnodes.gif
--rw-r--r--   0 alagyn    (1000) users      (100)   114226 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/imnodes.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    18234 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/imnodes.h
--rw-r--r--   0 alagyn    (1000) users      (100)    12852 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/imnodes_internal.h
--rw-r--r--   0 alagyn    (1000) users      (100)      213 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/imnodes/vcpkg.json
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.101074 py_imgui_redux-2.2.0/third-party/implot/
--rw-r--r--   0 alagyn    (1000) users      (100)       46 2024-04-16 00:36:51.000000 py_imgui_redux-2.2.0/third-party/implot/.git
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.101074 py_imgui_redux-2.2.0/third-party/implot/.github/
--rw-r--r--   0 alagyn    (1000) users      (100)     3117 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/.github/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) users      (100)     1480 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/.github/example_implot.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.101074 py_imgui_redux-2.2.0/third-party/implot/.github/workflows/
--rw-r--r--   0 alagyn    (1000) users      (100)     3317 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) users      (100)     1068 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/LICENSE
--rw-r--r--   0 alagyn    (1000) users      (100)    12224 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/README.md
--rw-r--r--   0 alagyn    (1000) users      (100)     3591 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/TODO.md
--rw-r--r--   0 alagyn    (1000) users      (100)   273673 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/implot.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    79742 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/implot.h
--rw-r--r--   0 alagyn    (1000) users      (100)   114100 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/implot_demo.cpp
--rw-r--r--   0 alagyn    (1000) users      (100)    67521 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/implot_internal.h
--rw-r--r--   0 alagyn    (1000) users      (100)   123095 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/implot/implot_items.cpp
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.102074 py_imgui_redux-2.2.0/third-party/pybind11/
--rw-r--r--   0 alagyn    (1000) users      (100)     1271 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.appveyor.yml
--rw-r--r--   0 alagyn    (1000) users      (100)      996 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.clang-format
--rw-r--r--   0 alagyn    (1000) users      (100)     2605 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.clang-tidy
--rw-r--r--   0 alagyn    (1000) users      (100)     2196 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.cmake-format.yaml
--rw-r--r--   0 alagyn    (1000) users      (100)     1308 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.codespell-ignore-lines
--rw-r--r--   0 alagyn    (1000) users      (100)       48 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.git
--rw-r--r--   0 alagyn    (1000) users      (100)       18 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.gitattributes
--rw-r--r--   0 alagyn    (1000) users      (100)      502 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.gitignore
--rw-r--r--   0 alagyn    (1000) users      (100)     4332 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 alagyn    (1000) users      (100)       62 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/.readthedocs.yml
--rw-r--r--   0 alagyn    (1000) users      (100)    11983 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) users      (100)     1684 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/LICENSE
--rw-r--r--   0 alagyn    (1000) users      (100)      223 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) users      (100)     7686 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/README.rst
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.089074 py_imgui_redux-2.2.0/third-party/pybind11/include/
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.103074 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/
--rw-r--r--   0 alagyn    (1000) users      (100)    23959 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 alagyn    (1000) users      (100)     7069 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 alagyn    (1000) users      (100)    65660 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 alagyn    (1000) users      (100)     8458 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 alagyn    (1000) users      (100)      120 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/common.h
--rw-r--r--   0 alagyn    (1000) users      (100)     2096 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.103074 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/
--rw-r--r--   0 alagyn    (1000) users      (100)    28251 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 alagyn    (1000) users      (100)    52929 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 alagyn    (1000) users      (100)     5491 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 alagyn    (1000) users      (100)    17869 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 alagyn    (1000) users      (100)    26305 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 alagyn    (1000) users      (100)    42613 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 alagyn    (1000) users      (100)     1625 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.103074 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen/
--rw-r--r--   0 alagyn    (1000) users      (100)    31418 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 alagyn    (1000) users      (100)    18108 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 alagyn    (1000) users      (100)      316 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 alagyn    (1000) users      (100)    13471 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 alagyn    (1000) users      (100)     4731 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 alagyn    (1000) users      (100)     5002 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 alagyn    (1000) users      (100)     8262 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/gil.h
--rw-r--r--   0 alagyn    (1000) users      (100)     8862 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 alagyn    (1000) users      (100)    79408 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 alagyn    (1000) users      (100)     9103 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 alagyn    (1000) users      (100)     2734 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/options.h
--rw-r--r--   0 alagyn    (1000) users      (100)   126420 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 alagyn    (1000) users      (100)    94641 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.103074 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl/
--rw-r--r--   0 alagyn    (1000) users      (100)     4185 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 alagyn    (1000) users      (100)    15337 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 alagyn    (1000) users      (100)    29747 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 alagyn    (1000) users      (100)     2765 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/noxfile.py
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.103074 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/
--rw-r--r--   0 alagyn    (1000) users      (100)      414 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/__init__.py
--rw-r--r--   0 alagyn    (1000) users      (100)     1360 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/__main__.py
--rw-r--r--   0 alagyn    (1000) users      (100)      228 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/_version.py
--rw-r--r--   0 alagyn    (1000) users      (100)     1226 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/commands.py
--rw-r--r--   0 alagyn    (1000) users      (100)        0 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/py.typed
--rw-r--r--   0 alagyn    (1000) users      (100)    17609 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 alagyn    (1000) users      (100)     1261 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/pyproject.toml
--rw-r--r--   0 alagyn    (1000) users      (100)     1618 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/setup.cfg
--rw-r--r--   0 alagyn    (1000) users      (100)     4877 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/setup.py
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.104074 py_imgui_redux-2.2.0/third-party/pybind11/tools/
--rw-r--r--   0 alagyn    (1000) users      (100)     2350 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)     3105 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)    11190 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)      817 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 alagyn    (1000) users      (100)     1423 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/check-style.sh
--rw-r--r--   0 alagyn    (1000) users      (100)      952 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 alagyn    (1000) users      (100)     1040 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 alagyn    (1000) users      (100)     1031 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/libsize.py
--rwxr-xr-x   0 alagyn    (1000) users      (100)     1311 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/make_changelog.py
--rw-r--r--   0 alagyn    (1000) users      (100)      196 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 alagyn    (1000) users      (100)    14033 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)     6930 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 alagyn    (1000) users      (100)     8960 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)     8361 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 alagyn    (1000) users      (100)       94 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/pyproject.toml
--rw-r--r--   0 alagyn    (1000) users      (100)     2104 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 alagyn    (1000) users      (100)     1234 2024-04-16 00:36:53.000000 py_imgui_redux-2.2.0/third-party/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 alagyn    (1000) users      (100)        0 2024-04-16 03:03:36.104074 py_imgui_redux-2.2.0/third-party/stb/
--rw-r--r--   0 alagyn    (1000) users      (100)   282848 2024-04-15 22:56:06.000000 py_imgui_redux-2.2.0/third-party/stb/stb_image.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2900 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1070 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      259 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7787 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7059 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.167697 py_imgui_redux-3.0.0/build/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/build/py_imgui_redux.egg-info/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14741 2024-05-11 21:54:25.000000 py_imgui_redux-3.0.0/build/py_imgui_redux.egg-info/SOURCES.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.169697 py_imgui_redux-3.0.0/cmake/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      978 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/cmake/setupPyBindLib.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44479 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/pybind11_stubgen.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      850 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/setup.cfg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10460 2024-05-11 16:10:04.000000 py_imgui_redux-3.0.0/setup.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.167697 py_imgui_redux-3.0.0/source/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.167697 py_imgui_redux-3.0.0/source/inc/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.169697 py_imgui_redux-3.0.0/source/inc/bind-imgui/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      688 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/bind-imgui/glfw-modules.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1242 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/bind-imgui/imgui-modules.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      482 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/bind-imgui/imnodes-modules.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      647 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/bind-imgui/implot-modules.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      244 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/bind-imgui/texture.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/inc/binder/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      298 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/inc/binder/bind-modules.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      798 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/inc/binder/enum-utility.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1076 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/inc/binder/list-wrapper.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      149 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/inc/binder/numpy.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      233 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/inc/binder/struct-utility.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1980 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/inc/binder/wraps.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/src/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      513 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/bind-imgui.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/src/binder/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1024 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/src/binder/enum-utility.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4210 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/source/src/binder/wraps.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/src/glfw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      345 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/bind-glfw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5800 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/callbacks.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7632 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/constants.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1471 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/context.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1750 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/input.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1688 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/joystick.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2458 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/monitors.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2221 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/structs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4302 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/glfw/windows.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/src/imgui-core/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.170697 py_imgui_redux-3.0.0/source/src/imgui-core/bind-backends/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5760 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/bind-backends/glfw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      710 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/bind-backends/opengl3.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      903 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/bind-imgui-core.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.171697 py_imgui_redux-3.0.0/source/src/imgui-core/modules/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      891 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/cursor-layout.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1738 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/demos.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9846 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/drawlist.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4299 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/im-windows.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      733 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-context.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26721 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-enums.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15222 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-structs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2025 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/stacks.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      822 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/styles.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.171697 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2280 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/colors.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8010 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/drag-inputs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3705 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/images.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5557 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/input.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11645 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/main.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6387 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/slide-inputs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1176 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tables.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      712 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tabs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1579 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/text.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1463 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tree.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.171697 py_imgui_redux-3.0.0/source/src/imnodes/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      261 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imnodes/bind-imnodes.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.171697 py_imgui_redux-3.0.0/source/src/imnodes/modules/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8485 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-context.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3365 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-enums.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3054 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-structs.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.171697 py_imgui_redux-3.0.0/source/src/implot/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      467 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/bind-implot.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.172697 py_imgui_redux-3.0.0/source/src/implot/modules/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2159 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-colormap.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      885 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-context.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10149 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-enums.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1620 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-misc.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17075 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-plotting.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3873 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-setup-funcs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3595 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-structs.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3218 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-tools.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4501 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/source/src/implot/modules/implot-utils.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.172697 py_imgui_redux-3.0.0/third-party/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1777 2024-05-11 21:45:05.000000 py_imgui_redux-3.0.0/third-party/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.168697 py_imgui_redux-3.0.0/third-party/glad/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.168697 py_imgui_redux-3.0.0/third-party/glad/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.172697 py_imgui_redux-3.0.0/third-party/glad/include/KHR/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11131 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/third-party/glad/include/KHR/khrplatform.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.172697 py_imgui_redux-3.0.0/third-party/glad/include/glad/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   299906 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/third-party/glad/include/glad/gl.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.172697 py_imgui_redux-3.0.0/third-party/glad/src/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   163913 2024-05-11 15:12:28.000000 py_imgui_redux-3.0.0/third-party/glad/src/gl.c
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.173697 py_imgui_redux-3.0.0/third-party/glfw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1196 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1275 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/.editorconfig
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       44 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      142 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/.gitattributes
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1449 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/.mailmap
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.173697 py_imgui_redux-3.0.0/third-party/glfw/CMake/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1653 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/GenerateMappings.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/Info.plist.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1117 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/cmake_uninstall.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      440 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/glfw3.pc.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      115 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/glfw3Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      596 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      588 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/i686-w64-mingw32.cmake
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.173697 py_imgui_redux-3.0.0/third-party/glfw/CMake/modules/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      747 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/modules/FindEpollShim.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      445 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/modules/FindOSMesa.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      606 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      598 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/CMake/x86_64-w64-mingw32.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5951 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5328 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/CONTRIBUTORS.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      904 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/LICENSE.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25748 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.174697 py_imgui_redux-3.0.0/third-party/glfw/deps/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/getopt.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2136 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/getopt.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.175697 py_imgui_redux-3.0.0/third-party/glfw/deps/glad/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   326437 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/glad/gl.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81113 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/glad/gles2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   336197 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/glad/vulkan.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14123 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/linmath.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.175697 py_imgui_redux-3.0.0/third-party/glfw/deps/mingw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3111 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/mingw/_mingw_dxhelper.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   112560 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/mingw/dinput.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7950 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/mingw/xinput.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   990698 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/nuklear.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14081 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/nuklear_glfw_gl2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    71221 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/stb_image_write.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13065 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/tinycthread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15660 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/tinycthread.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.175697 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4636 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/fractional-scale-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4017 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/idle-inhibit-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15451 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/pointer-constraints-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6584 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/relative-pointer-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8232 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/viewporter.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   144896 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/wayland.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9016 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/xdg-activation-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7089 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/xdg-decoration-unstable-v1.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    60418 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/deps/wayland/xdg-shell.xml
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.176697 py_imgui_redux-3.0.0/third-party/glfw/examples/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3774 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19484 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/boing.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9945 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/gears.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27988 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/glfw.icns
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21630 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/glfw.ico
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       53 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/glfw.rc
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16086 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/heightmap.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4854 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/offscreen.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35989 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/particles.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7146 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/sharing.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15210 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/splitview.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5131 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/triangle-opengl.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5264 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/triangle-opengles.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11894 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/wave.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3157 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/examples/windows.c
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.168697 py_imgui_redux-3.0.0/third-party/glfw/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.176697 py_imgui_redux-3.0.0/third-party/glfw/include/GLFW/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   241826 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/include/GLFW/glfw3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21201 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/include/GLFW/glfw3native.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.180697 py_imgui_redux-3.0.0/third-party/glfw/src/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13945 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24776 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_init.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1849 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15740 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_joystick.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19638 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_monitor.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12920 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1890 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1378 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_time.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    60250 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/cocoa_window.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25670 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29593 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/egl_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      771 2024-05-09 02:50:54.000000 py_imgui_redux-3.0.0/third-party/glfw/src/glfw.rc.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23690 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/glx_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14504 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41395 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/input.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35817 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12404 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/linux_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2322 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/linux_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   256981 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/mappings.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5280 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/mappings.h.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15194 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11919 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/nsgl_context.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14437 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1753 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1424 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5178 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11827 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18608 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/null_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11935 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/osmesa_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6566 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/platform.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6421 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1816 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_module.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3044 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_poll.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1292 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_poll.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3245 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_thread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1674 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_thread.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2206 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1489 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/posix_time.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11947 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/vulkan.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27071 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/wgl_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28467 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26711 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1870 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1822 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_module.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16993 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25101 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3085 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_thread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1956 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_thread.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1911 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1703 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_time.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81112 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/win32_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35148 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    45024 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/wl_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8627 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/wl_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    34576 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/wl_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   102422 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/wl_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    70476 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/x11_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20136 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/x11_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44741 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/x11_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   106290 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/x11_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22943 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/xkb_unicode.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1288 2024-05-09 02:51:32.000000 py_imgui_redux-3.0.0/third-party/glfw/src/xkb_unicode.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.180697 py_imgui_redux-3.0.0/third-party/imconfig/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9664 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/third-party/imconfig/bind-imconfig.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.182697 py_imgui_redux-3.0.0/third-party/imgui/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1063 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/.editorconfig
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       45 2024-05-09 00:10:00.000000 py_imgui_redux-3.0.0/third-party/imgui/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      397 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/.gitattributes
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1173 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1083 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/LICENSE.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.184697 py_imgui_redux-3.0.0/third-party/imgui/backends/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29589 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_allegro5.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2188 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_allegro5.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16189 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_android.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2153 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_android.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27386 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx10.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1473 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx10.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29334 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx11.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1538 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx11.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35510 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx12.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2544 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx12.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18488 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx9.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1467 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx9.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    46787 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glfw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4012 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glfw.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14229 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glut.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3123 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glut.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3318 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_metal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27587 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_metal.mm
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15484 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl2.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2162 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47025 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3402 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    36341 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3_loader.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2399 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_osx.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35849 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_osx.mm
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    36305 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl2.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2578 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29721 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl3.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2583 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11797 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1979 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11301 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1987 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    82654 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_vulkan.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10282 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_vulkan.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32620 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_wgpu.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1693 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_wgpu.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    46165 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_win32.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3433 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_win32.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.184697 py_imgui_redux-3.0.0/third-party/imgui/backends/vulkan/
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)      254 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/vulkan/generate_spv.sh
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      249 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/vulkan/glsl_shader.frag
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      454 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/backends/vulkan/glsl_shader.vert
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10507 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imconfig.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   791356 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   327986 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   436764 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui_demo.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   221094 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui_draw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   258269 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   236180 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui_tables.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   441238 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/imgui_widgets.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20344 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/imstb_rectpack.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    55207 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/imstb_textedit.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   199484 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/imstb_truetype.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.184697 py_imgui_redux-3.0.0/third-party/imgui/misc/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      998 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/README.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.184697 py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      586 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/README.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3357 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/imgui_stdlib.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1172 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/imgui_stdlib.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.184697 py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      487 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/README.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.gdb
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1419 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.natstepfilter
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1917 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.natvis
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.186697 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    43912 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Cousine-Regular.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   190044 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/DroidSans.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16848 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Karla-Regular.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41208 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/ProggyClean.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35656 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/ProggyTiny.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   162588 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Roboto-Medium.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13792 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.187697 py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2502 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    46376 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/imgui_freetype.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3599 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/imgui_freetype.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.187697 py_imgui_redux-3.0.0/third-party/imgui/misc/single_file/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      994 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imgui/misc/single_file/imgui_single_file.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.187697 py_imgui_redux-3.0.0/third-party/imnodes/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1022 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/.clang-format
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1400 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/.clang-tidy
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       47 2024-05-09 00:10:01.000000 py_imgui_redux-3.0.0/third-party/imnodes/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9001 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       80 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/.gitmodules
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2180 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1072 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/LICENSE.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9463 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.188697 py_imgui_redux-3.0.0/third-party/imnodes/example/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24843 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/color_node_editor.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9464 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/graph.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      977 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/hello.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4164 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/main.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3595 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/multi_editor.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      135 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/node_editor.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5865 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/example/save_load.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.188697 py_imgui_redux-3.0.0/third-party/imnodes/img/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)  1517285 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/img/imnodes.gif
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114226 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/imnodes.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18234 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/imnodes.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12852 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/imnodes_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      213 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/imnodes/vcpkg.json
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.190697 py_imgui_redux-3.0.0/third-party/implot/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       46 2024-05-09 00:10:02.000000 py_imgui_redux-3.0.0/third-party/implot/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1068 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12224 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3591 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/TODO.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   273673 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/implot.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79742 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/implot.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114100 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/implot_demo.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    67521 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/implot_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   123095 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/implot/implot_items.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.191697 py_imgui_redux-3.0.0/third-party/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1271 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      996 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.clang-format
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2605 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.clang-tidy
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2196 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.cmake-format.yaml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1308 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       48 2024-05-09 00:10:03.000000 py_imgui_redux-3.0.0/third-party/pybind11/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       18 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.gitattributes
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      502 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4332 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       62 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/.readthedocs.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11983 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1684 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      223 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7686 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/README.rst
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.168697 py_imgui_redux-3.0.0/third-party/pybind11/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.192697 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23959 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7069 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    65660 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8458 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      120 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2096 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.193697 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28251 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    52929 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5491 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17869 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26305 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    42613 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1625 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.193697 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31418 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18108 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      316 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13471 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4731 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5002 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8262 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8862 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79408 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9103 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2734 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   126420 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    94641 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.193697 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4185 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15337 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29747 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2765 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/noxfile.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.193697 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      414 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/__init__.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1360 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/__main__.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      228 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/_version.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1226 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/commands.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/py.typed
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17609 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1261 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1618 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/setup.cfg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4877 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/setup.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/third-party/pybind11/tools/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2350 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3105 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11190 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      817 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1423 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/check-style.sh
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      952 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1040 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1031 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1311 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      196 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14033 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6930 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8960 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8361 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       94 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2104 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1234 2024-05-09 00:10:04.000000 py_imgui_redux-3.0.0/third-party/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2024-05-11 21:54:25.194697 py_imgui_redux-3.0.0/third-party/stb/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   282848 2024-04-22 03:34:42.000000 py_imgui_redux-3.0.0/third-party/stb/stb_image.h
```

### Comparing `py_imgui_redux-2.2.0/LICENSE` & `py_imgui_redux-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/PKG-INFO` & `py_imgui_redux-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: py-imgui-redux
-Version: 2.2.0
+Version: 3.0.0
 Summary: A python wrapper for DearImGUI and popular extensions
 Author: Alagyn
 Project-URL: Homepage, https://github.com/alagyn/py-imgui-redux
 Project-URL: Bug Tracker, https://github.com/alagyn/py-imgui-redux/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: py-glfw-redux==1.1.0
 
 <img src="https://github.com/alagyn/py-imgui-redux/blob/main/docs/pyimgui-logo-512.png?raw=true" width="256" align="right"/>
 
 
 # PyImGui
 DearImGui wrapper for python made with PyBind11
 
@@ -36,20 +35,21 @@
 pip install py-imgui-redux
 ```
 
 ## Modules:
 
 `imgui` - [Core DearImGUI](https://github.com/ocornut/imgui)  
 `imgui.implot` - [ImPlot library](https://github.com/epezent/implot)  
-`imgui.imnodes` - [ImNodes library](https://github.com/Nelarius/imnodes)
+`imgui.imnodes` - [ImNodes library](https://github.com/Nelarius/imnodes)  
+`imgui.glfw` - [GLFW Bindings](https://www.glfw.org)
 
 
 ## Backends:
 
-This module only uses the GFLW+OpenGL3 backend. Access to GLFW is provided via [py-glfw-redux](https://github.com/alagyn/py-glfw-redux)
+This module only uses the GFLW+OpenGL3 backend. `imgui.glfw` provides full access to GLFW's API, see below for it's adjustments
 
 ---
 
 ## API Adjustments
 
 I am writing this library with the primary goal of keeping the original Dear ImGui functional
 API as intact as possible. This is because:
@@ -246,30 +246,30 @@
 texture = imgui.LoadTexture(image.tobytes(),
                             image.size[0],
                             image.size[1],
                             len(image.getbands()))
 
 ```
 
+### GLFW API Adjustments
+
+This wrapper aims to be as close to the original API as possible.
+Exceptions:
+- Functions have lost the `glfw` prefix as this is already in the module name
+- Functions that returned pointers to arrays now return list-like objects
+- Functions that took pointers to output variables as arguments now return tuples
+
+
 ---
 
 ### Build Dependencies
 
 **Debian/apt**
 ```
-libx11-dev
-libxrandr-dev
-libxinerama-dev
-libxcursor-dev
-libxi-dev
-libgl-dev
+libx11-dev libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev libgl-dev
 ```
 
 **Fedora/yum**
 ```
-libXrandr-devel
-libXinerama-devel
-libXcursor-devel
-libXi-devel
-mesa-libGL-devel
+libXrandr-devel libXinerama-devel libXcursor-devel libXi-devel mesa-libGL-devel
 ```
```

### Comparing `py_imgui_redux-2.2.0/README.md` & `py_imgui_redux-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 pip install py-imgui-redux
 ```
 
 ## Modules:
 
 `imgui` - [Core DearImGUI](https://github.com/ocornut/imgui)  
 `imgui.implot` - [ImPlot library](https://github.com/epezent/implot)  
-`imgui.imnodes` - [ImNodes library](https://github.com/Nelarius/imnodes)
+`imgui.imnodes` - [ImNodes library](https://github.com/Nelarius/imnodes)  
+`imgui.glfw` - [GLFW Bindings](https://www.glfw.org)
 
 
 ## Backends:
 
-This module only uses the GFLW+OpenGL3 backend. Access to GLFW is provided via [py-glfw-redux](https://github.com/alagyn/py-glfw-redux)
+This module only uses the GFLW+OpenGL3 backend. `imgui.glfw` provides full access to GLFW's API, see below for it's adjustments
 
 ---
 
 ## API Adjustments
 
 I am writing this library with the primary goal of keeping the original Dear ImGui functional
 API as intact as possible. This is because:
@@ -227,30 +228,30 @@
 texture = imgui.LoadTexture(image.tobytes(),
                             image.size[0],
                             image.size[1],
                             len(image.getbands()))
 
 ```
 
+### GLFW API Adjustments
+
+This wrapper aims to be as close to the original API as possible.
+Exceptions:
+- Functions have lost the `glfw` prefix as this is already in the module name
+- Functions that returned pointers to arrays now return list-like objects
+- Functions that took pointers to output variables as arguments now return tuples
+
+
 ---
 
 ### Build Dependencies
 
 **Debian/apt**
 ```
-libx11-dev
-libxrandr-dev
-libxinerama-dev
-libxcursor-dev
-libxi-dev
-libgl-dev
+libx11-dev libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev libgl-dev
 ```
 
 **Fedora/yum**
 ```
-libXrandr-devel
-libXinerama-devel
-libXcursor-devel
-libXi-devel
-mesa-libGL-devel
+libXrandr-devel libXinerama-devel libXcursor-devel libXi-devel mesa-libGL-devel
 ```
```

### Comparing `py_imgui_redux-2.2.0/cmake/setupPyBindLib.cmake` & `py_imgui_redux-3.0.0/cmake/setupPyBindLib.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/pybind11_stubgen.py` & `py_imgui_redux-3.0.0/pybind11_stubgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         if c == s[start]:
             return i
     return -1
 
 
 def _is_balanced(s):
     closing = {
-        "(": ")", "{": "}", "[": "]"
+        "(": ")",
+        "{": "}",
+        "[": "]"
     }
 
     stack = []
     i = 0
     while i < len(s):
         c = s[i]
         if c in "\"'":
@@ -327,15 +329,15 @@
         ):
         replace_numpy_array,
         re.compile(
             r"(?<!\w)(?P<type>Callable|Dict|[Ii]terator|[Ii]terable|List"
             r"|Optional|Set|Tuple|Union|ItemsView|KeysView|ValuesView)(?!\w)"
         ):
         replace_typing_types,
-        re.compile(": (?P<type>\w+) = None"):
+        re.compile(r": (?P<type>\w+) = None"):
         make_optional
     }
 
     def parse(self):
         raise NotImplementedError
 
     def to_lines(self):  # type: () -> List[str]
```

### Comparing `py_imgui_redux-2.2.0/setup.py` & `py_imgui_redux-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,17 @@
                 os.listdir(bin_dir) if 
                 os.path.isfile(os.path.join(bin_dir, _lib)) and 
                 os.path.splitext(_lib)[1] in [".dll", ".so"]
                 and not (_lib.startswith("python") or _lib.startswith(PACKAGE_NAME))]
         """
 
         for lib in libs:
-            shutil.copy(lib, os.path.join(self.build_dir,
-                                          os.path.basename(lib)))
+            shutil.copy(
+                lib, os.path.join(self.build_dir, os.path.basename(lib))
+            )
 
         log(f"Generating stubs in {bin_dir}")
         env = dict(os.environ)
         try:
             oldPath = env["PYTHONPATH"]
         except KeyError:
             oldPath = ""
@@ -122,34 +123,37 @@
         if IS_WINDOWS:
             newPath = f"{bin_dir};" + oldPath
 
             # force glfw dll to be in the same dir
             # because we can't change the DLL lookup path via PATH
             # because reasons
             # https://docs.python.org/3/library/os.html#os.add_dll_directory
-            shutil.copy(f'{sysconfig.get_path("purelib")}/glfw3.dll', bin_dir)
+            # shutil.copy(f'{sysconfig.get_path("purelib")}/glfw3.dll', bin_dir)
         else:
             newPath = f"{bin_dir}:" + oldPath
 
         env["PYTHONPATH"] = newPath
-        """
-        subprocess.check_call([
-            sys.executable,
-            os.path.join(SOURCE_DIR, "pybind11_stubgen.py"), "--no-setup-py",
-            "imgui"
-        ],
-                              env=env,
-                              cwd=bin_dir)
+
+        subprocess.check_call(
+            [
+                sys.executable,
+                os.path.join(SOURCE_DIR, "pybind11_stubgen.py"),
+                "--no-setup-py",
+                "imgui"
+            ],
+            env=env,
+            cwd=bin_dir
+        )
 
         stub_dir = os.path.join(self.build_dir, "imgui")
         if os.path.exists(stub_dir):
             shutil.rmtree(stub_dir)
 
         shutil.move(os.path.join(bin_dir, "stubs/imgui-stubs"), stub_dir)
-        """
+
         # Mark the libs for installation, adding them to
         # distribution.data_files seems to ensure that setuptools' record
         # writer appends them to installed-files.txt in the package's egg-info
         #
         # Also tried adding the libraries to the distribution.libraries list,
         # but that never seemed to add them to the installed-files.txt in the
         # egg-info, and the online recommendation seems to be adding libraries
@@ -204,15 +208,16 @@
         log(f"Script dirs: {scripts_dirs}")
         log(f"Destination: {self.build_dir}")
 
         for scripts_dir in scripts_dirs:
 
             shutil.move(
                 scripts_dir,
-                os.path.join(self.build_dir, os.path.basename(scripts_dir)))
+                os.path.join(self.build_dir, os.path.basename(scripts_dir))
+            )
 
         # Mark the scripts for installation, adding them to
         # distribution.scripts seems to ensure that the setuptools' record
         # writer appends them to installed-files.txt in the package's egg-info
 
         self.distribution.scripts = scripts_dirs
 
@@ -253,17 +258,25 @@
 
         log("Configuring cmake project")
 
         PY_ROOT, _ = os.path.split(sys.executable)
         log(f"Using Py Root: {PY_ROOT}")
 
         args = [
-            "cmake", "-E", "env", "CMAKE_BUILD_PARALLEL_LEVEL=8",
-            f"Python3_ROOT_DIR={PY_ROOT}", "--", 'cmake', '-S', SOURCE_DIR,
-            '-B', self.build_temp
+            "cmake",
+            "-E",
+            "env",
+            "CMAKE_BUILD_PARALLEL_LEVEL=8",
+            f"Python3_ROOT_DIR={PY_ROOT}",
+            "--",
+            'cmake',
+            '-S',
+            SOURCE_DIR,
+            '-B',
+            self.build_temp
         ]
 
         if not IS_WINDOWS:
             args.append("-DCMAKE_BUILD_TYPE=Release")
 
         self.spawn(args)
 
@@ -317,15 +330,17 @@
         # These commands are subclassed above to avoid pitfalls that
         # setuptools tries to impose when installing these, as it usually
         # wants to build those libs and scripts as well or move them to a
         # different place. See comments above for additional information
 
 
 # Most of this is pulled from pyproject.toml
-setup(ext_modules=[CMakeExtension(name="imgui")],
-      packages=[],
-      cmdclass={
-          'build_ext': BuildCMakeExt,
-          'install_data': InstallCMakeLibsData,
-          'install_lib': InstallCMakeLibs,
-          'install_scripts': InstallCMakeScripts
-      })
+setup(
+    ext_modules=[CMakeExtension(name="imgui")],
+    packages=[],
+    cmdclass={
+        'build_ext': BuildCMakeExt,
+        'install_data': InstallCMakeLibsData,
+        'install_lib': InstallCMakeLibs,
+        'install_scripts': InstallCMakeScripts
+    }
+)
```

### Comparing `py_imgui_redux-2.2.0/source/inc/binder/enum-utility.h` & `py_imgui_redux-3.0.0/source/inc/binder/enum-utility.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/source/inc/binder/list-wrapper.h` & `py_imgui_redux-3.0.0/source/inc/binder/list-wrapper.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/source/inc/binder/wraps.h` & `py_imgui_redux-3.0.0/source/inc/binder/wraps.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/source/src/binder/enum-utility.cpp` & `py_imgui_redux-3.0.0/source/src/binder/enum-utility.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/source/src/binder/wraps.cpp` & `py_imgui_redux-3.0.0/source/src/binder/wraps.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/bind-backends/glfw.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/bind-backends/glfw.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 #include <pybind11/functional.h>
 
 #include <glad/gl.h>
 
 #include <GLFW/glfw3.h>
 #include <backends/imgui_impl_glfw.h>
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/bind-backends/opengl3.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/bind-backends/opengl3.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 #include <backends/imgui_impl_opengl3.h>
 
 // TODO not compiled atm
 
 void init_backend_opengl3(py::module& m)
 {
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/bind-imgui-core.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/bind-imgui-core.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/bind-modules.h>
 
 void init_core_imgui(py::module& m)
 {
     // Structs
     init_imgui_structs(m);
     // Enums
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/cursor-layout.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/cursor-layout.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 void init_cursor_and_layout(py::module& m)
 {
     QUICK(Separator);
     m.def(IMFUNC(SameLine), "offset_from_start_x"_a = 0.0f, "spacing"_a = 1.0f);
     QUICK(NewLine);
     QUICK(Spacing);
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/demos.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/demos.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_demos(py::module& m)
 {
     m.def(
         "ShowDemoWindow",
         [](BoolRef p_open)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/drawlist.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/drawlist.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
-#include <bind-imgui/imgui-core/texture.h>
+#include <bind-imgui/imgui-modules.h>
+#include <bind-imgui/texture.h>
 #include <binder/struct-utility.h>
 
 #include <pybind11/stl.h>
 
 #include <vector>
 
 void init_drawlist(py::module& m)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/im-windows.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/im-windows.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_windows(py::module& m)
 {
     // Windows
     m.def(
         "Begin",
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-context.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-context.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <imgui_internal.h>
 
 void init_imgui_context(py::module& m)
 {
     // Context
     // Make opaque wrapper
     py::class_<ImGuiContext>(m, "Context");
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-enums.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-enums.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/enum-utility.h>
 
 void init_imgui_enums(py::module& m)
 {
     ENUM(ImGui, WindowFlags)
         .RAW_VALUE(None_, ImGuiWindowFlags_None)
         .VALUE(ImGui, WindowFlags, NoTitleBar)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/imgui-structs.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/imgui-structs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/list-wrapper.h>
 #include <binder/struct-utility.h>
 
 #define RO_ARRAY(STRUCT, TYPE, VALUE, SIZE) \
     def_property_readonly( \
         #VALUE, \
         [](STRUCT* self) \
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/stacks.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/stacks.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 void init_stacks(py::module& m)
 {
     // Parameter Stacks (Shared)
     m.def(IMFUNC(PushFont), "font"_a);
     QUICK(PopFont);
     m.def(
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/styles.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/styles.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 void init_styles(py::module& m)
 {
     m.def(IMFUNC(StyleColorsDark), "dst"_a = nullptr);
     m.def(IMFUNC(StyleColorsLight), "dst"_a = nullptr);
     m.def(IMFUNC(StyleColorsClassic), "dst"_a = nullptr);
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/colors.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/colors.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_colors(py::module& m)
 {
     m.def(
         "ColorEdit3",
         [](const char* label, ImVec4& col, const int flags)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/drag-inputs.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/drag-inputs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_drags(py::module& m)
 {
     // Floats
     m.def(
         "DragFloat",
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/images.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/images.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/struct-utility.h>
 
 #include <sstream>
 
-#include <bind-imgui/imgui-core/texture.h>
+#include <bind-imgui/texture.h>
 
 #define STB_IMAGE_IMPLEMENTATION
 #include "stb_image.h"
 
 Texture _LoadTexture(
     char* bytes,
     unsigned width,
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/input.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/input.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_input(py::module& m)
 {
     // Ignoring callbacks and user-data
     m.def(
         "InputText",
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/main.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 #include <imgui_internal.h>
 
-#include <bind-imgui/imgui-core/texture.h>
+#include <bind-imgui/texture.h>
 
 void init_widgets_main(py::module& m)
 {
     m.def(
         IMFUNC(Button),
         "label"_a,
         py::arg_v("size", ImVec2(0, 0), "Vec2(0, 0)")
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/slide-inputs.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/slide-inputs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_slide(py::module& m)
 {
     // Float
     m.def(
         "SliderFloat",
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tables.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tables.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 void init_widgets_tables(py::module& m)
 {
     m.def(
         IMFUNC(BeginTable),
         "str_id"_a,
         "column"_a,
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tabs.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tabs.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_tabs(py::module& m)
 {
     m.def(IMFUNC(BeginTabBar), "str_id"_a, "flags"_a = 0);
     QUICK(EndTabBar);
     m.def(
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/text.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/text.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 
 void init_widgets_text(py::module& m)
 {
     // Leave Text formatting to the python side
     m.def(
         "Text",
         [](const char* text)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imgui-core/modules/widgets/tree.cpp` & `py_imgui_redux-3.0.0/source/src/imgui-core/modules/widgets/tree.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imgui-core/imgui-modules.h>
+#include <bind-imgui/imgui-modules.h>
 #include <binder/wraps.h>
 
 void init_widgets_tree(py::module& m)
 {
     m.def("TreeNode", py::overload_cast<const char*>(ImGui::TreeNode), "label"_a);
     // Leaving formatting to python
     m.def(
```

### Comparing `py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-context.cpp` & `py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-context.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-#include <bind-imgui/imnodes/imnodes-modules.h>
+#include <bind-imgui/imnodes-modules.h>
 #include <binder/wraps.h>
 
 // Include internal to get context class def
 #include <imnodes_internal.h>
 #include <pybind11/stl.h>
 
 void init_imnodes_context(py::module& m)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-enums.cpp` & `py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-enums.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imnodes/imnodes-modules.h>
+#include <bind-imgui/imnodes-modules.h>
 #include <binder/enum-utility.h>
 #include <imnodes.h>
 
 void init_imnodes_enums(py::module& m)
 {
     ENUM(ImNodes, Col)
         .VALUE(ImNodes, Col, NodeBackground)
```

### Comparing `py_imgui_redux-2.2.0/source/src/imnodes/modules/imnodes-structs.cpp` & `py_imgui_redux-3.0.0/source/src/imnodes/modules/imnodes-structs.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/imnodes/imnodes-modules.h>
+#include <bind-imgui/imnodes-modules.h>
 #include <binder/list-wrapper.h>
 #include <binder/struct-utility.h>
 
 bool* getIOPointer(int key)
 {
     bool* tgt = nullptr;
     switch(key)
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-colormap.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-colormap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 #include <binder/numpy.h>
 #include <binder/wraps.h>
 
 void init_colormaps(py::module& m)
 {
     m.def(
         "AddColorMap",
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-context.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-context.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #ifndef IMGUI_DEFINE_MATH_OPERATORS
     #define IMGUI_DEFINE_MATH_OPERATORS
 #endif
 
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 
 // Import internal so that we get the context class def
 #include <implot_internal.h>
 
 void init_implot_context(py::module& m)
 {
     // Def opaque class
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-enums.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-enums.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 #include <binder/enum-utility.h>
 
 void init_implot_enums(py::module& m)
 {
     ENUM(Im, Axis)
         .VALUE(Im, Axis, X1)
         .VALUE(Im, Axis, X2)
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-misc.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-misc.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 #include <binder/wraps.h>
 
 void init_misc(py::module& m)
 {
     // Input mapping
     QUICK(GetInputMap);
     m.def(
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-plotting.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-plotting.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#include <bind-imgui/imgui-core/texture.h>
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
+#include <bind-imgui/texture.h>
 #include <binder/numpy.h>
 
 void init_plotting(py::module& m)
 {
     m.def(
         "PlotLine",
         [](const char* label_id,
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-setup-funcs.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-setup-funcs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 #include <binder/wraps.h>
 
 void init_setup_funcs(py::module& m)
 {
     m.def(IMFUNC(SetupAxis), "axis"_a, "label"_a = nullptr, "flags"_a = 0);
     m.def(
         IMFUNC(SetupAxisLimits),
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-structs.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-structs.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 #include <binder/list-wrapper.h>
 #include <binder/struct-utility.h>
 
 void init_implot_structs(py::module& m)
 {
     py::class_<ImPlotPoint>(m, "Point")
         .def(py::init<double, double>(), "x"_a = 0, "y"_a = 0)
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-tools.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-tools.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 
 void init_tools(py::module& m)
 {
     m.def(
         "DragPoint",
         [](int id,
            double x,
```

### Comparing `py_imgui_redux-2.2.0/source/src/implot/modules/implot-utils.cpp` & `py_imgui_redux-3.0.0/source/src/implot/modules/implot-utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <bind-imgui/implot/implot-modules.h>
+#include <bind-imgui/implot-modules.h>
 
 #define STR(x) #x
 #define AUTO_COL_STR STR(IMPLOT_AUTO_COL)
 
 void init_utils(py::module& m)
 {
     m.def(IMFUNC(SetAxis), "axis"_a);
```

### Comparing `py_imgui_redux-2.2.0/third-party/imconfig/bind-imconfig.h` & `py_imgui_redux-3.0.0/third-party/imconfig/bind-imconfig.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/.editorconfig` & `py_imgui_redux-3.0.0/third-party/imgui/.editorconfig`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/.gitignore` & `py_imgui_redux-3.0.0/third-party/imgui/.gitignore`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/LICENSE.txt` & `py_imgui_redux-3.0.0/third-party/imgui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_allegro5.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_allegro5.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_allegro5.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_allegro5.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_android.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_android.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_android.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_android.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx10.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx10.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx10.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx10.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx11.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx11.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx11.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx11.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx12.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx12.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx12.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx12.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx9.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx9.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_dx9.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_dx9.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glfw.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glfw.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glfw.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glfw.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glut.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glut.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_glut.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_glut.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_metal.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_metal.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_metal.mm` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_metal.mm`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl2.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl2.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl2.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl2.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_opengl3_loader.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_opengl3_loader.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_osx.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_osx.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_osx.mm` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_osx.mm`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl2.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl2.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl2.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl2.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl3.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl3.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdl3.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdl3.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer2.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_sdlrenderer3.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_vulkan.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_vulkan.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_vulkan.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_vulkan.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_wgpu.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_wgpu.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_wgpu.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_wgpu.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_win32.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_win32.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/backends/imgui_impl_win32.h` & `py_imgui_redux-3.0.0/third-party/imgui/backends/imgui_impl_win32.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imconfig.h` & `py_imgui_redux-3.0.0/third-party/imgui/imconfig.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/imgui.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui.h` & `py_imgui_redux-3.0.0/third-party/imgui/imgui.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui_demo.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/imgui_demo.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui_draw.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/imgui_draw.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui_internal.h` & `py_imgui_redux-3.0.0/third-party/imgui/imgui_internal.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui_tables.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/imgui_tables.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imgui_widgets.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/imgui_widgets.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imstb_rectpack.h` & `py_imgui_redux-3.0.0/third-party/imgui/imstb_rectpack.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imstb_textedit.h` & `py_imgui_redux-3.0.0/third-party/imgui/imstb_textedit.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/imstb_truetype.h` & `py_imgui_redux-3.0.0/third-party/imgui/imstb_truetype.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/README.txt` & `py_imgui_redux-3.0.0/third-party/imgui/misc/README.txt`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/README.txt` & `py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/README.txt`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/imgui_stdlib.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/imgui_stdlib.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/cpp/imgui_stdlib.h` & `py_imgui_redux-3.0.0/third-party/imgui/misc/cpp/imgui_stdlib.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.gdb` & `py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.gdb`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.natstepfilter` & `py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.natstepfilter`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/debuggers/imgui.natvis` & `py_imgui_redux-3.0.0/third-party/imgui/misc/debuggers/imgui.natvis`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Cousine-Regular.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Cousine-Regular.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/DroidSans.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Karla-Regular.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/ProggyClean.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/ProggyClean.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/ProggyTiny.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/ProggyTiny.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/Roboto-Medium.ttf` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/README.md` & `py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/README.md`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/imgui_freetype.cpp` & `py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/imgui_freetype.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/freetype/imgui_freetype.h` & `py_imgui_redux-3.0.0/third-party/imgui/misc/freetype/imgui_freetype.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imgui/misc/single_file/imgui_single_file.h` & `py_imgui_redux-3.0.0/third-party/imgui/misc/single_file/imgui_single_file.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/.clang-format` & `py_imgui_redux-3.0.0/third-party/imnodes/.clang-format`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/.clang-tidy` & `py_imgui_redux-3.0.0/third-party/imnodes/.clang-tidy`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/.gitignore` & `py_imgui_redux-3.0.0/third-party/imnodes/.gitignore`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/CMakeLists.txt` & `py_imgui_redux-3.0.0/third-party/imnodes/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/LICENSE.md` & `py_imgui_redux-3.0.0/third-party/imnodes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/README.md` & `py_imgui_redux-3.0.0/third-party/imnodes/README.md`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/color_node_editor.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/example/color_node_editor.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/graph.h` & `py_imgui_redux-3.0.0/third-party/imnodes/example/graph.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/hello.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/example/hello.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/main.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/example/main.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/multi_editor.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/example/multi_editor.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/example/save_load.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/example/save_load.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/img/imnodes.gif` & `py_imgui_redux-3.0.0/third-party/imnodes/img/imnodes.gif`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/imnodes.cpp` & `py_imgui_redux-3.0.0/third-party/imnodes/imnodes.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/imnodes.h` & `py_imgui_redux-3.0.0/third-party/imnodes/imnodes.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/imnodes/imnodes_internal.h` & `py_imgui_redux-3.0.0/third-party/imnodes/imnodes_internal.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/LICENSE` & `py_imgui_redux-3.0.0/third-party/implot/LICENSE`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/README.md` & `py_imgui_redux-3.0.0/third-party/implot/README.md`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/TODO.md` & `py_imgui_redux-3.0.0/third-party/implot/TODO.md`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/implot.cpp` & `py_imgui_redux-3.0.0/third-party/implot/implot.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/implot.h` & `py_imgui_redux-3.0.0/third-party/implot/implot.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/implot_demo.cpp` & `py_imgui_redux-3.0.0/third-party/implot/implot_demo.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/implot_internal.h` & `py_imgui_redux-3.0.0/third-party/implot/implot_internal.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/implot/implot_items.cpp` & `py_imgui_redux-3.0.0/third-party/implot/implot_items.cpp`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.appveyor.yml` & `py_imgui_redux-3.0.0/third-party/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.clang-format` & `py_imgui_redux-3.0.0/third-party/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.clang-tidy` & `py_imgui_redux-3.0.0/third-party/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.cmake-format.yaml` & `py_imgui_redux-3.0.0/third-party/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.codespell-ignore-lines` & `py_imgui_redux-3.0.0/third-party/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/.pre-commit-config.yaml` & `py_imgui_redux-3.0.0/third-party/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/CMakeLists.txt` & `py_imgui_redux-3.0.0/third-party/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/LICENSE` & `py_imgui_redux-3.0.0/third-party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/README.rst` & `py_imgui_redux-3.0.0/third-party/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/attr.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/buffer_info.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/cast.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/chrono.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/complex.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/class.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/common.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/descr.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/init.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/internals.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/detail/typeid.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen/matrix.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eigen/tensor.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/embed.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/eval.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/functional.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/gil.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/iostream.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/numpy.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/operators.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/options.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/pybind11.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/pytypes.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl/filesystem.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/include/pybind11/stl_bind.h` & `py_imgui_redux-3.0.0/third-party/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/noxfile.py` & `py_imgui_redux-3.0.0/third-party/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/pybind11/__main__.py` & `py_imgui_redux-3.0.0/third-party/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/pybind11/commands.py` & `py_imgui_redux-3.0.0/third-party/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/pybind11/setup_helpers.py` & `py_imgui_redux-3.0.0/third-party/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/pyproject.toml` & `py_imgui_redux-3.0.0/third-party/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/setup.cfg` & `py_imgui_redux-3.0.0/third-party/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/setup.py` & `py_imgui_redux-3.0.0/third-party/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/FindCatch.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/FindEigen3.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/FindPythonLibsNew.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/JoinPaths.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/check-style.sh` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/cmake_uninstall.cmake.in` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/libsize.py` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/make_changelog.py` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Common.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Config.cmake.in` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11NewTools.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/pybind11Tools.cmake` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/setup_global.py.in` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/pybind11/tools/setup_main.py.in` & `py_imgui_redux-3.0.0/third-party/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `py_imgui_redux-2.2.0/third-party/stb/stb_image.h` & `py_imgui_redux-3.0.0/third-party/stb/stb_image.h`

 * *Files identical despite different names*

