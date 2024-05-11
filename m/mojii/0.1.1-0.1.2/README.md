# Comparing `tmp/mojii-0.1.1-py3-none-any.whl.zip` & `tmp/mojii-0.1.2.tar.gz`

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  tmp/mojii-0.1.2.tar.gz*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,94 +1,100 @@
-00000000: 504b 0304 1400 0000 0800 9b4c 9058 0000  PK.........L.X..
-00000010: 0000 0200 0000 0000 0000 1000 0000 6d6f  ..............mo
-00000020: 6a69 2f5f 5f69 6e69 745f 5f2e 7079 0300  ji/__init__.py..
-00000030: 504b 0304 1400 0000 0800 e14c 9058 5b1b  PK.........L.X[.
-00000040: 6b95 2300 0000 2300 0000 0c00 0000 6d6f  k.#...#.......mo
-00000050: 6a69 2f6d 6f6a 692e 7079 4b49 4d53 48d4  ji/moji.pyKIMSH.
-00000060: d0b4 e2e5 5200 8282 a2cc bc12 0d75 8fd4  ....R........u..
-00000070: 9c9c 7c85 f0fc a29c 1445 754d 0050 4b03  ..|......EuM.PK.
-00000080: 0414 0000 0008 00bd b4a2 584f 2e3d 112a  ..........XO.=.*
-00000090: 0100 00d2 0200 001e 0000 006d 6f6a 6969  ...........mojii
-000000a0: 2d30 2e31 2e31 2e64 6973 742d 696e 666f  -0.1.1.dist-info
-000000b0: 2f4d 4554 4144 4154 4195 924b 4fc3 3010  /METADATA..KO.0.
-000000c0: 84ef 96fc 1f2c 714e a045 e2e1 13a5 bd14  .....,qN.E......
-000000d0: 5a5a d18a bb49 b661 217e e047 69fe 3deb  ZZ...I.a!~.Gi.=.
-000000e0: d022 f598 9b57 b3df 78a5 9925 4455 aba8  ."...W..x..%DU..
-000000f0: 8a37 f001 ad91 625c 8e38 7b51 1aa4 d0f6  .7....b\.8{Q....
-00000100: 1391 b37f e9aa 1c65 7193 b456 be93 6206  .......eq..V..b.
-00000110: da8a 16df 3d4d 9c4d 52fc b05e 8a27 bbdb  ....=M.MR..^.'..
-00000120: 79e8 c423 82d9 8349 27a5 00ad b095 020e  y..#...I'.......
-00000130: 4abb 161e fab1 acac e66c 8115 9840 3f2e  J........l...@?.
-00000140: e75b cea6 ad0a 0177 0864 3637 114c 0db5  .[.....w.d67.L..
-00000150: 98a4 9afc 2a10 32ff bb87 d63a 3aeb 7cf9  ....*.2....::.|.
-00000160: 6893 5756 9bb9 9838 e7ed 9e58 d91b 9fe4  h.WV...8...X....
-00000170: 7366 ed6d e395 d668 1ab1 50a6 49aa e90d  sf.m...h..P.I...
-00000180: d61d dd6c 86ec e6d7 f560 a0bc 198e dc0e  ...l.....`......
-00000190: 47ee 8623 f7c3 91d1 f89c 5951 462a 6662  G..#......YQF*fb
-000001a0: d385 08fa 2f19 0ab5 0697 6335 91b3 1984  ..../.....c5....
-000001b0: caa3 8bd4 b062 6a73 dcb1 d876 8eca 10e1  .....bjs...v....
-000001c0: 102f a969 5fb5 fda1 245e e13b a187 50cc  ./.i_...$^.;..P.
-000001d0: 3044 294c d28e 5ac7 d945 df53 f1ac 3c6a  0D)L..Z..E.S..<j
-000001e0: 6aeb 2f50 4b03 0414 0000 0008 00bd b4a2  j./PK...........
-000001f0: 58fc 0e7b 4b5c 0000 005c 0000 001b 0000  X..{K\...\......
-00000200: 006d 6f6a 6969 2d30 2e31 2e31 2e64 6973  .mojii-0.1.1.dis
-00000210: 742d 696e 666f 2f57 4845 454c 0bcf 484d  t-info/WHEEL..HM
-00000220: cdd1 0d4b 2d2a cecc cfb3 5230 d433 e072  ...K-*....R0.3.r
-00000230: 4fcd 4b2d 4a2c c92f b252 484a c92c 2e89  O.K-J,./.RHJ.,..
-00000240: 2f07 a951 d030 d033 31d6 33d0 e40a cacf  /..Q.0.31.3.....
-00000250: 2fd1 f52c d60d 282d 4acd c94c b252 2829  /..,..(-J..L.R()
-00000260: 2a4d e50a 494c b752 28a8 34d6 cdcb cf4b  *M..IL.R(.4....K
-00000270: d54d ccab e4e2 0200 504b 0304 1400 0000  .M......PK......
-00000280: 0800 bdb4 a258 b2d4 6fd5 0700 0000 0500  .....X..o.......
-00000290: 0000 2300 0000 6d6f 6a69 692d 302e 312e  ..#...mojii-0.1.
-000002a0: 312e 6469 7374 2d69 6e66 6f2f 746f 705f  1.dist-info/top_
-000002b0: 6c65 7665 6c2e 7478 74cb cdcf cae4 0200  level.txt.......
-000002c0: 504b 0304 1400 0000 0800 bdb4 a258 194c  PK...........X.L
-000002d0: 4cca 2401 0000 a901 0000 1c00 0000 6d6f  L.$...........mo
-000002e0: 6a69 692d 302e 312e 312e 6469 7374 2d69  jii-0.1.1.dist-i
-000002f0: 6e66 6f2f 5245 434f 5244 75d0 4d6f 8230  nfo/RECORDu.Mo.0
-00000300: 00c6 f1bb 9fa5 282a e5e5 b003 0222 283a  ......(*....."(:
-00000310: a048 e6a5 615a a548 a193 22b2 4fbf b984  .H..aZ.H..".O...
-00000320: 6417 f324 ffe3 eff0 b0ba a013 8c69 4505  d..$.........iE.
-00000330: c663 de83 26cf 6650 7d53 34db 0979 a1af  .c..&.fP}S4..y..
-00000340: 1671 2661 e4b1 5482 be45 da90 4457 06b7  .q&a..T..E..DW..
-00000350: 01f7 d383 3bcf e376 9900 79c4 9eca 33ff  ....;..v..y...3.
-00000360: 0491 bf13 b667 5e21 475c eebf 522b 8b95  .....g^!G\..R+..
-00000370: 29d3 19ea 2c53 e9ed 1b64 92f0 0e55 70f6  )...,S...d...Up.
-00000380: 1330 877f 0495 e4f1 f477 27da 0889 56e7  .0.......w'...V.
-00000390: 7a12 38c8 b44d 640e a86c 2b47 9cf9 c834  z.8..Md..l+G...4
-000003a0: 4cab 28ef a730 246b 845b 9d04 8fd6 3733  L.(..0$k.[....73
-000003b0: 14bb f448 4915 f587 0bd0 66b3 176a ba72  ...HI.....f..j.r
-000003c0: 9ccd 40ba be26 f035 5d2c fbee 33bb ac21  ..@..&.5],..3..!
-000003d0: a90d af4e ba4d aad6 fd8e a035 0b25 83ae  ...N.M.....5.%..
-000003e0: 96fb ed23 04c6 2b51 d41c 97e4 4eca b178  ...#..+Q....N..x
-000003f0: 8841 ee8e 3264 4e08 bfcb 8f9d 95b8 a5a1  .A..2dN.........
-00000400: 064a 9122 95f3 c638 0955 dd5a b97e d59a  .J."...8.U.Z.~..
-00000410: 5b7f f7c0 ab03 22c7 da45 3600 a31f 504b  [....."..E6...PK
-00000420: 0102 1400 1400 0000 0800 9b4c 9058 0000  ...........L.X..
-00000430: 0000 0200 0000 0000 0000 1000 0000 0000  ................
-00000440: 0000 0000 0000 b681 0000 0000 6d6f 6a69  ............moji
-00000450: 2f5f 5f69 6e69 745f 5f2e 7079 504b 0102  /__init__.pyPK..
-00000460: 1400 1400 0000 0800 e14c 9058 5b1b 6b95  .........L.X[.k.
-00000470: 2300 0000 2300 0000 0c00 0000 0000 0000  #...#...........
-00000480: 0000 0000 b681 3000 0000 6d6f 6a69 2f6d  ......0...moji/m
-00000490: 6f6a 692e 7079 504b 0102 1400 1400 0000  oji.pyPK........
-000004a0: 0800 bdb4 a258 4f2e 3d11 2a01 0000 d202  .....XO.=.*.....
-000004b0: 0000 1e00 0000 0000 0000 0000 0000 b681  ................
-000004c0: 7d00 0000 6d6f 6a69 692d 302e 312e 312e  }...mojii-0.1.1.
-000004d0: 6469 7374 2d69 6e66 6f2f 4d45 5441 4441  dist-info/METADA
-000004e0: 5441 504b 0102 1400 1400 0000 0800 bdb4  TAPK............
-000004f0: a258 fc0e 7b4b 5c00 0000 5c00 0000 1b00  .X..{K\...\.....
-00000500: 0000 0000 0000 0000 0000 b681 e301 0000  ................
-00000510: 6d6f 6a69 692d 302e 312e 312e 6469 7374  mojii-0.1.1.dist
-00000520: 2d69 6e66 6f2f 5748 4545 4c50 4b01 0214  -info/WHEELPK...
-00000530: 0014 0000 0008 00bd b4a2 58b2 d46f d507  ..........X..o..
-00000540: 0000 0005 0000 0023 0000 0000 0000 0000  .......#........
-00000550: 0000 00b6 8178 0200 006d 6f6a 6969 2d30  .....x...mojii-0
-00000560: 2e31 2e31 2e64 6973 742d 696e 666f 2f74  .1.1.dist-info/t
-00000570: 6f70 5f6c 6576 656c 2e74 7874 504b 0102  op_level.txtPK..
-00000580: 1400 1400 0000 0800 bdb4 a258 194c 4cca  ...........X.LL.
-00000590: 2401 0000 a901 0000 1c00 0000 0000 0000  $...............
-000005a0: 0000 0000 b481 c002 0000 6d6f 6a69 692d  ..........mojii-
-000005b0: 302e 312e 312e 6469 7374 2d69 6e66 6f2f  0.1.1.dist-info/
-000005c0: 5245 434f 5244 504b 0506 0000 0000 0600  RECORDPK........
-000005d0: 0600 a801 0000 1e04 0000 0000            ............
+00000000: 1f8b 0808 a616 3466 02ff 6d6f 6a69 692d  ......4f..mojii-
+00000010: 302e 312e 322e 7461 7200 ed5c 6d73 9b38  0.1.2.tar..\ms.8
+00000020: 10ce 6766 f80f 3af7 83ed 9918 f34e e219  ..gf..:......N..
+00000030: 669a 6b72 6dae 4d93 4972 771f 3a1d 4605  f.krm.M.Irw.:.F.
+00000040: d9d1 0510 0722 89ff fd49 60dc d879 6999  ....."...I`..yi.
+00000050: c65c e7bc cf87 1824 ed22 22ed 3e2b d0a2  .\.....$."".>+..
+00000060: 8db5 f1eb 337c f78e e088 e43b 1b81 5ee3  ....3|.....;..^.
+00000070: a95f 5db7 ccaf c7b2 dcd0 4d43 df41 773b  ._].......MC.Aw;
+00000080: 1da0 2c38 cec5 e577 b613 a68b 124e 13e2  ..,8...w.....N..
+00000090: 1b9e 61bb 7bfb 9e6e 6a86 69da b6b2 03d8  ..a.{..nj.i.....
+000000a0: 0224 ec6f 4a47 ba66 68e6 7853 d790 46ed  .$.oJG.fh.xS..F.
+000000b0: 79de d3f6 2f8e c5e4 331c ddb0 4cdb 15e5  y.../...3...L...
+000000c0: 9ee3 383b c801 fbdf 38b4 9fc2 ffdb 0ffd  ..8;....8.......
+000000d0: bf09 febf 13ff bff7 88ff 37f6 f675 c702  ..........7..u..
+000000e0: 06d8 32ff 7ff6 feed e8f8 e36f a79b b07f  ..2........o....
+000000f0: d775 9fb2 7fe1 f4cd 55ff 6fe8 ae23 e23f  .u......U.o..#.?
+00000100: 1dec 7fe3 3821 1c47 98e3 d19f 242f 284b  ....8!.G....$/(K
+00000110: 2748 d8bf aa7c c409 99a0 6a72 a8ca b2aa  'H...|....jr....
+00000120: 9a26 aa72 5126 09ce e713 7448 1286 62fa  .&.rQ&....tH..b.
+00000130: 2517 67aa 7250 f22b 964f d0ef 6c3a cdc9  %.g.rP.+.O..l:..
+00000140: 1cfd 4a49 7a43 d2b2 a919 9104 d378 82c8  ..JIzC.......x..
+00000150: 1d4e b298 bcae 4eb5 9025 aaf2 8186 242d  .N....N..%....$-
+00000160: c415 4f8e 2f55 e54d 8c8b 824e 2911 ca8e  ..O./U.M...N)...
+00000170: 534e d288 44e8 a08c 84be 90a0 89bc ee0d  SN..D...........
+00000180: 8959 26ba b5da 78a1 4636 39bd 3846 0759  .Y&...x.F69.8F.Y
+00000190: 96b3 1b21 3ba9 1437 d5ab 3267 399b e538  ...!;..7..2g9..8
+000001a0: 4968 3a43 1f70 3a2b f1ac 5270 3617 7d4e  Ih:C.p:+..Rp6.}N
+000001b0: dbb4 9547 566b 01cd 6d2f e2b5 17d9 6b2f  ...GVk..m/....k/
+000001c0: b2df 5ec4 3057 654e c518 612e 252e e605  ..^.0WeN..a.%...
+000001d0: 2749 3d32 6250 2392 c961 4db9 aa1c 9222  'I=2bP#..aM...."
+000001e0: cc69 c6c5 0c1b bd61 72b8 f9e8 729e 89c9  .i.....ar...r...
+000001f0: c0c9 1d1f 8b99 761d b15b 3112 e7e4 9f92  ......v..[1.....
+00000200: e6a4 181d d282 4f50 5a26 9998 75aa f2aa  ......OPZ&..u...
+00000210: 9aa7 e83d ce69 2266 2bf8 7488 ffc0 ffff  ...=.i"f+.t.....
+00000220: 48fc a7ef dbb6 6142 fcb7 6df1 9f3c 1e6f  H.....aB..m..<.o
+00000230: c8fe 5bad ff0d dd31 2c58 ff6f 8dff 37dd  ..[....1,X.o..7.
+00000240: 87fe df02 ffdf 89ff 37bf fa7f cb74 c53f  ........7....t.?
+00000250: ded1 74f0 fcdb ebff 8380 a694 0781 96cd  ..t.............
+00000260: 3b5a ff37 fe5f f76c 5b4c 41c1 1386 e99a  ;Z.7._.l[LA.....
+00000270: 0eac ffc1 ffc3 f877 e9ff 65fc ef3a 36f8  .......w..e..:6.
+00000280: ff6d f6ff f2cf 0bfa feef f1ff 86e5 2ee3  .m..............
+00000290: 7f43 b633 4cdd b4c1 ff77 019a 642c e7f5  .C.3L....w..d,..
+000002a0: 1334 5ca0 4255 2232 4578 309c a80a 12c8  .4\.BU"2Ex0.....
+000002b0: 729a f241 ff1d 8963 86fe 6279 1cfd d21f  r..A...c..by....
+000002c0: caa7 6eaa 42a7 2808 529c 9020 40be 8ffa  ..n.B.(.R.. @...
+000002d0: 4190 609a 0641 7f21 2a94 807d 01ff c3f3  A.`..A.!*..}....
+000002e0: bf9f 9aff 1f7d ffeb 9aee be0b 51c0 16f2  .....}......Q...
+000002f0: 3fd5 c86c 36a2 e994 8d5f d4fe db3d ff33  ?..l6...._...=.3
+00000300: 2dc7 85e7 7fb0 fe83 f1ef 7afd e7e9 06ac  -.........z.....
+00000310: ffc0 ff4b ffff 62db 81da edff 7184 fd5b  ...K..b.....q..[
+00000320: 36ec ffe9 06b0 ff07 f6ff c0fe 1f58 ff43  6............X.C
+00000330: fc07 f11f c47f 10ff dd8b ff2e 4eff 387f  ............N.8.
+00000340: 7374 a1f1 3bbe d1f8 4f98 bfbb 16ff d9f2  st..;...O.......
+00000350: 07e2 bf0e 5010 5e66 5a36 57d6 5ffe 2bf7  ....P.^fZ6W._.+.
+00000360: df06 294f 2c0d 94a7 a7cc 7a55 c3f8 e13c  ..)O,.....zU...<
+00000370: 8869 7a5d 3cd6 265f 30fc 6375 9c65 412c  .iz]<.&_0.cu.eA,
+00000380: e3be 1f9f 8f00 e07f b07f e07f c0b3 fcff  ................
+00000390: 98c7 de08 ffeb bab1 c6ff ae6d 5ac0 ff5d  ...........mZ..]
+000003a0: 004c 1df8 1ff8 1ff8 1ff8 1ff8 ff99 d5d8  .L..............
+000003b0: 46d7 ffa2 767d fdef 3906 f07f 17a8 9ea2  F...v}..9.......
+000003c0: 83bd 03ff 03ff 03ff 03ff 03ff 6fe0 89eb  ............o...
+000003d0: b7f9 df59 e37f 4778 00e0 ffae c61f cc1d  ...Y..Gx........
+000003e0: f8ff bfdd ff6f 3de4 7f03 f8bf 13fe f71e  .....o=.........
+000003f0: fbfe a765 db0e 7885 6de3 fffa 5d70 389d  ...e..x.m...]p8.
+00000400: 6dc0 fe9f e57f 67fd fb6f 86e5 c1f3 ff4e  m.....g..o.....N
+00000410: f049 847b 810c f73e ab0a c7b3 e04b 49e3  .I.{...>.....KI.
+00000420: 08f9 a83e 8b30 27e2 4497 dbec c056 80ff  ...>.0'.D....V..
+00000430: 61fd ff7f 5fff 43fe ffb6 f3ff cbe6 fe7f  a..._.C.........
+00000440: 07ff 9b8e 61ac e5ff 1bf2 3330 c0ff 1de0  ....a.....30....
+00000450: 153a 886f f1bc 4059 4ea6 2447 d51c e08c  .:.o..@YN.$G....
+00000460: c505 6237 e23c a205 2f39 8d0b 5599 e62c  ..b7.<../9..U..,
+00000470: b95f bff8 7440 55b2 8ba6 348d 820c 87d7  ._..t@U...4.....
+00000480: 7846 8a7a 5bfe 2543 6541 1046 214b 0ba1  xF.z[.%CeA.F!K..
+00000490: 87a4 1c91 3464 114d 670b 75e2 8484 4b55  ....4d.Mg.u...KU
+000004a0: 2c23 e9a2 822d 0b33 ccaf 16fa ae88 e84f  ,#...-.3.......O
+000004b0: 4e42 cef2 b954 ca31 4d65 7201 bfa2 85e8  NB...T.1Mer.....
+000004c0: 404c 54e5 ddd1 f991 8858 a490 86bf 14f2  @LT......X......
+000004d0: 7750 9d08 41f9 ad82 4110 c886 4130 1cd6  wP..A...A...A0..
+000004e0: 4adf 122e e409 8a99 5014 7dcd 4540 5537  J.......P.}.E@U7
+000004f0: 64cd f9d1 c1e1 c9d1 42ff 2de5 5755 3f6b  d.......B.-.WU?k
+00000500: ad7f 339a 0ee4 3577 513f 1714 9a10 2d89  ..3...5wQ?....-.
+00000510: fac3 dde5 7dfa fd92 4f47 7bfd a1fc bac2  ....}...OG{.....
+00000520: 74f1 6504 79ad e0fe b57c 34d5 a4f8 60d8  t.e.y....|4...`.
+00000530: dca9 b8a1 10c7 31e2 acfe 070f 8628 62a4  ......1......(b.
+00000540: 4055 99e8 d42d cbaf 55a5 aeaa 95ca bbf3  @U...-..U.......
+00000550: 7b95 3df7 76eb a29b 3a71 c7ef 55f6 dd94  {.=.v...:q..U...
+00000560: debb b0df bb9f c2d3 3458 ef9e bf5e f044  ........4X...^.D
+00000570: bb20 acd3 3702 3ecf 4457 56d2 371a ddaf  . ..7.>.DWV.7...
+00000580: 5099 c77e ef8a f3ac 988c ebfd a5f2 cec5  P..~............
+00000590: 3d45 2c2c 34ca c64d 535c 650d f9bd f57c  =E,,4..MS\e....|
+000005a0: a2d5 faa0 4a23 f27b 0fb2 8a96 7753 67fd  ....J#.{....wSg.
+000005b0: f8bd 93e3 cba6 2c5c e6a8 14fe a7ba 48a2  ......,\......H.
+000005c0: f78d 6ca3 46bc 6afb 7dc9 462b 22cf a7d0  ..l.F.j.}.F+"...
+000005d0: b468 5a65 dbb4 6daf b9ad 25bc d612 7bad  .hZe..m...%...{.
+000005e0: 25f6 5b4b 18e6 8ac8 b793 8c7a 75eb cf0b  %.[K.......zu...
+000005f0: a9c6 4bf9 9f2a 73e9 35e5 340d e332 228d  ..K..*s.5.4..2".
+00000600: 1793 ab1f ec5f e625 59d6 0bae 88e3 a079  ....._.%Y......y
+00000610: 312e e4ab d7a7 3db1 7682 4f9d 0000 0000  1.....=.v.O.....
+00000620: 0000 0000 0000 0000 00f8 59f1 2fca 24f4  ..........Y./.$.
+00000630: 3c00 7800 00                             <.x..
```

## Comparing `tmp/mojii-0.1.1-py3-none-any.whl.zip` & `tmp/mojii-0.1.2.tar.gz`

```diff
@@ -1,94 +1,100 @@
-00000000: 504b 0304 1400 0000 0800 9b4c 9058 0000  PK.........L.X..
-00000010: 0000 0200 0000 0000 0000 1000 0000 6d6f  ..............mo
-00000020: 6a69 2f5f 5f69 6e69 745f 5f2e 7079 0300  ji/__init__.py..
-00000030: 504b 0304 1400 0000 0800 e14c 9058 5b1b  PK.........L.X[.
-00000040: 6b95 2300 0000 2300 0000 0c00 0000 6d6f  k.#...#.......mo
-00000050: 6a69 2f6d 6f6a 692e 7079 4b49 4d53 48d4  ji/moji.pyKIMSH.
-00000060: d0b4 e2e5 5200 8282 a2cc bc12 0d75 8fd4  ....R........u..
-00000070: 9c9c 7c85 f0fc a29c 1445 754d 0050 4b03  ..|......EuM.PK.
-00000080: 0414 0000 0008 00bd b4a2 584f 2e3d 112a  ..........XO.=.*
-00000090: 0100 00d2 0200 001e 0000 006d 6f6a 6969  ...........mojii
-000000a0: 2d30 2e31 2e31 2e64 6973 742d 696e 666f  -0.1.1.dist-info
-000000b0: 2f4d 4554 4144 4154 4195 924b 4fc3 3010  /METADATA..KO.0.
-000000c0: 84ef 96fc 1f2c 714e a045 e2e1 13a5 bd14  .....,qN.E......
-000000d0: 5a5a d18a bb49 b661 217e e047 69fe 3deb  ZZ...I.a!~.Gi.=.
-000000e0: d022 f598 9b57 b3df 78a5 9925 4455 aba8  ."...W..x..%DU..
-000000f0: 8a37 f001 ad91 625c 8e38 7b51 1aa4 d0f6  .7....b\.8{Q....
-00000100: 1391 b37f e9aa 1c65 7193 b456 be93 6206  .......eq..V..b.
-00000110: da8a 16df 3d4d 9c4d 52fc b05e 8a27 bbdb  ....=M.MR..^.'..
-00000120: 79e8 c423 82d9 8349 27a5 00ad b095 020e  y..#...I'.......
-00000130: 4abb 161e fab1 acac e66c 8115 9840 3f2e  J........l...@?.
-00000140: e75b cea6 ad0a 0177 0864 3637 114c 0db5  .[.....w.d67.L..
-00000150: 98a4 9afc 2a10 32ff bb87 d63a 3aeb 7cf9  ....*.2....::.|.
-00000160: 6893 5756 9bb9 9838 e7ed 9e58 d91b 9fe4  h.WV...8...X....
-00000170: 7366 ed6d e395 d668 1ab1 50a6 49aa e90d  sf.m...h..P.I...
-00000180: d61d dd6c 86ec e6d7 f560 a0bc 198e dc0e  ...l.....`......
-00000190: 47ee 8623 f7c3 91d1 f89c 5951 462a 6662  G..#......YQF*fb
-000001a0: d385 08fa 2f19 0ab5 0697 6335 91b3 1984  ..../.....c5....
-000001b0: caa3 8bd4 b062 6a73 dcb1 d876 8eca 10e1  .....bjs...v....
-000001c0: 102f a969 5fb5 fda1 245e e13b a187 50cc  ./.i_...$^.;..P.
-000001d0: 3044 294c d28e 5ac7 d945 df53 f1ac 3c6a  0D)L..Z..E.S..<j
-000001e0: 6aeb 2f50 4b03 0414 0000 0008 00bd b4a2  j./PK...........
-000001f0: 58fc 0e7b 4b5c 0000 005c 0000 001b 0000  X..{K\...\......
-00000200: 006d 6f6a 6969 2d30 2e31 2e31 2e64 6973  .mojii-0.1.1.dis
-00000210: 742d 696e 666f 2f57 4845 454c 0bcf 484d  t-info/WHEEL..HM
-00000220: cdd1 0d4b 2d2a cecc cfb3 5230 d433 e072  ...K-*....R0.3.r
-00000230: 4fcd 4b2d 4a2c c92f b252 484a c92c 2e89  O.K-J,./.RHJ.,..
-00000240: 2f07 a951 d030 d033 31d6 33d0 e40a cacf  /..Q.0.31.3.....
-00000250: 2fd1 f52c d60d 282d 4acd c94c b252 2829  /..,..(-J..L.R()
-00000260: 2a4d e50a 494c b752 28a8 34d6 cdcb cf4b  *M..IL.R(.4....K
-00000270: d54d ccab e4e2 0200 504b 0304 1400 0000  .M......PK......
-00000280: 0800 bdb4 a258 b2d4 6fd5 0700 0000 0500  .....X..o.......
-00000290: 0000 2300 0000 6d6f 6a69 692d 302e 312e  ..#...mojii-0.1.
-000002a0: 312e 6469 7374 2d69 6e66 6f2f 746f 705f  1.dist-info/top_
-000002b0: 6c65 7665 6c2e 7478 74cb cdcf cae4 0200  level.txt.......
-000002c0: 504b 0304 1400 0000 0800 bdb4 a258 194c  PK...........X.L
-000002d0: 4cca 2401 0000 a901 0000 1c00 0000 6d6f  L.$...........mo
-000002e0: 6a69 692d 302e 312e 312e 6469 7374 2d69  jii-0.1.1.dist-i
-000002f0: 6e66 6f2f 5245 434f 5244 75d0 4d6f 8230  nfo/RECORDu.Mo.0
-00000300: 00c6 f1bb 9fa5 282a e5e5 b003 0222 283a  ......(*....."(:
-00000310: a048 e6a5 615a a548 a193 22b2 4fbf b984  .H..aZ.H..".O...
-00000320: 6417 f324 ffe3 eff0 b0ba a013 8c69 4505  d..$.........iE.
-00000330: c663 de83 26cf 6650 7d53 34db 0979 a1af  .c..&.fP}S4..y..
-00000340: 1671 2661 e4b1 5482 be45 da90 4457 06b7  .q&a..T..E..DW..
-00000350: 01f7 d383 3bcf e376 9900 79c4 9eca 33ff  ....;..v..y...3.
-00000360: 0491 bf13 b667 5e21 475c eebf 522b 8b95  .....g^!G\..R+..
-00000370: 29d3 19ea 2c53 e9ed 1b64 92f0 0e55 70f6  )...,S...d...Up.
-00000380: 1330 877f 0495 e4f1 f477 27da 0889 56e7  .0.......w'...V.
-00000390: 7a12 38c8 b44d 640e a86c 2b47 9cf9 c834  z.8..Md..l+G...4
-000003a0: 4cab 28ef a730 246b 845b 9d04 8fd6 3733  L.(..0$k.[....73
-000003b0: 14bb f448 4915 f587 0bd0 66b3 176a ba72  ...HI.....f..j.r
-000003c0: 9ccd 40ba be26 f035 5d2c fbee 33bb ac21  ..@..&.5],..3..!
-000003d0: a90d af4e ba4d aad6 fd8e a035 0b25 83ae  ...N.M.....5.%..
-000003e0: 96fb ed23 04c6 2b51 d41c 97e4 4eca b178  ...#..+Q....N..x
-000003f0: 8841 ee8e 3264 4e08 bfcb 8f9d 95b8 a5a1  .A..2dN.........
-00000400: 064a 9122 95f3 c638 0955 dd5a b97e d59a  .J."...8.U.Z.~..
-00000410: 5b7f f7c0 ab03 22c7 da45 3600 a31f 504b  [....."..E6...PK
-00000420: 0102 1400 1400 0000 0800 9b4c 9058 0000  ...........L.X..
-00000430: 0000 0200 0000 0000 0000 1000 0000 0000  ................
-00000440: 0000 0000 0000 b681 0000 0000 6d6f 6a69  ............moji
-00000450: 2f5f 5f69 6e69 745f 5f2e 7079 504b 0102  /__init__.pyPK..
-00000460: 1400 1400 0000 0800 e14c 9058 5b1b 6b95  .........L.X[.k.
-00000470: 2300 0000 2300 0000 0c00 0000 0000 0000  #...#...........
-00000480: 0000 0000 b681 3000 0000 6d6f 6a69 2f6d  ......0...moji/m
-00000490: 6f6a 692e 7079 504b 0102 1400 1400 0000  oji.pyPK........
-000004a0: 0800 bdb4 a258 4f2e 3d11 2a01 0000 d202  .....XO.=.*.....
-000004b0: 0000 1e00 0000 0000 0000 0000 0000 b681  ................
-000004c0: 7d00 0000 6d6f 6a69 692d 302e 312e 312e  }...mojii-0.1.1.
-000004d0: 6469 7374 2d69 6e66 6f2f 4d45 5441 4441  dist-info/METADA
-000004e0: 5441 504b 0102 1400 1400 0000 0800 bdb4  TAPK............
-000004f0: a258 fc0e 7b4b 5c00 0000 5c00 0000 1b00  .X..{K\...\.....
-00000500: 0000 0000 0000 0000 0000 b681 e301 0000  ................
-00000510: 6d6f 6a69 692d 302e 312e 312e 6469 7374  mojii-0.1.1.dist
-00000520: 2d69 6e66 6f2f 5748 4545 4c50 4b01 0214  -info/WHEELPK...
-00000530: 0014 0000 0008 00bd b4a2 58b2 d46f d507  ..........X..o..
-00000540: 0000 0005 0000 0023 0000 0000 0000 0000  .......#........
-00000550: 0000 00b6 8178 0200 006d 6f6a 6969 2d30  .....x...mojii-0
-00000560: 2e31 2e31 2e64 6973 742d 696e 666f 2f74  .1.1.dist-info/t
-00000570: 6f70 5f6c 6576 656c 2e74 7874 504b 0102  op_level.txtPK..
-00000580: 1400 1400 0000 0800 bdb4 a258 194c 4cca  ...........X.LL.
-00000590: 2401 0000 a901 0000 1c00 0000 0000 0000  $...............
-000005a0: 0000 0000 b481 c002 0000 6d6f 6a69 692d  ..........mojii-
-000005b0: 302e 312e 312e 6469 7374 2d69 6e66 6f2f  0.1.1.dist-info/
-000005c0: 5245 434f 5244 504b 0506 0000 0000 0600  RECORDPK........
-000005d0: 0600 a801 0000 1e04 0000 0000            ............
+00000000: 1f8b 0808 a616 3466 02ff 6d6f 6a69 692d  ......4f..mojii-
+00000010: 302e 312e 322e 7461 7200 ed5c 6d73 9b38  0.1.2.tar..\ms.8
+00000020: 10ce 6766 f80f 3af7 83ed 9918 f34e e219  ..gf..:......N..
+00000030: 669a 6b72 6dae 4d93 4972 771f 3a1d 4605  f.krm.M.Irw.:.F.
+00000040: d9d1 0510 0722 89ff fd49 60dc d879 6999  ....."...I`..yi.
+00000050: c65c e7bc cf87 1824 ed22 22ed 3e2b d0a2  .\.....$."".>+..
+00000060: 8db5 f1eb 337c f78e e088 e43b 1b81 5ee3  ....3|.....;..^.
+00000070: a95f 5db7 ccaf c7b2 dcd0 4d43 df41 773b  ._].......MC.Aw;
+00000080: 1da0 2c38 cec5 e577 b613 a68b 124e 13e2  ..,8...w.....N..
+00000090: 1b9e 61bb 7bfb 9e6e 6a86 69da b6b2 03d8  ..a.{..nj.i.....
+000000a0: 0224 ec6f 4a47 ba66 68e6 7853 d790 46ed  .$.oJG.fh.xS..F.
+000000b0: 79de d3f6 2f8e c5e4 331c ddb0 4cdb 15e5  y.../...3...L...
+000000c0: 9ee3 383b c801 fbdf 38b4 9fc2 ffdb 0ffd  ..8;....8.......
+000000d0: bf09 febf 13ff bff7 88ff 37f6 f675 c702  ..........7..u..
+000000e0: 06d8 32ff 7ff6 feed e8f8 e36f a79b b07f  ..2........o....
+000000f0: d775 9fb2 7fe1 f4cd 55ff 6fe8 ae23 e23f  .u......U.o..#.?
+00000100: 1dec 7fe3 3821 1c47 98e3 d19f 242f 284b  ....8!.G....$/(K
+00000110: 2748 d8bf aa7c c409 99a0 6a72 a8ca b2aa  'H...|....jr....
+00000120: 9a26 aa72 5126 09ce e713 7448 1286 62fa  .&.rQ&....tH..b.
+00000130: 2517 67aa 7250 f22b 964f d0ef 6c3a cdc9  %.g.rP.+.O..l:..
+00000140: 1cfd 4a49 7a43 d2b2 a919 9104 d378 82c8  ..JIzC.......x..
+00000150: 1d4e b298 bcae 4eb5 9025 aaf2 8186 242d  .N....N..%....$-
+00000160: c415 4f8e 2f55 e54d 8c8b 824e 2911 ca8e  ..O./U.M...N)...
+00000170: 534e d288 44e8 a08c 84be 90a0 89bc ee0d  SN..D...........
+00000180: 8959 26ba b5da 78a1 4636 39bd 3846 0759  .Y&...x.F69.8F.Y
+00000190: 96b3 1b21 3ba9 1437 d5ab 3267 399b e538  ...!;..7..2g9..8
+000001a0: 4968 3a43 1f70 3a2b f1ac 5270 3617 7d4e  Ih:C.p:+..Rp6.}N
+000001b0: dbb4 9547 566b 01cd 6d2f e2b5 17d9 6b2f  ...GVk..m/....k/
+000001c0: b2df 5ec4 3057 654e c518 612e 252e e605  ..^.0WeN..a.%...
+000001d0: 2749 3d32 6250 2392 c961 4db9 aa1c 9222  'I=2bP#..aM...."
+000001e0: cc69 c6c5 0c1b bd61 72b8 f9e8 729e 89c9  .i.....ar...r...
+000001f0: c0c9 1d1f 8b99 761d b15b 3112 e7e4 9f92  ......v..[1.....
+00000200: e6a4 181d d282 4f50 5a26 9998 75aa f2aa  ......OPZ&..u...
+00000210: 9aa7 e83d ce69 2266 2bf8 7488 ffc0 ffff  ...=.i"f+.t.....
+00000220: 48fc a7ef dbb6 6142 fcb7 6df1 9f3c 1e6f  H.....aB..m..<.o
+00000230: c8fe 5bad ff0d dd31 2c58 ff6f 8dff 37dd  ..[....1,X.o..7.
+00000240: 87fe df02 ffdf 89ff 37bf fa7f cb74 c53f  ........7....t.?
+00000250: ded1 74f0 fcdb ebff 8380 a694 0781 96cd  ..t.............
+00000260: 3b5a ff37 fe5f f76c 5b4c 41c1 1386 e99a  ;Z.7._.l[LA.....
+00000270: 0eac ffc1 ffc3 f877 e9ff 65fc ef3a 36f8  .......w..e..:6.
+00000280: ff6d f6ff f2cf 0bfa feef f1ff 86e5 2ee3  .m..............
+00000290: 7f43 b633 4cdd b4c1 ff77 019a 642c e7f5  .C.3L....w..d,..
+000002a0: 1334 5ca0 4255 2232 4578 309c a80a 12c8  .4\.BU"2Ex0.....
+000002b0: 729a f241 ff1d 8963 86fe 6279 1cfd d21f  r..A...c..by....
+000002c0: caa7 6eaa 42a7 2808 529c 9020 40be 8ffa  ..n.B.(.R.. @...
+000002d0: 4190 609a 0641 7f21 2a94 807d 01ff c3f3  A.`..A.!*..}....
+000002e0: bf9f 9aff 1f7d ffeb 9aee be0b 51c0 16f2  .....}......Q...
+000002f0: 3fd5 c86c 36a2 e994 8d5f d4fe db3d ff33  ?..l6...._...=.3
+00000300: 2dc7 85e7 7fb0 fe83 f1ef 7afd e7e9 06ac  -.........z.....
+00000310: ffc0 ff4b ffff 62db 81da edff 7184 fd5b  ...K..b.....q..[
+00000320: 36ec ffe9 06b0 ff07 f6ff c0fe 1f58 ff43  6............X.C
+00000330: fc07 f11f c47f 10ff dd8b ff2e 4eff 387f  ............N.8.
+00000340: 7374 a1f1 3bbe d1f8 4f98 bfbb 16ff d9f2  st..;...O.......
+00000350: 07e2 bf0e 5010 5e66 5a36 57d6 5ffe 2bf7  ....P.^fZ6W._.+.
+00000360: df06 294f 2c0d 94a7 a7cc 7a55 c3f8 e13c  ..)O,.....zU...<
+00000370: 8869 7a5d 3cd6 265f 30fc 6375 9c65 412c  .iz]<.&_0.cu.eA,
+00000380: e3be 1f9f 8f00 e07f b07f e07f c0b3 fcff  ................
+00000390: 98c7 de08 ffeb bab1 c6ff ae6d 5ac0 ff5d  ...........mZ..]
+000003a0: 004c 1df8 1ff8 1ff8 1ff8 1ff8 ff99 d5d8  .L..............
+000003b0: 46d7 ffa2 767d fdef 3906 f07f 17a8 9ea2  F...v}..9.......
+000003c0: 83bd 03ff 03ff 03ff 03ff 03ff 6fe0 89eb  ............o...
+000003d0: b7f9 df59 e37f 4778 00e0 ffae c61f cc1d  ...Y..Gx........
+000003e0: f8ff bfdd ff6f 3de4 7f03 f8bf 13fe f71e  .....o=.........
+000003f0: fbfe a765 db0e 7885 6de3 fffa 5d70 389d  ...e..x.m...]p8.
+00000400: 6dc0 fe9f e57f 67fd fb6f 86e5 c1f3 ff4e  m.....g..o.....N
+00000410: f049 847b 810c f73e ab0a c7b3 e04b 49e3  .I.{...>.....KI.
+00000420: 08f9 a83e 8b30 27e2 4497 dbec c056 80ff  ...>.0'.D....V..
+00000430: 61fd ff7f 5fff 43fe ffb6 f3ff cbe6 fe7f  a..._.C.........
+00000440: 07ff 9b8e 61ac e5ff 1bf2 3330 c0ff 1de0  ....a.....30....
+00000450: 153a 886f f1bc 4059 4ea6 2447 d51c e08c  .:.o..@YN.$G....
+00000460: c505 6237 e23c a205 2f39 8d0b 5599 e62c  ..b7.<../9..U..,
+00000470: b95f bff8 7440 55b2 8ba6 348d 820c 87d7  ._..t@U...4.....
+00000480: 7846 8a7a 5bfe 2543 6541 1046 214b 0ba1  xF.z[.%CeA.F!K..
+00000490: 87a4 1c91 3464 114d 670b 75e2 8484 4b55  ....4d.Mg.u...KU
+000004a0: 2c23 e9a2 822d 0b33 ccaf 16fa ae88 e84f  ,#...-.3.......O
+000004b0: 4e42 cef2 b954 ca31 4d65 7201 bfa2 85e8  NB...T.1Mer.....
+000004c0: 404c 54e5 ddd1 f991 8858 a490 86bf 14f2  @LT......X......
+000004d0: 7750 9d08 41f9 ad82 4110 c886 4130 1cd6  wP..A...A...A0..
+000004e0: 4adf 122e e409 8a99 5014 7dcd 4540 5537  J.......P.}.E@U7
+000004f0: 64cd f9d1 c1e1 c9d1 42ff 2de5 5755 3f6b  d.......B.-.WU?k
+00000500: ad7f 339a 0ee4 3577 513f 1714 9a10 2d89  ..3...5wQ?....-.
+00000510: fac3 dde5 7dfa fd92 4f47 7bfd a1fc bac2  ....}...OG{.....
+00000520: 74f1 6504 79ad e0fe b57c 34d5 a4f8 60d8  t.e.y....|4...`.
+00000530: dca9 b8a1 10c7 31e2 acfe 070f 8628 62a4  ......1......(b.
+00000540: 4055 99e8 d42d cbaf 55a5 aeaa 95ca bbf3  @U...-..U.......
+00000550: 7b95 3df7 76eb a29b 3a71 c7ef 55f6 dd94  {.=.v...:q..U...
+00000560: debb b0df bb9f c2d3 3458 ef9e bf5e f044  ........4X...^.D
+00000570: bb20 acd3 3702 3ecf 4457 56d2 371a ddaf  . ..7.>.DWV.7...
+00000580: 5099 c77e ef8a f3ac 988c ebfd a5f2 cec5  P..~............
+00000590: 3d45 2c2c 34ca c64d 535c 650d f9bd f57c  =E,,4..MS\e....|
+000005a0: a2d5 faa0 4a23 f27b 0fb2 8a96 7753 67fd  ....J#.{....wSg.
+000005b0: f8bd 93e3 cba6 2c5c e6a8 14fe a7ba 48a2  ......,\......H.
+000005c0: f78d 6ca3 46bc 6afb 7dc9 462b 22cf a7d0  ..l.F.j.}.F+"...
+000005d0: b468 5a65 dbb4 6daf b9ad 25bc d612 7bad  .hZe..m...%...{.
+000005e0: 25f6 5b4b 18e6 8ac8 b793 8c7a 75eb cf0b  %.[K.......zu...
+000005f0: a9c6 4bf9 9f2a 73e9 35e5 340d e332 228d  ..K..*s.5.4..2".
+00000600: 1793 ab1f ec5f e625 59d6 0bae 88e3 a079  ....._.%Y......y
+00000610: 312e e4ab d7a7 3db1 7682 4f9d 0000 0000  1.....=.v.O.....
+00000620: 0000 0000 0000 0000 00f8 59f1 2fca 24f4  ..........Y./.$.
+00000630: 3c00 7800 00                             <.x..
```
