# Comparing `tmp/sqlite_vec-0.0.1a3-py3-none-win_amd64.whl.zip` & `tmp/sqlite_vec-0.0.1a7-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 149409 bytes, number of entries: 6
--rw-r--r--  4.6 unx      314 b- stor 24-Apr-27 19:55 sqlite_vec/__init__.py
--rw-r--r--  4.6 unx   147453 b- stor 24-Apr-27 19:55 sqlite_vec/vec0.dll
--rw-r--r--  4.6 unx      199 b- stor 24-Apr-27 19:55 sqlite_vec-0.0.1a3.dist-info/METADATA
--rw-r--r--  4.6 unx      102 b- stor 24-Apr-27 19:55 sqlite_vec-0.0.1a3.dist-info/WHEEL
--rw-r--r--  4.6 unx       11 b- stor 24-Apr-27 19:55 sqlite_vec-0.0.1a3.dist-info/top_level.txt
--rw-r--r--  4.6 unx      474 b- stor 24-Apr-27 19:55 sqlite_vec-0.0.1a3.dist-info/RECORD
+-rw-r--r--  4.6 unx      314 b- stor 24-May-11 04:34 sqlite_vec/__init__.py
+-rw-r--r--  4.6 unx   147453 b- stor 24-May-11 04:34 sqlite_vec/vec0.dll
+-rw-r--r--  4.6 unx      199 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/METADATA
+-rw-r--r--  4.6 unx      102 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/WHEEL
+-rw-r--r--  4.6 unx       11 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/top_level.txt
+-rw-r--r--  4.6 unx      474 b- stor 24-May-11 04:34 sqlite_vec-0.0.1a7.dist-info/RECORD
 6 files, 148553 bytes uncompressed, 148553 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sqlite_vec/__init__.py
 Comment: 
 
 Filename: sqlite_vec/vec0.dll
 Comment: 
 
-Filename: sqlite_vec-0.0.1a3.dist-info/METADATA
+Filename: sqlite_vec-0.0.1a7.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_vec-0.0.1a3.dist-info/WHEEL
+Filename: sqlite_vec-0.0.1a7.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_vec-0.0.1a3.dist-info/top_level.txt
+Filename: sqlite_vec-0.0.1a7.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_vec-0.0.1a3.dist-info/RECORD
+Filename: sqlite_vec-0.0.1a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_vec/__init__.py

