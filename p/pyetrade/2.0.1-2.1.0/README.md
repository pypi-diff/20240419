# Comparing `tmp/pyetrade-2.0.1.tar.gz` & `tmp/pyetrade-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetrade-2.0.1.tar", last modified: Mon Mar 25 12:33:45 2024, max compression
+gzip compressed data, was "pyetrade-2.1.0.tar", last modified: Fri Apr 19 20:50:34 2024, max compression
```

## Comparing `pyetrade-2.0.1.tar` & `pyetrade-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:33:44.994801 pyetrade-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34801 2024-03-25 12:33:34.000000 pyetrade-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 12:33:34.000000 pyetrade-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-25 12:33:44.994801 pyetrade-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-25 12:33:34.000000 pyetrade-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:33:44.994801 pyetrade-2.0.1/pyetrade/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/market.py
--rw-r--r--   0 runner    (1001) docker     (127)    23604 2024-03-25 12:33:34.000000 pyetrade-2.0.1/pyetrade/order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:33:44.994801 pyetrade-2.0.1/pyetrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-25 12:33:44.000000 pyetrade-2.0.1/pyetrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-25 12:33:44.000000 pyetrade-2.0.1/pyetrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:33:44.000000 pyetrade-2.0.1/pyetrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 12:33:44.000000 pyetrade-2.0.1/pyetrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 12:33:44.000000 pyetrade-2.0.1/pyetrade.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-25 12:33:34.000000 pyetrade-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:33:44.994801 pyetrade-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-25 12:33:34.000000 pyetrade-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:33:44.994801 pyetrade-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-03-25 12:33:34.000000 pyetrade-2.0.1/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-25 12:33:34.000000 pyetrade-2.0.1/tests/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-25 12:33:34.000000 pyetrade-2.0.1/tests/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-03-25 12:33:34.000000 pyetrade-2.0.1/tests/test_market.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-03-25 12:33:34.000000 pyetrade-2.0.1/tests/test_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:50:34.539501 pyetrade-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34780 2024-04-19 20:50:24.000000 pyetrade-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 20:50:24.000000 pyetrade-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-19 20:50:34.539501 pyetrade-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-19 20:50:24.000000 pyetrade-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:50:34.535501 pyetrade-2.1.0/pyetrade/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyetrade/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:50:34.539501 pyetrade-2.1.0/pyetrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-19 20:50:34.000000 pyetrade-2.1.0/pyetrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 20:50:34.000000 pyetrade-2.1.0/pyetrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:50:34.000000 pyetrade-2.1.0/pyetrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 20:50:34.000000 pyetrade-2.1.0/pyetrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 20:50:34.000000 pyetrade-2.1.0/pyetrade.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 20:50:24.000000 pyetrade-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-19 20:50:24.000000 pyetrade-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:50:34.539501 pyetrade-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-19 20:50:24.000000 pyetrade-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:50:34.539501 pyetrade-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-19 20:50:24.000000 pyetrade-2.1.0/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-19 20:50:24.000000 pyetrade-2.1.0/tests/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-19 20:50:24.000000 pyetrade-2.1.0/tests/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-19 20:50:24.000000 pyetrade-2.1.0/tests/test_market.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-04-19 20:50:24.000000 pyetrade-2.1.0/tests/test_order.py
```

### Comparing `pyetrade-2.0.1/LICENSE` & `pyetrade-2.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-GNU GENERAL PUBLIC LICENSE 
+GNU GENERAL PUBLIC LICENSE
 Version 3, 29 June 2007
 Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
 Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
 
 Preamble
 
@@ -42,58 +42,58 @@
 
 To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
 
 To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
 
 An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
 
-1. Source Code. 
+1. Source Code.
 The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
 
 A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
 
 The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
 
 The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
 
 The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
 
 The Corresponding Source for a work in source code form is that same work.
 
-2. Basic Permissions. 
+2. Basic Permissions.
 All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
 
 You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
 
 Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
 
-3. Protecting Users' Legal Rights From Anti-Circumvention Law. 
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
 No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
 
 When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
 
-4. Conveying Verbatim Copies. 
+4. Conveying Verbatim Copies.
 You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
 
 You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
 
-5. Conveying Modified Source Versions. 
+5. Conveying Modified Source Versions.
 You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
 
 a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
 
 b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
 
 c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
 
 d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
 
 A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
 
-6. Conveying Non-Source Forms. 
+6. Conveying Non-Source Forms.
 You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
 
 a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
 
 b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
 
 c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
@@ -110,15 +110,15 @@
 
 If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
 
 The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
 
 Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
 
-7. Additional Terms. 
+7. Additional Terms.
 “Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
 
 When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
 
 Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
 
 a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
@@ -135,34 +135,34 @@
 
 All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
 
 If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
 
 Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
 
-8. Termination. 
+8. Termination.
 You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
 
 However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
 
 Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
 
 Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
 
-9. Acceptance Not Required for Having Copies. 
+9. Acceptance Not Required for Having Copies.
 You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
 
-10. Automatic Licensing of Downstream Recipients. 
+10. Automatic Licensing of Downstream Recipients.
 Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
 
 An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
 
 You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
 
-11. Patents. 
+11. Patents.
 A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
 
 A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
 
 Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
 
 In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
@@ -171,61 +171,61 @@
 
 If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
 
 A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
 
 Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
 
-12. No Surrender of Others' Freedom. 
+12. No Surrender of Others' Freedom.
 If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
 
-13. Use with the GNU Affero General Public License. 
+13. Use with the GNU Affero General Public License.
 Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
 
-14. Revised Versions of this License. 
+14. Revised Versions of this License.
 The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
 
 Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
 
 If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
 
 Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
 
-15. Disclaimer of Warranty. 
+15. Disclaimer of Warranty.
 THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
 
-16. Limitation of Liability. 
+16. Limitation of Liability.
 IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
 
-17. Interpretation of Sections 15 and 16. 
+17. Interpretation of Sections 15 and 16.
 If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
 
 END OF TERMS AND CONDITIONS
 
 How to Apply These Terms to Your New Programs
 
 If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
 
 To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
 
-<one line to give the program's name and a brief idea of what it does.> 
+<one line to give the program's name and a brief idea of what it does.>
 Copyright (C) <year> <name of author>
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
 If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
 
-<program> Copyright (C) <year> <name of author> 
-This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'. 
+<program> Copyright (C) <year> <name of author>
+This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
 This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
 
 You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
 
 The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `pyetrade-2.0.1/README.md` & `pyetrade-2.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,87 @@
-# pyetrade
+# pyetrade (Python E-Trade API Wrapper)
 
-Python E-Trade API Wrapper
 [![PyPI](https://img.shields.io/pypi/v/pyetrade.svg)](https://pypi.python.org/pypi/pyetrade)
 [![PyPI](https://img.shields.io/pypi/l/pyetrade.svg)]()
 [![PyPI](https://img.shields.io/pypi/pyversions/pyetrade.svg)](https://pypi.python.org/pypi/pyetrade)
 [![Build Status](https://github.com/jessecooper/pyetrade/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/jessecooper/pyetrade/actions/workflows/build.yml/badge.svg?branch=master)
 [![codecov](https://codecov.io/gh/jessecooper/pyetrade/branch/master/graph/badge.svg)](https://codecov.io/gh/jessecooper/pyetrade)
 
 ## Completed
-v1 API
-Authorization API - ALL
-Accounts
-* list accounts
-
-Authorization API - ALL
-Order API -
-* List Orders
-* Place Equity Order
-* Cancel Order
-
-Market API -
-* Look Up Product
-* optionchain
-* Get Quote
+
+* Authorization API (OAuth)
+  * get_request_token
+  * get_access_token
+  * renew_access_token
+  * revoke_access_token
+
+
+* Alerts API
+  * list_alerts
+  * list_alert_details
+  * delete_alert
+
+
+* Accounts API
+  * list_accounts
+  * get_account_balance
+  * get_account_portfolio
+  * get_portfolio_position_lot
+  * list_transactions
+  * list_transaction_details
+
+
+* Order API
+  * list_orders
+  * list_order_details
+  * find_option_orders
+  * preview_equity_order
+  * change_preview_equity_order
+  * place_equity_order
+  * place_changed_equity_order
+  * place_option_order
+  * place_changed_option_order
+  * cancel_order
+
+
+* Market API
+  * look_up_product
+  * get_quote
+  * get_option_chains
+  * get_option_expire_date
 
 ## Install
-```
+
+```bash
 pip install pyetrade
-- or -
+```
+OR
+```bash
 git clone https://github.com/jessecooper/pyetrade.git
 cd pyetrade
 sudo make init
 sudo make install
 ```
+
 ## Example Usage
 
 To create the OAuth tokens:
+
 ```python
 import pyetrade
 
 consumer_key = "<CONSUMER_KEY>"
 consumer_secret = "<SECRET_KEY>"
 
 oauth = pyetrade.ETradeOAuth(consumer_key, consumer_secret)
 print(oauth.get_request_token())  # Use the printed URL
 
 verifier_code = input("Enter verification code: ")
 tokens = oauth.get_access_token(verifier_code)
+
 print(tokens)
 ```
 
 And then on the example code:
 
 ```python
 import pyetrade
@@ -65,37 +96,51 @@
     consumer_secret,
     tokens['oauth_token'],
     tokens['oauth_token_secret']
 )
 
 print(accounts.list_accounts())
 ```
+
 ## Documentation
