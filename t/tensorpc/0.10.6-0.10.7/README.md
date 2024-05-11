# Comparing `tmp/tensorpc-0.10.6.tar.gz` & `tmp/tensorpc-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorpc-0.10.6.tar", last modified: Sat Apr 27 14:11:15 2024, max compression
+gzip compressed data, was "tensorpc-0.10.7.tar", last modified: Sat May 11 05:40:24 2024, max compression
```

## Comparing `tensorpc-0.10.6.tar` & `tensorpc-0.10.7.tar`

### file list

```diff
@@ -1,360 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.018931 tensorpc-0.10.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-27 14:10:46.000000 tensorpc-0.10.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-27 14:10:46.000000 tensorpc-0.10.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-27 14:11:15.018931 tensorpc-0.10.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-27 14:10:46.000000 tensorpc-0.10.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-27 14:10:46.000000 tensorpc-0.10.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 14:11:15.018931 tensorpc-0.10.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-27 14:10:46.000000 tensorpc-0.10.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.970930 tensorpc-0.10.6/tensorpc/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.970930 tensorpc-0.10.6/tensorpc/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.970930 tensorpc-0.10.6/tensorpc/apps/cbvc/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/apps/cbvc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/apps/file/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/apps/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    52830 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/coretypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/media/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/media/hooks-bash-legacy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/media/hooks-bash.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/scheduler/init_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/init_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/init_scheduler/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/scheduler/runtask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/runtask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/runtask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/scheduler/tmux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/serv_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/autossh/services/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/autossh/services/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.974930 tensorpc-0.10.6/tensorpc/cli/cppls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/cppls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/cppls/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/cpuusage/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/cpuusage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/cpuusage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/createmsg/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/createmsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/createmsg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/download_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/download_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/download_file/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/free_port/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/free_port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/free_port/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/gpuusage/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/gpuusage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/gpuusage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/iperf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/iperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/iperf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/ping/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/ping/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/proto_files/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/proto_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/proto_files/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/proto_root/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/proto_root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/proto_root/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/pyls/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/pyls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/pyls/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/pyright_launch/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/pyright_launch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/pyright_launch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.978930 tensorpc-0.10.6/tensorpc/cli/start_worker/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/start_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/cli/start_worker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.982930 tensorpc-0.10.6/tensorpc/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/asyncserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/asynctools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/bgserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16973 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/core_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/dataclass_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.986930 tensorpc-0.10.6/tensorpc/core/event_emitter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/event_emitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/event_emitter/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/event_emitter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/funcid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.986930 tensorpc-0.10.6/tensorpc/core/httpservers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpservers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpservers/aiohttp_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpservers/all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpservers/blacksheep_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    35329 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/httpservers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/inspecttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/moduleid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/prim.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/rprint_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/server_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    52173 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/serviceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/core/tree_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.986930 tensorpc-0.10.6/tensorpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.986930 tensorpc-0.10.6/tensorpc/examples/ai/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/ai/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.966930 tensorpc-0.10.6/tensorpc/examples/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.986930 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.1-Hello World.md
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.12-App Context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.4-Containers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.0-Common Props.md
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.1-Button.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.10-Slider.md
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.11-Tab.md
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.12-Drawer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.13-Dialog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.14-Collapse.md
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.15-Chip.md
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.16-Progress.md
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.17-MenuList.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.18-JsonLikeTree.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.19-DynamicControl.md
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.2-Typography.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.20-VirtualizedBox.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.21-DataFlexBox.md
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.23-Special.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.24-Editor.md
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.25-Plotly.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.26-Map.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.27-Allotment.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.28-JsonViewer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.3-Markdown.md
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.4-TextField.md
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.5-List.md
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.6-Select.md
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.9-Image.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.2-3D Events.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.3-Controls.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.4-Selection.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.5-Views.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.6-Resources.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.7-Custom Shaders.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/04-3d components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/04-3d components/4.1-Canvas.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/04-3d components/4.2-Mesh.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/04-3d components/4.3-Points.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/04-3d components/4.4-Lines.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/05-advanced/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/05-advanced/5.1-Inspector.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/05-advanced/5.2-SimpleCanvas.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/06-sample apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/06-sample apps/6.1-Chat App.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/06-sample apps/6.2-Deep Learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.994930 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.2-Events.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.3-Lines.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.4-Image.md
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.5-Points.md
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/examples/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.998930 tensorpc-0.10.6/tensorpc/flow/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17924 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.998930 tensorpc-0.10.6/tensorpc/flow/close_langserv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/close_langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/close_langserv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/coretypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.998930 tensorpc-0.10.6/tensorpc/flow/flowapp/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76779 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/appcore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:14.998930 tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.002930 tensorpc-0.10.6/tensorpc/flow/flowapp/components/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/annocore.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/leaflet.py
--rw-r--r--   0 runner    (1001) docker     (127)   178760 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/mui.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.002930 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/arraycommon.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/arraygrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    32169 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.002930 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.006930 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)    44599 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/reload_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/scriptmgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/sliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.006930 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56801 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/treeview.py
--rw-r--r--   0 runner    (1001) docker     (127)    27521 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py
--rw-r--r--   0 runner    (1001) docker     (127)   144462 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/three.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/threecore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/components/typemetas.py
--rw-r--r--   0 runner    (1001) docker     (127)    79929 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/objtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/flowapp/reload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.006930 tensorpc-0.10.6/tensorpc/flow/init_langserv/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/init_langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/init_langserv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/jsonlike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.006930 tensorpc-0.10.6/tensorpc/flow/langserv/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/langserv/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/langserv/pyls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/langserv/pyrightcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.006930 tensorpc-0.10.6/tensorpc/flow/runapp/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/runapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/runapp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.010930 tensorpc-0.10.6/tensorpc/flow/sampleapp/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59344 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/arraygrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    41653 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/d3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/sample_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/sample_reload_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/sampleapp/v_nextgen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.010930 tensorpc-0.10.6/tensorpc/flow/serv/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/serv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105903 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/serv/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18927 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/serv/flowapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/serv/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/flow/serv_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.010930 tensorpc-0.10.6/tensorpc/protos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/arraybuf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/arraybuf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/arraybuf_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/remote_object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/remote_object_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/remote_object_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/rpc_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/rpc_message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/wsdef_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos/wsdef_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/protos_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/arraybuf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/arraybuf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/remote_object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/remote_object_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/rpc_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/rpc_message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/wsdef_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/protos_legacy/wsdef_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/scheduler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/serve/flowapp_script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve/flowapp_script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve/flowapp_script/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/serve_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/serve_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/services/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.014930 tensorpc-0.10.6/tensorpc/services/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/flow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/for_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/services/vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.018931 tensorpc-0.10.6/tensorpc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/df_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/gpuusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/typeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/uniquename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-27 14:10:46.000000 tensorpc-0.10.6/tensorpc/utils/wait_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.018931 tensorpc-0.10.6/tensorpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 14:11:14.000000 tensorpc-0.10.6/tensorpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 14:11:15.018931 tensorpc-0.10.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-27 14:10:46.000000 tensorpc-0.10.6/test/test_tmux_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-11 05:39:55.000000 tensorpc-0.10.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 05:39:55.000000 tensorpc-0.10.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-11 05:40:24.321910 tensorpc-0.10.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-11 05:39:55.000000 tensorpc-0.10.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-11 05:39:55.000000 tensorpc-0.10.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 05:40:24.321910 tensorpc-0.10.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-11 05:39:55.000000 tensorpc-0.10.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.277910 tensorpc-0.10.7/tensorpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.277910 tensorpc-0.10.7/tensorpc/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.277910 tensorpc-0.10.7/tensorpc/apps/cbvc/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/apps/cbvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.277910 tensorpc-0.10.7/tensorpc/apps/file/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/apps/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.277910 tensorpc-0.10.7/tensorpc/autossh/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52830 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/coretypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/autossh/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/media/hooks-bash-legacy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/media/hooks-bash.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/autossh/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/autossh/scheduler/init_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/init_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/init_scheduler/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/autossh/scheduler/runtask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/runtask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/runtask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/scheduler/tmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/serv_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/autossh/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/autossh/services/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/cppls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/cppls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/cppls/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/cpuusage/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/cpuusage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/cpuusage/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/createmsg/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/createmsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/createmsg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/download_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/download_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/download_file/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.281910 tensorpc-0.10.7/tensorpc/cli/free_port/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/free_port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/free_port/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/gpuusage/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/gpuusage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/gpuusage/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/iperf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/iperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/iperf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/ping/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/proto_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/proto_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/proto_files/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/proto_root/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/proto_root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/proto_root/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/pyls/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/pyls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/pyls/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/pyright_launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/pyright_launch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/pyright_launch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.285910 tensorpc-0.10.7/tensorpc/cli/start_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/start_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/cli/start_worker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.289910 tensorpc-0.10.7/tensorpc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/asyncserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/asynctools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/bgserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16973 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35849 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/core_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/dataclass_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.289910 tensorpc-0.10.7/tensorpc/core/event_emitter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/event_emitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/event_emitter/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/event_emitter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/funcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.289910 tensorpc-0.10.7/tensorpc/core/httpservers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpservers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpservers/aiohttp_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpservers/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpservers/blacksheep_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35329 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/httpservers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/inspecttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/moduleid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/prim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/rprint_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/server_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52173 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/serviceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/core/tree_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.289910 tensorpc-0.10.7/tensorpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.289910 tensorpc-0.10.7/tensorpc/examples/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/ai/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.273910 tensorpc-0.10.7/tensorpc/examples/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.293910 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.1-Hello World.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.12-App Context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.4-Containers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.297910 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.0-Common Props.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.1-Button.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.10-Slider.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.11-Tab.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.12-Drawer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.13-Dialog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.14-Collapse.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.15-Chip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.16-Progress.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.17-MenuList.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.18-JsonLikeTree.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.19-DynamicControl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.2-Typography.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.20-VirtualizedBox.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.21-DataFlexBox.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.23-Special.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.24-Editor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.25-Plotly.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.26-Map.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.27-Allotment.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.28-JsonViewer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.3-Markdown.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.4-TextField.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.5-List.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.6-Select.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.9-Image.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.297910 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.2-3D Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.3-Controls.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.4-Selection.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.5-Views.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.6-Resources.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.7-Custom Shaders.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.297910 tensorpc-0.10.7/tensorpc/examples/tutorials/04-3d components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/04-3d components/4.1-Canvas.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/04-3d components/4.2-Mesh.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/04-3d components/4.3-Points.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/04-3d components/4.4-Lines.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/examples/tutorials/05-advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/05-advanced/5.1-Inspector.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/05-advanced/5.2-SimpleCanvas.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/examples/tutorials/06-sample apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/06-sample apps/6.1-Chat App.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/06-sample apps/6.2-Deep Learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.2-Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.3-Lines.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.4-Image.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.5-Points.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/examples/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19011 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/flow/close_langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/close_langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/close_langserv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/coretypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.301910 tensorpc-0.10.7/tensorpc/flow/flowapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76779 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/appcore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.305910 tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.305910 tensorpc-0.10.7/tensorpc/flow/flowapp/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/annocore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/leaflet.py
+-rw-r--r--   0 runner    (1001) docker     (127)   178760 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/mui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.309910 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/arraycommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/arraygrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32169 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.309910 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.309910 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44599 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/reload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/scriptmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/sliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56801 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/treeview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27521 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144462 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/three.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/threecore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/components/typemetas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79929 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/objtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/flowapp/reload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/init_langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/init_langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/init_langserv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/jsonlike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/langserv/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/langserv/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/langserv/pyrightcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/runapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/runapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/runapp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/sampleapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59344 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/arraygrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41653 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/d3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/sample_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/sample_reload_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/sampleapp/v_nextgen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.313910 tensorpc-0.10.7/tensorpc/flow/serv/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/serv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105903 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/serv/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19192 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/serv/flowapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/serv/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/flow/serv_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.317910 tensorpc-0.10.7/tensorpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/arraybuf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/arraybuf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/arraybuf_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/remote_object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/remote_object_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/remote_object_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/rpc_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/rpc_message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/wsdef_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos/wsdef_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.317910 tensorpc-0.10.7/tensorpc/protos_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/arraybuf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/arraybuf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/remote_object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/remote_object_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/rpc_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/rpc_message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/wsdef_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/protos_legacy/wsdef_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.317910 tensorpc-0.10.7/tensorpc/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/scheduler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.317910 tensorpc-0.10.7/tensorpc/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.317910 tensorpc-0.10.7/tensorpc/serve/flowapp_script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve/flowapp_script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve/flowapp_script/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/tensorpc/serve_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/serve_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/tensorpc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/tensorpc/services/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/flow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/for_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/services/vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/tensorpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/df_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/gpuusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/uniquename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-11 05:39:55.000000 tensorpc-0.10.7/tensorpc/utils/wait_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/tensorpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 05:40:24.000000 tensorpc-0.10.7/tensorpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 05:40:24.321910 tensorpc-0.10.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-11 05:39:55.000000 tensorpc-0.10.7/test/test_tmux_scheduler.py
```

### Comparing `tensorpc-0.10.6/LICENSE` & `tensorpc-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/PKG-INFO` & `tensorpc-0.10.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorpc
-Version: 0.10.6
+Version: 0.10.7
 Summary: Backend for devflow.
 Home-page: https://github.com/FindDefinition/tensorpc
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `tensorpc-0.10.6/README.md` & `tensorpc-0.10.7/README.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/setup.py` & `tensorpc-0.10.7/setup.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/__init__.py` & `tensorpc-0.10.7/tensorpc/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/__main__.py` & `tensorpc-0.10.7/tensorpc/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/apps/__init__.py` & `tensorpc-0.10.7/tensorpc/apps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/apps/cbvc/__init__.py` & `tensorpc-0.10.7/tensorpc/apps/cbvc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/apps/file/__init__.py` & `tensorpc-0.10.7/tensorpc/apps/file/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/__init__.py` & `tensorpc-0.10.7/tensorpc/autossh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/autossh/constants.py` & `tensorpc-0.10.7/tensorpc/autossh/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/core.py` & `tensorpc-0.10.7/tensorpc/autossh/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/coretypes.py` & `tensorpc-0.10.7/tensorpc/autossh/coretypes.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/media/hooks-bash-legacy.sh` & `tensorpc-0.10.7/tensorpc/autossh/media/hooks-bash-legacy.sh`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/media/hooks-bash.sh` & `tensorpc-0.10.7/tensorpc/autossh/media/hooks-bash.sh`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/client.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/constants.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/core.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/runtask/__main__.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/runtask/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/task_client.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/task_client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/scheduler/tmux.py` & `tensorpc-0.10.7/tensorpc/autossh/scheduler/tmux.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/serv_names.py` & `tensorpc-0.10.7/tensorpc/autossh/serv_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/autossh/services/__init__.py` & `tensorpc-0.10.7/tensorpc/autossh/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/autossh/services/scheduler.py` & `tensorpc-0.10.7/tensorpc/autossh/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/cli/cpuusage/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/cpuusage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/cpuusage/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/cpuusage/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/createmsg/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/createmsg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/createmsg/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/createmsg/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/free_port/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/free_port/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/gpuusage/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/gpuusage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/gpuusage/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/gpuusage/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/iperf/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/iperf/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/cli/ping/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/ping/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/proto_files/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/proto_files/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/proto_files/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/proto_files/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/proto_root/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/proto_root/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/proto_root/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/proto_root/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/pyls/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/pyls/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/cli/pyright_launch/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/pyright_launch/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/cli/start_worker/__init__.py` & `tensorpc-0.10.7/tensorpc/cli/start_worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/cli/start_worker/__main__.py` & `tensorpc-0.10.7/tensorpc/cli/start_worker/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/compat.py` & `tensorpc-0.10.7/tensorpc/compat.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/constants.py` & `tensorpc-0.10.7/tensorpc/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/__init__.py` & `tensorpc-0.10.7/tensorpc/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/core/asyncclient.py` & `tensorpc-0.10.7/tensorpc/core/asyncclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/core/asyncserver.py` & `tensorpc-0.10.7/tensorpc/core/asyncserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/core/bgserver.py` & `tensorpc-0.10.7/tensorpc/core/bgserver.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/client.py` & `tensorpc-0.10.7/tensorpc/core/client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/core_io.py` & `tensorpc-0.10.7/tensorpc/core/core_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import json
 import pickle
 from collections import abc
 from enum import Enum
 from functools import reduce
-from typing import Any, Callable, Dict, Hashable, List, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Hashable, List, Optional, Tuple, TypeVar, Union
 from typing_extensions import Literal
 
 import msgpack
 import numpy as np
 from tensorpc.protos_export import arraybuf_pb2, rpc_message_pb2, wsdef_pb2
 import traceback
 import numpy.typing as npt
@@ -185,15 +185,15 @@
         self.current_buf_length = -1
         self.current_buf_shape = None
         self.current_dtype = None
         self.func_key = None
         self.current_datas = []
         self.args = []
 
-    def __call__(self, buf):
+    def __call__(self, buf: rpc_message_pb2.RemoteCallStream):
         if buf.arg_id == 0:
             self.num_args = buf.num_args
         if buf.chunk_id == 0:
             self.current_buf_shape = list(buf.shape)
             self.current_buf_length = buf.num_chunk
             self.current_dtype = buf.dtype
             self.func_key = buf.func_key
@@ -301,30 +301,32 @@
 
 
 def _extract_arrays_from_data(arrays,
                               data,
                               object_classes=(np.ndarray, bytes),
                               json_index=False):
     # can't use abc.Sequence because string is sequence too.
+    data_skeleton: Optional[Union[List[Any], Dict[str, Any], Placeholder]]
     if isinstance(data, (list, tuple)):
         data_skeleton = [None] * len(data)
         for i in range(len(data)):
             e = data[i]
             if isinstance(e, object_classes):
                 if json_index:
                     data_skeleton[i] = {JSON_INDEX_KEY: len(arrays)}
                 else:
                     data_skeleton[i] = Placeholder(len(arrays), byte_size(e))
                 arrays.append(e)
             else:
                 data_skeleton[i] = _extract_arrays_from_data(
                     arrays, e, object_classes, json_index)
+        data_skeleton_res = data_skeleton
         if isinstance(data, tuple):
-            data_skeleton = tuple(data_skeleton)
-        return data_skeleton
+            data_skeleton_res = tuple(data_skeleton)
+        return data_skeleton_res
     elif isinstance(data, abc.Mapping):
         data_skeleton = {}
         for k, v in data.items():
             if isinstance(v, object_classes):
                 if json_index:
                     data_skeleton[k] = {JSON_INDEX_KEY: len(arrays)}
                 else:
@@ -348,15 +350,15 @@
             data_skeleton = data
         return data_skeleton
 
 
 def extract_arrays_from_data(data,
                              object_classes=(np.ndarray, bytes),
                              json_index=False):
-    arrays = []
+    arrays: List[Union[np.ndarray, bytes]] = []
     data_skeleton = _extract_arrays_from_data(arrays,
                                               data,
                                               object_classes=object_classes,
                                               json_index=json_index)
     return arrays, data_skeleton
 
 
@@ -505,22 +507,23 @@
     arrays, data_skeleton = extract_arrays_from_data(data)
     data_skeleton_bytes = pickle.dumps(data_skeleton)
     data_to_be_send = arrays + [data_skeleton_bytes]
     data_to_be_send = [data2pb(a, send_data=False) for a in data_to_be_send]
     sum_array_nbytes = 0
     array_buffers = []
     for i in range(len(arrays)):
-        if isinstance(arrays[i], bytes):
+        arr = arrays[i]
+        if isinstance(arr, bytes):
             sum_array_nbytes += len(arrays[i])
             array_buffers.append((arrays[i], len(arrays[i])))
         else:
-            if not arrays[i].flags['C_CONTIGUOUS']:
-                arrays[i] = np.ascontiguousarray(arrays[i])
-            sum_array_nbytes += arrays[i].nbytes
-            array_buffers.append((arrays[i].view(np.uint8), arrays[i].nbytes))
+            if not arr.flags['C_CONTIGUOUS']:
+                arrays[i] = np.ascontiguousarray(arr)
+            sum_array_nbytes += arr.nbytes
+            array_buffers.append((arr.view(np.uint8), arr.nbytes))
     if sum_array_nbytes + len(data_skeleton_bytes) > shared_mem.nbytes:
         x, y = sum_array_nbytes + len(data_skeleton_bytes), shared_mem.nbytes
         raise ValueError("your shared mem is too small: {} vs {}.".format(
             x, y))
     # assign datas to shared mem
     start = 0
     for a_buf, size in array_buffers:
@@ -732,15 +735,15 @@
     binary_view[1:5] = cnt_arr.tobytes()
     binary_view[5:req_msg_size + 5] = req.SerializeToString()
     return binary
 
 
 class SocketMessageEncoder:
     """
-    distflow socket message format
+    tensorpc socket message format
 
     0-1: msg type, can be rpc/event/error/raw
 
     if type is raw, following bytes are raw byte message.
 
     if not:
```

