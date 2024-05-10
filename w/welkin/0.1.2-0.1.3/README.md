# Comparing `tmp/welkin-0.1.2.tar.gz` & `tmp/welkin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "welkin-0.1.2.tar", max compression
+gzip compressed data, was "welkin-0.1.3.tar", max compression
```

## Comparing `welkin-0.1.2.tar` & `welkin-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34659 2024-02-28 22:22:39.051095 welkin-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     2228 2024-02-28 22:22:39.051095 welkin-0.1.2/README.md
--rw-r--r--   0        0        0     1296 2024-02-28 22:22:39.051095 welkin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2228 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/__init__.py
--rw-r--r--   0        0        0      503 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/__version__.py
--rw-r--r--   0        0        0     1848 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/authentication.py
--rw-r--r--   0        0        0     9598 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/client.py
--rw-r--r--   0        0        0      746 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/exceptions.py
--rw-r--r--   0        0        0     1644 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/__init__.py
--rw-r--r--   0        0        0     3148 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/assessment.py
--rw-r--r--   0        0        0     3548 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/base.py
--rw-r--r--   0        0        0     3892 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/calendar.py
--rw-r--r--   0        0        0      690 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/care_plan.py
--rw-r--r--   0        0        0     2008 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/cdt.py
--rw-r--r--   0        0        0     1542 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/chat.py
--rw-r--r--   0        0        0     2065 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/document.py
--rw-r--r--   0        0        0      802 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/email.py
--rw-r--r--   0        0        0     3127 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/encounter.py
--rw-r--r--   0        0        0     2663 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/formation.py
--rw-r--r--   0        0        0     2377 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/patient.py
--rw-r--r--   0        0        0     2172 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/program.py
--rw-r--r--   0        0        0      791 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/sms.py
--rw-r--r--   0        0        0     1596 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/models/user.py
--rw-r--r--   0        0        0     5270 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/pagination.py
--rw-r--r--   0        0        0     5430 2024-02-28 22:22:39.059095 welkin-0.1.2/welkin/util.py
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 welkin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35050 2024-05-10 19:52:28.724519 welkin-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2226 2024-05-10 19:52:28.724519 welkin-0.1.3/README.md
+-rw-r--r--   0        0        0     2889 2024-05-10 19:52:28.728520 welkin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2250 2024-05-10 19:52:28.732519 welkin-0.1.3/welkin/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-10 19:52:28.732519 welkin-0.1.3/welkin/__version__.py
+-rw-r--r--   0        0        0     1897 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/authentication.py
+-rw-r--r--   0        0        0    10160 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/client.py
+-rw-r--r--   0        0        0      789 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/exceptions.py
+-rw-r--r--   0        0        0     1644 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/assessment.py
+-rw-r--r--   0        0        0     3651 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/base.py
+-rw-r--r--   0        0        0     4049 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/calendar.py
+-rw-r--r--   0        0        0      727 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/care_plan.py
+-rw-r--r--   0        0        0     2159 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/cdt.py
+-rw-r--r--   0        0        0     1556 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/chat.py
+-rw-r--r--   0        0        0     2108 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/document.py
+-rw-r--r--   0        0        0      845 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/email.py
+-rw-r--r--   0        0        0     3312 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/encounter.py
+-rw-r--r--   0        0        0     2637 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/formation.py
+-rw-r--r--   0        0        0     2456 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/patient.py
+-rw-r--r--   0        0        0     2321 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/program.py
+-rw-r--r--   0        0        0      834 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/sms.py
+-rw-r--r--   0        0        0     1617 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/models/user.py
+-rw-r--r--   0        0        0     5300 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/pagination.py
+-rw-r--r--   0        0        0     5447 2024-05-10 19:52:28.736519 welkin-0.1.3/welkin/util.py
+-rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 welkin-0.1.3/PKG-INFO
```

### Comparing `welkin-0.1.2/LICENSE.md` & `welkin-0.1.3/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-# GNU GENERAL PUBLIC LICENSE
+<p align="center">
+  <img src="https://www.gnu.org/graphics/gplv3-or-later.svg" width="200" height="84"/>
+</p>
 
-### Version 3, 29 June 2007
+# <p align="center">GNU GENERAL PUBLIC LICENSE</p>
 
-Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-Everyone is permitted to copy and distribute verbatim copies
-of this license document, but changing it is not allowed.
+***<p align="center">Version 3, 29 June 2007</p>***
 
-## Preamble
+Copyright (C) 2007 Free Software Foundation, Inc.
+<<https://fsf.org/>>
+
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+## <p align="center">Preamble</p>
 
 The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
 
 The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works. By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users. We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors. You can apply it to
-your programs, too.
+the GNU General Public License is intended to guarantee your freedom
+to share and change all versions of a program--to make sure it remains
+free software for all its users. We, the Free Software Foundation, use
+the GNU General Public License for most of our software; it applies
+also to any other work released this way by its authors. You can apply
+it to your programs, too.
 
 When we speak of free software, we are referring to freedom, not
 price. Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
 To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights. Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
+these rights or asking you to surrender the rights. Therefore, you
+have certain responsibilities if you distribute copies of the
+software, or if you modify it: responsibilities to respect the freedom
+of others.
 
 For example, if you distribute copies of such a program, whether
 gratis or for a fee, you must pass on to the recipients the same
 freedoms that you received. You must make sure that they, too, receive
 or can get the source code. And you must show them these terms so they
 know their rights.
 
@@ -45,80 +53,82 @@
 For the developers' and authors' protection, the GPL clearly explains
 that there is no warranty for this free software. For both users' and
 authors' sake, the GPL requires that modified versions be marked as
 changed, so that their problems will not be attributed erroneously to
 authors of previous versions.
 
 Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so. This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software. The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable. Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products. If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
+modified versions of the software inside them, although the
+manufacturer can do so. This is fundamentally incompatible with the
+aim of protecting users' freedom to change the software. The
+systematic pattern of such abuse occurs in the area of products for
+individuals to use, which is precisely where it is most unacceptable.
+Therefore, we have designed this version of the GPL to prohibit the
+practice for those products. If such problems arise substantially in
+other domains, we stand ready to extend this provision to those
+domains in future versions of the GPL, as needed to protect the
+freedom of users.
 
 Finally, every program is threatened constantly by software patents.
 States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary. To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+software on general-purpose computers, but in those that do, we wish
+to avoid the special danger that patents applied to a free program
+could make it effectively proprietary. To prevent this, the GPL
+assures that patents cannot be used to render the program non-free.
 
 The precise terms and conditions for copying, distribution and
 modification follow.
 
-## TERMS AND CONDITIONS
+## <p align="center">TERMS AND CONDITIONS</p>
 
-### 0. Definitions.
+### *0. Definitions.*
 
 "This License" refers to version 3 of the GNU General Public License.
 
-"Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
 
 "The Program" refers to any copyrightable work licensed under this
 License. Each licensee is addressed as "you". "Licensees" and
 "recipients" may be individuals or organizations.
 
 To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy. The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
 
 A "covered work" means either the unmodified Program or a work based
 on the Program.
 
 To "propagate" a work means to do anything with it that, without
 permission, would make you directly or secondarily liable for
 infringement under applicable copyright law, except executing it on a
 computer or modifying a private copy. Propagation includes copying,
 distribution (with or without modification), making available to the
 public, and in some countries other activities as well.
 
 To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
 
-An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
+An interactive user interface displays "Appropriate Legal Notices" to
+the extent that it includes a convenient and prominently visible
 feature that (1) displays an appropriate copyright notice, and (2)
 tells the user that there is no warranty for the work (except to the
 extent that warranties are provided), that licensees may convey the
 work under this License, and how to view a copy of this License. If
 the interface presents a list of user commands or options, such as a
 menu, a prominent item in the list meets this criterion.
 
-### 1. Source Code.
+### *1. Source Code.*
 
-The "source code" for a work means the preferred form of the work
-for making modifications to it. "Object code" means any non-source
-form of a work.
+The "source code" for a work means the preferred form of the work for
+making modifications to it. "Object code" means any non-source form of
+a work.
 
 A "Standard Interface" means an interface that either is an official
 standard defined by a recognized standards body, or, in the case of
 interfaces specified for a particular programming language, one that
 is widely used among developers working in that language.
 
 The "System Libraries" of an executable work include anything, other
