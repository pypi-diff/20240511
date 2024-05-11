# Comparing `tmp/nonecorn-0.16.0.dev6.tar.gz` & `tmp/nonecorn-0.16.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonecorn-0.16.0.dev6.tar", last modified: Tue May  7 11:13:12 2024, max compression
+gzip compressed data, was "nonecorn-0.16.0.dev7.tar", last modified: Sat May 11 09:18:06 2024, max compression
```

## Comparing `nonecorn-0.16.0.dev6.tar` & `nonecorn-0.16.0.dev7.tar`

### file list

```diff
@@ -1,161 +1,164 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.823251 nonecorn-0.16.0.dev6/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.713225 nonecorn-0.16.0.dev6/.github/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.729229 nonecorn-0.16.0.dev6/.github/workflows/
--rw-rw-rw-   0        0        0     3183 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev6/.gitignore
--rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev6/.readthedocs.yaml
--rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/LICENSE
--rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/MANIFEST.in
--rw-rw-rw-   0        0        0     4929 2024-05-07 11:13:12.824252 nonecorn-0.16.0.dev6/PKG-INFO
--rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.733230 nonecorn-0.16.0.dev6/artwork/
--rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/LICENSE
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo.png
--rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo.svg
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo_small.png
--rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo_small.svg
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.714226 nonecorn-0.16.0.dev6/compliance/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.735231 nonecorn-0.16.0.dev6/compliance/autobahn/
--rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/autobahn/fuzzingclient.json
--rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/autobahn/server.py
--rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/autobahn/summarise.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.738231 nonecorn-0.16.0.dev6/compliance/h2spec/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/h2spec/cert.pem
--rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/h2spec/key.pem
--rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/h2spec/server.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.741232 nonecorn-0.16.0.dev6/docs/
--rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.743232 nonecorn-0.16.0.dev6/docs/_static/
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/_static/logo.png
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/_static/logo_small.png
--rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.749234 nonecorn-0.16.0.dev6/docs/discussion/
--rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/backpressure.rst
--rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/closing.rst
--rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/design_choices.rst
--rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev6/docs/discussion/dos_mitigations.rst
--rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/docs/discussion/flow.rst
--rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/http2.rst
--rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/docs/discussion/index.rst
--rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/workers.rst
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.757236 nonecorn-0.16.0.dev6/docs/how_to_guides/
--rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/api_usage.rst
--rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/binds.rst
--rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/configuring.rst
--rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/dispatch_apps.rst
--rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/http_https_redirect.rst
--rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/index.rst
--rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/logging.rst
--rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/proxy_fix.rst
--rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/server_names.rst
--rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/statsd.rst
--rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/wsgi_apps.rst
--rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/index.rst
--rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.759236 nonecorn-0.16.0.dev6/docs/reference/
--rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/reference/api.rst
--rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/reference/index.rst
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.762237 nonecorn-0.16.0.dev6/docs/tutorials/
--rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/docs/tutorials/installation.rst
--rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/quickstart.rst
--rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/usage.rst
--rw-rw-rw-   0        0        0     3127 2024-05-07 11:12:57.000000 nonecorn-0.16.0.dev6/pyproject.toml
--rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/readme_zh.markdown
--rw-rw-rw-   0        0        0      156 2024-05-07 11:13:12.824252 nonecorn-0.16.0.dev6/setup.cfg
--rw-rw-rw-   0        0        0     2242 2024-05-07 11:12:32.000000 nonecorn-0.16.0.dev6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.717226 nonecorn-0.16.0.dev6/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.771239 nonecorn-0.16.0.dev6/src/hypercorn/
--rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/__init__.py
--rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/__main__.py
--rw-rw-rw-   0        0        0     5675 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/src/hypercorn/app_wrappers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.777241 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/
--rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/__init__.py
--rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/lifespan.py
--rw-rw-rw-   0        0        0     8240 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/run.py
--rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/statsd.py
--rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/task_group.py
--rw-rw-rw-   0        0        0     6455 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/tcp_server.py
--rw-rw-rw-   0        0        0     3228 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/udp_server.py
--rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/worker_context.py
--rw-rw-rw-   0        0        0    14318 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/src/hypercorn/config.py
--rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/events.py
--rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.780241 nonecorn-0.16.0.dev6/src/hypercorn/middleware/
--rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/dispatcher.py
--rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/http_to_https.py
--rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/proxy_fix.py
--rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.786243 nonecorn-0.16.0.dev6/src/hypercorn/protocol/
--rw-rw-rw-   0        0        0     3235 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/events.py
--rw-rw-rw-   0        0        0    13933 2024-01-15 10:30:30.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h11.py
--rw-rw-rw-   0        0        0    17133 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h2.py
--rw-rw-rw-   0        0        0     6125 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h3.py
--rw-rw-rw-   0        0        0    14834 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/http_stream.py
--rw-rw-rw-   0        0        0     5346 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/quic.py
--rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/ws_stream.py
--rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/py.typed
--rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/run.py
--rw-rw-rw-   0        0        0     3985 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/src/hypercorn/statsd.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.794245 nonecorn-0.16.0.dev6/src/hypercorn/trio/
--rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/__init__.py
--rw-rw-rw-   0        0        0     3728 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/lifespan.py
--rw-rw-rw-   0        0        0     5209 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/run.py
--rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/statsd.py
--rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/task_group.py
--rw-rw-rw-   0        0        0     5373 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/tcp_server.py
--rw-rw-rw-   0        0        0     1783 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/udp_server.py
--rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/worker_context.py
--rw-rw-rw-   0        0        0     8258 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/typing.py
--rw-rw-rw-   0        0        0     9646 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/utils.py
--rw-rw-rw-   0        0        0    14215 2024-05-07 11:05:55.000000 nonecorn-0.16.0.dev6/src/hypercorn/workers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.799246 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/
--rw-rw-rw-   0        0        0     4929 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3694 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      273 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.806247 nonecorn-0.16.0.dev6/tests/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.809248 nonecorn-0.16.0.dev6/tests/assets/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/cert.pem
--rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config.py
--rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config.toml
--rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config_ssl.py
--rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/key.pem
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.814249 nonecorn-0.16.0.dev6/tests/asyncio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/asyncio/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/asyncio/helpers.py
--rw-rw-rw-   0        0        0     4075 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_keep_alive.py
--rw-rw-rw-   0        0        0     2654 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_lifespan.py
--rw-rw-rw-   0        0        0     8765 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_sanity.py
--rw-rw-rw-   0        0        0     1571 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_task_group.py
--rw-rw-rw-   0        0        0     1680 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_tcp_server.py
--rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/conftest.py
--rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev6/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.817250 nonecorn-0.16.0.dev6/tests/middleware/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/middleware/__init__.py
--rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev6/tests/middleware/test_dispatcher.py
--rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/middleware/test_http_to_https.py
--rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev6/tests/middleware/test_proxy_fix.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.820251 nonecorn-0.16.0.dev6/tests/protocol/
--rw-rw-rw-   0        0        0    15278 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_h11.py
--rw-rw-rw-   0        0        0     3612 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_h2.py
--rw-rw-rw-   0        0        0    10742 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/tests/protocol/test_http_stream.py
--rw-rw-rw-   0        0        0    17493 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_ws_stream.py
--rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test___main__.py
--rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/tests/test_app_wrappers.py
--rw-rw-rw-   0        0        0     5687 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/test_config.py
--rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test_logging.py
--rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.823251 nonecorn-0.16.0.dev6/tests/trio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/trio/__init__.py
--rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/tests/trio/test_keep_alive.py
--rw-rw-rw-   0        0        0     1661 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/trio/test_lifespan.py
--rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/tests/trio/test_sanity.py
--rw-rw-rw-   0        0        0     1245 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.827329 nonecorn-0.16.0.dev7/
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.706796 nonecorn-0.16.0.dev7/.github/
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.726312 nonecorn-0.16.0.dev7/.github/workflows/
+-rw-rw-rw-   0        0        0     3183 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev7/.gitignore
+-rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev7/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4981 2024-05-11 09:18:06.827329 nonecorn-0.16.0.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev7/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.730306 nonecorn-0.16.0.dev7/artwork/
+-rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/artwork/LICENSE
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/artwork/logo.png
+-rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/artwork/logo.svg
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/artwork/logo_small.png
+-rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/artwork/logo_small.svg
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.708797 nonecorn-0.16.0.dev7/compliance/
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.732307 nonecorn-0.16.0.dev7/compliance/autobahn/
+-rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/compliance/autobahn/fuzzingclient.json
+-rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/compliance/autobahn/server.py
+-rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/compliance/autobahn/summarise.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.735307 nonecorn-0.16.0.dev7/compliance/h2spec/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/compliance/h2spec/cert.pem
+-rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/compliance/h2spec/key.pem
+-rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/compliance/h2spec/server.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.739308 nonecorn-0.16.0.dev7/docs/
+-rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.740308 nonecorn-0.16.0.dev7/docs/_static/
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/_static/logo.png
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/_static/logo_small.png
+-rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/docs/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.747310 nonecorn-0.16.0.dev7/docs/discussion/
+-rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/discussion/backpressure.rst
+-rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/discussion/closing.rst
+-rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/discussion/design_choices.rst
+-rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev7/docs/discussion/dos_mitigations.rst
+-rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/docs/discussion/flow.rst
+-rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/discussion/http2.rst
+-rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/docs/discussion/index.rst
+-rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/discussion/workers.rst
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.756312 nonecorn-0.16.0.dev7/docs/how_to_guides/
+-rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/api_usage.rst
+-rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/binds.rst
+-rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/configuring.rst
+-rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/dispatch_apps.rst
+-rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/http_https_redirect.rst
+-rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/index.rst
+-rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/logging.rst
+-rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/proxy_fix.rst
+-rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/server_names.rst
+-rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/statsd.rst
+-rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev7/docs/how_to_guides/wsgi_apps.rst
+-rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/index.rst
+-rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.758313 nonecorn-0.16.0.dev7/docs/reference/
+-rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/reference/api.rst
+-rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/reference/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.761314 nonecorn-0.16.0.dev7/docs/tutorials/
+-rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev7/docs/tutorials/installation.rst
+-rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/tutorials/quickstart.rst
+-rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/docs/tutorials/usage.rst
+-rw-rw-rw-   0        0        0     3122 2024-05-11 09:14:58.000000 nonecorn-0.16.0.dev7/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/readme_zh.markdown
+-rw-rw-rw-   0        0        0      156 2024-05-11 09:18:06.828329 nonecorn-0.16.0.dev7/setup.cfg
+-rw-rw-rw-   0        0        0     2351 2024-05-11 09:15:40.000000 nonecorn-0.16.0.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.711798 nonecorn-0.16.0.dev7/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.771316 nonecorn-0.16.0.dev7/src/hypercorn/
+-rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/src/hypercorn/__init__.py
+-rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/src/hypercorn/__main__.py
+-rw-rw-rw-   0        0        0     5675 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/src/hypercorn/app_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.778317 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/
+-rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/lifespan.py
+-rw-rw-rw-   0        0        0     8240 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/run.py
+-rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/statsd.py
+-rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/task_group.py
+-rw-rw-rw-   0        0        0     6454 2024-05-11 09:12:15.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-rw-   0        0        0     3228 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/udp_server.py
+-rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/src/hypercorn/asyncio/worker_context.py
+-rw-rw-rw-   0        0        0    14318 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev7/src/hypercorn/config.py
+-rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/events.py
+-rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/src/hypercorn/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.783318 nonecorn-0.16.0.dev7/src/hypercorn/middleware/
+-rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev7/src/hypercorn/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/src/hypercorn/middleware/dispatcher.py
+-rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/src/hypercorn/middleware/http_to_https.py
+-rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev7/src/hypercorn/middleware/proxy_fix.py
+-rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/src/hypercorn/middleware/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.789320 nonecorn-0.16.0.dev7/src/hypercorn/protocol/
+-rw-rw-rw-   0        0        0     3235 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/events.py
+-rw-rw-rw-   0        0        0    14035 2024-05-11 08:55:34.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/h11.py
+-rw-rw-rw-   0        0        0    17133 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/h2.py
+-rw-rw-rw-   0        0        0     6125 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/h3.py
+-rw-rw-rw-   0        0        0    14834 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/http_stream.py
+-rw-rw-rw-   0        0        0     5346 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/quic.py
+-rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev7/src/hypercorn/protocol/ws_stream.py
+-rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/src/hypercorn/py.typed
+-rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/src/hypercorn/run.py
+-rw-rw-rw-   0        0        0     3985 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev7/src/hypercorn/statsd.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.796321 nonecorn-0.16.0.dev7/src/hypercorn/trio/
+-rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/__init__.py
+-rw-rw-rw-   0        0        0     3728 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/lifespan.py
+-rw-rw-rw-   0        0        0     5209 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/run.py
+-rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/statsd.py
+-rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/task_group.py
+-rw-rw-rw-   0        0        0     6014 2024-05-11 09:15:03.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/tcp_server.py
+-rw-rw-rw-   0        0        0     1783 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/udp_server.py
+-rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/src/hypercorn/trio/worker_context.py
+-rw-rw-rw-   0        0        0     8258 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev7/src/hypercorn/typing.py
+-rw-rw-rw-   0        0        0     9575 2024-05-11 09:12:15.000000 nonecorn-0.16.0.dev7/src/hypercorn/utils.py
+-rw-rw-rw-   0        0        0    14215 2024-05-07 11:05:55.000000 nonecorn-0.16.0.dev7/src/hypercorn/workers.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.800322 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/
+-rw-rw-rw-   0        0        0     4981 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3740 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      296 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 09:18:06.000000 nonecorn-0.16.0.dev7/src/nonecorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.806324 nonecorn-0.16.0.dev7/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.810325 nonecorn-0.16.0.dev7/tests/assets/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/assets/cert.pem
+-rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/assets/config.py
+-rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/assets/config.toml
+-rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/assets/config_ssl.py
+-rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/assets/key.pem
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.816326 nonecorn-0.16.0.dev7/tests/asyncio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/asyncio/helpers.py
+-rw-rw-rw-   0        0        0     4075 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/asyncio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     2654 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/asyncio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8765 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/asyncio/test_sanity.py
+-rw-rw-rw-   0        0        0     1571 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/asyncio/test_task_group.py
+-rw-rw-rw-   0        0        0     1680 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/asyncio/test_tcp_server.py
+-rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.818327 nonecorn-0.16.0.dev7/tests/e2e/
+-rw-rw-rw-   0        0        0        0 2024-05-11 08:55:34.000000 nonecorn-0.16.0.dev7/tests/e2e/__init__.py
+-rw-rw-rw-   0        0        0     1549 2024-05-11 08:55:34.000000 nonecorn-0.16.0.dev7/tests/e2e/test_httpx.py
+-rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev7/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.821327 nonecorn-0.16.0.dev7/tests/middleware/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev7/tests/middleware/test_dispatcher.py
+-rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/middleware/test_http_to_https.py
+-rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev7/tests/middleware/test_proxy_fix.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.824328 nonecorn-0.16.0.dev7/tests/protocol/
+-rw-rw-rw-   0        0        0    15278 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/protocol/test_h11.py
+-rw-rw-rw-   0        0        0     3612 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/protocol/test_h2.py
+-rw-rw-rw-   0        0        0    10742 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev7/tests/protocol/test_http_stream.py
+-rw-rw-rw-   0        0        0    17493 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/protocol/test_ws_stream.py
+-rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/test___main__.py
+-rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev7/tests/test_app_wrappers.py
+-rw-rw-rw-   0        0        0     5687 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/test_config.py
+-rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/test_logging.py
+-rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 09:18:06.827329 nonecorn-0.16.0.dev7/tests/trio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev7/tests/trio/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/tests/trio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     1661 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev7/tests/trio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev7/tests/trio/test_sanity.py
+-rw-rw-rw-   0        0        0     1256 2024-05-11 08:55:34.000000 nonecorn-0.16.0.dev7/tox.ini
```

### Comparing `nonecorn-0.16.0.dev6/.github/workflows/ci.yml` & `nonecorn-0.16.0.dev7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/.github/workflows/publish.yml` & `nonecorn-0.16.0.dev7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/CHANGELOG.rst` & `nonecorn-0.16.0.dev7/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/LICENSE` & `nonecorn-0.16.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/PKG-INFO` & `nonecorn-0.16.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev6
+Version: 0.16.0.dev7
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: h3
 Provides-Extra: tests
 Provides-Extra: trio
 Provides-Extra: uvloop