+
 [PyEtrade Documentation](https://pyetrade.readthedocs.io/en/latest/)
+
 ## Contribute to pyetrade
-* [ETrade API Docs](https://apisb.etrade.com/docs/api/account/api-account-v1.html)
+
+[ETrade API Docs](https://apisb.etrade.com/docs/api/account/api-account-v1.html)
+
+### Development Setup:
+
 * Fork pyetrade
-* Development Setup:
-```
-    make init
-    make devel
-```
-or
-```
-    pip install -r requirements.txt
-    pip install -r requirements_dev.txt
-    pip install -e .
-```
-* Lint
+* Setup development environment
+
+```bash
+make init
+make devel
 ```
-# Run Black
-black pyetrade/
-# Run Linter
-pylint pyetrade/  #Lint score should be >=8
+OR
+```bash
+pip install -r requirements.txt
+pip install -r requirements_dev.txt
+pip install -e .
+pre-commit install --hook-type pre-commit --hook-type pre-push --install-hooks -t post-checkout -t post-merge
 ```
-* Test
+
+* Lint (Run analysis - pre-commit-config)
+
+```bash
+make analysis
 ```
-make test #Ensure test coverage is >80%
+
+* Test (Coverage >= 90%)
+
+```bash
+make test
 ```
-* Push Changes:
-Push changes to a branch on your forked repo
+
+* Push Changes
+  * Push changes to a branch on your forked repo
+
+
 * Create pull request
+  * Open a pull request on pyetrade and put your fork as the source of your changes
```

### Comparing `pyetrade-2.0.1/pyetrade/__init__.py` & `pyetrade-2.1.0/pyetrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Init for pyetrade module  """
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 
 from . import authorization  # noqa: F401
 from .authorization import ETradeOAuth, ETradeAccessManager  # noqa: F401
 from . import accounts  # noqa: F401
 from .accounts import ETradeAccounts  # noqa: F401
 from . import market  # noqa: F401
 from .market import ETradeMarket  # noqa: F401
```

### Comparing `pyetrade-2.0.1/pyetrade/accounts.py` & `pyetrade-2.1.0/pyetrade/accounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,161 +1,169 @@
-"""Accounts - ETrade Accounts API Calls
-
-   TODO:
-       * Check request response for error
-
-       """
-
 import logging
+from datetime import datetime
+
 import xmltodict
 from requests_oauthlib import OAuth1Session
 
-# Set up logging
 LOGGER = logging.getLogger(__name__)
 
 
 class ETradeAccounts(object):
     """:description: Accounts object to access account information
 
-       :param client_key: Client key provided by Etrade
-       :type client_key: str, required
-       :param client_secret: Client secret provided by Etrade
-       :type client_secret: str, required
-       :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_key: str, required
-       :param resource_owner_secret: Resource secret from
-            :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_secret: str, required
-       :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
-       :type dev: bool, optional
-       :EtradeRef: https://apisb.etrade.com/docs/api/account/api-account-v1.html
-        """
+    :param client_key: Client key provided by Etrade
+    :type client_key: str, required
+    :param client_secret: Client secret provided by Etrade
+    :type client_secret: str, required
+    :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_key: str, required
+    :param resource_owner_secret: Resource secret from
+         :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_secret: str, required
+    :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
+    :type dev: bool, optional
+    :EtradeRef: https://apisb.etrade.com/docs/api/account/api-account-v1.html
+    """
 
     def __init__(
         self,
         client_key: str,
         client_secret: str,
         resource_owner_key: str,
         resource_owner_secret: str,
         dev: bool = True,
     ):
-        """__init_()
-           """
         self.client_key = client_key
         self.client_secret = client_secret
         self.resource_owner_key = resource_owner_key
         self.resource_owner_secret = resource_owner_secret
-        suffix = "apisb" if dev else "api"
-        self.base_url = r"https://%s.etrade.com/v1/accounts" % suffix
-        # self.base_url_prod = r"https://api.etrade.com/v1/accounts"
-        # self.base_url_dev = r"https://apisb.etrade.com/v1/accounts"
+        self.base_url = f'https://{"apisb" if dev else "api"}.etrade.com/v1/accounts'
         self.session = OAuth1Session(
             self.client_key,
             self.client_secret,
             self.resource_owner_key,
             self.resource_owner_secret,
             signature_type="AUTH_HEADER",
         )
 
-    def list_accounts(self, resp_format="xml") -> dict:
+    def list_accounts(self, resp_format: str = "xml") -> dict:
         """:description: Lists accounts in Etrade
 
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: List of accounts
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/account/api-account-v1.html
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: List of accounts
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-account-v1.html
         """
 
         api_url = "%s/list%s" % (
             self.base_url,
             ".json" if resp_format == "json" else "",
         )
 
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url)
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
-    def get_account_balance(self, account_id_key: str, account_type: str = None, real_time: bool = True, resp_format="xml") -> dict:  # noqa: E501
+    def get_account_balance(
+        self,
+        account_id_key: str,
+        account_type: str = None,
+        real_time: bool = True,
+        resp_format: str = "xml",
+    ) -> dict:
         """:description: Retrieves account balance for an account
 
-           :param account_id_key: AccountIDkey retrieved from :class:`list_accounts`
-           :type  account_id_key: str, required
-           :param account_type: The registered account type, defaults to None
-           :type  account_type: str, optional
-           :param real_time: Use real time balance or not, defaults to True
-           :type  real_time: bool, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Balance of account with key ``account_id_key``
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/account/api-balance-v1.html
+        :param account_id_key: AccountIDkey retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :param account_type: The registered account type, defaults to None
+        :type  account_type: str, optional
+        :param real_time: Use real time balance or not, defaults to True
+        :type  real_time: bool, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Balance of account with key ``account_id_key``
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-balance-v1.html
         """
 
         api_url = "%s/%s/balance%s" % (
             self.base_url,
             account_id_key,
             ".json" if resp_format == "json" else "",
         )
 
         payload = {"realTimeNAV": real_time, "instType": "BROKERAGE"}
 
         if account_type:
             payload["accountType"] = account_type
 
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url, params=payload)
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
     def get_account_portfolio(
-            self,
-            account_id_key: str,
-            count: int = 50,
-            sort_by: str = None,
-            sort_order: str = "DESC",
-            page_number: int = None,
-            market_session: str = "REGULAR",
-            totals_required: bool = False,
-            lots_required: bool = False,
-            view: str = "QUICK",
-            resp_format="xml"
+        self,
+        account_id_key: str,
+        count: int = 50,
+        sort_by: str = None,
+        sort_order: str = "DESC",
+        page_number: int = None,
+        market_session: str = "REGULAR",
+        totals_required: bool = False,
+        lots_required: bool = False,
+        view: str = "QUICK",
+        resp_format: str = "xml",
     ) -> dict:
         """:description: Retrieves account portfolio for an account
 
-           :param account_id_key: AccountIDkey retrieved from :class:`list_accounts`
-           :type  account_id_key: str, required
-           :param count: The number of positions to return in the response, defaults to 50
-           :type  count: int, optional
-           :param sort_by: Sorting done based on the column specified in the query parameter.
-           :type  sort_by: str, optional
-           :param sort_order: Sort orders (ASC or DESC), defaults to DESC
-           :type  sort_order: str, optional
-           :param page_number: The specific page that in the list that is to be returned. Each page has a default count of 50 positions.  # noqa: E501
-           :type  page_number: int, optional
-           :param market_session: The market session (Regular or Extended), defaults to REGULAR
-           :type  market_session: str, optional
-           :param totals_required: It gives the total values of the portfolio, defaults to False
-           :type  totals_required: bool, optional
-           :param lots_required: It gives position lots for positions, defaults to False
-           :type  lots_required: bool, optional
-           :param view: The view query: PERFORMANCE, FUNDAMENTAL, OPTIONSWATCH, QUICK, COMPLETE. Defaults to QUICK.
-           :type  view: str, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Account portfolio of account with key ``account_id_key``
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/account/api-portfolio-v1.html
-
-           """
+        :param account_id_key: AccountIDkey retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :param count: The number of positions to return in the response, defaults to 50
+        :type  count: int, optional
+        :param sort_by: Sorting done based on the column specified in the query parameter.
+        :type  sort_by: str, optional
+        :param sort_order: Sort orders (ASC or DESC), defaults to DESC
+        :type  sort_order: str, optional
+        :param page_number: The specific page that in the list that is to be returned.
+                            Each page has a default count of 50 positions.
+        :type  page_number: int, optional
+        :param market_session: The market session, defaults to REGULAR
+        :type  market_session: str, optional
+        :market_session values:
+            * REGULAR
+            * EXTENDED
+        :param totals_required: It gives the total values of the portfolio, defaults to False
+        :type  totals_required: bool, optional
+        :param lots_required: It gives position lots for positions, defaults to False
+        :type  lots_required: bool, optional
+        :param view: The view query, defaults to QUICK.
+        :type  view: str, optional
+        :view values:
+            * PERFORMANCE
+            * FUNDAMENTAL
+            * OPTIONSWATCH
+            * QUICK
+            * COMPLETE
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Account portfolio of account with key ``account_id_key``
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-portfolio-v1.html
+        """
 
         api_url = "%s/%s/portfolio%s" % (
             self.base_url,
             account_id_key,
             ".json" if resp_format == "json" else "",
         )
 
@@ -163,106 +171,170 @@
             "count": count,
             "sortBy": sort_by,
             "sortOrder": sort_order,
             "pageNumber": page_number,
             "marketSession": market_session,
             "totalsRequired": totals_required,
             "lotsRequired": lots_required,
-            "view": view
+            "view": view,
         }
 
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url, params=payload)
         req.raise_for_status()
+
+        LOGGER.debug(req.text)
+
+        return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
+
+    def get_portfolio_position_lot(
+        self, symbol: str, account_id_key: str, resp_format: str = "xml"
+    ) -> dict:
+        """:description: Retrieves account portfolio position lot based on provided symbol
+
+        :param symbol: Desired equity symbol to search for position lots in desired account portfolio
+        :type  symbol: str, required
+        :param account_id_key: AccountIDkey retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: PositionLot of ``symbol`` in account portfolio of account with key ``account_id_key``
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-portfolio-v1.html
+        """
+
+        account_portfolio = self.get_account_portfolio(
+            account_id_key, lots_required=True, resp_format="json"
+        )["PortfolioResponse"]["AccountPortfolio"][0]["Position"]
+
+        lot_position_id = [
+            position["positionId"]
+            for position in account_portfolio
+            if symbol.upper() == position["Product"]["symbol"].upper()
+        ]
+
+        # If the symbol exists then there should only be one ID filtered from the portfolio response
+        if len(lot_position_id) != 1:
+            raise KeyError(
+                f'Symbol "{symbol}" could not be found in the current portfolio. '
+                f"Please check your portfolio and symbol before trying again."
+            )
+
+        LOGGER.debug(lot_position_id[0])
+
+        api_url = "%s/%s/portfolio/%s%s" % (
+            self.base_url,
+            account_id_key,
+            lot_position_id[0],
+            ".json" if resp_format == "json" else "",
+        )
+
+        req = self.session.get(api_url)
+        req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
     def list_transactions(
-            self,
-            account_id_key: str,
-            start_date: str = None,
-            end_date: str = None,
-            sort_order: str = "DESC",
-            marker=None,
-            count: int = 50,
-            resp_format="xml"
+        self,
+        account_id_key: str,
+        start_date: datetime = None,
+        end_date: datetime = None,
+        sort_order: str = "DESC",
+        marker: str = None,
+        count: int = 50,
+        resp_format: str = "xml",
     ) -> dict:
         """:description: Retrieves transactions for an account
 
-           :param account_id_key: AccountIDKey retrieved from :class:`list_accounts`
-           :type  account_id_key: str, required
-           :param start_date: The earliest date to include in the date range, formatted as MMDDYYYY (history is available for two years), default is None  # noqa: E501
-           :type  start_date: str, optional
-           :param end_date: The latest date to include in the date range, formatted as MMDDYYYY, default is None
-           :type  end_date: `str, optional
-           :param sort_order: The sort order request (ASC or DESC), default is DESC
-           :type  sort_order: str, optional
-           :param marker: Specifies the desired starting point of the set of items to return (used for paging), default is None  # noqa: E501
-           :type  marker: ??, optional
-           :param count: Number of transactions to return in the response, default is 50
-           :type  count: int, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Transactions list for account with key ``account_id_key``
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/account/api-transaction-v1.html
+        :param account_id_key: AccountIDKey retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :param start_date: The earliest date to include in the date range (history is available for two years),
+                           defaults to None
+        :type  start_date: datetime obj, optional
+        :param end_date: The latest date to include in the date range (history is available for two years),
+                         defaults to None
+        :type  end_date: datetime obj, optional
+        :param sort_order: The sort order request (ASC or DESC), default is DESC
+        :type  sort_order: str, optional
+        :param marker: Specifies the desired starting point of the set of items to return (used for paging),
+                       default is None
+        :type  marker: str, optional
+        :param count: Number of transactions to return in the response, default is 50
+        :type  count: int, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Transactions list for account with key ``account_id_key``
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-transaction-v1.html
         """
 
         api_url = "%s/%s/transactions%s" % (
             self.base_url,
             account_id_key,
             ".json" if resp_format == "json" else "",
         )
 
         payload = {
-            "startDate": start_date,
-            "endDate": end_date,
+            "startDate": start_date.date().strftime("%m%d%Y") if start_date else None,
+            "endDate": end_date.date().strftime("%m%d%Y") if end_date else None,
             "sortOrder": sort_order,
             "marker": marker,
-            "count": count
+            "count": count,
         }
 
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url, params=payload)
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         # Depending on when transactions are completed and start/end date
         # restrictions, it's possible for the response to return nothing: ""
         if req.text == "":
             return {}
         elif resp_format.lower() == "xml":
             return xmltodict.parse(req.text)
         else:
             return req.json()
 
-    def list_transaction_details(self, account_id_key: str, transaction_id: int, resp_format="xml", **kwargs) -> dict:
+    def list_transaction_details(
+        self,
+        account_id_key: str,
+        transaction_id: int,
+        store_id: any = None,
+        resp_format: str = "xml",
+    ) -> dict:
         """:description: Retrieves transaction details for an account
 
-           :param account_id_key: AccountIDKey retrieved from :class:`list_accounts`
-           :type  account_id_key: str, required
-           :param transaction_id: Numeric transaction ID obtained from :class:`list_transactions`
-           :type  transaction_id: int, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :param kwargs: Parameters for api
-           :type  kwargs: ``**kwargs``, optional
-           :return: Transaction Details for ``transaction_id`` for account key ``account_id_key``
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/account/api-transaction-v1.html
-           """
+        :param account_id_key: AccountIDKey retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :param transaction_id: Numeric transaction ID obtained from :class:`list_transactions`
+        :type  transaction_id: int, required
+        :param store_id: storage location for older transactions
+        :type  store_id: Unknown, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Transaction Details for ``transaction_id`` for account key ``account_id_key``
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/account/api-transaction-v1.html
+        """
 
         # Set Env
-        api_url = "%s/%s/transactions%s/%s" % (
+        api_url = "%s/%s/transactions/%s%s" % (
             self.base_url,
             account_id_key,
-            ".json" if resp_format == "json" else "",
             transaction_id,
+            ".json" if resp_format == "json" else "",
         )
 
         LOGGER.debug(api_url)
-        req = self.session.get(api_url, params=kwargs)
+
+        req = self.session.get(api_url, params={"storeId": store_id})
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
```

### Comparing `pyetrade-2.0.1/pyetrade/alerts.py` & `pyetrade-2.1.0/pyetrade/alerts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,127 +1,144 @@
 """Alerts - ETrade Alerts API
 """
-
 import logging
+
 import xmltodict
 from requests_oauthlib import OAuth1Session
 
 # Set up logging
 LOGGER = logging.getLogger(__name__)
 
 
 class ETradeAlerts(object):
     """:description: Object to retrieve alerts
 
-       :param client_key: Client key provided by Etrade
-       :type client_key: str, required
-       :param client_secret: Client secret provided by Etrade
-       :type client_secret: str, required
-       :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_key: str, required
-       :param resource_owner_secret: Resource secret from
-              :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_secret: str, required
-       :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
-       :type dev: bool, optional
-       :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
-
+    :param client_key: Client key provided by Etrade
+    :type client_key: str, required
+    :param client_secret: Client secret provided by Etrade
+    :type client_secret: str, required
+    :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_key: str, required
+    :param resource_owner_secret: Resource secret from
+           :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_secret: str, required
+    :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
+    :type dev: bool, optional
+    :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
     """
 
     def __init__(
         self,
         client_key: str,
         client_secret: str,
         resource_owner_key: str,
         resource_owner_secret: str,
         dev: bool = True,
     ):
         self.client_key = client_key
         self.client_secret = client_secret
         self.resource_owner_key = resource_owner_key
         self.resource_owner_secret = resource_owner_secret
-        suffix = "apisb" if dev else "api"
-        self.base_url = r"https://%s.etrade.com/v1/user/alerts" % suffix
+        self.base_url = f'https://{"apisb" if dev else "api"}.etrade.com/v1/user/alerts'
         self.session = OAuth1Session(
             self.client_key,
             self.client_secret,
             self.resource_owner_key,
             self.resource_owner_secret,
             signature_type="AUTH_HEADER",
         )
 
-    def list_alerts(self, count: int = 25 <= 300, sort_order: str = "DESC", resp_format="xml") -> dict:
+    def list_alerts(
+        self, count: int = 25, sort_order: str = "DESC", resp_format: str = "xml"
+    ) -> dict:
         """:description: Lists alerts in Etrade
 
-           :param count: The alert count, defaults to 25 (max 300)
-           :type  count: int, optional
-           :param sort_order: Sorting is done based on the createDate (ASC or DESC), defaults to DESC
-           :type  sort_order: str, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: List of alerts
-           :rtype: ``xml`` or ``json`` based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
-
-           """
-        api_url = "%s%s" % (self.base_url, ".json" if resp_format == "json" else "")
+        :param count: The alert count, defaults to 25 (max 300)
+        :type  count: int, optional
+        :param sort_order: Sorting is done based on the createDate (ASC or DESC), defaults to DESC
+        :type  sort_order: str, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: List of alerts
+        :rtype: ``xml`` or ``json`` based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
+        """
 
+        api_url = "%s%s" % (
+            self.base_url,
+            ".json" if resp_format == "json" else "",
+        )
         LOGGER.debug(api_url)
-        req = self.session.get(api_url, params={"count": count, "direction": sort_order})
+
+        if count >= 301:
+            LOGGER.debug(
+                f"Count {count} is greater than the max allowable value (300), using 300"
+            )
+            count = 300
+
+        req = self.session.get(
+            api_url, params={"count": count, "direction": sort_order}
+        )
+
         req.raise_for_status()
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
-    def list_alert_details(self, alert_id: int, html_tags: bool = False, resp_format="xml") -> dict:
+    def list_alert_details(
+        self, alert_id: int, html_tags: bool = False, resp_format: str = "xml"
+    ) -> dict:
         """:description: Provides details for an alert
 
-           :param alert_id: Alert ID obtained from :class:`list_alerts`
-           :type alert_id: int, required
-           :param html_tags: The HTML tags on the alert, defaults to false. If set to true, it returns the alert details msgText with html tags.  # noqa: E501
-           :type  html_tags: bool, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: List of alert details
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
-
-           """
+        :param alert_id: Alert ID obtained from :class:`list_alerts`
+        :type alert_id: int, required
+        :param html_tags: The HTML tags on the alert, defaults to false. If set to true,
+                          it returns the alert details msgText with html tags.
+        :type  html_tags: bool, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: List of alert details
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
+        """
 
         api_url = "%s%s/%s" % (
             self.base_url,
             ".json" if resp_format == "json" else "",
             alert_id,
         )
 
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url, params={"htmlTags": html_tags})
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
-    def delete_alert(self, alert_id: int, resp_format="xml") -> dict:
+    def delete_alert(self, alert_id: int, resp_format: str = "xml") -> dict:
         """:description: Deletes specified alert
 
-           :param alert_id: Alert ID obtained from :class:`list_alerts`
-           :type alert_id: int, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: List of alert details
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
-
+        :param alert_id: Alert ID obtained from :class:`list_alerts`
+        :type alert_id: int, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: List of alert details
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/user/api-alert-v1.html
         """
 
         api_url = "%s%s/%s" % (
             self.base_url,
             ".json" if resp_format == "json" else "",
             alert_id,
         )
 
         LOGGER.debug(api_url)
+
         req = self.session.delete(api_url)
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
```

### Comparing `pyetrade-2.0.1/pyetrade/authorization.py` & `pyetrade-2.1.0/pyetrade/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """Authorization - ETrade Authorization API Calls
 
    TODO:
     * Catch events
 
 """
-
 import logging
+
 from requests_oauthlib import OAuth1Session
 
 # Set up logging
 LOGGER = logging.getLogger(__name__)
 
 
 class ETradeOAuth(object):
     """:description: Performs authorization for OAuth 1.0a
 
-       :param consumer_key: Client key provided by Etrade
-       :type consumer_key: str, required
-       :param consumer_secret: Client secret provided by Etrade
-       :type consumer_secret: str, required
-       :param callback_url: Callback URL passed to OAuth mod, defaults to "oob"
-       :type callback_url: str, optional
-       :EtradeRef: https://apisb.etrade.com/docs/api/authorization/request_token.html
-
+    :param consumer_key: Client key provided by Etrade
+    :type consumer_key: str, required
+    :param consumer_secret: Client secret provided by Etrade
+    :type consumer_secret: str, required
+    :param callback_url: Callback URL passed to OAuth mod, defaults to "oob"
+    :type callback_url: str, optional
+    :EtradeRef: https://apisb.etrade.com/docs/api/authorization/request_token.html
     """
 