@@ -141,210 +151,206 @@
 which are not part of the work. For example, Corresponding Source
 includes interface definition files associated with source files for
 the work, and the source code for shared libraries and dynamically
 linked subprograms that the work is specifically designed to require,
 such as by intimate data communication or control flow between those
 subprograms and other parts of the work.
 
-The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
+The Corresponding Source need not include anything that users can
+regenerate automatically from other parts of the Corresponding Source.
 
-The Corresponding Source for a work in source code form is that
-same work.
+The Corresponding Source for a work in source code form is that same
+work.
 
-### 2. Basic Permissions.
+### *2. Basic Permissions.*
 
 All rights granted under this License are granted for the term of
 copyright on the Program, and are irrevocable provided the stated
 conditions are met. This License explicitly affirms your unlimited
 permission to run the unmodified Program. The output from running a
 covered work is covered by this License only if the output, given its
 content, constitutes a covered work. This License acknowledges your
 rights of fair use or other equivalent, as provided by copyright law.
 
-You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force. You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright. Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under
-the conditions stated below. Sublicensing is not allowed; section 10
-makes it unnecessary.
+You may make, run and propagate covered works that you do not convey,
+without conditions so long as your license otherwise remains in force.
+You may convey covered works to others for the sole purpose of having
+them make modifications exclusively for you, or provide you with
+facilities for running those works, provided that you comply with the
+terms of this License in conveying all material for which you do not
+control copyright. Those thus making or running the covered works for
+you must do so exclusively on your behalf, under your direction and
+control, on terms that prohibit them from making any copies of your
+copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the
+conditions stated below. Sublicensing is not allowed; section 10 makes
+it unnecessary.
 
-### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+### *3. Protecting Users' Legal Rights From Anti-Circumvention Law.*
 
 No covered work shall be deemed part of an effective technological
 measure under any applicable law fulfilling obligations under article
 11 of the WIPO copyright treaty adopted on 20 December 1996, or
 similar laws prohibiting or restricting circumvention of such
 measures.
 
 When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
 
-### 4. Conveying Verbatim Copies.
+### *4. Conveying Verbatim Copies.*
 
 You may convey verbatim copies of the Program's source code as you
 receive it, in any medium, provided that you conspicuously and
 appropriately publish on each copy an appropriate copyright notice;
 keep intact all notices stating that this License and any
 non-permissive terms added in accord with section 7 apply to the code;
 keep intact all notices of the absence of any warranty; and give all
 recipients a copy of this License along with the Program.
 
 You may charge any price or no price for each copy that you convey,
 and you may offer support or warranty protection for a fee.
 
-### 5. Conveying Modified Source Versions.
+### *5. Conveying Modified Source Versions.*
 
 You may convey a work based on the Program, or the modifications to
 produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
+terms of section 4, provided that you also meet all of these
+conditions:
 
 - a) The work must carry prominent notices stating that you modified
-  it, and giving a relevant date.
-
+    it, and giving a relevant date.
 - b) The work must carry prominent notices stating that it is
-  released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to
-  "keep intact all notices".
-
+    released under this License and any conditions added under
+    section 7. This requirement modifies the requirement in section 4
+    to "keep intact all notices".
 - c) You must license the entire work, as a whole, under this
-  License to anyone who comes into possession of a copy. This
-  License will therefore apply, along with any applicable section 7
-  additional terms, to the whole of the work, and all its parts,
-  regardless of how they are packaged. This License gives no
-  permission to license the work in any other way, but it does not
-  invalidate such permission if you have separately received it.
-
+    License to anyone who comes into possession of a copy. This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged. This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
 - d) If the work has interactive user interfaces, each must display
-  Appropriate Legal Notices; however, if the Program has interactive
-  interfaces that do not display Appropriate Legal Notices, your
-  work need not make them do so.
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
 
 A compilation of a covered work with other separate and independent
 works, which are not by their nature extensions of the covered work,
 and which are not combined with it such as to form a larger program,
 in or on a volume of a storage or distribution medium, is called an
 "aggregate" if the compilation and its resulting copyright are not
 used to limit the access or legal rights of the compilation's users
 beyond what the individual works permit. Inclusion of a covered work
 in an aggregate does not cause this License to apply to the other
 parts of the aggregate.
 
-### 6. Conveying Non-Source Forms.
+### *6. Conveying Non-Source Forms.*
 
-You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
+You may convey a covered work in object code form under the terms of
+sections 4 and 5, provided that you also convey the machine-readable
+Corresponding Source under the terms of this License, in one of these
+ways:
 
 - a) Convey the object code in, or embodied in, a physical product
-  (including a physical distribution medium), accompanied by the
-  Corresponding Source fixed on a durable physical medium
-  customarily used for software interchange.
-
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
 - b) Convey the object code in, or embodied in, a physical product
-  (including a physical distribution medium), accompanied by a
-  written offer, valid for at least three years and valid for as
-  long as you offer spare parts or customer support for that product
-  model, to give anyone who possesses the object code either (1) a
-  copy of the Corresponding Source for all the software in the
-  product that is covered by this License, on a durable physical
-  medium customarily used for software interchange, for a price no
-  more than your reasonable cost of physically performing this
-  conveying of source, or (2) access to copy the
-  Corresponding Source from a network server at no charge.
-
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the Corresponding
+    Source from a network server at no charge.
 - c) Convey individual copies of the object code with a copy of the
-  written offer to provide the Corresponding Source. This
-  alternative is allowed only occasionally and noncommercially, and
-  only if you received the object code with such an offer, in accord
-  with subsection 6b.
-
+    written offer to provide the Corresponding Source. This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
 - d) Convey the object code by offering access from a designated
-  place (gratis or for a charge), and offer equivalent access to the
-  Corresponding Source in the same way through the same place at no
-  further charge. You need not require recipients to copy the
-  Corresponding Source along with the object code. If the place to
-  copy the object code is a network server, the Corresponding Source
-  may be on a different server (operated by you or a third party)
-  that supports equivalent copying facilities, provided you maintain
-  clear directions next to the object code saying where to find the
-  Corresponding Source. Regardless of what server hosts the
-  Corresponding Source, you remain obligated to ensure that it is
-  available for as long as needed to satisfy these requirements.
-
-- e) Convey the object code using peer-to-peer transmission, provided
-  you inform other peers where the object code and Corresponding
-  Source of the work are being offered to the general public at no
-  charge under subsection 6d.
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge. You need not require recipients to copy the
+    Corresponding Source along with the object code. If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source. Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+- e) Convey the object code using peer-to-peer transmission,
+    provided you inform other peers where the object code and
+    Corresponding Source of the work are being offered to the general
+    public at no charge under subsection 6d.
 
 A separable portion of the object code, whose source code is excluded
 from the Corresponding Source as a System Library, need not be
 included in conveying the object code work.
 
 A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling. In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage. For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product. A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
+incorporation into a dwelling. In determining whether a product is a
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
 
 "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source. The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
 
 If you convey an object code work under this section in, or with, or
 specifically for use in, a User Product, and the conveying occurs as
 part of a transaction in which the right of possession and use of the
 User Product is transferred to the recipient in perpetuity or for a
 fixed term (regardless of how the transaction is characterized), the
 Corresponding Source conveyed under this section must be accompanied
 by the Installation Information. But this requirement does not apply
 if neither you nor any third party retains the ability to install
 modified object code on the User Product (for example, the work has
 been installed in ROM).
 
 The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed. Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
 
 Corresponding Source conveyed, and Installation Information provided,
 in accord with this section must be in a format that is publicly
 documented (and with an implementation available to the public in
 source code form), and must require no special password or key for
 unpacking, reading or copying.
 
-### 7. Additional Terms.
+### *7. Additional Terms.*
 
 "Additional permissions" are terms that supplement the terms of this
 License by making exceptions from one or more of its conditions.
 Additional permissions that are applicable to the entire Program shall
 be treated as though they were included in this License, to the extent
 that they are valid under applicable law. If additional permissions
 apply only to part of the Program, that part may be used separately