```

### Comparing `nonecorn-0.16.0.dev6/README.rst` & `nonecorn-0.16.0.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/artwork/LICENSE` & `nonecorn-0.16.0.dev7/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/artwork/logo.png` & `nonecorn-0.16.0.dev7/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/artwork/logo.svg` & `nonecorn-0.16.0.dev7/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/artwork/logo_small.png` & `nonecorn-0.16.0.dev7/artwork/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/artwork/logo_small.svg` & `nonecorn-0.16.0.dev7/artwork/logo_small.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/compliance/autobahn/server.py` & `nonecorn-0.16.0.dev7/compliance/autobahn/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/compliance/h2spec/cert.pem` & `nonecorn-0.16.0.dev7/compliance/h2spec/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/compliance/h2spec/key.pem` & `nonecorn-0.16.0.dev7/compliance/h2spec/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/compliance/h2spec/server.py` & `nonecorn-0.16.0.dev7/compliance/h2spec/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/Makefile` & `nonecorn-0.16.0.dev7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/_static/logo.png` & `nonecorn-0.16.0.dev7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/_static/logo_small.png` & `nonecorn-0.16.0.dev7/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/conf.py` & `nonecorn-0.16.0.dev7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/backpressure.rst` & `nonecorn-0.16.0.dev7/docs/discussion/backpressure.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/closing.rst` & `nonecorn-0.16.0.dev7/docs/discussion/closing.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/dos_mitigations.rst` & `nonecorn-0.16.0.dev7/docs/discussion/dos_mitigations.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/flow.rst` & `nonecorn-0.16.0.dev7/docs/discussion/flow.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/http2.rst` & `nonecorn-0.16.0.dev7/docs/discussion/http2.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/discussion/workers.rst` & `nonecorn-0.16.0.dev7/docs/discussion/workers.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/api_usage.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/api_usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/binds.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/binds.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/configuring.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/configuring.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/dispatch_apps.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/dispatch_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/http_https_redirect.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/http_https_redirect.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/logging.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/logging.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/proxy_fix.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/proxy_fix.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/server_names.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/server_names.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/statsd.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/statsd.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/how_to_guides/wsgi_apps.rst` & `nonecorn-0.16.0.dev7/docs/how_to_guides/wsgi_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/index.rst` & `nonecorn-0.16.0.dev7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/make.bat` & `nonecorn-0.16.0.dev7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/tutorials/quickstart.rst` & `nonecorn-0.16.0.dev7/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/docs/tutorials/usage.rst` & `nonecorn-0.16.0.dev7/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/pyproject.toml` & `nonecorn-0.16.0.dev7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonecorn"
-version = "0.16.0dev6"
+version = "0.16.0dev7"
 description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -37,28 +37,29 @@
 taskgroup = { version = "*", python = "<3.11", allow-prereleases = true }
 tomli = { version = "*", python = "<3.11" }
 trio = { version = ">=0.22.0", optional = true }
 uvloop = { version = "*", markers = "platform_system != 'Windows'", optional = true }
 wsproto = ">=0.14.0"
 
 [tool.poetry.dev-dependencies]