-    def __init__(self, consumer_key: str, consumer_secret: str, callback_url: str = "oob"):
+    def __init__(
+        self, consumer_key: str, consumer_secret: str, callback_url: str = "oob"
+    ):
         self.consumer_key = consumer_key
         self.consumer_secret = consumer_secret
         self.base_url_prod = r"https://api.etrade.com"
         self.base_url_dev = r"https://apisb.etrade.com"
         self.req_token_url = r"https://api.etrade.com/oauth/request_token"
         self.auth_token_url = r"https://us.etrade.com/e/t/etws/authorize"
         self.access_token_url = r"https://api.etrade.com/oauth/access_token"
         self.callback_url = callback_url
         self.access_token = None
         self.resource_owner_key = None
 
     def get_request_token(self) -> str:
         """:description: Obtains the token URL from Etrade.
 
-           :param None: Takes no parameters
-           :return: Formatted Authorization URL (Access this to obtain taken)
-           :rtype: str
-           :EtradeRef: https://apisb.etrade.com/docs/api/authorization/request_token.html
-
+        :param None: Takes no parameters
+        :return: Formatted Authorization URL (Access this to obtain taken)
+        :rtype: str
+        :EtradeRef: https://apisb.etrade.com/docs/api/authorization/request_token.html
         """
 
         # Set up session
         self.session = OAuth1Session(
             self.consumer_key,
             self.consumer_secret,
             callback_uri=self.callback_url,
@@ -70,83 +70,91 @@
         LOGGER.debug(formated_auth_url)
 
         return formated_auth_url
 
     def get_access_token(self, verifier: str) -> dict:
         """:description: Obtains access token. Requires token URL from :class:`get_request_token`
 
-           :param verifier: OAuth Verification Code from Etrade
-           :type verifier: str, required
-           :return: OAuth access tokens
-           :rtype: dict
-           :EtradeRef: https://apisb.etrade.com/docs/api/authorization/get_access_token.html
-
+        :param verifier: OAuth Verification Code from Etrade
+        :type verifier: str, required
+        :return: OAuth access tokens
+        :rtype: dict
+        :EtradeRef: https://apisb.etrade.com/docs/api/authorization/get_access_token.html
         """
 
         # Set verifier
         self.session._client.client.verifier = verifier
         # Get access token
         self.access_token = self.session.fetch_access_token(self.access_token_url)
         LOGGER.debug(self.access_token)
 
         return self.access_token
 
 
 class ETradeAccessManager(object):
     """:description: Renews and revokes ETrade OAuth access tokens
 
-       :param client_key: Client key provided by Etrade
-       :type client_key: str, required
-       :param client_secret: Client secret provided by Etrade
-       :type client_secret: str, required
-       :param resource_owner_key: Resource key from :class:`ETradeOAuth`
-       :type resource_owner_key: str, required
-       :param resource_owner_secret: Resource secret from :class:`ETradeOAuth`
-       :type resource_owner_secret: str, required
-       :EtradeRef: https://apisb.etrade.com/docs/api/authorization/renew_access_token.html
-
+    :param client_key: Client key provided by Etrade
+    :type client_key: str, required
+    :param client_secret: Client secret provided by Etrade
+    :type client_secret: str, required
+    :param resource_owner_key: Resource key from :class:`ETradeOAuth`
+    :type resource_owner_key: str, required
+    :param resource_owner_secret: Resource secret from :class:`ETradeOAuth`
+    :type resource_owner_secret: str, required
+    :EtradeRef: https://apisb.etrade.com/docs/api/authorization/renew_access_token.html
     """
 
-    def __init__(self, client_key: str, client_secret: str, resource_owner_key: str, resource_owner_secret: str):
+    def __init__(
+        self,
+        client_key: str,
+        client_secret: str,
+        resource_owner_key: str,
+        resource_owner_secret: str,
+    ):
         self.client_key = client_key
         self.client_secret = client_secret
         self.resource_owner_key = resource_owner_key
         self.resource_owner_secret = resource_owner_secret
         self.renew_access_token_url = r"https://api.etrade.com/oauth/renew_access_token"
-        self.revoke_access_token_url = r"https://api.etrade.com/oauth/revoke_access_token"
+        self.revoke_access_token_url = (
+            r"https://api.etrade.com/oauth/revoke_access_token"
+        )
         self.session = OAuth1Session(
             self.client_key,
             self.client_secret,
             self.resource_owner_key,
             self.resource_owner_secret,
             signature_type="AUTH_HEADER",
         )
 
     def renew_access_token(self) -> bool:
         """:description: Renews access tokens obtained from :class:`ETradeOAuth`
 
-           :param None: Takes no parameters
-           :return: Success or failure
-           :rtype: bool (True or False)
-           :EtradeRef: https://apisb.etrade.com/docs/api/authorization/renew_access_token.html
-
+        :param None: Takes no parameters
+        :return: Success or failure
+        :rtype: bool (True or False)
+        :EtradeRef: https://apisb.etrade.com/docs/api/authorization/renew_access_token.html
         """
+
         resp = self.session.get(self.renew_access_token_url)
-        LOGGER.debug(resp.text)
         resp.raise_for_status()
 
+        LOGGER.debug(resp.text)
+
         return True
 
     def revoke_access_token(self) -> bool:
         """:description: Revokes access tokens obtained from :class:`ETradeOAuth`
 
-           :param None: Takes no parameters
-           :return: Success or failure
-           :rtype: bool (True or False)
-           :EtradeRef: https://apisb.etrade.com/docs/api/authorization/revoke_access_token.html
-
+        :param None: Takes no parameters
+        :return: Success or failure
+        :rtype: bool (True or False)
+        :EtradeRef: https://apisb.etrade.com/docs/api/authorization/revoke_access_token.html
         """
+
         resp = self.session.get(self.revoke_access_token_url)
-        LOGGER.debug(resp.text)
         resp.raise_for_status()
 
+        LOGGER.debug(resp.text)
+
         return True
```

### Comparing `pyetrade-2.0.1/pyetrade/market.py` & `pyetrade-2.1.0/pyetrade/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Market - ETrade Market API V1
 
     TODO:
-    * move logger into object under self.logger
+     * move logger into object under self.logger
 
 """
-
 import logging
-import xmltodict
 from datetime import datetime
+
+import xmltodict
 from requests_oauthlib import OAuth1Session
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ETradeMarket(object):
     """:description: Performs Market functions
 
-       :param client_key: Client key provided by Etrade
-       :type client_key: str, required
-       :param client_secret: Client secret provided by Etrade
-       :type client_secret: str, required
-       :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_key: str, required
-       :param resource_owner_secret: Resource secret from
-              :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_secret: str, required
-       :param dev: Defines Sandboxi (True) or Live (False) ETrade, defaults to True
-       :type dev: bool, optional
-       :EtradeRef: https://apisb.etrade.com/docs/api/market/api-quote-v1.html
+    :param client_key: Client key provided by Etrade
+    :type client_key: str, required
+    :param client_secret: Client secret provided by Etrade
+    :type client_secret: str, required
+    :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_key: str, required
+    :param resource_owner_secret: Resource secret from
+           :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_secret: str, required
+    :param dev: Defines Sandboxi (True) or Live (False) ETrade, defaults to True
+    :type dev: bool, optional
+    :EtradeRef: https://apisb.etrade.com/docs/api/market/api-quote-v1.html
 
     """
 
     def __init__(
         self,
         client_key: str,
         client_secret: str,
@@ -40,99 +40,98 @@
         dev: bool = True,
     ):
         self.client_key = client_key
         self.client_secret = client_secret
         self.resource_owner_key = resource_owner_key
         self.resource_owner_secret = resource_owner_secret
         self.dev_environment = dev
-        suffix = "apisb" if dev else "api"
-        self.base_url = r"https://%s.etrade.com/v1/market/" % suffix
+        self.base_url = f'https://{"apisb" if dev else "api"}.etrade.com/v1/market/'
         self.session = OAuth1Session(
             self.client_key,
             self.client_secret,
             self.resource_owner_key,
             self.resource_owner_secret,
             signature_type="AUTH_HEADER",
         )
 
     def __str__(self):
         ret = [
             "Use development environment: %s" % self.dev_environment,
-            "base URL: %s" % self.base_url,
+            "Base URL: %s" % self.base_url,
         ]
         return "\n".join(ret)
 
-    def look_up_product(self, search_str: str, resp_format="xml") -> dict:
+    def look_up_product(self, search_str: str, resp_format: str = "xml") -> dict:
         """:description: Performs a look-up product
 
-           :param search_str: Full or partial name of the company.
-           :type search_str: str, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Product lookup
-           :rtype: ``xml`` or ``json`` as defined by ``resp_format``
-           :Note: Etrade abbreviates common words such as company, industry and systems
-                  and generally skips punctuation.
-           :EtradeRef:
-                  https://apisb.etrade.com/docs/api/market/api-market-v1.html#/definition/Lookup
-
+        :param search_str: Full or partial name of the company.
+        :type search_str: str, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Product lookup
+        :rtype: ``xml`` or ``json`` as defined by ``resp_format``
+        :Note: Etrade abbreviates common words such as company, industry and systems
+               and generally skips punctuation.
+        :EtradeRef: https://apisb.etrade.com/docs/api/market/api-market-v1.html#/definition/Lookup
         """
 
         # api_url = self.base_url + "lookup/%s" % search_str
         api_url = "%slookup/%s" % (
             self.base_url,
-            search_str if resp_format.lower() == "xml" else search_str + ".json",
+            search_str if resp_format.lower() == "xml" else f"{search_str}.json",
         )
         LOGGER.debug(api_url)
+
         req = self.session.get(api_url)
         req.raise_for_status()
+
         LOGGER.debug(req.text)
+
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
     def get_quote(
         self,
-        symbols: list,
+        symbols: list[str],
         detail_flag: str = None,
         require_earnings_date: str = None,
         skip_mini_options_check: str = None,
-        resp_format="xml",
+        resp_format: str = "xml",
     ) -> dict:
         """:description: Get quote data on symbols provided in the list args.
 
-           :param symbols: Symbols in list args format. Limit 25.
-           :type symbols: list[], required
-           :param detail_flag: Market fields returned from a quote request, defaults to None
-           :type detail_flag: str, optional
-           :param require_earnings_date: Provides Earnings date if True, defaults to None
-           :type require_earnings_date: str, optional
-           :param skip_mini_options_check: Skips mini options check if True, defaults to None
-           :type skip_mini_options_check: str, optional
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Returns quote data on symbols provided
-           :rtype: xml or json based on ``resp_format``
-           :symbols values:
-               * Limited to 25. If exceeded, first 25 will be processed with warnings
-               * Equities format - ``symbol`` name sufficient, e.g. GOOGL.
-               * Options format - ``underlier:year:month:day:optionType:strikePrice``
-           :detailflag values:
-               * fundamental - Instrument fundamentals and latest price
-               * intraday - Performance for the current of most recent trading day
-               * options - Information on a given option offering
-               * week_52 - 52-week high and low (highest high and lowest low)
-               * mf_detail - MutualFund structure gets displayed
-               * all (default) - All of the above information and more
-               * None - Defaults to all.
-           :skipMiniOptionsCheck values:
-               * True - Call is NOT made to check whether the symbol has mini options
-               * False - Call is made to check whether the symbol has mini options
-               * None - Call is made to check whether the symbol has mini options (default)
-           :EtradeRef: https://apisb.etrade.com/docs/api/market/api-quote-v1.html
-
-            """
+        :param symbols: Symbols in list args format. Limit 25.
+        :type symbols: list[str], required
+        :param detail_flag: Market fields returned from a quote request, defaults to None
+        :type detail_flag: str, optional
+        :param require_earnings_date: Provides Earnings date if True, defaults to None
+        :type require_earnings_date: str, optional
+        :param skip_mini_options_check: Skips mini options check if True, defaults to None
+        :type skip_mini_options_check: str, optional
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Returns quote data on symbols provided
+        :rtype: xml or json based on ``resp_format``
+        :symbols values:
+            * Limited to 25. If exceeded, first 25 will be processed with warnings
+            * Equities format - ``symbol`` name sufficient, e.g. GOOGL.
+            * Options format - ``underlier:year:month:day:optionType:strikePrice``
+        :detailflag values:
+            * fundamental - Instrument fundamentals and latest price
+            * intraday - Performance for the current of most recent trading day
+            * options - Information on a given option offering
+            * week_52 - 52-week high and low (highest high and lowest low)
+            * mf_detail - MutualFund structure gets displayed
+            * all (default) - All of the above information and more
+            * None - Defaults to all.
+        :skipMiniOptionsCheck values:
+            * True - Call is NOT made to check whether the symbol has mini options
+            * False - Call is made to check whether the symbol has mini options
+            * None - Call is made to check whether the symbol has mini options (default)
+        :EtradeRef: https://apisb.etrade.com/docs/api/market/api-quote-v1.html
+        """
 
         if detail_flag is not None:
             detail_flag = detail_flag.lower()
 
         assert detail_flag in (
             "fundamental",
             "intraday",
@@ -143,18 +142,21 @@
             None,
         )
 
         assert require_earnings_date in (True, False, None)
         assert skip_mini_options_check in (True, False, None)
         assert isinstance(symbols, list or tuple)
 
-        if len(symbols) > 25:
-            LOGGER.warning("get_quote asked for %d requests; only first 25 returned" % len(symbols))
+        if len(symbols) >= 26:
+            LOGGER.warning(
+                "get_quote asked for %d requests; only first 25 returned" % len(symbols)
+            )
 
         args = list()
+
         if detail_flag is not None:
             args.append("detailflag=%s" % detail_flag.upper())
         if require_earnings_date:
             args.append("requireEarningsDate=true")
         if skip_mini_options_check is not None:
             args.append("skipMiniOptionsCheck=%s" % str(skip_mini_options_check))
 
@@ -178,57 +180,56 @@
         expiry_date: datetime.date,
         skip_adjusted: str = None,
         chain_type: str = None,
         strike_price_near: int = None,
         no_of_strikes: int = None,
         option_category: str = None,
         price_type: str = None,
-        resp_format="xml",
+        resp_format: str = "xml",
     ) -> dict:
         """:description: Returns the option chain information for the
-                         requested expiry_date and chaintype in the desired format.
-                         This should be a list of dictionaries,
-                         one for each option chain.
-
-           :param underlier: Market Symbol
-           :type underlier: str, required
-           :param expiry_date: Contract expiration date, None produces closest to today
-           :type expiry_date: datetime.date(year, month, day), optional
-           :param skip_adjusted: Specifies whether to show (True) or not show (False) adjusted
-                                 options, defaults to True
-           :type skip_adjusted: str, optional
-           :param chain_type: Type of option chain, defaults to callput
-           :type chain_type: str, optional
-           :param strike_price_near: Optionchains fetched will have strike price close to this value
-           :type strike_price_near: int, optional
-           :param no_of_strikes: Indicates number of strikes for which the optionchain
-                                 needs to be fetched, defaults to None
-           :type no_of_strikes: int, optional
-           :param option_category: The option category, defaults to ``standard``
-           :type option_category: str, optional
-           :param price_type: The price type, defaults to ``atnm``
-           :type price_type: str, optional
-           :param resp_format: Desired Response format, defaults to ``xml``
-           :type  resp_format: str, optional
-           :return: Returns list of option chains for a specific underlying instrument
-           :rtype: xml or json based on ``resp_format``
-           :chain_type values:
-               * put
-               * call
-               * callput (default)
-           :option_category values:
-               * standard (default)
-               * all
-               * mini
-           :price_type values:
-               * atnm
-               * all
-           :sampleURL: https://api.etrade.com/v1/market/optionchains?expiryDay=03&expiryMonth=04&expiryYear=2011&chainType=PUT&skipAdjusted=true&symbol=GOOGL  # noqa: E501
-           :EtradeRef: https://apisb.etrade.com/docs/api/market/api-market-v1.html
-
+                      requested expiry_date and chain-type in the desired format.
+                      This should be a list of dictionaries,
+                      one for each option chain.
+
+        :param underlier: Market Symbol
+        :type underlier: str, required
+        :param expiry_date: Contract expiration date, None produces closest to today
+        :type expiry_date: datetime.date(year, month, day), optional
+        :param skip_adjusted: Specifies whether to show (True) or not show (False) adjusted
+                              options, defaults to True
+        :type skip_adjusted: str, optional
+        :param chain_type: Type of option chain, defaults to call/put
+        :type chain_type: str, optional
+        :param strike_price_near: Option chains fetched will have strike price close to this value
+        :type strike_price_near: int, optional
+        :param no_of_strikes: Indicates number of strikes for which the option chain
+                              needs to be fetched, defaults to None
+        :type no_of_strikes: int, optional
+        :param option_category: The option category, defaults to ``standard``
+        :type option_category: str, optional
+        :param price_type: The price type, defaults to ``atnm``
+        :type price_type: str, optional
+        :param resp_format: Desired Response format, defaults to ``xml``
+        :type  resp_format: str, optional
+        :return: Returns list of option chains for a specific underlying instrument
+        :rtype: xml or json based on ``resp_format``
+        :chain_type values:
+            * put
+            * call
+            * call/put (default)
+        :option_category values:
+            * standard (default)
+            * all
+            * mini
+        :price_type values:
+            * atnm
+            * all
+        :sampleURL: https://api.etrade.com/v1/market/optionchains?expiryDay=03&expiryMonth=04&expiryYear=2011&chainType=PUT&skipAdjusted=true&symbol=GOOGL  # noqa: E501
+        :EtradeRef: https://apisb.etrade.com/docs/api/market/api-market-v1.html
         """
 
         if chain_type is not None:
             chain_type = chain_type.lower()
         assert chain_type in ("put", "call", "callput", None)
 
         if option_category is not None:
