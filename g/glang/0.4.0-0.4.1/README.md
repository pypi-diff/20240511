# Comparing `tmp/glang-0.4.0.tar.gz` & `tmp/glang-0.4.1.tar.gz`

## Comparing `glang-0.4.0.tar` & `glang-0.4.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 glang-0.4.0/.gitattributes
--rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 glang-0.4.0/.pylintrc
--rwxr-xr-x   0        0        0     2256 2020-02-02 00:00:00.000000 glang-0.4.0/bootstrap.sh
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 glang-0.4.0/demo.c3
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 glang-0.4.0/glang.spec
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 glang-0.4.0/printers.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 glang-0.4.0/.vscode/launch.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 glang-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/__init__.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/driver.py
--rw-r--r--   0        0        0    40944 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/graphene_parser.py
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/target.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/bin/parser -> ../../../dist/parser
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/__init__.py
--rw-r--r--   0        0        0    19637 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/builtin_callables.py
--rw-r--r--   0        0        0    29459 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/builtin_types.py
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/debug.py
--rw-r--r--   0        0        0    30879 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/expressions.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/floats.py
--rw-r--r--   0        0        0    19928 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/generatable.py
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/interfaces.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/mangling.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/strings.py
--rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/translation_unit.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/type_conversions.py
--rw-r--r--   0        0        0    50601 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/type_resolution.py
--rw-r--r--   0        0        0    15902 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/user_facing_errors.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/algorithms.c3
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arithmetic.c3
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/assert.c3
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/assignments.c3
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/fcntl.c3
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/format.c3
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/io.c3
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/iterators.c3
--rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/json.c3
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/logical.c3
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/math.c3
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/memory.c3
--rw-r--r--   0        0        0    15388 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/rb_tree.c3
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/span.c3
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/string.c3
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/type_traits.c3
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/unistd.c3
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/util.c3
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/vector.c3
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/wrappers.c3
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/runtime.S
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/syscalls.c3
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/sys/kstat.c3
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arm_linux/runtime.S
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arm_linux/syscalls.c3
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/mman.c3
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/stat.c3
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/types.c3
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/uio.c3
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/runtime.S
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/syscalls.c3
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/sys/kstat.c3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/__init__.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/file_info.c3
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/lexer_parser.py
--rw-r--r--   0        0        0    58452 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/parser.c3
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/self_hosted_parser.py
--rw-r--r--   0        0        0    26857 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/syntax_tree.c3
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/aarch64_linux.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/arm_linux.yml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/x86_64_linux.yml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/utils/stack.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 glang-0.4.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 glang-0.4.0/LICENSE
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 glang-0.4.0/hatch_build.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 glang-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 glang-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 glang-0.4.1/.gitattributes
+-rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 glang-0.4.1/.pylintrc
+-rwxr-xr-x   0        0        0     2256 2020-02-02 00:00:00.000000 glang-0.4.1/bootstrap.sh
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glang-0.4.1/demo.c3
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 glang-0.4.1/glang.spec
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 glang-0.4.1/printers.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 glang-0.4.1/.vscode/launch.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 glang-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/__init__.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/driver.py
+-rw-r--r--   0        0        0    40944 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/graphene_parser.py
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/target.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/bin/parser -> ../../../dist/parser
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/__init__.py
+-rw-r--r--   0        0        0    19637 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/builtin_callables.py
+-rw-r--r--   0        0        0    29459 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/builtin_types.py
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/debug.py
+-rw-r--r--   0        0        0    30879 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/expressions.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/floats.py
+-rw-r--r--   0        0        0    19928 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/generatable.py
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/interfaces.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/mangling.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/strings.py
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/translation_unit.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/type_conversions.py
+-rw-r--r--   0        0        0    50601 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/type_resolution.py
+-rw-r--r--   0        0        0    15902 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/codegen/user_facing_errors.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/algorithms.c3
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/arithmetic.c3
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/assert.c3
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/assignments.c3
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/fcntl.c3
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/format.c3
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/io.c3
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/iterators.c3
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/json.c3
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/logical.c3
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/math.c3
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/memory.c3
+-rw-r--r--   0        0        0    15388 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/rb_tree.c3
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/span.c3
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/string.c3
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/type_traits.c3
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/unistd.c3
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/util.c3
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/vector.c3
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/wrappers.c3
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/aarch64_linux/runtime.S
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/aarch64_linux/syscalls.c3
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/aarch64_linux/sys/kstat.c3
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/arm_linux/runtime.S
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/arm_linux/syscalls.c3
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/sys/mman.c3
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/sys/stat.c3
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/sys/types.c3
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/sys/uio.c3
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/x86_64_linux/runtime.S
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/x86_64_linux/syscalls.c3
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/lib/std/x86_64_linux/sys/kstat.c3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/__init__.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/file_info.c3
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/lexer_parser.py
+-rw-r--r--   0        0        0    58452 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/parser.c3
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/self_hosted_parser.py
+-rw-r--r--   0        0        0    26857 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/parser/syntax_tree.c3
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/targets/aarch64_linux.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/targets/arm_linux.yml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/targets/x86_64_linux.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 glang-0.4.1/src/glang/utils/stack.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 glang-0.4.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 glang-0.4.1/LICENSE
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 glang-0.4.1/hatch_build.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 glang-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 glang-0.4.1/PKG-INFO
```

### Comparing `glang-0.4.0/.pylintrc` & `glang-0.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/bootstrap.sh` & `glang-0.4.1/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/glang.spec` & `glang-0.4.1/glang.spec`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:           glang
-Version:        0.4.0
+Version:        0.4.1
 Release:        %autorelease
 Summary:        A Graphene front-end for LLVM
 
 License:        AGPL-3.0-only
 URL:            https://github.com/DaveDuck321/GrapheneLang
 Source0:        %{url}/archive/refs/tags/v%{version}.tar.gz
 Source1:        %{url}/archive/refs/tags/bootstrap/1.tar.gz
```

