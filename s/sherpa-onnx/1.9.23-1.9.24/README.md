# Comparing `tmp/sherpa-onnx-1.9.23.tar.gz` & `tmp/sherpa-onnx-1.9.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.9.23.tar", last modified: Thu Apr 25 10:04:07 2024, max compression
+gzip compressed data, was "sherpa-onnx-1.9.24.tar", last modified: Sat May 11 04:35:14 2024, max compression
```

## Comparing `sherpa-onnx-1.9.23.tar` & `sherpa-onnx-1.9.24.tar`

### file list

```diff
@@ -1,528 +1,541 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.545154 sherpa-onnx-1.9.23/
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-25 10:04:07.545154 sherpa-onnx-1.9.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.473154 sherpa-onnx-1.9.23/c-api-examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/add-punctuation-c-api.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.477154 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/c-api-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/audio-tagging-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/decode-file-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/offline-tts-c-api.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/speaker-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/spoken-language-identification-c-api.c
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/c-api-examples/streaming-hlg-decode-file-c-api.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.481154 sherpa-onnx-1.9.23/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/asio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/cargs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/cppjieba.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/espeak-ng-for-piper.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/kaldi-decoder.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/kaldi-native-fbank.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/kaldifst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-aarch64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-arm-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-riscv64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-riscv64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-arm64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-arm64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-universal-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-universal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-x86_64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-osx-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-wasm-simd.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-gpu.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86-static-debug.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86-static.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/onnxruntime.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/openfst.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/piper-phonemize.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/portaudio.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/sherpa-onnx-no-tts.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/sherpa-onnx.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/cmake/websocketpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:04:07.545154 sherpa-onnx-1.9.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.481154 sherpa-onnx-1.9.23/sherpa-onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.481154 sherpa-onnx-1.9.23/sherpa-onnx/c-api/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/c-api/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    42366 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/c-api/c-api.cc
--rw-r--r--   0 runner    (1001) docker     (127)    45819 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/c-api/c-api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.525154 sherpa-onnx-1.9.23/sherpa-onnx/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa-play.h
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-ced-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-label-file.cc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-label-file.h
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/base64-decode.cc
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/base64-decode.h
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat.cc
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat.h
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/cppjieba-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/file-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/file-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/hypothesis.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/hypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/jieba-lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/jieba-lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/log.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/math.h
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/microphone.h
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ced-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ced-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-character-frontend.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-character-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-frontend.h
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-conformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-conformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lstm-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lstm-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-rnn-lm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-rnn-lm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-client.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/onnx-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/onnx-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence.cc
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/parse-options.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/parse-options.h
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-lexicon.h
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/provider.cc
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/provider.h
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/resample.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/resample.h
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/session.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/session.h
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice.h
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack.cc
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack.h
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/symbol-table.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/symbol-table.h
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/tee-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/text-utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/text-utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/transducer-keyword-decoder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/transducer-keyword-decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose.cc
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind.cc
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/utfcpp-test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-reader.cc
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-reader.h
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.529154 sherpa-onnx-1.9.23/sherpa-onnx/jni/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/jni.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/jni/wave-reader.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.529154 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/AudioTagging.kt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/FeatureConfig.kt
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/KeywordSpotter.kt
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OfflineRecognizer.kt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OfflineStream.kt
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OnlineRecognizer.kt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OnlineStream.kt
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/Speaker.kt
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/Vad.kt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/WaveReader.kt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.529154 sherpa-onnx-1.9.23/sherpa-onnx/python/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.541154 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/alsa.h
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/audio-tagging.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/audio-tagging.h
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/circular-buffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/circular-buffer.h
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/display.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/display.h
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/endpoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/endpoint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/faked-alsa.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/features.cc
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/features.h
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/keyword-spotter.cc
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/keyword-spotter.h
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-punctuation.cc
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-punctuation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts.h
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-whisper-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-lm-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-lm-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-paraformer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-recognizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-recognizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-stream.h
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-transducer-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-transducer-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/sherpa-onnx.cc
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/sherpa-onnx.h
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/silero-vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/silero-vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/spoken-language-identification.cc
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/spoken-language-identification.h
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model-config.cc
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model-config.h
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model.cc
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model.h
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/voice-activity-detector.cc
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/voice-activity-detector.h
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/wave-writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/wave-writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.541154 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.545154 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_feature_extractor_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_keyword_spotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_offline_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_online_recognizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_online_transducer_model_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7132 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_speaker_recognition.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-04-25 09:54:36.000000 sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_text2token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:04:07.545154 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 10:04:07.000000 sherpa-onnx-1.9.23/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.886140 sherpa-onnx-1.9.24/
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-11 04:35:14.886140 sherpa-onnx-1.9.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.814140 sherpa-onnx-1.9.24/c-api-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/add-punctuation-c-api.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.814140 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/c-api-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/audio-tagging-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/decode-file-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/offline-tts-c-api.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1952 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/speaker-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/spoken-language-identification-c-api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/c-api-examples/streaming-hlg-decode-file-c-api.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.818140 sherpa-onnx-1.9.24/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/asio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/cargs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/cppjieba.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/espeak-ng-for-piper.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/kaldi-decoder.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/kaldi-native-fbank.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/kaldifst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-aarch64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-arm-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-riscv64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-riscv64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-arm64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-arm64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-universal-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-universal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-x86_64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-osx-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-wasm-simd.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-gpu.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86-static-debug.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86-static.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/onnxruntime.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/openfst.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/piper-phonemize.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/portaudio.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/sherpa-onnx-no-tts.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/sherpa-onnx.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/cmake/websocketpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:35:14.886140 sherpa-onnx-1.9.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.818140 sherpa-onnx-1.9.24/sherpa-onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.822140 sherpa-onnx-1.9.24/sherpa-onnx/c-api/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/c-api/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    42366 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/c-api/c-api.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    45819 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/c-api/c-api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.866140 sherpa-onnx-1.9.24/sherpa-onnx/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa-play.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-ced-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-label-file.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-label-file.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/base64-decode.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/base64-decode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/cppjieba-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/file-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/file-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/hypothesis.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/hypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/jieba-lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/jieba-lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/log.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/math.h
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/microphone.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ced-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ced-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-character-frontend.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-character-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-frontend.h
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-conformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-conformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lstm-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lstm-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-nemo-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-nemo-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-nemo-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-nemo-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-ctc-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-transducer-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-rnn-lm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-rnn-lm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-client.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13906 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-transducer-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/onnx-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/onnx-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/parse-options.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/parse-options.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-lexicon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-lexicon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/provider.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/provider.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/resample.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/resample.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/session.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/session.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/symbol-table.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/symbol-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/tee-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/text-utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/text-utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/transducer-keyword-decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/transducer-keyword-decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind.h
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/utfcpp-test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.870140 sherpa-onnx-1.9.24/sherpa-onnx/jni/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/jni.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/jni/wave-reader.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.870140 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/AudioTagging.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/FeatureConfig.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/KeywordSpotter.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OfflinePunctuation.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OfflineRecognizer.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OfflineStream.kt
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OnlineRecognizer.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OnlineStream.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/Speaker.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/Vad.kt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/WaveReader.kt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.870140 sherpa-onnx-1.9.24/sherpa-onnx/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.882140 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/alsa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/audio-tagging.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/audio-tagging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/circular-buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/circular-buffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/display.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/display.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/endpoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/endpoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/faked-alsa.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/features.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/keyword-spotter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/keyword-spotter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-punctuation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-punctuation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tdnn-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-vits-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts.h
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-whisper-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-whisper-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-lm-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-lm-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-nemo-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-paraformer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-paraformer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-recognizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-recognizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-transducer-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-transducer-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/sherpa-onnx.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/sherpa-onnx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/silero-vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/silero-vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-manager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/spoken-language-identification.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/spoken-language-identification.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model-config.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model-config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/voice-activity-detector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/voice-activity-detector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/wave-writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/wave-writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.882140 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.886140 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      851 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_feature_extractor_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7548 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_keyword_spotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12338 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_offline_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10928 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_online_recognizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      772 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_online_transducer_model_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7132 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_speaker_recognition.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3905 2024-05-11 04:25:11.000000 sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_text2token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:35:14.886140 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 04:35:14.000000 sherpa-onnx-1.9.24/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.9.23/CMakeLists.txt` & `sherpa-onnx-1.9.24/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_minimum_required(VERSION 3.13 FATAL_ERROR)
 project(sherpa-onnx)
 
-set(SHERPA_ONNX_VERSION "1.9.23")
+set(SHERPA_ONNX_VERSION "1.9.24")
 
 # Disable warning about
 #
 # "The DOWNLOAD_EXTRACT_TIMESTAMP option was not given and policy CMP0135 is
 #  not set.
 if (CMAKE_VERSION VERSION_GREATER_EQUAL "3.24.0")
   cmake_policy(SET CMP0135 NEW)
@@ -262,14 +262,15 @@
   include(piper-phonemize)
   include(cppjieba) # For Chinese TTS. It is a header-only C++ library
 endif()
 
 add_subdirectory(sherpa-onnx)
 
 if(SHERPA_ONNX_ENABLE_C_API AND SHERPA_ONNX_ENABLE_BINARY)
+  set(SHERPA_ONNX_PKG_WITH_CARGS "-lcargs")
   add_subdirectory(c-api-examples)
 endif()
 
 if(SHERPA_ONNX_ENABLE_WASM)
   add_subdirectory(wasm)
 endif()
```

### Comparing `sherpa-onnx-1.9.23/LICENSE` & `sherpa-onnx-1.9.24/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/CMakeLists.txt` & `sherpa-onnx-1.9.24/c-api-examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/README.md` & `sherpa-onnx-1.9.24/c-api-examples/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/add-punctuation-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/add-punctuation-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/alsa.cc` & `sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/alsa.h` & `sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/asr-microphone-example/c-api-alsa.cc` & `sherpa-onnx-1.9.24/c-api-examples/asr-microphone-example/c-api-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/audio-tagging-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/audio-tagging-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/decode-file-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/offline-tts-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/offline-tts-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/run.sh` & `sherpa-onnx-1.9.24/c-api-examples/run.sh`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/speaker-identification-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/speaker-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/spoken-language-identification-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/spoken-language-identification-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/c-api-examples/streaming-hlg-decode-file-c-api.c` & `sherpa-onnx-1.9.24/c-api-examples/streaming-hlg-decode-file-c-api.c`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/asio.cmake` & `sherpa-onnx-1.9.24/cmake/asio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/cargs.cmake` & `sherpa-onnx-1.9.24/cmake/cargs.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/cmake_extension.py` & `sherpa-onnx-1.9.24/cmake/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/cppjieba.cmake` & `sherpa-onnx-1.9.24/cmake/cppjieba.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/eigen.cmake` & `sherpa-onnx-1.9.24/cmake/eigen.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/espeak-ng-for-piper.cmake` & `sherpa-onnx-1.9.24/cmake/espeak-ng-for-piper.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/googletest.cmake` & `sherpa-onnx-1.9.24/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/kaldi-decoder.cmake` & `sherpa-onnx-1.9.24/cmake/kaldi-decoder.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/kaldi-native-fbank.cmake` & `sherpa-onnx-1.9.24/cmake/kaldi-native-fbank.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/kaldifst.cmake` & `sherpa-onnx-1.9.24/cmake/kaldifst.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-aarch64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-aarch64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-aarch64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-arm-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-arm-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-arm.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-arm.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-riscv64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-riscv64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-riscv64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-riscv64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64-gpu.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-linux-x86_64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-linux-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-arm64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-arm64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-arm64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-arm64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-universal-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-universal-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-universal.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-universal.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-x86_64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-x86_64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-osx-x86_64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-osx-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-wasm-simd.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-wasm-simd.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-gpu.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-gpu.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-static-debug.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x64.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x64.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86-static-debug.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86-static-debug.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86-static.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86-static.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime-win-x86.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime-win-x86.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/onnxruntime.cmake` & `sherpa-onnx-1.9.24/cmake/onnxruntime.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/openfst.cmake` & `sherpa-onnx-1.9.24/cmake/openfst.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/piper-phonemize.cmake` & `sherpa-onnx-1.9.24/cmake/piper-phonemize.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/portaudio.cmake` & `sherpa-onnx-1.9.24/cmake/portaudio.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/pybind11.cmake` & `sherpa-onnx-1.9.24/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/cmake/sherpa-onnx-no-tts.pc.in` & `sherpa-onnx-1.9.24/cmake/sherpa-onnx.pc.in`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 prefix="@CMAKE_INSTALL_PREFIX@"
 exec_prefix="${prefix}"
 includedir="${prefix}/include"
 libdir="${exec_prefix}/lib"
 
 Name: sherpa-onnx
-Description: pkg-config for sherpa-onnx with TTS support
+Description: pkg-config for sherpa-onnx
 URL: https://github.com/k2-fsa/sherpa-onnx
 
 Version: @SHERPA_ONNX_VERSION@
 Cflags: -I"${includedir}"
 
 # Note: -lcargs is required only for the following file
 # https://github.com/k2-fsa/sherpa-onnx/blob/master/c-api-examples/decode-file-c-api.c
 # We add it here so that users don't need to specify -lcargs when compiling decode-file-c-api.c
-Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fst -lkaldi-native-fbank-core -lcargs -lonnxruntime -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
+Libs: -L"${libdir}" -lsherpa-onnx-c-api -lsherpa-onnx-core -lkaldi-decoder-core -lsherpa-onnx-kaldifst-core -lsherpa-onnx-fstfar -lsherpa-onnx-fst -lkaldi-native-fbank-core -lpiper_phonemize -lespeak-ng -lucd -lonnxruntime -Wl,-rpath,${libdir} @SHERPA_ONNX_PKG_WITH_CARGS@ @SHERPA_ONNX_PKG_CONFIG_EXTRA_LIBS@
```

### Comparing `sherpa-onnx-1.9.23/cmake/websocketpp.cmake` & `sherpa-onnx-1.9.24/cmake/websocketpp.cmake`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/setup.py` & `sherpa-onnx-1.9.24/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/c-api/c-api.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/c-api/c-api.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/c-api/c-api.h` & `sherpa-onnx-1.9.24/sherpa-onnx/c-api/c-api.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,19 @@
   offline-recognizer-impl.cc
   offline-recognizer.cc
   offline-rnn-lm.cc
   offline-stream.cc
   offline-tdnn-ctc-model.cc
   offline-tdnn-model-config.cc
   offline-transducer-greedy-search-decoder.cc
+  offline-transducer-greedy-search-nemo-decoder.cc
   offline-transducer-model-config.cc
   offline-transducer-model.cc
   offline-transducer-modified-beam-search-decoder.cc
