# Comparing `tmp/imaparms-2.6.0.tar.gz` & `tmp/imaparms-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaparms-2.6.0.tar", last modified: Tue Feb 13 12:52:07 2024, max compression
+gzip compressed data, was "imaparms-2.6.1.tar", last modified: Sat May 11 16:05:24 2024, max compression
```

## Comparing `imaparms-2.6.0.tar` & `imaparms-2.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-02-13 12:52:07.525032 imaparms-2.6.0/
--rw-------   0 oxij      (1000) oxij      (1000)    35149 2023-12-19 01:21:34.000000 imaparms-2.6.0/LICENSE.txt
--rw-------   0 oxij      (1000) oxij      (1000)    63550 2024-02-13 12:52:07.525032 imaparms-2.6.0/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)    62262 2024-02-13 12:51:53.000000 imaparms-2.6.0/README.md
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-02-13 12:52:07.523032 imaparms-2.6.0/imaparms/
--rw-------   0 oxij      (1000) oxij      (1000)        0 2023-08-10 16:58:11.000000 imaparms-2.6.0/imaparms/__init__.py
--rwx------   0 oxij      (1000) oxij      (1000)    85583 2024-02-13 11:07:27.000000 imaparms-2.6.0/imaparms/__main__.py
--rw-------   0 oxij      (1000) oxij      (1000)     8610 2024-01-23 16:54:28.000000 imaparms-2.6.0/imaparms/argparse_better.py
--rw-------   0 oxij      (1000) oxij      (1000)     1818 2023-12-19 01:21:34.000000 imaparms-2.6.0/imaparms/exceptions.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-02-13 12:52:07.525032 imaparms-2.6.0/imaparms.egg-info/
--rw-------   0 oxij      (1000) oxij      (1000)    63550 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)      332 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/SOURCES.txt
--rw-------   0 oxij      (1000) oxij      (1000)        1 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/dependency_links.txt
--rw-------   0 oxij      (1000) oxij      (1000)       52 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/entry_points.txt
--rw-------   0 oxij      (1000) oxij      (1000)       46 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/requires.txt
--rw-------   0 oxij      (1000) oxij      (1000)        9 2024-02-13 12:52:07.000000 imaparms-2.6.0/imaparms.egg-info/top_level.txt
--rw-------   0 oxij      (1000) oxij      (1000)     1546 2024-02-13 11:09:53.000000 imaparms-2.6.0/pyproject.toml
--rw-------   0 oxij      (1000) oxij      (1000)       38 2024-02-13 12:52:07.525032 imaparms-2.6.0/setup.cfg
--rw-------   0 oxij      (1000) oxij      (1000)       60 2023-07-17 16:31:11.000000 imaparms-2.6.0/setup.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:05:24.208047 imaparms-2.6.1/
+-rw-------   0 oxij      (1000) oxij      (1000)    35149 2023-12-19 01:21:34.000000 imaparms-2.6.1/LICENSE.txt
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    63668 2024-05-11 16:05:24.207047 imaparms-2.6.1/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)    62262 2024-05-11 15:11:15.000000 imaparms-2.6.1/README.md
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:05:24.205047 imaparms-2.6.1/imaparms/
+-rw-------   0 oxij      (1000) oxij      (1000)        0 2023-08-10 16:58:11.000000 imaparms-2.6.1/imaparms/__init__.py
+-rwx------   0 oxij      (1000) oxij      (1000)    85278 2024-05-11 15:57:39.000000 imaparms-2.6.1/imaparms/__main__.py
+-rw-------   0 oxij      (1000) oxij      (1000)     8610 2024-01-23 16:54:28.000000 imaparms-2.6.1/imaparms/argparse_better.py
+-rw-------   0 oxij      (1000) oxij      (1000)     1818 2023-12-19 01:21:34.000000 imaparms-2.6.1/imaparms/exceptions.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:05:24.207047 imaparms-2.6.1/imaparms.egg-info/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    63668 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)      332 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/SOURCES.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        1 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/dependency_links.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       52 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/entry_points.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       46 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/requires.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        9 2024-05-11 16:05:24.000000 imaparms-2.6.1/imaparms.egg-info/top_level.txt
+-rw-------   0 oxij      (1000) oxij      (1000)     1598 2024-05-11 15:57:39.000000 imaparms-2.6.1/pyproject.toml
+-rw-------   0 oxij      (1000) oxij      (1000)       38 2024-05-11 16:05:24.208047 imaparms-2.6.1/setup.cfg
+-rw-------   0 oxij      (1000) oxij      (1000)       60 2023-07-17 16:31:11.000000 imaparms-2.6.1/setup.py
```

### Comparing `imaparms-2.6.0/LICENSE.txt` & `imaparms-2.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imaparms-2.6.0/PKG-INFO` & `imaparms-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: imaparms
-Version: 2.6.0
+Version: 2.6.1
 Summary: A handy Swiss-army-knife-like utility for fetching, flagging/marking, deleting/expiring, and performing other batch operations on messages residing on IMAP servers
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/imaparms/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/imaparms
+Project-URL: Support Development, https://oxij.org/#support
 Keywords: IMAP,IMAP4,mail,email,e-mail,mail delivery agent,MDA,LDA,fetchmail,getmail,fdm,fetch,archive,download,delete,expire,mark,star,mark as seen,mark as unseen,mark as flagged,mark as unflagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Office/Business