+httpx = "*"
 hypothesis = "*"
 mock = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-trio = "*"
 trio = "*"
 
 [tool.poetry.scripts]
 hypercorn = "hypercorn.__main__:main"
 
 [tool.poetry.extras]
 docs = ["pydata_sphinx_theme", "sphinxcontrib_mermaid"]
 h3 = ["aioquic"]
-trio = ["exceptiongroup", "trio"]
+trio = ["trio"]
 uvloop = ["uvloop"]
 
 [tool.black]
 line-length = 100
 target-version = ["py38"]
 
 [tool.isort]
```

### Comparing `nonecorn-0.16.0.dev6/readme_zh.markdown` & `nonecorn-0.16.0.dev7/readme_zh.markdown`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/setup.py` & `nonecorn-0.16.0.dev7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 with open(os.path.join(PROJECT_ROOT, "README.rst")) as file_:
     long_description = file_.read()
 
 INSTALL_REQUIRES = [
     "h11",
     "h2 >= 3.1.0",
     "priority",
-    "toml",
+    "tomli; python_version < '3.11'",
+    "exceptiongroup >= 1.1.0",
     "typing_extensions >= 3.7.4; python_version < '3.8'",
     "taskgroup; python_version < '3.11'",
     "wsproto >= 0.14.0",
 ]
 
 TESTS_REQUIRE = [
     "hypothesis",
@@ -29,15 +30,15 @@
     "pytest-cov",
     "pytest-trio",
     "trio",
 ]
 
 setup(
     name="nonecorn",
-    version="0.16.0dev6",
+    version="0.16.0dev7",
     python_requires=">=3.7",
     description="A ASGI Server forked from hypercorn with more extra feature beyond ASGI",
     long_description=long_description,
     url="https://gitlab.com/pgjones/hypercorn/",
     author="P G Jones",
     author_email="philip.graham.jones@googlemail.com",
     license="MIT",
@@ -50,14 +51,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["hypercorn"],
     install_requires=INSTALL_REQUIRES,
```

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/__main__.py` & `nonecorn-0.16.0.dev7/src/hypercorn/__main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/app_wrappers.py` & `nonecorn-0.16.0.dev7/src/hypercorn/app_wrappers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/__init__.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/lifespan.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/run.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/statsd.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/task_group.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/tcp_server.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/tcp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         try:
             client = parse_socket_addr(socket.family, socket.getpeername())
             server = parse_socket_addr(socket.family, socket.getsockname())
             ssl_object = self.writer.get_extra_info("ssl_object")
             if ssl_object is not None:
                 ssl = True
                 alpn_protocol = ssl_object.selected_alpn_protocol()