+  offline-transducer-nemo-model.cc
   offline-wenet-ctc-model-config.cc
   offline-wenet-ctc-model.cc
   offline-whisper-greedy-search-decoder.cc
   offline-whisper-model-config.cc
   offline-whisper-model.cc
   offline-zipformer-ctc-model-config.cc
   offline-zipformer-ctc-model.cc
@@ -55,14 +57,16 @@
   online-ctc-fst-decoder.cc
   online-ctc-greedy-search-decoder.cc
   online-ctc-model.cc
   online-lm-config.cc
   online-lm.cc
   online-lstm-transducer-model.cc
   online-model-config.cc
+  online-nemo-ctc-model-config.cc
+  online-nemo-ctc-model.cc
   online-paraformer-model-config.cc
   online-paraformer-model.cc
   online-recognizer-impl.cc
   online-recognizer.cc
   online-rnn-lm.cc
   online-stream.cc
   online-transducer-decoder.cc
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/README.md` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/README.md`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa-play.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa-play.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa-play.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/alsa.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/alsa.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-ced-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-ced-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-label-file.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-label-file.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-label-file.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-label-file.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging-zipformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/audio-tagging.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/audio-tagging.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/base64-decode.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/base64-decode.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/cat.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/cat.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/circular-buffer.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/circular-buffer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/context-graph.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/context-graph.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/cppjieba-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/cppjieba-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/display.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/display.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/endpoint.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/endpoint.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/endpoint.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/features.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/features.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/features.h`

 * *Files 24% similar despite different names*

```diff
@@ -52,14 +52,27 @@
   bool snip_edges = false;
   float frame_shift_ms = 10.0f;   // in milliseconds.
   float frame_length_ms = 25.0f;  // in milliseconds.
   bool is_librosa = false;
   bool remove_dc_offset = true;       // Subtract mean of wave before FFT.
   std::string window_type = "povey";  // e.g. Hamming window
 