@@ -18,14 +19,15 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
 
 # What is `imaparms`?
 
 `imaparms` is a *handy* Swiss-army-knife-like tool/utility/console app for POSIX-compatible systems that can help you to download/fetch/backup all your mail/email from an IMAP server (e.g. GMail, Yahoo, Hotmail, Yandex, etc, or your own private mail server) to your hard disk, programmatically change flags on messages on the IMAP server (e.g. mark all messages newer than a day old in some folder as unread), delete/expire old messages from the IMAP server, and similar.
 
 Or, more formally: `imaparms` is a utility for fetching and performing batch operations on messages residing on IMAP servers.
 That is: login to a specified server, fetch or perform specified actions (count, flag/mark, delete, etc) on all messages matching specified criteria in all specified folders, logout.
```

### Comparing `imaparms-2.6.0/README.md` & `imaparms-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `imaparms-2.6.0/imaparms/__main__.py` & `imaparms-2.6.1/imaparms/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,15 @@
     error(title)
     try:
         notify_failure(cfg, title, body)
     except Exception:
         pass
 
 class AccountFailure(Failure): pass
+class AccountSoftFailure(AccountFailure): pass
 class FolderFailure(AccountFailure): pass
 
 def format_imap_error(command : str, typ : str, data : _t.Any = None) -> _t.Any:
     if data is None:
         return gettext("IMAP %s command failed: %s") % (command, typ)
     else:
         return gettext("IMAP %s command failed: %s %s") % (command, typ, repr(data))
@@ -353,26 +354,50 @@
     host : str
     port : int
     user : str
     password : str
     allow_login : bool
     IMAP_base : type
 
+    no_conflicts : bool = _dc.field(default = True)
     num_delivered : int = _dc.field(default = 0)
     num_undelivered : int = _dc.field(default = 0)
     num_marked : int = _dc.field(default = 0)
     num_trashed : int = _dc.field(default = 0)
     num_deleted : int = _dc.field(default = 0)
     log : _t.List[str] = _dc.field(default_factory = lambda: [])
     errors : _t.List[str] = _dc.field(default_factory = lambda: [])
 
+    def reset(self) -> None:
+        self.no_conflicts = True
+        self.num_delivered = 0
+        self.num_undelivered = 0
+        self.num_marked = 0
+        self.num_trashed = 0
+        self.num_deleted = 0
+        self.log = []
+        self.errors = []
+
 def account_error(account : Account, message : str) -> None:
     account.errors.append(message)
     error(message)
 
+def account_conflict(account : Account, attrs : _t.Dict[bytes, bytes]) -> None:
+    chmsg = gettext("the other client changed: %s") % (repr(attrs),)
+    if account.no_conflicts:
+        account.no_conflicts = False
+        errmsg = gettext("another IMAP client is performing potentially conflicting actions in parallel with us")
+        account.errors.append(errmsg)
+        error(errmsg + "\n" + chmsg)
+    else:
+        issue(chmsg)
+    # we simply print this error and continue because `delete` command will do
+    # nothing if any `account.no_conflicts` is False or `account.errors` is
+    # not empty
+
 def connect(account : Account, debug : bool) -> _t.Any:
     if debug:
         binstderr = os.fdopen(sys.stderr.fileno(), "wb")
         class IMAP(account.IMAP_base): # type: ignore
             def send(self, data : bytes) -> int:
                 binstderr.write(b"C: " + data)
                 binstderr.flush()
@@ -488,20 +513,19 @@
     log = []
     errors = []
 
     account : Account
     for account in cfg.accounts:
         if want_stop: raise KeyboardInterrupt()
 
+        account.reset()
+
         try:
             srv = connect(account, cfg.debug)
-        except AccountFailure as exc:
-            state.num_errors += 1
-            account_error(account, str(exc))
-        else:
+
             do_logout = True
             try:
                 data = imap_check(AccountFailure, "CAPABILITY", srv.capability())
                 try:
                     capabilities = data[0].decode("ascii").split(" ")
                     if "IMAP4rev1" not in capabilities:
                         raise ValueError()
@@ -527,47 +551,47 @@
                 if typ != "OK":
                     raise AccountFailure("failed to login (%s) as %s to host %s port %d: %s", method, account.user, account.host, account.port, repr(data))
                 srv.state = "AUTH"
 
                 report("# " + gettext("logged in (%s) as %s to host %s port %d (%s)") % (method, account.user, account.host, account.port, account.socket.upper()))
 
                 func(cfg, state, account, srv, *args)
-            except AccountFailure as exc:
-                state.num_errors += 1
+            except AccountSoftFailure as exc:
                 account_error(account, str(exc))
-            except OSError as exc:
+            except BaseException:
                 do_logout = False
-                state.num_errors += 1
-                account_error(account, gettext("unexpected failure while working with host %s port %s: %s") % (account.host, account.port, repr(exc)))
+                raise
             finally:
                 if do_logout:
                     try:
                         srv.logout()
                     except Exception:
                         pass
                 else:
                     srv.shutdown()
                 srv = None
+        except AccountFailure as exc:
+            account_error(account, str(exc))
+        except IMAP4.abort as exc:
+            account_error(account, gettext("imaplib") + ": " + str(exc))
+        except OSError as exc:
+            account_error(account, gettext("unexpected failure while working with host %s port %s: %s") % (account.host, account.port, repr(exc)))
         finally:
             num_delivered += account.num_delivered
             num_marked += account.num_marked
             num_trashed += account.num_trashed
             num_deleted += account.num_deleted
             num_undelivered += account.num_undelivered
             if len(account.log) > 0:
                 log.append(gettext("%s on %s:") % \
                            (account.user, account.host) + \
                            "\n- " + "\n- ".join(account.log))
+            state.num_errors += len(account.errors)
             errors += account.errors
 
-            account.num_delivered, account.num_undelivered = 0, 0
-            account.num_marked, account.num_trashed, account.num_deleted = 0, 0, 0
-            account.log = []
-            account.errors = []
-
     if len(state.hooks) > 0:
         for hook in state.hooks:
             report("# " + gettext("running `%s`") % (hook,))
             run_hook(hook)
         state.hooks = []
 
     good = []
@@ -579,17 +603,18 @@
         good.append(ngettext("trashed %d message", "trashed %d messages", num_trashed) % (num_trashed,))
     if num_deleted > 0:
         good.append(ngettext("deleted %d message", "deleted %d messages", num_deleted) % (num_deleted,))
 
     bad = []
     if num_undelivered > 0:
         bad.append(ngettext("failed to fetch %d message", "failed to fetch %d messages", num_undelivered) % (num_undelivered,))
-    num_errors = len(errors)
-    if num_errors > 0:
-        bad.append(ngettext("produced %d new error", "produced %d new errors", num_errors) % (num_errors,))
+
+    num_new_errors = len(errors)
+    if num_new_errors > 0:
+        bad.append(ngettext("produced %d new error", "produced %d new errors", num_new_errors) % (num_new_errors,))
 
     if len(good) > 0:
         title = gettext(", ").join(good)
         info(cfg, "# " + gettext("poll: ") + title)
         notify_success(cfg, title, "\n".join(log))
 
     if len(bad) > 0:
@@ -722,26 +747,23 @@
         folders = cfg.folders
 
     for folder in filter(lambda f: f not in cfg.not_folders, folders):
         if want_stop: raise KeyboardInterrupt()
 
         typ, data = srv.select(imap_quote(folder))
         if typ != "OK":
-            state.num_errors += 1
-            error(format_imap_error("SELECT", typ, data))
-            account_error(account, gettext("failed to IMAP SELECT folder `%s`, skipping") % (folder,))
+            account_error(account, format_imap_error("SELECT", typ, data))
             continue
 
         try:
             func(cfg, state, account, srv, folder, *args)
         except FolderFailure as exc:
-            state.num_errors += 1
             account_error(account, str(exc))
-        finally:
-            srv.close()
+
+        srv.close()
 
 def do_folder_action(cfg : Namespace, state : State, account : Account, srv : IMAP4,
                      folder : str, command : str) -> None:
 
     typ, data = srv.uid("SEARCH", cfg.search_filter)
     if typ != "OK":
         raise imap_exc(FolderFailure, "SEARCH", typ, data)
@@ -790,16 +812,16 @@
             assert False
     else:
         assert False
 
     if cfg.dry_run:
         report(gettext("dry-run: (not) " + act) % actargs)
         return
-    elif command == "delete" and len(account.errors) > 0:
-        account_error(account, gettext("one of the previous commands produced errors, not " + act) % actargs)
+    elif command == "delete" and (not account.no_conflicts or len(account.errors) > 0):
+        account_error(account, gettext("one of the previous commands reported issues, not " + act) % actargs)
         return
     else:
         report(gettext(act) % actargs)
 
     if num_messages == 0:
         # nothing to do
         return
@@ -857,38 +879,36 @@
         if want_stop: raise KeyboardInterrupt()
 
         to_fetch, message_uids = message_uids[:fetch_num], message_uids[fetch_num:]
         to_fetch_set : _t.Set[bytes] = set(to_fetch)
         typ, data = srv.uid("FETCH", b",".join(to_fetch), "(RFC822.SIZE)") # type: ignore
         if typ != "OK":
             account.num_undelivered += len(to_fetch)
-            state.num_errors += 1
-            error(format_imap_error("FETCH", typ, data))
+            account_error(account, format_imap_error("FETCH", typ, data))
             continue
 
         new = []
         for el in data:
             _, attrs_ = imap_parse(el)
             attrs = imap_parse_attrs(attrs_)
             #print(attrs)
 
             try:
                 uid = attrs[b"UID"]
                 size = int(attrs[b"RFC822.SIZE"])
             except KeyError:
-                fetch_check_untagged(cfg, state, attrs)
+                account_conflict(account, attrs)
                 continue
 
             new.append((uid, size))
             to_fetch_set.remove(uid)
 
         if len(to_fetch_set) > 0:
             account.num_undelivered += len(to_fetch)
-            state.num_errors += 1
-            error(format_imap_error("FETCH", "did not get enough elements"))
+            account_error(account, format_imap_error("FETCH", "the result does not have all requested messages"))
             continue
 
         while True:
             leftovers = []
             for uel in new:
                 uid, size = uel
                 if len(batch) < cfg.batch_number and batch_total + size < cfg.batch_size:
@@ -908,48 +928,28 @@
             do_fetch_batch(cfg, state, account, srv, batch, batch_total)
             batch = []
             batch_total = 0
             new = leftovers
 
     do_fetch_batch(cfg, state, account, srv, batch, batch_total)
 
-def fetch_check_untagged(cfg : Namespace, state : State, attrs : _t.Dict[bytes, bytes]) -> None:
-    try:
-        flags = attrs[b"FLAGS"]
-        if len(attrs) != 1:
-            raise KeyError()
-    except KeyError:
-        sys.stderr.write("attrs dump: %s" % (repr(attrs),) + "\n")
-        sys.stderr.flush()
-        raise AccountFailure("another client is performing unknown conflicting actions in parallel with us, aborting `fetch`")
-
-    # This is an untagged response generated by the server because
-    # another client changed some flags.
-    # Let's check they did not add or remove the flag we use for tracking state.
-    if (cfg.mark == "seen" and b"\\Seen" in flags) or \
-       (cfg.mark == "unseen" and b"\\Seen" not in flags) or \
-       (cfg.mark == "flagged" and b"\\Flagged" in flags) or \
-       (cfg.mark == "unflagged" and b"\\Flagged" not in flags):
-        raise AccountFailure("another client is marking messages with potentially conflicting flags in parallel with us, aborting `fetch`")
-
 def do_fetch_batch(cfg : Namespace, state : State, account : Account, srv : IMAP4, message_uids : _t.List[bytes], total_size : int) -> None:
     if want_stop: raise KeyboardInterrupt()
 
     if len(message_uids) == 0: return
     info(cfg, "... " + gettext("fetching a batch of %d messages (%d bytes)") % (len(message_uids), total_size))
 
     # because time.time() gives a float
     epoch_ms = time.time_ns() // 1000000
 
     joined = b",".join(message_uids)
     typ, data = srv.uid("FETCH", joined, "(BODY.PEEK[HEADER] BODY.PEEK[TEXT])") # type: ignore
     if typ != "OK":
         account.num_undelivered += len(message_uids)
-        state.num_errors += 1
-        error(format_imap_error("FETCH", typ, data))
+        account_error(account, format_imap_error("FETCH", typ, data))
         return
 
     if cfg.maildir is not None:
         internal_mda = True
         unsynced = []
         destdir = os.path.expanduser(cfg.maildir)
         try:
@@ -992,15 +992,15 @@
         #print(attrs)
 
         try:
             uid = attrs[b"UID"]
             header = attrs[b"BODY[HEADER]"]
             body = attrs[b"BODY[TEXT]"]
         except KeyError:
-            fetch_check_untagged(cfg, state, attrs)
+            account_conflict(account, attrs)
             continue
 
         if True:
             # strip \r like fetchmail does
             header = header.replace(b"\r\n", b"\n")
             body = body.replace(b"\r\n", b"\n")
 
@@ -1155,19 +1155,18 @@
     else:
         how = "--mda " + cfg.mda
 
     if num_delivered > 0:
         info(cfg, "... " + ngettext("delivered %d message via `%s`", "delivered %d messages via `%s`", num_delivered) % (num_delivered, how))
 
     if num_undelivered > 0:
-        state.num_errors += 1
-        error(ngettext("failed to deliver %d message via `%s`", "failed to deliver %d messages via `%s`", num_undelivered) % (num_undelivered, how))
+        account_error(account, ngettext("failed to deliver %d message via `%s`", "failed to deliver %d messages via `%s`", num_undelivered) % (num_undelivered, how))
         if cfg.paranoid is not None:
             if num_delivered == 0:
-                raise AccountFailure(gettext("failed to deliver any messages, aborting `fetch`"))
+                raise AccountSoftFailure(gettext("failed to deliver any messages, aborting this `fetch` and any following commands"))
             elif cfg.paranoid:
                 raise CatastrophicFailure(gettext("failed to deliver %d messages in paranoid mode"), num_undelivered)
 
     do_store(cfg, state, account, srv, cfg.mark, done_uids, False)
 
 marking_as = "... " + gettext("marking a batch of %d messages as %s")
 
@@ -1209,16 +1208,15 @@
             if method in ["delete", "delete-noexpunge"]:
                 account.num_deleted += num_messages
             elif method == "gmail-trash":
                 account.num_trashed += num_messages
             else:
                 account.num_marked += num_messages
         else:
-            state.num_errors += 1
-            error(format_imap_error("STORE", typ, data))
+            account_error(account, format_imap_error("STORE", typ, data))
 
 def add_examples(fmt : _t.Any) -> None:
     _ = gettext
     fmt.add_text("# " + _("Notes on usage"))
 
     fmt.add_text(_("- When specifying account-related settings `--user` and `--pass*` options should be always specified last."))
     fmt.add_text(_("  Internally, new account definition gets emitted when a new `--pass*` option finishes processing."))
```