```diff
@@ -1,12 +1,12 @@
 
 import os
 import sqlite3
 
-__version__ = "0.0.1a3"
+__version__ = "0.0.1a7"
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
 
-Time/Date		Sat Apr 27 19:55:14 2024
+Time/Date		Sat May 11 04:33:51 2024
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
-CheckSum		0002b23b
+CheckSum		00032d2e
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
-Time/Date stamp 		662d5822
+Time/Date stamp 		663ef52f
 Major/Minor 			0/0
 Name 				000000000001c046 vec0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000003
 	[Name Pointer/Ordinal] Table	00000003
 Table Addresses
@@ -3850,29 +3850,29 @@
     6b481771:	push   %rbx
     6b481772:	sub    $0x28,%rsp
     6b481776:	cmpl   $0x1,0x8(%rcx)
     6b48177a:	mov    %rcx,%rbx
     6b48177d:	mov    %rdx,%rsi
     6b481780:	je     6b48179b <vec0Rowid+0x2b>
     6b481782:	lea    0x1387c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b481789:	mov    $0xea4,%r8d
+    6b481789:	mov    $0xeaa,%r8d
     6b48178f:	lea    0x13882(%rip),%rcx        # 6b495018 <.rdata+0x18>
     6b481796:	call   6b48f9e0 <_assert>
     6b48179b:	mov    0x20(%rbx),%rax
     6b48179f:	test   %rax,%rax
     6b4817a2:	je     6b4817b3 <vec0Rowid+0x43>
     6b4817a4:	mov    (%rax),%rax
     6b4817a7:	mov    %rax,(%rsi)
     6b4817aa:	xor    %eax,%eax
     6b4817ac:	add    $0x28,%rsp
     6b4817b0:	pop    %rbx
     6b4817b1:	pop    %rsi
     6b4817b2:	ret
     6b4817b3:	lea    0x1384b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4817ba:	mov    $0xea5,%r8d
+    6b4817ba:	mov    $0xeab,%r8d
     6b4817c0:	lea    0x13881(%rip),%rcx        # 6b495048 <.rdata+0x48>
     6b4817c7:	call   6b48f9e0 <_assert>
     6b4817cc:	mov    0x20(%rbx),%rax
     6b4817d0:	mov    (%rax),%rax
     6b4817d3:	mov    %rax,(%rsi)
     6b4817d6:	xor    %eax,%eax
     6b4817d8:	add    $0x28,%rsp
@@ -3925,28 +3925,28 @@
     6b481860:	ucomiss 0x156a1(%rip),%xmm0        # 6b496f08 <hamdist_table+0x108>
     6b481867:	setnp  %al
     6b48186a:	cmovne %edx,%eax
     6b48186d:	add    $0x20,%rsp
     6b481871:	pop    %rbx
     6b481872:	ret
     6b481873:	lea    0x1378b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48187a:	mov    $0xed2,%r8d
+    6b48187a:	mov    $0xed8,%r8d
     6b481880:	lea    0x137e6(%rip),%rcx        # 6b49506d <.rdata+0x6d>
     6b481887:	call   6b48f9e0 <_assert>
     6b48188c:	mov    0x18(%rbx),%rdx
     6b481890:	jmp    6b481802 <vec0Eof+0x22>
     6b481895:	lea    0x13769(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48189c:	mov    $0xece,%r8d
+    6b48189c:	mov    $0xed4,%r8d
     6b4818a2:	lea    0x137b0(%rip),%rcx        # 6b495059 <.rdata+0x59>
     6b4818a9:	call   6b48f9e0 <_assert>
     6b4818ae:	mov    0x10(%rbx),%rax
     6b4818b2:	jmp    6b481829 <vec0Eof+0x49>
     6b4818b7:	nopw   0x0(%rax,%rax,1)
     6b4818c0:	lea    0x1373e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4818c7:	mov    $0xed8,%r8d
+    6b4818c7:	mov    $0xede,%r8d
     6b4818cd:	lea    0x13774(%rip),%rcx        # 6b495048 <.rdata+0x48>
     6b4818d4:	call   6b48f9e0 <_assert>
     6b4818d9:	mov    0x20(%rbx),%rax
     6b4818dd:	jmp    6b481840 <vec0Eof+0x60>
     6b4818e2:	nopl   0x0(%rax)
     6b4818e6:	cs nopw 0x0(%rax,%rax,1)
 
@@ -4073,15 +4073,15 @@
     6b481a93:	jne    6b481ae5 <vec0BestIndex+0x155>
     6b481a95:	test   %r9d,%r9d
     6b481a98:	jne    6b481ae5 <vec0BestIndex+0x155>
     6b481a9a:	test   %cl,%cl
     6b481a9c:	je     6b481ae0 <vec0BestIndex+0x150>
     6b481a9e:	cmp    $0xffffffff,%edi
     6b481aa1:	je     6b481af0 <vec0BestIndex+0x160>
-    6b481aa3:	mov    $0xcbc,%r8d
+    6b481aa3:	mov    $0xcc2,%r8d
     6b481aa9:	mov    %r9d,0x28(%rsp)
     6b481aae:	movslq %esi,%rdi
     6b481ab1:	lea    0x1354d(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b481ab8:	lea    0x135d5(%rip),%rcx        # 6b495094 <.rdata+0x94>
     6b481abf:	call   6b48f9e0 <_assert>
     6b481ac4:	mov    0x28(%rsp),%r9d
     6b481ac9:	mov    0x2c8(%r12),%eax
@@ -4254,27 +4254,27 @@
     6b481da8:	jne    6b481d5d <vec0Next+0x2d>
     6b481daa:	mov    0x10(%rbx),%rax
     6b481dae:	movb   $0x1,0x8(%rax)
     6b481db2:	xor    %eax,%eax
     6b481db4:	jmp    6b481d5d <vec0Next+0x2d>
     6b481db6:	cs nopw 0x0(%rax,%rax,1)
     6b481dc0:	lea    0x1323e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b481dc7:	mov    $0xebb,%r8d
+    6b481dc7:	mov    $0xec1,%r8d
     6b481dcd:	lea    0x13299(%rip),%rcx        # 6b49506d <.rdata+0x6d>
     6b481dd4:	call   6b48f9e0 <_assert>
     6b481dd9:	mov    0x18(%rbx),%rax
     6b481ddd:	jmp    6b481d56 <vec0Next+0x26>
     6b481de2:	lea    0x1321c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b481de9:	mov    $0xeae,%r8d
+    6b481de9:	mov    $0xeb4,%r8d
     6b481def:	lea    0x13263(%rip),%rcx        # 6b495059 <.rdata+0x59>
     6b481df6:	call   6b48f9e0 <_assert>
     6b481dfb:	mov    0x10(%rbx),%rax
     6b481dff:	jmp    6b481d8b <vec0Next+0x5b>
     6b481e01:	lea    0x131fd(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b481e08:	mov    $0xec0,%r8d
+    6b481e08:	mov    $0xec6,%r8d
     6b481e0e:	lea    0x13233(%rip),%rcx        # 6b495048 <.rdata+0x48>
     6b481e15:	call   6b48f9e0 <_assert>
     6b481e1a:	mov    0x20(%rbx),%rax
     6b481e1e:	jmp    6b481d70 <vec0Next+0x40>
     6b481e23:	mov    $0x2,%ecx
     6b481e28:	call   *0x124f2(%rip)        # 6b494320 <__imp___acrt_iob_func>
     6b481e2e:	lea    0x1334b(%rip),%r8        # 6b495180 <.rdata+0x180>
@@ -5052,15 +5052,15 @@
     6b4828d8:	xor    %eax,%eax
     6b4828da:	add    $0x20,%rsp
     6b4828de:	pop    %rbx
     6b4828df:	pop    %rsi
     6b4828e0:	pop    %rdi
     6b4828e1:	ret
     6b4828e2:	lea    0x1271c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4828e9:	mov    $0xaff,%r8d
+    6b4828e9:	mov    $0xb05,%r8d
     6b4828ef:	lea    0x12988(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b4828f6:	call   6b48f9e0 <_assert>
     6b4828fb:	jmp    6b4827f0 <vec0Close+0x30>
 
 000000006b482900 <fvec_from_value>:
     6b482900:	push   %r15
     6b482902:	push   %r14
@@ -8713,41 +8713,41 @@
     6b486440:	mov    %r12,%r8
     6b486443:	mov    %rbp,%rdx
     6b486446:	mov    %rbx,%rcx
     6b486449:	call   6b485f60 <npy_token_next>
     6b48644e:	cmp    $0x2,%eax
     6b486451:	je     6b486700 <parse_npy_header+0x310>
     6b486457:	lea    0xeba7(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48645e:	mov    $0x787,%r8d
+    6b48645e:	mov    $0x78a,%r8d
     6b486464:	lea    0xf59d(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b48646b:	call   6b48f9e0 <_assert>
     6b486470:	mov    0x20(%rsp),%eax
     6b486474:	cmp    $0x5,%eax
     6b486477:	je     6b486712 <parse_npy_header+0x322>
     6b48647d:	cmp    $0x8,%eax
     6b486480:	je     6b48649b <parse_npy_header+0xab>
     6b486482:	lea    0xeb7c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486489:	mov    $0x78b,%r8d
+    6b486489:	mov    $0x78e,%r8d
     6b48648f:	lea    0xf3a2(%rip),%rcx        # 6b495838 <.rdata+0x838>
     6b486496:	call   6b48f9e0 <_assert>
     6b48649b:	mov    %r12,%r8
     6b48649e:	mov    %rbp,%rdx
     6b4864a1:	mov    %rbx,%rcx
     6b4864a4:	mov    0x28(%rsp),%r13
     6b4864a9:	call   6b485f60 <npy_token_next>
     6b4864ae:	cmp    $0x2,%eax
     6b4864b1:	je     6b486725 <parse_npy_header+0x335>
     6b4864b7:	lea    0xeb47(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4864be:	mov    $0x791,%r8d
+    6b4864be:	mov    $0x794,%r8d
     6b4864c4:	lea    0xf53d(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b4864cb:	call   6b48f9e0 <_assert>
     6b4864d0:	cmpl   $0x6,0x20(%rsp)
     6b4864d5:	je     6b4864f0 <parse_npy_header+0x100>
     6b4864d7:	lea    0xeb27(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4864de:	mov    $0x792,%r8d
+    6b4864de:	mov    $0x795,%r8d
     6b4864e4:	lea    0xf37d(%rip),%rcx        # 6b495868 <.rdata+0x868>
     6b4864eb:	call   6b48f9e0 <_assert>
     6b4864f0:	mov    $0x7,%ecx
     6b4864f5:	mov    %r13,%rsi
     6b4864f8:	mov    %r14,%rdi
     6b4864fb:	repz cmpsb %es:(%rdi),%ds:(%rsi)
     6b4864fd:	seta   %al
@@ -8773,68 +8773,68 @@
     6b486546:	mov    %r12,%r8
     6b486549:	mov    %rbp,%rdx
     6b48654c:	mov    %rbx,%rcx
     6b48654f:	call   6b485f60 <npy_token_next>
     6b486554:	cmp    $0x2,%eax
     6b486557:	je     6b4868e0 <parse_npy_header+0x4f0>
     6b48655d:	lea    0xeaa1(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486564:	mov    $0x7a5,%r8d
+    6b486564:	mov    $0x7a8,%r8d
     6b48656a:	lea    0xf497(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b486571:	call   6b48f9e0 <_assert>
     6b486576:	cmpl   $0x2,0x20(%rsp)
     6b48657b:	je     6b486596 <parse_npy_header+0x1a6>
     6b48657d:	lea    0xea81(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486584:	mov    $0x7a6,%r8d
+    6b486584:	mov    $0x7a9,%r8d
     6b48658a:	lea    0xf397(%rip),%rcx        # 6b495928 <.rdata+0x928>
     6b486591:	call   6b48f9e0 <_assert>
     6b486596:	mov    %r12,%r8
     6b486599:	mov    %rbp,%rdx
     6b48659c:	mov    %rbx,%rcx
     6b48659f:	call   6b485f60 <npy_token_next>
     6b4865a4:	cmp    $0x2,%eax
     6b4865a7:	je     6b4868d0 <parse_npy_header+0x4e0>
     6b4865ad:	lea    0xea51(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4865b4:	mov    $0x7a9,%r8d
+    6b4865b4:	mov    $0x7ac,%r8d
     6b4865ba:	lea    0xf447(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b4865c1:	call   6b48f9e0 <_assert>
     6b4865c6:	cmpl   $0x1,0x20(%rsp)
     6b4865cb:	je     6b4865e6 <parse_npy_header+0x1f6>
     6b4865cd:	lea    0xea31(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4865d4:	mov    $0x7aa,%r8d
+    6b4865d4:	mov    $0x7ad,%r8d
     6b4865da:	lea    0xf377(%rip),%rcx        # 6b495958 <.rdata+0x958>
     6b4865e1:	call   6b48f9e0 <_assert>
     6b4865e6:	mov    0x28(%rsp),%rcx
     6b4865eb:	xor    %edx,%edx
     6b4865ed:	mov    $0xa,%r8d
     6b4865f3:	call   6b493930 <strtol>
     6b4865f8:	mov    %r12,%r8
     6b4865fb:	mov    %rbp,%rdx
     6b4865fe:	mov    %rbx,%rcx
     6b486601:	movslq %eax,%r13
     6b486604:	call   6b485f60 <npy_token_next>
     6b486609:	cmp    $0x2,%eax
     6b48660c:	je     6b4868c0 <parse_npy_header+0x4d0>
     6b486612:	lea    0xe9ec(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486619:	mov    $0x7ae,%r8d
+    6b486619:	mov    $0x7b1,%r8d
     6b48661f:	lea    0xf3e2(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b486626:	call   6b48f9e0 <_assert>
     6b48662b:	cmpl   $0x7,0x20(%rsp)
     6b486630:	je     6b48664b <parse_npy_header+0x25b>
     6b486632:	lea    0xe9cc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486639:	mov    $0x7af,%r8d
+    6b486639:	mov    $0x7b2,%r8d
     6b48663f:	lea    0xf342(%rip),%rcx        # 6b495988 <.rdata+0x988>
     6b486646:	call   6b48f9e0 <_assert>
     6b48664b:	mov    %r12,%r8
     6b48664e:	mov    %rbp,%rdx
     6b486651:	mov    %rbx,%rcx
     6b486654:	call   6b485f60 <npy_token_next>
     6b486659:	cmp    $0x2,%eax
     6b48665c:	je     6b486823 <parse_npy_header+0x433>
     6b486662:	lea    0xe99c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486669:	mov    $0x7b2,%r8d
+    6b486669:	mov    $0x7b5,%r8d
     6b48666f:	lea    0xf392(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b486676:	call   6b48f9e0 <_assert>
     6b48667b:	mov    0x20(%rsp),%eax
     6b48667f:	cmp    $0x1,%eax
     6b486682:	je     6b486835 <parse_npy_header+0x445>
     6b486688:	cmp    $0x3,%eax
     6b48668b:	jne    6b486985 <parse_npy_header+0x595>
@@ -8845,21 +8845,21 @@
     6b4866ab:	mov    %r12,%r8
     6b4866ae:	mov    %rbp,%rdx
     6b4866b1:	mov    %rbx,%rcx
     6b4866b4:	call   6b485f60 <npy_token_next>
     6b4866b9:	cmp    $0x2,%eax
     6b4866bc:	je     6b486730 <parse_npy_header+0x340>
     6b4866be:	lea    0xe940(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4866c5:	mov    $0x7c4,%r8d
+    6b4866c5:	mov    $0x7c7,%r8d
     6b4866cb:	lea    0xf336(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b4866d2:	call   6b48f9e0 <_assert>
     6b4866d7:	cmpl   $0x7,0x20(%rsp)
     6b4866dc:	je     6b486440 <parse_npy_header+0x50>
     6b4866e2:	lea    0xe91c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4866e9:	mov    $0x7c5,%r8d
+    6b4866e9:	mov    $0x7c8,%r8d
     6b4866ef:	lea    0xf292(%rip),%rcx        # 6b495988 <.rdata+0x988>
     6b4866f6:	call   6b48f9e0 <_assert>
     6b4866fb:	jmp    6b486440 <parse_npy_header+0x50>
     6b486700:	mov    0x20(%rsp),%eax
     6b486704:	mov    0x30(%rsp),%rbx
     6b486709:	cmp    $0x5,%eax
     6b48670c:	jne    6b48647d <parse_npy_header+0x8d>
@@ -8883,21 +8883,21 @@
     6b486740:	mov    %r12,%r8
     6b486743:	mov    %rbp,%rdx
     6b486746:	mov    %rbx,%rcx
     6b486749:	call   6b485f60 <npy_token_next>
     6b48674e:	cmp    $0x2,%eax
     6b486751:	je     6b4868f0 <parse_npy_header+0x500>
     6b486757:	lea    0xe8a7(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48675e:	mov    $0x797,%r8d
+    6b48675e:	mov    $0x79a,%r8d
     6b486764:	lea    0xf29d(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b48676b:	call   6b48f9e0 <_assert>
     6b486770:	cmpl   $0x8,0x20(%rsp)
     6b486775:	je     6b486790 <parse_npy_header+0x3a0>
     6b486777:	lea    0xe887(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48677e:	mov    $0x798,%r8d
+    6b48677e:	mov    $0x79b,%r8d
     6b486784:	lea    0xf0ad(%rip),%rcx        # 6b495838 <.rdata+0x838>
     6b48678b:	call   6b48f9e0 <_assert>
     6b486790:	mov    0x28(%rsp),%rsi
     6b486795:	mov    $0x5,%ecx
     6b48679a:	lea    0xf0f8(%rip),%rdi        # 6b495899 <.rdata+0x899>
     6b4867a1:	repz cmpsb %es:(%rdi),%ds:(%rsi)
     6b4867a3:	seta   %al
@@ -8910,21 +8910,21 @@
     6b4867c0:	mov    %r12,%r8
     6b4867c3:	mov    %rbp,%rdx
     6b4867c6:	mov    %rbx,%rcx
     6b4867c9:	call   6b485f60 <npy_token_next>
     6b4867ce:	cmp    $0x2,%eax
     6b4867d1:	je     6b486920 <parse_npy_header+0x530>
     6b4867d7:	lea    0xe827(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4867de:	mov    $0x79e,%r8d
+    6b4867de:	mov    $0x7a1,%r8d
     6b4867e4:	lea    0xf21d(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b4867eb:	call   6b48f9e0 <_assert>
     6b4867f0:	cmpl   $0x9,0x20(%rsp)
     6b4867f5:	je     6b486810 <parse_npy_header+0x420>
     6b4867f7:	lea    0xe807(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4867fe:	mov    $0x79f,%r8d
+    6b4867fe:	mov    $0x7a2,%r8d
     6b486804:	lea    0xf0e5(%rip),%rcx        # 6b4958f0 <.rdata+0x8f0>
     6b48680b:	call   6b48f9e0 <_assert>
     6b486810:	mov    0xa8(%rsp),%rax
     6b486818:	movl   $0x0,(%rax)
     6b48681e:	jmp    6b4866ab <parse_npy_header+0x2bb>
     6b486823:	mov    0x20(%rsp),%eax
     6b486827:	mov    0x30(%rsp),%rbx
@@ -8942,21 +8942,21 @@
     6b48685b:	mov    0xb8(%rsp),%rsi
     6b486863:	cltq
     6b486865:	mov    %rax,(%rsi)
     6b486868:	call   6b485f60 <npy_token_next>
     6b48686d:	cmp    $0x2,%eax
     6b486870:	je     6b486930 <parse_npy_header+0x540>
     6b486876:	lea    0xe788(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48687d:	mov    $0x7b7,%r8d
+    6b48687d:	mov    $0x7ba,%r8d
     6b486883:	lea    0xf17e(%rip),%rcx        # 6b495a08 <.rdata+0xa08>
     6b48688a:	call   6b48f9e0 <_assert>
     6b48688f:	cmpl   $0x3,0x20(%rsp)
     6b486894:	je     6b4866ab <parse_npy_header+0x2bb>
     6b48689a:	lea    0xe764(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4868a1:	mov    $0x7b8,%r8d
+    6b4868a1:	mov    $0x7bb,%r8d
     6b4868a7:	lea    0xf10a(%rip),%rcx        # 6b4959b8 <.rdata+0x9b8>
     6b4868ae:	call   6b48f9e0 <_assert>
     6b4868b3:	jmp    6b4866ab <parse_npy_header+0x2bb>
     6b4868b8:	nopl   0x0(%rax,%rax,1)
     6b4868c0:	mov    0x30(%rsp),%rbx
     6b4868c5:	jmp    6b48662b <parse_npy_header+0x23b>
     6b4868ca:	nopw   0x0(%rax,%rax,1)
@@ -8966,15 +8966,15 @@
     6b4868e0:	mov    0x30(%rsp),%rbx
     6b4868e5:	jmp    6b486576 <parse_npy_header+0x186>
     6b4868ea:	nopw   0x0(%rax,%rax,1)
     6b4868f0:	mov    0x30(%rsp),%rbx
     6b4868f5:	jmp    6b486770 <parse_npy_header+0x380>
     6b4868fa:	nopw   0x0(%rax,%rax,1)
     6b486900:	lea    0xe6fe(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486907:	mov    $0x799,%r8d
+    6b486907:	mov    $0x79c,%r8d
     6b48690d:	lea    0xef8c(%rip),%rcx        # 6b4958a0 <.rdata+0x8a0>
     6b486914:	call   6b48f9e0 <_assert>
     6b486919:	jmp    6b4867b0 <parse_npy_header+0x3c0>
     6b48691e:	xchg   %ax,%ax
     6b486920:	mov    0x30(%rsp),%rbx
     6b486925:	jmp    6b4867f0 <parse_npy_header+0x400>
     6b48692a:	nopw   0x0(%rax,%rax,1)
@@ -9016,45 +9016,45 @@
     6b4869bf:	mov    %rdx,%rsi
     6b4869c2:	mov    %r8,%rdi
     6b4869c5:	mov    %r9,%r13
     6b4869c8:	jbe    6b486b60 <parse_npy+0x1c0>
     6b4869ce:	cmpb   $0x93,(%rbx)
     6b4869d1:	je     6b4869ec <parse_npy+0x4c>
     6b4869d3:	lea    0xe62b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4869da:	mov    $0x7d1,%r8d
+    6b4869da:	mov    $0x7d4,%r8d
     6b4869e0:	lea    0xf03b(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b4869e7:	call   6b48f9e0 <_assert>
     6b4869ec:	cmpb   $0x4e,0x1(%rbx)
     6b4869f0:	je     6b486a0b <parse_npy+0x6b>
     6b4869f2:	lea    0xe60c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4869f9:	mov    $0x7d1,%r8d
+    6b4869f9:	mov    $0x7d4,%r8d
     6b4869ff:	lea    0xf01c(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b486a06:	call   6b48f9e0 <_assert>
     6b486a0b:	cmpb   $0x55,0x2(%rbx)
     6b486a0f:	je     6b486a2a <parse_npy+0x8a>
     6b486a11:	lea    0xe5ed(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486a18:	mov    $0x7d1,%r8d
+    6b486a18:	mov    $0x7d4,%r8d
     6b486a1e:	lea    0xeffd(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b486a25:	call   6b48f9e0 <_assert>
     6b486a2a:	cmpb   $0x4d,0x3(%rbx)
     6b486a2e:	je     6b486a49 <parse_npy+0xa9>
     6b486a30:	lea    0xe5ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486a37:	mov    $0x7d1,%r8d
+    6b486a37:	mov    $0x7d4,%r8d
     6b486a3d:	lea    0xefde(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b486a44:	call   6b48f9e0 <_assert>
     6b486a49:	cmpb   $0x50,0x4(%rbx)
     6b486a4d:	je     6b486a68 <parse_npy+0xc8>
     6b486a4f:	lea    0xe5af(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486a56:	mov    $0x7d1,%r8d
+    6b486a56:	mov    $0x7d4,%r8d
     6b486a5c:	lea    0xefbf(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b486a63:	call   6b48f9e0 <_assert>
     6b486a68:	cmpb   $0x59,0x5(%rbx)
     6b486a6c:	je     6b486a87 <parse_npy+0xe7>
     6b486a6e:	lea    0xe590(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486a75:	mov    $0x7d1,%r8d
+    6b486a75:	mov    $0x7d4,%r8d
     6b486a7b:	lea    0xefa0(%rip),%rcx        # 6b495a22 <.rdata+0xa22>
     6b486a82:	call   6b48f9e0 <_assert>
     6b486a87:	movzwl 0x8(%rbx),%r15d
     6b486a8c:	lea    0xa(%rbx),%r14
     6b486a90:	lea    0xa(%r15),%rbp
     6b486a94:	sub    %rbp,%rsi
     6b486a97:	je     6b486b40 <parse_npy+0x1a0>
@@ -9074,15 +9074,15 @@
     6b486ad7:	sete   %cl
     6b486ada:	imul   (%r12),%rax
     6b486adf:	shl    $0x2,%rcx
     6b486ae3:	imul   %rcx,%rax
     6b486ae7:	cmp    %rsi,%rax
     6b486aea:	je     6b486b05 <parse_npy+0x165>
     6b486aec:	lea    0xe512(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486af3:	mov    $0x7ec,%r8d
+    6b486af3:	mov    $0x7ef,%r8d
     6b486af9:	lea    0xef50(%rip),%rcx        # 6b495a50 <.rdata+0xa50>
     6b486b00:	call   6b48f9e0 <_assert>
     6b486b05:	add    %rbp,%rbx
     6b486b08:	xor    %eax,%eax
     6b486b0a:	mov    %rbx,(%rdi)
     6b486b0d:	add    $0x48,%rsp
     6b486b11:	pop    %rbx
@@ -9092,27 +9092,27 @@
     6b486b15:	pop    %r12
     6b486b17:	pop    %r13
     6b486b19:	pop    %r14
     6b486b1b:	pop    %r15
     6b486b1d:	ret
     6b486b1e:	xchg   %ax,%ax
     6b486b20:	lea    0xe4de(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486b27:	mov    $0x7e5,%r8d
+    6b486b27:	mov    $0x7e8,%r8d
     6b486b2d:	lea    0xe74a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b486b34:	call   6b48f9e0 <_assert>
     6b486b39:	jmp    6b486ac3 <parse_npy+0x123>
     6b486b3b:	nopl   0x0(%rax,%rax,1)
     6b486b40:	lea    0xe4be(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486b47:	mov    $0x7df,%r8d
+    6b486b47:	mov    $0x7e2,%r8d
     6b486b4d:	lea    0xeee8(%rip),%rcx        # 6b495a3c <.rdata+0xa3c>
     6b486b54:	call   6b48f9e0 <_assert>
     6b486b59:	jmp    6b486a9d <parse_npy+0xfd>
     6b486b5e:	xchg   %ax,%ax
     6b486b60:	lea    0xe49e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486b67:	mov    $0x7cf,%r8d
+    6b486b67:	mov    $0x7d2,%r8d
     6b486b6d:	lea    0xee9c(%rip),%rcx        # 6b495a10 <.rdata+0xa10>
     6b486b74:	call   6b48f9e0 <_assert>
     6b486b79:	jmp    6b4869ce <parse_npy+0x2e>
     6b486b7e:	xchg   %ax,%ax
 
 000000006b486b80 <vec_npy_eachFilter>:
     6b486b80:	push   %r13
@@ -9123,15 +9123,15 @@
     6b486b87:	push   %rbx
     6b486b88:	sub    $0x68,%rsp
     6b486b8c:	mov    0xc0(%rsp),%rsi
     6b486b94:	cmp    $0x1,%r9d
     6b486b98:	mov    %rcx,%rbx
     6b486b9b:	je     6b486bb6 <vec_npy_eachFilter+0x36>
     6b486b9d:	lea    0xe461(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486ba4:	mov    $0x885,%r8d
+    6b486ba4:	mov    $0x888,%r8d
     6b486baa:	lea    0xe4cb(%rip),%rcx        # 6b49507c <.rdata+0x7c>
     6b486bb1:	call   6b48f9e0 <_assert>
     6b486bb6:	mov    0x38(%rbx),%rcx
     6b486bba:	test   %rcx,%rcx
     6b486bbd:	je     6b486bcc <vec_npy_eachFilter+0x4c>
     6b486bbf:	call   6b4939c0 <fclose>
     6b486bc4:	movq   $0x0,0x38(%rbx)
@@ -9265,82 +9265,82 @@
     6b486e14:	pop    %rdi
     6b486e15:	pop    %rbp
     6b486e16:	pop    %r12
     6b486e18:	pop    %r13
     6b486e1a:	ret
     6b486e1b:	nopl   0x0(%rax,%rax,1)
     6b486e20:	lea    0xe1de(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486e27:	mov    $0x8d6,%r8d
+    6b486e27:	mov    $0x8d9,%r8d
     6b486e2d:	lea    0xed04(%rip),%rcx        # 6b495b38 <.rdata+0xb38>
     6b486e34:	call   6b48f9e0 <_assert>
     6b486e39:	jmp    6b486df9 <vec_npy_eachFilter+0x279>
     6b486e3b:	nopl   0x0(%rax,%rax,1)
     6b486e40:	lea    0xeca1(%rip),%rcx        # 6b495ae8 <.rdata+0xae8>
-    6b486e47:	mov    $0x8c9,%r8d
+    6b486e47:	mov    $0x8cc,%r8d
     6b486e4d:	lea    0xe1b1(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b486e54:	call   6b48f9e0 <_assert>
     6b486e59:	mov    0x3c(%rsp),%r8d
     6b486e5e:	mov    0x40(%rsp),%rax
     6b486e63:	mov    0x48(%rsp),%rcx
     6b486e68:	jmp    6b486d87 <vec_npy_eachFilter+0x207>
     6b486e6d:	nopl   (%rax)
     6b486e70:	lea    0xe18e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486e77:	mov    $0x8b7,%r8d
+    6b486e77:	mov    $0x8ba,%r8d
     6b486e7d:	lea    0xec38(%rip),%rcx        # 6b495abc <.rdata+0xabc>
     6b486e84:	call   6b48f9e0 <_assert>
     6b486e89:	jmp    6b486d14 <vec_npy_eachFilter+0x194>
     6b486e8e:	xchg   %ax,%ax
     6b486e90:	lea    0xe16e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486e97:	mov    $0x8a6,%r8d
+    6b486e97:	mov    $0x8a9,%r8d
     6b486e9d:	lea    0xebf6(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486ea4:	call   6b48f9e0 <_assert>
     6b486ea9:	jmp    6b486cbf <vec_npy_eachFilter+0x13f>
     6b486eae:	xchg   %ax,%ax
     6b486eb0:	lea    0xe14e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486eb7:	mov    $0x8a6,%r8d
+    6b486eb7:	mov    $0x8a9,%r8d
     6b486ebd:	lea    0xebd6(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486ec4:	call   6b48f9e0 <_assert>
     6b486ec9:	cmpb   $0x59,0x55(%rsp)
     6b486ece:	je     6b486cbf <vec_npy_eachFilter+0x13f>
     6b486ed4:	jmp    6b486e90 <vec_npy_eachFilter+0x310>
     6b486ed6:	cs nopw 0x0(%rax,%rax,1)
     6b486ee0:	lea    0xe11e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486ee7:	mov    $0x8a6,%r8d
+    6b486ee7:	mov    $0x8a9,%r8d
     6b486eed:	lea    0xeba6(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486ef4:	call   6b48f9e0 <_assert>
     6b486ef9:	cmpb   $0x50,0x54(%rsp)
     6b486efe:	je     6b486cb4 <vec_npy_eachFilter+0x134>
     6b486f04:	jmp    6b486eb0 <vec_npy_eachFilter+0x330>
     6b486f06:	cs nopw 0x0(%rax,%rax,1)
     6b486f10:	lea    0xe0ee(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486f17:	mov    $0x8a6,%r8d
+    6b486f17:	mov    $0x8a9,%r8d
     6b486f1d:	lea    0xeb76(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486f24:	call   6b48f9e0 <_assert>
     6b486f29:	cmpb   $0x4d,0x53(%rsp)
     6b486f2e:	je     6b486ca9 <vec_npy_eachFilter+0x129>
     6b486f34:	jmp    6b486ee0 <vec_npy_eachFilter+0x360>
     6b486f36:	cs nopw 0x0(%rax,%rax,1)
     6b486f40:	lea    0xe0be(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486f47:	mov    $0x8a6,%r8d
+    6b486f47:	mov    $0x8a9,%r8d
     6b486f4d:	lea    0xeb46(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486f54:	call   6b48f9e0 <_assert>
     6b486f59:	cmpb   $0x55,0x52(%rsp)
     6b486f5e:	je     6b486c9e <vec_npy_eachFilter+0x11e>
     6b486f64:	jmp    6b486f10 <vec_npy_eachFilter+0x390>
     6b486f66:	cs nopw 0x0(%rax,%rax,1)
     6b486f70:	lea    0xe08e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486f77:	mov    $0x8a6,%r8d
+    6b486f77:	mov    $0x8a9,%r8d
     6b486f7d:	lea    0xeb16(%rip),%rcx        # 6b495a9a <.rdata+0xa9a>
     6b486f84:	call   6b48f9e0 <_assert>
     6b486f89:	cmpb   $0x4e,0x51(%rsp)
     6b486f8e:	je     6b486c93 <vec_npy_eachFilter+0x113>
     6b486f94:	jmp    6b486f40 <vec_npy_eachFilter+0x3c0>
     6b486f96:	cs nopw 0x0(%rax,%rax,1)
     6b486fa0:	lea    0xe05e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b486fa7:	mov    $0x8a3,%r8d
+    6b486fa7:	mov    $0x8a6,%r8d
     6b486fad:	lea    0xeade(%rip),%rcx        # 6b495a92 <.rdata+0xa92>
     6b486fb4:	call   6b48f9e0 <_assert>
     6b486fb9:	cmpb   $0x93,0x50(%rsp)
     6b486fbe:	je     6b486c88 <vec_npy_eachFilter+0x108>
     6b486fc4:	jmp    6b486f70 <vec_npy_eachFilter+0x3f0>
     6b486fc6:	cs nopw 0x0(%rax,%rax,1)
     6b486fd0:	mov    0x13049(%rip),%rax        # 6b49a020 <sqlite3_api>
@@ -9368,45 +9368,45 @@
     6b48703b:	mov    %rax,0x30(%rbx)
     6b48703f:	mov    0x3c(%rsp),%eax
     6b487043:	movups %xmm0,0x18(%rbx)
     6b487047:	mov    %eax,0x10(%rbx)
     6b48704a:	jmp    6b486e04 <vec_npy_eachFilter+0x284>
     6b48704f:	nop
     6b487050:	lea    0xdfae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487057:	mov    $0x8b2,%r8d
+    6b487057:	mov    $0x8b5,%r8d
     6b48705d:	lea    0xe9d8(%rip),%rcx        # 6b495a3c <.rdata+0xa3c>
     6b487064:	call   6b48f9e0 <_assert>
     6b487069:	jmp    6b486cde <vec_npy_eachFilter+0x15e>
     6b48706e:	xchg   %ax,%ax
     6b487070:	lea    0xdf8e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487077:	mov    $0x8c0,%r8d
+    6b487077:	mov    $0x8c3,%r8d
     6b48707d:	lea    0xe1fa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487084:	call   6b48f9e0 <_assert>
     6b487089:	jmp    6b486d57 <vec_npy_eachFilter+0x1d7>
     6b48708e:	xchg   %ax,%ax
     6b487090:	lea    0xdf6e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487097:	mov    $0x89a,%r8d
+    6b487097:	mov    $0x89d,%r8d
     6b48709d:	lea    0xe9e9(%rip),%rcx        # 6b495a8d <.rdata+0xa8d>
     6b4870a4:	call   6b48f9e0 <_assert>
     6b4870a9:	jmp    6b486c34 <vec_npy_eachFilter+0xb4>
     6b4870ae:	xchg   %ax,%ax
     6b4870b0:	lea    0xdf4e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4870b7:	mov    $0x8b5,%r8d
+    6b4870b7:	mov    $0x8b8,%r8d
     6b4870bd:	lea    0xe9f0(%rip),%rcx        # 6b495ab4 <.rdata+0xab4>
     6b4870c4:	call   6b48f9e0 <_assert>
     6b4870c9:	jmp    6b486cf9 <vec_npy_eachFilter+0x179>
     6b4870ce:	xchg   %ax,%ax
     6b4870d0:	lea    0xdf2e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4870d7:	mov    $0x8d3,%r8d
+    6b4870d7:	mov    $0x8d6,%r8d
     6b4870dd:	lea    0xea3d(%rip),%rcx        # 6b495b21 <.rdata+0xb21>
     6b4870e4:	call   6b48f9e0 <_assert>
     6b4870e9:	mov    0x40(%rbx),%rax
     6b4870ed:	jmp    6b486dd6 <vec_npy_eachFilter+0x256>
     6b4870f2:	lea    0xdf0c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4870f9:	mov    $0x8e7,%r8d
+    6b4870f9:	mov    $0x8ea,%r8d
     6b4870ff:	lea    0xe178(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487106:	call   6b48f9e0 <_assert>
     6b48710b:	jmp    6b487024 <vec_npy_eachFilter+0x4a4>
     6b487110:	mov    $0x2,%ecx
     6b487115:	call   *0xd205(%rip)        # 6b494320 <__imp___acrt_iob_func>
     6b48711b:	lea    0xe9ac(%rip),%r8        # 6b495ace <.rdata+0xace>
     6b487122:	lea    0xe067(%rip),%rdx        # 6b495190 <.rdata+0x190>
@@ -9561,15 +9561,15 @@
     6b487336:	call   *0x28(%rax)
     6b487339:	mov    0x12ce0(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487340:	mov    0x2f0(%rbx),%rcx
     6b487347:	call   *0x2f0(%rax)
     6b48734d:	cmp    $0x64,%eax
     6b487350:	je     6b48736b <vec0_get_vector_data+0xab>
     6b487352:	lea    0xdcac(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487359:	mov    $0xa5d,%r8d
+    6b487359:	mov    $0xa63,%r8d
     6b48735f:	lea    0xe844(%rip),%rcx        # 6b495baa <.rdata+0xbaa>
     6b487366:	call   6b48f9e0 <_assert>
     6b48736b:	mov    0x12cae(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487372:	lea    (%rbx,%r13,8),%rdi
     6b487376:	mov    $0x1,%edx
     6b48737b:	mov    0x2f0(%rbx),%rcx
     6b487382:	call   *0xe8(%rax)
@@ -9624,36 +9624,36 @@
     6b487455:	pop    %rbp
     6b487456:	pop    %r12
     6b487458:	pop    %r13
     6b48745a:	pop    %r14
     6b48745c:	ret
     6b48745d:	nopl   (%rax)
     6b487460:	lea    0xdb9e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487467:	mov    $0xa57,%r8d
+    6b487467:	mov    $0xa5d,%r8d
     6b48746d:	lea    0xe6ec(%rip),%rcx        # 6b495b60 <.rdata+0xb60>
     6b487474:	call   6b48f9e0 <_assert>
     6b487479:	jmp    6b4872f8 <vec0_get_vector_data+0x38>
     6b48747e:	xchg   %ax,%ax
     6b487480:	lea    0xdb7e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487487:	mov    $0xa62,%r8d
+    6b487487:	mov    $0xa68,%r8d
     6b48748d:	lea    0xddea(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487494:	call   6b48f9e0 <_assert>
     6b487499:	jmp    6b4873c6 <vec0_get_vector_data+0x106>
     6b48749e:	xchg   %ax,%ax
     6b4874a0:	lea    0xdb5e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4874a7:	mov    $0xa6b,%r8d
+    6b4874a7:	mov    $0xa71,%r8d
     6b4874ad:	lea    0xddca(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b4874b4:	call   6b48f9e0 <_assert>
     6b4874b9:	jmp    6b48743f <vec0_get_vector_data+0x17f>
     6b4874bb:	nopl   0x0(%rax,%rax,1)
     6b4874c0:	shr    $0x3,%rcx
     6b4874c4:	jmp    6b4873ff <vec0_get_vector_data+0x13f>
     6b4874c9:	nopl   0x0(%rax)
     6b4874d0:	lea    0xdb2e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4874d7:	mov    $0xa68,%r8d
+    6b4874d7:	mov    $0xa6e,%r8d
     6b4874dd:	lea    0xe6d0(%rip),%rcx        # 6b495bb4 <.rdata+0xbb4>
     6b4874e4:	call   6b48f9e0 <_assert>
     6b4874e9:	jmp    6b48741e <vec0_get_vector_data+0x15e>
     6b4874ee:	xchg   %ax,%ax
 
 000000006b4874f0 <vec0Column>:
     6b4874f0:	push   %rbp
@@ -9819,27 +9819,27 @@
     6b48777d:	mov    0x34(%rsp),%r8d
     6b487782:	mov    0x38(%rsp),%rdx
     6b487787:	mov    0x1d0(%rax),%r9
     6b48778e:	call   *0x270(%rax)
     6b487794:	jmp    6b487549 <vec0Column+0x59>
     6b487799:	nopl   0x0(%rax)
     6b4877a0:	lea    0xd85e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4877a7:	mov    $0xf13,%r8d
+    6b4877a7:	mov    $0xf19,%r8d
     6b4877ad:	lea    0xd8b9(%rip),%rcx        # 6b49506d <.rdata+0x6d>
     6b4877b4:	call   6b48f9e0 <_assert>
     6b4877b9:	jmp    6b487524 <vec0Column+0x34>
     6b4877be:	xchg   %ax,%ax
     6b4877c0:	lea    0xd83e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4877c7:	mov    $0xef9,%r8d
+    6b4877c7:	mov    $0xeff,%r8d
     6b4877cd:	lea    0xd874(%rip),%rcx        # 6b495048 <.rdata+0x48>
     6b4877d4:	call   6b48f9e0 <_assert>
     6b4877d9:	jmp    6b48761b <vec0Column+0x12b>
     6b4877de:	xchg   %ax,%ax
     6b4877e0:	lea    0xd81e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4877e7:	mov    $0xee0,%r8d
+    6b4877e7:	mov    $0xee6,%r8d
     6b4877ed:	lea    0xd865(%rip),%rcx        # 6b495059 <.rdata+0x59>
     6b4877f4:	call   6b48f9e0 <_assert>
     6b4877f9:	mov    0x10(%rbx),%rax
     6b4877fd:	jmp    6b487561 <vec0Column+0x71>
     6b487802:	mov    0x18(%rbx),%rax
     6b487806:	pxor   %xmm1,%xmm1
     6b48780a:	mov    %rbp,%rcx
@@ -9847,21 +9847,21 @@
     6b487811:	mov    0x10(%rax),%rax
     6b487815:	cvtss2sd (%rax,%rdx,4),%xmm1
     6b48781a:	mov    0x127ff(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487821:	call   *0x278(%rax)
     6b487827:	jmp    6b487549 <vec0Column+0x59>
     6b48782c:	nopl   0x0(%rax)
     6b487830:	lea    0xd7ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487837:	mov    $0xee9,%r8d
+    6b487837:	mov    $0xeef,%r8d
     6b48783d:	lea    0xda3a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487844:	call   6b48f9e0 <_assert>
     6b487849:	jmp    6b4875b7 <vec0Column+0xc7>
     6b48784e:	xchg   %ax,%ax
     6b487850:	lea    0xd7ae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487857:	mov    $0xf24,%r8d
+    6b487857:	mov    $0xf2a,%r8d
     6b48785d:	lea    0xda1a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487864:	call   6b48f9e0 <_assert>
     6b487869:	jmp    6b487773 <vec0Column+0x283>
     6b48786e:	xchg   %ax,%ax
     6b487870:	shr    $0x3,%r8
     6b487874:	jmp    6b487691 <vec0Column+0x1a1>
     6b487879:	nopl   0x0(%rax)
@@ -9889,15 +9889,15 @@
     6b4878d2:	call   *0x28(%rax)
     6b4878d5:	mov    0x12744(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b4878dc:	mov    0x2f0(%rbx),%rcx
     6b4878e3:	call   *0x2f0(%rax)
     6b4878e9:	cmp    $0x64,%eax
     6b4878ec:	je     6b487907 <vec0_get_chunk_position+0x87>
     6b4878ee:	lea    0xd710(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4878f5:	mov    $0xa84,%r8d
+    6b4878f5:	mov    $0xa8a,%r8d
     6b4878fb:	lea    0xe2b6(%rip),%rcx        # 6b495bb8 <.rdata+0xbb8>
     6b487902:	call   6b48f9e0 <_assert>
     6b487907:	mov    0x12712(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48790e:	mov    $0x1,%edx
     6b487913:	mov    0x2f0(%rbx),%rcx
     6b48791a:	call   *0xe8(%rax)
     6b487920:	mov    0x2f0(%rbx),%rcx
@@ -9908,15 +9908,15 @@
     6b48793c:	mov    0x2f0(%rbx),%rcx
     6b487943:	mov    %rax,(%rsi)
     6b487946:	mov    0x126d3(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48794d:	call   *0x2f0(%rax)
     6b487953:	cmp    $0x65,%eax
     6b487956:	je     6b487971 <vec0_get_chunk_position+0xf1>
     6b487958:	lea    0xd6a6(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48795f:	mov    $0xa88,%r8d
+    6b48795f:	mov    $0xa8e,%r8d
     6b487965:	lea    0xe25d(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48796c:	call   6b48f9e0 <_assert>
     6b487971:	xor    %eax,%eax
     6b487973:	add    $0x28,%rsp
     6b487977:	pop    %rbx
     6b487978:	pop    %rsi
     6b487979:	pop    %rdi
@@ -9987,15 +9987,15 @@
     6b487a87:	jne    6b487d30 <vec0_new_chunk+0x3b0>
     6b487a8d:	mov    0x1258c(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487a94:	mov    0x48(%rsp),%rcx
     6b487a99:	call   *0x2f0(%rax)
     6b487a9f:	cmp    $0x65,%eax
     6b487aa2:	je     6b487abd <vec0_new_chunk+0x13d>
     6b487aa4:	lea    0xd55a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487aab:	mov    $0xab3,%r8d
+    6b487aab:	mov    $0xab9,%r8d
     6b487ab1:	lea    0xe111(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b487ab8:	call   6b48f9e0 <_assert>
     6b487abd:	mov    0x18(%rsi),%rcx
     6b487ac1:	lea    0xd8(%rsi),%rbp
     6b487ac8:	xor    %edi,%edi
     6b487aca:	xor    %r15d,%r15d
     6b487acd:	mov    0x1254c(%rip),%rax        # 6b49a020 <sqlite3_api>
@@ -10051,15 +10051,15 @@
     6b487bc5:	jne    6b487c42 <vec0_new_chunk+0x2c2>
     6b487bc7:	mov    0x12452(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487bce:	mov    0x48(%rsp),%rcx
     6b487bd3:	call   *0x2f0(%rax)
     6b487bd9:	cmp    $0x65,%eax
     6b487bdc:	je     6b487bf3 <vec0_new_chunk+0x273>
     6b487bde:	lea    0xdfe4(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
-    6b487be5:	mov    $0xade,%r8d
+    6b487be5:	mov    $0xae4,%r8d
     6b487beb:	mov    %r12,%rdx
     6b487bee:	call   6b48f9e0 <_assert>
     6b487bf3:	mov    0x12426(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b487bfa:	add    $0x1,%edi
     6b487bfd:	add    $0x20,%rbp
     6b487c01:	mov    0x48(%rsp),%rcx
     6b487c06:	call   *0x1c8(%rax)
@@ -10070,27 +10070,27 @@
     6b487c20:	je     6b487cb5 <vec0_new_chunk+0x335>
     6b487c26:	cmp    $0xe1,%eax
     6b487c2b:	jne    6b487b10 <vec0_new_chunk+0x190>
     6b487c31:	movslq 0x2cc(%rsi),%rbx
     6b487c38:	imul   0x0(%rbp),%rbx
     6b487c3d:	jmp    6b487b1d <vec0_new_chunk+0x19d>
     6b487c42:	lea    0xd635(%rip),%rcx        # 6b49527e <.rdata+0x27e>
-    6b487c49:	mov    $0xadb,%r8d
+    6b487c49:	mov    $0xae1,%r8d
     6b487c4f:	mov    %r12,%rdx
     6b487c52:	call   6b48f9e0 <_assert>
     6b487c57:	jmp    6b487bc7 <vec0_new_chunk+0x247>
     6b487c5c:	nopl   0x0(%rax)
     6b487c60:	lea    0xd617(%rip),%rcx        # 6b49527e <.rdata+0x27e>
-    6b487c67:	mov    $0xad8,%r8d
+    6b487c67:	mov    $0xade,%r8d
     6b487c6d:	mov    %r12,%rdx
     6b487c70:	call   6b48f9e0 <_assert>
     6b487c75:	jmp    6b487ba9 <vec0_new_chunk+0x229>
     6b487c7a:	nopw   0x0(%rax,%rax,1)
     6b487c80:	lea    0xd5f7(%rip),%rcx        # 6b49527e <.rdata+0x27e>
-    6b487c87:	mov    $0xad6,%r8d
+    6b487c87:	mov    $0xadc,%r8d
     6b487c8d:	mov    %r12,%rdx
     6b487c90:	call   6b48f9e0 <_assert>
     6b487c95:	jmp    6b487b88 <vec0_new_chunk+0x208>
     6b487c9a:	nopw   0x0(%rax,%rax,1)
     6b487ca0:	movslq 0x2cc(%rsi),%rbx
     6b487ca7:	imul   0x0(%rbp),%rbx
     6b487cac:	shl    $0x2,%rbx
@@ -10100,15 +10100,15 @@
     6b487cc0:	imul   0x0(%rbp),%rax
     6b487cc5:	shr    $0x3,%rax
     6b487cc9:	cvtsi2sd %rax,%xmm0
     6b487cce:	cvttsd2si %xmm0,%rbx
     6b487cd3:	jmp    6b487b1d <vec0_new_chunk+0x19d>
     6b487cd8:	nopl   0x0(%rax,%rax,1)
     6b487ce0:	lea    0xdf38(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
-    6b487ce7:	mov    $0xad3,%r8d
+    6b487ce7:	mov    $0xad9,%r8d
     6b487ced:	mov    %r12,%rdx
     6b487cf0:	call   6b48f9e0 <_assert>
     6b487cf5:	jmp    6b487b48 <vec0_new_chunk+0x1c8>
     6b487cfa:	nopw   0x0(%rax,%rax,1)
     6b487d00:	cmpq   $0x0,0xa8(%rsp)
     6b487d09:	je     6b487d1b <vec0_new_chunk+0x39b>
     6b487d0b:	mov    0xa8(%rsp),%rax
@@ -10123,39 +10123,39 @@
     6b487d25:	pop    %r12
     6b487d27:	pop    %r13
     6b487d29:	pop    %r14
     6b487d2b:	pop    %r15
     6b487d2d:	ret
     6b487d2e:	xchg   %ax,%ax
     6b487d30:	lea    0xd2ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487d37:	mov    $0xab1,%r8d
+    6b487d37:	mov    $0xab7,%r8d
     6b487d3d:	lea    0xd53a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487d44:	call   6b48f9e0 <_assert>
     6b487d49:	jmp    6b487a8d <vec0_new_chunk+0x10d>
     6b487d4e:	xchg   %ax,%ax
     6b487d50:	lea    0xd2ae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487d57:	mov    $0xaae,%r8d
+    6b487d57:	mov    $0xab4,%r8d
     6b487d5d:	lea    0xd51a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487d64:	call   6b48f9e0 <_assert>
     6b487d69:	jmp    6b487a63 <vec0_new_chunk+0xe3>
     6b487d6e:	xchg   %ax,%ax
     6b487d70:	lea    0xd28e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487d77:	mov    $0xaab,%r8d
+    6b487d77:	mov    $0xab1,%r8d
     6b487d7d:	lea    0xd4fa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487d84:	call   6b48f9e0 <_assert>
     6b487d89:	jmp    6b487a30 <vec0_new_chunk+0xb0>
     6b487d8e:	xchg   %ax,%ax
     6b487d90:	lea    0xd26e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487d97:	mov    $0xaa6,%r8d
+    6b487d97:	mov    $0xaac,%r8d
     6b487d9d:	lea    0xd4da(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b487da4:	call   6b48f9e0 <_assert>
     6b487da9:	jmp    6b487a0d <vec0_new_chunk+0x8d>
     6b487dae:	xchg   %ax,%ax
     6b487db0:	lea    0xd24e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487db7:	mov    $0xaa3,%r8d
+    6b487db7:	mov    $0xaa9,%r8d
     6b487dbd:	lea    0xde5b(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b487dc4:	call   6b48f9e0 <_assert>
     6b487dc9:	jmp    6b4879c3 <vec0_new_chunk+0x43>
     6b487dce:	xchg   %ax,%ax
 
 000000006b487dd0 <vec0_init.constprop.16>:
     6b487dd0:	push   %r15
@@ -10217,15 +10217,15 @@
     6b487ec8:	je     6b4887f0 <vec0_init.constprop.16+0xa20>
     6b487ece:	add    $0x1,%ebp
     6b487ed1:	cmp    %rsi,%r13
     6b487ed4:	je     6b487fa7 <vec0_init.constprop.16+0x1d7>
     6b487eda:	cmp    $0x10,%ebp
     6b487edd:	jle    6b487ef8 <vec0_init.constprop.16+0x128>
     6b487edf:	lea    0xd11f(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487ee6:	mov    $0xb51,%r8d
+    6b487ee6:	mov    $0xb57,%r8d
     6b487eec:	lea    0xdd7a(%rip),%rcx        # 6b495c6d <.rdata+0xc6d>
     6b487ef3:	call   6b48f9e0 <_assert>
     6b487ef8:	add    $0x8,%rsi
     6b487efc:	mov    (%rsi),%r15
     6b487eff:	movslq %ebp,%rbx
     6b487f02:	mov    %r15,%rcx
     6b487f05:	call   6b493940 <strlen>
@@ -10249,15 +10249,15 @@
     6b487f58:	mov    %rbx,%rcx
     6b487f5b:	call   6b4859a0 <parse_primary_key_definition>
     6b487f60:	test   %eax,%eax
     6b487f62:	jne    6b4886f0 <vec0_init.constprop.16+0x920>
     6b487f68:	test   %r14,%r14
     6b487f6b:	je     6b487f86 <vec0_init.constprop.16+0x1b6>
     6b487f6d:	lea    0xd091(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b487f74:	mov    $0xb65,%r8d
+    6b487f74:	mov    $0xb6b,%r8d
     6b487f7a:	lea    0xdd73(%rip),%rcx        # 6b495cf4 <.rdata+0xcf4>
     6b487f81:	call   6b48f9e0 <_assert>
     6b487f86:	mov    0x78(%rsp),%eax
     6b487f8a:	cmp    %rsi,%r13
     6b487f8d:	mov    0x88(%rsp),%r14
     6b487f95:	mov    %eax,0x64(%rsp)
     6b487f99:	mov    0x7c(%rsp),%eax
@@ -10431,15 +10431,15 @@
     6b4882e5:	jne    6b488b49 <vec0_init.constprop.16+0xd79>
     6b4882eb:	mov    0x11d2e(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b4882f2:	mov    0x98(%rsp),%rcx
     6b4882fa:	call   *0x2f0(%rax)
     6b488300:	cmp    $0x65,%eax
     6b488303:	je     6b48831e <vec0_init.constprop.16+0x54e>
     6b488305:	lea    0xccf9(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48830c:	mov    $0xbd4,%r8d
+    6b48830c:	mov    $0xbda,%r8d
     6b488312:	lea    0xd8b0(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b488319:	call   6b48f9e0 <_assert>
     6b48831e:	mov    0x11cfb(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b488325:	lea    0xdcc4(%rip),%r12        # 6b495ff0 <.rdata+0xff0>
     6b48832c:	xor    %ebx,%ebx
     6b48832e:	mov    0x98(%rsp),%rcx
     6b488336:	lea    0xccc8(%rip),%r14        # 6b495005 <.rdata+0x5>
@@ -10468,15 +10468,15 @@
     6b4883b1:	test   %eax,%eax
     6b4883b3:	jne    6b4889a0 <vec0_init.constprop.16+0xbd0>
     6b4883b9:	mov    0x11c60(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b4883c0:	mov    0x98(%rsp),%rcx
     6b4883c8:	call   *0x2f0(%rax)
     6b4883ce:	cmp    $0x65,%eax
     6b4883d1:	je     6b488960 <vec0_init.constprop.16+0xb90>
-    6b4883d7:	mov    $0xbde,%r8d
+    6b4883d7:	mov    $0xbe4,%r8d
     6b4883dd:	mov    %r14,%rdx
     6b4883e0:	add    $0x1,%ebx
     6b4883e3:	lea    0xd7df(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b4883ea:	call   6b48f9e0 <_assert>
     6b4883ef:	mov    0x11c2a(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b4883f6:	mov    0x98(%rsp),%rcx
     6b4883fe:	call   *0x1c8(%rax)
@@ -10652,15 +10652,15 @@
     6b48874d:	mov    0x90(%rsp),%rcx
     6b488755:	call   *0x558(%rax)
     6b48875b:	test   %eax,%eax
     6b48875d:	jne    6b488c24 <vec0_init.constprop.16+0xe54>
     6b488763:	cmp    $0xffffffff,%r12d
     6b488767:	je     6b488782 <vec0_init.constprop.16+0x9b2>
     6b488769:	lea    0xc895(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488770:	mov    $0xb72,%r8d
+    6b488770:	mov    $0xb78,%r8d
     6b488776:	lea    0xd590(%rip),%rcx        # 6b495d0d <.rdata+0xd0d>
     6b48877d:	call   6b48f9e0 <_assert>
     6b488782:	mov    0x98(%rsp),%rcx
     6b48878a:	call   6b4939e0 <atoi>
     6b48878f:	test   %eax,%eax
     6b488791:	mov    %eax,%r12d
     6b488794:	jle    6b488c0d <vec0_init.constprop.16+0xe3d>
@@ -10672,43 +10672,43 @@
     6b4887b4:	lea    0xc9d5(%rip),%rdx        # 6b495190 <.rdata+0x190>
     6b4887bb:	mov    %rax,%rcx
     6b4887be:	call   6b4939b0 <fprintf>
     6b4887c3:	mov    $0x1,%ecx
     6b4887c8:	call   6b4939c8 <exit>
     6b4887cd:	nopl   (%rax)
     6b4887d0:	lea    0xc82e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4887d7:	mov    $0xb56,%r8d
+    6b4887d7:	mov    $0xb5c,%r8d
     6b4887dd:	lea    0xd4a4(%rip),%rcx        # 6b495c88 <.rdata+0xc88>
     6b4887e4:	call   6b48f9e0 <_assert>
     6b4887e9:	jmp    6b487e96 <vec0_init.constprop.16+0xc6>
     6b4887ee:	xchg   %ax,%ax
     6b4887f0:	lea    0xc80e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4887f7:	mov    $0xb5a,%r8d
+    6b4887f7:	mov    $0xb60,%r8d
     6b4887fd:	lea    0xd4c4(%rip),%rcx        # 6b495cc8 <.rdata+0xcc8>
     6b488804:	call   6b48f9e0 <_assert>
     6b488809:	jmp    6b487ece <vec0_init.constprop.16+0xfe>
     6b48880e:	lea    0xc7f0(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488815:	mov    $0xb87,%r8d
+    6b488815:	mov    $0xb8d,%r8d
     6b48881b:	lea    0xd44b(%rip),%rcx        # 6b495c6d <.rdata+0xc6d>
     6b488822:	call   6b48f9e0 <_assert>
     6b488827:	jmp    6b487fc5 <vec0_init.constprop.16+0x1f5>
     6b48882c:	nopl   0x0(%rax)
-    6b488830:	mov    $0xc28,%r8d
+    6b488830:	mov    $0xc2e,%r8d
     6b488836:	mov    %r14,%rdx
     6b488839:	mov    %r12,%rcx
     6b48883c:	call   6b48f9e0 <_assert>
     6b488841:	add    $0x1,%esi
     6b488844:	add    $0x8,%rbx
     6b488848:	cmp    %esi,0x2c8(%rdi)
     6b48884e:	jg     6b488680 <vec0_init.constprop.16+0x8b0>
     6b488854:	jmp    6b4886d0 <vec0_init.constprop.16+0x900>
     6b488859:	xor    %r14d,%r14d
     6b48885c:	mov    $0x400,%r12d
     6b488862:	lea    0xc79c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488869:	mov    $0xb86,%r8d
+    6b488869:	mov    $0xb8c,%r8d
     6b48886f:	lea    0xd518(%rip),%rcx        # 6b495d8e <.rdata+0xd8e>
     6b488876:	call   6b48f9e0 <_assert>
     6b48887b:	mov    0x1179e(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b488882:	xor    %ecx,%ecx
     6b488884:	call   *0x720(%rax)
     6b48888a:	lea    0xd512(%rip),%rdx        # 6b495da3 <.rdata+0xda3>
     6b488891:	mov    %rax,%rcx
@@ -10736,20 +10736,20 @@
     6b488901:	jmp    6b488016 <vec0_init.constprop.16+0x246>
     6b488906:	mov    0x11713(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48890d:	lea    0xd5cc(%rip),%rcx        # 6b495ee0 <.rdata+0xee0>
     6b488914:	call   *0x228(%rax)
     6b48891a:	mov    %rax,%rbx
     6b48891d:	jmp    6b48829e <vec0_init.constprop.16+0x4ce>
     6b488922:	lea    0xc6dc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488929:	mov    $0xbc3,%r8d
+    6b488929:	mov    $0xbc9,%r8d
     6b48892f:	lea    0xd293(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b488936:	call   6b48f9e0 <_assert>
     6b48893b:	jmp    6b48825f <vec0_init.constprop.16+0x48f>
     6b488940:	lea    0xc6be(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488947:	mov    $0xbc1,%r8d
+    6b488947:	mov    $0xbc7,%r8d
     6b48894d:	lea    0xc92a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488954:	call   6b48f9e0 <_assert>
     6b488959:	jmp    6b488241 <vec0_init.constprop.16+0x471>
     6b48895e:	xchg   %ax,%ax
     6b488960:	mov    0x116b9(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b488967:	add    $0x1,%ebx
     6b48896a:	mov    0x98(%rsp),%rcx
@@ -10758,113 +10758,113 @@
     6b48897f:	mov    %rsi,%rcx
     6b488982:	call   *0x1d0(%rax)
     6b488988:	cmp    0x2c8(%rdi),%ebx
     6b48898e:	jl     6b488360 <vec0_init.constprop.16+0x590>
     6b488994:	jmp    6b488420 <vec0_init.constprop.16+0x650>
     6b488999:	nopl   0x0(%rax)
     6b4889a0:	lea    0xc8d7(%rip),%rcx        # 6b49527e <.rdata+0x27e>
-    6b4889a7:	mov    $0xbdc,%r8d
+    6b4889a7:	mov    $0xbe2,%r8d
     6b4889ad:	mov    %r14,%rdx
     6b4889b0:	call   6b48f9e0 <_assert>
     6b4889b5:	jmp    6b4883b9 <vec0_init.constprop.16+0x5e9>
     6b4889ba:	nopw   0x0(%rax,%rax,1)
-    6b4889c0:	mov    $0xbda,%r8d
+    6b4889c0:	mov    $0xbe0,%r8d
     6b4889c6:	mov    %r14,%rdx
     6b4889c9:	mov    %r15,%rcx
     6b4889cc:	call   6b48f9e0 <_assert>
     6b4889d1:	jmp    6b488387 <vec0_init.constprop.16+0x5b7>
     6b4889d6:	mov    $0x7,%r13d
     6b4889dc:	jmp    6b4886d0 <vec0_init.constprop.16+0x900>
     6b4889e1:	lea    0xc61d(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4889e8:	mov    $0xc1e,%r8d
+    6b4889e8:	mov    $0xc24,%r8d
     6b4889ee:	lea    0xc889(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b4889f5:	call   6b48f9e0 <_assert>
     6b4889fa:	jmp    6b488651 <vec0_init.constprop.16+0x881>
     6b4889ff:	lea    0xc5ff(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a06:	mov    $0xbfa,%r8d
+    6b488a06:	mov    $0xc00,%r8d
     6b488a0c:	lea    0xc86b(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488a13:	call   6b48f9e0 <_assert>
     6b488a18:	jmp    6b48850d <vec0_init.constprop.16+0x73d>
     6b488a1d:	lea    0xc5e1(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a24:	mov    $0xbee,%r8d
+    6b488a24:	mov    $0xbf4,%r8d
     6b488a2a:	lea    0xc84d(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488a31:	call   6b48f9e0 <_assert>
     6b488a36:	jmp    6b4884a1 <vec0_init.constprop.16+0x6d1>
     6b488a3b:	lea    0xc5c3(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a42:	mov    $0xc12,%r8d
+    6b488a42:	mov    $0xc18,%r8d
     6b488a48:	lea    0xc82f(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488a4f:	call   6b48f9e0 <_assert>
     6b488a54:	jmp    6b4885e5 <vec0_init.constprop.16+0x815>
     6b488a59:	lea    0xc5a5(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a60:	mov    $0xc05,%r8d
+    6b488a60:	mov    $0xc0b,%r8d
     6b488a66:	lea    0xc811(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488a6d:	call   6b48f9e0 <_assert>
     6b488a72:	jmp    6b488579 <vec0_init.constprop.16+0x7a9>
     6b488a77:	lea    0xc587(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a7e:	mov    $0xb9b,%r8d
+    6b488a7e:	mov    $0xba1,%r8d
     6b488a84:	lea    0xd194(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488a8b:	call   6b48f9e0 <_assert>
     6b488a90:	jmp    6b4880a7 <vec0_init.constprop.16+0x2d7>
     6b488a95:	lea    0xc569(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488a9c:	mov    $0xba2,%r8d
+    6b488a9c:	mov    $0xba8,%r8d
     6b488aa2:	lea    0xd354(%rip),%rcx        # 6b495dfd <.rdata+0xdfd>
     6b488aa9:	call   6b48f9e0 <_assert>
     6b488aae:	jmp    6b4880e4 <vec0_init.constprop.16+0x314>
     6b488ab3:	lea    0xc54b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488aba:	mov    $0xc02,%r8d
+    6b488aba:	mov    $0xc08,%r8d
     6b488ac0:	lea    0xd158(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488ac7:	call   6b48f9e0 <_assert>
     6b488acc:	jmp    6b488535 <vec0_init.constprop.16+0x765>
     6b488ad1:	lea    0xc52d(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488ad8:	mov    $0xbf6,%r8d
+    6b488ad8:	mov    $0xbfc,%r8d
     6b488ade:	lea    0xd13a(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488ae5:	call   6b48f9e0 <_assert>
     6b488aea:	jmp    6b4884c9 <vec0_init.constprop.16+0x6f9>
     6b488aef:	lea    0xc50f(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488af6:	mov    $0xbeb,%r8d
+    6b488af6:	mov    $0xbf1,%r8d
     6b488afc:	lea    0xd11c(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488b03:	call   6b48f9e0 <_assert>
     6b488b08:	jmp    6b48845d <vec0_init.constprop.16+0x68d>
     6b488b0d:	lea    0xc4f1(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488b14:	mov    $0xc1a,%r8d
+    6b488b14:	mov    $0xc20,%r8d
     6b488b1a:	lea    0xd0fe(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488b21:	call   6b48f9e0 <_assert>
     6b488b26:	jmp    6b48860d <vec0_init.constprop.16+0x83d>
     6b488b2b:	lea    0xc4d3(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488b32:	mov    $0xc0e,%r8d
+    6b488b32:	mov    $0xc14,%r8d
     6b488b38:	lea    0xd0e0(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b488b3f:	call   6b48f9e0 <_assert>
     6b488b44:	jmp    6b4885a1 <vec0_init.constprop.16+0x7d1>
     6b488b49:	lea    0xc4b5(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488b50:	mov    $0xbd2,%r8d
+    6b488b50:	mov    $0xbd8,%r8d
     6b488b56:	lea    0xc721(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488b5d:	call   6b48f9e0 <_assert>
     6b488b62:	jmp    6b4882eb <vec0_init.constprop.16+0x51b>
     6b488b67:	lea    0xc497(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488b6e:	mov    $0xbe4,%r8d
+    6b488b6e:	mov    $0xbea,%r8d
     6b488b74:	lea    0xc7df(%rip),%rcx        # 6b49535a <.rdata+0x35a>
     6b488b7b:	call   6b48f9e0 <_assert>
     6b488b80:	jmp    6b488432 <vec0_init.constprop.16+0x662>
     6b488b85:	mov    0x11494(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b488b8c:	lea    0xd5dd(%rip),%rdx        # 6b496170 <.rdata+0x1170>
     6b488b93:	mov    %rbx,%rcx
     6b488b96:	xor    %ebp,%ebp
     6b488b98:	call   *0x748(%rax)
     6b488b9e:	mov    0x1147b(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b488ba5:	lea    0xd21c(%rip),%rdx        # 6b495dc8 <.rdata+0xdc8>
     6b488bac:	mov    %rbx,%rcx
     6b488baf:	call   *0x748(%rax)
     6b488bb5:	jmp    6b48808b <vec0_init.constprop.16+0x2bb>
     6b488bba:	lea    0xc444(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488bc1:	mov    $0xbcf,%r8d
+    6b488bc1:	mov    $0xbd5,%r8d
     6b488bc7:	lea    0xd40b(%rip),%rcx        # 6b495fd9 <.rdata+0xfd9>
     6b488bce:	call   6b48f9e0 <_assert>
     6b488bd3:	jmp    6b4882a7 <vec0_init.constprop.16+0x4d7>
     6b488bd8:	lea    0xc426(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488bdf:	mov    $0xbbe,%r8d
+    6b488bdf:	mov    $0xbc4,%r8d
     6b488be5:	lea    0xd2d9(%rip),%rcx        # 6b495ec5 <.rdata+0xec5>
     6b488bec:	call   6b48f9e0 <_assert>
     6b488bf1:	jmp    6b4881f5 <vec0_init.constprop.16+0x425>
     6b488bf6:	mov    $0x2,%ecx
     6b488bfb:	call   *0xb71f(%rip)        # 6b494320 <__imp___acrt_iob_func>
     6b488c01:	lea    0xd16e(%rip),%r8        # 6b495d76 <.rdata+0xd76>
     6b488c08:	jmp    6b4887b4 <vec0_init.constprop.16+0x9e4>
@@ -10907,15 +10907,15 @@
     6b488c9f:	jne    6b488cb0 <vec0_query_fullscan_data_clear+0x30>
     6b488ca1:	movq   $0x0,(%rbx)
     6b488ca8:	xor    %eax,%eax
     6b488caa:	add    $0x20,%rsp
     6b488cae:	pop    %rbx
     6b488caf:	ret
     6b488cb0:	lea    0xc34e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488cb7:	mov    $0xaff,%r8d
+    6b488cb7:	mov    $0xb05,%r8d
     6b488cbd:	lea    0xc5ba(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b488cc4:	call   6b48f9e0 <_assert>
     6b488cc9:	jmp    6b488ca1 <vec0_query_fullscan_data_clear+0x21>
     6b488ccb:	nopl   0x0(%rax,%rax,1)
 
 000000006b488cd0 <vec0_query_knn_data_clear>:
     6b488cd0:	push   %rbx
@@ -11073,15 +11073,15 @@
     6b488ee4:	cmpb   $0x0,-0x1(%rsi,%rcx,1)
     6b488ee9:	je     6b488f71 <min_idx+0x111>
     6b488eef:	mov    %rcx,%rdx
     6b488ef2:	cmp    %rdx,%r13
     6b488ef5:	mov    %edx,%ebx
     6b488ef7:	jne    6b488ee0 <min_idx+0x80>
     6b488ef9:	lea    0xc105(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488f00:	mov    $0xd4d,%r8d
+    6b488f00:	mov    $0xd53,%r8d
     6b488f06:	lea    0xd27e(%rip),%rcx        # 6b49618b <.rdata+0x118b>
     6b488f0d:	call   6b48f9e0 <_assert>
     6b488f12:	lea    (%r12,%r13,4),%rax
     6b488f16:	movss  (%rax),%xmm1
     6b488f1a:	xor    %edx,%edx
     6b488f1c:	nopl   0x0(%rax)
     6b488f20:	movss  (%r12,%rdx,4),%xmm0
@@ -11112,37 +11112,37 @@
     6b488f6a:	pop    %r12
     6b488f6c:	pop    %r13
     6b488f6e:	pop    %r14
     6b488f70:	ret
     6b488f71:	lea    (%r12,%rdx,4),%rax
     6b488f75:	jmp    6b488f16 <min_idx+0xb6>
     6b488f77:	xor    %ebx,%ebx
-    6b488f79:	mov    $0xd4d,%r8d
+    6b488f79:	mov    $0xd53,%r8d
     6b488f7f:	add    $0x4,%r14
     6b488f83:	lea    0xc07b(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b488f8a:	lea    0xd1fa(%rip),%rcx        # 6b49618b <.rdata+0x118b>
     6b488f91:	call   6b48f9e0 <_assert>
     6b488f96:	mov    %ebx,-0x4(%r14)
     6b488f9a:	xor    %eax,%eax
     6b488f9c:	cmp    %rbp,%r14
     6b488f9f:	movb   $0x1,(%rsi,%rax,1)
     6b488fa3:	jne    6b488ec0 <min_idx+0x60>
     6b488fa9:	jmp    6b488f58 <min_idx+0xf8>
     6b488fab:	lea    0xc053(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488fb2:	mov    $0xd42,%r8d
+    6b488fb2:	mov    $0xd48,%r8d
     6b488fb8:	lea    0xd1bf(%rip),%rcx        # 6b49617e <.rdata+0x117e>
     6b488fbf:	call   6b48f9e0 <_assert>
     6b488fc4:	jmp    6b488e8a <min_idx+0x2a>
     6b488fc9:	lea    0xc035(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488fd0:	mov    $0xd41,%r8d
+    6b488fd0:	mov    $0xd47,%r8d
     6b488fd6:	lea    0xd19b(%rip),%rcx        # 6b496178 <.rdata+0x1178>
     6b488fdd:	call   6b48f9e0 <_assert>
     6b488fe2:	jmp    6b488e82 <min_idx+0x22>
     6b488fe7:	lea    0xc017(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b488fee:	mov    $0xd45,%r8d
+    6b488fee:	mov    $0xd4b,%r8d
     6b488ff4:	lea    0xd18a(%rip),%rcx        # 6b496185 <.rdata+0x1185>
     6b488ffb:	call   6b48f9e0 <_assert>
     6b489000:	jmp    6b488ea3 <min_idx+0x43>
     6b489005:	nop
     6b489006:	cs nopw 0x0(%rax,%rax,1)
 
 000000006b489010 <vec0Filter>:
@@ -11302,22 +11302,22 @@
     6b4892e5:	sub    $0x64,%eax
     6b4892e8:	cmp    $0x1,%eax
     6b4892eb:	ja     6b48a550 <vec0Filter+0x1540>
     6b4892f1:	mov    0x230(%rsp),%rax
     6b4892f9:	mov    %rsi,0x10(%rax)
     6b4892fd:	jmp    6b489119 <vec0Filter+0x109>
     6b489302:	lea    0xbcfc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b489309:	mov    $0xe7b,%r8d
+    6b489309:	mov    $0xe81,%r8d
     6b48930f:	lea    0xbd66(%rip),%rcx        # 6b49507c <.rdata+0x7c>
     6b489316:	call   6b48f9e0 <_assert>
     6b48931b:	jmp    6b48916a <vec0Filter+0x15a>
     6b489320:	mov    $0x7,%ebp
     6b489325:	jmp    6b489119 <vec0Filter+0x109>
     6b48932a:	nopw   0x0(%rax,%rax,1)
-    6b489330:	mov    $0xe88,%r8d
+    6b489330:	mov    $0xe8e,%r8d
     6b489336:	mov    %r14,%rdx
     6b489339:	mov    %rdi,%rcx
     6b48933c:	call   6b48f9e0 <_assert>
     6b489341:	add    $0x1,%esi
     6b489344:	add    $0x8,%r15
     6b489348:	cmp    %esi,0x2c8(%rbx)
     6b48934e:	jg     6b4891e0 <vec0Filter+0x1d0>
@@ -11349,24 +11349,24 @@
     6b4893f2:	movslq %r14d,%rax
     6b4893f5:	mov    0x14c(%rsp),%edi
     6b4893fc:	mov    %rax,0x60(%rsp)
     6b489401:	shl    $0x5,%rax
     6b489405:	cmp    %edi,0xe0(%rbx,%rax,1)
     6b48940c:	je     6b489427 <vec0Filter+0x417>
     6b48940e:	lea    0xbbf0(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b489415:	mov    $0xd75,%r8d
+    6b489415:	mov    $0xd7b,%r8d
     6b48941b:	lea    0xcdc6(%rip),%rcx        # 6b4961e8 <.rdata+0x11e8>
     6b489422:	call   6b48f9e0 <_assert>
     6b489427:	mov    0x60(%rsp),%rax
     6b48942c:	mov    0x158(%rsp),%rdi
     6b489434:	shl    $0x5,%rax
     6b489438:	cmp    %rdi,0xd8(%rbx,%rax,1)
     6b489440:	je     6b48945b <vec0Filter+0x44b>
     6b489442:	lea    0xbbbc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b489449:	mov    $0xd76,%r8d
+    6b489449:	mov    $0xd7c,%r8d
     6b48944f:	lea    0xcdc2(%rip),%rcx        # 6b496218 <.rdata+0x1218>
     6b489456:	call   6b48f9e0 <_assert>
     6b48945b:	mov    0x10bbe(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b489462:	mov    0x8(%r12),%rcx
     6b489467:	call   *0x358(%rax)
     6b48946d:	test   %rax,%rax
     6b489470:	mov    %rax,%rdi
@@ -11616,15 +11616,15 @@
     6b489931:	lea    0x7(%rcx),%edx
     6b489934:	test   %ecx,%ecx
     6b489936:	cmovns %ecx,%edx
     6b489939:	sar    $0x3,%edx
     6b48993c:	cmp    %edx,%eax
     6b48993e:	je     6b489959 <vec0Filter+0x949>
     6b489940:	lea    0xb6be(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b489947:	mov    $0xdc0,%r8d
+    6b489947:	mov    $0xdc6,%r8d
     6b48994d:	lea    0xc964(%rip),%rcx        # 6b4962b8 <.rdata+0x12b8>
     6b489954:	call   6b48f9e0 <_assert>
     6b489959:	mov    0x106c0(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b489960:	mov    $0x2,%edx
     6b489965:	mov    0x178(%rsp),%rcx
     6b48996d:	call   *0x98(%rax)
     6b489973:	mov    $0x2,%edx
@@ -11634,15 +11634,15 @@
     6b48998a:	call   *0xa0(%rax)
     6b489990:	movslq 0x2cc(%rbx),%rdx
     6b489997:	cltq
     6b489999:	shl    $0x3,%rdx
     6b48999d:	cmp    %rax,%rdx
     6b4899a0:	je     6b4899bb <vec0Filter+0x9ab>
     6b4899a2:	lea    0xb65c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b4899a9:	mov    $0xdc3,%r8d
+    6b4899a9:	mov    $0xdc9,%r8d
     6b4899af:	lea    0xc92a(%rip),%rcx        # 6b4962e0 <.rdata+0x12e0>
     6b4899b6:	call   6b48f9e0 <_assert>
     6b4899bb:	mov    0x60(%rsp),%rax
     6b4899c0:	lea    0xc7a1(%rip),%r9        # 6b496168 <.rdata+0x1168>
     6b4899c7:	mov    0x28(%rbx),%rdx
     6b4899cb:	mov    0x18(%rbx),%rcx
     6b4899cf:	mov    0x48(%rbx,%rax,8),%r8
@@ -11673,15 +11673,15 @@
     6b489a59:	cmovne 0x50(%rsp),%rax
     6b489a5f:	mov    %rax,0x50(%rsp)
     6b489a64:	mov    0x50(%rsp),%rax
     6b489a69:	imul   %rdx,%rax
     6b489a6d:	cmp    %rax,%r8
     6b489a70:	je     6b489a8b <vec0Filter+0xa7b>
     6b489a72:	lea    0xb58c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b489a79:	mov    $0xdcc,%r8d
+    6b489a79:	mov    $0xdd2,%r8d
     6b489a7f:	lea    0xc88a(%rip),%rcx        # 6b496310 <.rdata+0x1310>
     6b489a86:	call   6b48f9e0 <_assert>
     6b489a8b:	cmp    0x70(%rsp),%rbp
     6b489a90:	mov    0x10589(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b489a97:	jle    6b489ace <vec0Filter+0xabe>
     6b489a99:	test   %r13,%r13
     6b489a9c:	je     6b489aae <vec0Filter+0xa9e>
@@ -12148,21 +12148,21 @@
     6b48a2b2:	sqrtsd %xmm1,%xmm7
     6b48a2b6:	jbe    6b48a110 <vec0Filter+0x1100>
     6b48a2bc:	jmp    6b48a1ac <vec0Filter+0x119c>
     6b48a2c1:	mov    %rax,0x50(%rsp)
     6b48a2c6:	jmp    6b489a64 <vec0Filter+0xa54>
     6b48a2cb:	nopl   0x0(%rax,%rax,1)
     6b48a2d0:	lea    0xad2e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a2d7:	mov    $0xdd8,%r8d
+    6b48a2d7:	mov    $0xdde,%r8d
     6b48a2dd:	lea    0xaf9a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a2e4:	call   6b48f9e0 <_assert>
     6b48a2e9:	jmp    6b489aed <vec0Filter+0xadd>
     6b48a2ee:	xchg   %ax,%ax
     6b48a2f0:	lea    0xad0e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a2f7:	mov    $0xdc9,%r8d
+    6b48a2f7:	mov    $0xdcf,%r8d
     6b48a2fd:	lea    0xaf7a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a304:	call   6b48f9e0 <_assert>
     6b48a309:	jmp    6b489a03 <vec0Filter+0x9f3>
     6b48a30e:	xchg   %ax,%ax
     6b48a310:	shr    $0x3,%rax
     6b48a314:	mov    %rax,0x50(%rsp)
     6b48a319:	jmp    6b489a64 <vec0Filter+0xa54>
@@ -12175,35 +12175,35 @@
     6b48a339:	mov    %r8,(%r12,%rax,2)
     6b48a33d:	movss  %xmm0,(%r14,%rax,1)
     6b48a343:	add    $0x4,%rax
     6b48a347:	cmp    %r9,%rax
     6b48a34a:	jne    6b48a330 <vec0Filter+0x1320>
     6b48a34c:	jmp    6b489dbe <vec0Filter+0xdae>
     6b48a351:	lea    0xacad(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a358:	mov    $0xe29,%r8d
+    6b48a358:	mov    $0xe2f,%r8d
     6b48a35e:	lea    0xc028(%rip),%rcx        # 6b49638d <.rdata+0x138d>
     6b48a365:	call   6b48f9e0 <_assert>
     6b48a36a:	jmp    6b489c0b <vec0Filter+0xbfb>
     6b48a36f:	nop
     6b48a370:	lea    0xac8e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a377:	mov    $0xddc,%r8d
+    6b48a377:	mov    $0xde2,%r8d
     6b48a37d:	lea    0xbff9(%rip),%rcx        # 6b49637d <.rdata+0x137d>
     6b48a384:	call   6b48f9e0 <_assert>
     6b48a389:	mov    0x2cc(%rbx),%edx
     6b48a38f:	test   %edx,%edx
     6b48a391:	jg     6b489b21 <vec0Filter+0xb11>
     6b48a397:	nopw   0x0(%rax,%rax,1)
     6b48a3a0:	lea    0x188(%rsp),%rax
     6b48a3a8:	mov    %rax,0x58(%rsp)
     6b48a3ad:	jmp    6b489beb <vec0Filter+0xbdb>
     6b48a3b2:	pxor   %xmm7,%xmm7
     6b48a3b6:	jmp    6b489ba7 <vec0Filter+0xb97>
     6b48a3bb:	nopl   0x0(%rax,%rax,1)
     6b48a3c0:	lea    0xac3e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a3c7:	mov    $0xdd3,%r8d
+    6b48a3c7:	mov    $0xdd9,%r8d
     6b48a3cd:	lea    0xbf9d(%rip),%rcx        # 6b496371 <.rdata+0x1371>
     6b48a3d4:	call   6b48f9e0 <_assert>
     6b48a3d9:	jmp    6b489ac2 <vec0Filter+0xab2>
     6b48a3de:	xchg   %ax,%ax
     6b48a3e0:	mov    0xfc39(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48a3e7:	mov    %r13,%rcx
     6b48a3ea:	mov    0x78(%rsp),%r15
@@ -12243,30 +12243,30 @@
     6b48a4a9:	movapd %xmm1,%xmm10
     6b48a4ae:	jmp    6b48a0f6 <vec0Filter+0x10e6>
     6b48a4b3:	movapd %xmm6,%xmm7
     6b48a4b7:	movapd %xmm6,%xmm2
     6b48a4bb:	movapd %xmm6,%xmm9
     6b48a4c0:	jmp    6b48a008 <vec0Filter+0xff8>
     6b48a4c5:	lea    0xab39(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a4cc:	mov    $0xe6b,%r8d
+    6b48a4cc:	mov    $0xe71,%r8d
     6b48a4d2:	lea    0xada5(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a4d9:	call   6b48f9e0 <_assert>
     6b48a4de:	jmp    6b4892ce <vec0Filter+0x2be>
     6b48a4e3:	xor    %edx,%edx
     6b48a4e5:	pxor   %xmm7,%xmm7
     6b48a4e9:	pxor   %xmm4,%xmm4
     6b48a4ed:	pxor   %xmm5,%xmm5
     6b48a4f1:	jmp    6b489f4e <vec0Filter+0xf3e>
     6b48a4f6:	cs nopw 0x0(%rax,%rax,1)
     6b48a500:	xor    %edx,%edx
     6b48a502:	pxor   %xmm1,%xmm1
     6b48a506:	jmp    6b48a25d <vec0Filter+0x124d>
     6b48a50b:	nopl   0x0(%rax,%rax,1)
     6b48a510:	lea    0xaaee(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a517:	mov    $0xd8f,%r8d
+    6b48a517:	mov    $0xd95,%r8d
     6b48a51d:	lea    0xad5a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a524:	call   6b48f9e0 <_assert>
     6b48a529:	jmp    6b48953b <vec0Filter+0x52b>
     6b48a52e:	xchg   %ax,%ax
     6b48a530:	mov    0x128(%rsp),%rax
     6b48a538:	mov    0x230(%rsp),%rdi
     6b48a540:	movq   $0x0,(%rax)
@@ -12281,91 +12281,91 @@
     6b48a56e:	test   %eax,%eax
     6b48a570:	jne    6b48a6b0 <vec0Filter+0x16a0>
     6b48a576:	movq   $0x0,(%rsi)
     6b48a57d:	mov    $0x1,%ebp
     6b48a582:	jmp    6b489119 <vec0Filter+0x109>
     6b48a587:	nopw   0x0(%rax,%rax,1)
     6b48a590:	lea    0xaa6e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a597:	mov    $0xd60,%r8d
+    6b48a597:	mov    $0xd66,%r8d
     6b48a59d:	lea    0xbc3a(%rip),%rcx        # 6b4961de <.rdata+0x11de>
     6b48a5a4:	call   6b48f9e0 <_assert>
     6b48a5a9:	jmp    6b48936a <vec0Filter+0x35a>
     6b48a5ae:	xchg   %ax,%ax
     6b48a5b0:	lea    0xaa4e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a5b7:	mov    $0xd79,%r8d
+    6b48a5b7:	mov    $0xd7f,%r8d
     6b48a5bd:	lea    0xbc7c(%rip),%rcx        # 6b496240 <.rdata+0x1240>
     6b48a5c4:	call   6b48f9e0 <_assert>
     6b48a5c9:	jmp    6b48947f <vec0Filter+0x46f>
     6b48a5ce:	xchg   %ax,%ax
     6b48a5d0:	lea    0xaa2e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a5d7:	mov    $0xe68,%r8d
+    6b48a5d7:	mov    $0xe6e,%r8d
     6b48a5dd:	lea    0xb63b(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b48a5e4:	call   6b48f9e0 <_assert>
     6b48a5e9:	jmp    6b48928e <vec0Filter+0x27e>
     6b48a5ee:	xchg   %ax,%ax
     6b48a5f0:	lea    0xaa0e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a5f7:	mov    $0xdb0,%r8d
+    6b48a5f7:	mov    $0xdb6,%r8d
     6b48a5fd:	lea    0xac7a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a604:	call   6b48f9e0 <_assert>
     6b48a609:	jmp    6b48974f <vec0Filter+0x73f>
     6b48a60e:	xchg   %ax,%ax
     6b48a610:	lea    0xa9ee(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a617:	mov    $0xe41,%r8d
+    6b48a617:	mov    $0xe47,%r8d
     6b48a61d:	lea    0xac5a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a624:	call   6b48f9e0 <_assert>
     6b48a629:	jmp    6b48a419 <vec0Filter+0x1409>
     6b48a62e:	xchg   %ax,%ax
     6b48a630:	lea    0xa9ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a637:	mov    $0xd91,%r8d
+    6b48a637:	mov    $0xd97,%r8d
     6b48a63d:	lea    0xb585(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48a644:	call   6b48f9e0 <_assert>
     6b48a649:	jmp    6b4895c9 <vec0Filter+0x5b9>
     6b48a64e:	xchg   %ax,%ax
     6b48a650:	lea    0xa9ae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a657:	mov    $0xdad,%r8d
+    6b48a657:	mov    $0xdb3,%r8d
     6b48a65d:	lea    0xb5bb(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b48a664:	call   6b48f9e0 <_assert>
     6b48a669:	jmp    6b489708 <vec0Filter+0x6f8>
     6b48a66e:	xchg   %ax,%ax
     6b48a670:	lea    0xa98e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a677:	mov    $0xd97,%r8d
+    6b48a677:	mov    $0xd9d,%r8d
     6b48a67d:	lea    0xbbd1(%rip),%rcx        # 6b496255 <.rdata+0x1255>
     6b48a684:	call   6b48f9e0 <_assert>
     6b48a689:	jmp    6b489608 <vec0Filter+0x5f8>
     6b48a68e:	xchg   %ax,%ax
     6b48a690:	lea    0xa96e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a697:	mov    $0xd9d,%r8d
+    6b48a697:	mov    $0xda3,%r8d
     6b48a69d:	lea    0xbd08(%rip),%rcx        # 6b4963ac <.rdata+0x13ac>
     6b48a6a4:	call   6b48f9e0 <_assert>
     6b48a6a9:	jmp    6b48965a <vec0Filter+0x64a>
     6b48a6ae:	xchg   %ax,%ax
     6b48a6b0:	lea    0xa94e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a6b7:	mov    $0xaff,%r8d
+    6b48a6b7:	mov    $0xb05,%r8d
     6b48a6bd:	lea    0xabba(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a6c4:	call   6b48f9e0 <_assert>
     6b48a6c9:	jmp    6b48a576 <vec0Filter+0x1566>
     6b48a6ce:	mov    %r14d,%ecx
     6b48a6d1:	call   *%rsi
     6b48a6d3:	test   %rax,%rax
     6b48a6d6:	mov    %rax,%r14
     6b48a6d9:	jne    6b4896e0 <vec0Filter+0x6d0>
     6b48a6df:	lea    0xa91f(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a6e6:	mov    $0xd9d,%r8d
+    6b48a6e6:	mov    $0xda3,%r8d
     6b48a6ec:	lea    0xbcb9(%rip),%rcx        # 6b4963ac <.rdata+0x13ac>
     6b48a6f3:	call   6b48f9e0 <_assert>
     6b48a6f8:	jmp    6b4896e0 <vec0Filter+0x6d0>
     6b48a6fd:	xor    %eax,%eax
     6b48a6ff:	jmp    6b4896ae <vec0Filter+0x69e>
     6b48a704:	lea    0xa8fa(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a70b:	mov    $0xd88,%r8d
+    6b48a70b:	mov    $0xd8e,%r8d
     6b48a711:	lea    0xbb2f(%rip),%rcx        # 6b496247 <.rdata+0x1247>
     6b48a718:	call   6b48f9e0 <_assert>
     6b48a71d:	jmp    6b4894ad <vec0Filter+0x49d>
     6b48a722:	lea    0xa8dc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48a729:	mov    $0xd8a,%r8d
+    6b48a729:	mov    $0xd90,%r8d
     6b48a72f:	lea    0xab48(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48a736:	call   6b48f9e0 <_assert>
     6b48a73b:	jmp    6b4894e0 <vec0Filter+0x4d0>
     6b48a740:	mov    $0x2,%ecx
     6b48a745:	call   *0x9bd5(%rip)        # 6b494320 <__imp___acrt_iob_func>
     6b48a74b:	lea    0xbb4f(%rip),%r8        # 6b4962a1 <.rdata+0x12a1>
     6b48a752:	lea    0xaa37(%rip),%rdx        # 6b495190 <.rdata+0x190>
@@ -12703,15 +12703,15 @@
     6b48ae0e:	lea    0x7(%rcx),%edx
     6b48ae11:	test   %ecx,%ecx
     6b48ae13:	cmovns %ecx,%edx
     6b48ae16:	sar    $0x3,%edx
     6b48ae19:	cmp    %edx,%eax
     6b48ae1b:	je     6b48ae36 <vec0Filter_knn+0x636>
     6b48ae1d:	lea    0xa1e1(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ae24:	mov    $0xdc0,%r8d
+    6b48ae24:	mov    $0xdc6,%r8d
     6b48ae2a:	lea    0xb487(%rip),%rcx        # 6b4962b8 <.rdata+0x12b8>
     6b48ae31:	call   6b48f9e0 <_assert>
     6b48ae36:	mov    0xf1e3(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48ae3d:	mov    $0x2,%edx
     6b48ae42:	mov    0x168(%rsp),%rcx
     6b48ae4a:	call   *0x98(%rax)
     6b48ae50:	mov    $0x2,%edx
@@ -12721,15 +12721,15 @@
     6b48ae67:	call   *0xa0(%rax)
     6b48ae6d:	movslq 0x2cc(%rsi),%rdx
     6b48ae74:	cltq
     6b48ae76:	shl    $0x3,%rdx
     6b48ae7a:	cmp    %rax,%rdx
     6b48ae7d:	je     6b48ae98 <vec0Filter_knn+0x698>
     6b48ae7f:	lea    0xa17f(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ae86:	mov    $0xdc3,%r8d
+    6b48ae86:	mov    $0xdc9,%r8d
     6b48ae8c:	lea    0xb44d(%rip),%rcx        # 6b4962e0 <.rdata+0x12e0>
     6b48ae93:	call   6b48f9e0 <_assert>
     6b48ae98:	mov    0x50(%rsp),%rax
     6b48ae9d:	lea    0xb2c4(%rip),%r9        # 6b496168 <.rdata+0x1168>
     6b48aea4:	mov    0x28(%rsi),%rdx
     6b48aea8:	mov    0x18(%rsi),%rcx
     6b48aeac:	mov    0x48(%rsi,%rax,8),%r8
@@ -12760,15 +12760,15 @@
     6b48af36:	cmovne 0x68(%rsp),%rax
     6b48af3c:	mov    %rax,0x68(%rsp)
     6b48af41:	mov    0x68(%rsp),%rax
     6b48af46:	imul   %rdx,%rax
     6b48af4a:	cmp    %rax,%r8
     6b48af4d:	je     6b48af68 <vec0Filter_knn+0x768>
     6b48af4f:	lea    0xa0af(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48af56:	mov    $0xdcc,%r8d
+    6b48af56:	mov    $0xdd2,%r8d
     6b48af5c:	lea    0xb3ad(%rip),%rcx        # 6b496310 <.rdata+0x1310>
     6b48af63:	call   6b48f9e0 <_assert>
     6b48af68:	cmp    %rbx,0x78(%rsp)
     6b48af6d:	mov    0xf0ac(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48af74:	jge    6b48afb0 <vec0Filter_knn+0x7b0>
     6b48af76:	mov    0x58(%rsp),%rcx
     6b48af7b:	test   %rcx,%rcx
@@ -12952,20 +12952,20 @@
     6b48b2eb:	mov    %rbx,%rcx
     6b48b2ee:	call   *0x1d0(%rax)
     6b48b2f4:	mov    0xed25(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48b2fb:	mov    0x160(%rsp),%rcx
     6b48b303:	call   *0x3d0(%rax)
     6b48b309:	jmp    6b48ad90 <vec0Filter_knn+0x590>
     6b48b30e:	lea    0x9cf0(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b315:	mov    $0xd76,%r8d
+    6b48b315:	mov    $0xd7c,%r8d
     6b48b31b:	lea    0xaef6(%rip),%rcx        # 6b496218 <.rdata+0x1218>
     6b48b322:	call   6b48f9e0 <_assert>
     6b48b327:	jmp    6b48a937 <vec0Filter_knn+0x137>
     6b48b32c:	lea    0x9cd2(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b333:	mov    $0xd75,%r8d
+    6b48b333:	mov    $0xd7b,%r8d
     6b48b339:	lea    0xaea8(%rip),%rcx        # 6b4961e8 <.rdata+0x11e8>
     6b48b340:	call   6b48f9e0 <_assert>
     6b48b345:	jmp    6b48a918 <vec0Filter_knn+0x118>
     6b48b34a:	mov    0x120(%rsp),%rax
     6b48b352:	mov    0x230(%rsp),%rdi
     6b48b35a:	movq   $0x0,(%rax)
     6b48b361:	mov    %rax,0x18(%rdi)
@@ -13267,21 +13267,21 @@
     6b48b845:	jbe    6b48b69c <vec0Filter_knn+0xe9c>
     6b48b84b:	jmp    6b48b7dc <vec0Filter_knn+0xfdc>
     6b48b84d:	nopl   (%rax)
     6b48b850:	mov    %rax,0x68(%rsp)
     6b48b855:	jmp    6b48af41 <vec0Filter_knn+0x741>
     6b48b85a:	nopw   0x0(%rax,%rax,1)
     6b48b860:	lea    0x979e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b867:	mov    $0xdd8,%r8d
+    6b48b867:	mov    $0xdde,%r8d
     6b48b86d:	lea    0x9a0a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48b874:	call   6b48f9e0 <_assert>
     6b48b879:	jmp    6b48afd1 <vec0Filter_knn+0x7d1>
     6b48b87e:	xchg   %ax,%ax
     6b48b880:	lea    0x977e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b887:	mov    $0xdc9,%r8d
+    6b48b887:	mov    $0xdcf,%r8d
     6b48b88d:	lea    0x99ea(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48b894:	call   6b48f9e0 <_assert>
     6b48b899:	jmp    6b48aee0 <vec0Filter_knn+0x6e0>
     6b48b89e:	xchg   %ax,%ax
     6b48b8a0:	shr    $0x3,%rax
     6b48b8a4:	mov    %rax,0x68(%rsp)
     6b48b8a9:	jmp    6b48af41 <vec0Filter_knn+0x741>
@@ -13294,37 +13294,37 @@
     6b48b8c9:	mov    %r8,0x0(%rbp,%rax,2)
     6b48b8ce:	movss  %xmm0,(%r15,%rax,1)
     6b48b8d4:	add    $0x4,%rax
     6b48b8d8:	cmp    %r9,%rax
     6b48b8db:	jne    6b48b8c0 <vec0Filter_knn+0x10c0>
     6b48b8dd:	jmp    6b48b2b2 <vec0Filter_knn+0xab2>
     6b48b8e2:	lea    0x971c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b8e9:	mov    $0xddc,%r8d
+    6b48b8e9:	mov    $0xde2,%r8d
     6b48b8ef:	lea    0xaa87(%rip),%rcx        # 6b49637d <.rdata+0x137d>
     6b48b8f6:	call   6b48f9e0 <_assert>
     6b48b8fb:	mov    0x2cc(%rsi),%eax
     6b48b901:	test   %eax,%eax
     6b48b903:	jg     6b48b005 <vec0Filter_knn+0x805>
     6b48b909:	nopl   0x0(%rax)
     6b48b910:	lea    0x178(%rsp),%rax
     6b48b918:	mov    %rax,0x60(%rsp)
     6b48b91d:	jmp    6b48b0d1 <vec0Filter_knn+0x8d1>
     6b48b922:	lea    0x96dc(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b929:	mov    $0xe29,%r8d
+    6b48b929:	mov    $0xe2f,%r8d
     6b48b92f:	lea    0xaa57(%rip),%rcx        # 6b49638d <.rdata+0x138d>
     6b48b936:	call   6b48f9e0 <_assert>
     6b48b93b:	jmp    6b48b0f1 <vec0Filter_knn+0x8f1>
     6b48b940:	pxor   %xmm7,%xmm7
     6b48b944:	jmp    6b48b090 <vec0Filter_knn+0x890>
     6b48b949:	lea    0x96b5(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48b950:	mov    $0xdd3,%r8d
+    6b48b950:	mov    $0xdd9,%r8d
     6b48b956:	lea    0xaa14(%rip),%rcx        # 6b496371 <.rdata+0x1371>
     6b48b95d:	call   6b48f9e0 <_assert>
     6b48b962:	jmp    6b48afa4 <vec0Filter_knn+0x7a4>
-    6b48b967:	mov    $0xd8f,%r8d
+    6b48b967:	mov    $0xd95,%r8d
     6b48b96d:	mov    %r14,%rdx
     6b48b970:	mov    %r13,%rcx
     6b48b973:	call   6b48f9e0 <_assert>
     6b48b978:	jmp    6b48aa2b <vec0Filter_knn+0x22b>
     6b48b97d:	mov    0xe69c(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48b984:	mov    0x58(%rsp),%rcx
     6b48b989:	call   *0x1d0(%rax)
@@ -13372,74 +13372,74 @@
     6b48ba61:	pxor   %xmm5,%xmm5
     6b48ba65:	pxor   %xmm4,%xmm4
     6b48ba69:	jmp    6b48b4ec <vec0Filter_knn+0xcec>
     6b48ba6e:	xor    %eax,%eax
     6b48ba70:	pxor   %xmm1,%xmm1
     6b48ba74:	jmp    6b48b77d <vec0Filter_knn+0xf7d>
     6b48ba79:	lea    0x9585(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ba80:	mov    $0xd60,%r8d
+    6b48ba80:	mov    $0xd66,%r8d
     6b48ba86:	lea    0xa751(%rip),%rcx        # 6b4961de <.rdata+0x11de>
     6b48ba8d:	call   6b48f9e0 <_assert>
     6b48ba92:	jmp    6b48a86d <vec0Filter_knn+0x6d>
     6b48ba97:	lea    0x9567(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ba9e:	mov    $0xd79,%r8d
+    6b48ba9e:	mov    $0xd7f,%r8d
     6b48baa4:	lea    0xa795(%rip),%rcx        # 6b496240 <.rdata+0x1240>
     6b48baab:	call   6b48f9e0 <_assert>
     6b48bab0:	jmp    6b48a95c <vec0Filter_knn+0x15c>
     6b48bab5:	lea    0x9549(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48babc:	mov    $0xd97,%r8d
+    6b48babc:	mov    $0xd9d,%r8d
     6b48bac2:	lea    0xa78c(%rip),%rcx        # 6b496255 <.rdata+0x1255>
     6b48bac9:	call   6b48f9e0 <_assert>
     6b48bace:	jmp    6b48aaf1 <vec0Filter_knn+0x2f1>
     6b48bad3:	mov    %r14d,%ecx
     6b48bad6:	call   *%rbx
     6b48bad8:	test   %rax,%rax
     6b48badb:	mov    %rax,%r15
     6b48bade:	jne    6b48abd5 <vec0Filter_knn+0x3d5>
     6b48bae4:	lea    0x951a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48baeb:	mov    $0xd9d,%r8d
+    6b48baeb:	mov    $0xda3,%r8d
     6b48baf1:	lea    0xa8b4(%rip),%rcx        # 6b4963ac <.rdata+0x13ac>
     6b48baf8:	call   6b48f9e0 <_assert>
     6b48bafd:	jmp    6b48abd5 <vec0Filter_knn+0x3d5>
     6b48bb02:	mov    $0x7,%eax
     6b48bb07:	jmp    6b48b367 <vec0Filter_knn+0xb67>
     6b48bb0c:	lea    0x94f2(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bb13:	mov    $0xe41,%r8d
+    6b48bb13:	mov    $0xe47,%r8d
     6b48bb19:	lea    0x975e(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48bb20:	call   6b48f9e0 <_assert>
     6b48bb25:	jmp    6b48b9ac <vec0Filter_knn+0x11ac>
     6b48bb2a:	lea    0x94d4(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bb31:	mov    $0xdb0,%r8d
+    6b48bb31:	mov    $0xdb6,%r8d
     6b48bb37:	lea    0x9740(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48bb3e:	call   6b48f9e0 <_assert>
     6b48bb43:	jmp    6b48ac44 <vec0Filter_knn+0x444>
     6b48bb48:	lea    0x94b6(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bb4f:	mov    $0xd91,%r8d
+    6b48bb4f:	mov    $0xd97,%r8d
     6b48bb55:	lea    0xa06d(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48bb5c:	call   6b48f9e0 <_assert>
     6b48bb61:	jmp    6b48aab3 <vec0Filter_knn+0x2b3>
     6b48bb66:	lea    0x9498(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bb6d:	mov    $0xdad,%r8d
+    6b48bb6d:	mov    $0xdb3,%r8d
     6b48bb73:	lea    0xa0a5(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b48bb7a:	call   6b48f9e0 <_assert>
     6b48bb7f:	jmp    6b48abfd <vec0Filter_knn+0x3fd>
     6b48bb84:	lea    0x947a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bb8b:	mov    $0xd9d,%r8d
+    6b48bb8b:	mov    $0xda3,%r8d
     6b48bb91:	lea    0xa814(%rip),%rcx        # 6b4963ac <.rdata+0x13ac>
     6b48bb98:	call   6b48f9e0 <_assert>
     6b48bb9d:	jmp    6b48ab43 <vec0Filter_knn+0x343>
     6b48bba2:	lea    0x945c(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bba9:	mov    $0xd88,%r8d
+    6b48bba9:	mov    $0xd8e,%r8d
     6b48bbaf:	lea    0xa691(%rip),%rcx        # 6b496247 <.rdata+0x1247>
     6b48bbb6:	call   6b48f9e0 <_assert>
     6b48bbbb:	jmp    6b48a988 <vec0Filter_knn+0x188>
     6b48bbc0:	xor    %eax,%eax
     6b48bbc2:	jmp    6b48ab9e <vec0Filter_knn+0x39e>
     6b48bbc7:	lea    0x9437(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bbce:	mov    $0xd8a,%r8d
+    6b48bbce:	mov    $0xd90,%r8d
     6b48bbd4:	lea    0x96a3(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48bbdb:	call   6b48f9e0 <_assert>
     6b48bbe0:	jmp    6b48a9ba <vec0Filter_knn+0x1ba>
     6b48bbe5:	movsd  %xmm1,0x128(%rsp)
     6b48bbee:	movapd %xmm7,%xmm0
     6b48bbf2:	call   6b48f770 <sqrt>
     6b48bbf7:	movsd  0x128(%rsp),%xmm1
@@ -13522,15 +13522,15 @@
     6b48bd6b:	add    $0x38,%rsp
     6b48bd6f:	pop    %rbx
     6b48bd70:	pop    %rsi
     6b48bd71:	pop    %rdi
     6b48bd72:	pop    %rbp
     6b48bd73:	ret
     6b48bd74:	lea    0x928a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bd7b:	mov    $0xe6b,%r8d
+    6b48bd7b:	mov    $0xe71,%r8d
     6b48bd81:	lea    0x94f6(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48bd88:	call   6b48f9e0 <_assert>
     6b48bd8d:	jmp    6b48bd46 <vec0Filter_fullscan+0xa6>
     6b48bd8f:	nop
     6b48bd90:	mov    (%rbx),%rcx
     6b48bd93:	mov    $0x1,%eax
     6b48bd98:	test   %rcx,%rcx
@@ -13551,21 +13551,21 @@
     6b48bdc8:	add    $0x38,%rsp
     6b48bdcc:	pop    %rbx
     6b48bdcd:	pop    %rsi
     6b48bdce:	pop    %rdi
     6b48bdcf:	pop    %rbp
     6b48bdd0:	ret
     6b48bdd1:	lea    0x922d(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bdd8:	mov    $0xe68,%r8d
+    6b48bdd8:	mov    $0xe6e,%r8d
     6b48bdde:	lea    0x9e3a(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b48bde5:	call   6b48f9e0 <_assert>
     6b48bdea:	jmp    6b48bd0a <vec0Filter_fullscan+0x6a>
     6b48bdef:	nop
     6b48bdf0:	lea    0x920e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bdf7:	mov    $0xaff,%r8d
+    6b48bdf7:	mov    $0xb05,%r8d
     6b48bdfd:	lea    0x947a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48be04:	call   6b48f9e0 <_assert>
     6b48be09:	jmp    6b48bdae <vec0Filter_fullscan+0x10e>
     6b48be0b:	nopl   0x0(%rax,%rax,1)
 
 000000006b48be10 <vec0Filter_point>:
     6b48be10:	push   %r15
@@ -13578,15 +13578,15 @@
     6b48be1b:	push   %rbx
     6b48be1c:	sub    $0x38,%rsp
     6b48be20:	cmpl   $0x1,0xa0(%rsp)
     6b48be28:	mov    %rcx,%r14
     6b48be2b:	mov    %rdx,%rbp
     6b48be2e:	je     6b48be49 <vec0Filter_point+0x39>
     6b48be30:	lea    0x91ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48be37:	mov    $0xe7b,%r8d
+    6b48be37:	mov    $0xe81,%r8d
     6b48be3d:	lea    0x9238(%rip),%rcx        # 6b49507c <.rdata+0x7c>
     6b48be44:	call   6b48f9e0 <_assert>
     6b48be49:	mov    0xa8(%rsp),%rax
     6b48be51:	mov    (%rax),%rcx
     6b48be54:	mov    0xe1c5(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48be5b:	call   *0x358(%rax)
     6b48be61:	movl   $0x1,0x8(%r14)
@@ -13631,15 +13631,15 @@
     6b48befe:	pop    %rbp
     6b48beff:	pop    %r12
     6b48bf01:	pop    %r13
     6b48bf03:	pop    %r14
     6b48bf05:	pop    %r15
     6b48bf07:	ret
     6b48bf08:	nopl   0x0(%rax,%rax,1)
-    6b48bf10:	mov    $0xe88,%r8d
+    6b48bf10:	mov    $0xe8e,%r8d
     6b48bf16:	mov    %r15,%rdx
     6b48bf19:	mov    %rdi,%rcx
     6b48bf1c:	call   6b48f9e0 <_assert>
     6b48bf21:	add    $0x1,%ebx
     6b48bf24:	add    $0x8,%rsi
     6b48bf28:	cmp    0x2c8(%rbp),%ebx
     6b48bf2e:	jl     6b48beb5 <vec0Filter_point+0xa5>
@@ -13678,30 +13678,30 @@
     6b48bfb5:	call   *0x60(%rax)
     6b48bfb8:	mov    0xe061(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48bfbf:	mov    0x2e0(%rbx),%rcx
     6b48bfc6:	call   *0x2f0(%rax)
     6b48bfcc:	cmp    $0x65,%eax
     6b48bfcf:	je     6b48bfea <vec0Update_InsertRowidStep+0xaa>
     6b48bfd1:	lea    0x902d(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48bfd8:	mov    $0xf62,%r8d
+    6b48bfd8:	mov    $0xf68,%r8d
     6b48bfde:	lea    0x9be4(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48bfe5:	call   6b48f9e0 <_assert>
     6b48bfea:	mov    0xe02f(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48bff1:	mov    0x18(%rbx),%rcx
     6b48bff5:	call   *0x208(%rax)
     6b48bffb:	mov    %rax,(%rdi)
     6b48bffe:	xor    %eax,%eax
     6b48c000:	add    $0x20,%rsp
     6b48c004:	pop    %rbx
     6b48c005:	pop    %rsi
     6b48c006:	pop    %rdi
     6b48c007:	ret
     6b48c008:	nopl   0x0(%rax,%rax,1)
     6b48c010:	lea    0x8fee(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c017:	mov    $0xf59,%r8d
+    6b48c017:	mov    $0xf5f,%r8d
     6b48c01d:	lea    0xa39c(%rip),%rcx        # 6b4963c0 <.rdata+0x13c0>
     6b48c024:	call   6b48f9e0 <_assert>
     6b48c029:	jmp    6b48bf77 <vec0Update_InsertRowidStep+0x37>
     6b48c02e:	xchg   %ax,%ax
     6b48c030:	call   *%rax
     6b48c032:	mov    %rsi,%rcx
     6b48c035:	cmp    $0x1,%eax
@@ -13718,20 +13718,20 @@
     6b48c072:	call   *0x3b0(%rax)
     6b48c078:	mov    0xdfa1(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c07f:	mov    0x2e0(%rbx),%rcx
     6b48c086:	call   *0x2f0(%rax)
     6b48c08c:	cmp    $0x65,%eax
     6b48c08f:	je     6b48bfea <vec0Update_InsertRowidStep+0xaa>
     6b48c095:	lea    0x8f69(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c09c:	mov    $0xf7f,%r8d
+    6b48c09c:	mov    $0xf85,%r8d
     6b48c0a2:	lea    0x9b20(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48c0a9:	call   6b48f9e0 <_assert>
     6b48c0ae:	jmp    6b48bfea <vec0Update_InsertRowidStep+0xaa>
     6b48c0b3:	lea    0x8f4b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c0ba:	mov    $0xf76,%r8d
+    6b48c0ba:	mov    $0xf7c,%r8d
     6b48c0c0:	lea    0xa321(%rip),%rcx        # 6b4963e8 <.rdata+0x13e8>
     6b48c0c7:	call   6b48f9e0 <_assert>
     6b48c0cc:	jmp    6b48c050 <vec0Update_InsertRowidStep+0x110>
     6b48c0ce:	xchg   %ax,%ax
     6b48c0d0:	call   *0x358(%rax)
     6b48c0d6:	mov    0x2d8(%rbx),%rcx
     6b48c0dd:	mov    %rax,%rsi
@@ -13747,15 +13747,15 @@
     6b48c117:	call   *0x28(%rax)
     6b48c11a:	mov    0xdeff(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c121:	mov    0x2d8(%rbx),%rcx
     6b48c128:	call   *0x2f0(%rax)
     6b48c12e:	cmp    $0x65,%eax
     6b48c131:	je     6b48c14c <vec0Update_InsertRowidStep+0x20c>
     6b48c133:	lea    0x8ecb(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c13a:	mov    $0xf71,%r8d
+    6b48c13a:	mov    $0xf77,%r8d
     6b48c140:	lea    0x9a82(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48c147:	call   6b48f9e0 <_assert>
     6b48c14c:	xor    %eax,%eax
     6b48c14e:	mov    %rsi,(%rdi)
     6b48c151:	add    $0x20,%rsp
     6b48c155:	pop    %rbx
     6b48c156:	pop    %rsi
@@ -13782,29 +13782,29 @@
     6b48c195:	call   *0x268(%rax)
     6b48c19b:	mov    0xde7e(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c1a2:	mov    0x2d0(%rbx),%rcx
     6b48c1a9:	call   *0x2f0(%rax)
     6b48c1af:	cmp    $0x64,%eax
     6b48c1b2:	je     6b48c1cd <vec0Update_InsertNextAvailableStep+0x6d>
     6b48c1b4:	lea    0x8e4a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c1bb:	mov    $0xfa5,%r8d
+    6b48c1bb:	mov    $0xfab,%r8d
     6b48c1c1:	lea    0x99e2(%rip),%rcx        # 6b495baa <.rdata+0xbaa>
     6b48c1c8:	call   6b48f9e0 <_assert>
     6b48c1cd:	mov    0xde4c(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c1d4:	xor    %edx,%edx
     6b48c1d6:	mov    0x2d0(%rbx),%rcx
     6b48c1dd:	call   *0xe8(%rax)
     6b48c1e3:	mov    0x2d0(%rbx),%rcx
     6b48c1ea:	mov    %rax,0x0(%rbp)
     6b48c1ee:	mov    0xde2b(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c1f5:	call   *0x2f0(%rax)
     6b48c1fb:	cmp    $0x65,%eax
     6b48c1fe:	je     6b48c219 <vec0Update_InsertNextAvailableStep+0xb9>
     6b48c200:	lea    0x8dfe(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c207:	mov    $0xfa8,%r8d
+    6b48c207:	mov    $0xfae,%r8d
     6b48c20d:	lea    0x99b5(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48c214:	call   6b48f9e0 <_assert>
     6b48c219:	mov    %rsi,0x30(%rsp)
     6b48c21e:	mov    0x28(%rbx),%rdx
     6b48c222:	lea    0xa1e5(%rip),%r9        # 6b49640e <.rdata+0x140e>
     6b48c229:	movl   $0x1,0x28(%rsp)
     6b48c231:	mov    0x0(%rbp),%rax
@@ -13823,15 +13823,15 @@
     6b48c270:	lea    0x7(%rdx),%eax
     6b48c273:	test   %edx,%edx
     6b48c275:	cmovns %edx,%eax
     6b48c278:	sar    $0x3,%eax
     6b48c27b:	cmp    %eax,%r13d
     6b48c27e:	je     6b48c299 <vec0Update_InsertNextAvailableStep+0x139>
     6b48c280:	lea    0x8d7e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c287:	mov    $0xfaf,%r8d
+    6b48c287:	mov    $0xfb5,%r8d
     6b48c28d:	lea    0xa024(%rip),%rcx        # 6b4962b8 <.rdata+0x12b8>
     6b48c294:	call   6b48f9e0 <_assert>
     6b48c299:	mov    0xdd80(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c2a0:	mov    %r13d,%ecx
     6b48c2a3:	call   *0x220(%rax)
     6b48c2a9:	test   %rax,%rax
     6b48c2ac:	mov    %rax,(%rdi)
@@ -13891,21 +13891,21 @@
     6b48c362:	pop    %rdi
     6b48c363:	pop    %rbp
     6b48c364:	pop    %r12
     6b48c366:	pop    %r13
     6b48c368:	ret
     6b48c369:	nopl   0x0(%rax)
     6b48c370:	lea    0x8c8e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c377:	mov    $0xfac,%r8d
+    6b48c377:	mov    $0xfb2,%r8d
     6b48c37d:	lea    0x8efa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c384:	call   6b48f9e0 <_assert>
     6b48c389:	jmp    6b48c257 <vec0Update_InsertNextAvailableStep+0xf7>
     6b48c38e:	xchg   %ax,%ax
     6b48c390:	lea    0x8c6e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c397:	mov    $0xfb6,%r8d
+    6b48c397:	mov    $0xfbc,%r8d
     6b48c39d:	lea    0x8eda(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c3a4:	call   6b48f9e0 <_assert>
     6b48c3a9:	jmp    6b48c2d6 <vec0Update_InsertNextAvailableStep+0x176>
     6b48c3ae:	xchg   %ax,%ax
     6b48c3b0:	cmpq   $0xffffffffffffffff,(%r12)
     6b48c3b5:	jne    6b48c35a <vec0Update_InsertNextAvailableStep+0x1fa>
     6b48c3b7:	mov    %rbp,%rdx
@@ -13952,36 +13952,36 @@
     6b48c46f:	mov    %rax,(%rdi)
     6b48c472:	mov    %rax,%rdx
     6b48c475:	mov    0xdba4(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c47c:	call   *0x3e0(%rax)
     6b48c482:	test   %eax,%eax
     6b48c484:	je     6b48c35a <vec0Update_InsertNextAvailableStep+0x1fa>
     6b48c48a:	lea    0x8b74(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c491:	mov    $0xfd7,%r8d
+    6b48c491:	mov    $0xfdd,%r8d
     6b48c497:	lea    0x8de0(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c49e:	call   6b48f9e0 <_assert>
     6b48c4a3:	jmp    6b48c35a <vec0Update_InsertNextAvailableStep+0x1fa>
     6b48c4a8:	lea    0x8b56(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c4af:	mov    $0xfd3,%r8d
+    6b48c4af:	mov    $0xfd9,%r8d
     6b48c4b5:	lea    0x9dfc(%rip),%rcx        # 6b4962b8 <.rdata+0x12b8>
     6b48c4bc:	call   6b48f9e0 <_assert>
     6b48c4c1:	jmp    6b48c457 <vec0Update_InsertNextAvailableStep+0x2f7>
     6b48c4c3:	lea    0x8b3b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c4ca:	mov    $0xfd1,%r8d
+    6b48c4ca:	mov    $0xfd7,%r8d
     6b48c4d0:	lea    0x8da7(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c4d7:	call   6b48f9e0 <_assert>
     6b48c4dc:	jmp    6b48c430 <vec0Update_InsertNextAvailableStep+0x2d0>
     6b48c4e1:	lea    0x8b1d(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c4e8:	mov    $0xfc7,%r8d
+    6b48c4e8:	mov    $0xfcd,%r8d
     6b48c4ee:	lea    0x8e65(%rip),%rcx        # 6b49535a <.rdata+0x35a>
     6b48c4f5:	call   6b48f9e0 <_assert>
     6b48c4fa:	jmp    6b48c3ca <vec0Update_InsertNextAvailableStep+0x26a>
     6b48c4ff:	nop
     6b48c500:	lea    0x8afe(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c507:	mov    $0xfb2,%r8d
+    6b48c507:	mov    $0xfb8,%r8d
     6b48c50d:	lea    0x9f03(%rip),%rcx        # 6b496417 <.rdata+0x1417>
     6b48c514:	call   6b48f9e0 <_assert>
     6b48c519:	mov    (%rdi),%rax
     6b48c51c:	jmp    6b48c2b5 <vec0Update_InsertNextAvailableStep+0x155>
     6b48c521:	mov    $0x1,%eax
     6b48c526:	jmp    6b48c350 <vec0Update_InsertNextAvailableStep+0x1f0>
     6b48c52b:	mov    $0x2,%eax
@@ -14081,15 +14081,15 @@
     6b48c6d2:	mov    0xd8(%rbx,%r12,1),%r9
     6b48c6da:	movslq 0x2cc(%rbx),%rdx
     6b48c6e1:	mov    %eax,%eax
     6b48c6e3:	imul   %r9,%rdx
     6b48c6e7:	cmp    %rdx,%rax
     6b48c6ea:	je     6b48c7d0 <vec0Update_InsertWriteFinalStep+0x260>
     6b48c6f0:	lea    0x890e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c6f7:	mov    $0x1024,%r8d
+    6b48c6f7:	mov    $0x102a,%r8d
     6b48c6fd:	lea    0x9dac(%rip),%rcx        # 6b4964b0 <.rdata+0x14b0>
     6b48c704:	call   6b48f9e0 <_assert>
     6b48c709:	mov    0xe0(%rbx,%r12,1),%r8d
     6b48c711:	mov    0xd8(%rbx,%r12,1),%r9
     6b48c719:	mov    0x58(%rsp),%rcx
     6b48c71e:	mov    0xd8fb(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c725:	mov    0xd0(%rsp),%rdx
@@ -14103,18 +14103,18 @@
     6b48c74e:	mov    %ebp,%r8d
     6b48c751:	imul   %r9d,%esi
     6b48c755:	mov    %esi,%r9d
     6b48c758:	call   *0x3e8(%rax)
     6b48c75e:	test   %eax,%eax
     6b48c760:	je     6b48c63c <vec0Update_InsertWriteFinalStep+0xcc>
     6b48c766:	lea    0x8898(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c76d:	mov    $0xff3,%r8d
+    6b48c76d:	mov    $0xff9,%r8d
     6b48c773:	lea    0x8b04(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c77a:	call   6b48f9e0 <_assert>
-    6b48c77f:	mov    $0x102f,%r8d
+    6b48c77f:	mov    $0x1035,%r8d
     6b48c785:	lea    0x8879(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b48c78c:	lea    0x8aeb(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c793:	call   6b48f9e0 <_assert>
     6b48c798:	jmp    6b48c63c <vec0Update_InsertWriteFinalStep+0xcc>
     6b48c79d:	nopl   (%rax)
     6b48c7a0:	cmp    $0xdf,%r8d
     6b48c7a7:	jne    6b48c628 <vec0Update_InsertWriteFinalStep+0xb8>
@@ -14125,29 +14125,29 @@
     6b48c7c8:	nopl   0x0(%rax,%rax,1)
     6b48c7d0:	mov    0xe0(%rbx,%r12,1),%r8d
     6b48c7d8:	mov    0x58(%rsp),%rcx
     6b48c7dd:	mov    0xd83c(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c7e4:	jmp    6b48c725 <vec0Update_InsertWriteFinalStep+0x1b5>
     6b48c7e9:	nopl   0x0(%rax)
     6b48c7f0:	lea    0x880e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c7f7:	mov    $0x101a,%r8d
+    6b48c7f7:	mov    $0x1020,%r8d
     6b48c7fd:	lea    0x8a7a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48c804:	call   6b48f9e0 <_assert>
     6b48c809:	jmp    6b48c699 <vec0Update_InsertWriteFinalStep+0x129>
     6b48c80e:	xchg   %ax,%ax
     6b48c810:	call   *0x3c8(%rax)
     6b48c816:	mov    0xd8(%rbx,%r12,1),%r9
     6b48c81e:	movslq 0x2cc(%rbx),%rdx
     6b48c825:	mov    %eax,%eax
     6b48c827:	imul   %r9,%rdx
     6b48c82b:	shl    $0x2,%rdx
     6b48c82f:	cmp    %rdx,%rax
     6b48c832:	je     6b48c7d0 <vec0Update_InsertWriteFinalStep+0x260>
     6b48c834:	lea    0x87ca(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c83b:	mov    $0x1020,%r8d
+    6b48c83b:	mov    $0x1026,%r8d
     6b48c841:	lea    0x9bf0(%rip),%rcx        # 6b496438 <.rdata+0x1438>
     6b48c848:	jmp    6b48c704 <vec0Update_InsertWriteFinalStep+0x194>
     6b48c84d:	nopl   (%rax)
     6b48c850:	mov    %r9,%rbp
     6b48c853:	imul   %r14,%r9
     6b48c857:	shr    $0x3,%rbp
     6b48c85b:	shr    $0x3,%r9
@@ -14159,15 +14159,15 @@
     6b48c87e:	movslq 0x2cc(%rbx),%rdx
     6b48c885:	mov    %eax,%eax
     6b48c887:	imul   %r9,%rdx
     6b48c88b:	shr    $0x3,%rdx
     6b48c88f:	cmp    %rdx,%rax
     6b48c892:	je     6b48c7d0 <vec0Update_InsertWriteFinalStep+0x260>
     6b48c898:	lea    0x8766(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c89f:	mov    $0x1028,%r8d
+    6b48c89f:	mov    $0x102e,%r8d
     6b48c8a5:	lea    0x9c7c(%rip),%rcx        # 6b496528 <.rdata+0x1528>
     6b48c8ac:	jmp    6b48c704 <vec0Update_InsertWriteFinalStep+0x194>
     6b48c8b1:	mov    0x28(%rbx),%rdx
     6b48c8b5:	mov    %r15,0x30(%rsp)
     6b48c8ba:	lea    0x9b6c(%rip),%r9        # 6b49642d <.rdata+0x142d>
     6b48c8c1:	mov    0xd758(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c8c8:	movl   $0x1,0x28(%rsp)
@@ -14182,15 +14182,15 @@
     6b48c8f7:	call   *0x3c8(%rax)
     6b48c8fd:	movslq 0x2cc(%rbx),%rdx
     6b48c904:	cltq
     6b48c906:	shl    $0x3,%rdx
     6b48c90a:	cmp    %rdx,%rax
     6b48c90d:	je     6b48c928 <vec0Update_InsertWriteFinalStep+0x3b8>
     6b48c90f:	lea    0x86ef(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48c916:	mov    $0x1038,%r8d
+    6b48c916:	mov    $0x103e,%r8d
     6b48c91c:	lea    0x9c75(%rip),%rcx        # 6b496598 <.rdata+0x1598>
     6b48c923:	call   6b48f9e0 <_assert>
     6b48c928:	mov    0xd6f1(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c92f:	lea    0xc8(%rsp),%rdx
     6b48c937:	mov    $0x8,%r8d
     6b48c93d:	lea    0x0(,%r14,8),%r9d
     6b48c945:	mov    0x58(%rsp),%rcx
@@ -14223,15 +14223,15 @@
     6b48c9df:	call   *0x28(%rax)
     6b48c9e2:	mov    0xd637(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48c9e9:	mov    0x2e8(%rbx),%rcx
     6b48c9f0:	call   *0x2f0(%rax)
     6b48c9f6:	cmp    $0x65,%eax
     6b48c9f9:	je     6b48ca14 <vec0Update_InsertWriteFinalStep+0x4a4>
     6b48c9fb:	lea    0x8603(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ca02:	mov    $0x1046,%r8d
+    6b48ca02:	mov    $0x104c,%r8d
     6b48ca08:	lea    0x91ba(%rip),%rcx        # 6b495bc9 <.rdata+0xbc9>
     6b48ca0f:	call   6b48f9e0 <_assert>
     6b48ca14:	xor    %eax,%eax
     6b48ca16:	add    $0x68,%rsp
     6b48ca1a:	pop    %rbx
     6b48ca1b:	pop    %rsi
     6b48ca1c:	pop    %rdi
@@ -14239,27 +14239,27 @@
     6b48ca1e:	pop    %r12
     6b48ca20:	pop    %r13
     6b48ca22:	pop    %r14
     6b48ca24:	pop    %r15
     6b48ca26:	ret
     6b48ca27:	nopw   0x0(%rax,%rax,1)
     6b48ca30:	lea    0x85ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ca37:	mov    $0x103b,%r8d
+    6b48ca37:	mov    $0x1041,%r8d
     6b48ca3d:	lea    0x883a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48ca44:	call   6b48f9e0 <_assert>
     6b48ca49:	jmp    6b48c958 <vec0Update_InsertWriteFinalStep+0x3e8>
     6b48ca4e:	xchg   %ax,%ax
     6b48ca50:	lea    0x85ae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ca57:	mov    $0x1036,%r8d
+    6b48ca57:	mov    $0x103c,%r8d
     6b48ca5d:	lea    0x881a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48ca64:	call   6b48f9e0 <_assert>
     6b48ca69:	jmp    6b48c8eb <vec0Update_InsertWriteFinalStep+0x37b>
     6b48ca6e:	xchg   %ax,%ax
     6b48ca70:	lea    0x858e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ca77:	mov    $0x1013,%r8d
+    6b48ca77:	mov    $0x1019,%r8d
     6b48ca7d:	lea    0x87fa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48ca84:	call   6b48f9e0 <_assert>
     6b48ca89:	jmp    6b48c5f4 <vec0Update_InsertWriteFinalStep+0x84>
     6b48ca8e:	xchg   %ax,%ax
 
 000000006b48ca90 <vec0Update_Insert.constprop.12>:
     6b48ca90:	push   %r15
@@ -14295,23 +14295,23 @@
     6b48cb19:	je     6b48cc50 <vec0Update_Insert.constprop.12+0x1c0>
     6b48cb1f:	lea    0x88a7(%rip),%rcx        # 6b4953cd <.rdata+0x3cd>
     6b48cb26:	mov    %eax,%edx
     6b48cb28:	mov    0xd4f1(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48cb2f:	call   *0x228(%rax)
     6b48cb35:	mov    %rax,0x88(%rsp)
     6b48cb3d:	lea    0x84c1(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cb44:	mov    $0x1073,%r8d
+    6b48cb44:	mov    $0x1079,%r8d
     6b48cb4a:	lea    0x872d(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48cb51:	call   6b48f9e0 <_assert>
     6b48cb56:	mov    %rbx,%rsi
     6b48cb59:	shl    $0x5,%rsi
     6b48cb5d:	cmp    %r13d,0xe0(%rdi,%rsi,1)
     6b48cb65:	je     6b48cb80 <vec0Update_Insert.constprop.12+0xf0>
     6b48cb67:	lea    0x8497(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cb6e:	mov    $0x1074,%r8d
+    6b48cb6e:	mov    $0x107a,%r8d
     6b48cb74:	lea    0x9a6d(%rip),%rcx        # 6b4965e8 <.rdata+0x15e8>
     6b48cb7b:	call   6b48f9e0 <_assert>
     6b48cb80:	mov    0x80(%rsp),%rax
     6b48cb88:	cmp    %rax,0xd8(%rdi,%rsi,1)
     6b48cb90:	jne    6b48cd33 <vec0Update_Insert.constprop.12+0x2a3>
     6b48cb96:	mov    0x2c8(%rdi),%eax
     6b48cb9c:	add    $0x1,%rbx
@@ -14473,25 +14473,25 @@
     6b48ce7b:	call   *0x1d0(%rax)
     6b48ce81:	mov    0x68(%rsp),%rax
     6b48ce86:	mov    0x1f0(%rsp),%rdi
     6b48ce8e:	mov    %rax,(%rdi)
     6b48ce91:	xor    %eax,%eax
     6b48ce93:	jmp    6b48ccd8 <vec0Update_Insert.constprop.12+0x248>
     6b48ce98:	lea    0x8166(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ce9f:	mov    $0x108f,%r8d
+    6b48ce9f:	mov    $0x1095,%r8d
     6b48cea5:	lea    0x83d2(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48ceac:	call   6b48f9e0 <_assert>
     6b48ceb1:	jmp    6b48cdb0 <vec0Update_Insert.constprop.12+0x320>
     6b48ceb6:	lea    0x8148(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cebd:	mov    $0x109d,%r8d
+    6b48cebd:	mov    $0x10a3,%r8d
     6b48cec3:	lea    0x83b4(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48ceca:	call   6b48f9e0 <_assert>
     6b48cecf:	jmp    6b48ce2a <vec0Update_Insert.constprop.12+0x39a>
     6b48ced4:	lea    0x812a(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cedb:	mov    $0x1096,%r8d
+    6b48cedb:	mov    $0x109c,%r8d
     6b48cee1:	lea    0x8396(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48cee8:	call   6b48f9e0 <_assert>
     6b48ceed:	jmp    6b48cddf <vec0Update_Insert.constprop.12+0x34f>
     6b48cef2:	nopl   0x0(%rax)
     6b48cef6:	cs nopw 0x0(%rax,%rax,1)
 
 000000006b48cf00 <vec0Update_Insert>:
@@ -14528,23 +14528,23 @@
     6b48cf89:	je     6b48d0c0 <vec0Update_Insert+0x1c0>
     6b48cf8f:	lea    0x8437(%rip),%rcx        # 6b4953cd <.rdata+0x3cd>
     6b48cf96:	mov    %eax,%edx
     6b48cf98:	mov    0xd081(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48cf9f:	call   *0x228(%rax)
     6b48cfa5:	mov    %rax,0x88(%rsp)
     6b48cfad:	lea    0x8051(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cfb4:	mov    $0x1073,%r8d
+    6b48cfb4:	mov    $0x1079,%r8d
     6b48cfba:	lea    0x82bd(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48cfc1:	call   6b48f9e0 <_assert>
     6b48cfc6:	mov    %rbx,%rsi
     6b48cfc9:	shl    $0x5,%rsi
     6b48cfcd:	cmp    %r13d,0xe0(%rdi,%rsi,1)
     6b48cfd5:	je     6b48cff0 <vec0Update_Insert+0xf0>
     6b48cfd7:	lea    0x8027(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48cfde:	mov    $0x1074,%r8d
+    6b48cfde:	mov    $0x107a,%r8d
     6b48cfe4:	lea    0x95fd(%rip),%rcx        # 6b4965e8 <.rdata+0x15e8>
     6b48cfeb:	call   6b48f9e0 <_assert>
     6b48cff0:	mov    0x80(%rsp),%rax
     6b48cff8:	cmp    %rax,0xd8(%rdi,%rsi,1)
     6b48d000:	jne    6b48d1a3 <vec0Update_Insert+0x2a3>
     6b48d006:	mov    0x2c8(%rdi),%eax
     6b48d00c:	add    $0x1,%rbx
@@ -14706,25 +14706,25 @@
     6b48d2eb:	call   *0x1d0(%rax)
     6b48d2f1:	mov    0x68(%rsp),%rax
     6b48d2f6:	mov    0x1f8(%rsp),%rdi
     6b48d2fe:	mov    %rax,(%rdi)
     6b48d301:	xor    %eax,%eax
     6b48d303:	jmp    6b48d148 <vec0Update_Insert+0x248>
     6b48d308:	lea    0x7cf6(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d30f:	mov    $0x108f,%r8d
+    6b48d30f:	mov    $0x1095,%r8d
     6b48d315:	lea    0x7f62(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d31c:	call   6b48f9e0 <_assert>
     6b48d321:	jmp    6b48d220 <vec0Update_Insert+0x320>
     6b48d326:	lea    0x7cd8(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d32d:	mov    $0x109d,%r8d
+    6b48d32d:	mov    $0x10a3,%r8d
     6b48d333:	lea    0x7f44(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d33a:	call   6b48f9e0 <_assert>
     6b48d33f:	jmp    6b48d29a <vec0Update_Insert+0x39a>
     6b48d344:	lea    0x7cba(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d34b:	mov    $0x1096,%r8d
+    6b48d34b:	mov    $0x109c,%r8d
     6b48d351:	lea    0x7f26(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d358:	call   6b48f9e0 <_assert>
     6b48d35d:	jmp    6b48d24f <vec0Update_Insert+0x34f>
     6b48d362:	nopl   0x0(%rax)
     6b48d366:	cs nopw 0x0(%rax,%rax,1)
 
 000000006b48d370 <vec0Update_Delete>:
@@ -14833,59 +14833,59 @@
     6b48d545:	add    $0x70,%rsp
     6b48d549:	pop    %rbx
     6b48d54a:	pop    %rsi
     6b48d54b:	pop    %rdi
     6b48d54c:	ret
     6b48d54d:	nopl   (%rax)
     6b48d550:	lea    0x7aae(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d557:	mov    $0x10b3,%r8d
+    6b48d557:	mov    $0x10b9,%r8d
     6b48d55d:	lea    0x7d1a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d564:	call   6b48f9e0 <_assert>
     6b48d569:	jmp    6b48d39d <vec0Update_Delete+0x2d>
     6b48d56e:	xchg   %ax,%ax
     6b48d570:	lea    0x7a8e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d577:	mov    $0x10d1,%r8d
+    6b48d577:	mov    $0x10d7,%r8d
     6b48d57d:	lea    0x7cfa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d584:	call   6b48f9e0 <_assert>
     6b48d589:	jmp    6b48d508 <vec0Update_Delete+0x198>
     6b48d58e:	xchg   %ax,%ax
     6b48d590:	lea    0x7a6e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d597:	mov    $0x10c2,%r8d
+    6b48d597:	mov    $0x10c8,%r8d
     6b48d59d:	lea    0x7cda(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d5a4:	call   6b48f9e0 <_assert>
     6b48d5a9:	jmp    6b48d490 <vec0Update_Delete+0x120>
     6b48d5ae:	xchg   %ax,%ax
     6b48d5b0:	lea    0x7a4e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d5b7:	mov    $0x10bd,%r8d
+    6b48d5b7:	mov    $0x10c3,%r8d
     6b48d5bd:	lea    0x9119(%rip),%rcx        # 6b4966dd <.rdata+0x16dd>
     6b48d5c4:	call   6b48f9e0 <_assert>
     6b48d5c9:	mov    0x58(%rsp),%r9
     6b48d5ce:	movzbl 0x4e(%rsp),%r10d
     6b48d5d4:	mov    %r9,%rax
     6b48d5d7:	sar    $0x3f,%rax
     6b48d5db:	shr    $0x3d,%rax
     6b48d5df:	lea    (%r9,%rax,1),%r8
     6b48d5e3:	and    $0x7,%r8d
     6b48d5e7:	sub    %eax,%r8d
     6b48d5ea:	jmp    6b48d44b <vec0Update_Delete+0xdb>
     6b48d5ef:	nop
     6b48d5f0:	lea    0x7a0e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d5f7:	mov    $0x10bc,%r8d
+    6b48d5f7:	mov    $0x10c2,%r8d
     6b48d5fd:	lea    0x7c7a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d604:	call   6b48f9e0 <_assert>
     6b48d609:	jmp    6b48d41a <vec0Update_Delete+0xaa>
     6b48d60e:	xchg   %ax,%ax
     6b48d610:	lea    0x79ee(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d617:	mov    $0x10b8,%r8d
+    6b48d617:	mov    $0x10be,%r8d
     6b48d61d:	lea    0x7d36(%rip),%rcx        # 6b49535a <.rdata+0x35a>
     6b48d624:	call   6b48f9e0 <_assert>
     6b48d629:	jmp    6b48d3e1 <vec0Update_Delete+0x71>
     6b48d62e:	xchg   %ax,%ax
     6b48d630:	lea    0x79ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d637:	mov    $0x10cd,%r8d
+    6b48d637:	mov    $0x10d3,%r8d
     6b48d63d:	lea    0x85db(%rip),%rcx        # 6b495c1f <.rdata+0xc1f>
     6b48d644:	call   6b48f9e0 <_assert>
     6b48d649:	jmp    6b48d4ca <vec0Update_Delete+0x15a>
     6b48d64e:	xchg   %ax,%ax
 
 000000006b48d650 <vec0Update>:
     6b48d650:	push   %r15
@@ -15052,25 +15052,25 @@
     6b48d917:	mov    0xc702(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48d91e:	mov    %r15,%rcx
     6b48d921:	call   *0x338(%rax)
     6b48d927:	movslq %eax,%r13
     6b48d92a:	jmp    6b48d81b <vec0Update+0x1cb>
     6b48d92f:	nop
     6b48d930:	lea    0x76ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d937:	mov    $0xff3,%r8d
+    6b48d937:	mov    $0xff9,%r8d
     6b48d93d:	lea    0x793a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d944:	call   6b48f9e0 <_assert>
-    6b48d949:	mov    $0x110c,%r8d
+    6b48d949:	mov    $0x1112,%r8d
     6b48d94f:	lea    0x76af(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b48d956:	lea    0x7921(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d95d:	call   6b48f9e0 <_assert>
     6b48d962:	jmp    6b48d8ba <vec0Update+0x26a>
     6b48d967:	nopw   0x0(%rax,%rax,1)
     6b48d970:	lea    0x768e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48d977:	mov    $0x1107,%r8d
+    6b48d977:	mov    $0x110d,%r8d
     6b48d97d:	lea    0x78fa(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48d984:	call   6b48f9e0 <_assert>
     6b48d989:	jmp    6b48d86a <vec0Update+0x21a>
     6b48d98e:	xchg   %ax,%ax
     6b48d990:	mov    0xc689(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48d997:	mov    %r15,%rcx
     6b48d99a:	call   *0x338(%rax)
@@ -15127,15 +15127,15 @@
     6b48da87:	mov    0xd8(%rsi,%rax,1),%r8
     6b48da8f:	mov    0xc58a(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48da96:	mov    0x8(%rsi,%r15,1),%rdx
     6b48da9b:	call   *0x228(%rax)
     6b48daa1:	mov    %rax,0x10(%rsi)
     6b48daa5:	jmp    6b48d764 <vec0Update+0x114>
     6b48daaa:	lea    0x7554(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48dab1:	mov    $0x10e5,%r8d
+    6b48dab1:	mov    $0x10eb,%r8d
     6b48dab7:	lea    0x77c0(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48dabe:	call   6b48f9e0 <_assert>
     6b48dac3:	jmp    6b48d7df <vec0Update+0x18f>
     6b48dac8:	nopl   0x0(%rax,%rax,1)
 
 000000006b48dad0 <vec0Update_UpdateOnRowid>:
     6b48dad0:	push   %r15
@@ -15250,25 +15250,25 @@
     6b48dcd4:	mov    0x8(%rdi,%r15,1),%rdx
     6b48dcd9:	call   *0x228(%rax)
     6b48dcdf:	mov    %rax,0x10(%rdi)
     6b48dce3:	mov    $0x1,%eax
     6b48dce8:	jmp    6b48dde2 <vec0Update_UpdateOnRowid+0x312>
     6b48dced:	nopl   (%rax)
     6b48dcf0:	lea    0x730e(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48dcf7:	mov    $0xff3,%r8d
+    6b48dcf7:	mov    $0xff9,%r8d
     6b48dcfd:	lea    0x757a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48dd04:	call   6b48f9e0 <_assert>
-    6b48dd09:	mov    $0x110c,%r8d
+    6b48dd09:	mov    $0x1112,%r8d
     6b48dd0f:	lea    0x72ef(%rip),%rdx        # 6b495005 <.rdata+0x5>
     6b48dd16:	lea    0x7561(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48dd1d:	call   6b48f9e0 <_assert>
     6b48dd22:	jmp    6b48dbe8 <vec0Update_UpdateOnRowid+0x118>
     6b48dd27:	nopw   0x0(%rax,%rax,1)
     6b48dd30:	lea    0x72ce(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48dd37:	mov    $0x1107,%r8d
+    6b48dd37:	mov    $0x110d,%r8d
     6b48dd3d:	lea    0x753a(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48dd44:	call   6b48f9e0 <_assert>
     6b48dd49:	jmp    6b48db99 <vec0Update_UpdateOnRowid+0xc9>
     6b48dd4e:	xchg   %ax,%ax
     6b48dd50:	mov    0xc2c9(%rip),%rax        # 6b49a020 <sqlite3_api>
     6b48dd57:	mov    %r15,%rcx
     6b48dd5a:	call   *0x338(%rax)
@@ -15308,15 +15308,15 @@
     6b48dde9:	pop    %rbp
     6b48ddea:	pop    %r12
     6b48ddec:	pop    %r13
     6b48ddee:	pop    %r14
     6b48ddf0:	pop    %r15
     6b48ddf2:	ret
     6b48ddf3:	lea    0x720b(%rip),%rdx        # 6b495005 <.rdata+0x5>
-    6b48ddfa:	mov    $0x10e5,%r8d
+    6b48ddfa:	mov    $0x10eb,%r8d
     6b48de00:	lea    0x7477(%rip),%rcx        # 6b49527e <.rdata+0x27e>
     6b48de07:	call   6b48f9e0 <_assert>
     6b48de0c:	jmp    6b48db18 <vec0Update_UpdateOnRowid+0x48>
     6b48de11:	nopl   0x0(%rax,%rax,1)
     6b48de16:	cs nopw 0x0(%rax,%rax,1)
 
 000000006b48de20 <sqlite3_mmap_warm>:
@@ -24954,55 +24954,54 @@
     6b496970:	jbe    6b4969d7 <aMod.9650+0x97>
     6b496972:	movsxd 0x76(%rdi),%ebx
     6b496975:	gs jb  6b4969eb <aMod.9650+0xab>
     6b496978:	imul   $0x2e307600,0x6e(%rdi),%ebp
     6b49697f:	xor    %ch,(%rsi)
     6b496981:	xor    %ebp,0x68706c61(%rip)        # d3b9d5e8 <.debug_str+0x686f65e8>
     6b496987:	(bad)
-    6b496988:	cs xor (%rax),%eax
-    6b49698b:	jbe    6b4969f2 <aMod.9650+0xb2>
+    6b496988:	cs (bad)
+    6b49698a:	add    %dh,0x65(%rsi)
     6b49698d:	movsxd 0x64(%rdi),%ebx
     6b496990:	(bad)
     6b496996:	add    %al,(%rax)
     6b496998:	push   %rsi
     6b496999:	gs jb  6b496a0f <aMod.9650+0xcf>
     6b49699c:	imul   $0x3076203a,0x6e(%rdi),%ebp
     6b4969a3:	cs xor %ch,(%rsi)
     6b4969a6:	xor    %ebp,0x68706c61(%rip)        # d3b9d60d <.debug_str+0x686f660d>
     6b4969ac:	(bad)
-    6b4969ad:	cs xor (%rdx),%ecx
-    6b4969b0:	rex.R (bad)
-    6b4969b2:	je     6b496a19 <aMod.9650+0xd9>
-    6b4969b4:	cmp    (%rax),%ah
+    6b4969ad:	cs (bad)
+    6b4969af:	or     0x74(%rcx,%riz,2),%al
+    6b4969b3:	cmp    %gs:(%rax),%ah
     6b4969b6:	xor    (%rax),%dh
-    6b4969b8:	xor    0x322d3430(,%rbp,1),%dh
-    6b4969bf:	(bad)
-    6b4969c0:	push   %rsp
-    6b4969c1:	xor    %edi,(%rcx)
-    6b4969c3:	cmp    0x32303a35(%rip),%dh        # 9d79a3fe <.debug_str+0x322f33fe>
+    6b4969b8:	xor    0x312d3530(,%rbp,1),%dh
+    6b4969bf:	xor    %edx,0x34(%rax,%rsi,1)
+    6b4969c3:	cmp    (%rbx),%dh
+    6b4969c5:	xor    (%rdx),%edi
+    6b4969c7:	xor    $0x35,%al
     6b4969c9:	pop    %rdx
     6b4969ca:	sub    (%rax),%esi
     6b4969cc:	xor    %dh,(%rax)
     6b4969ce:	xor    %cl,(%rdx)
     6b4969d0:	rex.XB outsl %ds:(%rsi),(%dx)
     6b4969d2:	insl   (%dx),%es:(%rdi)
     6b4969d3:	insl   (%dx),%es:(%rdi)
-    6b4969d4:	imul   $0x66623530,0x20(%rdx,%rdi,1),%esi
-    6b4969dc:	gs xor $0x66333636,%eax
-    6b4969e2:	cmp    %edi,(%rcx)
-    6b4969e4:	cmp    %dh,(%rdi)
-    6b4969e6:	xor    $0x63323732,%eax
-    6b4969eb:	xor    0x64(%rdi,%rsi,1),%ah
-    6b4969ef:	fs (bad)
-    6b4969f1:	xor    %fs:0x30(%rcx),%esp
-    6b4969f5:	xor    $0x31,%al
-    6b4969f7:	xor    $0x61386631,%eax
-    6b4969fc:	xor    %dh,(%rdx)
-    6b4969fe:	xor    $0x62,%al
-    6b496a00:	or     0x75(%rdx),%al
+    6b4969d4:	imul   $0x36376433,0x20(%rdx,%rdi,1),%esi
+    6b4969dc:	xor    0x34(%rsi),%esp
+    6b4969df:	cmp    %edi,(%rcx)
+    6b4969e1:	cmp    %dh,0x65316639(%rip)        # d07ad020 <.debug_str+0x65306020>
+    6b4969e7:	cmp    %edi,(%rcx)
+    6b4969e9:	cmp    %dh,(%rsi,%riz,2)
+    6b4969ec:	xor    (%rcx),%esi
+    6b4969ee:	xor    %esp,0x32(%rbp)
+    6b4969f1:	cmp    %ah,0x66(%rcx)
+    6b4969f4:	cmp    %esi,(%rsi)
+    6b4969f6:	xor    $0x63616464,%eax
+    6b4969fb:	ss xor (%rax),%esi
+    6b4969fe:	data16 or %gs:0x75(%rdx),%al
     6b496a03:	imul   $0x67616c66,0x20(%rsp,%riz,2),%ebp
     6b496a0b:	jae    6b496a47 <aMod.9650+0x107>
     6b496a0d:	and    %ah,(%rax)
     6b496a0f:	add    %dh,0x65(%rsi)
     6b496a12:	movsxd 0x64(%rdi),%ebx
     6b496a15:	imul   $0x65636e61,0x74(%rbx),%esi
     6b496a1c:	pop    %rdi
@@ -28317,16 +28316,17 @@
 	...
 
 Disassembly of section .edata:
 
 000000006b49c000 <.edata>:
     6b49c000:	add    %al,(%rax)
     6b49c002:	add    %al,(%rax)
-    6b49c004:	and    0x2d(%rax),%bl
-    6b49c007:	data16 add %al,(%rax)
+    6b49c004:	(bad)
+    6b49c005:	cmc
+    6b49c006:	ds data16 add %al,(%rax)
     6b49c00a:	add    %al,(%rax)
     6b49c00c:	rex.RX rolb $0x0,(%rcx)
     6b49c010:	add    %eax,(%rax)
     6b49c012:	add    %al,(%rax)
     6b49c014:	add    (%rax),%eax
     6b49c016:	add    %al,(%rax)
     6b49c018:	add    (%rax),%eax
```

