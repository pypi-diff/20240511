# Comparing `tmp/badkeys-0.0.8.tar.gz` & `tmp/badkeys-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badkeys-0.0.8.tar", last modified: Fri Apr 26 13:22:35 2024, max compression
+gzip compressed data, was "badkeys-0.0.9.tar", last modified: Fri May  3 08:23:31 2024, max compression
```

## Comparing `badkeys-0.0.8.tar` & `badkeys-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.418523 badkeys-0.0.8/
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.406524 badkeys-0.0.8/.github/
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.408523 badkeys-0.0.8/.github/workflows/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      574 2024-04-25 16:20:20.000000 badkeys-0.0.8/.github/workflows/codeql.yml
--rw-r--r--   0 hanno     (1000) hanno     (1000)      924 2024-04-25 16:20:20.000000 badkeys-0.0.8/.github/workflows/runci.yml
--rw-r--r--   0 hanno     (1000) hanno     (1000)       58 2024-04-25 16:20:20.000000 badkeys-0.0.8/.gitignore
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1138 2024-04-25 16:20:20.000000 badkeys-0.0.8/LICENSE
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3627 2024-04-26 13:22:35.417523 badkeys-0.0.8/PKG-INFO
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2565 2024-04-26 06:48:07.000000 badkeys-0.0.8/README.md
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.409524 badkeys-0.0.8/badkeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      362 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/__init__.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.410524 badkeys-0.0.8/badkeys/allkeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      105 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/allkeys/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3324 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/allkeys/block.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     7989 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/checks.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.412524 badkeys-0.0.8/badkeys/keydata/
--rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)   255328 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes1024.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)    78961 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes2048.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)      770 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes4096.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)    11449 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes512.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)      434 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes768.dat
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.413524 badkeys-0.0.8/badkeys/rsakeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      358 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      587 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/fermat.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      211 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/pattern.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1046 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/roca.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      192 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/rsainvalid.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      720 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/sharedprimes.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      599 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/smallfactors.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      533 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/xzbackdoor.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     7216 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/runcli.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1222 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/scanssh.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      380 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/scantls.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2573 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/update.py
--rwxr-xr-x   0 hanno     (1000) hanno     (1000)       68 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys-cli
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.417523 badkeys-0.0.8/badkeys.egg-info/
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3627 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/PKG-INFO
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1582 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/SOURCES.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)        1 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/dependency_links.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)       50 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/entry_points.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)       67 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/requires.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)        8 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/top_level.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1114 2024-04-26 13:16:19.000000 badkeys-0.0.8/pyproject.toml
--rw-r--r--   0 hanno     (1000) hanno     (1000)       19 2024-04-25 16:20:20.000000 badkeys-0.0.8/requirements.txt
--rwxr-xr-x   0 hanno     (1000) hanno     (1000)      363 2024-04-26 06:39:03.000000 badkeys-0.0.8/runci.sh
--rw-r--r--   0 hanno     (1000) hanno     (1000)       38 2024-04-26 13:22:35.418523 badkeys-0.0.8/setup.cfg
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.414523 badkeys-0.0.8/tests/
--rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/__init__.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.416524 badkeys-0.0.8/tests/data/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      206 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/ec-p256-rfc-example.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      149 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/ed25519-rfc-example.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      531 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-debianweak.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      453 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-e1.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      513 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-hexmodulus.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)      502 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-pkcs1.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      498 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-pkcs8.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1153 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat.crt
--rw-r--r--   0 hanno     (1000) hanno     (1000)      935 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat.csr
--rw-r--r--   0 hanno     (1000) hanno     (1000)      457 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-nprime.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      464 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-ok.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-pattern.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      426 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-roca.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      508 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-sharedprimes.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      491 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-smallfactors.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      146 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/x448-ok.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      857 2024-04-25 16:23:00.000000 badkeys-0.0.8/tests/test_ecbl.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      620 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_failures.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2090 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_fermat.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      560 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_pattern.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      545 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_roca.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      654 2024-04-25 16:22:54.000000 badkeys-0.0.8/tests/test_rsabl.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      651 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_rsainvalid.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_sharedprimes.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      591 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_smallprimes.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.467672 badkeys-0.0.9/
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.458672 badkeys-0.0.9/.github/
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.459672 badkeys-0.0.9/.github/workflows/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      574 2024-04-29 13:22:03.000000 badkeys-0.0.9/.github/workflows/codeql.yml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      924 2024-04-29 13:22:03.000000 badkeys-0.0.9/.github/workflows/runci.yml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       58 2024-04-29 13:22:03.000000 badkeys-0.0.9/.gitignore
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1138 2024-04-29 13:22:03.000000 badkeys-0.0.9/LICENSE
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3690 2024-05-03 08:23:31.466672 badkeys-0.0.9/PKG-INFO
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2565 2024-04-29 13:22:03.000000 badkeys-0.0.9/README.md
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.460672 badkeys-0.0.9/badkeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      384 2024-05-03 08:19:33.000000 badkeys-0.0.9/badkeys/__init__.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.461672 badkeys-0.0.9/badkeys/allkeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      105 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/allkeys/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3324 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/allkeys/block.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     8266 2024-04-29 16:10:01.000000 badkeys-0.0.9/badkeys/checks.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1093 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/dkim.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.462672 badkeys-0.0.9/badkeys/keydata/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)   255328 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/primes1024.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)    78961 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/primes2048.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      770 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/primes4096.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)    11449 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/primes512.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      434 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/keydata/primes768.dat
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.463672 badkeys-0.0.9/badkeys/rsakeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      358 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      587 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/fermat.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      211 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/pattern.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1046 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/roca.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      192 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/rsainvalid.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      720 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/sharedprimes.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      599 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/smallfactors.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      533 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/rsakeys/xzbackdoor.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     8638 2024-05-02 18:58:05.000000 badkeys-0.0.9/badkeys/runcli.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1222 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/scanssh.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      380 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/scantls.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2573 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys/update.py
+-rwxr-xr-x   0 hanno     (1000) hanno     (1000)       68 2024-04-29 13:22:03.000000 badkeys-0.0.9/badkeys-cli
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.466672 badkeys-0.0.9/badkeys.egg-info/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3690 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/PKG-INFO
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1622 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        1 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       50 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/entry_points.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       85 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/requires.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        8 2024-05-03 08:23:31.000000 badkeys-0.0.9/badkeys.egg-info/top_level.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1230 2024-05-03 08:14:06.000000 badkeys-0.0.9/pyproject.toml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       19 2024-04-29 13:22:03.000000 badkeys-0.0.9/requirements.txt
+-rwxr-xr-x   0 hanno     (1000) hanno     (1000)      363 2024-04-29 13:22:03.000000 badkeys-0.0.9/runci.sh
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       38 2024-05-03 08:23:31.467672 badkeys-0.0.9/setup.cfg
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.464672 badkeys-0.0.9/tests/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/__init__.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-05-03 08:23:31.466672 badkeys-0.0.9/tests/data/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      640 2024-04-29 13:24:54.000000 badkeys-0.0.9/tests/data/dsa-sshpub-ietf-example.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      206 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/ec-p256-rfc-example.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      149 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/ed25519-rfc-example.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      531 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-debianweak.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      453 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-e1.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      513 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-fermat-hexmodulus.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      502 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-fermat-pkcs1.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      498 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-fermat-pkcs8.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1153 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-fermat.crt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      935 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-fermat.csr
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      457 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-nprime.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      464 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-ok.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-pattern.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      426 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-roca.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      508 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-sharedprimes.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      491 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/rsa-smallfactors.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      146 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/data/x448-ok.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1802 2024-04-29 13:25:23.000000 badkeys-0.0.9/tests/test_blocklist.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      620 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_failures.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2090 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_fermat.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      560 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_pattern.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      545 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_roca.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      651 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_rsainvalid.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_sharedprimes.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      591 2024-04-29 13:22:03.000000 badkeys-0.0.9/tests/test_smallprimes.py
```

### Comparing `badkeys-0.0.8/.github/workflows/codeql.yml` & `badkeys-0.0.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/.github/workflows/runci.yml` & `badkeys-0.0.9/.github/workflows/runci.yml`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/LICENSE` & `badkeys-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/PKG-INFO` & `badkeys-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badkeys
-Version: 0.0.8
+Version: 0.0.9
 Summary: Check cryptographic keys for known weaknesses
 Author: Hanno Böck
 License: MIT
 Project-URL: Homepage, https://badkeys.info/
 Project-URL: Source, https://github.com/badkeys/badkeys
 Project-URL: Bug Tracker, https://github.com/badkeys/badkeys/issues
 Keywords: security,cryptography,rsa
@@ -22,14 +22,16 @@
 License-File: LICENSE
 Requires-Dist: gmpy2
 Requires-Dist: cryptography
 Provides-Extra: urllookup
 Requires-Dist: binary-file-search; extra == "urllookup"
 Provides-Extra: ssh
 Requires-Dist: paramiko; extra == "ssh"
+Provides-Extra: dkim
+Requires-Dist: dnspython; extra == "dkim"
 
 # badkeys
 
 Tool and library to check cryptographic public keys for known vulnerabilities
 
 # what?
```