### Comparing `imaparms-2.6.0/imaparms/argparse_better.py` & `imaparms-2.6.1/imaparms/argparse_better.py`

 * *Files identical despite different names*

### Comparing `imaparms-2.6.0/imaparms/exceptions.py` & `imaparms-2.6.1/imaparms/exceptions.py`

 * *Files identical despite different names*

### Comparing `imaparms-2.6.0/imaparms.egg-info/PKG-INFO` & `imaparms-2.6.1/imaparms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: imaparms
-Version: 2.6.0
+Version: 2.6.1
 Summary: A handy Swiss-army-knife-like utility for fetching, flagging/marking, deleting/expiring, and performing other batch operations on messages residing on IMAP servers
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/imaparms/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/imaparms
+Project-URL: Support Development, https://oxij.org/#support
 Keywords: IMAP,IMAP4,mail,email,e-mail,mail delivery agent,MDA,LDA,fetchmail,getmail,fdm,fetch,archive,download,delete,expire,mark,star,mark as seen,mark as unseen,mark as flagged,mark as unflagged
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Office/Business
@@ -18,14 +19,15 @@
 Classifier: Topic :: System :: Archiving :: Mirroring
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.8"
 
 # What is `imaparms`?
 
 `imaparms` is a *handy* Swiss-army-knife-like tool/utility/console app for POSIX-compatible systems that can help you to download/fetch/backup all your mail/email from an IMAP server (e.g. GMail, Yahoo, Hotmail, Yandex, etc, or your own private mail server) to your hard disk, programmatically change flags on messages on the IMAP server (e.g. mark all messages newer than a day old in some folder as unread), delete/expire old messages from the IMAP server, and similar.
 
 Or, more formally: `imaparms` is a utility for fetching and performing batch operations on messages residing on IMAP servers.
 That is: login to a specified server, fetch or perform specified actions (count, flag/mark, delete, etc) on all messages matching specified criteria in all specified folders, logout.
```

### Comparing `imaparms-2.6.0/pyproject.toml` & `imaparms-2.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "imaparms"
-version = "2.6.0"
+version = "2.6.1"
 authors = [{ name = "Jan Malakhovski", email = "oxij@oxij.org" }]
 description = "A handy Swiss-army-knife-like utility for fetching, flagging/marking, deleting/expiring, and performing other batch operations on messages residing on IMAP servers"
 readme = "README.md"
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
@@ -36,9 +36,10 @@
 dependencies = [
     'importlib-metadata; python_version<"3.8"',
 ]
 requires-python = ">=3.7"
 [project.urls]
 "Homepage" = "https://oxij.org/software/imaparms/"
 "GitHub" = "https://github.com/Own-Data-Privateer/imaparms"
+"Support Development" = "https://oxij.org/#support"
 [project.scripts]
 imaparms = "imaparms.__main__:main"
```