### Comparing `glang-0.4.0/printers.py` & `glang-0.4.1/printers.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/.vscode/launch.json` & `glang-0.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/graphene_parser.py` & `glang-0.4.1/src/glang/graphene_parser.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/target.py` & `glang-0.4.1/src/glang/target.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/__init__.py` & `glang-0.4.1/src/glang/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/builtin_callables.py` & `glang-0.4.1/src/glang/codegen/builtin_callables.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/builtin_types.py` & `glang-0.4.1/src/glang/codegen/builtin_types.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/debug.py` & `glang-0.4.1/src/glang/codegen/debug.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/expressions.py` & `glang-0.4.1/src/glang/codegen/expressions.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/floats.py` & `glang-0.4.1/src/glang/codegen/floats.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/generatable.py` & `glang-0.4.1/src/glang/codegen/generatable.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/interfaces.py` & `glang-0.4.1/src/glang/codegen/interfaces.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/mangling.py` & `glang-0.4.1/src/glang/codegen/mangling.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/strings.py` & `glang-0.4.1/src/glang/codegen/strings.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/translation_unit.py` & `glang-0.4.1/src/glang/codegen/translation_unit.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/type_conversions.py` & `glang-0.4.1/src/glang/codegen/type_conversions.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/type_resolution.py` & `glang-0.4.1/src/glang/codegen/type_resolution.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/codegen/user_facing_errors.py` & `glang-0.4.1/src/glang/codegen/user_facing_errors.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/algorithms.c3` & `glang-0.4.1/src/glang/lib/std/algorithms.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/arithmetic.c3` & `glang-0.4.1/src/glang/lib/std/arithmetic.c3`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,14 @@
 
 @operator [U, V] > : (lhs: U, rhs: V) -> ArithmeticCompareResult<U, V> = {
     let lhs_widen: CommonArithmeticType<U, V> = lhs;
     let rhs_widen: CommonArithmeticType<U, V> = rhs;
     return __builtin_is_greater_than(lhs_widen, rhs_widen);
 }
 
-// TODO: remove unnecessary widening by allowing partial specialization
-function [T] Narrow : (value : i128) -> TypeIf<T, IsIntegral<T>> = {
-    return __builtin_narrow<T>(value);
-}
-
 @operator [U, V] <= : (lhs: U, rhs: V) -> ArithmeticCompareResult<U, V> = {
     return !(lhs > rhs);
 }
 
 @operator [U, V] >= : (lhs: U, rhs: V) -> ArithmeticCompareResult<U, V> = {
     return !(lhs < rhs);
 }
```

### Comparing `glang-0.4.0/src/glang/lib/std/assignments.c3` & `glang-0.4.1/src/glang/lib/std/assignments.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/fcntl.c3` & `glang-0.4.1/src/glang/lib/std/fcntl.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/format.c3` & `glang-0.4.1/src/glang/lib/std/format.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/io.c3` & `glang-0.4.1/src/glang/lib/std/io.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/iterators.c3` & `glang-0.4.1/src/glang/lib/std/iterators.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/json.c3` & `glang-0.4.1/src/glang/lib/std/json.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/logical.c3` & `glang-0.4.1/src/glang/lib/std/logical.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/math.c3` & `glang-0.4.1/src/glang/lib/std/math.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/memory.c3` & `glang-0.4.1/src/glang/lib/std/memory.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/rb_tree.c3` & `glang-0.4.1/src/glang/lib/std/rb_tree.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/span.c3` & `glang-0.4.1/src/glang/lib/std/span.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/string.c3` & `glang-0.4.1/src/glang/lib/std/string.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/type_traits.c3` & `glang-0.4.1/src/glang/lib/std/type_traits.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/util.c3` & `glang-0.4.1/src/glang/lib/std/util.c3`

 * *Files 6% similar despite different names*

```diff
@@ -59,12 +59,24 @@
 
 function as_logical : (value : i8)   -> u8   = { return __builtin_bitcast<u8>(value); }
 function as_logical : (value : i16)  -> u16  = { return __builtin_bitcast<u16>(value); }
 function as_logical : (value : i32)  -> u32  = { return __builtin_bitcast<u32>(value); }
 function as_logical : (value : i64)  -> u64  = { return __builtin_bitcast<u64>(value); }
 function as_logical : (value : i128) -> u128 = { return __builtin_bitcast<u128>(value); }
 
