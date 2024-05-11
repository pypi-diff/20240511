# Comparing `tmp/ai_commit_cli-0.7.0.tar.gz` & `tmp/ai_commit_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_commit_cli-0.7.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ai_commit_cli-0.7.0.tar` & `ai_commit_cli-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,37 @@
--rw-r--r--   0        0        0     1063 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/LICENSE
--rw-r--r--   0        0        0     4584 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/README.md
--rw-r--r--   0        0        0       78 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/__init__.py
--rw-r--r--   0        0        0       41 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/__main__.py
--rw-r--r--   0        0        0     5623 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/app.py
--rw-r--r--   0        0        0        0 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/cmd/__init__.py
--rw-r--r--   0        0        0      779 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/cmd/bw.py
--rw-r--r--   0        0        0     2536 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/cmd/git.py
--rw-r--r--   0        0        0      653 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/cmd/pre_commit.py
--rw-r--r--   0        0        0      752 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/diff.py
--rw-r--r--   0        0        0     5392 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/gpt.py
--rw-r--r--   0        0        0     1556 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/log.py
--rw-r--r--   0        0        0     1266 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/msg.py
--rw-r--r--   0        0        0     5362 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/prompt.py
--rw-r--r--   0        0        0     6477 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/ai_commit_cli/spec.py
--rw-r--r--   0        0        0      734 2024-02-04 10:08:07.616391 ai_commit_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5311 1970-01-01 00:00:00.000000 ai_commit_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.cspell.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.envrc
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.python-version
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/Makefile
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/requirements.lock
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/ruff.toml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/auto-label.yaml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/blunderbuss.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/renovate.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/sync-repo-settings.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/release-please/.manifest.json
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/release-please/config.json
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/__main__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/commit_lint.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/config.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/git.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/log.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/pretty.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/api/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/api/openrouter.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/cli/__init__.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/cli/list_models.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/cli/main.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/prompt/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/prompt/_type.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/src/aic/prompt/template.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/.gitignore
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ai_commit_cli-0.8.0/PKG-INFO
```

### Comparing `ai_commit_cli-0.7.0/ai_commit_cli/msg.py` & `ai_commit_cli-0.8.0/src/aic/commit_lint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import re
-from collections.abc import Sequence
-from typing import Optional
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from collections.abc import Sequence
 
 PATTERN: re.Pattern[str] = re.compile(
     r"(?P<type>\w+)(?:\((?P<scope>[^\)]+)\))?(?P<breaking>!)?: (?P<description>.+)"
 )
 
 
-def check(msg: str) -> bool:
-    title_line: str = msg.splitlines()[0]
-    return title_line == sanitize_line(title_line)
-
-
 def sanitize(msg: str) -> str:
-    msg = re.sub(r"^```.*$", "", msg, flags=re.MULTILINE)
-    msg = re.sub(r"\n\n\n+", "\n\n", msg)
+    msg = msg.strip()
+    msg = msg.removeprefix("<Answer>").removesuffix("</Answer>")
     msg = msg.strip()
     lines: Sequence[str] = [sanitize_line(line) for line in msg.splitlines()]
     return "\n".join(lines)
 
 
 def sanitize_line(line: str) -> str:
-    matches: Optional[re.Match[str]] = PATTERN.fullmatch(line)
+    matches: re.Match[str] | None = PATTERN.fullmatch(line)
     if matches is None:
         return line
     type_: str = matches.group("type")
-    scope: Optional[str] = matches.group("scope")
-    breaking: Optional[str] = matches.group("breaking")
+    scope: str | None = matches.group("scope")
+    breaking: str | None = matches.group("breaking")
     description: str = matches.group("description")
     type_ = type_.strip().lower()
     line = type_
     if scope is not None:
         scope = scope.strip().lower()
         line += f"({scope})"
     if breaking is not None:
```

### Comparing `ai_commit_cli-0.7.0/ai_commit_cli/spec.py` & `ai_commit_cli-0.8.0/src/aic/prompt/template.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,79 @@
 # ruff: noqa: E501
