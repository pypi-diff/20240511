# Comparing `tmp/niwatoko-1.1.3.tar.gz` & `tmp/niwatoko-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.1.3.tar", last modified: Sat May 11 07:10:36 2024, max compression
+gzip compressed data, was "niwatoko-1.1.4.tar", last modified: Sat May 11 19:02:51 2024, max compression
```

## Comparing `niwatoko-1.1.3.tar` & `niwatoko-1.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.085992 niwatoko-1.1.3/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.3/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 07:10:36.085826 niwatoko-1.1.3/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-11 04:01:06.000000 niwatoko-1.1.3/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.078935 niwatoko-1.1.3/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.3/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     7769 2024-05-11 06:56:53.000000 niwatoko-1.1.3/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.077332 niwatoko-1.1.3/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.077371 niwatoko-1.1.3/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.080182 niwatoko-1.1.3/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.3/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.3/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.080384 niwatoko-1.1.3/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.3/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.3/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.079801 niwatoko-1.1.3/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 07:10:36.000000 niwatoko-1.1.3/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 07:10:36.086028 niwatoko-1.1.3/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 07:07:14.000000 niwatoko-1.1.3/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.082156 niwatoko-1.1.3/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.3/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.3/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.3/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.3/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.3/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 07:10:36.085492 niwatoko-1.1.3/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.3/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.3/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-11 00:55:54.000000 niwatoko-1.1.3/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-11 00:56:05.000000 niwatoko-1.1.3/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.3/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.3/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.3/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.3/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.3/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.3/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.3/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.3/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.3/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.3/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.3/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.3/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.575771 niwatoko-1.1.4/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.4/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 19:02:51.575368 niwatoko-1.1.4/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-11 04:01:06.000000 niwatoko-1.1.4/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.571132 niwatoko-1.1.4/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.4/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     8724 2024-05-11 18:42:36.000000 niwatoko-1.1.4/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.570301 niwatoko-1.1.4/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.570338 niwatoko-1.1.4/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.572181 niwatoko-1.1.4/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.4/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.4/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.572298 niwatoko-1.1.4/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.4/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.4/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.571901 niwatoko-1.1.4/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 19:02:51.000000 niwatoko-1.1.4/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 19:02:51.575807 niwatoko-1.1.4/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 19:02:18.000000 niwatoko-1.1.4/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.573294 niwatoko-1.1.4/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.4/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.4/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.4/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.4/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.4/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 19:02:51.575152 niwatoko-1.1.4/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.4/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.4/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-11 00:55:54.000000 niwatoko-1.1.4/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-11 00:56:05.000000 niwatoko-1.1.4/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.4/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.4/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.4/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.4/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.4/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.4/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.4/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.4/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.4/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.4/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.4/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.4/tests/test_parser.py
```

### Comparing `niwatoko-1.1.3/LICENSE` & `niwatoko-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/PKG-INFO` & `niwatoko-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.3
+Version: 1.1.4
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.3/README.md` & `niwatoko-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/niwatoko/cli.py` & `niwatoko-1.1.4/niwatoko/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 @click.command()
 @click.argument('file_path', type=click.Path(exists=True), required=False)
 @click.option('-m', '--model', type=click.Choice(['openai', 'claude']), default='claude', help='使用するモデルを選択します。')
 @click.option('-o', '--output', type=click.Path(), help='生成されたコードの出力先ファイルを指定します。')
 @click.option('-v', '--version',  is_flag=True, help='バージョン情報を表示します。')
 
 def main(file_path, model, output, version):
+    print('file_path:', file_path)
     """
     自然言語のソースコードを読み込んで実行するコマンドラインインターフェース。
 
     Args:
         file_path (str): 自然言語のソースコードが書かれたファイルのパス。
         model (str): 使用するモデル（OpenAIまたはClaude）。
         output (str): 生成されたコードの出力先ファイルのパス。
@@ -35,15 +36,15 @@
         return
     if not file_path:
         print("ファイルパスが指定されていません。")
         return
 
     processed_content = process_imports(file_path)
 
-    print("実行中...")
+    print("実行中... (Processing...)")
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
 
     if model == 'openai':
@@ -66,20 +67,20 @@
     # ぐるぐるアニメーションを停止
     done = True
     spinner.join()
 
     if output:
         with open(output, 'w', encoding = "utf-8") as file:
             file.write(generated_code)
-            print(f"\n生成されたコードを {output} に書き出しました。")
+            print(f"生成されたコードを {output} に書き出しました。")
+            print(f"Generated code has been written to {output}.")
 
 def spin(done):
     """
     ぐるぐるアニメーションを表示する関数