@@ -239,14 +240,15 @@
             price_type = price_type.lower()
         assert price_type in ("atmn", "all", None)
 
         assert skip_adjusted in (True, False, None)
         assert isinstance(resp_format, str)
 
         args = ["symbol=%s" % underlier]
+
         if expiry_date is not None:
             args.append(
                 "expiryDay=%02d&expiryMonth=%02d&expiryYear=%04d"
                 % (expiry_date.day, expiry_date.month, expiry_date.year)
             )
         if strike_price_near is not None:
             args.append("strikePriceNear=%0.2f" % strike_price_near)
@@ -258,49 +260,50 @@
             args.append("priceType=%s" % price_type.upper())
         if skip_adjusted is not None:
             args.append("skipAdjusted=%s" % str(skip_adjusted))
         if no_of_strikes is not None:
             args.append("noOfStrikes=%d" % no_of_strikes)
 
         api_url = "%s%s%s" % (
-            self.base_url, "optionchains?" if resp_format.lower() == "xml" else "optionchains.json?", "&".join(args),
+            self.base_url,
+            "optionchains?" if resp_format.lower() == "xml" else "optionchains.json?",
+            "&".join(args),
         )
+        LOGGER.debug(api_url)
 
         req = self.session.get(api_url)
         req.raise_for_status()
-        LOGGER.debug(api_url)
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
-    def get_option_expire_date(self, symbol: str, resp_format="xml") -> dict:
+    def get_option_expire_date(self, symbol: str, resp_format: str = "xml") -> dict:
         """:description: Returns a list of dates suitable for structuring an option table display
 
-           :param symbol: Market Symbol
-           :type symbol: str, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, optional
-           :return: Returns expiry of options for symbol
-           :rtype: xml or json based on ``resp_format``
-           :sampleURL: https://api.etrade.com/v1/market/optionexpiredate?symbol=GOOG&expiryType=ALL
-           :EtradeRef: https://apisb.etrade.com/docs/api/market/api-market-v1.html
-
+        :param symbol: Market Symbol
+        :type symbol: str, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, optional
+        :return: Returns expiry of options for symbol
+        :rtype: xml or json based on ``resp_format``
+        :sampleURL: https://api.etrade.com/v1/market/optionexpiredate?symbol=GOOG&expiryType=ALL
+        :EtradeRef: https://apisb.etrade.com/docs/api/market/api-market-v1.html
         """
 
-        assert isinstance(resp_format, str)
         assert resp_format in ["xml", "json"]
 
         api_url = "%s%s" % (
             self.base_url,
             "optionexpiredate"
             if resp_format.lower() == "xml"
             else "optionexpiredate.json",
         )
 
-        payload = {"symbol": symbol, "expiryType": "ALL"}
         LOGGER.debug(api_url)
 
-        req = self.session.get(api_url, params=payload)
+        req = self.session.get(api_url, params={"symbol": symbol, "expiryType": "ALL"})
         req.raise_for_status()
+
         LOGGER.debug(req.text)
 
         return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
```

### Comparing `pyetrade-2.0.1/pyetrade/order.py` & `pyetrade-2.1.0/pyetrade/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,218 +1,314 @@
-"""Order - ETrade Order API
-
-   TODO:
-       * Preview equity order change
-       * Place equity order change
-       * Preview option order
-       * Place option order
-       * Preview option order change
-       * Place option order change
-
-"""
-
 import logging
-import xmltodict
-import dateutil.parser
-
+from datetime import datetime
 from typing import Union
+
+import dateutil.parser
+import xmltodict
 from jxmlease import emit_xml
 from requests_oauthlib import OAuth1Session
 
 LOGGER = logging.getLogger(__name__)
 
 # some constants
 CALL = "Call"
 PUT = "Put"
 
 
-# price: number
-# round_down: bool
-# return string
 def to_decimal_str(price: float, round_down: bool) -> str:
     spstr = "%.2f" % price  # round to 2-place decimal
     spstrf = float(spstr)  # convert back to float again
     diff = price - spstrf
 
     if diff != 0:  # have to work hard to round to decimal
-        HALF_CENT = 0.005  # e.g. BUY  stop: round   up to decimal
+        HALF_CENT = 0.005  # e.g. BUY  stop: round up to decimal
 
         if round_down:
             HALF_CENT *= -1  # e.g. SELL stop: round down to decimal
         price += HALF_CENT
 
         if price > 0:
             spstr = "%.2f" % price  # now round to 2-place decimal
 
     return spstr
 
 
-# resp_format: xml (default)
-# empty_json: either [] or {}, depends on the caller's semantics
-def get_request_result(req: OAuth1Session.request, empty_json: dict, resp_format: str = "xml") -> dict:
+def get_request_result(req: OAuth1Session.request, resp_format: str = "xml") -> dict:
     LOGGER.debug(req.text)
 
-    if resp_format == "json":
-        if req.text.strip() == "":
-            # otherwise, when ETrade server return empty string, we got this error:
-            # simplejson.errors.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
-            req_output = empty_json  # empty json object
-        else:
-            req_output = req.json()
-    else:
+    # Initialize as empty dict, otherwise, when ETrade server returns an empty string, you get this error:
+    # "simplejson.errors.JSONDecodeError: Expecting value: line 1 column 1 (char 0)"
+    req_output = {}
+
+    assert resp_format in ["xml", "json"]
+
+    if resp_format == "json" and req.text.strip() != "":
+        req_output = req.json()
+    elif resp_format == "xml":
         req_output = xmltodict.parse(req.text)
 
-    if 'Error' in req_output.keys():
-        raise Exception(f'Etrade API Error - Code: {req_output["Error"]["code"]}, Msg: {req_output["Error"]["message"]}')  # noqa: E501
-    else:
-        return req_output
+    if "Error" in req_output.keys():
+        raise Exception(
+            f'Etrade API Error - Code: {req_output["Error"]["code"]}, Msg: {req_output["Error"]["message"]}'
+        )
+
+    return req_output
 
 
 # return Etrade internal option symbol: e.g. "PLTR--220218P00023000" ref:_test_option_symbol()
-def option_symbol(symbol: str, call_put: str, expiry_date: str, strike_price: float) -> str:
+def option_symbol(
+    symbol: str, call_put: str, expiry_date: str, strike_price: float
+) -> str:
     sym = symbol.strip().upper()
     symstr = sym + ("-" * (6 - len(sym)))
 
     ed = dateutil.parser.parse(expiry_date)  # dateutil can handle most date formats
     edstr = ed.strftime("%y%m%d")
-    assert (len(edstr) == 6)
+    assert len(edstr) == 6
 
     sp = "%08d" % (float(strike_price) * 1000)
-    assert (len(sp) == 8)
+    assert len(sp) == 8
 
     opt_sym = symstr + edstr + call_put.strip().upper()[0] + sp
-    assert (len(opt_sym) == 21)
+    assert len(opt_sym) == 21
 
     return opt_sym
 
 
 class OrderException(Exception):
-    """:description: Exception raised when giving bad args to a method not from Etrade calls
-
-    """
+    """:description: Exception raised when giving bad args to a method not from Etrade calls"""
 
     def __init__(self, explanation=None, params=None) -> None:
         super().__init__()
         self.required = params
         self.args = (explanation, params)
 
     def __str__(self) -> str:
         return "Missing required parameters"
 
 
 class ETradeOrder(object):
     """:description: Object to perform Orders
 
-       :param client_key: Client key provided by Etrade
-       :type client_key: str, required
-       :param client_secret: Client secret provided by Etrade
-       :type client_secret: str, required
-       :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_key: str, required
-       :param resource_owner_secret: Resource secret from
-            :class:`pyetrade.authorization.ETradeOAuth`
-       :type resource_owner_secret: str, required
-       :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
-       :type dev: bool, optional
-       :param timeout: Timeout value for OAuth, defaults to 30
-       :type timeout: int, optional
-       :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
-
+    :param client_key: Client key provided by Etrade
+    :type client_key: str, required
+    :param client_secret: Client secret provided by Etrade
+    :type client_secret: str, required
+    :param resource_owner_key: Resource key from :class:`pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_key: str, required
+    :param resource_owner_secret: Resource secret from
+           :class: `pyetrade.authorization.ETradeOAuth`
+    :type resource_owner_secret: str, required
+    :param dev: Defines Sandbox (True) or Live (False) ETrade, defaults to True
+    :type dev: bool, optional
+    :param timeout: Timeout value for OAuth, defaults to 30
+    :type timeout: int, optional
+    :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
     """
 
     def __init__(
         self,
-        client_key,
-        client_secret,
-        resource_owner_key,
-        resource_owner_secret,
-        dev=True,
-        timeout=30,
+        client_key: str,
+        client_secret: str,
+        resource_owner_key: str,
+        resource_owner_secret: str,
+        dev: bool = True,
+        timeout: int = 30,
     ):
-        self.base_url = (
-            r"https://apisb.etrade.com/v1/accounts"
-            if dev
-            else r"https://api.etrade.com/v1/accounts"
-        )
         self.dev_environment = dev
+        self.base_url = f'https://{"apisb" if dev else "api"}.etrade.com/v1/accounts'
         self.timeout = timeout
         self.session = OAuth1Session(
             client_key,
             client_secret,
             resource_owner_key,
             resource_owner_secret,
             signature_type="AUTH_HEADER",
         )
 
-    def list_orders(self, account_id_key: str, resp_format: str = "json", **kwargs) -> dict:
+    def list_orders(
+        self,
+        account_id_key: str,
+        marker: str = None,
+        count: int = 25,
+        status: str = None,
+        from_date: datetime = None,
+        to_date: datetime = None,
+        symbols: list[str] = None,
+        security_type: str = None,
+        transaction_type: str = None,
+        market_session: str = "REGULAR",
+        resp_format: str = "json",
+    ) -> dict:
         """:description: Lists orders for a specific account ID Key
 
-            :param account_id_key: AccountIDKey from :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
-            :type  account_id_key: str, required
-            :param resp_format: Desired Response format, defaults to xml
-            :type  resp_format: str, optional
-            :param kwargs: Parameters for api. Refer to EtradeRef for options
-            :type  kwargs: ``**kwargs``, optional
-            :return: List of orders for an account
-            :rtype: ``xml`` or ``json`` based on ``resp_format``
-            :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param account_id_key: AccountIDKey from :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
+        :type  account_id_key: str, required
+        :param marker: Specifies the desired starting point of the set of items to return (defaults to None)
+        :type  marker: str, optional
+        :param count: Number of transactions to return, defaults to 25 (max 100)
+        :type  count: int, optional
+        :param status: Order status (defaults to None)
+        :type  status: str, optional
+        :status values:
+            * OPEN
+            * EXECUTED
+            * CANCELLED
+            * INDIVIDUAL_FILLS
+            * CANCEL_REQUESTED
+            * EXPIRED
+            * REJECTED
+        :param from_date: The earliest date to include in the date range (history is available for two years).
+                          Both fromDate and toDate should be used together, toDate should be greater than fromDate.
+                          (defaults to None)
+        :type  from_date: datetime obj, optional
+        :param to_date: The latest date to include in the date range (history is available for two years).
+                        Both fromDate and toDate should be used together, toDate should be greater than fromDate.
+                        (defaults to None)
+        :type  to_date: datetime obj, optional
+        :param symbols: The market symbol(s) for the security being bought or sold. (defaults to None, Max 25 symbols)
+        :type  symbols: list[str], optional
+        :param security_type: The security type (defaults to None - Returns all types)
+        :type  security_type: str, optional
+        :security_type values:
+            * EQ
+            * OPTN
+            * MF
+            * MMF
+        :param transaction_type: Type of transaction (defaults to None - Returns all types)
+        :type  transaction_type: str, optional
+        :transaction_type values:
+            * ATNM
+            * BUY
+            * SELL
+            * SELL_SHORT
+            * BUY_TO_COVER
+            * MF_EXCHANGE
+        :param market_session: The market session, defaults to REGULAR
+        :type  market_session: str, optional
+        :market_session values:
+            * REGULAR
+            * EXTENDED
+        :param resp_format: Desired Response format, defaults to json
+        :type  resp_format: str, optional
+        :return: List of orders for an account
+        :rtype: ``xml`` or ``json`` based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        """
+
+        if symbols and len(symbols) >= 26:
+            LOGGER.warning(
+                "list_orders asked for %d requests; only first 25 returned"
+                % len(symbols)
+            )
 
-            :return: List of orders in an account
+        api_url = f"{self.base_url}/{account_id_key}/orders{'.json' if resp_format == 'json' else ''}"
+        LOGGER.debug(api_url)
 
-        """
+        if count >= 101:
+            LOGGER.debug(
+                f"Count {count} is greater than the max allowable value (100), using 100."
+            )
+            count = 100
 
-        api_url = f'{self.base_url}/{account_id_key}/orders'
+        payload = {
+            "marker": marker,
+            "count": count,
+            "status": status,
+            "fromDate": from_date.date().strftime("%m%d%Y") if from_date else None,
+            "toDate": to_date.date().strftime("%m%d%Y") if to_date else None,
+            "symbol": ",".join([sym for sym in symbols[:25]]) if symbols else None,
+            "securityType": security_type,
+            "transactionType": transaction_type,
+            "marketSession": market_session,
+        }
 
-        if resp_format == "json":
-            api_url += ".json"
+        req = self.session.get(api_url, params=payload, timeout=self.timeout)
+        req.raise_for_status()
 
+        LOGGER.debug(req.text)
+
+        return get_request_result(req, resp_format)
+
+    def list_order_details(
+        self, account_id_key: str, order_id: int, resp_format: str = "json"
+    ):
+        """
+        :description: Lists order details of a specific account ID Key and order ID
+
+        :param account_id_key: AccountIDKey from :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
+        :type  account_id_key: str, required
+        :param order_id: Order ID of placed order, order IDs can be retrieved from calling the list_orders() function
+        :type  account_id_key: int, required
+        :param resp_format: Desired Response format, defaults to json
+        :type  resp_format: str, optional
+        :return: List of orders for an account
+        :rtype: ``xml`` or ``json`` based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        """
+
+        api_url = f"{self.base_url}/{account_id_key}/orders/{order_id}{'.json' if resp_format == 'json' else ''}"
         LOGGER.debug(api_url)
-        req = self.session.get(api_url, params=kwargs, timeout=self.timeout)
 
-        return get_request_result(req, {}, resp_format)
+        req = self.session.get(api_url)
+        req.raise_for_status()
 
-    def find_option_orders(self, account_id_key: str, symbol: str, call_put: str, expiry_date: str, strike_price: float) -> list:  # noqa: E501
-        """:description: Lists option orders for a specific account ID Key
+        LOGGER.debug(req.text)
 
-            :param account_id_key: AccountIDKey from :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
-            :type  account_id_key: str, required
-            :param symbol: ticker symbol for options chain
-            :type  symbol: str, required
-            :param call_put: whether the option is a call or put
-            :type  call_put: str, required
-            :param expiry_date: desired expiry of option (ex: 12-05-2021)
-            :type  expiry_date: str, required
-            :param strike_price: strike price of desired option
-            :type  strike_price: str, required
+        return xmltodict.parse(req.text) if resp_format.lower() == "xml" else req.json()
 