+function [Ret, In] Narrow : (value : In) ->
+TypeIf<
+    Ret,
+    Either<
+        Both<IsIntegral<Ret>, IsIntegral<In>>,
+        Both<IsLogical<Ret>, IsLogical<In>>
+    >> =
+{
+    // TODO: reject sizeof(Ret) >= sizeof(In) at compile time
+    return __builtin_narrow<Ret>(value);
+}
+
 function value<TrueType> : () -> bool = { return true; }
 function value<FalseType> : () -> bool = { return false; }
 
 // TODO: constant version of this is impossible atm (since __builtin_has_next is mutable)
 function [T] has_next : (iter : T mut&) -> bool = { return iter:__builtin_has_next(); }
```

### Comparing `glang-0.4.0/src/glang/lib/std/vector.c3` & `glang-0.4.1/src/glang/lib/std/vector.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/wrappers.c3` & `glang-0.4.1/src/glang/lib/std/wrappers.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/aarch64_linux/runtime.S` & `glang-0.4.1/src/glang/lib/std/aarch64_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/aarch64_linux/syscalls.c3` & `glang-0.4.1/src/glang/lib/std/aarch64_linux/syscalls.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/aarch64_linux/sys/kstat.c3` & `glang-0.4.1/src/glang/lib/std/aarch64_linux/sys/kstat.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/arm_linux/runtime.S` & `glang-0.4.1/src/glang/lib/std/arm_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/sys/mman.c3` & `glang-0.4.1/src/glang/lib/std/sys/mman.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/sys/stat.c3` & `glang-0.4.1/src/glang/lib/std/sys/stat.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/x86_64_linux/runtime.S` & `glang-0.4.1/src/glang/lib/std/x86_64_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/lib/std/x86_64_linux/syscalls.c3` & `glang-0.4.1/src/glang/lib/std/x86_64_linux/syscalls.c3`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     fd: int,
     offset: off_t
 ) -> iptr = {
     return _syscall_6(addr, length, prot, flags,
                       fd, offset, /* mmap */ 9);
 }
 
-function sys_munmap : (addr: isize, length : isize) -> int = {
-    let result : i64 = _syscall_2(addr, length, /* munmap */ 11);
-    return Narrow<int>(result);
+function sys_munmap : (addr: isize, length : isize) -> i64 = {
+    return _syscall_2(addr, length, /* munmap */ 11);
 }
 
 function sys_exit : (code : int) -> void = {
     _syscall_1(code, 60);
 }
```

### Comparing `glang-0.4.0/src/glang/parser/file_info.c3` & `glang-0.4.1/src/glang/parser/file_info.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/parser/lexer_parser.py` & `glang-0.4.1/src/glang/parser/lexer_parser.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/parser/parser.c3` & `glang-0.4.1/src/glang/parser/parser.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/parser/self_hosted_parser.py` & `glang-0.4.1/src/glang/parser/self_hosted_parser.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/parser/syntax_tree.c3` & `glang-0.4.1/src/glang/parser/syntax_tree.c3`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/targets/aarch64_linux.yml` & `glang-0.4.1/src/glang/targets/aarch64_linux.yml`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/src/glang/targets/arm_linux.yml` & `glang-0.4.1/src/glang/targets/arm_linux.yml`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/.gitignore` & `glang-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/LICENSE` & `glang-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/hatch_build.py` & `glang-0.4.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `glang-0.4.0/pyproject.toml` & `glang-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling~=1.21"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "glang"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name = "Antros Economides", email = "antroseconomides@hotmail.co.uk" },
   { name = "Tom Grant", email = "thomas.grant.mail@gmail.com" },
 ]
 description = "A Graphene front-end for LLVM"
 # TODO readme = "README.md"
 license = "AGPL-3.0-only"
```

### Comparing `glang-0.4.0/PKG-INFO` & `glang-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: glang
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Graphene front-end for LLVM
 Project-URL: Homepage, https://github.com/DaveDuck321/GrapheneLang/
 Project-URL: Bug Tracker, https://github.com/DaveDuck321/GrapheneLang/issues
 Author-email: Antros Economides <antroseconomides@hotmail.co.uk>, Tom Grant <thomas.grant.mail@gmail.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