-                tls = get_tls_info(self.writer)
+                tls = get_tls_info(ssl_object)
                 if tls:
                     tls["server_cert"] = self.config.cert_pem
             else:
                 ssl = False
                 alpn_protocol = "http/1.1"
 
             async with TaskGroup(self.loop) as task_group:
```

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/udp_server.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/worker_context.py` & `nonecorn-0.16.0.dev7/src/hypercorn/asyncio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/config.py` & `nonecorn-0.16.0.dev7/src/hypercorn/config.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/events.py` & `nonecorn-0.16.0.dev7/src/hypercorn/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/logging.py` & `nonecorn-0.16.0.dev7/src/hypercorn/logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/middleware/dispatcher.py` & `nonecorn-0.16.0.dev7/src/hypercorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/middleware/http_to_https.py` & `nonecorn-0.16.0.dev7/src/hypercorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/middleware/proxy_fix.py` & `nonecorn-0.16.0.dev7/src/hypercorn/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/middleware/wsgi.py` & `nonecorn-0.16.0.dev7/src/hypercorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/__init__.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/events.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h11.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/h11.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,17 +134,20 @@
         elif isinstance(event, Closed):
             if self.stream is not None:
                 await self._close_stream()
 
     async def stream_send(self, event: StreamEvent) -> None:
         if isinstance(event, Response):
             if event.status_code >= 200:
+                headers = list(chain(event.headers, self.config.response_headers("h11")))
+                if self.keep_alive_requests >= self.config.keep_alive_max_requests:
+                    headers.append((b"connection", b"close"))
                 await self._send_h11_event(
                     h11.Response(
-                        headers=list(chain(event.headers, self.config.response_headers("h11"))),
+                        headers=headers,
                         status_code=event.status_code,
                         reason=event.reason.encode("ascii"),
                     )
                 )
             else:
                 await self._send_h11_event(
                     h11.InformationalResponse(
@@ -309,15 +312,14 @@
 
     async def _maybe_recycle(self) -> None:
         await self._close_stream()
         if (
             not self.context.terminated.is_set()
             and self.connection.our_state is h11.DONE
             and self.connection.their_state is h11.DONE
-            and self.keep_alive_requests <= self.config.keep_alive_max_requests
         ):
             try:
                 self.connection.start_next_cycle()
             except h11.LocalProtocolError:
                 await self.send(Closed())
             else:
                 self.response = None
```

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h2.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h3.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/http_stream.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/http_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/quic.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/protocol/ws_stream.py` & `nonecorn-0.16.0.dev7/src/hypercorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/run.py` & `nonecorn-0.16.0.dev7/src/hypercorn/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/statsd.py` & `nonecorn-0.16.0.dev7/src/hypercorn/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/__init__.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/lifespan.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/run.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/task_group.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/tcp_server.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/tcp_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from math import inf
 from typing import Any, Dict, Generator, Optional
 