-            :return: List of matching option orders in an account
+    def find_option_orders(
+        self,
+        account_id_key: str,
+        symbol: str,
+        call_put: str,
+        expiry_date: str,
+        strike_price: float,
+    ) -> list:
+        """:description: Lists option orders for a specific account ID Key
+
+        :param account_id_key: AccountIDKey from :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
+        :type  account_id_key: str, required
+        :param symbol: ticker symbol for options chain
+        :type  symbol: str, required
+        :param call_put: whether the option is a call or put
+        :type  call_put: str, required
+        :param expiry_date: desired expiry of option (ex: 12-05-2021)
+        :type  expiry_date: str, required
+        :param strike_price: strike price of desired option
+        :type  strike_price: str, required
 
+        :return: List of matching option orders in an account
         """
 
         opt_sym = option_symbol(symbol, call_put, expiry_date, strike_price)
-        orders = self.list_orders(account_id_key, resp_format="json", status="OPEN")  # this call may return empty
+        orders = self.list_orders(
+            account_id_key, resp_format="json", status="OPEN"
+        )  # this call may return empty
 
         results = []
 
         if len(orders) > 0:
             for o in orders["OrdersResponse"]["Order"]:
                 product = o["OrderDetail"][0]["Instrument"][0]["Product"]
 
                 if product["securityType"] == "OPTN":
-                    symbol = product["productId"]["symbol"]  # e.g. "PLTR--220218P00023000"
+                    symbol = product["productId"][
+                        "symbol"
+                    ]  # e.g. "PLTR--220218P00023000"
 
                     if symbol == opt_sym:
                         results.append(o)
         return results
 
     @staticmethod
     def check_order(**kwargs):
         """:description: Check that required params for preview or place order are there and correct
 
-                         (Used internally)
+        (Used internally)
         """
 
         mandatory = [
             "accountIdKey",
             "symbol",
             "orderAction",
             "clientOrderId",
@@ -226,47 +322,52 @@
             raise OrderException
 
         if kwargs["priceType"] == "STOP" and "stopPrice" not in kwargs:
             raise OrderException
         if kwargs["priceType"] == "LIMIT" and "limitPrice" not in kwargs:
             raise OrderException
         if (
-                kwargs["priceType"] == "STOP_LIMIT"
-                and "limitPrice" not in kwargs
-                and "stopPrice" not in kwargs
+            kwargs["priceType"] == "STOP_LIMIT"
+            and "limitPrice" not in kwargs
+            and "stopPrice" not in kwargs
         ):
             raise OrderException
 
-    def build_order_payload(self, order_type: str, **kwargs) -> dict:
+    @staticmethod
+    def build_order_payload(order_type: str, **kwargs) -> dict:
         """:description: Builds the POST payload of a preview or place order
-                         (Used internally)
+                      (Used internally)
 
-           :param order_type: PreviewOrderRequest or PlaceOrderRequest
-           :type  order_type: str, required
-           :securityType: EQ or OPTN
-           :orderAction: for OPTN: BUY_OPEN, SELL_CLOSE
-           :callPut: CALL or PUT
-           :expiryDate: string, e.g. "2022-02-18"
-           :return: Builds Order Payload
-           :rtype: ``xml`` or ``json`` based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param order_type: PreviewOrderRequest or PlaceOrderRequest
+        :type  order_type: str, required
+        :securityType: EQ or OPTN
+        :orderAction: for OPTN: BUY_OPEN, SELL_CLOSE
+        :callPut: CALL or PUT
+        :expiryDate: string, e.g. "2022-02-18"
+        :return: Builds Order Payload
+        :rtype: ``xml`` or ``json`` based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
 
         """
         securityType = kwargs.get("securityType", "EQ")  # EQ by default
         product = {"securityType": securityType, "symbol": kwargs["symbol"]}
 
         if securityType == "OPTN":
-            expiryDate = dateutil.parser.parse(kwargs.pop("expiryDate"))  # dateutil can handle most date formats
-            product.update({
-                "expiryDay": expiryDate.day,
-                "expiryMonth": expiryDate.month,
-                "expiryYear": expiryDate.year,
-                "callPut": kwargs["callPut"],
-                "strikePrice": kwargs["strikePrice"]
-            })
+            expiryDate = dateutil.parser.parse(
+                kwargs.pop("expiryDate")
+            )  # dateutil can handle most date formats
+            product.update(
+                {
+                    "expiryDay": expiryDate.day,
+                    "expiryMonth": expiryDate.month,
+                    "expiryYear": expiryDate.year,
+                    "callPut": kwargs["callPut"],
+                    "strikePrice": kwargs["strikePrice"],
+                }
+            )
 
         instrument = {
             "Product": product,
             "orderAction": kwargs["orderAction"],
             "quantityType": "QUANTITY",
             "quantity": kwargs["quantity"],
         }
@@ -279,15 +380,15 @@
                 kwargs.pop(key, 0)
 
         remove_invalid_price_from_kwargs("stopPrice")
         remove_invalid_price_from_kwargs("limitPrice")
 
         if "stopPrice" in kwargs:
             stopPrice = float(kwargs["stopPrice"])
-            round_down = ("SELL" == kwargs["orderAction"][:4])
+            round_down = "SELL" == kwargs["orderAction"][:4]
             spstr = to_decimal_str(stopPrice, round_down)
 
             order["stopPrice"] = spstr
 
         payload = {
             order_type: {
                 "orderType": securityType,
@@ -297,238 +398,247 @@
         }
 
         if "previewId" in kwargs:
             payload[order_type]["PreviewIds"] = {"previewId": kwargs["previewId"]}
 
         return payload
 
-    def perform_request(self, method, api_url: str, payload: Union[dict, str], resp_format: str = "xml") -> dict:
+    def perform_request(
+        self, method, api_url: str, payload: Union[dict, str], resp_format: str = "xml"
+    ) -> dict:
         """:description: POST or PUT request with json or xml used by preview, place and cancel
 
-           :param method: PUT or POST method
-           :type method: session, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, required
-           :param api_url: API URL
-           :type  api_url: str, required
-           :param payload: Payload
-           :type  payload: json/dict or str xml, required
-           :return: Return request
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param method: PUT or POST method
+        :type method: session, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, required
+        :param api_url: API URL
+        :type  api_url: str, required
+        :param payload: Payload
+        :type  payload: json/dict or str xml, required
+        :return: Return request
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
 
         """
 
         LOGGER.debug(api_url)
         LOGGER.debug("payload: %s", payload)
 
         if resp_format == "json":
             req = method(api_url, json=payload, timeout=self.timeout)
         else:
             headers = {"Content-Type": "application/xml"}
             payload = emit_xml(payload)
             LOGGER.debug("xml payload: %s", payload)
             req = method(api_url, data=payload, headers=headers, timeout=self.timeout)
 
-        return get_request_result(req, {}, resp_format)
+        return get_request_result(req, resp_format)
 
     def preview_equity_order(self, **kwargs) -> dict:
         """API is used to submit an order request for preview before placing it
 
-           :param accountIdKey: AccountIDkey retrieved from :class:`list_accounts`
-           :type  accountIdKey: str, required
-           :param symbol: Market symbol for the security being bought or sold
-           :type  symbol: str, required
-           :param orderAction: Action that the broker is requested to perform
-           :type  orderAction: str, required
-           :orderAction values:
-               * BUY
-               * SELL
-               * BUY_TO_COVER
-               * SELL_SHORT
-           :param previewId: Required only if order was previewed.
-                             Numeric preview ID from preview.
-                             **Note** - Other parameters much match that of preview
-           :type  previewId: long, conditional
-           :param clientOrderId: Reference number generated by developer.
-                                 Used to ensure duplicate order is not submitted.
-                                 Value can be of 20 alphanmeric characters or less
-                                 Must be uniquewithin this account.
-                                 Does not appear in any API responses.
-           :type  clientOrderId: str, required
-           :param priceType: Type of pricing specified in equity order
-           :type  priceType: str, required
-           :priceType values:
-               * MARKET
-               * LIMIT - Requires `limitPrice`
-               * STOP - Requires `stopPrice`
-               * STOP_LIMIT - Requires `limitPrice`
-               * MARKET_ON_CLOSE
-           :param limitPrice: Highest to buy or lowest to sell.
-                              Required if `priceType` is `STOP` or `STOP_LIMIT`
-           :type  limitPrice: double, conditional
-           :param stopPrice: Price to buy or sell if specified in a stop order.
-                             Required if `priceType` is  `STOP` or `STOP_LIMIT`
-           :type  stopPrice: double, conditional
-           :param allOrNone: Specifies if order must be executed all at once.
-                             TRUE triggers `allOrNone`, defaults to FALSE
-           :type  allOrNone: bool, optional
-           :param quantity: Number of shares to buy or sell
-           :type  quantity: int, required
-           :param reserveOrder: If set to TRUE, publicly displays only a limited
-                                number of shares (the reserve quantity), instead
-                                of the entire order, to avoid influencing other
-                                traders. If TRUE, must also specify the
-                                `reserveQuantity`, defaults to FALSE
-           :type  reserveOrder: bool, optional
-           :param reserveQuantity: Number of shares to be publicly displayed if
-                                   this is a reserve order. Required if
-                                   `reserveOrder` is TRUE.
-           :type reserveQuantity: int, conditional
-           :param marketSession: Session to place the equity order
-           :type  marketSession: str, required
-           :marketSession values:
-               * REGULAR
-               * EXTENDED
-           :param orderTerm: Term for which the order is in effect.
-           :type  orderTerm: str, required
-           :orderTerm values:
-               * GOOD_UNTIL_CANCEL
-               * GOOD_FOR_DAY
-               * IMMEDIATE_OR_CANCEL (only for `LIMIT` orders)
-               * FILL_OR_KILL (only for `LIMIT` orders)
-           :param routingDestination: Exchange where the order should be executed.
-           :type  routingDestination: str, optional
-           :routingDestination values:
-               * AUTO (default)
-               * ARCA
-               * NSDQ
-               * NYSE
-           :param estimatedCommission: Cost billed to the user to preform requested action
-           :type  estimatedCommission: double
-           :param estimatedTotalAmount: Cost including commission
-           :type  estimatedTotalAmount: double
-           :param messageList: Container for messages describing the result of the action
-           :type  messageList: dict
-           :param msgDesc: Text of the result message, indicating order status, success
-                           or failure, additional requirements that must be met before
-                           placing the order, etc. Applications typically display this
-                           message to the user, which may result in further user action
-           :type  msgDesc: str
-           :param msgCode: Standard numeric code of the result message. Refer to
-                           the Error Messages documentation for examples. May optionally
-                           be displayed to the user, but is primarily intended for
-                           internal use.
-           :type  msgCode: int
-           :param orderNum: Numeric ID for this order in the E*TRADE system
-           :type  orderNum: int
-           :param orderTime: The epoch time the order was submitted.
-           :type  orderTime: long
-           :param symbolDesc: Text description of the security
-           :type  symbolDesc: str
-           :param symbol: The market symbol for the underlier
-           :type  symbol: str
-           :return: Confirmation of the Preview Equity Order
-           :rtype: ``xml`` or ``json`` based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param accountIdKey: AccountIDkey retrieved from :class:`list_accounts`
+        :type  accountIdKey: str, required
+        :param symbol: Market symbol for the security being bought or sold
+        :type  symbol: str, required
+        :param orderAction: Action that the broker is requested to perform
+        :type  orderAction: str, required
+        :orderAction values:
+            * BUY
+            * SELL
+            * BUY_TO_COVER
+            * SELL_SHORT
+        :param previewId: Required only if order was previewed.
+                          Numeric preview ID from preview.
+                          **Note** - Other parameters much match that of preview
+        :type  previewId: long, conditional
+        :param clientOrderId: Reference number generated by developer.
+                              Used to ensure duplicate order is not submitted.
+                              Value can be of 20 alphanmeric characters or less
+                              Must be uniquewithin this account.
+                              Does not appear in any API responses.
+        :type  clientOrderId: str, required
+        :param priceType: Type of pricing specified in equity order
+        :type  priceType: str, required
+        :priceType values:
+            * MARKET
+            * LIMIT - Requires `limitPrice`
+            * STOP - Requires `stopPrice`
+            * STOP_LIMIT - Requires `limitPrice`
+            * MARKET_ON_CLOSE
+        :param limitPrice: Highest to buy or lowest to sell.
+                           Required if `priceType` is `STOP` or `STOP_LIMIT`
+        :type  limitPrice: double, conditional
+        :param stopPrice: Price to buy or sell if specified in a stop order.
+                          Required if `priceType` is  `STOP` or `STOP_LIMIT`
+        :type  stopPrice: double, conditional
+        :param allOrNone: Specifies if order must be executed all at once.
+                          TRUE triggers `allOrNone`, defaults to FALSE
+        :type  allOrNone: bool, optional
+        :param quantity: Number of shares to buy or sell
+        :type  quantity: int, required
+        :param reserveOrder: If set to TRUE, publicly displays only a limited
+                             number of shares (the reserve quantity), instead
+                             of the entire order, to avoid influencing other
+                             traders. If TRUE, must also specify the
+                             `reserveQuantity`, defaults to FALSE
+        :type  reserveOrder: bool, optional
+        :param reserveQuantity: Number of shares to be publicly displayed if
+                                this is a reserve order. Required if
+                                `reserveOrder` is TRUE.
+        :type reserveQuantity: int, conditional
+        :param marketSession: Session to place the equity order
+        :type  marketSession: str, required
+        :marketSession values:
+            * REGULAR
+            * EXTENDED
+        :param orderTerm: Term for which the order is in effect.
+        :type  orderTerm: str, required
+        :orderTerm values:
+            * GOOD_UNTIL_CANCEL
+            * GOOD_FOR_DAY
+            * IMMEDIATE_OR_CANCEL (only for `LIMIT` orders)
+            * FILL_OR_KILL (only for `LIMIT` orders)
+        :param routingDestination: Exchange where the order should be executed.
+        :type  routingDestination: str, optional
+        :routingDestination values:
+            * AUTO (default)
+            * ARCA
+            * NSDQ
+            * NYSE
+        :param estimatedCommission: Cost billed to the user to preform requested action
+        :type  estimatedCommission: double
+        :param estimatedTotalAmount: Cost including commission
+        :type  estimatedTotalAmount: double
+        :param messageList: Container for messages describing the result of the action
+        :type  messageList: dict
+        :param msgDesc: Text of the result message, indicating order status, success
+                        or failure, additional requirements that must be met before
+                        placing the order, etc. Applications typically display this
+                        message to the user, which may result in further user action
+        :type  msgDesc: str
+        :param msgCode: Standard numeric code of the result message. Refer to
+                        the Error Messages documentation for examples. May optionally
+                        be displayed to the user, but is primarily intended for
+                        internal use.
+        :type  msgCode: int
+        :param orderNum: Numeric ID for this order in the E*TRADE system
+        :type  orderNum: int
+        :param orderTime: The epoch time the order was submitted.
+        :type  orderTime: long
+        :param symbolDesc: Text description of the security
+        :type  symbolDesc: str
+        :param symbol: The market symbol for the underlier
+        :type  symbol: str
+        :return: Confirmation of the Preview Equity Order
+        :rtype: ``xml`` or ``json`` based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
 
         """
         LOGGER.debug(kwargs)
 
         # Test required values
         self.check_order(**kwargs)
 
         api_url = f'{self.base_url}/{kwargs["accountIdKey"]}/orders/preview'
 
         # payload creation
         payload = self.build_order_payload("PreviewOrderRequest", **kwargs)
 
         return self.perform_request(self.session.post, api_url, payload, "xml")
 
-    def change_preview_equity_order(self, account_id_key: str, order_id: str, **kwargs):
+    def change_preview_equity_order(
+        self, account_id_key: str, order_id: str, **kwargs
+    ) -> dict:
         """:description: Same as :class:`preview_equity_order` with orderId
-           :param order_id: order_id to modify, refer :class:`list_orders`
-           :type  order_id: str, required
-           :param account_id_key: account_id_key retrieved from :class:`list_accounts`
-           :type  account_id_key: str, required
-           :return: Previews Changed order with orderId for account with account_id_key
-           :rtype: dict/json
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param order_id: order_id to modify, refer :class:`list_orders`
+        :type  order_id: str, required
+        :param account_id_key: account_id_key retrieved from :class:`list_accounts`
+        :type  account_id_key: str, required
+        :return: Previews Changed order with orderId for account with account_id_key
+        :rtype: dict/json
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
 
         """
 
         LOGGER.debug(kwargs)
 
         # Test required values
         self.check_order(**kwargs)
 
-        api_url = f'{self.base_url}/{account_id_key}/orders/{order_id}/change/preview'
+        api_url = f"{self.base_url}/{account_id_key}/orders/{order_id}/change/preview"
 
         # payload creation
         payload = self.build_order_payload("PreviewOrderRequest", **kwargs)
 
         return self.perform_request(self.session.put, api_url, payload, "xml")
 
     def place_option_order(self, **kwargs) -> dict:
         """:description: Places Option Order, only single leg CALL or PUT is supported for now
-           :return: Returns confirmation of the equity order
+        :return: Returns confirmation of the equity order
         """
         kwargs["securityType"] = "OPTN"
 
         return self.place_equity_order(**kwargs)
 
     def place_equity_order(self, **kwargs) -> dict:
         """:description: Places Equity Order
 
-           :param kwargs: Parameters for api, refer :class:`preview_equity_order`
-           :type  kwargs: ``**kwargs``, required
-           :return: Returns confirmation of the equity order
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param kwargs: Parameters for api, refer :class:`preview_equity_order`
+        :type  kwargs: ``**kwargs``, required
+        :return: Returns confirmation of the equity order
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
         """
 
         LOGGER.debug(kwargs)
 
         # Test required values
         self.check_order(**kwargs)
 
         if "previewId" not in kwargs:
             LOGGER.debug(
                 "No previewId given, previewing before placing order "
                 "because of an Etrade bug as of 1/1/2019"
             )
+
             preview = self.preview_equity_order(**kwargs)
-            kwargs["previewId"] = preview["PreviewOrderResponse"]["PreviewIds"]["previewId"]
+            kwargs["previewId"] = preview["PreviewOrderResponse"]["PreviewIds"][
+                "previewId"
+            ]
 
-            LOGGER.debug("Got a successful preview with previewId: %s", kwargs["previewId"])
+            LOGGER.debug(
+                "Got a successful preview with previewId: %s", kwargs["previewId"]
+            )
 
         api_url = f'{self.base_url}/{kwargs["accountIdKey"]}/orders/place'
 
         # payload creation
         payload = self.build_order_payload("PlaceOrderRequest", **kwargs)
 
         return self.perform_request(self.session.post, api_url, payload, "xml")
 
     def place_changed_option_order(self, **kwargs) -> dict:
         """:description: Places Option Order, only single leg CALL or PUT is supported for now
-           :return: Returns confirmation of the equity order
+        :return: Returns confirmation of the equity order
         """
         kwargs["securityType"] = "OPTN"
 
         return self.place_changed_equity_order(**kwargs)
 
     def place_changed_equity_order(self, **kwargs) -> dict:
         """:description: Places changes to equity orders
-            NOTE: the ETrade server will actually cancel the old orderId, and create a new orderId
+         NOTE: the ETrade server will actually cancel the old orderId, and create a new orderId
 
-           :param kwargs: Parameters for api, refer :class:`change_preview_equity_order`
-           :type  kwargs: ``**kwargs``, required
-           :return: Returns confirmation similar to :class:`preview_equity_order`
-           :rtype: xml or json based on ``resp_format``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param kwargs: Parameters for api, refer :class:`change_preview_equity_order`
+        :type  kwargs: ``**kwargs``, required
+        :return: Returns confirmation similar to :class:`preview_equity_order`
+        :rtype: xml or json based on ``resp_format``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
 
         """
 
         LOGGER.debug(kwargs)
 
         # Test required values
         self.check_order(**kwargs)
@@ -540,36 +650,42 @@
             )
             preview = self.preview_equity_order(**kwargs)
 
             if "Error" in preview:
                 LOGGER.error(preview)
                 raise Exception("Please check your order!")
 
-            kwargs["previewId"] = preview["PreviewOrderResponse"]["PreviewIds"]["previewId"]
-            LOGGER.debug("Got a successful preview with previewId: %s", kwargs["previewId"])
+            kwargs["previewId"] = preview["PreviewOrderResponse"]["PreviewIds"][
+                "previewId"
+            ]
+            LOGGER.debug(
+                "Got a successful preview with previewId: %s", kwargs["previewId"]
+            )
 
         api_url = f'{self.base_url}/{kwargs["accountIdKey"]}/orders/{kwargs["orderId"]}/change/place'
 
         # payload creation
         payload = self.build_order_payload("PlaceOrderRequest", **kwargs)
 
         return self.perform_request(self.session.put, api_url, payload, "xml")
 
-    def cancel_order(self, account_id_key: str, order_num: int, resp_format: str = "xml") -> dict:
+    def cancel_order(
+        self, account_id_key: str, order_num: int, resp_format: str = "xml"
+    ) -> dict:
         """:description: Cancels a specific order for a given account
 
-           :param account_id_key: AccountIDkey retrieved from
-                              :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
-           :type  account_id_key: str, required
-           :param order_num: Numeric id for this order listed in :class:`list_orders`
-           :type  order_num: int, required
-           :param resp_format: Desired Response format, defaults to xml
-           :type  resp_format: str, required
-           :return: Confirmation of cancellation
-           :rtype: ``dict/json``
-           :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
+        :param account_id_key: AccountIDkey retrieved from
+                           :class:`pyetrade.accounts.ETradeAccounts.list_accounts`
+        :type  account_id_key: str, required
+        :param order_num: Numeric id for this order listed in :class:`list_orders`
+        :type  order_num: int, required
+        :param resp_format: Desired Response format, defaults to xml
+        :type  resp_format: str, required
+        :return: Confirmation of cancellation
+        :rtype: ``dict/json``
+        :EtradeRef: https://apisb.etrade.com/docs/api/order/api-order-v1.html
         """
 
-        api_url = f'{self.base_url}/{account_id_key}/orders/cancel'
+        api_url = f"{self.base_url}/{account_id_key}/orders/cancel"
         payload = {"CancelOrderRequest": {"orderId": order_num}}
 
         return self.perform_request(self.session.put, api_url, payload, resp_format)
```

### Comparing `pyetrade-2.0.1/setup.py` & `pyetrade-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
-
-from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "2.0.1"
+from setuptools import find_packages
+from setuptools import setup
+
+__version__ = "2.1.0"
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # requirements
@@ -35,14 +36,14 @@
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

### Comparing `pyetrade-2.0.1/tests/test_accounts.py` & `pyetrade-2.1.0/tests/test_accounts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python3
 """pyetrade authorization unit tests
    TODO:
-       * Test request error"""
-
+       * Test request error
+"""
 import unittest
+from unittest.mock import MagicMock
 from unittest.mock import patch
+
 from pyetrade import accounts
 
 
 class TestETradeAccounts(unittest.TestCase):
     """TestEtradeAccounts Unit Test"""
 
-    # Mock out OAuth1Session
     @patch("pyetrade.accounts.OAuth1Session")
     def test_list_accounts(self, MockOAuthSession):
         """test_list_accounts(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock object for OAuth1Sessions"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions"""
         # Set Mock returns
         MockOAuthSession().get().json.return_value = "{'account': 'abc123'}"
         MockOAuthSession().get().text = r"<xml> returns </xml>"
         account = accounts.ETradeAccounts("abc123", "xyz123", "abctoken", "xyzsecret")
         # Test Dev JSON
         self.assertEqual(
             account.list_accounts(resp_format="json"), "{'account': 'abc123'}"
@@ -47,21 +48,20 @@
             ("https://api.etrade.com/v1/accounts/list.json")
         )
         # Test XML
         result = account.list_accounts(resp_format="xml")
         self.assertTrue(isinstance(result, dict))
         self.assertTrue(MockOAuthSession().get.called)
 
-    # Mock out OAuth1Session
     @patch("pyetrade.accounts.OAuth1Session")
     def test_get_account_balance(self, MockOAuthSession):
         """test_get_account_balance(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock object for OAuth1Sessions"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions"""
         # Set Mock returns
         MockOAuthSession().get().json.return_value = {"account": "abc123"}
         MockOAuthSession().get().text = r"<xml> returns </xml>"
         account = accounts.ETradeAccounts("abc123", "xyz123", "abctoken", "xyzsecret")
         # Test Dev XML
         result = account.get_account_balance("12345abcd", resp_format="xml")
         self.assertTrue(isinstance(result, dict))
@@ -94,174 +94,277 @@
             params={"instType": "BROKERAGE", "realTimeNAV": True},
         )
 
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
         # Test API URL
-        result = account.get_account_balance("12345abcd", account_type="TRUST", resp_format="json")
+        result = account.get_account_balance(
+            "12345abcd", account_type="TRUST", resp_format="json"
+        )
         self.assertTrue(isinstance(result, dict))
 
         MockOAuthSession().get.assert_called_with(
             "https://api.etrade.com/v1/accounts/12345abcd/balance.json",
-            params={"realTimeNAV": True, "instType": "BROKERAGE", "accountType": "TRUST"},
+            params={
+                "realTimeNAV": True,
+                "instType": "BROKERAGE",
+                "accountType": "TRUST",
+            },
         )
 
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
-    # Mock out OAuth1Session
     @patch("pyetrade.accounts.OAuth1Session")
     def test_get_account_portfolio(self, MockOAuthSession):
         """test_get_account_positions(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock object for OAuth1Sessions"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions"""
+
         # Set Mock returns
         MockOAuthSession().get().json.return_value = {"account": "abc123"}
         MockOAuthSession().get().text = r"<xml> returns </xml>"
 
         account = accounts.ETradeAccounts("abc123", "xyz123", "abctoken", "xyzsecret")
         default_params = {
-            'count': 50,
-            'sortBy': None,
-            'sortOrder': 'DESC',
-            'pageNumber': None,
-            'marketSession': 'REGULAR',
-            'totalsRequired': False,
-            'lotsRequired': False,
-            'view': 'QUICK'
+            "count": 50,
+            "sortBy": None,
+            "sortOrder": "DESC",
+            "pageNumber": None,
+            "marketSession": "REGULAR",
+            "totalsRequired": False,
+            "lotsRequired": False,
+            "view": "QUICK",
         }
 
         # Test Dev
         result = account.get_account_portfolio("12345abcd")
         self.assertTrue(isinstance(result, dict))
 
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://apisb.etrade.com/v1/accounts/12345abcd/portfolio", params=default_params
+            "https://apisb.etrade.com/v1/accounts/12345abcd/portfolio",
+            params=default_params,
         )
         result = account.get_account_portfolio("12345abcd", resp_format="json")
         self.assertTrue(isinstance(result, dict))
 
         # Test Prod
         account = accounts.ETradeAccounts(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
         result = account.get_account_portfolio("12345abcd")
         self.assertTrue(isinstance(result, dict))
 
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://api.etrade.com/v1/accounts/12345abcd/portfolio", params=default_params
+            "https://api.etrade.com/v1/accounts/12345abcd/portfolio",
+            params=default_params,
         )
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
         result = account.get_account_portfolio("12345abcd", resp_format="xml")
         self.assertTrue(isinstance(result, dict))
 