@@ -355,39 +361,34 @@
 remove any additional permissions from that copy, or from any part of
 it. (Additional permissions may be written to require their own
 removal in certain cases when you modify the work.) You may place
 additional permissions on material, added by you to a covered work,
 for which you have or can give appropriate copyright permission.
 
 Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
+add to a covered work, you may (if authorized by the copyright holders
+of that material) supplement the terms of this License with terms:
 
 - a) Disclaiming warranty or limiting liability differently from the
-  terms of sections 15 and 16 of this License; or
-
+    terms of sections 15 and 16 of this License; or
 - b) Requiring preservation of specified reasonable legal notices or
-  author attributions in that material or in the Appropriate Legal
-  Notices displayed by works containing it; or
-
-- c) Prohibiting misrepresentation of the origin of that material, or
-  requiring that modified versions of such material be marked in
-  reasonable ways as different from the original version; or
-
-- d) Limiting the use for publicity purposes of names of licensors or
-  authors of the material; or
-
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+- c) Prohibiting misrepresentation of the origin of that material,
+    or requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+- d) Limiting the use for publicity purposes of names of licensors
+    or authors of the material; or
 - e) Declining to grant rights under trademark law for use of some
-  trade names, trademarks, or service marks; or
-
+    trade names, trademarks, or service marks; or
 - f) Requiring indemnification of licensors and authors of that
-  material by anyone who conveys the material (or modified versions of
-  it) with contractual assumptions of liability to the recipient, for
-  any liability that these contractual assumptions directly impose on
-  those licensors and authors.
+    material by anyone who conveys the material (or modified versions
+    of it) with contractual assumptions of liability to the recipient,
+    for any liability that these contractual assumptions directly
+    impose on those licensors and authors.
 
 All other non-permissive additional terms are considered "further
 restrictions" within the meaning of section 10. If the Program as you
 received it, or any part of it, contains a notice stating that it is
 governed by this License along with a term that is a further
 restriction, you may remove that term. If a license document contains
 a further restriction but permits relicensing or conveying under this
@@ -397,57 +398,57 @@
 
 If you add terms to a covered work in accord with this section, you
 must place, in the relevant source files, a statement of the
 additional terms that apply to those files, or a notice indicating
 where to find the applicable terms.
 
 Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
 
-### 8. Termination.
+### *8. Termination.*
 
 You may not propagate or modify a covered work except as expressly
 provided under this License. Any attempt otherwise to propagate or
 modify it is void, and will automatically terminate your rights under
 this License (including any patent licenses granted under the third
 paragraph of section 11).
 
-However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
+However, if you cease all violation of this License, then your license
+from a particular copyright holder is reinstated (a) provisionally,
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
 
 Moreover, your license from a particular copyright holder is
 reinstated permanently if the copyright holder notifies you of the
 violation by some reasonable means, this is the first time you have
 received notice of violation of this License (for any work) from that
 copyright holder, and you cure the violation prior to 30 days after
 your receipt of the notice.
 
 Termination of your rights under this section does not terminate the
 licenses of parties who have received copies or rights from you under
 this License. If your rights have been terminated and not permanently
 reinstated, you do not qualify to receive new licenses for the same
 material under section 10.
 
-### 9. Acceptance Not Required for Having Copies.
+### *9. Acceptance Not Required for Having Copies.*
 
-You are not required to accept this License in order to receive or
-run a copy of the Program. Ancillary propagation of a covered work
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
 occurring solely as a consequence of using peer-to-peer transmission
 to receive a copy likewise does not require acceptance. However,
 nothing other than this License grants you permission to propagate or
 modify any covered work. These actions infringe copyright if you do
 not accept this License. Therefore, by modifying or propagating a
 covered work, you indicate your acceptance of this License to do so.
 
-### 10. Automatic Licensing of Downstream Recipients.
+### *10. Automatic Licensing of Downstream Recipients.*
 
 Each time you convey a covered work, the recipient automatically
 receives a license from the original licensors, to run, modify and
 propagate that work, subject to this License. You are not responsible
 for enforcing compliance by third parties with this License.
 
 An "entity transaction" is a transaction transferring control of an
@@ -464,22 +465,22 @@
 rights granted or affirmed under this License. For example, you may
 not impose a license fee, royalty, or other charge for exercise of
 rights granted under this License, and you may not initiate litigation
 (including a cross-claim or counterclaim in a lawsuit) alleging that
 any patent claim is infringed by making, using, selling, offering for
 sale, or importing the Program or any portion of it.
 
-### 11. Patents.
+### *11. Patents.*
 
 A "contributor" is a copyright holder who authorizes use under this
 License of the Program or a work on which the Program is based. The
 work thus licensed is called the contributor's "contributor version".
 
-A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
 hereafter acquired, that would be infringed by some manner, permitted
 by this License, of making, using, or selling its contributor version,
 but do not include claims that would be infringed only as a
 consequence of further modification of the contributor version. For
 purposes of this definition, "control" includes the right to grant
 patent sublicenses in a manner consistent with the requirements of
 this License.
@@ -514,126 +515,129 @@
 arrangement, you convey, or propagate by procuring conveyance of, a
 covered work, and grant a patent license to some of the parties
 receiving the covered work authorizing them to use, propagate, modify
 or convey a specific copy of the covered work, then the patent license
 you grant is automatically extended to all recipients of the covered
 work and works based on it.
 
-A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License. You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
+A patent license is "discriminatory" if it does not include within the
+scope of its coverage, prohibits the exercise of, or is conditioned on
+the non-exercise of one or more of the rights that are specifically
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
 
 Nothing in this License shall be construed as excluding or limiting
 any implied license or other defenses to infringement that may
 otherwise be available to you under applicable patent law.
 
-### 12. No Surrender of Others' Freedom.
+### *12. No Surrender of Others' Freedom.*
 
 If conditions are imposed on you (whether by court order, agreement or
 otherwise) that contradict the conditions of this License, they do not
 excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all. For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
 
-### 13. Use with the GNU Affero General Public License.
+### *13. Use with the GNU Affero General Public License.*
 
 Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
 under version 3 of the GNU Affero General Public License into a single
 combined work, and to convey the resulting work. The terms of this
 License will continue to apply to the part which is the covered work,
 but the special requirements of the GNU Affero General Public License,
 section 13, concerning interaction through a network will apply to the
 combination as such.
 
-### 14. Revised Versions of this License.
+### *14. Revised Versions of this License.*
 
-The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time. Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number. If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation. If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
+The Free Software Foundation may publish revised and/or new versions
+of the GNU General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in
+detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program
+specifies that a certain numbered version of the GNU General Public
+License "or any later version" applies to it, you have the option of
+following the terms and conditions either of that numbered version or
+of any later version published by the Free Software Foundation. If the
+Program does not specify a version number of the GNU General Public
+License, you may choose any version ever published by the Free
+Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions
+of the GNU General Public License can be used, that proxy's public
+statement of acceptance of a version permanently authorizes you to
+choose that version for the Program.
 
 Later license versions may give you additional or different
 permissions. However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
 
-### 15. Disclaimer of Warranty.
+### *15. Disclaimer of Warranty.*
 
 THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
 APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
+WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
 
-### 16. Limitation of Liability.
+### *16. Limitation of Liability.*
 
 IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
+CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
 
-### 17. Interpretation of Sections 15 and 16.
+### *17. Interpretation of Sections 15 and 16.*
 
 If the disclaimer of warranty and limitation of liability provided
 above cannot be given local legal effect according to their terms,
 reviewing courts shall apply local law that most closely approximates
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
-#### _END OF TERMS AND CONDITIONS_
+#### **<p align="center">END OF TERMS AND CONDITIONS<p>**
 
-## How to Apply These Terms to Your New Programs
+## <p align="center">How to Apply These Terms to Your New Programs</p>
 
 If you develop a new program, and you want it to be of the greatest
 possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
+free software which everyone can redistribute and change under these
+terms.
 