+from aic.prompt import _type
 
-SPEC: str = """\
-# Conventional Commits 1.0.0
 
-## Summary
+def format_types() -> str:
+    result: str = ""
+    for t in _type.CommitType:
+        result += f"- `{t.value}`: {t.description}\n"
+    return result.strip()
 
-The Conventional Commits specification is a lightweight convention on top of commit messages.
-It provides an easy set of rules for creating an explicit commit history;
-which makes it easier to write automated tools on top of.
-This convention dovetails with [SemVer](http://semver.org),
-by describing the features, fixes, and breaking changes made in commit messages.
+
+# https://docs.anthropic.com/claude/docs/helper-metaprompt-experimental
+# https://github.com/gitkraken/vscode-gitlens/blob/27e0658e277b060e06ae5d250f0afdf9a5d6e4b5/src/ai/openaiProvider.ts#L59-L67
+TEMPLATE: str = f"""\
+You are an advanced AI programming assistant tasked with summarizing code changes into a concise and meaningful commit message. Compose a commit message that:
+
+- Strictly synthesizes meaningful information from the provided code diff
+- Utilizes any additional user-provided context to comprehend the rationale behind the code changes
+- Is clear and brief, with an informal yet professional tone, and without superfluous descriptions
+- Avoids unnecessary phrases such as "this commit", "this change", and the like
+- Avoids direct mention of specific code identifiers, names, or file names, unless they are crucial for understanding the purpose of the changes
+- Most importantly emphasizes the 'why' of the change, its benefits, or the problem it addresses rather than only the 'what' that changed
+
+Follow the user's instructions carefully, don't repeat yourself, don't include the code in the output, or make anything up!
+
+## Read the Inputs
+
+Begin by examining the inputs provided:
+
+<ConventionalCommitsSpecification>
+
+The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).
+
+1. Commits MUST be prefixed with a type, which consists of a noun, `feat`, `fix`, etc., followed by the OPTIONAL scope, OPTIONAL `!`, and REQUIRED terminal colon and space.
+2. The type `feat` MUST be used when a commit adds a new feature to your application or library.
+3. The type `fix` MUST be used when a commit represents a bug fix for your application.
+4. A scope MAY be provided after a type. A scope MUST consist of a noun describing a section of the codebase surrounded by parenthesis, e.g., `fix(parser):`
+5. A description MUST immediately follow the colon and space after the type/scope prefix. The description is a short summary of the code changes, e.g., _fix: array parsing issue when multiple spaces were contained in string_.
+6. A longer commit body MAY be provided after the short description, providing additional contextual information about the code changes. The body MUST begin one blank line after the description.
+7. A commit body is free-form and MAY consist of any number of newline separated paragraphs.
+8. One or more footers MAY be provided one blank line after the body. Each footer MUST consist of a word token, followed by either a `:<space>` or `<space>#` separator, followed by a string value (this is inspired by the [git trailer convention](https://git-scm.com/docs/git-interpret-trailers)).
+9. A footer's token MUST use `-` in place of whitespace characters, e.g., `Acked-by` (this helps differentiate the footer section from a multi-paragraph body). An exception is made for `BREAKING CHANGE`, which MAY also be used as a token.
+10. A footer's value MAY contain spaces and newlines, and parsing MUST terminate when the next valid footer token/separator pair is observed.
+11. Breaking changes MUST be indicated in the type/scope prefix of a commit, or as an entry in the footer.
+12. If included as a footer, a breaking change MUST consist of the uppercase text BREAKING CHANGE, followed by a colon, space, and description, e.g., _BREAKING CHANGE: environment variables now take precedence over config files_.
+13. If included in the type/scope prefix, breaking changes MUST be indicated by a `!` immediately before the `:`. If `!` is used, `BREAKING CHANGE:` MAY be omitted from the footer section, and the commit description SHALL be used to describe the breaking change.
+14. Types other than `feat` and `fix` MAY be used in your commit messages, e.g., _docs: update ref docs._
+15. The units of information that make up Conventional Commits MUST NOT be treated as case sensitive by implementors, with the exception of BREAKING CHANGE which MUST be uppercase.
+16. BREAKING-CHANGE MUST be synonymous with BREAKING CHANGE, when used as a token in a footer.
+</ConventionalCommitsSpecification>
+
+<GitDiff>
+$GIT_DIFF</GitDiff>
+<Type>$TYPE</Type>
+<Scope>$SCOPE</SCOPE> (optional)
+<BreakingChange>$BREAKING_CHANGE</BreakingChange> (optional)
+
+## Determine Commit Type
+
+The commit type (<Type>) is mandatory. If it is provided (i.e. not `None`), use it. Otherwise, when <Type> is `None`, you must infer it from <GitDiff>. Common types include:
+
+{format_types()}
+
+## Determine Scope of the Commit
+
+The scope of commit (<Scope>) is optional. If <Scope> is provided, use it. If <Scope> is empty, omit it. If <Scope> is `None`, infer the scope from the <GitDiff> by identifying the primary area of the codebase affected. If the diff does not provide a clear scope, you can omit it.
+
+## Determine Breaking Changes
+
+Breaking Changes (<BreakingChange>) are optional. If <BreakingChange> is provided, use it. If <BreakingChange> is empty, omit it. If <BreakingChange> is `None`, check <GitDiff> for significant changes that could break existing functionality. If there is no breaking change, you can omit this section.
+
+## Construct the Commit Message
 
 The commit message should be structured as follows:
 
 ```
 <type>[optional scope]: <description>
 
 [optional body]
@@ -22,107 +82,79 @@
 ```
 
 The commit contains the following structural elements, to communicate intent to the
 consumers of your library:
 
 1. **fix:** a commit of the _type_ `fix` patches a bug in your codebase (this correlates with [`PATCH`](http://semver.org/#summary) in Semantic Versioning).
 2. **feat:** a commit of the _type_ `feat` introduces a new feature to the codebase (this correlates with [`MINOR`](http://semver.org/#summary) in Semantic Versioning).
-3. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:`, or appends a `!` after the type/scope, introduces a breaking API change (correlating with [`MAJOR`](http://semver.org/#summary) in Semantic Versioning).
-   A BREAKING CHANGE can be part of commits of any _type_.
-4. _types_ other than `fix:` and `feat:` are allowed, for example [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/%40commitlint/config-conventional) (based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)) recommends `build:`, `chore:`,
-   `ci:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others.
-5. _footers_ other than `BREAKING CHANGE: <description>` may be provided and follow a convention similar to
-   [git trailer format](https://git-scm.com/docs/git-interpret-trailers).
+3. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:`, or appends a `!` after the type/scope, introduces a breaking API change (correlating with [`MAJOR`](http://semver.org/#summary) in Semantic Versioning). A BREAKING CHANGE can be part of commits of any _type_.
+4. _types_ other than `fix:` and `feat:` are allowed, for example [@commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/%40commitlint/config-conventional) (based on the [Angular convention](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines)) recommends `build:`, `chore:`, `ci:`, `docs:`, `style:`, `refactor:`, `perf:`, `test:`, and others.
+5. _footers_ other than `BREAKING CHANGE: <description>` may be provided and follow a convention similar to [git trailer format](https://git-scm.com/docs/git-interpret-trailers).
 
 Additional types are not mandated by the Conventional Commits specification, and have no implicit effect in Semantic Versioning (unless they include a BREAKING CHANGE).
 
 A scope may be provided to a commit's type, to provide additional contextual information and is contained within parenthesis, e.g., `feat(parser): add ability to parse arrays`.
 
-## Examples
-
-### Commit message with description and breaking change footer
-
-```
-feat: allow provided config object to extend other configs
-
-BREAKING CHANGE: `extends` key in config file is now used for extending other config files
-```
+## Example Commit Messages
 
 ### Commit message with `!` to draw attention to breaking change
 
-```
+<Example>
+<Answer>
 feat!: send an email to the customer when a product is shipped
-```
+</Answer>
+</Example>
 
 ### Commit message with scope and `!` to draw attention to breaking change
 
-```
+<Example>
+<Answer>
 feat(api)!: send an email to the customer when a product is shipped
-```
+</Answer>
+</Example>
 
 ### Commit message with both `!` and BREAKING CHANGE footer
 
-```
+<Example>
+<Answer>
 chore!: drop support for Node 6
 
 BREAKING CHANGE: use JavaScript features not available in Node 6.
-```
+</Answer>
+</Example>
 
 ### Commit message with no body
 
-```
+<Example>
+<Answer>
 docs: correct spelling of CHANGELOG
-```
+</Answer>
+</Example>
 
 ### Commit message with scope
 
-```
+<Example>
+<Answer>
 feat(lang): add Polish language
-```
+</Answer>
+</Example>
 
-### Commit message with multi-paragraph body and multiple footers
+### Commit message with multi-paragraph body
 
-```
+<Example>
+<Answer>
 fix: prevent racing of requests
 
 Introduce a request id and a reference to latest request. Dismiss
 incoming responses other than from latest request.
 
 Remove timeouts which were used to mitigate the racing issue but are
 obsolete now.
+</Answer>
+</Example>
 
-Reviewed-by: Z
-Refs: #123
-```
-
-## Specification
+## Final Output
 
-The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).
+Write your final commit message inside <Answer> tags. Ensure it is clear, concise, and follows the conventional commit specification.
 
-1. Commits MUST be prefixed with a type, which consists of a noun, `feat`, `fix`, etc., followed
-   by the OPTIONAL scope, OPTIONAL `!`, and REQUIRED terminal colon and space.
-2. The type `feat` MUST be used when a commit adds a new feature to your application or library.
-3. The type `fix` MUST be used when a commit represents a bug fix for your application.
-4. A scope MAY be provided after a type. A scope MUST consist of a noun describing a
-   section of the codebase surrounded by parenthesis, e.g., `fix(parser):`
-5. A description MUST immediately follow the colon and space after the type/scope prefix.
-   The description is a short summary of the code changes, e.g., _fix: array parsing issue when multiple spaces were contained in string_.
-6. A longer commit body MAY be provided after the short description, providing additional contextual information about the code changes. The body MUST begin one blank line after the description.
-7. A commit body is free-form and MAY consist of any number of newline separated paragraphs.
-8. One or more footers MAY be provided one blank line after the body. Each footer MUST consist of
-   a word token, followed by either a `:<space>` or `<space>#` separator, followed by a string value (this is inspired by the
-   [git trailer convention](https://git-scm.com/docs/git-interpret-trailers)).
-9. A footer's token MUST use `-` in place of whitespace characters, e.g., `Acked-by` (this helps differentiate
-   the footer section from a multi-paragraph body). An exception is made for `BREAKING CHANGE`, which MAY also be used as a token.
-10. A footer's value MAY contain spaces and newlines, and parsing MUST terminate when the next valid footer
-    token/separator pair is observed.
-11. Breaking changes MUST be indicated in the type/scope prefix of a commit, or as an entry in the
-    footer.
-12. If included as a footer, a breaking change MUST consist of the uppercase text BREAKING CHANGE, followed by a colon, space, and description, e.g.,
-    _BREAKING CHANGE: environment variables now take precedence over config files_.
-13. If included in the type/scope prefix, breaking changes MUST be indicated by a
-    `!` immediately before the `:`. If `!` is used, `BREAKING CHANGE:` MAY be omitted from the footer section,
-    and the commit description SHALL be used to describe the breaking change.
-14. Types other than `feat` and `fix` MAY be used in your commit messages, e.g., _docs: update ref docs._
-15. The units of information that make up Conventional Commits MUST NOT be treated as case sensitive by implementors, with the exception of BREAKING CHANGE which MUST be uppercase.
-16. BREAKING-CHANGE MUST be synonymous with BREAKING CHANGE, when used as a token in a footer.
+By following these steps, you will create a well-structured and informative git commit message that adheres to the conventional commit standards.
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