-    # Mock out OAuth1Session
+    @patch("pyetrade.accounts.OAuth1Session")
+    def test_get_portfolio_position_lot(self, MockOAuthSession):
+        """test_get_portfolio_position_lot(MockOAuthSession) -> None
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions"""
+
+        # Set Mock returns
+        MockOAuthSession().get().json.return_value = {
+            "PositionLotsResponse": {
+                "shortType": 1,
+                "PositionLot": [
+                    {
+                        "positionId": 297825015900,
+                        "positionLotId": 1855385101103,
+                        "price": 227.7,
+                        "termCode": 1,
+                        "daysGain": 5.0,
+                        "daysGainPct": 1.4802,
+                        "marketValue": 342.78,
+                        "totalCost": 227.7,
+                        "totalCostForGainPct": 50.5401,
+                        "totalGain": 115.0799,
+                        "lotSourceCode": 1,
+                        "originalQty": 1,
+                        "remainingQty": 1,
+                        "availableQty": 0,
+                        "orderNo": 18,
+                        "legNo": 1,
+                        "acquiredDate": 1674622900000,
+                        "locationCode": 1,
+                        "exchangeRate": 1.0,
+                        "settlementCurrency": "USD",
+                        "paymentCurrency": "USD",
+                        "adjPrice": 0.0,
+                        "commPerShare": 0.0,
+                        "feesPerShare": 0.0,
+                        "shortType": 1,
+                    }
+                ],
+            }
+        }
+
+        MockOAuthSession().get().text = r"<xml> returns </xml>"
+
+        account = accounts.ETradeAccounts("abc123", "xyz123", "abctoken", "xyzsecret")
+
+        account.get_account_portfolio = MagicMock(
+            return_value={
+                "PortfolioResponse": {
+                    "AccountPortfolio": [
+                        {
+                            "Position": [
+                                {"positionId": "1", "Product": {"symbol": "AAPL"}}
+                            ]
+                        }
+                    ]
+                }
+            }
+        )
+
+        result = account.get_portfolio_position_lot("AAPL", "account_id_key", "xml")
+        self.assertTrue(isinstance(result, dict))
+
+        # Check for when the symbol doesn't exist
+        with self.assertRaises(KeyError):
+            account.get_portfolio_position_lot("GOOG", "account_id_key", "xml")
+
     @patch("pyetrade.accounts.OAuth1Session")
     def test_list_transactions(self, MockOAuthSession):
         """test_list_transactions(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock object for OAuth1Sessions"""