-To do so, attach the following notices to the program. It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
+To do so, attach the following notices to the program. It is safest to
+attach them to the start of each source file to most effectively state
+the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
 
 ```
 <one line to give the program's name and a brief idea of what it does.>
 Copyright (C) <year>  <name of author>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
@@ -644,35 +648,37 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-Also add information on how to contact you by electronic and paper mail.
+Also add information on how to contact you by electronic and paper
+mail.
 ```
 
 If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
 ```
 <program>  Copyright (C) <year>  <name of author>
-This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+This program comes with ABSOLUTELY NO WARRANTY; for details type `show w`.
 This is free software, and you are welcome to redistribute it
-under certain conditions; type `show c' for details.
+under certain conditions; type `show c` for details.
 ```
 
-The hypothetical commands `show w` and `show c` should show the appropriate
-parts of the General Public License. Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-The GNU General Public License does not permit incorporating your program
-into proprietary programs. If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library. If this is what you want to do, use the GNU Lesser General
-Public License instead of this License. But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+The hypothetical commands `show w` and `show c` should show the
+appropriate parts of the General Public License. Of course, your
+program's commands might be different; for a GUI interface, you would
+use an "about box".
+
+You should also get your employer (if you work as a programmer) or
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary. For more information on this, and how to apply and follow
+the GNU GPL, see <<https://www.gnu.org/licenses/>>.
+
+The GNU General Public License does not permit incorporating your
+program into proprietary programs. If your program is a subroutine
+library, you may consider it more useful to permit linking proprietary
+applications with the library. If this is what you want to do, use the
+GNU Lesser General Public License instead of this License. But first,
+please read <<https://www.gnu.org/licenses/why-not-lgpl.html>>.
```

