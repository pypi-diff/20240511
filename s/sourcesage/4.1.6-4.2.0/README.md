# Comparing `tmp/sourcesage-4.1.6.tar.gz` & `tmp/sourcesage-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.1.6.tar", last modified: Fri May 10 14:17:22 2024, max compression
+gzip compressed data, was "sourcesage-4.2.0.tar", last modified: Sat May 11 21:16:31 2024, max compression
```

## Comparing `sourcesage-4.1.6.tar` & `sourcesage-4.2.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 14:17:17.000000 sourcesage-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-10 14:17:22.028912 sourcesage-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-05-10 14:17:17.000000 sourcesage-4.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:17:22.028912 sourcesage-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-10 14:17:18.000000 sourcesage-4.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.024912 sourcesage-4.1.6/sourcesage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/.SourceSageignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/language_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/ChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/ChangelogUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/DiffChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/EnvFileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/GitHubIssueRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/IssuesToMarkdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/StageInfoGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/StagedDiffGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/markdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/source_sage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-10 14:17:18.000000 sourcesage-4.1.6/tests/test_sourcesage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 21:16:27.000000 sourcesage-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-11 21:16:31.927785 sourcesage-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-11 21:16:27.000000 sourcesage-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 21:16:31.927785 sourcesage-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-11 21:16:28.000000 sourcesage-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.923786 sourcesage-4.2.0/sourcesage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.923786 sourcesage-4.2.0/sourcesage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/.SourceSageignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/sourcesage/config/ISSUES_RESOLVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/sourcesage/config/STAGE_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/config/language_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/sourcesage/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/ChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/ChangelogUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/DiffChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/EnvFileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/IssuesToMarkdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/StageInfoGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/StagedDiffGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/markdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-11 21:16:28.000000 sourcesage-4.2.0/sourcesage/modules/source_sage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/sourcesage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 21:16:31.000000 sourcesage-4.2.0/sourcesage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:16:31.927785 sourcesage-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-11 21:16:28.000000 sourcesage-4.2.0/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.1.6/LICENSE` & `sourcesage-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/PKG-INFO` & `sourcesage-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.1.6
+Version: 4.2.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
@@ -53,17 +53,20 @@
 
 >[!IMPORTANT]
 >このリポジトリ自体も[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
 
 
 ## 更新内容
 
+## 更新内容
+
+- [【2024/05/12】 SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.2.0)
+  - ステージング情報のテンプレートに絵文字と[GAIAH](https://github.com/Sunwood-ai-labs/Gaiah)に対応
 - [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2)
   - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
-
 - [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
   - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
   - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
   - CLI引数の追加とコアモジュールの修正
   - プロジェクトの構成とファイルの変更によるシンプル化
   - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
 - [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
@@ -81,14 +84,15 @@
   - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
 - 【2024/03/29】 初期リリース
 
+
 ## 主な機能
 
 ### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
 
 - GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
 - 課題を効率的に特定し、迅速に解決策を見つけられます
 
@@ -146,15 +150,15 @@
 
 ```bash 
 sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
 上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+>[!Note] GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
 
 以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 ### 除外ファイルの指定
 
 作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
 
@@ -204,21 +208,33 @@
 
 `SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
 
 このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
 
+絵文字を活用した視覚的に分かりやすいコミットメッセージの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+
+このファイルでは、コミットメッセージのフォーマットに絵文字を取り入れ、変更内容をより直感的に表現しています。
+
+また、Gaiah用のコミットメッセージ生成を支援するテンプレートの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+
+このテンプレートでは、効果的で意味のあるコミットメッセージを作成するためのベストプラクティスに従ったガイドラインを提供しています。主要な変更とその目的に焦点を当て、コミットで行われた変更を明確かつ簡潔に説明するように促します。
+
 Issueとマージされたファイルの例はこちらです。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 
 このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
 
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。絵文字の活用やGaiahのテンプレートを利用することで、よりわかりやすく効果的なコミットメッセージの作成が可能になります。
 
 ## 3. DocuMind：リリース後のドキュメント化
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.6 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.2.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
@@ -25,17 +25,21 @@
                                WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
-(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
-30ã SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/
-tag/vv4.1.2) - GitHub
+(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ ## æ´æ°åå®¹
+- [ã2024/05/12ã SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/v4.2.0) -
+ã¹ãã¼ã¸ã³ã°æå ±ã®ãã³ãã¬ã¼ãã«çµµæå­ã¨[GAIAH](https://
+github.com/Sunwood-ai-labs/Gaiah)ã«å¯¾å¿ - [ã2024/04/30ã SourceSage
+4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2) -
+GitHub
 Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
 - [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
 SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
@@ -111,15 +115,15 @@
 ãããã®ãã¡ã¤ã«ãä½¿ã£ã¦ãAIã«ãããã­ã¸ã§ã¯ãã®è§£æãèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãªã©ãè¡ããã¨ãã§ãã¾ãã
 ### ãªãã¸ããªã®Issueãåå¾ããæ¹æ³
 ããã©ã«ãã§ã¯ãSourceSageã¯ç¾å¨ã®ãã£ã¬ã¯ããªããã­ã¸ã§ã¯ãã®ã«ã¼ãã¨ãã¦è§£æãã¾ãããã ããGitHubä¸ã®ãªãã¸ããªã®Issueãåå¾ãããå ´åã¯ãä»¥ä¸ã®ããã«ãªãã¸ããªã®ãªã¼ãã¼åã¨ãªãã¸ããªåãã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
 ```bash sourcesage --owner Sunwood-ai-labs --repository SourceSage ```
 ä¸è¨ã®ä¾ã§ã¯ã`Sunwood-ai-
 labs`ããªãã¸ããªã®ãªã¼ãã¼åã`SourceSage`ããªãã¸ããªåã§ãããããã®å¼æ°ãæå®ãããã¨ã§ãSourceSageã¯GitHub
 APIãä½¿ã£ã¦ãªãã¸ããªã®ãªã¼ãã³ãªIssueãåå¾ãã`open_issues_filtered.json`ãã¡ã¤ã«ã«ä¿å­ãã¾ãã
-Note: GitHub
+>[!Note] GitHub
 APIãä½¿ç¨ããã«ã¯ãã¤ã³ã¿ã¼ãããæ¥ç¶ãå¿è¦ã§ããã¾ãããªãã¸ããªããã©ã¤ãã¼ãã®å ´åã¯ãé©åãªã¢ã¯ã»ã¹ãã¼ã¯ã³ãè¨­å®ããå¿è¦ãããã¾ãã
 ä»¥ä¸ããSourceSageã®åºæ¬çãªä½¿ç¨æ¹æ³ã§ãããã²èªåã®ãã­ã¸ã§ã¯ãã§SourceSageãæ´»ç¨ãã¦ãéçºå¹çã®åä¸ãä½é¨ãã¦ã¿ã¦ãã ããï¼
 ### é¤å¤ãã¡ã¤ã«ã®æå®
 ä½æ¥­ãã£ã¬ã¯ããªã«`.SourceSageignore`ãã¡ã¤ã«ãä½æãããã¨ã§ãä»»æã®ãã¡ã¤ã«ããã£ã¬ã¯ããªãå¦çããé¤å¤ã§ãã¾ãããã®ãã¡ã¤ã«ã«ã¯ãé¤å¤ããããã¡ã¤ã«ããã£ã¬ã¯ããªã®ãã¿ã¼ã³ã1è¡ãã¤è¨è¿°ãã¾ããä¾ãã°ãä»¥ä¸ã®ããã«æå®ãã¾ãï¼
 ```plaintext # .SourceSageignoreã®ä¾ node_modules/ *.log *.tmp ```
 ä¸è¨ã®ä¾ã§ã¯ã`node_modules`ãã£ã¬ã¯ããªã¨ãæ¡å¼µå­ã`.log`ã¾ãã¯`.tmp`ã®ãã¡ã¤ã«ãé¤å¤ããã¾ãã
 `.SourceSageignore`ãã¡ã¤ã«ãä½¿ç¨ããå ´åã¯ãä»¥ä¸ã®ããã«ã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
@@ -146,20 +150,30 @@
 CommitCraftã¯ãéçºä¸­ã®ã¹ãã¼ã¸ãããå¤æ´ãè¿½è·¡ããAIãæ´»ç¨ãã¦é©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçæãããã¼ã«ã§ããããã«ãããéçºèã¯ã³ãããã®åå®¹ãæ­£ç¢ºã«è¨è¿°ãããã¨ãã§ãããã­ã¸ã§ã¯ãã®å¤æ´å±¥æ­´ãããæç¢ºã«ç®¡çã§ãã¾ãã
 `SourceSageAssets/COMMIT_CRAFT/
 STAGED_DIFF.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/
 Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_PROMT.md)
 ãã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ããã®ã¾ã¾AIã«å¥åãããã¨ã§ãAIãã³ãããã¡ãã»ã¼ã¸ãçæãã¾ããAIã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åãåæãããã®åå®¹ãè¦ç´ããã³ãããã¡ãã»ã¼ã¸ãææ¡ãã¾ãã
+çµµæå­ãæ´»ç¨ããè¦è¦çã«åãããããã³ãããã¡ãã»ã¼ã¸ã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+ãã®ãã¡ã¤ã«ã§ã¯ãã³ãããã¡ãã»ã¼ã¸ã®ãã©ã¼ãããã«çµµæå­ãåãå¥ããå¤æ´åå®¹ãããç´æçã«è¡¨ç¾ãã¦ãã¾ãã
+ã¾ããGaiahç¨ã®ã³ãããã¡ãã»ã¼ã¸çæãæ¯æ´ãããã³ãã¬ã¼ãã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+ãã®ãã³ãã¬ã¼ãã§ã¯ãå¹æçã§æå³ã®ããã³ãããã¡ãã»ã¼ã¸ãä½æããããã®ãã¹ããã©ã¯ãã£ã¹ã«å¾ã£ãã¬ã¤ãã©ã¤ã³ãæä¾ãã¦ãã¾ããä¸»è¦ãªå¤æ´ã¨ãã®ç®çã«ç¦ç¹ãå½ã¦ãã³ãããã§è¡ãããå¤æ´ãæç¢ºãã¤ç°¡æ½ã«èª¬æããããã«ä¿ãã¾ãã
 Issueã¨ãã¼ã¸ããããã¡ã¤ã«ã®ä¾ã¯ãã¡ãã§ãã ä¾ï¼[`docs/
 SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-
 ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 ãã®ãã¡ã¤ã«ã«ã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åã¨ãªã¼ãã³ãªIssueã®æå ±ãå«ã¾ãã¦ãã¾ããAIã¯ãããã®æå ±ãçµã¿åããã¦åæããããåæ¬çãªã³ãããã¡ãã»ã¼ã¸ãçæãã¾ãã
-CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ãã
+CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ããçµµæå­ã®æ´»ç¨ãGaiahã®ãã³ãã¬ã¼ããå©ç¨ãããã¨ã§ãããããããããå¹æçãªã³ãããã¡ãã»ã¼ã¸ã®ä½æãå¯è½ã«ãªãã¾ãã
 ## 3. DocuMindï¼ãªãªã¼ã¹å¾ã®ãã­ã¥ã¡ã³ãå
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                                 head_icon7.png]
 DocuMindã¯ããªãªã¼ã¹å¾ã®ãã­ã¸ã§ã¯ãã®çµ±åã¨ãã­ã¥ã¡ã³ãåãæ¯æ´ãããã¼ã«ã§ããSourceSageãçæãããã­ã¸ã§ã¯ãã®æ¦è¦ã¨ãèªåçæãããGitã®å¤æ´å±¥æ­´ãçµã¿åããããã¨ã§ããã­ã¸ã§ã¯ãã®å¨ä½åãæç¢ºã«ææ¡ã§ãã¾ããããã«ãããéçºèã¯ãã­ã¸ã§ã¯ãã®ãã­ã¥ã¡ã³ããå¹ççã«ä½æããã¡ã³ããã³ã¹æ§ãåä¸ããããã¨ãã§ãã¾ãã
 `SourceSageAssets/
 DocuMind.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.6/README.md` & `sourcesage-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,20 @@
 
 >[!IMPORTANT]
 >このリポジトリ自体も[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
 
 
 ## 更新内容
 
+## 更新内容
+
+- [【2024/05/12】 SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.2.0)
+  - ステージング情報のテンプレートに絵文字と[GAIAH](https://github.com/Sunwood-ai-labs/Gaiah)に対応
 - [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2)
   - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
-
 - [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
   - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
   - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
   - CLI引数の追加とコアモジュールの修正
   - プロジェクトの構成とファイルの変更によるシンプル化
   - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
 - [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
@@ -67,14 +70,15 @@
   - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
 - 【2024/03/29】 初期リリース
 
+
 ## 主な機能
 
 ### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
 
 - GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
 - 課題を効率的に特定し、迅速に解決策を見つけられます
 
@@ -132,15 +136,15 @@
 
 ```bash 
 sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
 上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+>[!Note] GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
 
 以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 ### 除外ファイルの指定
 
 作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
 
@@ -190,21 +194,33 @@
 
 `SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
 
 このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
 
+絵文字を活用した視覚的に分かりやすいコミットメッセージの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+
+このファイルでは、コミットメッセージのフォーマットに絵文字を取り入れ、変更内容をより直感的に表現しています。
+
+また、Gaiah用のコミットメッセージ生成を支援するテンプレートの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+
+このテンプレートでは、効果的で意味のあるコミットメッセージを作成するためのベストプラクティスに従ったガイドラインを提供しています。主要な変更とその目的に焦点を当て、コミットで行われた変更を明確かつ簡潔に説明するように促します。
+
 Issueとマージされたファイルの例はこちらです。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 
 このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
 
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。絵文字の活用やGaiahのテンプレートを利用することで、よりわかりやすく効果的なコミットメッセージの作成が可能になります。
 
 ## 3. DocuMind：リリース後のドキュメント化
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
 </p>
```

#### html2text {}

```diff
@@ -20,17 +20,21 @@
                                WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
-(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
-30ã SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/
-tag/vv4.1.2) - GitHub
+(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ ## æ´æ°åå®¹
+- [ã2024/05/12ã SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/v4.2.0) -
+ã¹ãã¼ã¸ã³ã°æå ±ã®ãã³ãã¬ã¼ãã«çµµæå­ã¨[GAIAH](https://
+github.com/Sunwood-ai-labs/Gaiah)ã«å¯¾å¿ - [ã2024/04/30ã SourceSage
+4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2) -
+GitHub
 Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
 - [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
 SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
@@ -106,15 +110,15 @@
 ãããã®ãã¡ã¤ã«ãä½¿ã£ã¦ãAIã«ãããã­ã¸ã§ã¯ãã®è§£æãèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãªã©ãè¡ããã¨ãã§ãã¾ãã
 ### ãªãã¸ããªã®Issueãåå¾ããæ¹æ³
 ããã©ã«ãã§ã¯ãSourceSageã¯ç¾å¨ã®ãã£ã¬ã¯ããªããã­ã¸ã§ã¯ãã®ã«ã¼ãã¨ãã¦è§£æãã¾ãããã ããGitHubä¸ã®ãªãã¸ããªã®Issueãåå¾ãããå ´åã¯ãä»¥ä¸ã®ããã«ãªãã¸ããªã®ãªã¼ãã¼åã¨ãªãã¸ããªåãã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
 ```bash sourcesage --owner Sunwood-ai-labs --repository SourceSage ```
 ä¸è¨ã®ä¾ã§ã¯ã`Sunwood-ai-
 labs`ããªãã¸ããªã®ãªã¼ãã¼åã`SourceSage`ããªãã¸ããªåã§ãããããã®å¼æ°ãæå®ãããã¨ã§ãSourceSageã¯GitHub
 APIãä½¿ã£ã¦ãªãã¸ããªã®ãªã¼ãã³ãªIssueãåå¾ãã`open_issues_filtered.json`ãã¡ã¤ã«ã«ä¿å­ãã¾ãã
-Note: GitHub
+>[!Note] GitHub
 APIãä½¿ç¨ããã«ã¯ãã¤ã³ã¿ã¼ãããæ¥ç¶ãå¿è¦ã§ããã¾ãããªãã¸ããªããã©ã¤ãã¼ãã®å ´åã¯ãé©åãªã¢ã¯ã»ã¹ãã¼ã¯ã³ãè¨­å®ããå¿è¦ãããã¾ãã
 ä»¥ä¸ããSourceSageã®åºæ¬çãªä½¿ç¨æ¹æ³ã§ãããã²èªåã®ãã­ã¸ã§ã¯ãã§SourceSageãæ´»ç¨ãã¦ãéçºå¹çã®åä¸ãä½é¨ãã¦ã¿ã¦ãã ããï¼
 ### é¤å¤ãã¡ã¤ã«ã®æå®
 ä½æ¥­ãã£ã¬ã¯ããªã«`.SourceSageignore`ãã¡ã¤ã«ãä½æãããã¨ã§ãä»»æã®ãã¡ã¤ã«ããã£ã¬ã¯ããªãå¦çããé¤å¤ã§ãã¾ãããã®ãã¡ã¤ã«ã«ã¯ãé¤å¤ããããã¡ã¤ã«ããã£ã¬ã¯ããªã®ãã¿ã¼ã³ã1è¡ãã¤è¨è¿°ãã¾ããä¾ãã°ãä»¥ä¸ã®ããã«æå®ãã¾ãï¼
 ```plaintext # .SourceSageignoreã®ä¾ node_modules/ *.log *.tmp ```
 ä¸è¨ã®ä¾ã§ã¯ã`node_modules`ãã£ã¬ã¯ããªã¨ãæ¡å¼µå­ã`.log`ã¾ãã¯`.tmp`ã®ãã¡ã¤ã«ãé¤å¤ããã¾ãã
 `.SourceSageignore`ãã¡ã¤ã«ãä½¿ç¨ããå ´åã¯ãä»¥ä¸ã®ããã«ã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
@@ -141,20 +145,30 @@
 CommitCraftã¯ãéçºä¸­ã®ã¹ãã¼ã¸ãããå¤æ´ãè¿½è·¡ããAIãæ´»ç¨ãã¦é©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçæãããã¼ã«ã§ããããã«ãããéçºèã¯ã³ãããã®åå®¹ãæ­£ç¢ºã«è¨è¿°ãããã¨ãã§ãããã­ã¸ã§ã¯ãã®å¤æ´å±¥æ­´ãããæç¢ºã«ç®¡çã§ãã¾ãã
 `SourceSageAssets/COMMIT_CRAFT/
 STAGED_DIFF.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/
 Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_PROMT.md)
 ãã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ããã®ã¾ã¾AIã«å¥åãããã¨ã§ãAIãã³ãããã¡ãã»ã¼ã¸ãçæãã¾ããAIã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åãåæãããã®åå®¹ãè¦ç´ããã³ãããã¡ãã»ã¼ã¸ãææ¡ãã¾ãã
+çµµæå­ãæ´»ç¨ããè¦è¦çã«åãããããã³ãããã¡ãã»ã¼ã¸ã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+ãã®ãã¡ã¤ã«ã§ã¯ãã³ãããã¡ãã»ã¼ã¸ã®ãã©ã¼ãããã«çµµæå­ãåãå¥ããå¤æ´åå®¹ãããç´æçã«è¡¨ç¾ãã¦ãã¾ãã
+ã¾ããGaiahç¨ã®ã³ãããã¡ãã»ã¼ã¸çæãæ¯æ´ãããã³ãã¬ã¼ãã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+ãã®ãã³ãã¬ã¼ãã§ã¯ãå¹æçã§æå³ã®ããã³ãããã¡ãã»ã¼ã¸ãä½æããããã®ãã¹ããã©ã¯ãã£ã¹ã«å¾ã£ãã¬ã¤ãã©ã¤ã³ãæä¾ãã¦ãã¾ããä¸»è¦ãªå¤æ´ã¨ãã®ç®çã«ç¦ç¹ãå½ã¦ãã³ãããã§è¡ãããå¤æ´ãæç¢ºãã¤ç°¡æ½ã«èª¬æããããã«ä¿ãã¾ãã
 Issueã¨ãã¼ã¸ããããã¡ã¤ã«ã®ä¾ã¯ãã¡ãã§ãã ä¾ï¼[`docs/
 SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-
 ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 ãã®ãã¡ã¤ã«ã«ã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åã¨ãªã¼ãã³ãªIssueã®æå ±ãå«ã¾ãã¦ãã¾ããAIã¯ãããã®æå ±ãçµã¿åããã¦åæããããåæ¬çãªã³ãããã¡ãã»ã¼ã¸ãçæãã¾ãã
-CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ãã
+CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ããçµµæå­ã®æ´»ç¨ãGaiahã®ãã³ãã¬ã¼ããå©ç¨ãããã¨ã§ãããããããããå¹æçãªã³ãããã¡ãã»ã¼ã¸ã®ä½æãå¯è½ã«ãªãã¾ãã
 ## 3. DocuMindï¼ãªãªã¼ã¹å¾ã®ãã­ã¥ã¡ã³ãå
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                                 head_icon7.png]
 DocuMindã¯ããªãªã¼ã¹å¾ã®ãã­ã¸ã§ã¯ãã®çµ±åã¨ãã­ã¥ã¡ã³ãåãæ¯æ´ãããã¼ã«ã§ããSourceSageãçæãããã­ã¸ã§ã¯ãã®æ¦è¦ã¨ãèªåçæãããGitã®å¤æ´å±¥æ­´ãçµã¿åããããã¨ã§ããã­ã¸ã§ã¯ãã®å¨ä½åãæç¢ºã«ææ¡ã§ãã¾ããããã«ãããéçºèã¯ãã­ã¸ã§ã¯ãã®ãã­ã¥ã¡ã³ããå¹ççã«ä½æããã¡ã³ããã³ã¹æ§ãåä¸ããããã¨ãã§ãã¾ãã
 `SourceSageAssets/
 DocuMind.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.6/setup.py` & `sourcesage-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    required = f.read().splitlines()
 
 setup(
     # パッケージの名前
     name='sourcesage',
     
     # パッケージのバージョン
-    version='4.1.6',
+    version='4.2.0',
     
     # パッケージに含めるモジュールを自動的に探す
     packages=find_packages(),
     
     # パッケージの分類情報
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `sourcesage-4.1.6/sourcesage/cli.py` & `sourcesage-4.2.0/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md` & `sourcesage-4.2.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md` & `sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md` & `sourcesage-4.2.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/config/constants.py` & `sourcesage-4.2.0/sourcesage/config/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,8 +31,11 @@
 
         self.TEMPLATE_STAGE_INFO_DIR = os.path.join(self.DOCS_DIR, "STAGE_INFO")
         self.STAGE_INFO_OUTPUT_MD = "STAGE_INFO_AND_ISSUES_AND_PROMT.md"
         self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
 
         self.STAGE_INFO_SIMPLE_OUTPUT_MD = "STAGE_INFO_AND_PROMT.md"
         self.STAGE_INFO_SIMPLE_TEMPLATE_MD = "STAGE_INFO_TEMPLATE.md"
-        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI = "STAGE_INFO_TEMPLATE_EMOJI.md"
+        self.STAGE_INFO_SIMPLE_OUTPUT_MD_EMOJI = "STAGE_INFO_AND_PROMT_EMOJI.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI = "STAGE_INFO_TEMPLATE_EMOJI.md"
+        self.STAGE_INFO_SIMPLE_OUTPUT_MD_GAIAH = "STAGE_INFO_AND_PROMT_GAIAH.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_GAIAH = "STAGE_INFO_TEMPLATE_GAIAH.md"
```

### Comparing `sourcesage-4.1.6/sourcesage/config/language_map.json` & `sourcesage-4.2.0/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/core.py` & `sourcesage-4.2.0/sourcesage/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                                                   stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
                                                   template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD),
                                                   output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
         stage_info_generator.run()
         stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                                   stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
                                                   template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI),
-                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
+                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD_EMOJI))
         stage_info_generator.run()
 
         # Convert issues to markdown
         issues_to_markdown = IssuesToMarkdown(issues_file=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                               sourcesage_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
                                               template_file=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_ISSUES_RESOLVE_DIR, self.constants.ISSUES_RESOLVE_TEMPLATE_MD),
                                               output_folder=self.constants.ISSUES_RESOLVE_DIR)