### Comparing `badkeys-0.0.8/README.md` & `badkeys-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/allkeys/block.py` & `badkeys-0.0.9/badkeys/allkeys/block.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/checks.py` & `badkeys-0.0.9/badkeys/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+import warnings
 import cryptography
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import rsa, dsa, ec, dh
 from cryptography.hazmat.primitives.asymmetric import ed25519, x25519
 from cryptography.hazmat.primitives.asymmetric import x448, ed448
 from cryptography.hazmat.primitives import serialization
 
@@ -55,14 +56,22 @@
     "blocklist": {
         "type": "all",
         "function": blocklist,
         "desc": "Blocklists of compromised keys",
     },
 }
 
+# cryptography warns about SSH DSA keys being deprecated.
+# For now, disable the warnings. Needs a better long-term solution.
+warnings.filterwarnings(
+    "ignore",
+    category=cryptography.utils.CryptographyDeprecationWarning,
+    module="badkeys.checks",
+)
+
 
 def _checkkey(key, checks):
     r = {}
     if isinstance(key, rsa.RSAPublicKey):
         r["type"] = "rsa"
         r["n"] = key.public_numbers().n
         r["e"] = key.public_numbers().e
```

### Comparing `badkeys-0.0.8/badkeys/keydata/primes1024.dat` & `badkeys-0.0.9/badkeys/keydata/primes1024.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/keydata/primes2048.dat` & `badkeys-0.0.9/badkeys/keydata/primes2048.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/keydata/primes4096.dat` & `badkeys-0.0.9/badkeys/keydata/primes4096.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/keydata/primes512.dat` & `badkeys-0.0.9/badkeys/keydata/primes512.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/rsakeys/fermat.py` & `badkeys-0.0.9/badkeys/rsakeys/fermat.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/rsakeys/roca.py` & `badkeys-0.0.9/badkeys/rsakeys/roca.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/rsakeys/sharedprimes.py` & `badkeys-0.0.9/badkeys/rsakeys/sharedprimes.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/rsakeys/smallfactors.py` & `badkeys-0.0.9/badkeys/rsakeys/smallfactors.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/rsakeys/xzbackdoor.py` & `badkeys-0.0.9/badkeys/rsakeys/xzbackdoor.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/runcli.py` & `badkeys-0.0.9/badkeys/runcli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import sys
 import argparse
 import signal
 import re
 import json
 
 from .checks import detectandcheck, allchecks