+import exceptiongroup
 import trio
 
 from .task_group import TaskGroup
 from .worker_context import WorkerContext
 from ..config import Config
 from ..events import Closed, Event, RawData, Updated
 from ..protocol import ProtocolWrapper
 from ..typing import AppWrapper
-from ..utils import parse_socket_addr
+from ..utils import get_tls_info, parse_socket_addr
 
 MAX_RECV = 2**16
 
 
 class TCPServer:
     def __init__(
         self,
@@ -44,43 +45,54 @@
             try:
                 with trio.fail_after(self.config.ssl_handshake_timeout):
                     await self.stream.do_handshake()
             except (trio.BrokenResourceError, trio.TooSlowError):
                 return  # Handshake failed
             alpn_protocol = self.stream.selected_alpn_protocol()
             socket = self.stream.transport_stream.socket
+            ssl_object = self.stream._ssl_object
+            tls = get_tls_info(ssl_object)
+            if tls:
+                tls["server_cert"] = self.config.cert_pem
             ssl = True
         except AttributeError:  # Not SSL
             alpn_protocol = "http/1.1"
             socket = self.stream.socket
+            tls = None
             ssl = False
 
-        try:
-            client = parse_socket_addr(socket.family, socket.getpeername())
-            server = parse_socket_addr(socket.family, socket.getsockname())
+        def log_handler(e: Exception) -> None:
+            if self.config.log.error_logger is not None:
+                self.config.log.error_logger.exception("Internal hypercorn error", exc_info=e)
 
-            async with TaskGroup() as task_group:
-                self._task_group = task_group
-                self.protocol = ProtocolWrapper(
-                    self.app,
-                    self.config,
-                    self.context,
-                    task_group,
-                    ssl,
-                    client,
-                    server,
-                    self.protocol_send,
-                    alpn_protocol,
-                    self.app_state,
-                )
-                await self.protocol.initiate()
-                await self._start_idle()
-                await self._read_data()
-        except OSError:
-            pass
+        try:
+            with exceptiongroup.catch(
+                {OSError: lambda e: None, Exception: log_handler}  # type: ignore
+            ):
+                client = parse_socket_addr(socket.family, socket.getpeername())
+                server = parse_socket_addr(socket.family, socket.getsockname())
+
+                async with TaskGroup() as task_group:
+                    self._task_group = task_group
+                    self.protocol = ProtocolWrapper(
+                        self.app,
+                        self.config,
+                        self.context,
+                        task_group,
+                        ssl,
+                        client,
+                        server,
+                        self.protocol_send,
+                        alpn_protocol,
+                        tls,
+                        self.app_state,
+                    )
+                    await self.protocol.initiate()
+                    await self._start_idle()
+                    await self._read_data()
         finally:
             await self._close()
 
     async def protocol_send(self, event: Event) -> None:
         if isinstance(event, RawData):
             async with self.send_lock:
                 try:
```

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/udp_server.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/trio/worker_context.py` & `nonecorn-0.16.0.dev7/src/hypercorn/trio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/typing.py` & `nonecorn-0.16.0.dev7/src/hypercorn/typing.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/utils.py` & `nonecorn-0.16.0.dev7/src/hypercorn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     "TLSv1": 0x0301,
     "TLSv1.1": 0x0302,
     "TLSv1.2": 0x0303,
     "TLSv1.3": 0x0304,
 }
 
 
-def get_tls_info(writer: asyncio.StreamWriter) -> Optional[Dict]:
+def get_tls_info(ssl_object: ssl.SSLObject) -> Optional[Dict]:
     """
     # server_cert: Unable to set from transport information
     # client_cert_chain: Just the peercert, currently no access to the full cert chain
     # client_cert_name:
     # client_cert_error: No access to this
     # tls_version:
     # cipher_suite: Too hard to convert without direct access to openssl
@@ -253,15 +253,14 @@
         "client_cert_chain": [],
         "client_cert_name": None,
         "client_cert_error": None,
         "tls_version": None,
         "cipher_suite": None,
     }
 
-    ssl_object = writer.get_extra_info("ssl_object", default=None)
     peercert = ssl_object.getpeercert()
 
     if peercert:
         rdn_strings = []
         for rdn in peercert["subject"]:
             rdn_strings.append(
                 "+".join(
```

### Comparing `nonecorn-0.16.0.dev6/src/hypercorn/workers.py` & `nonecorn-0.16.0.dev7/src/hypercorn/workers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/src/nonecorn.egg-info/PKG-INFO` & `nonecorn-0.16.0.dev7/src/nonecorn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev6
+Version: 0.16.0.dev7
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: h3
 Provides-Extra: tests
 Provides-Extra: trio
 Provides-Extra: uvloop
```

### Comparing `nonecorn-0.16.0.dev6/src/nonecorn.egg-info/SOURCES.txt` & `nonecorn-0.16.0.dev7/src/nonecorn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,16 @@
 tests/asyncio/__init__.py
 tests/asyncio/helpers.py
 tests/asyncio/test_keep_alive.py
 tests/asyncio/test_lifespan.py
 tests/asyncio/test_sanity.py
 tests/asyncio/test_task_group.py
 tests/asyncio/test_tcp_server.py
+tests/e2e/__init__.py
+tests/e2e/test_httpx.py
 tests/middleware/__init__.py
 tests/middleware/test_dispatcher.py
 tests/middleware/test_http_to_https.py
 tests/middleware/test_proxy_fix.py
 tests/protocol/test_h11.py
 tests/protocol/test_h2.py
 tests/protocol/test_http_stream.py
```

### Comparing `nonecorn-0.16.0.dev6/tests/assets/cert.pem` & `nonecorn-0.16.0.dev7/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/assets/key.pem` & `nonecorn-0.16.0.dev7/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/helpers.py` & `nonecorn-0.16.0.dev7/tests/asyncio/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/test_keep_alive.py` & `nonecorn-0.16.0.dev7/tests/asyncio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/test_lifespan.py` & `nonecorn-0.16.0.dev7/tests/asyncio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/test_sanity.py` & `nonecorn-0.16.0.dev7/tests/asyncio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/test_task_group.py` & `nonecorn-0.16.0.dev7/tests/asyncio/test_task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/asyncio/test_tcp_server.py` & `nonecorn-0.16.0.dev7/tests/asyncio/test_tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/conftest.py` & `nonecorn-0.16.0.dev7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/helpers.py` & `nonecorn-0.16.0.dev7/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/middleware/test_dispatcher.py` & `nonecorn-0.16.0.dev7/tests/middleware/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/middleware/test_http_to_https.py` & `nonecorn-0.16.0.dev7/tests/middleware/test_http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/middleware/test_proxy_fix.py` & `nonecorn-0.16.0.dev7/tests/middleware/test_proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/protocol/test_h11.py` & `nonecorn-0.16.0.dev7/tests/protocol/test_h11.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/protocol/test_h2.py` & `nonecorn-0.16.0.dev7/tests/protocol/test_h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/protocol/test_http_stream.py` & `nonecorn-0.16.0.dev7/tests/protocol/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/protocol/test_ws_stream.py` & `nonecorn-0.16.0.dev7/tests/protocol/test_ws_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/test___main__.py` & `nonecorn-0.16.0.dev7/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/test_app_wrappers.py` & `nonecorn-0.16.0.dev7/tests/test_app_wrappers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/test_config.py` & `nonecorn-0.16.0.dev7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/test_logging.py` & `nonecorn-0.16.0.dev7/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/test_utils.py` & `nonecorn-0.16.0.dev7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/trio/test_keep_alive.py` & `nonecorn-0.16.0.dev7/tests/trio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/trio/test_lifespan.py` & `nonecorn-0.16.0.dev7/tests/trio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tests/trio/test_sanity.py` & `nonecorn-0.16.0.dev7/tests/trio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev6/tox.ini` & `nonecorn-0.16.0.dev7/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -3,76 +3,77 @@
 00000020: 792c 7079 3338 2c70 7933 392c 7079 3331  y,py38,py39,py31
 00000030: 302c 7079 3331 312c 7079 3331 322c 7061  0,py311,py312,pa
 00000040: 636b 6167 652c 7065 7038 0d0a 6d69 6e76  ckage,pep8..minv
 00000050: 6572 7369 6f6e 203d 2033 2e33 0d0a 6973  ersion = 3.3..is
 00000060: 6f6c 6174 6564 5f62 7569 6c64 203d 2074  olated_build = t
 00000070: 7275 650d 0a0d 0a5b 7465 7374 656e 765d  rue....[testenv]
 00000080: 0d0a 6465 7073 203d 0d0a 2020 2020 7079  ..deps =..    py
-00000090: 3337 3a20 6d6f 636b 0d0a 2020 2020 6879  37: mock..    hy
-000000a0: 706f 7468 6573 6973 0d0a 2020 2020 7079  pothesis..    py
-000000b0: 7465 7374 0d0a 2020 2020 7079 7465 7374  test..    pytest
-000000c0: 2d61 7379 6e63 696f 0d0a 2020 2020 7079  -asyncio..    py
-000000d0: 7465 7374 2d63 6f76 0d0a 2020 2020 7079  test-cov..    py
-000000e0: 7465 7374 2d73 7567 6172 0d0a 2020 2020  test-sugar..    
-000000f0: 7079 7465 7374 2d74 7269 6f0d 0a63 6f6d  pytest-trio..com
-00000100: 6d61 6e64 7320 3d20 7079 7465 7374 202d  mands = pytest -
-00000110: 2d63 6f76 3d68 7970 6572 636f 726e 207b  -cov=hypercorn {
-00000120: 706f 7361 7267 737d 0d0a 0d0a 5b74 6573  posargs}....[tes
-00000130: 7465 6e76 3a64 6f63 735d 0d0a 6261 7365  tenv:docs]..base
-00000140: 7079 7468 6f6e 203d 2070 7974 686f 6e33  python = python3
-00000150: 2e31 320d 0a64 6570 7320 3d0d 0a20 2020  .12..deps =..   
-00000160: 2070 7964 6174 612d 7370 6869 6e78 2d74   pydata-sphinx-t
-00000170: 6865 6d65 0d0a 2020 2020 7370 6869 6e78  heme..    sphinx
-00000180: 0d0a 2020 2020 7370 6869 6e78 636f 6e74  ..    sphinxcont
-00000190: 7269 622d 6d65 726d 6169 640d 0a20 2020  rib-mermaid..   
-000001a0: 2074 7269 6f0d 0a63 6f6d 6d61 6e64 7320   trio..commands 
-000001b0: 3d0d 0a20 2020 2073 7068 696e 782d 6170  =..    sphinx-ap
-000001c0: 6964 6f63 202d 6520 2d66 202d 6f20 646f  idoc -e -f -o do
-000001d0: 6373 2f72 6566 6572 656e 6365 2f73 6f75  cs/reference/sou
-000001e0: 7263 652f 2073 7263 2f68 7970 6572 636f  rce/ src/hyperco
-000001f0: 726e 2f20 7372 632f 6879 7065 7263 6f72  rn/ src/hypercor
-00000200: 6e2f 7072 6f74 6f63 6f6c 2f71 7569 632e  n/protocol/quic.
-00000210: 7079 2073 7263 2f68 7970 6572 636f 726e  py src/hypercorn
-00000220: 2f70 726f 746f 636f 6c2f 6833 2e70 790d  /protocol/h3.py.
-00000230: 0a20 2020 2073 7068 696e 782d 6275 696c  .    sphinx-buil
-00000240: 6420 2d57 202d 2d6b 6565 702d 676f 696e  d -W --keep-goin
-00000250: 6720 2d62 2068 746d 6c20 2d64 207b 656e  g -b html -d {en
-00000260: 7674 6d70 6469 727d 2f64 6f63 7472 6565  vtmpdir}/doctree
-00000270: 7320 646f 6373 2f20 646f 6373 2f5f 6275  s docs/ docs/_bu
-00000280: 696c 642f 6874 6d6c 2f0d 0a0d 0a5b 7465  ild/html/....[te
-00000290: 7374 656e 763a 666f 726d 6174 5d0d 0a62  stenv:format]..b
-000002a0: 6173 6570 7974 686f 6e20 3d20 7079 7468  asepython = pyth
-000002b0: 6f6e 332e 3132 0d0a 6465 7073 203d 0d0a  on3.12..deps =..
-000002c0: 2020 2020 626c 6163 6b0d 0a20 2020 2069      black..    i
-000002d0: 736f 7274 0d0a 636f 6d6d 616e 6473 203d  sort..commands =
-000002e0: 0d0a 2020 2020 626c 6163 6b20 2d2d 6368  ..    black --ch
-000002f0: 6563 6b20 2d2d 6469 6666 2073 7263 2f68  eck --diff src/h
-00000300: 7970 6572 636f 726e 2f20 7465 7374 732f  ypercorn/ tests/
-00000310: 0d0a 2020 2020 6973 6f72 7420 2d2d 6368  ..    isort --ch
-00000320: 6563 6b20 2d2d 6469 6666 2073 7263 2f68  eck --diff src/h
-00000330: 7970 6572 636f 726e 2074 6573 7473 0d0a  ypercorn tests..
-00000340: 0d0a 5b74 6573 7465 6e76 3a70 6570 385d  ..[testenv:pep8]
-00000350: 0d0a 6261 7365 7079 7468 6f6e 203d 2070  ..basepython = p
-00000360: 7974 686f 6e33 2e31 320d 0a64 6570 7320  ython3.12..deps 
-00000370: 3d0d 0a20 2020 2066 6c61 6b65 380d 0a20  =..    flake8.. 
-00000380: 2020 2070 6570 382d 6e61 6d69 6e67 0d0a     pep8-naming..
-00000390: 2020 2020 666c 616b 6538 2d66 7574 7572      flake8-futur
-000003a0: 652d 696d 706f 7274 0d0a 2020 2020 666c  e-import..    fl
-000003b0: 616b 6538 2d70 7269 6e74 0d0a 636f 6d6d  ake8-print..comm
-000003c0: 616e 6473 203d 2066 6c61 6b65 3820 7372  ands = flake8 sr
-000003d0: 632f 6879 7065 7263 6f72 6e2f 2074 6573  c/hypercorn/ tes
-000003e0: 7473 2f0d 0a0d 0a5b 7465 7374 656e 763a  ts/....[testenv:
-000003f0: 6d79 7079 5d0d 0a62 6173 6570 7974 686f  mypy]..basepytho
-00000400: 6e20 3d20 7079 7468 6f6e 332e 3132 0d0a  n = python3.12..
-00000410: 6465 7073 203d 0d0a 2020 2020 6d79 7079  deps =..    mypy
-00000420: 0d0a 2020 2020 7079 7465 7374 0d0a 636f  ..    pytest..co
-00000430: 6d6d 616e 6473 203d 0d0a 2020 2020 6d79  mmands =..    my
-00000440: 7079 2073 7263 2f68 7970 6572 636f 726e  py src/hypercorn
-00000450: 2f20 7465 7374 732f 0d0a 0d0a 5b74 6573  / tests/....[tes
-00000460: 7465 6e76 3a70 6163 6b61 6765 5d0d 0a62  tenv:package]..b
-00000470: 6173 6570 7974 686f 6e20 3d20 7079 7468  asepython = pyth
-00000480: 6f6e 332e 3132 0d0a 6465 7073 203d 0d0a  on3.12..deps =..
-00000490: 2020 2020 706f 6574 7279 0d0a 2020 2020      poetry..    
-000004a0: 7477 696e 650d 0a63 6f6d 6d61 6e64 7320  twine..commands 
-000004b0: 3d0d 0a20 2020 2070 6f65 7472 7920 6275  =..    poetry bu
-000004c0: 696c 640d 0a20 2020 2074 7769 6e65 2063  ild..    twine c
-000004d0: 6865 636b 2064 6973 742f 2a0d 0a         heck dist/*..
+00000090: 3337 3a20 6d6f 636b 0d0a 2020 2020 6874  37: mock..    ht
+000000a0: 7470 780d 0a20 2020 2068 7970 6f74 6865  tpx..    hypothe
+000000b0: 7369 730d 0a20 2020 2070 7974 6573 740d  sis..    pytest.
+000000c0: 0a20 2020 2070 7974 6573 742d 6173 796e  .    pytest-asyn
+000000d0: 6369 6f0d 0a20 2020 2070 7974 6573 742d  cio..    pytest-
+000000e0: 636f 760d 0a20 2020 2070 7974 6573 742d  cov..    pytest-
+000000f0: 7375 6761 720d 0a20 2020 2070 7974 6573  sugar..    pytes
+00000100: 742d 7472 696f 0d0a 636f 6d6d 616e 6473  t-trio..commands
+00000110: 203d 2070 7974 6573 7420 2d2d 636f 763d   = pytest --cov=
+00000120: 6879 7065 7263 6f72 6e20 7b70 6f73 6172  hypercorn {posar
+00000130: 6773 7d0d 0a0d 0a5b 7465 7374 656e 763a  gs}....[testenv:
+00000140: 646f 6373 5d0d 0a62 6173 6570 7974 686f  docs]..basepytho
+00000150: 6e20 3d20 7079 7468 6f6e 332e 3132 0d0a  n = python3.12..
+00000160: 6465 7073 203d 0d0a 2020 2020 7079 6461  deps =..    pyda
+00000170: 7461 2d73 7068 696e 782d 7468 656d 650d  ta-sphinx-theme.
+00000180: 0a20 2020 2073 7068 696e 780d 0a20 2020  .    sphinx..   
+00000190: 2073 7068 696e 7863 6f6e 7472 6962 2d6d   sphinxcontrib-m
+000001a0: 6572 6d61 6964 0d0a 2020 2020 7472 696f  ermaid..    trio
+000001b0: 0d0a 636f 6d6d 616e 6473 203d 0d0a 2020  ..commands =..  
+000001c0: 2020 7370 6869 6e78 2d61 7069 646f 6320    sphinx-apidoc 
+000001d0: 2d65 202d 6620 2d6f 2064 6f63 732f 7265  -e -f -o docs/re
+000001e0: 6665 7265 6e63 652f 736f 7572 6365 2f20  ference/source/ 
+000001f0: 7372 632f 6879 7065 7263 6f72 6e2f 2073  src/hypercorn/ s
+00000200: 7263 2f68 7970 6572 636f 726e 2f70 726f  rc/hypercorn/pro
+00000210: 746f 636f 6c2f 7175 6963 2e70 7920 7372  tocol/quic.py sr
+00000220: 632f 6879 7065 7263 6f72 6e2f 7072 6f74  c/hypercorn/prot
+00000230: 6f63 6f6c 2f68 332e 7079 0d0a 2020 2020  ocol/h3.py..    
+00000240: 7370 6869 6e78 2d62 7569 6c64 202d 5720  sphinx-build -W 
+00000250: 2d2d 6b65 6570 2d67 6f69 6e67 202d 6220  --keep-going -b 
+00000260: 6874 6d6c 202d 6420 7b65 6e76 746d 7064  html -d {envtmpd
+00000270: 6972 7d2f 646f 6374 7265 6573 2064 6f63  ir}/doctrees doc
+00000280: 732f 2064 6f63 732f 5f62 7569 6c64 2f68  s/ docs/_build/h
+00000290: 746d 6c2f 0d0a 0d0a 5b74 6573 7465 6e76  tml/....[testenv
+000002a0: 3a66 6f72 6d61 745d 0d0a 6261 7365 7079  :format]..basepy
+000002b0: 7468 6f6e 203d 2070 7974 686f 6e33 2e31  thon = python3.1
+000002c0: 320d 0a64 6570 7320 3d0d 0a20 2020 2062  2..deps =..    b
+000002d0: 6c61 636b 0d0a 2020 2020 6973 6f72 740d  lack..    isort.
+000002e0: 0a63 6f6d 6d61 6e64 7320 3d0d 0a20 2020  .commands =..   
+000002f0: 2062 6c61 636b 202d 2d63 6865 636b 202d   black --check -
+00000300: 2d64 6966 6620 7372 632f 6879 7065 7263  -diff src/hyperc
+00000310: 6f72 6e2f 2074 6573 7473 2f0d 0a20 2020  orn/ tests/..   
+00000320: 2069 736f 7274 202d 2d63 6865 636b 202d   isort --check -
+00000330: 2d64 6966 6620 7372 632f 6879 7065 7263  -diff src/hyperc
+00000340: 6f72 6e20 7465 7374 730d 0a0d 0a5b 7465  orn tests....[te
+00000350: 7374 656e 763a 7065 7038 5d0d 0a62 6173  stenv:pep8]..bas
+00000360: 6570 7974 686f 6e20 3d20 7079 7468 6f6e  epython = python
+00000370: 332e 3132 0d0a 6465 7073 203d 0d0a 2020  3.12..deps =..  
+00000380: 2020 666c 616b 6538 0d0a 2020 2020 7065    flake8..    pe
+00000390: 7038 2d6e 616d 696e 670d 0a20 2020 2066  p8-naming..    f
+000003a0: 6c61 6b65 382d 6675 7475 7265 2d69 6d70  lake8-future-imp
+000003b0: 6f72 740d 0a20 2020 2066 6c61 6b65 382d  ort..    flake8-
+000003c0: 7072 696e 740d 0a63 6f6d 6d61 6e64 7320  print..commands 
+000003d0: 3d20 666c 616b 6538 2073 7263 2f68 7970  = flake8 src/hyp
+000003e0: 6572 636f 726e 2f20 7465 7374 732f 0d0a  ercorn/ tests/..
+000003f0: 0d0a 5b74 6573 7465 6e76 3a6d 7970 795d  ..[testenv:mypy]
+00000400: 0d0a 6261 7365 7079 7468 6f6e 203d 2070  ..basepython = p
+00000410: 7974 686f 6e33 2e31 320d 0a64 6570 7320  ython3.12..deps 
+00000420: 3d0d 0a20 2020 206d 7970 790d 0a20 2020  =..    mypy..   
+00000430: 2070 7974 6573 740d 0a63 6f6d 6d61 6e64   pytest..command
+00000440: 7320 3d0d 0a20 2020 206d 7970 7920 7372  s =..    mypy sr
+00000450: 632f 6879 7065 7263 6f72 6e2f 2074 6573  c/hypercorn/ tes
+00000460: 7473 2f0d 0a0d 0a5b 7465 7374 656e 763a  ts/....[testenv:
+00000470: 7061 636b 6167 655d 0d0a 6261 7365 7079  package]..basepy
+00000480: 7468 6f6e 203d 2070 7974 686f 6e33 2e31  thon = python3.1
+00000490: 320d 0a64 6570 7320 3d0d 0a20 2020 2070  2..deps =..    p
+000004a0: 6f65 7472 790d 0a20 2020 2074 7769 6e65  oetry..    twine
+000004b0: 0d0a 636f 6d6d 616e 6473 203d 0d0a 2020  ..commands =..  
+000004c0: 2020 706f 6574 7279 2062 7569 6c64 0d0a    poetry build..
+000004d0: 2020 2020 7477 696e 6520 6368 6563 6b20      twine check 
+000004e0: 6469 7374 2f2a 0d0a                      dist/*..
```