```

### Comparing `sourcesage-4.1.6/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.2.0/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.2.0/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.2.0/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.2.0/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.2.0/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.2.0/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.2.0/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.2.0/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.2.0/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/file_utils.py` & `sourcesage-4.2.0/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/markdown_utils.py` & `sourcesage-4.2.0/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage/modules/source_sage.py` & `sourcesage-4.2.0/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.6/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.2.0/sourcesage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.1.6
+Version: 4.2.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
@@ -53,17 +53,20 @@
 
 >[!IMPORTANT]
 >このリポジトリ自体も[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage)を活用しており、リリースノートやREADME、コミットメッセージの9割は[SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ＋ [claude.ai](https://claude.ai/)で生成しています。
 
 
 ## 更新内容
 
+## 更新内容
+
+- [【2024/05/12】 SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.2.0)
+  - ステージング情報のテンプレートに絵文字と[GAIAH](https://github.com/Sunwood-ai-labs/Gaiah)に対応
 - [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2)
   - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
-
 - [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
   - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
   - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
   - CLI引数の追加とコアモジュールの修正
   - プロジェクトの構成とファイルの変更によるシンプル化
   - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
 - [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
@@ -81,14 +84,15 @@
   - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
 - [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
   - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
   - 言語ごとのシンタックスハイライト機能を追加
   - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
 - 【2024/03/29】 初期リリース
 
+
 ## 主な機能
 
 ### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
 
 - GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
 - 課題を効率的に特定し、迅速に解決策を見つけられます
 
@@ -146,15 +150,15 @@
 
 ```bash 
 sourcesage --owner Sunwood-ai-labs --repository SourceSage
 ```
 
 上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
 
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+>[!Note] GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
 
 以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
 
 ### 除外ファイルの指定
 
 作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
 
@@ -204,21 +208,33 @@
 
 `SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
 
 このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
 
+絵文字を活用した視覚的に分かりやすいコミットメッセージの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+
+このファイルでは、コミットメッセージのフォーマットに絵文字を取り入れ、変更内容をより直感的に表現しています。
+
+また、Gaiah用のコミットメッセージ生成を支援するテンプレートの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+
+このテンプレートでは、効果的で意味のあるコミットメッセージを作成するためのベストプラクティスに従ったガイドラインを提供しています。主要な変更とその目的に焦点を当て、コミットで行われた変更を明確かつ簡潔に説明するように促します。
+
 Issueとマージされたファイルの例はこちらです。
 
 例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 
 このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
 
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。絵文字の活用やGaiahのテンプレートを利用することで、よりわかりやすく効果的なコミットメッセージの作成が可能になります。
 
 ## 3. DocuMind：リリース後のドキュメント化
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.6 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.2.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
@@ -25,17 +25,21 @@
                                WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
-(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
-30ã SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/
-tag/vv4.1.2) - GitHub
+(https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ ## æ´æ°åå®¹
+- [ã2024/05/12ã SourceSage 4.2.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/v4.2.0) -
+ã¹ãã¼ã¸ã³ã°æå ±ã®ãã³ãã¬ã¼ãã«çµµæå­ã¨[GAIAH](https://
+github.com/Sunwood-ai-labs/Gaiah)ã«å¯¾å¿ - [ã2024/04/30ã SourceSage
+4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/vv4.1.2) -
+GitHub
 Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
 - [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
 SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
@@ -111,15 +115,15 @@
 ãããã®ãã¡ã¤ã«ãä½¿ã£ã¦ãAIã«ãããã­ã¸ã§ã¯ãã®è§£æãèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãªã©ãè¡ããã¨ãã§ãã¾ãã
 ### ãªãã¸ããªã®Issueãåå¾ããæ¹æ³
 ããã©ã«ãã§ã¯ãSourceSageã¯ç¾å¨ã®ãã£ã¬ã¯ããªããã­ã¸ã§ã¯ãã®ã«ã¼ãã¨ãã¦è§£æãã¾ãããã ããGitHubä¸ã®ãªãã¸ããªã®Issueãåå¾ãããå ´åã¯ãä»¥ä¸ã®ããã«ãªãã¸ããªã®ãªã¼ãã¼åã¨ãªãã¸ããªåãã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
 ```bash sourcesage --owner Sunwood-ai-labs --repository SourceSage ```
 ä¸è¨ã®ä¾ã§ã¯ã`Sunwood-ai-
 labs`ããªãã¸ããªã®ãªã¼ãã¼åã`SourceSage`ããªãã¸ããªåã§ãããããã®å¼æ°ãæå®ãããã¨ã§ãSourceSageã¯GitHub
 APIãä½¿ã£ã¦ãªãã¸ããªã®ãªã¼ãã³ãªIssueãåå¾ãã`open_issues_filtered.json`ãã¡ã¤ã«ã«ä¿å­ãã¾ãã
-Note: GitHub
+>[!Note] GitHub
 APIãä½¿ç¨ããã«ã¯ãã¤ã³ã¿ã¼ãããæ¥ç¶ãå¿è¦ã§ããã¾ãããªãã¸ããªããã©ã¤ãã¼ãã®å ´åã¯ãé©åãªã¢ã¯ã»ã¹ãã¼ã¯ã³ãè¨­å®ããå¿è¦ãããã¾ãã
 ä»¥ä¸ããSourceSageã®åºæ¬çãªä½¿ç¨æ¹æ³ã§ãããã²èªåã®ãã­ã¸ã§ã¯ãã§SourceSageãæ´»ç¨ãã¦ãéçºå¹çã®åä¸ãä½é¨ãã¦ã¿ã¦ãã ããï¼
 ### é¤å¤ãã¡ã¤ã«ã®æå®
 ä½æ¥­ãã£ã¬ã¯ããªã«`.SourceSageignore`ãã¡ã¤ã«ãä½æãããã¨ã§ãä»»æã®ãã¡ã¤ã«ããã£ã¬ã¯ããªãå¦çããé¤å¤ã§ãã¾ãããã®ãã¡ã¤ã«ã«ã¯ãé¤å¤ããããã¡ã¤ã«ããã£ã¬ã¯ããªã®ãã¿ã¼ã³ã1è¡ãã¤è¨è¿°ãã¾ããä¾ãã°ãä»¥ä¸ã®ããã«æå®ãã¾ãï¼
 ```plaintext # .SourceSageignoreã®ä¾ node_modules/ *.log *.tmp ```
 ä¸è¨ã®ä¾ã§ã¯ã`node_modules`ãã£ã¬ã¯ããªã¨ãæ¡å¼µå­ã`.log`ã¾ãã¯`.tmp`ã®ãã¡ã¤ã«ãé¤å¤ããã¾ãã
 `.SourceSageignore`ãã¡ã¤ã«ãä½¿ç¨ããå ´åã¯ãä»¥ä¸ã®ããã«ã³ãã³ãã©ã¤ã³å¼æ°ã§æå®ãã¾ãï¼
@@ -146,20 +150,30 @@
 CommitCraftã¯ãéçºä¸­ã®ã¹ãã¼ã¸ãããå¤æ´ãè¿½è·¡ããAIãæ´»ç¨ãã¦é©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçæãããã¼ã«ã§ããããã«ãããéçºèã¯ã³ãããã®åå®¹ãæ­£ç¢ºã«è¨è¿°ãããã¨ãã§ãããã­ã¸ã§ã¯ãã®å¤æ´å±¥æ­´ãããæç¢ºã«ç®¡çã§ãã¾ãã
 `SourceSageAssets/COMMIT_CRAFT/
 STAGED_DIFF.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/
 Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_PROMT.md)
 ãã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ããã®ã¾ã¾AIã«å¥åãããã¨ã§ãAIãã³ãããã¡ãã»ã¼ã¸ãçæãã¾ããAIã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åãåæãããã®åå®¹ãè¦ç´ããã³ãããã¡ãã»ã¼ã¸ãææ¡ãã¾ãã
+çµµæå­ãæ´»ç¨ããè¦è¦çã«åãããããã³ãããã¡ãã»ã¼ã¸ã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_EMOJI.md)
+ãã®ãã¡ã¤ã«ã§ã¯ãã³ãããã¡ãã»ã¼ã¸ã®ãã©ã¼ãããã«çµµæå­ãåãå¥ããå¤æ´åå®¹ãããç´æçã«è¡¨ç¾ãã¦ãã¾ãã
+ã¾ããGaiahç¨ã®ã³ãããã¡ãã»ã¼ã¸çæãæ¯æ´ãããã³ãã¬ã¼ãã®ä¾ã¯ãã¡ãã§ãã
+ä¾ï¼[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md`](https://github.com/
+Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/
+SAMPLE_STAGE_INFO_AND_PROMT_GAIAH.md)
+ãã®ãã³ãã¬ã¼ãã§ã¯ãå¹æçã§æå³ã®ããã³ãããã¡ãã»ã¼ã¸ãä½æããããã®ãã¹ããã©ã¯ãã£ã¹ã«å¾ã£ãã¬ã¤ãã©ã¤ã³ãæä¾ãã¦ãã¾ããä¸»è¦ãªå¤æ´ã¨ãã®ç®çã«ç¦ç¹ãå½ã¦ãã³ãããã§è¡ãããå¤æ´ãæç¢ºãã¤ç°¡æ½ã«èª¬æããããã«ä¿ãã¾ãã
 Issueã¨ãã¼ã¸ããããã¡ã¤ã«ã®ä¾ã¯ãã¡ãã§ãã ä¾ï¼[`docs/
 SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-
 ai-labs/SourceSage/blob/main/docs/SAMPLE/
 SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
 ãã®ãã¡ã¤ã«ã«ã¯ãã¹ãã¼ã¸ãããå¤æ´ã®å·®åã¨ãªã¼ãã³ãªIssueã®æå ±ãå«ã¾ãã¦ãã¾ããAIã¯ãããã®æå ±ãçµã¿åããã¦åæããããåæ¬çãªã³ãããã¡ãã»ã¼ã¸ãçæãã¾ãã
-CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ãã
+CommitCraftãä½¿ç¨ãããã¨ã§ãéçºèã¯ã³ãããã¡ãã»ã¼ã¸ãèããè² æãè»½æ¸ããä¸è²«æ§ã®ããé©åãªã³ãããã¡ãã»ã¼ã¸ãèªåçã«çæã§ãã¾ããçµµæå­ã®æ´»ç¨ãGaiahã®ãã³ãã¬ã¼ããå©ç¨ãããã¨ã§ãããããããããå¹æçãªã³ãããã¡ãã»ã¼ã¸ã®ä½æãå¯è½ã«ãªãã¾ãã
 ## 3. DocuMindï¼ãªãªã¼ã¹å¾ã®ãã­ã¥ã¡ã³ãå
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                                 head_icon7.png]
 DocuMindã¯ããªãªã¼ã¹å¾ã®ãã­ã¸ã§ã¯ãã®çµ±åã¨ãã­ã¥ã¡ã³ãåãæ¯æ´ãããã¼ã«ã§ããSourceSageãçæãããã­ã¸ã§ã¯ãã®æ¦è¦ã¨ãèªåçæãããGitã®å¤æ´å±¥æ­´ãçµã¿åããããã¨ã§ããã­ã¸ã§ã¯ãã®å¨ä½åãæç¢ºã«ææ¡ã§ãã¾ããããã«ãããéçºèã¯ãã­ã¸ã§ã¯ãã®ãã­ã¥ã¡ã³ããå¹ççã«ä½æããã¡ã³ããã³ã¹æ§ãåä¸ããããã¨ãã§ãã¾ãã
 `SourceSageAssets/
 DocuMind.md`ã«çæããããã¼ã¯ãã¦ã³ãã¡ã¤ã«ãä½¿ç¨ãã¾ãã
 ä¾ï¼[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.6/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.2.0/sourcesage.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 sourcesage/config/.SourceSageignore
 sourcesage/config/constants.py
 sourcesage/config/language_map.json
 sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
+sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
```

### Comparing `sourcesage-4.1.6/tests/test_sourcesage.py` & `sourcesage-4.2.0/tests/test_sourcesage.py`

 * *Files identical despite different names*