-from .checks import checkrsa, checkcrt, checksshpubkey
+from .checks import checkrsa, checkcrt, checksshpubkey, checkpubkey
 from .allkeys import urllookup, loadextrabl
 from .scanssh import scanssh
 from .scantls import scantls
 from .update import update_bl
+from .dkim import parsedkim
+from . import __version__
 
 MAXINPUTSIZE = 10000
 
 count = 0
 
 PRECRT = "-----BEGIN CERTIFICATE-----\n"
 POSTCRT = "\n-----END CERTIFICATE-----\n"
@@ -79,14 +81,20 @@
     )
     ap.add_argument(
         "--crt-lines", action="store_true", help="Input file is list of base64 certs"
     )
     ap.add_argument(
         "--ssh-lines", action="store_true", help="Input file is list of ssh public keys"
     )
+    ap.add_argument("--dkim", action="store_true", help="Scan DKIM records (in files)")
+    ap.add_argument(
+        "--dkim-dns",
+        action="store_true",
+        help="Scan DKIM DNS record (hostnames instead of files)",
+    )
     ap.add_argument("-a", "--all", action="store_true", help="Show all keys")
     ap.add_argument("-v", "--verbose", action="store_true", help="Verbose output")
     ap.add_argument("-j", "--json", action="store_true", help="JSON output")
     ap.add_argument(
         "-u", "--url", action="store_true", help="Show private key URL if possible"
     )
     ap.add_argument("--update-bl", action="store_true", help="Update blocklist")