### Comparing `tensorpc-0.10.6/tensorpc/core/defs.py` & `tensorpc-0.10.7/tensorpc/core/defs.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/event_emitter/aio.py` & `tensorpc-0.10.7/tensorpc/core/event_emitter/aio.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/event_emitter/base.py` & `tensorpc-0.10.7/tensorpc/core/event_emitter/base.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/funcid.py` & `tensorpc-0.10.7/tensorpc/core/funcid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/httpclient.py` & `tensorpc-0.10.7/tensorpc/core/httpclient.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/httpservers/aiohttp_impl.py` & `tensorpc-0.10.7/tensorpc/core/httpservers/aiohttp_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         headers = {
             'Access-Control-Allow-Origin': '*',
             # 'Access-Control-Allow-Headers': '*',
             # 'Access-Control-Allow-Method': 'POST',
         }
         res = web.Response(body=byte, headers=headers)
         return res
-    
+
     async def fetch_status(self, request: web.Request):
         status = {
             "status": "ok",
         }
         # TODO better headers
         headers = {
             'Access-Control-Allow-Origin': '*',
```

### Comparing `tensorpc-0.10.6/tensorpc/core/httpservers/all.py` & `tensorpc-0.10.7/tensorpc/core/httpservers/all.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/httpservers/blacksheep_impl.py` & `tensorpc-0.10.7/tensorpc/core/httpservers/blacksheep_impl.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/httpservers/core.py` & `tensorpc-0.10.7/tensorpc/core/httpservers/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/inspecttools.py` & `tensorpc-0.10.7/tensorpc/core/inspecttools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/marker.py` & `tensorpc-0.10.7/tensorpc/core/marker.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/moduleid.py` & `tensorpc-0.10.7/tensorpc/core/moduleid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/core/prim.py` & `tensorpc-0.10.7/tensorpc/core/prim.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/server.py` & `tensorpc-0.10.7/tensorpc/core/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/core/server_core.py` & `tensorpc-0.10.7/tensorpc/core/server_core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/serviceunit.py` & `tensorpc-0.10.7/tensorpc/core/serviceunit.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/tracer.py` & `tensorpc-0.10.7/tensorpc/core/tracer.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/core/tree_id.py` & `tensorpc-0.10.7/tensorpc/core/tree_id.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/__init__.py` & `tensorpc-0.10.7/tensorpc/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/ai/__init__.py` & `tensorpc-0.10.7/tensorpc/examples/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/ai/engine.py` & `tensorpc-0.10.7/tensorpc/examples/ai/engine.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.12-App Context.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.12-App Context.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.4-Containers.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.4-Containers.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.0-Common Props.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.0-Common Props.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.1-Button.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.1-Button.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.10-Slider.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.10-Slider.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.11-Tab.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.11-Tab.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.12-Drawer.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.12-Drawer.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.13-Dialog.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.13-Dialog.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.14-Collapse.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.14-Collapse.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.15-Chip.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.15-Chip.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.16-Progress.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.16-Progress.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.17-MenuList.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.17-MenuList.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.2-Typography.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.2-Typography.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.25-Plotly.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.25-Plotly.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.26-Map.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.26-Map.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.3-Markdown.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.3-Markdown.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.4-TextField.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.4-TextField.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.5-List.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.5-List.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.6-Select.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.6-Select.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/02-components/2.9-Image.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/02-components/2.9-Image.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md` & `tensorpc-0.10.7/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/examples/tutorials.py` & `tensorpc-0.10.7/tensorpc/examples/tutorials.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/client.py` & `tensorpc-0.10.7/tensorpc/flow/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import dataclasses
 from typing import Any, AsyncGenerator, List, Optional, Tuple, Generator
 
+from tensorpc.core import prim
 from tensorpc.protos_export import rpc_message_pb2
 
 from ..utils.address import get_url_port
 from . import constants
 from .serv_names import serv_names
 from tensorpc.core.httpclient import http_remote_call_request
 import tensorpc
 
 import os
 import time
 from tensorpc.flow.coretypes import Message, MessageItem, MessageLevel, RelayUpdateNodeEvent
 import uuid
 
+import psutil 
 
 class MasterMeta:
 
     def __init__(self) -> None:
         gid = os.getenv(constants.TENSORPC_FLOW_GRAPH_ID)
         nid = os.getenv(constants.TENSORPC_FLOW_NODE_ID)
         nrid = os.getenv(constants.TENSORPC_FLOW_NODE_READABLE_ID)
@@ -85,14 +88,23 @@
         return self._node_readable_id
 
     @property
     def node_id(self):
         assert self._node_id is not None
         return self._node_id
 
+    @property
+    def process_title(self):
+        gport = self.grpc_port if self.grpc_port else 0
+        port = self.http_port if self.http_port else 0
+        app_meta = AppLocalMeta()
+        app_gport = app_meta.grpc_port if app_meta.grpc_port else 0
+        app_port = app_meta.http_port if app_meta.http_port else 0
+        return f"{constants.TENSORPC_FLOW_PROCESS_NAME_PREFIX}-{gport}-{port}-{app_gport}-{app_port}"
+
 
 class AppLocalMeta:
 
     def __init__(self) -> None:
         gport = os.getenv(constants.TENSORPC_FLOW_APP_GRPC_PORT)
         port = os.getenv(constants.TENSORPC_FLOW_APP_HTTP_PORT)
         self.module_name = os.getenv(constants.TENSORPC_FLOW_APP_MODULE_NAME,
@@ -105,14 +117,32 @@
             grpc_url = f"localhost:{gport}"
         self.grpc_port = gport
         self.http_port = port
         self.grpc_url = grpc_url
         self.http_url = url
         self.is_inside_devflow = gport is not None and port is not None and self.module_name != ""
 
+@dataclasses.dataclass
+class AppProcessMeta:
+    name: str 
+    pid: int
+    port: int 
+    grpc_port: int 
+    app_port: int 
+    app_grpc_port: int
+
+def list_all_app_in_machine():
+    res: List[AppProcessMeta] = []
+    for proc in psutil.process_iter(['pid', 'name']):
+        proc_name = proc.info["name"]
+        if proc_name.startswith(constants.TENSORPC_FLOW_PROCESS_NAME_PREFIX):
+            ports = list(map(int, proc_name.split("-")[1:]))
+            meta = AppProcessMeta(proc_name, proc.info["pid"], ports[0], ports[1], ports[2], ports[3])
+            res.append(meta)
+    return res 
 
 def is_inside_devflow():
     meta = MasterMeta()
     return meta.is_inside_devflow
 
 
 def is_inside_app_session():
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/close_langserv/__main__.py` & `tensorpc-0.10.7/tensorpc/flow/close_langserv/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/constants.py` & `tensorpc-0.10.7/tensorpc/flow/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -54,8 +54,11 @@
 
 # basic uid use ".", flexlayout use "#" and "-"
 # FIXME use safe key
 TENSORPC_FLOW_COMP_UID_TEMPLATE_SPLIT = "$&&"
 TENSORPC_FLOW_COMP_UID_STRUCTURE_SPLIT = ":"
 
 
-TENSORPC_FLOW_EFFECTS_OBSERVE = "TENSORPC_FLOW_EFFECTS_OBSERVE"
+TENSORPC_FLOW_EFFECTS_OBSERVE = "TENSORPC_FLOW_EFFECTS_OBSERVE"
+
+
+TENSORPC_FLOW_PROCESS_NAME_PREFIX = "__tensorpc_flow"
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/coretypes.py` & `tensorpc-0.10.7/tensorpc/flow/coretypes.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/app.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/appcore.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/appcore.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/canvas.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/appctx/inspector.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/appctx/inspector.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/colors.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/common.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/leaflet.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/leaflet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/mui.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/mui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plotly.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/arraycommon.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/arraycommon.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/arraygrid.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/arraygrid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/canvas.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/collection.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/collection.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/config.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/figure.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/common.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/common.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/monitor.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/monitor.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/layout.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/layout.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/reload.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/reload.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/tree.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/tree.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/options.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/options.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/reload_utils.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/reload_utils.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/scheduler.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/scheduler.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/scriptmgr.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/scriptmgr.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/sliders.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/sliders.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/tutorials.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/tutorials.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/canvas.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/treeview.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/treeview.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/three.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/three.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/threecore.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/threecore.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/components/typemetas.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/components/typemetas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/core.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/objtree.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/objtree.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/flowapp/reload.py` & `tensorpc-0.10.7/tensorpc/flow/flowapp/reload.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/init_langserv/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/init_langserv/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/jsonlike.py` & `tensorpc-0.10.7/tensorpc/flow/jsonlike.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/langserv/core.py` & `tensorpc-0.10.7/tensorpc/flow/langserv/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/langserv/pyls.py` & `tensorpc-0.10.7/tensorpc/flow/langserv/pyls.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/langserv/pyrightcfg.py` & `tensorpc-0.10.7/tensorpc/flow/langserv/pyrightcfg.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/marker.py` & `tensorpc-0.10.7/tensorpc/flow/marker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/runapp/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/runapp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/runapp/__main__.py` & `tensorpc-0.10.7/tensorpc/flow/runapp/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/app.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/arraygrid.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/arraygrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/collection.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/collection.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/d3.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/d3.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/file.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/sample_reload_fn.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/sample_reload_fn.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/sampleapp/v_nextgen.py` & `tensorpc-0.10.7/tensorpc/flow/sampleapp/v_nextgen.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/flow/serv/__init__.py` & `tensorpc-0.10.7/tensorpc/flow/serv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/serv/core.py` & `tensorpc-0.10.7/tensorpc/flow/serv/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/serv/flowapp.py` & `tensorpc-0.10.7/tensorpc/flow/serv/flowapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,15 +32,15 @@
 from tensorpc.core import marker
 from tensorpc.core.httpclient import http_remote_call
 from tensorpc.core.serviceunit import AppFuncType, ReloadableDynamicClass, ServiceUnit
 import tensorpc
 from tensorpc.flow.flowapp.reload import AppReloadManager, FlowSpecialMethods
 
 from tensorpc.flow.langserv import close_tmux_lang_server, get_tmux_lang_server_info_may_create
-from ..client import MasterMeta
+from ..client import AppLocalMeta, MasterMeta
 from tensorpc import prim
 from tensorpc.flow.serv_names import serv_names
 from tensorpc.core.serviceunit import ServiceEventType
 import traceback
 import time
 import sys 
 from urllib import parse
@@ -61,14 +61,21 @@
         # print(module_name, config)
         if external_argv is not None:
             print("external_argv", external_argv)
         self.module_name = module_name
         self.config = config
         self.shutdown_ev = asyncio.Event()
         self.master_meta = MasterMeta()
+        self.app_meta = AppLocalMeta()
+        process_title = self.master_meta.process_title
+        try:
+            import setproctitle
+            setproctitle.setproctitle(process_title)
+        except ImportError:
+            pass 
         if not headless:
             assert self.master_meta.is_inside_devflow, "this service must run inside devflow"
             # assert self.master_meta.is_http_valid
         self._send_loop_task: Optional[asyncio.Task] = None
         self._need_to_send_env: Optional[AppEvent] = None
         self.shutdown_ev.clear()
         if not headless:
@@ -116,15 +123,15 @@
     @marker.mark_server_event(event_type=marker.ServiceEventType.Init)
     async def init(self):
         if self.app._force_special_layout_method:
             layout_created = False
             special_methods = FlowSpecialMethods(self.app_su.serv_metas)
             if special_methods.create_layout is not None:
                 await self.app._app_run_layout_function(
-                    decorator_fn=special_methods.create_layout.fn)
+                    decorator_fn=special_methods.create_layout.get_binded_fn())
                 layout_created = True
             if not layout_created:
                 await self.app._app_run_layout_function()
         else:
             self.app.root._attach(UniqueTreeId.from_parts(["root"]), self.app._flow_app_comp_core)
         # print(lay["layout"])
         self.app.app_initialize()
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/serv/worker.py` & `tensorpc-0.10.7/tensorpc/flow/serv/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/flow/serv_names.py` & `tensorpc-0.10.7/tensorpc/flow/serv_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/protos/arraybuf_pb2.py` & `tensorpc-0.10.7/tensorpc/protos/arraybuf_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/arraybuf_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos/arraybuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/remote_object_pb2.py` & `tensorpc-0.10.7/tensorpc/protos/remote_object_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/remote_object_pb2_grpc.py` & `tensorpc-0.10.7/tensorpc/protos/remote_object_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/rpc_message_pb2.py` & `tensorpc-0.10.7/tensorpc/protos/rpc_message_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/rpc_message_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos/rpc_message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/wsdef_pb2.py` & `tensorpc-0.10.7/tensorpc/protos/wsdef_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos/wsdef_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos/wsdef_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/arraybuf_pb2.py` & `tensorpc-0.10.7/tensorpc/protos_legacy/arraybuf_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/arraybuf_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos_legacy/arraybuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/remote_object_pb2.py` & `tensorpc-0.10.7/tensorpc/protos_legacy/remote_object_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/remote_object_pb2_grpc.py` & `tensorpc-0.10.7/tensorpc/protos_legacy/remote_object_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/rpc_message_pb2.py` & `tensorpc-0.10.7/tensorpc/protos_legacy/rpc_message_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/rpc_message_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos_legacy/rpc_message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/wsdef_pb2.py` & `tensorpc-0.10.7/tensorpc/protos_legacy/wsdef_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/protos_legacy/wsdef_pb2.pyi` & `tensorpc-0.10.7/tensorpc/protos_legacy/wsdef_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/serve/__init__.py` & `tensorpc-0.10.7/tensorpc/serve/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/serve/__main__.py` & `tensorpc-0.10.7/tensorpc/serve/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/serve/flowapp_script/__main__.py` & `tensorpc-0.10.7/tensorpc/serve/flowapp_script/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/serve_sync/__main__.py` & `tensorpc-0.10.7/tensorpc/serve_sync/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     fire.Fire(serve_in_terminal)
 
 
 def ping(ip: str):
     with RemoteManager(ip) as robj:
         t = time.time()
         robj.health_check()
-        print("[distflow.ping]{} response time: {:.4f}ms".format(
+        print("[tensorpc.ping]{} response time: {:.4f}ms".format(
             ip, 1000 * (time.time() - t)))
 
 
 def ping_main():
     fire.Fire(ping)
```

### Comparing `tensorpc-0.10.6/tensorpc/services/__init__.py` & `tensorpc-0.10.7/tensorpc/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/services/collection.py` & `tensorpc-0.10.7/tensorpc/services/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/services/flow/__init__.py` & `tensorpc-0.10.7/tensorpc/services/flow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/services/flow/core.py` & `tensorpc-0.10.7/tensorpc/services/flow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/services/for_test.py` & `tensorpc-0.10.7/tensorpc/services/for_test.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/services/vis.py` & `tensorpc-0.10.7/tensorpc/services/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/tools.py` & `tensorpc-0.10.7/tensorpc/tools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/utils/__init__.py` & `tensorpc-0.10.7/tensorpc/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/utils/df_logging.py` & `tensorpc-0.10.7/tensorpc/utils/df_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     _logger_lock.acquire()
 
     try:
         if _logger:
             return _logger
 
         # Scope the TensorFlow logger to not conflict with users' loggers.
-        logger = _logging.getLogger('distflow')
+        logger = _logging.getLogger('tensorpc')
 
         # Override findCaller on the logger to skip internal helper functions
         logger.findCaller = _logger_find_caller
 
         # Don't further configure the TensorFlow logger if the root logger is
         # already configured. This prevents double logging in those cases.
         if not _logging.getLogger().handlers:
```

### Comparing `tensorpc-0.10.6/tensorpc/utils/gpuusage.py` & `tensorpc-0.10.7/tensorpc/utils/gpuusage.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/utils/registry.py` & `tensorpc-0.10.7/tensorpc/utils/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/utils/reload.py` & `tensorpc-0.10.7/tensorpc/utils/reload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/utils/subproc.py` & `tensorpc-0.10.7/tensorpc/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc/utils/uniquename.py` & `tensorpc-0.10.7/tensorpc/utils/uniquename.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Yan Yan
+# Copyright 2024 Yan Yan
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tensorpc-0.10.6/tensorpc/utils/wait_tools.py` & `tensorpc-0.10.7/tensorpc/utils/wait_tools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/tensorpc.egg-info/PKG-INFO` & `tensorpc-0.10.7/tensorpc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorpc
-Version: 0.10.6
+Version: 0.10.7
 Summary: Backend for devflow.
 Home-page: https://github.com/FindDefinition/tensorpc
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `tensorpc-0.10.6/tensorpc.egg-info/SOURCES.txt` & `tensorpc-0.10.7/tensorpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.6/test/test_tmux_scheduler.py` & `tensorpc-0.10.7/test/test_tmux_scheduler.py`

 * *Files identical despite different names*