-
     Args:
         done (function): アニメーションを停止するかどうかを判定する関数
     """
     for c in itertools.cycle(['|', '/', '-', '\\']):
         if done():
             break
         sys.stdout.write(f'\r{c}')
@@ -90,24 +91,25 @@
 import os
 def process_imports(file_path):
     with open(file_path, 'r') as file:
         lines = file.readlines()
     
     output = []
     for line in lines:
+        output.extend(process_variable_imports(line))
         if line.startswith('- '):
             parts = line.strip().split(' = ')
             if len(parts) == 2:
                 import_path = parts[1].strip()
+                print('import_path:', import_path)
                 if '[' in import_path and not import_path.startswith('['):
                     # ブラケットで囲まれたパスを抽出
                     path_within_brackets = import_path[import_path.index('[') + 1:import_path.index(']')]
                     # 拡張子を取得
                     extension = path_within_brackets.split('.')[-1]
-                    print(extension)
                     # 拡張子に応じた処理を行う
                     if extension == 'md':
                         output.extend(process_md_import(import_path, line))
                     elif extension == 'py':
                         output.extend(process_py_import(import_path, line))
                     elif extension == 'rst':
                         output.extend(process_rst_import(import_path, line))
@@ -120,14 +122,37 @@
             else:
                 output.append(line)
         else:
             output.append(line)
     
     return ''.join(output)
 
+def process_variable_imports(line):
+    """
+    {{}}で囲まれた変数のインポートを処理する関数
+
+    Args:
+        line (str): ファイルの行
+
+    Returns:
+        list: 処理後の出力行のリスト
+    """
+    output = []
+    if '{{' in line and '}}' in line:
+        # {{ }} で囲まれた変数を抽出
+        variable = line[line.index('{{') + 2:line.index('}}')]
+        # print(variable)
+        # 変数名を小文字に変換し、拡張子.mdを追加
+        import_path = variable.lower() + '.md'
+        # 同一階層内のファイルの内容を取得
+        import_content = get_file_content(import_path)
+        output.extend([line, '```\n', import_content, '```\n'])
+    else:
+        output.append(line)
+    return output
 def process_no_extension_import(import_path, line):
     """
     Markdownファイルのインポートを処理する関数
 
     Args:
         import_path (str): インポートするファイルのパス
         line (str): インポート文の行
```

### Comparing `niwatoko-1.1.3/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.1.4/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.1.4/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/niwatoko/grammar/system.md` & `niwatoko-1.1.4/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.1.4/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.3
+Version: 1.1.4
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.3/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.1.4/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/setup.py` & `niwatoko-1.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.1.3',
+    version='1.1.4',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.1.3/tests/README.md` & `niwatoko-1.1.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/__init__.py` & `niwatoko-1.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_compiler.md` & `niwatoko-1.1.4/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_compiler.py` & `niwatoko-1.1.4/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_compiler_v1_2.py` & `niwatoko-1.1.4/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/__init__.py` & `niwatoko-1.1.4/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/output copy.md` & `niwatoko-1.1.4/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/output.md` & `niwatoko-1.1.4/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/output.py` & `niwatoko-1.1.4/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/output_.md` & `niwatoko-1.1.4/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_doc1.md` & `niwatoko-1.1.4/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_doc2.md` & `niwatoko-1.1.4/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_doc3.md` & `niwatoko-1.1.4/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.1.4/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.1.4/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.1.4/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.1.4/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.1.4/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_docs/test_import_function.md` & `niwatoko-1.1.4/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_interpreter.py` & `niwatoko-1.1.4/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.3/tests/test_parser.py` & `niwatoko-1.1.4/tests/test_parser.py`

 * *Files identical despite different names*

