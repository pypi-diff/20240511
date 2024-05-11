# Comparing `tmp/git_cliff-2.2.1.tar.gz` & `tmp/git_cliff-2.2.2.tar.gz`

## Comparing `git_cliff-2.2.1.tar` & `git_cliff-2.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0     1001      127     2335 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/Cargo.toml
--rw-r--r--   0     1001      127    20321 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/changelog.rs
--rw-r--r--   0     1001      127     2068 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/command.rs
--rw-r--r--   0     1001      127    18579 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/commit.rs
--rw-r--r--   0     1001      127    10306 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/config.rs
--rw-r--r--   0     1001      127     1617 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/embed.rs
--rw-r--r--   0     1001      127     4909 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/error.rs
--rw-r--r--   0     1001      127     7528 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/github.rs
--rw-r--r--   0     1001      127     1278 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/lib.rs
--rw-r--r--   0     1001      127    18124 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/release.rs
--rw-r--r--   0     1001      127     7990 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/repo.rs
--rw-r--r--   0     1001      127     6227 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/src/template.rs
--rw-r--r--   0     1001      127     7500 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff-core/tests/integration_test.rs
--rw-r--r--   0     1001      127     5383 2024-04-10 22:29:25.000000 git_cliff-2.2.1/README.md
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 git_cliff-2.2.1/git-cliff/Cargo.toml
--rw-r--r--   0     1001      127     8460 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/args.rs
--rw-r--r--   0     1001      127      701 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/bin/completions.rs
--rw-r--r--   0     1001      127      754 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/bin/mangen.rs
--rw-r--r--   0     1001      127    13842 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/lib.rs
--rw-r--r--   0     1001      127     3408 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/logger.rs
--rw-r--r--   0     1001      127      546 2024-04-10 22:29:25.000000 git_cliff-2.2.1/git-cliff/src/main.rs
--rw-r--r--   0     1001      127    74172 2024-04-10 22:29:25.000000 git_cliff-2.2.1/Cargo.lock
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 git_cliff-2.2.1/Cargo.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 git_cliff-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 git_cliff-2.2.1/PKG-INFO
+-rw-r--r--   0     1001      127     2366 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/Cargo.toml
+-rw-r--r--   0     1001      127    22801 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/changelog.rs
+-rw-r--r--   0     1001      127     2068 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/command.rs
+-rw-r--r--   0     1001      127    18530 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/commit.rs
+-rw-r--r--   0     1001      127    10306 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/config.rs
+-rw-r--r--   0     1001      127     1617 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/embed.rs
+-rw-r--r--   0     1001      127     4909 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/error.rs
+-rw-r--r--   0     1001      127     7528 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/github.rs
+-rw-r--r--   0     1001      127     1278 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/lib.rs
+-rw-r--r--   0     1001      127    18124 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/release.rs
+-rw-r--r--   0     1001      127     7621 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/repo.rs
+-rw-r--r--   0     1001      127     6235 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/template.rs
+-rw-r--r--   0     1001      127     7500 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/tests/integration_test.rs
+-rw-r--r--   0     1001      127     5927 2024-05-11 20:02:07.000000 git_cliff-2.2.2/README.md
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 git_cliff-2.2.2/git-cliff/Cargo.toml
+-rw-r--r--   0     1001      127     8460 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/args.rs
+-rw-r--r--   0     1001      127      701 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/bin/completions.rs
+-rw-r--r--   0     1001      127      754 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/bin/mangen.rs
+-rw-r--r--   0     1001      127    13842 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/lib.rs
+-rw-r--r--   0     1001      127     3408 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/logger.rs
+-rw-r--r--   0     1001      127      546 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/main.rs
+-rw-r--r--   0     1001      127    80522 2024-05-11 20:02:07.000000 git_cliff-2.2.2/Cargo.lock
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 git_cliff-2.2.2/Cargo.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 git_cliff-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 git_cliff-2.2.2/PKG-INFO
```

### Comparing `git_cliff-2.2.1/git-cliff-core/Cargo.toml` & `git_cliff-2.2.2/git-cliff-core/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "git-cliff-core"
-version = "2.2.1" # managed by release.sh
+version = "2.2.2" # managed by release.sh
 description = "Core library of git-cliff"
 authors = ["git-cliff contributors <git-cliff@protonmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "../README.md"
 homepage = "https://github.com/orhun/git-cliff"
 repository = "https://github.com/orhun/git-cliff"
 keywords = ["changelog", "generator", "conventional", "commit"]
@@ -31,31 +31,32 @@
 [dependencies]
 glob = { workspace = true, optional = true }
 regex.workspace = true
 log.workspace = true
 secrecy.workspace = true
 dirs.workspace = true
 lazy_static.workspace = true
-thiserror = "1.0.58"
-serde = { version = "1.0.197", features = ["derive"] }
-serde_json = "1.0.115"
+thiserror = "1.0.60"
+serde = { version = "1.0.201", features = ["derive"] }
+serde_json = "1.0.117"
 serde_regex = "1.1.0"
 tera = "1.19.1"
 indexmap = { version = "2.2.6", optional = true }
 toml = "0.8.12"
 lazy-regex = "3.1.0"
-next_version = "0.2.15"
-semver = "1.0.22"
+next_version = "0.2.16"
+semver = "1.0.23"
 document-features = { version = "0.2.8", optional = true }
-reqwest = { version = "0.11.27", default-features = false, features = [
+reqwest = { version = "0.12.4", default-features = false, features = [
   "rustls-tls",
   "json",
+  "zstd",
 ], optional = true }
-http-cache-reqwest = { version = "0.13.0", optional = true }
-reqwest-middleware = { version = "0.2.5", optional = true }
+http-cache-reqwest = { version = "0.14.0", optional = true }
+reqwest-middleware = { version = "0.3.1", optional = true }
 tokio = { version = "1.37.0", features = [
   "rt-multi-thread",
   "macros",
 ], optional = true }
 futures = { version = "0.3.30", optional = true }
 url = "2.5.0"
 
@@ -70,16 +71,17 @@
 features = ["toml", "yaml"]
 
 [dependencies.git-conventional]
 version = "0.12.6"
 features = ["serde"]
 
 [dependencies.rust-embed]
-version = "8.3.0"
+version = "8.4.0"
 features = ["debug-embed", "compression"]
 
 [dev-dependencies]
 pretty_assertions = "1.4.0"
+expect-test = "1.5.0"
 
 [package.metadata.docs.rs]
 all-features = true
 rustdoc-args = ["--cfg", "docsrs"]
```

### Comparing `git_cliff-2.2.1/git-cliff-core/src/changelog.rs` & `git_cliff-2.2.2/git-cliff-core/src/changelog.rs`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 	UNIX_EPOCH,
 };
 
 /// Changelog generator.
 #[derive(Debug)]
 pub struct Changelog<'a> {
 	/// Releases that the changelog will contain.
-	pub releases:    Vec<Release<'a>>,
-	body_template:   Template,
-	footer_template: Option<Template>,
-	config:          &'a Config,
+	pub releases:       Vec<Release<'a>>,
+	body_template:      Template,
+	footer_template:    Option<Template>,
+	config:             &'a Config,
+	additional_context: HashMap<String, serde_json::Value>,
 }
 
 impl<'a> Changelog<'a> {
 	/// Constructs a new instance.
 	pub fn new(releases: Vec<Release<'a>>, config: &'a Config) -> Result<Self> {
 		let trim = config.changelog.trim.unwrap_or(true);
 		let mut changelog = Self {
@@ -50,20 +51,38 @@
 				trim,
 			)?,
 			footer_template: match &config.changelog.footer {
 				Some(footer) => Some(Template::new(footer.to_string(), trim)?),
 				None => None,
 			},
 			config,
+			additional_context: HashMap::new(),
 		};
 		changelog.process_commits();
 		changelog.process_releases();
 		Ok(changelog)
 	}
 
+	/// Adds a key value pair to the template context.
+	///
+	/// These values will be used when generating the changelog.
+	///
+	/// # Errors
+	///
+	/// This operation fails if the deserialization fails.
+	pub fn add_context(
+		&mut self,
+		key: impl Into<String>,
+		value: impl serde::Serialize,
+	) -> Result<()> {
+		self.additional_context
+			.insert(key.into(), serde_json::to_value(value)?);
+		Ok(())
+	}
+
 	/// Processes a single commit and returns/logs the result.
 	fn process_commit(
 		commit: Commit<'a>,
 		git_config: &GitConfig,
 	) -> Option<Commit<'a>> {
 		match commit.process(git_config) {
 			Ok(commit) => Some(commit),
@@ -90,18 +109,22 @@
 				.cloned()
 				.filter_map(|commit| Self::process_commit(commit, &self.config.git))
 				.flat_map(|commit| {
 					if self.config.git.split_commits.unwrap_or(false) {
 						commit
 							.message
 							.lines()
-							.flat_map(|line| {
+							.filter_map(|line| {
 								let mut c = commit.clone();
 								c.message = line.to_string();
-								Self::process_commit(c, &self.config.git)
+								if !c.message.is_empty() {
+									Self::process_commit(c, &self.config.git)
+								} else {
+									None
+								}
 							})
 							.collect()
 					} else {
 						vec![commit]
 					}
 				})
 				.collect::<Vec<Commit>>();
@@ -224,16 +247,19 @@
 		}
 		Ok(None)
 	}
 
 	/// Generates the changelog and writes it to the given output.
 	pub fn generate<W: Write>(&self, out: &mut W) -> Result<()> {
 		debug!("Generating changelog...");
-		let mut additional_context = HashMap::new();
-		additional_context.insert("remote", self.config.remote.clone());
+		let mut additional_context = self.additional_context.clone();
+		additional_context.insert(
+			"remote".to_string(),
+			serde_json::to_value(self.config.remote.clone())?,
+		);
 		#[cfg(feature = "github")]
 		let (github_commits, github_pull_requests) = self.get_github_metadata()?;
 		let postprocessors = self
 			.config
 			.changelog
 			.postprocessors
 			.clone()
@@ -718,14 +744,15 @@
 ",
 			),
 		));
 		releases[2].commits.push(Commit::new(
 			String::from("123abc"),
 			String::from(
 				"chore(deps): bump some deps
+
 chore(deps): bump some more deps
 chore(deps): fix broken deps
 ",
 			),
 		));
 		let changelog = Changelog::new(releases, &config)?;
 		let mut out = Vec::new();
@@ -809,8 +836,91 @@
 			"#
 			)
 			.replace("			", ""),
 			str::from_utf8(&out).unwrap_or_default()
 		);
 		Ok(())
 	}
+
+	#[test]
+	fn changelog_adds_additional_context() -> Result<()> {
+		let (mut config, releases) = get_test_data();
+		// add `{{ custom_field }}` to the template
+		config.changelog.body = Some(
+			r#"{% if version %}
+				## {{ custom_field }} [{{ version }}] - {{ timestamp | date(format="%Y-%m-%d") }}
+				{% if commit_id %}({{ commit_id }}){% endif %}{% else %}
+				## Unreleased{% endif %}
+				{% for group, commits in commits | group_by(attribute="group") %}
+				### {{ group }}{% for group, commits in commits | group_by(attribute="scope") %}
+				#### {{ group }}{% for commit in commits %}
+				- {{ commit.message }}{% endfor %}
+				{% endfor %}{% endfor %}"#
+				.to_string(),
+		);
+		let mut changelog = Changelog::new(releases, &config)?;
+		changelog.add_context("custom_field", "Hello")?;
+		let mut out = Vec::new();
+		changelog.generate(&mut out)?;
+		expect_test::expect![[r#"
+    # Changelog
+    ## Unreleased
+
+    ### Bug Fixes
+    #### app
+    - fix abc
+
+    ### New features
+    #### app
+    - add xyz
+
+    ### Other
+    #### app
+    - document zyx
+
+    #### ui
+    - do exciting stuff
+
+    ## Hello [v1.0.0] - 1971-08-02
+    (0bc123)
+
+    ### Bug Fixes
+    #### ui
+    - fix more stuff
+
+    ### Documentation
+    #### documentation
+    - update docs
+    - add some documentation
+
+    ### I love tea
+    #### app
+    - damn right
+
+    ### Matched (group)
+    #### group
+    - support regex-replace for groups
+
+    ### New features
+    #### app
+    - add cool features
+
+    #### other
+    - support unscoped commits
+    - support breaking commits
+
+    ### Other
+    #### app
+    - do nothing
+
+    #### other
+    - support unconventional commits
+    - this commit is preprocessed
+
+    #### ui
+    - make good stuff
+    -- total releases: 2 --
+"#]]
+		.assert_eq(str::from_utf8(&out).unwrap_or_default());
+		Ok(())
+	}
 }
```

### Comparing `git_cliff-2.2.1/git-cliff-core/src/command.rs` & `git_cliff-2.2.2/git-cliff-core/src/command.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/commit.rs` & `git_cliff-2.2.2/git-cliff-core/src/commit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -258,33 +258,31 @@
 		filter: bool,
 	) -> Result<Self> {
 		for parser in parsers {
 			let mut regex_checks = Vec::new();
 			if let Some(message_regex) = parser.message.as_ref() {
 				regex_checks.push((message_regex, self.message.to_string()))
 			}
-			if let (Some(body_regex), Some(body)) = (
-				parser.body.as_ref(),
-				self.conv.as_ref().and_then(|v| v.body()),
-			) {
-				regex_checks.push((body_regex, body.to_string()))
+			let body = self
+				.conv
+				.as_ref()
+				.and_then(|v| v.body())
+				.map(|v| v.to_string());
+			if let Some(body_regex) = parser.body.as_ref() {
+				regex_checks.push((body_regex, body.clone().unwrap_or_default()))
 			}
 			if let (Some(field_name), Some(pattern_regex)) =
 				(parser.field.as_ref(), parser.pattern.as_ref())
 			{
 				regex_checks.push((
 					pattern_regex,
 					match field_name.as_str() {
 						"id" => Some(self.id.clone()),
 						"message" => Some(self.message.clone()),
-						"body" => self
-							.conv
-							.as_ref()
-							.and_then(|v| v.body())
-							.map(|v| v.to_string()),
+						"body" => body,
 						"author.name" => self.author.name.clone(),
 						"author.email" => self.author.email.clone(),
 						"committer.name" => self.committer.name.clone(),
 						"committer.email" => self.committer.email.clone(),
 						_ => None,
 					}
 					.ok_or_else(|| {
```

### Comparing `git_cliff-2.2.1/git-cliff-core/src/config.rs` & `git_cliff-2.2.2/git-cliff-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/embed.rs` & `git_cliff-2.2.2/git-cliff-core/src/embed.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/error.rs` & `git_cliff-2.2.2/git-cliff-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/github.rs` & `git_cliff-2.2.2/git-cliff-core/src/github.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/lib.rs` & `git_cliff-2.2.2/git-cliff-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/release.rs` & `git_cliff-2.2.2/git-cliff-core/src/release.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff-core/src/repo.rs` & `git_cliff-2.2.2/git-cliff-core/src/repo.rs`

 * *Files 6% similar despite different names*

```diff
@@ -206,15 +206,14 @@
 	}
 }
 
 #[cfg(test)]
 mod test {
 	use super::*;
 	use crate::commit::Commit as AppCommit;
-	use git_conventional::ErrorKind;
 	use std::env;
 	use std::process::Command;
 	use std::str;
 
 	fn get_last_commit_hash() -> Result<String> {
 		Ok(str::from_utf8(
 			Command::new("git")
@@ -235,50 +234,44 @@
 				.stdout
 				.as_ref(),
 		)?
 		.trim()
 		.to_string())
 	}
 
-	#[test]
-	fn git_log() -> Result<()> {
-		let repository = Repository::init(
+	fn get_repository() -> Result<Repository> {
+		Repository::init(
 			PathBuf::from(env!("CARGO_MANIFEST_DIR"))
 				.parent()
 				.expect("parent directory not found")
 				.to_path_buf(),
-		)?;
+		)
+	}
+
+	#[test]
+	fn get_latest_commit() -> Result<()> {
+		let repository = get_repository()?;
 		let commits = repository.commits(None, None, None)?;
 		let last_commit =
 			AppCommit::from(&commits.first().expect("no commits found").clone());
 		assert_eq!(get_last_commit_hash()?, last_commit.id);
-		if let Err(e) = last_commit.into_conventional() {
-			match e {
-				Error::ParseError(e) => {
-					eprintln!("\nthe last commit is not conventional\n");
-					assert_eq!(ErrorKind::InvalidFormat, e.kind())
-				}
-				_ => {
-					unreachable!()
-				}
-			}
-		}
+		Ok(())
+	}
+
+	#[test]
+	fn get_latest_tag() -> Result<()> {
+		let repository = get_repository()?;
 		let tags = repository.tags(&None, false)?;
 		assert_eq!(&get_last_tag()?, tags.last().expect("no tags found").1);
 		Ok(())
 	}
 
 	#[test]
 	fn git_tags() -> Result<()> {
-		let repository = Repository::init(
-			PathBuf::from(env!("CARGO_MANIFEST_DIR"))
-				.parent()
-				.expect("parent directory not found")
-				.to_path_buf(),
-		)?;
+		let repository = get_repository()?;
 		let tags = repository.tags(&None, true)?;
 		assert_eq!(
 			tags.get("2b8b4d3535f29231e05c3572e919634b9af907b6").expect(
 				"the commit hash does not exist in the repository (tag v0.1.0)"
 			),
 			"v0.1.0"
 		);
@@ -304,20 +297,15 @@
 		);
 		assert!(!tags.contains_key("4ddef08debfff48117586296e49d5caa0800d1b5"));
 		Ok(())
 	}
 
 	#[test]
 	fn git_upstream_remote() -> Result<()> {
-		let repository = Repository::init(
-			PathBuf::from(env!("CARGO_MANIFEST_DIR"))
-				.parent()
-				.expect("parent directory not found")
-				.to_path_buf(),
-		)?;
+		let repository = get_repository()?;
 		let remote = repository.upstream_remote()?;
 		assert_eq!(
 			Remote {
 				owner: String::from("orhun"),
 				repo:  String::from("git-cliff"),
 				token: None,
 			},
```

### Comparing `git_cliff-2.2.1/git-cliff-core/src/template.rs` & `git_cliff-2.2.2/git-cliff-core/src/template.rs`

 * *Files 1% similar despite different names*

```diff
@@ -139,24 +139,24 @@
 	pub(crate) fn contains_github_variable(&self) -> bool {
 		self.variables
 			.iter()
 			.any(|v| v.starts_with("github") || v.starts_with("commit.github"))
 	}
 
 	/// Renders the template.
-	pub fn render<C: Serialize, T: Serialize, S: Into<String> + Copy>(
+	pub fn render<C: Serialize, T: Serialize, S: Into<String> + Clone>(
 		&self,
 		context: &C,
 		additional_context: Option<&HashMap<S, T>>,
 		postprocessors: &[TextProcessor],
 	) -> Result<String> {
 		let mut context = TeraContext::from_serialize(context)?;
 		if let Some(additional_context) = additional_context {
 			for (key, value) in additional_context {
-				context.insert(*key, &value);
+				context.insert(key.clone(), &value);
 			}
 		}
 		match self.tera.render("template", &context) {
 			Ok(mut v) => {
 				for postprocessor in postprocessors {
 					postprocessor.replace(&mut v, vec![])?;
 				}
```

### Comparing `git_cliff-2.2.1/git-cliff-core/tests/integration_test.rs` & `git_cliff-2.2.2/git-cliff-core/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/README.md` & `git_cliff-2.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,20 +21,14 @@
     <a href="https://hub.docker.com/r/orhunp/git-cliff">
         <img src="https://img.shields.io/github/actions/workflow/status/orhun/git-cliff/docker.yml?style=flat&labelColor=1C2C2E&color=BEC5C9&label=docker&logo=Docker&logoColor=BEC5C9">
     </a>
     <a href="https://docs.rs/git-cliff-core/">
         <img src="https://img.shields.io/docsrs/git-cliff-core?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=Rust&logoColor=BEC5C9">
     </a>
     <br>
-    <a href="https://matrix.to/#/#git-cliff:matrix.org">
-        <img src="https://img.shields.io/matrix/git-cliff:matrix.org?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=matrix&logoColor=BEC5C9&label=join%20matrix">
-    </a>
-    <a href="https://discord.gg/W3mAwMDWH4">
-        <img src="https://img.shields.io/discord/1093977388892819553?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=discord&logoColor=BEC5C9&label=join%20discord">
-    </a>
 </p>
 
 <h4 align="center">
   <a href="https://git-cliff.org/docs">Documentation</a> |
   <a href="https://git-cliff.org">Website</a>
 </h4>
 
@@ -78,14 +72,33 @@
 
 <a href="https://github.com/orhun/git-cliff/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=orhun/git-cliff" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
+## Socials
+
+<a href="https://discord.gg/W3mAwMDWH4">
+    <img src="https://discord.com/api/guilds/1093977388892819553/embed.png?style=banner2">
+</a>
+<br>
+<a href="https://matrix.to/#/#git-cliff:matrix.org">
+    <img src="https://img.shields.io/matrix/git-cliff:matrix.org?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=matrix&logoColor=BEC5C9&label=join%20matrix">
+</a>
+<a href="https://discord.gg/W3mAwMDWH4">
+    <img src="https://img.shields.io/discord/1093977388892819553?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=discord&logoColor=BEC5C9&label=join%20discord">
+</a>
+<a href="https://twitter.com/git_cliff">
+    <img src="https://img.shields.io/twitter/follow/git_cliff?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=twitter&logoColor=BEC5C9">
+</a>
+<a href="https://fosstodon.org/@git_cliff">
+    <img src="https://img.shields.io/mastodon/follow/111545487385097711?domain=https%3A%2F%2Ffosstodon.org&style=flat&labelColor=1C2C2E&color=BEC5C9&logo=mastodon&logoColor=BEC5C9">
+</a>
+
 ## License
 
 Licensed under either of [Apache License Version 2.0](./LICENSE-APACHE) or [The MIT License](./LICENSE-MIT) at your option.
 
 ## Copyright
 
 Copyright © 2021-2024, [git-cliff contributors](mailto:git-cliff@protonmail.com)
```

#### html2text {}

```diff
@@ -10,18 +10,14 @@
 _c_i_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_G_i_t_H_u_b_%_2_0_A_c_t_i_o_n_s_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_/
 _c_d_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_G_i_t_H_u_b_%_2_0_A_c_t_i_o_n_s_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_d_e_p_l_o_y_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_/
 _d_o_c_k_e_r_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_d_o_c_k_e_r_&_l_o_g_o_=_D_o_c_k_e_r_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
                    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_s_r_s_/_g_i_t_-_c_l_i_f_f_-
   _c_o_r_e_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_R_u_s_t_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
-                   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_t_r_i_x_/_g_i_t_-_c_l_i_f_f_:
-_m_a_t_r_i_x_._o_r_g_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_t_r_i_x_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_m_a_t_r_i_x_]
-                       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
-_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_d_i_s_c_o_r_d_]
                         ****** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _WW_ee_bb_ss_ii_tt_ee ******
 **git-cliff** can generate [changelog](https://en.wikipedia.org/wiki/Changelog)
 files from the [Git](https://git-scm.com/) history by utilizing [conventional
 commits](https://git-cliff.org/docs/configuration/git#conventional_commits) as
 well as regex-powered [custom parsers](https://git-cliff.org/docs/
 configuration/git#commit_parsers). The [changelog template](https://git-
 cliff.org/docs/category/templating) can be customized with a [configuration
@@ -49,11 +45,20 @@
 changelog/tree/master/packages/conventional-recommended-bump) to semantically
 bump a NodeJS package and generate a git-cliff powered changelog. - [release-
 plz](https://github.com/MarcoIeni/release-plz) - Release Rust packages from CI.
 - [git-changelog-command-line](https://github.com/tomasbjerre/git-changelog-
 command-line) - Generate changelog and determine next version with conventional
 commits. ## Contributors Thanks goes to these wonderful people â¨ _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_]Made with [contrib.rocks](https://
-contrib.rocks). ## License Licensed under either of [Apache License Version
-2.0](./LICENSE-APACHE) or [The MIT License](./LICENSE-MIT) at your option. ##
-Copyright Copyright Â© 2021-2024, [git-cliff contributors](mailto:git-
-cliff@protonmail.com)
+contrib.rocks). ## Socials _[_h_t_t_p_s_:_/_/_d_i_s_c_o_r_d_._c_o_m_/_a_p_i_/_g_u_i_l_d_s_/_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_/
+_e_m_b_e_d_._p_n_g_?_s_t_y_l_e_=_b_a_n_n_e_r_2_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_t_r_i_x_/_g_i_t_-_c_l_i_f_f_:
+_m_a_t_r_i_x_._o_r_g_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_t_r_i_x_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_m_a_t_r_i_x_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
+_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_d_i_s_c_o_r_d_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
+_g_i_t___c_l_i_f_f_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_t_w_i_t_t_e_r_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_s_t_o_d_o_n_/_f_o_l_l_o_w_/
+_1_1_1_5_4_5_4_8_7_3_8_5_0_9_7_7_1_1_?_d_o_m_a_i_n_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_f_o_s_s_t_o_d_o_n_._o_r_g_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_s_t_o_d_o_n_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]##
+License Licensed under either of [Apache License Version 2.0](./LICENSE-APACHE)
+or [The MIT License](./LICENSE-MIT) at your option. ## Copyright Copyright Â©
+2021-2024, [git-cliff contributors](mailto:git-cliff@protonmail.com)
```

### Comparing `git_cliff-2.2.1/git-cliff/Cargo.toml` & `git_cliff-2.2.2/git-cliff/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "git-cliff"
-version = "2.2.1" # managed by release.sh
+version = "2.2.2" # managed by release.sh
 description = "A highly customizable changelog generator ⛰️"
 authors = ["git-cliff contributors <git-cliff@protonmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "../README.md"
 homepage = "https://github.com/orhun/git-cliff"
 repository = "https://github.com/orhun/git-cliff"
 keywords = ["changelog", "generator", "conventional", "commit"]
@@ -41,15 +41,15 @@
 clap_mangen = "0.2.20"
 shellexpand = "3.1.0"
 update-informer = { version = "1.1.0", optional = true }
 indicatif = { version = "0.17.8", optional = true }
 env_logger = "0.10.2"
 
 [dependencies.git-cliff-core]
-version = "2.2.1" # managed by release.sh
+version = "2.2.2" # managed by release.sh
 path = "../git-cliff-core"
 
 [dev-dependencies]
 pretty_assertions = "1.4.0"
 
 # metadata for cargo-binstall to get the right artifacts
 [package.metadata.binstall]
```

### Comparing `git_cliff-2.2.1/git-cliff/src/args.rs` & `git_cliff-2.2.2/git-cliff/src/args.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff/src/bin/completions.rs` & `git_cliff-2.2.2/git-cliff/src/bin/completions.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff/src/bin/mangen.rs` & `git_cliff-2.2.2/git-cliff/src/bin/mangen.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff/src/lib.rs` & `git_cliff-2.2.2/git-cliff/src/lib.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff/src/logger.rs` & `git_cliff-2.2.2/git-cliff/src/logger.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/git-cliff/src/main.rs` & `git_cliff-2.2.2/git-cliff/src/main.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.1/Cargo.lock` & `git_cliff-2.2.2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -45,82 +45,97 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
+
+[[package]]
+name = "async-compression"
+version = "0.4.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c90a406b4495d129f00461241616194cb8a032c8d1c53c657f0961d5f8e0498"
+dependencies = [
+ "futures-core",
+ "memchr",
+ "pin-project-lite",
+ "tokio",
+ "zstd",
+ "zstd-safe",
+]
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -136,14 +151,20 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -189,17 +210,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cacache"
-version = "12.0.0"
+version = "13.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "142316461ed3a3dfcba10417317472da5bfd0461e4d276bf7c07b330766d9490"
+checksum = "a61ff12b19d89c752c213316b87fdb4a587f073d219b893cc56974b8c9f39bf7"
 dependencies = [
  "digest",
  "either",
  "futures",
  "hex",
  "libc",
  "memmap2",
@@ -216,38 +237,39 @@
  "tokio",
  "tokio-stream",
  "walkdir",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "chrono-tz"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
@@ -305,15 +327,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -326,17 +348,17 @@
 dependencies = [
  "clap",
  "roff",
 ]
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "config"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7328b20597b53c2454f0b1919720c25c7339051c02b72b7e05409e00b14132be"
 dependencies = [
@@ -447,17 +469,17 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "deunicode"
-version = "1.4.3"
+version = "1.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6e854126756c496b8c81dec88f9a706b15b875c5849d4097a3854476b9fdf94"
+checksum = "322ef0094744e63628e6f0eb2295517f79276a5b342a4c2ff3042566ca181d4e"
 
 [[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
@@ -498,14 +520,20 @@
  "libc",
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "dissimilar"
+version = "1.0.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59f8e79d1fbf76bdfbde321e902714bf6c49df88a7dda6fc682fc2979226962d"
+
+[[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "document-features"
@@ -514,17 +542,17 @@
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
  "litrs",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -554,33 +582,43 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "expect-test"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e0be0a561335815e06dab7c62e50353134c796e7a6155402a64bcff66b6a5e0"
+dependencies = [
+ "dissimilar",
+ "once_cell",
+]
+
+[[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -649,15 +687,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -694,32 +732,32 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "git-cliff"
-version = "2.2.1"
+version = "2.2.2"
 dependencies = [
  "clap",
  "clap_complete",
  "clap_mangen",
  "dirs",
  "env_logger",
  "git-cliff-core",
@@ -732,32 +770,33 @@
  "secrecy",
  "shellexpand",
  "update-informer",
 ]
 
 [[package]]
 name = "git-cliff-core"
-version = "2.2.1"
+version = "2.2.2"
 dependencies = [
  "config",
  "dirs",
  "document-features",
+ "expect-test",
  "futures",
  "git-conventional",
  "git2",
  "glob",
  "http-cache-reqwest",
  "indexmap",
  "lazy-regex",
  "lazy_static",
  "log",
  "next_version",
  "pretty_assertions",
  "regex",
- "reqwest",
+ "reqwest 0.12.4",
  "reqwest-middleware",
  "rust-embed",
  "secrecy",
  "semver",
  "serde",
  "serde_json",
  "serde_regex",
@@ -830,27 +869,27 @@
 checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
+ "http 0.2.12",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
@@ -874,77 +913,110 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
 name = "http-body"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.12",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "http-body"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
+dependencies = [
+ "bytes",
+ "http 1.1.0",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http 1.1.0",
+ "http-body 1.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "http-cache"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b5ab65432bbdfe8490dfde21d0366353a8d39f2bc24aca0146889f931b0b4b5"
+checksum = "d6ffb12b95bb2a369fe47ca8924016c72c2fa0e6059ba98bd1516f558696c5a8"
 dependencies = [
  "async-trait",
  "bincode",
  "cacache",
- "http",
+ "http 1.1.0",
  "http-cache-semantics",
  "httpdate",
  "serde",
  "url",
 ]
 
 [[package]]
 name = "http-cache-reqwest"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8285341ce7e709c56a0f259ff1c789c70edfbaa88acd69d27e4d63980b92dc"
+checksum = "be3e27c4e2e510571cbcc601407b639667146aa9a4e818d5cc1d97c8b4b27d61"
 dependencies = [
  "anyhow",
  "async-trait",
- "http",
+ "http 1.1.0",
  "http-cache",
  "http-cache-semantics",
- "reqwest",
+ "reqwest 0.12.4",
  "reqwest-middleware",
  "serde",
- "task-local-extensions",
  "url",
 ]
 
 [[package]]
 name = "http-cache-semantics"
-version = "1.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7aec9f678bca3f4a15194b980f20ed9bfe0dd38e8d298c65c559a93dfbd6380a"
+checksum = "92baf25cf0b8c9246baecf3a444546360a97b569168fdf92563ee6a47829920c"
 dependencies = [
- "http",
+ "http 1.1.0",
  "http-serde",
  "serde",
  "time",
 ]
 
 [[package]]
 name = "http-serde"
-version = "1.1.3"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f560b665ad9f1572cfcaf034f7fb84338a7ce945216d64a90fd81f046a3caee"
+checksum = "1133cafcce27ea69d35e56b3a8772e265633e04de73c5f4e1afdffc1d19b5419"
 dependencies = [
- "http",
+ "http 1.1.0",
  "serde",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -978,39 +1050,95 @@
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
- "http",
- "http-body",
+ "http 0.2.12",
+ "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
+name = "hyper"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "httparse",
+ "itoa",
+ "pin-project-lite",
+ "smallvec",
+ "tokio",
+ "want",
+]
+
+[[package]]
 name = "hyper-rustls"
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
- "http",
- "hyper",
- "rustls 0.21.10",
+ "http 0.2.12",
+ "hyper 0.14.28",
+ "rustls 0.21.12",
+ "tokio",
+ "tokio-rustls 0.24.1",
+]
+
+[[package]]
+name = "hyper-rustls"
+version = "0.26.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0bea761b46ae2b24eb4aef630d8d1c398157b6fc29e6350ecf090a0b70c952c"
+dependencies = [
+ "futures-util",
+ "http 1.1.0",
+ "hyper 1.3.1",
+ "hyper-util",
+ "rustls 0.22.4",
+ "rustls-pki-types",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.25.0",
+ "tower-service",
+]
+
+[[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "hyper 1.3.1",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
@@ -1138,24 +1266,30 @@
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -1181,28 +1315,28 @@
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44bcd58e6c97a7fcbaffcdc95728b393b8d98933bfadad49ed4097845b57ef0b"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libflate"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ff4ae71b685bbad2f2f391fe74f6b7659a34871c08b210fdc039e43bee07d18"
 dependencies = [
@@ -1315,34 +1449,24 @@
 name = "miette-derive"
 version = "5.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49e7bc1560b95a3c4a25d03de42fe76ca718ab92d1a22a55b9b4cf67b3ae635c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
-name = "mime_guess"
-version = "2.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4192263c238a5f0d0c6bfd21f336a313a4ce1c450542449ca191bb657b4642ef"
-dependencies = [
- "mime",
- "unicase",
-]
-
-[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
@@ -1362,17 +1486,17 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "next_version"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0b8566ec538405d0feb0a7bb8262daa997f4cee2a9f9a9b7ab81f1262110d59"
+checksum = "d3e541a09da6184deaa5f0c9eeec570dbea6ea841d92c84cdfa4ff985aa535fa"
 dependencies = [
  "conventional_commit_parser",
  "semver",
 ]
 
 [[package]]
 name = "nom"
@@ -1388,17 +1512,17 @@
 name = "num-conv"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1434,17 +1558,17 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "parse-zoneinfo"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+checksum = "1f2a05b18d44e2957b88f96ba460715e295bc1d7510468a2f3d3b44535d26c24"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "pathdiff"
 version = "0.2.1"
@@ -1455,51 +1579,51 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.9"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "311fb059dee1a7b802f036316d790138c613a4e8b180c822e3925a662e9f0c95"
+checksum = "560131c633294438da9f7c4b08189194b20946c8274c6b9e38881a7874dc8ee8"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.7.9"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f73541b156d32197eecda1a4014d7f868fd2bcb3c550d5386087cfba442bf69c"
+checksum = "26293c9193fbca7b1a3bf9b79dc1e388e927e6cacaa78b4a3ab705a1d3d41459"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.7.9"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c35eeed0a3fab112f75165fdc026b3913f4183133f19b49be773ac9ea966e8bd"
+checksum = "3ec22af7d3fb470a85dd2ca96b7c577a1eb4ef6f1683a9fe9a8c16e136c04687"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.7.9"
+version = "2.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2adbf29bb9776f28caece835398781ab24435585fe0d4dc1374a61db5accedca"
+checksum = "d7a240022f37c361ec1878d646fc5b7d7c4d28d5946e1a80ad5a7a4f4ca0bdcd"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -1537,14 +1661,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
@@ -1590,17 +1734,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
@@ -1649,17 +1793,17 @@
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "reflink-copy"
-version = "0.1.15"
+version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52b1349400e2ffd64a9fb5ed9008e33c0b8ef86bd5bae8f73080839c7082f1d5"
+checksum = "7c3138c30c59ed9b8572f82bed97ea591ecd7e45012566046cc39e72679cff22"
 dependencies = [
  "cfg-if",
  "rustix",
  "windows",
 ]
 
 [[package]]
@@ -1693,63 +1837,105 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
- "http",
- "http-body",
- "hyper",
- "hyper-rustls",
+ "http 0.2.12",
+ "http-body 0.4.6",
+ "hyper 0.14.28",
+ "hyper-rustls 0.24.2",
  "ipnet",
  "js-sys",
  "log",
  "mime",
- "mime_guess",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.10",
- "rustls-pemfile",
+ "rustls 0.21.12",
+ "rustls-pemfile 1.0.4",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
- "tokio-rustls",
+ "tokio-rustls 0.24.1",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "webpki-roots 0.25.4",
- "winreg",
+ "winreg 0.50.0",
+]
+
+[[package]]
+name = "reqwest"
+version = "0.12.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
+dependencies = [
+ "async-compression",
+ "base64 0.22.1",
+ "bytes",
+ "futures-core",
+ "futures-util",
+ "http 1.1.0",
+ "http-body 1.0.0",
+ "http-body-util",
+ "hyper 1.3.1",
+ "hyper-rustls 0.26.0",
+ "hyper-util",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "rustls 0.22.4",
+ "rustls-pemfile 2.1.2",
+ "rustls-pki-types",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "sync_wrapper",
+ "tokio",
+ "tokio-rustls 0.25.0",
+ "tokio-util",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "webpki-roots 0.26.1",
+ "winreg 0.52.0",
 ]
 
 [[package]]
 name = "reqwest-middleware"
-version = "0.2.5"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a735987236a8e238bf0296c7e351b999c188ccc11477f311b82b55c93984216"
+checksum = "a45d100244a467870f6cb763c4484d010a6bed6bd610b3676e3825d93fb4cfbd"
 dependencies = [
  "anyhow",
  "async-trait",
- "http",
- "reqwest",
+ "http 1.1.0",
+ "reqwest 0.12.4",
  "serde",
- "task-local-extensions",
  "thiserror",
+ "tower-service",
 ]
 
 [[package]]
 name = "ring"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
@@ -1773,133 +1959,143 @@
 name = "roff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b833d8d034ea094b1ea68aa6d5c740e0d04bad9d16568d08ba6f76823a114316"
 
 [[package]]
 name = "rust-embed"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb78f46d0066053d16d4ca7b898e9343bc3530f71c61d5ad84cd404ada068745"
+checksum = "19549741604902eb99a7ed0ee177a0663ee1eda51a29f71401f166e47e77806a"
 dependencies = [
  "include-flate",
  "rust-embed-impl",
  "rust-embed-utils",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-impl"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b91ac2a3c6c0520a3fb3dd89321177c3c692937c4eb21893378219da10c44fc8"
+checksum = "cb9f96e283ec64401f30d3df8ee2aaeb2561f34c824381efa24a35f79bf40ee4"
 dependencies = [
  "proc-macro2",
  "quote",
  "rust-embed-utils",
- "syn 2.0.58",
+ "syn 2.0.63",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-utils"
-version = "8.3.0"
+version = "8.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f69089032567ffff4eada41c573fc43ff466c7db7c5688b2e7969584345581"
+checksum = "38c74a686185620830701348de757fd36bef4aa9680fd23c49fc539ddcc1af32"
 dependencies = [
  "sha2",
  "walkdir",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
- "rustls-webpki 0.102.2",
+ "rustls-webpki 0.102.3",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
+]
+
+[[package]]
+name = "rustls-pemfile"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
+dependencies = [
+ "base64 0.22.1",
+ "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1924,43 +2120,43 @@
 dependencies = [
  "serde",
  "zeroize",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2058,18 +2254,24 @@
 checksum = "3bd94acec9c8da640005f8e135a39fc0372e74535e6b368b7a04b875f784c8c4"
 dependencies = [
  "deunicode",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "smallvec"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -2079,15 +2281,15 @@
 
 [[package]]
 name = "ssri"
 version = "9.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da7a2b3c2bc9693bcb40870c4e9b5bf0d79f9cb46273321bf855ec513e919082"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "digest",
  "hex",
  "miette",
  "serde",
  "sha-1",
  "sha2",
  "thiserror",
@@ -2115,17 +2317,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2152,23 +2354,14 @@
 checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
-name = "task-local-extensions"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba323866e5d033818e3240feeb9f7db2c4296674e4d9e16b97b7bf8f490434e8"
-dependencies = [
- "pin-utils",
-]
-
-[[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
@@ -2215,37 +2408,37 @@
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.35"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef89ece63debf11bc32d1ed8d078ac870cbeb44da02afb02a9ff135ae7ca0582"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -2304,24 +2497,35 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.10",
+ "rustls 0.21.12",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-rustls"
+version = "0.25.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
+dependencies = [
+ "rustls 0.22.4",
+ "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2330,24 +2534,23 @@
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml"
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
@@ -2365,37 +2568,60 @@
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.9"
+version = "0.22.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
+checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
@@ -2501,51 +2727,51 @@
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "update-informer"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f8811797a24ff123db3c6e1087aa42551d03d772b3724be421ad063da1f5f3f"
 dependencies = [
  "directories",
- "reqwest",
+ "reqwest 0.11.27",
  "semver",
  "serde",
  "serde_json",
  "ureq",
 ]
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64",
+ "base64 0.22.1",
  "flate2",
  "log",
  "once_cell",
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
- "rustls-webpki 0.102.2",
+ "rustls-webpki 0.102.3",
  "serde",
  "serde_json",
  "url",
  "webpki-roots 0.26.1",
 ]
 
 [[package]]
@@ -2620,15 +2846,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2654,15 +2880,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2691,80 +2917,82 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
 dependencies = [
  "rustls-pki-types",
 ]
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "winapi-util"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-util"
-version = "0.1.6"
+name = "windows"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "1de69df01bdf1ead2f4ac895dc77c9351aefff65b2f3db429a343f9cbf05e132"
 dependencies = [
- "winapi",
+ "windows-core 0.56.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.5",
+]
 
 [[package]]
-name = "windows"
-version = "0.54.0"
+name = "windows-core"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9252e5725dbed82865af151df558e754e4a3c2c30818359eb17465f1346a1b49"
+checksum = "4698e52ed2d08f8658ab0c39512a7c00ee5fe2688c65f8c0a4f06750d729f2a6"
 dependencies = [
- "windows-core 0.54.0",
- "windows-targets 0.52.4",
+ "windows-implement",
+ "windows-interface",
+ "windows-result",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
-name = "windows-core"
-version = "0.52.0"
+name = "windows-implement"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+checksum = "f6fc35f58ecd95a9b71c4f2329b911016e6bec66b3f2e6a4aad86bd2e99e2f9b"
 dependencies = [
- "windows-targets 0.52.4",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
 ]
 
 [[package]]
-name = "windows-core"
-version = "0.54.0"
+name = "windows-interface"
+version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12661b9c89351d684a50a8a643ce5f608e20243b9fb84687800163429f161d65"
+checksum = "08990546bf4edef8f431fa6326e032865f27138718c587dc21bc0265bbcb57cc"
 dependencies = [
- "windows-result",
- "windows-targets 0.52.4",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "windows-result"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd19df78e5168dfb0aedc343d1d1b8d422ab2db6756d2dc3fef75035402a3f64"
+checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2774,15 +3002,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2794,116 +3022,123 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -2911,14 +3146,24 @@
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "winreg"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
+dependencies = [
+ "cfg-if",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "xxhash-rust"
 version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927da81e25be1e1a2901d59b81b37dd2efd1fc9c9345a55007f09bf5a2d3ee03"
 
 [[package]]
 name = "yaml-rust"
@@ -2936,7 +3181,35 @@
 checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+
+[[package]]
+name = "zstd"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "7.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
+dependencies = [
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.10+zstd.1.5.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
+dependencies = [
+ "cc",
+ "pkg-config",
+]
```

### Comparing `git_cliff-2.2.1/PKG-INFO` & `git_cliff-2.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: git-cliff
-Version: 2.2.1
+Version: 2.2.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A highly customizable changelog generator ⛰️
 Keywords: changelog,generator,conventional,commit
@@ -39,20 +39,14 @@
     <a href="https://hub.docker.com/r/orhunp/git-cliff">
         <img src="https://img.shields.io/github/actions/workflow/status/orhun/git-cliff/docker.yml?style=flat&labelColor=1C2C2E&color=BEC5C9&label=docker&logo=Docker&logoColor=BEC5C9">
     </a>
     <a href="https://docs.rs/git-cliff-core/">
         <img src="https://img.shields.io/docsrs/git-cliff-core?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=Rust&logoColor=BEC5C9">
     </a>
     <br>
-    <a href="https://matrix.to/#/#git-cliff:matrix.org">
-        <img src="https://img.shields.io/matrix/git-cliff:matrix.org?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=matrix&logoColor=BEC5C9&label=join%20matrix">
-    </a>
-    <a href="https://discord.gg/W3mAwMDWH4">
-        <img src="https://img.shields.io/discord/1093977388892819553?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=discord&logoColor=BEC5C9&label=join%20discord">
-    </a>
 </p>
 
 <h4 align="center">
   <a href="https://git-cliff.org/docs">Documentation</a> |
   <a href="https://git-cliff.org">Website</a>
 </h4>
 
@@ -96,14 +90,33 @@
 
 <a href="https://github.com/orhun/git-cliff/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=orhun/git-cliff" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
 
+## Socials
+
+<a href="https://discord.gg/W3mAwMDWH4">
+    <img src="https://discord.com/api/guilds/1093977388892819553/embed.png?style=banner2">
+</a>
+<br>
+<a href="https://matrix.to/#/#git-cliff:matrix.org">
+    <img src="https://img.shields.io/matrix/git-cliff:matrix.org?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=matrix&logoColor=BEC5C9&label=join%20matrix">
+</a>
+<a href="https://discord.gg/W3mAwMDWH4">
+    <img src="https://img.shields.io/discord/1093977388892819553?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=discord&logoColor=BEC5C9&label=join%20discord">
+</a>
+<a href="https://twitter.com/git_cliff">
+    <img src="https://img.shields.io/twitter/follow/git_cliff?style=flat&labelColor=1C2C2E&color=BEC5C9&logo=twitter&logoColor=BEC5C9">
+</a>
+<a href="https://fosstodon.org/@git_cliff">
+    <img src="https://img.shields.io/mastodon/follow/111545487385097711?domain=https%3A%2F%2Ffosstodon.org&style=flat&labelColor=1C2C2E&color=BEC5C9&logo=mastodon&logoColor=BEC5C9">
+</a>
+
 ## License
 
 Licensed under either of [Apache License Version 2.0](./LICENSE-APACHE) or [The MIT License](./LICENSE-MIT) at your option.
 
 ## Copyright
 
 Copyright © 2021-2024, [git-cliff contributors](mailto:git-cliff@protonmail.com)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: git-cliff Version: 2.2.1 Classifier: Intended
+Metadata-Version: 2.3 Name: git-cliff Version: 2.2.2 Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development Classifier:
 Programming Language :: Rust Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Summary: A highly customizable changelog generator
 â°ï¸ Keywords: changelog,generator,conventional,commit Home-Page: https://
 github.com/orhun/git-cliff Author: git-cliff contributors
 protonmail.com> Author-email: git-cliff contributors
@@ -21,18 +21,14 @@
 _c_i_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_G_i_t_H_u_b_%_2_0_A_c_t_i_o_n_s_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_/
 _c_d_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_G_i_t_H_u_b_%_2_0_A_c_t_i_o_n_s_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_d_e_p_l_o_y_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_/
 _d_o_c_k_e_r_._y_m_l_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_d_o_c_k_e_r_&_l_o_g_o_=_D_o_c_k_e_r_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
                    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_s_r_s_/_g_i_t_-_c_l_i_f_f_-
   _c_o_r_e_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_R_u_s_t_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
-                   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_t_r_i_x_/_g_i_t_-_c_l_i_f_f_:
-_m_a_t_r_i_x_._o_r_g_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_t_r_i_x_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_m_a_t_r_i_x_]
-                       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
-_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_d_i_s_c_o_r_d_]
                         ****** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _WW_ee_bb_ss_ii_tt_ee ******
 **git-cliff** can generate [changelog](https://en.wikipedia.org/wiki/Changelog)
 files from the [Git](https://git-scm.com/) history by utilizing [conventional
 commits](https://git-cliff.org/docs/configuration/git#conventional_commits) as
 well as regex-powered [custom parsers](https://git-cliff.org/docs/
 configuration/git#commit_parsers). The [changelog template](https://git-
 cliff.org/docs/category/templating) can be customized with a [configuration
@@ -60,11 +56,20 @@
 changelog/tree/master/packages/conventional-recommended-bump) to semantically
 bump a NodeJS package and generate a git-cliff powered changelog. - [release-
 plz](https://github.com/MarcoIeni/release-plz) - Release Rust packages from CI.
 - [git-changelog-command-line](https://github.com/tomasbjerre/git-changelog-
 command-line) - Generate changelog and determine next version with conventional
 commits. ## Contributors Thanks goes to these wonderful people â¨ _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_o_r_h_u_n_/_g_i_t_-_c_l_i_f_f_]Made with [contrib.rocks](https://
-contrib.rocks). ## License Licensed under either of [Apache License Version
-2.0](./LICENSE-APACHE) or [The MIT License](./LICENSE-MIT) at your option. ##
-Copyright Copyright Â© 2021-2024, [git-cliff contributors](mailto:git-
-cliff@protonmail.com)
+contrib.rocks). ## Socials _[_h_t_t_p_s_:_/_/_d_i_s_c_o_r_d_._c_o_m_/_a_p_i_/_g_u_i_l_d_s_/_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_/
+_e_m_b_e_d_._p_n_g_?_s_t_y_l_e_=_b_a_n_n_e_r_2_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_t_r_i_x_/_g_i_t_-_c_l_i_f_f_:
+_m_a_t_r_i_x_._o_r_g_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_t_r_i_x_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_m_a_t_r_i_x_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
+_1_0_9_3_9_7_7_3_8_8_8_9_2_8_1_9_5_5_3_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_&_l_a_b_e_l_=_j_o_i_n_%_2_0_d_i_s_c_o_r_d_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/
+_g_i_t___c_l_i_f_f_?_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_t_w_i_t_t_e_r_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_m_a_s_t_o_d_o_n_/_f_o_l_l_o_w_/
+_1_1_1_5_4_5_4_8_7_3_8_5_0_9_7_7_1_1_?_d_o_m_a_i_n_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_f_o_s_s_t_o_d_o_n_._o_r_g_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_1_C_2_C_2_E_&_c_o_l_o_r_=_B_E_C_5_C_9_&_l_o_g_o_=_m_a_s_t_o_d_o_n_&_l_o_g_o_C_o_l_o_r_=_B_E_C_5_C_9_]##
+License Licensed under either of [Apache License Version 2.0](./LICENSE-APACHE)
+or [The MIT License](./LICENSE-MIT) at your option. ## Copyright Copyright Â©
+2021-2024, [git-cliff contributors](mailto:git-cliff@protonmail.com)
```