### Comparing `welkin-0.1.2/README.md` & `welkin-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # welkin-health
 
 ## A Python wrapper of the Welkin Health API
 
 [![Version](https://img.shields.io/pypi/v/welkin?style=for-the-badge&logo=pypi&logoColor=fff)](https://pypi.org/project/welkin/)
 [![Python](https://img.shields.io/pypi/pyversions/welkin?style=for-the-badge&logo=python&logoColor=fff)](https://pypi.org/project/welkin/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge&logo=gnu&logoColor=fff)](https://www.gnu.org/licenses/gpl-3.0)
-[![Tests](https://img.shields.io/github/actions/workflow/status/lightmatter/welkin-health/test.yaml?branch=develop&style=for-the-badge&logo=githubactions&logoColor=fff&label=Tests)](https://github.com/Lightmatter/welkin-health/actions)
+[![Tests](https://img.shields.io/github/actions/workflow/status/lightmatter/welkin-health/ci.yaml?branch=develop&style=for-the-badge&logo=githubactions&logoColor=fff&label=Tests)](https://github.com/Lightmatter/welkin-health/actions)
 
 [![codecov](https://img.shields.io/codecov/c/gh/Lightmatter/welkin-health?logo=codecov&logoColor=fff&style=for-the-badge)](https://codecov.io/gh/Lightmatter/welkin-health)
 
 This package allows Python developers to write software that makes use of the Welkin Health API. Functions available in the API are mirrored in this package as closely as possible, translating JSON responses to Python objects. You can find the current documentation for the Welkin Health API here:
 
 [Welkin Health API Documentation](https://developers.welkinhealth.com/)
```

### Comparing `welkin-0.1.2/welkin/__init__.py` & `welkin-0.1.3/welkin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Welkin Health API wrapper
+"""Welkin Health API wrapper.
 
 https://developers.welkinhealth.com/
 
 Introduction
 ========
 When reading this API, we take a liberty and assume that you are familiar with the
 following Welkin concepts, but for the sake of clarity will shortly repeat them here:
@@ -41,14 +41,17 @@
 
 Reminder: Security Policies and Roles are defined in the Designer and assigned in the
 Admin
 
 For this example we will assume Client Name is VBOPNRYRWJIP and Secret Key is
 +}B{KGTG6#zG%P;tQm0C
 """
+
+# ruff: noqa: F401
+
 from welkin.__version__ import (
     __author__,
     __author_email__,
     __copyright__,
     __description__,
     __license__,
     __title__,
```

### Comparing `welkin-0.1.2/welkin/authentication.py` & `welkin-0.1.3/welkin/authentication.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from __future__ import annotations
+
 import logging
 import shelve
 import tempfile
 from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 from portalocker import Lock
-from requests import PreparedRequest
 from requests.auth import AuthBase
 
+if TYPE_CHECKING:
+    from requests import PreparedRequest
+
+
 logger = logging.getLogger(__name__)
 
 
 DB_PATH = str(Path(tempfile.gettempdir(), ".welkin.db"))
 DB_LOCK = f"{DB_PATH}.lock"
 
 
@@ -46,26 +51,24 @@
         if "api_clients" not in r.path_url:
             r.headers["Authorization"] = f"Bearer {self.token}"
 
         return r
 
     @property
     def token(self) -> str:
-        with Lock(DB_LOCK):
-            with shelve.open(DB_PATH) as db:
-                try:
-                    return db[self.tenant]["token"]
-                except KeyError:
-                    pass
+        with Lock(DB_LOCK), shelve.open(DB_PATH) as db:  # noqa: S301
+            try:
+                return db[self.tenant]["token"]
+            except KeyError:
+                pass
 
         self.refresh_token()
 
         return self.token
 
     @token.setter
     def token(self, value: dict) -> None:
-        with Lock(DB_LOCK):
-            with shelve.open(DB_PATH) as db:
-                db[self.tenant] = value
+        with Lock(DB_LOCK), shelve.open(DB_PATH) as db:  # noqa: S301
+            db[self.tenant] = value
 
     def refresh_token(self) -> None:
         self.token = self.token_method()
```

### Comparing `welkin-0.1.2/welkin/client.py` & `welkin-0.1.3/welkin/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-"""Client
+"""Client.
 
 This module provides a Client object to interface with the Welkin Health API.
 """
+
+from __future__ import annotations
+
 import logging
 from http import HTTPStatus
 from json import JSONDecodeError
 
 from requests import HTTPError, Session
 from requests.adapters import HTTPAdapter
 from requests.compat import urljoin
@@ -58,15 +61,15 @@
 
         ### User methods
         user = client.User(username="bar", email="bar@foo.com").create()  # Create
 
         user = welkin.User(id="301b2895-cbf0-4cac-b4cf-1d082faee95c").get()  # Read
         users = welkin.Users().get()  # Read all/list
         uasers = welkin.Users().get(
-            search="lightmatter", region="east-coast", seat_assigned=True, user_state="ACTIVE"
+            search="foo", region="east-coast", seat_assigned=True, user_state="ACTIVE"
         )  # Filtered read all/list
 
         user.update(firstName="Baz")  # Update
         user.delete()  # Delete
     """
 
     Assessment = models.Assessment
@@ -102,15 +105,15 @@
     SearchChats = models.SearchChats
     SMS = models.SMS
     SMSes = models.SMSes
     User = models.User
     Users = models.Users
     WorkHours = models.WorkHours
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         tenant,
         instance,
         api_client,
         secret_key,
         timeout=5,
         total=5,
@@ -167,39 +170,45 @@
         if request.json:
             request.json = clean_request_payload(request.json)
         if request.params:
             request.params = clean_request_params(request.params)
 
         return super().prepare_request(request)
 
-    def request(
+    def request(  # noqa: C901, PLR0912
         self,
         method: str,
         path: str,
-        meta_key: str = None,
-        meta_dict: dict = {},
+        meta_key: str | None = None,
+        meta_dict: dict | None = None,
         *args,
         **kwargs,
     ):
         """Override :obj:`Session` request method to add retries and output JSON.
 
         Args:
             method (str): Method for the new Request object.
             path (str): Path from host for the new Request object.
+            meta_key (str | None, optional): Key for metadata in the response JSON.
+                Defaults to None.
+            meta_dict (dict | None, optional): Metadata dictionary for the response JSON.
+                Defaults to None.
+            *args: Arguments to pass to `Session.request`.
+            **kwargs: Keyword arguments to pass to `Session.request`.
 
         Returns:
             dict: Response JSON
         """
         if not isinstance(path, str):
-            path = "/".join((str(s) for s in path if s))
+            path = "/".join(str(s) for s in path if s)
         path = path.rstrip("/")
 
         for _ in range(2):
             response = super().request(
-                method=method, url=urljoin(self.host, path), *args, **kwargs
+                *args, method=method, url=urljoin(self.host, path), **kwargs
             )
 
             try:
                 response.raise_for_status()
                 break
             except HTTPError as exc:
                 code = exc.response.status_code
@@ -264,27 +273,29 @@
                 meta = json.pop(meta_key, {})
             meta.update(json)
             return resource, meta
 
         return resource or json
 
     def get_token(self) -> dict:
-        data = {"secret": self.auth.secret_key}
-        response = self.post(f"admin/api_clients/{self.auth.api_client}", json=data)
-
-        return response
+        return self.post(
+            f"admin/api_clients/{self.auth.api_client}",
+            json={"secret": self.auth.secret_key},
+        )
 
 
 class TimeoutHTTPAdapter(HTTPAdapter):
     def __init__(self, timeout, *args, **kwargs):
         """TimeoutHTTPAdapter constructor.
 
         Args:
             timeout (int): How many seconds to wait for the server to send data before
                 giving up.
+            *args: Arguments to pass to `HTTPAdapter`.
+            **kwargs: Keyword arguments to pass to `HTTPAdapter`.
         """
         self.timeout = timeout
         super().__init__(*args, **kwargs)
 
     def send(self, request, **kwargs):
         """Override :obj:`HTTPAdapter` send method to add a default timeout."""
         timeout = kwargs.get("timeout")
```

### Comparing `welkin-0.1.2/welkin/models/__init__.py` & `welkin-0.1.3/welkin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.2/welkin/models/assessment.py` & `welkin-0.1.3/welkin/models/assessment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageableIterator
 from welkin.util import model_id
 
 
 class Assessment(Resource):
     @model_id("Patient", "Encounter")
@@ -54,15 +56,15 @@
         return super().put(
             f"{self._client.instance}/patients/{patient_id}/"
             f"assessment-records/{assessment_record_id}/answers"
         )
 
 
 class AssessmentRecord(Resource):
-    subresources = [AssessmentRecordAnswers]
+    subresources = (AssessmentRecordAnswers,)
 
     @model_id("Patient")
     def create(self, patient_id: str):
         return super().post(
             f"{self._client.instance}/patients/{patient_id}/assessment-records"
         )
```

### Comparing `welkin-0.1.2/welkin/models/base.py` & `welkin-0.1.3/welkin/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import sys
+from types import MappingProxyType
 
 from welkin.pagination import PageIterator
 
 
 class SchemaBase:
     _client = None
     _parent = None
-    subresources = []
+    subresources = ()
 
     def __getattr__(self, name):
         try:
             for r in self.subresources:
                 if r.__name__ == name:
                     r._parent = self
                     return r
@@ -21,15 +24,15 @@
         try:
             return super().__getattribute__(name)
         except AttributeError as e:
             raise AttributeError(e) from None
 
 
 class Resource(dict, SchemaBase):
-    nested_objects = {}
+    nested_objects = MappingProxyType({})
 
     def __getattr__(self, name):
         try:
             value = super().__getitem__(name)
         except KeyError:
             value = super().__getattr__(name)
 
@@ -45,15 +48,15 @@
     def __setattr__(self, name, value):
         super().__setitem__(name, value)
 
     def __delattr__(self, name):
         super().__delitem__(name)
 
     def __str__(self):
-        id = getattr(self, "id", "")
+        id = getattr(self, "id", "")  # noqa: A001
 
         return f"{self.__class__.__name__} #{id}" if id else self.__class__.__name__
 
     def __repr__(self):
         return object.__repr__(self)
 
     def get(self, resource, subresource=None, *args, **kwargs):
@@ -61,39 +64,39 @@
         super().update(response)
 
         return self
 
     def patch(self, resource, data, *args, **kwargs):
         response = self._client.patch(
             resource,
-            json=data,
             *args,
+            json=data,
             **kwargs,
         )
 
         super().update(response)
 
         return self
 
     def post(self, resource, *args, **kwargs):
         response = self._client.post(
             resource,
-            json=self,
             *args,
+            json=self,
             **kwargs,
         )
         super().update(response)
 
         return self
 
     def put(self, resource, *args, **kwargs):
         response = self._client.put(
             resource,
-            json=self,
             *args,
+            json=self,
             **kwargs,
         )
 
         super().update(response)
 
         return self
```

### Comparing `welkin-0.1.2/welkin/models/calendar.py` & `welkin-0.1.3/welkin/models/calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-from datetime import datetime, timezone
+from __future__ import annotations
+
 from enum import Enum
+from typing import TYPE_CHECKING
 
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageableIterator
 
+if TYPE_CHECKING:
+    from datetime import datetime
+
 
 class EventType(Enum):
     GROUP_THERAPY = "GROUP_THERAPY"
     APPOINTMENT = "APPOINTMENT"
     LEAVE = "LEAVE"
     ENCOUNTER = "ENCOUNTER"
 
@@ -30,37 +35,35 @@
         # TODO: Accept User and Patient instances as participants
         return super().post(f"{self._client.instance}/calendar/events")
 
     def get(self):
         return super().get(f"{self._client.instance}/calendar/events/{self.id}")
 
     def update(self, **kwargs):
-        return super().patch(
-            f"{self._client.instance}/calendar/events/{self.id}", kwargs
-        )
+        return super().patch(f"{self._client.instance}/calendar/events/{self.id}", kwargs)
 
     def delete(self):
         return super().delete(f"{self._client.instance}/calendar/events/{self.id}")
 
 
 class CalendarEvents(Collection):
     resource = CalendarEvent
     iterator = PageableIterator
 
-    def get(
+    def get(  # noqa: PLR0913
         self,
         from_date: datetime,
         to_date: datetime,
-        participant_ids: list = None,
-        event_type: str = None,
-        sort: str = None,
-        include_cancelled: bool = None,
-        include_encounter_info: bool = None,
-        exclude_assigned_to_encounter_events: bool = None,
-        viewer_timezone: str = None,
+        participant_ids: list | None = None,
+        event_type: str | None = None,
+        sort: str | None = None,
+        include_cancelled: bool | None = None,
+        include_encounter_info: bool | None = None,
+        exclude_assigned_to_encounter_events: bool | None = None,
+        viewer_timezone: str | None = None,
         *args,
         **kwargs,
     ):
         # Validation
         if event_type:
             EventType(event_type)
 
@@ -74,32 +77,32 @@
             "includeCancelled": include_cancelled,
             "includeEncounterInfo": include_encounter_info,
             "excludeAssignedToEncounterEvents": exclude_assigned_to_encounter_events,
             "viewerTimezone": viewer_timezone,
         }
 
         return super().get(
-            f"{self._client.instance}/calendar/events", params=params, *args, **kwargs
+            f"{self._client.instance}/calendar/events", *args, params=params, **kwargs
         )
 
 
 class Schedule(Resource):
     pass
 
 
 class Schedules(Collection):
     resource = Schedule
     iterator = PageableIterator
 
-    def get(
+    def get(  # noqa: PLR0913
         self,
         ids: list,
         from_date: datetime,
         to_date: datetime,
-        include_cancelled: bool = None,
+        include_cancelled: bool | None = None,
         available: bool = False,
         full: bool = False,
         *args,
         **kwargs,
     ):
         route = "psm-schedules"
         if available:
@@ -111,27 +114,27 @@
             "psmIds": ids,
             "from": from_date,
             "to": to_date,
             "includeCancelled": include_cancelled,
         }
 
         return super().get(
-            f"{self._client.instance}/calendar/{route}", params=params, *args, **kwargs
+            f"{self._client.instance}/calendar/{route}", *args, params=params, **kwargs
         )
 
 
 class WorkHours(Collection):
     iterator = PageableIterator
 
     def get(
         self,
         from_date: datetime,
         to_date: datetime,
-        psm_ids: list = None,
-        timezone: str = None,
+        psm_ids: list | None = None,
+        timezone: str | None = None,
         *args,
         **kwargs,
     ):
         params = {
             "from": from_date,
             "to": to_date,
             "psm-ids": psm_ids,
@@ -142,11 +145,11 @@
             f"{self._client.instance}/calendar/work-hours/",
             *args,
             params=params,
             **kwargs,
         )
 
         # When no work hours are found Welkin returns an {None: []} dictionary
-        if isinstance(response, dict) and None in response.keys():
+        if isinstance(response, dict) and None in response:
             return WorkHours([])
 
         return response
```

### Comparing `welkin-0.1.2/welkin/models/care_plan.py` & `welkin-0.1.3/welkin/models/care_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 from welkin.models.base import Resource
 from welkin.util import model_id
 
 
 class CarePlanOverview(Resource):
     @model_id("Patient")
     def update(self, patient_id: str):
         return super().put(
             f"{self._client.instance}/patients/{patient_id}/care-plan/overview"
         )
 
 
 class CarePlan(Resource):
-    subresources = [CarePlanOverview]
+    subresources = (CarePlanOverview,)
 
     @model_id("Patient")
     def create(self, patient_id: str):
         return super().post(
             f"{self._client.instance}/patients/{patient_id}/care-plan/overview"
         )
```

### Comparing `welkin-0.1.2/welkin/models/cdt.py` & `welkin-0.1.3/welkin/models/cdt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-from datetime import datetime
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageNumberIterator
 from welkin.util import model_id
 
+if TYPE_CHECKING:
+    from datetime import datetime
+
 
 class CDT(Resource):
     @model_id("Patient")
     def create(self, patient_id: str):
         return super().post(
             f"{self._client.instance}/patients/{patient_id}/cdts/{self.cdtName}"
         )
@@ -33,41 +38,41 @@
 
 
 class CDTs(Collection):
     resource = CDT
     iterator = PageNumberIterator
 
     @model_id("Patient")
-    def get(
+    def get(  # noqa: PLR0913
         self,
         patient_id: str,
         cdt_name: str,
-        fields: list = None,
-        filters: dict = None,
-        date_start: datetime = None,
-        date_end: datetime = None,
-        sort: str = None,
+        fields: list | None = None,
+        filters: dict | None = None,
+        date_start: datetime | None = None,
+        date_end: datetime | None = None,
+        sort: str | None = None,
         *args,
         **kwargs,
     ):
         params = {
             "fields": fields,
             "filters": filters,
             "sort": sort,
             "dateStart": date_start,
             "dateEnd": date_end,
         }
 
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/cdts/{cdt_name}",
-            params=params,
             *args,
+            params=params,
             **kwargs,
         )
 
     @model_id("Patient")
-    def update(self, patient_id: str, cdt_name: str, body: dict = None, **kwargs):
+    def update(self, patient_id: str, cdt_name: str, body: dict | None = None, **kwargs):
         return super().patch(
             f"{self._client.instance}/patients/{patient_id}/cdts/{cdt_name}",
             json=body,
             **kwargs,
         )
```

### Comparing `welkin-0.1.2/welkin/models/chat.py` & `welkin-0.1.3/welkin/models/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from __future__ import annotations
+
 from welkin.models.base import Collection, Resource
 from welkin.pagination import MetaIterator
 from welkin.util import model_id
 
 
 class Chat(Resource):
     @model_id("Patient")
     def create(self, patient_id: str):
-        return super().post(
-            f"{self._client.instance}/patients/{patient_id}/chat/inbound"
-        )
+        return super().post(f"{self._client.instance}/patients/{patient_id}/chat/inbound")
 
     def __str__(self):
         return f"{self.sender['clientType']} {self.message}"
 
 
 class Chats(Collection):
     resource = Chat
@@ -22,16 +22,16 @@
     def get(self, patient_id: str, include_archived: bool = False, *args, **kwargs):
         params = {
             "includeArchived": include_archived,
         }
 
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/chat",
-            params=params,
             *args,
+            params=params,
             **kwargs,
         )
 
 
 class ChatSearchResult(Resource):
     pass
 
@@ -54,11 +54,11 @@
             "query": query,
             "contentPageSize": content_page_size,
             "includeArchived": include_archived,
         }
 
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/chat/search",
-            params=params,
             *args,
+            params=params,
             **kwargs,
         )
```

### Comparing `welkin-0.1.2/welkin/models/document.py` & `welkin-0.1.3/welkin/models/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from io import BytesIO
 
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageableIterator
 from welkin.util import model_id
 
 
@@ -21,29 +23,29 @@
     iterator = PageableIterator
 
     @model_id("Patient", "DocumentSummary")
     def create(
         self,
         patient_id: str,
         document_summary_id: str,
-        files: list = None,
+        files: list | None = None,
         *args,
         **kwargs,
     ):
         return super().post(
             f"{self._client.instance}/patients/{patient_id}/document-summary/"
             f"{document_summary_id}/files",
-            files=files,
             *args,
+            files=files,
             **kwargs,
         )
 
 
 class DocumentSummary(Resource):
-    subresources = [DocumentSummaryFile, DocumentSummaryFiles]
+    subresources = (DocumentSummaryFile, DocumentSummaryFiles)
 
     @model_id("Patient")
     def get(self, patient_id: str):
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/document-summary/{self.id}"
         )
```

### Comparing `welkin-0.1.2/welkin/models/email.py` & `welkin-0.1.3/welkin/models/email.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageableIterator
 from welkin.util import model_id
 
 
 class Email(Resource):
     @model_id("Patient")
@@ -14,18 +16,18 @@
 
 
 class Emails(Collection):
     resource = Email
     iterator = PageableIterator
 
     @model_id("Patient")
-    def get(self, patient_id: str, sort: str = None, *args, **kwargs):
+    def get(self, patient_id: str, sort: str | None = None, *args, **kwargs):
         params = {
             "sort": sort,
         }
 
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/emails",
-            params=params,
             *args,
+            params=params,
             **kwargs,
         )
```

### Comparing `welkin-0.1.2/welkin/models/encounter.py` & `welkin-0.1.3/welkin/models/encounter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from __future__ import annotations
+
 from enum import Enum
+from types import MappingProxyType
 
 from welkin.models.assessment import Assessment, Assessments
 from welkin.models.base import Collection, Resource
 from welkin.pagination import MetaInfoIterator
 from welkin.util import model_id
 
 
@@ -25,20 +28,22 @@
     OPEN = "OPEN"
     CANCELLED = "CANCELLED"
     DRAFT = "DRAFT"
     FINALIZED = "FINALIZED"
 
 
 class Encounter(Resource):
-    subresources = [Assessment, Assessments, EncounterDisposition]
-    nested_objects = {
-        "assessmentLinks": "Assessments",
-        "userRelatedToCalendarEvent": "User",
-        "disposition": "EncounterDisposition",
-    }
+    subresources = (Assessment, Assessments, EncounterDisposition)
+    nested_objects = MappingProxyType(
+        {
+            "assessmentLinks": "Assessments",
+            "userRelatedToCalendarEvent": "User",
+            "disposition": "EncounterDisposition",
+        }
+    )
 
     @model_id("Patient")
     def create(self, patient_id: str):
         return super().post(f"{self._client.instance}/patients/{patient_id}/encounters")
 
     @model_id("Patient")
     def get(self, patient_id: str, related_data: bool = False):
@@ -64,23 +69,23 @@
         )
 
 
 class Encounters(Collection):
     resource = Encounter
     iterator = MetaInfoIterator
 
-    def get(
+    def get(  # noqa: PLR0913
         self,
-        patient_id: str = None,
-        user_id: str = None,
-        related_data: bool = None,
-        with_care_team: bool = None,
-        only_with_calendar_event: bool = None,
-        statuses: list = None,
-        sort: str = None,
+        patient_id: str | None = None,
+        user_id: str | None = None,
+        related_data: bool | None = None,
+        with_care_team: bool | None = None,
+        only_with_calendar_event: bool | None = None,
+        statuses: list | None = None,
+        sort: str | None = None,
         *args,
         **kwargs,
     ):
         path = f"{self._client.instance}/"
         if patient_id:
             path += f"patients/{patient_id}/"
         elif user_id:
@@ -95,8 +100,8 @@
         params = {
             "withCareTeam": with_care_team,
             "statuses": statuses,
             "sort": sort,
             "onlyWithCalendarEvent": only_with_calendar_event,
         }
 
-        return super().get(path, params=params, *args, **kwargs)
+        return super().get(path, *args, params=params, **kwargs)
```

### Comparing `welkin-0.1.2/welkin/models/formation.py` & `welkin-0.1.3/welkin/models/formation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import Union
+from __future__ import annotations
 
 from welkin.models.base import Collection, Resource
 from welkin.pagination import FormationIterator
 from welkin.util import Target, _build_resources
 
 
 class FormationBase:
     endpoint: str = None
 
     def __new__(cls, *args, **kwargs):
         if not cls.endpoint:
-            raise AttributeError(
-                f"The `endpoint` attribute must be set on {cls.__name__}"
-            )
+            raise AttributeError(f"The `endpoint` attribute must be set on {cls.__name__}")
 
         return super().__new__(cls)
 
 
 class FormationResource(FormationBase, Resource):
     def get(self, *args, **kwargs):
         return super().get(
@@ -112,13 +110,13 @@
     EncounterDisposition = EncounterDisposition
     Encounters = Encounters
     Goal = Goal
     Goals = Goals
     Program = Program
     Programs = Programs
 
-    def __init__(self, version: Union[int, str] = "current"):
+    def __init__(self, version: int | str = "current"):
         super().__init__()
 
         self._base_path = f"{self._client.instance}/formations/{version}"
 
         _build_resources(self, "_formation")
```

### Comparing `welkin-0.1.2/welkin/models/patient.py` & `welkin-0.1.3/welkin/models/patient.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from welkin.models.assessment import AssessmentRecord, AssessmentRecords
 from welkin.models.base import Collection, Resource
 from welkin.models.care_plan import CarePlan
 from welkin.models.cdt import CDT, CDTs
 from welkin.models.chat import Chat, Chats, SearchChats
 from welkin.models.document import (
     DocumentSummaries,
@@ -12,15 +14,15 @@
 from welkin.models.encounter import Encounter, Encounters
 from welkin.models.program import PatientProgram, PatientPrograms
 from welkin.models.sms import SMS, SMSes
 from welkin.pagination import PageableIterator
 
 
 class Patient(Resource):
-    subresources = [
+    subresources = (
         AssessmentRecord,
         AssessmentRecords,
         CarePlan,
         CDT,
         CDTs,
         Chat,
         Chats,
@@ -32,38 +34,38 @@
         Encounter,
         Encounters,
         PatientProgram,
         PatientPrograms,
         SearchChats,
         SMS,
         SMSes,
-    ]
+    )
 
     def create(self):
         return super().post(f"{self._client.instance}/patients")
 
-    def get(self, expand: bool = None):
+    def get(self, expand: bool | None = None):
         _id = None
         if hasattr(self, "id"):
-            type = None
+            _type = None
             _id = self.id
         elif hasattr(self, "externalId"):
-            type = "EID"
+            _type = "EID"
             _id = self.externalId
         elif hasattr(self, "externalGuid"):
-            type = "EGUID"
+            _type = "EGUID"
             _id = self.externalGuid
         elif hasattr(self, "mrn"):
-            type = "MRN"
+            _type = "MRN"
             _id = self.mrn
 
         return super().get(
             f"{self._client.instance}/patients/{_id}",
             params={
-                "type": type,
+                "type": _type,
                 expand: expand,
             },
         )
 
     def update(self, **kwargs):
         return super().patch(f"{self._client.instance}/patients/{self.id}", kwargs)
 
@@ -74,12 +76,12 @@
         return f"{self.firstName} {self.lastName}"
 
 
 class Patients(Collection):
     resource = Patient
     iterator = PageableIterator
 
-    def get(self, filter={}, *args, **kwargs):
+    def get(self, filter: dict | None = None, *args, **kwargs):  # noqa: A002
         # TODO: Add sort and query arguments.
         return super().post(
-            f"{self._client.instance}/by-filter/patients", json=filter, *args, **kwargs
+            f"{self._client.instance}/by-filter/patients", *args, json=filter, **kwargs
         )
```

### Comparing `welkin-0.1.2/welkin/models/program.py` & `welkin-0.1.3/welkin/models/program.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,58 @@
+from __future__ import annotations
+
+from types import MappingProxyType
+
 from welkin.models.base import Collection, Resource
 from welkin.pagination import MetaInfoIterator
 from welkin.util import model_id
 
 
 class ProgramPhase(Resource):
     pass
 
 
 class ProgramPhases(Collection):
     resource = ProgramPhase
 
 
 class PatientProgram(Resource):
-    subresources = [ProgramPhase]
-    nested_objects = {
-        "phases": "ProgramPhase",
-        "currentPhase": "ProgramPhase",
-        "pathHistory": "ProgramPhases",
-    }
+    subresources = (ProgramPhase,)
+    nested_objects = MappingProxyType(
+        {
+            "phases": "ProgramPhase",
+            "currentPhase": "ProgramPhase",
+            "pathHistory": "ProgramPhases",
+        }
+    )
 
     @model_id("Patient")
     def get(
         self,
         patient_id: str,
-        assigned_programs: bool = None,
-        sort: str = None,
+        assigned_programs: bool | None = None,
+        sort: str | None = None,
         *args,
         **kwargs,
     ):
         path = f"{self._client.instance}/patients/{patient_id}/programs"
         if hasattr(self, "id"):
             path += f"/history/{self.id}"
         elif hasattr(self, "programName"):
             path += f"/current/{self.programName}"
         else:
             raise ValueError("Program must have either programName or id attributes")
 
         return super().get(
             path,
+            *args,
             params={
                 "assignedPrograms": assigned_programs,
                 "sort": sort,
             },
-            *args,
             **kwargs,
         )
 
     @model_id("Patient")
     def update(self, patient_id: str, **kwargs):
         return super().patch(
             f"{self._client.instance}/patients/{patient_id}/programs/"
@@ -65,21 +71,21 @@
     resource = PatientProgram
     iterator = MetaInfoIterator
 
     @model_id("Patient")
     def get(
         self,
         patient_id: str,
-        assigned_programs: bool = None,
-        sort: str = None,
+        assigned_programs: bool | None = None,
+        sort: str | None = None,
         *args,
         **kwargs,
     ):
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/programs",
+            *args,
             params={
                 "assignedPrograms": assigned_programs,
                 "sort": sort,
             },
-            *args,
             **kwargs,
         )
```

### Comparing `welkin-0.1.2/welkin/models/sms.py` & `welkin-0.1.3/welkin/models/sms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from welkin.models.base import Collection, Resource
 from welkin.pagination import PageableIterator
 from welkin.util import model_id
 
 
 class SMS(Resource):
     @model_id("Patient")
@@ -14,18 +16,18 @@
 
 
 class SMSes(Collection):
     resource = SMS
     iterator = PageableIterator
 
     @model_id("Patient")
-    def get(self, patient_id: str, sort: str = None, *args, **kwargs):
+    def get(self, patient_id: str, sort: str | None = None, *args, **kwargs):
         params = {
             "sort": sort,
         }
 
         return super().get(
             f"{self._client.instance}/patients/{patient_id}/sms",
-            params=params,
             *args,
+            params=params,
             **kwargs,
         )
```

### Comparing `welkin-0.1.2/welkin/pagination.py` & `welkin-0.1.3/welkin/pagination.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+from __future__ import annotations
+
+DEFAULT_PAGE_SIZE = 20
+
+
 class PageIterator:
-    def __init__(self, collection, resource, method, size=20, *args, **kwargs):
+    def __init__(
+        self, collection, resource, method, size=DEFAULT_PAGE_SIZE, *args, **kwargs
+    ):
         self.collection = collection
         self.resource = resource
         self.method = method
         self.size = size
         self.meta_key = None
         self.meta_dict = {"totalPages": 1, "number": 0, "last": True}
 
-        if size != 20:
+        if size != DEFAULT_PAGE_SIZE:
             kwargs.setdefault("params", {}).update(size=size)
 
         self.args = args
         self.kwargs = kwargs
 
     def __iter__(self):
         self._resources = []
@@ -24,52 +31,46 @@
             return self.resources.pop(0)
 
         if not self.last:
             self._pre_request()
 
             self.resources, meta = self.method(
                 self.resource,
+                *self.args,
                 meta_key=self.meta_key,
                 meta_dict=self.meta_dict,
-                *self.args,
                 **self.kwargs,
             )
 
             self._post_request(meta)
 
             return next(self)
 
         raise StopIteration
 
     def _pre_request(self):
-        """
-        Function to execute before making the next request, e.g. update paging params
-        """
+        """Function to execute before making the next request, e.g. update paging params."""
         self.kwargs.setdefault("params", {})
 
     def _post_request(self, meta):
-        """
-        Function to execute after making the next request, e.g. updating page tracking
-        """
+        """Function to execute after making the next request, e.g. update page tracking."""
         self.last = True
 
     @property
     def resources(self):
         return self._resources
 
     @resources.setter
     def resources(self, value):
         self._resources = [self.collection.resource(v) for v in value]
         self.collection.extend(self.resources)
 
 
 class PageableIterator(PageIterator):
-    """
-    Most common paging class
-    """
+    """Most common paging class."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_key = "pageable"
 
     def __iter__(self):
         self.page = 0
@@ -80,18 +81,18 @@
 
     def _post_request(self, meta):
         self.page = meta["number"] + 1
         self.last = meta.get("last")
 
 
 class FormationIterator(PageIterator):
-    """
-    Specifically for paginating formations responses
-    Similar to PageableIterator but includes special behavior for
-    single item formations, e.g. encounter disposition
+    """Specifically for paginating formations responses.
+
+    Similar to PageableIterator but includes special behavior for single item formations,
+    e.g. encounter disposition
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_key = "pageable"
 
     def __iter__(self):
@@ -103,17 +104,17 @@
             return self.resources.pop(0)
 
         if not self.last:
             self._pre_request()
 
             data = self.method(
                 self.resource,
+                *self.args,
                 meta_key=self.meta_key,
                 meta_dict=self.meta_dict,
-                *self.args,
                 **self.kwargs,
             )
             if isinstance(data, dict):
                 data = [data]
 
             self.resources = data
 
@@ -128,32 +129,28 @@
 
     def _post_request(self, meta):
         self.page = meta.get("number", 0) + 1
         self.last = meta.get("last", True)
 
 
 class PageNumberIterator(PageableIterator):
-    """
-    PageableIterator with a different key used for the page count
-    """
+    """PageableIterator with a different key used for the page count."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_dict.pop("number")
         self.meta_dict["pageNumber"] = 0
 
     def _post_request(self, meta):
         self.page = meta["pageNumber"] + 1
         self.last = meta.get("last")
 
 
 class MetaInfoIterator(PageIterator):
-    """
-    Functionally identical to PageableIterator with various renamed keys
-    """
+    """Functionally identical to PageableIterator with various renamed keys."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_key = "metaInfo"
         self.meta_dict.pop("number")
         self.meta_dict["page"] = 0
 
@@ -166,17 +163,15 @@
 
     def _post_request(self, meta):
         self.page = meta["page"] + 1
         self.last = meta.get("lastPage")
 
 
 class MetaIterator(PageIterator):
-    """
-    Paging class for token based paging
-    """
+    """Paging class for token based paging."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta_key = "meta"
         self.meta_dict = {
             "nextPageToken": None,
             "prevPageToken": None,
```

### Comparing `welkin-0.1.2/welkin/util.py` & `welkin-0.1.3/welkin/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from datetime import date, datetime, timezone
 from functools import lru_cache, wraps
-from typing import Any, Callable, Tuple, Union
+from typing import Any, Callable
 from uuid import UUID
 
 import inflection
 
 from welkin.models.base import Collection, Resource, SchemaBase
 
 # NOTE: `clean_request_payload` and `clean_request_params` are intentionally DRY
@@ -16,15 +18,17 @@
     _client = None
 
     def __init__(self):
         self._base_path = ""
         _build_resources(self, "_client", self._client)
 
 
-def _build_resources(instance: type, attribute_name: str, value: type = None) -> None:
+def _build_resources(
+    instance: type, attribute_name: str, value: type | None = None
+) -> None:
     """Add an attribute pointing to an instance for each resource.
 
     Args:
         instance (type): _description_
         attribute_name (str): _description_
         value (type, optional): _description_. Defaults to None.
     """
@@ -50,21 +54,21 @@
         value (Any): The value to clean.
 
     Returns:
         Any: The cleaned value.
     """
     if isinstance(value, datetime):
         return clean_datetime(value)
-    elif isinstance(value, date):
+    if isinstance(value, date):
         return clean_date(value)
-    elif isinstance(value, dict):
+    if isinstance(value, dict):
         return clean_request_payload(value)
-    elif isinstance(value, list):
+    if isinstance(value, list):
         return clean_json_list(value)
-    elif isinstance(value, UUID):
+    if isinstance(value, UUID):
         return str(value)
 
     # No cleaning needed
     return value
 
 
 def clean_request_payload(payload: dict) -> dict:
@@ -108,15 +112,15 @@
     return (
         dt.astimezone(tz=timezone.utc)
         .isoformat(timespec="milliseconds")
         .replace("+00:00", "Z")
     )
 
 
-def find_model_id(instance: Union[Collection, Resource], model_name: str) -> str:
+def find_model_id(instance: Collection | Resource, model_name: str) -> str:
     """Recursively traverse the `_parent` chain searching for a model id.
 
     Args:
         instance (Union[Collection, Resource]): The instanceect instance to inspect.
         model_name (str): The class name of the model to find.
 
     Raises:
@@ -125,29 +129,29 @@
     Returns:
         str: The model id.
     """
     body_id_key = f"{to_camel_case(model_name)}Id"
 
     if instance.__class__.__name__ == model_name:
         return instance.id
-    elif hasattr(instance, body_id_key):
+    if hasattr(instance, body_id_key):
         return getattr(instance, body_id_key)
-    elif instance._parent is not None:
+    if instance._parent is not None:
         return find_model_id(instance._parent, model_name)
 
     raise AttributeError(
         f"Cannot find {model_name} id. Model._parent chain ends in {instance}"
     )
 
 
-def model_id(*models: Tuple[str]) -> Callable:
+def model_id(*models: tuple[str]) -> Callable:
     """Insert values for `model_id` arguments if not provided.
 
     Args:
-        *models (Tuple[str]): The model names to search for.
+        *models (tuple[str]): The model names to search for.
 
     Raises:
         TypeError: If no ID is found and no arguments are provided.
     """
 
     def decorator(f: Callable):
         @wraps(f)
```

### Comparing `welkin-0.1.2/PKG-INFO` & `welkin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: welkin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Welkin Health API Wrapper.
 Home-page: https://github.com/lightmatter/welkin-health
 License: GPL-3.0-or-later
 Author: Sam Morgan
 Author-email: sama4mail@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 # welkin-health
 
 ## A Python wrapper of the Welkin Health API
 
 [![Version](https://img.shields.io/pypi/v/welkin?style=for-the-badge&logo=pypi&logoColor=fff)](https://pypi.org/project/welkin/)
 [![Python](https://img.shields.io/pypi/pyversions/welkin?style=for-the-badge&logo=python&logoColor=fff)](https://pypi.org/project/welkin/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge&logo=gnu&logoColor=fff)](https://www.gnu.org/licenses/gpl-3.0)
-[![Tests](https://img.shields.io/github/actions/workflow/status/lightmatter/welkin-health/test.yaml?branch=develop&style=for-the-badge&logo=githubactions&logoColor=fff&label=Tests)](https://github.com/Lightmatter/welkin-health/actions)
+[![Tests](https://img.shields.io/github/actions/workflow/status/lightmatter/welkin-health/ci.yaml?branch=develop&style=for-the-badge&logo=githubactions&logoColor=fff&label=Tests)](https://github.com/Lightmatter/welkin-health/actions)
 
 [![codecov](https://img.shields.io/codecov/c/gh/Lightmatter/welkin-health?logo=codecov&logoColor=fff&style=for-the-badge)](https://codecov.io/gh/Lightmatter/welkin-health)
 
 This package allows Python developers to write software that makes use of the Welkin Health API. Functions available in the API are mirrored in this package as closely as possible, translating JSON responses to Python objects. You can find the current documentation for the Welkin Health API here:
 
 [Welkin Health API Documentation](https://developers.welkinhealth.com/)
```

