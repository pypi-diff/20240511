# Comparing `tmp/abarms-1.1.1.tar.gz` & `tmp/abarms-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abarms-1.1.1.tar", last modified: Fri Mar 22 09:22:55 2024, max compression
+gzip compressed data, was "abarms-1.1.2.tar", last modified: Sat May 11 16:50:21 2024, max compression
```

## Comparing `abarms-1.1.1.tar` & `abarms-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 09:22:55.538946 abarms-1.1.1/
--rw-------   0 oxij      (1000) oxij      (1000)    35149 2024-03-22 09:19:04.000000 abarms-1.1.1/LICENSE.txt
--rw-r--r--   0 oxij      (1000) oxij      (1000)    26081 2024-03-22 09:22:55.537946 abarms-1.1.1/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)    24908 2024-03-22 09:19:04.000000 abarms-1.1.1/README.md
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 09:22:55.535946 abarms-1.1.1/abarms/
--rw-------   0 oxij      (1000) oxij      (1000)        0 2024-02-01 08:53:18.000000 abarms-1.1.1/abarms/__init__.py
--rwx------   0 oxij      (1000) oxij      (1000)    35273 2024-03-22 09:19:04.000000 abarms-1.1.1/abarms/__main__.py
--rw-------   0 oxij      (1000) oxij      (1000)     8610 2024-02-01 08:53:18.000000 abarms-1.1.1/abarms/argparse_better.py
--rw-------   0 oxij      (1000) oxij      (1000)     1818 2024-02-01 08:53:18.000000 abarms-1.1.1/abarms/exceptions.py
--rw-------   0 oxij      (1000) oxij      (1000)     8877 2024-02-01 09:12:15.000000 abarms-1.1.1/abarms/tariter.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-22 09:22:55.537946 abarms-1.1.1/abarms.egg-info/
--rw-r--r--   0 oxij      (1000) oxij      (1000)    26081 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)      330 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/SOURCES.txt
--rw-------   0 oxij      (1000) oxij      (1000)        1 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/dependency_links.txt
--rw-------   0 oxij      (1000) oxij      (1000)       48 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/entry_points.txt
--rw-------   0 oxij      (1000) oxij      (1000)       59 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/requires.txt
--rw-------   0 oxij      (1000) oxij      (1000)        7 2024-03-22 09:22:55.000000 abarms-1.1.1/abarms.egg-info/top_level.txt
--rw-------   0 oxij      (1000) oxij      (1000)     1288 2024-03-22 09:19:53.000000 abarms-1.1.1/pyproject.toml
--rw-------   0 oxij      (1000) oxij      (1000)       38 2024-03-22 09:22:55.538946 abarms-1.1.1/setup.cfg
--rw-------   0 oxij      (1000) oxij      (1000)       60 2024-02-01 08:53:18.000000 abarms-1.1.1/setup.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:50:21.883179 abarms-1.1.2/
+-rw-------   0 oxij      (1000) oxij      (1000)    35149 2024-03-22 09:19:04.000000 abarms-1.1.2/LICENSE.txt
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    26228 2024-05-11 16:50:21.882179 abarms-1.1.2/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)    25055 2024-05-11 16:44:50.000000 abarms-1.1.2/README.md
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:50:21.880179 abarms-1.1.2/abarms/
+-rw-------   0 oxij      (1000) oxij      (1000)        0 2024-02-01 08:53:18.000000 abarms-1.1.2/abarms/__init__.py
+-rwx------   0 oxij      (1000) oxij      (1000)    35437 2024-05-11 16:44:50.000000 abarms-1.1.2/abarms/__main__.py
+-rw-------   0 oxij      (1000) oxij      (1000)     8610 2024-02-01 08:53:18.000000 abarms-1.1.2/abarms/argparse_better.py
+-rw-------   0 oxij      (1000) oxij      (1000)     1818 2024-02-01 08:53:18.000000 abarms-1.1.2/abarms/exceptions.py
+-rw-------   0 oxij      (1000) oxij      (1000)     8877 2024-02-01 09:12:15.000000 abarms-1.1.2/abarms/tariter.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-05-11 16:50:21.882179 abarms-1.1.2/abarms.egg-info/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)    26228 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)      330 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/SOURCES.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        1 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/dependency_links.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       48 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/entry_points.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       59 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/requires.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        7 2024-05-11 16:50:21.000000 abarms-1.1.2/abarms.egg-info/top_level.txt
+-rw-------   0 oxij      (1000) oxij      (1000)     1288 2024-05-11 16:44:50.000000 abarms-1.1.2/pyproject.toml
+-rw-------   0 oxij      (1000) oxij      (1000)       38 2024-05-11 16:50:21.883179 abarms-1.1.2/setup.cfg
+-rw-------   0 oxij      (1000) oxij      (1000)       60 2024-02-01 08:53:18.000000 abarms-1.1.2/setup.py
```

### Comparing `abarms-1.1.1/LICENSE.txt` & `abarms-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abarms-1.1.1/PKG-INFO` & `abarms-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abarms
-Version: 1.1.1
+Version: 1.1.2
 Summary: A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/abarms/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/abarms
 Project-URL: Support Development, https://oxij.org/#support
 Keywords: android,android backup,adb,ab,adb backup