@@ -112,24 +120,27 @@
     ap.add_argument(
         "-s",
         "--ssh",
         action="store_true",
         help="Scan SSH (pass hostnames or IPs instead of files)",
     )
     ap.add_argument("--ssh-ports", default="22", help="SSH ports (comma-separated)")
+    ap.add_argument("--version", action="version", version=__version__)
     args = ap.parse_args()
 
     if (
         (args.moduli and args.crt_lines)
         or (args.moduli and args.ssh_lines)
         or (args.ssh_lines and args.crt_lines)
     ):
         sys.exit("Multiple input format parameters cannot be combined.")
 
-    if (args.moduli or args.crt_lines or args.ssh_lines) and (args.tls or args.ssh):
+    if (args.moduli or args.crt_lines or args.ssh_lines) and (
+        args.tls or args.ssh or args.dkim_dns
+    ):
         sys.exit("Scan modes and input file modes cannot be combined.")
 
     if args.update_bl_and_urls:
         update_bl(lookup=True)
         sys.exit()
     if args.update_bl:
         update_bl()
@@ -169,15 +180,33 @@
         ports = [int(p) for p in args.ssh_ports.split(",")]
         for host in args.infiles:
             for port in ports:
                 keys = scanssh(host, port)
                 for k in keys:
                     _printresults(k, f"ssh:{host}:{port}", args)
 
-    if args.ssh or args.tls:
+    if args.dkim_dns:
+        try:
+            import dns.resolver
+        except ModuleNotFoundError:
+            sys.stderr.write("Error: DKIM DNS record scanning needs dnspython\n")
+            sys.exit(1)
+        for host in args.infiles:
+            try:
+                records = dns.resolver.resolve(host, "TXT").response
+            except dns.resolver.NXDOMAIN:
+                continue
+            for record in records.answer[-1]:
+                dk = b"".join(record.strings).decode()
+                key = parsedkim(dk)
+                if key:
+                    r = checkpubkey(key, checks=userchecks)
+                    _printresults(r, host, args)
+
+    if args.ssh or args.tls or args.dkim_dns:
         sys.exit(1)
 
     for fn in args.infiles:
         if fn == "-":
             f = sys.stdin
         else:
             f = open(fn, errors="replace")
@@ -209,14 +238,24 @@
                 ll = line.rstrip().split(" ", 2)
                 if len(ll) == 3:
                     desc += f" {ll[2]}"
                 r = checksshpubkey(line, checks=userchecks)
                 _printresults(r, desc, args)
                 lno += 1
                 count += 1
+        elif args.dkim:
+            lno = 0
+            for line in f:
+                desc = f"{fn}[{lno}]"
+                key = parsedkim(line)
+                if key:
+                    r = checkpubkey(key, checks=userchecks)
+                    _printresults(r, desc, args)
+                    count += 1
+                lno += 1
         else:
             fcontent = f.read(MAXINPUTSIZE)
             r = detectandcheck(fcontent, checks=userchecks)
             _printresults(r, fn, args)
 
         if fn != "-":
             f.close()
```

### Comparing `badkeys-0.0.8/badkeys/scanssh.py` & `badkeys-0.0.9/badkeys/scanssh.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys/update.py` & `badkeys-0.0.9/badkeys/update.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/badkeys.egg-info/PKG-INFO` & `badkeys-0.0.9/badkeys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badkeys
-Version: 0.0.8
+Version: 0.0.9
 Summary: Check cryptographic keys for known weaknesses
 Author: Hanno Böck
 License: MIT
 Project-URL: Homepage, https://badkeys.info/
 Project-URL: Source, https://github.com/badkeys/badkeys
 Project-URL: Bug Tracker, https://github.com/badkeys/badkeys/issues
 Keywords: security,cryptography,rsa