-        # Set Mock returns
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions
+        """
+
         MockOAuthSession().get().json.return_value = "{'transaction': 'abc123'}"
         MockOAuthSession().get().text = r"<xml> returns </xml>"
 
         account = accounts.ETradeAccounts("abc123", "xyz123", "abctoken", "xyzsecret")
-        default_params = {'startDate': None, 'endDate': None, 'sortOrder': 'DESC', 'marker': None, 'count': 50}
+        default_params = {
+            "startDate": None,
+            "endDate": None,
+            "sortOrder": "DESC",
+            "marker": None,
+            "count": 50,
+        }
 
         # Test Dev JSON
         self.assertEqual(
-            account.list_transactions('12345abcd', resp_format="json"), "{'transaction': 'abc123'}"
-
+            account.list_transactions("12345abcd", resp_format="json"),
+            "{'transaction': 'abc123'}",
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions.json", params=default_params,
+            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions.json",
+            params=default_params,
         )
         # Test Dev XML
         self.assertEqual(
-            dict(account.list_transactions('12345abcd', resp_format="xml")), {"xml": "returns"},
+            dict(account.list_transactions("12345abcd", resp_format="xml")),
+            {"xml": "returns"},
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions", params=default_params,
+            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions",
+            params=default_params,
         )
         account = accounts.ETradeAccounts(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
         # Test Prod JSON
         self.assertEqual(
-            account.list_transactions('12345abcd', resp_format="json"), "{'transaction': 'abc123'}",
+            account.list_transactions("12345abcd", resp_format="json"),
+            "{'transaction': 'abc123'}",
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://api.etrade.com/v1/accounts/12345abcd/transactions.json", params=default_params,
+            "https://api.etrade.com/v1/accounts/12345abcd/transactions.json",
+            params=default_params,
         )
         # Test Prod XML
         self.assertEqual(
-            dict(account.list_transactions('12345abcd', resp_format="xml")), {"xml": "returns"},
+            dict(account.list_transactions("12345abcd", resp_format="xml")),
+            {"xml": "returns"},
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://api.etrade.com/v1/accounts/12345abcd/transactions", params=default_params
+            "https://api.etrade.com/v1/accounts/12345abcd/transactions",
+            params=default_params,
         )
+
+        MockOAuthSession().get().text = ""
+
+        # Test Dev JSON
+        self.assertEqual(account.list_transactions("12345abcd", resp_format="json"), {})
+
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
-    # Mock out OAuth1Session
     @patch("pyetrade.accounts.OAuth1Session")
     def test_list_transaction_details(self, MockOAuthSession):
         """test_get_transaction_details(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock object for OAuth1Sessions"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock object for OAuth1Sessions
+        """
         # Set Mock returns
         MockOAuthSession().get().json.return_value = "{'transaction': 'abc123'}"
         MockOAuthSession().get().text = r"<xml> returns </xml>"
         account = accounts.ETradeAccounts(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=True
         )
         # Test Dev JSON
         self.assertEqual(
-            account.list_transaction_details('12345abcd', 67890, resp_format="json"),
+            account.list_transaction_details("12345abcd", 67890, resp_format="json"),
             "{'transaction': 'abc123'}",
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://apisb.etrade.com/v1/accounts" "/12345abcd/transactions.json/67890", params={},
+            "https://apisb.etrade.com/v1/accounts" "/12345abcd/transactions/67890.json",
+            params={"storeId": None},
         )
         # Test Dev XML
         self.assertEqual(
-            dict(account.list_transaction_details('12345abcd', 67890, resp_format="xml")),
+            dict(
+                account.list_transaction_details("12345abcd", 67890, resp_format="xml")
+            ),
             {"xml": "returns"},
         )
         MockOAuthSession().get.assert_called_with(
-            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions/67890", params={},
+            "https://apisb.etrade.com/v1/accounts/12345abcd/transactions/67890",
+            params={"storeId": None},
         )
         account = accounts.ETradeAccounts(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
         # Test Prod JSON
         self.assertEqual(
-            account.list_transaction_details('12345abcd', 67890, resp_format="json"),
+            account.list_transaction_details("12345abcd", 67890, resp_format="json"),
             "{'transaction': 'abc123'}",
         )
         # Test API URL
         MockOAuthSession().get.assert_called_with(
-            "https://api.etrade.com/v1/accounts/12345abcd/transactions.json/67890", params={},
+            "https://api.etrade.com/v1/accounts/12345abcd/transactions/67890.json",
+            params={"storeId": None},
         )
         # Test Prod XML
         self.assertEqual(
-            dict(account.list_transaction_details('12345abcd', 67890, resp_format="xml")),
+            dict(
+                account.list_transaction_details("12345abcd", 67890, resp_format="xml")
+            ),
             {"xml": "returns"},
         )
         MockOAuthSession().get.assert_called_with(
-            "https://api.etrade.com/v1/accounts/12345abcd/transactions/67890", params={},
+            "https://api.etrade.com/v1/accounts/12345abcd/transactions/67890",
+            params={"storeId": None},
         )
 
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
```

### Comparing `pyetrade-2.0.1/tests/test_alerts.py` & `pyetrade-2.1.0/tests/test_alerts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,113 @@
 from pyetrade import alerts
 
 
 # Mock out OAuth1Session
 def test_list_alerts(mocker):
     """test_list_alerts(MockOAuthSession) -> None
-       param: MockOAuthSession
-       type: mock.MagicMock
-       description: MagicMock object for OAuth1Sessions"""
+    param: MockOAuthSession
+    type: mock.MagicMock
+    description: MagicMock object for OAuth1Sessions"""
     MockOAuthSession = mocker.patch("pyetrade.alerts.OAuth1Session")
     # Set Mock returns
     MockOAuthSession().get().json.return_value = "{'alert': 'abc123'}"
     MockOAuthSession().get().text = r"<xml> returns </xml>"
 
     alert = alerts.ETradeAlerts("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
-    default_params = {'count': True, 'direction': 'DESC'}
+    default_params = {"count": 25, "direction": "DESC"}
 
     # Test Dev JSON
     assert alert.list_alerts(resp_format="json") == "{'alert': 'abc123'}"
     # Test API URL
-    MockOAuthSession().get.assert_called_with("https://apisb.etrade.com/v1/user/alerts.json", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://apisb.etrade.com/v1/user/alerts.json", params=default_params
+    )
 
     # Test Dev XML
     assert dict(alert.list_alerts(resp_format="xml")) == {"xml": "returns"}
-    MockOAuthSession().get.assert_called_with("https://apisb.etrade.com/v1/user/alerts", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://apisb.etrade.com/v1/user/alerts", params=default_params
+    )
     alert = alerts.ETradeAlerts("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
 
     # Test Prod JSON
     assert alert.list_alerts(resp_format="json") == "{'alert': 'abc123'}"
     # Test API URL
-    MockOAuthSession().get.assert_called_with("https://api.etrade.com/v1/user/alerts.json", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://api.etrade.com/v1/user/alerts.json", params=default_params
+    )
 
     # test Prod XML
     assert alert.list_alerts(resp_format="xml") == {"xml": "returns"}
 
-    MockOAuthSession().get.assert_called_with("https://api.etrade.com/v1/user/alerts", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://api.etrade.com/v1/user/alerts", params=default_params
+    )
+
+    assert alert.list_alerts(count=301, resp_format="json") == "{'alert': 'abc123'}"
+    MockOAuthSession().get.assert_called_with(
+        "https://api.etrade.com/v1/user/alerts.json",
+        params={"count": 300, "direction": "DESC"},
+    )
+
     assert MockOAuthSession().get().json.called
     assert MockOAuthSession().get.called
 
 
 # Mock out OAuth1Session
 def test_list_alert_details(mocker):
     """test_list_alerts(MockOAuthSession) -> None
-       param: MockOAuthSession
-       type: mock.MagicMock
-       description: MagicMock object for OAuth1Sessions"""
+    param: MockOAuthSession
+    type: mock.MagicMock
+    description: MagicMock object for OAuth1Sessions"""
     MockOAuthSession = mocker.patch("pyetrade.alerts.OAuth1Session")
     # Set Mock returns
     MockOAuthSession().get().json.return_value = "{'alert': 'abc123'}"
     MockOAuthSession().get().text = r"<xml> returns </xml>"
 
     alert = alerts.ETradeAlerts("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
-    default_params = {'htmlTags': False}
+    default_params = {"htmlTags": False}
 
     # Test Dev JSON
     assert alert.list_alert_details(1234, resp_format="json") == "{'alert': 'abc123'}"
     # Test API URL
-    MockOAuthSession().get.assert_called_with("https://apisb.etrade.com/v1/user/alerts.json/1234", params=default_params)  # noqa: E501
+    MockOAuthSession().get.assert_called_with(
+        "https://apisb.etrade.com/v1/user/alerts.json/1234", params=default_params
+    )  # noqa: E501
 
     # Test Dev XML
     assert dict(alert.list_alert_details(1234, resp_format="xml")) == {"xml": "returns"}
-    MockOAuthSession().get.assert_called_with("https://apisb.etrade.com/v1/user/alerts/1234", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://apisb.etrade.com/v1/user/alerts/1234", params=default_params
+    )
     assert dict(alert.list_alert_details(1234, resp_format="xml")) == {"xml": "returns"}
 
     alert = alerts.ETradeAlerts("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
     # Test Prod JSON
     assert alert.list_alert_details(1234, resp_format="json") == "{'alert': 'abc123'}"
 
     # Test API URL
-    MockOAuthSession().get.assert_called_with("https://api.etrade.com/v1/user/alerts.json/1234", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://api.etrade.com/v1/user/alerts.json/1234", params=default_params
+    )
     assert dict(alert.list_alert_details(1234, resp_format="xml")) == {"xml": "returns"}
 
-    MockOAuthSession().get.assert_called_with("https://api.etrade.com/v1/user/alerts/1234", params=default_params)
+    MockOAuthSession().get.assert_called_with(
+        "https://api.etrade.com/v1/user/alerts/1234", params=default_params
+    )
     assert MockOAuthSession().get().json.called
     assert MockOAuthSession().get.called
 
 
 # Mock out OAuth1Session
 def test_delete_alert(mocker):
     """test_list_alerts(MockOAuthSession) -> None
-       param: MockOAuthSession
-       type: mock.MagicMock
-       description: MagicMock object for OAuth1Sessions"""
+    param: MockOAuthSession
+    type: mock.MagicMock
+    description: MagicMock object for OAuth1Sessions"""
     MockOAuthSession = mocker.patch("pyetrade.alerts.OAuth1Session")
     # Set Mock returns
     MockOAuthSession().delete().json.return_value = "{'alert': 'abc123'}"
     MockOAuthSession().delete().text = r"<xml> returns </xml>"
     alert = alerts.ETradeAlerts("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
     # Test Dev JSON
     assert alert.delete_alert(1234, resp_format="json") == "{'alert': 'abc123'}"
```

### Comparing `pyetrade-2.0.1/tests/test_authorization.py` & `pyetrade-2.1.0/tests/test_authorization.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """pyetrade authorization unit tests
    TODO:
     * add more mock tests for revoke
     * add more mock tests for renew"""
-
 import unittest
 from unittest.mock import patch
+
 from pyetrade import authorization
 
 
 class TestETradeAuthorization(unittest.TestCase):
     """TestEtradeAuthorization Unit Test"""
 
     # Mock out OAuth1Session
```

### Comparing `pyetrade-2.0.1/tests/test_market.py` & `pyetrade-2.1.0/tests/test_market.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,62 +2,82 @@
 """pyetrade market unit tests
    TODO:
     * pyetrade.market fixture
 """
 import datetime as dt
 import unittest
 from unittest.mock import patch
+
 from pyetrade import market
 
 
 # Mock out OAuth1Session
 class TestETradeMarket(unittest.TestCase):
     """TestEtradeAccounts Unit Test"""
 
+    def test__str__(self):
+        """test__str__()
+        type: mock.MagicMock
+        """
+
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+
+        # Test __str__ response
+        self.assertEqual(
+            "Use development environment: False\nBase URL: https://api.etrade.com/v1/market/",
+            mark.__str__(),
+        )
+
     @patch("pyetrade.market.OAuth1Session")
     def test_look_up_product(self, MockOAuthSession):
         """test_look_up_product(MockOAuthSession)
-            param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session
-
-           3 tests based on resp_format = (None,'xml')
-           test exception raised when resp_format is something
-           different from two choices
+         param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session
+
+        3 tests based on resp_format = (None,'xml')
+        test exception raised when resp_format is something
+        different from two choices
         """
 
         response = {"symbol": "MMM", "description": "3M CO COM", "type": "EQUITY"}
         XML_response = r"""<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
                             <LookupResponse>
                                 <Data><symbol>MMM</symbol>
                                 <description>3M CO COM</description>
                                 <type>EQUITY</type></Data>
                             </LookupResponse>"""
         # Set Mock returns for resp_format=xml
         MockOAuthSession().get().text = XML_response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
         # Test Get Quote returning python dict
         resp = mark.look_up_product("mmm")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Set Mock returns for resp_format=json
         MockOAuthSession().get().json.return_value = response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
         # Test Get Quote returning python dict
         resp = mark.look_up_product("mmm", resp_format="json")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
     @patch("pyetrade.market.OAuth1Session")
     def test_get_quote(self, MockOAuthSession):
         """test_get_quote(MockOAuthSession)
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session
         """
 
         response = {
             "securityType": "EQ",
             "symbol": "MMM",
             "dateTimeUTC": 1546545180,
             "adjustedFlag": "false",
@@ -79,39 +99,46 @@
                             <symbol>MMM</symbol></Product>
                             </QuoteData></QuoteResponse>
                          """
         # Set Mock returns for resp_format=None
         MockOAuthSession().get().text = XML_response
         MockOAuthSession().get().json.return_value = response
 
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
 
         # Test XML return
         resp = mark.get_quote(["MMM"])
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Test JSON return
         resp = mark.get_quote(["MMM"], resp_format="json")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Test list of symbols greater than 25
-        resp = mark.get_quote(["MMM"]*26, resp_format="json")
+        resp = mark.get_quote(["MMM"] * 26, resp_format="json")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Test list of symbols greater than 25
         resp = mark.get_quote(["MMM"] * 26, resp_format="json")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Test detail_flag, requireEarningsDate, skipMiniOptionsCheck
-        resp = mark.get_quote(["MMM"], detail_flag="ALL", require_earnings_date=True,
-                              skip_mini_options_check=True, resp_format="json")
+        resp = mark.get_quote(
+            ["MMM"],
+            detail_flag="ALL",
+            require_earnings_date=True,
+            skip_mini_options_check=True,
+            resp_format="json",
+        )
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         MockOAuthSession().get.assert_called_with(
             "https://api.etrade.com/v1/market/quote/MMM.json?detailflag=ALL&requireEarningsDate=true&skipMiniOptionsCheck=True"  # noqa: E501
         )
         self.assertTrue(MockOAuthSession().get().json.called)
@@ -119,54 +146,89 @@
 
         # test the assertion failure of detail_flag, requireEarningsDate,
         # skipMiniOptionsCheck
 
     @patch("pyetrade.market.OAuth1Session")
     def test_get_option_chains(self, MockOAuthSession):
         """test_get_optionexpiredate(MockOAuthSession)
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session
         """
 
-        response = {"timeStamp": 1546546266, "bid": 41.55, "OptionGreeks": {"iv": 0.6716}}
+        response = {
+            "timeStamp": 1546546266,
+            "bid": 41.55,
+            "OptionGreeks": {"iv": 0.6716},
+        }
         XML_response = r"""<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
         <OptionChainResponse><OptionPair><Call>
                            <timeStamp>1546546266</timeStamp><bid>41.55</bid>
                            <OptionGreeks><iv>0.435700</iv></OptionGreeks></Call>
                            </OptionPair></OptionChainResponse>
                         """
 
         # Set Mock returns for resp_format=xml
         MockOAuthSession().get().text = XML_response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
-        resp = mark.get_option_chains("AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml")
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+        resp = mark.get_option_chains(
+            "AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml"
+        )
+        assert isinstance(resp, dict)
+        assert MockOAuthSession().get.called
+
+        # Set Mock returns for resp_format=xml and expiry_date=None
+        MockOAuthSession().get().text = XML_response
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+        resp = mark.get_option_chains("AAPL", expiry_date=None, resp_format="xml")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Set Mock returns for resp_format=xml and dev=True
         MockOAuthSession().get().text = XML_response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
-        resp = mark.get_option_chains("AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml")
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=True
+        )
+        resp = mark.get_option_chains(
+            "AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml"
+        )
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Set Mock returns for resp_format=xml
         MockOAuthSession().get().json.return_value = response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
-        resp = mark.get_option_chains("AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml")
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=True
+        )
+        resp = mark.get_option_chains(
+            "AAPL", expiry_date=dt.date(2019, 2, 15), resp_format="xml"
+        )
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         # Set Mock returns for resp_format=json
         MockOAuthSession().get().json.return_value = response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
-        resp = mark.get_option_chains("AAPL", expiry_date=dt.date(2019, 2, 15),
-                                      strike_price_near=100, chain_type="CALL", option_category="ALL",
-                                      price_type="ALL", skip_adjusted=False, no_of_strikes=5, resp_format="json")
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+        resp = mark.get_option_chains(
+            "AAPL",
+            expiry_date=dt.date(2019, 2, 15),
+            strike_price_near=100,
+            chain_type="CALL",
+            option_category="ALL",
+            price_type="ALL",
+            skip_adjusted=False,
+            no_of_strikes=5,
+            resp_format="json",
+        )
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         MockOAuthSession().get.assert_called_with(
             "https://api.etrade.com/v1/market/optionchains.json?symbol=AAPL&expiryDay=15&expiryMonth=02&expiryYear=2019&strikePriceNear=100.00&chainType=CALL&optionCategory=ALL&priceType=ALL&skipAdjusted=False&noOfStrikes=5"  # noqa: E501
         )
         self.assertTrue(MockOAuthSession().get().json.called)
@@ -174,29 +236,33 @@
 
         # test the assertion failure of chainType, optionCategory,
         # priceType, skipAdjusted
 
     @patch("pyetrade.market.OAuth1Session")
     def test_get_option_expire_date(self, MockOAuthSession):
         """test_get_optionexpiredate(MockOAuthSession)
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session
         """
 
         # response = [dt.date(2019, 1, 18), dt.date(2019, 1, 25)]
         XML_response = (
             r'<?xml version="1.0" encoding="UTF-8" standalone="yes"?>'
             r"<ExpirationDate></ExpirationDate>"
         )
         # Set Mock returns for resp_format=None
         MockOAuthSession().get().text = XML_response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
         resp = mark.get_option_expire_date("AAPL", resp_format="xml")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
 
         MockOAuthSession().get().text = XML_response
-        mark = market.ETradeMarket("abc123", "xyz123", "abctoken", "xyzsecret", dev=True)
+        mark = market.ETradeMarket(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=True
+        )
         resp = mark.get_option_expire_date("AAPL", resp_format="xml")
         assert isinstance(resp, dict)
         assert MockOAuthSession().get.called
```

### Comparing `pyetrade-2.0.1/tests/test_order.py` & `pyetrade-2.1.0/tests/test_order.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,142 @@
 #!/usr/bin/env python3
 """pyetrade authorization unit tests
    TODO:
        * Test request error
        * Test API URL
 """
-
 import unittest
+from unittest.mock import MagicMock
 from unittest.mock import patch
+
 from pyetrade import order
 
 
 class TestETradeOrder(unittest.TestCase):
     """TestEtradeOrder Unit Test"""
 
     def test_option_symbol(self):
         expected = "PLTR--220218P00023000"
-        self.assertEqual(expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", 23))
-        self.assertEqual(expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", 23.00))
-        self.assertEqual(expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", "23.0"))
+        self.assertEqual(
+            expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", 23)
+        )
+        self.assertEqual(
+            expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", 23.00)
+        )
+        self.assertEqual(
+            expected, order.option_symbol("PLTR", order.PUT, "2022-02-18", "23.0")
+        )
 
     @patch("pyetrade.order.OAuth1Session")
     def test_list_orders(self, MockOAuthSession):
         """test_place_equity_order(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session"""
         # Set Mock returns
-        MockOAuthSession().get().json.return_value = {'accountId': '12345'}
+        MockOAuthSession().get().json.return_value = {"accountId": "12345"}
         MockOAuthSession().get().text = r"<xml> returns </xml>"
         orders = order.ETradeOrder(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
 
         # Test Dev buy order equity
-        self.assertEqual(orders.list_orders("12345"), {'accountId': '12345'})
+        self.assertEqual(orders.list_orders("12345"), {"accountId": "12345"})
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
         # Test Prod buy order equity
-        self.assertEqual(orders.list_orders("12345"), {'accountId': '12345'})
+        self.assertEqual(orders.list_orders("12345"), {"accountId": "12345"})
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
-        self.assertTrue(isinstance(orders.list_orders("12345", resp_format="xml"), dict))
+        self.assertTrue(
+            isinstance(orders.list_orders("12345", resp_format="xml"), dict)
+        )
+        self.assertTrue(MockOAuthSession().get().json.called)
+        self.assertTrue(MockOAuthSession().get.called)
+
+    @patch("pyetrade.order.OAuth1Session")
+    def test_list_order_details(self, MockOAuthSession):
+        MockOAuthSession().get().json.return_value = {"accountId": "12345"}
+        MockOAuthSession().get().text = r"<xml> returns </xml>"
+
+        orders = order.ETradeOrder(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+
+        self.assertTrue(
+            isinstance(orders.list_order_details("12345", 123, "json"), dict)
+        )
         self.assertTrue(MockOAuthSession().get().json.called)
         self.assertTrue(MockOAuthSession().get.called)
 
+    def test_find_option_orders(self):
+        orders = order.ETradeOrder(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
+
+        orders.option_symbol = MagicMock(return_value="AAPL--220218C00065000")
+
+        orders.list_orders = MagicMock(
+            return_value={
+                "OrdersResponse": {
+                    "Order": [
+                        {
+                            "OrderDetail": [
+                                {
+                                    "Instrument": [
+                                        {
+                                            "Product": {
+                                                "securityType": "OPTN",
+                                                "productId": {
+                                                    "symbol": "AAPL--220218C00065000"
+                                                },
+                                            }
+                                        }
+                                    ]
+                                }
+                            ]
+                        }
+                    ]
+                }
+            }
+        )
+
+        # Call the function being tested
+        result = orders.find_option_orders(
+            "34fsdf43f", "AAPL", "call", "02-08-2021", 65.0
+        )
+
+        self.assertTrue(isinstance(result, list))
+
     # Mock out OAuth1Session
     @patch("pyetrade.order.OAuth1Session")
     def test_place_equity_order(self, MockOAuthSession):
         """test_place_equity_order(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session"""
 
         # Set Mock returns
         MockOAuthSession().post().text = r"<PreviewOrderResponse><PreviewIds><previewId>321</previewId></PreviewIds></PreviewOrderResponse>"  # noqa: E501
-        orders = order.ETradeOrder("abc123", "xyz123", "abctoken", "xyzsecret", dev=False)  # noqa: E501
+        orders = order.ETradeOrder(
+            "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
+        )
 
         result = orders.place_equity_order(
-                    accountIdKey="12345",
-                    symbol="ABC",
-                    orderAction="BUY",
-                    clientOrderId="1a2b3c",
-                    priceType="MARKET",
-                    quantity=100,
-                    orderTerm="GOOD_UNTIL_CANCEL",
-                    marketSession="REGULAR",
-                )
+            accountIdKey="12345",
+            symbol="ABC",
+            orderAction="BUY",
+            clientOrderId="1a2b3c",
+            priceType="MARKET",
+            quantity=100,
+            orderTerm="GOOD_UNTIL_CANCEL",
+            marketSession="REGULAR",
+        )
 
         # Test xml buy order equity
         self.assertTrue(isinstance(result, dict))
         # self.assertTrue(MockOAuthSession().post().json.called)
         self.assertTrue(MockOAuthSession().post.called)
 
         # Test OrderedDict buy order equity
@@ -87,15 +152,15 @@
                 marketSession="REGULAR",
             )["PreviewOrderResponse"]["PreviewIds"]["previewId"],
             "321",
         )
         self.assertTrue(MockOAuthSession().post.called)
 
         # Test json buy order equity
-        ret_val = {"PreviewOrderResponse": {"PreviewIds": {"previewId": '321'}}}
+        ret_val = {"PreviewOrderResponse": {"PreviewIds": {"previewId": "321"}}}
 
         MockOAuthSession().post().json.return_value = ret_val
         self.assertEqual(
             orders.place_equity_order(
                 accountIdKey="12345",
                 symbol="ABC",
                 orderAction="BUY",
@@ -107,91 +172,121 @@
             ),
             ret_val,
         )
         # self.assertTrue(MockOAuthSession().post().json.called)
         self.assertTrue(MockOAuthSession().post.called)
 
         # Test payload: BUY MARKET
-        payload = orders.build_order_payload("PreviewOrderRequest",
-                                             resp_format="json",
-                                             accountId="12345",
-                                             symbol="ABC",
-                                             orderAction="BUY",
-                                             clientOrderId="1a2b3c",
-                                             priceType="MARKET",
-                                             quantity=100,
-                                             orderTerm="GOOD_UNTIL_CANCEL",
-                                             marketSession="REGULAR",
-                                             )
-        # print(payload)  # to debug
-        expected = {'PreviewOrderRequest': {'orderType': 'EQ', 'clientOrderId': '1a2b3c',
-                                            'Order': {'resp_format': 'json', 'accountId': '12345', 'symbol': 'ABC',
-                                                      'orderAction': 'BUY', 'clientOrderId': '1a2b3c',
-                                                      'priceType': 'MARKET', 'quantity': 100,
-                                                      'orderTerm': 'GOOD_UNTIL_CANCEL', 'marketSession': 'REGULAR',
-                                                      'Instrument': {'Product': {'securityType': 'EQ', 'symbol': 'ABC'},
-                                                                     'orderAction': 'BUY', 'quantityType': 'QUANTITY',
-                                                                     'quantity': 100}}}}
+        payload = orders.build_order_payload(
+            "PreviewOrderRequest",
+            resp_format="json",
+            accountId="12345",
+            symbol="ABC",
+            orderAction="BUY",
+            clientOrderId="1a2b3c",
+            priceType="MARKET",
+            quantity=100,
+            orderTerm="GOOD_UNTIL_CANCEL",
+            marketSession="REGULAR",
+        )
+
+        expected = {
+            "PreviewOrderRequest": {
+                "orderType": "EQ",
+                "clientOrderId": "1a2b3c",
+                "Order": {
+                    "resp_format": "json",
+                    "accountId": "12345",
+                    "symbol": "ABC",
+                    "orderAction": "BUY",
+                    "clientOrderId": "1a2b3c",
+                    "priceType": "MARKET",
+                    "quantity": 100,
+                    "orderTerm": "GOOD_UNTIL_CANCEL",
+                    "marketSession": "REGULAR",
+                    "Instrument": {
+                        "Product": {"securityType": "EQ", "symbol": "ABC"},
+                        "orderAction": "BUY",
+                        "quantityType": "QUANTITY",
+                        "quantity": 100,
+                    },
+                },
+            }
+        }
         self.assertTrue(expected == payload)
 
         # Test payload: SELL STOP
         float_decimals = [
-            (19.99999, '19.99'),  # double values are not exact; SELL: round down to decimal
-            (20, '20.00'),  # exact int
-            (20.01001, '20.01'),
-            (20.01, '20.01'),
-            (20.00999, '20.00'),
-            (20.00001, '20.00'),
+            (
+                19.99999,
+                "19.99",
+            ),  # double values are not exact; SELL: round down to decimal
+            (20, "20.00"),  # exact int
+            (20.01001, "20.01"),
+            (20.01, "20.01"),
+            (20.00999, "20.00"),
+            (20.00001, "20.00"),
         ]
 
         for fd in float_decimals:
             for orderAction in ["SELL", "SELL_SHORT"]:
-                payload = orders.build_order_payload("PreviewOrderRequest",
-                                                     accountIdKey="12345",
-                                                     symbol="ABC",
-                                                     orderAction=orderAction,
-                                                     clientOrderId="1a2b3c",
-                                                     priceType="STOP",
-                                                     stopPrice=fd[0],
-                                                     quantity=100,
-                                                     orderTerm="GOOD_UNTIL_CANCEL",
-                                                     marketSession="REGULAR",
-                                                     )
-                self.assertEqual(payload['PreviewOrderRequest']['Order']['stopPrice'], fd[1])
+                payload = orders.build_order_payload(
+                    "PreviewOrderRequest",
+                    accountIdKey="12345",
+                    symbol="ABC",
+                    orderAction=orderAction,
+                    clientOrderId="1a2b3c",
+                    priceType="STOP",
+                    stopPrice=fd[0],
+                    quantity=100,
+                    orderTerm="GOOD_UNTIL_CANCEL",
+                    marketSession="REGULAR",
+                )
+
+                self.assertEqual(
+                    payload["PreviewOrderRequest"]["Order"]["stopPrice"], fd[1]
+                )
 
         # Test payload: BUY STOP
         float_decimals = [
-            (19.99999, '20.00'),  # double values are not exact; BUY: round   up to decimal
-            (20, '20.00'),  # exact int
-            (20.01001, '20.02'),
-            (20.01, '20.01'),
-            (20.00999, '20.01'),
-            (20.00001, '20.01'),
+            (
+                19.99999,
+                "20.00",
+            ),  # double values are not exact; BUY: round   up to decimal
+            (20, "20.00"),  # exact int
+            (20.01001, "20.02"),
+            (20.01, "20.01"),
+            (20.00999, "20.01"),
+            (20.00001, "20.01"),
         ]
+
         for fd in float_decimals:
             for orderAction in ["BUY", "BUY_TO_COVER"]:
-                payload = orders.build_order_payload("PreviewOrderRequest",
-                                                     accountIdKey="12345",
-                                                     symbol="ABC",
-                                                     orderAction=orderAction,
-                                                     clientOrderId="1a2b3c",
-                                                     priceType="STOP",
-                                                     stopPrice=fd[0],
-                                                     quantity=100,
-                                                     orderTerm="GOOD_UNTIL_CANCEL",
-                                                     marketSession="REGULAR",
-                                                     )
-                self.assertEqual(payload['PreviewOrderRequest']['Order']['stopPrice'], fd[1])
+                payload = orders.build_order_payload(
+                    "PreviewOrderRequest",
+                    accountIdKey="12345",
+                    symbol="ABC",
+                    orderAction=orderAction,
+                    clientOrderId="1a2b3c",
+                    priceType="STOP",
+                    stopPrice=fd[0],
+                    quantity=100,
+                    orderTerm="GOOD_UNTIL_CANCEL",
+                    marketSession="REGULAR",
+                )
 
-    @patch("pyetrade.order.OAuth1Session")
-    def test_place_equity_order_exception(self, MockOAuthSession):
+                self.assertEqual(
+                    payload["PreviewOrderRequest"]["Order"]["stopPrice"], fd[1]
+                )
+
+    def test_place_equity_order_exception(self):
         """test_place_equity_order_exception(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session"""
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session"""
         orders = order.ETradeOrder(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
 
         # Test exception class
         with self.assertRaises(order.OrderException):
             orders.place_equity_order()
@@ -232,36 +327,34 @@
                 orderAction="BUY",
                 clientOrderId="1a2b3c",
                 priceType="STOP_LIMIT",
                 quantity=100,
                 orderTerm="GOOD_UNTIL_CANCEL",
                 marketSession="REGULAR",
             )
-        # Test Prod JSON
-        # self.assertEqual(orders.place_equity_order(), "{'account': 'abc123'}")
-        # Test Dev XML
-        # self.assertEqual(orders.place_equity_order(resp_format='xml'), r'<xml> returns </xml>')
-        # self.assertTrue(MockOAuthSession().get().text.called)
 
     @patch("pyetrade.order.OAuth1Session")
     def test_cancel_order(self, MockOAuthSession):
         """test_cancel_order(MockOAuthSession) -> None
-           param: MockOAuthSession
-           type: mock.MagicMock
-           description: MagicMock of OAuth1Session"""
-        MockOAuthSession().put().json.return_value = {'accountIdKey': '12345'}
+        param: MockOAuthSession
+        type: mock.MagicMock
+        description: MagicMock of OAuth1Session"""
+        MockOAuthSession().put().json.return_value = {"accountIdKey": "12345"}
         MockOAuthSession().put().text = r"<xml> returns </xml>"
         orders = order.ETradeOrder(
             "abc123", "xyz123", "abctoken", "xyzsecret", dev=False
         )
         # Prod
         self.assertEqual(
-            orders.cancel_order("12345", 42, resp_format="json"), {'accountIdKey': '12345'},
+            orders.cancel_order("12345", 42, resp_format="json"),
+            {"accountIdKey": "12345"},
         )
         MockOAuthSession().put.assert_called_with(
             "https://api.etrade.com/v1/accounts" "/12345/orders/cancel",
             json={"CancelOrderRequest": {"orderId": 42}},
             timeout=30,
         )
         self.assertTrue(MockOAuthSession().put().json.called)
         self.assertTrue(MockOAuthSession().put.called)
-        self.assertTrue(isinstance(orders.cancel_order("12345", 42, resp_format="xml"), dict))
+        self.assertTrue(
+            isinstance(orders.cancel_order("12345", 42, resp_format="xml"), dict)
+        )
```

