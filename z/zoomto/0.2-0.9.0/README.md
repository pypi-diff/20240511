# Comparing `tmp/zoomto-0.2.tar.gz` & `tmp/zoomto-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomto-0.2.tar", last modified: Thu Dec 21 19:46:33 2023, max compression
+gzip compressed data, was "zoomto-0.9.0.tar", max compression
```

## Comparing `zoomto-0.2.tar` & `zoomto-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.108992 zoomto-0.2/
--rw-rw-rw-   0        0        0     1085 2023-12-08 00:59:26.000000 zoomto-0.2/LICENSE
--rw-rw-rw-   0        0        0      277 2023-12-21 19:46:33.108992 zoomto-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-12-11 23:24:55.000000 zoomto-0.2/README.md
--rw-rw-rw-   0        0        0      142 2023-12-15 19:30:13.000000 zoomto-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-21 19:46:33.108992 zoomto-0.2/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-12-21 19:46:20.000000 zoomto-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.095641 zoomto-0.2/zoomto/
--rw-rw-rw-   0        0        0       78 2023-12-21 19:34:01.000000 zoomto-0.2/zoomto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.105462 zoomto-0.2/zoomto/_internal/
--rw-rw-rw-   0        0        0      100 2023-12-21 17:37:04.000000 zoomto-0.2/zoomto/_internal/__init__.py
--rw-rw-rw-   0        0        0      542 2023-12-15 19:24:17.000000 zoomto-0.2/zoomto/_internal/debug.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.105987 zoomto-0.2/zoomto/_internal/img/
--rw-rw-rw-   0        0        0     1107 2023-12-07 21:06:05.000000 zoomto-0.2/zoomto/_internal/img/sharescreen_advanced_video.png
--rw-rw-rw-   0        0        0     1039 2023-12-21 19:15:36.000000 zoomto-0.2/zoomto/_internal/record.py
--rw-rw-rw-   0        0        0      974 2023-12-21 19:38:42.000000 zoomto-0.2/zoomto/_internal/win32.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.106992 zoomto-0.2/zoomto/core/
--rw-rw-rw-   0        0        0      630 2023-12-21 17:36:03.000000 zoomto-0.2/zoomto/core/cfg.py
--rw-rw-rw-   0        0        0     6606 2023-12-21 19:45:09.000000 zoomto-0.2/zoomto/core/driver.py
--rw-rw-rw-   0        0        0     2551 2023-12-21 19:45:21.000000 zoomto-0.2/zoomto/core/zoomto.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.107992 zoomto-0.2/zoomto/tools/
--rw-rw-rw-   0        0        0     3425 2023-12-11 05:34:13.000000 zoomto-0.2/zoomto/tools/getCurrentCoord.py
--rw-rw-rw-   0        0        0     2323 2023-12-12 03:47:14.000000 zoomto-0.2/zoomto/tools/shell.py
--rw-rw-rw-   0        0        0      348 2023-12-21 19:25:54.000000 zoomto-0.2/zoomto/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-21 19:46:33.107992 zoomto-0.2/zoomto.egg-info/
--rw-rw-rw-   0        0        0      277 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-12-21 19:46:33.000000 zoomto-0.2/zoomto.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1086 2024-05-03 23:07:07.450366 zoomto-0.9.0/LICENSE
+-rw-r--r--   0        0        0      686 2024-05-11 05:15:20.119785 zoomto-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-05-03 23:07:07.450366 zoomto-0.9.0/README.md
+-rw-r--r--   0        0        0       33 2024-05-04 00:57:37.752615 zoomto-0.9.0/src/zoomto/__init__.py
+-rw-r--r--   0        0        0     2853 2024-05-11 04:22:43.556700 zoomto-0.9.0/src/zoomto/app.py
+-rw-r--r--   0        0        0     2831 2024-05-11 04:26:37.084276 zoomto-0.9.0/src/zoomto/autogui.py
+-rw-r--r--   0        0        0      914 2024-05-04 00:56:37.724950 zoomto-0.9.0/src/zoomto/overload.py
+-rw-r--r--   0        0        0     1872 2024-05-11 01:29:54.580215 zoomto-0.9.0/src/zoomto/proc.py
+-rw-r--r--   0        0        0      608 2024-05-11 04:15:05.582367 zoomto-0.9.0/src/zoomto/static/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-05-11 02:29:32.022809 zoomto-0.9.0/src/zoomto/static/build/favicon.ico
+-rw-r--r--   0        0        0      709 2024-05-11 04:15:05.582367 zoomto-0.9.0/src/zoomto/static/build/index.html
+-rw-r--r--   0        0        0     5347 2024-05-11 02:29:32.483794 zoomto-0.9.0/src/zoomto/static/build/logo192.png
+-rw-r--r--   0        0        0     9664 2024-05-11 02:29:32.502794 zoomto-0.9.0/src/zoomto/static/build/logo512.png
+-rw-r--r--   0        0        0      492 2024-05-11 02:29:32.317095 zoomto-0.9.0/src/zoomto/static/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-11 02:29:32.543302 zoomto-0.9.0/src/zoomto/static/build/robots.txt
+-rw-r--r--   0        0        0      337 2024-05-11 04:15:05.582367 zoomto-0.9.0/src/zoomto/static/build/static/css/main.e6c13ad2.css
+-rw-r--r--   0        0        0      584 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/css/main.e6c13ad2.css.map
+-rw-r--r--   0        0        0     4532 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/js/453.9d3adcdd.chunk.js
+-rw-r--r--   0        0        0    10597 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/js/453.9d3adcdd.chunk.js.map
+-rw-r--r--   0        0        0   174462 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/js/main.eb11e087.js
+-rw-r--r--   0        0        0      971 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/js/main.eb11e087.js.LICENSE.txt
+-rw-r--r--   0        0        0   512548 2024-05-11 04:15:05.583367 zoomto-0.9.0/src/zoomto/static/build/static/js/main.eb11e087.js.map
+-rw-r--r--   0        0        0     4800 2024-05-11 04:39:12.496139 zoomto-0.9.0/src/zoomto/static/default-video-thumbnail.jpg
+-rw-r--r--   0        0        0      832 2024-05-03 23:59:54.737885 zoomto-0.9.0/src/zoomto/static/meeting_expand.png
+-rw-r--r--   0        0        0     1215 2024-05-04 01:08:26.068778 zoomto-0.9.0/src/zoomto/static/sharevid.png
+-rw-r--r--   0        0        0     1136 2024-05-11 04:22:24.007565 zoomto-0.9.0/src/zoomto/utils.py
+-rw-r--r--   0        0        0     1635 2024-05-11 04:41:06.631563 zoomto-0.9.0/src/zoomto/videoIndex.py
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 zoomto-0.9.0/PKG-INFO
```

### Comparing `zoomto-0.2/LICENSE` & `zoomto-0.9.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