@@ -22,14 +22,16 @@
 License-File: LICENSE
 Requires-Dist: gmpy2
 Requires-Dist: cryptography
 Provides-Extra: urllookup
 Requires-Dist: binary-file-search; extra == "urllookup"
 Provides-Extra: ssh
 Requires-Dist: paramiko; extra == "ssh"
+Provides-Extra: dkim
+Requires-Dist: dnspython; extra == "dkim"
 
 # badkeys
 
 Tool and library to check cryptographic public keys for known vulnerabilities
 
 # what?
```

### Comparing `badkeys-0.0.8/badkeys.egg-info/SOURCES.txt` & `badkeys-0.0.9/badkeys.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pyproject.toml
 requirements.txt
 runci.sh
 .github/workflows/codeql.yml
 .github/workflows/runci.yml
 badkeys/__init__.py
 badkeys/checks.py
+badkeys/dkim.py
 badkeys/runcli.py
 badkeys/scanssh.py
 badkeys/scantls.py
 badkeys/update.py
 badkeys.egg-info/PKG-INFO
 badkeys.egg-info/SOURCES.txt
 badkeys.egg-info/dependency_links.txt
@@ -32,23 +33,23 @@
 badkeys/rsakeys/pattern.py
 badkeys/rsakeys/roca.py
 badkeys/rsakeys/rsainvalid.py
 badkeys/rsakeys/sharedprimes.py
 badkeys/rsakeys/smallfactors.py
 badkeys/rsakeys/xzbackdoor.py
 tests/__init__.py
-tests/test_ecbl.py
+tests/test_blocklist.py
 tests/test_failures.py
 tests/test_fermat.py
 tests/test_pattern.py
 tests/test_roca.py
-tests/test_rsabl.py
 tests/test_rsainvalid.py
 tests/test_sharedprimes.py
 tests/test_smallprimes.py
+tests/data/dsa-sshpub-ietf-example.key
 tests/data/ec-p256-rfc-example.key
 tests/data/ed25519-rfc-example.key
 tests/data/rsa-debianweak.key
 tests/data/rsa-e1.key
 tests/data/rsa-fermat-hexmodulus.txt
 tests/data/rsa-fermat-pkcs1.key
 tests/data/rsa-fermat-pkcs8.key
```

### Comparing `badkeys-0.0.8/pyproject.toml` & `badkeys-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "badkeys"
-version = "0.0.8"
 description = "Check cryptographic keys for known weaknesses"
 readme = "README.md"
 authors = [{name = "Hanno Böck"}]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3",
@@ -18,14 +17,20 @@
 license = {text = "MIT"}
 keywords = ["security", "cryptography", "rsa"]
 requires-python = ">=3.9"
 dependencies = [
   "gmpy2",
   "cryptography"
 ]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "badkeys.__version__"}
+
+[tool.setuptools_scm]
 
 [project.urls]
 "Homepage" = "https://badkeys.info/"
 "Source" = "https://github.com/badkeys/badkeys"
 "Bug Tracker" = "https://github.com/badkeys/badkeys/issues"
 
 [build-system]
@@ -34,7 +39,8 @@
 
 [project.scripts]
 badkeys = "badkeys.runcli:runcli"
 
 [project.optional-dependencies]
 urllookup = ["binary-file-search"]
 ssh = ["paramiko"]
