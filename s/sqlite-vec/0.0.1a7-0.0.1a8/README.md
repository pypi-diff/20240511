# Comparing `tmp/sqlite_vec-0.0.1a7-py3-none-win_amd64.whl.zip` & `tmp/sqlite_vec-0.0.1a8-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 149409 bytes, number of entries: 6
--rw-r--r--  4.6 unx      314 b- stor 24-May-11 04:34 sqlite_vec/__init__.py
--rw-r--r--  4.6 unx   147453 b- stor 24-May-11 04:34 sqlite_vec/vec0.dll
--rw-r--r--  4.6 unx      199 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/METADATA
--rw-r--r--  4.6 unx      102 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/WHEEL
--rw-r--r--  4.6 unx       11 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/top_level.txt
--rw-r--r--  4.6 unx      474 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/RECORD
+-rw-r--r--  4.6 unx      314 b- stor 24-May-11 05:53 sqlite_vec/__init__.py
+-rw-r--r--  4.6 unx   147453 b- stor 24-May-11 05:53 sqlite_vec/vec0.dll
+-rw-r--r--  4.6 unx      199 b- stor 24-May-11 05:53 sqlite_vec-0.0.1a8.dist-info/METADATA
+-rw-r--r--  4.6 unx      102 b- stor 24-May-11 05:53 sqlite_vec-0.0.1a8.dist-info/WHEEL
+-rw-r--r--  4.6 unx       11 b- stor 24-May-11 05:53 sqlite_vec-0.0.1a8.dist-info/top_level.txt
+-rw-r--r--  4.6 unx      474 b- stor 24-May-11 05:53 sqlite_vec-0.0.1a8.dist-info/RECORD
 6 files, 148553 bytes uncompressed, 148553 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sqlite_vec/__init__.py
 Comment: 
 
 Filename: sqlite_vec/vec0.dll
 Comment: 
 
-Filename: sqlite_vec-0.0.1a7.dist-info/METADATA
+Filename: sqlite_vec-0.0.1a8.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_vec-0.0.1a7.dist-info/WHEEL
+Filename: sqlite_vec-0.0.1a8.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_vec-0.0.1a7.dist-info/top_level.txt
+Filename: sqlite_vec-0.0.1a8.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_vec-0.0.1a7.dist-info/RECORD
+Filename: sqlite_vec-0.0.1a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_vec/__init__.py

```diff
@@ -1,12 +1,12 @@
 
 import os
 import sqlite3
 
-__version__ = "0.0.1a7"
+__version__ = "0.0.1a8"
 __version_info__ = tuple(__version__.split("."))
 
 def loadable_path():
   loadable_path = os.path.join(os.path.dirname(__file__), "vec0")
   return os.path.normpath(loadable_path)
 
 def load(conn: sqlite3.Connection)  -> None:
```

## sqlite_vec/vec0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Sat May 11 04:33:51 2024
+Time/Date		Sat May 11 05:52:29 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
 SizeOfCode		0000000000013000
 SizeOfInitializedData	0000000000018400
 SizeOfUninitializedData	0000000000001600
 AddressOfEntryPoint	0000000000001330
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00028000
 SizeOfHeaders		00000600
-CheckSum		00032d2e
+CheckSum		000317e1
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -147,15 +147,15 @@
  0001d050	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x6b49c000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		663ef52f
+Time/Date stamp 		663f079d
 Major/Minor 			0/0
 Name 				000000000001c046 vec0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000003
 	[Name Pointer/Ordinal] Table	00000003
 Table Addresses
@@ -24954,54 +24954,52 @@
     6b496970:	jbe    6b4969d7 <aMod.9650+0x97>
     6b496972:	movsxd 0x76(%rdi),%ebx
     6b496975:	gs jb  6b4969eb <aMod.9650+0xab>
     6b496978:	imul   $0x2e307600,0x6e(%rdi),%ebp
     6b49697f:	xor    %ch,(%rsi)
     6b496981:	xor    %ebp,0x68706c61(%rip)        # d3b9d5e8 <.debug_str+0x686f65e8>
     6b496987:	(bad)
-    6b496988:	cs (bad)
-    6b49698a:	add    %dh,0x65(%rsi)
+    6b496988:	cs cmp %al,(%rax)
+    6b49698b:	jbe    6b4969f2 <aMod.9650+0xb2>
     6b49698d:	movsxd 0x64(%rdi),%ebx
     6b496990:	(bad)
     6b496996:	add    %al,(%rax)
     6b496998:	push   %rsi
     6b496999:	gs jb  6b496a0f <aMod.9650+0xcf>
     6b49699c:	imul   $0x3076203a,0x6e(%rdi),%ebp
     6b4969a3:	cs xor %ch,(%rsi)
     6b4969a6:	xor    %ebp,0x68706c61(%rip)        # d3b9d60d <.debug_str+0x686f660d>
     6b4969ac:	(bad)