@@ -31,15 +31,15 @@
 `abarms` can
 
 - list contents of Android Backup files,
 - strip encryption and compression from Android Backup files (so that you could re-compress them with something better for long-term storage),
 - convert Android Backup files into TAR files (which you can then unpack with standard `tar`),
 - convert TAR files into Android Backup files (though, see the documentation for `abarms wrap` below explaining why you should be careful about doing that),
 - split Android Backup files into smaller by-app backups (each of which you can then give to `adb restore` to restore that one app, or just file-level de-duplicate them between different backups),
-- merge those back into full-system backups like those produced by `adb backup`,
+- merge those small by-app backups back into full-system backups like those produced by `adb backup`,
 - and other similar things.
 
 Basically, this is a simpler pure Python implementation (only requires `setuptools` and `cryptography` modules) of [android-backup-extractor](https://github.com/nelenkov/android-backup-extractor) and the parts of [android-backup-toolkit](https://sourceforge.net/projects/android-backup-toolkit/) and [android-backup-processor](https://sourceforge.net/projects/android-backup-processor/) that I use myself.
 
 `abarms` will run on Linux and all other POSIX-compatible operating systems Python supports.
 The author also expects it will work fine on Windows, even though it was not tested there (do report an Issue if it does not).
 
@@ -66,15 +66,15 @@
 
 So, basically, according to Google (and Samsung, which ship with their own `bmgr`-like service in parallel with `bmgr`), to restore to a previous state of an app, or to migrate between phones you now apparently have to upload all your data to their servers in plain-text for their convenient data-mining and selling of your data to interested third parties.
 Google even went as far as to hide `adb backup` subcommand from their official Android documentation: compare the [old manual for `adb`](https://web.archive.org/web/20180426100826/https://developer.android.com/studio/command-line/adb) with the [current one](https://web.archive.org/web/20240129131223/https://developer.android.com/tools/adb), Control+F for "backup".
 
 This resulted into every Android vendor now making their own vendor-specific phone-to-phone migration utilities, and a whole ecosystem of commercial apps that do what `adb backup` already does, but worse.
 
 This also resulted in usefulness of `adb backup` itself being reduced because in Android version 6 Google made automatic daily file-based backups that get uploaded to Google the default when you attach your phone to your Google account.
-So, most apps started to opt-out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
+So, most apps started opting out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
 Some of those apps now implement their own in-app backup buttons hidden away in the settings menu somewhere, but most do not.
 
 Yes, this is stupid, see [this discussion on StackOverflow](https://stackoverflow.com/questions/12648373/what-is-androidallowbackup).
 See also old Android developer docs that explained this fairly clearly [here](https://web.archive.org/web/20181122123338/https://developer.android.com/guide/topics/data/backup) and [here](https://web.archive.org/web/20181118184751/https://developer.android.com/guide/topics/data/testingbackup).
 
 (You can also force an app to be included in `adb backup` by rebuilding its APK to enable `android:allowBackup` attribute in the manifest and installing the result manually, see [this](https://stackpointer.io/mobile/android-enable-adb-backup-for-any-app/462/) for more info.
 But this will only work for newly installed apps as you will have to re-sign the resulting APK with your own private key and Android forbids app updates that change the signing key.)
@@ -279,15 +279,15 @@
 
 # Usage
 
 ## abarms
 
 A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools.
 
-Android Backup files consist of a metadata header followed by a PAX-formatted TAR files optionally compressed with zlib (the only compressing Android Backup file format supports) optionally encrypted with AES-256 (the only encryption Android Backup file format supports).
+Android Backup file consists of a metadata header followed by a PAX-formatted TAR file (optionally) compressed with zlib (the only compressing Android Backup file format supports) and then (optionally) encrypted with AES-256 (the only encryption Android Backup file format supports).
 
 Below, all input decryption options apply to all subcommands taking Android Backup files as input(s) and all output encryption options apply to all subcommands producing Android Backup files as output(s).
 
 - options:
   - `--version`
   : show program's version number and exit
   - `-h, --help`
@@ -295,31 +295,31 @@
   - `--markdown`
   : show help messages formatted in Markdown
 
 - input decryption passphrase:
   - `-p PASSPHRASE, --passphrase PASSPHRASE`
   : passphrase for an encrypted `INPUT_AB_FILE`
   - `--passfile PASSFILE`
-  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" and ".adb" extensions with ".passphrase.txt"
+  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" or ".adb" extension with ".passphrase.txt"
 
 - input decryption checksum verification:
   - `--ignore-checksum`
   : ignore checksum field in `INPUT_AB_FILE`, useful when decrypting backups produced by weird Android firmwares
 
 - output encryption passphrase:
   - `--output-passphrase OUTPUT_PASSPHRASE`
   : passphrase for an encrypted `OUTPUT_AB_FILE`
   - `--output-passfile OUTPUT_PASSFILE`
   : a file containing the passphrase for an encrypted `OUTPUT_AB_FILE`
 
 - output encryption parameters:
   - `--output-salt-bytes SALT_BYTES`
-  : PBKDF2HMAC salt length in bytes (default: 64)
+  : PBKDF2HMAC salt length in bytes; default: 64
   - `--output-iterations ITERATIONS`
-  : PBKDF2HMAC iterations (default: 10000)
+  : PBKDF2HMAC iterations; default: 10000
 
 - subcommands:
   - `{ls,list,rewrap,strip,ab2ab,split,ab2many,merge,many2ab,unwrap,ab2tar,wrap,tar2ab}`
     - `ls (list)`
     : list contents of an Android Backup file
     - `rewrap (strip, ab2ab)`
     : strip or apply encyption and/or compression from/to an Android Backup file
@@ -350,25 +350,25 @@
 The former of which is useful if your Android firmware forces you to encrypt your backups but you store your backups on an encrypted media anyway and don't want to remember more passphrases than strictly necessary.
 Or if you want to strip encryption and compression and re-compress using something better than zlib.
 
 - positional arguments:
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
 
 - options:
   - `-d, --decompress`
   : produce decompressed output; this is the default
   - `-k, --keep-compression`
   : copy compression flag and data from input to output verbatim; this will make the output into a compressed Android Backup file if the input Android Backup file is compressed; this is the fastest way to `strip`, since it just copies bytes around
   - `-c, --compress`
-  : (re-)compress the output file; it will use higher compression level defaults than those used by Android, so enabling this option could make it take awhile
+  : (re-)compress the output file; it will use higher compression level defaults than those used by Android; with this option enabled `abarms` will be quite slow
   - `-e, --encrypt`
-  : (re-)encrypt the output file; enabling this option costs basically nothing on a modern CPU
+  : (re-)encrypt the output file; on a modern CPU (with AES-NI) enabling this option costs almost nothing, on an old CPU it will be quite slow
 
 ### abarms split
 
 Split a full-system Android Backup file into a bunch of per-app Android Backup files.
 
 Resulting per-app files can be given to `adb restore` to restore selected apps.
 
@@ -378,15 +378,15 @@
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
 
 - options:
   - `-c, --compress`
   : compress per-app output files
   - `-e, --encrypt`
-  : encrypt per-app output files; when enabled, the `--output-passphrase` will be reused for all the generated files (but all encryption keys will be unique)
+  : encrypt per-app output files; when enabled, the `--output-passphrase`/`--output-passfile` and other `output encryption parameters` will be reused for all the generated files, but all encryption keys and salts will be unique
   - `--prefix PREFIX`
   : file name prefix for output files; default: `abarms_split_backup` if `INPUT_AB_FILE` is "-", `abarms_split_<INPUT_AB_FILE without its ".ab" or ".adb" extension>` otherwise
 
 ### abarms merge
 
 Merge many smaller Android Backup files into a single larger one.
 A reverse operation to `split`.
@@ -427,23 +427,23 @@
 
 So you should only use this on files previously produced by `abarms unwrap` or if you know what it is you are doing.
 
 - positional arguments:
   - `INPUT_TAR_FILE`
   : a TAR file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.ab`
 
 - options:
   - `-c, --compress`
   : compress the output file
   - `-e, --encrypt`
   : encrypt the output file
   - `--output-version OUTPUT_VERSION`
-  : Android Backup file version to use (required)
+  : Android Backup file version to use; required
 
 ## Usage notes
 
 Giving an encrypted `INPUT_AB_FILE` as input, not specifying `--passphrase` or `--passfile`, and not having a file named `{INPUT_AB_FILE with ".ab" or ".adb" extension replaced with ".passphrase.txt"}` in the same directory will case the passphrase to be read interactively from the tty.
 
 ## Examples
```

### Comparing `abarms-1.1.1/README.md` & `abarms-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 `abarms` can
 
 - list contents of Android Backup files,
 - strip encryption and compression from Android Backup files (so that you could re-compress them with something better for long-term storage),
 - convert Android Backup files into TAR files (which you can then unpack with standard `tar`),
 - convert TAR files into Android Backup files (though, see the documentation for `abarms wrap` below explaining why you should be careful about doing that),
 - split Android Backup files into smaller by-app backups (each of which you can then give to `adb restore` to restore that one app, or just file-level de-duplicate them between different backups),
-- merge those back into full-system backups like those produced by `adb backup`,
+- merge those small by-app backups back into full-system backups like those produced by `adb backup`,
 - and other similar things.
 
 Basically, this is a simpler pure Python implementation (only requires `setuptools` and `cryptography` modules) of [android-backup-extractor](https://github.com/nelenkov/android-backup-extractor) and the parts of [android-backup-toolkit](https://sourceforge.net/projects/android-backup-toolkit/) and [android-backup-processor](https://sourceforge.net/projects/android-backup-processor/) that I use myself.
 
 `abarms` will run on Linux and all other POSIX-compatible operating systems Python supports.
 The author also expects it will work fine on Windows, even though it was not tested there (do report an Issue if it does not).
 
@@ -40,15 +40,15 @@
 
 So, basically, according to Google (and Samsung, which ship with their own `bmgr`-like service in parallel with `bmgr`), to restore to a previous state of an app, or to migrate between phones you now apparently have to upload all your data to their servers in plain-text for their convenient data-mining and selling of your data to interested third parties.
 Google even went as far as to hide `adb backup` subcommand from their official Android documentation: compare the [old manual for `adb`](https://web.archive.org/web/20180426100826/https://developer.android.com/studio/command-line/adb) with the [current one](https://web.archive.org/web/20240129131223/https://developer.android.com/tools/adb), Control+F for "backup".
 
 This resulted into every Android vendor now making their own vendor-specific phone-to-phone migration utilities, and a whole ecosystem of commercial apps that do what `adb backup` already does, but worse.
 
 This also resulted in usefulness of `adb backup` itself being reduced because in Android version 6 Google made automatic daily file-based backups that get uploaded to Google the default when you attach your phone to your Google account.
-So, most apps started to opt-out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
+So, most apps started opting out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
 Some of those apps now implement their own in-app backup buttons hidden away in the settings menu somewhere, but most do not.
 
 Yes, this is stupid, see [this discussion on StackOverflow](https://stackoverflow.com/questions/12648373/what-is-androidallowbackup).
 See also old Android developer docs that explained this fairly clearly [here](https://web.archive.org/web/20181122123338/https://developer.android.com/guide/topics/data/backup) and [here](https://web.archive.org/web/20181118184751/https://developer.android.com/guide/topics/data/testingbackup).
 
 (You can also force an app to be included in `adb backup` by rebuilding its APK to enable `android:allowBackup` attribute in the manifest and installing the result manually, see [this](https://stackpointer.io/mobile/android-enable-adb-backup-for-any-app/462/) for more info.
 But this will only work for newly installed apps as you will have to re-sign the resulting APK with your own private key and Android forbids app updates that change the signing key.)
@@ -253,15 +253,15 @@
 
 # Usage
 
 ## abarms
 
 A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools.
 
-Android Backup files consist of a metadata header followed by a PAX-formatted TAR files optionally compressed with zlib (the only compressing Android Backup file format supports) optionally encrypted with AES-256 (the only encryption Android Backup file format supports).
+Android Backup file consists of a metadata header followed by a PAX-formatted TAR file (optionally) compressed with zlib (the only compressing Android Backup file format supports) and then (optionally) encrypted with AES-256 (the only encryption Android Backup file format supports).
 
 Below, all input decryption options apply to all subcommands taking Android Backup files as input(s) and all output encryption options apply to all subcommands producing Android Backup files as output(s).
 
 - options:
   - `--version`
   : show program's version number and exit
   - `-h, --help`
@@ -269,31 +269,31 @@
   - `--markdown`
   : show help messages formatted in Markdown
 
 - input decryption passphrase:
   - `-p PASSPHRASE, --passphrase PASSPHRASE`
   : passphrase for an encrypted `INPUT_AB_FILE`
   - `--passfile PASSFILE`
-  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" and ".adb" extensions with ".passphrase.txt"
+  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" or ".adb" extension with ".passphrase.txt"
 
 - input decryption checksum verification:
   - `--ignore-checksum`
   : ignore checksum field in `INPUT_AB_FILE`, useful when decrypting backups produced by weird Android firmwares
 
 - output encryption passphrase:
   - `--output-passphrase OUTPUT_PASSPHRASE`
   : passphrase for an encrypted `OUTPUT_AB_FILE`
   - `--output-passfile OUTPUT_PASSFILE`
   : a file containing the passphrase for an encrypted `OUTPUT_AB_FILE`
 
 - output encryption parameters:
   - `--output-salt-bytes SALT_BYTES`
-  : PBKDF2HMAC salt length in bytes (default: 64)
+  : PBKDF2HMAC salt length in bytes; default: 64
   - `--output-iterations ITERATIONS`
-  : PBKDF2HMAC iterations (default: 10000)
+  : PBKDF2HMAC iterations; default: 10000
 
 - subcommands:
   - `{ls,list,rewrap,strip,ab2ab,split,ab2many,merge,many2ab,unwrap,ab2tar,wrap,tar2ab}`
     - `ls (list)`
     : list contents of an Android Backup file
     - `rewrap (strip, ab2ab)`
     : strip or apply encyption and/or compression from/to an Android Backup file
@@ -324,25 +324,25 @@
 The former of which is useful if your Android firmware forces you to encrypt your backups but you store your backups on an encrypted media anyway and don't want to remember more passphrases than strictly necessary.
 Or if you want to strip encryption and compression and re-compress using something better than zlib.
 
 - positional arguments:
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
 
 - options:
   - `-d, --decompress`
   : produce decompressed output; this is the default
   - `-k, --keep-compression`
   : copy compression flag and data from input to output verbatim; this will make the output into a compressed Android Backup file if the input Android Backup file is compressed; this is the fastest way to `strip`, since it just copies bytes around
   - `-c, --compress`
-  : (re-)compress the output file; it will use higher compression level defaults than those used by Android, so enabling this option could make it take awhile
+  : (re-)compress the output file; it will use higher compression level defaults than those used by Android; with this option enabled `abarms` will be quite slow
   - `-e, --encrypt`
-  : (re-)encrypt the output file; enabling this option costs basically nothing on a modern CPU
+  : (re-)encrypt the output file; on a modern CPU (with AES-NI) enabling this option costs almost nothing, on an old CPU it will be quite slow
 
 ### abarms split
 
 Split a full-system Android Backup file into a bunch of per-app Android Backup files.
 
 Resulting per-app files can be given to `adb restore` to restore selected apps.
 
@@ -352,15 +352,15 @@
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
 
 - options:
   - `-c, --compress`
   : compress per-app output files
   - `-e, --encrypt`
-  : encrypt per-app output files; when enabled, the `--output-passphrase` will be reused for all the generated files (but all encryption keys will be unique)
+  : encrypt per-app output files; when enabled, the `--output-passphrase`/`--output-passfile` and other `output encryption parameters` will be reused for all the generated files, but all encryption keys and salts will be unique
   - `--prefix PREFIX`
   : file name prefix for output files; default: `abarms_split_backup` if `INPUT_AB_FILE` is "-", `abarms_split_<INPUT_AB_FILE without its ".ab" or ".adb" extension>` otherwise
 
 ### abarms merge
 
 Merge many smaller Android Backup files into a single larger one.
 A reverse operation to `split`.
@@ -401,23 +401,23 @@
 
 So you should only use this on files previously produced by `abarms unwrap` or if you know what it is you are doing.
 
 - positional arguments:
   - `INPUT_TAR_FILE`
   : a TAR file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.ab`
 
 - options:
   - `-c, --compress`
   : compress the output file
   - `-e, --encrypt`
   : encrypt the output file
   - `--output-version OUTPUT_VERSION`
-  : Android Backup file version to use (required)
+  : Android Backup file version to use; required
 
 ## Usage notes
 
 Giving an encrypted `INPUT_AB_FILE` as input, not specifying `--passphrase` or `--passfile`, and not having a file named `{INPUT_AB_FILE with ".ab" or ".adb" extension replaced with ".passphrase.txt"}` in the same directory will case the passphrase to be read interactively from the tty.
 
 ## Examples
```

### Comparing `abarms-1.1.1/abarms/__main__.py` & `abarms-1.1.2/abarms/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,18 +698,17 @@
 def make_argparser(real : bool = True) -> _t.Any:
     _ = gettext
 
     parser = argparse.BetterArgumentParser(
         prog=__package__,
         description = _("""A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools.
 
-Android Backup files consist of a metadata header followed by a PAX-formatted TAR files optionally compressed with zlib (the only compressing Android Backup file format supports) optionally encrypted with AES-256 (the only encryption Android Backup file format supports).
-
-Below, all input decryption options apply to all subcommands taking Android Backup files as input(s) and all output encryption options apply to all subcommands producing Android Backup files as output(s).
-"""),
+Android Backup file consists of a metadata header followed by a PAX-formatted TAR file (optionally) compressed with zlib (the only compressing Android Backup file format supports) and then (optionally) encrypted with AES-256 (the only encryption Android Backup file format supports).
+""") + ("" if real else _("""
+Below, all input decryption options apply to all subcommands taking Android Backup files as input(s) and all output encryption options apply to all subcommands producing Android Backup files as output(s).""")),
         additional_sections = [add_examples],
         allow_abbrev = False,
         add_help = False,
         add_version = True)
     parser.add_argument("-h", "--help", action="store_true", help=_("show this help message and exit"))
     parser.add_argument("--markdown", action="store_true", help=_("show help messages formatted in Markdown"))
     parser.set_defaults(func=None)
@@ -719,40 +718,40 @@
         parser.error(_("no subcommand specified"))
     parser.set_defaults(func=no_cmd)
 
     def add_pass(cmd : _t.Any) -> None:
         agrp = cmd.add_argument_group(_("input decryption passphrase"))
         grp = agrp.add_mutually_exclusive_group()
         grp.add_argument("-p", "--passphrase", type=str, help=_("passphrase for an encrypted `INPUT_AB_FILE`"))
-        grp.add_argument("--passfile", type=str, help=_('a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" and ".adb" extensions with ".passphrase.txt"'))
+        grp.add_argument("--passfile", type=str, help=_('a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" or ".adb" extension with ".passphrase.txt"'))
 
         agrp = cmd.add_argument_group(_("input decryption checksum verification"))
         agrp.add_argument("--ignore-checksum", action="store_true", help=_("ignore checksum field in `INPUT_AB_FILE`, useful when decrypting backups produced by weird Android firmwares"))
 
     def add_encpass(cmd : _t.Any) -> None:
         agrp = cmd.add_argument_group(_("output encryption passphrase"))
         grp = agrp.add_mutually_exclusive_group()
         grp.add_argument("--output-passphrase", type=str, help=_("passphrase for an encrypted `OUTPUT_AB_FILE`"))
         grp.add_argument("--output-passfile", type=str, help=_("a file containing the passphrase for an encrypted `OUTPUT_AB_FILE`"))
 
         agrp = cmd.add_argument_group(_("output encryption parameters"))
-        agrp.add_argument("--output-salt-bytes", dest="salt_bytes", default=64, type=int, help=_("PBKDF2HMAC salt length in bytes (default: %(default)s)"))
-        agrp.add_argument("--output-iterations", dest="iterations", default=10000, type=int, help=_("PBKDF2HMAC iterations (default: %(default)s)"))
+        agrp.add_argument("--output-salt-bytes", dest="salt_bytes", default=64, type=int, help=_("PBKDF2HMAC salt length in bytes; default: %(default)s"))
+        agrp.add_argument("--output-iterations", dest="iterations", default=10000, type=int, help=_("PBKDF2HMAC iterations; default: %(default)s"))
 
     if not real:
         add_pass(parser)
         add_encpass(parser)
 
     subparsers = parser.add_subparsers(title="subcommands")
 
     def add_input(cmd : _t.Any) -> None:
         cmd.add_argument("input_file", metavar="INPUT_AB_FILE", type=str, help=_('an Android Backup file to be used as input, set to "-" to use standard input'))
 
     def add_output(cmd : _t.Any, extension : str) -> None:
-        cmd.add_argument("output_file", metavar="OUTPUT_AB_FILE", nargs="?", default=None, type=str, help=_('file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `%s`' % (extension,)))
+        cmd.add_argument("output_file", metavar="OUTPUT_AB_FILE", nargs="?", default=None, type=str, help=_('file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `%s`' % (extension,)))
 
     cmd = subparsers.add_parser("ls", aliases = ["list"],
                                 help=_("list contents of an Android Backup file"),
                                 description=_("List contents of an Android Backup file similar to how `tar -tvf` would do, but this will also show Android Backup file version, compression, and encryption parameters."))
     if real:
         add_pass(cmd)
     add_input(cmd)
@@ -769,16 +768,16 @@
 Or if you want to strip encryption and compression and re-compress using something better than zlib."""))
     if real:
         add_pass(cmd)
         add_encpass(cmd)
     grp = cmd.add_mutually_exclusive_group()
     grp.add_argument("-d", "--decompress", action="store_true", help=_("produce decompressed output; this is the default"))
     grp.add_argument("-k", "--keep-compression", action="store_true", help=_("copy compression flag and data from input to output verbatim; this will make the output into a compressed Android Backup file if the input Android Backup file is compressed; this is the fastest way to `strip`, since it just copies bytes around"))
-    grp.add_argument("-c", "--compress", action="store_true", help=_("(re-)compress the output file; it will use higher compression level defaults than those used by Android, so enabling this option could make it take awhile"))
-    cmd.add_argument("-e", "--encrypt", action="store_true", help=_("(re-)encrypt the output file; enabling this option costs basically nothing on a modern CPU"))
+    grp.add_argument("-c", "--compress", action="store_true", help=_(f"(re-)compress the output file; it will use higher compression level defaults than those used by Android; with this option enabled `{__package__}` will be quite slow"))
+    cmd.add_argument("-e", "--encrypt", action="store_true", help=_("(re-)encrypt the output file; on a modern CPU (with AES-NI) enabling this option costs almost nothing, on an old CPU it will be quite slow"))
 
     add_input(cmd)
     add_output(cmd, ".stripped.ab")
     cmd.set_defaults(func=ab_strip)
 
     cmd = subparsers.add_parser("split", aliases = ["ab2many"],
                                 help=_("split a full-system Android Backup file into a bunch of per-app Android Backup files"),
@@ -788,15 +787,15 @@
 
 Also, if you do backups regularly, then splitting large Android Backup files like this and deduplicating per-app files between backups could save a lot of disk space.
 """))
     if real:
         add_pass(cmd)
         add_encpass(cmd)
     cmd.add_argument("-c", "--compress", action="store_true", help=_("compress per-app output files"))
-    cmd.add_argument("-e", "--encrypt", action="store_true", help=_("encrypt per-app output files; when enabled, the `--output-passphrase` will be reused for all the generated files (but all encryption keys will be unique)"))
+    cmd.add_argument("-e", "--encrypt", action="store_true", help=_("encrypt per-app output files; when enabled, the `--output-passphrase`/`--output-passfile` and other `output encryption parameters` will be reused for all the generated files, but all encryption keys and salts will be unique"))
     cmd.add_argument("--prefix", type=str, help=_('file name prefix for output files; default: `abarms_split_backup` if `INPUT_AB_FILE` is "-", `abarms_split_<INPUT_AB_FILE without its ".ab" or ".adb" extension>` otherwise'))
     add_input(cmd)
     cmd.set_defaults(func=ab_split)
 
 
     cmd = subparsers.add_parser("merge", aliases = ["many2ab"],
                                 help=_("merge a bunch of Android Backup files into one"),
@@ -834,15 +833,15 @@
 
 So you should only use this on files previously produced by `{__package__} unwrap` or if you know what it is you are doing.
 """))
     if real:
         add_encpass(cmd)
     cmd.add_argument("-c", "--compress", action="store_true", help=_("compress the output file"))
     cmd.add_argument("-e", "--encrypt", action="store_true", help=_("encrypt the output file"))
-    cmd.add_argument("--output-version", type=int, required=True, help=_("Android Backup file version to use (required)"))
+    cmd.add_argument("--output-version", type=int, required=True, help=_("Android Backup file version to use; required"))
     cmd.add_argument("input_file", metavar="INPUT_TAR_FILE", type=str, help=_('a TAR file to be used as input, set to "-" to use standard input'))
     add_output(cmd, ".ab")
     cmd.set_defaults(func=ab_wrap)
 
     return parser
 
 def main() -> None:
```

### Comparing `abarms-1.1.1/abarms/argparse_better.py` & `abarms-1.1.2/abarms/argparse_better.py`

 * *Files identical despite different names*

### Comparing `abarms-1.1.1/abarms/exceptions.py` & `abarms-1.1.2/abarms/exceptions.py`

 * *Files identical despite different names*

### Comparing `abarms-1.1.1/abarms/tariter.py` & `abarms-1.1.2/abarms/tariter.py`

 * *Files identical despite different names*

### Comparing `abarms-1.1.1/abarms.egg-info/PKG-INFO` & `abarms-1.1.2/abarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abarms
-Version: 1.1.1
+Version: 1.1.2
 Summary: A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools
 Author-email: Jan Malakhovski <oxij@oxij.org>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://oxij.org/software/abarms/
 Project-URL: GitHub, https://github.com/Own-Data-Privateer/abarms
 Project-URL: Support Development, https://oxij.org/#support
 Keywords: android,android backup,adb,ab,adb backup
@@ -31,15 +31,15 @@
 `abarms` can
 
 - list contents of Android Backup files,
 - strip encryption and compression from Android Backup files (so that you could re-compress them with something better for long-term storage),
 - convert Android Backup files into TAR files (which you can then unpack with standard `tar`),
 - convert TAR files into Android Backup files (though, see the documentation for `abarms wrap` below explaining why you should be careful about doing that),
 - split Android Backup files into smaller by-app backups (each of which you can then give to `adb restore` to restore that one app, or just file-level de-duplicate them between different backups),
-- merge those back into full-system backups like those produced by `adb backup`,
+- merge those small by-app backups back into full-system backups like those produced by `adb backup`,
 - and other similar things.
 
 Basically, this is a simpler pure Python implementation (only requires `setuptools` and `cryptography` modules) of [android-backup-extractor](https://github.com/nelenkov/android-backup-extractor) and the parts of [android-backup-toolkit](https://sourceforge.net/projects/android-backup-toolkit/) and [android-backup-processor](https://sourceforge.net/projects/android-backup-processor/) that I use myself.
 
 `abarms` will run on Linux and all other POSIX-compatible operating systems Python supports.
 The author also expects it will work fine on Windows, even though it was not tested there (do report an Issue if it does not).
 
@@ -66,15 +66,15 @@
 
 So, basically, according to Google (and Samsung, which ship with their own `bmgr`-like service in parallel with `bmgr`), to restore to a previous state of an app, or to migrate between phones you now apparently have to upload all your data to their servers in plain-text for their convenient data-mining and selling of your data to interested third parties.
 Google even went as far as to hide `adb backup` subcommand from their official Android documentation: compare the [old manual for `adb`](https://web.archive.org/web/20180426100826/https://developer.android.com/studio/command-line/adb) with the [current one](https://web.archive.org/web/20240129131223/https://developer.android.com/tools/adb), Control+F for "backup".
 
 This resulted into every Android vendor now making their own vendor-specific phone-to-phone migration utilities, and a whole ecosystem of commercial apps that do what `adb backup` already does, but worse.
 
 This also resulted in usefulness of `adb backup` itself being reduced because in Android version 6 Google made automatic daily file-based backups that get uploaded to Google the default when you attach your phone to your Google account.
-So, most apps started to opt-out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
+So, most apps started opting out of those backups for privacy and security reasons -- which also started opting them out of being included in `adb backup` output, since `bmgr` and `bu` share most of the infrastructure.
 Some of those apps now implement their own in-app backup buttons hidden away in the settings menu somewhere, but most do not.
 
 Yes, this is stupid, see [this discussion on StackOverflow](https://stackoverflow.com/questions/12648373/what-is-androidallowbackup).
 See also old Android developer docs that explained this fairly clearly [here](https://web.archive.org/web/20181122123338/https://developer.android.com/guide/topics/data/backup) and [here](https://web.archive.org/web/20181118184751/https://developer.android.com/guide/topics/data/testingbackup).
 
 (You can also force an app to be included in `adb backup` by rebuilding its APK to enable `android:allowBackup` attribute in the manifest and installing the result manually, see [this](https://stackpointer.io/mobile/android-enable-adb-backup-for-any-app/462/) for more info.
 But this will only work for newly installed apps as you will have to re-sign the resulting APK with your own private key and Android forbids app updates that change the signing key.)
@@ -279,15 +279,15 @@
 
 # Usage
 
 ## abarms
 
 A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools.
 
-Android Backup files consist of a metadata header followed by a PAX-formatted TAR files optionally compressed with zlib (the only compressing Android Backup file format supports) optionally encrypted with AES-256 (the only encryption Android Backup file format supports).
+Android Backup file consists of a metadata header followed by a PAX-formatted TAR file (optionally) compressed with zlib (the only compressing Android Backup file format supports) and then (optionally) encrypted with AES-256 (the only encryption Android Backup file format supports).
 
 Below, all input decryption options apply to all subcommands taking Android Backup files as input(s) and all output encryption options apply to all subcommands producing Android Backup files as output(s).
 
 - options:
   - `--version`
   : show program's version number and exit
   - `-h, --help`
@@ -295,31 +295,31 @@
   - `--markdown`
   : show help messages formatted in Markdown
 
 - input decryption passphrase:
   - `-p PASSPHRASE, --passphrase PASSPHRASE`
   : passphrase for an encrypted `INPUT_AB_FILE`
   - `--passfile PASSFILE`
-  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" and ".adb" extensions with ".passphrase.txt"
+  : a file containing the passphrase for an encrypted `INPUT_AB_FILE`; similar to `-p` option but the whole contents of the file will be used verbatim, allowing you to, e.g. use new line symbols or strange character encodings in there; default: guess based on `INPUT_AB_FILE` trying to replace ".ab" or ".adb" extension with ".passphrase.txt"
 
 - input decryption checksum verification:
   - `--ignore-checksum`
   : ignore checksum field in `INPUT_AB_FILE`, useful when decrypting backups produced by weird Android firmwares
 
 - output encryption passphrase:
   - `--output-passphrase OUTPUT_PASSPHRASE`
   : passphrase for an encrypted `OUTPUT_AB_FILE`
   - `--output-passfile OUTPUT_PASSFILE`
   : a file containing the passphrase for an encrypted `OUTPUT_AB_FILE`
 
 - output encryption parameters:
   - `--output-salt-bytes SALT_BYTES`
-  : PBKDF2HMAC salt length in bytes (default: 64)
+  : PBKDF2HMAC salt length in bytes; default: 64
   - `--output-iterations ITERATIONS`
-  : PBKDF2HMAC iterations (default: 10000)
+  : PBKDF2HMAC iterations; default: 10000
 
 - subcommands:
   - `{ls,list,rewrap,strip,ab2ab,split,ab2many,merge,many2ab,unwrap,ab2tar,wrap,tar2ab}`
     - `ls (list)`
     : list contents of an Android Backup file
     - `rewrap (strip, ab2ab)`
     : strip or apply encyption and/or compression from/to an Android Backup file
@@ -350,25 +350,25 @@
 The former of which is useful if your Android firmware forces you to encrypt your backups but you store your backups on an encrypted media anyway and don't want to remember more passphrases than strictly necessary.
 Or if you want to strip encryption and compression and re-compress using something better than zlib.
 
 - positional arguments:
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.stripped.ab`
 
 - options:
   - `-d, --decompress`
   : produce decompressed output; this is the default
   - `-k, --keep-compression`
   : copy compression flag and data from input to output verbatim; this will make the output into a compressed Android Backup file if the input Android Backup file is compressed; this is the fastest way to `strip`, since it just copies bytes around
   - `-c, --compress`
-  : (re-)compress the output file; it will use higher compression level defaults than those used by Android, so enabling this option could make it take awhile
+  : (re-)compress the output file; it will use higher compression level defaults than those used by Android; with this option enabled `abarms` will be quite slow
   - `-e, --encrypt`
-  : (re-)encrypt the output file; enabling this option costs basically nothing on a modern CPU
+  : (re-)encrypt the output file; on a modern CPU (with AES-NI) enabling this option costs almost nothing, on an old CPU it will be quite slow
 
 ### abarms split
 
 Split a full-system Android Backup file into a bunch of per-app Android Backup files.
 
 Resulting per-app files can be given to `adb restore` to restore selected apps.
 
@@ -378,15 +378,15 @@
   - `INPUT_AB_FILE`
   : an Android Backup file to be used as input, set to "-" to use standard input
 
 - options:
   - `-c, --compress`
   : compress per-app output files
   - `-e, --encrypt`
-  : encrypt per-app output files; when enabled, the `--output-passphrase` will be reused for all the generated files (but all encryption keys will be unique)
+  : encrypt per-app output files; when enabled, the `--output-passphrase`/`--output-passfile` and other `output encryption parameters` will be reused for all the generated files, but all encryption keys and salts will be unique
   - `--prefix PREFIX`
   : file name prefix for output files; default: `abarms_split_backup` if `INPUT_AB_FILE` is "-", `abarms_split_<INPUT_AB_FILE without its ".ab" or ".adb" extension>` otherwise
 
 ### abarms merge
 
 Merge many smaller Android Backup files into a single larger one.
 A reverse operation to `split`.
@@ -427,23 +427,23 @@
 
 So you should only use this on files previously produced by `abarms unwrap` or if you know what it is you are doing.
 
 - positional arguments:
   - `INPUT_TAR_FILE`
   : a TAR file to be used as input, set to "-" to use standard input
   - `OUTPUT_AB_FILE`
-  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" and ".adb" extension of `INPUT_TAR_FILE` with `.ab`
+  : file to write the output to, set to "-" to use standard output; default: "-" if `INPUT_TAR_FILE` is "-", otherwise replace ".ab" or ".adb" extension of `INPUT_TAR_FILE` with `.ab`
 
 - options:
   - `-c, --compress`
   : compress the output file
   - `-e, --encrypt`
   : encrypt the output file
   - `--output-version OUTPUT_VERSION`
-  : Android Backup file version to use (required)
+  : Android Backup file version to use; required
 
 ## Usage notes
 
 Giving an encrypted `INPUT_AB_FILE` as input, not specifying `--passphrase` or `--passfile`, and not having a file named `{INPUT_AB_FILE with ".ab" or ".adb" extension replaced with ".passphrase.txt"}` in the same directory will case the passphrase to be read interactively from the tty.
 
 ## Examples
```

### Comparing `abarms-1.1.1/pyproject.toml` & `abarms-1.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "abarms"
-version = "1.1.1"
+version = "1.1.2"
 authors = [{ name = "Jan Malakhovski", email = "oxij@oxij.org" }]
 description = "A handy Swiss-army-knife-like utility for manipulating Android Backup files (`*.ab`, `*.adb`) produced by `adb backup`, `bmgr`, and similar tools"
 readme = "README.md"
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
```