+dkim = ["dnspython"]
```

### Comparing `badkeys-0.0.8/tests/data/rsa-debianweak.key` & `badkeys-0.0.9/tests/data/rsa-debianweak.key`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/data/rsa-fermat-hexmodulus.txt` & `badkeys-0.0.9/tests/data/rsa-fermat-hexmodulus.txt`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/data/rsa-fermat.crt` & `badkeys-0.0.9/tests/data/rsa-fermat.crt`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/data/rsa-fermat.csr` & `badkeys-0.0.9/tests/data/rsa-fermat.csr`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/data/rsa-pattern.key` & `badkeys-0.0.9/tests/data/rsa-pattern.key`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_ecbl.py` & `badkeys-0.0.9/tests/test_blocklist.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,27 @@
 import os
 
 import badkeys
 
 TDPATH = f"{os.path.dirname(__file__)}/data/"
 
 
-class TestEcbl(unittest.TestCase):
+class TestBlocklist(unittest.TestCase):
+
+    @unittest.skipUnless(os.environ.get("RUNBLTESTS"), "Not running blocklist tests")
+    def test_rsabl(self):
+        with open(f"{TDPATH}rsa-debianweak.key") as f:
+            key = f.read()
+        r = badkeys.checkpubkey(key, checks=["blocklist"])
+        self.assertTrue("blocklist" in r["results"])
+        with open(f"{TDPATH}rsa-ok.key") as f:
+            key = f.read()
+        r = badkeys.checkpubkey(key, checks=["blocklist"])
+        self.assertFalse(r["results"])
+
     @unittest.skipUnless(os.environ.get("RUNBLTESTS"), "Not running blocklist tests")
     def test_ecbl(self):
         with open(f"{TDPATH}ec-p256-rfc-example.key") as f:
             key = f.read()
         r = badkeys.checkpubkey(key, checks=["blocklist"])
         self.assertTrue("blocklist" in r["results"])
         with open(f"{TDPATH}ed25519-rfc-example.key") as f:
@@ -18,10 +30,20 @@
         r = badkeys.checkpubkey(key, checks=["blocklist"])
         self.assertTrue("blocklist" in r["results"])
         with open(f"{TDPATH}x448-ok.key") as f:
             key = f.read()
         r = badkeys.checkpubkey(key, checks=["blocklist"])
         self.assertFalse(r["results"])
 
+    # Testing key in SSH DSA pubkey format.
+    # Python cryptography plans to deprecate this format,
+    # we will need to find a solution.
+    @unittest.skipUnless(os.environ.get("RUNBLTESTS"), "Not running blocklist tests")
+    def test_dsabl(self):
+        with open(f"{TDPATH}dsa-sshpub-ietf-example.key") as f:
+            key = f.read()
+        r = badkeys.checksshpubkey(key, checks=["blocklist"])
+        self.assertTrue("blocklist" in r["results"])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `badkeys-0.0.8/tests/test_failures.py` & `badkeys-0.0.9/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_fermat.py` & `badkeys-0.0.9/tests/test_fermat.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_pattern.py` & `badkeys-0.0.9/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_roca.py` & `badkeys-0.0.9/tests/test_roca.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_rsabl.py` & `badkeys-0.0.9/tests/test_rsainvalid.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import os
 
 import badkeys
 
 TDPATH = f"{os.path.dirname(__file__)}/data/"
 
 
-class TestRsabl(unittest.TestCase):
-    @unittest.skipUnless(os.environ.get("RUNBLTESTS"), "Not running blocklist tests")
-    def test_rsabl(self):
-        with open(f"{TDPATH}rsa-debianweak.key") as f:
+class TestRSAInvalid(unittest.TestCase):
+    def test_rsainvalid(self):
+        with open(f"{TDPATH}rsa-e1.key") as f:
             key = f.read()
-        r = badkeys.checkpubkey(key, checks=["blocklist"])
-        self.assertTrue("blocklist" in r["results"])
+        r = badkeys.checkpubkey(key, checks=["rsainvalid"])
+        self.assertTrue("rsainvalid" in r["results"])
+        self.assertEqual("invalid_e", r["results"]["rsainvalid"]["subtest"])
+
         with open(f"{TDPATH}rsa-ok.key") as f:
             key = f.read()
-        r = badkeys.checkpubkey(key, checks=["blocklist"])
+        r = badkeys.checkpubkey(key, checks=["rsainvalid"])
         self.assertFalse(r["results"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `badkeys-0.0.8/tests/test_sharedprimes.py` & `badkeys-0.0.9/tests/test_sharedprimes.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.8/tests/test_smallprimes.py` & `badkeys-0.0.9/tests/test_smallprimes.py`

 * *Files identical despite different names*