-    6b4969ad:	cs (bad)
-    6b4969af:	or     0x74(%rcx,%riz,2),%al
-    6b4969b3:	cmp    %gs:(%rax),%ah
+    6b4969ad:	cs cmp %cl,(%rdx)
+    6b4969b0:	rex.R (bad)
+    6b4969b2:	je     6b496a19 <aMod.9650+0xd9>
+    6b4969b4:	cmp    (%rax),%ah
     6b4969b6:	xor    (%rax),%dh
     6b4969b8:	xor    0x312d3530(,%rbp,1),%dh
-    6b4969bf:	xor    %edx,0x34(%rax,%rsi,1)
-    6b4969c3:	cmp    (%rbx),%dh
-    6b4969c5:	xor    (%rdx),%edi
-    6b4969c7:	xor    $0x35,%al
+    6b4969bf:	xor    %edx,0x35(%rax,%rsi,1)
+    6b4969c3:	cmp    0x31323a32(%rip),%dh        # 9c7ba3fb <.debug_str+0x313133fb>
     6b4969c9:	pop    %rdx
     6b4969ca:	sub    (%rax),%esi
     6b4969cc:	xor    %dh,(%rax)
     6b4969ce:	xor    %cl,(%rdx)
     6b4969d0:	rex.XB outsl %ds:(%rsi),(%dx)
     6b4969d2:	insl   (%dx),%es:(%rdi)
     6b4969d3:	insl   (%dx),%es:(%rdi)
-    6b4969d4:	imul   $0x36376433,0x20(%rdx,%rdi,1),%esi
-    6b4969dc:	xor    0x34(%rsi),%esp
-    6b4969df:	cmp    %edi,(%rcx)
-    6b4969e1:	cmp    %dh,0x65316639(%rip)        # d07ad020 <.debug_str+0x65306020>
-    6b4969e7:	cmp    %edi,(%rcx)
-    6b4969e9:	cmp    %dh,(%rsi,%riz,2)
-    6b4969ec:	xor    (%rcx),%esi
-    6b4969ee:	xor    %esp,0x32(%rbp)
-    6b4969f1:	cmp    %ah,0x66(%rcx)
-    6b4969f4:	cmp    %esi,(%rsi)
-    6b4969f6:	xor    $0x63616464,%eax
-    6b4969fb:	ss xor (%rax),%esi
-    6b4969fe:	data16 or %gs:0x75(%rdx),%al
+    6b4969d4:	imul   $0x35373162,0x20(%rdx,%rdi,1),%esi
+    6b4969dc:	xor    0x33(%rbp),%esp
+    6b4969df:	xor    $0x63376339,%eax
+    6b4969e4:	(bad)
+    6b4969e5:	xor    $0x36,%al
+    6b4969e7:	(bad)
+    6b4969ed:	xor    %fs:0x66(%rbp),%esp
+    6b4969f1:	(bad)
+    6b4969f2:	cmp    %esi,0x63353766(,%rsi,1)
+    6b4969f9:	xor    $0x38356636,%eax
+    6b4969fe:	xor    (%rcx),%bh
+    6b496a00:	or     0x75(%rdx),%al
     6b496a03:	imul   $0x67616c66,0x20(%rsp,%riz,2),%ebp
     6b496a0b:	jae    6b496a47 <aMod.9650+0x107>
     6b496a0d:	and    %ah,(%rax)
     6b496a0f:	add    %dh,0x65(%rsi)
     6b496a12:	movsxd 0x64(%rdi),%ebx
     6b496a15:	imul   $0x65636e61,0x74(%rbx),%esi
     6b496a1c:	pop    %rdi
@@ -28316,17 +28314,18 @@
 	...
 
 Disassembly of section .edata:
 
 000000006b49c000 <.edata>:
     6b49c000:	add    %al,(%rax)
     6b49c002:	add    %al,(%rax)
-    6b49c004:	(bad)
-    6b49c005:	cmc
-    6b49c006:	ds data16 add %al,(%rax)
+    6b49c004:	popf
+    6b49c005:	(bad)
+    6b49c006:	(bad)
+    6b49c007:	data16 add %al,(%rax)
     6b49c00a:	add    %al,(%rax)
     6b49c00c:	rex.RX rolb $0x0,(%rcx)
     6b49c010:	add    %eax,(%rax)
     6b49c012:	add    %al,(%rax)
     6b49c014:	add    (%rax),%eax
     6b49c016:	add    %al,(%rax)
     6b49c018:	add    (%rax),%eax
```