+  // For models from NeMo
+  // This option is not exposed and is set internally when loading models.
+  // Possible values:
+  // - per_feature
+  // - all_features (not implemented yet)
+  // - fixed_mean (not implemented)
+  // - fixed_std (not implemented)
+  // - or just leave it to empty
+  // See
+  // https://github.com/NVIDIA/NeMo/blob/main/nemo/collections/asr/parts/preprocessing/features.py#L59
+  // for details
+  std::string nemo_normalize_type;
+
   std::string ToString() const;
 
   void Register(ParseOptions *po);
 };
 
 class FeatureExtractor {
  public:
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/file-utils.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/file-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/file-utils.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/file-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/hypothesis.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/hypothesis.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/hypothesis.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/hypothesis.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/jieba-lexicon.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/jieba-lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/jieba-lexicon.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/jieba-lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter-transducer-impl.h`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 class KeywordSpotterTransducerImpl : public KeywordSpotterImpl {
  public:
   explicit KeywordSpotterTransducerImpl(const KeywordSpotterConfig &config)
       : config_(config),
         model_(OnlineTransducerModel::Create(config.model_config)),
         sym_(config.model_config.tokens) {
-    if (sym_.contains("<unk>")) {
+    if (sym_.Contains("<unk>")) {
       unk_id_ = sym_["<unk>"];
     }
 
     model_->SetFeatureDim(config.feat_config.feature_dim);
 
     InitKeywords();
 
@@ -83,15 +83,15 @@
 
 #if __ANDROID_API__ >= 9
   KeywordSpotterTransducerImpl(AAssetManager *mgr,
                                const KeywordSpotterConfig &config)
       : config_(config),
         model_(OnlineTransducerModel::Create(mgr, config.model_config)),
         sym_(mgr, config.model_config.tokens) {
-    if (sym_.contains("<unk>")) {
+    if (sym_.Contains("<unk>")) {
       unk_id_ = sym_["<unk>"];
     }
 
     model_->SetFeatureDim(config.feat_config.feature_dim);
 
     InitKeywords(mgr);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/keyword-spotter.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/keyword-spotter.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/lexicon.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/lexicon.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/log.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/log.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/log.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/log.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/macros.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/macros.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/math.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/math.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/microphone.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ced-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ced-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ced-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ced-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ct-transformer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ct-transformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-fst-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-model.cc`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #include "sherpa-onnx/csrc/offline-zipformer-ctc-model.h"
 #include "sherpa-onnx/csrc/onnx-utils.h"
 
 namespace {
 
 enum class ModelType {
   kEncDecCTCModelBPE,
+  kEncDecHybridRNNTCTCBPEModel,
   kTdnn,
   kZipformerCtc,
   kWenetCtc,
   kUnknown,
 };
 
 }  // namespace
@@ -51,25 +52,30 @@
   auto model_type =
       meta_data.LookupCustomMetadataMapAllocated("model_type", allocator);
   if (!model_type) {
     SHERPA_ONNX_LOGE(
         "No model_type in the metadata!\n"
         "If you are using models from NeMo, please refer to\n"
         "https://huggingface.co/csukuangfj/"
-        "sherpa-onnx-nemo-ctc-en-citrinet-512/blob/main/add-model-metadata.py"
+        "sherpa-onnx-nemo-ctc-en-citrinet-512/blob/main/add-model-metadata.py\n"
+        "or "
+        "https://github.com/k2-fsa/sherpa-onnx/tree/master/scripts/nemo/"
+        "fast-conformer-hybrid-transducer-ctc\n"
         "If you are using models from WeNet, please refer to\n"
         "https://github.com/k2-fsa/sherpa-onnx/blob/master/scripts/wenet/"
         "run.sh\n"
         "\n"
         "for how to add metadta to model.onnx\n");
     return ModelType::kUnknown;
   }
 
   if (model_type.get() == std::string("EncDecCTCModelBPE")) {
     return ModelType::kEncDecCTCModelBPE;
+  } else if (model_type.get() == std::string("EncDecHybridRNNTCTCBPEModel")) {
+    return ModelType::kEncDecHybridRNNTCTCBPEModel;
   } else if (model_type.get() == std::string("tdnn")) {
     return ModelType::kTdnn;
   } else if (model_type.get() == std::string("zipformer2_ctc")) {
     return ModelType::kZipformerCtc;
   } else if (model_type.get() == std::string("wenet_ctc")) {
     return ModelType::kWenetCtc;
   } else {
@@ -102,14 +108,17 @@
     model_type = GetModelType(buffer.data(), buffer.size(), config.debug);
   }
 
   switch (model_type) {
     case ModelType::kEncDecCTCModelBPE:
       return std::make_unique<OfflineNemoEncDecCtcModel>(config);
       break;
+    case ModelType::kEncDecHybridRNNTCTCBPEModel:
+      return std::make_unique<OfflineNemoEncDecHybridRNNTCTCBPEModel>(config);
+      break;
     case ModelType::kTdnn:
       return std::make_unique<OfflineTdnnCtcModel>(config);
       break;
     case ModelType::kZipformerCtc:
       return std::make_unique<OfflineZipformerCtcModel>(config);
       break;
     case ModelType::kWenetCtc:
@@ -149,14 +158,17 @@
     model_type = GetModelType(buffer.data(), buffer.size(), config.debug);
   }
 
   switch (model_type) {
     case ModelType::kEncDecCTCModelBPE:
       return std::make_unique<OfflineNemoEncDecCtcModel>(mgr, config);
       break;
+    case ModelType::kEncDecHybridRNNTCTCBPEModel:
+      return std::make_unique<OfflineNemoEncDecHybridRNNTCTCBPEModel>(config);
+      break;
     case ModelType::kTdnn:
       return std::make_unique<OfflineTdnnCtcModel>(mgr, config);
       break;
     case ModelType::kZipformerCtc:
       return std::make_unique<OfflineZipformerCtcModel>(mgr, config);
       break;
     case ModelType::kWenetCtc:
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-lm.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.cc
 //
-// Copyright (c)  2023  Xiaomi Corporation
+// Copyright (c)  2023-2024  Xiaomi Corporation
 
 #include "sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h"
 
 #include "sherpa-onnx/csrc/macros.h"
 #include "sherpa-onnx/csrc/onnx-utils.h"
 #include "sherpa-onnx/csrc/session.h"
 #include "sherpa-onnx/csrc/text-utils.h"
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-nemo-enc-dec-ctc-model.h`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,12 @@
   std::string FeatureNormalizationMethod() const override;
 
  private:
   class Impl;
   std::unique_ptr<Impl> impl_;
 };
 
+using OfflineNemoEncDecHybridRNNTCTCBPEModel = OfflineNemoEncDecCtcModel;
+
 }  // namespace sherpa_onnx
 
 #endif  // SHERPA_ONNX_CSRC_OFFLINE_NEMO_ENC_DEC_CTC_MODEL_H_
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.cc`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
       results[i].tokens.push_back(max_idx);
 
       p += vocab_size;
     }
 
     if (us_cif_peak) {
-      int32_t dim = us_cif_peak.GetTensorTypeAndShapeInfo().GetShape()[1];
+      int32_t dim = us_cif_peak.GetTensorTypeAndShapeInfo().GetShape().back();
 
       const auto *peak = us_cif_peak.GetTensorData<float>() + i * dim;
       std::vector<float> timestamps;
       timestamps.reserve(results[i].tokens.size());
 
       // 10.0: frameshift is 10 milliseconds
       // 6: LfrWindowSize
@@ -53,15 +53,18 @@
       float scale = 10.0 * 6 / 3 / 1000;
 
       for (int32_t k = 0; k != dim; ++k) {
         if (peak[k] > 1 - 1e-4) {
           timestamps.push_back(k * scale);
         }
       }
-      timestamps.pop_back();
+
+      if (!timestamps.empty()) {
+        timestamps.pop_back();
+      }
 
       if (timestamps.size() == results[i].tokens.size()) {
         results[i].timestamps = std::move(timestamps);
       } else {
         SHERPA_ONNX_LOGE("time stamp for batch: %d, %d vs %d", i,
                          static_cast<int32_t>(results[i].tokens.size()),
                          static_cast<int32_t>(timestamps.size()));
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-paraformer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 // sherpa-onnx/csrc/offline-punctuation-ct-transformer-impl.h
 //
 // Copyright (c)  2024  Xiaomi Corporation
 #ifndef SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_CT_TRANSFORMER_IMPL_H_
 #define SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_CT_TRANSFORMER_IMPL_H_
 
+#include <math.h>
+
 #include <memory>
 #include <string>
 #include <utility>
 #include <vector>
 
+#if __ANDROID_API__ >= 9
+#include "android/asset_manager.h"
+#include "android/asset_manager_jni.h"
+#endif
+
 #include "sherpa-onnx/csrc/macros.h"
 #include "sherpa-onnx/csrc/math.h"
 #include "sherpa-onnx/csrc/offline-ct-transformer-model.h"
 #include "sherpa-onnx/csrc/offline-punctuation-impl.h"
 #include "sherpa-onnx/csrc/offline-punctuation.h"
 #include "sherpa-onnx/csrc/text-utils.h"
 
@@ -20,14 +27,20 @@
 
 class OfflinePunctuationCtTransformerImpl : public OfflinePunctuationImpl {
  public:
   explicit OfflinePunctuationCtTransformerImpl(
       const OfflinePunctuationConfig &config)
       : config_(config), model_(config.model) {}
 
+#if __ANDROID_API__ >= 9
+  OfflinePunctuationCtTransformerImpl(AAssetManager *mgr,
+                                      const OfflinePunctuationConfig &config)
+      : config_(config), model_(mgr, config.model) {}
+#endif
+
   std::string AddPunctuation(const std::string &text) const override {
     if (text.empty()) {
       return {};
     }
 
     std::vector<std::string> tokens = SplitUtf8(text);
     std::vector<int32_t> token_ids;
@@ -45,15 +58,17 @@
     }
 
     auto memory_info =
         Ort::MemoryInfo::CreateCpu(OrtDeviceAllocator, OrtMemTypeDefault);
 
     int32_t segment_size = 20;
     int32_t max_len = 200;
-    int32_t num_segments = (token_ids.size() + segment_size - 1) / segment_size;
+    int32_t num_segments =
+        ceil((static_cast<float>(token_ids.size()) + segment_size - 1) /
+             segment_size);
 
     std::vector<int32_t> punctuations;
     int32_t last = -1;
     for (int32_t i = 0; i != num_segments; ++i) {
       int32_t this_start = i * segment_size;         // inclusive
       int32_t this_end = this_start + segment_size;  // exclusive
       if (this_end > token_ids.size()) {
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-decoder.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-// sherpa-onnx/csrc/offline-punctuation-impl.h
+// sherpa-onnx/csrc/online-paraformer-decoder.h
 //
-// Copyright (c)  2024  Xiaomi Corporation
-#ifndef SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
-#define SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
+// Copyright (c)  2023  Xiaomi Corporation
+
+#ifndef SHERPA_ONNX_CSRC_ONLINE_PARAFORMER_DECODER_H_
+#define SHERPA_ONNX_CSRC_ONLINE_PARAFORMER_DECODER_H_
 
-#include <memory>
-#include <string>
 #include <vector>
 
-#include "sherpa-onnx/csrc/offline-punctuation.h"
+#include "onnxruntime_cxx_api.h"  // NOLINT
 
 namespace sherpa_onnx {
 
-class OfflinePunctuationImpl {
- public:
-  virtual ~OfflinePunctuationImpl() = default;
-
-  static std::unique_ptr<OfflinePunctuationImpl> Create(
-      const OfflinePunctuationConfig &config);
+struct OnlineParaformerDecoderResult {
+  /// The decoded token IDs
+  std::vector<int32_t> tokens;
 
-  virtual std::string AddPunctuation(const std::string &text) const = 0;
+  int32_t last_non_blank_frame_index = 0;
 };
 
 }  // namespace sherpa_onnx
 
-#endif  // SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
+#endif  // SHERPA_ONNX_CSRC_ONLINE_PARAFORMER_DECODER_H_
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation-impl.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,36 @@
-// sherpa-onnx/csrc/offline-punctuation.cc
+// sherpa-onnx/csrc/offline-punctuation-impl.h
 //
 // Copyright (c)  2024  Xiaomi Corporation
+#ifndef SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
+#define SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
 
-#include "sherpa-onnx/csrc/offline-punctuation.h"
+#include <memory>
+#include <string>
+#include <vector>
+#if __ANDROID_API__ >= 9
+#include "android/asset_manager.h"
+#include "android/asset_manager_jni.h"
+#endif
 
-#include "sherpa-onnx/csrc/macros.h"
-#include "sherpa-onnx/csrc/offline-punctuation-impl.h"
+#include "sherpa-onnx/csrc/offline-punctuation.h"
 
 namespace sherpa_onnx {
 
-void OfflinePunctuationConfig::Register(ParseOptions *po) {
-  model.Register(po);
-}
-
-bool OfflinePunctuationConfig::Validate() const {
-  if (!model.Validate()) {
-    return false;
-  }
-
-  return true;
-}
-
-std::string OfflinePunctuationConfig::ToString() const {
-  std::ostringstream os;
+class OfflinePunctuationImpl {
+ public:
+  virtual ~OfflinePunctuationImpl() = default;
+
+  static std::unique_ptr<OfflinePunctuationImpl> Create(
+      const OfflinePunctuationConfig &config);
+
+#if __ANDROID_API__ >= 9
+  static std::unique_ptr<OfflinePunctuationImpl> Create(
+      AAssetManager *mgr, const OfflinePunctuationConfig &config);
+#endif
 
-  os << "OfflinePunctuationConfig(";
-  os << "model=" << model.ToString() << ")";
-
-  return os.str();
-}
-
-OfflinePunctuation::OfflinePunctuation(const OfflinePunctuationConfig &config)
-    : impl_(OfflinePunctuationImpl::Create(config)) {}
-
-OfflinePunctuation::~OfflinePunctuation() = default;
-
-std::string OfflinePunctuation::AddPunctuation(const std::string &text) const {
-  return impl_->AddPunctuation(text);
-}
+  virtual std::string AddPunctuation(const std::string &text) const = 0;
+};
 
 }  // namespace sherpa_onnx
+
+#endif  // SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_IMPL_H_
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-punctuation.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-punctuation.h`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 #ifndef SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_H_
 #define SHERPA_ONNX_CSRC_OFFLINE_PUNCTUATION_H_
 
 #include <memory>
 #include <string>
 #include <vector>
 
+#if __ANDROID_API__ >= 9
+#include "android/asset_manager.h"
+#include "android/asset_manager_jni.h"
+#endif
+
 #include "sherpa-onnx/csrc/offline-punctuation-model-config.h"
 #include "sherpa-onnx/csrc/parse-options.h"
 
 namespace sherpa_onnx {
 
 struct OfflinePunctuationConfig {
   OfflinePunctuationModelConfig model;
@@ -29,14 +34,19 @@
 
 class OfflinePunctuationImpl;
 
 class OfflinePunctuation {
  public:
   explicit OfflinePunctuation(const OfflinePunctuationConfig &config);
 
+#if __ANDROID_API__ >= 9
+  OfflinePunctuation(AAssetManager *mgr,
+                     const OfflinePunctuationConfig &config);
+#endif
+
   ~OfflinePunctuation();
 
   // Add punctuation to the input text and return it.
   std::string AddPunctuation(const std::string &text) const;
 
  private:
   std::unique_ptr<OfflinePunctuationImpl> impl_;
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-ctc-impl.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   OfflineRecognitionResult r;
   r.tokens.reserve(src.tokens.size());
   r.timestamps.reserve(src.timestamps.size());
 
   std::string text;
 
   for (int32_t i = 0; i != src.tokens.size(); ++i) {
-    if (sym_table.contains("SIL") && src.tokens[i] == sym_table["SIL"]) {
+    if (sym_table.Contains("SIL") && src.tokens[i] == sym_table["SIL"]) {
       // tdnn models from yesno have a SIL token, we should remove it.
       continue;
     }
     auto sym = sym_table[src.tokens[i]];
     text.append(sym);
 
     if (sym.size() == 1 && (sym[0] < 0x20 || sym[0] > 0x7e)) {
@@ -99,30 +99,30 @@
 
     if (!config_.ctc_fst_decoder_config.graph.empty()) {
       // TODO(fangjun): Support android to read the graph from
       // asset_manager
       decoder_ = std::make_unique<OfflineCtcFstDecoder>(
           config_.ctc_fst_decoder_config);
     } else if (config_.decoding_method == "greedy_search") {
-      if (!symbol_table_.contains("<blk>") &&
-          !symbol_table_.contains("<eps>") &&
-          !symbol_table_.contains("<blank>")) {
+      if (!symbol_table_.Contains("<blk>") &&
+          !symbol_table_.Contains("<eps>") &&
+          !symbol_table_.Contains("<blank>")) {
         SHERPA_ONNX_LOGE(
             "We expect that tokens.txt contains "
             "the symbol <blk> or <eps> or <blank> and its ID.");
         exit(-1);
       }
 
       int32_t blank_id = 0;
-      if (symbol_table_.contains("<blk>")) {
+      if (symbol_table_.Contains("<blk>")) {
         blank_id = symbol_table_["<blk>"];
-      } else if (symbol_table_.contains("<eps>")) {
+      } else if (symbol_table_.Contains("<eps>")) {
         // for tdnn models of the yesno recipe from icefall
         blank_id = symbol_table_["<eps>"];
-      } else if (symbol_table_.contains("<blank>")) {
+      } else if (symbol_table_.Contains("<blank>")) {
         // for Wenet CTC models
         blank_id = symbol_table_["<blank>"];
       }
 
       decoder_ = std::make_unique<OfflineCtcGreedySearchDecoder>(blank_id);
     } else {
       SHERPA_ONNX_LOGE("Only greedy_search is supported at present. Given %s",
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-impl.cc`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 #include <string>
 
 #include "onnxruntime_cxx_api.h"  // NOLINT
 #include "sherpa-onnx/csrc/macros.h"
 #include "sherpa-onnx/csrc/offline-recognizer-ctc-impl.h"
 #include "sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h"
 #include "sherpa-onnx/csrc/offline-recognizer-transducer-impl.h"
+#include "sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h"
 #include "sherpa-onnx/csrc/offline-recognizer-whisper-impl.h"
 #include "sherpa-onnx/csrc/onnx-utils.h"
 #include "sherpa-onnx/csrc/text-utils.h"
 
 namespace sherpa_onnx {
 
 std::unique_ptr<OfflineRecognizerImpl> OfflineRecognizerImpl::Create(
     const OfflineRecognizerConfig &config) {
   if (!config.model_config.model_type.empty()) {
     const auto &model_type = config.model_config.model_type;
     if (model_type == "transducer") {
       return std::make_unique<OfflineRecognizerTransducerImpl>(config);
+    } else if (model_type == "nemo_transducer") {
+      return std::make_unique<OfflineRecognizerTransducerNeMoImpl>(config);
     } else if (model_type == "paraformer") {
       return std::make_unique<OfflineRecognizerParaformerImpl>(config);
     } else if (model_type == "nemo_ctc" || model_type == "tdnn" ||
                model_type == "zipformer2_ctc" || model_type == "wenet_ctc") {
       return std::make_unique<OfflineRecognizerCtcImpl>(config);
     } else if (model_type == "whisper") {
       return std::make_unique<OfflineRecognizerWhisperImpl>(config);
@@ -118,29 +121,37 @@
     return std::make_unique<OfflineRecognizerTransducerImpl>(config);
   }
 
   if (model_type == "paraformer") {
     return std::make_unique<OfflineRecognizerParaformerImpl>(config);
   }
 
-  if (model_type == "EncDecCTCModelBPE" || model_type == "tdnn" ||
+  if (model_type == "EncDecHybridRNNTCTCBPEModel" &&
+      !config.model_config.transducer.decoder_filename.empty() &&
+      !config.model_config.transducer.joiner_filename.empty()) {
+    return std::make_unique<OfflineRecognizerTransducerNeMoImpl>(config);
+  }
+
+  if (model_type == "EncDecCTCModelBPE" ||
+      model_type == "EncDecHybridRNNTCTCBPEModel" || model_type == "tdnn" ||
       model_type == "zipformer2_ctc" || model_type == "wenet_ctc") {
     return std::make_unique<OfflineRecognizerCtcImpl>(config);
   }
 
   if (strncmp(model_type.c_str(), "whisper", 7) == 0) {
     return std::make_unique<OfflineRecognizerWhisperImpl>(config);
   }
 
   SHERPA_ONNX_LOGE(
       "\nUnsupported model_type: %s\n"
       "We support only the following model types at present: \n"
       " - Non-streaming transducer models from icefall\n"
       " - Non-streaming Paraformer models from FunASR\n"
       " - EncDecCTCModelBPE models from NeMo\n"
+      " - EncDecHybridRNNTCTCBPEModel models from NeMo\n"
       " - Whisper models\n"
       " - Tdnn models\n"
       " - Zipformer CTC models\n"
       " - WeNet CTC models\n",
       model_type.c_str());
 
   exit(-1);
@@ -149,14 +160,16 @@
 #if __ANDROID_API__ >= 9
 std::unique_ptr<OfflineRecognizerImpl> OfflineRecognizerImpl::Create(
     AAssetManager *mgr, const OfflineRecognizerConfig &config) {
   if (!config.model_config.model_type.empty()) {
     const auto &model_type = config.model_config.model_type;
     if (model_type == "transducer") {
       return std::make_unique<OfflineRecognizerTransducerImpl>(mgr, config);
+    } else if (model_type == "nemo_transducer") {
+      return std::make_unique<OfflineRecognizerTransducerNeMoImpl>(mgr, config);
     } else if (model_type == "paraformer") {
       return std::make_unique<OfflineRecognizerParaformerImpl>(mgr, config);
     } else if (model_type == "nemo_ctc" || model_type == "tdnn" ||
                model_type == "zipformer2_ctc" || model_type == "wenet_ctc") {
       return std::make_unique<OfflineRecognizerCtcImpl>(mgr, config);
     } else if (model_type == "whisper") {
       return std::make_unique<OfflineRecognizerWhisperImpl>(mgr, config);
@@ -248,29 +261,37 @@
     return std::make_unique<OfflineRecognizerTransducerImpl>(mgr, config);
   }
 
   if (model_type == "paraformer") {
     return std::make_unique<OfflineRecognizerParaformerImpl>(mgr, config);
   }
 
-  if (model_type == "EncDecCTCModelBPE" || model_type == "tdnn" ||
+  if (model_type == "EncDecHybridRNNTCTCBPEModel" &&
+      !config.model_config.transducer.decoder_filename.empty() &&
+      !config.model_config.transducer.joiner_filename.empty()) {
+    return std::make_unique<OfflineRecognizerTransducerNeMoImpl>(mgr, config);
+  }
+
+  if (model_type == "EncDecCTCModelBPE" ||
+      model_type == "EncDecHybridRNNTCTCBPEModel" || model_type == "tdnn" ||
       model_type == "zipformer2_ctc" || model_type == "wenet_ctc") {
     return std::make_unique<OfflineRecognizerCtcImpl>(mgr, config);
   }
 
   if (strncmp(model_type.c_str(), "whisper", 7) == 0) {
     return std::make_unique<OfflineRecognizerWhisperImpl>(mgr, config);
   }
 
   SHERPA_ONNX_LOGE(
       "\nUnsupported model_type: %s\n"
       "We support only the following model types at present: \n"
       " - Non-streaming transducer models from icefall\n"
       " - Non-streaming Paraformer models from FunASR\n"
       " - EncDecCTCModelBPE models from NeMo\n"
+      " - EncDecHybridRNNTCTCBPEModel models from NeMo\n"
       " - Whisper models\n"
       " - Tdnn models\n"
       " - Zipformer CTC models\n"
       " - WeNet CTC models\n",
       model_type.c_str());
 
   exit(-1);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-transducer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer-whisper-impl.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 static OfflineRecognitionResult Convert(const OfflineWhisperDecoderResult &src,
                                         const SymbolTable &sym_table) {
   OfflineRecognitionResult r;
   r.tokens.reserve(src.tokens.size());
 
   std::string text;
   for (auto i : src.tokens) {
-    if (!sym_table.contains(i)) {
+    if (!sym_table.Contains(i)) {
       continue;
     }
 
     const auto &s = sym_table[i];
     text += s;
     r.tokens.push_back(s);
   }
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-recognizer.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-recognizer.h`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 #include <vector>
 
 #if __ANDROID_API__ >= 9
 #include "android/asset_manager.h"
 #include "android/asset_manager_jni.h"
 #endif
 
+#include "sherpa-onnx/csrc/features.h"
 #include "sherpa-onnx/csrc/offline-ctc-fst-decoder-config.h"
 #include "sherpa-onnx/csrc/offline-lm-config.h"
 #include "sherpa-onnx/csrc/offline-model-config.h"
 #include "sherpa-onnx/csrc/offline-stream.h"
 #include "sherpa-onnx/csrc/offline-transducer-model-config.h"
 #include "sherpa-onnx/csrc/parse-options.h"
 
 namespace sherpa_onnx {
 
 struct OfflineRecognitionResult;
 
 struct OfflineRecognizerConfig {
-  OfflineFeatureExtractorConfig feat_config;
+  FeatureExtractorConfig feat_config;
   OfflineModelConfig model_config;
   OfflineLMConfig lm_config;
   OfflineCtcFstDecoderConfig ctc_fst_decoder_config;
 
   std::string decoding_method = "greedy_search";
   int32_t max_active_paths = 4;
 
@@ -40,15 +41,15 @@
   float blank_penalty = 0.0;
 
   // only greedy_search is implemented
   // TODO(fangjun): Implement modified_beam_search
 
   OfflineRecognizerConfig() = default;
   OfflineRecognizerConfig(
-      const OfflineFeatureExtractorConfig &feat_config,
+      const FeatureExtractorConfig &feat_config,
       const OfflineModelConfig &model_config, const OfflineLMConfig &lm_config,
       const OfflineCtcFstDecoderConfig &ctc_fst_decoder_config,
       const std::string &decoding_method, int32_t max_active_paths,
       const std::string &hotwords_file, float hotwords_score,
       float blank_penalty)
       : feat_config(feat_config),
         model_config(model_config),
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-rnn-lm.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-rnn-lm.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-stream.cc`

 * *Files 9% similar despite different names*

```diff
@@ -48,50 +48,33 @@
     (*mean)[i] = t;
 
     float stddev = std::sqrt(sum_sq[i] / num_rows - t * t);
     (*inv_stddev)[i] = 1.0f / (stddev + 1e-5f);
   }
 }
 
-void OfflineFeatureExtractorConfig::Register(ParseOptions *po) {
-  po->Register("sample-rate", &sampling_rate,
-               "Sampling rate of the input waveform. "
-               "Note: You can have a different "
-               "sample rate for the input waveform. We will do resampling "
-               "inside the feature extractor");
-
-  po->Register("feat-dim", &feature_dim,
-               "Feature dimension. Must match the one expected by the model.");
-}
-
-std::string OfflineFeatureExtractorConfig::ToString() const {
-  std::ostringstream os;
-
-  os << "OfflineFeatureExtractorConfig(";
-  os << "sampling_rate=" << sampling_rate << ", ";
-  os << "feature_dim=" << feature_dim << ")";
-
-  return os.str();
-}
-
 class OfflineStream::Impl {
  public:
-  explicit Impl(const OfflineFeatureExtractorConfig &config,
+  explicit Impl(const FeatureExtractorConfig &config,
                 ContextGraphPtr context_graph)
       : config_(config), context_graph_(context_graph) {
-    opts_.frame_opts.dither = 0;
-    opts_.frame_opts.snip_edges = false;
+    opts_.frame_opts.dither = config.dither;
+    opts_.frame_opts.snip_edges = config.snip_edges;
     opts_.frame_opts.samp_freq = config.sampling_rate;
+    opts_.frame_opts.frame_shift_ms = config.frame_shift_ms;
+    opts_.frame_opts.frame_length_ms = config.frame_length_ms;
+    opts_.frame_opts.remove_dc_offset = config.remove_dc_offset;
+    opts_.frame_opts.window_type = config.window_type;
+
     opts_.mel_opts.num_bins = config.feature_dim;
 
-    // Please see
-    // https://github.com/lhotse-speech/lhotse/blob/master/lhotse/features/fbank.py#L27
-    // and
-    // https://github.com/k2-fsa/sherpa-onnx/issues/514
-    opts_.mel_opts.high_freq = -400;
+    opts_.mel_opts.high_freq = config.high_freq;
+    opts_.mel_opts.low_freq = config.low_freq;
+
+    opts_.mel_opts.is_librosa = config.is_librosa;
 
     fbank_ = std::make_unique<knf::OnlineFbank>(opts_);
   }
 
   explicit Impl(WhisperTag /*tag*/) {
     config_.normalize_samples = true;
     opts_.frame_opts.samp_freq = 16000;
@@ -233,25 +216,24 @@
         p[i] = (p[i] - mean[i]) * inv_stddev[i];
       }
       p += feature_dim;
     }
   }
 
  private:
-  OfflineFeatureExtractorConfig config_;
+  FeatureExtractorConfig config_;
   std::unique_ptr<knf::OnlineFbank> fbank_;
   std::unique_ptr<knf::OnlineWhisperFbank> whisper_fbank_;
   knf::FbankOptions opts_;
   OfflineRecognitionResult r_;
   ContextGraphPtr context_graph_;
 };
 
-OfflineStream::OfflineStream(
-    const OfflineFeatureExtractorConfig &config /*= {}*/,
-    ContextGraphPtr context_graph /*= nullptr*/)
+OfflineStream::OfflineStream(const FeatureExtractorConfig &config /*= {}*/,
+                             ContextGraphPtr context_graph /*= nullptr*/)
     : impl_(std::make_unique<Impl>(config, context_graph)) {}
 
 OfflineStream::OfflineStream(WhisperTag tag)
     : impl_(std::make_unique<Impl>(tag)) {}
 
 OfflineStream::OfflineStream(CEDTag tag) : impl_(std::make_unique<Impl>(tag)) {}
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-stream.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-stream.h`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #include <stdint.h>
 
 #include <memory>
 #include <string>
 #include <vector>
 
 #include "sherpa-onnx/csrc/context-graph.h"
+#include "sherpa-onnx/csrc/features.h"
 #include "sherpa-onnx/csrc/parse-options.h"
 
 namespace sherpa_onnx {
 
 struct OfflineRecognitionResult {
   // Recognition results.
   // For English, it consists of space separated words.
@@ -28,54 +29,20 @@
   /// timestamps.size() == tokens.size()
   /// timestamps[i] records the time in seconds when tokens[i] is decoded.
   std::vector<float> timestamps;
 
   std::string AsJsonString() const;
 };
 
-struct OfflineFeatureExtractorConfig {
-  // Sampling rate used by the feature extractor. If it is different from
-  // the sampling rate of the input waveform, we will do resampling inside.
-  int32_t sampling_rate = 16000;
-
-  // Feature dimension
-  int32_t feature_dim = 80;
-
-  // Set internally by some models, e.g., paraformer and wenet CTC models set
-  // it to false.
-  // This parameter is not exposed to users from the commandline
-  // If true, the feature extractor expects inputs to be normalized to
-  // the range [-1, 1].
-  // If false, we will multiply the inputs by 32768
-  bool normalize_samples = true;
-
-  // For models from NeMo
-  // This option is not exposed and is set internally when loading models.
-  // Possible values:
-  // - per_feature
-  // - all_features (not implemented yet)
-  // - fixed_mean (not implemented)
-  // - fixed_std (not implemented)
-  // - or just leave it to empty
-  // See
-  // https://github.com/NVIDIA/NeMo/blob/main/nemo/collections/asr/parts/preprocessing/features.py#L59
-  // for details
-  std::string nemo_normalize_type;
-
-  std::string ToString() const;
-
-  void Register(ParseOptions *po);
-};
-
 struct WhisperTag {};
 struct CEDTag {};
 
 class OfflineStream {
  public:
-  explicit OfflineStream(const OfflineFeatureExtractorConfig &config = {},
+  explicit OfflineStream(const FeatureExtractorConfig &config = {},
                          ContextGraphPtr context_graph = {});
 
   explicit OfflineStream(WhisperTag tag);
   explicit OfflineStream(CEDTag tag);
   ~OfflineStream();
 
   /**
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tdnn-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tdnn-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #include "sherpa-onnx/csrc/offline-transducer-decoder.h"
 #include "sherpa-onnx/csrc/offline-transducer-model.h"
 
 namespace sherpa_onnx {
 
 class OfflineTransducerGreedySearchDecoder : public OfflineTransducerDecoder {
  public:
-  explicit OfflineTransducerGreedySearchDecoder(OfflineTransducerModel *model,
-                                                float blank_penalty)
+  OfflineTransducerGreedySearchDecoder(OfflineTransducerModel *model,
+                                       float blank_penalty)
       : model_(model), blank_penalty_(blank_penalty) {}
 
   std::vector<OfflineTransducerDecoderResult> Decode(
       Ort::Value encoder_out, Ort::Value encoder_out_length,
       OfflineStream **ss = nullptr, int32_t n = 0) override;
 
  private:
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-character-frontend.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-character-frontend.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-character-frontend.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-character-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-frontend.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-frontend.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model-metadata.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts-vits-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts-vits-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-tts.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-tts.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-websocket-server.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-wenet-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-whisper-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-whisper-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-audio-tagging-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/offline-zipformer-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/offline-zipformer-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-conformer-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-conformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-conformer-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-conformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-fst-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-fst-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-greedy-search-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-model.cc`

 * *Files 8% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 
 #include <algorithm>
 #include <memory>
 #include <sstream>
 #include <string>
 
 #include "sherpa-onnx/csrc/macros.h"
+#include "sherpa-onnx/csrc/online-nemo-ctc-model.h"
 #include "sherpa-onnx/csrc/online-wenet-ctc-model.h"
 #include "sherpa-onnx/csrc/online-zipformer2-ctc-model.h"
 #include "sherpa-onnx/csrc/onnx-utils.h"
 
 namespace sherpa_onnx {
 
 std::unique_ptr<OnlineCtcModel> OnlineCtcModel::Create(
     const OnlineModelConfig &config) {
   if (!config.wenet_ctc.model.empty()) {
     return std::make_unique<OnlineWenetCtcModel>(config);
   } else if (!config.zipformer2_ctc.model.empty()) {
     return std::make_unique<OnlineZipformer2CtcModel>(config);
+  } else if (!config.nemo_ctc.model.empty()) {
+    return std::make_unique<OnlineNeMoCtcModel>(config);
   } else {
     SHERPA_ONNX_LOGE("Please specify a CTC model");
     exit(-1);
   }
 }
 
 #if __ANDROID_API__ >= 9
 
 std::unique_ptr<OnlineCtcModel> OnlineCtcModel::Create(
     AAssetManager *mgr, const OnlineModelConfig &config) {
   if (!config.wenet_ctc.model.empty()) {
     return std::make_unique<OnlineWenetCtcModel>(mgr, config);
   } else if (!config.zipformer2_ctc.model.empty()) {
     return std::make_unique<OnlineZipformer2CtcModel>(mgr, config);
+  } else if (!config.nemo_ctc.model.empty()) {
+    return std::make_unique<OnlineNeMoCtcModel>(mgr, config);
   } else {
     SHERPA_ONNX_LOGE("Please specify a CTC model");
     exit(-1);
   }
 }
 #endif
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lm.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lstm-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lstm-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-lstm-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-lstm-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-model-config.cc`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 namespace sherpa_onnx {
 
 void OnlineModelConfig::Register(ParseOptions *po) {
   transducer.Register(po);
   paraformer.Register(po);
   wenet_ctc.Register(po);
   zipformer2_ctc.Register(po);
+  nemo_ctc.Register(po);
 
   po->Register("tokens", &tokens, "Path to tokens.txt");
 
   po->Register("num-threads", &num_threads,
                "Number of threads to run the neural network");
 
   po->Register("warm-up", &warm_up,
@@ -27,19 +28,19 @@
 
   po->Register("debug", &debug,
                "true to print model information while loading it.");
 
   po->Register("provider", &provider,
                "Specify a provider to use: cpu, cuda, coreml");
 
-  po->Register(
-      "model-type", &model_type,
-      "Specify it to reduce model initialization time. "
-      "Valid values are: conformer, lstm, zipformer, zipformer2, wenet_ctc"
-      "All other values lead to loading the model twice.");
+  po->Register("model-type", &model_type,
+               "Specify it to reduce model initialization time. "
+               "Valid values are: conformer, lstm, zipformer, zipformer2, "
+               "wenet_ctc, nemo_ctc. "
+               "All other values lead to loading the model twice.");
 }
 
 bool OnlineModelConfig::Validate() const {
   if (num_threads < 1) {
     SHERPA_ONNX_LOGE("num_threads should be > 0. Given %d", num_threads);
     return false;
   }
@@ -57,25 +58,30 @@
     return wenet_ctc.Validate();
   }
 
   if (!zipformer2_ctc.model.empty()) {
     return zipformer2_ctc.Validate();
   }
 
+  if (!nemo_ctc.model.empty()) {
+    return nemo_ctc.Validate();
+  }
+
   return transducer.Validate();
 }
 
 std::string OnlineModelConfig::ToString() const {
   std::ostringstream os;
 
   os << "OnlineModelConfig(";
   os << "transducer=" << transducer.ToString() << ", ";
   os << "paraformer=" << paraformer.ToString() << ", ";
   os << "wenet_ctc=" << wenet_ctc.ToString() << ", ";
   os << "zipformer2_ctc=" << zipformer2_ctc.ToString() << ", ";
+  os << "nemo_ctc=" << nemo_ctc.ToString() << ", ";
   os << "tokens=\"" << tokens << "\", ";
   os << "num_threads=" << num_threads << ", ";
   os << "warm_up=" << warm_up << ", ";
   os << "debug=" << (debug ? "True" : "False") << ", ";
   os << "provider=\"" << provider << "\", ";
   os << "model_type=\"" << model_type << "\")";
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-model-config.h`

 * *Files 10% similar despite different names*

```diff
@@ -2,54 +2,59 @@
 //
 // Copyright (c)  2023  Xiaomi Corporation
 #ifndef SHERPA_ONNX_CSRC_ONLINE_MODEL_CONFIG_H_
 #define SHERPA_ONNX_CSRC_ONLINE_MODEL_CONFIG_H_
 
 #include <string>
 
+#include "sherpa-onnx/csrc/online-nemo-ctc-model-config.h"
 #include "sherpa-onnx/csrc/online-paraformer-model-config.h"
 #include "sherpa-onnx/csrc/online-transducer-model-config.h"
 #include "sherpa-onnx/csrc/online-wenet-ctc-model-config.h"
 #include "sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h"
 
 namespace sherpa_onnx {
 
 struct OnlineModelConfig {
   OnlineTransducerModelConfig transducer;
   OnlineParaformerModelConfig paraformer;
   OnlineWenetCtcModelConfig wenet_ctc;
   OnlineZipformer2CtcModelConfig zipformer2_ctc;
+  OnlineNeMoCtcModelConfig nemo_ctc;
   std::string tokens;
   int32_t num_threads = 1;
   int32_t warm_up = 0;
   bool debug = false;
   std::string provider = "cpu";
 
   // Valid values:
   //  - conformer, conformer transducer from icefall
   //  - lstm, lstm transducer from icefall
   //  - zipformer, zipformer transducer from icefall
   //  - zipformer2, zipformer2 transducer or CTC from icefall
   //  - wenet_ctc, wenet CTC model
+  //  - nemo_ctc, NeMo CTC model
   //
   // All other values are invalid and lead to loading the model twice.
   std::string model_type;
 
   OnlineModelConfig() = default;
   OnlineModelConfig(const OnlineTransducerModelConfig &transducer,
                     const OnlineParaformerModelConfig &paraformer,
                     const OnlineWenetCtcModelConfig &wenet_ctc,
                     const OnlineZipformer2CtcModelConfig &zipformer2_ctc,
+                    const OnlineNeMoCtcModelConfig &nemo_ctc,
                     const std::string &tokens, int32_t num_threads,
                     int32_t warm_up, bool debug, const std::string &provider,
                     const std::string &model_type)
       : transducer(transducer),
         paraformer(paraformer),
         wenet_ctc(wenet_ctc),
         zipformer2_ctc(zipformer2_ctc),
+        nemo_ctc(nemo_ctc),
         tokens(tokens),
         num_threads(num_threads),
         warm_up(warm_up),
         debug(debug),
         provider(provider),
         model_type(model_type) {}
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-paraformer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-paraformer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-ctc-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-ctc-impl.h`

 * *Files 2% similar despite different names*

```diff
@@ -219,29 +219,29 @@
     // Note: We only update counters. The underlying audio samples
     // are not discarded.
     s->Reset();
   }
 
  private:
   void InitDecoder() {
-    if (!sym_.contains("<blk>") && !sym_.contains("<eps>") &&
-        !sym_.contains("<blank>")) {
+    if (!sym_.Contains("<blk>") && !sym_.Contains("<eps>") &&
+        !sym_.Contains("<blank>")) {
       SHERPA_ONNX_LOGE(
           "We expect that tokens.txt contains "
           "the symbol <blk> or <eps> or <blank> and its ID.");
       exit(-1);
     }
 
     int32_t blank_id = 0;
-    if (sym_.contains("<blk>")) {
+    if (sym_.Contains("<blk>")) {
       blank_id = sym_["<blk>"];
-    } else if (sym_.contains("<eps>")) {
+    } else if (sym_.Contains("<eps>")) {
       // for tdnn models of the yesno recipe from icefall
       blank_id = sym_["<eps>"];
-    } else if (sym_.contains("<blank>")) {
+    } else if (sym_.Contains("<blank>")) {
       // for WeNet CTC models
       blank_id = sym_["<blank>"];
     }
 
     if (!config_.ctc_fst_decoder_config.graph.empty()) {
       decoder_ = std::make_unique<OnlineCtcFstDecoder>(
           config_.ctc_fst_decoder_config, blank_id);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-impl.cc`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
   }
 
   if (!config.model_config.paraformer.encoder.empty()) {
     return std::make_unique<OnlineRecognizerParaformerImpl>(config);
   }
 
   if (!config.model_config.wenet_ctc.model.empty() ||
-      !config.model_config.zipformer2_ctc.model.empty()) {
+      !config.model_config.zipformer2_ctc.model.empty() ||
+      !config.model_config.nemo_ctc.model.empty()) {
     return std::make_unique<OnlineRecognizerCtcImpl>(config);
   }
 
   SHERPA_ONNX_LOGE("Please specify a model");
   exit(-1);
 }
 
@@ -37,15 +38,16 @@
   }
 
   if (!config.model_config.paraformer.encoder.empty()) {
     return std::make_unique<OnlineRecognizerParaformerImpl>(mgr, config);
   }
 
   if (!config.model_config.wenet_ctc.model.empty() ||
-      !config.model_config.zipformer2_ctc.model.empty()) {
+      !config.model_config.zipformer2_ctc.model.empty() ||
+      !config.model_config.nemo_ctc.model.empty()) {
     return std::make_unique<OnlineRecognizerCtcImpl>(mgr, config);
   }
 
   SHERPA_ONNX_LOGE("Please specify a model");
   exit(-1);
 }
 #endif
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-paraformer-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer-transducer-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer-transducer-impl.h`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 class OnlineRecognizerTransducerImpl : public OnlineRecognizerImpl {
  public:
   explicit OnlineRecognizerTransducerImpl(const OnlineRecognizerConfig &config)
       : config_(config),
         model_(OnlineTransducerModel::Create(config.model_config)),
         sym_(config.model_config.tokens),
         endpoint_(config_.endpoint_config) {
-    if (sym_.contains("<unk>")) {
+    if (sym_.Contains("<unk>")) {
       unk_id_ = sym_["<unk>"];
     }
 
     model_->SetFeatureDim(config.feat_config.feature_dim);
 
     if (config.decoding_method == "modified_beam_search") {
       if (!config_.hotwords_file.empty()) {
@@ -100,33 +100,37 @@
 
       if (!config_.lm_config.model.empty()) {
         lm_ = OnlineLM::Create(config.lm_config);
       }
 
       decoder_ = std::make_unique<OnlineTransducerModifiedBeamSearchDecoder>(
           model_.get(), lm_.get(), config_.max_active_paths,
-          config_.lm_config.scale, unk_id_, config_.blank_penalty);
+          config_.lm_config.scale, unk_id_, config_.blank_penalty,
+          config_.temperature_scale);
+
     } else if (config.decoding_method == "greedy_search") {
       decoder_ = std::make_unique<OnlineTransducerGreedySearchDecoder>(
-          model_.get(), unk_id_, config_.blank_penalty);
+          model_.get(), unk_id_, config_.blank_penalty,
+          config_.temperature_scale);
+
     } else {
       SHERPA_ONNX_LOGE("Unsupported decoding method: %s",
                        config.decoding_method.c_str());
       exit(-1);
     }
   }
 
 #if __ANDROID_API__ >= 9
   explicit OnlineRecognizerTransducerImpl(AAssetManager *mgr,
                                           const OnlineRecognizerConfig &config)
       : config_(config),
         model_(OnlineTransducerModel::Create(mgr, config.model_config)),
         sym_(mgr, config.model_config.tokens),
         endpoint_(config_.endpoint_config) {
-    if (sym_.contains("<unk>")) {
+    if (sym_.Contains("<unk>")) {
       unk_id_ = sym_["<unk>"];
     }
 
     model_->SetFeatureDim(config.feat_config.feature_dim);
 
     if (config.decoding_method == "modified_beam_search") {
 #if 0
@@ -138,18 +142,22 @@
 
       if (!config_.hotwords_file.empty()) {
         InitHotwords(mgr);
       }
 
       decoder_ = std::make_unique<OnlineTransducerModifiedBeamSearchDecoder>(
           model_.get(), lm_.get(), config_.max_active_paths,
-          config_.lm_config.scale, unk_id_, config_.blank_penalty);
+          config_.lm_config.scale, unk_id_, config_.blank_penalty,
+          config_.temperature_scale);
+
     } else if (config.decoding_method == "greedy_search") {
       decoder_ = std::make_unique<OnlineTransducerGreedySearchDecoder>(
-          model_.get(), unk_id_, config_.blank_penalty);
+          model_.get(), unk_id_, config_.blank_penalty,
+          config_.temperature_scale);
+
     } else {
       SHERPA_ONNX_LOGE("Unsupported decoding method: %s",
                        config.decoding_method.c_str());
       exit(-1);
     }
   }
 #endif
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer.cc`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,16 @@
       "The file containing hotwords, one words/phrases per line, and for each"
       "phrase the bpe/cjkchar are separated by a space. For example: "
       "▁HE LL O ▁WORLD"
       "你 好 世 界");
   po->Register("decoding-method", &decoding_method,
                "decoding method,"
                "now support greedy_search and modified_beam_search.");
+  po->Register("temperature-scale", &temperature_scale,
+               "Temperature scale for confidence computation in decoding.");
 }
 
 bool OnlineRecognizerConfig::Validate() const {
   if (decoding_method == "modified_beam_search" && !lm_config.model.empty()) {
     if (max_active_paths <= 0) {
       SHERPA_ONNX_LOGE("max_active_paths is less than 0! Given: %d",
                        max_active_paths);
@@ -138,15 +140,16 @@
   os << "endpoint_config=" << endpoint_config.ToString() << ", ";
   os << "ctc_fst_decoder_config=" << ctc_fst_decoder_config.ToString() << ", ";
   os << "enable_endpoint=" << (enable_endpoint ? "True" : "False") << ", ";
   os << "max_active_paths=" << max_active_paths << ", ";
   os << "hotwords_score=" << hotwords_score << ", ";
   os << "hotwords_file=\"" << hotwords_file << "\", ";
   os << "decoding_method=\"" << decoding_method << "\", ";
-  os << "blank_penalty=" << blank_penalty << ")";
+  os << "blank_penalty=" << blank_penalty << ", ";
+  os << "temperature_scale=" << temperature_scale << ")";
 
   return os.str();
 }
 
 OnlineRecognizer::OnlineRecognizer(const OnlineRecognizerConfig &config)
     : impl_(OnlineRecognizerImpl::Create(config)) {}
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-recognizer.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-recognizer.h`

 * *Files 12% similar despite different names*

```diff
@@ -92,35 +92,43 @@
 
   /// used only for modified_beam_search
   float hotwords_score = 1.5;
   std::string hotwords_file;
 
   float blank_penalty = 0.0;
 
+  float temperature_scale = 2.0;
+
   OnlineRecognizerConfig() = default;
 
   OnlineRecognizerConfig(
       const FeatureExtractorConfig &feat_config,
-      const OnlineModelConfig &model_config, const OnlineLMConfig &lm_config,
+      const OnlineModelConfig &model_config,
+      const OnlineLMConfig &lm_config,
       const EndpointConfig &endpoint_config,
       const OnlineCtcFstDecoderConfig &ctc_fst_decoder_config,
-      bool enable_endpoint, const std::string &decoding_method,
-      int32_t max_active_paths, const std::string &hotwords_file,
-      float hotwords_score, float blank_penalty)
+      bool enable_endpoint,
+      const std::string &decoding_method,
+      int32_t max_active_paths,
+      const std::string &hotwords_file,
+      float hotwords_score,
+      float blank_penalty,
+      float temperature_scale)
       : feat_config(feat_config),
         model_config(model_config),
         lm_config(lm_config),
         endpoint_config(endpoint_config),
         ctc_fst_decoder_config(ctc_fst_decoder_config),
         enable_endpoint(enable_endpoint),
         decoding_method(decoding_method),
         max_active_paths(max_active_paths),
-        hotwords_score(hotwords_score),
         hotwords_file(hotwords_file),
-        blank_penalty(blank_penalty) {}
+        hotwords_score(hotwords_score),
+        blank_penalty(blank_penalty),
+        temperature_scale(temperature_scale) {}
 
   void Register(ParseOptions *po);
   bool Validate() const;
 
   std::string ToString() const;
 };
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-rnn-lm.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-rnn-lm.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-rnn-lm.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-rnn-lm.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-stream.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.cc`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,18 @@
         r.num_trailing_blanks = 0;
       } else {
         ++r.num_trailing_blanks;
       }
 
       // export the per-token log scores
       if (y != 0 && y != unk_id_) {
+        // apply temperature-scaling
+        for (int32_t n = 0; n < vocab_size; ++n) {
+          p_logit[n] /= temperature_scale_;
+        }
         LogSoftmax(p_logit, vocab_size);   // renormalize probabilities,
                                            // save time by doing it only for
                                            // emitted symbols
         const float *p_logprob = p_logit;  // rename p_logit as p_logprob,
                                            // now it contains normalized
                                            // probability
         r.ys_probs.push_back(p_logprob[y]);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-greedy-search-decoder.h`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 #include "sherpa-onnx/csrc/online-transducer-model.h"
 
 namespace sherpa_onnx {
 
 class OnlineTransducerGreedySearchDecoder : public OnlineTransducerDecoder {
  public:
   OnlineTransducerGreedySearchDecoder(OnlineTransducerModel *model,
-                                      int32_t unk_id, float blank_penalty)
-      : model_(model), unk_id_(unk_id), blank_penalty_(blank_penalty) {}
+                                      int32_t unk_id,
+                                      float blank_penalty,
+                                      float temperature_scale)
+      : model_(model),
+      unk_id_(unk_id),
+      blank_penalty_(blank_penalty),
+      temperature_scale_(temperature_scale) {}
 
   OnlineTransducerDecoderResult GetEmptyResult() const override;
 
   void StripLeadingBlanks(OnlineTransducerDecoderResult *r) const override;
 
   void Decode(Ort::Value encoder_out,
               std::vector<OnlineTransducerDecoderResult> *result) override;
 
  private:
   OnlineTransducerModel *model_;  // Not owned
   int32_t unk_id_;
   float blank_penalty_;
+  float temperature_scale_;
 };
 
 }  // namespace sherpa_onnx
 
 #endif  // SHERPA_ONNX_CSRC_ONLINE_TRANSDUCER_GREEDY_SEARCH_DECODER_H_
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.cc`

 * *Files 5% similar despite different names*

```diff
@@ -125,14 +125,30 @@
         GetEncoderOutFrame(model_->Allocator(), &encoder_out, t);
     cur_encoder_out =
         Repeat(model_->Allocator(), &cur_encoder_out, hyps_row_splits);
     Ort::Value logit =
         model_->RunJoiner(std::move(cur_encoder_out), View(&decoder_out));
 
     float *p_logit = logit.GetTensorMutableData<float>();
+
+    // copy raw logits, apply temperature-scaling  (for confidences)
+    // Note: temperature scaling is used only for the confidences,
+    //       the decoding algorithm uses the original logits
+    int32_t p_logit_items = vocab_size * num_hyps;
+    std::vector<float> logit_with_temperature(p_logit_items);
+    {
+      std::copy(p_logit,
+                p_logit + p_logit_items,
+                logit_with_temperature.begin());
+      for (float& elem : logit_with_temperature) {
+        elem /= temperature_scale_;
+      }
+      LogSoftmax(logit_with_temperature.data(), vocab_size, num_hyps);
+    }
+
     if (blank_penalty_ > 0.0) {
       // assuming blank id is 0
       SubtractBlank(p_logit, vocab_size, num_hyps, 0, blank_penalty_);
     }
     LogSoftmax(p_logit, vocab_size, num_hyps);
 
     // now p_logit contains log_softmax output, we rename it to p_logprob
@@ -184,18 +200,15 @@
           ++new_hyp.num_trailing_blanks;
         }
         new_hyp.log_prob = p_logprob[k] + context_score -
                            prev_lm_log_prob;  // log_prob only includes the
                                               // score of the transducer
         // export the per-token log scores
         if (new_token != 0 && new_token != unk_id_) {
-          const Hypothesis &prev_i = prev[hyp_index];
-          // subtract 'prev[i]' path scores, which were added before
-          // getting topk tokens
-          float y_prob = p_logprob[k] - prev_i.log_prob - prev_i.lm_log_prob;
+          float y_prob = logit_with_temperature[start * vocab_size + k];
           new_hyp.ys_probs.push_back(y_prob);
 
           if (lm_) {  // export only when LM is used
             float lm_prob = new_hyp.lm_log_prob - prev_lm_log_prob;
             if (lm_scale_ != 0.0) {
               lm_prob /= lm_scale_;  // remove lm-scale
             }
@@ -209,15 +222,15 @@
         }
 
         hyps.Add(std::move(new_hyp));
       }  // for (auto k : topk)
       cur.push_back(std::move(hyps));
       p_logprob += (end - start) * vocab_size;
     }  // for (int32_t b = 0; b != batch_size; ++b)
-  }
+  }  // for (int32_t t = 0; t != num_frames; ++t)
 
   for (int32_t b = 0; b != batch_size; ++b) {
     auto &hyps = cur[b];
     auto best_hyp = hyps.GetMostProbable(true);
     auto &r = (*result)[b];
 
     r.hyps = std::move(hyps);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-transducer-modified-beam-search-decoder.h`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 class OnlineTransducerModifiedBeamSearchDecoder
     : public OnlineTransducerDecoder {
  public:
   OnlineTransducerModifiedBeamSearchDecoder(OnlineTransducerModel *model,
                                             OnlineLM *lm,
                                             int32_t max_active_paths,
                                             float lm_scale, int32_t unk_id,
-                                            float blank_penalty)
+                                            float blank_penalty,
+                                            float temperature_scale)
       : model_(model),
         lm_(lm),
         max_active_paths_(max_active_paths),
         lm_scale_(lm_scale),
         unk_id_(unk_id),
-        blank_penalty_(blank_penalty) {}
+        blank_penalty_(blank_penalty),
+        temperature_scale_(temperature_scale) {}
 
   OnlineTransducerDecoderResult GetEmptyResult() const override;
 
   void StripLeadingBlanks(OnlineTransducerDecoderResult *r) const override;
 
   void Decode(Ort::Value encoder_out,
               std::vector<OnlineTransducerDecoderResult> *result) override;
@@ -46,12 +48,13 @@
   OnlineTransducerModel *model_;  // Not owned
   OnlineLM *lm_;                  // Not owned
 
   int32_t max_active_paths_;
   float lm_scale_;  // used only when lm_ is not nullptr
   int32_t unk_id_;
   float blank_penalty_;
+  float temperature_scale_;
 };
 
 }  // namespace sherpa_onnx
 
 #endif  // SHERPA_ONNX_CSRC_ONLINE_TRANSDUCER_MODIFIED_BEAM_SEARCH_DECODER_H_
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-client.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-client.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-websocket-server.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-websocket-server.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-wenet-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-wenet-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-ctc-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-ctc-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-transducer-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/online-zipformer2-transducer-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/online-zipformer2-transducer-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/onnx-utils.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/onnx-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/onnx-utils.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/onnx-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/packed-sequence.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/packed-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/pad-sequence.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/pad-sequence.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/parse-options.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/parse-options.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/parse-options.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/parse-options.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-lexicon.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-lexicon.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-lexicon.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-lexicon.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/piper-phonemize-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/piper-phonemize-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/provider.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/provider.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/provider.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/provider.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/resample.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/resample.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/resample.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/resample.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/session.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/session.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/session.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/session.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline-speaker-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-microphone.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-microphone.cc`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 // Copyright (c)  2022-2023  Xiaomi Corporation
 
 #include <signal.h>
 #include <stdio.h>
 #include <stdlib.h>
 
 #include <algorithm>
-#include <cctype>  // std::tolower
+#include <clocale>
+#include <cwctype>
 
 #include "portaudio.h"  // NOLINT
 #include "sherpa-onnx/csrc/display.h"
 #include "sherpa-onnx/csrc/microphone.h"
 #include "sherpa-onnx/csrc/online-recognizer.h"
 
 bool stop = false;
@@ -33,14 +34,39 @@
 }
 
 static void Handler(int32_t sig) {
   stop = true;
   fprintf(stderr, "\nCaught Ctrl + C. Exiting...\n");
 }
 
+static std::string tolowerUnicode(const std::string &input_str) {
+  // Use system locale
+  std::setlocale(LC_ALL, "");
+
+  // From char string to wchar string
+  std::wstring input_wstr(input_str.size() + 1, '\0');
+  std::mbstowcs(&input_wstr[0], input_str.c_str(), input_str.size());
+  std::wstring lowercase_wstr;
+
+  for (wchar_t wc : input_wstr) {
+    if (std::iswupper(wc)) {
+      lowercase_wstr += std::towlower(wc);
+    } else {
+      lowercase_wstr += wc;
+    }
+  }
+
+  // Back to char string
+  std::string lowercase_str(input_str.size() + 1, '\0');
+  std::wcstombs(&lowercase_str[0], lowercase_wstr.c_str(),
+                lowercase_wstr.size());
+
+  return lowercase_str;
+}
+
 int32_t main(int32_t argc, char *argv[]) {
   signal(SIGINT, Handler);
 
   const char *kUsageMessage = R"usage(
 This program uses streaming models with microphone for speech recognition.
 Usage:
 
@@ -168,19 +194,15 @@
         recognizer.DecodeStream(s.get());
       }
       text = recognizer.GetResult(s.get()).text;
     }
 
     if (!text.empty() && last_text != text) {
       last_text = text;
-
-      std::transform(text.begin(), text.end(), text.begin(),
-                     [](auto c) { return std::tolower(c); });
-
-      display.Print(segment_index, text);
+      display.Print(segment_index, tolowerUnicode(text));
       fflush(stderr);
     }
 
     if (is_endpoint) {
       if (!text.empty()) {
         ++segment_index;
       }
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-parallel.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts-play.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-offline.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-offline.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-microphone-offline-asr.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx-vad-microphone.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/silero-vad-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/silero-vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/slice.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/slice.h`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 namespace sherpa_onnx {
 
 /** Get a deep copy by slicing a 3-D tensor v.
  *
  * It returns v[dim0_start:dim0_end, dim1_start:dim1_end, :]
  *
  * @param allocator
- * @param v A 2-D tensor. Its data type is T.
+ * @param v A 3-D tensor. Its data type is T.
  * @param dim0_start  Start index of the first dimension..
  * @param dim0_end    End index of the first dimension..
  * @param dim1_start Start index of the second dimension.
  * @param dim1_end  End index of the second dimension.
  *
  * @return Return a 3-D tensor of shape
  *         (dim0_end-dim0_start, dim1_end-dim1_start, v.shape[2])
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-general-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model-meta-data.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor-nemo-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-extractor.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-extractor.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/speaker-embedding-manager.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/speaker-embedding-manager.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-impl.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-impl.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification-whisper-impl.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/spoken-language-identification.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/spoken-language-identification.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/stack.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/stack.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/symbol-table.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/symbol-table.cc`

 * *Files 9% similar despite different names*

```diff
@@ -63,17 +63,21 @@
     assert(!sym.empty());
 
     // for byte bpe, after replacing ▁ with a space, whose ascii is also 0x20,
     // there is a conflict between the real byte 0x20 and ▁, so we disable
     // the following check.
     //
     // Note: Only id2sym_ matters as we use it to convert ID to symbols.
+#if 0
+    // we disable the test here since for some multi-lingual BPE models
+    // from NeMo, the same symbol can appear multiple times with different IDs.
     if (sym != " ") {
       assert(sym2id_.count(sym) == 0);
     }
+#endif
 
     assert(id2sym_.count(id) == 0);
 
     sym2id_.insert({sym, id});
     id2sym_.insert({id, sym});
   }
   assert(is.eof());
@@ -92,17 +96,17 @@
   return id2sym_.at(id);
 }
 
 int32_t SymbolTable::operator[](const std::string &sym) const {
   return sym2id_.at(sym);
 }
 
-bool SymbolTable::contains(int32_t id) const { return id2sym_.count(id) != 0; }
+bool SymbolTable::Contains(int32_t id) const { return id2sym_.count(id) != 0; }
 
-bool SymbolTable::contains(const std::string &sym) const {
+bool SymbolTable::Contains(const std::string &sym) const {
   return sym2id_.count(sym) != 0;
 }
 
 std::ostream &operator<<(std::ostream &os, const SymbolTable &symbol_table) {
   return os << symbol_table.ToString();
 }
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/symbol-table.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/symbol-table.h`

 * *Files 14% similar despite different names*

```diff
@@ -36,22 +36,24 @@
 
   /// Return the symbol corresponding to the given ID.
   const std::string &operator[](int32_t id) const;
   /// Return the ID corresponding to the given symbol.
   int32_t operator[](const std::string &sym) const;
 
   /// Return true if there is a symbol with the given ID.
-  bool contains(int32_t id) const;
+  bool Contains(int32_t id) const;
 
   /// Return true if there is a given symbol in the symbol table.
-  bool contains(const std::string &sym) const;
+  bool Contains(const std::string &sym) const;
 
   // for tokens.txt from Whisper
   void ApplyBase64Decode();
 
+  int32_t NumSymbols() const { return id2sym_.size(); }
+
  private:
   void Init(std::istream &is);
 
  private:
   std::unordered_map<std::string, int32_t> sym2id_;
   std::unordered_map<int32_t, std::string> id2sym_;
 };
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/tee-stream.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/tee-stream.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/text-utils.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/text-utils.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/text-utils.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/text-utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/transducer-keyword-decoder.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/transducer-keyword-decoder.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/transducer-keyword-decoder.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/transducer-keyword-decoder.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/transpose.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/transpose.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind-test.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind-test.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/unbind.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/unbind.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/utils.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/utils.cc`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         // For BPE-based models, we replace ▁ with a space
         // Unicode 9601, hex 0x2581, utf8 0xe29681
         const uint8_t *p = reinterpret_cast<const uint8_t *>(word.c_str());
         if (p[0] == 0xe2 && p[1] == 0x96 && p[2] == 0x81) {
           word = word.replace(0, 3, " ");
         }
       }
-      if (symbol_table.contains(word)) {
+      if (symbol_table.Contains(word)) {
         int32_t id = symbol_table[word];
         tmp_ids.push_back(id);
       } else {
         switch (word[0]) {
           case ':':  // boosting score for current keyword
             score = std::stof(word.substr(1));
             has_scores = true;
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/utils.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model-config.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model-config.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/vad-model.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/vad-model.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/voice-activity-detector.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/voice-activity-detector.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-reader.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-reader.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-reader.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-reader.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-writer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/csrc/wave-writer.h` & `sherpa-onnx-1.9.24/sherpa-onnx/csrc/wave-writer.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/CMakeLists.txt` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   include_directories($ENV{JAVA_HOME}/include/darwin)
 endif()
 
 set(sources
   audio-tagging.cc
   jni.cc
   keyword-spotter.cc
+  offline-punctuation.cc
   offline-recognizer.cc
   offline-stream.cc
   online-recognizer.cc
   online-stream.cc
   speaker-embedding-extractor.cc
   speaker-embedding-manager.cc
   spoken-language-identification.cc
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/common.h` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/common.h`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/jni.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/jni.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/keyword-spotter.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-recognizer.cc`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,27 @@
   ans.model_config.whisper.task = p;
   env->ReleaseStringUTFChars(s, p);
 
   fid = env->GetFieldID(whisper_config_cls, "tailPaddings", "I");
   ans.model_config.whisper.tail_paddings =
       env->GetIntField(whisper_config, fid);
 
+  fid = env->GetFieldID(
+      model_config_cls, "nemo",
+      "Lcom/k2fsa/sherpa/onnx/OfflineNemoEncDecCtcModelConfig;");
+  jobject nemo_config = env->GetObjectField(model_config, fid);
+  jclass nemo_config_cls = env->GetObjectClass(nemo_config);
+
+  fid = env->GetFieldID(paraformer_config_cls, "model", "Ljava/lang/String;");
+
+  s = (jstring)env->GetObjectField(nemo_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.model_config.nemo_ctc.model = p;
+  env->ReleaseStringUTFChars(s, p);
+
   return ans;
 }
 
 }  // namespace sherpa_onnx
 
 SHERPA_ONNX_EXTERN_C
 JNIEXPORT jlong JNICALL
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/offline-tts.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/offline-tts.cc`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
   return ans;
 }
 
 }  // namespace sherpa_onnx
 
 SHERPA_ONNX_EXTERN_C
-JNIEXPORT jlong JNICALL Java_com_k2fsa_sherpa_onnx_OfflineTts_newForAsset(
+JNIEXPORT jlong JNICALL Java_com_k2fsa_sherpa_onnx_OfflineTts_newFromAsset(
     JNIEnv *env, jobject /*obj*/, jobject asset_manager, jobject _config) {
 #if __ANDROID_API__ >= 9
   AAssetManager *mgr = AAssetManager_fromJava(env, asset_manager);
   if (!mgr) {
     SHERPA_ONNX_LOGE("Failed to get asset manager: %p", mgr);
   }
 #endif
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/online-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/online-recognizer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,30 @@
   p = env->GetStringUTFChars(s, nullptr);
   ans.lm_config.model = p;
   env->ReleaseStringUTFChars(s, p);
 
   fid = env->GetFieldID(lm_model_config_cls, "scale", "F");
   ans.lm_config.scale = env->GetFloatField(lm_model_config, fid);
 
+  fid = env->GetFieldID(cls, "ctcFstDecoderConfig",
+                        "Lcom/k2fsa/sherpa/onnx/OnlineCtcFstDecoderConfig;");
+
+  jobject fst_decoder_config = env->GetObjectField(config, fid);
+  jclass fst_decoder_config_cls = env->GetObjectClass(fst_decoder_config);
+
+  fid = env->GetFieldID(fst_decoder_config_cls, "graph", "Ljava/lang/String;");
+  s = (jstring)env->GetObjectField(fst_decoder_config, fid);
+  p = env->GetStringUTFChars(s, nullptr);
+  ans.ctc_fst_decoder_config.graph = p;
+  env->ReleaseStringUTFChars(s, p);
+
+  fid = env->GetFieldID(fst_decoder_config_cls, "maxActive", "I");
+  ans.ctc_fst_decoder_config.max_active =
+      env->GetIntField(fst_decoder_config, fid);
+
   return ans;
 }
 }  // namespace sherpa_onnx
 
 SHERPA_ONNX_EXTERN_C
 JNIEXPORT jlong JNICALL
 Java_com_k2fsa_sherpa_onnx_OnlineRecognizer_newFromAsset(JNIEnv *env,
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/online-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/spoken-language-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/voice-activity-detector.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/jni/wave-reader.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/jni/wave-reader.cc`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 //
 // Copyright (c)  2024  Xiaomi Corporation
 #include "sherpa-onnx/csrc/wave-reader.h"
 
 #include <fstream>
 
 #include "sherpa-onnx/csrc/macros.h"
+#include "sherpa-onnx/csrc/onnx-utils.h"
 #include "sherpa-onnx/jni/common.h"
 
 static jobjectArray ReadWaveImpl(JNIEnv *env, std::istream &is,
                                  const char *p_filename) {
   bool is_ok = false;
   int32_t sampling_rate = -1;
   std::vector<float> samples =
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/AudioTagging.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/AudioTagging.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/KeywordSpotter.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/KeywordSpotter.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OfflineRecognizer.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OfflineRecognizer.kt`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,31 @@
     var joiner: String = "",
 )
 
 data class OfflineParaformerModelConfig(
     var model: String = "",
 )
 
+data class OfflineNemoEncDecCtcModelConfig(
+    var model: String = "",
+)
+
 data class OfflineWhisperModelConfig(
     var encoder: String = "",
     var decoder: String = "",
     var language: String = "en", // Used with multilingual model
     var task: String = "transcribe", // transcribe or translate
     var tailPaddings: Int = 1000, // Padding added at the end of the samples
 )
 
 data class OfflineModelConfig(
     var transducer: OfflineTransducerModelConfig = OfflineTransducerModelConfig(),
     var paraformer: OfflineParaformerModelConfig = OfflineParaformerModelConfig(),
     var whisper: OfflineWhisperModelConfig = OfflineWhisperModelConfig(),
+    var nemo: OfflineNemoEncDecCtcModelConfig = OfflineNemoEncDecCtcModelConfig(),
     var numThreads: Int = 1,
     var debug: Boolean = false,
     var provider: String = "cpu",
     var modelType: String = "",
     var tokens: String,
 )
 
@@ -212,10 +217,20 @@
                     joiner = "$modelDir/joiner-epoch-20-avg-1.int8.onnx",
                 ),
                 tokens = "$modelDir/tokens.txt",
                 modelType = "zipformer2",
             )
         }
 
+        6 -> {
+            val modelDir = "sherpa-onnx-nemo-ctc-en-citrinet-512"
+            return OfflineModelConfig(
+                nemo = OfflineNemoEncDecCtcModelConfig(
+                    model = "$modelDir/model.int8.onnx",
+                ),
+                tokens = "$modelDir/tokens.txt",
+            )
+        }
+
     }
     return null
 }
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OfflineStream.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OfflineStream.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OnlineRecognizer.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OnlineRecognizer.kt`

 * *Files 5% similar despite different names*

```diff
@@ -41,19 +41,25 @@
 )
 
 data class OnlineLMConfig(
     var model: String = "",
     var scale: Float = 0.5f,
 )
 
+data class OnlineCtcFstDecoderConfig(
+    var graph: String = "",
+    var maxActive: Int = 3000,
+)
+
 
 data class OnlineRecognizerConfig(
     var featConfig: FeatureConfig = FeatureConfig(),
     var modelConfig: OnlineModelConfig,
     var lmConfig: OnlineLMConfig = OnlineLMConfig(),
+    var ctcFstDecoderConfig : OnlineCtcFstDecoderConfig = OnlineCtcFstDecoderConfig(),
     var endpointConfig: EndpointConfig = EndpointConfig(),
     var enableEndpoint: Boolean = true,
     var decodingMethod: String = "greedy_search",
     var maxActivePaths: Int = 4,
     var hotwordsFile: String = "",
     var hotwordsScore: Float = 1.5f,
 )
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/OnlineStream.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/OnlineStream.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/Speaker.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/Speaker.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/Vad.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/Vad.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/kotlin-api/WaveReader.kt` & `sherpa-onnx-1.9.24/sherpa-onnx/kotlin-api/WaveReader.kt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/CMakeLists.txt` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   offline-transducer-model-config.cc
   offline-wenet-ctc-model-config.cc
   offline-whisper-model-config.cc
   offline-zipformer-ctc-model-config.cc
   online-ctc-fst-decoder-config.cc
   online-lm-config.cc
   online-model-config.cc
+  online-nemo-ctc-model-config.cc
   online-paraformer-model-config.cc
   online-recognizer.cc
   online-stream.cc
   online-transducer-model-config.cc
   online-wenet-ctc-model-config.cc
   online-zipformer2-ctc-model-config.cc
   sherpa-onnx.cc
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/audio-tagging.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/audio-tagging.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/circular-buffer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/circular-buffer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/endpoint.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/endpoint.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/faked-alsa.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/faked-alsa.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/features.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/features.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/keyword-spotter.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/keyword-spotter.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-lm-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-nemo-enc-dec-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-punctuation.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-punctuation.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-recognizer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 #include "sherpa-onnx/csrc/offline-recognizer.h"
 
 namespace sherpa_onnx {
 
 static void PybindOfflineRecognizerConfig(py::module *m) {
   using PyClass = OfflineRecognizerConfig;
   py::class_<PyClass>(*m, "OfflineRecognizerConfig")
-      .def(py::init<const OfflineFeatureExtractorConfig &,
-                    const OfflineModelConfig &, const OfflineLMConfig &,
-                    const OfflineCtcFstDecoderConfig &, const std::string &,
-                    int32_t, const std::string &, float, float>(),
+      .def(py::init<const FeatureExtractorConfig &, const OfflineModelConfig &,
+                    const OfflineLMConfig &, const OfflineCtcFstDecoderConfig &,
+                    const std::string &, int32_t, const std::string &, float,
+                    float>(),
            py::arg("feat_config"), py::arg("model_config"),
            py::arg("lm_config") = OfflineLMConfig(),
            py::arg("ctc_fst_decoder_config") = OfflineCtcFstDecoderConfig(),
            py::arg("decoding_method") = "greedy_search",
            py::arg("max_active_paths") = 4, py::arg("hotwords_file") = "",
            py::arg("hotwords_score") = 1.5, py::arg("blank_penalty") = 0.0)
       .def_readwrite("feat_config", &PyClass::feat_config)
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-stream.cc`

 * *Files 10% similar despite different names*

```diff
@@ -21,38 +21,28 @@
     A 1-D float32 tensor containing audio samples. It must be normalized
     to the range [-1, 1].
 )";
 
 static void PybindOfflineRecognitionResult(py::module *m) {  // NOLINT
   using PyClass = OfflineRecognitionResult;
   py::class_<PyClass>(*m, "OfflineRecognitionResult")
+      .def("__str__", &PyClass::AsJsonString)
       .def_property_readonly(
           "text",
           [](const PyClass &self) -> py::str {
             return py::str(PyUnicode_DecodeUTF8(self.text.c_str(),
                                                 self.text.size(), "ignore"));
           })
       .def_property_readonly("tokens",
                              [](const PyClass &self) { return self.tokens; })
       .def_property_readonly(
           "timestamps", [](const PyClass &self) { return self.timestamps; });
 }
 
-static void PybindOfflineFeatureExtractorConfig(py::module *m) {
-  using PyClass = OfflineFeatureExtractorConfig;
-  py::class_<PyClass>(*m, "OfflineFeatureExtractorConfig")
-      .def(py::init<int32_t, int32_t>(), py::arg("sampling_rate") = 16000,
-           py::arg("feature_dim") = 80)
-      .def_readwrite("sampling_rate", &PyClass::sampling_rate)
-      .def_readwrite("feature_dim", &PyClass::feature_dim)
-      .def("__str__", &PyClass::ToString);
-}
-
 void PybindOfflineStream(py::module *m) {
-  PybindOfflineFeatureExtractorConfig(m);
   PybindOfflineRecognitionResult(m);
 
   using PyClass = OfflineStream;
   py::class_<PyClass>(*m, "OfflineStream")
       .def(
           "accept_waveform",
           [](PyClass &self, float sample_rate,
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tdnn-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-transducer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts-vits-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-tts.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-tts.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-whisper-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-whisper-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-lm-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-lm-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-model-config.cc`

 * *Files 8% similar despite different names*

```diff
@@ -5,46 +5,51 @@
 #include "sherpa-onnx/python/csrc/online-model-config.h"
 
 #include <string>
 #include <vector>
 
 #include "sherpa-onnx/csrc/online-model-config.h"
 #include "sherpa-onnx/csrc/online-transducer-model-config.h"
+#include "sherpa-onnx/python/csrc/online-nemo-ctc-model-config.h"
 #include "sherpa-onnx/python/csrc/online-paraformer-model-config.h"
 #include "sherpa-onnx/python/csrc/online-transducer-model-config.h"
 #include "sherpa-onnx/python/csrc/online-wenet-ctc-model-config.h"
 #include "sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.h"
 
 namespace sherpa_onnx {
 
 void PybindOnlineModelConfig(py::module *m) {
   PybindOnlineTransducerModelConfig(m);
   PybindOnlineParaformerModelConfig(m);
   PybindOnlineWenetCtcModelConfig(m);
   PybindOnlineZipformer2CtcModelConfig(m);
+  PybindOnlineNeMoCtcModelConfig(m);
 
   using PyClass = OnlineModelConfig;
   py::class_<PyClass>(*m, "OnlineModelConfig")
       .def(py::init<const OnlineTransducerModelConfig &,
                     const OnlineParaformerModelConfig &,
                     const OnlineWenetCtcModelConfig &,
-                    const OnlineZipformer2CtcModelConfig &, const std::string &,
+                    const OnlineZipformer2CtcModelConfig &,
+                    const OnlineNeMoCtcModelConfig &, const std::string &,
                     int32_t, int32_t, bool, const std::string &,
                     const std::string &>(),
            py::arg("transducer") = OnlineTransducerModelConfig(),
            py::arg("paraformer") = OnlineParaformerModelConfig(),
            py::arg("wenet_ctc") = OnlineWenetCtcModelConfig(),
            py::arg("zipformer2_ctc") = OnlineZipformer2CtcModelConfig(),
-           py::arg("tokens"), py::arg("num_threads"), py::arg("warm_up") = 0,
+           py::arg("nemo_ctc") = OnlineNeMoCtcModelConfig(), py::arg("tokens"),
+           py::arg("num_threads"), py::arg("warm_up") = 0,
            py::arg("debug") = false, py::arg("provider") = "cpu",
            py::arg("model_type") = "")
       .def_readwrite("transducer", &PyClass::transducer)
       .def_readwrite("paraformer", &PyClass::paraformer)
       .def_readwrite("wenet_ctc", &PyClass::wenet_ctc)
       .def_readwrite("zipformer2_ctc", &PyClass::zipformer2_ctc)
+      .def_readwrite("nemo_ctc", &PyClass::nemo_ctc)
       .def_readwrite("tokens", &PyClass::tokens)
       .def_readwrite("num_threads", &PyClass::num_threads)
       .def_readwrite("debug", &PyClass::debug)
       .def_readwrite("provider", &PyClass::provider)
       .def_readwrite("model_type", &PyClass::model_type)
       .def("validate", &PyClass::Validate)
       .def("__str__", &PyClass::ToString);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-paraformer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-paraformer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-recognizer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-recognizer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -38,44 +38,48 @@
                              [](PyClass &self) -> std::vector<float> {
                                return self.context_scores;
                              })
       .def_property_readonly(
           "segment", [](PyClass &self) -> int32_t { return self.segment; })
       .def_property_readonly(
           "is_final", [](PyClass &self) -> bool { return self.is_final; })
+      .def("__str__", &PyClass::AsJsonString,
+           py::call_guard<py::gil_scoped_release>())
       .def("as_json_string", &PyClass::AsJsonString,
            py::call_guard<py::gil_scoped_release>());
 }
 
 static void PybindOnlineRecognizerConfig(py::module *m) {
   using PyClass = OnlineRecognizerConfig;
   py::class_<PyClass>(*m, "OnlineRecognizerConfig")
       .def(
           py::init<const FeatureExtractorConfig &, const OnlineModelConfig &,
                    const OnlineLMConfig &, const EndpointConfig &,
                    const OnlineCtcFstDecoderConfig &, bool, const std::string &,
-                   int32_t, const std::string &, float, float>(),
+                   int32_t, const std::string &, float, float, float>(),
           py::arg("feat_config"), py::arg("model_config"),
           py::arg("lm_config") = OnlineLMConfig(),
           py::arg("endpoint_config") = EndpointConfig(),
           py::arg("ctc_fst_decoder_config") = OnlineCtcFstDecoderConfig(),
           py::arg("enable_endpoint"), py::arg("decoding_method"),
           py::arg("max_active_paths") = 4, py::arg("hotwords_file") = "",
-          py::arg("hotwords_score") = 0, py::arg("blank_penalty") = 0.0)
+          py::arg("hotwords_score") = 0, py::arg("blank_penalty") = 0.0,
+          py::arg("temperature_scale") = 2.0)
       .def_readwrite("feat_config", &PyClass::feat_config)
       .def_readwrite("model_config", &PyClass::model_config)
       .def_readwrite("lm_config", &PyClass::lm_config)
       .def_readwrite("endpoint_config", &PyClass::endpoint_config)
       .def_readwrite("ctc_fst_decoder_config", &PyClass::ctc_fst_decoder_config)
       .def_readwrite("enable_endpoint", &PyClass::enable_endpoint)
       .def_readwrite("decoding_method", &PyClass::decoding_method)
       .def_readwrite("max_active_paths", &PyClass::max_active_paths)
       .def_readwrite("hotwords_file", &PyClass::hotwords_file)
       .def_readwrite("hotwords_score", &PyClass::hotwords_score)
       .def_readwrite("blank_penalty", &PyClass::blank_penalty)
+      .def_readwrite("temperature_scale", &PyClass::temperature_scale)
       .def("__str__", &PyClass::ToString);
 }
 
 void PybindOnlineRecognizer(py::module *m) {
   PybindOnlineRecognizerResult(m);
   PybindOnlineRecognizerConfig(m);
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-stream.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-stream.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-transducer-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-transducer-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-wenet-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/online-zipformer2-ctc-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/sherpa-onnx.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/sherpa-onnx.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/silero-vad-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/silero-vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-extractor.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/speaker-embedding-manager.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/speaker-embedding-manager.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/spoken-language-identification.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/spoken-language-identification.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model-config.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model-config.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/vad-model.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/vad-model.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/voice-activity-detector.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/voice-activity-detector.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/csrc/wave-writer.cc` & `sherpa-onnx-1.9.24/sherpa-onnx/python/csrc/wave-writer.cc`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/__init__.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     write_wave,
 )
 
 from .keyword_spotter import KeywordSpotter
 from .offline_recognizer import OfflineRecognizer
 from .online_recognizer import OnlineRecognizer
 from .utils import text2token
-__version__ = '1.9.23'
+__version__ = '1.9.24'
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/cli.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/cli.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c)  2023 by manyeyes
 # Copyright (c)  2023  Xiaomi Corporation
 from pathlib import Path
 from typing import List, Optional
 
 from _sherpa_onnx import (
+    FeatureExtractorConfig,
     OfflineCtcFstDecoderConfig,
-    OfflineFeatureExtractorConfig,
     OfflineModelConfig,
     OfflineNemoEncDecCtcModelConfig,
     OfflineParaformerModelConfig,
 )
 from _sherpa_onnx import OfflineRecognizer as _Recognizer
 from _sherpa_onnx import (
     OfflineRecognizerConfig,
@@ -47,14 +47,15 @@
         decoding_method: str = "greedy_search",
         max_active_paths: int = 4,
         hotwords_file: str = "",
         hotwords_score: float = 1.5,
         blank_penalty: float = 0.0,
         debug: bool = False,
         provider: str = "cpu",
+        model_type: str = "transducer",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/offline-transducer/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -102,18 +103,18 @@
                 decoder_filename=decoder,
                 joiner_filename=joiner,
             ),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
-            model_type="transducer",
+            model_type=model_type,
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         if len(hotwords_file) > 0 and decoding_method != "modified_beam_search":
             raise ValueError(
                 "Please use --decoding-method=modified_beam_search when using "
@@ -178,15 +179,15 @@
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
             model_type="paraformer",
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
@@ -242,15 +243,15 @@
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
             model_type="nemo_ctc",
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
@@ -322,15 +323,15 @@
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
             model_type="whisper",
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=16000,
             feature_dim=80,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
@@ -385,15 +386,15 @@
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
             model_type="tdnn",
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
@@ -449,15 +450,15 @@
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
             model_type="wenet_ctc",
         )
 
-        feat_config = OfflineFeatureExtractorConfig(
+        feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
         recognizer_config = OfflineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,19 @@
     OnlineLMConfig,
     OnlineModelConfig,
     OnlineParaformerModelConfig,
 )
 from _sherpa_onnx import OnlineRecognizer as _Recognizer
 from _sherpa_onnx import (
     OnlineRecognizerConfig,
+    OnlineRecognizerResult,
     OnlineStream,
     OnlineTransducerModelConfig,
     OnlineWenetCtcModelConfig,
+    OnlineNeMoCtcModelConfig,
     OnlineZipformer2CtcModelConfig,
     OnlineCtcFstDecoderConfig,
 )
 
 
 def _assert_file_exists(f: str):
     assert Path(f).is_file(), f"{f} does not exist"
@@ -54,14 +56,16 @@
         hotwords_score: float = 1.5,
         blank_penalty: float = 0.0,
         hotwords_file: str = "",
         provider: str = "cpu",
         model_type: str = "",
         lm: str = "",
         lm_scale: float = 0.1,
+        temperature_scale: float = 2.0,
+        debug: bool = False,
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -119,14 +123,18 @@
             The penalty applied on blank symbol during decoding.
           hotwords_file:
             The file containing hotwords, one words/phrases per line, and for each
             phrase the bpe/cjkchar are separated by a space.
           hotwords_score:
             The hotword score of each token for biasing word/phrase. Used only if
             hotwords_file is given with modified_beam_search as decoding method.
+          temperature_scale:
+            Temperature scaling for output symbol confidence estiamation.
+            It affects only confidence values, the decoding uses the original
+            logits without temperature.
           provider:
             onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
           model_type:
             Online transducer model type. Valid values are: conformer, lstm,
             zipformer, zipformer2. All other values lead to loading the model twice.
         """
         self = cls.__new__(cls)
@@ -145,14 +153,15 @@
 
         model_config = OnlineModelConfig(
             transducer=transducer_config,
             tokens=tokens,
             num_threads=num_threads,
             provider=provider,
             model_type=model_type,
+            debug=debug,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
             low_freq=low_freq,
             high_freq=high_freq,
@@ -189,14 +198,15 @@
             endpoint_config=endpoint_config,
             enable_endpoint=enable_endpoint_detection,
             decoding_method=decoding_method,
             max_active_paths=max_active_paths,
             hotwords_score=hotwords_score,
             hotwords_file=hotwords_file,
             blank_penalty=blank_penalty,
+            temperature_scale=temperature_scale,
         )
 
         self.recognizer = _Recognizer(recognizer_config)
         self.config = recognizer_config
         return self
 
     @classmethod
@@ -210,14 +220,15 @@
         feature_dim: int = 80,
         enable_endpoint_detection: bool = False,
         rule1_min_trailing_silence: float = 2.4,
         rule2_min_trailing_silence: float = 1.2,
         rule3_min_utterance_length: float = 20.0,
         decoding_method: str = "greedy_search",
         provider: str = "cpu",
+        debug: bool = False,
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -273,14 +284,15 @@
 
         model_config = OnlineModelConfig(
             paraformer=paraformer_config,
             tokens=tokens,
             num_threads=num_threads,
             provider=provider,
             model_type="paraformer",
+            debug=debug,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -314,14 +326,15 @@
         rule1_min_trailing_silence: float = 2.4,
         rule2_min_trailing_silence: float = 1.2,
         rule3_min_utterance_length: float = 20.0,
         decoding_method: str = "greedy_search",
         ctc_graph: str = "",
         ctc_max_active: int = 3000,
         provider: str = "cpu",
+        debug: bool = False,
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/online-ctc/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -376,14 +389,15 @@
         zipformer2_ctc_config = OnlineZipformer2CtcModelConfig(model=model)
 
         model_config = OnlineModelConfig(
             zipformer2_ctc=zipformer2_ctc_config,
             tokens=tokens,
             num_threads=num_threads,
             provider=provider,
+            debug=debug,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -408,14 +422,114 @@
         )
 
         self.recognizer = _Recognizer(recognizer_config)
         self.config = recognizer_config
         return self
 
     @classmethod
+    def from_nemo_ctc(
+        cls,
+        tokens: str,
+        model: str,
+        num_threads: int = 2,
+        sample_rate: float = 16000,
+        feature_dim: int = 80,
+        enable_endpoint_detection: bool = False,
+        rule1_min_trailing_silence: float = 2.4,
+        rule2_min_trailing_silence: float = 1.2,
+        rule3_min_utterance_length: float = 20.0,
+        decoding_method: str = "greedy_search",
+        provider: str = "cpu",
+        debug: bool = False,
+    ):
+        """
+        Please refer to
+        `<https://github.com/k2-fsa/sherpa-onnx/releases/tag/asr-models>`_
+        to download pre-trained models.
+
+        Args:
+          tokens:
+            Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
+            columns::
+
+                symbol integer_id
+
+          model:
+            Path to ``model.onnx``.
+          num_threads:
+            Number of threads for neural network computation.
+          sample_rate:
+            Sample rate of the training data used to train the model.
+          feature_dim:
+            Dimension of the feature used to train the model.
+          enable_endpoint_detection:
+            True to enable endpoint detection. False to disable endpoint
+            detection.
+          rule1_min_trailing_silence:
+            Used only when enable_endpoint_detection is True. If the duration
+            of trailing silence in seconds is larger than this value, we assume
+            an endpoint is detected.
+          rule2_min_trailing_silence:
+            Used only when enable_endpoint_detection is True. If we have decoded
+            something that is nonsilence and if the duration of trailing silence
+            in seconds is larger than this value, we assume an endpoint is
+            detected.
+          rule3_min_utterance_length:
+            Used only when enable_endpoint_detection is True. If the utterance
+            length in seconds is larger than this value, we assume an endpoint
+            is detected.
+          decoding_method:
+            The only valid value is greedy_search.
+          provider:
+            onnxruntime execution providers. Valid values are: cpu, cuda, coreml.
+          debug:
+            True to show meta data in the model.
+        """
+        self = cls.__new__(cls)
+        _assert_file_exists(tokens)
+        _assert_file_exists(model)
+
+        assert num_threads > 0, num_threads
+
+        nemo_ctc_config = OnlineNeMoCtcModelConfig(
+            model=model,
+        )
+
+        model_config = OnlineModelConfig(
+            nemo_ctc=nemo_ctc_config,
+            tokens=tokens,
+            num_threads=num_threads,
+            provider=provider,
+            debug=debug,
+        )
+
+        feat_config = FeatureExtractorConfig(
+            sampling_rate=sample_rate,
+            feature_dim=feature_dim,
+        )
+
+        endpoint_config = EndpointConfig(
+            rule1_min_trailing_silence=rule1_min_trailing_silence,
+            rule2_min_trailing_silence=rule2_min_trailing_silence,
+            rule3_min_utterance_length=rule3_min_utterance_length,
+        )
+
+        recognizer_config = OnlineRecognizerConfig(
+            feat_config=feat_config,
+            model_config=model_config,
+            endpoint_config=endpoint_config,
+            enable_endpoint=enable_endpoint_detection,
+            decoding_method=decoding_method,
+        )
+
+        self.recognizer = _Recognizer(recognizer_config)
+        self.config = recognizer_config
+        return self
+
+    @classmethod
     def from_wenet_ctc(
         cls,
         tokens: str,
         model: str,
         chunk_size: int = 16,
         num_left_chunks: int = 4,
         num_threads: int = 2,
@@ -423,14 +537,15 @@
         feature_dim: int = 80,
         enable_endpoint_detection: bool = False,
         rule1_min_trailing_silence: float = 2.4,
         rule2_min_trailing_silence: float = 1.2,
         rule3_min_utterance_length: float = 20.0,
         decoding_method: str = "greedy_search",
         provider: str = "cpu",
+        debug: bool = False,
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/wenet/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
 
@@ -487,14 +602,15 @@
         )
 
         model_config = OnlineModelConfig(
             wenet_ctc=wenet_ctc_config,
             tokens=tokens,
             num_threads=num_threads,
             provider=provider,
+            debug=debug,
         )
 
         feat_config = FeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -527,14 +643,17 @@
 
     def decode_streams(self, ss: List[OnlineStream]):
         self.recognizer.decode_streams(ss)
 
     def is_ready(self, s: OnlineStream) -> bool:
         return self.recognizer.is_ready(s)
 
+    def get_result_all(self, s: OnlineStream) -> OnlineRecognizerResult:
+        return self.recognizer.get_result(s)
+
     def get_result(self, s: OnlineStream) -> str:
         return self.recognizer.get_result(s).text.strip()
 
     def get_result_as_json_string(self, s: OnlineStream) -> str:
         return self.recognizer.get_result(s).as_json_string()
 
     def tokens(self, s: OnlineStream) -> List[str]:
```

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/CMakeLists.txt` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_feature_extractor_config.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_feature_extractor_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_keyword_spotter.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_keyword_spotter.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_offline_recognizer.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_online_recognizer.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_online_transducer_model_config.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_online_transducer_model_config.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_speaker_recognition.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_speaker_recognition.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa-onnx/python/tests/test_text2token.py` & `sherpa-onnx-1.9.24/sherpa-onnx/python/tests/test_text2token.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.9.23/sherpa_onnx.egg-info/SOURCES.txt` & `sherpa-onnx-1.9.24/sherpa_onnx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -159,34 +159,39 @@
 sherpa-onnx/csrc/offline-punctuation.cc
 sherpa-onnx/csrc/offline-punctuation.h
 sherpa-onnx/csrc/offline-recognizer-ctc-impl.h
 sherpa-onnx/csrc/offline-recognizer-impl.cc
 sherpa-onnx/csrc/offline-recognizer-impl.h
 sherpa-onnx/csrc/offline-recognizer-paraformer-impl.h
 sherpa-onnx/csrc/offline-recognizer-transducer-impl.h
+sherpa-onnx/csrc/offline-recognizer-transducer-nemo-impl.h
 sherpa-onnx/csrc/offline-recognizer-whisper-impl.h
 sherpa-onnx/csrc/offline-recognizer.cc
 sherpa-onnx/csrc/offline-recognizer.h
 sherpa-onnx/csrc/offline-rnn-lm.cc
 sherpa-onnx/csrc/offline-rnn-lm.h
 sherpa-onnx/csrc/offline-stream.cc
 sherpa-onnx/csrc/offline-stream.h
 sherpa-onnx/csrc/offline-tdnn-ctc-model.cc
 sherpa-onnx/csrc/offline-tdnn-ctc-model.h
 sherpa-onnx/csrc/offline-tdnn-model-config.cc
 sherpa-onnx/csrc/offline-tdnn-model-config.h
 sherpa-onnx/csrc/offline-transducer-decoder.h
 sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.cc
 sherpa-onnx/csrc/offline-transducer-greedy-search-decoder.h
+sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.cc
+sherpa-onnx/csrc/offline-transducer-greedy-search-nemo-decoder.h
 sherpa-onnx/csrc/offline-transducer-model-config.cc
 sherpa-onnx/csrc/offline-transducer-model-config.h
 sherpa-onnx/csrc/offline-transducer-model.cc
 sherpa-onnx/csrc/offline-transducer-model.h
 sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.cc
 sherpa-onnx/csrc/offline-transducer-modified-beam-search-decoder.h
+sherpa-onnx/csrc/offline-transducer-nemo-model.cc
+sherpa-onnx/csrc/offline-transducer-nemo-model.h
 sherpa-onnx/csrc/offline-tts-character-frontend.cc
 sherpa-onnx/csrc/offline-tts-character-frontend.h
 sherpa-onnx/csrc/offline-tts-frontend.h
 sherpa-onnx/csrc/offline-tts-impl.cc
 sherpa-onnx/csrc/offline-tts-impl.h
 sherpa-onnx/csrc/offline-tts-model-config.cc
 sherpa-onnx/csrc/offline-tts-model-config.h
@@ -235,14 +240,18 @@
 sherpa-onnx/csrc/online-lm-config.h
 sherpa-onnx/csrc/online-lm.cc
 sherpa-onnx/csrc/online-lm.h
 sherpa-onnx/csrc/online-lstm-transducer-model.cc
 sherpa-onnx/csrc/online-lstm-transducer-model.h
 sherpa-onnx/csrc/online-model-config.cc
 sherpa-onnx/csrc/online-model-config.h
+sherpa-onnx/csrc/online-nemo-ctc-model-config.cc
+sherpa-onnx/csrc/online-nemo-ctc-model-config.h
+sherpa-onnx/csrc/online-nemo-ctc-model.cc
+sherpa-onnx/csrc/online-nemo-ctc-model.h
 sherpa-onnx/csrc/online-paraformer-decoder.h
 sherpa-onnx/csrc/online-paraformer-model-config.cc
 sherpa-onnx/csrc/online-paraformer-model-config.h
 sherpa-onnx/csrc/online-paraformer-model.cc
 sherpa-onnx/csrc/online-paraformer-model.h
 sherpa-onnx/csrc/online-recognizer-ctc-impl.h
 sherpa-onnx/csrc/online-recognizer-impl.cc
@@ -380,27 +389,29 @@
 sherpa-onnx/csrc/wave-writer.cc
 sherpa-onnx/csrc/wave-writer.h
 sherpa-onnx/jni/CMakeLists.txt
 sherpa-onnx/jni/audio-tagging.cc
 sherpa-onnx/jni/common.h
 sherpa-onnx/jni/jni.cc
 sherpa-onnx/jni/keyword-spotter.cc
+sherpa-onnx/jni/offline-punctuation.cc
 sherpa-onnx/jni/offline-recognizer.cc
 sherpa-onnx/jni/offline-stream.cc
 sherpa-onnx/jni/offline-tts.cc
 sherpa-onnx/jni/online-recognizer.cc
 sherpa-onnx/jni/online-stream.cc
 sherpa-onnx/jni/speaker-embedding-extractor.cc
 sherpa-onnx/jni/speaker-embedding-manager.cc
 sherpa-onnx/jni/spoken-language-identification.cc
 sherpa-onnx/jni/voice-activity-detector.cc
 sherpa-onnx/jni/wave-reader.cc
 sherpa-onnx/kotlin-api/AudioTagging.kt
 sherpa-onnx/kotlin-api/FeatureConfig.kt
 sherpa-onnx/kotlin-api/KeywordSpotter.kt
+sherpa-onnx/kotlin-api/OfflinePunctuation.kt
 sherpa-onnx/kotlin-api/OfflineRecognizer.kt
 sherpa-onnx/kotlin-api/OfflineStream.kt
 sherpa-onnx/kotlin-api/OnlineRecognizer.kt
 sherpa-onnx/kotlin-api/OnlineStream.kt
 sherpa-onnx/kotlin-api/Speaker.kt
 sherpa-onnx/kotlin-api/SpokenLanguageIdentification.kt
 sherpa-onnx/kotlin-api/Vad.kt
@@ -456,14 +467,16 @@
 sherpa-onnx/python/csrc/offline-zipformer-ctc-model-config.h
 sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.cc
 sherpa-onnx/python/csrc/online-ctc-fst-decoder-config.h
 sherpa-onnx/python/csrc/online-lm-config.cc
 sherpa-onnx/python/csrc/online-lm-config.h
 sherpa-onnx/python/csrc/online-model-config.cc
 sherpa-onnx/python/csrc/online-model-config.h
+sherpa-onnx/python/csrc/online-nemo-ctc-model-config.cc
+sherpa-onnx/python/csrc/online-nemo-ctc-model-config.h
 sherpa-onnx/python/csrc/online-paraformer-model-config.cc
 sherpa-onnx/python/csrc/online-paraformer-model-config.h
 sherpa-onnx/python/csrc/online-recognizer.cc
 sherpa-onnx/python/csrc/online-recognizer.h
 sherpa-onnx/python/csrc/online-stream.cc
 sherpa-onnx/python/csrc/online-stream.h
 sherpa-onnx/python/csrc/online-transducer-model-config.cc
```

