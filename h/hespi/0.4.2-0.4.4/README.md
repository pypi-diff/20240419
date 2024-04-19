# Comparing `tmp/hespi-0.4.2.tar.gz` & `tmp/hespi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hespi-0.4.2.tar", max compression
+gzip compressed data, was "hespi-0.4.4.tar", max compression
```

## Comparing `hespi-0.4.2.tar` & `hespi-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0    10761 2024-02-28 01:50:46.014106 hespi-0.4.2/LICENSE
--rw-r--r--   0        0        0     4829 2024-02-28 01:50:46.014106 hespi-0.4.2/README.rst
--rw-r--r--   0        0        0       24 2024-02-28 01:50:46.014106 hespi-0.4.2/hespi/__init__.py
--rw-r--r--   0        0        0   671160 2024-02-28 01:50:46.018106 hespi-0.4.2/hespi/data/authority.txt
--rw-r--r--   0        0        0    38256 2024-02-28 01:50:46.018106 hespi-0.4.2/hespi/data/family.txt
--rw-r--r--   0        0        0   148687 2024-02-28 01:50:46.018106 hespi-0.4.2/hespi/data/genus.txt
--rw-r--r--   0        0        0      639 2024-02-28 01:50:46.018106 hespi-0.4.2/hespi/data/mk-lists.py
--rw-r--r--   0        0        0     1175 2024-02-28 01:50:46.018106 hespi-0.4.2/hespi/data/references.bib
--rw-r--r--   0        0        0   697211 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/data/species.txt
--rw-r--r--   0        0        0     3403 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/download.py
--rw-r--r--   0        0        0    10785 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/hespi.py
--rw-r--r--   0        0        0     3459 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/main.py
--rw-r--r--   0        0        0     1963 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/ocr.py
--rw-r--r--   0        0        0     1621 2024-02-28 01:50:46.022106 hespi-0.4.2/hespi/report.py
--rw-r--r--   0        0        0   186041 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/templates/assets/css/bootstrap.hespi.min.css
--rw-r--r--   0        0        0     2976 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/templates/assets/img/favicon.svg
--rw-r--r--   0        0        0     3018 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/templates/assets/img/hespi-favicon.png
--rw-r--r--   0        0        0     4200 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/templates/assets/img/hespi-logo2.svg
--rw-r--r--   0        0        0    12791 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/templates/report-template.html
--rw-r--r--   0        0        0      962 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/tools.py
--rw-r--r--   0        0        0     3573 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/util.py
--rw-r--r--   0        0        0     2490 2024-02-28 01:50:46.026106 hespi-0.4.2/hespi/yolo.py
--rw-r--r--   0        0        0     1719 2024-02-28 01:50:46.026106 hespi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 hespi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10761 2022-08-02 00:08:53.223434 hespi-0.4.4/LICENSE
+-rw-r--r--   0        0        0     5177 2024-03-25 03:22:52.717198 hespi-0.4.4/README.rst
+-rw-r--r--   0        0        0       24 2024-03-22 02:11:53.079775 hespi-0.4.4/hespi/__init__.py
+-rw-r--r--   0        0        0   666941 2024-03-25 03:22:52.729434 hespi-0.4.4/hespi/data/authority.txt
+-rw-r--r--   0        0        0    39057 2024-03-25 03:22:52.731433 hespi-0.4.4/hespi/data/family.txt
+-rw-r--r--   0        0        0   153728 2024-03-25 03:22:52.735044 hespi-0.4.4/hespi/data/genus.txt
+-rw-r--r--   0        0        0      639 2022-09-07 07:14:55.470443 hespi-0.4.4/hespi/data/mk-lists.py
+-rw-r--r--   0        0        0     1175 2024-02-21 22:27:06.746373 hespi-0.4.4/hespi/data/references.bib
+-rw-r--r--   0        0        0   709380 2024-03-25 03:22:52.748450 hespi-0.4.4/hespi/data/species.txt
+-rw-r--r--   0        0        0     3403 2023-03-03 02:50:22.847217 hespi-0.4.4/hespi/download.py
+-rw-r--r--   0        0        0    16090 2024-04-09 07:15:21.579756 hespi-0.4.4/hespi/hespi.py
+-rw-r--r--   0        0        0     3439 2024-03-25 03:22:52.751682 hespi-0.4.4/hespi/main.py
+-rw-r--r--   0        0        0     1851 2024-03-25 03:22:52.753448 hespi-0.4.4/hespi/ocr.py
+-rw-r--r--   0        0        0     2175 2024-03-25 03:22:52.754703 hespi-0.4.4/hespi/report.py
+-rw-r--r--   0        0        0   186041 2023-03-03 01:50:08.888854 hespi-0.4.4/hespi/templates/assets/css/bootstrap.hespi.min.css
+-rw-r--r--   0        0        0     2720 2024-03-25 03:22:52.756040 hespi-0.4.4/hespi/templates/assets/css/hespi.css
+-rw-r--r--   0        0        0     1849 2024-03-25 03:22:52.757564 hespi-0.4.4/hespi/templates/assets/css/hespi.min.css
+-rw-r--r--   0        0        0     2976 2023-02-27 03:47:17.852725 hespi-0.4.4/hespi/templates/assets/img/favicon.svg
+-rw-r--r--   0        0        0      369 2024-03-25 03:22:52.759105 hespi-0.4.4/hespi/templates/assets/img/feather-image.svg
+-rw-r--r--   0        0        0     3018 2023-02-27 03:48:19.585477 hespi-0.4.4/hespi/templates/assets/img/hespi-favicon.png
+-rw-r--r--   0        0        0     6179 2024-03-25 03:22:52.761048 hespi-0.4.4/hespi/templates/assets/img/hespi-logo2.svg
+-rw-r--r--   0        0        0    60404 2024-03-25 03:22:52.763223 hespi-0.4.4/hespi/templates/assets/js/bootstrap.min.js
+-rw-r--r--   0        0        0     9310 2024-04-09 07:08:00.805295 hespi-0.4.4/hespi/templates/report-template.html
+-rw-r--r--   0        0        0     1761 2024-03-25 03:22:52.766219 hespi-0.4.4/hespi/tools.py
+-rw-r--r--   0        0        0     8515 2024-03-25 03:22:52.767528 hespi-0.4.4/hespi/util.py
+-rw-r--r--   0        0        0     2858 2024-03-25 03:22:52.769065 hespi-0.4.4/hespi/yolo.py
+-rw-r--r--   0        0        0     1738 2024-03-25 03:22:52.780524 hespi-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 hespi-0.4.4/PKG-INFO
```

### Comparing `hespi-0.4.2/LICENSE` & `hespi-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/README.rst` & `hespi-0.4.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,24 @@
 .. start-credits
 
 Robert Turnbull, Emily Fitzgerald, Karen Thompson and Jo Birch from the University of Melbourne.
 
 This research was supported by The University of Melbourne’s Research Computing Services and the Petascale Campus Initiative. 
 The authors thank collaborators Niels Klazenga, Heroen Verbruggen, Nunzio Knerr, Noel Faux, Simon Mutch, Babak Shaban, Andrew Drinnan, Michael Bayly and Hannah Turnbull.
 
+Plant refererence data obtained from the `Australian National Species List (auNSL) <https://biodiversity.org.au/nsl>`_, as of March 2024, using the:
+
+- Australian Plant Name Index (APNI)
+- Australian Bryophyte Name Index (AusMoss)
+- Australian Fungi Name Index (AFNI) 
+- Australian Lichen Name Index (ALNI) 
+- Australian Algae Name Index (AANI)
+
+
+
 This pipeline depends on `YOLOv8 <https://github.com/ultralytics/ultralytics>`_, 
 `torchapp <https://github.com/rbturnbull/torchapp>`_,
 Microsoft's `TrOCR <https://www.microsoft.com/en-us/research/publication/trocr-transformer-based-optical-character-recognition-with-pre-trained-models/>`_.
 
 Logo derived from artwork by `ka reemov <https://thenounproject.com/icon/plant-1386076/>`_.
 
 .. end-credits
```

### Comparing `hespi-0.4.2/hespi/data/authority.txt` & `hespi-0.4.4/hespi/data/authority.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 't Mannetje
 (A.A.Fisch.Waldh.) Nannf.
 (A.A.Fisch.Waldh.) Vánky
+(A.A.Francis & Bougher) Kuhar, Nouhra & M.E.Sm.
 (A.A.Ham.) E.J.Thomps.
 (A.A.Ham.) Kük.
 (A.A.Ham.) Vickery
 (A.A.Ham.) W.R.Barker
 (A.A.Padhye & Ajello) de Hoog, Kwon-Chung & McGinnis
 (A.A.Padhye, Ajello & McGinnis) de Hoog & A.A.Padhye
 (A.B.Frank) Donk
+(A.B.Frank) Quaedvl., Verkley & Crous
 (A.B.Jacks.) Bean
 (A.B.Joly & Yam.-Tomita) A.B.Joly & Yam.-Tomita
 (A.B.Joly) R.E.Norris
 (A.Batko) Humber & Ben Ze'ev
 (A.Berger) Backeb.
 (A.Berger) Britton & Rose
 (A.Berger) Riccob.
 (A.Bloxam ex Berk. & Broome) Sacc.
 (A.Braun & Casp.) Southw.
 (A.Braun & Nordst.) R.D.Wood
 (A.Braun & Rabenh.) Lemmerm.
-(A.Braun ex Kütz) Lemmerm. ex Schmidle
 (A.Braun ex Kütz.) A.Braun
 (A.Braun ex Kütz.) A.Ernst
+(A.Braun ex Kütz.) Lemmerm. ex Schmidle
 (A.Braun ex Kütz.) Playfair
 (A.Braun ex Kütz.) Sande Lac. & Suringar
 (A.Braun) A.Braun
 (A.Braun) A.Fisch.
 (A.Braun) Baker
 (A.Braun) Cornu
 (A.Braun) Domin
@@ -96,14 +98,16 @@
 (A.Cunn. ex Benth.) Paul G.Wilson
 (A.Cunn. ex Benth.) Pedley
 (A.Cunn. ex Benth.) Radlk. ex Holle
 (A.Cunn. ex Benth.) Randell
 (A.Cunn. ex Benth.) Rodway
 (A.Cunn. ex Benth.) S.T.Blake ex W.D.Francis
 (A.Cunn. ex Benth.) Tiegh.
+(A.Cunn. ex C.Fraser & Hook.) Fée
+(A.Cunn. ex C.Fraser & Hook.) J.Sm.
 (A.Cunn. ex DC.) A.R.Bean
 (A.Cunn. ex DC.) Anderb.
 (A.Cunn. ex DC.) Benth.
 (A.Cunn. ex DC.) D.J.N.Hind
 (A.Cunn. ex DC.) Domin
 (A.Cunn. ex DC.) Druce
 (A.Cunn. ex DC.) F.Muell.
@@ -118,34 +122,33 @@
 (A.Cunn. ex DC.) N.A.Wakef.
 (A.Cunn. ex DC.) Orchard
 (A.Cunn. ex DC.) Paul G.Wilson
 (A.Cunn. ex DC.) Puente-Lel.
 (A.Cunn. ex DC.) Sch.Bip.
 (A.Cunn. ex DC.) Schmidt-Leb.
 (A.Cunn. ex DC.) Siebert & Voss
+(A.Cunn. ex DC.) T.L.Collins
 (A.Cunn. ex DC.) T.L.Collins & I.Telford
 (A.Cunn. ex DC.) Tovey & P.Morris
 (A.Cunn. ex DC.) Walp.
 (A.Cunn. ex Endl.) Benth.
 (A.Cunn. ex Endl.) F.Muell.
 (A.Cunn. ex Endl.) J.Garden
 (A.Cunn. ex Endl.) Paul G.Wilson
 (A.Cunn. ex Endl.) Silba
 (A.Cunn. ex Ettingsh.) Tiegh.
 (A.Cunn. ex F.Muell.) Radlk.
 (A.Cunn. ex Fenzl) Benth.
 (A.Cunn. ex Fenzl) Orchard
-(A.Cunn. ex Fenzl) Orchard x Gonocarpus oreophilus Orchard
 (A.Cunn. ex Fenzl) Steud.
 (A.Cunn. ex G.Don) C.Moore
 (A.Cunn. ex G.Don) C.T.White
 (A.Cunn. ex G.Don) Court
 (A.Cunn. ex G.Don) Domin
 (A.Cunn. ex G.Don) F.Muell.
-(A.Cunn. ex G.Don) F.Muell. x Brachychiton discolor F.Muell.
 (A.Cunn. ex G.Don) Pedley
 (A.Cunn. ex Heward) Kirk
 (A.Cunn. ex Heward) P.S.Green
 (A.Cunn. ex Hook.) Baker
 (A.Cunn. ex Hook.) Benth.
 (A.Cunn. ex Hook.) Domin
 (A.Cunn. ex Hook.) Endl. ex Heynh.
@@ -192,32 +195,33 @@
 (A.Cunn. ex R.Br.) Christenh. & M.W.Chase
 (A.Cunn. ex R.Br.) Domin
 (A.Cunn. ex R.Br.) Kuntze
 (A.Cunn. ex R.Br.) Makinson
 (A.Cunn. ex R.Br.) O.Deg.
 (A.Cunn. ex Schauer) C.Moore
 (A.Cunn. ex Schauer) Cheel
+(A.Cunn. ex Schauer) Crisp & L.G.Cook
 (A.Cunn. ex Schauer) Domin
 (A.Cunn. ex Schauer) Druce
 (A.Cunn. ex Schauer) F.Muell.
 (A.Cunn. ex Schauer) H.Deane & Maiden
 (A.Cunn. ex Schauer) K.D.Hill & L.A.S.Johnson
 (A.Cunn. ex Schauer) Kuntze
 (A.Cunn. ex Schauer) W.Piep.
-(A.Cunn. ex Sims) A.DC.
 (A.Cunn. ex Tul.) Schodde
 (A.Cunn. ex Walp.) Briq.
 (A.Cunn. ex Walp.) Kattari & Heubl
 (A.Cunn.) A.DC.
 (A.Cunn.) Allan
 (A.Cunn.) Benth.
 (A.Cunn.) Benth. ex Seem.
 (A.Cunn.) Butzin
 (A.Cunn.) C.A.Mey.
 (A.Cunn.) C.Chr.
+(A.Cunn.) C.Fraser & Hook. ex Underw.
 (A.Cunn.) C.Moore
 (A.Cunn.) Christenh. & Byng
 (A.Cunn.) Copel.
 (A.Cunn.) Crisp & P.H.Weston
 (A.Cunn.) D.C.Hassall
 (A.Cunn.) D.Dietr.
 (A.Cunn.) DC.
@@ -249,34 +253,37 @@
 (A.Cunn.) Meisn.
 (A.Cunn.) Mett.
 (A.Cunn.) Miers
 (A.Cunn.) P.I.Forst.
 (A.Cunn.) P.S.Green
 (A.Cunn.) Paul G.Wilson
 (A.Cunn.) Pedley
+(A.Cunn.) Peter G.Wilson
 (A.Cunn.) Planch.
 (A.Cunn.) R.T.Clausen
 (A.Cunn.) Raf.
 (A.Cunn.) Rauschert
-(A.Cunn.) Rauschert x Dockrillia fairfaxii (F.Muell. & Fitzg.) Rauschert
-(A.Cunn.) Rauschert x Dockrillia linguiformis (Sw.) Brieger
-(A.Cunn.) Rauschert x Dockrillia mortii (F.Muell.) Rauschert
-(A.Cunn.) Rauschert x Dockrillia striolata (Rchb.f.) Rauschert
-(A.Cunn.) Rauschert x Dockrillia striolata (Rchb.f.) Rauschert) x Dockrillia pugioniformis (A.Cunn.) Rauschert
 (A.Cunn.) Razafim. & B.Bremer
 (A.Cunn.) Rupp
 (A.Cunn.) Schauer
 (A.Cunn.) Threlfall
 (A.Cunn.) Trudgen
 (A.Cunn.) Tul.
 (A.Cunn.) Voss
 (A.Cunn.) Walp.
 (A.D.Chapm. ex Engelm.) Vasey ex Sarg.
 (A.D.Hawkes) Butzin
 (A.D.Hawkes) Rauschert
+(A.D.Hocking & Pitt) C.A.Rosa & Lachance
+(A.D.Hocking & Pitt) Frisvad, Samson & Stolk
+(A.D.Hocking & Pitt) Houbraken, S.L.Leong & Vinnere-Pettersson
+(A.D.Hocking & Pitt) Minnis & D.L.Lindner
+(A.D.Hocking & Pitt) Samson, N.Yilmaz, Frisvad & Seifert
+(A.D.Hocking & Whitelaw) Samson, N.Yilmaz, Frisvad & Seifert
+(A.D.Hocking) Samson, N.Yilmaz, Frisvad & Seifert
 (A.DC. ex Meisn.) R.Br.
 (A.DC.) Baehni
 (A.DC.) Baill.
 (A.DC.) Benth.
 (A.DC.) Blume
 (A.DC.) C.Moore
 (A.DC.) D.Dietr.
@@ -296,29 +303,31 @@
 (A.DC.) Müll.Arg.
 (A.DC.) Pedley
 (A.DC.) Pichon
 (A.DC.) R.T.Clausen
 (A.DC.) Schönland
 (A.DC.) Stapf
 (A.DC.) Stauffer
+(A.David & Rajchenb.) Hjortstam & K.H.Larss.
 (A.Dietr.) Kuntze
 (A.Dietr.) Lavrov
 (A.Evans) Benedix
-(A.Evans) Steph.
 (A.G.Eliasson) Lindr.
 (A.Gepp & E.Gepp) A.H.S.Lucas
 (A.Gepp & E.Gepp) Cribb
 (A.Gepp & E.Gepp) G.T.Kraft & M.J.Wynne
 (A.Gepp & E.Gepp) R.E.Norris
 (A.Gepp & E.Gepp) R.J.Wilkes, L.M.McIvor & Guiry
 (A.Gepp & E.Gepp) Skottsb.
 (A.Gepp & E.Gepp) V.May
 (A.Gepp & E.Gepp) Zinova
 (A.Gepp) C.F.Reed
+(A.Gepp) Ching
 (A.Gepp) Holttum
+(A.Gepp) S.E.Fawc. & A.R.Sm.
 (A.Gray) Baill.
 (A.Gray) Baill. ex Harms
 (A.Gray) Barneby
 (A.Gray) Benth.
 (A.Gray) C.A.Gardner
 (A.Gray) Carolin ex Hershk.
 (A.Gray) Cogn.
@@ -326,86 +335,97 @@
 (A.Gray) Druce
 (A.Gray) F.M.Bailey
 (A.Gray) F.Muell.
 (A.Gray) H.Eichler
 (A.Gray) H.Ohashi & K.Ohashi
 (A.Gray) Harms
 (A.Gray) Hershk.
+(A.Gray) Jackes & Trias-Blasi
 (A.Gray) Kuntze
 (A.Gray) Latiff
 (A.Gray) Maiden & Betche
 (A.Gray) Ostenf.
 (A.Gray) P.S.Short
 (A.Gray) Paul G.Wilson
 (A.Gray) Pedley
 (A.Gray) Radlk.
 (A.Gray) Rothm.
 (A.Gray) S.Fuentes, Uotila & Borsch
+(A.Gray) Shinners
 (A.Gray) Soják
 (A.Gray) T.I.Chuang & Heckard
 (A.Gray) Tiegh.
 (A.Gray) Voss
 (A.Gray) Wiegand
 (A.H.S.Lucas) A.Millar
+(A.H.S.Lucas) G.H.Boo & Wernberg
 (A.H.S.Lucas) G.T.Kraft
 (A.H.S.Lucas) V.May
 (A.H.S.Lucas) Womersley
 (A.H.S.Lucas) Womersley & Guiry
 (A.H.S.Lucas) Y.Saito & Womersley
 (A.H.Sm. & Hesler) Boertm.
-(A.H.Sm. & M.Lange) Vilgalys, Hopple & Jacq.Johnson
 (A.H.Sm.) Bougher & Castellano
 (A.H.Sm.) Gasparini
 (A.H.Sm.) Grgur.
 (A.H.Sm.) T.W.May
+(A.Hay & S.Taylor) M.D.Barrett, A.Hay & Hett.
 (A.Hay) A.Hay
+(A.Hay) M.D.Barrett, A.Hay & Hett.
+(A.Hay, M.D.Barrett & R.L.Barrett) M.D.Barrett, A.Hay & Hett.
 (A.Heller) Hultén
 (A.Heller) T.I.Chuang & Heckard
 (A.J.Br. & N.G.Walsh) S.W.L.Jacobs
 (A.J.G.Wilson & Hislop) Hislop, Crayn & Puente-Lel.
+(A.J.L.Phillips & Luque) A.J.L.Phillips, A.Alves & Crous
 (A.J.Schill.) G.A.Klebs
 (A.J.Schill.) Kof. & Swezy
 (A.J.Schill.) Lemmerm.
 (A.J.Schill.) Playfair
 (A.J.Scott) Guymer
 (A.J.Scott) N.Snow & Guymer
 (A.Jaeger) Broth.
 (A.Jaeger) Hampe
 (A.Jaeger) J.E.Beever & I.G.Stone
 (A.Jaeger) J.R.Spence & H.P.Ramsay
 (A.Jaeger) M.Fleisch.
 (A.Jaeger) Mitt.
+(A.Jaeger) Ochyra & Bedn.-Ochyra
+(A.Jaeger) Renauld & Cardot
 (A.Jaeger) Watts & Whitel.
 (A.Juss.) Baill.
 (A.Juss.) Benth.
 (A.Juss.) C.DC.
 (A.Juss.) Druce
 (A.Juss.) Engl.
 (A.Juss.) F.Muell.
 (A.Juss.) Kuntze
 (A.Juss.) M.Roem.
 (A.Juss.) Mabb. & Hauenschild
 (A.Juss.) Miq.
 (A.Juss.) Paul G.Wilson
 (A.Jörg.) F.C.Harrison
 (A.Jörg.) Kurtzman
-(A.Kern.) Greuter
+(A.K.Gibbs & Ladiges) Bayly & R.Fowler
 (A.L.Sm.) J.H.Haines & Dumont
-(A.Lister) Meyl.
 (A.M.Gray & R.G.Williams) Ebihara & K.Iwats.
 (A.M.Gray & R.G.Williams) K.Iwats.
 (A.M.Scott & Grönblad) Coesel
 (A.M.Scott & Grönblad) Croasdale
 (A.M.Scott & Grönblad) Teiling
 (A.M.Scott & Prescott) A.M.Scott & Prescott
 (A.M.Scott & Prescott) C.E.M.Bicudo & Compère
 (A.M.Scott & Prescott) Croasdale
+(A.M.Scott & Prescott) R.A.Towns.
 (A.M.Scott & Prescott) Teiling
 (A.M.Scott & Prescott) Thomasson
 (A.M.Young) A.M.Young
+(A.M.Young) J.A.Cooper
+(A.M.Young) Lodge
+(A.M.Young) P.M.Kirk
 (A.Mann) Fryxell & Hasle
 (A.Mann) Hust.
 (A.Mann) Stosch
 (A.Massal. & De Not.) Jatta
 (A.Massal.) A.Massal.
 (A.Massal.) Bornet & Flahault
 (A.Massal.) D.Hawksw.
@@ -463,15 +483,14 @@
 (A.Rich.) Hochr.
 (A.Rich.) Hochst. ex Steud.
 (A.Rich.) Hook.
 (A.Rich.) Hook.f.
 (A.Rich.) J.Raynal
 (A.Rich.) Joy Thomps.
 (A.Rich.) Kirk
-(A.Rich.) Kirk - Apium prostratum Labill. ex Vent.
 (A.Rich.) Kuhn
 (A.Rich.) Kuntze
 (A.Rich.) Lindl.
 (A.Rich.) Meisn. ex Walp.
 (A.Rich.) N.Hallé
 (A.Rich.) O.Schwarz
 (A.Rich.) P.H.Raven & Engelhorn
@@ -504,14 +523,16 @@
 (A.S.George) N.G.Marchant & Keighery
 (A.S.George) Pedley
 (A.S.George) Radcl.-Sm.
 (A.S.George) Rye
 (A.S.George) Stimpson & J.J.Bruhl
 (A.S.George) Szlach.
 (A.S.George) T.L.Maguire, Sedgley & Conran
+(A.S.Patil & V.G.Rao) Alcorn
+(A.S.Patil & V.G.Rao) Manamgoda, L.Cai & K.D.Hyde
 (A.Schimp. ex G.Karst.) F.Gómez
 (A.Schimp. ex G.Karst.) F.Gómez, D.Moreira & López-García
 (A.Schott ex Engelm.) Backeb.
 (A.Schott ex Engelm.) J.M.Coult.
 (A.St.-Hil., A.Juss. & Cambess.) Ravenna
 (A.Stokes) Deflandre
 (A.Stokes) G.A.Klebs
@@ -559,15 +580,14 @@
 (Aa) Alcorn
 (Abbayes) D.J.Galloway
 (Abbayes) Hale
 (Ach. ex Flot.) Körb.
 (Ach.) A.L.Sm.
 (Ach.) A.Massal.
 (Ach.) Ach.
-(Ach.) Ahti & P.James
 (Ach.) Anzi
 (Ach.) Aptroot & Lücking
 (Ach.) Arnold
 (Ach.) Arup, Frödén & Søchting
 (Ach.) B.J.Moore
 (Ach.) Berk. & Broome
 (Ach.) Bory
@@ -595,15 +615,14 @@
 (Ach.) Fryday & Arcadia
 (Ach.) Gray
 (Ach.) Gyeln.
 (Ach.) H.Olivier
 (Ach.) Hafellner
 (Ach.) Hale
 (Ach.) Hale & A.Fletcher
-(Ach.) Hazsl.
 (Ach.) Hertel
 (Ach.) Hertel & Knoph
 (Ach.) Hertel & Leuckert
 (Ach.) Hoffm.
 (Ach.) Jatta
 (Ach.) Kalb, Rivas-Plata & Lumbsch
 (Ach.) Kremp.
@@ -649,14 +668,15 @@
 (Ach.) Th.Fr.
 (Ach.) Tibell
 (Ach.) Trevis.
 (Ach.) Tuck.
 (Ach.) Vain.
 (Ach.) Zahlbr.
 (Adans.) F.Muell.
+(Adans.) Koehne
 (Adans.) Kuntze
 (Adans.) Nied.
 (Adelb.) Verdc.
 (Aderh. & Ruhland) Honey ex Whetzel
 (Aderh.) Boerema, Gruyter & Noordel.
 (Aellen) A.J.Scott
 (Aellen) Aellen
@@ -709,29 +729,27 @@
 (Aiton) Small
 (Aiton) Stearn
 (Aiton) T.Durand & Schinz
 (Aiton) Vent.
 (Aiton) Willd.
 (Ajello) Ajello, Weitzman, McGinnis, & A.A.Padhye
 (Ajello, Georg & C.J.K.Wang) W.Gams, Crous & M.J.Wingf.
-(Alb. & Schwein. : Fr.) P.Kumm.
 (Alb. & Schwein.) Berthier
 (Alb. & Schwein.) Boud.
 (Alb. & Schwein.) Bres.
 (Alb. & Schwein.) Cooke & Quél.
 (Alb. & Schwein.) Corner
 (Alb. & Schwein.) Dennis
 (Alb. & Schwein.) Ditmar
 (Alb. & Schwein.) Fr.
 (Alb. & Schwein.) G.Winter
 (Alb. & Schwein.) Gillet
 (Alb. & Schwein.) J.Schröt.
 (Alb. & Schwein.) Korf
 (Alb. & Schwein.) Kotl. & Pouzar
-(Alb. & Schwein.) Kuhner
 (Alb. & Schwein.) Kuntze
 (Alb. & Schwein.) Kühner
 (Alb. & Schwein.) Massee
 (Alb. & Schwein.) Murrill
 (Alb. & Schwein.) P.Crouan & H.Crouan
 (Alb. & Schwein.) P.Karst.
 (Alb. & Schwein.) P.Kumm.
@@ -740,17 +758,21 @@
 (Alb. & Schwein.) Pouzar
 (Alb. & Schwein.) Rabenh.
 (Alb. & Schwein.) Ricken
 (Alb. & Schwein.) Rostaf.
 (Alb. & Schwein.) Sacc.
 (Alb. & Schwein.) Seaver
 (Alb. & Schwein.) de Bary
+(Albr. & J.G.West) Hershk.
 (Albr. & N.G.Walsh) Paul G.Wilson
+(Alcorn & P.M.Kirk) J.S.Monteiro, S.M.Leão, Gusmão, P.M.Kirk & R.F.Castañeda
 (Alcorn) Alcorn
+(Alcorn) Manamgoda, L.Cai & K.D.Hyde
 (Alcorn) Tsuda & Ueyama
+(Alcorn) Y.P.Tan & R.G.Shivas
 (Alderw.) A.R.Field & Bostock
 (Alderw.) Ching
 (Alexop. & Beneke) Alexop.
 (Ali) I.Thomps.
 (All.) Chiov.
 (All.) Coss. & Durieu
 (All.) Janch.
@@ -840,19 +862,19 @@
 (Ant.Mayer) A.D.Hardy
 (Antoine) Endl.
 (Antoine) F.M.Bailey
 (Anzi) Coppins & R.Sant.
 (Anzi) Matzer & Hafellner
 (Anzi) Müll.Arg.
 (Anzi) Vězda
+(Apinis & R.G. Rees) H.Kandemir & de Hoog
 (Apinis) Currah
 (Apstein) Entz
 (Apstein) Lebour
 (Aptroot & Sipman) Aptroot
-(Araguello & A.Crespo) A.Crespo, Divakar & Elix
 (Ard.) Fiori
 (Ard.) Fritsch
 (Ard.) Host
 (Ard.) O.Bolos & Masclans
 (Ard.) Roem. & Schult.
 (Ard.) Spreng.
 (Ardré) R.E.Norris
@@ -894,22 +916,20 @@
 (Arnold) M.Choisy
 (Arnold) Sérus.
 (Artari) Oltm.
 (Arthur) Arthur
 (Arthur) Vánky
 (Arx & Constant.) Crous
 (Arx) P.F.Cannon & D.Hawksw.
+(Arzanlou & Crous) Crous & U.Braun
 (Asah.) Trass
-(Asahina) Asahina
 (Asahina) Elix
 (Asahina) Elix & Hale
-(Asahina) Elix & J.Johnst.
 (Asahina) Hale
 (Asahina) I.M.Lamb & A.Ward
-(Asahina) Krog & Swinscow
 (Asahina) Yoshim.
 (Asch.) Asch.
 (Asch.) Dandy
 (Asch.) Ostenf.
 (Asch.) Palla
 (Asch.) S.W.L.Jacobs
 (Asch.) Toml. & Posl.
@@ -943,14 +963,15 @@
 (Auriv.) Broch
 (Auriv.) Cleve
 (Auriv.) Parke & J.D.Dodge
 (Auriv.) Paulsen
 (Austin) A.Evans
 (Austin) Austin
 (Austin) Douin
+(Austin) Steere
 (B.Boivin) J.H.Willis
 (B.Boivin) W.M.Curtis
 (B.C.Stone) B.C.Stone
 (B.C.Zhang & Minter) Kraisit., Pfister & M.E.Sm.
 (B.Eichler & Gutw.) Compere
 (B.Eichler & Gutw.) West & G.S.West
 (B.Eichler) Playfair
@@ -974,14 +995,15 @@
 (B.J.Conn & Tame) Pedley
 (B.J.Conn) A.J.Paton
 (B.J.Conn) C.S.P.Foster & B.J.Conn
 (B.J.Conn) K.L.Gibbons, B.J.Conn & Henwood
 (B.K.Simon) B.K.Simon
 (B.K.Simon) E.J.Thomps.
 (B.K.Simon) Night.
+(B.K.Simon) P.M.Peterson, Romasch. & Soreng
 (B.K.Simon) R.D.Webster
 (B.K.Simon) R.L.Barrett & P.M.Peterson
 (B.K.Simon) Veldkamp
 (B.K.Simon) Zuloaga
 (B.L.Burtt) A.R.Mast & K.R.Thiele
 (B.L.Burtt) A.S.George
 (B.L.Burtt) Jackes
@@ -992,44 +1014,47 @@
 (B.Lindeb.) Kukkonen
 (B.M.Thiers) B.M.Thiers
 (B.M.Thiers) Bechteler, G.E.Lee, Schaf.-Verw. & Heinrichs
 (B.M.Thiers) Pócs & Bernecker
 (B.M.Thiers) X.-L.He
 (B.Sutton & Alcorn) W.A.Baker & Morgan-Jones
 (B.Sutton & Ganap.) Crous & U.Braun
+(B.Sutton & Ganap.) Quaedvl. & Crous
 (B.Sutton & Hodges) Aramb. & Cabello
 (B.Sutton & Hodges) Whitton, McKenzie & K.D.Hyde
+(B.Sutton & Pascoe) D.A.C.Almeida & Gusmão
 (B.Sutton & Pascoe) Z.Q.Yuan
 (B.Sutton) Crous
+(B.Sutton) D’souza, Boonmee & K.D.Hyde
+(B.Sutton) Shoemaker
 (B.Sutton) Whitton, McKenzie & K.D.Hyde
 (B.de Lesd. ex Harmand) Elix & Hale
 (B.de Lesd. ex Harmand) Lendemer & B.P.Hodk.
-(B.de Lesd.) Elix & Hale
 (B.de Lesd.) J.R.Laundon
 (B.de Lesd.) R.C.Harris
 (Baarud) Balech
 (Bab.) Aedo
 (Bab.) Hitchc.
 (Bab.) Nyl.
-(Bab.) Rostaf.
 (Babeva & Reshetova) Golubev
 (Bach.Pyl.) Hampe
 (Bach.Pyl.) Mont.
 (Bach.Pyl.) Steud.
 (Backh. & Harv.) Goldblatt & J.C.Manning
 (Backh. ex Hook.f.) Benth.
 (Backh. ex Planch.) B.J.Conn
 (Backh. ex Planch.) Chrtek & Slavikova
 (Bagl.) Guderley & Lumbsch
 (Bagl.) J.Steiner
 (Bagl.) Swinscow & Krog
 (Bailey ex Harv.) Falkenb.
-(Bailey ex J.T.Queckett) W.Sm.
+(Bailey ex J.T.Quekett) J.W.Griff. & Henfr.
+(Bailey ex J.T.Quekett) W.Sm.
 (Bailey) A.M.Edwards
-(Bailey) A.Mann.
+(Bailey) A.Mann
 (Bailey) Balech
 (Bailey) C.H.G.Pouchet
 (Bailey) C.S.Boyer
 (Bailey) Cleve
 (Bailey) D.G.Mann
 (Bailey) F.Gómez
 (Bailey) Gran
@@ -1039,15 +1064,14 @@
 (Bailey) Poulin
 (Bailey) Ralfs
 (Bailey) Reimer
 (Bailey) Roper
 (Bailey) Van Heurck
 (Bailey) W.Archer
 (Bailey) Wittr.
-(Bailey) ex L.W.Bailey
 (Baill.) Airy Shaw
 (Baill.) B.G.Thomson
 (Baill.) Baehni
 (Baill.) Baill.
 (Baill.) Baill. ex Benth.
 (Baill.) Benth.
 (Baill.) Burret
@@ -1085,15 +1109,14 @@
 (Baker) Christ
 (Baker) Christenh.
 (Baker) Copel.
 (Baker) Diels
 (Baker) Domin
 (Baker) F.Ballard
 (Baker) F.Muell.
-(Baker) Farw.
 (Baker) Holttum
 (Baker) J.Sm.
 (Baker) Kuntze
 (Baker) Luerss. ex Salomon
 (Baker) M.F.Fay & Christenh.
 (Baker) M.W.Chase, Rudall & Conran
 (Baker) Oberm.
@@ -1116,15 +1139,14 @@
 (Balech) Montresor, Zingone & D.Marino
 (Banks & Sol. ex DC.) Hook.f.
 (Banks & Sol. ex Gaertn.) Heads
 (Banks & Sol. ex Hook.f.) C.Yen & J.L.Yang
 (Banks & Sol. ex Hook.f.) Govaerts
 (Banks & Sol. ex Hook.f.) Kirk ex Cheeseman
 (Banks & Sol. ex Hook.f.) Á.Löve & Connor
-(Banks & Sol.) Sm.
 (Banks ex DC.) R.L.Barrett
 (Banks ex Gaertn.) Kuntze
 (Banks ex Gaertn.) L.S.Sm.
 (Banks ex Gaertn.) N.Snow & Guymer
 (Banks) Blume
 (Banks) M.W.Chase, Christenh. & Schuit.
 (Banks) R.Br.
@@ -1153,45 +1175,45 @@
 (Bastow) Paris
 (Bat.) B.Sutton & Pascoe
 (Bat.) M.B.Ellis
 (Bateman ex Lindl.) Kuntze
 (Bateman ex Rchb.f.) Kuntze
 (Bateman ex Rchb.f.) M.A.Clem. & D.L.Jones
 (Bateman ex Rchb.f.) Rchb.f.
-(Batsch : Fr.) Fr.
-(Batsch : Fr.) Quel.
 (Batsch) Alb. & Schwein.
 (Batsch) Berk. & Broome
+(Batsch) Bertill.
 (Batsch) Binyamini
 (Batsch) Boud.
 (Batsch) Bres.
 (Batsch) Cooke
 (Batsch) Corner
 (Batsch) Fr.
 (Batsch) Fuckel
 (Batsch) Gillet
 (Batsch) Gray
 (Batsch) Harmaja
 (Batsch) Hesler
 (Batsch) Hollós
-(Batsch) J.-E.Gilbert
 (Batsch) J.F.Gmel.
 (Batsch) J.Schröt.
 (Batsch) Korf & S.E.Carp.
 (Batsch) Kühner
 (Batsch) Kühner & Maire
 (Batsch) Lloyd
 (Batsch) McAlpine
 (Batsch) Nann.-Bremek.
 (Batsch) Nann.-Bremek. ex G.W.Martin & Alexop.
+(Batsch) Niskanen & Liimat.
 (Batsch) P.Karst.
 (Batsch) P.Kumm.
 (Batsch) Pers.
 (Batsch) Quél.
 (Batsch) R.N.Ames
+(Batsch) Redhead, Moncalvo & Vilgalys
 (Batsch) Rostaf.
 (Batsch) Rostk.
 (Batsch) Singer
 (Batsch) T.Macbr.
 (Batsch) Zahlbr.
 (Battarra) Fr.
 (Batters) Feldmann & Feldm.-Maz.
@@ -1226,14 +1248,15 @@
 (Beeby) Walters
 (Beeli) Heinem.
 (Beeli) Thoen
 (Beetle) Oteng-Yeb.
 (Behr) Engl.
 (Behr) Tiegh.
 (Behre) Kurt Först.
+(Beilharz, Pascoe, M.J.Wingf. & Crous) Videira & Crous
 (Bellynck) Boerema, Loer. & Hamers
 (Belt.) Tibell
 (Benl & H.Eichler) R.W.Davis
 (Benl) A.R.Bean
 (Benl) Benl
 (Benl) Benl & H.Eichler
 (Benl) Lally & W.R.Barker
@@ -1305,14 +1328,15 @@
 (Benth.) Buchanan
 (Benth.) Burret
 (Benth.) Burtt Davy
 (Benth.) C.A.Gardner
 (Benth.) C.A.Newell & Hymowitz
 (Benth.) C.B.Clarke
 (Benth.) C.E.Hubb.
+(Benth.) C.E.Hughes & G.P.Lewis
 (Benth.) C.F.Wilkins & Chappill
 (Benth.) C.F.Wilkins & Whitlock
 (Benth.) C.H.Mill. & J.G.West
 (Benth.) C.H.Wright
 (Benth.) C.Moore
 (Benth.) C.Norman
 (Benth.) C.S.P.Foster & B.J.Conn
@@ -1331,33 +1355,34 @@
 (Benth.) Corrick
 (Benth.) Court
 (Benth.) Cowie
 (Benth.) Craven
 (Benth.) Craven & Lepschi
 (Benth.) Craven & R.D.Edwards
 (Benth.) Crisp
+(Benth.) Crisp & L.G.Cook
 (Benth.) D'Arcy
 (Benth.) D.C.Hassall
 (Benth.) D.C.Thomas, Chaowasku & R.M.K.Saunders
 (Benth.) D.G.Lloyd & C.J.Webb
 (Benth.) D.I.Morris
 (Benth.) D.L.Jones & M.A.Clem.
 (Benth.) DC.
 (Benth.) Danser
 (Benth.) De Wild.
 (Benth.) Diels
 (Benth.) Dockrill
 (Benth.) Domin
-(Benth.) Domin x Eucalyptus orthostemon D.Nicolle & Brooker
 (Benth.) Druce
 (Benth.) Drude
 (Benth.) Dunlop
 (Benth.) Duretto
 (Benth.) Duretto & Heslewood
 (Benth.) E.A.Shaw
+(Benth.) E.J.Thomps.
 (Benth.) E.M.Benn.
 (Benth.) E.Pritz.
 (Benth.) Eichler
 (Benth.) Endl.
 (Benth.) Engl.
 (Benth.) Ewart
 (Benth.) Ewart & B.Rees
@@ -1367,22 +1392,18 @@
 (Benth.) F.J.Herm.
 (Benth.) F.L.Erickson & J.H.Willis
 (Benth.) F.M.Bailey
 (Benth.) F.Muell.
 (Benth.) F.Muell. ex Benth.
 (Benth.) F.Muell. ex C.T.White & W.D.Francis
 (Benth.) F.Muell. ex H.B.Will.
-(Benth.) F.Muell. ex H.B.Will. x Pultenaea euchila DC.
-(Benth.) F.Muell. ex H.B.Will. x Pultenaea flexilis Sm.
-(Benth.) F.Muell. ex H.B.Will. x Pultenaea villosa Andrews
 (Benth.) F.Muell. ex Hieron.
 (Benth.) F.Muell. ex Hochr.
 (Benth.) F.Muell. ex Maiden
 (Benth.) F.Muell. ex Tate
-(Benth.) F.Muell. x Eremophila polyclada (F.Muell.) F.Muell.
 (Benth.) F.N.Williams
 (Benth.) Fosberg
 (Benth.) Fryxell
 (Benth.) G.Chandler & Crisp
 (Benth.) G.Goeze
 (Benth.) G.L.Davis
 (Benth.) G.L.Nesom
@@ -1435,36 +1456,37 @@
 (Benth.) J.M.Powell
 (Benth.) J.Palmer
 (Benth.) J.R.Wheeler
 (Benth.) J.R.Wheeler & N.G.Marchant
 (Benth.) J.Schust.
 (Benth.) J.W.Horn
 (Benth.) J.Z.Weber
+(Benth.) Jackes & Trias-Blasi
 (Benth.) Jacques
 (Benth.) Janes & Duretto
 (Benth.) Jansen
 (Benth.) Jarman
 (Benth.) Jeanes
 (Benth.) Jessup
 (Benth.) Jessup, Kessler & Mols
 (Benth.) Joy Thomps.
 (Benth.) Jørg.
 (Benth.) K.A.Sheph.
 (Benth.) K.A.Sheph. & C.F.Wilkins
 (Benth.) K.A.Sheph. & Paul G.Wilson
 (Benth.) K.D.Hill & L.A.S.Johnson
-(Benth.) K.D.Hill & L.A.S.Johnson x Corymbia dimorpha (Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson
 (Benth.) K.Koch
 (Benth.) K.Krause
 (Benth.) K.L.Wilson
 (Benth.) K.L.Wilson & R.L.Barrett
 (Benth.) K.Schum.
 (Benth.) Keighery
 (Benth.) Kodela
 (Benth.) Koehne
+(Benth.) Kosterm.
 (Benth.) Kraenzl.
 (Benth.) Kuntze
 (Benth.) Kyal. & Boatwr.
 (Benth.) Kük.
 (Benth.) L.A.S.Johnson
 (Benth.) L.A.S.Johnson & Blaxell
 (Benth.) L.A.S.Johnson & O.D.Evans
@@ -1514,30 +1536,31 @@
 (Benth.) O.E.Schulz
 (Benth.) Ohwi
 (Benth.) Olde & Marriott
 (Benth.) Oliv.
 (Benth.) Orchard
 (Benth.) Ostenf.
 (Benth.) P.I.Forst.
-(Benth.) P.I.Forst. x Leichhardtia viridiflora (R.Br.) P.I.Forst.
 (Benth.) P.J.H.Hurter
+(Benth.) P.J.Lang
 (Benth.) P.M.Peterson & N.Snow
+(Benth.) P.M.Peterson, Romasch. & Soreng
 (Benth.) P.S.Green
 (Benth.) P.S.Short
 (Benth.) Pamp.
 (Benth.) Parr-Sm.
 (Benth.) Paul G.Wilson
 (Benth.) Paul G.Wilson & M.A.Wilson
-(Benth.) Paul G.Wilson - Phebalium squamulosum subsp. ozothamnoides (F.Muell.) Paul G.Wilson
 (Benth.) Paulsen
 (Benth.) Pax & K.Hoffm.
 (Benth.) Pedley
 (Benth.) Pedley ex R.Butcher
 (Benth.) Pennell
 (Benth.) Perkins
+(Benth.) Peter G.Wilson
 (Benth.) Peter G.Wilson & J.T.Waterh.
 (Benth.) Pilg.
 (Benth.) Planch.
 (Benth.) Pojark.
 (Benth.) Polhill
 (Benth.) Quinn
 (Benth.) R.A.Kerrigan
@@ -1628,33 +1651,34 @@
 (Bergh) F.Schütt
 (Bergh) J.Schiller
 (Bergh) Kof. & Swezy
 (Bergh) Paulsen
 (Bergius) Willd.
 (Bergmans ex J.W.Ingram) D.H.Kent
 (Bergon) Hasle
-(Berk. & Broome ex C.W.Dodge & Zeller) G.W.Beaton
-(Berk. & Broome ex C.W.Dodge & Zeller) Peintner & M.M.Moser
+(Berk. & A.Bloxam) Petr.
 (Berk. & Broome ex Cooke) Cooke
 (Berk. & Broome ex Cooke) G.Cunn.
 (Berk. & Broome ex Cooke) Kuntze
 (Berk. & Broome ex Cooke) L.Hansen
 (Berk. & Broome ex Cooke) Pat.
+(Berk. & Broome ex Zeller & C.W.Dodge) G.W.Beaton
+(Berk. & Broome ex Zeller & C.W.Dodge) Peintner & M.M.Moser
 (Berk. & Broome) A.H.Sm.
 (Berk. & Broome) A.M.Young
 (Berk. & Broome) Agerer
 (Berk. & Broome) B.L.Brady, B.Sutton & Samson
+(Berk. & Broome) Bailey
 (Berk. & Broome) Berl.
 (Berk. & Broome) Berl. & Voglino
 (Berk. & Broome) Boedijn
 (Berk. & Broome) Boidin
 (Berk. & Broome) Boud.
 (Berk. & Broome) Burds.
 (Berk. & Broome) C.W.Dodge
-(Berk. & Broome) C.W.Dodge & Zeller
 (Berk. & Broome) C.Walker & A.Schüssler
 (Berk. & Broome) Cleland
 (Berk. & Broome) Cleland & Cheel
 (Berk. & Broome) Cooke
 (Berk. & Broome) Cooke ex G.Cunn.
 (Berk. & Broome) Corner
 (Berk. & Broome) Cáceres & Lücking
@@ -1691,14 +1715,15 @@
 (Berk. & Broome) Locq.
 (Berk. & Broome) M.B.Ellis
 (Berk. & Broome) M.L.Wu & J.H.Haines
 (Berk. & Broome) Maas Geest.
 (Berk. & Broome) Massee
 (Berk. & Broome) McAlpine
 (Berk. & Broome) McNabb
+(Berk. & Broome) Miettinen
 (Berk. & Broome) Nakasone & D.L.Lindner
 (Berk. & Broome) Nannf.
 (Berk. & Broome) P.A.Lemke
 (Berk. & Broome) P.F.Cannon
 (Berk. & Broome) Pat.
 (Berk. & Broome) Pat. ex Reinking
 (Berk. & Broome) Pegler
@@ -1713,35 +1738,41 @@
 (Berk. & Broome) Renny
 (Berk. & Broome) Rick
 (Berk. & Broome) Ricker
 (Berk. & Broome) Rifai
 (Berk. & Broome) Rossman & Samuels
 (Berk. & Broome) Rostaf.
 (Berk. & Broome) Ryvarden
+(Berk. & Broome) S.H.He & Nakasone
 (Berk. & Broome) S.Hughes
 (Berk. & Broome) Sacc.
 (Berk. & Broome) Sacc. & D.Sacc.
+(Berk. & Broome) Samuels, Nalim & Geiser
 (Berk. & Broome) Seaver
 (Berk. & Broome) Seaver & Waterston
 (Berk. & Broome) Sheng H.Wu
 (Berk. & Broome) Singer
 (Berk. & Broome) Spooner
 (Berk. & Broome) Stalpers
 (Berk. & Broome) T.W.May & A.E.Wood
 (Berk. & Broome) Teng
 (Berk. & Broome) Theiss. & Syd.
 (Berk. & Broome) Thirum. & M.J.O'Brien
 (Berk. & Broome) Trappe & Gerd.
+(Berk. & Broome) Trappe, Desirò, M.E. Sm., Bonito & Bidartondo
 (Berk. & Broome) Vánky
 (Berk. & Broome) W.B.Cooke
 (Berk. & Broome) Y.M.Ju & J.D.Rogers
+(Berk. & Broome) Zeller & C.W.Dodge
 (Berk. & Cooke) Cooke
 (Berk. & Cooke) Kuntze
 (Berk. & Cooke) Ryvarden
 (Berk. & Cooke) Sacc.
+(Berk. & Corda) S.Hughes
+(Berk. & Corda) Sacc.
 (Berk. & F.Muell.) Kuntze
 (Berk. & F.Muell.) Sacc.
 (Berk. & Hook.f.) Berk.
 (Berk. & M.A.Curtis ex Cooke) G.Cunn.
 (Berk. & M.A.Curtis ex Cooke) Pat.
 (Berk. & M.A.Curtis ex Cooke) Ryvarden
 (Berk. & M.A.Curtis ex Cooke) Sheng H.Wu
@@ -1751,14 +1782,15 @@
 (Berk. & M.A.Curtis ex Sacc.) Shoemaker
 (Berk. & M.A.Curtis ex Sacc.) Subram. & B.L.Jain
 (Berk. & M.A.Curtis ex W.Phillips) J.R.Dixon
 (Berk. & M.A.Curtis) A.H.Sm.
 (Berk. & M.A.Curtis) A.L.Welden
 (Berk. & M.A.Curtis) Arx
 (Berk. & M.A.Curtis) B.J.Rees
+(Berk. & M.A.Curtis) B.K.Cui, M.L.Han & Y.C.Dai
 (Berk. & M.A.Curtis) Boidin
 (Berk. & M.A.Curtis) Brumm.
 (Berk. & M.A.Curtis) Burds.
 (Berk. & M.A.Curtis) Burt
 (Berk. & M.A.Curtis) Burt ex Coker
 (Berk. & M.A.Curtis) C.T.Wei
 (Berk. & M.A.Curtis) Chamuris
@@ -1777,45 +1809,54 @@
 (Berk. & M.A.Curtis) Gilb. & Ryvarden
 (Berk. & M.A.Curtis) Ginns & Weresub
 (Berk. & M.A.Curtis) Gresl., Nakasone & Rajchenb.
 (Berk. & M.A.Curtis) Henn.
 (Berk. & M.A.Curtis) Höhn.
 (Berk. & M.A.Curtis) Imazeki
 (Berk. & M.A.Curtis) J.D.Rogers, Y.M.Ju & F.San Martín
+(Berk. & M.A.Curtis) J.L.Zhou & B.K.Cui
+(Berk. & M.A.Curtis) J.S.Oliveira
 (Berk. & M.A.Curtis) Jülich
 (Berk. & M.A.Curtis) Kreisel & Dring
 (Berk. & M.A.Curtis) Kuntze
 (Berk. & M.A.Curtis) Kõljalg
+(Berk. & M.A.Curtis) L.W.Zhou & Y.C.Dai
 (Berk. & M.A.Curtis) Le Gal
 (Berk. & M.A.Curtis) Lloyd
 (Berk. & M.A.Curtis) M.A.Litv.
 (Berk. & M.A.Curtis) M.B.Ellis
 (Berk. & M.A.Curtis) M.J.Larsen
 (Berk. & M.A.Curtis) Morgan
 (Berk. & M.A.Curtis) Murrill
 (Berk. & M.A.Curtis) Nikol.
 (Berk. & M.A.Curtis) Pat.
 (Berk. & M.A.Curtis) Pegler
 (Berk. & M.A.Curtis) Pilát
 (Berk. & M.A.Curtis) Pouzar
 (Berk. & M.A.Curtis) R.H.Petersen
+(Berk. & M.A.Curtis) R.R.Gomes, Glienke & Crous
+(Berk. & M.A.Curtis) Riebesehl & Langer
 (Berk. & M.A.Curtis) Rifai
 (Berk. & M.A.Curtis) Ryvarden
+(Berk. & M.A.Curtis) S.H.He & Jiao Yang
+(Berk. & M.A.Curtis) S.H.He & Y.C.Dai
 (Berk. & M.A.Curtis) S.Hughes
 (Berk. & M.A.Curtis) S.Hughes & Piroz. ex D.Hawksw. & Mibey
 (Berk. & M.A.Curtis) S.Ito & S.Imai
 (Berk. & M.A.Curtis) Sacc.
 (Berk. & M.A.Curtis) Sacc. & Trotter
 (Berk. & M.A.Curtis) Seaver
 (Berk. & M.A.Curtis) Singer
 (Berk. & M.A.Curtis) Speg.
 (Berk. & M.A.Curtis) T.Wagner & M.Fisch.
 (Berk. & M.A.Curtis) Teng
+(Berk. & M.A.Curtis) Vlasák
 (Berk. & M.A.Curtis) Wakef.
 (Berk. & M.A.Curtis) Zeller
+(Berk. & Ravenel) 
 (Berk. & Ravenel) Cooke
 (Berk. & Ravenel) Morgan
 (Berk. & Ravenel) Sacc.
 (Berk. & Ravenel) Thaxt.
 (Berk. & W.Phillips) Sacc.
 (Berk. ex Cooke) Bres.
 (Berk. ex Cooke) Cooke
@@ -1828,44 +1869,45 @@
 (Berk. ex Cooke) Pat.
 (Berk. ex Cooke) Pilát
 (Berk. ex Cooke) Ryvarden
 (Berk. ex Cooke) Sacc.
 (Berk. ex Curr.) Sacc.
 (Berk. ex F.Muell.) E.Fisch.
 (Berk. ex Fisch.) G.Cunn.
+(Berk. ex Fr.) 
 (Berk. ex Fr.) Cooke
 (Berk. ex Fr.) F.M.Bailey
 (Berk. ex Fr.) F.Muell.
 (Berk. ex Fr.) G.Cunn.
 (Berk. ex Lloyd) Cleland & Cheel
-(Berk. ex Massee) Berk.
 (Berk. ex Massee) E.Horak
 (Berk. ex Massee) G.Cunn.
 (Berk. ex Massee) Vánky
 (Berk. ex Sacc.) Cooke
 (Berk. ex Sacc.) G.Cunn.
 (Berk. ex Sacc.) Kuntze
 (Berk. ex Sacc.) Pat.
 (Berk.) A.A.Fisch.Waldh.
 (Berk.) A.Gepp & E.Gepp
 (Berk.) A.M.Young
 (Berk.) Aberdeen
 (Berk.) Aoshima
 (Berk.) Aveskamp, Gruyter & Verkley
+(Berk.) B.K.Cui & Shun Liu
+(Berk.) B.K.Cui, M.L.Han & Y.C.Dai
 (Berk.) Berk.
 (Berk.) Berk. & Broome
 (Berk.) Berk. & M.A.Curtis
 (Berk.) Berk. ex Cooke
 (Berk.) Boedijn
 (Berk.) Boidin
 (Berk.) Bres.
 (Berk.) Bres. ex Wakef.
 (Berk.) Bresinsky & Jarosch
 (Berk.) Brittleb.
-(Berk.) Castellano & Trappe
 (Berk.) Cheel
 (Berk.) Cif.
 (Berk.) Cleland
 (Berk.) Cleland & Cheel
 (Berk.) Cooke
 (Berk.) Cooke ex Sacc.
 (Berk.) Corner
@@ -1885,76 +1927,84 @@
 (Berk.) Eichelb.
 (Berk.) F.M.Bailey
 (Berk.) F.Muell.
 (Berk.) Farl.
 (Berk.) Fiasson & Niemelä
 (Berk.) Fr.
 (Berk.) G.Cunn.
-(Berk.) Gilb. & J.Carranza
 (Berk.) Gilb. & Ryvarden
 (Berk.) Ginns
 (Berk.) Gomont
+(Berk.) H.S.Yuan
 (Berk.) Hansf.
 (Berk.) Hassall
 (Berk.) Henn.
 (Berk.) Hjortstam
 (Berk.) Hjortstam & Ryvarden
 (Berk.) Hollós
 (Berk.) Hood & M.A.Dick
 (Berk.) Höhn.
 (Berk.) Höhn. & Litsch.
 (Berk.) Imazeki
+(Berk.) J.A.Cooper
+(Berk.) J.Carranza & Gilb.
 (Berk.) J.E.Wright & J.R.Deschamps
 (Berk.) J.R.Dixon
+(Berk.) Jaklitsch & Voglmayr
+(Berk.) Justo
 (Berk.) Jülich
-(Berk.) Kantvilas & Y.S.Chang
 (Berk.) Karun. & K.D.Hyde
 (Berk.) Kits van Wav.
 (Berk.) Kobayasi
 (Berk.) Komark.-Legn.
 (Berk.) Kotl. & Pouzar
 (Berk.) Kreisel
+(Berk.) Kuhar, Nouhra & M.E.Sm.
 (Berk.) Kuntze
 (Berk.) Le Gal
 (Berk.) Linder
 (Berk.) Lloyd
-(Berk.) Lloyd ex E.K.Cash & J.A.Stev.
+(Berk.) Lloyd ex J.A.Stev. & E.K.Cash
 (Berk.) Lloyd ex J.E.Wright
 (Berk.) Locq.
 (Berk.) Lév.
+(Berk.) M.D.Barrett
 (Berk.) M.J.Larsen
 (Berk.) M.Piepenbr.
 (Berk.) M.Piepenbr. & Begerow
 (Berk.) Massee
 (Berk.) McAlpine
 (Berk.) McNabb
+(Berk.) McTaggart & R.G.Shivas
+(Berk.) Miettinen
+(Berk.) Mossebo & Ambit
 (Berk.) Mundk.
 (Berk.) Murrill
 (Berk.) N.Walters & E.W.B.Da Costa
 (Berk.) Nakasone
 (Berk.) Nannf. & Korf
 (Berk.) Nieuwl.
 (Berk.) Noordel.
 (Berk.) O.K.Mill.
 (Berk.) Overeem
 (Berk.) P.D.Orton
-(Berk.) P.Henn.
 (Berk.) P.K.Buchanan & Ryvarden
 (Berk.) P.Karst.
+(Berk.) P.R.Johnst., Baral & R.Galán
 (Berk.) P.Roberts
 (Berk.) Parmasto
 (Berk.) Pat.
 (Berk.) Peck
 (Berk.) Pegler
-(Berk.) Pegler & Lodge
 (Berk.) Pegler & R.W.Rayner
 (Berk.) Pegler & T.W.K.Young
 (Berk.) Petch
 (Berk.) Pilát
 (Berk.) Pilát ex Pilát
+(Berk.) Quaedvl., Verkley & Crous
 (Berk.) Quanten
 (Berk.) Quél.
 (Berk.) R.H.Petersen
 (Berk.) R.H.Petersen & Nagas.
 (Berk.) R.Heim
 (Berk.) Rajchenb.
 (Berk.) Rajchenb. & Bianchin.
@@ -1965,41 +2015,50 @@
 (Berk.) Rick
 (Berk.) Rifai
 (Berk.) Rodway
 (Berk.) Romell
 (Berk.) Rostaf.
 (Berk.) Ryvarden
 (Berk.) S.E.Carp.
+(Berk.) S.H.He & Y.C.Dai
 (Berk.) S.M.Berch
 (Berk.) Sacc.
 (Berk.) Sacc. & Traverso
 (Berk.) Samuels & Lowen
 (Berk.) Schltdl.
 (Berk.) Seaver
 (Berk.) Singer
 (Berk.) Singer & A.H.Sm.
 (Berk.) Singer, J.García & L.D.Gómez
+(Berk.) Spatafora, Kepler & C.A.Quandt
 (Berk.) Speg.
+(Berk.) Spirin & Miettinen
 (Berk.) Spooner
 (Berk.) Stalpers
 (Berk.) Syd. & P.Syd.
 (Berk.) T.Lebel
 (Berk.) T.Lebel, C.W.Dunk & T.W.May
 (Berk.) Teixeira
 (Berk.) Teng
 (Berk.) Theiss. & Syd.
+(Berk.) Thorn
 (Berk.) Thüm.
 (Berk.) Torrend
+(Berk.) Trappe & Castellano
 (Berk.) Tul. & C.Tul.
 (Berk.) Vánky
 (Berk.) Vánky, M.Lutz, & Piątek
 (Berk.) Wakef.
 (Berk.) Watling
+(Berk.) Welti & Courtec.
 (Berk.) X.L.Zeng
+(Berk.) Y.F.Sun, D.H.Costa & B.K.Cui
+(Berk.) Y.S.Chang & Kantvilas
 (Berk.) Z.T.Guo
+(Berk.) Zmitr. & Malysheva
 (Berl.) B.Sutton, Galea & T.V.Price
 (Berl.) Magnus
 (Bern.) Thomasson
 (Bernard) Playfair
 (Bernard) Willi Krieg.
 (Bernh. ex Rchb.) Fritsch
 (Bernh. ex Willd.) Edmonds
@@ -2007,14 +2066,16 @@
 (Bernh.) C.F.Reed
 (Bernh.) C.Presl
 (Bernh.) Holttum
 (Bernh.) Malme
 (Bernh.) Mett.
 (Bernh.) Müll.Berol.
 (Bernh.) Nyl.
+(Bertault & Malençon) G.Moreno & Kreisel
+(Bertault & Malençon) Malençon
 (Bertel) Eveleigh
 (Berthold) F.Schmitz
 (Berthold) P.C.Silva
 (Bertol.) Kuntze
 (Bertol.) Nees
 (Bertol.) Pax
 (Bertol.) Schauer
@@ -2048,15 +2109,17 @@
 (Bitter) Edmonds
 (Bitter) Elix
 (Bitter) Orchard
 (Bitter) Rass.
 (Bjerk.) G.Winter
 (Blackmore & Clemesha) Szlach.
 (Blackmore) D.L.Jones & M.A.Clem.
+(Blakely & C.T.White) Chippend.
 (Blakely & H.Steedman) L.A.S.Johnson & Blaxell
+(Blakely & Jacobs) D.Nicolle
 (Blakely & Jacobs) K.D.Hill & L.A.S.Johnson
 (Blakely & Jacobs) L.A.S.Johnson & K.D.Hill
 (Blakely & McKie) L.A.S.Johnson
 (Blakely & McKie) L.A.S.Johnson & Blaxell
 (Blakely & McKie) L.A.S.Johnson & K.D.Hill
 (Blakely & McKie) McGill.
 (Blakely ex C.T.White) Barlow
@@ -2067,50 +2130,53 @@
 (Blakely) Brooker & Hopper
 (Blakely) Brooker & M.W.McDonald
 (Blakely) Cameron
 (Blakely) Carolin
 (Blakely) Chippend.
 (Blakely) Christenh. & Byng
 (Blakely) Craven
+(Blakely) Crisp & L.G.Cook
 (Blakely) D.Nicolle
 (Blakely) Danser
 (Blakely) H.Eichler
 (Blakely) J.T.Hunter
 (Blakely) Jobson & P.H.Weston
 (Blakely) K.D.Hill & L.A.S.Johnson
 (Blakely) L.A.S.Johnson
 (Blakely) L.A.S.Johnson & Blaxell
 (Blakely) L.A.S.Johnson & K.D.Hill
-(Blakely) L.A.S.Johnson & K.D.Hill x Eucalyptus propinqua H.Deane & Maiden
 (Blakely) L.D.Pryor & L.A.S.Johnson ex Boomsma
 (Blakely) Parra-Os. & Ladiges
 (Blakely) Paul G.Wilson
 (Blakely) Pedley
+(Blanco) Baehni
+(Blanco) Bakh.f.
 (Blanco) Benth.
 (Blanco) Blanco
 (Blanco) H.J.Lam
 (Blanco) Harms
 (Blanco) I.M.Johnst.
 (Blanco) Kuntze
 (Blanco) Mabb.
 (Blanco) Merr.
+(Blanco) Pierre
 (Blanco) Radlk.
-(Blanco) Rintz
 (Blanco) Schindl.
 (Blanco) Verdc.
 (Blanco) de Wit
 (Blaxell) D.L.Jones & M.A.Clem.
 (Bleisch & Rabenh.) Cleve
 (Bleisch) D.G.Mann
 (Bleisch) Grunow
 (Bleisch) H.L.Sm.
 (Bleisch) Reimer
 (Bliding) H.S.Hayden, Blomster, Maggs, P.C.Silva, Stanhope & Waaland
 (Bloemb.) W.J.de Wilde & Duyfjes
-(Blume ex Blume) C.Presl
+(Blume & T.Nees) B.K.Cui, M.L.Han & Y.C.Dai
+(Blume & T.Nees) Berk.
 (Blume ex Korth.) Danser
 (Blume ex Schult. & Schult.f.) Bakh.f.
 (Blume ex Schult. & Schult.f.) Masam.
 (Blume ex Schult.f.) Hook.f.
 (Blume) A.D.Hawkes
 (Blume) A.DC.
 (Blume) A.Juss.
@@ -2147,15 +2213,14 @@
 (Blume) Danser
 (Blume) Decne.
 (Blume) Diels
 (Blume) Ding Hou
 (Blume) Domin
 (Blume) Donk
 (Blume) Druce
-(Blume) Dubard
 (Blume) Ebihara & K.Iwats.
 (Blume) Elmer
 (Blume) Endl.
 (Blume) Engl.
 (Blume) F.Muell.
 (Blume) Forman
 (Blume) Fosberg & Sachet
@@ -2238,15 +2303,14 @@
 (Blume) Skottsb.
 (Blume) Sleumer
 (Blume) Sleumer ex Jessup
 (Blume) Soják
 (Blume) Spreng.
 (Blume) T.G.Hartley
 (Blume) T.Moore
-(Blume) Teo
 (Blume) Tindale
 (Blume) Trevis.
 (Blume) Triana
 (Blume) Wangerin
 (Blume) Wedd.
 (Blume) Y.P.Ng & P.J.Cribb
 (Blume) de Laub.
@@ -2286,32 +2350,35 @@
 (Boiss.) Ewart
 (Boiss.) Hurus.
 (Boiss.) Kuntze
 (Boiss.) L.C.Wheeler
 (Boiss.) Lange
 (Boiss.) Mirb.
 (Boiss.) Pax & K.Hoffm.
-(Boiss.) Sennen & Mauriccio
+(Boiss.) Sennen & Mauricio
 (Boiss.) Stoj. & Stef.
 (Bojer ex Hook.) Raf.
+(Boland) D.Nicolle
 (Boland) Rule
 (Boldt) West & G.S.West
 (Bolt.) Fr.
 (Bolt.) Pat.
 (Bolt.) Singer
 (Bolton) Antonín
-(Bolton) De Not. & Ces.
+(Bolton) Ces. & De Not.
 (Bolton) Fr.
 (Bolton) Godfrin
 (Bolton) Gray
 (Bolton) Grev.
+(Bolton) J.S.Oliveira
 (Bolton) J.Schröt.
 (Bolton) Locq.
 (Bolton) P.Kumm.
 (Bolton) Pers.
+(Bolton) R.H.Petersen
 (Bolton) Redhead, Vilgalys & Moncalvo
 (Bolton) S.Ito
 (Bolton) Vilgalys, Hopple & Jacq.Johnson
 (Bonnem.) F.Schmitz
 (Bonord.) Demoulin
 (Bonord.) Hollós
 (Bonord.) Höhn.
@@ -2395,14 +2462,15 @@
 (Bory) Gaudich.
 (Bory) Grev.
 (Bory) Hassall
 (Bory) Hook.f.
 (Bory) Hook.f. & Harv.
 (Bory) J.Agardh
 (Bory) J.Sm.
+(Bory) K.M.Drew & Ron.Ross
 (Bory) K.W.Nam
 (Bory) Kunth
 (Bory) Kütz.
 (Bory) M.E.Ramírez & A.F.Peters
 (Bory) M.Howe
 (Bory) Menegh. ex Ralfs
 (Bory) Mont.
@@ -2439,17 +2507,16 @@
 (Bosch) Ebihara & K.Iwats.
 (Bosch) Farw.
 (Bosch) Luerss.
 (Bosch) Maiden & Betche
 (Bosch) Müll.Arg.
 (Bosch) Pic.Serm.
 (Bosch) Staiger
+(Bosw.) F.Lara, Garilleti & Goffinet
 (Bosw.) Paris
-(Boud. & Chatin) Bertault & Malençon
-(Boud. & Chatin) P.D.Orton
 (Boud. ex Cooke) Eckblad
 (Boud.) Bon
 (Boud.) Boud.
 (Boud.) Corner
 (Boud.) Juel
 (Boud.) Pat.
 (Boud.) Sacc. & Traverso
@@ -2458,15 +2525,15 @@
 (Bougher & Castellano) Gasparini
 (Bougher & T.Lebel) Justo
 (Bougher & Thiers) Halling & N.A.Fechner
 (Bougher) Bougher & Trappe
 (Bougher) Justo
 (Bougher) Peintner & M.M.Moser
 (Bougher) T.Lebel
-(Bougher, Fuhrer & E.Horak) M.M.Moser, E.Horak, Peintner & Vilgalys
+(Bougher, Fuhrer & E.Horak) Peintner, E.Horak, M.M.Moser & Vilgalys
 (Boulos) J.Kost.
 (Bourdot & Galzin) Bourdot & Galzin
 (Bourdot & Galzin) Corner
 (Bourdot & Galzin) Donk
 (Bourdot & Galzin) Hallenb.
 (Bourdot & Galzin) J.Erikss.
 (Bourdot & Galzin) Liberta
@@ -2487,77 +2554,87 @@
 (Braarud) Balech
 (Braarud) Balech & Tangen
 (Braarud) Konovalova
 (Brack.) Alderw.
 (Brack.) Bonap.
 (Brack.) Bostock
 (Brack.) C.F.Reed
+(Brack.) Ching
 (Brack.) Copel.
 (Brack.) Domin
 (Brack.) Ebihara & K.Iwats.
 (Brack.) Holttum
 (Brack.) Hook.
 (Brack.) K.U.Kramer
-(Brack.) K.U.Kramer x Lindsaea microphylla Sw.
 (Brack.) Lehtonen & Tuomisto
 (Brack.) M.Kato
+(Brack.) S.E.Fawc. & A.R.Sm.
 (Brack.) T.Moore
 (Braithw.) Loeske
 (Brako) Elix
 (Brand) Noot.
 (Brandegee) Barneby & J.W.Grimes
 (Braun) G.S.West
 (Breda de Haan) Shoemaker
 (Breda) Lindl.
 (Bref.) M.Piepenbr.
+(Bref.) McTaggart & R.G.Shivas
 (Bref.) Möller
-(Bref.) P.Syd. & Sacc.
 (Bref.) Sacc. & P.Syd.
 (Bref.) Vánky
 (Bremek. & Oberm.) Exell
 (Bremek.) Y.F.Deng
+(Bremer & Petr.) U.Braun
 (Brenan) Verdc.
+(Bres. & Henn. ex Sacc.) G.Cunn.
+(Bres. & Henn. ex Sacc.) Ryvarden
+(Bres. & Henn. ex Sacc.) Steyaert
+(Bres. & Pat.) Corner
 (Bres. ex Lloyd) Beeli
 (Bres. ex Lloyd) D.A.Reid
 (Bres.) Arnolds
 (Bres.) B.Sutton
 (Bres.) Boud.
 (Bres.) Bres.
+(Bres.) Crous
 (Bres.) D.A.Reid
 (Bres.) E.Horak
 (Bres.) Hjortstam
 (Bres.) J.Erikss.
 (Bres.) J.Erikss. & Ryvarden
 (Bres.) Jülich
 (Bres.) Jülich & Stalpers
 (Bres.) Kühner
 (Bres.) Lloyd
 (Bres.) Maire
+(Bres.) Matheny & Esteve-Rav.
 (Bres.) P.D.Orton
 (Bres.) Parmasto
 (Bres.) R.C.Harris
 (Bres.) Ryvarden
+(Bres.) S.H.He & Nakasone
 (Bres.) Sacc.
-(Bres.) Syd. & Sacc.
+(Bres.) Sacc. & P.Syd.
 (Bressan) Y.M.Chamb.
-(Breton, Bernalier, Fonty, B.Gaillard, Bonnemoy & Gouet) J.L.Li, I.B.Heath & K.J.Cheng
+(Breton, Bernalier, Bonnemoy, Fonty, B.Gaillard, & Gouet) J.L.Li, I.B.Heath & K.J.Cheng
 (Breuss) Breuss
 (Brid. ex F.Weber) Nees
 (Brid. ex Lehm. & Lindenb.) Lindenb.
 (Brid.) A.Jaeger
 (Brid.) Arn.
 (Brid.) Bach.Pyl.
 (Brid.) Besch.
 (Brid.) Blandow
 (Brid.) Brid.
 (Brid.) Broth.
 (Brid.) Bruch & Schimp.
 (Brid.) Cardot
 (Brid.) Delogne
 (Brid.) E.Britton
+(Brid.) Enroth
 (Brid.) Fransén
 (Brid.) Garov.
 (Brid.) Grout
 (Brid.) H.A.Crum
 (Brid.) Hampe
 (Brid.) Hedenäs
 (Brid.) Hook.f.
@@ -2576,37 +2653,40 @@
 (Brid.) Paris
 (Brid.) Podp.
 (Brid.) R.H.Zander
 (Brid.) Schwägr.
 (Brid.) Steud.
 (Brid.) T.J.Kop.
 (Brid.) Turton
+(Brid.) W.R.Buck, P.E.A.S.Câmara & Carv.-Silva
 (Brid.) Wijk & Margad.
 (Brieger) Dockrill
-(Brightw.) Chavez & T.R.Baumg.
 (Brightw.) Cleve
 (Brightw.) Medlin
+(Brightw.) P.A.Sims & D.M.Williams
 (Brightw.) Ralfs
 (Brightw.) Sundström
 (Brightw.) Van Heurck
 (Brinsley) D.L.Jones
 (Brinsley) D.L.Jones & M.A.Clem.
 (Briot) Zabel
 (Briq.) P.W.Michael
 (Briq.) Small
 (Brittan) Sirisena, Conran & T.D.Macfarl.
-(Britten & S.Moore ex S.Moore) B.Hyland
+(Britten & S.Moore) B.Hyland
 (Britten) Pichon
 (Brittleb. & D.B.Adam) Shoemaker
 (Britton & Killip) Stehle
 (Britzelm.) Kreisel
 (Britzelm.) Maas Geest.
 (Britzelm.) Noordel.
 (Britzelm.) Sacc.
 (Britzelm.) Singer
+(Britzelm.) W.B.Cooke
+(Britzelm.) Örstadius & E.Larss.
 (Broch) Balech
 (Broch) J.Schiller
 (Brockm.) Brockm.
 (Brond.) Cheel
 (Brond.) Cleland & Cheel
 (Brond.) Sacc.
 (Brongn. & Gris) Baill. ex Guillaumin
@@ -2625,21 +2705,22 @@
 (Brongn.) Kuntze
 (Brongn.) Lazarides
 (Brongn.) Lindl.
 (Brongn.) M.A.Clem. & D.L.Jones
 (Brongn.) Orchard
 (Brongn.) Roberty
 (Brongn.) Trin.
+(Brooker & A.R.Bean) Crisp & L.G.Cook
 (Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson
-(Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson x Corymbia tessellaris (F.Muell.) K.D.Hill & L.A.S.Johnson
+(Brooker & Dunlop) Crisp & L.G.Cook
 (Brooker & Dunlop) K.D.Hill & L.A.S.Johnson
+(Brooker & Edgecombe) Crisp & L.G.Cook
 (Brooker & Edgecombe) K.D.Hill & L.A.S.Johnson
 (Brooker & Hopper) D.Nicolle
 (Brooker & Hopper) D.Nicolle & M.E.French
-(Brooker & Hopper) D.Nicolle & M.E.French - Eucalyptus obesa Brooker & Hopper
 (Brooker & Hopper) Gosper & Hopper
 (Brooker & Hopper) M.E.French & D.Nicolle
 (Brooker & Kleinig) A.R.Bean
 (Brooker) Brooker
 (Brooker) Brooker & Hopper
 (Brooker) D.Nicolle & M.E.French
 (Brooker) L.A.S.Johnson & K.D.Hill
@@ -2652,81 +2733,78 @@
 (Brot.) R.Fern.
 (Brot.) Sweet
 (Brot.) T.W.May & A.E.Wood
 (Broth. & Geh.) Broth.
 (Broth. & Geh.) Catches.
 (Broth. & Geh.) H.A.Crum
 (Broth. & Geh.) H.Rob.
-(Broth. & Geh.) Kindb.
 (Broth. & Geh.) M.Fleisch.
 (Broth. & Geh.) Paris
 (Broth. & Geh.) Renauld
 (Broth. & Paris) I.G.Stone
 (Broth. & Paris) Thér.
+(Broth. & Paris) W.R.Buck & Ireland
 (Broth. & Watts) B.C.Tan, H.P.Ramsay & W.B.Schofield
 (Broth. & Watts) Broth.
 (Broth. & Watts) Brugg.-Nann., Pursell & Z.Iwats.
 (Broth. & Watts) I.G.Stone
 (Broth.) A.J.Shaw
 (Broth.) B.C.Tan, H.P.Ramsay & W.B.Schofield
 (Broth.) B.C.Tan, W.B.Schofield & H.P.Ramsay
 (Broth.) Broth.
 (Broth.) Broth. ex Paris
 (Broth.) Cardot
 (Broth.) Crosby
 (Broth.) Dixon
 (Broth.) Fife
-(Broth.) Goffinet
 (Broth.) Granzow
 (Broth.) H.A.Crum
 (Broth.) H.A.Mill.
 (Broth.) H.Rob.
 (Broth.) I.G.Stone
 (Broth.) I.G.Stone & G.A.M.Scott
 (Broth.) Ireland
 (Broth.) J.-P.Frahm
 (Broth.) J.R.Spence & H.P.Ramsay
+(Broth.) Jan Kučera & Ignatov
 (Broth.) Kindb.
 (Broth.) M.Fleisch.
 (Broth.) Manuel
 (Broth.) Müll.Hal.
 (Broth.) Ochyra & J.Muñoz
 (Broth.) Paris
 (Broth.) Paris & Schimp.
+(Broth.) R.H.Zander
 (Broth.) Renauld
-(Broth.) Rodway
 (Broth.) Sainsbury
 (Broth.) Touw
 (Broth.) W.R.Buck
 (Broth.) W.R.Buck & B.C.Tan
 (Broth.) W.R.Buck & Vitt
 (Broth.) Watts & Whitel.
 (Broth.) Wijk & Margad.
 (Broth.) Wijk & Margad. ex D.N.McVean
+(Broth.) Z. Iwats. & Tad. Suzuki
 (Brouss. ex Willd.) Assenov
 (Brownsey & Lovis) Christenh.
 (Brownsey) Ogle
 (Bruch & Schimp.) De Not.
 (Bruch & Schimp.) E.J.Craig
-(Bruch & Schimp.) Hampe
 (Bruch & Schimp.) J.R.Spence & H.P.Ramsay
 (Bruch & Schimp.) Limpr.
 (Bruch & Schimp.) Lindb.
 (Bruch & Schimp.) Loeske
 (Bruch & Schimp.) Mitt.
 (Bruch & Schimp.) Müll.Hal.
 (Bruch & Schimp.) Regel
 (Bruch & Schimp.) Schimp.
 (Bruch & Schimp.) Schwägr.
 (Bruch & Schimp.) Warnst.
 (Bruch & Schimp.) Zanten
-(Bruch ex De Not.) J.R.Spence
-(Bruch ex De Not.) Kindb.
 (Bruch) Broth.
-(Brumm.) Eckblad
 (Brun & Hérib.) Playfair
 (Brun & Héribaud-Joseph) Hust.
 (Brun) Playfair
 (Brun) R.Ross
 (Brun) Simonsen
 (Brunaud) Gruyter, Aveskamp & Verkley
 (Bruner) Gryzenh. & M.J.Wingf.
@@ -2808,53 +2886,48 @@
 (Buch.-Ham. ex DC.) Hassk.
 (Buch.-Ham. ex Graebn.) C.D.K.Cook & M.S.Nicholls
 (Buch.-Ham. ex Graebn.) H.Hara
 (Buch.-Ham. ex Roxb.) Dalzell & A.Gibson
 (Buch.-Ham. ex Roxb.) Koehne
 (Buch.-Ham.) T.Nees & C.H.Eberm.
 (Buchanan) Anderb.
-(Buchanan) B.G.Briggs & Ehrend.
 (Buchanan) Cockayne
 (Buchanan) J.M.Ward & Breitw.
 (Buchanan) Kirk
 (Buchanan) L.B.Moore
 (Buchanan) S.W.L.Jacobs & J.Everett
 (Buchenau) Buchenau
 (Buchenau) Edgar
 (Buchenau) H.Nordensk.
 (Buchenau) Ostenf.
 (Buchenau) Snogerup
 (Buchenau) Vierh.
 (Buckley) R.D.Webster
 (Buckley) S.T.Blake
 (Buffham) Batters
+(Bugnic.) Manamgoda, L.Cai & K.D.Hyde
 (Bugnic.) Subram. & B.L.Jain
 (Bull. & St.- Amans) Maire
 (Bull. & Vent.) A.F.M.Reijnders
 (Bull. & Vent.) Harmaja
 (Bull. & Vent.) P.Kumm.
 (Bull. & Vent.) Quél.
 (Bull. & Vent.) Sacc.
 (Bull. & Vent.) Singer
-(Bull. : Fr.) Cooke
-(Bull. : Fr.) Fr.
-(Bull. : Fr.) P.Karst.
-(Bull. : Fr.) Quel.
-(Bull. : Fr.) Raithelh.
-(Bull. ex Pers. : Fr.) P.Karst.
 (Bull.) A.Pearson & Dennis
 (Bull.) Antonín, Halling & Noordel.
+(Bull.) B.K.Cui, M.L.Han & Y.C.Dai
 (Bull.) Baral
 (Bull.) Bataille
 (Bull.) Berk.
 (Bull.) Bon
 (Bull.) Boud.
 (Bull.) Chevall.
 (Bull.) Cooke
-(Bull.) DC. & Lam.
+(Bull.) DC.
 (Bull.) Donk
 (Bull.) Duby
 (Bull.) Fayod
 (Bull.) Fr.
 (Bull.) Fuckel
 (Bull.) Gillet
 (Bull.) Gray
@@ -2874,27 +2947,29 @@
 (Bull.) Locq.
 (Bull.) Lázaro Ibiza
 (Bull.) M.L.Farr
 (Bull.) M.M.Moser
 (Bull.) Maas Geest.
 (Bull.) Maire
 (Bull.) Massee
+(Bull.) Matheny & Esteve-Rav.
 (Bull.) Morgan
 (Bull.) Murrill
 (Bull.) Nees
 (Bull.) P.D.Orton
 (Bull.) P.Karst.
 (Bull.) P.Kumm.
 (Bull.) Pat.
 (Bull.) Pers.
 (Bull.) Pilát
 (Bull.) Quél.
 (Bull.) Raithelh.
 (Bull.) Rea
 (Bull.) Redhead
+(Bull.) Redhead, Moncalvo, Vilgalys, Desjardin & B.A.Perry
 (Bull.) Redhead, Vilgalys & Moncalvo
 (Bull.) Ricken
 (Bull.) Rostaf.
 (Bull.) Rostaf. ex Lister
 (Bull.) Roze
 (Bull.) S.E.Carp.
 (Bull.) Sacc.
@@ -2954,14 +3029,15 @@
 (Burm.f.) Fosberg
 (Burm.f.) G.D.Rowley
 (Burm.f.) Goldblatt
 (Burm.f.) H.S.Irwin & Barneby
 (Burm.f.) Hallier f.
 (Burm.f.) Hiern
 (Burm.f.) Hochr.
+(Burm.f.) Hoffmanns.
 (Burm.f.) J.C.Manning & Goldblatt
 (Burm.f.) J.Kern
 (Burm.f.) J.R.I.Wood & Scotland
 (Burm.f.) Juss. ex Schult.
 (Burm.f.) K.L.Gibbons
 (Burm.f.) Ker Gawl.
 (Burm.f.) Kral
@@ -2987,15 +3063,14 @@
 (Burm.f.) Spreng.
 (Burm.f.) Stapf & C.E.Hubb.
 (Burm.f.) Sw.
 (Burm.f.) T.Anderson
 (Burm.f.) T.Yamaz.
 (Burm.f.) Trin. ex Hensch.
 (Burm.f.) Underw.
-(Burm.f.) Underw. x Sticherus flabellatus var. compactus (C.T.White & Goy) D.A.Sm.
 (Burm.f.) Wall. ex Nees
 (Burm.f.) Walp.
 (Burm.f.) Wannan, W.R.Barker, Y.S.Liang
 (Burm.f.) Willd.
 (Burnat) Gürke
 (Burnat) P.W.Ball & Heywood
 (Burnside) Skou
@@ -3086,14 +3161,15 @@
 (C.A.Gardner) Silba
 (C.A.Gardner) T.C.Wilson & Henwood
 (C.A.Gardner) Trudgen
 (C.A.Mey.) Benth.
 (C.A.Mey.) Meisn.
 (C.A.Mey.) Soják
 (C.Agardh ex Gomont) Anagn. & Komárek
+(C.Agardh ex Gomont) Strunecký, Bohunická, J.R.Johans. & Komárek
 (C.Agardh ex Sond.) J.Agardh
 (C.Agardh ex Sond.) Kuntze
 (C.Agardh ex Sond.) Kütz.
 (C.Agardh) Ambronn
 (C.Agardh) Anagn.
 (C.Agardh) Anagn. & Komárek
 (C.Agardh) Aresch.
@@ -3128,29 +3204,30 @@
 (C.Agardh) Gaillon
 (C.Agardh) Garbary & J.T.Harper
 (C.Agardh) Gomont
 (C.Agardh) Grev.
 (C.Agardh) Grunow
 (C.Agardh) Grunow ex Hust.
 (C.Agardh) Hamel
-(C.Agardh) Hariot
+(C.Agardh) Har.
 (C.Agardh) Harv.
 (C.Agardh) Hassall ex Bornet & Flahault
 (C.Agardh) Heiberg
 (C.Agardh) Hollenb.
 (C.Agardh) Hook.f.
 (C.Agardh) Hook.f. & Harv.
 (C.Agardh) J.Agardh
 (C.Agardh) Kajimura
 (C.Agardh) Kuntze
 (C.Agardh) Kylin
 (C.Agardh) Kütz.
 (C.Agardh) L.E.Phillips
 (C.Agardh) Lange-Bert.
 (C.Agardh) Levkov
+(C.Agardh) Lyngb.
 (C.Agardh) M.Howe
 (C.Agardh) M.J.Wynne
 (C.Agardh) Menegh.
 (C.Agardh) Min-Thein & Womersley
 (C.Agardh) Mont.
 (C.Agardh) Mont. & Bory
 (C.Agardh) Mont. ex Harv.
@@ -3168,15 +3245,14 @@
 (C.Agardh) Sond.
 (C.Agardh) Spreng.
 (C.Agardh) Suhr
 (C.Agardh) Trevis.
 (C.Agardh) Van Heurck
 (C.Agardh) Van Hoek
 (C.Agardh) Vickers
-(C.Agardh) W.Sm.
 (C.Agardh) Weber Bosse
 (C.Agardh) Yamada
 (C.Agardh) Yendo
 (C.Agardh) Zanardini
 (C.B.Clarke ex Domin) Kük.
 (C.B.Clarke) Benth.
 (C.B.Clarke) C.A.Gardner
@@ -3208,23 +3284,26 @@
 (C.Bab.) D.J.Galloway & Hafellner
 (C.Bab.) Gotth.Schneid.
 (C.Bab.) J.S.Murray
 (C.Bab.) M.Schultz
 (C.Bab.) Malme
 (C.Bab.) Müll.Arg.
 (C.Bab.) P.James
+(C.Bab.) Rostaf.
 (C.Bab.) Sato
 (C.Bab.) Stirt.
 (C.Bab.) Wedin
 (C.Bailey) F.Hanb. ex A.K.Jacks.
 (C.Bernard) Alcorn
 (C.Bernard) Playfair
 (C.Bernard) S.H.Li
 (C.Bernard) Thomasson
 (C.Bernard) Willi Krieg.
+(C.Booth & Shipton) Arx
+(C.Booth & Shipton) X.Wei Wang & Crous
 (C.Brockmann) Witkowski
 (C.C.Gmel.) Benth. & Hook.f.
 (C.C.Gmel.) Palla
 (C.C.Jao) Garbary & Rueness
 (C.C.Jao) Papenf.
 (C.C.Jao) Woelk.
 (C.Chr.) C.Chr.
@@ -3232,14 +3311,16 @@
 (C.Chr.) C.F.Reed
 (C.Chr.) Ching
 (C.Chr.) Hovenkamp
 (C.Chr.) M.D.Turner & R.A.White
 (C.Chr.) Tindale
 (C.Chr.) W.R.B.Oliv.
 (C.Cusset & G.Cusset) M.Kato, Y.Kita & Koi
+(C.D.Moon & Schardl) Leuchtm.
+(C.D.Moon, C.O.Miles & Schardl) Leuchtm. & Schardl
 (C.DC.) Kuntze
 (C.E.Hubb.) Lazarides
 (C.E.Hubb.) P.M.Peterson & Saarela
 (C.E.Hubb.) Pilg.
 (C.E.Hubb.) R.L.Barrett & P.M.Peterson
 (C.E.Hubb.) Roberty
 (C.E.Hubb.) S.T.Blake
@@ -3263,18 +3344,19 @@
 (C.H.G.Pouchet) Cachon & Cachon-Enj.
 (C.H.G.Pouchet) F.Gómez
 (C.H.G.Pouchet) F.Gómez, D.Moreira & López-García
 (C.H.G.Pouchet) F.Schütt
 (C.H.G.Pouchet) Gourret
 (C.H.G.Pouchet) J.D.Dodge
 (C.H.G.Pouchet) J.Schiller
-(C.H.G.Pouchet) Jörg.
+(C.H.G.Pouchet) Jørg.
 (C.H.G.Pouchet) Kof.
 (C.H.G.Pouchet) Kof. & Swezy
 (C.H.G.Pouchet) Lemmerm.
+(C.I.Weber) Hasle
 (C.J.Gould) Oberw. & Bandoni
 (C.J.Webb) Breitw. & J.M.Ward
 (C.Janisch ex Grunow) Hust.
 (C.Janisch) Cleve
 (C.Janisch) Grunow
 (C.Janisch) S.Blanco
 (C.K.Allen) Kosterm.
@@ -3322,29 +3404,29 @@
 (C.Massal.) Schiffn. & Gottsche
 (C.Massal.) Steph.
 (C.Moore & F.Muell.) Becc.
 (C.Moore & F.Muell.) Benth.
 (C.Moore & F.Muell.) C.Moore & F.Muell.
 (C.Moore & F.Muell.) Drude & H.Wendl.
 (C.Moore & F.Muell.) F.Muell.
+(C.Moore & F.Muell.) F.Muell. ex Benth.
 (C.Moore & F.Muell.) H.Wendl. & Drude
 (C.Moore & F.Muell.) H.Wendl. ex Anon.
 (C.Moore & F.Muell.) Harms
 (C.Moore & F.Muell.) Hutch.
 (C.Moore & F.Muell.) Klatt
 (C.Moore & F.Muell.) Kuntze
 (C.Moore & F.Muell.) L.A.S.Johnson & B.G.Briggs
 (C.Moore & F.Muell.) O.F.Cook
 (C.Moore & F.Muell.) R.Vig.
 (C.Moore & F.Muell.) Regel
 (C.Moore & F.Muell.) Seem.
 (C.Moore & F.Muell.) T.G.Hartley
 (C.Moore & F.Muell.) W.R.B.Oliv.
 (C.Moore ex F.Muell.) F.M.Bailey
-(C.Moore ex J.Sm.) Christenh. x Blechnum rupestre (Kaulf. ex Link) Christenh.
 (C.Moore) A.Terracc.
 (C.Moore) C.Moore
 (C.Moore) D.J.Dixon
 (C.Moore) J.Schust.
 (C.Moore) L.A.S.Johnson
 (C.Moore) Maiden & Betche
 (C.Moore) P.S.Green
@@ -3428,14 +3510,15 @@
 (C.T.White & W.D.Francis) Christenh. & Byng
 (C.T.White & W.D.Francis) Gill.K.Br. & Bayly
 (C.T.White & W.D.Francis) Harms
 (C.T.White & W.D.Francis) I.C.Nielsen
 (C.T.White & W.D.Francis) L.S.Sm.
 (C.T.White & W.D.Francis) P.Royen
 (C.T.White & W.D.Francis) Pedley
+(C.T.White & W.D.Francis) Peter G.Wilson
 (C.T.White & W.D.Francis) S.T.Blake
 (C.T.White & W.D.Francis) Swenson
 (C.T.White & W.D.Francis) Swenson, Bartish & Munzinger
 (C.T.White & W.D.Francis) T.G.Hartley
 (C.T.White ex S.T.Blake) Craven
 (C.T.White) A.J.Scott
 (C.T.White) A.V.Bobrov & Melikyan
@@ -3484,46 +3567,39 @@
 (C.T.White) Paul G.Wilson
 (C.T.White) Pedley
 (C.T.White) Peter B.Adams
 (C.T.White) Polhill
 (C.T.White) Quinn
 (C.T.White) R.A.Howard
 (C.T.White) R.J.F.Hend.
+(C.T.White) R.W.Bouman
 (C.T.White) Rados.
 (C.T.White) S.T.Reynolds
 (C.T.White) S.T.Reynolds & R.J.F.Hend.
 (C.T.White) Sleumer
 (C.T.White) Stearn
 (C.T.White) Swenson, Bartish & Munzinger
 (C.T.White) T.G.Hartley
 (C.T.White) Toelken
 (C.T.White) Trudgen
 (C.T.White) Upton
 (C.W.Dodge & Rudolph) Øvstedal
-(C.W.Dodge & Zeller) A.H.Sm.
-(C.W.Dodge & Zeller) E.Horak
-(C.W.Dodge & Zeller) G.Cunn.
-(C.W.Dodge & Zeller) G.W.Beaton, Pegler & T.W.K.Young
-(C.W.Dodge & Zeller) Peintner & M.M.Moser
-(C.W.Dodge & Zeller) Singer & A.H.Sm.
 (C.W.Dodge) D.Hawksw. & Iturr.
 (C.W.Dodge) D.J.Galloway
 (C.W.Dodge) D.J.Galloway & P.James
 (C.W.Dodge) Diederich
-(C.W.Dodge) Filson
 (C.W.Dodge) H.Mayrhofer & P.M.McCarthy
 (C.W.Dodge) Hale
 (C.W.Dodge) Hertel
 (C.W.Dodge) I.M.Lamb
 (C.W.Dodge) J.W.Groves & Skolko
 (C.W.Dodge) Krog & Swinscow
 (C.W.Dodge) Ohlsson
 (C.W.Dodge) P.M.Jørg. & D.J.Galloway
 (C.W.Dodge) S.Stenroos & Ahti
-(C.W.Dodge) Serus.
 (C.W.Dodge) Sérus.
 (C.W.Dodge) Wedin
 (C.W.Dodge) Øvstedal
 (C.W.Thomson) Haeckel
 (C.Walter) D.L.Jones & M.A.Clem.
 (C.Wright) Killip
 (Cabejsz.) Körner
@@ -3537,16 +3613,22 @@
 (Cambess.) Hiern ex Vidal
 (Cand. & Sulmont) Unter. & F.A.Naveau
 (Cardot) M.Fleisch.
 (Cardot) S.P.Churchill & W.R.Buck
 (Carlquist) Wege
 (Carmich. ex Berk.) J.Agardh
 (Carmich. ex Harv.) Kornmann
+(Carnegie & Beilharz) Carnegie & Crous
+(Carnegie & G.S.Pegg) Crous & Carnegie
+(Carnegie & G.S.Pegg) Quaedvl. & Crous
+(Carnegie & Keane) Quaedvl. & Crous
 (Carnegie & M.J.Wingf.) Carnegie & M.J.Wingf.
 (Carnegie) Carnegie
+(Carnegie) U.Braun, C.Nakash., Videira & Crous
+(Carnegie) Videira & Crous
 (Carnegie, Andjic & P.A.Barber) Carnegie, Andjic & P.A.Barber
 (Carolin) Carolin
 (Carolin) K.A.Sheph.
 (Carrick) B.J.Conn
 (Carrick) Christenh. & Byng
 (Carrington & Pearson) Bastow
 (Carrington & Pearson) E.A.Hodgs. & Allison
@@ -3594,15 +3676,14 @@
 (Castrac.) H.Perag.
 (Castrac.) Hust.
 (Castrac.) L.Mangin
 (Castrac.) Lange-Bert.
 (Castrac.) R.W.Jord. & Ligowski
 (Castrac.) Round
 (Catches. & I.G.Stone) I.G.Stone
-(Catches. ex J.R.Spence & H.P.Ramsay) J.R.Spence & H.P.Ramsay
 (Catches.) Catches.
 (Catches.) Fife & Seppelt
 (Catches.) I.G.Stone
 (Catt.) Penz.
 (Cav.) Baker
 (Cav.) Benth.
 (Cav.) Benth. & Hook.f. ex A.Gray
@@ -3616,15 +3697,14 @@
 (Cav.) C.Norman
 (Cav.) C.Presl
 (Cav.) Christenh. & Byng
 (Cav.) DC.
 (Cav.) Dalzell & A.Gibson
 (Cav.) Desv.
 (Cav.) Domin
-(Cav.) Domin x Persoonia linearis Andrews
 (Cav.) Druce
 (Cav.) Dryand.
 (Cav.) F.Muell.
 (Cav.) Farw.
 (Cav.) Fern.-Vill.
 (Cav.) G.Don
 (Cav.) G.M.Thomson
@@ -3639,26 +3719,25 @@
 (Cav.) Kuntze
 (Cav.) Luerss.
 (Cav.) Maiden & Betche
 (Cav.) Melvaine
 (Cav.) Noot.
 (Cav.) Nutt.
 (Cav.) P.Beauv.
+(Cav.) P.M.Peterson, Romasch. & Soreng
 (Cav.) Pennell
 (Cav.) Pers.
 (Cav.) Pic.Serm.
 (Cav.) Poir.
 (Cav.) R.Br.
-(Cav.) R.Br. var. caudata x Doodia caudata var. laminosa F.Muell.
-(Cav.) R.Br. x Doodia linearis C.Moore ex J.Sm.
-(Cav.) R.Br. x Doodia media R.Br.
 (Cav.) Roem. & Schult.
 (Cav.) S.T.Blake
 (Cav.) Sendtn.
 (Cav.) Sims
+(Cav.) Soldano, Banfi & Galasso
 (Cav.) Spreng.
 (Cav.) Sw.
 (Cav.) Sweet
 (Cav.) Tirveng.
 (Cav.) Trin. ex Steud.
 (Cav.) Ulbr.
 (Cav.) Underw.
@@ -3668,14 +3747,15 @@
 (Cavara) Cavara
 (Cavara) Corner
 (Cavara) R.H.Petersen
 (Cedergren) T.Bando
 (Celak.) B.Schmid
 (Celan) Santel.
 (Cels ex Link) DC.
+(Ces. & De Not.) De Not.
 (Ces.) Ching
 (Ces.) G.H.Sung, J.M.Sung, Hywel-Jones & Spatafora
 (Ces.) Holttum
 (Ces.) Rostaf.
 (Ces.) Y.M.Ju & J.D.Rogers
 (Ces.) Y.M.Ju, J.D.Rogers & H.M.Hsieh
 (Chaillet ex Fr.) Boidin
@@ -3701,47 +3781,56 @@
 (Champ. ex Benth.) Benth.
 (Champ. ex Benth.) Domin
 (Chapm.) Fernald
 (Chapm.) R.T.Clausen
 (Chapm.) Small
 (Chase) Henrard
 (Chase) M.R.Hend.
+(Chatin & Boud.) Malençon & Bertault
+(Chatin & Boud.) P.D.Orton
 (Chauv. ex Duby) Harv.
 (Chauv. ex Duby) J.Agardh
 (Chauv. ex Duby) Kütz.
 (Chauv. ex Mont.) J.Agardh
 (Chauv.) Kütz.
 (Chauv.) V.May
 (Chauv.) Zanardini
 (Cheel) B.G.Briggs
 (Cheel) Cheel
 (Cheel) Craven
 (Cheel) Duretto & Heslewood
 (Cheel) J.H.Willis
 (Cheel) Joy Thomps.
+(Cheel) Peter G.Wilson
 (Cheeseman) Allan
 (Cheeseman) Allan & Jansen
 (Cheeseman) D.L.Jones & M.A.Clem.
 (Cheeseman) Frodin
 (Cheeseman) Heads
 (Cheeseman) N.Pfeiff.
 (Cheeseman) Ornduff
 (Cheeseman) Rupp
 (Cheeseman) Szlach.
 (Cheeseman) W.M.Curtis
+(Cheew. & Crous) Chen Chen, Verkley & Crous
+(Cheew. & Crous) X.L.Fan & Crous
+(Cheew., Summerell & Crous) Chen Chen, Verkley & Crous
+(Cheew., Summerell & Crous) Crous
 (Chev.) Arnold
 (Chev.) Zahlbr.
 (Ching) Ching
 (Ching) J.P.Roux
 (Chinnock & J.G.West) Hershk.
 (Chinnock) A.R.Field
 (Chinnock) R.Fowler
 (Chippend.) Brooker
+(Chippend.) Crisp & L.G.Cook
 (Chippend.) Govaerts
 (Chippend.) Parra-Os. & Ladiges
+(Chodat & F.Chodat) Komárek
 (Chodat & Hassl.) Mohlenbr.
 (Chodat) Bourr.
 (Chodat) Chodat
 (Chodat) G.M.Sm.
 (Chodat) Iltis
 (Chodat) Komárek & Hindak
 (Chodat) Lemmerm.
@@ -3771,75 +3860,83 @@
 (Christoph.) T.G.Hartley
 (Chrtek & Chrtkova) J.P.Bailey
 (Cibot ex L.f.) Fr.
 (Cienk.) A.R.Loebl. & Tappan
 (Cienk.) Kent
 (Cienk.) Scherff.
 (Cif. & Ashford) Langeron & Guerra
-(Cif. & Gonz.Frag.) M.B.Ellis
 (Cirillo) Engl.
 (Clap. & J.Lachm.) Balech
 (Clap. & J.Lachm.) Buetschli
 (Clap. & J.Lachm.) Diesing
 (Clap. & J.Lachm.) F.Gómez
 (Clap. & J.Lachm.) F.Gómez, D.Moreira & López-García
 (Clap. & J.Lachm.) F.Stein
-(Clap. & J.Lachm.) Jörg.
+(Clap. & J.Lachm.) Jørg.
 (Clap. & J.Lachm.) Kof. & J.R.Michener
 (Clap. & J.Lachm.) Schröd.
 (Clarion ex P.Beauv.) Hook.f.
 (Clauzade & Cl.Roux) Hafellner
 (Clayton) Soreng, L.J.Gillespie & S.W.L.Jacobs
 (Cleland & Cheel) C.J.Sheph.
 (Cleland & Cheel) Cleland
 (Cleland & Cheel) D.A.Reid
 (Cleland & Cheel) E.-J.Gilbert
 (Cleland & Cheel) E.Horak
 (Cleland & Cheel) Grgur.
+(Cleland & Cheel) Liimat. & Niskanen
 (Cleland & Cheel) R.H.Petersen
 (Cleland & Cheel) Singer
 (Cleland & Cheel) Southcott
+(Cleland & Cheel) T.Lebel
 (Cleland & G.Cunn.) M.M.Moser
 (Cleland & G.Cunn.) Peintner & M.M.Moser
-(Cleland & J.R.Harris) Grgur.
 (Cleland & J.R.Harris) T.W.May
+(Cleland & Rodway) D.A.Reid
+(Cleland & Rodway) P.K.Buchanan & Ryvarden
+(Cleland & Rodway) Ryvarden
+(Cleland & Rodway) Y.C.Dai
+(Cleland) A.M.Young
 (Cleland) Bougher & Matheny
 (Cleland) Bresinsky & Jarosch
 (Cleland) C.J.Sheph. & Totterdell
 (Cleland) Cleland
 (Cleland) Corner
-(Cleland) D.A.Reid
+(Cleland) D.A.Reid & E.Horak
 (Cleland) Desjardin, Halling & B.A.Perry
 (Cleland) E.-J.Gilbert
 (Cleland) E.Horak
-(Cleland) E.Horak & D.A.Reid
-(Cleland) E.J.Gilbert
 (Cleland) E.M.Newman
 (Cleland) Eygelsh.
 (Cleland) G.Cunn.
 (Cleland) G.Stev.
 (Cleland) Garrido
 (Cleland) Grgur.
+(Cleland) Guzmán, Bandala & Montoya
+(Cleland) J.A.Cooper
 (Cleland) J.A.Simpson & Grgur.
+(Cleland) J.S.Oliveira
 (Cleland) K.Syme
-(Cleland) Lutzoni, Redhead, Moncalvo & Vilgalys
 (Cleland) M.M.Moser
 (Cleland) M.M.Moser & E.Horak
-(Cleland) Montoya, Guzmán & Bandala
+(Cleland) Matheny & Bougher
+(Cleland) Niskanen & Liimat.
 (Cleland) P.K.Buchanan & Ryvarden
 (Cleland) R.H.Petersen
+(Cleland) R.H.Petersen & Desjardin
 (Cleland) R.H.Petersen & Kovalenko
 (Cleland) R.Heim
 (Cleland) Redhead & Ginns
 (Cleland) Redhead & Kuyper
 (Cleland) Redhead, Lutzoni, Moncalvo & Vilgalys
 (Cleland) Singer
 (Cleland) Sk.Moore & O'Sullivan
 (Cleland) T.H.Li & Watling
 (Cleland) T.W.May & A.E.Wood
+(Cleland) Verbeken
 (Cleland) Watling
 (Cleland) Watling & N.M.Greg.
 (Clemente) C.Agardh
 (Clemente) Cremades
 (Clemente) Kütz.
 (Clemente) M.J.Wynne
 (Clemesha) Clemesha
@@ -3861,57 +3958,55 @@
 (Cleve) Gran
 (Cleve) Grunow
 (Cleve) Hallegr. & Huisman
 (Cleve) Hasle
 (Cleve) Heiden
 (Cleve) Hendey
 (Cleve) Hust.
-(Cleve) Jörg.
+(Cleve) Jørg.
 (Cleve) Krammer
 (Cleve) Levkov
 (Cleve) Mereschk.
 (Cleve) P.C.Silva
 (Cleve) P.Lundell
 (Cleve) Perag.
 (Cleve) Playfair
 (Cleve) Poulin & Cardinal
 (Cleve) Reimer
 (Cleve) Simonsen
 (Cleve) Witkowski, Lange-Bert. & Metzeltin
 (Cleve) Wittr.
 (Cobb) L. Ling
 (Cobb) L.Ling
+(Cobb) McTaggart & R.G.Shivas
 (Cobb) Sacc.
 (Cobb) Vánky
 (Cockayne) P.H.Raven & Engelhorn
 (Cogn.) F.M.Bailey
 (Cogn.) Kuntze
 (Cogn.) Mansf.
 (Cohn ex Gomont) J.Kost.
 (Cohn) Fresen.
 (Cohn) Playfair
 (Cohn) Sacc. & Trotter
+(Cohn) Schipper & Stalpers
 (Cohn) Schmidle
 (Cohn) Seligo
-(Cohn) Stalpers & Schipper
 (Cohn) Vuill.
 (Coker & Couch) Guzmán
 (Coker) Corner
 (Coker) R.H.Petersen
 (Coker) Schild
 (Colebr. ex G.Don) F.Muell.
 (Colebr.) A.Gray
 (Colebr.) Kuntze
 (Colebr.) Miers ex Hook.f. & Thomson
 (Colenso) Alston
 (Colenso) Brownlie
 (Colenso) Brownsey
-(Colenso) Brownsey x Asplenium flaccidum G.Forst.
-(Colenso) Brownsey x Asplenium hookerianum Colenso
-(Colenso) Brownsey x Asplenium obtusatum subsp. northlandicum Brownsey
 (Colenso) C.Chr.
 (Colenso) Cheeseman
 (Colenso) Copel.
 (Colenso) Diels
 (Colenso) Domin
 (Colenso) E.A.Hodgs.
 (Colenso) E.D.Cooper
@@ -3928,14 +4023,15 @@
 (Colenso) Pax & K.Hoffm.
 (Colenso) Prosk.
 (Colenso) R.M.Schust.
 (Colenso) Rodway
 (Colenso) Steph.
 (Colenso) T.C.Chambers
 (Colenso) T.J.Kop.
+(Colenso) T.J.Kop. & Y.Sun
 (Colenso) Tindale
 (Colenso) Wedin
 (Colla) Baker
 (Colla) Benth.
 (Colla) G.Don
 (Colla) Hewson
 (Colla) Raf.
@@ -3949,133 +4045,142 @@
 (Collins) Papenf.
 (Collins) Sauv.
 (Collins) W.R.Taylor, A.B.Joly & Bernat.
 (Collins) Woelk.
 (Colsm.) Alston
 (Colsm.) Pennell
 (Colsm.) Spreng.
-(Comm. ex DC.) Engl.
 (Const.) M.W.Dick
 (Const.) Sparrow
+(Contu) Niskanen & Liimat.
 (Cooke & Balf.f.) G.Lister
 (Cooke & Balf.f.) Lister
 (Cooke & Ellis) J.E.Wright
 (Cooke & Ellis) M.B.Ellis
 (Cooke & Ellis) Sacc.
 (Cooke & Ellis) Seaver
 (Cooke & Harkn.) Subram.
-(Cooke & Kalchbr.) Theiss.
-(Cooke & Massee ex Cooke) J.Lloyd
 (Cooke & Massee) A.H.Sm.
 (Cooke & Massee) A.H.Sm. & Singer
 (Cooke & Massee) A.M.Young
 (Cooke & Massee) Aberdeen
 (Cooke & Massee) Ahmad
 (Cooke & Massee) Arx
 (Cooke & Massee) Arx & E.Müll.
 (Cooke & Massee) B.Sutton
+(Cooke & Massee) B.Sutton & H.J.Swart
+(Cooke & Massee) Beilharz & Pascoe
 (Cooke & Massee) Bougher & K.Syme
-(Cooke & Massee) C.W.Dodge & Zeller
-(Cooke & Massee) Castellano, Trappe & Amar.
+(Cooke & Massee) Callan & J.D.Rogers
 (Cooke & Massee) Cleland
 (Cooke & Massee) Cleland & Cheel
 (Cooke & Massee) Cooke
 (Cooke & Massee) Cooke & Massee
+(Cooke & Massee) Crous
+(Cooke & Massee) Crous & Carnegie
 (Cooke & Massee) Crous & U.Braun
-(Cooke & Massee) Crous, B.Sutton & F.A.Ferreira
+(Cooke & Massee) Crous, F.A.Ferreira & B.Sutton
 (Cooke & Massee) D.A.Reid
 (Cooke & Massee) De Toni
 (Cooke & Massee) Dietel
 (Cooke & Massee) Dyko & B.Sutton
 (Cooke & Massee) E.-J.Gilbert
 (Cooke & Massee) E.Fisch.
 (Cooke & Massee) E.Horak
 (Cooke & Massee) G.Cunn.
 (Cooke & Massee) H.J.Swart
-(Cooke & Massee) H.J.Swart & B.Sutton
 (Cooke & Massee) Hansf.
 (Cooke & Massee) Henn.
 (Cooke & Massee) Hollós
 (Cooke & Massee) Höhn.
-(Cooke & Massee) J.D.Rogers & Callan
 (Cooke & Massee) J.N.Mill.
-(Cooke & Massee) J.Walker, Pascoe & B.Sutton
+(Cooke & Massee) J.Walker, B.Sutton & Pascoe
 (Cooke & Massee) Jülich
 (Cooke & Massee) Karak.
 (Cooke & Massee) Kukkonen
 (Cooke & Massee) Kuntze
 (Cooke & Massee) L.Holm
 (Cooke & Massee) L.Ling
 (Cooke & Massee) Lloyd
 (Cooke & Massee) Lloyd ex Sacc. & Trotter
 (Cooke & Massee) M.B.Ellis
 (Cooke & Massee) Magnus
 (Cooke & Massee) Mains
 (Cooke & Massee) Massee
 (Cooke & Massee) McAlpine
 (Cooke & Massee) McLennan ex Trappe, Kovács & Claridge
+(Cooke & Massee) McTaggart & R.G.Shivas
 (Cooke & Massee) Minter
 (Cooke & Massee) Nag Raj
+(Cooke & Massee) Nag Raj & W.B.Kendr.
+(Cooke & Massee) Núñez & Ryvarden
 (Cooke & Massee) P.Joly
 (Cooke & Massee) P.M.D.Martin
 (Cooke & Massee) P.Syd. & Theiss.
-(Cooke & Massee) Pascoe & Beilharz
 (Cooke & Massee) Pegler
 (Cooke & Massee) Peintner & M.M.Moser
 (Cooke & Massee) Petch
+(Cooke & Massee) Pintos & P.Alvarado
 (Cooke & Massee) Priest
 (Cooke & Massee) R.H.Petersen
 (Cooke & Massee) R.Sant.
 (Cooke & Massee) R.T.Baker
 (Cooke & Massee) Rick
 (Cooke & Massee) Rodway
 (Cooke & Massee) Rossman
-(Cooke & Massee) Ryvarden & Núñez
+(Cooke & Massee) Rossman & W.C.Allen
 (Cooke & Massee) Sacc.
 (Cooke & Massee) Savile
 (Cooke & Massee) Seifert
 (Cooke & Massee) Sheng H.Wu
 (Cooke & Massee) Sherwood
 (Cooke & Massee) Singer
 (Cooke & Massee) Spooner & Bridge
 (Cooke & Massee) Syd.
 (Cooke & Massee) Syd. & P.Syd.
 (Cooke & Massee) T.H.Li & Watling
 (Cooke & Massee) Theiss.
 (Cooke & Massee) Tomilin
+(Cooke & Massee) Trappe, Castellano & Amar.
 (Cooke & Massee) U.Braun
+(Cooke & Massee) U.Braun, C.Nakash., Videira & Crous
 (Cooke & Massee) W.B.Cooke
 (Cooke & Massee) Wakef.
 (Cooke & Massee) Watling
 (Cooke & Massee) Wiltshire
+(Cooke & Massee) Zeller & C.W.Dodge
+(Cooke & Massee) Zhu L.Yang, J.Qin & G.M.Gates
 (Cooke & Peck) Sacc.
 (Cooke & Peck) U.Braun & S.Takam.
-(Cooke & W.Phillips) Cain, Luck-Allen & Kimbr.
 (Cooke & W.Phillips) Dennis
 (Cooke & W.Phillips) G.Cunn.
+(Cooke & W.Phillips) Kimbr., Luck-Allen & Cain
 (Cooke & W.Phillips) Kuntze
 (Cooke & W.Phillips) Sacc.
 (Cooke & W.Phillips) Spooner
 (Cooke & W.Phillips) W.Phillips
 (Cooke & W.R.Gerard) Sacc.
 (Cooke ex Massee) Cleland & Cheel
 (Cooke ex W.Phillips) Massee
 (Cooke) Aptroot
 (Cooke) Aptroot & Lücking
 (Cooke) Arx & E.Müll.
+(Cooke) B.K.Cui & Shun Liu
 (Cooke) Berk. & Broome
 (Cooke) Berl.
 (Cooke) Berl. & Voglino
 (Cooke) Boise
 (Cooke) Boud.
 (Cooke) Bres.
 (Cooke) Bres. & Sacc.
 (Cooke) Burt
 (Cooke) Cleland & Cheel
 (Cooke) Cooke
+(Cooke) Crous
+(Cooke) Crous & U.Braun
 (Cooke) D.A.Reid
 (Cooke) Deighton
 (Cooke) Dennis
 (Cooke) E.J.Durand
 (Cooke) Faus
 (Cooke) G.A.de Vries
 (Cooke) G.Cunn.
@@ -4092,91 +4197,99 @@
 (Cooke) Kuntze
 (Cooke) L.G.Br. & Morgan-Jones
 (Cooke) Ladó
 (Cooke) Lambotte
 (Cooke) Lindau
 (Cooke) Lister
 (Cooke) Lloyd
+(Cooke) M.D.Barrett
+(Cooke) M.D.Barrett & Spirin
 (Cooke) Magnus
 (Cooke) Massee
 (Cooke) Massee & Rodway
+(Cooke) Matheny & Esteve-Rav.
 (Cooke) McAlpine
 (Cooke) McLennan & F.Halsey
 (Cooke) McNabb
 (Cooke) Nakasone
+(Cooke) Núñez & Ryvarden
+(Cooke) P.A.Barber & Crous
 (Cooke) P.D.Orton
 (Cooke) P.Joly
 (Cooke) P.K.Buchanan & Ryvarden
-(Cooke) P.Syd. & Sacc.
 (Cooke) P.Syd. & Syd.
 (Cooke) Pat.
 (Cooke) Petr. & Syd.
 (Cooke) Pilát
 (Cooke) R.Heim
 (Cooke) Rajchenb.
 (Cooke) Rea
 (Cooke) Ryvarden
-(Cooke) Ryvarden & Núñez
 (Cooke) Réblová
 (Cooke) Sacc.
+(Cooke) Sacc. & P.Syd.
 (Cooke) Sacc. ex Bres.
 (Cooke) Schroers
 (Cooke) Singer
 (Cooke) Speare
 (Cooke) Steyaert
 (Cooke) Syd.
+(Cooke) Tassi
 (Cooke) Teng
 (Cooke) Theiss. & Syd.
+(Cooke) U.Braun & Crous
 (Cooke) W.G.Sm.
 (Cooke) W.Phillips
 (Cooke) Wakef. ex Cleland
 (Cookson) L.A.S.Johnson
+(Cooney & R.Emers.) Schipper
 (Copel.) C.V.Morton
 (Copel.) Copel.
 (Copel.) Holttum
 (Copel.) M.Kato & Tsutsumi
 (Copel.) Yesilyurt & H.Schneider
-(Corda & Berk.) S.Hughes
-(Corda & Berk.) Sacc.
 (Corda) A.Braun
 (Corda) Bohlin
 (Corda) Bonord.
 (Corda) Corda
 (Corda) De Toni
 (Corda) Dumort. ex Lindb.
 (Corda) E.Fisch.
 (Corda) Hansg.
+(Corda) Hern.-Restr., R.F.Castañeda & Gené
 (Corda) Kalchbr.
 (Corda) Komark.-Legn.
 (Corda) Lloyd
+(Corda) Oorschot & Stalpers
 (Corda) Preuss
 (Corda) Quél.
 (Corda) Rabenh.
 (Corda) Ralfs
 (Corda) S.Hughes
 (Corda) Sacc.
 (Corda) Samson
 (Corda) Singer
-(Corda) Stalpers & Oorschot
 (Corda) Th.Fr.
 (Corda) W.Gams
 (Corner & E.Horak) Largent & Abell-Davis
+(Corner & E.Horak) Noordel. & Co-David
 (Corner & Hawker) A.H.Sm.
 (Corner) C.C.Berg
 (Corner) D.A.Crawford
 (Corner) G.Cunn.
 (Corner) Heinem. & Rammeloo
 (Corner) Imazeki
 (Corner) M.A.Neves & Halling
 (Corner) Pegler
 (Corner) Pegler & T.W.K.Young
 (Corner) R.H.Petersen
 (Corner) Ryvarden
 (Corner) Singer
 (Corner) Wolfe
+(Corner) Y.C.Li & Zhu L.Yang
 (Cornu) A.Fisch.
 (Cornu) Thaxt.
 (Coss. ex Barcelo) Sauvage
 (Coss.) P.W.Ball & Heywood
 (Coss.) Willk.
 (Costa) Widder
 (Costantin) A.Batko
@@ -4198,17 +4311,17 @@
 (Craven & Dunlop) J.W.Horn
 (Craven & S.M.Douglas) Udovicic & R.D.Spencer
 (Craven) Diane & Hilger
 (Craven) M.W.Chase
 (Craven) M.W.Frohl. & M.W.Chase
 (Craven) Udovicic & R.D.Spencer
 (Craven, Lepschi & Fryxell) R.L.Barrett
-(Cribb & J.W.Cribb) E.B.G.Jones & K.L.Pang
 (Cribb & J.W.Cribb) G.C.Hughes
 (Cribb & J.W.Cribb) Jørg.Koch
+(Cribb & J.W.Cribb) K.L.Pang & E.B.G.Jones
 (Cribb & J.W.Cribb) Kohlm.
 (Cribb & J.W.Cribb) T.W.Johnson
 (Cribb & J.W.Herb.) Cribb & J.W.Cribb
 (Cribb & J.W.Herb.) Kohlm. & E.Kohlm.
 (Cribb & J.W.Herb.) Meyers
 (Cribb) Bourr.
 (Cribb) De Clerck & Coppejans
@@ -4225,38 +4338,59 @@
 (Cromb.) Dodge
 (Cromb.) Hale
 (Cromb.) Hertel & Rambold
 (Cromb.) Imshaug ex Coppins & Fryday
 (Cromb.) Stizenb.
 (Cromb.) Vain.
 (Croome & P.A.Tyler) Asmund & Kristiansen
-(Crous & Arzanlou) Crous & U.Braun
 (Crous & C.Mohammed) Crous
+(Crous & Carnegie) Crous
 (Crous & Carnegie) Crous & Carnegie
 (Crous & Carnegie) Crous & Summerell
 (Crous & Carnegie) Crous & U.Braun
+(Crous & Carnegie) Guatim., R.W.Barreto & Crous
+(Crous & Carnegie) Hern.-Restr. & Crous
+(Crous & Carnegie) Quaedvl. & Crous
+(Crous & Carnegie) Videira & Crous
+(Crous & Jacq.Edwards) Crous
+(Crous & K.D.Hyde) L.Lombard, M.J.Wingf. & Crous
 (Crous & M.J.Wingf.) Crous
 (Crous & M.J.Wingf.) Crous & U.Braun
+(Crous & M.J.Wingf.) L.V.Alvarez & Crous
+(Crous & P.A.Barber) Crous
+(Crous & R.G.Shivas) C.Nakash. & Crous
+(Crous & R.G.Shivas) Crous
+(Crous & R.G.Shivas) Hern.-Restr. & Crous
+(Crous & R.G.Shivas) M.M.Wang & L.Cai
 (Crous & Summerell) Crous
 (Crous & Summerell) Crous & Summerell
 (Crous & Summerell) Crous & U.Braun
+(Crous & Summerell) Guatim., R.W.Barreto & Crous
+(Crous & Summerell) L.V.Alvarez & Crous
+(Crous & Summerell) Madrid & Hern.-Restr.
+(Crous & Summerell) Videira & Crous
+(Crous & Summerell) Voglmayr & Jaklitsch
+(Crous) B.Sutton
+(Crous) C.Nakash., Videira & Crous
 (Crous) Crous
 (Crous) Crous & U.Braun
-(Crous, M.J.Wingf. & H.Sm.ter) Crous, Slippers & A.J.L.Phillips
-(Crous, M.J.Wingf. & Slippers) Crous, Slippers & A.J.L.Phillips
-(Crous, M.J.Wingf. & W.J.Swart) J.A.Simpson
+(Crous) Hern.-Restr. & Crous
+(Crous) Thiyagaraja, Bundhun & K.D.Hyde
+(Crous) Valenz.-Lopez, Crous, Stchigel, Guarro & Cano
+(Crous, H.Sm.ter & M.J.Wingf.) Crous, Slippers & A.J.L.Phillips
+(Crous, Jacq.Edwards & P.W.J.Taylor) Hern.-Restr. & Crous
+(Crous, Jacq.Edwards & Pascoe) Crous
+(Crous, Jacq.Edwards & Pascoe) Valenz.-Lopez, Crous, Stchigel, Guarro & Cano
+(Crous, Pascoe & Jacq.Edwards) Quaedvl. & Crous
+(Crous, R.G.Shivas & McTaggart) Crous
 (Croxall) Bostock
 (Croxall) D.J.Ohlsen
 (Croxall) Ebihara & K.Iwats.
 (Cummins) Y.Ono
 (Cupp) Hasle
-(Curr. & Welw.) A.L.Sm.
-(Curr. & Welw.) Cooke
-(Curr. & Welw.) D.Hawksw.
-(Curr. & Welw.) Sacc.
 (Curr.) Boud.
 (Curr.) Cooke
 (Curr.) Lister
 (Curr.) Massee
 (Curr.) Sacc.
 (Curr.) Seaver
 (Curtis) Benth.
@@ -4274,29 +4408,30 @@
 (Curtis) Pers.
 (Curtis) Quél.
 (Curtis) Redhead, Vilgalys & Hopple
 (Curtis) Singer
 (Curtis) Skeels
 (Curtis) Stapf
 (Curtis) Vent.
+(Curzi) C.C.Tu & Kimbr.
 (Curzi) E.West
-(Curzi) Kimbr. & C.C.Tu
 (Czern.) Hollós
 (Czern.) Vellinga
 (D.A.Cooke) G.L.Nesom
 (D.A.Cooke) Jeanes
 (D.A.Cooke) Lander
 (D.A.Cooke) P.S.Short
 (D.A.Cooke) Paul G.Wilson
 (D.A.Herb.) C.S.P.Foster & B.J.Conn
 (D.A.Herb.) N.G.Marchant & Keighery
 (D.A.Reid) A.H.Sm. & D.A.Reid
 (D.A.Reid) D.A.Reid
 (D.A.Reid) Hjortstam
 (D.A.Reid) Hjortstam & Ryvarden
+(D.A.Reid) T.Lebel & T.W.May
 (D.A.Saunders) Hollenb. & I.A.Abbott
 (D.A.Sm.) Croxall
 (D.A.Sm.) Tindale
 (D.B.Scott & Van der Walt) Kurtzman, Robnett & Basehoar-Powers
 (D.B.Ward) E.Murray
 (D.B.Ward) P.I.Forst.
 (D.Ballant.) J.Larsen
@@ -4314,15 +4449,14 @@
 (D.Don) Blume
 (D.Don) Brouillet
 (D.Don) Buchenau
 (D.Don) C.Chr.
 (D.Don) C.J.Saldanha
 (D.Don) C.V.Morton
 (D.Don) Christenh. & Byng
-(D.Don) D.L.Jones & M.A.Clem.
 (D.Don) Decne.
 (D.Don) Domin
 (D.Don) Endl.
 (D.Don) F.Muell.
 (D.Don) Hochr.
 (D.Don) Holttum
 (D.Don) Hook.
@@ -4339,14 +4473,15 @@
 (D.Don) Munz
 (D.Don) P.F.Hunt & Summerh.
 (D.Don) Pamp.
 (D.Don) Pennell
 (D.Don) Raf. ex Olmstead
 (D.Don) Roxb. ex DC.
 (D.Don) Sch.Bip. ex Oliv.
+(D.Don) Schltr.
 (D.Don) Seidenf.
 (D.Don) Sherff
 (D.Don) Siebold & Zucc.
 (D.Don) Steud.
 (D.Don) Szlach.
 (D.E.Shaw & Alcorn) D.E.Shaw & Alcorn
 (D.E.Shaw) Thirum. & Neerg.
@@ -4364,20 +4499,14 @@
 (D.I.Morris) Doust & B.J.Conn
 (D.I.Morris) H.P.Linder
 (D.I.Morris) L.P.M.Willemse
 (D.I.Morris) Orchard
 (D.I.Morris) Pedley
 (D.I.Morris) S.W.L.Jacobs
 (D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson - Corymbia novoguinensis (D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson - Corymbia polycarpa (F.Muell.) K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson x Corymbia plena K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson x Corymbia setosa (Schauer) K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson x Corymbia setosa subsp. pedicellaris K.D.Hill & L.A.S.Johnson
-(D.J.Carr & S.G.M.Carr) K.D.Hill & L.A.S.Johnson x Corymbia terminalis (F.Muell.) K.D.Hill & L.A.S.Johnson
 (D.J.Carr) Prosk.
 (D.J.Galloway & P.M.Jørg.) P.M.Jørg. & D.J.Galloway
 (D.J.Galloway) D.J.Galloway
 (D.J.Galloway) F.J.Walker
 (D.J.Galloway) Filson
 (D.J.Galloway) Kantvilas & Grube
 (D.J.Read) Baral
@@ -4404,15 +4533,14 @@
 (D.L.Jones & M.A.Clem.) D.L.Jones
 (D.L.Jones & M.A.Clem.) D.L.Jones & M.A.Clem.
 (D.L.Jones & M.A.Clem.) G.N.Backh.
 (D.L.Jones & M.A.Clem.) J.M.H.Shaw
 (D.L.Jones & M.A.Clem.) Janes & Duretto
 (D.L.Jones & M.A.Clem.) M.A.Clem.
 (D.L.Jones & M.A.Clem.) M.A.Clem. & D.L.Jones
-(D.L.Jones & M.A.Clem.) M.A.Clem. & D.L.Jones x Dockrillia schoenina (Lindl.) M.A.Clem. & D.L.Jones
 (D.L.Jones & M.A.Clem.) Szlach.
 (D.L.Jones & M.A.Clem.) Szlach. & Rutk.
 (D.L.Jones & R.C.Nash) D.L.Jones & M.A.Clem.
 (D.L.Jones & R.J.Bates) J.M.H.Shaw
 (D.L.Jones & R.J.Bates) M.A.Clem. & D.L.Jones
 (D.L.Jones ex M.T.Mathieson) M.A.Clem. & D.L.Jones
 (D.L.Jones) A.P.Br.
@@ -4449,39 +4577,40 @@
 (DC. ex Sweet) Benth. & Hook.f.
 (DC. ex Triana & Planch.) Killip
 (DC.) A.Braun & Asch.
 (DC.) A.Chev.
 (DC.) A.Cunn. ex F.Muell.
 (DC.) A.Gray
 (DC.) A.R.Bean
-(DC.) A.R.Bean x Pterocaulon paradoxum A.R.Bean
 (DC.) A.R.Penfold
 (DC.) Allan
 (DC.) Anderb.
+(DC.) Anderb. & Haegi
 (DC.) Arcang.
-(DC.) B.L.Burtt
 (DC.) B.Nord.
 (DC.) Backeb.
 (DC.) Backer ex K.Heyne
 (DC.) Baill.
 (DC.) Baker
 (DC.) Bakh.f.
 (DC.) Banfi
+(DC.) Banks ex Vesque
 (DC.) Barlow
 (DC.) Bayly
 (DC.) Beauverd
-(DC.) Begerow, Oberw. & M.Piepenbr.
 (DC.) Benth.
 (DC.) Benth. & Hook.f.
 (DC.) Benth. ex Baker
 (DC.) Bercht. & J.Presl
 (DC.) Bernh.
 (DC.) Blakely
 (DC.) Blume ex A.Juss.
+(DC.) Boekhout & Enderle
 (DC.) Boerl.
+(DC.) Bondartsev & Singer
 (DC.) Brand
 (DC.) Brummitt
 (DC.) C.A.Gardner
 (DC.) C.Agardh
 (DC.) C.E.Anderson
 (DC.) C.M.Weiller
 (DC.) C.Norman
@@ -4498,24 +4627,22 @@
 (DC.) Cummins
 (DC.) DC.
 (DC.) DC. ex Benth.
 (DC.) Danser
 (DC.) De Not.
 (DC.) De Toni
 (DC.) Decne. & Planch.
-(DC.) Degel.
 (DC.) Degel. ["G.Nilsson"]
 (DC.) Diels
 (DC.) Domin
 (DC.) Druce
 (DC.) Duby
 (DC.) Dunlop
 (DC.) Eckl. & Zeyh.
 (DC.) Elkan
-(DC.) Enderle & Boekhout
 (DC.) Ettingsh.
 (DC.) Ewart
 (DC.) Ewart & O.B.Davies
 (DC.) F.M.Bailey
 (DC.) F.M.Knuth
 (DC.) F.Muell.
 (DC.) F.Muell. ex Benth.
@@ -4560,15 +4687,14 @@
 (DC.) Hoogland
 (DC.) Hook.f.
 (DC.) Hook.f. & Thomson
 (DC.) Hook.f. ex Hook.
 (DC.) Hutch.
 (DC.) I.Thomps.
 (DC.) J.G.West
-(DC.) J.G.West - Dodonaea viscosa subsp. spatulata (Sm.) J.G.West
 (DC.) J.H.Willis
 (DC.) J.M.Black
 (DC.) J.R.Wheeler & N.G.Marchant
 (DC.) J.Schröt.
 (DC.) J.V.Lamour.
 (DC.) Jeanes
 (DC.) Joy Thomps.
@@ -4588,14 +4714,15 @@
 (DC.) Lindl.
 (DC.) Loret & Barrandon
 (DC.) Lourteig
 (DC.) Lév.
 (DC.) M.A.Baker
 (DC.) M.Hiroe
 (DC.) M.J.Larsen & Zak
+(DC.) M.Piepenbr., Begerow & Oberw.
 (DC.) M.Roem.
 (DC.) Mabb.
 (DC.) Maiden
 (DC.) Maiden & Betche
 (DC.) Maire
 (DC.) Mart.
 (DC.) Mast.
@@ -4653,18 +4780,18 @@
 (DC.) Secr.
 (DC.) Ser.
 (DC.) Shinners
 (DC.) Sieber ex Sch.Bip.
 (DC.) Siebert & Voss
 (DC.) Sims
 (DC.) Singer
-(DC.) Singer & Bondartsev
 (DC.) Sleumer
 (DC.) Small
 (DC.) Sond.
+(DC.) Sotome & T.Hatt.
 (DC.) Span.
 (DC.) Speer
 (DC.) Spreng.
 (DC.) Stapf
 (DC.) Steetz
 (DC.) Steud.
 (DC.) Summerh.
@@ -4677,47 +4804,50 @@
 (DC.) Trautv.
 (DC.) Tul. & C.Tul.
 (DC.) Urb.
 (DC.) V.May
 (DC.) Verdc.
 (DC.) Vilgalys, Hopple & Jacq.Johnson
 (DC.) Vis.
+(DC.) Vizzini & Angelini
 (DC.) Vizzini, Contu & Justo
 (DC.) Voss
 (DC.) W.M.Curtis
 (DC.) Wallr.
 (DC.) Walp.
 (DC.) Webb & Berthel.
 (DC.) Wight & Arn.
 (DC.) Zahlbr.
 (DC.) Zeller
 (DC.) de Vriese
 (DC.) de Wit
+(Daday) Cleve
 (Daday) F.Gómez
 (Daday) F.Gómez, D.Moreira & López-García
 (Dade) C.Moreau
 (Dalzell) Airy Shaw
 (Dalzell) Kuntze
 (Dalzell) Ohwi & H.Ohashi
 (Dang.) Francé
 (Daniker) Guillaumin
+(Danks, T.Lebel & Vernes) Niskanen & Liimat.
 (Danquah) Alcorn
+(Danquah) Y.P.Tan & R.G.Shivas
 (Danser) K.L.Wilson & Makinson
 (Danser) Soják
 (Darb.) Fryday
 (Darb.) I.M.Lamb
 (Darb.) P.M.Jørg.
 (Dastur) G.M.Waterh.
 (Dasz.) Diddens & Lodder
 (Dasz.) Prillinger, Lopandic & Sugita
 (Davies) Branth & Rostr.
 (Davies) Taylor
 (Davies) Vězda
 (De Nardi) Veldkamp
-(De Not. & Ces.) De Not.
 (De Not.) A.Evans
 (De Not.) Arcang.
 (De Not.) Bagl.
 (De Not.) Bornet
 (De Not.) Crous & U.Braun
 (De Not.) Delgad.
 (De Not.) Fulford
@@ -4749,15 +4879,14 @@
 (Decne.) Benth.
 (Decne.) C.F.Reed
 (Decne.) E.S.Barton
 (Decne.) Engl.
 (Decne.) F.Muell.
 (Decne.) Harv.
 (Decne.) Holttum
-(Decne.) Hook.f.
 (Decne.) I.A.Abbott
 (Decne.) J.Agardh
 (Decne.) J.W.Grimes
 (Decne.) K.L.Wilson
 (Decne.) Kuntze
 (Decne.) Kütz.
 (Decne.) Lindl.
@@ -4839,15 +4968,15 @@
 (Desf.) Pers.
 (Desf.) S.T.Reynolds
 (Desf.) Spreng.
 (Desf.) Trin.
 (Desf.) Tzvelev
 (Desf.) Willd.
 (Desm.) Allesch.
-(Desm.) De Not. & Ces.
+(Desm.) Ces. & De Not.
 (Desm.) Donk
 (Desm.) Fr.
 (Desm.) G.Winter
 (Desm.) Höhn.
 (Desm.) J.J.Kickx
 (Desm.) S.Ito
 (Desm.) Sacc.
@@ -4904,39 +5033,38 @@
 (Desv.) Steud.
 (Desv.) T.Moore
 (Desv.) Thell.
 (Desv.) Trevis.
 (Desv.) Walp.
 (Desv.) Wess.Boer
 (Desv.) de Wet & J.R.Harlan ex Davidse
-(Di Menna & Marples) A.A.Padhye, Ajello & Tad.Matsumoto
+(Di Menna & Marples) Tad.Matsumoto, A.A.Padhye & Ajello
 (Dickie) Børgesen
 (Dickie) De Toni
 (Dickie) Feldmann
 (Dickie) G.Murray & De Toni
 (Dickie) Sauv.
 (Dickie) W.R.Taylor & F.E.Drouet
 (Dickie) Weber Bosse
-(Dicks. : Fr.) Pers.
 (Dicks.) A.Massal.
 (Dicks.) Ach.
-(Dicks.) Boul.
 (Dicks.) Boulay
 (Dicks.) Brid.
 (Dicks.) De Not.
 (Dicks.) Flot.
 (Dicks.) Fr.
 (Dicks.) Gray
 (Dicks.) Hook. & Taylor
 (Dicks.) J.Steiner
 (Dicks.) Kalb & Lücking
 (Dicks.) Körb.
 (Dicks.) Lettau
 (Dicks.) P.M.Jørg. & P.James
 (Dicks.) Pers.
+(Dicks.) R.H.Zander
 (Dicks.) Raddi
 (Dicks.) Rostaf.
 (Dicks.) Stein
 (Dicks.) Syme
 (Dicks.) Trevis.
 (Dicks.) Vain.
 (Dicks.) Zahlbr.
@@ -4959,15 +5087,14 @@
 (Diels) Carolin ex Hershk.
 (Diels) Christenh. & Byng
 (Diels) Chrtek & Slavikova
 (Diels) Corner
 (Diels) D.D.Sokoloff, Remizowa, T.D.Macfarl. & Rudall
 (Diels) Diels ex Kraenzl.
 (Diels) Domin
-(Diels) Domin x Kunzea recurva Schauer
 (Diels) Duretto & Heslewood
 (Diels) Ewart
 (Diels) Ewart & B.Rees
 (Diels) Farw.
 (Diels) H.Eichler
 (Diels) H.Walter
 (Diels) Heimerl
@@ -4992,17 +5119,19 @@
 (Diels) Ostenf.
 (Diels) P.S.Short
 (Diels) Paul G.Wilson
 (Diels) Peter G.Wilson
 (Diels) Prain
 (Diels) S.T.Blake
 (Diels) Schinz
+(Diels) T.Krueger & A.Fleischm.
 (Diels) Ulbr.
 (Diels) W.R.Barker & R.M.Barker
 (Diesing) Kof. & Swezy
+(Dietel) McTaggart & R.G.Shivas
 (Dill. ex Ach.) Meyen & Flot.
 (Dillwyn) Aresch.
 (Dillwyn) Bornet
 (Dillwyn) C.Agardh
 (Dillwyn) Gain
 (Dillwyn) Grev.
 (Dillwyn) H.Perag. & M.Perag.
@@ -5043,14 +5172,15 @@
 (Dixon) Dixon & Sainsbury
 (Dixon) H.A.Crum
 (Dixon) J.E.Beever
 (Dixon) J.K.Bartlett
 (Dixon) R.H.Zander
 (Dixon) Sainsbury
 (Dixon) Zanten
+(Dixon-Stew.) Y.N.Wang, X.Y.Liu & R.Y.Zheng
 (Dockrill) D.L.Jones & M.A.Clem.
 (Dockrill) D.P.Banks & Clemesha
 (Dockrill) Dockrill
 (Dockrill) Garay
 (Dockrill) M.A.Clem. & B.J.Wallace
 (Dockrill) Rauschert
 (Dockrill) S.P.Lyon, M.A.Clem. & D.L.Jones
@@ -5059,15 +5189,14 @@
 (Dogiel) F.J.R.Taylor
 (Dogiel) Kof. & Swezy
 (Doidge) Cummins & S.M.Husain
 (Dombey ex Lam.) Griseb.
 (Dombrain) Asch. & Graebn.
 (Domin ex F.M.Bailey) Domin
 (Domin) A.E.Holland
-(Domin) A.E.Holland - Trachymene montana A.E.Holland
 (Domin) A.R.Bean
 (Domin) A.S.George
 (Domin) Airy Shaw
 (Domin) B.G.Thomson
 (Domin) B.K.Simon
 (Domin) B.L.Burtt
 (Domin) Baehni
@@ -5116,24 +5245,23 @@
 (Domin) Halford
 (Domin) Henrard
 (Domin) Hershk.
 (Domin) Hitchc.
 (Domin) Hopper & A.P.Br.
 (Domin) Hughes
 (Domin) J.H.Ross
-(Domin) J.H.Ross x Hovea ramulosa A.Cunn. ex Lindl.
-(Domin) J.H.Ross x Hovea tholiformis I.Thomps.
 (Domin) J.Kern
 (Domin) J.M.Black
 (Domin) J.M.Hart
 (Domin) J.M.Powell
 (Domin) J.R.I.Wood & Scotland
 (Domin) J.W.Grimes
 (Domin) Jackes
 (Domin) Jeanes
+(Domin) K.R.Thiele & T.Hammer
 (Domin) Kük.
 (Domin) L.A.S.Johnson
 (Domin) L.G.Adams
 (Domin) L.W.Cayzer, Crisp & I.Telford
 (Domin) Lazarides
 (Domin) Lazarides & R.D.Webster
 (Domin) M.A.Clem. & D.L.Jones
@@ -5169,21 +5297,23 @@
 (Domin) S.T.Reynolds & A.E.Holland
 (Domin) S.Y.Dong
 (Domin) Stapf
 (Domin) Swingle
 (Domin) Szlach.
 (Domin) T.G.Hartley
 (Domin) T.Koyama
+(Domin) T.L.Collins
 (Domin) Threlfall
 (Domin) Tindale
 (Domin) Vickery
 (Domin) W.Hartley
 (Domin) W.R.Barker & Beardsley
 (Domin) Watts
 (Domin) Wills & J.J.Bruhl
+(Donk) Bon
 (Donk) Corner
 (Donk) Niemelä
 (Donk) R.H.Petersen
 (Donkin) Cleve
 (Donkin) E.J.Cox
 (Donkin) Grunow
 (Donkin) Hust.
@@ -5218,37 +5348,40 @@
 (Dozy & Molk.) Müll.Hal.
 (Dozy & Molk.) R.Watan.
 (Dozy & Molk.) Sande Lac.
 (Dozy & Molk.) T.Yamag.
 (Dozy & Molk.) W.R.Buck & B.C.Tan
 (Dozy & Molk.) Wijk & Margad.
 (Drayton) Whetzel
+(Drechsler) Abad, De Cock, K.Bala, Robideau, A.M.Lodhi & Lévesque
 (Drechsler) K.J.Leonard & Suggs
 (Drechsler) Khokhr.
 (Drechsler) M.J.Richardson & E.M.Fraser
 (Drechsler) M.Scholler, Hagedorn & A.Rubner
 (Drechsler) R.Spargue
+(Drechsler) Rossman & K.D.Hyde
 (Drechsler) Shoemaker
 (Drechsler) Subram. & B.L.Jain
+(Drechsler) Thorn
 (Drechsler) Uzuhashi, Tojo & Kakish.
 (Dreschler) Suggs & Leonard
 (Drude) Becc.
-(Drumm. ex Harv.) Benth.
 (Drumm. ex Harv.) E.M.Benn.
 (Drumm. ex Harv.) F.Muell.
 (Drumm.) N.G.Marchant & Keighery
 (Dryand.) Alston
 (Dryand.) Benth.
 (Dryand.) Domin
 (Dryand.) J.Sm.
 (Dryand.) Kuhn
 (Dryand.) Poir.
 (Du Rietz) I.M.Lamb
 (Du Rietz) W.R.Barker
 (Dubard & R.Vig.) Lowry
+(Dubard) Teo
 (Duby) A.Jaeger
 (Duby) Essl.
 (Duby) Giese & J.-P.Frahm
 (Duby) M.Fleisch.
 (Duby) Nyl.
 (Duby) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (Duby) R.Knuth
@@ -5256,23 +5389,22 @@
 (Duchass. & Walp.) Baker
 (Duchass. & Walp.) Benth.
 (Duchass. & Walp.) Griseb.
 (Duchass. & Walp.) Kuntze
 (Duchass. & Walp.) Pedley
 (Duchass. ex J.Agardh) A.H.S.Lucas
 (Duchesne ex Rozier) Mabb.
-(Duché & R.Heim) G.Sm. & A.H.S.Br.
+(Duché & R.Heim) A.H.S.Br. & G.Sm.
 (Dufour) Ach.
 (Dufour) Foslie
 (Dufour) G.Furnari, Cormaci & Alongi
 (Dufour) Hue
 (Dufour) Malme
 (Duhamel) Rehder
 (Dujard.) F.Stein
-(Dujard.) Fresen.
 (Dujard.) G.A.Klebs
 (Dujard.) Hübner
 (Dujard.) Kent
 (Dujard.) Warm.
 (Duke) Vánky
 (Dum.Cours.) Court
 (Dum.Cours.) Czern. & Schwarz
@@ -5302,71 +5434,78 @@
 (Dunal) Rydb.
 (Dunal) Seithe
 (Dunal) Teodor.
 (Dunal) Wettst.
 (Dur. & Mont.) Bagl. & Car.
 (Durazz.) Kuntze
 (Duretto) Duretto & Heslewood
+(Durieu & Mont. ex Sacc.) Sacc.
 (Durieu & Mont.) A.L.Sm.
+(Durieu & Mont.) Donk
+(Durieu & Mont.) E.Fisch.
+(Durieu & Mont.) Sacc.
+(Durieu & Mont.) Zmitr. & Malysheva
+(Durieu & Mont.) Zmitr., Wasser & Ezhov
 (Durieu) Durieu & Asch.
 (Durieu) Gillet & Magne
 (Durieu) Nyman
+(Dusén) Ochyra & R.H.Zander
 (Dusén) R.H.Zander
 (Dörfelt) Pegler & T.W.K.Young
 (Dörfelt) R.H.Petersen
 (E.A.Hodgs.) E.A.Hodgs.
 (E.A.Hodgs.) J.J.Engel & R.M.Schust.
 (E.B.Alexeev) Soreng & L.J.Gillespie
 (E.B.Bartram) B.C.Tan, H.P.Ramsay & W.B.Schofield
 (E.B.Bartram) Enroth
 (E.B.Bartram) Streimann
 (E.B.Bartram) Zanten
-(E.B.G.Jones & Camp.-Als.) E.B.G.Jones & J.Dupont
+(E.B.G.Jones & Camp.-Als.) J.Dupont & E.B.G.Jones
 (E.C.Berry) Hale
 (E.C.Hansen) E.C.Hansen
 (E.Coleman) A.S.George
 (E.Coleman) D.L.Jones & M.A.Clem.
 (E.Coleman) M.A.Clem. & D.L.Jones
 (E.Coleman) M.A.Clem. & Hopper
 (E.Coleman) Szlach.
 (E.D.Garber) Spangler
 (E.Dale) G.Sm.
 (E.Fisch.) E.Fisch.
 (E.Fisch.) Hansf.
 (E.Fisch.) Lloyd
 (E.Fisch.) Locq.
-(E.Fisch.) P.Syd. & Sacc.
+(E.Fisch.) Sacc. & P.Syd.
+(E.Fisch.) Trierv.-Per. & K.Hosaka
 (E.Fourn.) Parris
-(E.G.Jørg.) F.Gómez
+(E.G.Simmons) Woudenb. & Crous
 (E.H.Lombard & Capon) A.R.Loebl., Sherley & R.J.Schmidt
 (E.Horak) A.M.Young
 (E.Horak) E.Horak
+(E.Horak) G.Garnier
 (E.Horak) Garrido
-(E.Horak) Gasparini
+(E.Horak) J.A.Cooper
 (E.Horak) K.Griffiths
+(E.Horak) Niskanen & Liimat.
 (E.Horak) Noordel. & Co-David
 (E.Horak) Peintner & M.M.Moser
 (E.Horak) R.H.Jones & T.W.May
 (E.Horak) T.W.May & A.E.Wood
 (E.Horak, Peintner, M.M.Moser & Vilgalys) E.Horak, Peintner, M.M.Moser & Vilgalys
 (E.J.Butler) Arthur
 (E.J.Butler) Karling
 (E.J.Butler) M.W.Dick
 (E.J.Butler) Shoemaker
 (E.J.Butler) Sparrow
 (E.J.Butler) W.Gams
-(E.J.Butler, Syd. & P.Syd.) Mundk.
-(E.J.Butler, Syd. & P.Syd.) Theiss. & Syd.
-(E.J.Butler, Syd. & P.Syd.) Vánky
 (E.J.F.Wood) A.R.Loebl.
 (E.J.F.Wood) Balech
 (E.J.F.Wood) F.Gómez
 (E.J.F.Wood) F.Gómez, D.Moreira & López-García
 (E.J.Schmidt) F.Gómez
-(E.J.Schmidt) Jörg.
+(E.J.Schmidt) Jørg.
 (E.L.Robertson) T.D.Macfarl. & D.D.Sokoloff
 (E.L.Robertson) Yu Ito
 (E.L.Stewart & Trappe) Pegler & T.W.K.Young
 (E.M.Benn.) L.W.Cayzer & Crisp
 (E.M.Benn.) L.W.Cayzer, Crisp & I.Telford
 (E.M.Benn.) P.I.Forst.
 (E.M.Ross) K.R.Thiele
@@ -5416,16 +5555,15 @@
 (E.Y.Dawson) Baldock
 (E.Y.Dawson) E.M.Woll.
 (E.Y.Dawson) Papenf.
 (E.Y.Dawson) Santel.
 (E.Y.Dawson) W.R.Taylor
 (E.Y.Dawson) Woelk.
 (E.Young) Deighton
-(Earle & Tracy) Boedijn
-(Earle & Tracy) Magnus
+(E.Yuill) Malloch & Cain
 (Earle) A.H.Sm. & Hesler
 (Earle) Deighton
 (Earle) Sacc. & Trotter
 (Earle) Singer
 (Eastw.) Jeps.
 (Eckfeldt) Aptroot & M.Cáceras
 (Eckfeldt) Marbach
@@ -5440,17 +5578,20 @@
 (Eckl.) Bég.
 (Eckl.) Kuntze
 (Eckl.) Reinw. ex Hook.f.
 (Edgar & A.P.Druce) Barberá, Quintanar, Soreng & P.M.Peterson
 (Edgar) M.E.Jansen
 (Edgar) Soják
 (Edson) Fitzp.
+(Egunyomi & Olar.) R.H.Zander
 (Ehrenb. ex Fr.) Lév.
 (Ehrenb. ex Fr.) Syd.
+(Ehrenb. ex Gomont) Geitler
 (Ehrenb. ex Link) G.P.Clinton
+(Ehrenb. ex Ralfs) W.Archer
 (Ehrenb. ex Ralfs) Willi Krieg.
 (Ehrenb.) A.Mayer
 (Ehrenb.) Asch.
 (Ehrenb.) Auersw.
 (Ehrenb.) Balech
 (Ehrenb.) Brun
 (Ehrenb.) Bréb.
@@ -5474,42 +5615,39 @@
 (Ehrenb.) E.J.F.Wood
 (Ehrenb.) Ehrenb.
 (Ehrenb.) Ehrenb. ex Endl.
 (Ehrenb.) Ehrenb. ex Kütz.
 (Ehrenb.) F.Gómez
 (Ehrenb.) F.Gómez, D.Moreira & López-García
 (Ehrenb.) F.Meister
-(Ehrenb.) F.Schütt
 (Ehrenb.) F.Stein
 (Ehrenb.) Fr.
 (Ehrenb.) G.A.Klebs
 (Ehrenb.) G.C.Wall.
 (Ehrenb.) G.Karst.
 (Ehrenb.) G.R.Hasle & P.A.Sims
 (Ehrenb.) G.W.Andrews
-(Ehrenb.) Geitler
 (Ehrenb.) Gourret
 (Ehrenb.) Gran
 (Ehrenb.) Grunow
 (Ehrenb.) Hallegr. & Huisman
 (Ehrenb.) Hassall ex Ralfs
 (Ehrenb.) Heiden
 (Ehrenb.) Hust.
 (Ehrenb.) J.Roy & Bisset
 (Ehrenb.) J.Schiller
 (Ehrenb.) J.W.Griff. & Henfr.
-(Ehrenb.) Jörg.
-(Ehrenb.) Karajeva
+(Ehrenb.) Jørg.
+(Ehrenb.) Karaeva
 (Ehrenb.) Kent
 (Ehrenb.) Kirchn.
 (Ehrenb.) Krammer
 (Ehrenb.) Kreisel
 (Ehrenb.) Kretschmann, Elbr., C.Zinssm., S.Soehner, Kirsch, Kusber & Gottschling
 (Ehrenb.) Kuntze
-(Ehrenb.) Kütz
 (Ehrenb.) Kütz.
 (Ehrenb.) Lange-Bert.
 (Ehrenb.) Lange-Bert., Metzeltin & Witkowski
 (Ehrenb.) Lemmerm.
 (Ehrenb.) M.Lebour
 (Ehrenb.) Menegh.
 (Ehrenb.) Menegh. ex Ralfs
@@ -5534,15 +5672,14 @@
 (Ehrenb.) Ryvarden
 (Ehrenb.) S.Hughes
 (Ehrenb.) S.Lill.
 (Ehrenb.) Schaarschm.
 (Ehrenb.) Simonsen
 (Ehrenb.) Siver & P.B.Hamilton
 (Ehrenb.) Starbäck
-(Ehrenb.) Stein
 (Ehrenb.) Teiling
 (Ehrenb.) Thwaites
 (Ehrenb.) Tillmann, Gottschling, Elbr., Kusber & Hoppenrath
 (Ehrenb.) Van Heurck
 (Ehrenb.) Vanhöffen
 (Ehrenb.) W.Archer
 (Ehrenb.) W.Sm.
@@ -5563,15 +5700,15 @@
 (Ehrh.) Th.Fr.
 (Ehrh.) W.L.Culb.
 (Ehrh.) Zahlbr.
 (Eichler) Benth. & Hook.f.
 (Eichler) Pax & K.Hoffm.
 (Eichw.) A.Braun
 (Eichw.) Playfair
-(Elbr. & Schnepf) G.I.Hansen, Botes & de Salas
+(Elbr. & Schnepf) Gert Hansen, Botes & de Salas
 (Elenkin & Woron.) Vězda
 (Elenkin) Anagn. & Komárek
 (Elfving) West & G.S.West
 (Elix & A.W.Archer) A.W.Archer & Elix
 (Elix & A.W.Archer) I.Schmitt, B.P.Hodk. & Lumbsch
 (Elix & A.W.Archer) Kantvilas & Elix
 (Elix & Bawingan) O.Blanco, A.Crespo, Divakar, Elix & Lumbsch
@@ -5607,15 +5744,15 @@
 (Elix) Kantvilas & Divakar
 (Elix) Kantvilas & Elix
 (Elix) Lücking, Elix & A.W.Archer
 (Elix) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (Elix) S.Y.Kondr., Fedorenko, S.Stenroos, Kärnefelt & A.Thell
 (Elix, S.Y.Kondr. & Kärnefelt) S.Y.Kondr., Kärnefelt, Elix, A.Thell, J.Kim, A.S.Kondr. & Hur
 (Elliott) Nash
-(Ellis & Everh. ex H.S.Jacks. & D.P.Rogers) G.Cunn.
+(Ellis & Everh. ex D.P.Rogers & H.S.Jacks.) G.Cunn.
 (Ellis & Everh.) Aa & Boerema
 (Ellis & Everh.) Arx
 (Ellis & Everh.) B.Sutton
 (Ellis & Everh.) Deighton
 (Ellis & Everh.) Dennis
 (Ellis & Everh.) E.S.Salmon
 (Ellis & Everh.) G.Cunn.
@@ -5739,26 +5876,25 @@
 (Endl.) N.Snow & Guymer
 (Endl.) Neck. ex Pojark.
 (Endl.) Nicholls & Goadby
 (Endl.) Ostenf.
 (Endl.) P.S.Green
 (Endl.) Pamp.
 (Endl.) Pax
+(Endl.) Peter G.Wilson
 (Endl.) Petrie
 (Endl.) Pfeiff.
 (Endl.) Pierre
 (Endl.) Planch.
 (Endl.) R.J.F.Hend.
 (Endl.) R.M.Barker
 (Endl.) Rchb.f.
 (Endl.) Rchb.f. ex Lindl.
 (Endl.) Rye
 (Endl.) Schauer
-(Endl.) Schauer x Hypocalymma ericifolium Benth.
-(Endl.) Schauer x Hypocalymma robustum (Endl.) Lindl.
 (Endl.) Schindl.
 (Endl.) Schltdl.
 (Endl.) Schot
 (Endl.) Seem.
 (Endl.) Skottsb.
 (Endl.) Sond.
 (Endl.) Spach
@@ -5778,31 +5914,32 @@
 (Endl.) de Lange
 (Endl.) de Lange & R.O.Gardner
 (Endl.) de Laub.
 (Endl.) Á.Löve
 (Engelm. & A.Gray) W.L.Wagner & Hoch
 (Engelm. & J.M.Bigelow) B.D.Parfitt
 (Engelm. & J.M.Bigelow) F.M.Knuth
+(Engelm. & J.M.Bigelow) M.A.Baker, Cloud-H. & Majure
+(Engelm. & J.M.Bigelow) Toumey
 (Engelm. ex A.Berger) A.Berger
 (Engelm. ex A.Berger) Britton & Rose
 (Engelm.) Bogin
 (Engelm.) F.M.Knuth
 (Engelm.) J.G.Sm.
 (Engelm.) L.D.Benson
-(Engelm.) M.A.Baker, Cloud-H. & Majure
 (Engelm.) Micheli
 (Engelm.) Moran
-(Engelm.) Toumey
 (Engelm.) Yunck.
 (Engl.) B.L.Linden
 (Engl.) Blakely
 (Engl.) Conran & Clifford
 (Engl.) Corner
 (Engl.) Domin
 (Engl.) Engl. & K.Krause
+(Engl.) Goffinet & W.R.Buck
 (Engl.) Leenh.
 (Engl.) Paul G.Wilson
 (Engl.) Sleumer
 (Engl.) Swingle
 (Engl.) W.D.Francis
 (Engl.) W.R.Buck & Goffinet
 (Enroth & S.He) Wijk & Margad.
@@ -5867,14 +6004,15 @@
 (Ewart & M.Gordon) L.A.S.Johnson
 (Ewart & Morrison) Crisp
 (Ewart & Morrison) Maesen
 (Ewart & Morrison) S.T.Reynolds & Pedley
 (Ewart & O.B.Davies) A.J.Scott
 (Ewart & O.B.Davies) Airy Shaw
 (Ewart & O.B.Davies) Guillaumin
+(Ewart & O.B.Davies) I.Telford & J.J.Bruhl
 (Ewart & O.B.Davies) Lazarides
 (Ewart & O.B.Davies) McGill.
 (Ewart & O.B.Davies) Paul G.Wilson
 (Ewart & Sharman) D.L.Jones & M.A.Clem.
 (Ewart & Sharman) M.A.Clem. & D.L.Jones
 (Ewart & Sharman) Pedley
 (Ewart) A.S.George & N.Gibson
@@ -5922,16 +6060,16 @@
 (F.J.R.Taylor) Hasle
 (F.L.Bauer ex Benth.) Benth.
 (F.L.Erickson & J.H.Willis) Carlquist
 (F.L.Erickson & J.H.Willis) Lowrie & Carlquist
 (F.L.Erickson & J.H.Willis) Lowrie, A.H.Burb. & Kenneally
 (F.Ludw.) Kuntze
 (F.Ludw.) McAlpine
-(F.Ludw.) McKenzie & Vánky
 (F.Ludw.) Syd.
+(F.Ludw.) Vánky & McKenzie
 (F.M.Bailey & F.Muell.) A.R.Bean
 (F.M.Bailey ex Ralfs) P.Lundell
 (F.M.Bailey) A.J.Scott
 (F.M.Bailey) A.R.Bean
 (F.M.Bailey) A.S.George
 (F.M.Bailey) A.V.Bobrov & Melikyan
 (F.M.Bailey) Adema & Sirich.
@@ -5965,30 +6103,29 @@
 (F.M.Bailey) Christenson
 (F.M.Bailey) Clemesha
 (F.M.Bailey) Cogn.
 (F.M.Bailey) Copel.
 (F.M.Bailey) Corner
 (F.M.Bailey) Craven
 (F.M.Bailey) Craven & Biffin
+(F.M.Bailey) Crisp & L.G.Cook
 (F.M.Bailey) D.C.Hassall ex P.I.Forst. & R.J.F.Hend.
 (F.M.Bailey) D.J.Dixon
 (F.M.Bailey) D.J.Ohlsen
 (F.M.Bailey) D.L.Jones
 (F.M.Bailey) D.L.Jones & M.A.Clem.
 (F.M.Bailey) D.P.Banks & Clemesha
-(F.M.Bailey) D.P.Banks & Clemesha x Dendrobium speciosum subsp. hillii (Mast.) D.P.Banks & Clemesha
 (F.M.Bailey) Danser
 (F.M.Bailey) Diels
 (F.M.Bailey) Dockrill
 (F.M.Bailey) Domin
-(F.M.Bailey) Edlin ex J.H.Boas
+(F.M.Bailey) Edlin ex I.H.Boas
 (F.M.Bailey) Engl.
 (F.M.Bailey) Erlee
 (F.M.Bailey) Ewart
-(F.M.Bailey) Ewart & Jean White
 (F.M.Bailey) F.Ballard
 (F.M.Bailey) F.M.Bailey
 (F.M.Bailey) F.Muell.
 (F.M.Bailey) Fahn
 (F.M.Bailey) Forman
 (F.M.Bailey) Fosberg & Sachet
 (F.M.Bailey) G.Cunn.
@@ -6008,15 +6145,14 @@
 (F.M.Bailey) J.Dransf., A.K.Irvine & N.W.Uhl
 (F.M.Bailey) J.J.Sm.
 (F.M.Bailey) J.Schust.
 (F.M.Bailey) Jackes
 (F.M.Bailey) Jessup
 (F.M.Bailey) K.D.Hill
 (F.M.Bailey) K.D.Hill & L.A.S.Johnson
-(F.M.Bailey) K.D.Hill & L.A.S.Johnson x Corymbia tessellaris (F.Muell.) K.D.Hill & L.A.S.Johnson
 (F.M.Bailey) K.Iwats.
 (F.M.Bailey) K.Larsen & S.S.Larsen
 (F.M.Bailey) K.M.Wong
 (F.M.Bailey) K.Schum.
 (F.M.Bailey) Kalkman
 (F.M.Bailey) Kosterm.
 (F.M.Bailey) Kuntze
@@ -6029,15 +6165,14 @@
 (F.M.Bailey) Leenh.
 (F.M.Bailey) Lewton
 (F.M.Bailey) Lloyd
 (F.M.Bailey) M.A.Clem. & D.L.Jones
 (F.M.Bailey) M.T.Mathieson
 (F.M.Bailey) Maiden
 (F.M.Bailey) Maiden & Betche
-(F.M.Bailey) Maiden x Eucalyptus melanophloia F.Muell.
 (F.M.Bailey) Merr.
 (F.M.Bailey) Merr. & L.M.Perry
 (F.M.Bailey) Merr. ex J.F.Bailey & C.T.White
 (F.M.Bailey) Mich.J.Parsons
 (F.M.Bailey) N.A.Wakef.
 (F.M.Bailey) Ngan
 (F.M.Bailey) Nicholls
@@ -6046,15 +6181,15 @@
 (F.M.Bailey) P.I.Forst.
 (F.M.Bailey) P.K.Endress
 (F.M.Bailey) P.Royen
 (F.M.Bailey) P.S.Green
 (F.M.Bailey) Parris
 (F.M.Bailey) Pedley
 (F.M.Bailey) Perkins
-(F.M.Bailey) Peter G.Wilson & J.T.Waterh.
+(F.M.Bailey) Peter G.Wilson
 (F.M.Bailey) Philipson
 (F.M.Bailey) Pic.Serm.
 (F.M.Bailey) Prain & Burkill
 (F.M.Bailey) Puttock
 (F.M.Bailey) R.Govaerts & J.M.H.Shaw
 (F.M.Bailey) R.K.Wilson & Bayly
 (F.M.Bailey) Radlk.
@@ -6099,30 +6234,32 @@
 (F.Muell. & Baker) Parris
 (F.Muell. & Baker) Perrie & Brownsey
 (F.Muell. & Baker) S.B.Andrews
 (F.Muell. & Baker) Testo, Sundue & A.R.Field
 (F.Muell. & Behr ex F.Muell.) N.T.Burb.
 (F.Muell. & C.Stuart ex Meisn.) Kuntze
 (F.Muell. & F.M.Bailey) Craven
+(F.Muell. & F.M.Bailey) F.Muell.
 (F.Muell. & F.M.Bailey) F.Muell. & F.M.Bailey
 (F.Muell. & F.M.Bailey) L.A.S.Johnson
+(F.Muell. & F.M.Bailey) Peter G.Wilson & J.T.Waterh.
 (F.Muell. & F.M.Bailey) S.T.Blake
 (F.Muell. & F.M.Bailey) W.D.Francis
 (F.Muell. & Fitzg.) Fitzg.
 (F.Muell. & Fitzg.) Kuntze
 (F.Muell. & Fitzg.) Rauschert
 (F.Muell. & Kalchbr.) Cooke
 (F.Muell. & Kalchbr.) Sacc.
 (F.Muell. & Kraenzl.) J.J.Sm.
 (F.Muell. & Kraenzl.) M.A.Clem. & D.L.Jones
 (F.Muell. & Kraenzl.) Szlach.
 (F.Muell. & Maiden) Pedley
-(F.Muell. & Sond. ex Sond.) Benth.
-(F.Muell. & Sond. ex Sond.) Kuntze
+(F.Muell. & Sond.) Benth.
 (F.Muell. & Sond.) F.Muell.
+(F.Muell. & Sond.) Kuntze
 (F.Muell. & Sond.) Paul G.Wilson
 (F.Muell. & Tate ex J.M.Black) Threlfall
 (F.Muell. & Tate) C.A.Gardner
 (F.Muell. & Tate) Craven
 (F.Muell. & Tate) Crisp
 (F.Muell. & Tate) Crisp & P.H.Weston
 (F.Muell. & Tate) Domin
@@ -6131,28 +6268,27 @@
 (F.Muell. & Tate) Ewart & Jean White
 (F.Muell. & Tate) Ewart & P.H.Jarrett
 (F.Muell. & Tate) F.Muell.
 (F.Muell. & Tate) F.Muell. & Tate
 (F.Muell. & Tate) Haegi
 (F.Muell. & Tate) Heine
 (F.Muell. & Tate) J.H.Willis
-(F.Muell. & Tate) J.H.Willis - Phebalium tuberculosum (F.Muell.) Benth.
 (F.Muell. & Tate) J.M.Black
 (F.Muell. & Tate) J.W.Green
 (F.Muell. & Tate) J.W.Horn
 (F.Muell. & Tate) Lander
 (F.Muell. & Tate) Melville
 (F.Muell. & Tate) O.E.Schulz
 (F.Muell. & Tate) P.S.Short
 (F.Muell. & Tate) Paul G.Wilson
 (F.Muell. & Tate) Rye
 (F.Muell. & Tate) Schodde
 (F.Muell. & Tate) Tiegh.
 (F.Muell. & Tate) Volkens
-(F.Muell. & Tate) Volkens x Osteocarpum pentapterum (F.Muell. & Tate) Volkens
+(F.Muell. & Thüm.) Sacc.
 (F.Muell. ex A.Braun) Kuntze
 (F.Muell. ex A.Braun) R.D.Wood
 (F.Muell. ex A.Gray) G.L.Nesom
 (F.Muell. ex A.S.Mitch.) M.W.Frohl. & M.W.Chase
 (F.Muell. ex Baill.) F.Muell.
 (F.Muell. ex Baill.) Grüning
 (F.Muell. ex Becc.) Kuntze
@@ -6181,16 +6317,16 @@
 (F.Muell. ex Benth.) Cowie
 (F.Muell. ex Benth.) D.L.Jones & M.A.Clem.
 (F.Muell. ex Benth.) Dockrill
 (F.Muell. ex Benth.) Domin
 (F.Muell. ex Benth.) Duretto
 (F.Muell. ex Benth.) Engl.
 (F.Muell. ex Benth.) Ewart
+(F.Muell. ex Benth.) Ewart & O.B.Davies
 (F.Muell. ex Benth.) F.Muell.
-(F.Muell. ex Benth.) F.Muell. - Sida macropoda F.Muell. ex Benth.
 (F.Muell. ex Benth.) F.Muell. ex Maiden & Betche
 (F.Muell. ex Benth.) F.Turner
 (F.Muell. ex Benth.) Flicker
 (F.Muell. ex Benth.) G.L.Davis
 (F.Muell. ex Benth.) G.L.Nesom
 (F.Muell. ex Benth.) Greene
 (F.Muell. ex Benth.) Guymer
@@ -6199,27 +6335,29 @@
 (F.Muell. ex Benth.) H.J.Lam
 (F.Muell. ex Benth.) H.Ohashi & K.Ohashi
 (F.Muell. ex Benth.) Hack.
 (F.Muell. ex Benth.) Hershk.
 (F.Muell. ex Benth.) Hughes
 (F.Muell. ex Benth.) I.Telford & Pruesapan
 (F.Muell. ex Benth.) J.M.Black
+(F.Muell. ex Benth.) Jackes & Trias-Blasi
 (F.Muell. ex Benth.) Jansen
 (F.Muell. ex Benth.) Jessup
 (F.Muell. ex Benth.) Kodela & Tindale
 (F.Muell. ex Benth.) Kraenzl.
 (F.Muell. ex Benth.) Kuhn
 (F.Muell. ex Benth.) Kuntze
 (F.Muell. ex Benth.) Kük.
 (F.Muell. ex Benth.) L.P.M.Willemse
 (F.Muell. ex Benth.) L.S.Sm.
 (F.Muell. ex Benth.) Labiak, Sundue & R.C.Moran
 (F.Muell. ex Benth.) Latiff
 (F.Muell. ex Benth.) Lazarides & R.D.Webster
 (F.Muell. ex Benth.) M.A.Clem., D.L.Jones & D.P.Banks
+(F.Muell. ex Benth.) M.D.Barrett, A.Hay & Hett.
 (F.Muell. ex Benth.) M.E.Jansen
 (F.Muell. ex Benth.) M.Gray & Given
 (F.Muell. ex Benth.) M.W.Frohl. & M.W.Chase
 (F.Muell. ex Benth.) Maesen
 (F.Muell. ex Benth.) Maiden
 (F.Muell. ex Benth.) Maiden & Betche
 (F.Muell. ex Benth.) Maiden & Blakely
@@ -6229,14 +6367,15 @@
 (F.Muell. ex Benth.) Nied.
 (F.Muell. ex Benth.) Noot.
 (F.Muell. ex Benth.) O.D.Evans
 (F.Muell. ex Benth.) O.E.Schulz
 (F.Muell. ex Benth.) Orchard
 (F.Muell. ex Benth.) P.I.Forst.
 (F.Muell. ex Benth.) P.M.Peterson
+(F.Muell. ex Benth.) P.M.Peterson, Romasch. & Soreng
 (F.Muell. ex Benth.) P.Royen
 (F.Muell. ex Benth.) P.S.Short
 (F.Muell. ex Benth.) Paul G.Wilson
 (F.Muell. ex Benth.) Pedley
 (F.Muell. ex Benth.) Perrie & Brownsey
 (F.Muell. ex Benth.) Pescott
 (F.Muell. ex Benth.) Planch.
@@ -6269,26 +6408,30 @@
 (F.Muell. ex Benth.) Tiegh.
 (F.Muell. ex Benth.) Tirveng.
 (F.Muell. ex Benth.) Trudgen
 (F.Muell. ex Benth.) Veldkamp
 (F.Muell. ex Benth.) W.M.Curtis
 (F.Muell. ex Benth.) W.R.Barker
 (F.Muell. ex Benth.) Zotov
+(F.Muell. ex Berk.) Dennis
 (F.Muell. ex Berk.) Kuntze
 (F.Muell. ex Berk.) Sacc.
 (F.Muell. ex Boeckeler) Domin
 (F.Muell. ex C.Moore) A.T.Lee
 (F.Muell. ex C.Moore) Craven & Biffin
 (F.Muell. ex C.Moore) Guymer & B.Hyland
+(F.Muell. ex Cooke) Henn.
+(F.Muell. ex Cooke) Sacc.
 (F.Muell. ex D.Dietr.) F.Muell.
 (F.Muell. ex Diels) Kraenzl.
 (F.Muell. ex Domin) Halford
 (F.Muell. ex Ewart & Sharman) B.G.Briggs & L.A.S.Johnson
 (F.Muell. ex Ewart) Ewart
 (F.Muell. ex F.L.Erickson & J.H.Willis) P.G.Farrell & S.H.James
+(F.Muell. ex F.M.Bailey) Ewart & Jean White
 (F.Muell. ex F.M.Bailey) Ewart, Jean White & B.Rees
 (F.Muell. ex F.M.Bailey) G.Harden & J.B.Williams
 (F.Muell. ex F.M.Bailey) W.D.Francis
 (F.Muell. ex H.Walter) A.S.George
 (F.Muell. ex H.Wendl. & Drude) F.M.Bailey
 (F.Muell. ex Hannaford) F.Muell.
 (F.Muell. ex Hannaford) Paul G.Wilson
@@ -6300,27 +6443,29 @@
 (F.Muell. ex Hook.f.) Benth.
 (F.Muell. ex Hook.f.) Domin
 (F.Muell. ex Hook.f.) E.B.Alexeev
 (F.Muell. ex Hook.f.) F.Muell.
 (F.Muell. ex Hook.f.) S.W.L.Jacobs
 (F.Muell. ex Hook.f.) Vickery
 (F.Muell. ex K.Schum.) Triest
+(F.Muell. ex Kalchbr.) Sacc.
 (F.Muell. ex Klatt) Benth.
 (F.Muell. ex Klatt) Domin
 (F.Muell. ex Klatt) L.W.Cayzer & Crisp
 (F.Muell. ex Kurz) Hegelm.
 (F.Muell. ex Kütz.) R.D.Wood
 (F.Muell. ex Kütz.) Zaneveld
 (F.Muell. ex Maiden & Betche) Maiden & Betche
 (F.Muell. ex Maiden) Pedley
 (F.Muell. ex Maiden) R.T.Baker
 (F.Muell. ex McGill.) Christenh. & Byng
 (F.Muell. ex Meisn.) Benth.
 (F.Muell. ex Meisn.) Christenh. & Byng
 (F.Muell. ex Meisn.) F.M.Bailey
+(F.Muell. ex Meisn.) F.Muell.
 (F.Muell. ex Meisn.) Kuntze
 (F.Muell. ex Miq.) Boland
 (F.Muell. ex Miq.) Cheel
 (F.Muell. ex Miq.) F.Muell.
 (F.Muell. ex Miq.) F.Muell. ex A.DC.
 (F.Muell. ex Miq.) F.Muell. ex Blakely
 (F.Muell. ex Miq.) F.Muell. ex Miq.
@@ -6331,28 +6476,28 @@
 (F.Muell. ex Müll.Arg.) Kuntze
 (F.Muell. ex Müll.Arg.) Müll.Arg.
 (F.Muell. ex Müll.Arg.) R.W.Bouman
 (F.Muell. ex N.A.Wakef.) Pedley
 (F.Muell. ex N.A.Wakef.) Tindale
 (F.Muell. ex Nyl.) Bibby
 (F.Muell. ex Nyl.) Nyl.
-(F.Muell. ex Nyl.) Nyl. ex Cromb.
 (F.Muell. ex Nyl.) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (F.Muell. ex Parl.) Quinn
 (F.Muell. ex Reissek) Benth.
 (F.Muell. ex Reissek) Druce
 (F.Muell. ex Reissek) F.Muell.
 (F.Muell. ex Reissek) J.M.Black
 (F.Muell. ex Reissek) L.B.Moore
 (F.Muell. ex Rodway) Kük.
 (F.Muell. ex Rodway) Rodway
 (F.Muell. ex Schltdl.) Benth.
 (F.Muell. ex Schltdl.) Domin
 (F.Muell. ex Schltdl.) F.Muell.
 (F.Muell. ex Schltdl.) R.M.Barker
+(F.Muell. ex Schott) M.D.Barrett, A.Hay & Hett.
 (F.Muell. ex Scort.) Christenh. & Byng
 (F.Muell. ex Scort.) F.Muell.
 (F.Muell. ex Sond.) F.Muell.
 (F.Muell. ex Sond.) Hieron.
 (F.Muell. ex Sond.) N.A.Wakef.
 (F.Muell. ex Tate) C.F.Wilkins & Whitlock
 (F.Muell. ex Tate) Carrick
@@ -6374,14 +6519,15 @@
 (F.Muell.) A.S.George & N.Gibson
 (F.Muell.) A.S.Mitch.
 (F.Muell.) A.T.Lee
 (F.Muell.) A.Terracc.
 (F.Muell.) A.V.Bobrov & Melikyan
 (F.Muell.) Aellen
 (F.Muell.) Airy Shaw
+(F.Muell.) Al-Shehbaz & Lysak
 (F.Muell.) Albr.
 (F.Muell.) Anderb.
 (F.Muell.) Anon.
 (F.Muell.) Aubrév.
 (F.Muell.) B.D.Jacks.
 (F.Muell.) B.G.Briggs & Ehrend.
 (F.Muell.) B.G.Briggs & L.A.S.Johnson
@@ -6463,40 +6609,41 @@
 (F.Muell.) Cranfield
 (F.Muell.) Craven
 (F.Muell.) Craven & Biffin
 (F.Muell.) Craven & R.D.Edwards
 (F.Muell.) Craven & S.R.Jones
 (F.Muell.) Crayn & Hislop
 (F.Muell.) Crisp
+(F.Muell.) Crisp & L.G.Cook
 (F.Muell.) Crisp & P.H.Weston
 (F.Muell.) Crisp & R.L.Barrett
 (F.Muell.) D.A.Cooke
 (F.Muell.) D.A.Simpson
 (F.Muell.) D.A.Sm. & Tindale
 (F.Muell.) D.C.Thomas, Chaowasku & R.M.K.Saunders
 (F.Muell.) D.F.Cutler
 (F.Muell.) D.J.Bedford
 (F.Muell.) D.L.Jones
 (F.Muell.) D.L.Jones & M.A.Clem.
 (F.Muell.) D.Legrand
 (F.Muell.) Danser
-(F.Muell.) Dennis
 (F.Muell.) Diels
 (F.Muell.) Diels & Loes.
 (F.Muell.) Dockrill
 (F.Muell.) Domin
 (F.Muell.) Domin ex Ulbr.
 (F.Muell.) Downing
 (F.Muell.) Druce
 (F.Muell.) Drude
 (F.Muell.) Dubard
 (F.Muell.) Dunlop
 (F.Muell.) Duretto & Heslewood
 (F.Muell.) Duretto & K.L.Durham
 (F.Muell.) E.A.Shaw
+(F.Muell.) E.B.Knox
 (F.Muell.) E.L.Robertson
 (F.Muell.) E.M.Benn.
 (F.Muell.) E.Pritz.
 (F.Muell.) E.Wimm.
 (F.Muell.) Eb.Fisch., Schäferh. & Kai Müll.
 (F.Muell.) Edlin
 (F.Muell.) Engl.
@@ -6519,16 +6666,15 @@
 (F.Muell.) F.Muell. ex Holle
 (F.Muell.) F.Muell. ex Hook.f.
 (F.Muell.) F.Muell. ex J.M.Black
 (F.Muell.) F.Muell. ex Klatt
 (F.Muell.) F.Muell. ex Koehne
 (F.Muell.) F.Muell. ex Maiden
 (F.Muell.) F.Muell. ex Parl.
-(F.Muell.) F.Muell. x Duboisia myoporoides R.Br.
-(F.Muell.) F.Muell. x Grammosolen dixonii (F.Muell. & Tate) Haegi
+(F.Muell.) F.Muell. ex Schltdl.
 (F.Muell.) Fagerl.
 (F.Muell.) Farmar
 (F.Muell.) Fitzg.
 (F.Muell.) Forman
 (F.Muell.) Fosberg
 (F.Muell.) Fosberg & Sachet
 (F.Muell.) Fritsch
@@ -6555,26 +6701,24 @@
 (F.Muell.) H.Deane & Maiden
 (F.Muell.) H.Eichler
 (F.Muell.) H.J.Lam
 (F.Muell.) H.Ohashi & K.Ohashi
 (F.Muell.) H.Wendl. & Drude
 (F.Muell.) Hack.
 (F.Muell.) Haegi
-(F.Muell.) Haegi x Grammosolen dixonii (F.Muell. & Tate) Haegi
 (F.Muell.) Halford
 (F.Muell.) Halford & R.J.F.Hend.
 (F.Muell.) Hallier f.
 (F.Muell.) Harms
 (F.Muell.) Hartog
 (F.Muell.) Hattink
 (F.Muell.) Heads
 (F.Muell.) Heenan & Smissen
 (F.Muell.) Heine
 (F.Muell.) Hemsl.
-(F.Muell.) Henn.
 (F.Muell.) Hershk.
 (F.Muell.) Heslewood
 (F.Muell.) Heusden
 (F.Muell.) Hislop, Crayn & Puente-Lel.
 (F.Muell.) Hochr.
 (F.Muell.) Holttum
 (F.Muell.) Hoogland
@@ -6614,15 +6758,14 @@
 (F.Muell.) Jackes & Rossetto
 (F.Muell.) Jeanes
 (F.Muell.) Jessup
 (F.Muell.) Jobson & P.H.Weston
 (F.Muell.) K.A.Sheph.
 (F.Muell.) K.A.Sheph. & Paul G.Wilson
 (F.Muell.) K.D.Hill & L.A.S.Johnson
-(F.Muell.) K.D.Hill & L.A.S.Johnson x Corymbia lamprophylla (Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson
 (F.Muell.) K.D.Scott, W.K.Harris & Playford
 (F.Muell.) K.F.Chung
 (F.Muell.) K.Krause
 (F.Muell.) K.L.Gibbons
 (F.Muell.) K.L.Wilson
 (F.Muell.) K.L.Wilson & J.J.Bruhl
 (F.Muell.) K.R.Thiele
@@ -6658,44 +6801,41 @@
 (F.Muell.) Lazarides
 (F.Muell.) Lehtonen
 (F.Muell.) Lewton
 (F.Muell.) Liede
 (F.Muell.) Lincz.
 (F.Muell.) Lindau
 (F.Muell.) Loes.
-(F.Muell.) Loes. x Maytenus silvestris Lander & L.A.S.Johnson
 (F.Muell.) Luerss.
 (F.Muell.) Lugger
 (F.Muell.) M.A.Clem.
 (F.Muell.) M.A.Clem. & D.L.Jones
+(F.Muell.) M.D.Barrett, A.Hay & Hett.
 (F.Muell.) M.G.Harr.
 (F.Muell.) M.G.Harr. & Zich
 (F.Muell.) M.Gray
 (F.Muell.) M.Hiroe
 (F.Muell.) M.Kral
 (F.Muell.) M.L.Moody & Les
 (F.Muell.) M.P.Simmons
-(F.Muell.) M.P.Simmons x Denhamia silvestris (Lander & L.A.S.Johnson) M.P.Simmons
 (F.Muell.) M.Pell. & C.N.Horn
 (F.Muell.) M.W.Chase, Christenh. & Schuit.
 (F.Muell.) M.W.Frohl. & M.W.Chase
 (F.Muell.) Mabb.
 (F.Muell.) Mabb. & Holzmeyer
 (F.Muell.) Maconochie
 (F.Muell.) Maesen
 (F.Muell.) Maiden
 (F.Muell.) Maiden & Betche
-(F.Muell.) Maiden & Betche x Phebalium rotundifolium (A.Cunn. ex Endl.) Benth.
 (F.Muell.) Makinson
 (F.Muell.) Marchand
 (F.Muell.) Martelli
 (F.Muell.) Mattf.
 (F.Muell.) McGill.
 (F.Muell.) Meijden
-(F.Muell.) Meisn. ex F.Muell.
 (F.Muell.) Melville
 (F.Muell.) Merr.
 (F.Muell.) Merr. & L.M.Perry
 (F.Muell.) Mez
 (F.Muell.) Mich.J.Parsons
 (F.Muell.) Miers
 (F.Muell.) Mildbr.
@@ -6734,15 +6874,14 @@
 (F.Muell.) P.S.Short
 (F.Muell.) P.S.Short & Paul G.Wilson
 (F.Muell.) P.W.Michael & Vickery
 (F.Muell.) Pamp.
 (F.Muell.) Paris
 (F.Muell.) Parl.
 (F.Muell.) Paul G.Wilson
-(F.Muell.) Paul G.Wilson x Leionema rotundifolium (A.Cunn. ex Endl.) Paul G.Wilson
 (F.Muell.) Pax
 (F.Muell.) Pax & K.Hoffm.
 (F.Muell.) Pedley
 (F.Muell.) Pedley ex Halford
 (F.Muell.) Pedley ex K.L.Gibbons
 (F.Muell.) Perkins
 (F.Muell.) Pescott
@@ -6793,31 +6932,29 @@
 (F.Muell.) Roberty
 (F.Muell.) Rodway
 (F.Muell.) Rolfe
 (F.Muell.) Roshev.
 (F.Muell.) Rozefelds & H.C.Hopkins
 (F.Muell.) Rupp
 (F.Muell.) Rupp & T.E.Hunt
-(F.Muell.) Rupp & T.E.Hunt x Dendrobium affine (Decne.) Steud.
 (F.Muell.) Rye
 (F.Muell.) Rye & Kellermann
 (F.Muell.) Rye & Trudgen
 (F.Muell.) S.A.Graham & Gandhi
 (F.Muell.) S.B.Andrews
 (F.Muell.) S.Moore
-(F.Muell.) S.Moore x Cratystylis microphylla S.Moore
 (F.Muell.) S.T.Blake
 (F.Muell.) S.T.Reynolds
 (F.Muell.) S.T.Reynolds & P.I.Forst.
 (F.Muell.) S.T.Reynolds & R.J.F.Hend.
 (F.Muell.) S.Venter
 (F.Muell.) S.W.L.Jacobs
 (F.Muell.) S.W.L.Jacobs & J.Everett
 (F.Muell.) S.Y.Dong
-(F.Muell.) Sacc.
+(F.Muell.) Satthaphorn
 (F.Muell.) Schindl.
 (F.Muell.) Schltr.
 (F.Muell.) Schmidt-Leb.
 (F.Muell.) Schodde
 (F.Muell.) Schot
 (F.Muell.) Seem.
 (F.Muell.) Skeels
@@ -6872,57 +7009,60 @@
 (F.Muell.) Wangerin
 (F.Muell.) Weber Bosse
 (F.Muell.) Wettst.
 (F.Muell.) Whiffin
 (F.Muell.) Wills & J.J.Bruhl
 (F.Muell.) Wunderlin
 (F.Muell.) X.A.Weber & Schmidt-Leb.
+(F.Muell.) Zuntini & Frankel
 (F.Muell.) Škorničk. & M.F.Newman
 (F.Schill.) Vězda
 (F.Schmidt) Janch.
 (F.Schmidt) Nakai
 (F.Schmidt) Ronse Decr.
 (F.Schmitz ex Mazza) Papenf.
 (F.Schütt) Balech
 (F.Schütt) D.X.Qiu & Senjie Lin
 (F.Schütt) E.J.Schmidt
 (F.Schütt) Entz
 (F.Schütt) F.Gómez
 (F.Schütt) F.Schütt
 (F.Schütt) G.A.Klebs
 (F.Schütt) G.Murray & Whitting
-(F.Schütt) Jörg.
+(F.Schütt) Jørg.
 (F.Schütt) Kof.
 (F.Schütt) Kof. & Swezy
 (F.Schütt) Lemmerm.
 (F.Schütt) Pavill.
 (F.Schütt) T.H.Abé
 (F.Schütt) VanLand.
-(F.Stein ex Jörg.) J.D.Dodge & S.Toriumi
+(F.Stein ex Jørg.) J.D.Dodge & S.Toriumi
 (F.Stein) A.R.Loebl.
 (F.Stein) Balech
 (F.Stein) Biecheler
 (F.Stein) Bourr.
 (F.Stein) Calado & Moestrup
 (F.Stein) Carty
 (F.Stein) E.G.Pringsh.
 (F.Stein) Er.Lindem.
 (F.Stein) F.J.R.Taylor
 (F.Stein) G.A.Klebs
 (F.Stein) G.Murray & Whitting
 (F.Stein) Gert Hansen & G.Flaim
 (F.Stein) Hub.-Pest.
 (F.Stein) J.D.Dodge
-(F.Stein) Jörg.
+(F.Stein) Jørg.
 (F.Stein) Kof. & Skogsb.
 (F.Stein) Lemmerm.
+(F.Stein) Ostenf.
 (F.Stein) Parke & P.S.Dixon
 (F.Stein) Pascher
 (F.Stein) Schröd.
 (F.Stein) T.H.Abé
+(F.Stein) T.H.Abé ex J.D.Dodge
 (F.Stein) Y.Takano & T.Horiguchi
 (F.Stevens & Dalbey) U.Braun
 (F.Stevens & Tehon) F.Stevens
 (F.Stevens) Deighton
 (F.Stevens) M.B.Ellis
 (F.Stevens) Petr.
 (F.Stevens) Piroz. & S.D.Patil
@@ -6931,26 +7071,26 @@
 (F.W.Lewis) Playfair
 (F.W.Lewis) Van Heurck ex Hanna
 (F.W.Schultz ex Godr.) A.R.Clapham
 (F.W.Schultz ex Godr.) P.Fourn.
 (F.W.Schultz) Cout.
 (F.W.Schultz) Kindb.
 (F.Weber & D.Mohr) A.L.Andrews
+(F.Weber & D.Mohr) Aresch.
+(F.Weber & D.Mohr) C.Agardh
 (F.Weber & D.Mohr) H.Rob.
 (F.Weber & D.Mohr) I.Hagen
 (F.Weber & D.Mohr) J.Agardh
 (F.Weber & D.Mohr) J.J.Amann
 (F.Weber & D.Mohr) Jenn.
 (F.Weber & D.Mohr) Kütz.
 (F.Weber & D.Mohr) Lindb.
 (F.Weber & D.Mohr) Schimp.
-(F.Weber & Mohr) Aresch.
-(F.Weber & Mohr) C.Agardh
-(F.Weber & Mohr) Kütz.
 (F.Weber) Grolle
+(F.Weber) Jan Kučera
 (F.Weber) Mitt.
 (F.Weber) R.M.Schust.
 (F.Wilson) D.J.Galloway
 (F.Wilson) D.J.Galloway & P.James
 (F.Wilson) Degel.
 (F.Wilson) F.Wilson
 (F.Wilson) Hale
@@ -6958,32 +7098,33 @@
 (F.Wilson) J.H.Willis
 (F.Wilson) J.S.Murray
 (F.Wilson) Müll.Arg.
 (F.Wilson) Shirley
 (F.Wilson) Tibell
 (F.Wilson) Yoshim.
 (F.Wilson) Zahlbr.
+(Fairm.) Petr. & Syd.
 (Falkenb.) Kylin
 (Farkas & Vězda) Kalb & Lücking
 (Farkas & Vězda) Lücking
 (Farl. & Burt) Vellinga
 (Farl.) Levring
 (Farl.) P.S.Dixon
 (Farl.) R.E.Norris & A.Millar
 (Farl.) Samson
 (Farmar) Benl
 (Fautrey & Roum.) G.A.de Vries
 (Fawcett) Lickey, K.W.Hughes & R.H.Petersen
 (Fayod) Kühner
-(Fayod) R.Heim
+(Feldm.-Maz.) Huisman & G.T.Kraft
 (Feldmann & Hamel) Santel.
 (Feldmann) Cribb & J.W.Cribb
 (Feldmann) Feldmann & Hamel
 (Feldmann) Kohlm.
-(Fennell & Raper) Kozak., Aspergillus
+(Fennell & Raper) Kozak.
 (Fenzl) A.R.Bean
 (Fenzl) A.S.George ex J.W.Green
 (Fenzl) Benth.
 (Fenzl) Carolin ex Hershk.
 (Fenzl) Cufod.
 (Fenzl) F.Muell.
 (Fenzl) Hereman
@@ -6994,15 +7135,15 @@
 (Fenzl) Nees
 (Fenzl) Nees ex Reissek
 (Fenzl) Rouy & Fouc.
 (Fenzl) Rye
 (Fenzl) Seem.
 (Fenzl) Tiegh.
 (Fenzl) Walters
-(Ferd. & Winge) Samuels & Schroers
+(Ferd. & Winge) Schroers & Samuels
 (Fernald) Bogin
 (Fernald) Cabrera
 (Fernald) S.F.Blake
 (Ficinus & C.Schub.) Castagne
 (Fielding & Gardner) Hnatiuk
 (Fig. & De Not.) Henrard
 (Fig. & De Not.) S.T.Blake
@@ -7032,43 +7173,39 @@
 (Fitzg.) J.H.Willis & Court
 (Fitzg.) J.J.Verm.
 (Fitzg.) J.M.H.Shaw
 (Fitzg.) J.Z.Weber & R.J.Bates
 (Fitzg.) Kuntze
 (Fitzg.) M.A.Clem.
 (Fitzg.) M.A.Clem. & D.L.Jones
+(Fitzg.) M.A.M.Renner
 (Fitzg.) Maiden & Betche
 (Fitzg.) Nicholls
 (Fitzg.) Rauschert
 (Fitzg.) Rchb.f.
 (Fitzg.) Rupp
 (Fitzg.) St.Cloud
 (Fitzg.) Szlach.
 (Flann) R.J.Bayer
-(Florke ex Sommerf.) Spreng.
 (Florke ex Sommerf.) Zopf
-(Florke) Fr.
-(Florke) Hale
-(Florke) Schaer.
-(Florke) Vain.
 (Flot. ex Kütz.) Hansg.
 (Flot.) Flot.
 (Flot.) Hertel & Poelt
 (Flot.) Kalb & Hafellner
 (Flot.) Kalb, Hafellner, Fryday & Lendemer
 (Flot.) Körb.
+(Flot.) Kütz.
 (Flot.) Mudd
 (Flot.) Nyl.
 (Flot.) Poelt & Vězda
 (Flot.) Sipman
 (Flot.) Wittr.
 (Flot.) Zahlbr.
 (Flotow) S.Ekman & M.Svennson
 (Flotow) Vězda & V.Wirth
-(Flowtow) Kütz.
 (Flörke ex Rabenh.) Hertel & Rambold
 (Flörke ex Sommerf.) Spreng.
 (Flörke) A.Schmidt
 (Flörke) Arup, Frödén & Søchting
 (Flörke) F.Wilson
 (Flörke) Fr.
 (Flörke) H.Mayrhofer & Poelt
@@ -7095,15 +7232,14 @@
 (Fontell) Hust.
 (Forbes ex Otto & A.Dietr.) Riccob.
 (Forde & Ising) Pedley
 (Forssk.) Asch.
 (Forssk.) Asch. & Schweinf. ex Asch.
 (Forssk.) Baker
 (Forssk.) Brownsey & Jermy
-(Forssk.) Brownsey & Jermy x Christella parasitica (L.) H.Lev.
 (Forssk.) Bubani
 (Forssk.) Børgesen
 (Forssk.) C.Agardh
 (Forssk.) C.Chr.
 (Forssk.) Ching
 (Forssk.) Chiov.
 (Forssk.) Christenh.
@@ -7168,57 +7304,58 @@
 (Foslie) Weber Bosse
 (Foslie) Wilks & Woelk.
 (Foslie) Woelk.
 (Foslie) Woelk., Y.M.Chamb. & P.C.Silva
 (Foslie) Y.M.Chamb.
 (Foslie) Zaberzhinskaya ex Zinova
 (Fr. & Hök) A.H.Sm. & Thiers
-(Fr. : Fr.) Fr.
-(Fr. : Fr.) P.Kumm.
-(Fr. : Fr.) Staude
-(Fr. : Fr.) Wunsche
+(Fr. & Palmquist) G.Lister
 (Fr. ex Klotzsch) Fr.
 (Fr. ex Klotzsch) Ryvarden
 (Fr. ex P.Karst.) G.Cunn.
 (Fr. ex P.Karst.) Murrill
 (Fr. ex P.Karst.) Pilát
 (Fr. ex Rabenh.) P.Kumm.
 (Fr.) A.H.Sm.
-(Fr.) A.H.Sm. & H.E.Bigelow
 (Fr.) A.Massal.
+(Fr.) A.N.Mill. & Huhndorf
 (Fr.) A.Pearson & Dennis
 (Fr.) Antonín, Halling & Noordel.
-(Fr.) Aptroot
 (Fr.) Arnold
 (Fr.) Arnolds
 (Fr.) Arx
+(Fr.) Audet
+(Fr.) B.K.Cui, M.L.Han & Y.C.Dai
 (Fr.) Barbier
+(Fr.) Bertill.
 (Fr.) Bigeard & H.Guill.
 (Fr.) Boedijn
 (Fr.) Boidin
 (Fr.) Bon
+(Fr.) Bondartsev & Singer
 (Fr.) Boud.
 (Fr.) Bourdot
 (Fr.) Bref.
 (Fr.) Bres.
 (Fr.) Britzelm.
 (Fr.) Burt
 (Fr.) C.F.Baker
 (Fr.) Ces.
+(Fr.) Ces. & De Not.
 (Fr.) Cleland & Cheel
 (Fr.) Cooke
 (Fr.) Cooke & Quél.
 (Fr.) Coppins & P.James
 (Fr.) Corda
 (Fr.) Corner
+(Fr.) Crous & Aptroot
 (Fr.) D.A.Reid
 (Fr.) D.D.Awasthi
 (Fr.) D.J.Galloway
 (Fr.) De Not.
-(Fr.) De Not. & Ces.
 (Fr.) De Toni
 (Fr.) Dennis
 (Fr.) Dennis & Rifai
 (Fr.) Donk
 (Fr.) Dyko & B.Sutton
 (Fr.) E.-J.Gilbert
 (Fr.) E.Horak
@@ -7228,38 +7365,41 @@
 (Fr.) Flörke
 (Fr.) Fr.
 (Fr.) G.Cunn.
 (Fr.) G.Winter
 (Fr.) Gilb.
 (Fr.) Gilb. & Ryvarden
 (Fr.) Gillet
+(Fr.) Ginns
 (Fr.) Ginns & Weresub
+(Fr.) Gminder
 (Fr.) Gray
 (Fr.) Gulden
+(Fr.) H.E.Bigelow & A.H.Sm.
 (Fr.) H.Olivier
+(Fr.) Hai J.Li & S.H.He
 (Fr.) Haszl.
 (Fr.) Hedl.
 (Fr.) Heinem.
 (Fr.) Henn.
 (Fr.) Hertel & A.J.Schwab
 (Fr.) Hesler
-(Fr.) Huhndorf & A.N.Mill.
 (Fr.) Höhn. & Litsch.
 (Fr.) J.E.Lange
 (Fr.) J.Erikss.
 (Fr.) J.Erikss. & Ryvarden
-(Fr.) J.Kickx f
 (Fr.) J.Kickx f.
 (Fr.) J.T.Palmer
 (Fr.) J.Walker
 (Fr.) Jarosch & Besl
 (Fr.) Jülich
 (Fr.) Jülich & Stalpers
 (Fr.) Kalb
 (Fr.) Kits van Wav.
+(Fr.) Konrad & Maubl.
 (Fr.) Kotl. & Pouzar
 (Fr.) Kreisel
 (Fr.) Kuntze
 (Fr.) Kuyper & Noordel.
 (Fr.) Körb.
 (Fr.) Kühner
 (Fr.) Kühner & Maire
@@ -7268,32 +7408,32 @@
 (Fr.) Lambotte
 (Fr.) Largent & R.G.Benedict
 (Fr.) Liberta
 (Fr.) Lind
 (Fr.) Link
 (Fr.) Lister
 (Fr.) Lloyd
-(Fr.) Lombard & M.J.Larsen
 (Fr.) Lowe
-(Fr.) Lutzoni, Redhead, Moncalvo & Vilgalys
 (Fr.) Lév.
+(Fr.) M.J.Larsen & Lombard
 (Fr.) M.Lange
 (Fr.) M.Lange & Sivertsen
 (Fr.) M.M.Moser
 (Fr.) M.P.Christ.
 (Fr.) Maire
 (Fr.) Marbach & H.Mayrhofer
 (Fr.) Massee
-(Fr.) Maubl. & Konrad
+(Fr.) Melo & Ryvarden
 (Fr.) Mont.
 (Fr.) Mudd
 (Fr.) Murrill
 (Fr.) Müll.Arg
 (Fr.) Müll.Arg.
 (Fr.) Nakasone
+(Fr.) Niskanen & Liimat.
 (Fr.) Nobles
 (Fr.) Noordel.
 (Fr.) Nyl.
 (Fr.) Opiz
 (Fr.) Overh.
 (Fr.) P.A.Lemke
 (Fr.) P.D.Orton
@@ -7302,61 +7442,67 @@
 (Fr.) P.M.Jørg.
 (Fr.) P.M.Jørg. & D.J.Galloway
 (Fr.) Park.-Rhodes
 (Fr.) Pat.
 (Fr.) Pegler & T.W.K.Young
 (Fr.) Pilát
 (Fr.) Pouzar
-(Fr.) Quel.
 (Fr.) Quél.
 (Fr.) R.H.Petersen
 (Fr.) R.Heim
 (Fr.) Rabenh.
 (Fr.) Raithelh.
 (Fr.) Rauschert
+(Fr.) Redhead
+(Fr.) Redhead, Lutzoni, Moncalvo & Vilgalys
 (Fr.) Redhead, Moncalvo, Vilgalys & Lutzoni
+(Fr.) Redhead, Moncalvo, Vilgalys, Desjardin & B.A.Perry
 (Fr.) Redhead, Vilgalys & Hopple
 (Fr.) Redhead, Vilgalys & Moncalvo
 (Fr.) Rehm
 (Fr.) Rexer
 (Fr.) Ricken
 (Fr.) Rostaf.
 (Fr.) Rostr.
 (Fr.) Ryvarden
+(Fr.) S.H.He & Jiao Yang
+(Fr.) S.H.He & Y.C.Dai
 (Fr.) Sacc.
 (Fr.) Sawada
 (Fr.) Singer
-(Fr.) Singer & Bondartsev
 (Fr.) Singer ex Bon & Bellù
 (Fr.) Staude
 (Fr.) Syd. & P.Syd.
 (Fr.) T.Wagner & M.Fisch.
 (Fr.) Teng
 (Fr.) Th.Fr.
 (Fr.) Tul.
 (Fr.) Tul. & C.Tul.
+(Fr.) V.Hofst., Clémençon, Vilgalys & Redhead
+(Fr.) Vizzini & Matheny
 (Fr.) W.B.Cooke
 (Fr.) W.G.Sm.
 (Fr.) W.Phillips
 (Fr.) Wallr.
 (Fr.) Warcup
 (Fr.) Watling
 (Fr.) Wünsche
+(Fr.) Zmitr. & Kovalenko
+(Fr.) Zmitr., Wasser & Ezhov
 (Franch. & Sav.) C.B.Clarke
 (Franch. & Sav.) C.Chr.
 (Franch. & Sav.) J.Jung & H.K.Choi
 (Franch. & Sav.) T.Koyama
 (Franch.) C.K.Schneid.
 (Franch.) Focke
 (Franch.) M.F.Fay & Christenh.
 (Franch.) Skottsb.
 (Franch.) Wunderlin
 (Franch.) de la Sota
 (Francé) Lemmerm.
-(Fraser) Cif. & Bat.
 (Freng.) Hust.
 (Fresen.) A.Batko
 (Fresen.) Cienkowski
 (Fresen.) F.C.Harrison
 (Fresen.) G.A.Klebs
 (Fresen.) G.A.de Vries
 (Fresen.) H.S.Irwin & Barneby
@@ -7372,38 +7518,40 @@
 (Fryxell & Hasle) A.J.Alverson, S.H.Kang & E.C.Ther.
 (Fryxell) B.E.Pfeil & Craven
 (Fryxell) Craven & B.E.Pfeil
 (Frémy) Anagn. & Komárek
 (Frémy) Umezaki & M.Watan.
 (Fuckel) Boud.
 (Fuckel) Dunegan
+(Fuckel) Fresen.
+(Fuckel) Gräfenhan, Seifert & Schroers
 (Fuckel) J.Moravec
 (Fuckel) Karak.
-(Fuckel) M.A.Litv. & Tranzschel
 (Fuckel) M.E.Barr
 (Fuckel) M.E.Barr & E.G.Simmons
 (Fuckel) Nannf.
 (Fuckel) Raitv.
 (Fuckel) S.Hughes
 (Fuckel) Sacc.
 (Fuckel) T.Schumach.
+(Fuckel) Tranzschel & M.A.Litv.
 (Fuckel) W.Phillips
 (Fuckel) Woronin
 (Fukushi) Arx
 (Fukuy.) Masam.
+(Funck) Bedn.-Ochyra & Ochyra
 (Funck) Bruch & Schimp.
 (Fée) A.Massal.
 (Fée) A.W.Archer
 (Fée) Alderw.
 (Fée) Aptroot & Lücking
 (Fée) Aptroot, Lücking & G.Thor
 (Fée) Baker
 (Fée) Bedd.
 (Fée) Benth.
-(Fée) C.Presl
 (Fée) Copel.
 (Fée) D.D.Awasthi
 (Fée) D.J.Galloway & P.James
 (Fée) Domin
 (Fée) Egea & Torrente
 (Fée) F.Muell.
 (Fée) Fée
@@ -7430,53 +7578,54 @@
 (Fée) Tagawa
 (Fée) Tagawa & K.Iwats.
 (Fée) Tuck.
 (Fée) Underw.
 (Fée) Vain.
 (Fée) Vězda
 (Fée) Zahlbr.
+(G.A.Forbes, Windels & L.W.Burgess) L.W.Burgess & Summerell
 (G.A.Klebs) Er.Lindem.
 (G.A.Klebs) Lemmerm.
 (G.A.Klebs) Pascher
 (G.A.Klebs) Playfair
-(G.A.de Vries & de Hoog) R.T.Moore
-(G.A.de Vries & de Hoog) Sigler
-(G.A.de Vries & de Hoog) Z.W.de Beer, Begerow & R.Bauer
 (G.Arnaud) Cif. & Bat.
 (G.C.Wall.) F.Gómez, Lu Wang & Senjie Lin
 (G.C.Wall.) F.Schütt
 (G.C.Wall.) Grunow
 (G.C.Wall.) Hendey
 (G.C.Wall.) Medlin & P.A.Sims
 (G.C.Wall.) P.Lundell
 (G.C.Wall.) W.B.Turner
 (G.Cunn.) Bougher & Castellano
 (G.Cunn.) Burds.
-(G.Cunn.) Castellano & Trappe
 (G.Cunn.) Corner
 (G.Cunn.) D.A.Reid
 (G.Cunn.) E.Horak
 (G.Cunn.) G.Cunn.
 (G.Cunn.) G.W.Beaton, Pegler & T.W.K.Young
 (G.Cunn.) Grgur.
 (G.Cunn.) Hjortstam
+(G.Cunn.) J.A.Cooper
 (G.Cunn.) J.Walker
 (G.Cunn.) Jülich
+(G.Cunn.) Kuhar, Nouhra & M.E.Sm.
+(G.Cunn.) M.D.Barrett
 (G.Cunn.) M.P.Christ.
-(G.Cunn.) McKenzie & Vánky
 (G.Cunn.) Meng Zhou, Y.C.Dai & T.W.May
 (G.Cunn.) Nakasone
 (G.Cunn.) P.K.Buchanan & Ryvarden
 (G.Cunn.) Pfister
 (G.Cunn.) Rajchenb.
 (G.Cunn.) Ryvarden
 (G.Cunn.) Singer
 (G.Cunn.) Stalpers
 (G.Cunn.) Stalpers & P.K.Buchanan
+(G.Cunn.) Trappe & Castellano
 (G.Cunn.) Vánky
+(G.Cunn.) Vánky & McKenzie
 (G.Don) A.J.Scott
 (G.Don) A.S.George
 (G.Don) A.T.Lee
 (G.Don) A.Terracc.
 (G.Don) Asch. & Graebn.
 (G.Don) Benth.
 (G.Don) Carolin
@@ -7487,15 +7636,14 @@
 (G.Don) Ford & Vickery
 (G.Don) Goodsp.
 (G.Don) Hutch. & Dalziel
 (G.Don) Joy Thomps.
 (G.Don) K.A.Sheph.
 (G.Don) K.Schum.
 (G.Don) Kuntze
-(G.Don) Kuntze x Brachychiton diversifolius R.Br.
 (G.Don) Paul G.Wilson
 (G.Don) Pedley
 (G.Don) Polhill
 (G.Don) Radlk.
 (G.Don) Sol. ex Lindl.
 (G.Don) Spach
 (G.Don) Steud.
@@ -7536,15 +7684,14 @@
 (G.Forst.) Carr
 (G.Forst.) Cham. & Schltdl.
 (G.Forst.) Chew
 (G.Forst.) Ching
 (G.Forst.) Christ
 (G.Forst.) Christenh.
 (G.Forst.) Cockayne
-(G.Forst.) Cockayne x Pteridium revolutum (Blume) Nakai
 (G.Forst.) Copel.
 (G.Forst.) Croizat
 (G.Forst.) DC.
 (G.Forst.) Desv.
 (G.Forst.) Domin
 (G.Forst.) Endl.
 (G.Forst.) F.M.Bailey
@@ -7594,17 +7741,19 @@
 (G.Forst.) R.Br. ex Roem. & Schult.
 (G.Forst.) R.Br. ex Sm.
 (G.Forst.) R.W.Bouman
 (G.Forst.) Radlk.
 (G.Forst.) Rchb.f.
 (G.Forst.) Roem. & Schult.
 (G.Forst.) Rothm.
+(G.Forst.) S.E.Fawc. & A.R.Sm.
 (G.Forst.) Schkuhr
 (G.Forst.) Schltdl.
 (G.Forst.) Seem.
+(G.Forst.) Smissen, Breitw. & de Lange
 (G.Forst.) Spreng.
 (G.Forst.) Steud.
 (G.Forst.) Sw.
 (G.Forst.) Sweet
 (G.Forst.) T.Anderson ex Hemsl.
 (G.Forst.) T.Moore
 (G.Forst.) Testo & A.R.Field
@@ -7619,41 +7768,39 @@
 (G.Forst.) Willd.
 (G.Forst.) Zotov
 (G.Forst.) d'Urv.
 (G.Forst.) Á.Löve & D.Löve
 (G.H.Otth) Arx
 (G.J.Allman) Kof. & Swezy
 (G.J.Leach) Brooker
+(G.J.Leach) D.Nicolle
 (G.J.Leach) K.R.Thiele & Ladiges
 (G.J.Leach) L.A.S.Johnson & K.D.Hill
 (G.J.Leach) Pedley
 (G.Karst.) Balech
 (G.Karst.) Böhm
 (G.Karst.) F.Gómez
 (G.Karst.) F.Gómez, D.Moreira & López-García
 (G.Karst.) G.Karst.
-(G.Karst.) Jörg
-(G.Karst.) Jörg.
+(G.Karst.) Jørg.
 (G.Karst.) Nothig & Ligowski
 (G.Karst.) Paulsen
 (G.Karst.) Sournia
 (G.Kirchn.) Bean
-(G.L.Barron & L.V.Busch) Arx & de Hoog
+(G.L.Barron & L.V.Busch) de Hoog & Arx
 (G.L.Barron) Udagawa & Furuya
 (G.L.Davis) Jeanes
 (G.L.Davis) P.S.Short
 (G.L.Mey.) Gumbl.
-(G.L.Mey.) Gumbl. x Freesia leichtlinii Klatt
 (G.L.Mey.) J.C.Manning & Goldblatt
 (G.L.Stout) Shoemaker
 (G.L.Stout) Subram. & B.L.Jain
 (G.L.Webster) R.W.Bouman
 (G.Lister & Cran) Alexop.
 (G.Lister & Cran) R.J.G.Hertel ex Nann.-Bremek.
-(G.Lister & Lister) Lister ex E.Jahn
 (G.Lister) G.Lister
 (G.Lister) Hagelst.
 (G.Lister) Ing
 (G.Lister) Ladó
 (G.Lister) Nann.-Bremek.
 (G.Lodd.) Benth. ex Voss
 (G.Lodd.) G.Don
@@ -7682,15 +7829,14 @@
 (G.Mey.) L.P.Queiroz & Snak
 (G.Mey.) Les & D.J.Crawford
 (G.Mey.) Maréchal, Mascherpa & Stainier
 (G.Mey.) Massee
 (G.Mey.) Pat.
 (G.Mey.) Sacc.
 (G.Mey.) Verdc.
-(G.Moreno & Manjón) Hjortstam, Manjón & G.Moreno
 (G.Murray & Whitting) Balech
 (G.Murray & Whitting) G.Murray & Whitting
 (G.Murray & Whitting) J.D.Dodge
 (G.Murray & Whitting) Kof.
 (G.Murray & Whitting) Kof. & Skogsb.
 (G.Murray & Whitting) Schröd.
 (G.Murray & Whitting) T.H.Abé
@@ -7717,58 +7863,67 @@
 (G.Schellenb.) Sleumer
 (G.Schmid) Anagn. & Komárek
 (G.Schneid.) Nakai
 (G.Schneid.) S.B.Andrews
 (G.Stev.) A.M.Young
 (G.Stev.) E.Horak
 (G.Stev.) Herink
+(G.Stev.) J.A.Cooper
+(G.Stev.) Largent
 (G.Stev.) McNabb
 (G.Stev.) Segedin
 (G.Stev.) Segedin, P.K.Buchanan & J.P.Wilkie
 (G.Stev.) T.W.May & A.E.Wood
+(G.Stev.) Vizzini
 (G.Stev.) Watling
 (G.Stev.) Wolfe
 (G.T.Kraft & A.Millar) G.T.Kraft
 (G.Thor & Vězda) Lücking, Aptroot & Sipman
 (G.Thor) Aptroot, Lücking & G.Thor
 (G.Thor) G.Thor
-(G.W.Beaton & Malajczuk) Castellano, Trappe & Malajczuk
-(G.W.Beaton & Weste) Castellano, Trappe & Malajczuk
+(G.W.Beaton & M.B.Ellis) S.Hughes
+(G.W.Beaton & Malajczuk) Trappe, Castellano & Malajczuk
 (G.W.Beaton & Weste) L.M.Kohn
+(G.W.Beaton & Weste) P.R.Johnst.
 (G.W.Beaton & Weste) Spooner
+(G.W.Beaton & Weste) Trappe, Castellano & Malajczuk
 (G.W.Beaton) B.C.Zhang & Minter
-(G.W.Beaton) Castellano, Trappe & Amar.
 (G.W.Beaton) Kraisit., Pfister & M.E.Sm.
 (G.W.Beaton) Spooner
 (G.W.Beaton) Trappe & G.W.Beaton
+(G.W.Beaton) Trappe, Castellano & Amar.
 (G.W.Beaton) W.Y.Zhuang
 (G.W.Beaton, Pegler & T.W.K.Young) Bougher & Castellano
 (G.W.Beaton, Pegler & T.W.K.Young) Bougher & T.Lebel
 (G.W.Beaton, Pegler & T.W.K.Young) Gasparini
 (G.W.Beaton, Pegler & T.W.K.Young) Justo
+(G.W.Beaton, Pegler & T.W.K.Young) Kuhar, Nouhra & M.E.Sm.
+(G.W.Beaton, Pegler & T.W.K.Young) P.M.Kirk
 (G.W.Beaton, Pegler & T.W.K.Young) Peintner & M.M.Moser
+(G.W.Beaton, Pegler & T.W.K.Young) T.Lebel
 (G.W.Beaton, Pegler & T.W.K.Young) T.Lebel & Castellano
 (G.W.Carr) D.L.Jones & M.A.Clem.
 (G.W.Carr) Hopper & A.P.Br.
 (G.W.Carr) Jeanes
 (G.W.Carr) Szlach.
 (G.W.Martin ex G.W.Martin) K.Wells
-(G.Winter & Plowr.) Syd.
+(G.Winter) Beenken
 (G.Winter) Cummins & Y.Hirats.
 (G.Winter) Hansf.
 (G.Winter) Honey
 (G.Winter) J.Walker
 (G.Winter) Kuntze
 (G.Winter) M.Scholler & Aime
 (G.Winter) Neerg.
 (G.Winter) Niessl
 (G.Winter) Rehm
 (G.Winter) S.Hughes
 (G.Winter) Vánky
 (G.Zeller) Nordst.
+(Gadgil & M.A.Dick) Crous
 (Gaertn.) Baill.
 (Gaertn.) Benth.
 (Gaertn.) Britten
 (Gaertn.) Cav.
 (Gaertn.) Craven
 (Gaertn.) DC.
 (Gaertn.) Domin
@@ -7782,14 +7937,15 @@
 (Gaertn.) Joy Thomps.
 (Gaertn.) K.D.Hill & L.A.S.Johnson
 (Gaertn.) K.Schum.
 (Gaertn.) Kitam.
 (Gaertn.) Knight
 (Gaertn.) Kuntze
 (Gaertn.) Merr.
+(Gaertn.) Peter G.Wilson
 (Gaertn.) Pfeiff.
 (Gaertn.) R.Knuth
 (Gaertn.) Roxb.
 (Gaertn.) Schauer
 (Gaertn.) Sm.
 (Gaertn.) Sol. ex A.Rich.
 (Gaertn.) Vent.
@@ -7825,14 +7981,15 @@
 (Garov.) Boise & D.Hawksw.
 (Garsault) Muschl. & Thell.
 (Gasp. ex Ten.) N.E.Br.
 (Gasp.) Benth.
 (Gasp.) Corner
 (Gasp.) Mildbr. & Burret
 (Gasp.) Miq.
+(Gasparini) Niskanen & Liimat.
 (Gatty) Batters
 (Gatty) Levring
 (Gauba) Paul G.Wilson
 (Gauba) S.Fuentes & Borsch
 (Gaudich. ex DC.) Randell
 (Gaudich.) A.R.Field & Bostock
 (Gaudich.) Alston
@@ -7853,15 +8010,14 @@
 (Gaudich.) Desv.
 (Gaudich.) Dittrich
 (Gaudich.) Endl.
 (Gaudich.) Exell
 (Gaudich.) F.M.Bailey
 (Gaudich.) F.Muell.
 (Gaudich.) F.Muell. ex Benth.
-(Gaudich.) F.Muell. x Ptilotus xerophilus T.Hammer & R.W.Davis
 (Gaudich.) Fosberg & Sachet
 (Gaudich.) Fryxell
 (Gaudich.) Gaudich.
 (Gaudich.) Gaudich. ex Steud.
 (Gaudich.) H.P.Linder
 (Gaudich.) H.Pfeiff.
 (Gaudich.) H.Rob. & Skvarla
@@ -7903,31 +8059,31 @@
 (Gay) Lokhorst
 (Gay) Reiche
 (Geerinck) Hopper
 (Geh. & Hampe) Broth. ex Dixon
 (Geh. & Hampe) M.Fleisch.
 (Geh.) Broth.
 (Geh.) Dixon
+(Geh.) Ignatov & Huttunen
 (Geh.) M.Fleisch.
 (Geh.) Mitt.
 (Geh.) Paris
 (Geh.) Watts & Whitel.
 (Gehrm.) Jabl.
 (Geiseler) Airy Shaw
 (Geiseler) Baill.
 (Geiseler) Kuntze
 (Geiseler) Müll.Arg.
 (Geiseler) Pax
 (Geitler) L.Hoffm.
-(Genev.) Roze & Richon
-(Gerd. & T.H.Nicolson) C.Walker & A.Schüssler
-(Gerd. & T.H.Nicolson) C.Walker & F.E.Sanders
-(Gerd. & T.H.Nicolson) Trappe & Gerd.
-(Gerlach & L.Nilsson) Chaverri & C.Salgado
-(Gerlach & L.Nilsson) Samuels & Mantiri
+(Genev.) Richon & Roze
+(Gerd. & Trappe) Oehl, G.A.Silva & Sieverd.
+(Gerd. & Trappe) R.T.Almeida & N.C.Schenck
+(Gerlach & L.Nilsson) Mantiri & Samuels
+(Gerlach & L.Nilsson) P.Chaverri & C.G.Salgado
 (Gerneck) Herndon
 (Gerr.-Corn. & J.A.Simpson) H.H.Ho & S.C.Jong
 (Gilg) Airy Shaw
 (Gilg) B.G.Briggs & L.A.S.Johnson
 (Gilg) Gilg-Ben.
 (Gilg) L.A.S.Johnson & B.G.Briggs
 (Gilib.) Asch.
@@ -7952,23 +8108,27 @@
 (Giseke) Mart.
 (Godey) Corner
 (Godey) R.H.Petersen
 (Godr.) Arriaga & Barkworth
 (Godr.) Barkworth
 (Godr.) Peñail.
 (Godr.) Thell.
+(Goh & K.D.Hyde) D.A.C.Almeida & Gusmão
+(Goh & K.D.Hyde) Réblová
+(Goh, W.H.Ho, K.D.Hyde & K.M.Tsui) Kaz.Tanaka & K.Hiray.
 (Goldblatt) Goldblatt
 (Goldring) Rehder
 (Gomes) Hayne
 (Gomes) Radlk.
 (Gomont) Anagn. & Komárek
 (Gomont) F.E.Drouet
 (Gomont) L.Hoffm.
 (Gomont) Siegesmund, J.R.Johans. & Friedl
 (Gomont) Turicchia, S.Ventura, Komárk.-Legn.& Komárek
+(Gonz.Frag. & Cif.) M.B.Ellis
 (Gooden. & Woodw.) F.Schmitz
 (Gooden. & Woodw.) Grev.
 (Gooden. & Woodw.) Kütz.
 (Goor) M.-E.Meffert
 (Goor) P.C.Silva
 (Gooss.) Rensb.
 (Gordon) Bartel
@@ -8002,33 +8162,34 @@
 (Gottsche) Schiffn.
 (Gottsche) Steph.
 (Gottsche) Steph. ex Schiffn.
 (Gottsche) Trevis.
 (Gottsche, Lindenb. & Nees) A.Evans
 (Gottsche, Lindenb. & Nees) Carrington & Pearson
 (Gottsche, Lindenb. & Nees) J.J.Engel
-(Gottsche, Lindenb. & Nees) Pócs
 (Gottsche, Lindenb. & Nees) R.M.Schust.
 (Gottsche, Lindenb. & Nees) R.M.Schust. & Kachroo
 (Gottsche, Lindenb. & Nees) Steph.
 (Gouan) Breistr.
 (Gouan) F.M.Bailey
 (Gouan) Rchb.
 (Gouan) Schinz & Thell.
+(Gouan) Vollm.
 (Gourret) A.R.Loebl. & L.A.Loebl.
 (Gourret) Cleve
 (Gourret) F.Gómez
+(Gourret) F.Gómez ex Hallegr. & Huisman
 (Gourret) F.Gómez, D.Moreira & López-García
 (Gourret) F.Schütt
 (Gourret) G.I.Gail
 (Gourret) G.Karst.
 (Gourret) Hallegr. & Huisman
 (Gourret) Huisman
 (Gourret) J.Schiller
-(Gourret) Jörg.
+(Gourret) Jørg.
 (Gourret) Kof.
 (Gourret) Kof. & Swezy
 (Gourret) Lemmerm.
 (Gourret) Pavill.
 (Gourret) Schröd.
 (Gourret) Vanhöffen
 (Govindu & Thirum.) U.Braun
@@ -8053,15 +8214,14 @@
 (Graham) Rodway
 (Graham) Siebert & Voss
 (Graham) Voss
 (Graham) Walp.
 (Graham) Wight & Arn.
 (Gran & Braarud) Balech
 (Gran) Balech
-(Gran) F.Gómez
 (Gran) J.Schiller
 (Gran) Lillick
 (Gran) Ostenf. & E.J.Schmidt
 (Gran) P.C.Silva
 (Gratel. ex Bory) Hauck
 (Gratel. ex Bory) J.Agardh
 (Gratel.) J.Agardh
@@ -8112,14 +8272,15 @@
 (Grev.) Kuntze
 (Grev.) Kylin
 (Grev.) Kütz.
 (Grev.) L.Junell
 (Grev.) Lange-Bert.
 (Grev.) Lindenb.
 (Grev.) Massee
+(Grev.) Menegh.
 (Grev.) Mont.
 (Grev.) Nägeli ex Kütz.
 (Grev.) P.A.Sims
 (Grev.) Pant.
 (Grev.) Parris
 (Grev.) R.Y.Zheng & G.Q.Chen
 (Grev.) Ralfs
@@ -8134,27 +8295,28 @@
 (Greves) Craven
 (Grgur.) D.Stubbe
 (Grgur.) Gasparini
 (Grgur.) J.A.Simpson & Grgur.
 (Grgur.) Peintner & M.M.Moser
 (Grgur.) R.H.Petersen
 (Grgur.) T.Lebel
+(Grgur.) Verbeken
 (Griff.) A.Jaeger
 (Griff.) A.Schimp.
 (Griff.) Ding Hou
-(Griff.) Ding Hou x Ceriops tagal (Perr.) C.B.Rob.
 (Griff.) F.Muell.
 (Griff.) Gangulee
 (Griff.) Griff.
 (Griff.) Kuntze
 (Griff.) Margad. & Nork.
 (Griff.) Rchb.f.
 (Griff.) V.Naray. ex Bor
 (Griffiths) L.D.Benson
 (Griffiths) L.D.Benson & Walk.
+(Griffiths) McTaggart & R.G.Shivas
 (Griffiths) S.I.Ahmed & Cain
 (Griffiths) Valldos. & Guarro
 (Griffiths) Vánky
 (Griffon & Maubl.) U.Braun & S.Takam.
 (Griseb.) Bitter & Lillo
 (Griseb.) D.A.Sutton
 (Griseb.) Glenny
@@ -8176,14 +8338,16 @@
 (Grolle) Pócs
 (Grolle) R.M.Schust.
 (Grose & Marink.) Kurtzman & Robnett
 (Grossh.) Grossh.
 (Grove) Ingold
 (Grove) W.Gams
 (Gruith.) Kütz.
+(Grunow ex A.W.F.Schmidt) Bailey
+(Grunow ex A.W.F.Schmidt) Cleve
 (Grunow ex Cleve) D.G.Mann
 (Grunow ex Cleve) F.Meister
 (Grunow ex Cleve) Hasle
 (Grunow ex E.Post) R.J.King & Puttock
 (Grunow ex G.Murray & Boodle) Papenf.
 (Grunow) A.Cleve
 (Grunow) A.Mann
@@ -8195,15 +8359,14 @@
 (Grunow) Compére
 (Grunow) Czarn.
 (Grunow) Czarnecki
 (Grunow) D.G.Mann
 (Grunow) D.M.Williams & Round
 (Grunow) De Toni
 (Grunow) E.J.Cox
-(Grunow) E.Jörg.
 (Grunow) E.Reichardt & Lange-Bert.
 (Grunow) F.Meister
 (Grunow) F.Schmitz
 (Grunow) F.Studnička
 (Grunow) Freng.
 (Grunow) Fryxell & Hasle
 (Grunow) Fryxell, Simonsen & Hasle
@@ -8217,20 +8380,22 @@
 (Grunow) Hasle
 (Grunow) Hasle & Fryxell
 (Grunow) Heiden
 (Grunow) Hendey
 (Grunow) Hust.
 (Grunow) J.L.Moreno
 (Grunow) Jurilj
+(Grunow) Jørg.
 (Grunow) K.Osada & K.Kobay.
 (Grunow) K.Stachura-Suchoples & D.M.Williams
 (Grunow) Krammer
 (Grunow) Krammer & Lange-Bert.
 (Grunow) Kuntze
 (Grunow) Kylin
+(Grunow) Laing
 (Grunow) Lange-Bert.
 (Grunow) Lange-Bert. ex Lange-Bert. & Rumrich
 (Grunow) Lemmerm.
 (Grunow) M.J.Wynne
 (Grunow) Mereschk.
 (Grunow) O.Müll.
 (Grunow) Okuno
@@ -8257,14 +8422,15 @@
 (Grunow) Turner
 (Grunow) Van Heurck
 (Grunow) W.R.Taylor
 (Grunow) Weber Bosse
 (Grunow) West & G.S.West
 (Grunow) Wille
 (Grunow) Witkowski, Lange-Bert. & Metzeltin
+(Gruyter) Qian Chen & L.Cai
 (Grönblad & Scott) Teiling
 (Grönblad) Croasdale
 (Grönblad) Kurt Först.
 (Grönblad) Teiling
 (Grönblad) Willi Krieg.
 (Grönblad) Willi Krieg. & Gerloff
 (Grüning) Airy Shaw
@@ -8275,15 +8441,14 @@
 (Guilf.) Cheel
 (Guill.) Engl.
 (Guill.) F.A.Barkley
 (Guillaumin) Barlow
 (Guillaumin) C.S.P.Foster & B.J.Conn
 (Guillaumin) Craven & J.W.Dawson
 (Guillaumin) D.L.Jones & M.A.Clem.
-(Guillaumin) J.W.Dawson
 (Guillaumin) L.A.S.Johnson & B.G.Briggs
 (Guillaumin) N.Snow & Guymer
 (Guillaumin) P.H.Weston & A.R.Mast
 (Guillaumin) Sleumer
 (Guillaumin) Steenis & Leenh.
 (Guiry & Womersley) Santel. & Hommers.
 (Gunn ex Hook.f.) Benth.
@@ -8312,21 +8477,20 @@
 (Gutw.) Teiling
 (Gutw.) West & G.S.West
 (Gutw.) Willi Krieg.
 (Guymer) C.F.Wilkins & Whitlock
 (Guég.) Saito
 (Gyeln.) A.Crespo, Ferencova & Divakar
 (Gyeln.) D.J.Galloway
-(Gyeln.) Elix
 (Gyeln.) Elix & Kantvilas
-(Gyeln.) Essl.
 (Gyeln.) Gyeln.
 (Gyeln.) Hale
 (Gyeln.) Inumaru
 (Gyeln.) Vitik.
+(Gérôme & Labroy) Byng & Christenh.
 (Gürke) B.Thomas
 (Güssow & W.R.Foster) B.Sutton
 (H.A.Mill.) E.D.Cooper
 (H.B.Will.) Christenh. & Byng
 (H.B.Will.) J.H.Willis
 (H.B.Will.) Paul G.Wilson
 (H.B.Will.) Pedley
@@ -8340,23 +8504,30 @@
 (H.Deane & Maiden) Maiden
 (H.E.Petersen) Buisman
 (H.E.Petersen) Dogma
 (H.Eichler ex R.M.Barker) Beier & Thulin
 (H.Eichler) Airy Shaw
 (H.Eichler) Beier & Thulin
 (H.Gross) T.M.Schust.
+(H.Groves & J.Groves) P.M.Peterson & Saarela
 (H.Ito) A.R.Sm.
 (H.Ito) Ching
 (H.Ito) H.Ito
 (H.J.Carter) Lemmerm.
 (H.J.Lam) Baehni
 (H.J.Lam) Moldenke
+(H.J.Swart & D.A.Griffiths) Crous
+(H.J.Swart & D.A.Griffiths) F.Liu, L.Cai & Crous
 (H.J.Swart & D.A.Griffiths) Nag Raj
+(H.J.Swart & M.A.Will.) Crous
+(H.J.Swart & M.A.Will.) P.A.Barber & Crous
 (H.J.Swart) Arx & E.Müll.
-(H.J.Swart) K.D.Hyde & C.A.Pearce
+(H.J.Swart) C.A.Pearce & K.D.Hyde
+(H.J.Swart) Crous
+(H.J.Swart) Crous & Summerell
 (H.J.Swart) Nag Raj
 (H.J.Swart) Sivan.
 (H.L.Sm.) Round & Crawford
 (H.L.Wendl. ex H.J.Veitch) Kuntze
 (H.L.Wendl.) DC.
 (H.L.Wendl.) Pedley
 (H.L.Wendl.) Voss
@@ -8381,14 +8552,15 @@
 (H.Perag.) Hasle
 (H.Perag.) Hernández-Becerril
 (H.Perag.) Pavill.
 (H.Richards) Feldm.-Maz.
 (H.S.Jacks. & Dearden) Donk
 (H.S.Jacks.) Donk
 (H.S.Jacks.) Hjortstam & Ryvarden
+(H.S.Jacks.) McTaggart & R.G.Shivas
 (H.S.Jacks.) Vánky
 (H.S.Nielsen & Conant) McGinnis
 (H.S.Randhawa & R.S.Sandhu) Apinis
 (H.S.Randhawa & R.S.Sandhu) Garg
 (H.S.Yates) Arx & E.Müll.
 (H.St.John) B.C.Stone
 (H.W.Anderson) Diddens & Lodder
@@ -8415,15 +8587,14 @@
 (H.Y.Yip) H.Y.Yip
 (Hack. & Arechav.) Parodi
 (Hack. ex Cheeseman) Domin
 (Hack. ex Cheeseman) Edgar & Connor
 (Hack. ex Cheeseman) Zotov
 (Hack. ex Steud.) Hack.
 (Hack.) A.Camus
-(Hack.) A.Camus x Cymbopogon queenslandicus S.T.Blake
 (Hack.) Bor
 (Hack.) C.E.Hubb.
 (Hack.) Dandy
 (Hack.) Domin
 (Hack.) Fernald
 (Hack.) Henrard
 (Hack.) Hitchc.
@@ -8442,14 +8613,15 @@
 (Haegi) Haegi
 (Haegi) P.S.Short
 (Haegi) Paul G.Wilson
 (Hafellner & R.W.Rogers) Kantvilas, Papong & Lumbsch
 (Hafellner) Hafellner & R.W.Rogers
 (Hafellner) R.W.Rogers & Hafellner
 (Hagelst.) Giffen
+(Hagem) Urquhart & Douch
 (Hajsig) S.A.Mey. & Yarrow
 (Hale & Kurok.) Elix
 (Hale & Kurok.) Hale
 (Hale) A.Crespo, Divakar & Elix
 (Hale) A.Crespo, Ferencova & Divakar
 (Hale) Elix
 (Hale) Elix & G.N.Stevens
@@ -8470,26 +8642,28 @@
 (Hallier f.) Garay
 (Hallier f.) Ooststr.
 (Hallier f.) Schlittler
 (Hallier f.) Szlach.
 (Ham.) Roseng., B.R.Arrill. & Izag.
 (Hampe & Geh.) Paris
 (Hampe & Müll.Hal.) Broth.
+(Hampe & Müll.Hal.) Pursell
 (Hampe) A.Jaeger
 (Hampe) A.Jaeger ex Paris
 (Hampe) B.C.Tan, W.B.Schofield & H.P.Ramsay
 (Hampe) B.H.Allen
 (Hampe) Broth.
 (Hampe) Broth. & Watts
 (Hampe) Broth. ex Paris
 (Hampe) Broth. ex Watts
 (Hampe) Dixon
 (Hampe) Dozy & Molk.
 (Hampe) During
 (Hampe) E.Lawton
+(Hampe) Fedosov, M.Stech & Ignatov
 (Hampe) Hampe
 (Hampe) Hedenäs
 (Hampe) I.G.Stone
 (Hampe) J.H.Willis
 (Hampe) J.H.Willis ex Seppelt
 (Hampe) J.R.Spence
 (Hampe) J.R.Spence & H.P.Ramsay
@@ -8508,26 +8682,29 @@
 (Hampe) R.M.Schust.
 (Hampe) Renauld ex Paris
 (Hampe) Steph.
 (Hampe) Warnst.
 (Hampe) Watts & Whitel.
 (Hampe) Wilson
 (Hance) Rehder
+(Hansf.) C.A.Pearce & K.D.Hyde
+(Hansf.) Crous
 (Hansf.) Dennis
 (Hansf.) Dingley
 (Hansf.) E.G.Simmons
 (Hansf.) H.J.Swart
 (Hansf.) H.J.Swart & J.Walker
 (Hansf.) Hansf.
+(Hansf.) J.A.Simpson & Grgur.
 (Hansf.) J.L.Crane & A.G.Jones
 (Hansf.) J.Walker
 (Hansf.) J.Walker & H.J.Swart
-(Hansf.) K.D.Hyde & C.A.Pearce
 (Hansf.) M.B.Ellis
 (Hansf.) Nag Raj
+(Hansf.) P.R.Johnst.
 (Hansf.) Sivan. & B.Sutton
 (Hansf.) Spooner
 (Hansf.) Tubaki & Nishih.
 (Hansg.) Bohlin
 (Hansg.) Hansg.
 (Hansg.) Kovacik
 (Hansg.) P.C.Silva
@@ -8536,22 +8713,25 @@
 (Hantzsch) Cleve
 (Hantzsch) Grunow
 (Hantzsch) Heib.
 (Hantzsch) Protíc
 (Hantzsch) Reinsch
 (Hantzsch) Teiling
 (Hantzsch) West & G.S.West
+(Har. & Pat.) Mains
+(Har. & Pat.) Vánky
 (Har.) Draisma, Prud'homme & H.Kawai
 (Har.) H.Y.Yoon
+(Har.) Heydr.
 (Har.) M.L.Mend.
 (Hara) D.Hawksw.
 (Hara) Deighton
 (Hargraves & Guillard) Hasle, Stosch & Syvertsen
-(Harkn.) C.W.Dodge & Zeller
 (Harkn.) Singer & A.H.Sm.
+(Harkn.) Zeller & C.W.Dodge
 (Harm.) Frisch
 (Harm.) Hale
 (Harm.) Lettau
 (Harms) Lowry & G.M.Plunkett
 (Harms) Pedley
 (Harms) Philipson
 (Harms) Verdc.
@@ -8569,15 +8749,14 @@
 (Harv. & Bailey) W.R.Taylor
 (Harv. & Grev.) De Toni
 (Harv. & Grev.) Harv.
 (Harv. & Grev.) Papenf.
 (Harv. & Sond.) Sherff
 (Harv. ex Berk. & Desm.) Thüm.
 (Harv. ex E.P.Wright) J.Agardh
-(Harv. ex Hook.) J.R.Spence & H.P.Ramsay
 (Harv. ex J.Agardh) D.L.Dixit
 (Harv. ex J.Agardh) Falkenb.
 (Harv. ex J.Agardh) G.Furnari
 (Harv. ex J.Agardh) Hyung S.Kim & I.K.Lee
 (Harv. ex J.Agardh) Kuntze
 (Harv. ex J.Agardh) Kylin
 (Harv. ex J.Agardh) M.J.Parsons
@@ -8640,15 +8819,14 @@
 (Harv.) Grunow ex Picc.
 (Harv.) H.A.Mill., H.Whittier & B.Whittier
 (Harv.) H.G.Choi, G.T.Kraft & G.W.Saunders
 (Harv.) H.Rob.
 (Harv.) H.W.Johans. & Womersley
 (Harv.) H.Y.Yoon
 (Harv.) Hamel
-(Harv.) Hampe
 (Harv.) Harv.
 (Harv.) Harv.-Gibs.
 (Harv.) Heydr.
 (Harv.) Hollenb. & I.A.Abbott
 (Harv.) Hommers.
 (Harv.) Hook.f. & Harv.
 (Harv.) Hook.f. & Harv. ex Harv.
@@ -8777,18 +8955,20 @@
 (Hayata) Merr.
 (Hayata) Rauschert
 (Hayata) Rehder
 (Hayata) Schltr.
 (Hayne) Banfi & Galasso
 (Hazen) Collins
 (Hedgc.) C.Moreau
+(Hedgc.) Z.W.de Beer, T.A.Duong & M.J.Wingf.
 (Hedw.) A.Jaeger
 (Hedw.) Ach.
 (Hedw.) Arn.
 (Hedw.) Bach.Pyl.
+(Hedw.) Bonfim Santos & Fedosov
 (Hedw.) Brid.
 (Hedw.) Brid. ex Mitt.
 (Hedw.) Broth.
 (Hedw.) Bruch
 (Hedw.) Bruch & Schimp.
 (Hedw.) C.E.O.Jensen
 (Hedw.) Corda
@@ -8805,17 +8985,18 @@
 (Hedw.) Hampe
 (Hedw.) Hilf. ex H.A.Crum & L.E.Anderson
 (Hedw.) Hoffm.
 (Hedw.) Hook. & Grev.
 (Hedw.) Hook. & Taylor
 (Hedw.) Hook.f.
 (Hedw.) Hook.f. & Wilson
+(Hedw.) Ignatov & Huttunen
+(Hedw.) Ignatov & Ignatova
 (Hedw.) J.R.Spence
 (Hedw.) J.R.Spence & H.P.Ramsay
-(Hedw.) J.R.Spence & H.P.Ramsay ex D.T.Holyoak & N.Pedersen
 (Hedw.) Jenn.
 (Hedw.) Kindb.
 (Hedw.) Lam. & DC.
 (Hedw.) Limpr.
 (Hedw.) Lindb.
 (Hedw.) Lindb. ex Mitt.
 (Hedw.) Loeske
@@ -8840,43 +9021,42 @@
 (Hedw.) Schwägr.
 (Hedw.) Sm.
 (Hedw.) Steere
 (Hedw.) Turner
 (Hedw.) Warnst.
 (Hedw.) Watts & Whitel.
 (Hedw.) Wilson
+(Hedw.) Z.Iwats.
 (Hegetschw.) Vězda
 (Heiden & Kolbe) Kolbe
 (Heiden) A.Cleve
 (Heiden) Simonsen
 (Heimerl) Croasdale
 (Heimerl) Kimbr.
 (Heimerl) Schmidle
 (Heimerl) Teiling
 (Heimerl) Willi Krieg. & Gerloff
 (Heinem. & Goos.) Corner
-(Heinem. & Gooss.-Font.) Bertault & Malençon
+(Heinem. & Gooss.-Font.) Malençon & Bertault
 (Heinem. & Gooss.-Font.) Singer
 (Heist. ex Fabr.) A.Gray
 (Heldr. & Sartori ex Boiss.) I.Richardson
 (Hemsl.) A.Gray
 (Hemsl.) Adamson & Sprague
 (Hemsl.) Airy Shaw
 (Hemsl.) C.A.Gardner
 (Hemsl.) Giesen
 (Hemsl.) Mabb. & Holzmeyer
 (Hemsl.) Paul G.Wilson
 (Hemsl.) Renvoize
 (Hemsl.) Stapf
+(Hend. ex R.Hogg) Mabb.
 (Hendey) Hasle
 (Henfr.) Burtt Davy
 (Henfr.) Chopinet
-(Henn. & Bres. ex Sacc.) G.Cunn.
-(Henn. & Bres. ex Sacc.) Ryvarden
-(Henn. & Bres. ex Sacc.) Steyaert
 (Henn. ex McAlpine) Buriticá & J.F.Hennen
 (Henn.) Alcorn
 (Henn.) C.Walker & A.Schüssler
 (Henn.) Corner
 (Henn.) D.A.Reid
 (Henn.) Dennis
 (Henn.) E.J.Durand
@@ -8887,31 +9067,35 @@
 (Henn.) Höhn. & Litsch.
 (Henn.) J.A.Mey.
 (Henn.) J.H.Mill.
 (Henn.) K.D.Hyde
 (Henn.) L.Ling
 (Henn.) Langdon & Full.
 (Henn.) Lloyd
+(Henn.) Læssøe & Spooner
 (Henn.) M.Piepenbr.
+(Henn.) McAlpine
+(Henn.) McTaggart & R.G.Shivas
 (Henn.) Nag Raj
 (Henn.) Nannf.
+(Henn.) Petr.
 (Henn.) Sacc.
 (Henn.) Sacc. & D.Sacc.
+(Henn.) Sacc. & P.Syd.
 (Henn.) Singer
 (Henn.) Spooner
-(Henn.) Spooner & Læssøe
 (Henn.) Syd. & P.Syd.
-(Henn.) Syd. & Sacc.
 (Henn.) Theiss.
 (Henn.) Theiss. & Syd.
 (Henn.) Trappe & Gerd.
 (Henn.) Vánky
+(Henn.) Y.P.Tan & R.G.Shivas
 (Henn.) Zundel
 (Henneberg) Lodder & Kreger-van Rij
-(Hennebert & B.G.Desai) de Hoog & E.Guého
+(Hennebert & B.G.Desai) E.Guého & de Hoog
 (Henrard) H.Eichler
 (Henrard) Lazarides
 (Henrard) Mabb.
 (Henrard) S.T.Blake
 (Henrard) S.T.Blake ex J.M.Black
 (Henriques) R.Sant.
 (Hensen) Gran
@@ -8948,14 +9132,15 @@
 (Hering & G.Martens) J.Agardh
 (Hering) De Toni
 (Hering) Delf & Michell
 (Hering) G.De Toni
 (Hering) J.Agardh
 (Hering) Papenf.
 (Hering) Tyson
+(Herink) R.A.Koch & Aime
 (Herre) Herre
 (Hertel) Hertel
 (Herter ex Nessel) A.R.Field & Bostock
 (Herter) A.R.Field & Bostock
 (Herter) Allan
 (Herter) Herter ex Nessel
 (Herter) Holub
@@ -8983,16 +9168,16 @@
 (Heydr.) Heydr.
 (Heydr.) M.L.Mend. & Cabioch
 (Heydr.) M.S.Balakr. & Kinkar
 (Heydr.) P.C.Silva
 (Heydr.) Penrose & Woelk.
 (Heydr.) Setch. & L.R.Mason
 (Heydr.) Verheij
+(Hickie) Bukht.
 (Hickie) Cleve
-(Hickie) Lange-Bert.
 (Hiern) F.White
 (Hieron. ex Brause) Nakai
 (Hieron.) Anagn. & Komárek
 (Hieron.) Benth.
 (Hieron.) Schmidle
 (Hildebrand) Wille
 (Hildenbrand) R.H.Thompson & D.E.Wujek
@@ -9005,15 +9190,15 @@
 (Hils. & Bojer ex Tul.) A.Berger
 (Hilse) Cleve
 (Hilse) D.G.Mann
 (Hilse) Grunow
 (Hilse) Lange-Bert.
 (Hilse) West & G.S.West
 (Hirano) Thomasson
-(Hirasaka) G.I.Hansen & Moestrup
+(Hirasaka) Gert Hansen & Moestrup
 (Hislop & A.J.G.Wilson) Hislop, Crayn & Puente-Lel.
 (Hislop) Hislop, Crayn & Puente-Lel.
 (Hitchc.) Honda
 (Hitchc.) Thell. ex B.de Lesd.
 (Hnatiuk) Craven & R.D.Edwards
 (Hochr. ex Britten) Fosberg
 (Hochr. ex Britten) Nimbalkar, Nandikar & Sardesai
@@ -9085,27 +9270,31 @@
 (Hoffm.) Räsänen
 (Hoffm.) Schaer.
 (Hoffm.) Th.Fr.
 (Hoffm.) Vain.
 (Hoffm.) W.B.Cooke
 (Hoffm.) Zahlbr.
 (Hoffmanns. & Link) Fritsch
+(Hol.-Jech. & Mercado) Nawawi & Kuthub.
 (Hollenb.) I.A.Abbott
 (Hollenb.) M.S.Kim & I.K.Lee
 (Holmsk.) Eckblad
 (Holmsk.) Fr.
 (Holmsk.) J.Schröt.
+(Holmsk.) Kepler, B.Shrestha & Spatafora
 (Holmsk.) Korf & J.K.Rogers
 (Holmsk.) Kük.
 (Holmsk.) Quél.
 (Holttum) A.R.Field
+(Holttum) A.R.Field & Z.Bloesch
 (Holttum) Christenh.
 (Holttum) D.L.Jones
 (Holttum) Lehnert
 (Holttum) R.M.Tryon
+(Holttum) S.E.Fawc. & A.R.Sm.
 (Holttum) T.E.Almeida & A.R.Field
 (Holub) B.Øllg.
 (Hombr. & Jacquinot ex Hook.f.) A.Gray
 (Hombr. & Jacquinot ex Hook.f.) G.M.Plunkett & A.N.Nicolas
 (Hombr. & Jacquinot) Hook.f.
 (Hombr. ex Decne.) S.Venter
 (Hombr.) Hook.f.
@@ -9127,30 +9316,29 @@
 (Hook. & Grev.) Alderw.
 (Hook. & Grev.) Bonap.
 (Hook. & Grev.) Brid.
 (Hook. & Grev.) C.Presl
 (Hook. & Grev.) Copel.
 (Hook. & Grev.) F.Muell.
 (Hook. & Grev.) H.Rob.
+(Hook. & Grev.) Jan Kučera
 (Hook. & Grev.) M.Fleisch.
 (Hook. & Grev.) Mitt.
 (Hook. & Grev.) R.H.Zander
 (Hook. & Grev.) Salvo, Prada & T.E.Diaz
 (Hook. & Grev.) Schwägr.
 (Hook. & Grev.) T.Moore
 (Hook. & Grev.) Tindale
 (Hook. & Grev.) Vitt
 (Hook. & Grev.) Wilson
 (Hook. & Harv.) Harv. ex Kütz.
 (Hook. & Taylor) K.Feldberg, Vana, Hentschel & Heinrichs
-(Hook. & Taylor) Zahlbr.
 (Hook. & Wilson) A.Jaeger
 (Hook. & Wilson) Broth.
 (Hook. & Wilson) Fife & Seppelt
-(Hook. & Wilson) J.R.Spence & H.P.Ramsay
 (Hook. & Wilson) Mitt.
 (Hook. & Wilson) Müll.Hal.
 (Hook. & Wilson) Paris
 (Hook. & Wilson) Wilson
 (Hook. ex F.Muell.) Domin
 (Hook. ex F.Muell.) R.M.Tryon
 (Hook. ex Graham) D.Don
@@ -9191,16 +9379,16 @@
 (Hook.) Christenh.
 (Hook.) Christenh. & Byng
 (Hook.) Chrtek & Slavikova
 (Hook.) Cooke
 (Hook.) Copel.
 (Hook.) Corner
 (Hook.) Crisp
+(Hook.) Crisp & L.G.Cook
 (Hook.) Crisp & P.H.Weston
-(Hook.) Curtis
 (Hook.) D.Dietr.
 (Hook.) Diels
 (Hook.) Dixon
 (Hook.) Domin
 (Hook.) Druce
 (Hook.) Dumort.
 (Hook.) Dumort. ex Trevis.
@@ -9222,33 +9410,29 @@
 (Hook.) Gottsche, Lindenb. & Nees
 (Hook.) Gray
 (Hook.) Grolle
 (Hook.) H.Walter
 (Hook.) H.Wendl.
 (Hook.) Hampe
 (Hook.) Heenan & Smissen
+(Hook.) Hemsl.
 (Hook.) Holttum
 (Hook.) Hook.
 (Hook.) Hook. & Grev.
 (Hook.) Hook. ex Gottsche, Lindenb. & Nees
 (Hook.) Hook.f.
 (Hook.) Hook.f. & Wilson
 (Hook.) Hook.f. ex Benth.
 (Hook.) J.F.Macbr.
 (Hook.) J.P.Roux
 (Hook.) J.R.Spence
 (Hook.) J.R.Spence & H.P.Ramsay
 (Hook.) J.Sm.
 (Hook.) Jord.
 (Hook.) K.D.Hill & L.A.S.Johnson
-(Hook.) K.D.Hill & L.A.S.Johnson subsp. citriodora x Corymbia watsoniana subsp. capillata (Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson
-(Hook.) K.D.Hill & L.A.S.Johnson x Corymbia leichhardtii (F.M.Bailey) K.D.Hill & L.A.S.Johnson
-(Hook.) K.D.Hill & L.A.S.Johnson x Corymbia peltata (Benth.) K.D.Hill & L.A.S.Johnson
-(Hook.) K.D.Hill & L.A.S.Johnson x Corymbia torelliana (F.Muell.) K.D.Hill & L.A.S.Johnson
-(Hook.) K.D.Hill & L.A.S.Johnson x Corymbia watsoniana subsp. capillata (Brooker & A.R.Bean) K.D.Hill & L.A.S.Johnson
 (Hook.) K.Iwats.
 (Hook.) K.Koch
 (Hook.) Klotzsch
 (Hook.) Kuhn
 (Hook.) Kuntze
 (Hook.) L.A.S.Johnson
 (Hook.) L.B.Moore
@@ -9412,15 +9596,14 @@
 (Hook.f. & Taylor) L.Söderstr. & A.Hagborg
 (Hook.f. & Taylor) Lehm.
 (Hook.f. & Taylor) Leight.
 (Hook.f. & Taylor) Lindb.
 (Hook.f. & Taylor) Mitt.
 (Hook.f. & Taylor) Mitt. ex Bastow
 (Hook.f. & Taylor) Mitt. ex Steph.
-(Hook.f. & Taylor) Mont. & Bosch
 (Hook.f. & Taylor) Müll.Arg.
 (Hook.f. & Taylor) Nees
 (Hook.f. & Taylor) Nees ex Gottsche, Lindenb. & Nees
 (Hook.f. & Taylor) Nyl.
 (Hook.f. & Taylor) P.James
 (Hook.f. & Taylor) P.M.Jørg.
 (Hook.f. & Taylor) P.M.Jørg. & H.L.Andersen
@@ -9441,60 +9624,66 @@
 (Hook.f. & Taylor) Verd. ex G.A.M.Scott & J.A.Bradshaw
 (Hook.f. & Taylor) Yoshim.
 (Hook.f. & Taylor) Zahlbr.
 (Hook.f. & Taylor.) Cromb.
 (Hook.f. & Wilson) A.Jaeger
 (Hook.f. & Wilson) B.H.Allen
 (Hook.f. & Wilson) Beckett
-(Hook.f. & Wilson) Bosch & Sande Lac.
+(Hook.f. & Wilson) Bedn.-Ochyra & Ochyra
 (Hook.f. & Wilson) Braithw.
 (Hook.f. & Wilson) Broth.
 (Hook.f. & Wilson) Broth. & Watts
 (Hook.f. & Wilson) Broth. ex Paris
 (Hook.f. & Wilson) Cardot & Bryhn
 (Hook.f. & Wilson) Dixon
 (Hook.f. & Wilson) Dusén
 (Hook.f. & Wilson) Dusén ex Broth.
 (Hook.f. & Wilson) Enroth
 (Hook.f. & Wilson) Enroth & S.He
+(Hook.f. & Wilson) F.Lara, Garilleti & Goffinet
 (Hook.f. & Wilson) Fife
 (Hook.f. & Wilson) G.L.Sm.
 (Hook.f. & Wilson) H.A.Crum
 (Hook.f. & Wilson) Hampe
 (Hook.f. & Wilson) Hook.f.
 (Hook.f. & Wilson) Hook.f. & Wilson
+(Hook.f. & Wilson) Huttunen & Ignatov
 (Hook.f. & Wilson) I.G.Stone & G.A.M.Scott
+(Hook.f. & Wilson) Ignatov & Huttunen
 (Hook.f. & Wilson) J.R.Spence & H.P.Ramsay
 (Hook.f. & Wilson) Kindb.
 (Hook.f. & Wilson) Lindb.
 (Hook.f. & Wilson) Lindb. ex Paris
 (Hook.f. & Wilson) M.Fleisch.
 (Hook.f. & Wilson) M.Fleisch. ex Broth.
 (Hook.f. & Wilson) Matteri
 (Hook.f. & Wilson) Meijer
 (Hook.f. & Wilson) Mitt.
 (Hook.f. & Wilson) Müll.Hal.
 (Hook.f. & Wilson) Müll.Hal. & Broth.
+(Hook.f. & Wilson) N.E.Bell & Hyvönen
 (Hook.f. & Wilson) Nieuwl.
 (Hook.f. & Wilson) Nog.
 (Hook.f. & Wilson) Ochyra
 (Hook.f. & Wilson) Paris
 (Hook.f. & Wilson) Paris & Schimp.
+(Hook.f. & Wilson) Pursell
 (Hook.f. & Wilson) R.H.Zander
 (Hook.f. & Wilson) Reichardt
 (Hook.f. & Wilson) Reimers
+(Hook.f. & Wilson) S.Olsson, Enroth & D.Quandt
 (Hook.f. & Wilson) Sainsbury
 (Hook.f. & Wilson) Taylor
 (Hook.f. & Wilson) Thér.
 (Hook.f. & Wilson) Vitt
 (Hook.f. & Wilson) Vitt & Crosby
 (Hook.f. & Wilson) Watts & Whitel.
 (Hook.f. & Wilson) Wijk & Margad.
 (Hook.f. & Wilson) Wilson
-(Hook.f. & Wilson) Z.Iwats. H.P.Ramsay & Fife
+(Hook.f. & Wilson) Z. Iwats., H.P. Ramsay & Fife
 (Hook.f. ex A.Gray) Benth.
 (Hook.f. ex Benth.) A.W.Hill
 (Hook.f. ex Benth.) C.A.Gardner
 (Hook.f. ex Benth.) Dunlop
 (Hook.f. ex Boeckeler) Benl
 (Hook.f. ex Boeckeler) Kük.
 (Hook.f. ex Kirk) Kuntze
@@ -9649,15 +9838,15 @@
 (Hook.f.) Schauer
 (Hook.f.) Schindl.
 (Hook.f.) Schltr.
 (Hook.f.) Seem.
 (Hook.f.) Sherff
 (Hook.f.) Skeels
 (Hook.f.) Skottsb.
-(Hook.f.) Small ex Hanks & Small
+(Hook.f.) Small
 (Hook.f.) Soják
 (Hook.f.) Sond.
 (Hook.f.) Steud.
 (Hook.f.) Summerh.
 (Hook.f.) Szlach.
 (Hook.f.) Tiegh.
 (Hook.f.) Tirveng. & Sastre
@@ -9687,17 +9876,14 @@
 (Hornem.) F.Herm.
 (Hornem.) Fisch. & C.A.Mey.
 (Hornem.) Henrard
 (Hornem.) Hertel & A.J.Schwab
 (Hornem.) Link
 (Hornem.) Redouté
 (Hornem.) Spreng.
-(Hornsch. ex Müll.Hal.) Broth.
-(Hornsch. ex Müll.Hal.) Grout
-(Hornsch. ex Müll.Hal.) Mitt.
 (Hornsch.) A.Braun
 (Hornsch.) Broth.
 (Hornsch.) Cufod.
 (Hornsch.) Mitt.
 (Hornsch.) Paris
 (Hornsch.) Wijk & Margad.
 (Horta) McGinnis & Schell
@@ -9710,26 +9896,26 @@
 (Host) P.Beauv.
 (Host) Runemark
 (Host) Schrad.
 (Host) Trin.
 (Host) Á.Löve
 (Houlston) C.V.Morton
 (Houlston) Labiak, Sundue & R.C.Moran
+(Houlston) Watts
 (Houtt.) A.R.Simões & Staples
 (Houtt.) Decne.
 (Houtt.) H.Ohashi
 (Houtt.) Hedberg
 (Houtt.) Merr.
 (Houtt.) Merr. & F.P.Metcalf
 (Houtt.) Ronse Decr.
 (Houtt.) Stapf
 (Houtt.) Veldkamp
 (Howe) U.Braun & S.Takam.
 (Huber) Prance
-(Huds. : Fr.) P.Kumm.
 (Huds.) A.Gray
 (Huds.) A.Massal.
 (Huds.) Ach.
 (Huds.) Baumg.
 (Huds.) Bref.
 (Huds.) C.Agardh
 (Huds.) Coville
@@ -9785,38 +9971,40 @@
 (Hue) Lettau
 (Hue) Matzer, H.Mayrhofer & Scheid.
 (Hue) R.C.Harris
 (Hue) S.Y.Kondr., Kärnefelt, A.Thell, Elix, J.Kim, A.S.Kondr. & Hur
 (Hue) Sipman
 (Hue) Søchting & Øvstedal
 (Hue) Søchting, Frödén & Arup
-(Hue) Tomas.
 (Hue) Vain.
 (Hue) Zahlbr.
 (Hughes) B.K.Simon
 (Hughes) Lazarides
 (Hughes) Lazarides & R.D.Webster
 (Hughes) R.D.Webster
 (Hughes) S.W.L.Jacobs & J.Everett
 (Hughes) Vickery, S.W.L.Jacobs & J.Everett
 (Huijsman ex P.D.Orton) M.M.Moser
-(Hulburt) G.I.Hansen
+(Hulburt) Gert Hansen
 (Hulburt) Hallegr.
 (Hulburt) S.Y.Cho, J.S.Ki & M.S.Han
 (Hulburt, J.A.McLaughlin & Zahl) Sh.Murray, M.Salas & Hallegr.
 (Humb. & Bonpl. ex Schult.) Moq.
 (Humb. & Bonpl. ex Schult.) Small
 (Humb. & Bonpl. ex Willd.) Benth.
 (Humb. & Bonpl. ex Willd.) Bercht. & J.Presl
+(Humb. & Bonpl. ex Willd.) Britton & Rose
 (Humb. & Bonpl. ex Willd.) Britton & Rose ex Britton & Killip
 (Humb. & Bonpl. ex Willd.) Buchenau
 (Humb. & Bonpl. ex Willd.) Byng & Christenh.
+(Humb. & Bonpl. ex Willd.) C.E.Hughes & G.P.Lewis
 (Humb. & Bonpl. ex Willd.) DC.
 (Humb. & Bonpl. ex Willd.) H.S.Irwin & Barneby
 (Humb. & Bonpl. ex Willd.) Heine
+(Humb. & Bonpl. ex Willd.) Kunth
 (Humb. & Bonpl. ex Willd.) Kuntze
 (Humb. & Bonpl. ex Willd.) M.C.Johnst.
 (Humb. & Bonpl. ex Willd.) Poir.
 (Humb. & Bonpl. ex Willd.) Rothm.
 (Humb.) Donk
 (Humb.) Fürnr.
 (Humb.) Pers.
@@ -9831,20 +10019,20 @@
 (Hust.) E.J.F.Wood
 (Hust.) Freng.
 (Hust.) H.Kobayasi
 (Hust.) Hallegr.
 (Hust.) Hasle
 (Hust.) Hust.
 (Hust.) J.L.Moreno
+(Hust.) J.N.Navarro & Lobban
 (Hust.) J.W.G.Lund
 (Hust.) Krammer
 (Hust.) Lange-Bert.
 (Hust.) Lange-Bert. & Archibald
 (Hust.) Levkov
-(Hust.) Navarro & Lobban
 (Hust.) Reimer
 (Hust.) Sabbe, Witkowski & Vyverman
 (Hust.) Simonsen
 (Hust.) VanLand.
 (Hust.) Witkowski
 (Hust.) Yan Liu bis, Kociolek & Q.X.Wang
 (Hutch. & Dalziel) O.C.Schmidt
@@ -9865,14 +10053,15 @@
 (Höhn.) F.Stevens & Manter
 (Höhn.) Singer
 (Höhn.) Spooner
 (Höhn.) Theiss. & Syd.
 (Höhn.) W.Y.Zhuang
 (Höhnk) Cribb & J.W.Cribb
 (Höhnk) Kohlm.
+(Høil. & Watling) T.W.May & A.E.Wood
 (Hügel ex Benth.) Benth.
 (Hügel ex Benth.) Domin
 (Hügel ex Benth.) Greene
 (Hügel ex Benth.) Ostenf.
 (Hügel ex Benth.) Steud.
 (Hügel ex Endl.) Christenh. & Byng
 (Hügel ex Endl.) Domin
@@ -9880,34 +10069,38 @@
 (Hügel ex Endl.) F.Muell.
 (Hügel ex Endl.) Kuntze
 (Hügel) Baill.
 (Hügel) Domin
 (I.C.Nielsen) Barneby & J.W.Grimes
 (I.C.Nielsen) Maslin
 (I.C.Nielsen) Maslin, B.C.Ho, H.Sun & L.Bai
+(I.G.Stone & G.A.M.Scott) Hedd. & R.H.Zander
+(I.G.Stone) B.C.Tan, T.J.Kop. & D.H.Norris
 (I.G.Stone) B.C.Tan, Z.Iwats. & D.H.Norris
 (I.G.Stone) Brugg.-Nann.
 (I.G.Stone) I.G.Stone
 (I.G.Stone) J.E.Beever & I.G.Stone
+(I.G.Stone) Pursell
 (I.G.Stone) R.H.Zander
 (I.Hutton & P.S.Green) M.A.Jaram.
 (I.M.Johnst.) Craven
 (I.M.Johnst.) Frodin
 (I.M.Lamb) D.J.Galloway
 (I.M.Lamb) I.M.Lamb
 (I.M.Lamb) P.James
 (I.M.Lamb) Räsänen
 (I.M.Lamb) Wedin
 (I.M.Wilson) T.W.Johnson
 (I.P.Price & P.H.B.Talbot) Descals
 (I.R.Hall) R.N.Ames & R.W.Schneid.
+(I.R.Hall) Sieverd., G.A.Silva & Oehl
 (I.Telford & R.L.Barrett) R.W.Bouman
 (I.Telford) E.A.Br.
 (I.Thomps.) Schmidt-Leb.
-(Iljin) Soo
+(Iljin) Soó
 (Iltis) R.L.Barrett
 (Inoue & Fukuyo) Balech
 (Inoue & Fukuyo) F.Gómez & Artigas
 (Irmisch ex Asch.) Toml. & Posl.
 (Ising) A.J.Scott
 (Ising) Beier & Thulin
 (Ising) Chinnock
@@ -9941,14 +10134,15 @@
 (J.Agardh) D.P.Cheney & P.W.Gabrielson
 (J.Agardh) De Clerck & Coppejans
 (J.Agardh) De Toni
 (J.Agardh) Ducker
 (J.Agardh) E.J.Faye & Masuda
 (J.Agardh) E.M.Heine
 (J.Agardh) E.M.Woll.
+(J.Agardh) E.Post
 (J.Agardh) E.Y.Dawson
 (J.Agardh) Edyvane & Womersley
 (J.Agardh) Eubank
 (J.Agardh) F.Muell.
 (J.Agardh) F.Schmitz
 (J.Agardh) Falkenb.
 (J.Agardh) Feldm.-Maz.
@@ -10066,25 +10260,28 @@
 (J.Drumm.) Benth.
 (J.Drumm.) Chodat ex Anon.
 (J.Drumm.) Crisp
 (J.Drumm.) Orchard
 (J.E.Br.) F.Muell. ex Maiden
 (J.E.Br.) J.M.Black
 (J.E.Br.) Pedley
+(J.E.Chilton) P.F.Cannon
 (J.E.Gray) J.Agardh
 (J.E.Jacques) Crous & U.Braun
 (J.E.Lange) Bon
 (J.E.Lange) F.H.Møller & Jul.Schäff.
 (J.E.Lange) Imbach
 (J.E.Lange) Lamoure
 (J.E.Lange) M.M.Moser
 (J.E.Lange) Métrod
 (J.E.Lange) Singer
 (J.E.Sm. ex Ach.) Hale
 (J.E.Sm. ex Ach.) Müll.Arg.
+(J.E.Wright & J.R.Deschamps) B.K.Cui & Shun Liu
+(J.E.Wright & J.R.Deschamps) Rajchenb., Gorjón & Pildain
 (J.Ellis & Sol.) F.Schmitz
 (J.Ellis & Sol.) H.W.Johans.
 (J.Ellis & Sol.) Harv.
 (J.Ellis & Sol.) Huisman & Borow.
 (J.Ellis & Sol.) J.Agardh
 (J.Ellis & Sol.) J.V.Lamour.
 (J.Ellis & Sol.) Kuntze
@@ -10122,26 +10319,28 @@
 (J.F.Gmel.) Schinz & Thell.
 (J.F.Gmel.) Soják
 (J.F.Gmel.) T.Koyama
 (J.F.Gmel.) Torr. & A.Gray
 (J.F.Gmel.) Veldkamp
 (J.F.Gmel.) W.R.B.Oliv.
 (J.F.H.Beyma) E.Weber, Görke & Begerow
-(J.F.H.Beyma) McGinnis & W.Gams
 (J.F.H.Beyma) Schol-Schwarz
 (J.F.H.Beyma) Stolk & D.B.Scott
+(J.F.H.Beyma) W.Gams & McGinnis
 (J.F.H.Beyma) de Hoog
 (J.F.Macbr.) Pedley
 (J.F.Redhead ex T.H.Nicholson & N.C.Schenck) C.Walker & F.E.Sanders
 (J.Forbes ex Otto & A.Dietr.) Britton & Rose
+(J.Fröhl. & K.D.Hyde) Wulandari
 (J.G.Bruce) B.Øllg.
 (J.G.Kühn) Bubák
 (J.G.Kühn) G.P.Clinton
 (J.G.Kühn) Langdon & Full.
 (J.G.Kühn) McAlpine
+(J.G.West & Albr.) Hershk.
 (J.Garden) K.D.Hill
 (J.Garden) Silba
 (J.Gay ex Kunth) Endl.
 (J.Gay ex Kunth) J.Gay
 (J.Gay ex Kunth) Kuntze
 (J.Gay ex Kunth) Steetz
 (J.Gay ex Poir.) A.Benn.
@@ -10166,14 +10365,15 @@
 (J.H.Willis) Crisp
 (J.H.Willis) Crisp & P.H.Weston
 (J.H.Willis) Hawke ex Messina
 (J.H.Willis) Hislop, Crayn & Puente-Lel.
 (J.H.Willis) J.H.Willis
 (J.H.Willis) L.B.Moore
 (J.H.Willis) N.A.Wakef.
+(J.H.Willis) Ochyra
 (J.H.Willis) P.S.Short
 (J.H.Willis) Paul G.Wilson
 (J.H.Willis) Pedley
 (J.H.Willis) R.H.Zander
 (J.H.Willis) S.W.L.Jacobs & J.Everett
 (J.H.Willis) W.R.Barker
 (J.H.Willis) de Kok
@@ -10181,44 +10381,46 @@
 (J.J.Engel & G.L.Merr.) E.D.Cooper
 (J.J.Engel & G.L.Merr.) J.J.Engel
 (J.J.Engel & R.M.Schust.) Xiao L.He & Glenny
 (J.J.Engel) Hässel
 (J.J.Lee, C.W.Reimer & McEnery) Hallegr. & Burford
 (J.J.Lee, Reimer & McEnery) Hallegr. & Burford
 (J.J.Lee, Reimer & McEnery) Round, Hallsteinsen & Paasche
+(J.J.Muchovej) Alcorn
 (J.J.Rodr.) Kylin
 (J.J.Sm.) A.A.Eaton
 (J.J.Sm.) J.J.Sm.
 (J.J.Sm.) J.J.Verm.
 (J.J.Sm.) Kraenzl.
 (J.J.Sm.) M.A.Clem.
 (J.J.Sm.) M.A.Clem. & D.L.Jones
 (J.J.Sm.) Ormerod
 (J.J.Sm.) Pax & K.Hoffm.
 (J.J.Wood & C.L.Chan) D.L.Jones & M.A.Clem.
+(J.John) J.John & D.M.Williams
 (J.Kirk ex Benth.) J.Léonard
 (J.Koenig ex Roxb.) Nees
 (J.Koenig) Alston
 (J.Koenig) M.A.Clem. & D.L.Jones
 (J.Koenig) Ormerod
 (J.Koenig) S.R.Dutta
 (J.Koenig) Seidenf.
 (J.Koenig) Seidenf. & Ormerod
 (J.Koenig) Sm.
 (J.Koenig) Stapf
 (J.Kost.) Ghafoor
 (J.Kost.) Swenson & K.Bremer
 (J.Kuo) S.W.L.Jacobs & Les
-(J.L.Crane & Shearer) E.B.G.Jones & K.L.Pang
+(J.L.Crane & Shearer) K.L.Pang & E.B.G.Jones
 (J.L.Crane & Shearer) M.E.Palm & E.L.Stewart
-(J.L.Yuill) Malloch & Cain
+(J.L.Cunn.) Hern.-Restr. & Crous
+(J.L.Mulder) U.Braun & Crous
 (J.Larsen) de Salas, Bolch & Hallegr.
 (J.Lloyd ex Billot) F.W.Schultz
 (J.Lloyd ex Billot) Maire & Weiller
-(J.Lloyd) J.E.Wright
 (J.Lloyd) Kuntze
 (J.Lowe) D.A.Reid
 (J.Lowe) Jean Keller
 (J.M.Black ex Eardley) K.J.Cowley
 (J.M.Black) A.J.Scott
 (J.M.Black) A.T.Lee
 (J.M.Black) Aston
@@ -10276,15 +10478,15 @@
 (J.M.Black) Ulbr.
 (J.M.Black) Zotov
 (J.M.Powell) Hislop, Crayn & Puente-Lel.
 (J.M.Powell) Quinn
 (J.M.Yen) Deighton
 (J.Mackay ex Sweet) Court
 (J.Mackay ex Sweet) J.M.Black
-(J.Müller) Hariot
+(J.Müller) Har.
 (J.N.Rai, J.P.Tewari & Mukerji) P.F.Cannon
 (J.N.Rai, Wadhwani & J.P.Tewari) Mouch.
 (J.P.Ellis) D.R.Reynolds
 (J.Presl & C.Presl) C.B.Clarke
 (J.Presl & C.Presl) E.G.Camus
 (J.Presl) C.E.Hubb.
 (J.Presl) Chase
@@ -10349,25 +10551,24 @@
 (J.Roy & Bisset) Playfair
 (J.Roy & Bisset) Ruzicka
 (J.Roy & Bisset) West & G.S.West
 (J.Roy & Bissett) West & West
 (J.Roy) Playfair
 (J.Roy) West & G.S.West
 (J.Roy) Willi Krieg.
-(J.S.F.Barker & M.W.Mill.) Kurtzman & Robnett
-(J.S.F.Barker, M.W.Mill., Phaff, Starmer & M.Miranda) Y.Yamada
 (J.S.McCulloch) B.E.Tucker
 (J.S.Murray) Filson
 (J.Schiller) Balech
 (J.Schiller) D.K.Hilliard & Asmund
 (J.Schiller) D.Wall & B.Dale
-(J.Schiller) F.Gómez
 (J.Schiller) J.D.Dodge
+(J.Schiller) J.Schiller
 (J.Schiller) Lillick
 (J.Schröt. ex Höhn. & Litsch.) Hallenb.
+(J.Schröt.) Earle
 (J.Schröt.) Fritsch
 (J.Schröt.) Hauerslev & P.Roberts
 (J.Schröt.) Maire ex Martin-Sans
 (J.Schröt.) Vánky
 (J.Sm. ex C.Chr.) Christenh.
 (J.Sm.) Alderw.
 (J.Sm.) Baill.
@@ -10377,30 +10578,29 @@
 (J.Sm.) Hereman
 (J.Sm.) Holttum
 (J.Sm.) Hook.
 (J.Sm.) Müll.Arg.
 (J.Sm.) T.Moore
 (J.Sm.) Wall. ex Hook.
 (J.Steiner & Zahlbr.) Hale
-(J.Steiner & Zahlbr.) Serus.
 (J.Steiner & Zahlbr.) Sérus.
 (J.Steiner ex Fritsch) Lowen
 (J.Steiner) C.W.Dodge
 (J.Steiner) Essl.
 (J.Steiner) Hale
 (J.Steiner) Lowen
 (J.Steiner) Marbach
 (J.Steiner) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (J.Steiner) R.C.Harris
 (J.Steiner) Swinscow & Krog
 (J.T.Hunter & J.J.Bruhl) I.Telford & J.J.Bruhl
 (J.T.Hunter & J.J.Bruhl) I.Telford & Pruesapan
 (J.T.Hunter & J.J.Bruhl) R.W.Bouman
 (J.T.Hunter) Pedley
-(J.T.Queckett) W.Sm.
+(J.T.Quekett) W.Sm.
 (J.Tanaka & Pham-Hoàng) R.J.King & Puttock
 (J.Thompson) Crisp & P.H.Weston
 (J.V.Lamour. ex Duby) Ardiss. & J.Straff.
 (J.V.Lamour. ex Duby) Guiry & Hollenb.
 (J.V.Lamour. ex Duby) Mont.
 (J.V.Lamour. ex Duby) Schotter
 (J.V.Lamour. ex Poir.) J.Agardh
@@ -10446,52 +10646,59 @@
 (J.V.Lamour.) Womersley ex E.C.Oliveira
 (J.V.Lamour.) Y.M.Chamb.
 (J.W.Cribb) A.H.Sm.
 (J.W.Cribb) A.H.Sm. & D.A.Reid
 (J.W.Cribb) B.C.Zhang & Minter
 (J.W.Cribb) Bougher & Castellano
 (J.W.Cribb) Castellano
+(J.W.Cribb) Kuhar, Nouhra & M.E.Sm.
+(J.W.Cribb) P.M.Kirk
 (J.W.Cribb) Pegler & T.W.K.Young
 (J.W.Cribb) T.Lebel & Castellano
+(J.W.Cribb) T.Lebel & T.W.May
 (J.W.Cribb) T.W.May
 (J.W.Cribb) Trappe
 (J.W.Dawson) A.R.Bean
 (J.W.Dawson) Craven & J.W.Dawson
 (J.W.Green) Hopper
+(J.W.Green) Rye & Peter G.Wilson
 (J.W.Griff.) Skuja
 (J.W.Loudon) E.Wimm.
 (J.W.Mathews & L.Bolus) D.A.Cooke
 (J.W.Moore) N.Hallé
 (J.Walker & A.M.Sm.bis) H.C.Wetzel, Hulbert & Tisserat
 (J.Walker & A.M.Sm.bis) Shoemaker & C.E.Babc.
 (J.Walker & Bertus) J.A.Simpson
 (J.Walker & Bertus) U.Braun & Crous
+(J.Walker & Kile) Z.W.de Beer, T.A.Duong & M.J.Wingf.
 (J.Walker & R.G.Shivas) M.Scholler & Aime
+(J.Walker) Hern.-Restr. & Crous
 (J.Walker) J.A.Simpson, K.Thomas & Grgur.
 (J.Walker) J.Walker
 (J.Walker) Vánky
-(J.Walker, Pascoe & B.Sutton) Crous & Andjic
-(J.Walker, Pascoe & B.Sutton) Crous, B.Sutton & F.A.Ferreira
+(J.Walker, B.Sutton & Pascoe) Crous & Andjic
+(J.Walker, B.Sutton & Pascoe) Crous, F.A.Ferreira & B.Sutton
 (J.White) Cav.
 (J.White) Donn ex Sm.
 (J.White) Joy Thomps.
+(J.White) Peter G.Wilson
 (J.White) Sm.
 (J.Z.Weber & R.J.Bates) M.A.Clem. & D.L.Jones
 (J.Z.Weber) J.Z.Weber
 (Jaag) Anagn. & Komárek
 (Jaap) Aptroot
 (Jack ex Wall.) Sugumaran
 (Jack) Merr.
 (Jack) Planch. ex Hook.f.
 (Jack) Spreng.
 (Jack) Voigt
-(Jack) Voigt x Lumnitzera racemosa Willd.
 (Jackes) Jackes
 (Jacobi) Gentry
 (Jacobsen) Bourr.
+(Jacobsen) Grönblad
 (Jacq.) A.R.Simões & Staples
 (Jacq.) Alb. & Schwein.
 (Jacq.) All.
 (Jacq.) B.K.Simon & S.W.L.Jacobs
 (Jacq.) Baker
 (Jacq.) Benth.
 (Jacq.) Bég.
@@ -10557,15 +10764,14 @@
 (Jacq.) Schwantes
 (Jacq.) Spach
 (Jacq.) Steud. ex Fawc. & Rendle
 (Jacq.) Sw.
 (Jacq.) Sweet
 (Jacq.) T.Post & Kuntze
 (Jacq.) Vahl
-(Jacq.) Vahl x Stachytarpheta jamaicensis (L.) Vahl
 (Jacq.) W.F.Wright
 (Jacq.) Wahlenb.
 (Jacq.) Willd.
 (Jacq.) With.
 (Janisch & Rabenh.) Grunow
 (Janisch) Fryxell
 (Jansen) Eck-Borsb.
@@ -10587,48 +10793,54 @@
 (Jenner ex Hassall) P.Crouan & H.Crouan
 (Jessup) B.Xue & R.M.K.Saunders
 (Jessup) D.C.Thomas & R.M.K.Saunders
 (Jessup) Jessup
 (Jessup) L.L.Zhou, Y.C.F.Zu & R.M.K.Saunders
 (Jessup) M.P.Simmons
 (Jessup) Y.C.F.Su & R.M.K.Saunders
+(Joanne E.Taylor, K.D.Hyde & E.B.G.Jones) S.Konta & K.D.Hyde
 (Jolycl.) Ångstr.
 (Jord.) Ball
 (Jord.) Pugsley
 (Joshua) Croasdale
 (Joshua) Hirano
 (Joshua) Playfair
 (Joshua) Teiling
 (Joshua) Willi Krieg.
 (Joss. ex Dennis) Redhead, Vilgalys & Moncalvo
 (Joss.) Joss.
 (Joss.) Noordel.
+(Joy Thomps.) Peter G.Wilson
 (Juel) Juel
 (Jul.Schäff.) E.Horak
 (Jul.Schäff.) Kühner
 (Jul.Schäff.) M.M.Moser
+(Jungh.) Audet
 (Jungh.) Bres.
 (Jungh.) C.Y.Wu
 (Jungh.) Cleland & Cheel
 (Jungh.) Cooke
 (Jungh.) Corner
 (Jungh.) Fr.
 (Jungh.) G.Cunn.
 (Jungh.) Höhn.
 (Jungh.) Imazeki
 (Jungh.) Jean Keller
 (Jungh.) Jülich
 (Jungh.) Lév.
 (Jungh.) Massee
+(Jungh.) Miettinen
 (Jungh.) Murrill
 (Jungh.) Pavill. & Lagarde
 (Jungh.) Rostaf.
 (Jungh.) Ryvarden
 (Jungh.) Singer
 (Jungh.) Teng
+(Jungh.) Zmitr. & Kovalenko
+(Jungh.) Zmitr. & Malysheva
 (Juss. ex Aubl.) C.F.Baker
 (Juss. ex Poir.) Leenh.
 (Juss. ex Poir.) Radlk.
 (Juss.) Baker
 (Juss.) Bakh.
 (Juss.) Benth.
 (Juss.) D'Arcy
@@ -10637,50 +10849,49 @@
 (Juss.) Less.
 (Juss.) Miq.
 (Juss.) Nied.
 (Juss.) Planch.
 (Juss.) Schult.
 (Juss.) Sweet
 (Juswara) M.C.Pace
-(Jörg) F.Gómez, D.Moreira & López-García
-(Jörg) Steem.Niels.
-(Jörg.) Balech
-(Jörg.) Böhm
-(Jörg.) F.Gómez
-(Jörg.) F.Gómez, D.Moreira & López-García
-(Jörg.) Jörg.
-(Jörg.) Ostenf. & E.J.Schmidt
-(Jörg.) Parke & J.D.Dodge
-(Jörg.) Paulsen
-(Jörg.) Sournia
-(Jörg.) Steem.Niels.
-(Jörg.) T.H.Abé
+(Jørg.) Balech
+(Jørg.) Böhm
+(Jørg.) F.Gómez
+(Jørg.) F.Gómez, D.Moreira & López-García
+(Jørg.) Jørg.
+(Jørg.) Ostenf. & E.J.Schmidt
+(Jørg.) Parke & J.D.Dodge
+(Jørg.) Paulsen
+(Jørg.) Sournia
+(Jørg.) Steem.Niels.
+(Jørg.) T.H.Abé
 (Jülich) D.A.Reid
-(Jülich) L.G.Krieglst.
+(Jülich) Krieglst.
 (Jülich) Sheng H.Wu
 (K.Ahlner) H.S.Hayden, Blomster, Maggs, P.C.Silva, Stanhope & Waaland
+(K.Ando & Pitt) Houbraken & Samson
 (K.Brandt) Beij.
 (K.D.Hill & L.A.S.Johnson) A.R.Bean
 (K.D.Hill & L.A.S.Johnson) Brooker
 (K.D.Hill & L.A.S.Johnson) Brooker & Kleinig
+(K.D.Hill & L.A.S.Johnson) Crisp & L.G.Cook
+(K.D.Hill & L.A.S.Johnson) D.Nicolle
 (K.D.Hill) Brooker
 (K.D.Hill) P.I.Forst. & Liddle
 (K.D.Hyde & Borse) Suetrong, Sakay., E.B.G.Jones & C.L.Schoch
-(K.D.Hyde & Crous) L.Lombard, M.J.Wingf. & Crous
-(K.D.Hyde & Shearer) K.Hiray., Kaz.Tanaka & Shearer
-(K.D.Hyde & Yanna) K.D.Hyde & Yanna
+(K.D.Hyde) E.C.Y.Liew, Aptroot & K.D.Hyde
+(K.D.Hyde) J.Campb., J.L.Anderson & Shearer
 (K.D.Hyde) K.D.Hyde
-(K.D.Hyde) K.D.Hyde & S.J.Stanley
-(K.D.Hyde) K.D.Hyde, Aptroot & E.C.Y.Liew
-(K.D.Hyde) K.D.Hyde, E.B.G.Jones & S.W.Wong
-(K.D.Hyde) Shearer, J.Campb. & J.L.Anderson
-(K.D.Hyde, C.A.Pearce & Læssøe) J.D.Rogers, Y.M.Ju & F.San Martín
+(K.D.Hyde) K.D.Hyde, S.W.Wong & E.B.G.Jones
+(K.D.Hyde) Réblová & A.N.Mill.
+(K.D.Hyde) S.J.Stanley & K.D.Hyde
+(K.D.Hyde) Z.L.Luo, Maharachch. & K.D.Hyde
+(K.D.Hyde, J.Fröhl. & Joanne E.Taylor) K.D.Hyde, J.Fröhl. & Joanne E.Taylor
 (K.D.Koenig ex Retz.) Merr.
 (K.D.Koenig) Benth.
-(K.D.Koenig) Link
 (K.Harris & D.E.Bradley) K.Harris
 (K.I.Goebel) Herzog
 (K.I.Goebel) Mizut.
 (K.J.Brooks) Craven & R.D.Edwards
 (K.J.Cowley) Craven
 (K.Kirkman) A.R.Bean
 (K.Koch) Asch. & Graebn.
@@ -10724,31 +10935,31 @@
 (K.Schum.) Schltr.
 (K.Schum.) Tiegh.
 (K.Strøm) Teiling
 (K.W.Dixon & Meney) B.G.Briggs & L.A.S.Johnson
 (Kalb & Elix) Kalb & Elix
 (Kalb & Elix) Kalb, Lumbsch & Elix
 (Kalb & Vězda) Lücking
+(Kalchbr. & Cooke) Theiss.
 (Kalchbr. & F.Muell.) Cooke
 (Kalchbr. & F.Muell.) McAlpine
 (Kalchbr. & F.Muell.) Sacc.
 (Kalchbr. ex Cooke) Bres.
 (Kalchbr. ex Cooke) Cheel
 (Kalchbr. ex Cooke) Cooke
 (Kalchbr. ex Cooke) G.Cunn.
 (Kalchbr. ex Cooke) J.E.Wright
 (Kalchbr. ex Cooke) Kuntze
 (Kalchbr. ex Cooke) S.Ahmad
 (Kalchbr. ex Cooke) Sacc.
-(Kalchbr. ex Massee) C.W.Dodge & Zeller
 (Kalchbr. ex Massee) Lloyd
 (Kalchbr. ex Massee) Pegler & T.W.K.Young
+(Kalchbr. ex Massee) Zeller & C.W.Dodge
 (Kalchbr.) A.M.Young
 (Kalchbr.) Antonín & Noordel.
-(Kalchbr.) Brittleb.
 (Kalchbr.) Cleland
 (Kalchbr.) Cleland & Cheel
 (Kalchbr.) Cooke
 (Kalchbr.) D.A.Reid
 (Kalchbr.) D.Hawksw.
 (Kalchbr.) De Toni
 (Kalchbr.) Dring
@@ -10760,25 +10971,29 @@
 (Kalchbr.) G.Stev.
 (Kalchbr.) Henn.
 (Kalchbr.) Kalchbr.
 (Kalchbr.) Killerm.
 (Kalchbr.) Kuntze
 (Kalchbr.) Lloyd
 (Kalchbr.) Locq.
+(Kalchbr.) Lodge, Padamsee & S.A.Cantrell
 (Kalchbr.) McAlpine
 (Kalchbr.) N.Walters & E.W.B.Da Costa
 (Kalchbr.) P.Karst.
 (Kalchbr.) Pat.
 (Kalchbr.) Pegler
 (Kalchbr.) Pilát
 (Kalchbr.) R.H.Petersen
 (Kalchbr.) Sacc.
 (Kalchbr.) Sacc. & Traverso
+(Kalchbr.) Spirin
 (Kalchbr.) Vassilkov
 (Kalchbr.) Vilgalys, Hopple & Jacq.Johnson
+(Kamg.Nkuek., K.Jacobs & M.J.Wingf.) Z.W.de Beer & M.J.Wingf.
+(Kamgan & Jol.Roux) Z.W.de Beer, T.A.Duong & M.J.Wingf.
 (Kamienski) Barnhart
 (Kaneh.) Sleumer
 (Kano) de Hoog
 (Kanouse) Seaver
 (Kanouse) Spooner
 (Kantvilas & Coppins) Resl & T.Sprib.
 (Kantvilas & Elix) A.W.Archer & Elix
@@ -10796,35 +11011,34 @@
 (Kantvilas) I.Schmitt, Kalb & Lumbsch
 (Kantvilas) Kantvilas & Grube
 (Kar. & Kir.) Cullen
 (Kar. & Kir.) Tzvelev
 (Karling) Karling
 (Karling) M.W.Dick
 (Karling) Sparrow
-(Karsten) Hariot
+(Karsten) Har.
 (Kauffman) A.H.Sm.
-(Kauffman) A.H.Sm. & Leathers
 (Kauffman) Boedijn
 (Kauffman) Jülich
+(Kauffman) Leathers & A.H.Sm.
 (Kauffman) Singer
 (Kaulf. ex Link) Christenh.
-(Kaulf. ex Link) Christenh. x Blechnum lineare (C.Moore ex J.Sm.) Christenh.
-(Kaulf. ex Link) Christenh. x Blechnum medium (R.Br.) Christenh.
 (Kaulf.) Alston
 (Kaulf.) C.Chr.
 (Kaulf.) C.Presl
 (Kaulf.) Farw.
 (Kaulf.) Fosberg
 (Kaulf.) Holttum
 (Kaulf.) Hook. & Grev.
 (Kaulf.) J.P.Roux
 (Kaulf.) Trevis.
 (Keighery & Cranfield) Christenh. & Byng
 (Keighery) Christenh. & Byng
 (Keighery) Hislop
+(Keighery) Olde & Keighery
 (Keighery) R.L.Barrett
 (Keissl.) Hollerb.
 (Keissl.) Lemmerm.
 (Kellogg) Greene
 (Kellogg) Kuntze
 (Kellogg) M.F.Ray
 (Kenneally & E.L.Schneid.) Löhne, Wiersema & Borsch
@@ -10846,33 +11060,32 @@
 (Kers) R.L.Barrett
 (Keyserl.) C.Chr.
 (Keyserl.) Ching
 (Keyserl.) Christ
 (Kiffer) P.M.Kirk
 (Kill.) F.A.Wolf
 (Kindb.) L.G.Adams
-(Kindb.) M.Fleisch.
 (Kindb.) Müll.Hal. ex Loeske
 (Kindb.) R.S.Chopra
 (Kindb.) Watts & Whitel.
 (Kindb.) Willk.
 (King & Gamble) P.I.Forst.
+(King & Pantl.) Pradhan
 (King ex Hook.f.) Zerega, Supardi & T.J.Motley
 (King) C.C.Berg
 (King) Corner
 (King) Pannell
 (Kippist ex Lindl.) G.Chandler & Crisp
 (Kippist ex Meisn.) A.R.Mast & K.R.Thiele
 (Kippist ex Meisn.) Benth.
 (Kippist ex Meisn.) Christenh. & Byng
 (Kippist ex Meisn.) E.M.Benn.
 (Kippist) Benth.
+(Kippist) Crisp & L.G.Cook
 (Kippist) K.D.Hill & L.A.S.Johnson
-(Kippist) K.D.Hill & L.A.S.Johnson x Corymbia dallachiana (Benth.) K.D.Hill & L.A.S.Johnson
-(Kippist) K.D.Hill & L.A.S.Johnson x Corymbia tessellaris (F.Muell.) K.D.Hill & L.A.S.Johnson
 (Kippist) T.Baines
 (Kippist) Veitch
 (Kirchn.) Hansg.
 (Kirchn.) Hieron.
 (Kirchn.) K.Möbius
 (Kirchn.) Kuntze
 (Kirchn.) Lütkem.
@@ -10946,23 +11159,25 @@
 (Klotzsch) Rauschert
 (Klotzsch) Ryvarden
 (Klotzsch) Schauer
 (Klotzsch) Singer
 (Klotzsch) Sleumer
 (Klotzsch) Sond.
 (Klotzsch) Teng
-(Klöcker) Samson & Stolk
+(Klotzsch) Zmitr. & Malysheva
+(Klöcker) Stolk & Samson
 (Knight) A.R.Mast & K.R.Thiele
 (Knight) Christenh. & Byng
 (Knight) Domin
 (Knight) McGill.
 (Knight) Sweet
 (Knowles & Westc.) Benth.
 (Kny) Karling
 (Kobayasi & Imazeki) Corner
+(Kobayasi) G.H.Sung, J.M.Sung, Hywel-Jones & Spatafora
 (Koch) Burnat
 (Koch) J.M.Black
 (Koch) Pilg.
 (Kodela & Tame) Pedley
 (Kodela) Pedley
 (Kodela, Tindale & D.Keith) Pedley
 (Koehne) Hewson
@@ -10986,35 +11201,35 @@
 (Kof.) E.J.F.Wood
 (Kof.) F.Gómez
 (Kof.) F.Gómez, D.Moreira & López-García
 (Kof.) F.J.R.Taylor
 (Kof.) Hallegr. & Huisman
 (Kof.) Hernández-Becerril
 (Kof.) J.Schiller
-(Kof.) Jörg.
+(Kof.) Jørg.
 (Kof.) Kof. & J.R.Michener
 (Kof.) Kof. & Skogsb.
 (Kof.) N.Peters
 (Kof.) Pavill.
-(Kohlm. & E.Kohlm.) E.B.G.Jones & J.Dupont
 (Kohlm. & E.Kohlm.) Hafellner
+(Kohlm. & E.Kohlm.) J.Dupont & E.B.G.Jones
 (Kohlm. & E.Kohlm.) Kohlm. & Volkm.-Kohlm.
 (Kohlm. & E.Kohlm.) Shearer & J.L.Crane
 (Kohlm. & Vittal) Kohlm., Volkm.-Kohlm., Suetrong, Sakay. & E.B.G.Jones
 (Kohlm. & Volkm.-Kohlm.) Suetrong, Sakay., E.B.G.Jones, Kohlm., Volkm.-Kohlm. & C.L.Schoch
 (Kohlm.) B.Sutton
-(Kohlm.) E.B.G.Jones & K.L.Pang
+(Kohlm.) K.L.Pang & E.B.G.Jones
 (Kohlm.) Kohlm.
 (Kohlm.) Kohlm. & Volkm.-Kohlm.
 (Kohlm.) Meyers & R.T.Moore
+(Kohlm., I.Schmidt & N.B.Nair) P.Correia, E.Azevedo & M.F.Caeiro
 (Kolbe) Nagumo & Kobayashi
 (Komárek) Compère
 (Komárek) Komárek ex Komárek
 (Komárek) M.Watanabe
-(Konrad) Kuhner
 (Konrad) Kühner
 (Koord.) Aa
 (Koord.) Merr.
 (Koord.) Speg.
 (Kores) M.A.Clem. & D.L.Jones
 (Kores) Szlach.
 (Korf) Korf
@@ -11045,14 +11260,15 @@
 (Krasske) D.G.Mann
 (Krasske) Hust.
 (Krasske) Krasske
 (Krasske) Lange-Bert.
 (Krasske) M.Nörpel & Alles
 (Kreger-van Rij) M.Suzuki & Kurtzman
 (Kreger-van Rij) Van der Walt, Y.Yamada, K.Maeda & I.Banno
+(Kreisel & D.Krüger) Vizzini
 (Kremp. ex Nyl.) G.Thor
 (Kremp. ex Nyl.) Henssen & G.Thor
 (Kremp.) A.W.Archer
 (Kremp.) A.W.Archer & Elix
 (Kremp.) Aptroot
 (Kremp.) Aptroot & Lücking
 (Kremp.) D.J.Galloway
@@ -11079,37 +11295,37 @@
 (Kremp.) R.Sant.
 (Kremp.) Rambold & Hafellner
 (Kremp.) Rivas Plata & Lumbsch
 (Kremp.) Vain.
 (Kremp.) Vězda
 (Kremp.) Wetmore
 (Kremp.) Zahlbr.
-(Krempelhüber) Hariot
+(Krempelhüber) Har.
 (Krock.) Philcox
 (Krog & Swinscow) Elix & Hale
 (Krog & Swinscow) G.N.Stevens
 (Krog & Swinscow) Krog & Swinscow
 (Krog) Hale
 (Krombh.) Britzelm.
 (Krombh.) Fr.
 (Krombh.) Quél.
 (Krombh.) Wasser
 (Kuck.) Hamel
 (Kuck.) Kylin
+(Kuehn & G.F.Orr) Doweld
 (Kuetz.) Rabenh.
 (Kuff.) F.A.Skinner
 (Kuff.) Geitler
+(Kuhar, Nouhra & M.E.Sm.) Trappe & Claridge
 (Kuhn) Domin
-(Kulk.) Thirum. & Mundk.
+(Kulk.) Mundk. & Thirum.
 (Kunth & C.D.Bouché) F.Muell.
 (Kunth & C.D.Bouché) Hallier f. ex Schlittler
 (Kunth & C.D.Bouché) Miq.
-(Kunth) A.Gray
 (Kunth) Asch. & Graebn.
-(Kunth) Baker
 (Kunth) Balansa
 (Kunth) Bartl.
 (Kunth) Benth. & Hook.f.
 (Kunth) Bess
 (Kunth) Beurlin
 (Kunth) Blume
 (Kunth) Boeckeler
@@ -11169,25 +11385,25 @@
 (Kunth) Sch.Bip.
 (Kunth) Schult.
 (Kunth) Seem.
 (Kunth) Spangler
 (Kunth) Spreng.
 (Kunth) Stapf
 (Kunth) Steud.
-(Kunth) Strother
 (Kunth) T.Koyama
 (Kunth) Trel.
 (Kunth) Tzvelev
 (Kunth) Vasey
 (Kunth) Wedd.
 (Kuntze ex Fr.) Dennis
 (Kuntze) Azevedo-Gonc. & Matzenb.
 (Kuntze) C.B.Clarke ex Domin
 (Kuntze) C.E.Hubb.
 (Kuntze) Cabrera
+(Kuntze) Cleland & Cheel
 (Kuntze) Domin
 (Kuntze) Harms
 (Kuntze) J.Agardh
 (Kuntze) J.J.Sm.
 (Kuntze) J.W.Grimes
 (Kuntze) Kuntze
 (Kuntze) Kük.
@@ -11202,15 +11418,14 @@
 (Kunze ex Cooke) G.Cunn.
 (Kunze ex Fr.) Fr.
 (Kunze ex Fr.) Rabenh.
 (Kunze ex Fr.) Ryvarden
 (Kunze ex Fr.) S.C.Jong & E.E.Davis
 (Kunze ex Mett.) C.Chr.
 (Kunze ex Mett.) Copel.
-(Kunze ex Mett.) Fée
 (Kunze ex Mett.) Tindale
 (Kunze) A.Braun
 (Kunze) A.Braun & C.D.Bouché
 (Kunze) A.J.Br.
 (Kunze) Alston
 (Kunze) B.Øllg.
 (Kunze) Bonap.
@@ -11241,27 +11456,25 @@
 (Kurok.) Elix
 (Kurok.) Elix & Hale
 (Kurok.) Elix & J.Johnst.
 (Kurok.) Elix, A.Thell & Søchting
 (Kurok.) Hale
 (Kurok.) Hale & Elix
 (Kurok.) J.-C.Wei & J.-M.Jiang
-(Kurok.) Krog & Swinscow
 (Kurok.) Kurok.
 (Kurok.) Streimann
 (Kurok.) Swinscow & Krog
 (Kurok.) W.L.Culb.
 (Kurt Forst. & Eckert) Kurt Först.
-(Kurtzman, Vaughan-Mart., S.A.Mey. & E.B.O'Neill) Kurtzman & M.Suzuki
-(Kurtzman, Wick. & Herman) Arx & Van der Walt
 (Kurz) B.C.Stone
 (Kurz) Hegelm.
 (Kurz) Kuntze
 (Kurz) Pax & K.Hoffm.
 (Kurz) Willi Krieg. & Gerloff
+(Kuyper) Matheny, Vizzini & Esteve-Rav.
 (Kylin) E.Y.Dawson
 (Kylin) Garbary
 (Kylin) Hamel
 (Kylin) K.M.Drew
 (Kylin) Necchi & Entwisle
 (Kylin) Papenf.
 (Kylin) R.E.Norris
@@ -11290,52 +11503,51 @@
 (Körb.) S.Y.Kondr., Fedorenko, S.Stenroos, Kärnefelt & A.Thell
 (Körb.) Sheard
 (Körb.) Zahlbr.
 (Körn. ex Müll.Berol.) Asch.
 (Körn. ex Müll.Berol.) Benth.
 (Körn.) Erikss. & Henning
 (Körn.) Liro
+(Küchenm. & Rabenh.) Vuill.
 (Kühner ex Wasser) Bon
 (Kühner) Joss.
+(Kühner) Matheny & Esteve-Rav.
 (Kük. ex Cheeseman) Hamlin
 (Kük. ex Cheeseman) Kük.
 (Kük.) K.L.Wilson
 (Kük.) Kük.
 (Kük.) R.L.Barrett
 (Kük.) S.T.Blake
 (Kük.) T.Koyama
-(Kütz) Bréb. & Godey
 (Kütz. ex Bornet & Flahault) Komárek & Anagn.
 (Kütz. ex Bréb.) Bréb.
 (Kütz. ex Gomont) Anagn. & Komárek
 (Kütz. ex Gomont) F.E.Drouet
 (Kütz. ex Ralfs) Rabenh.
-(Kütz. ex W.D.J.Koch) Lansdown
-(Kütz. ex W.D.J.Koch) Stace
 (Kütz.) A.B.Joly
 (Kütz.) A.Braun ex G.A.Klebs
 (Kütz.) A.Cleve
 (Kütz.) A.Mayer
 (Kütz.) A.W.Griffiths & Harv.
 (Kütz.) Aboal
 (Kütz.) Ardiss.
 (Kütz.) Aresch.
 (Kütz.) Baldock
 (Kütz.) Batters
 (Kütz.) Beger & Wichmann
 (Kütz.) Bliding
-(Kütz.) Boedeker
 (Kütz.) Bornet
 (Kütz.) Bornet & Flahault
 (Kütz.) Bornet ex De Toni
 (Kütz.) Brun
 (Kütz.) Bréb.
 (Kütz.) Bréb. & Godey
 (Kütz.) Bréb. ex Kütz.
 (Kütz.) Børgesen
+(Kütz.) C.Boed.
 (Kütz.) Cleve
 (Kütz.) Compère
 (Kütz.) Compère & Bukht.
 (Kütz.) Croasdale
 (Kütz.) Czarn.
 (Kütz.) D.G.Mann
 (Kütz.) D.M.Williams & Round
@@ -11418,14 +11630,15 @@
 (Kütz.) P.C.Silva, K.Mattox & W.Blackwell
 (Kütz.) P.Crouan & H.Crouan
 (Kütz.) P.W.Gabrielson
 (Kütz.) Papenf.
 (Kütz.) Picc.
 (Kütz.) Playfair
 (Kütz.) Printz
+(Kütz.) R.A.Towns.
 (Kütz.) R.D.Wood
 (Kütz.) R.M.Patrick
 (Kütz.) Rabenh.
 (Kütz.) Ralfs
 (Kütz.) Reinbold
 (Kütz.) Reinke
 (Kütz.) Reinsch
@@ -11462,20 +11675,16 @@
 (L'Hér.) Kuntze
 (L'Hér.) Link
 (L'Hér.) Müll.Arg.
 (L'Hér.) Pedley
 (L'Hér.) Pers.
 (L'Hér.) Sweet
 (L'Hér.) Willd.
-(L. : Fr.) Gray
-(L. : Fr.) Lam.
-(L. : Fr.) Quel.
 (L. : Fr.) Quél.
 (L. : Fr.) Redhead, Lutzoni, Moncalvo & Vilgalys
-(L. ex Jolycl.) Angstr.
 (L.) A.Braun & Asch.
 (L.) A.Camus
 (L.) A.Chev.
 (L.) A.DC.
 (L.) A.Gray
 (L.) A.H.Gentry
 (L.) A.J.Scott
@@ -11676,14 +11885,15 @@
 (L.) Fée
 (L.) G.Brückn.
 (L.) G.Cunn.
 (L.) G.Don
 (L.) G.Gaertn., B.Mey. & Scherb.
 (L.) G.J.Lewis
 (L.) G.L.Nesom
+(L.) G.L.Webster
 (L.) G.Lopez
 (L.) G.Mans.
 (L.) G.Mey.
 (L.) G.Nicholson
 (L.) Gaertn.
 (L.) Gagnep.
 (L.) Gaillon
@@ -11714,14 +11924,15 @@
 (L.) H.Karst. ex Farw.
 (L.) H.Lev.
 (L.) H.Ohashi
 (L.) H.Ohashi & K.Ohashi
 (L.) H.Rob.
 (L.) H.Rob. & Cuatrec.
 (L.) H.S.Irwin & Barneby
+(L.) H.Scholz
 (L.) H.Walter
 (L.) Hack.
 (L.) Haines
 (L.) Halacsy
 (L.) Hale
 (L.) Hallier f.
 (L.) Hanelt
@@ -11796,30 +12007,29 @@
 (L.) Juss. ex Kunth
 (L.) Juss. ex Schult.
 (L.) K.Iwats.
 (L.) K.Koch
 (L.) K.Lewin
 (L.) K.Richt.
 (L.) K.Schum.
-(L.) Kallersjo
 (L.) Karsten
 (L.) Kaulf.
 (L.) Ker Gawl.
 (L.) Kerguelen
 (L.) Kjellm.
 (L.) Koehne
 (L.) Kosterm.
 (L.) Krock.
 (L.) Kuhn
 (L.) Kunth
 (L.) Kunth ex C.B.Clarke
 (L.) Kuntze
-(L.) Kuntze x Valerianoides mutabilis (Jacq.) Kuntze
 (L.) Kurz
 (L.) Kylin
+(L.) Källersjö
 (L.) Körb.
 (L.) Körn.
 (L.) Kütz.
 (L.) L'Hér.
 (L.) L'Hér. ex Vent.
 (L.) L.
 (L.) L. ex Bartal.
@@ -11837,25 +12047,23 @@
 (L.) Lambotte
 (L.) Lange
 (L.) Lassen
 (L.) Laterr.
 (L.) Les & R.R.Haynes
 (L.) Less.
 (L.) Levyns
-(L.) Levyns x Arctotheca populifolia (P.J.Bergius) Norl.
 (L.) Leyss.
 (L.) Liebm.
 (L.) Lindl.
 (L.) Lindsay
 (L.) Link
 (L.) Lippold
 (L.) Lloyd
 (L.) Loisel.
 (L.) Lunell
-(L.) Lutzoni, Redhead, Moncalvo & Vilgalys
 (L.) Lye
 (L.) Lyngb.
 (L.) M.B.Crespo, Mart.-Azorin & Mavrodiev
 (L.) M.Bieb.
 (L.) M.Choisy
 (L.) M.Roem.
 (L.) M.Roser & H.R.Hamasha
@@ -12000,14 +12208,15 @@
 (L.) Roussel
 (L.) Rouy
 (L.) Roxb.
 (L.) Rudolph
 (L.) Rusby ex A.Lyons
 (L.) Rydb.
 (L.) Röhl.
+(L.) S.E.Fawc. & A.R.Sm.
 (L.) S.F.Blake
 (L.) S.F.Gray
 (L.) S.Fuentes, Uotila & Borsch
 (L.) S.S.Hooper
 (L.) S.Y.Hu
 (L.) Sacc.
 (L.) Salisb.
@@ -12088,15 +12297,14 @@
 (L.) Turner
 (L.) Tutin
 (L.) Tzvelev
 (L.) U.Manns & Anderb.
 (L.) Underw.
 (L.) Urb.
 (L.) Vahl
-(L.) Vahl x Stachytarpheta mutabilis (Jacq.) Vahl
 (L.) Vain.
 (L.) Vent.
 (L.) Verdc.
 (L.) Vill.
 (L.) Vis.
 (L.) Voigt
 (L.) Voss
@@ -12105,15 +12313,14 @@
 (L.) W.Wight
 (L.) Wahlb.
 (L.) Wahlenb.
 (L.) Wall.
 (L.) Wallr.
 (L.) Walp.
 (L.) Webb & Berthel.
-(L.) Webb & Berthel. x Malva preissiana Miq.
 (L.) Webb ex Prantl
 (L.) Webb ex Sch.Bip.
 (L.) Weber
 (L.) Weber ex F.H.Wigg.
 (L.) Wedd.
 (L.) Wettst.
 (L.) Wight
@@ -12131,66 +12338,67 @@
 (L.A.S.Johnson & Blaxell) Brooker & Kleinig
 (L.A.S.Johnson & K.D.Hill) A.R.Bean
 (L.A.S.Johnson & K.D.Hill) Brooker
 (L.A.S.Johnson & K.D.Hill) Brooker, Slee & J.D.Briggs
 (L.A.S.Johnson & K.D.Hill) Byrne
 (L.A.S.Johnson & K.D.Hill) D.Nicolle
 (L.A.S.Johnson & K.D.Hill) D.Nicolle & Brooker
-(L.A.S.Johnson & K.D.Hill) D.Nicolle & Brooker - Eucalyptus spathulata subsp. salina D.Nicolle & Brooker
-(L.A.S.Johnson & K.D.Hill) D.Nicolle & Brooker - Eucalyptus suggrandis L.A.S.Johnson & K.D.Hill
 (L.A.S.Johnson & K.D.Hill) D.Nicolle & M.E.French
 (L.A.S.Johnson & K.D.Hill) J.T.Hunter
 (L.A.S.Johnson & O.D.Evans) B.G.Briggs & L.A.S.Johnson
 (L.A.S.Johnson & O.D.Evans) L.A.S.Johnson & B.G.Briggs
 (L.A.S.Johnson ex G.J.Leach) Brooker
+(L.A.S.Johnson ex G.J.Leach) D.Nicolle
 (L.A.S.Johnson ex G.J.Leach) K.R.Thiele & Ladiges
+(L.A.S.Johnson ex G.J.Leach) L.A.S.Johnson & K.D.Hill
 (L.A.S.Johnson) Brooker & Slee
 (L.A.S.Johnson) Christenh. & Byng
+(L.A.S.Johnson) Crisp & L.G.Cook
 (L.A.S.Johnson) D.L.Jones
+(L.A.S.Johnson) D.Nicolle
 (L.A.S.Johnson) L.A.S.Johnson
 (L.A.S.Johnson) L.A.S.Johnson & K.D.Hill
 (L.A.S.Johnson) Paul G.Wilson
 (L.Bolus) L.Bolus
 (L.Bolus) N.E.Br.
-(L.D.Pryor & L.A.S.Johnson) Parra-Os. & Ladiges
+(L.D.Pryor & L.A.S.Johnson ex Brooker) Crisp & L.G.Cook
+(L.D.Pryor & L.A.S.Johnson ex Brooker) Parra-Os. & Ladiges
 (L.G.Adams) Glenny
 (L.G.Adams) K.R.Thiele
 (L.G.Adams) R.J.Little & Leiper
 (L.G.Adams) Seppelt
 (L.G.Adams) T.A.James
 (L.H.Bailey) L.H.Bailey
 (L.H.Bailey) Mansf.
 (L.H.Bailey) Rydb.
 (L.K.Jones) Aveskamp, Gruyter & Verkley
 (L.K.Jones) Boerema
 (L.K.Jones) Morgan-Jones & K.B.Burch
 (L.Ling) L.Guo
+(L.Ling) McTaggart & R.G.Shivas
 (L.Ling) Vánky
-(L.M.Perry) Hoogland
 (L.Mangin) A.R.Loebl.
 (L.Mangin) Balech
 (L.Mangin) G.A.Fryxell & A.K.S.Prasad
 (L.Mangin) J.Schiller
 (L.Mangin) M.Lebour ex Balech
 (L.O.Williams) C.D.Adams ex W.C.Burger & C.M.Taylor
 (L.Preiss ex Endl.) K.Krause
 (L.Preiss ex Fr.) Kuntze
 (L.R.Fraser & Vickery) Menadue
+(L.R.Fraser) 
 (L.R.Fraser) Bat.
 (L.R.Fraser) Bat. & Cif.
+(L.R.Fraser) Cif. & Bat.
 (L.R.Fraser) S.Hughes
 (L.S.Sm.) Chinnock
-(L.S.Sm.) Chinnock - Eremophila bowmanii subsp. nutans Chinnock
-(L.S.Sm.) Chinnock - Eremophila latrobei F.Muell.
-(L.S.Sm.) Chinnock x Eremophila latrobei subsp. glabra (L.S.Sm.) Chinnock
 (L.S.Sm.) Jackes & M.Hurley
 (L.S.Sm.) Kosterm.
 (L.S.Sm.) Peter G.Wilson
-(L.W.Burgess & Sangal.) L.W.Burgess & Benyon
-(L.W.Burgess, G.A.Forbes & Windels) Summerell & L.W.Burgess
+(L.S.Sm.) Satthaphorn
 (L.f. ex Aiton) J.Schust.
 (L.f. ex Aiton) Lehm.
 (L.f.) A.DC.
 (L.f.) A.Dietr.
 (L.f.) A.Gray
 (L.f.) Ach.
 (L.f.) Adamson & Sprague
@@ -12204,39 +12412,40 @@
 (L.f.) C.Presl
 (L.f.) Casp.
 (L.f.) Cass.
 (L.f.) Chaz.
 (L.f.) Copel.
 (L.f.) DC.
 (L.f.) Desv.
+(L.f.) Diels
 (L.f.) Druce
 (L.f.) Engl.
 (L.f.) Ettingsh.
 (L.f.) F.Muell.
 (L.f.) F.N.Williams
 (L.f.) G.J.Lewis
 (L.f.) G.Nicholson
-(L.f.) Gaertn.
 (L.f.) Goetgh. & D.A.Simpson
 (L.f.) Goldblatt
 (L.f.) Hack.
 (L.f.) Haw.
 (L.f.) Heine
 (L.f.) Hook.f.
+(L.f.) Hort. ex Engl.
 (L.f.) I.M.Johnst.
 (L.f.) J.G.West
 (L.f.) J.Sm.
 (L.f.) K.Lewin
 (L.f.) K.Schum.
-(L.f.) Kallersjo
 (L.f.) Ker Gawl.
 (L.f.) Klatt
 (L.f.) Kuhn
 (L.f.) Kunth
 (L.f.) Kuntze
+(L.f.) Källersjö
 (L.f.) L'Hér.
 (L.f.) L.Bolus
 (L.f.) Lam.
 (L.f.) Less.
 (L.f.) Levyns
 (L.f.) Link
 (L.f.) M.Kato
@@ -12260,26 +12469,24 @@
 (L.f.) Retz.
 (L.f.) Royle
 (L.f.) Sch.Bip.
 (L.f.) Schrad.
 (L.f.) Schwantes
 (L.f.) Sherff
 (L.f.) Sm.
-(L.f.) Small ex Diels
 (L.f.) Sond.
 (L.f.) Spreng.
 (L.f.) Sw.
 (L.f.) Sweet
 (L.f.) Thunb.
 (L.f.) Trin.
 (L.f.) Willd.
 (Labill. ex Vent.) Bunge
 (Labill. ex Vent.) DC.
 (Labill.) A.DC.
-(Labill.) Ach.
 (Labill.) Allan
 (Labill.) Anderb.
 (Labill.) Anderb. & Haegi
 (Labill.) Anon.
 (Labill.) Aresch.
 (Labill.) Asch. & Graebn.
 (Labill.) B.G.Briggs & L.A.S.Johnson
@@ -12296,30 +12503,28 @@
 (Labill.) C.A.Mey.
 (Labill.) C.Agardh
 (Labill.) C.Chr.
 (Labill.) C.F.Reed
 (Labill.) C.M.Weiller
 (Labill.) C.Norman
 (Labill.) C.Presl
-(Labill.) C.Presl x Asplenium bulbiferum subsp. gracillimum (Colenso) Brownsey
 (Labill.) Cass.
 (Labill.) Cass. ex Less.
 (Labill.) Cheeseman
 (Labill.) Ching
 (Labill.) Chodat
 (Labill.) Chodat ex Anon.
 (Labill.) Choisy
 (Labill.) Christenh. & Byng
 (Labill.) Connor & Edgar
 (Labill.) Copel.
 (Labill.) Court
 (Labill.) D.Don
 (Labill.) D.L.Jones & M.A.Clem.
 (Labill.) DC.
-(Labill.) DC. x Bedfordia linearis (Labill.) DC.
 (Labill.) Domin
 (Labill.) Don
 (Labill.) Druce
 (Labill.) Drude
 (Labill.) Duby
 (Labill.) Dumort. ex Trevis.
 (Labill.) E.B.Alexeev
@@ -12361,15 +12566,14 @@
 (Labill.) K.A.Sheph.
 (Labill.) Klotzsch
 (Labill.) Knight
 (Labill.) Koidz.
 (Labill.) Kuntze
 (Labill.) Kük.
 (Labill.) Kütz.
-(Labill.) L.A.S.Johnson & B.G.Briggs
 (Labill.) Labill.
 (Labill.) Less.
 (Labill.) Less. ex Benth.
 (Labill.) Lindb. ex Paris
 (Labill.) Maiden & Betche
 (Labill.) Markgr.
 (Labill.) Mart.
@@ -12391,14 +12595,15 @@
 (Labill.) P.Beauv.
 (Labill.) Palla
 (Labill.) Parris
 (Labill.) Paul G.Wilson
 (Labill.) Pax & R.Knuth
 (Labill.) Pedley
 (Labill.) Pers.
+(Labill.) Peter G.Wilson
 (Labill.) Poir.
 (Labill.) R.Br.
 (Labill.) R.Br. ex G.Don
 (Labill.) R.Br. ex P.Beauv.
 (Labill.) R.Br. ex Sm.
 (Labill.) R.J.Bayer
 (Labill.) R.W.Bouman
@@ -12445,36 +12650,37 @@
 (Labill.) Á.Löve
 (Labour.) Britton
 (Labour.) Riccob.
 (Lace) I.C.Nielsen
 (Lace) Maslin, Seigler & Ebinger
 (Lace) Pedley
 (Lack) S.Holzapfel
+(Ladiges & Whiffin) D.Nicolle
 (Lag. & Rodr.) Britton & Rose
 (Lag. & Rodr.) N.P.Taylor
 (Lag. ex Link) Comes
 (Lag.) Bonnier
 (Lag.) Fedde
 (Lag.) H.Wolff
 (Lag.) Keng ex Lazarides
 (Lag.) Kunze
 (Lag.) Nees
 (Lag.) Small
 (Lagerh. & Nordst. ex Wittr.) West & G.S.West
-(Lagerh.) C.W.Dodge & Zeller
 (Lagerh.) Chodat
 (Lagerh.) E.Hegewald
 (Lagerh.) Magnus
 (Lagerh.) Mattox & H.C.Bold
 (Lagerh.) Playfair
 (Lagerh.) Racib.
 (Lagerh.) Schmidle
 (Lagerh.) Teiling
 (Lagerh.) Willi Krieg.
 (Lagerh.) Willi Krieg. & Gerloff
+(Lagerh.) Zeller & C.W.Dodge
 (Lagerst.) Cleve
 (Lagerst.) Playfair
 (Lagerst.) Temp. & Perag.
 (Laharpe) Kirschner
 (Lahm ex Rabenh.) Harm.
 (Lahm) Nyl.
 (Lam. & DC.) Roem. & Schult.
@@ -12533,14 +12739,15 @@
 (Lam.) Hayek
 (Lam.) Hitchc. & Chase
 (Lam.) Hook.f.
 (Lam.) Hook.f. & Thomson
 (Lam.) Husn.
 (Lam.) J.Raynal
 (Lam.) J.V.Lamour.
+(Lam.) Juss. ex Gagnep.
 (Lam.) K.Larsen
 (Lam.) K.Schum.
 (Lam.) Kaulf.
 (Lam.) King
 (Lam.) Koehne
 (Lam.) Kostel.
 (Lam.) Kuhn
@@ -12572,15 +12779,15 @@
 (Lam.) Poelt
 (Lam.) R.Br.
 (Lam.) R.Parker
 (Lam.) Roem. & Schult.
 (Lam.) Roxb.
 (Lam.) Sch.Bip.
 (Lam.) Schltr.
-(Lam.) Schrad. ex DC. & Lam.
+(Lam.) Schrad. ex DC.
 (Lam.) Spreng.
 (Lam.) Stapf
 (Lam.) T.Cooke
 (Lam.) T.Durand & H.Durand
 (Lam.) Taub.
 (Lam.) Thell.
 (Lam.) Trevis.
@@ -12599,38 +12806,41 @@
 (Lamb.) R.Br. ex A.Dietr.
 (Lamy) Knoph, Hertel & Rambold
 (Lamy) Zahlbr.
 (Lander & L.A.S.Johnson) M.P.Simmons
 (Lander & P.J.H.Hurter) K.R.Thiele & E.E.Schill.
 (Lander) G.L.Nesom
 (Lane-Poole) I.C.Nielsen
-(Lange) Gyeln.
+(Langdon) McTaggart & R.G.Shivas
 (Lange-Bert.) Lange-Bert.
 (Lange-Bert.) Levkov
 (Langsd. & Fisch.) Baker
 (Langsd. & Fisch.) Brownlie
 (Langsd. & Fisch.) Christenh.
 (Langsd. & Fisch.) Kuhn
 (Langsd. & Fisch.) Kuntze
 (Langsd. & Fisch.) R.F.Tryon & A.F.Tryon
 (Langsd. & Fisch.) S.B.Andrews
+(Largent & Abell-Davis) Blanco-Dios
+(Largent & Sk.Moore) Blanco-Dios
+(Largent & Sk.Moore) Noordel. & G.M.Gates
+(Largent) Blanco-Dios
 (Lasch) Fayod
 (Lasch) Gillet
 (Lasch) M.M.Moser
 (Lasch) Maas Geest.
 (Lasch) Nitschke
 (Lasch) P.F.Cannon
 (Lasch) P.Kumm.
 (Lasch) Quél.
 (Lasch) Sacc.
 (Lasch) Singer
 (Latz) K.L.Wilson & J.J.Bruhl
 (Laun.) Kuntze
 (Laurer) A.Massal.
-(Laurer) Florke
 (Laurer) Flörke
 (Laurer) Hale
 (Laurer) Hampe
 (Laurer) Hillmann
 (Laurer) J.S.Murray
 (Laurer) Kremp.
 (Laurer) Malme
@@ -12719,15 +12929,14 @@
 (Lehm. ex Miq.) Tate
 (Lehm. ex Miq.) Tiegh.
 (Lehm.) A.Nelson & J.F.Macbr.
 (Lehm.) Asch. & Graebn.
 (Lehm.) B.D.Jacks.
 (Lehm.) B.J.Conn & Henwood
 (Lehm.) Baill.
-(Lehm.) Benedix
 (Lehm.) Benth.
 (Lehm.) Boeckeler
 (Lehm.) Chrtek & Slavikova
 (Lehm.) Conard
 (Lehm.) Craven & R.D.Edwards
 (Lehm.) DC.
 (Lehm.) Domin
@@ -12786,19 +12995,19 @@
 (Lemmerm.) F.E.Drouet & W.A.Daily
 (Lemmerm.) F.Gómez
 (Lemmerm.) F.Gómez, D.Moreira & López-García
 (Lemmerm.) G.M.Sm.
 (Lemmerm.) Geitler
 (Lemmerm.) H.H.Shin, Zhun Li, K-Woo Lee & Matsuoka
 (Lemmerm.) Hollerb.
-(Lemmerm.) Jörg.
+(Lemmerm.) Jørg.
 (Lemmerm.) Kof.
 (Lemmerm.) Kof. & J.R.Michener
 (Lemmerm.) Kof. & Swezy
-(Lemmerm.) Kof. ex Jörg.
+(Lemmerm.) Kof. ex Jørg.
 (Lemmerm.) Komárek
 (Lemmerm.) Komárk.-Legn. & Cronberg
 (Lemmerm.) Lemmerm.
 (Lemmerm.) Paulsen
 (Lemmerm.) Playfair
 (Lemmerm.) Skvortsov
 (Lemmerm.) Van Goor
@@ -12807,41 +13016,39 @@
 (Lemoine ex É.Morren) N.E.Br.
 (Lemoine) D.Testoni & Villamil
 (Lemoine) Lemoine
 (Lemoine) Stapf
 (Lendn.) Peyronel & Dal Vesco
 (Lendn.) Schipper
 (Lenorm. ex Kütz.) Sirodot
+(Lenz) Blanco-Dios
 (Leonh.) Migula
-(Lepr. & Mont.) J.Lloyd
+(Lepr. & Mont.) Lloyd
 (Lesp. & Thevenau) A.Braun ex J.M.Coult & S.Watson
 (Lesq. & James) Renauld & Cardot
 (Less. ex Ledeb.) Schmalh.
 (Less.) A.Gray
 (Less.) Baill.
 (Less.) Beauverd
 (Less.) Benth.
 (Less.) Benth. & Hook.f. ex O.Hoffm.
 (Less.) DC.
-(Less.) F.Muell.
 (Less.) Harv.
 (Less.) Hook.f.
 (Less.) Hutch.
 (Less.) Kitam.
 (Less.) Kuntze
 (Less.) Maiden & Betche
 (Less.) Norl.
 (Less.) Porter
 (Less.) R.M.King & H.Rob.
 (Less.) Sch.Bip.
 (Letell.) E.J.Gilbert
 (Leud.-Fort.) Cleve
 (Leud.-Fortm.) Cleve
-(Lev.) Pat.
-(Lev.) Sacc.
 (Levander) Balech
 (Levander) Carty & El.R.Cox
 (Levander) Kof.
 (Levander) Kof. & Swezy
 (Levander) Moestrup, Hakanen, Gert Hansen, Daugbjerg & M.Ellegaard
 (Levring) Garbary
 (Levring) Huisman
@@ -12902,22 +13109,21 @@
 (Lindb.) Berggr.
 (Lindb.) Broth.
 (Lindb.) Dumort.
 (Lindb.) H.Rob.
 (Lindb.) I.Hagen
 (Lindb.) Limpr.
 (Lindb.) Lindb.
-(Lindb.) Lindb. ex Braithw.
 (Lindb.) Müll.Hal.
 (Lindb.) Schiffn.
-(Lindb.) Schlieph. ex Limpr.
-(Lindb.) Schlieph. ex Schimp.
+(Lindb.) Schimp.
 (Lindeb. ex F.Aresch.) A.Beek
 (Lindeb. ex F.Aresch.) Focke
 (Linden ex André) H.Wendl.
+(Linden) Colletta & V.C.Souza
 (Linden) V.C.Souza
 (Lindenb. & Gottsche ex Nees) Carrington & Pearson
 (Lindenb. & Gottsche ex Nees) Taylor & Hook.f.
 (Lindenb. & Gottsche) Grolle
 (Lindenb. & Gottsche) J.B.Jack & Steph.
 (Lindenb. & Gottsche) J.J.Engel & Xiao L.He
 (Lindenb. & Gottsche) Lacout.
@@ -12981,17 +13187,17 @@
 (Lindl.) Craven & R.D.Edwards
 (Lindl.) D.L.Jones & M.A.Clem.
 (Lindl.) Deb
 (Lindl.) Decne.
 (Lindl.) Diels
 (Lindl.) Dockrill
 (Lindl.) Domin
-(Lindl.) Domin x Iseilema vaginiflorum Domin
 (Lindl.) Druce
 (Lindl.) Duretto & Heslewood
+(Lindl.) E.B.Knox
 (Lindl.) E.M.Benn.
 (Lindl.) E.Wimm.
 (Lindl.) Endl.
 (Lindl.) Endl. ex Pfeiff.
 (Lindl.) Ewart
 (Lindl.) Ewart & Jean White
 (Lindl.) Ewart & O.B.Davies
@@ -13014,45 +13220,37 @@
 (Lindl.) Heads
 (Lindl.) Heine
 (Lindl.) Herb.
 (Lindl.) Hershk.
 (Lindl.) Hochr.
 (Lindl.) Hook.
 (Lindl.) Hook.f.
-(Lindl.) Hook.f. x Thelymitra gregaria D.L.Jones & M.A.Clem.
-(Lindl.) Hook.f. x Thelymitra luteocilium Fitzg.
-(Lindl.) Hook.f. x Thelymitra macrophylla Lindl.
-(Lindl.) Hook.f. x Thelymitra maculata Jeanes
-(Lindl.) Hook.f. x Thelymitra vulgaris Jeanes
 (Lindl.) Hopper
 (Lindl.) Hopper & A.P.Br.
 (Lindl.) Hügel
 (Lindl.) J.M.Black
 (Lindl.) J.R.I.Wood
 (Lindl.) J.W.Green
 (Lindl.) J.W.Grimes
 (Lindl.) Joyce
 (Lindl.) K.D.Hill & L.A.S.Johnson
-(Lindl.) K.D.Hill & L.A.S.Johnson x Corymbia haematoxylon (Maiden) K.D.Hill & L.A.S.Johnson
 (Lindl.) Kakudidi
 (Lindl.) Keighery
 (Lindl.) Kraenzl.
 (Lindl.) Kuntze
 (Lindl.) Kurz
 (Lindl.) L.H.Bailey
 (Lindl.) L.W.Cayzer & Crisp
 (Lindl.) Lazarides
 (Lindl.) Lem.
 (Lindl.) Lewton
 (Lindl.) Lindl.
 (Lindl.) Lodd., G.Lodd. & W.Lodd.
 (Lindl.) M.A.Clem.
 (Lindl.) M.A.Clem. & D.L.Jones
-(Lindl.) M.A.Clem. & D.L.Jones x Dockrillia mortii (F.Muell.) Rauschert
-(Lindl.) M.A.Clem. & D.L.Jones x Dockrillia pugioniformis (A.Cunn.) Rauschert
 (Lindl.) M.F.Fay & Christenh.
 (Lindl.) M.W.Chase, Christenh. & Schuit.
 (Lindl.) Maiden & Betche
 (Lindl.) Meisn.
 (Lindl.) Mildbr.
 (Lindl.) Miq.
 (Lindl.) N.T.Burb.
@@ -13062,14 +13260,15 @@
 (Lindl.) P.Royen
 (Lindl.) P.S.Green
 (Lindl.) Pamp.
 (Lindl.) Paul G.Wilson
 (Lindl.) Pax
 (Lindl.) Pedley
 (Lindl.) Pennell
+(Lindl.) Peter G.Wilson
 (Lindl.) Planch.
 (Lindl.) R.J.Bayer
 (Lindl.) R.S.Rogers
 (Lindl.) Rauschert
 (Lindl.) Rchb.
 (Lindl.) Rchb. ex Pfeiff.
 (Lindl.) Rchb.f.
@@ -13146,46 +13345,50 @@
 (Link) Valdés & H.Scholz
 (Link) Veldkamp
 (Link) Zucc. ex Pfeiff.
 (Link) Á.Löve
 (Linnem.) Arx
 (Liro) H.Scholz & I.Scholz
 (Liro) Padwick & A.Khan
+(Lister & G.Lister) Lister ex E.Jahn
+(Lister) Ing & Nann.-Bremek.
 (Lister) Lister
+(Lister) Meyl.
 (Lister) Nann.-Bremek.
-(Lister) Nann.-Bremek. & Ing
 (Litsch. ex Pilát) Jülich
 (Litsch.) Donk
 (Litsch.) Hjortstam
 (Litsch.) Jülich
 (Lloyd) A.Roy
 (Lloyd) Boedijn
 (Lloyd) C.J.Humphrey & Leus-Palo
-(Lloyd) C.W.Dodge & Zeller
-(Lloyd) Castellano, Trappe & Malajczuk ex Kantvilas & Y.S.Chang
 (Lloyd) Cleland & Cheel
 (Lloyd) Corner
 (Lloyd) D.A.Crawford
 (Lloyd) D.A.Reid
+(Lloyd) Decock, P.K.Buchanan & Ryvarden
 (Lloyd) G.Cunn.
 (Lloyd) G.W.Beaton
 (Lloyd) Ginns
 (Lloyd) Imazeki
+(Lloyd) J.A.Cooper
 (Lloyd) J.E.Wright
 (Lloyd) Lloyd
 (Lloyd) Maas Geest.
 (Lloyd) P.K.Buchanan & Ryvarden
-(Lloyd) P.K.Buchanan, Ryvarden & Decock
 (Lloyd) Pegler
 (Lloyd) Rajchenb.
 (Lloyd) Rick
 (Lloyd) Ryvarden
 (Lloyd) Sacc. & Traverso
 (Lloyd) Sacc. & Trotter
+(Lloyd) Spirin
 (Lloyd) T.Wagner & M.Fisch.
+(Lloyd) Trappe, Castellano & Malajczuk ex Y.S.Chang & Kantvilas
+(Lloyd) Zeller & C.W.Dodge
 (Locq. ex E.Horak) D.A.Reid
 (Lodd. ex Hook.) A.Berger
 (Lodd. ex Lindl.) Munro
 (Lodd.) Domin
 (Lodd.) M.A.Clem. & D.L.Jones
 (Lodd., G.Lodd. & W.Lodd.) Benth.
 (Lodd., G.Lodd. & W.Lodd.) Blume
@@ -13267,14 +13470,16 @@
 (Luehm.) Pedley
 (Luerss.) C.Chr.
 (Luerss.) Christenh.
 (Luerss.) F.M.Bailey
 (Luerss.) Wawra
 (Lumn.) P.Kumm.
 (Luttr.) K.J.Leonard & Suggs
+(Lyne & Crisp) Peter G.Wilson
+(Lyne) Peter G.Wilson
 (Lyngb.) Aresch.
 (Lyngb.) Bréb.
 (Lyngb.) C.Agardh
 (Lyngb.) C.Hoek
 (Lyngb.) Cleve
 (Lyngb.) F.Schmitz
 (Lyngb.) Fr.
@@ -13285,16 +13490,17 @@
 (Lyngb.) Mart.Schmidt
 (Lyngb.) Nägeli
 (Lyngb.) P.C.Silva
 (Lyngb.) P.S.Dixon
 (Lyngb.) Pringsh.
 (Lyngb.) Solier
 (Lyngb.) Woelk.
-(Lynge) Gyeln.
 (Lynge) Hale
+(Læssøe & Spooner) Y.M.Ju, J.D.Rogers & H.M.Hsieh
+(Læssøe, C.A.Pearce & K.D.Hyde) J.D.Rogers, Y.M.Ju & F.San Martín
 (Lév. & Durieu) Seaver
 (Lév.) B.Sutton
 (Lév.) Berk. ex Cooke
 (Lév.) Boidin
 (Lév.) Bondartseva & S.Herrera
 (Lév.) Bres.
 (Lév.) Burds.
@@ -13319,19 +13525,21 @@
 (Lév.) Lév.
 (Lév.) Maire
 (Lév.) Nakasone
 (Lév.) Pat.
 (Lév.) Rajchenb.
 (Lév.) Ryvarden
 (Lév.) Sacc.
+(Lév.) Spirin & Miettinen
 (Lév.) Steyaert
 (Lév.) T.W.May & A.E.Wood
 (Lév.) Teng
 (Lév.) Theiss. & Syd.
 (Lév.) Vassilkov
+(Lév.) Y.C.Dai, Hai J.Li & Vlasák
 (Lév.) Y.M.Ju, J.D.Rogers & H.M.Hsieh
 (Lév.) de Bary
 (Lücking & Barillas) Lücking, Sérus. & Vězda
 (Lücking & Vězda) Lücking
 (Lücking) Hafellner & Kalb
 (Lücking) Lücking
 (Lücking) Lücking, Sérus. & Vězda
@@ -13347,21 +13555,23 @@
 (M.A.Clem. & Hatch) Molloy, D.L.Jones & M.A.Clem.
 (M.A.Clem. & Hatch) Szlach.
 (M.A.Clem. & J.Stewart) Szlach.
 (M.A.Clem.) M.A.Clem. & D.L.Jones
 (M.A.Clem.) Szlach.
 (M.A.Clem., D.L.Jones, B.Gray & J.J.Wood) J.J.Wood
 (M.A.Clem., Matthias & D.L.Jones) Szlach.
+(M.A.Curtis) Manamgoda, L.Cai & K.D.Hyde
 (M.A.Curtis) Murrill
 (M.A.Curtis) Shoemaker
 (M.A.Curtis) Speg.
 (M.A.Curtis) Subram. & B.L.Jain
 (M.A.Lawson) Craib
-(M.B.Ellis & G.W.Beaton) S.Hughes
+(M.A.Salam & P.N.Rao) Subram.
 (M.B.Ellis) J.Y.Uchida & Aragaki
+(M.B.Ellis) Manamgoda, L.Cai & K.D.Hyde
 (M.B.Ellis) Tsuda & Ueyama
 (M.B.Harrison) C.S.Boyer
 (M.B.Harrison) Cleve
 (M.B.Scott) Verdc.
 (M.B.Williams) R.D.Wood
 (M.Bartolome) Pedley
 (M.Bieb. ex Willd.) Franco & Rocha Afonso
@@ -13380,28 +13590,31 @@
 (M.F.Rich) Teiling
 (M.Fleisch.) A.Eddy
 (M.Fleisch.) E.B.Bartram
 (M.Fleisch.) Goffinet & W.R.Buck
 (M.Fleisch.) H.Whittier
 (M.Fleisch.) J.R.Spence & H.P.Ramsay
 (M.Fleisch.) M.Fleisch.
+(M.Fleisch.) Matcham & O'Shea
 (M.Fleisch.) Ochyra
 (M.Fleisch.) Sainsbury
 (M.Fleisch.) W.R.Buck & Vitt
 (M.Gray) J.M.Ward & Breitw.
 (M.Gray) P.S.Short
 (M.Howe) Børgesen
 (M.Howe) De Toni
 (M.Howe) Duff, J.C.Villarreal, Cargill & Renzaglia
 (M.Howe) E.Y.Dawson
 (M.Howe) Kylin
 (M.Howe) Santel.
 (M.Howe) Y.Nakam.
 (M.I.Dawson & Heenan) Hislop, Crayn & Puente-Lel.
+(M.J.Wingf., Crous & W.J.Swart) J.A.Simpson
 (M.Koch ex Tate) Beier & Thulin
+(M.Lange & A.H.Sm.) Vilgalys, Hopple & Jacq.Johnson
 (M.Lebour) A.R.Loebl.
 (M.Lebour) A.R.Loebl. & L.A.Loebl.
 (M.Lebour) Balech
 (M.Lebour) Balech ex Sournia
 (M.Lebour) E.J.F.Wood
 (M.Lebour) F.J.R.Taylor
 (M.Lebour) J.D.Dodge
@@ -13413,28 +13626,29 @@
 (M.O.P.Iyengar & Vimala) Teiling
 (M.Ota) Cif. & Redaelli
 (M.Roem.) Merr.
 (M.Roem.) Miq.
 (M.Rossignol) D.Wall & B.Dale
 (M.Rossignol) Ellegaard, Daugbjerg, Rochon, J.A.Lewis & I.Harding
 (M.Rossignol) Sarjeant
+(M.S.Patil) McTaggart & R.G.Shivas
 (M.S.Patil) Vánky
 (M.Schultze) Sundström
 (M.T.Mathieson) D.L.Jones & M.A.Clem.
 (M.T.Sm., Van der Walt & Johannsen) Kurtzman & Robnett
 (M.Vahl) S.F.Gray
 (M.W.McDonald & Maslin) Pedley
 (M.W.McDonald) Pedley
+(M.W.Mill. & J.S.F.Barker) Kurtzman & Robnett
 (Maasen ex Claussen) L.S.Olive & Spiltoir
 (Mabille) Greuter
 (MacKee) Christenh. & Byng
 (MacKee) McGill.
 (MacLeay ex Lindl.) Brieger
 (MacLeay ex Lindl.) Kuntze
-(Macartney) Ehrenb.
 (Macartney) Kof. & Swezy
 (Mack. & Bush) Bogin
 (Macklin) L.A.S.Johnson
 (Maconochie) Pedley
 (Magnus) Ershad
 (Magnus) Lagerh.
 (Magnus) Papenf.
@@ -13473,17 +13687,19 @@
 (Maiden & Betche) Pedley
 (Maiden & Betche) R.T.Baker
 (Maiden & Betche) Radlk.
 (Maiden & Betche) S.B.Andrews
 (Maiden & Betche) S.T.Blake
 (Maiden & Betche) Sleumer
 (Maiden & Betche) Stapf
+(Maiden & Betche) T.L.Collins
 (Maiden & Betche) Trudgen
 (Maiden & Blakely) Blakely & C.T.White
 (Maiden & Blakely) C.A.Gardner
+(Maiden & Blakely) Crisp & L.G.Cook
 (Maiden & Blakely) J.M.Black
 (Maiden & Blakely) K.D.Hill & L.A.S.Johnson
 (Maiden & Blakely) L.A.S.Johnson
 (Maiden & Blakely) L.A.S.Johnson & Blaxell
 (Maiden & Blakely) L.A.S.Johnson & K.D.Hill
 (Maiden & Blakely) Pedley
 (Maiden & Blakely) S.T.Blake
@@ -13495,78 +13711,77 @@
 (Maiden & R.T.Baker) Kosterm.
 (Maiden & R.T.Baker) Maiden & Betche
 (Maiden & R.T.Baker) Pedley
 (Maiden & R.T.Baker) Steenis
 (Maiden) Blakely
 (Maiden) Brooker
 (Maiden) C.T.White
+(Maiden) Crisp & L.G.Cook
 (Maiden) D.Nicolle
 (Maiden) D.Nicolle & M.E.French
 (Maiden) Ewart
 (Maiden) H.B.Will.
 (Maiden) K.D.Hill & L.A.S.Johnson
-(Maiden) K.D.Hill & L.A.S.Johnson x Corymbia citriodora (Hook.) K.D.Hill & L.A.S.Johnson
-(Maiden) K.D.Hill & L.A.S.Johnson x Corymbia watsoniana (F.Muell.) K.D.Hill & L.A.S.Johnson
 (Maiden) Kessell & C.A.Gardner
 (Maiden) L.A.S.Johnson
 (Maiden) L.A.S.Johnson & Blaxell
 (Maiden) M.A.Clem. & D.L.Jones
 (Maiden) Maiden
 (Maiden) Maiden & Blakely
-(Maiden) Maiden x Eucalyptus robusta Sm.
-(Maiden) Maiden x Eucalyptus viridis R.T.Baker
 (Maiden) Makinson
 (Maiden) Merr. & L.M.Perry
 (Maiden) P.S.Green
 (Maiden) Parra-Os. & Ladiges
 (Maiden) Pedley
-(Maiden) Pedley x Acacia julifera Benth.
 (Maiden) R.S.Cowan & Maslin
 (Maiden) S.T.Blake
 (Maiden) W.Hartley
 (Maiden, Blakely & Simmonds) Ewart
 (Maiden, Blakely & Simmonds) J.B.Kirkp.
+(Mains) B.Shrestha, G.H.Sung & Spatafora
 (Mainx) Fott
 (Maire) Bat. & Cif.
 (Maire) Bertault
-(Maire) Bertault & Malençon
 (Maire) D.A.Sutton
 (Maire) Donk
-(Maire) Maubl. & Konrad
+(Maire) Konrad & Maubl.
+(Maire) Malençon & Bertault
 (Maire) P.D.Orton
 (Maire) Singer
+(Maire) Vizzini & Contu
 (Maire, Weiller & Wilczek) J.T.Howell
 (Makhija & Patw.) Aptroot
 (Makhija & Patw.) R.C.Harris
 (Makino) Kitam.
 (Makino) Moldenke
 (Makino) T.Koyama
 (Makinson & Albr.) Christenh. & Byng
 (Makinson & M.D.Barrett) Christenh. & Byng
 (Makinson & Olde) Christenh. & Byng
 (Makinson) Christenh. & Byng
 (Malcolm & Vězda) R.Sant., Lücking & Sérus.
 (Malcolm & Vězda) Vězda
-(Malençon & Bertault) Kreisel & G.Moreno
-(Malençon & Bertault) Malençon
+(Malloch & Cain) L.W.Hou, L.Cai & Crous
 (Malme) C.W.Dodge
 (Malme) Hafellner & Bellem.
 (Malme) I.Schmitt & Lumbsch
 (Malme) Imshaug
 (Malme) Kalb & Giralt
 (Malme) Marbach
 (Malme) P.M.McCarthy
 (Malme) Runemark
 (Malme) Sheard
 (Malme) Zahlbr.
 (Malta) H.P.Ramsay
 (Mangold) Kraichak, Lücking & Lumbsch
 (Manguin) G.R.Hasle
 (Maniotis) Redhead, Vilgalys & Moncalvo
-(Marasas, P.S.van Wyk & Knox-Dav.) Crous & U.Braun
+(Manjón & G.Moreno) Hjortstam, Manjón & G.Moreno
+(Marcelino & Gouli) Pennycook
+(Marcelino & Gouli) R.G.Shivas & Y.P.Tan
 (Marchal) P.F.Cannon & D.Hawksw.
 (Marignoni) Shoemaker
 (Marignoni) Subram. & B.L.Jain
 (Markgr.) D.J.Middleton
 (Markgr.) Fosberg & Boiteau
 (Markgr.) Markgr.
 (Markgr.) Merr. & L.M.Perry
@@ -13602,30 +13817,31 @@
 (Maslin & Whibley) Pedley
 (Maslin) Maslin
 (Maslin) Pedley
 (Massart) A.R.Loebl.
 (Massee & E.S.Salmon) G.F.Orr, G.R.Ghosh & K.Roy
 (Massee & E.S.Salmon) Kuehn
 (Massee & Rodway) Bougher & Castellano
-(Massee & Rodway) C.W.Dodge
-(Massee & Rodway) C.W.Dodge & Zeller
 (Massee & Rodway) Castellano, Trappe & Claridge
 (Massee & Rodway) G.Cunn.
-(Massee & Rodway) Kantvilas & Y.S.Chang
+(Massee & Rodway) Kuhar, Nouhra & M.E.Sm.
 (Massee & Rodway) Peintner & M.M.Moser
 (Massee & Rodway) Rodway
 (Massee & Rodway) Singer & A.H.Sm.
+(Massee & Rodway) T.Lebel
 (Massee & Rodway) T.Lebel & Castellano
 (Massee & Rodway) T.W.May
+(Massee & Rodway) Y.S.Chang & Kantvilas
+(Massee & Rodway) Zeller & C.W.Dodge
 (Massee) A.H.Sm.
 (Massee) A.M.Young
 (Massee) Arx
 (Massee) Bougher & Castellano
-(Massee) C.W.Dodge & Zeller
 (Massee) Corner
+(Massee) Crous
 (Massee) D.A.Reid
 (Massee) Dennis
 (Massee) Donk
 (Massee) E.Horak
 (Massee) E.L.Stewart & Trappe
 (Massee) F.M.Bailey
 (Massee) G.Cunn.
@@ -13638,118 +13854,131 @@
 (Massee) Jülich
 (Massee) Kuntze
 (Massee) Ladó
 (Massee) Lloyd
 (Massee) Massee
 (Massee) McAlpine
 (Massee) McNabb
+(Massee) McTaggart & R.G.Shivas
 (Massee) Monks & A.K.Mills
 (Massee) P.Roberts
 (Massee) Peintner & M.M.Moser
 (Massee) R.H.Petersen
 (Massee) Rappaz
 (Massee) Rifai
 (Massee) Rodway
 (Massee) S.Hughes
 (Massee) Sacc.
 (Massee) Sacc. & D.Sacc.
 (Massee) Singer & A.H.Sm.
 (Massee) Spooner
+(Massee) T.Lebel
 (Massee) Torrend
 (Massee) Vánky
 (Massee) Watling
 (Massee) Zeller
+(Massee) Zeller & C.W.Dodge
 (Mast.) D.P.Banks & Clemesha
 (Mast.) Dockrill
 (Mast.) Domin
 (Mast.) F.Muell.
 (Mast.) J.Schust.
 (Mast.) Kuntze
+(Matheny & Bougher) Matheny & Esteve-Rav.
+(Matheny, Bougher & G.M.Gates) Matheny & Esteve-Rav.
 (Mathias & Constance) K.F.Chung
 (Matr.) W.Gams
+(Matsush.) B.Sutton & P.M.Kirk
 (Matsush.) Matsush.
-(Matsush.) P.M.Kirk & B.Sutton
 (Matsush.) R.F.Castañeda & Heredia
 (Matsush.) R.F.Castañeda, Saikawa & Gené
 (Matsush.) S.Hughes
 (Matsush.) Samuels
 (Matsush.) Subram.
 (Matsush.) Subram. & Sudha
-(Mattf.) Anderb.
 (Mattf.) Swenson & K.Bremer
 (Matv.) L.Ş.Péterfi & Momeu
 (Maxim.) H.L.Li
 (Maxim.) Momiy.
 (Maxim.) Steenis
 (Maxim.) Trautv.
 (Maxon) M.D.Turner & R.A.White
 (Mayer) R.M.Patrick
 (Mazza) V.J.Chapm. & P.G.Parkinson
 (McAlpine & Tepper) Henn.
+(McAlpine ex Hansf.) H.J.Swart
 (McAlpine) Bat. & Cif.
+(McAlpine) Berndt
 (McAlpine) Boerema
 (McAlpine) Burds.
+(McAlpine) C.A.Pearce & K.D.Hyde
 (McAlpine) Cif.
 (McAlpine) Constant.
 (McAlpine) Corner
+(McAlpine) Crous
 (McAlpine) Cummins & Y.Hirats.
 (McAlpine) Dietel
 (McAlpine) G.W.Wilson
 (McAlpine) H.J.Swart
-(McAlpine) Hansf. ex P.H.B.Talbot & Warcup
+(McAlpine) Hansf. ex Warcup & P.H.B.Talbot
 (McAlpine) J.L.Crane & Schokn.
 (McAlpine) J.Walker
 (McAlpine) J.Walker & S.M.Francis
 (McAlpine) Jülich
-(McAlpine) K.D.Hyde & C.A.Pearce
 (McAlpine) L.Guo
 (McAlpine) Liro
 (McAlpine) M.Scholler & Aime
 (McAlpine) McAlpine
+(McAlpine) McTaggart & R.G.Shivas
 (McAlpine) Morgan-Jones & J.F.White
 (McAlpine) Nag Raj
 (McAlpine) Pegler & T.W.K.Young
 (McAlpine) Priest
-(McAlpine) R.G.Shivas & Vánky
 (McAlpine) R.Y.Zheng & G.Q.Chen
 (McAlpine) Sacc. & D.Sacc.
 (McAlpine) Shoemaker
 (McAlpine) Singer
 (McAlpine) Subram. & K.Ramakr.
-(McAlpine) Swart
 (McAlpine) Syd.
 (McAlpine) Syd. & Höhn.
+(McAlpine) T.Bose
 (McAlpine) Thirum. & Neerg.
 (McAlpine) Tomilin
 (McAlpine) U.Braun & S.Takam.
 (McAlpine) Vanev
 (McAlpine) Vánky
+(McAlpine) Vánky & R.G.Shivas
 (McAlpine) W.B.Cooke
 (McAlpine) Wakef.
 (McAlpine) Weese
 (McAlpine) Wollenw.
 (McAulay & Brett) B.M.Potts
 (McClain) M.B.Ellis
 (McGill.) Christenh. & Byng
 (McGill.) E.M.Benn.
 (McGill.) Keighery
 (McGill.) Makinson
 (McGill.) McGill.
 (McGill.) Olde
 (McGill.) Olde & Marriott
-(McKenzie & Vánky) Vánky
+(McKenzie & D.Matthews) Rossman & K.D.Hyde
+(McLennan & Ducker) A.J.Chen, Houbraken & Samson
 (McLennan & F.Halsey) Caillet & Moyne
 (McLennan & F.Halsey) Rifai
 (McNabb) D.Stubbe
+(McNabb) J.A.Cooper
 (McNabb) Singer
 (McNabb) Wolfe
+(McTaggart & R.G.Shivas) Massee
+(McTaggart & R.G.Shivas) McTaggart, R.G.Shivas & Begerow
 (Me.Lemoine) Afonso-Carr.
 (Me.Lemoine) Littler ex W.H.Adey, R.A.Towns. & Boykins
 (Me.Lemoine) Me.Lemoine
 (Me.Lemoine) Woelk., Y.M.Chamb. & P.C.Silva
+(Me.Lemoine) Zaneveld & R.B.Sanford
 (Medik.) Dandy & Exell
 (Medik.) L.H.Bailey
 (Medik.) Moldenke
 (Medik.) N.E.Br.
 (Medik.) Roxb.
 (Meeuwen) H.Ohashi & K.Ohashi
 (Meinsh.) Ohwi
@@ -13821,36 +14050,33 @@
 (Menegh.) Nägeli
 (Menegh.) Rabenh.
 (Menegh.) Trevis.
 (Menegh.) Woelk.
 (Meney & Pate) B.G.Briggs
 (Menzies ex Hook.) Mitt.
 (Merat) Lainz
-(Mercado & Hol.-Jech.) Nawawi & Kuthub.
 (Mereschk.) Hust.
 (Merr. & L.M.Perry) B.J.Conn
 (Merr. & L.M.Perry) Craven & Biffin
 (Merr. & L.M.Perry) H.Turner
 (Merr. & L.M.Perry) Harms
 (Merr. & L.M.Perry) Mabb.
 (Merr. & L.M.Perry) R.W.Ham
 (Merr. & L.M.Perry) S.T.Reynolds & R.J.F.Hend.
 (Merr. & L.M.Perry) T.G.Hartley
-(Merr.) A.R.Bean
 (Merr.) Airy Shaw
 (Merr.) Barlow
 (Merr.) C.Monod
 (Merr.) Corner
 (Merr.) Hosok.
 (Merr.) J.W.Dawson
 (Merr.) Jansen
 (Merr.) L.Junell
 (Merr.) Moldenke
 (Merr.) Pedley
-(Merr.) Rye & Trudgen
 (Merr.) S.T.Blake
 (Merr.) Stapf
 (Merr.) T.Koyama
 (Mert. & W.D.J.Koch) Parl.
 (Mert. ex C.Agardh) Kütz.
 (Mert. ex Gomont) Anagn. & Komárek
 (Mert. ex Hornem.) Kütz.
@@ -13896,17 +14122,17 @@
 (Meunier) Kof. & Swezy
 (Meunier) Parke & J.D.Dodge
 (Meyen & Flot.) Aptroot
 (Meyen & Flot.) Müll.Arg.
 (Meyen & Flot.) Vain.
 (Meyen & Flot.) Zahlbr.
 (Meyen) Leonh.
-(Meyers) E.B.G.Jones & K.L.Pang
-(Meyers) E.B.G.Jones, Yusoff & S.T.Moss
+(Meyers) K.L.Pang & E.B.G.Jones
 (Meyers) Kohlm.
+(Meyers) Yusoff, E.B.G.Jones & S.T.Moss
 (Meyl.) Nann.-Bremek.
 (Mez) Bernacci & Jung-Mend.
 (Mez) Ewart
 (Mez) Jackes
 (Mez) K.Larsen & C.M.Hu
 (Mez) Pilg.
 (Mhaskar & V.G.Rao) K.D.Hyde
@@ -13952,15 +14178,15 @@
 (Mildbr.) Carlquist
 (Mildbr.) F.L.Erickson & J.H.Willis
 (Mildbr.) Lowrie, A.H.Burb. & Kenneally
 (Milde) De Not.
 (Milde) Hässel
 (Milde) J.J.Amann
 (Milde) Mull.Frib. ex Prosk.
-(Miles) B.Sutton & N.Pons
+(Miles) N.Pons & B.Sutton
 (Mill. ex Münchh.) Bean
 (Mill.) A.P.Ham.
 (Mill.) A.W.Hill
 (Mill.) Asch.
 (Mill.) Bartel
 (Mill.) Benth.
 (Mill.) Blake
@@ -13998,21 +14224,20 @@
 (Mill.) S.F.Blake
 (Mill.) Schinz & Thell.
 (Mill.) Small
 (Mill.) Stearn
 (Mill.) Stokes
 (Mill.) Swingle
 (Mill.) Thell.
-(Mill.) U.Manns & Anderb.
 (Mill.) Urb.
 (Mill.) Wedd.
 (Mill.) Weigel
 (Mill.) de Laub.
 (Millsp.) Dressler
-(Minter & B.C.Zhang) Castellano, Trappe & Malajczuk
+(Minter & B.C.Zhang) Trappe, Castellano & Malajczuk
 (Miq.) A.Cunn. ex Miq.
 (Miq.) A.DC.
 (Miq.) A.P.Davis
 (Miq.) A.S.Mitch.
 (Miq.) Airy Shaw & Turrill
 (Miq.) Bakh.
 (Miq.) Benth.
@@ -14029,15 +14254,14 @@
 (Miq.) E.Fourn.
 (Miq.) Engl.
 (Miq.) F.Muell.
 (Miq.) F.Muell. ex Maiden
 (Miq.) F.Muell. ex Miq.
 (Miq.) Geesink
 (Miq.) H.Huber
-(Miq.) H.Huber x Peperomia tetraphylla Hook. & Arn.
 (Miq.) Harms
 (Miq.) Holzmeyer & Hauenschild
 (Miq.) Hook.f.
 (Miq.) J.E.Piggin & J.J.Bruhl
 (Miq.) J.Kern
 (Miq.) J.Kost.
 (Miq.) Jabl.
@@ -14081,28 +14305,30 @@
 (Mitt. ex Steph.) J.J.Engel & R.M.Schust.
 (Mitt. ex Steph.) R.M.Schust.
 (Mitt.) A.Evans ex Reimers
 (Mitt.) A.Jaeger
 (Mitt.) Abeyw.
 (Mitt.) B.C.Tan, W.B.Schofield & H.P.Ramsay
 (Mitt.) Bastow
+(Mitt.) Bedn.-Ochyra & Ochyra
 (Mitt.) Benedix
 (Mitt.) Benedix ex Mizut.
 (Mitt.) Berggr.
 (Mitt.) Besch.
 (Mitt.) Besch. & C.Massal.
 (Mitt.) Broth.
 (Mitt.) Broth. & Watts
 (Mitt.) Broth. ex Paris
 (Mitt.) Catches.
 (Mitt.) Churchill
 (Mitt.) Dixon
 (Mitt.) E.W.Jones
 (Mitt.) F.Muell.
-(Mitt.) Fransen
+(Mitt.) Fedosov, Jan Kučera & M. Stech
+(Mitt.) Fife
 (Mitt.) Fransén
 (Mitt.) G.Roth
 (Mitt.) Gottsche
 (Mitt.) Grolle
 (Mitt.) H.Rob.
 (Mitt.) Hampe
 (Mitt.) Hilp.
@@ -14116,45 +14342,49 @@
 (Mitt.) J.J.Engel & R.M.Schust.
 (Mitt.) J.R.Spence
 (Mitt.) J.R.Spence & H.P.Ramsay
 (Mitt.) Kindb.
 (Mitt.) Klazenga
 (Mitt.) Kuntze
 (Mitt.) Kuwah.
+(Mitt.) L.Y. Pei, Y. Jia & Y.F. Wang
 (Mitt.) Lindb.
 (Mitt.) M.A.M.Renner
 (Mitt.) M.Fleisch.
 (Mitt.) Maschke
 (Mitt.) Mitt.
 (Mitt.) Mitt. ex E.A.Hodgs. & Allison
 (Mitt.) Mizut.
 (Mitt.) Müll.Hal.
 (Mitt.) Müll.Hal. & Broth.
+(Mitt.) N.N.Yu & Y.Jia
 (Mitt.) Ochyra
 (Mitt.) Ochyra & Bedn.-Ochyra
 (Mitt.) Ochyra & Matteri
 (Mitt.) Paris
 (Mitt.) Paris ex Catches.
 (Mitt.) R.H.Zander
 (Mitt.) R.M.Schust.
 (Mitt.) Reichardt
 (Mitt.) Renauld
 (Mitt.) S.D.F.Patzak, M.A.M.Renner & Heinrichs
 (Mitt.) S.D.F.Patzak, M.A.M.Renner, Schäf.-Verw. & Heinrichs
+(Mitt.) S.Olsson, Enroth & D.Quandt
 (Mitt.) Schiffn.
 (Mitt.) Schimp.
 (Mitt.) Snider
 (Mitt.) Spruce ex Schiffn.
 (Mitt.) Steph.
 (Mitt.) Tilden
 (Mitt.) Touw
 (Mitt.) Touw & Falter-van den Haak
 (Mitt.) Vitt
 (Mitt.) Warnst.
 (Mitt.) Watts & Whitel.
+(Miyake & Komin. ex M.Oda) Gert Hansen & Moestrup
 (Mizut.) Grolle
 (Moench) Asch.
 (Moench) C.B.Clarke
 (Moench) DC.
 (Moench) Garcke
 (Moench) Griseb.
 (Moench) Scheygr.
@@ -14176,14 +14406,15 @@
 (Molyneux & Stajsic) Christenh. & Byng
 (Molyneux & Stajsic) Molyneux & Stajsic
 (Molyneux) Christenh. & Byng
 (Mont. & Berk.) Berk.
 (Mont. & Berk.) Cleland & Cheel
 (Mont. & Berk.) Cooke
 (Mont. & Berk.) D.A.Reid
+(Mont. & Berk.) Decock & Yombiy.
 (Mont. & Berk.) Henn.
 (Mont. & Berk.) Massee
 (Mont. & Berk.) Pat.
 (Mont. & Berk.) Ryvarden
 (Mont. & Berk.) Speg.
 (Mont. & Berk.) Torrend
 (Mont. & Bosch) Aptroot & Lücking
@@ -14195,30 +14426,27 @@
 (Mont. & Bosch) Kirika, Divakar & Lumbsch
 (Mont. & Bosch) M.Nakan. & Kashiw.
 (Mont. & Bosch) Müll.Arg.
 (Mont. & Bosch) Nyl.
 (Mont. & Bosch) Staiger
 (Mont. & Bosch) Zahlbr.
 (Mont. & Bosch.) Kalb, Staiger & Elix
-(Mont. & Durieu ex Sacc.) Sacc.
-(Mont. & Durieu) Donk
-(Mont. & Durieu) E.Fisch.
-(Mont. & Durieu) Sacc.
 (Mont. & Fr.) J.Schröt.
-(Mont. & Lepr.) Lloyd
 (Mont. & Millardet) De Toni
 (Mont. ex Gomont) Anagn. & Komárek
-(Mont. ex Müll.Berol.) Henssen
 (Mont. ex Steph.) Jovet-Ast
+(Mont.) A.David & Rajchenb.
+(Mont.) A.Evans
 (Mont.) A.Gepp & E.Gepp
 (Mont.) A.Jaeger
 (Mont.) A.Massal.
 (Mont.) Arv. & D.J.Galloway
 (Mont.) B.C.Tan
 (Mont.) B.M.Xia & I.A.Abbott
+(Mont.) Bedn.-Ochyra & Ochyra
 (Mont.) Berthold
 (Mont.) Boidin
 (Mont.) Bondartseva & S.Herrera
 (Mont.) Brauner
 (Mont.) Bres.
 (Mont.) Broth.
 (Mont.) Brusse
@@ -14248,15 +14476,14 @@
 (Mont.) Hafellner & Magnes
 (Mont.) Hale
 (Mont.) Hamel
 (Mont.) Harv.
 (Mont.) Henn.
 (Mont.) Hjortstam & Ryvarden
 (Mont.) Hook.f. & Taylor
-(Mont.) Howe
 (Mont.) Hue
 (Mont.) Hässel & Solari
 (Mont.) I.A.Abbott
 (Mont.) J.Agardh
 (Mont.) J.B.Jack & Steph.
 (Mont.) J.D.Rogers & Y.M.Ju
 (Mont.) J.H.Haines & Dumont
@@ -14287,51 +14514,50 @@
 (Mont.) Parnmen, Lücking & Lumbsch
 (Mont.) Pat.
 (Mont.) Pat. & Lagerh.
 (Mont.) Pilát
 (Mont.) Pujals
 (Mont.) R.C.Harris
 (Mont.) R.F.Castañeda & Heredia
+(Mont.) R.H.Petersen
 (Mont.) R.M.Schust.
 (Mont.) Rajchenb.
-(Mont.) Rajchenb. & A.David
 (Mont.) Reimers
 (Mont.) Riddle
 (Mont.) Ryvarden
 (Mont.) Räsänen
 (Mont.) S.Hughes
 (Mont.) S.Olsson, Enroth, Huttunen & D.Quandt
 (Mont.) Sacc.
 (Mont.) Samp.
 (Mont.) Sauv.
 (Mont.) Singer
 (Mont.) Staiger
 (Mont.) Staiger, Kalb & Lücking
 (Mont.) Steph.
-(Mont.) Steph. ex A.Evans
 (Mont.) Sull.
 (Mont.) T.W.May & A.E.Wood
 (Mont.) Trevis.
 (Mont.) Tuck.
 (Mont.) Tul. & C.Tul.
 (Mont.) V.J.Chapm.
 (Mont.) Vain.
 (Mont.) Vickers
 (Mont.) Vězda
 (Mont.) W.R.Buck
 (Mont.) Weber Bosse
 (Mont.) Wittr.
+(Mont.) Y.C.Dai & L.W.Zhou
 (Mont.) Zahlbr.
 (Mont.) Zanardini
 (Montagu) F.Stein
 (Montagu) Will.
 (Montrouz.) B.L.Burtt
 (Montrouz.) Guillaumin
 (Montrouz.) Guillaumin & Beauvis.
-(Montrouz.) Guillaumin x Pterocaulon sphacelatum (Labill.) F.Muell.
 (Moon) Alston
 (Moore ex Ralfs) R.M.Crawford
 (Moq. ex Benth.) F.Muell.
 (Moq.) Aellen
 (Moq.) Benl
 (Moq.) Benth.
 (Moq.) D.Dietr.
@@ -14346,41 +14572,45 @@
 (Moq.) Kuntze
 (Moq.) Moq.
 (Moq.) Moss
 (Moq.) Murr
 (Moq.) Paul G.Wilson
 (Moq.) R.H.Anderson
 (Moq.) S.Fuentes & Borsch
+(Moq.) Sieber ex Moq.
+(Moq.) Sieber ex Vorosch.
 (Moq.) Tate
 (Moq.) Ulbr.
 (Moq.) Volkens
-(Moq.) Vorosch.
+(Mordue) Maharachch., K.D.Hyde & Crous
 (Moretti) D.Löve
 (Morgan) Dring
 (Morgan) Hollós
 (Morgan) Höhn.
 (Morgan) Torrend
+(Morgan-Jones & W.Gams) C.W.Bacon & Schardl
 (Morgan-Jones & W.Gams) Glenn, C.W.Bacon & Hanlin
 (Morgan-Jones) Carris & Glawe
 (Moris & De Not.) P.Crouan & H.Crouan
 (Moris) Chater
 (Morrison) Carolin ex Hershk.
 (Morrison) Hershk.
 (Morrison) P.Syd. & Syd.
 (Morrison) Pedley
 (Motyka) G.N.Stevens
 (Motyka) Swinscow & Krog
-(Moug.) De Not. & Ces.
-(Mrak & Recca) Van der Walt
+(Moug.) Ces. & De Not.
 (Mudie) Link
 (Mudie) Sweet
 (Muehlenpf.) Backeb.
 (Muehlenpf.) Engelm.
 (Muhl.) Tuck.
 (Mull.Frib.) H.Buch
+(Mundk. & Thirum.) McTaggart & R.G.Shivas
+(Mundk. & Thirum.) Vánky
 (Mundk.) Vánky
 (Munir) B.J.Conn & Henwood
 (Munir) Bramley
 (Munir) N.Streiber & B.J.Conn
 (Munir) Rye
 (Munro) F.Muell.
 (Murb.) Á.Löve
@@ -14391,18 +14621,19 @@
 (Murray ex G.Forst.) R.Br.
 (Murray) Copel.
 (Murray) Kuntze
 (Murray) Kurata
 (Murray) Nakai
 (Murray) Schindl.
 (Murrill) A.H.Sm. & Thiers
-(Murrill) A.M.Gottlieb, J.E.Wright & Moncalvo.
+(Murrill) A.M.Gottlieb, J.E.Wright & Moncalvo
 (Murrill) Aberdeen
 (Murrill) Dennis
 (Murrill) G.Cunn.
+(Murrill) J.S.Oliveira
 (Murrill) Lloyd
 (Murrill) Murrill
 (Murrill) Pat.
 (Murrill) Pegler
 (Murrill) Ryvarden
 (Murrill) Sacc. & D.Sacc.
 (Murrill) Sacc. & Trotter
@@ -14421,15 +14652,14 @@
 (Møller) Witkowski
 (Müll.Arg) Kantvilas
 (Müll.Arg) Kantvilas & Lücking
 (Müll.Arg.) A.C.Sm.
 (Müll.Arg.) A.Crespo, Divakar & Elix
 (Müll.Arg.) A.W.Archer
 (Müll.Arg.) Abbayes
-(Müll.Arg.) Abbayes ex Frey
 (Müll.Arg.) Ahti
 (Müll.Arg.) Ahti & DePriest
 (Müll.Arg.) Airy Shaw
 (Müll.Arg.) Allem
 (Müll.Arg.) Aptroot
 (Müll.Arg.) Aptroot & Lücking
 (Müll.Arg.) Arup, Frödén & Søchting
@@ -14452,29 +14682,27 @@
 (Müll.Arg.) D.J.Galloway & P.M.Jørg.
 (Müll.Arg.) Darb.
 (Müll.Arg.) Degel.
 (Müll.Arg.) Domin
 (Müll.Arg.) Egea
 (Müll.Arg.) Egea & Torrente
 (Müll.Arg.) Elix
-(Müll.Arg.) Elix & Hale
 (Müll.Arg.) Elix & J.Johnst.
 (Müll.Arg.) Elix, S.Y.Kondr. & Kärnefelt
 (Müll.Arg.) Essl.
 (Müll.Arg.) Etayo & Diederich
 (Müll.Arg.) F.M.Bailey
 (Müll.Arg.) F.Muell.
 (Müll.Arg.) F.Schill.
 (Müll.Arg.) F.Wilson
 (Müll.Arg.) Filson
 (Müll.Arg.) Fosberg
 (Müll.Arg.) Frisch
 (Müll.Arg.) Frisch & Kalb
 (Müll.Arg.) Fryday
-(Müll.Arg.) G.Schneid.
 (Müll.Arg.) Gotth.Schneid.
 (Müll.Arg.) Grube
 (Müll.Arg.) Grüning
 (Müll.Arg.) Gyeln.
 (Müll.Arg.) H.Eichler
 (Müll.Arg.) H.Magn.
 (Müll.Arg.) H.Mayrhofer
@@ -14522,15 +14750,14 @@
 (Müll.Arg.) Mangold & Lumbsch
 (Müll.Arg.) Mangold, Elix & Lumbsch
 (Müll.Arg.) Mangold, Lumbsch & Kalb
 (Müll.Arg.) Marbach
 (Müll.Arg.) Motyka
 (Müll.Arg.) Müll.Arg.
 (Müll.Arg.) Nagarkar & Hale
-(Müll.Arg.) P.James
 (Müll.Arg.) P.M.Jørg. & D.J.Galloway
 (Müll.Arg.) P.M.McCarthy
 (Müll.Arg.) Papong & Lücking
 (Müll.Arg.) Parnmen & Lumbsch
 (Müll.Arg.) Passo & Calvelo
 (Müll.Arg.) Patw. & Makhija
 (Müll.Arg.) Pax
@@ -14569,54 +14796,57 @@
 (Müll.Arg.) Vězda & Kantvilas
 (Müll.Arg.) W.L.Culb.
 (Müll.Arg.) W.Martin
 (Müll.Arg.) Zahlbr.
 (Müll.Arg.) van den Boom & Mayrhofer
 (Müll.Berol.) B.Øllg.
 (Müll.Hal. & Broth.) I.G.Stone
+(Müll.Hal. & Broth.) Pursell
 (Müll.Hal. & Hampe) A.Jaeger
 (Müll.Hal. & Hampe) Broth.
 (Müll.Hal. & Hampe) Catches.
 (Müll.Hal. & Hampe) Hampe
+(Müll.Hal. & Hampe) Matcham & O'Shea
 (Müll.Hal. & Hampe) Mitt.
 (Müll.Hal. & Hampe) Mitt. ex F.Muell.
 (Müll.Hal. & Hampe) Paris
-(Müll.Hal. ex Broth.) Müll.Hal.
 (Müll.Hal.) A.Jaeger
 (Müll.Hal.) Ando
 (Müll.Hal.) B.C.Tan
 (Müll.Hal.) B.C.Tan, W.B.Schofield & H.P.Ramsay
+(Müll.Hal.) Bedn.-Ochyra & Ochyra
 (Müll.Hal.) Besch.
 (Müll.Hal.) Bosch & Sande Lac.
 (Müll.Hal.) Broth.
 (Müll.Hal.) Broth. ex Paris
 (Müll.Hal.) Broth. ex Watts & Whitel.
 (Müll.Hal.) Cardot
 (Müll.Hal.) Dixon
 (Müll.Hal.) Dozy
 (Müll.Hal.) During
 (Müll.Hal.) Dusén
 (Müll.Hal.) F.M.Bailey
 (Müll.Hal.) F.Muell.
-(Müll.Hal.) Fife
 (Müll.Hal.) G.Roth
 (Müll.Hal.) Grout
 (Müll.Hal.) H.A.Mill. & D.R.Sm.
 (Müll.Hal.) H.K.Nowak
 (Müll.Hal.) H.Rob.
 (Müll.Hal.) Hampe
 (Müll.Hal.) Hampe ex Lindb.
 (Müll.Hal.) Hilp.
+(Müll.Hal.) Holyoak & N.Pedersen
 (Müll.Hal.) Hook.f. & Wilson
 (Müll.Hal.) I.G.Stone
 (Müll.Hal.) I.G.Stone & G.A.M.Scott
 (Müll.Hal.) J.-P.Frahm
 (Müll.Hal.) J.Guerra & Cano
 (Müll.Hal.) J.R.Spence
 (Müll.Hal.) J.R.Spence & H.P.Ramsay
+(Müll.Hal.) Jan Kučera & Ignatov
 (Müll.Hal.) Kindb.
 (Müll.Hal.) Kuntze
 (Müll.Hal.) L.R.Stark
 (Müll.Hal.) Lindb.
 (Müll.Hal.) Lorentz
 (Müll.Hal.) M.Fleisch.
 (Müll.Hal.) M.Fleisch. ex Broth.
@@ -14627,17 +14857,19 @@
 (Müll.Hal.) Mitt. ex Touw
 (Müll.Hal.) Müll.Hal.
 (Müll.Hal.) Müll.Hal. & Broth.
 (Müll.Hal.) Müll.Hal. ex M.Fleisch.
 (Müll.Hal.) N.E.Bell, A.E.Newton & D.Quandt
 (Müll.Hal.) N.G.Mill. & Manuel
 (Müll.Hal.) Ochyra
+(Müll.Hal.) Ochyra & Żarnowiec
 (Müll.Hal.) P.C.Chen
 (Müll.Hal.) P.Sollman
 (Müll.Hal.) Paris
+(Müll.Hal.) Pursell
 (Müll.Hal.) R.H.Zander
 (Müll.Hal.) R.S.Chopra & S.S.Kumar
 (Müll.Hal.) Reichardt
 (Müll.Hal.) Renauld
 (Müll.Hal.) Rodway
 (Müll.Hal.) S.H.Lin
 (Müll.Hal.) S.Olsson, Enroth & D.Quandt
@@ -14668,14 +14900,15 @@
 (N.G.Marchant) Chrtek & Slavikova
 (N.G.Marchant) Lowrie
 (N.G.Walsh & Albr.) Paul G.Wilson
 (N.G.Walsh & Coates) K.L.McDougall & Millott
 (N.G.Walsh) A.M.Humphreys & H.P.Linder
 (N.G.Walsh) H.P.Linder
 (N.G.Walsh) J.M.Ward & Breitw.
+(N.G.Walsh) P.M.Peterson, Romasch. & Soreng
 (N.Hallé) D.L.Jones & M.A.Clem.
 (N.Hallé) M.A.Clem. & D.L.Jones
 (N.L.Gardner) Anagn. & Komárek
 (N.L.Gardner) G.De Toni
 (N.Peters) Balech
 (N.Snow & B.K.Simon) P.M.Peterson & N.Snow
 (N.Snow) P.M.Peterson & N.Snow
@@ -14687,23 +14920,26 @@
 (N.T.Burb.) P.Horton
 (N.T.Burb.) S.W.L.Jacobs
 (N.T.Burb.) W.M.Curtis
 (N.T.Burb.) de Salas & Schmidt-Leb.
 (Naccari) Rabenh.
 (Nadeaud) Ebihara & K.Iwats.
 (Nadeaud) Tindale
+(Nag Raj) Crous
+(Nag Raj) P.A.Barber & Crous
 (Nagai) Perest.
+(Nakagiri & Tokura) E.Azevedo, P.Correia & M.F.Caeiro
 (Nann.) Stockdale
 (Nann.) Weitzman, McGinnis, A.A.Padhye & Ajello
 (Nann.-Bremek. & D.W.Mitch.) D.W.Mitch.
 (Nann.-Bremek. & Y.Yamam.) Ladó
 (Nann.-Bremek. & Y.Yamam.) Y.Yamam.
 (Nann.-Bremek.) Nann.-Bremek.
 (Nannf.) Conant
-(Nannf.) Crous, W.Gams & L.Mostert
+(Nannf.) L.Mostert, W.Gams & Crous
 (Nannf.) S.Hughes
 (Nash) Roberty
 (Naudin) F.Muell.
 (Naudin) Greb.
 (Naudin) Heiser & E.E.Schill.
 (Naudin) J.B.Kirkp.
 (Naudin) Maiden
@@ -14734,17 +14970,17 @@
 (Nees & Flot.) Hale
 (Nees & Hornsch.) Hampe
 (Nees & Hornsch.) Huebener
 (Nees & Hornsch.) Jur.
 (Nees & Hornsch.) Müll.Hal.
 (Nees & Hornsch.) Schimp.
 (Nees & Mart.) Maréchal & Baudet
-(Nees & Meyen ex Nees) Hance
 (Nees & Meyen ex Wight) C.B.Clarke
 (Nees & Meyen) C.E.Hubb.
+(Nees & Meyen) Hance
 (Nees & Mont.) Cooke
 (Nees & Mont.) Imazeki
 (Nees & Mont.) Nees & Mont. ex Gottsche, Lindenb. & Nees
 (Nees & Mont.) Schiffn.
 (Nees & T.Nees) Merr.
 (Nees ex Endl.) Henrard
 (Nees ex Hampe) L.T.Ellis
@@ -14841,41 +15077,41 @@
 (Nees) McClure ex Soderstr.
 (Nees) Melville
 (Nees) Miq.
 (Nees) Mitt.
 (Nees) Mitt. ex Gottsche
 (Nees) Mont.
 (Nees) Moq.
-(Nees) Müll.Hal.
 (Nees) Nees
 (Nees) Nees & Mont.
 (Nees) Nees ex Domin
 (Nees) Orchard
 (Nees) Ostenf.
+(Nees) P.M.Peterson, Romasch. & Soreng
 (Nees) Paris
 (Nees) Paul G.Wilson
 (Nees) Pax
 (Nees) Pilg.
 (Nees) Pilát
 (Nees) Quél.
 (Nees) R.L.Barrett & J.J.Bruhl
 (Nees) R.L.Barrett & K.L.Wilson
 (Nees) R.M.Barker
 (Nees) R.M.Schust.
 (Nees) R.M.Schust. ex Vana & D.G.Long
+(Nees) Reeder
 (Nees) Renvoize
 (Nees) S.D.F.Patzak, M.A.M.Renner, Schäf.-Verw. & Heinrichs
 (Nees) S.Fuentes & Borsch
 (Nees) S.Hatt.
 (Nees) S.T.Blake
 (Nees) S.W.L.Jacobs
 (Nees) S.W.L.Jacobs & J.Everett
 (Nees) Schiffn.
 (Nees) Schindl.
-(Nees) Sivasith., Websdane, K.W.Dixon & Meney
 (Nees) Spach
 (Nees) Stapf
 (Nees) Stapf & C.E.Hubb.
 (Nees) Steph.
 (Nees) Steph. & Watts
 (Nees) Steud.
 (Nees) Stieber
@@ -14886,14 +15122,15 @@
 (Nees) V.A.W.Graham
 (Nees) Valck.Sur.
 (Nees) Verd.
 (Nees) Vickery
 (Nees) Voss
 (Nees) Vánky
 (Nees) Walp.
+(Nees) Websdane, Sivasith., K.W.Dixon & Meney
 (Nees) Á.Löve
 (Nees) Á.Löve & Connor
 (Newnham, Ladiges & Whiffin) Rule
 (Nicholls & Goadby) D.L.Jones & M.A.Clem.
 (Nicholls) A.S.George
 (Nicholls) Blackmore & Clemesha
 (Nicholls) Clemesha & Dockrill
@@ -14963,15 +15200,15 @@
 (Nordst.) W.West & G.S.West
 (Nordst.) West & G.S.West
 (Nordst.) Willi Krieg.
 (Nordst.) Willi Krieg. & Gerloff
 (Nordst.) Zaneveld
 (Nordstedt & Loefgren) Teiling
 (Norman ex Ralfs) Hust.
-(Nowak. ex A.Batko) Hennebert & Remaud.
+(Nowak. ex A.Batko) Remaud. & Hennebert
 (Nowak.) J.Schröt.
 (Nutt. ex Torr. & A.Gray) Britton & Rose
 (Nutt. ex Torr. & A.Gray) L.Rico
 (Nutt.) Auquier
 (Nutt.) Benth.
 (Nutt.) Cronquist
 (Nutt.) Cronquist ex Cuatrec.
@@ -14990,30 +15227,28 @@
 (Nutt.) Torr. ex A.Gray
 (Nygaard) Cronberg & Komárek
 (Nygaard) Komárek
 (Nyl) Kalb & Giralt
 (Nyl. ex C.Bab. & Mitt.) Hertel
 (Nyl. ex C.Bab. & Mitt.) Kantvilas & Elix
 (Nyl. ex C.Bab. & Mitt.) Kuntze
-(Nyl. ex Cromb.) Elix
 (Nyl. ex Cromb.) Essl.
 (Nyl. ex Cromb.) Fryday
 (Nyl. ex Cromb.) Hale
 (Nyl. ex Cromb.) Müll.Arg.
 (Nyl. ex Cromb.) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (Nyl. ex Hue) Flagey
 (Nyl. ex Kremp.) Elix
 (Nyl. ex Kremp.) Müll.Arg.
 (Nyl. ex Kremp.) O.Blanco, A.Crespo, Elix, D.Hawksw. & Lumbsch
 (Nyl. ex Kremp.) Zahlbr.
 (Nyl. ex Malbr.) A.Nordin, S.Savic & Tibell
 (Nyl. ex Malbr.) Arnold
 (Nyl. ex Müll.Arg.) Aptroot & Lücking
 (Nyl. ex Müll.Arg.) D.Hawksw.
-(Nyl. ex Stizenb.) Nyl.
 (Nyl. ex Vain.) A.Schmidt
 (Nyl. ex Vain.) Aptroot
 (Nyl. ex Vain.) Lojka
 (Nyl.) A.Crespo, Divakar & Elix
 (Nyl.) A.Crespo, Ferencova & Divakar
 (Nyl.) A.L.Sm.
 (Nyl.) A.W.Archer
@@ -15071,37 +15306,35 @@
 (Nyl.) Hedl.
 (Nyl.) Hellb.
 (Nyl.) Henssen
 (Nyl.) Hepp
 (Nyl.) Hertel
 (Nyl.) Hertel & Hafellner
 (Nyl.) Hertel & V.Wirth
-(Nyl.) Hillmann
 (Nyl.) Hue
 (Nyl.) I.M.Lamb
 (Nyl.) Imshaug & Brodo
 (Nyl.) Imshaug ex Yoshim.
 (Nyl.) J.Steiner
 (Nyl.) Jatta
 (Nyl.) K.P.Singh
 (Nyl.) Kalb
-(Nyl.) Kanouse ex Korf, C.S.Ramamurthi & L.R.Batra
+(Nyl.) Kanouse ex C.S.Ramamurthi, Korf & L.R.Batra
 (Nyl.) Kantvilas & Coppins
 (Nyl.) Kantvilas & Grube
 (Nyl.) Keissl.
 (Nyl.) Kickx
 (Nyl.) Kirika, Divakar & Lumbsch
 (Nyl.) Knoph & Hertel
 (Nyl.) Knoph & Leuckert
 (Nyl.) Kohlm. & E.Kohlm.
 (Nyl.) Kremp.
 (Nyl.) Krog
 (Nyl.) Krog & Swinscow
 (Nyl.) Kurok.
-(Nyl.) Leight.
 (Nyl.) Lendemer & R.C.Harris
 (Nyl.) Lettau
 (Nyl.) Lindsay
 (Nyl.) Llano
 (Nyl.) Lumbsch
 (Nyl.) Lücking, M.P.Nelsen & Aptroot
 (Nyl.) Lücking, R.Miranda & Kalb
@@ -15125,16 +15358,14 @@
 (Nyl.) Pusswald
 (Nyl.) R.C.Harris
 (Nyl.) R.Sant.
 (Nyl.) R.Sant. & Hafellner
 (Nyl.) R.Sant. ex Kantvilas
 (Nyl.) Rambold & Hertel
 (Nyl.) Rambold & Triebel
-(Nyl.) Rasanen
-(Nyl.) Rass.
 (Nyl.) Redinger
 (Nyl.) Rivas Plata, Lücking & Lumbsch
 (Nyl.) Robbins ex A.Evans
 (Nyl.) Räsänen
 (Nyl.) S.Y.Kondr., Kärnefelt, Elix, A.Thell, J.Kim, M.-H.Jeong, N.N.Yu, A.S.Kondr. & Hur
 (Nyl.) Sandst.
 (Nyl.) Sipman
@@ -15194,15 +15425,14 @@
 (O'Meara) Hust.
 (O'Meara) I.V.Makarova & V.A.Nikolajev
 (O.Berg) Burret
 (O.Deg.) O.Deg. & I.Deg.
 (O.E.Erikss.) Diederich & Aptroot
 (O.E.Imhof) Lemmerm.
 (O.E.Imhof) Playfair
-(O.F.Mull. : Fr.) Pers.
 (O.F.Müll. ex Vahl) Kütz.
 (O.F.Müll.) Bory
 (O.F.Müll.) C.Agardh
 (O.F.Müll.) Dujard.
 (O.F.Müll.) Dumort.
 (O.F.Müll.) Ehrenb.
 (O.F.Müll.) F.Gómez, D.Moreira & López-García
@@ -15240,41 +15470,37 @@
 (O.Schwarz) Chippend.
 (O.Schwarz) Danser
 (O.Schwarz) Pax & K.Hoffm.
 (O.Schwarz) R.L.Barrett
 (O.Schwarz) Rupp
 (O.Schwarz) S.T.Reynolds & R.J.F.Hend.
 (O.Schwarz) W.R.Barker
-(O.Zacharias) F.Gómez
 (Obbens & J.G.West) Hershk.
 (Obbens & L.P.Hancock) Hershk.
 (Obbens) Hershk.
 (Oberw.) P.Roberts
 (Oberw.) Wojewoda
 (Ochyra) Ochyra
 (Oeder) Borbás
 (Oeder) De Not.
 (Oeder) Onsberg
 (Oeder) Vain.
 (Oerst.) Kuntze
 (Ohlsson) Tsch.-Woess & Poelt
 (Ohlsson) Wedin
 (Ohwi & Yabuno) Tzvelev
-(Ohwi ex Veldkamp) H.P.Linder
 (Ohwi) Eck-Borsb.
 (Ohwi) Nelmes
 (Ohwi) Ohwi
 (Ohwi) Ohwi ex Jansen
 (Ohwi) P.M.Peterson
 (Ohwi) R.W.Haines & Lye
 (Ohwi) Reeder
 (Ohwi) T.Koyama
-(Ohwi) Veldkamp
-(Okamura & Nishikawa) F.Gómez
-(Okamura & Nishikawa) Jörg.
+(Okamura & Nishikawa) Jørg.
 (Okamura & Nishikawa) Kof.
 (Okamura) Balech
 (Okamura) Børgesen
 (Okamura) C.F.Chang & B.M.Xia
 (Okamura) J.Schiller
 (Okamura) Levring
 (Okamura) P.C.Silva
@@ -15282,19 +15508,20 @@
 (Okamura) R.J.King & Puttock
 (Okamura) Segawa
 (Okamura) Setch. & N.L.Gardner
 (Okamura) T.Yoshida & M.Yoshida
 (Olde & Marriott) Christenh. & Byng
 (Olde & Marriott) I.M.Turner
 (Olde & Marriott) Makinson
+(Olde & Marriott) Olde
 (Olde & Molyneux) Christenh. & Byng
 (Olde) Christenh. & Byng
-(Oldfield & F.Muell. ex F.Muell.) Domin
-(Oldfield & F.Muell. ex F.Muell.) F.Muell.
-(Oldfield & F.Muell. ex F.Muell.) Geerinck
+(Oldfield & F.Muell.) Domin
+(Oldfield & F.Muell.) F.Muell.
+(Oldfield & F.Muell.) Geerinck
 (Oldfield & F.Muell.) Kuntze
 (Oliv. ex Benth.) Philipson
 (Oliv.) Burkill
 (Oliv.) C.Moore
 (Oliv.) F.M.Bailey
 (Oliv.) Feuillet
 (Oliv.) Kamienski
@@ -15314,62 +15541,63 @@
 (Ortega) O.Hoffm. ex Hicken
 (Osbeck) Hale & Ahti
 (Osbeck) J.Kern
 (Osbeck) Kosterm.
 (Osbeck) Mabb.
 (Osbeck) Merr.
 (Osbeck) Quél.
+(Osbeck) Redhead
 (Osbeck) Singer
 (Ostenf. & E.J.Schmidt) Böhm
 (Ostenf. & E.J.Schmidt) F.Gómez
 (Ostenf. & E.J.Schmidt) F.Gómez, D.Moreira & López-García
 (Ostenf. & E.J.Schmidt) Hallegr. & Huisman
 (Ostenf. & E.J.Schmidt) Schröd.
 (Ostenf.) A.J.Alverson, S.H.Kang & E.C.Ther.
 (Ostenf.) Aston
 (Ostenf.) Balech
-(Ostenf.) F.Gómez
 (Ostenf.) G.W.Carr & P.F.Horsfall
 (Ostenf.) Gran
 (Ostenf.) Hasle
 (Ostenf.) Hopper & A.P.Br.
 (Ostenf.) J.D.Dodge
-(Ostenf.) Jörg.
+(Ostenf.) Jørg.
 (Ostenf.) Ostenf.
 (Ostenf.) Paulsen
 (Ostenf.) Szlach.
 (Ostenf.) Toelken
 (Otto & A.Dietr.) Heynh.
 (Otto & A.Dietr.) Kuntze
 (Otto & A.Dietr.) L.A.S.Johnson
 (Otto & A.Dietr.) Schauer
 (Oudem. & Beij.) Vánky
 (Oudem.) B.Sutton
 (Oudem.) C.H.Dickinson
 (Oudem.) Davis
 (Oudem.) M.B.Ellis
 (Oudem.) Seifert & Samson
-(Oudem.) U.Braun, W.Gams & W.M.Pitt
 (Oudem.) Vuill.
 (Oudem.) W.Gams
+(Oudem.) W.M.Pitt, W.Gams & U.Braun
 (Oudem.) de Bary
 (Overeem) Corner
 (Overeem) R.H.Petersen
+(Overton) Jaklitsch & Voglmayr
 (O’Meara) Tempère & H.Perag.
+(P.A.Barber & Crous) Z.W.de Beer, T.A.Duong & M.J.Wingf.
 (P.A.Dang.) Domin
 (P.A.Dang.) Karling
 (P.A.Dang.) Scherff.
 (P.A.Dang.) Senn
 (P.A.Tandy) McGee
 (P.Beauv. ex Mirb.) Baker
 (P.Beauv. ex Roem. & Schult.) Hook.f.
 (P.Beauv. ex T.Lestib.) Boeckeler
 (P.Beauv. ex T.Lestib.) Endl.
 (P.Beauv. ex T.Lestib.) Ohwi
-(P.Beauv.) Arn.
 (P.Beauv.) Baker
 (P.Beauv.) Benth.
 (P.Beauv.) Benth. & Hook.f.
 (P.Beauv.) Boeckeler
 (P.Beauv.) Brid.
 (P.Beauv.) C.B.Clarke
 (P.Beauv.) Desv.
@@ -15387,29 +15615,34 @@
 (P.Beauv.) Peterm.
 (P.Beauv.) Rchb.
 (P.Beauv.) Ryvarden
 (P.Beauv.) Spreng.
 (P.Beauv.) Steud.
 (P.Beauv.) T.Moore
 (P.Beauv.) Touw
+(P.Beauv.) Trevis.
 (P.Beauv.) Trin.
 (P.Beauv.) Veldkamp
 (P.Beauv.) Wijk & Margad.
 (P.Beauv.) Wilson
+(P.Beauv.) Zmitr., Wasser & Ezhov
 (P.Browne) DC.
 (P.Browne) F.Muell.
 (P.Browne) Kuntze
 (P.C.Reid) Ellegaard, Daugbjerg, Rochon, J.A.Lewis & I.Harding
-(P.Crouan & H.Crouan) Arx & E.Müll.
+(P.Crouan & H.Crouan) 
 (P.Crouan & H.Crouan) Batters
+(P.Crouan & H.Crouan) Benkert & T.Schumach.
 (P.Crouan & H.Crouan) Boud.
 (P.Crouan & H.Crouan) Boudour.
 (P.Crouan & H.Crouan) Brumm.
 (P.Crouan & H.Crouan) D.P.Cheney & P.W.Gabrielson
+(P.Crouan & H.Crouan) Döbbeler
 (P.Crouan & H.Crouan) E.J.Faye & Masuda
+(P.Crouan & H.Crouan) E.Müll. & Arx
 (P.Crouan & H.Crouan) Falkenb.
 (P.Crouan & H.Crouan) Foslie
 (P.Crouan & H.Crouan) Gomont
 (P.Crouan & H.Crouan) Hamel
 (P.Crouan & H.Crouan) Har.
 (P.Crouan & H.Crouan) Heydr.
 (P.Crouan & H.Crouan) J.Agardh
@@ -15418,28 +15651,26 @@
 (P.Crouan & H.Crouan) Kimbr.
 (P.Crouan & H.Crouan) Knoepffler-Péguy
 (P.Crouan & H.Crouan) Kohlm.
 (P.Crouan & H.Crouan) L'Hardy-Halos
 (P.Crouan & H.Crouan) Me.Lemoine
 (P.Crouan & H.Crouan) Sacc.
 (P.Crouan & H.Crouan) Sacc. & Traverso
-(P.Crouan & H.Crouan) T.Schumach. & Benkert
 (P.Crouan & H.Crouan) W.H.Adey & P.J.Adey
 (P.Crouan & H.Crouan) Weber Bosse
 (P.Crouan & H.Crouan) Woelk., Y.M.Chamb. & P.C.Silva
 (P.Crouan & H.Crouan) Y.M.Chamb.
 (P.D.Orton) Boertm.
 (P.D.Orton) P.D.Orton
 (P.D.Orton) Redhead
 (P.G.Neish) Duretto & Heslewood
 (P.G.Richt.) Elenkin
 (P.G.Richt.) Hollerb.
 (P.G.Richt.) Playfair
 (P.G.Richt.) West & G.S.West
-(P.H.B.Talbot & Warcup) Liberta
 (P.H.B.Talbot) Hjortstam & Ryvarden
 (P.H.B.Talbot) Stalpers & T.F.Andersen
 (P.Henn.) Lücking
 (P.Horton) M.W.Chase & Christenh.
 (P.Horton) Symon & Lepschi
 (P.I.Forst.) D.J.Middleton
 (P.I.Forst.) Liede
@@ -15473,37 +15704,40 @@
 (P.Karst.) Gilb. & Ryvarden
 (P.Karst.) Höhn. & Litsch.
 (P.Karst.) J.Erikss.
 (P.Karst.) J.Erikss. & Ryvarden
 (P.Karst.) J.Erikss. & Å.Strid
 (P.Karst.) J.Moravec
 (P.Karst.) Jülich
+(P.Karst.) K.H.Larss.
 (P.Karst.) Liberta
 (P.Karst.) M.M.Moser
 (P.Karst.) Niemelä
 (P.Karst.) P.A.Lemke
 (P.Karst.) P.Karst.
-(P.Karst.) P.Syd. & Sacc.
 (P.Karst.) Parmasto
 (P.Karst.) Quél.
 (P.Karst.) Redhead, Vilgalys & Moncalvo
 (P.Karst.) Rick
 (P.Karst.) Ricken
 (P.Karst.) Rodway & Cleland
 (P.Karst.) Ryvarden
 (P.Karst.) S.E.Carp.
 (P.Karst.) S.M.Berch
 (P.Karst.) Sacc.
+(P.Karst.) Sacc. & P.Syd.
 (P.Karst.) Sogonov
 (P.Karst.) Speg.
 (P.Karst.) Velen.
 (P.Karst.) Y.Otani & Kanzawa
 (P.Kumm.) Gillet
 (P.Kumm.) M.M.Moser
 (P.Kumm.) Singer
+(P.Kumm.) Vizzini, G.Moreno & P.Alvarado
+(P.Kumm.) Örstadius & E.Larss.
 (P.L.J.Dang.) Kornmann & Sahling
 (P.Lewis & Summerh.) Lepschi
 (P.Lundell) Bourr.
 (P.Lundell) Hansg.
 (P.Lundell) J.Roy & Bisset
 (P.Lundell) Lagerh.
 (P.Lundell) Nordst.
@@ -15514,15 +15748,14 @@
 (P.Lundell) West & G.S.West
 (P.M.Jørg. & D.J.Galloway) P.M.Jørg.
 (P.M.Jørg. & D.J.Galloway) P.M.Jørg. & H.L.Andersen
 (P.M.Jørg.) P.M.Jørg.
 (P.M.Kirk) R.F.Castañeda & Heredia
 (P.M.Kirk) Sivan. & B.Sutton
 (P.M.McCarthy & Kantvilas) Aptroot
-(P.M.McCarthy & Kantvilas) Baloch & Lucking
 (P.M.McCarthy & Kantvilas) Baloch & Lücking
 (P.M.McCarthy & Kantvilas) P.M.McCarthy
 (P.M.McCarthy) Aptroot
 (P.M.McCarthy) Gueidan
 (P.M.McCarthy) Hafellner & Kalb
 (P.M.McCarthy) K.Knudsen & Lendemer
 (P.M.McCarthy) Lücking
@@ -15532,41 +15765,38 @@
 (P.M.Wells & R.S.Hill) R.S.Hill & R.Paull
 (P.Micheli ex Fr.) Cleland & Cheel
 (P.Micheli) Coker & Couch
 (P.Micheli) Pers.
 (P.Morris & J.H.Willis) Anderb.
 (P.Morris) Connor & Edgar
 (P.Morris) Veldkamp
-(P.N.Rao & M.A.Salam) Subram.
 (P.Parm.) Orchard
 (P.Petit) Tsarenko
 (P.Royen) Aubrév.
 (P.Royen) Baehni
 (P.Royen) Jessup
-(P.Royen) P.I.Forst.
 (P.Royen) R.M.Sm.
 (P.Royen) Swenson
 (P.Royen) Swenson, Bartish & Munzinger
 (P.Royen) T.G.Hartley
+(P.S.Catches. & T.Lebel) T.Lebel & T.W.May
 (P.S.Green) A.R.Bean
 (P.S.Green) G.L.Nesom
 (P.S.Green) Jackes
 (P.S.Green) P.I.Forst. & R.J.F.Hend.
 (P.S.Green) P.S.Green
 (P.S.Short) P.S.Short
 (P.S.Short) R.L.Barrett
-(P.Syd. & Sacc.) McAlpine
-(P.Syd. & Sacc.) Shear
-(P.Syd. & Sacc.) Singer
-(P.Syd. & Sacc.) Wolfe
+(P.S.van Wyk, Marasas & Knox-Dav.) Crous & U.Braun
 (P.Willemet) Ames
 (P.Willemet) Merr.
 (P.Willemet) Schott
+(P.Wong & A.M.Stirling) Khemmuk, Geering & R.G.Shivas
+(P.Wong & M.L.Dickinson) Khemmuk, Geering & R.G.Shivas
 (Paine) Wiersema & Hellq.
-(Pall. : Pers.) Kreisel
 (Pall. ex Willd.) C.A.Mey.
 (Pall. ex Willd.) DC.
 (Pall.) DC.
 (Pall.) Fr.
 (Pall.) Kreisel
 (Pall.) Kuntze
 (Pall.) Pers.
@@ -15574,28 +15804,26 @@
 (Pall.) Sims
 (Palla) Kük. ex Merr.
 (Pancher ex Brongn. & Gris) Burret
 (Pant.) Hust.
 (Pant.) R.Ross
 (Pant.) Åke Berg
 (Pantocsek) Cleve
-(Pantocsek) L.Crosby & E.J.F.Wood
+(Pantocsek) L.H.Crosby & E.J.F.Wood
+(Pančić ex A.Kern.) Greuter
 (Pappe ex Hook.) Planch.
-(Pappe ex Hook.) Planch. x Crocosmia pottsii (W.R.McNab ex Baker) N.E.Br.
-(Paris & Broth.) W.R.Buck & Ireland
 (Paris) A.Jaeger
 (Paris) B.C.Tan, W.B.Schofield & H.P.Ramsay
 (Paris) Broth.
 (Paris) Paris
 (Paris) Watts
 (Parke & D.Ballant.) A.R.Loebl.
 (Parkinson) Fosberg
 (Parl.) Benth.
 (Parl.) F.M.Bailey
-(Parl.) F.M.Bailey - Callitris glaucophylla Joy Thomps. & L.A.S.Johnson
 (Parl.) F.Muell.
 (Parl.) Goldblatt
 (Parl.) Grossh.
 (Parl.) Kuntze
 (Parl.) Maiden
 (Parl.) Nevski
 (Parl.) Roberty
@@ -15604,70 +15832,69 @@
 (Parm. ex Pfeiff.) Riccob.
 (Parmasto) Chamuris
 (Parmasto) J.Erikss. & Ryvarden
 (Parn.) Druce
 (Parris) Christenh.
 (Parris) Gasper & Salino
 (Parris) Parris
-(Parris) Parris - Doodia caudata (Cav.) R.Br.
-(Parris) Parris x Doodia linearis J.Sm.
 (Pascher & Jahoda) Gerloff & H.Ettl
 (Pascher) P.C.Silva
+(Pascoe & Crous) X.L.Fan & Crous
 (Pass.) Ainsw. & Sampson
-(Pass.) Begerow, Oberw., R.Bauer & A.Nagler
 (Pass.) Jenkins
 (Pass.) K.J.Leonard & Suggs
 (Pass.) Karling
 (Pass.) Kazn. & Siemaszko
 (Pass.) Magnus
-(Pat. & Bres.) Corner
+(Pass.) R.Bauer, Begerow, A.Nagler & Oberw.
 (Pat. & C.F.Baker) E.Horak
 (Pat. & Gaillard) Corner
 (Pat. & Har.) Cummins
-(Pat. & Har.) Mains
 (Pat. & Har.) Sathe.
 (Pat. & Har.) Thirum.
-(Pat. & Har.) Vánky
 (Pat. & Lagerh.) Karling
 (Pat.) Arx
 (Pat.) Bres.
 (Pat.) Cleland & Cheel
 (Pat.) D.P.Rogers
 (Pat.) E.J.Gilbert
-(Pat.) J.-E.Gilbert
+(Pat.) Griffon & Maubl.
 (Pat.) J.E.Lange
 (Pat.) K.D.Hyde & J.Fröhl.
 (Pat.) Lloyd
-(Pat.) Maubl. & Griffon
+(Pat.) McTaggart & R.G.Shivas
 (Pat.) Murrill
 (Pat.) Pat.
 (Pat.) Pegler
 (Pat.) Petr.
 (Pat.) Rea
+(Pat.) Redhead, Vilgalys & Hopple
 (Pat.) Sacc.
 (Pat.) Sacc. & D.Sacc.
 (Pat.) Sacc. & Trotter
 (Pat.) T.Wagner & M.Fisch.
 (Pat.) Trappe, Lumyong, P.Lumyong, Sanmee & Zhu L.Yang
 (Pat.) Vánky
 (Pate & Meney) B.G.Briggs & L.A.S.Johnson
 (Paton) Paton
+(Patricia McGee & Pascoe) Crous
 (Patw. & C.Kulk.) Mangold
 (Patw. & Nagarkar) Kraichak, Lücking & Lumbsch
 (Paul G.Wilson) Bayly
 (Paul G.Wilson) Duretto & Heslewood
 (Paul G.Wilson) I.Telford & J.J.Bruhl
 (Paul G.Wilson) Iamonico & Mosyakin
 (Paul G.Wilson) K.A.Sheph. & Paul G.Wilson
 (Paul G.Wilson) Mosyakin & Clemants
 (Paul G.Wilson) P.I.Forst.
 (Paul G.Wilson) Paul G.Wilson
 (Paul G.Wilson) Paul G.Wilson & K.A.Sheph.
 (Paul G.Wilson) Piirainen & G.Kadereit
 (Paul G.Wilson) S.Fuentes & Borsch
+(Paul G.Wilson) T.L.Collins
 (Paul G.Wilson) Wege
 (Paul.) Fr.
 (Paulet ex Vittad.) Bertill.
 (Paulet) Fr.
 (Paulsen) A.R.Loebl.
 (Paulsen) Balech
 (Paulsen) Balech & L.O.Soares
@@ -15676,72 +15903,78 @@
 (Paulsen) J.Schiller
 (Paulsen) K.A.Sheph. & Paul G.Wilson
 (Paulsen) M.Lebour
 (Paulsen) Meunier
 (Paulsen) Paul G.Wilson
 (Paulsen) Paulsen
 (Pavgi & Mundk.) Vánky
-(Pavgi) R.Bauer & M.Piepenbr.
+(Pavgi) M.Piepenbr. & R.Bauer
 (Pavill.) Balech
 (Pavill.) Elbr.
 (Pavill.) F.Gómez
 (Pavill.) F.Gómez, D.Moreira & López-García
 (Pavill.) F.J.R.Taylor
 (Pavill.) Hallegr.
 (Pavill.) J.Schiller
 (Pavill.) L.S.Tai & Skogsb.
+(Pavlic, T.I.Burgess & M.J.Wingf.) A.J.L.Phillips & A.Alves
 (Pax & K.Hoffm.) Airy Shaw
 (Pax & K.Hoffm.) P.S.Green
 (Pax) Bruyns
 (Pax) Mattf.
 (Paxton) Benth.
 (Paxton) Daveau
 (Paxton) Lewton
 (Paxton) Paul G.Wilson
 (Peck) A.H.Sm.
 (Peck) A.H.Sm. & Singer
 (Peck) Corner
 (Peck) E.Horak
-(Peck) G.L.Barron & Thorn
 (Peck) Gillet
 (Peck) Ginns
 (Peck) Heinem. & Rammeloo
 (Peck) Hongo
+(Peck) J.S.Oliveira
 (Peck) Jülich
 (Peck) Kanouse
 (Peck) Kauffman
 (Peck) Kreisel & Dring
 (Peck) Kuntze
 (Peck) Lloyd
 (Peck) M.C.Tulloch
+(Peck) McTaggart & R.G.Shivas
 (Peck) Morgan
 (Peck) Murrill
 (Peck) Nag Raj
 (Peck) Nannf.
 (Peck) Peck
 (Peck) Quadr.
+(Peck) R.H.Petersen
+(Peck) Redhead
 (Peck) Redhead, Vilgalys & Moncalvo
 (Peck) Sacc.
 (Peck) Schild
 (Peck) Seaver
 (Peck) Singer
+(Peck) Thorn & G.L.Barron
 (Peck) V.S.White
 (Peck) Watling
 (Peck) Y.Yamam.
 (Pedley & P.I.Forst.) Pedley
 (Pedley) H.Ohashi & K.Ohashi
 (Pedley) Hislop, Crayn & Puente-Lel.
 (Pedley) Kodela
 (Pedley) Orchard
 (Pedley) Pedley
 (Pedley) Quinn
 (Pedley) R.Clark & Gagnon
 (Pedley) R.S.Cowan & Maslin
 (Pedley) Tindale & Kodela
 (Pegg & Alcorn) H.H.Ho & S.C.Jong
+(Pegg & Alcorn) R.Benn. & Thines
 (Pegler) T.Wagner & M.Fisch.
 (Peglion) Kurtzman
 (Penard) Carty
 (Penard) Lemmerm.
 (Penard) Playfair
 (Pennycook & Samuels) Crous, Slippers & A.J.L.Phillips
 (Penz. & Sacc.) J.H.Mill.
@@ -15755,31 +15988,21 @@
 (Perag. & Herib.) Hust.
 (Perag. & Hérib.) M.Voigt
 (Perag. & Hérib.) R.M.Patrick
 (Perag.) A.Mann
 (Perag.) E.J.F.Wood
 (Perkins) A.C.Sm.
 (Perr.) C.B.Rob.
-(Pers. : Fr.) Bon
-(Pers. : Fr.) Fr.
-(Pers. : Fr.) Gillet
-(Pers. : Fr.) Gray
 (Pers. : Fr.) H.E.Bigelow
-(Pers. : Fr.) Maire
-(Pers. : Fr.) P.Kumm.
-(Pers. : Fr.) Pers.
-(Pers. : Fr.) Quel.
 (Pers. ex J.F.Gmel.) Cooke
 (Pers. ex J.F.Gmel.) Fr.
 (Pers. ex J.F.Gmel.) J.Schröt.
 (Pers. ex J.F.Gmel.) Pers.
 (Pers. ex J.F.Gmel.) Ryvarden
-(Pers. ex Lev.) Burds. & O.K.Mill.
-(Pers. ex Lev.) Singer
-(Pers. ex Lév.) O.K.Mill. & Burds.
+(Pers. ex Lév.) Burds. & O.K.Mill.
 (Pers. ex Lév.) Singer
 (Pers. ex Nyl.) Hafellner
 (Pers. ex Nyl.) Körb.
 (Pers. ex Nyl.) Vain.
 (Pers. ex Schleich.) Kuntze
 (Pers.) A.L.Sm.
 (Pers.) A.L.Welden
@@ -15790,24 +16013,23 @@
 (Pers.) Antonín, Halling & Noordel.
 (Pers.) Aptroot
 (Pers.) Arnould
 (Pers.) B.L.Burtt & R.M.Sm.
 (Pers.) Bacle ex DC.
 (Pers.) Baill.
 (Pers.) Balb.
-(Pers.) Balb. x Acacia paradoxa DC.
 (Pers.) Banker
 (Pers.) Baral
 (Pers.) Benth.
 (Pers.) Berk.
 (Pers.) Bernicchia
-(Pers.) Bertault & Malençon
 (Pers.) Berthier
 (Pers.) Boidin
 (Pers.) Bon
+(Pers.) Bondartsev & Singer
 (Pers.) Bondartsev ex Parmasto
 (Pers.) Bonord.
 (Pers.) Boud.
 (Pers.) Bourdot & Galzin
 (Pers.) Bref.
 (Pers.) Bres.
 (Pers.) Bridge & Spooner
@@ -15819,87 +16041,92 @@
 (Pers.) Chevall.
 (Pers.) Cleland & Cheel
 (Pers.) Cooke
 (Pers.) Corner
 (Pers.) D.A.Reid
 (Pers.) D.G.Burch
 (Pers.) DC.
-(Pers.) DC. & Lam.
 (Pers.) De Not.
 (Pers.) Dennis
 (Pers.) DiCosmo, Peredo & Minter
 (Pers.) Dietel
 (Pers.) Ditmar
 (Pers.) Donk
 (Pers.) Doty
-(Pers.) E.Langer & Vesterh.
 (Pers.) F.Muell.
 (Pers.) F.Muell. ex Benth.
 (Pers.) F.Wilson
+(Pers.) F.Wu, Jia J.Chen & Y.C.Dai
 (Pers.) Fayod
 (Pers.) Fiasson & Niemelä
 (Pers.) Fr.
 (Pers.) Fuckel
 (Pers.) Fuckel ex Sacc.
 (Pers.) G.Cunn.
 (Pers.) Gilb. & Ryvarden
 (Pers.) Gillet
 (Pers.) Ginns
 (Pers.) Ginns & M.N.L.Lefebvre
+(Pers.) Gminder
 (Pers.) Gray
 (Pers.) Greene
 (Pers.) Grev.
 (Pers.) Grove
 (Pers.) H.E.Bigelow
 (Pers.) Hack.
 (Pers.) Hafellner & Bellem.
 (Pers.) Hallenb.
 (Pers.) Hjortstam & Ryvarden
 (Pers.) Hoffmanns.
+(Pers.) Hustad, A.N.Mill., Dentinger & P.F.Cannon
 (Pers.) Höhn. & Litsch.
 (Pers.) J.E.Lange
 (Pers.) J.Erikss.
 (Pers.) J.G.Kühn
 (Pers.) J.Kickx f.
 (Pers.) J.M.Black
 (Pers.) J.Presl & C.Presl
 (Pers.) J.S.Furtado
 (Pers.) J.Schröt.
+(Pers.) Jaklitsch, W.Gams & Voglmayr
 (Pers.) Jatta
 (Pers.) Joss.
 (Pers.) Justo
 (Pers.) Jülich
 (Pers.) K.H.Larss.
 (Pers.) K.Schum.
 (Pers.) K.Wells
+(Pers.) Konrad & Maubl.
 (Pers.) Korf
 (Pers.) Kotl. & Pouzar
 (Pers.) Kreisel
 (Pers.) Krog
 (Pers.) Kunth
 (Pers.) Kuntze
 (Pers.) Körb.
 (Pers.) Kühner
+(Pers.) Kühner & Lamoure ex Redhead
 (Pers.) Kühner & Romagn. ex P.D.Orton
 (Pers.) L.L.Kenn.
 (Pers.) Ladó
 (Pers.) Lagerh.
+(Pers.) Lam. & DC.
 (Pers.) Lambotte
+(Pers.) Langer & Vesterh.
 (Pers.) Lentz
 (Pers.) Liberta
 (Pers.) Link
 (Pers.) Lloyd
-(Pers.) Lutzoni, Redhead, Moncalvo & Vilgalys
 (Pers.) Lév.
 (Pers.) M.M.Moser
 (Pers.) M.P.Christ.
 (Pers.) Magnus
 (Pers.) Maire
+(Pers.) Malençon & Bertault
 (Pers.) Massee
-(Pers.) Maubl. & Konrad
 (Pers.) Melderis
 (Pers.) Merr.
 (Pers.) Mirb. ex Endl.
 (Pers.) Mont.
 (Pers.) Morgan
 (Pers.) Murrill
 (Pers.) Müll.Arg.
@@ -15920,25 +16147,23 @@
 (Pers.) Pegler & T.W.K.Young
 (Pers.) Pers.
 (Pers.) Petr.
 (Pers.) Pilát
 (Pers.) Poelt
 (Pers.) Poir.
 (Pers.) Pouzar
-(Pers.) Quel.
 (Pers.) Quél.
 (Pers.) R.Br.
 (Pers.) R.E.Fr.
 (Pers.) R.H.Petersen
 (Pers.) Rabenh.
 (Pers.) Raf.
 (Pers.) Rea
-(Pers.) Redhead
 (Pers.) Redhead & Kuyper
-(Pers.) Redhead, Moncalvo & Thorn
+(Pers.) Redhead, Lutzoni, Moncalvo & Vilgalys
 (Pers.) Redhead, Vilgalys & Moncalvo
 (Pers.) Rehm
 (Pers.) Ricken
 (Pers.) Roem. & Schult.
 (Pers.) Rostaf.
 (Pers.) Rostr.
 (Pers.) Roussel
@@ -15947,86 +16172,91 @@
 (Pers.) S.E.Carp. & Korf
 (Pers.) Sacc.
 (Pers.) Saff.
 (Pers.) Sch.Bip.
 (Pers.) Schltdl.
 (Pers.) Schwein.
 (Pers.) Seaver
-(Pers.) Seaver ex Korf, C.S.Ramamurthi & L.R.Batra
+(Pers.) Seaver ex C.S.Ramamurthi, Korf & L.R.Batra
 (Pers.) Singer
-(Pers.) Singer & Bondartsev
 (Pers.) Sm.
 (Pers.) Sommerf.
 (Pers.) Spooner
 (Pers.) Sprague ex Britton & P.Wilson
 (Pers.) Spreng.
 (Pers.) Staiger & Kalb
 (Pers.) Steud.
 (Pers.) Sweet
 (Pers.) Swinscow & Krog
 (Pers.) Szatala
 (Pers.) T.Macbr.
 (Pers.) T.Wagner & M.Fisch.
 (Pers.) Takah.
 (Pers.) Th.Fr.
+(Pers.) Thorn, Moncalvo & Redhead
 (Pers.) Tul.
 (Pers.) Tul. & C.Tul.
 (Pers.) Tutin
 (Pers.) Vain.
+(Pers.) Vizzini, P.Alvarado, G.Moreno & Cons.
 (Pers.) Volkart ex Schinz & R.Keller
 (Pers.) W.B.Cooke
 (Pers.) W.Phillips
 (Pers.) Wallr.
+(Pers.) Wedin, J.C.Zamora & Millanes
 (Pers.) Y.C.Dai
 (Pers.) Y.M.Ju, J.D.Rogers & H.M.Hsieh
 (Pers.) Zahlbr.
-(Persoon ex Acharius) J.R.Laundon
+(Pers.) Zmitr. & Kovalenko
+(Pers.) Zmitr., Ezhov & Wasser
+(Pers.) Zmitr., Wasser & Ezhov
+(Persoon ex Ach.) J.R.Laundon
 (Perty) A.Braun
 (Perty) F.Stein
 (Perty) Playfair
 (Perty) Rabenh.
 (Perty) West & G.S.West
 (Pescott & Nicholls) D.L.Jones & M.A.Clem.
 (Pescott & Nicholls) Nicholls
-(Petch) B.Ortiz & Both
+(Petch) Both & B.Ortiz
 (Petch) J.T.Palmer
 (Petch) Krejzová
 (Petch) L.Ling
 (Petch) Milner
 (Petch) Pegler
 (Petch) S.Keller
 (Petch) S.Keller & Milner
 (Petch) Syd. & P.Syd.
 (Petch) Vánky
 (Peter B.Adams) M.A.Clem. & D.L.Jones
 (Peter G.Wilson & M.L.Moody) Christenh. & Byng
 (Petersen) Krasske
 (Petkoff) Willi Krieg.
-(Petr. & Bremer) U.Braun
 (Petr. & Cif.) U.Braun & Crous
 (Petr. & Syd.) Aa
 (Petr.) A.R.Liu, T.Xu & L.D.Guo
 (Petr.) Arx & Constant.
 (Petr.) Arx & E.Müll.
 (Petr.) B.Sutton
-(Petr.) K.D.Hyde, Aptroot & You Z.Wang
 (Petr.) Parbery & Minter
 (Petr.) Shoemaker & C.E.Babc.
 (Petr.) Thines
-(Petri) C.W.Dodge & Zeller
+(Petr.) You Z.Wang, Aptroot & K.D.Hyde
 (Petri) Corner & Hawker
 (Petri) J.W.Cribb
 (Petri) Kühner
 (Petri) L.A.Kantsch. & Gikaschvili
+(Petri) T.Lebel
+(Petri) Zeller & C.W.Dodge
 (Petrie) Clayton & Renvoize ex Connor & Edgar
 (Petrie) H.P.Linder
 (Petrie) Kük.
 (Petrie) Zotov
 (Pfeiff.) Zucc. ex Pfeiff. & Otto
-(Phaff, Mrak & O.B.Williams) S.A.Mey. & Fell
+(Phaff, Mrak & O.B.Williams) Fell & S.A.Mey.
 (Phil.) Aellen
 (Phillipson) A.E.Holland
 (Pic.Serm.) Crabbe, Jermy & Mickel
 (Pic.Serm.) R.M.Tryon & A.F.Tryon
 (Picc.) Børgesen
 (Pidopl.) W.Gams
 (Pierre) Pellegr.
@@ -16040,17 +16270,20 @@
 (Pilát) G.Cunn.
 (Pilát) Jülich
 (Pilát) Wasser
 (Pinoy) Stockdale, D.W.R.Mack. & Austwick
 (Piper) Chase
 (Piper) Stapf
 (Piper) Verdc.
+(Piroz. & Hodges) R.F.Castañeda & W.B.Kendr.
 (Piroz. & S.D.Patil) Gusmão
 (Pit.) Humphries
-(Pitt & Hocking) Lachance & Rosa
+(Pitt) Pitt
+(Pitt) Samson, N.Yilmaz, Frisvad & Seifert
+(Piątek & R.G.Shivas) Piątek & M.Lutz
 (Planch.) Benth.
 (Planch.) Blume
 (Planch.) Boiss.
 (Planch.) Bureau
 (Planch.) Casp.
 (Planch.) Chrtek & Slavikova
 (Planch.) Diels
@@ -16075,14 +16308,15 @@
 (Playfair) Pochm.
 (Playfair) Skvortsov
 (Playfair) Thomasson
 (Playfair) V.May
 (Playfair) W.Conrad
 (Playfair) Willi Krieg.
 (Playfair) Willi Krieg. & Gerloff
+(Plowr. & G.Winter) Syd.
 (Pochm.) Hub.-Pest.
 (Podp.) Barkworth & D.R.Dewey
 (Podp.) Á.Löve
 (Poelln.) Carolin ex Hershk.
 (Poelln.) Geesink
 (Poelln.) Pax & K.Hoffm.
 (Poelt) Essl.
@@ -16140,14 +16374,15 @@
 (Poir.) Palla
 (Poir.) Parl.
 (Poir.) Pedley
 (Poir.) Roberty
 (Poir.) Robyns & Tournay
 (Poir.) Roem. & Schult.
 (Poir.) Rydb.
+(Poir.) S.E.Fawc. & A.R.Sm.
 (Poir.) S.S.Hooper
 (Poir.) Schindl.
 (Poir.) Scribn.
 (Poir.) Scribn. & Merr.
 (Poir.) Spreng.
 (Poir.) Steud.
 (Poir.) T.Moore
@@ -16194,46 +16429,48 @@
 (Putt.) E.M.Benn.
 (Putt.) F.Muell.
 (Putt.) L.W.Cayzer & Crisp
 (Putt.) L.W.Cayzer, Crisp & I.Telford
 (Putt.) Lehm.
 (Putt.) Wawra
 (Pócs) Pócs
+(Q.M.Wang, F.Y.Bai, M.Groenew. & Boekhout) R.G.Shivas & Rodr.Mir.
+(Quél.) Bondartsev & Singer
 (Quél.) Bourdot & Galzin
 (Quél.) Cooke
 (Quél.) Jülich
 (Quél.) Kühner
 (Quél.) P.Karst.
 (Quél.) Pat.
 (Quél.) Quél.
 (Quél.) Rea
 (Quél.) S.E.Carp.
 (Quél.) Sacc.
 (Quél.) Schumach.
 (Quél.) Singer
-(Quél.) Singer & Bondartsev
+(Quél.) T.J.Baroni, Largent & V.Hofst.
 (Quél.) Watling
 (R.A.Braune) Vavra & Joyon ex I.B.Heath
 (R.A.Paterson) Karling
 (R.Br. ex A.Rich.) Benth.
 (R.Br. ex Benth.) C.A.Gardner
 (R.Br. ex Benth.) C.Moore
 (R.Br. ex Benth.) Chodat ex Steenis
 (R.Br. ex Benth.) Crisp
+(R.Br. ex Benth.) Crisp & L.G.Cook
 (R.Br. ex Benth.) Domin
 (R.Br. ex Benth.) F.Muell.
 (R.Br. ex Benth.) Govaerts
 (R.Br. ex Benth.) K.D.Hill & L.A.S.Johnson
 (R.Br. ex Benth.) Kuntze
 (R.Br. ex Benth.) Maiden
 (R.Br. ex Benth.) Paul G.Wilson
 (R.Br. ex Benth.) Pedley
 (R.Br. ex Benth.) Puttock
 (R.Br. ex Benth.) Rye
-(R.Br. ex Benth.) Rye x Astartea corniculata Schauer
 (R.Br. ex Benth.) S.T.Reynolds & R.J.F.Hend.
 (R.Br. ex Benth.) Specht
 (R.Br. ex Benth.) Valeton
 (R.Br. ex Britten) Orchard
 (R.Br. ex Cromb.) Elix
 (R.Br. ex Cromb.) Elvebakk
 (R.Br. ex Cromb.) Hale
@@ -16289,18 +16526,15 @@
 (R.Br.) A.Braun
 (R.Br.) A.Camus
 (R.Br.) A.Cunn. ex R.Br.
 (R.Br.) A.DC.
 (R.Br.) A.Dietr.
 (R.Br.) A.E.Holland
 (R.Br.) A.J.Paton
-(R.Br.) A.J.Paton x Coleus graveolens (R.Br.) A.J.Paton
-(R.Br.) A.J.Paton x Coleus suaveolens (S.T.Blake) P.I.Forst. & T.C.Wilson
 (R.Br.) A.J.Scott
-(R.Br.) A.J.Scott x Einadia trigonos subsp. stellulata (Benth.) Paul G.Wilson
 (R.Br.) A.M.Humphreys & H.P.Linder
 (R.Br.) A.R.Field
 (R.Br.) A.R.Field & Bostock
 (R.Br.) A.R.Mast & K.R.Thiele
 (R.Br.) A.R.Simões & Staples
 (R.Br.) A.S.George
 (R.Br.) A.T.Lee
@@ -16335,15 +16569,14 @@
 (R.Br.) Bonap.
 (R.Br.) Bory
 (R.Br.) Borzi
 (R.Br.) Bostock
 (R.Br.) Brack.
 (R.Br.) Bremek.
 (R.Br.) Brieger
-(R.Br.) Brieger x Dockrillia linguiformis (Sw.) Brieger
 (R.Br.) Briq.
 (R.Br.) Britten
 (R.Br.) Brongn.
 (R.Br.) Buchenau
 (R.Br.) Byng & Christenh.
 (R.Br.) C.A.Gardner
 (R.Br.) C.A.Mey.
@@ -16365,15 +16598,14 @@
 (R.Br.) Chase
 (R.Br.) Chase ex E.G.Camus & A.Camus
 (R.Br.) Ching
 (R.Br.) Choisy
 (R.Br.) Christ
 (R.Br.) Christenh.
 (R.Br.) Christenh. & Byng
-(R.Br.) Christenh. x Blechnum neohollandicum Christenh.
 (R.Br.) Cockayne
 (R.Br.) Colozza
 (R.Br.) Connor & Edgar
 (R.Br.) Copel.
 (R.Br.) Corner
 (R.Br.) Craven & R.D.Edwards
 (R.Br.) D.A.Cooke
@@ -16387,39 +16619,38 @@
 (R.Br.) Desv.
 (R.Br.) Diane & Hilger
 (R.Br.) Diels
 (R.Br.) Diels & E.Pritz.
 (R.Br.) Dimon & M.A.M.Renner
 (R.Br.) Dockrill
 (R.Br.) Domin
-(R.Br.) Domin x Cymbopogon refractus (R.Br.) A.Camus
 (R.Br.) Downing
 (R.Br.) Drake
 (R.Br.) Druce
 (R.Br.) Drude
 (R.Br.) Dum.Cours.
 (R.Br.) Dunlop
 (R.Br.) Duyfjes
+(R.Br.) E.J.Thomps.
 (R.Br.) E.M.Benn.
 (R.Br.) E.Wimm.
 (R.Br.) Endl.
 (R.Br.) Endl. ex Kunth
 (R.Br.) Endl. ex Walp.
 (R.Br.) Engelm.
 (R.Br.) Engl.
 (R.Br.) Ettingsh.
 (R.Br.) Ewart
 (R.Br.) Ewart & B.Rees
 (R.Br.) Ewart & Jean White
 (R.Br.) Ewart & O.B.Davies
 (R.Br.) F.M.Bailey
 (R.Br.) F.Muell.
-(R.Br.) F.Muell. & Sond. ex Sond.
+(R.Br.) F.Muell. & Sond.
 (R.Br.) F.Muell. ex Benth.
-(R.Br.) F.Muell. ex Benth. x Wrightia versicolor S.T.Blake
 (R.Br.) F.Muell. ex Kuntze
 (R.Br.) F.Muell. ex Maiden & Betche
 (R.Br.) F.Muell. ex Ulbr.
 (R.Br.) F.N.Williams
 (R.Br.) Farw.
 (R.Br.) Feuillet
 (R.Br.) Fitzg.
@@ -16427,15 +16658,14 @@
 (R.Br.) Fosberg
 (R.Br.) Fosberg & Sachet
 (R.Br.) Fée
 (R.Br.) G.Brückn.
 (R.Br.) G.Chandler & Crisp
 (R.Br.) G.Don
 (R.Br.) G.Mans.
-(R.Br.) G.Mans. x Schenkia clementii (Domin) G.Mans.
 (R.Br.) Gasper & Salino
 (R.Br.) Gasper & V.A.O.Dittrich
 (R.Br.) Gaudich.
 (R.Br.) Greene
 (R.Br.) Griseb.
 (R.Br.) Guill.
 (R.Br.) H.Gross
@@ -16505,14 +16735,15 @@
 (R.Br.) L.A.S.Johnson & P.H.Weston
 (R.Br.) L.R.Fraser & Vickery
 (R.Br.) L.Watson
 (R.Br.) Lauterb.
 (R.Br.) Lazarides
 (R.Br.) Lazarides & R.D.Webster
 (R.Br.) Lehm.
+(R.Br.) Lepschi
 (R.Br.) Lindl.
 (R.Br.) Link
 (R.Br.) Lowe ex Salomon
 (R.Br.) Luerss.
 (R.Br.) Lyon
 (R.Br.) M.A.Clem.
 (R.Br.) M.A.Clem. & D.L.Jones
@@ -16534,15 +16765,14 @@
 (R.Br.) Mez
 (R.Br.) Mildbr.
 (R.Br.) Moldenke
 (R.Br.) Moq.
 (R.Br.) Morrone
 (R.Br.) Mosyakin
 (R.Br.) Mosyakin & Clemants
-(R.Br.) Mosyakin & Clemants x Dysphania cristata (F.Muell.) Mosyakin & Clemants
 (R.Br.) Muasya
 (R.Br.) Munro ex Benth.
 (R.Br.) Murr & Thell.
 (R.Br.) Myint
 (R.Br.) Müll.Berol.
 (R.Br.) N.A.Wakef.
 (R.Br.) N.Hallé
@@ -16553,36 +16783,33 @@
 (R.Br.) Nevski
 (R.Br.) Newbold
 (R.Br.) O.Deg.
 (R.Br.) Ohwi
 (R.Br.) Olde & Marriott
 (R.Br.) Ooststr.
 (R.Br.) Opiz
+(R.Br.) Ormerod
 (R.Br.) Ostenf.
-(R.Br.) Ostenf. x Eremophila latrobei F.Muell.
 (R.Br.) P.Beauv.
 (R.Br.) P.Beauv. ex Roem. & Schult.
 (R.Br.) P.I.Forst.
 (R.Br.) P.M.Peterson & N.Snow
 (R.Br.) P.S.Green
 (R.Br.) P.Taylor
 (R.Br.) Palla
 (R.Br.) Paul G.Wilson
 (R.Br.) Pedley
 (R.Br.) Pedro
 (R.Br.) Pei
 (R.Br.) Pennell
 (R.Br.) Peter G.Wilson & J.T.Waterh.
-(R.Br.) Peter G.Wilson & J.T.Waterh. x Lophostemon grandiflorus (Benth.) Peter G.Wilson & J.T.Waterh.
-(R.Br.) Peter G.Wilson & J.T.Waterh. x Lophostemon suaveolens (Sol. ex Gaertn.) Peter G.Wilson & J.T.Waterh.
 (R.Br.) Pfeiff.
 (R.Br.) Pierre
 (R.Br.) Pilg.
 (R.Br.) Poir.
-(R.Br.) Poir. x Ptilotus polystachyus (Gaudich.) F.Muell.
 (R.Br.) Popov ex R.R.Mill
 (R.Br.) Praj. & J.Parn.
 (R.Br.) Quinn
 (R.Br.) R.Br.
 (R.Br.) R.D.Webster
 (R.Br.) R.J.F.Hend.
 (R.Br.) R.L.Barrett & P.M.Peterson
@@ -16622,15 +16849,14 @@
 (R.Br.) Seem.
 (R.Br.) Siebert & Voss
 (R.Br.) Skeels
 (R.Br.) Sleumer
 (R.Br.) Sm.
 (R.Br.) Snijman & Kocyan
 (R.Br.) Soják
-(R.Br.) Soják x Polygonum glabrum Willd.
 (R.Br.) Soreng, L.J.Gillespie & S.W.L.Jacobs
 (R.Br.) Spach
 (R.Br.) Spangler
 (R.Br.) Sprague & Summerh.
 (R.Br.) Spreng.
 (R.Br.) Spring
 (R.Br.) Standl.
@@ -16670,84 +16896,94 @@
 (R.Br.) W.A.Weber
 (R.Br.) W.R.Barker
 (R.Br.) W.R.Barker & Beardsley
 (R.Br.) Warb.
 (R.Br.) Wettst.
 (R.Br.) Wijk & Margad.
 (R.Br.) Wikstr.
+(R.Br.) Wilson
 (R.Br.) Zotov
 (R.Br.) de Koning & Sosef
 (R.Br.) de Lange & Mosyakin
 (R.Br.) de Vriese
 (R.Br.) de Wet
 (R.Br.) de Wet & J.R.Harlan
 (R.Br.) Á.Löve
 (R.Br.bis) Broth.
 (R.Br.bis) Dixon
 (R.Br.bis) J.R.Spence & H.P.Ramsay
 (R.Br.bis) Paris
 (R.Br.bis) Sainsbury
 (R.Br.bis) Wijk & Margad.
-(R.Br.ter.) J.R.Spence & H.P.Ramsay
 (R.C.Harris) Lücking, M.P.Nelsen & Aptroot
-(R.Chodat & F.Chodat) Komárek
 (R.Cunn. ex A.Cunn.) Andersen
 (R.Cunn. ex A.Cunn.) Cockayne & Allan
 (R.Cunn.) Garay
 (R.Cunn.) Rchb.f.
 (R.Cunn.) Rupp
 (R.D.Spencer & Lumley) Craven
 (R.D.Webster) B.K.Simon
 (R.D.Webster) R.D.Webster
 (R.D.Webster) Zuloaga
 (R.D.Wood) R.D.Wood
 (R.D.Wood) Raam
 (R.E.Massey ex Stapf) Clayton
 (R.E.Norris & M.J.Wynne) M.J.Wynne
 (R.E.Sm. & E.H.Sm.) Leonian
-(R.Emers. & Cooney) Schipper
 (R.Emers.) R.Emers. & C.M.Wilson
 (R.F.Castañeda) R.F.Castañeda & W.Gams
 (R.F.Park & Keane) Andjic
 (R.F.Park & Keane) Crous
 (R.F.Park & Keane) Crous & U.Braun
+(R.F.Park & Keane) Quaedvl. & Crous
 (R.Fern. & Verdc.) Munir
 (R.Fern. & Verdc.) P.W.Michael
 (R.G.Bagn. & Sheridan) Nag Raj
+(R.G.Shivas & Cunningt.) McTaggart & R.G.Shivas
+(R.G.Shivas & Rodr.Mir.) Kijporn. & Aime
+(R.G.Shivas & Rodr.Mir.) Q.M.Wang, F.Y.Bai, Begerow & Boekhout
+(R.G.Shivas & Rodr.Mir.) Q.M.Wang, F.Y.Bai, M.Groenew. & Boekhout
 (R.G.Shivas & Rodr.Mir.) Rodr.Mir. & Weijman
+(R.G.Shivas & Vánky) McTaggart & R.G.Shivas
+(R.G.Shivas & Vánky) McTaggart, R.G.Shivas & Begerow
 (R.G.Shivas & Vánky) Vánky & R.G.Shivas
+(R.G.Shivas, McTaggart & Vánky) M.Lutz & Piątek
+(R.G.Shivas, McTaggart & Vánky) McTaggart & R.G.Shivas
+(R.G.Shivas, S.J.Pethybr. & S.J.Jones) T.L.Pearce, J.B.Scott, Crous, S.J.Pethybr. & F.S.Hay
+(R.G.Shivas, Vánky & Cunningt.) McTaggart & R.G.Shivas
 (R.H.Anderson) A.J.Scott
 (R.H.Anderson) Aellen
 (R.H.Anderson) Ewart
 (R.H.Anderson) J.M.Black
 (R.H.Anderson) Paul G.Wilson
 (R.H.Anderson) Ulbr.
+(R.H.Petersen) J.A.Cooper
 (R.H.Petersen) Jülich
 (R.Haller Aar) Boertm.
 (R.Hartig) A.G.Newhall
 (R.Hartig) Deighton
 (R.Hedw.) Fr.
 (R.Hedw.) Raitv.
 (R.Hedw.) Sacc.
 (R.Heim) Heinem.
 (R.Heim) R.Heim
 (R.Heim) Singer
-(R.Hogg) Mabb.
 (R.J.Bates & D.L.Jones) M.A.Clem. & D.L.Jones
 (R.J.Bates) D.L.Jones & M.A.Clem.
 (R.J.Bates) I.Thomps.
 (R.J.Bates) J.M.H.Shaw
 (R.J.Bates) M.A.Clem.
 (R.J.Bates) M.A.Clem. & D.L.Jones
 (R.J.Bates) R.J.Bates
 (R.J.Bates) Szlach.
 (R.J.F.Hend.) P.F.Horsfall & G.W.Carr
 (R.J.F.Hend.) R.J.F.Hend.
 (R.J.F.Hend.) R.L.Barrett & T.D.Macfarl.
 (R.J.F.Hend.) Snijman & Kocyan
+(R.K.Benj.) Benny & M.Blackw.
 (R.L.Barrett & I.Telford) R.W.Bouman
 (R.L.Barrett) Messina
 (R.L.Barrett) P.I.Forst.
 (R.M.Barker) Beier & Thulin
 (R.M.Barker) R.M.Barker
 (R.M.Patrick) Metzeltin & Lange-Bert.
 (R.M.Schust.) E.A.Hodgs.
@@ -16789,16 +17025,18 @@
 (R.S.Rogers) W.M.Curtis
 (R.Sant.) Follmann & Ahti
 (R.Sant.) G.Thor, Sérus., Lücking & Matsumoto
 (R.Sant.) Hafellner & Kalb
 (R.Sant.) Lücking
 (R.Sant.) Lücking, Sérus. & Vězda
 (R.Sant.) Vězda
+(R.Sprague & Aar.G. Johnson) Crous & U.Braun
 (R.Sprague) Arx
 (R.Sprague) de Hoog & Herm.-Nijh.
+(R.Stone) Sivan.
 (R.T.Baker & H.G.Sm.) B.E.Pfeil & Henwood
 (R.T.Baker & H.G.Sm.) Blakely
 (R.T.Baker & H.G.Sm.) Ewart & O.B.Davies
 (R.T.Baker & H.G.Sm.) L.A.S.Johnson
 (R.T.Baker & H.G.Sm.) L.A.S.Johnson & Blaxell
 (R.T.Baker & H.G.Sm.) Silba
 (R.T.Baker) Barlow
@@ -16806,34 +17044,31 @@
 (R.T.Baker) Domin
 (R.T.Baker) Ewart, Jean White & B.Rees
 (R.T.Baker) H.B.Will.
 (R.T.Baker) K.D.Hill & L.A.S.Johnson
 (R.T.Baker) L.A.S.Johnson
 (R.T.Baker) L.A.S.Johnson & Blaxell
 (R.T.Baker) M.B.Welch, Coombs & McGlynn
-(R.T.Baker) M.B.Welch, Coombs & McGlynn x Acacia glaucocarpa Maiden & Blakely
 (R.T.Baker) Maiden
 (R.T.Baker) Maiden & Betche
 (R.T.Baker) Pedley
 (R.T.Baker) R.T.Baker
 (R.T.Baker) Skeels
 (R.V.Sm. & McGill.) Christenh. & Byng
 (R.V.Sm.) Anderb.
 (R.V.Sm.) Christenh. & Byng
 (R.V.Sm.) Pedley
 (R.Vig.) Domin
-(R.Vig.) Lowry
 (R.Vig.) Lowry & G.M.Plunkett
 (R.W.Davidson & Lombard) Ryvarden
 (R.W.Holmes) J.D.Dodge
 (R.W.Johnson) A.R.Simões & Staples
 (R.W.Phillips) Perman
 (R.W.Ricker) Hörnig, Schnetter & Prud'homme
 (R.Wagner) Chinnock
-(Rabenh. & Küchenm.) Vuill.
 (Rabenh. ex C.Janisch) O.Müll.
 (Rabenh.) Bréb. ex Grunow
 (Rabenh.) Chodat
 (Rabenh.) Cleve
 (Rabenh.) Cooke
 (Rabenh.) De Toni
 (Rabenh.) E.G.Simmons
@@ -16865,14 +17100,15 @@
 (Racib.) Nann.-Bremek. & Dhillon ex Ing
 (Racib.) Nordst.
 (Racib.) Playfair
 (Racib.) Racib.
 (Racib.) T.Wagner & M.Fisch.
 (Racib.) Taft
 (Racib.) Teiling
+(Racib.) Thirum.
 (Racib.) U.Braun
 (Racib.) West & G.S.West
 (Racib.) Willi Krieg.
 (Racib.) Willi Krieg. & Gerloff
 (Racov.) Döbbeler
 (Raddi) E.J.Lowe
 (Raddi) Fosberg
@@ -16903,20 +17139,18 @@
 (Raf.) Kuntze
 (Raf.) Moldenke
 (Raf.) P.Taylor
 (Raf.) Raf.
 (Rafn) Godr.
 (Raithelh.) Raithelh.
 (Raitv.) Baral
-(Rajchenb. & A.David) Hjortstam & K.H.Larss.
+(Rajchenb. & J.E.Wright) B.K.Cui & Shun Liu
+(Rajchenb. & P.K.Buchanan) B.K.Cui & Shun Liu
 (Rajchenb.) Miettinen & Rajchenb.
 (Ralfs ex Bornet & Flahault) Komárek & Anagn.
-(Ralfs ex Kütz.) D.M.Williams & Round
-(Ralfs ex Kütz.) Kütz.
-(Ralfs ex Kütz.) Lange-Bert.
 (Ralfs ex Ralfs) Bourr.
 (Ralfs ex Ralfs) Bourr. & Compere
 (Ralfs) A.Cleve
 (Ralfs) A.Louis & Peeters
 (Ralfs) Bando
 (Ralfs) Bréb.
 (Ralfs) Chodat
@@ -16946,22 +17180,17 @@
 (Randhawa) Transeau
 (Raoul) Baill.
 (Raoul) Connor & Edgar
 (Raoul) H.P.Linder
 (Raoul) Hook.f.
 (Raoul) Raoul
 (Raoul) Zotov
-(Rasanen) D.J.Galloway
-(Rasanen) Essl.
-(Rasanen) Streimann
 (Rattray) Hallegr.
 (Ravenel ex Berk. & M.A.Curtis) Pat.
 (Raym.-Hamet & H.Perrier) A.Berger
-(Raym.-Hamet & H.Perrier) A.Berger x Bryophyllum delagoense (Eckl. & Zeyh.) Schinz
-(Raym.-Hamet & H.Perrier) A.Berger x Bryophyllum tubiflorum Harv.
 (Raym.-Hamet & H.Perrier) Lauz.-March.
 (Raym.-Hamet) A.Berger
 (Rchb. ex Kunze) J.W.Grimes
 (Rchb. ex Kunze) Kuntze
 (Rchb. ex Spreng.) Heynh.
 (Rchb.) A.S.George
 (Rchb.) Benth.
@@ -17017,14 +17246,15 @@
 (Reader) Domin
 (Reader) Ewart
 (Reader) Ewart & Jean White
 (Reader) Ostenf.
 (Reader) Pedley
 (Reader) S.W.L.Jacobs & J.Everett
 (Reader) Toelken
+(Recca & Mrak) Van der Walt
 (Rech.f.) Rech.f.
 (Redhead) Singer
 (Redinger) A.W.Archer
 (Redinger) Staiger
 (Redouté) J.F.Macbr.
 (Redouté) Salisb.
 (Redouté) Spreng.
@@ -17039,19 +17269,19 @@
 (Regel) Nge & K.R.Thiele
 (Regel) Pedley
 (Regel) R.M.King & H.Rob.
 (Regel) Roshkova
 (Regel) Silva Tar.
 (Rehder & E.H.Wilson) M.F.Fay & Christenh.
 (Rehm ex Arnold) Arnold
-(Rehm ex Gamundí) T.Schumach. & Dissing
+(Rehm ex Gamundí) Dissing & T.Schumach.
+(Rehm) Aptroot, K.D.Hyde & Joanne E.Taylor
 (Rehm) D.Hawksw. & R.Sant.
 (Rehm) Hafellner & Kalb
 (Rehm) K.D.Hyde & J.Fröhl.
-(Rehm) K.D.Hyde, Joanne E.Taylor & Aptroot
 (Rehm) Kalb & Lücking
 (Rehm) M.P.Sharma
 (Rehm) R.Sant.
 (Rehm) Rehm
 (Rehm) Vězda
 (Rehm.) J.H.Haines ex Korf & Zhuang
 (Reichardt) Burley
@@ -17089,14 +17319,15 @@
 (Reinsch) Skuja
 (Reinsch) Sturch
 (Reinsch) Thaxt.
 (Reinsch) Wolle
 (Reinw. & Hornsch.) M.Fleisch.
 (Reinw. & Hornsch.) Mitt.
 (Reinw. & Hornsch.) Müll.Hal.
+(Reinw. & Hornsch.) Touw & Magill
 (Reinw. ex Blume) Blume
 (Reinw. ex Blume) Hassk.
 (Reinw. ex Blume) Holttum
 (Reinw. ex Blume) Miq.
 (Reinw. ex Korth.) Benth.
 (Reinw. ex Korth.) de Wit
 (Reinw. ex Nees & T.Nees) Blume
@@ -17152,26 +17383,28 @@
 (Req.) Duby
 (Req.) P.W.Ball
 (Req.) Parl.
 (Req.) Spreng.
 (Retz.) A.Camus
 (Retz.) A.R.Bean
 (Retz.) Alston
+(Retz.) Benth.
 (Retz.) Benth. ex Pilg.
 (Retz.) Bold.
 (Retz.) C.Chr.
 (Retz.) C.E.C.Fisch.
 (Retz.) C.E.Hubb.
 (Retz.) C.F.Reed
 (Retz.) C.Presl
 (Retz.) Christ
 (Retz.) Clayton
 (Retz.) Copel.
 (Retz.) DC.
 (Retz.) Domin
+(Retz.) Druce
 (Retz.) E.Walker
 (Retz.) F.Muell.
 (Retz.) Fée
 (Retz.) Hack.
 (Retz.) Honda
 (Retz.) J.F.Gmel.
 (Retz.) J.Presl & C.Presl
@@ -17186,15 +17419,14 @@
 (Retz.) Link
 (Retz.) Luerss.
 (Retz.) Moq.
 (Retz.) Nees
 (Retz.) Nees ex Steud.
 (Retz.) Ohwi
 (Retz.) P.Beauv.
-(Retz.) P.Beauv. x Sporobolus elongatus R.Br.
 (Retz.) P.M.Peterson & N.Snow
 (Retz.) Parl.
 (Retz.) Pers.
 (Retz.) Poir.
 (Retz.) R.Br.
 (Retz.) R.Br. ex Schult.
 (Retz.) R.W.Bouman
@@ -17213,27 +17445,26 @@
 (Retz.) Trin.
 (Retz.) Trin. ex Steud.
 (Retz.) Urb.
 (Retz.) Vahl
 (Retz.) Valck.Sur.
 (Retz.) Veldkamp
 (Retz.) Veldkamp ex Mesfin
-(Rex) Nann.-Bremek., Y.Yamam. & R.Sharma
+(Rex) Nann.-Bremek., R.Sharma & Y.Yamam.
 (Rex) Torrend
 (Rich) Teiling
 (Rich. ex Pers.) R.Hedw.
 (Rich.) Desv.
 (Rich.) F.Muell.
 (Rich.) G.Don
 (Rich.) H.S.Irwin & Barneby
 (Rich.) Hitchc.
 (Rich.) Kuntze
 (Rich.) Nees
 (Rich.) Vahl
-(Rich.) Vahl x Stachytarpheta jamaicensis (L.) Vahl
 (Richon) Costantin & L.M.Dufour
 (Rick) G.Cunn.
 (Rick) Imazeki
 (Rick) Lloyd
 (Rick) Singer
 (Rick) Stalpers & Hjortstam
 (Ridl.) Cogn.
@@ -17254,59 +17485,58 @@
 (Ridl.) Veldkamp
 (Rifai) Harmaja
 (Rifai) Korf & W.Y.Zhuang
 (Rifai) Kraisit., Pfister & M.E.Sm.
 (Rivolta) L.D.Galloway
 (Rob.Henry & Contu) A.Ortega
 (Roberty) Roberty
-(Rodway & Cleland) D.A.Reid
 (Rodway & Cleland) Kotl. & Pouzar
 (Rodway & Cleland) P.K.Buchanan & Ryvarden
-(Rodway & Cleland) Ryvarden
-(Rodway & Cleland) Y.C.Dai
 (Rodway & Cleland) Y.C.Dai, F.Wu, G.M.Gates & R.Du
 (Rodway) B.Sutton
 (Rodway) Beever, Castellano & T.Lebel
 (Rodway) Brittleb.
 (Rodway) Broth.
-(Rodway) C.W.Dodge & Zeller
 (Rodway) Castellano
 (Rodway) Castellano & Trappe
 (Rodway) D.I.Morris
 (Rodway) Dennis
 (Rodway) E.A.Hodgs.
 (Rodway) E.Horak
 (Rodway) G.Cunn.
+(Rodway) G.M.Gates & Van Vooren
 (Rodway) G.W.Beaton & Weste
 (Rodway) G.W.Beaton, Pegler & T.W.K.Young
 (Rodway) Gasparini
 (Rodway) Grolle
 (Rodway) Hewson
 (Rodway) J.H.Haines
 (Rodway) J.H.Willis
 (Rodway) J.J.Engel
 (Rodway) J.Townrow
 (Rodway) L.A.S.Johnson & B.G.Briggs
 (Rodway) L.M.Kohn
 (Rodway) M.P.Sharma
 (Rodway) Nebel
+(Rodway) Núñez & Ryvarden
 (Rodway) P.K.Buchanan & Hood
 (Rodway) R.M.Schust.
 (Rodway) R.M.Schust. & J.J.Engel
 (Rodway) Rifai
-(Rodway) Ryvarden & Núñez
 (Rodway) S.E.Carp.
 (Rodway) S.W.L.Jacobs & J.Everett
 (Rodway) Sacc.
 (Rodway) Sainsbury ex Wijk, Margad. & Florsch.
 (Rodway) Singer & A.H.Sm.
 (Rodway) Spooner
+(Rodway) T.Lebel
 (Rodway) T.Lebel & Castellano
 (Rodway) Trappe
 (Rodway) W.M.Curtis
+(Rodway) Zeller & C.W.Dodge
 (Roem. & Schult.) C.E.Hubb.
 (Roem. & Schult.) F.Muell.
 (Roem. & Schult.) Henrard
 (Roem. & Schult.) Hughes
 (Roem. & Schult.) Kunth
 (Roem. & Schult.) Link ex Bluff, Nees & Schauer
 (Roem. & Schult.) N.Snow
@@ -17321,18 +17551,18 @@
 (Roem. & Schult.) Vickery
 (Rohrb.) Graebn.
 (Rolfe ex Downie) Seidenf. & Smitinand
 (Rolfe) Garay
 (Rolfe) M.A.Clem. & D.L.Jones
 (Rolfe) Rolfe
 (Rolfe) Schltr.
-(Romagn.) Arnolds
+(Romagn.) Antonín & Noordel.
+(Romagn.) Largent
 (Romagn.) M.M.Moser
 (Romagn.) Noordel.
-(Romagn.) Noordel. & Antonín
 (Romagn.) P.D.Orton
 (Romagn.) Redhead, Vilgalys & Moncalvo
 (Romell ex Burt) Parmasto
 (Romell) Bondartseva
 (Romell) Chenant.
 (Romell) D.A.Reid
 (Romell) D.V.Baxter
@@ -17365,19 +17595,19 @@
 (Rosenv.) P.C.Silva
 (Rosenv.) Papenf.
 (Rosenv.) S.Lund
 (Rosenv.) Woelk.
 (Rosenv.) Woelk. & Womersley
 (Rostaf.) Nann.-Bremek.
 (Rostk.) Cooke
-(Rostk.) Hollos
 (Rostk.) Hollós
 (Rostk.) P.Ponce de León
 (Roth ex Roem. & Schult.) Koehne
 (Roth ex Schult.) Benth.
+(Roth) 
 (Roth) Ali
 (Roth) Alston
 (Roth) Aresch.
 (Roth) Baker
 (Roth) Bornet
 (Roth) Bory
 (Roth) Britton & Rose
@@ -17599,14 +17829,15 @@
 (Rupp) Rupp
 (Rupp) Szlach.
 (Rydb.) Waterf.
 (Rye) C.S.P.Foster & Henwood
 (Rye) Kellermann, Rye & K.R.Thiele
 (Rye) Rye
 (Rye, R.L.Barrett & M.D.Barrett) K.L.Wilson & J.J.Bruhl
+(Ryvarden) Y.C.Dai, F.Wu & C.L.Zhao
 (Räsänan) P.M.McCarthy
 (Räsänen) A.Crespo, Divakar & Elix
 (Räsänen) D.J.Galloway
 (Räsänen) Essl.
 (Räsänen) G.Wilh. & Ladd
 (Räsänen) Hafellner
 (Räsänen) Hertel
@@ -17623,15 +17854,15 @@
 (Räusch.) S.F.Gray
 (Röll) Willi Krieg.
 (S.A.J.Bell & L.M.Copel.) C.F.Wilkins & Whitlock
 (S.B.Andrews) Christenh.
 (S.B.Andrews) Parris
 (S.B.Saksena) Morgan-Jones, W.B.Kendr. & M.H.Hashmi
 (S.B.Saksena) Samson
-(S.Fraga & I.Bravo) G.I.Hansen & Moestrup
+(S.Fraga & I.Bravo) Gert Hansen & Moestrup
 (S.G.Gmel. ex Gugler) Hayek
 (S.G.Gmel.) Bornet
 (S.G.Gmel.) Decne.
 (S.G.Gmel.) F.Muell.
 (S.G.Gmel.) Gurgel & Fredericq
 (S.G.Gmel.) J.V.Lamour.
 (S.G.Gmel.) Kütz.
@@ -17648,14 +17879,16 @@
 (S.G.Gmel.) Turner
 (S.G.Gmel.) Weber Bosse
 (S.G.M.Fawc.) Corner
 (S.G.M.Fawc.) R.H.Petersen
 (S.H.Sun) Deighton
 (S.Hatt.) Inoue
 (S.Hughes & W.B.Kendr.) Hol.-Jech.
+(S.Hughes & W.B.Kendr.) Réblová & Hern.-Restr.
+(S.Hughes, W.B.Kendr. & Shoemaker) Réblová & Hern.-Restr.
 (S.Imai) Trappe
 (S.Ito & Kurib.) Drechsler ex Dastur
 (S.Ito) Hara
 (S.J.Dillon) Christenh. & Byng
 (S.J.Forbes & D.I.Morris) G.L.Nesom
 (S.J.Forbes) G.L.Nesom
 (S.M.Marshall) Greuet
@@ -17673,32 +17906,34 @@
 (S.Moore) Carolin ex Hershk.
 (S.Moore) Chinnock
 (S.Moore) Christenh. & Byng
 (S.Moore) Craven & R.D.Edwards
 (S.Moore) Crisp
 (S.Moore) Danser
 (S.Moore) Diels
-(S.Moore) Diels & Pritz.
+(S.Moore) Diels & E.Pritz.
 (S.Moore) Domin
 (S.Moore) Fosberg & Sachet
 (S.Moore) Hislop, Crayn & Puente-Lel.
+(S.Moore) I.Telford & J.J.Bruhl
 (S.Moore) I.Telford & Pruesapan
 (S.Moore) J.W.Green
 (S.Moore) K.A.Sheph.
 (S.Moore) Kraenzl.
 (S.Moore) Lally
 (S.Moore) M.G.Harr.
 (S.Moore) M.Hiroe
 (S.Moore) McGill.
 (S.Moore) Melville
 (S.Moore) Ostenf.
 (S.Moore) P.S.Short
 (S.Moore) Paczk. & A.R.Chapm.
 (S.Moore) Paul G.Wilson
 (S.Moore) Pedley
+(S.Moore) Peter G.Wilson
 (S.Moore) R.H.Anderson
 (S.Moore) R.W.Bouman
 (S.Moore) Randell
 (S.Moore) Rye
 (S.Moore) S.Moore
 (S.Moore) S.T.Reynolds & R.J.F.Hend.
 (S.Moore) Steenis
@@ -17706,36 +17941,35 @@
 (S.Moore) T.Hammer & R.W.Davis
 (S.Moore) Tronc.
 (S.Moore) Trudgen
 (S.Moore) Trudgen & Rye
 (S.Okamura) Nog.
 (S.Schatz) K.D.Hyde, E.B.G.Jones, Læssøe & Whalley
 (S.Schauer) Domin
+(S.Schauer) Peter G.Wilson
 (S.Skinner) S.Skinner & Entwisle
 (S.T.Blake ex Craven) Udovicic & R.D.Spencer
 (S.T.Blake) A.R.Bean
 (S.T.Blake) B.G.Briggs & L.A.S.Johnson
 (S.T.Blake) B.K.Simon
 (S.T.Blake) Brieger
 (S.T.Blake) C.A.Gardner
 (S.T.Blake) Chai-Anan
 (S.T.Blake) Clayton
 (S.T.Blake) Craven
+(S.T.Blake) Crisp & L.G.Cook
 (S.T.Blake) H.Ohashi
 (S.T.Blake) J.Raynal
 (S.T.Blake) K.D.Hill & L.A.S.Johnson
-(S.T.Blake) K.D.Hill & L.A.S.Johnson x Corymbia torelliana (F.Muell.) K.D.Hill & L.A.S.Johnson
 (S.T.Blake) K.L.Wilson
 (S.T.Blake) K.L.Wilson & J.J.Bruhl
 (S.T.Blake) L.A.S.Johnson & B.G.Briggs
 (S.T.Blake) Lye
 (S.T.Blake) Muasya
 (S.T.Blake) P.I.Forst. & T.C.Wilson
-(S.T.Blake) P.I.Forst. & T.C.Wilson x Coleus foetidus (Benth.) A.J.Paton
-(S.T.Blake) P.I.Forst. & T.C.Wilson x Coleus graveolens (R.Br.) A.J.Paton
 (S.T.Blake) P.M.Peterson
 (S.T.Blake) P.M.Peterson & N.Snow
 (S.T.Blake) Paul G.Wilson
 (S.T.Blake) Pedley
 (S.T.Blake) Peter G.Wilson
 (S.T.Blake) R.D.Webster
 (S.T.Blake) R.L.Barrett & K.L.Wilson
@@ -17795,80 +18029,89 @@
 (Sacc. & D.Sacc.) Vain.
 (Sacc. & Ellis) G.Cunn.
 (Sacc. & Ellis) Trappe & Gerd.
 (Sacc. & Ellis) W.B.Cooke
 (Sacc. & Ellis) de Hoog
 (Sacc. & Fiori) Höhn.
 (Sacc. & Magnus) Briosi & Cavara
+(Sacc. & P.Syd.) J.Lowe
+(Sacc. & P.Syd.) McAlpine
+(Sacc. & P.Syd.) Ryvarden
+(Sacc. & P.Syd.) Shear
+(Sacc. & P.Syd.) Singer
+(Sacc. & P.Syd.) Wolfe
+(Sacc. & Roum.) E.W.Mason & S.Hughes
 (Sacc. & Roum.) M.J.Richardson & E.M.Fraser
-(Sacc. & Roum.) S.Hughes & E.W.Mason
 (Sacc. & Roum.) Traverso & Spessa ex Cámara
 (Sacc. & Speg.) Oorschot
 (Sacc. & Therry) Malloch & Cain
 (Sacc. & Trotter) Jülich & Stalpers
-(Sacc.) A.A.Padhye, Ajello, McGinnis & Borelli
 (Sacc.) Aberdeen
 (Sacc.) Allesch.
 (Sacc.) Arx
 (Sacc.) Arx & D.L.Olivier
+(Sacc.) Arzanlou, W.Gams & Crous
 (Sacc.) Bainier
 (Sacc.) Berl. & Voglino
 (Sacc.) Borelli
 (Sacc.) Brittleb.
 (Sacc.) Bubák
 (Sacc.) Cain
-(Sacc.) Cain & Kimbr.
 (Sacc.) Cleland & Cheel
 (Sacc.) Cooke
 (Sacc.) Corner
 (Sacc.) Crous & U.Braun
-(Sacc.) Crous, Arzanlou & W.Gams
 (Sacc.) Deighton
 (Sacc.) Dennis
 (Sacc.) Died.
 (Sacc.) E.-J.Gilbert
-(Sacc.) E.J.Butler, Syd. & P.Syd.
 (Sacc.) E.W.Mason
 (Sacc.) Ferraris
 (Sacc.) Garn.-Jones & Malcolm
 (Sacc.) Henn.
 (Sacc.) Jenkins
-(Sacc.) Kantvilas & Y.S.Chang
+(Sacc.) Kimbr. & Cain
 (Sacc.) Kirschst.
 (Sacc.) Korf
 (Sacc.) Kuntze
 (Sacc.) Largent & Abell-Davis
 (Sacc.) M.B.Ellis
-(Sacc.) Malcolm & Garn.-Jones
 (Sacc.) Massee
 (Sacc.) McAlpine
+(Sacc.) McGinnis, A.A.Padhye, Borelli & Ajello
 (Sacc.) Niessl
 (Sacc.) Pegler
+(Sacc.) Pegler & Lodge
+(Sacc.) Qian Chen & L.Cai
 (Sacc.) R.H.Petersen
+(Sacc.) Redhead & Mullineux
 (Sacc.) Rehm
 (Sacc.) S.Hughes
 (Sacc.) Sacc.
 (Sacc.) Sacc. & D.Sacc.
 (Sacc.) Shoemaker
-(Sacc.) Singer
 (Sacc.) Speg. ex Sacc.
 (Sacc.) Spooner
 (Sacc.) Steyaert
 (Sacc.) Subram. & B.L.Jain
 (Sacc.) Syd. & P.Syd.
+(Sacc.) Syd., P.Syd. & E.J.Butler
 (Sacc.) Tassi
 (Sacc.) Theiss.
 (Sacc.) U.Braun
 (Sacc.) Vain.
+(Sacc.) Y.S.Chang & Kantvilas
 (Sacc.) Z.Xu, T.C.Harr., M.L.Gleason & Batzer
 (Sacc.) de Hoog
 (Sacc.) de Hoog, Kwon-Chung & McGinnis
 (Sacc., M.Rousseau & E.Bommer) S.Hughes
 (Sadler) Asch. & Graebn.
+(Sainsbury) Brinda, Ignatov & Fedosov
 (Sainsbury) Catches.
+(Sainsbury) J.Milne & Klazenga
 (Saito & M.Ota) Uden & H.R.Buckley ex S.A.Mey. & Ahearn
 (Saito) C.E.Skinner
 (Sakurai) Z.Iwats. & K.Saito
 (Salisb. ex Knight) Kuntze
 (Salisb.) Baker
 (Salisb.) Benth. & Hook.f.
 (Salisb.) Britten
@@ -17886,51 +18129,54 @@
 (Salisb.) G.J.Lewis
 (Salisb.) J.F.Macbr.
 (Salisb.) J.H.Willis & Court
 (Salisb.) Ker Gawl.
 (Salisb.) Knight
 (Salisb.) Kuntze
 (Salisb.) L.A.S.Johnson
-(Salisb.) L.A.S.Johnson x Allocasuarina thalassoscopica L.A.S.Johnson
 (Salisb.) Lehm.
 (Salisb.) Miq.
 (Salisb.) N.E.Br.
 (Salisb.) Pedley
 (Salisb.) Poir.
 (Salisb.) R.Br.
 (Salisb.) Rickett & Stafleu
 (Salisb.) Salisb.
 (Salisb.) Schult.
 (Salisb.) Sims
 (Salisb.) Skeels
 (Salisb.) Sm.
 (Salisb.) Stearn
 (Salisb.) Wikstr.
+(Salm-Dyck) A.Terracc.
 (Samp.) Knoph & Leuckert
+(Samson, S.B.Hong & Varga) Houbraken, Visagie & Samson
 (Samuels & Seifert) Rossman & Samuels
+(Samuels) L.W.Hou, L.Cai & Crous
 (Samuels) Rossman & Samuels
 (Sande Lac.) B.M.Thiers & Gradst.
 (Sande Lac.) Gottsche
 (Sande Lac.) Herzog
 (Sande Lac.) K.I.Goebel
 (Sande Lac.) Kachroo & R.M.Schust.
 (Sande Lac.) M.Fleisch.
 (Sande Lac.) R.M.Schust.
 (Sande Lac.) Schiffn.
 (Sande Lac.) Steph.
+(Sande Lac.) Tixier
 (Sande Lac.) Trevis.
 (Sande Lac.) Verd.
 (Sander) Goldblatt
 (Sander) Peter B.Adams
 (Sander) Rolfe
-(Sandst.) Hustich
 (Sandst.) Mong.
 (Sandst.) Ruoss
+(Sangal. & L.W.Burgess) Benyon & L.W.Burgess
 (Sarg.) Szlach.
-(Sartory, J.Mey., R.Sartory & Weill) Minter
+(Sartory, R.Sartory, Weill & J.Mey.) Minter
 (Sato) Kurok.
 (Sato) Swinscow & Krog
 (Sauerb.) Wijk & Margad.
 (Sauv.) Draisma, Prud'homme & H.Kawai
 (Sauv.) Komárek
 (Sauv.) Setch. & N.L.Gardner
 (Savi) Airy Shaw
@@ -17945,16 +18191,14 @@
 (Sch.Bip.) Benth. ex Baker
 (Sch.Bip.) Cabrera
 (Sch.Bip.) Paul G.Wilson
 (Sch.Bip.) R.E.Ballard ex Melchert
 (Sch.Bip.) R.J.Bayer
 (Schaarschm.) A.Fisch.
 (Schaarschm.) Letcher
-(Schaeff. : Fr.) P.Kumm.
-(Schaeff. ex Fr.) Gray
 (Schaeff.) Cheel
 (Schaeff.) Corner
 (Schaeff.) Donk
 (Schaeff.) Fr.
 (Schaeff.) Gray
 (Schaeff.) Henn.
 (Schaeff.) J.Schröt.
@@ -17967,14 +18211,15 @@
 (Schaeff.) Pers.
 (Schaeff.) Quél.
 (Schaeff.) R.H.Petersen
 (Schaeff.) Redhead, Vilgalys & Moncalvo
 (Schaeff.) Singer
 (Schaeff.) Singer & A.H.Sm.
 (Schaeff.) Staude
+(Schaeff.) Vizzini
 (Schaeff.) Wasser
 (Schaeff.) With.
 (Schaer. ex Nyl.) Hale
 (Schaer.) A.Massal.
 (Schaer.) Anzi
 (Schaer.) D.J.Galloway
 (Schaer.) Frey
@@ -17998,14 +18243,15 @@
 (Schauer) Brooker
 (Schauer) C.A.Gardner
 (Schauer) C.T.White
 (Schauer) Cheel
 (Schauer) Cranfield
 (Schauer) Craven
 (Schauer) Craven & R.D.Edwards
+(Schauer) Crisp & L.G.Cook
 (Schauer) Domin
 (Schauer) Druce
 (Schauer) F.C.Johnstone & Hallam
 (Schauer) F.M.Bailey
 (Schauer) F.Muell.
 (Schauer) G.Don ex Loudon
 (Schauer) J.R.Wheeler & N.G.Marchant
@@ -18055,33 +18301,31 @@
 (Schindl.) H.Ohashi & K.Ohashi
 (Schindl.) Hutch.
 (Schindl.) J.M.Black
 (Schindl.) M.L.Moody
 (Schindl.) M.L.Moody & Les
 (Schindl.) Meeuwen
 (Schindl.) Orchard
-(Schindl.) Orchard x Gonocarpus elatus (A.Cunn. ex Fenzl) Orchard
 (Schindl.) Pedley
 (Schipper) Arx
 (Schkuhr) C.Presl
 (Schkuhr) Kuntze
 (Schkuhr) Large & Braggins
 (Schkuhr) Link
 (Schkuhr) Röhl.
-(Schleich. ex Schwägr.) J.R.Spence
 (Schlieph. & Geh.) Zanten
-(Schlieph.) Warnst.
 (Schlittler) T.S.Liu & S.S.Ying
 (Schltdl. & Cham.) Benth.
 (Schltdl. ex Link) Craven
 (Schltdl. ex Link) DC.
 (Schltdl.) A.D.Chapm.
 (Schltdl.) A.Gray
 (Schltdl.) A.R.Bean
 (Schltdl.) Benth.
+(Schltdl.) Bref.
 (Schltdl.) Christenh. & Byng
 (Schltdl.) Copley
 (Schltdl.) D.L.Jones & M.A.Clem.
 (Schltdl.) E.Fisch.
 (Schltdl.) Ewart
 (Schltdl.) F.Muell.
 (Schltdl.) Fr.
@@ -18089,34 +18333,35 @@
 (Schltdl.) J.A.Stev. & Aar.G.Johnson
 (Schltdl.) J.M.Black
 (Schltdl.) J.W.Grimes
 (Schltdl.) J.Z.Weber
 (Schltdl.) K.Krause
 (Schltdl.) Kuntze
 (Schltdl.) Maire
-(Schltdl.) McKenzie & Vánky
 (Schltdl.) Meisn.
 (Schltdl.) Miers
 (Schltdl.) Moq.
 (Schltdl.) Orchard
 (Schltdl.) Paul G.Wilson
 (Schltdl.) Pedley
+(Schltdl.) Peter G.Wilson
 (Schltdl.) Rabenh.
 (Schltdl.) Radlk.
 (Schltdl.) Randell
 (Schltdl.) Reissek
 (Schltdl.) Rye
 (Schltdl.) Schltdl.
 (Schltdl.) Sleumer
 (Schltdl.) Snijman & Kocyan
 (Schltdl.) Sond.
 (Schltdl.) Szlach.
 (Schltdl.) Threlfall
 (Schltdl.) Voss
 (Schltdl.) Vánky
+(Schltdl.) Vánky & McKenzie
 (Schltdl.) Walp.
 (Schltr. & J.J.Sm.) Schuit., Y.P.Ng & H.A.Pedersen
 (Schltr.) A.R.Bean
 (Schltr.) Ames & C.Schweinf.
 (Schltr.) Brieger
 (Schltr.) C.T.White
 (Schltr.) Codd
@@ -18140,16 +18385,16 @@
 (Schltr.) Rauschert
 (Schltr.) Schltr.
 (Schltr.) Seidenf.
 (Schltr.) Szlach.
 (Schltr.) W.Kittr.
 (Schmarda) B.Marin & Melkonian
 (Schmarda) Deflandre
+(Schmarda) F.Stein
 (Schmarda) Kof. & Swezy
-(Schmarda) Stein
 (Schmidle) Anagn. & Komárek
 (Schmidle) Bohlin
 (Schmidle) Grönblad
 (Schmidle) Islam
 (Schmidle) Lemmerm.
 (Schmidle) Marvan, Komárek & Comas
 (Schmidle) Novacek ex Geitler
@@ -18157,37 +18402,36 @@
 (Schmidle) Schmidle
 (Schmidle) Teiling
 (Schmidle) Teiling ex Ruzicka & Pouzar
 (Schmidle) Transeau
 (Schmidle) West & G.S.West
 (Schmidle) Willi Krieg.
 (Schmidle) Willi Krieg. & Gerloff
-(Schmidt) F.Gómez
 (Schneev.) Ker Gawl.
 (Schneev.) Moench
 (Schneev.) Sprague
 (Schneev.) Stearn
 (Schneev.) Vent.
 (Schnizl.) D.R.Hunt
 (Schodde) P.S.Short
 (Schott & Endl.) A.Terracc.
 (Schott & Endl.) Benth.
 (Schott & Endl.) Domin
 (Schott & Endl.) Druce
 (Schott & Endl.) Endl.
 (Schott & Endl.) Kuntze
 (Schott & Endl.) R.Br.
-(Schott & Endl.) R.Br. x Brachychiton acerifolius (A.Cunn. ex G.Don) F.Muell.
 (Schott ex Rchb.) Asch.
 (Schott) Benth. & Hook.f.
 (Schott) Daniker
 (Schott) Engl.
 (Schott) F.Muell.
 (Schott) G.Don
 (Schott) Kuntze
+(Schott) M.D.Barrett
 (Schousb. ex Bornet) Feldm.-Maz.
 (Schousb. ex C.Agardh) J.Agardh
 (Schousb. ex J.Agardh) F.Schmitz
 (Schrad. & J.C.Wendl.) Benth.
 (Schrad. & J.C.Wendl.) Colvill ex Sweet
 (Schrad. & J.C.Wendl.) DC.
 (Schrad. & J.C.Wendl.) Hoffmanns.
@@ -18202,25 +18446,25 @@
 (Schrad. ex Schult. & Schult.f.) Boeckeler
 (Schrad.) Ach.
 (Schrad.) Bonap.
 (Schrad.) Cooke
 (Schrad.) Coppins & P.James
 (Schrad.) Coss. & Durieu
 (Schrad.) Donk
-(Schrad.) E.Langer & Vesterh.
 (Schrad.) Fr.
 (Schrad.) Gaudin
 (Schrad.) Gilb. & Ryvarden
 (Schrad.) Gillet
 (Schrad.) Hafellner
 (Schrad.) Halacsy
 (Schrad.) Hook.f.
 (Schrad.) Iltis
 (Schrad.) Jülich
 (Schrad.) Kuntze
+(Schrad.) Langer & Vesterh.
 (Schrad.) Lév.
 (Schrad.) Maire & Weiller
 (Schrad.) Massee
 (Schrad.) Mudd
 (Schrad.) Murrill
 (Schrad.) Nees
 (Schrad.) Nyl.
@@ -18274,15 +18518,15 @@
 (Schröd.) F.Gómez
 (Schröd.) G.M.Sm.
 (Schröd.) G.S.West
 (Schröd.) Hallegr. & Huisman
 (Schröd.) Hasle
 (Schröd.) Hust.
 (Schröd.) J.Schiller
-(Schröd.) Jörg.
+(Schröd.) Jørg.
 (Schröd.) Kof.
 (Schröd.) Lemmerm.
 (Schröd.) Playfair
 (Schröd.) S.H.Li
 (Schröd.) Steem.Niels.
 (Schröd.) Taylor
 (Schröt.) Komárek
@@ -18314,22 +18558,21 @@
 (Schultz) Hyl. ex Nordh.
 (Schultz) R.H.Zander
 (Schultz) Skuja
 (Schultze) Ostenf.
 (Schultze) Simonsen
 (Schulzer) Donk
 (Schulzer) Gillet
-(Schulzer) Roze & Richon
+(Schulzer) Richon & Roze
 (Schum.) A.Mayer
 (Schum.) Cleve
 (Schum.) Grunow
 (Schum.) Hust.
 (Schum.) Sabelina
 (Schumach. & Thonn.) Baker
-(Schumach. & Thonn.) Baker - Vigna vexillata var. youngiana F.M.Bailey
 (Schumach. & Thonn.) J.B.Hutch.
 (Schumach. & Thonn.) Roberty
 (Schumach.) B.K.Simon
 (Schumach.) Baker f. ex Exell
 (Schumach.) Borss.Waalk.
 (Schumach.) Boud.
 (Schumach.) Donk
@@ -18345,50 +18588,49 @@
 (Schumach.) R.W.Bouman
 (Schumach.) Rostaf. ex Lister
 (Schumach.) Ryvarden
 (Schumach.) Singer
 (Schumach.) Snell
 (Schumach.) Stapf & C.E.Hubb.
 (Schumach.) T.Koyama
+(Schumach.) Vizzini, P.Alvarado, G.Moreno & Cons.
 (Schumach.) de Bary
 (Schwager) Foslie
 (Schweick.) C.Jeffrey & P.Halliday
-(Schwein. : Fr.) G.W.Martin
 (Schwein. ex Fr.) Cooke
 (Schwein. ex Fr.) Murrill
 (Schwein. ex Fr.) Rajchenb.
 (Schwein.) A.H.Sm.
 (Schwein.) A.L.Welden
 (Schwein.) Andrus & W.D.Moore
 (Schwein.) Arthur
+(Schwein.) B.K.Cui, H.J.Li & Y.C.Dai
 (Schwein.) Berk.
 (Schwein.) Berk. & M.A.Curtis
 (Schwein.) Boidin
 (Schwein.) Boidin & Lanq.
+(Schwein.) Bondartsev & Singer
 (Schwein.) Bres.
 (Schwein.) Burrill
 (Schwein.) Burt
 (Schwein.) Carmarán & A.I.Romero
 (Schwein.) Chamuris
 (Schwein.) Cooke
 (Schwein.) Corner
 (Schwein.) D.A.Reid
-(Schwein.) D.P.Rogers & Teixeira
+(Schwein.) D.P.Rogers & H.S.Jacks.
 (Schwein.) De Toni
-(Schwein.) Earle & Underw.
 (Schwein.) Ellis & Everh.
 (Schwein.) Fr.
 (Schwein.) G.Cunn.
 (Schwein.) G.Lister
 (Schwein.) G.W.Martin
 (Schwein.) Gilb. & Ryvarden
-(Schwein.) H.S.Jacks. & D.P.Rogers
 (Schwein.) H.Zogg
 (Schwein.) Halsey
-(Schwein.) J.Lloyd
 (Schwein.) J.R.Dixon
 (Schwein.) Kuntze
 (Schwein.) Litsch.
 (Schwein.) Lloyd
 (Schwein.) M.A.Curtis
 (Schwein.) M.L.Lohman
 (Schwein.) Massee
@@ -18404,28 +18646,31 @@
 (Schwein.) Pilát
 (Schwein.) R.H.Petersen
 (Schwein.) Rostaf.
 (Schwein.) Ryvarden
 (Schwein.) Sacc.
 (Schwein.) Schwein.
 (Schwein.) Singer
-(Schwein.) Singer & Bondartsev
 (Schwein.) Steud.
 (Schwein.) Sull.
 (Schwein.) T.Wagner & M.Fisch.
+(Schwein.) Teixeira & D.P.Rogers
+(Schwein.) U.Braun & R.T.A.Cook
 (Schwein.) Underw.
+(Schwein.) Underw. & Earle
 (Schwägr.) A.Jaeger ex Dixon
-(Schwägr.) Angstr.
 (Schwägr.) Arn.
 (Schwägr.) Bosch & Sande Lac.
 (Schwägr.) Brid.
+(Schwägr.) Brinda, Jáuregui-Lazo & Mishler
 (Schwägr.) Broth.
 (Schwägr.) Bruch & Schimp.
 (Schwägr.) Carrington & Pearson
 (Schwägr.) Dixon
+(Schwägr.) F.Lara, Garilleti & Goffinet
 (Schwägr.) F.Muell.
 (Schwägr.) Fulford & J.Taylor
 (Schwägr.) Hampe ex Müll.Hal.
 (Schwägr.) Hook. & Grev.
 (Schwägr.) Hornsch. ex Müll.Hal.
 (Schwägr.) J.R.Spence
 (Schwägr.) J.R.Spence & H.P.Ramsay
@@ -18439,43 +18684,42 @@
 (Schwägr.) P.Sollman
 (Schwägr.) Paris
 (Schwägr.) R.M.Schust.
 (Schwägr.) Reichardt
 (Schwägr.) Schiffn.
 (Schwägr.) Schwägr.
 (Schwägr.) Spreng.
-(Schwägr.) Ther.
 (Schwägr.) Thér.
 (Schwägr.) Trevis.
 (Schwägr.) Ångstr.
-(Scop. : Fr.) Cooke
 (Scop.) Berk.
 (Scop.) Bres.
 (Scop.) Briq.
 (Scop.) Cooke
 (Scop.) DC.
 (Scop.) Emel
 (Scop.) Fr.
 (Scop.) G.Stev.
 (Scop.) Gillet
 (Scop.) Gray
 (Scop.) Hoffm.
 (Scop.) Holub
 (Scop.) J.Schröt.
 (Scop.) J.Steiner
+(Scop.) Konrad & Maubl.
 (Scop.) Krasser
 (Scop.) Ladó
-(Scop.) Maubl. & Konrad
 (Scop.) P.Beauv.
 (Scop.) P.Karst.
 (Scop.) P.Kumm.
 (Scop.) Pat.
 (Scop.) Pers.
 (Scop.) Prantl
 (Scop.) Quél.
+(Scop.) R.A.Koch & Aime
 (Scop.) R.Sant.
 (Scop.) Rauschert
 (Scop.) Redhead, Vilgalys & Moncalvo
 (Scop.) Rostaf. ex Lister
 (Scop.) Singer
 (Scop.) Timdal
 (Scop.) Wünsche
@@ -18511,54 +18755,54 @@
 (Ser.) H.Lev.
 (Ser.) Link
 (Ser.) M.Roem.
 (Ser.) Nakai
 (Ser.) P.Sebastian & I.Telford
 (Ser.) Wight
 (Servít) P.M.Jørg. & Vězda
-(Sesse & Moc.) P.S.Green
+(Sessé & Moc.) P.S.Green
 (Setch. & Estee) Cribb & J.W.Cribb
 (Setch. & Foslie) L.R.Mason
 (Setch. & N.L.Gardner) A.Hamel & Hamel
 (Setch. & N.L.Gardner) Cribb
 (Setch. & N.L.Gardner) Doty & Meñez
 (Setch. & N.L.Gardner) G.De Toni
 (Setch. & N.L.Gardner) Hollenb. & I.A.Abbott
 (Setch.) Dietel
 (Setch.) Hartog
 (Setch.) Hollenb.
 (Setch.) Huisman
+(Setch.) Neville & Poumarat
 (Setch.) Pouzar
 (Setch.) Setch.
 (Setch.) Setch. & N.L.Gardner
 (Shadbolt) Freng.
 (Shadbolt) Ralfs ex A.Pritch.
 (Shadbolt) Van Heurck
 (Shear) Boedijn
 (Shear) Zeller
 (Shearer & J.L.Crane) J.Campb., J.L.Anderson & Shearer
+(Shearer & K.D.Hyde) K.Hiray., Kaz.Tanaka & Shearer
 (Shearer) Boonmee & K.D.Hyde
-(Shearer) Shearer, J.Campb. & J.L.Anderson
-(Shipton & C.Booth) Arx
+(Shearer) J.Campb., J.L.Anderson & Shearer
 (Shipton) Boesew.
-(Shipton) C.L.Schoch & Crous
+(Shipton) Crous & C.L.Schoch
 (Shipton) Rossman & Samuels
 (Shirai) S.Ito
 (Shirley) A.W.Archer
 (Shirley) Kantvilas
 (Shirley) Kantvilas & Lumbsch
 (Shirley) Sipman
 (Shirley) Zahlbr.
 (Sibth. & Sm.) P.W.Ball
 (Sibth. & Sm.) Sibth. & Sm.
 (Sibth. ex Sm.) K.Richt.
 (Sibth.) Fr.
 (Sieber & Zucc.) S.Y.Hu
 (Sieber & Zucc.) Seem.
-(Sieber ex DC.) Anderb. & Haegi
 (Sieber ex DC.) Benth.
 (Sieber ex DC.) Britten
 (Sieber ex DC.) Brongn. ex Meisn.
 (Sieber ex DC.) Domin
 (Sieber ex DC.) Fenzl
 (Sieber ex DC.) H.Deane & Maiden
 (Sieber ex DC.) Harms
@@ -18603,24 +18847,27 @@
 (Sieber ex Spreng.) Maiden
 (Sieber ex Spreng.) Maiden & Betche
 (Sieber ex Spreng.) Mart.
 (Sieber ex Spreng.) N.A.Wakef.
 (Sieber ex Spreng.) Paul G.Wilson
 (Sieber ex Spreng.) Pedley
 (Sieber ex Spreng.) Rydb.
+(Sieber ex Spreng.) Sch.Bip.
 (Sieber ex Spreng.) Ser.
+(Sieber ex Spreng.) Sieber ex DC.
 (Sieber ex Spreng.) Steetz
 (Sieber ex Spreng.) Tiegh.
 (Sieber ex Spreng.) Voss
 (Sieber) Spreng. ex G.Don
 (Siebold & Zucc.) Kuntze
 (Siebold & Zucc.) Planch.
 (Siebold & Zucc.) T.Koyama ex C.E.Chang
 (Siebold) H.Ohashi
 (Siebold) T.Mori
+(Sigler, Deanna A.Sutton, Gibas, Summerb. & Iwen) Houbraken, Tanney, Visagie & Samson
 (Simonet & Guin.) Hyl.
 (Simonet & Guin.) Melderis
 (Simonk.) Rech.f.
 (Simonsen) G.W.Andrews
 (Simonsen) Witkowski
 (Sims) Benth.
 (Sims) Colvill ex Sweet
@@ -18650,30 +18897,32 @@
 (Sims) Sweet
 (Sims) T.M.Salter
 (Sims) Voss
 (Sims) Wawra
 (Sims) Willd.
 (Singer & A.H.Sm.) Castellano, Trappe & T.Lebel
 (Singer & Both) Thiers
-(Singer & Clémenc.) Redhead, Moncalvo, Vilgalys & Lutzoni
+(Singer & Clémencon) Redhead, Moncalvo, Vilgalys & Lutzoni
 (Singer ex Hora) Bon
 (Singer ex Hora) Singer
 (Singer ex Hora) Watling
 (Singer) E.Horak
+(Singer) Q.Y.Zhang & Y.C.Dai
 (Singer) Raithelh.
 (Singer) Redhead, Vilgalys & Moncalvo
 (Singer) Rexer
 (Singer) Singer
 (Singer) Singer ex Métrod
 (Singer) T.W.May & A.E.Wood
 (Sipman) Aptroot & Lücking
 (Sipman) Kalb & Bungartz
 (Sipman) Kantvilas & Lumbsch
 (Sirodot) M.Mori
-(Sivasith., Websdane, K.W.Dixon & Pate) Vánky
+(Sivan. & R.G.Shivas) Crous
+(Sivan. & R.G.Shivas) Crous & Carnegie
 (Skan) P.S.Green
 (Skottsb. & Levring) V.May
 (Skottsb.) A.F.Peters
 (Skottsb.) Kuck.
 (Skottsb.) Kuck. & Skottsb.
 (Skottsb.) M.J.Wynne
 (Skottsb.) Skottsb.
@@ -18691,14 +18940,15 @@
 (Skvortsov & C.I.Mey.) Poulin
 (Skvortsov) Deflandre
 (Skvortsov) Pochm.
 (Skvortzov & K.I.Mey.) Hust.
 (Slabber) Ehrenb.
 (Sleumer) Hislop, Crayn & Puente-Lel.
 (Sleumer) Pedley
+(Slippers, Crous & M.J.Wingf.) Crous, Slippers & A.J.L.Phillips
 (Sm. ex Ach.) Ach.
 (Sm. ex Vent.) J.L.Parm.
 (Sm. ex Vent.) Knight
 (Sm. ex Vent.) R.Br.
 (Sm.) A.Juss.
 (Sm.) A.L.Sm.
 (Sm.) A.Lyons
@@ -18732,16 +18982,14 @@
 (Sm.) D.L.Jones & M.A.Clem.
 (Sm.) DC.
 (Sm.) Desv.
 (Sm.) Domin
 (Sm.) Donn ex Sm.
 (Sm.) Donn.Sm. ex Sm.
 (Sm.) Druce
-(Sm.) Druce x Kunzea capitata (Sm.) Heynh.
-(Sm.) Druce x Kunzea capitata subsp. seminuda Toelken
 (Sm.) Duretto & Heslewood
 (Sm.) Duthie
 (Sm.) E.Pritz.
 (Sm.) F.M.Bailey
 (Sm.) F.Meigen
 (Sm.) F.Muell.
 (Sm.) Feldm.-Maz. & Meslin
@@ -18749,17 +18997,14 @@
 (Sm.) G.Nicholson
 (Sm.) Gray
 (Sm.) Griseb.
 (Sm.) Hale
 (Sm.) Hamel
 (Sm.) Hasselr.
 (Sm.) Heynh.
-(Sm.) Heynh. subsp. capitata x Kunzea capitata subsp. seminuda Toelken
-(Sm.) Heynh. subsp. capitata x Kunzea rupestris Blakely
-(Sm.) Heynh. subsp. ericifolia x Kunzea recurva Schauer
 (Sm.) Hook.
 (Sm.) Hook. & Taylor
 (Sm.) Hook.f.
 (Sm.) I.Hagen
 (Sm.) J.Agardh
 (Sm.) J.G.West
 (Sm.) J.J.Sm.
@@ -18768,15 +19013,14 @@
 (Sm.) K.A.Sheph. & C.F.Wilkins
 (Sm.) K.Krause
 (Sm.) Kindb.
 (Sm.) Knight
 (Sm.) Krog
 (Sm.) Kuntze
 (Sm.) Körb.
-(Sm.) Kütz
 (Sm.) Kütz.
 (Sm.) Lindb.
 (Sm.) Lindl.
 (Sm.) Link
 (Sm.) Lyngb.
 (Sm.) Lynge
 (Sm.) M.A.Clem. & D.L.Jones
@@ -18797,21 +19041,20 @@
 (Sm.) P.Beauv.
 (Sm.) P.C.Silva
 (Sm.) P.G.Richt.
 (Sm.) Passioura & J.E.Ash
 (Sm.) Paul G.Wilson
 (Sm.) Pedley
 (Sm.) Pers.
+(Sm.) Peter G.Wilson
 (Sm.) Peter G.Wilson & J.T.Waterh.
 (Sm.) Poelt
 (Sm.) Poir.
 (Sm.) R.Br.
 (Sm.) R.Br. ex Mirb.
-(Sm.) R.Br. x Hovea heterophylla A.Cunn. ex Hook.f.
-(Sm.) R.Br. x Hovea planifolia (Domin) J.H.Ross
 (Sm.) R.H.Zander
 (Sm.) R.M.Tryon
 (Sm.) Raf.
 (Sm.) Rauschert
 (Sm.) Rchb.
 (Sm.) Rech.f.
 (Sm.) Reichardt
@@ -18823,16 +19066,14 @@
 (Sm.) Siebert & Voss
 (Sm.) Sims
 (Sm.) Sm.
 (Sm.) Solier
 (Sm.) Spreng.
 (Sm.) Spruce
 (Sm.) Sweet
-(Sm.) Sweet x Angophora leiocarpa (L.A.S.Johnson ex G.J.Leach) K.R.Thiele & Ladiges
-(Sm.) Sweet x Angophora woodsiana F.M.Bailey
 (Sm.) Tausch
 (Sm.) Th.Fr.
 (Sm.) Tratt.
 (Sm.) Trevis.
 (Sm.) Triana
 (Sm.) Turner
 (Sm.) Veldkamp
@@ -18849,16 +19090,14 @@
 (Smejkal) Mennema
 (Snell & E.A.Dick) Singer
 (Soják) Soják
 (Sol. ex A.Cunn.) Sch.Bip.
 (Sol. ex Aiton) Schrad. & J.C.Wendl.
 (Sol. ex Aiton) Sm.
 (Sol. ex Aiton) W.T.Aiton
-(Sol. ex Benth.) I.C.Nielsen
-(Sol. ex Benth.) Kosterm.
 (Sol. ex Boott) Boott
 (Sol. ex Boott) Kük.
 (Sol. ex Correa) Kuntze
 (Sol. ex DC.) Benth.
 (Sol. ex Gaertn.) A.Lyons
 (Sol. ex Gaertn.) Byrnes
 (Sol. ex Gaertn.) Cheel
@@ -18890,24 +19129,25 @@
 (Sommerf.) Lynge
 (Sommerf.) Massee
 (Sommerf.) Menegh.
 (Sommerf.) P.Karst.
 (Sommerf.) Poelt
 (Sommerf.) Rostaf.
 (Sommerf.) S.Ekman & M.Svennson
+(Sommerf.) Zmitr. & Kovalenko
 (Sommier) Merxm.
-(Sond. & F.Muell. ex Sond.) Benth.
-(Sond. & F.Muell. ex Sond.) F.Muell.
-(Sond. & F.Muell. ex Sond.) Kroner
 (Sond. & F.Muell.) Benth.
 (Sond. & F.Muell.) F.Muell.
+(Sond. & F.Muell.) Kroner
 (Sond. & F.Muell.) Müll.Arg.
 (Sond. & F.Muell.) Paul G.Wilson
 (Sond. & F.Muell.) Sond. ex Druce
 (Sond. ex Kütz.) J.Agardh
+(Sond. ex W.D.J.Koch) Benth.
+(Sond.) 
 (Sond.) A.DC.
 (Sond.) A.Millar
 (Sond.) Anway
 (Sond.) Aresch.
 (Sond.) Askenasy
 (Sond.) Belcher
 (Sond.) Benth.
@@ -18976,14 +19216,15 @@
 (Sond.) Weber Bosse
 (Sond.) Womersley
 (Sond.) Womersley & A.Bailey
 (Sond.) Womersley & Shepley
 (Sond.) Yamada
 (Sond.) Yendo
 (Sond.) Zanardini
+(Soop) Niskanen & Liimat.
 (Sowerby) A.Pearson & Dennis
 (Sowerby) Antonín, Halling & Noordel.
 (Sowerby) Cooke
 (Sowerby) Corner
 (Sowerby) D.A.Reid
 (Sowerby) Fr.
 (Sowerby) Fuckel
@@ -18993,14 +19234,15 @@
 (Sowerby) P.Karst.
 (Sowerby) P.Kumm.
 (Sowerby) Pat.
 (Sowerby) Quél.
 (Sowerby) R.H.Petersen
 (Sowerby) Rea
 (Sowerby) Rostaf.
+(Sowerby) S.H.He & Jiao Yang
 (Sowerby) Sacc.
 (Sowerby) Singer
 (Sowerby) T.Schumach.
 (Sowerby) W.Phillips
 (Spach) Benth. & Hook.f.
 (Spach) Briq.
 (Spach) Gremli
@@ -19023,28 +19265,31 @@
 (Specht) Halford & R.J.F.Hend.
 (Specht) J.R.Clarkson
 (Specht) Pedley
 (Speg.) Arriaga & Barkworth
 (Speg.) Arx & E.Müll.
 (Speg.) Beck
 (Speg.) Bissett
+(Speg.) Blanco-Dios
 (Speg.) Corner
 (Speg.) Crous & Van Niekerk
 (Speg.) Cummins & Ramachar
 (Speg.) D.A.Reid
 (Speg.) E.W.Mason
 (Speg.) Henn.
 (Speg.) Joanne E.Taylor & K.D.Hyde
 (Speg.) Ladó
 (Speg.) M.B.Ellis
 (Speg.) M.L.Farr
+(Speg.) McTaggart & R.G.Shivas
 (Speg.) Nag Raj
 (Speg.) Niessl
 (Speg.) Petr. & Syd.
 (Speg.) Peñail.
+(Speg.) Pintos & P.Alvarado
 (Speg.) Planchuelo & P.M.Peterson
 (Speg.) Rajchenb. & J.E.Wright
 (Speg.) S.I.Ahmed & Cain
 (Speg.) Sacc.
 (Speg.) Singer
 (Speg.) Speg.
 (Speg.) Steyaert
@@ -19053,15 +19298,14 @@
 (Speg.) Vánky
 (Speg.) W.B.Cooke
 (Speg.) Y.M.Ju, J.D.Rogers & H.M.Hsieh
 (Spin) A.DC.
 (Spin) Benth.
 (Spin) Domin
 (Spin) Spin
-(Spooner & Læssøe) Y.M.Ju, J.D.Rogers & H.M.Hsieh
 (Sprague) Adema & Sirich.
 (Sprague) Jackes
 (Sprague) Sirich. & Adema
 (Sprague) Sprague
 (Spreng. ex Trin.) Barkworth
 (Spreng.) A.Braun
 (Spreng.) A.Cunn. ex DC.
@@ -19157,41 +19401,43 @@
 (Stapf & C.E.Hubb.) Veldkamp
 (Stapf & Jesson) Ewart & O.B.Davies
 (Stapf ex N.G.Walsh) N.G.Walsh & A.R.Williams
 (Stapf ex Thell.) C.A.Gardner
 (Stapf ex Thell.) C.E.Hubb. ex S.T.Blake
 (Stapf ex Thell.) J.M.Black
 (Stapf) B.K.Simon
+(Stapf) Byng & Christenh.
 (Stapf) Clayton
 (Stapf) Henrard
 (Stapf) L.G.Clark & Judz.
 (Stapf) P.M.Peterson
 (Stapf) R.D.Webster
 (Stapf) S.M.Phillips
 (Stapf) Stent
 (Stapf) Vickery
 (Staples) Staples
 (Starb.) R.C.Harris
 (Starback) Elix
 (Starback) Pusswald
 (Starbäck) Rossman & Samuels
+(Starmer, Phaff, M.Miranda, M.W.Mill. & J.S.F.Barker) Y.Yamada
 (Stauffer) Byng & Christenh.
+(Stauffer) N.Hallé
 (Stearn) Tuyn
 (Steem.Niels.) F.Gómez
 (Steenis) P.H.Weston & A.R.Mast
 (Steere) Blockeel
 (Steetz ex Sond.) Paul G.Wilson
 (Steetz) A.Gray
 (Steetz) Anderb.
 (Steetz) Baill.
 (Steetz) Benth.
 (Steetz) Chodat
 (Steetz) Diels
 (Steetz) Diels & E.Pritz.
-(Steetz) Diels & Pritz.
 (Steetz) Domin
 (Steetz) Druce
 (Steetz) Ewart & Jean White
 (Steetz) F.Muell.
 (Steetz) F.Muell. ex Benth.
 (Steetz) Hook.f.
 (Steetz) I.Thomps.
@@ -19208,16 +19454,14 @@
 (Steetz) Sond.
 (Steetz) Steenis
 (Steetz) Voss
 (Steetz) Wawra
 (Stein) D.D.Awasthi
 (Stein) Krog & Swinsc.
 (Stein) Nik.Hoffm. & Hafellner
-(Stein) Ostenf.
-(Stein) T.H.Abé ex J.D.Dodge
 (Steiner) Hale
 (Steinh.) Endl. ex Unger
 (Stenham.) Hertel & Rambold
 (Stent) Kok
 (Stent) Roberty
 (Steph. ex G.Hoffm.) Kachroo & R.M.Schust.
 (Steph. ex Hoffm.) R.M.Schust. & Kachroo
@@ -19297,14 +19541,15 @@
 (Steud.) Huygh
 (Steud.) J.Kern
 (Steud.) J.M.Black
 (Steud.) J.R.Wheeler
 (Steud.) Jovet & Guedes
 (Steud.) K.L.Wilson
 (Steud.) K.R.Thiele
+(Steud.) K.R.Thiele & T.Hammer
 (Steud.) Kuntze
 (Steud.) Kük.
 (Steud.) Larridon & Govaerts
 (Steud.) Mattf. & Kük.
 (Steud.) N.Snow
 (Steud.) Nash
 (Steud.) Ostenf.
@@ -19370,15 +19615,14 @@
 (Stirt.) Kantvilas & LaGreca
 (Stirt.) Krog & Swinscow
 (Stirt.) Kurok.
 (Stirt.) Lücking
 (Stirt.) Lücking, Sérus. & Vězda
 (Stirt.) Mangold, Elix & Lumbsch
 (Stirt.) Marbach
-(Stirt.) Marbach & Kalb
 (Stirt.) Mayrhofer & Sheard
 (Stirt.) Müll.Arg.
 (Stirt.) O.Blanco, A.Crespo, Divakar, Elix & Lumbsch
 (Stirt.) P.M.Jørg.
 (Stirt.) Pusswald
 (Stirt.) R.Sant.
 (Stirt.) R.W.Rogers
@@ -19411,16 +19655,15 @@
 (Stschegl.) Druce
 (Stschegl.) F.Muell.
 (Stschegl.) Hislop
 (Stschegl.) Hislop, Crayn & Puente-Lel.
 (Stschegl.) Sleumer
 (Sturgis) R.J.G.Hertel
 (Sturtev.) Irish
-(Stüwe) F.Gómez
-(Stüwe) Jörg.
+(Stüwe) Jørg.
 (Subram.) S.Hughes
 (Subram.) de Hoog
 (Suckow) Borkh.
 (Suckow) C.K.Schneid.
 (Sudw.) A.E.Murray
 (Sudw.) Bartel
 (Sudw.) D.P.Little
@@ -19445,25 +19688,25 @@
 (Sull.) H.Rob.
 (Sull.) Isov.
 (Sull.) Kindb.
 (Sull.) Mitt.
 (Sull.) Nog.
 (Sull.) Paris
 (Sull.) S.H.Lin
-(Sull.) Vitt
 (Summerell & L.W.Burgess) Benyon, Summerell & L.W.Burgess
 (Summerh. & C.E.Hubb.) Morrone
 (Summerh. & C.E.Hubb.) S.W.L.Jacobs & J.Everett
 (Summerh.) C.C.Berg
 (Summerh.) Corner
 (Summerh.) E.A.Br.
+(Summerh.) E.B.Knox
 (Summerh.) E.Wimm.
 (Summerh.) I.Telford
 (Summerh.) Sleumer
-(Sundaram) R.G.Shivas & Vánky
+(Sundaram) Vánky & R.G.Shivas
 (Sundström) Hasle
 (Suneson) Hamel & Me.Lemoine
 (Suringar) De Toni
 (Suringar) Har.
 (Suringar) Kuck.
 (Suringar) Kylin
 (Suringar) Willi Krieg.
@@ -19491,48 +19734,46 @@
 (Sw.) Cass.
 (Sw.) Ching
 (Sw.) Christ
 (Sw.) Cooke
 (Sw.) Copel.
 (Sw.) D.Don
 (Sw.) DC.
-(Sw.) DC. x Prosopis velutina Wooton
 (Sw.) Desv. ex DC.
 (Sw.) Diels
 (Sw.) Domin
 (Sw.) Druce
 (Sw.) Duby
 (Sw.) E.H.Crane
 (Sw.) Elenkin
 (Sw.) F.M.Bailey
 (Sw.) F.Muell.
 (Sw.) Fosberg
 (Sw.) Fr.
 (Sw.) Gasper & Salino
 (Sw.) Gasper & V.A.O.Dittrich
 (Sw.) Gottsche
-(Sw.) Gray
 (Sw.) Holttum
 (Sw.) Holub
 (Sw.) Hook.
 (Sw.) Hook. & Grev.
+(Sw.) Houlston
 (Sw.) Hovenkamp & S.Linds.
 (Sw.) J.Sm.
 (Sw.) K.Iwats.
 (Sw.) Kaulf.
 (Sw.) Kreisel
 (Sw.) Kuhn
 (Sw.) Kunth
 (Sw.) Kuntze
 (Sw.) Lindenb.
 (Sw.) Link
 (Sw.) Lynge
 (Sw.) M.Fidalgo
 (Sw.) Mett.
-(Sw.) Mitt.
 (Sw.) Mont.
 (Sw.) Munro ex Benth.
 (Sw.) Murrill
 (Sw.) Müll.Arg.
 (Sw.) Müll.Berol.
 (Sw.) Müll.Hal.
 (Sw.) Nakai
@@ -19545,36 +19786,35 @@
 (Sw.) P.Chandra
 (Sw.) P.Karst.
 (Sw.) Parodi
 (Sw.) Pat.
 (Sw.) Poir.
 (Sw.) Prantl
 (Sw.) R.Br.
-(Sw.) Raeusch.
 (Sw.) Raf.
 (Sw.) Raspail
 (Sw.) Rich.
 (Sw.) Roberty
 (Sw.) Rydb.
 (Sw.) Ryvarden
 (Sw.) Räusch.
+(Sw.) S.E.Fawc. & A.R.Sm.
 (Sw.) S.F.Gray
 (Sw.) S.T.Blake
 (Sw.) Sch.Bip.
 (Sw.) Schaer.
 (Sw.) Schaer. ex Clem.
 (Sw.) Schott
 (Sw.) Spreng.
 (Sw.) Spring
 (Sw.) Stearn
 (Sw.) Steph.
 (Sw.) Sw.
 (Sw.) T.Durand & Schinz
 (Sw.) T.Moore
-(Sw.) T.Moore & Houlston
 (Sw.) Tardieu
 (Sw.) Tindale
 (Sw.) Trevis.
 (Sw.) Turner
 (Sw.) W.H.Wagner
 (Sw.) Willd.
 (Sw.) Zahlbr.
@@ -19605,43 +19845,45 @@
 (Sweet) Randell
 (Sweet) Schult. & Schult.f.
 (Sweet) Siebert & Voss
 (Sweet) Steud.
 (Sweet) Voss
 (Swingle) Burkill
 (Syd. & P.Syd.) Arthur
-(Syd. & P.Syd.) Begerow, Oberw., R.Bauer & A.Nagler
 (Syd. & P.Syd.) Cummins & Ramachar
 (Syd. & P.Syd.) Deighton
 (Syd. & P.Syd.) E.Horak
 (Syd. & P.Syd.) F.Stevens & Manter
 (Syd. & P.Syd.) K.D.Hyde
+(Syd. & P.Syd.) McTaggart & R.G.Shivas
 (Syd. & P.Syd.) P.F.Cannon
+(Syd. & P.Syd.) R.Bauer, Begerow, A.Nagler & Oberw.
 (Syd. & P.Syd.) S.Kaneko & Hirats.f.
 (Syd. & P.Syd.) Syd. & P.Syd.
 (Syd. & P.Syd.) Vánky
-(Syd. & Sacc.) J.Lowe
-(Syd. & Sacc.) Ryvarden
 (Syd.) Arx
 (Syd.) B.Sutton
 (Syd.) Bat.
 (Syd.) Bat. & Nascim.
 (Syd.) Crous & Summerell
 (Syd.) Deighton ex Ellis
 (Syd.) H.Scholz
 (Syd.) Hansf.
 (Syd.) J.Walker
 (Syd.) Kochman
 (Syd.) L.Guo
 (Syd.) L.Ling
 (Syd.) Langdon & Full.
-(Syd.) Oberw., M.Stoll & M.Piepenbr.
+(Syd.) M.Piepenbr., M.Stoll & Oberw.
+(Syd.) McTaggart & R.G.Shivas
 (Syd.) S.Hughes
 (Syd.) Vánky
 (Syd.) Zundel
+(Syd., P.Syd. & E.J.Butler) Mundk.
+(Syd., P.Syd. & E.J.Butler) Theiss. & Syd.
 (Syd., P.Syd. & E.J.Butler) Vánky
 (Syeda & Carolin) Hershk.
 (Syeda ex Obbens) Hershk.
 (Syeda) Carolin ex Hershk.
 (Syeda) Hershk.
 (Sykes) Chinnock
 (Symon) Albr. & Symon
@@ -19666,18 +19908,24 @@
 (T.E.Hunt) D.L.Jones & M.A.Clem.
 (T.E.Hunt) M.A.Clem.
 (T.E.Hunt) M.A.Clem. & D.L.Jones
 (T.E.Hunt) Rauschert
 (T.E.T.Bond) J.C.Lindq. & Alippi
 (T.H.Abé) Balech
 (T.H.Abé) Matsuoka
+(T.H.Li, Watling & N.M.Greg.) Halling, N.A.Fechner & Davoodian
 (T.H.Nash) Egan
+(T.H.Nicholson & N.C.Schenck) Sieverd., G.A.Silva & Oehl
+(T.H.Nicolson & Gerd.) C.Walker & A.Schüssler
+(T.H.Nicolson & Gerd.) C.Walker & F.E.Sanders
+(T.H.Nicolson & Gerd.) Gerd. & Trappe
 (T.H.Nicolson & Gerd.) Trappe & Gerd.
 (T.H.Nicolson & N.C.Schenck) C.Walker & A.Schüssler
 (T.I.Burgess, P.A.Barber & G.E.Hardy) T.I.Burgess, P.A.Barber & G.E.Hardy
+(T.Lebel) T.Lebel
 (T.Mitch. ex Lindl.) A.Terracc.
 (T.Mitch. ex Lindl.) Benth.
 (T.Mitch. ex Lindl.) Guymer
 (T.Mitch. ex Lindl.) K.Schum.
 (T.Mitch.) C.A.Gardner
 (T.Mitch.) Kuntze
 (T.Moore ex Bosch) Copel.
@@ -19685,39 +19933,39 @@
 (T.Moore) Crisp
 (T.Moore) Domin
 (T.Moore) F.M.Bailey
 (T.Moore) Hennipman & M.C.Roos
 (T.Moore) Nakai
 (T.Moore) T.Moore
 (T.Moore) Underw.
-(T.Nees & Blume) Berk.
 (T.Nees & Blume) Sacc.
 (T.Ohta) S.Skinner
-(T.W.May) Seifert & Redhead
+(T.W.May) Redhead & Seifert
 (T.West) Grunow
 (T.Yamag., Seppelt & Z.Iwats.) Seppelt & H.A.Crum
 (Tak.Tanaka & K.Nozawa) Huisman
 (Takano) Takano
 (Tanaka) Tanaka
 (Tandon & Bilgrami) M.B.Ellis
 (Tanfani) Sprague
 (Tanner-Fullemann) G.M.Sm.
+(Targ.Tozz.) Endl.
 (Tassi) Nag Raj
 (Tassi) P.M.Kirk
 (Tate ex J.M.Black) J.M.Black
 (Tate) B.L.Burtt
 (Tate) Beier & Thulin
 (Tate) Christenh. & Byng
 (Tate) D.L.Jones & M.A.Clem.
 (Tate) Danser
 (Tate) E.A.Shaw
 (Tate) J.M.Black
 (Tate) Kellermann & W.R.Barker
 (Tate) Kuntze
-(Tate) Lemee
+(Tate) Lemée
 (Tate) O.E.Schulz
 (Tate) Orchard
 (Tate) Paul G.Wilson
 (Tate) Pedley
 (Tate) Puttock
 (Tate) S.W.L.Jacobs & J.Everett
 (Tate) Szlach.
@@ -19757,18 +20005,18 @@
 (Taylor) Grolle
 (Taylor) H.A.Crum
 (Taylor) H.A.Mill.
 (Taylor) Hale
 (Taylor) Hale & A.Fletcher
 (Taylor) Hertel
 (Taylor) Hue
+(Taylor) J.A.Jiménez & M.J.Cano
 (Taylor) J.R.Spence
 (Taylor) J.R.Spence & H.P.Ramsay
 (Taylor) Kindb.
-(Taylor) Krog & Swinscow
 (Taylor) Kurok.
 (Taylor) M.Choisy
 (Taylor) Mitt.
 (Taylor) Mudd
 (Taylor) Müll.Arg.
 (Taylor) Müll.Hal.
 (Taylor) Nyl.
@@ -19811,28 +20059,30 @@
 (Ten.) B.L.Burtt & P.Lewis
 (Ten.) Baill.
 (Ten.) Hayek
 (Ten.) Kuntze
 (Ten.) Ponert
 (Ten.) Sch.Bip.
 (Ten.) Steenis
+(Teng) S.H.He & Nakasone
 (Tepper ex F.Ludw.) Kuntze
 (Tepper) J.M.Black
 (Tepper) Lowrie
 (Tepper) Raym.-Hamet
 (Th.Fr.) Czarnota, Guzow-Krzeminska & Coppins
 (Th.Fr.) Giralt
 (Th.Fr.) Hafellner
 (Th.Fr.) Th.Fr.
 (Thaxt.) C.Walker & A.Schüssler
-(Thaxt.) Trappe & Gerd.
+(Thaxt.) Gerd. & Trappe
+(Thaxt.) Sieverd., G.A.Silva & Oehl
 (Theiss.) Lloyd
 (Thell.) Domin
 (Thell.) Thell. & Aellen
-(Thirum. & Mundk.) Vánky
+(Thines) Simamora & T.I.Burgess
 (Thom) Doty
 (Thom) Samson
 (Thouars ex Pfitzer) Schltr.
 (Thouars) Benth.
 (Thouars) F.Muell.
 (Thouars) H.Perrier
 (Thouars) Kuntze
@@ -19877,23 +20127,25 @@
 (Thunb.) Domin
 (Thunb.) Druce
 (Thunb.) Eckl. & Zeyh.
 (Thunb.) Engl.
 (Thunb.) Ewart, Jean White & B.Rees
 (Thunb.) F.Muell.
 (Thunb.) Fenzl ex Harv.
+(Thunb.) Fourc.
 (Thunb.) Franch. & Sav.
 (Thunb.) Gagnep.
 (Thunb.) Galley & H.P.Linder
 (Thunb.) Goldblatt
 (Thunb.) Goldblatt & J.C.Manning
 (Thunb.) H.Ohashi
 (Thunb.) H.Ohashi & K.Ohashi
 (Thunb.) H.P.Linder
 (Thunb.) Hayata
+(Thunb.) Hemsl.
 (Thunb.) Henrard
 (Thunb.) Hilliard
 (Thunb.) Hilliard & B.L.Burtt
 (Thunb.) Holub
 (Thunb.) Hook.
 (Thunb.) Hook. & Arn.
 (Thunb.) Hutch.
@@ -19927,14 +20179,15 @@
 (Thunb.) N.E.Br.
 (Thunb.) Nakai
 (Thunb.) Nakai ex A.T.Lee
 (Thunb.) Nees
 (Thunb.) Oberm.
 (Thunb.) Ohwi & H.Ohashi
 (Thunb.) P.Beauv.
+(Thunb.) Prokudin ex Á.Löve
 (Thunb.) R.Br.
 (Thunb.) R.Br. ex Mirb.
 (Thunb.) R.J.F.Hend.
 (Thunb.) Raf.
 (Thunb.) Renvoize
 (Thunb.) Roem. & Schult.
 (Thunb.) Salisb.
@@ -19953,22 +20206,24 @@
 (Thunb.) Trin.
 (Thunb.) Walp.
 (Thunb.) Weymouth
 (Thunb.) Willd.
 (Thunb.) Zucc.
 (Thunb.) de Laub.
 (Thunb.) Á.Löve
+(Thur.) 
 (Thur.) De Toni
 (Thur.) Gomont
 (Thur.) Kuck.
 (Thur.) Playfair
 (Thuret ex Bornet & Flahault) Kirchner
 (Thuret ex Bornet & Flahault) Kováčik & Komárek
 (Thwaites & Mitt.) A.Jaeger
 (Thwaites & Mitt.) B.C.Tan
+(Thwaites & Mitt.) Hilp.
 (Thwaites & Mitt.) W.R.Buck & B.C.Tan
 (Thwaites ex Gomont) Anagn. & Komárek
 (Thwaites ex Harv.) Grunow
 (Thwaites ex Harv.) Hyung S.Kim & I.K.Lee
 (Thwaites) Benth.
 (Thwaites) C.B.Clarke
 (Thwaites) C.S.Boyer
@@ -19990,15 +20245,14 @@
 (Thwaites) Playfair
 (Thwaites) R.L.Barrett, K.L.Wilson & J.J.Bruhl
 (Thwaites) Ridl.
 (Thwaites) Soderstr. & R.P.Ellis
 (Thwaites) T.Koyama
 (Thwaites) Thwaites ex W.Sm.
 (Thwaites) Van Heurck
-(Thüm. & F.Muell.) Sacc.
 (Thüm.) Cif.
 (Thüm.) G.Winter
 (Thüm.) J.C.F.Hopkins
 (Thüm.) K.Yokoy. & S.Kaneko
 (Thüm.) Langdon & Full.
 (Thüm.) McAlpine
 (Thüm.) Oudem.
@@ -20040,34 +20294,35 @@
 (Tindale) Kodela
 (Tindale) Labiak, Sundue & R.C.Moran
 (Tindale) Pedley
 (Tineo & Guss.) Hegi
 (Tineo ex Guss.) D.A.Webb
 (Tixier) Pócs
 (Tod.) Fryxell
-(Tode) De Not. & Ces.
+(Tode) Ces. & De Not.
 (Tode) Desm.
 (Tode) Ginns
-(Tode) Spooner & Læssøe
+(Tode) L.Lombard & Crous
+(Tode) Læssøe & Spooner
 (Tode) Westend.
 (Toelken) A.P.Druce & Sykes
+(Toelken) T.Hammer
 (Toelken) Toelken
 (Toelken) Toelken & de Lange
 (Togashi & Y.Maki) Vánky
 (Tokida) Garbary & J.T.Harper
 (Tomaschek) A.Fisch.
 (Tomaschek) Lemmerm.
 (Tomm. ex Freyn) Murb.
 (Tomm. ex Freyn) Murb. ex Asch. & Graebn.
 (Tornab.) Runemark
 (Torr. & A.Gray) A.Gray
 (Torr. & A.Gray) Greene
 (Torr. & A.Gray) Heiser
 (Torr. & A.Gray) Iltis
-(Torr. & A.Gray) Sch.Bip.
 (Torr. & A.Gray) Voss
 (Torr.) A.Gray
 (Torr.) Beal
 (Torr.) Britton & Rose
 (Torr.) Cockerell
 (Torr.) E.P.Bicknell
 (Torr.) Mattf. & Kük.
@@ -20080,24 +20335,28 @@
 (Torr.) Á.Löve & D.Löve
 (Torrend) Ginns
 (Torrend) Hjortstam
 (Torrend) Jülich & Stalpers
 (Torrend) Singer
 (Touw) Touw
 (Tovey & P.Morris) J.H.Ross
+(Tracy & Earle) Boedijn
+(Tracy & Earle) Magnus
 (Trail) Hara
 (Transeau) Czurda
 (Transeau) G.M.Sm.
 (Trappe & Claridge) Gasparini
+(Trappe & Claridge) Kuhar, Nouhra & M.E.Sm.
 (Trappe & Claridge) Trappe & Claridge
 (Trappe & Gerd.) C.Walker & F.E.Sanders
-(Trappe & Gerd.) R.T.Almeida & N.C.Schenck
+(Trappe & Gerd.) Trappe, Desirò, M.E. Sm., Bonito & Bidartondo
 (Trappe) Trappe & Claridge
 (Trappe) Trappe & G.W.Beaton
 (Trappe, Gerd. & I.Ho) C.Walker & F.E.Sanders
+(Trappe, V.L.Oliveira, Castellano & Claridge) Kuhar, Nouhra & M.E.Sm.
 (Tratman ex Morrison) Carolin ex Hershk.
 (Tratman ex Morrison) Hershk.
 (Tratt.) DC.
 (Tratt.) Domin
 (Tratt.) F.Muell.
 (Tratt.) Sweet
 (Trautv.) Cullen
@@ -20151,14 +20410,15 @@
 (Trin.) Trin. & Rupr.
 (Trin.) Trin. ex Nees
 (Trin.) Veldkamp
 (Trin.) É.Desv.
 (Trudgen & Keighery) de Lange & Toelken
 (Trudgen) Rye
 (Tsuda & Ueyama) Alcorn
+(Tsuda & Ueyama) H.Deng, Y.P.Tan & R.G.Shivas
 (Tsuda & Ueyama) Sivan.
 (Tuck. & Mont.) Mangold
 (Tuck. ex Mich.) Müll.Arg.
 (Tuck. ex Nyl.) Kalb
 (Tuck. ex Nyl.) Poelt
 (Tuck. ex Nyl.) R.C.Harris
 (Tuck.) B.de Lesd.
@@ -20173,15 +20433,14 @@
 (Tuck.) Henssen
 (Tuck.) Hertel
 (Tuck.) Hertel & Rambold
 (Tuck.) Imshaug
 (Tuck.) J.W.Thomson
 (Tuck.) Kalb
 (Tuck.) Kalb & Gierl
-(Tuck.) Krog & Swinscow
 (Tuck.) Marbach
 (Tuck.) Matzer, H.Mayrhofer & Rambold
 (Tuck.) Müll.Arg.
 (Tuck.) Otálora, P.M.Jørg. & Wedin
 (Tuck.) R.C.Harris
 (Tuck.) Riddle
 (Tuck.) Swinscow & Krog
@@ -20197,22 +20456,21 @@
 (Tul. & C.Tul.) J.T.Palmer
 (Tul. & C.Tul.) McAlpine
 (Tul. & C.Tul.) Tul. & C.Tul.
 (Tul. ex G.H.Otth) Cummins & H.C.Greene
 (Tul. ex M.Raoul) E.Fisch.
 (Tul.) A.DC.
 (Tul.) Benth.
-(Tul.) C.W.Dodge & Zeller
 (Tul.) Damon
 (Tul.) J.C.David & D.Hawksw.
 (Tul.) Koehne
 (Tul.) Singer & A.H.Sm.
 (Tul.) Triebel & Rambold
-(Tul.) Tul. & C.Tul.
-(Turconi) S.Hughes & E.W.Mason
+(Tul.) Zeller & C.W.Dodge
+(Turconi) E.W.Mason & S.Hughes
 (Turconi) Zare & W.Gams
 (Turcz.) A.S.George
 (Turcz.) A.S.George & N.Gibson
 (Turcz.) Anderb.
 (Turcz.) B.D.Jacks.
 (Turcz.) B.J.Conn & Henwood
 (Turcz.) B.L.Burtt
@@ -20231,16 +20489,18 @@
 (Turcz.) Crisp & Orthia
 (Turcz.) Domin
 (Turcz.) Druce
 (Turcz.) Dunlop
 (Turcz.) E.M.Benn.
 (Turcz.) Edgew. & Hook.f.
 (Turcz.) Ewart
+(Turcz.) F.J.Mou
 (Turcz.) F.M.Bailey
 (Turcz.) F.Muell.
+(Turcz.) F.Muell. ex Schltdl.
 (Turcz.) Furtado & Montien
 (Turcz.) G.Chandler & Crisp
 (Turcz.) G.L.Davis
 (Turcz.) Gardner
 (Turcz.) Gilg
 (Turcz.) Govaerts
 (Turcz.) Greene
@@ -20261,21 +20521,20 @@
 (Turcz.) N.G.Marchant & Keighery
 (Turcz.) N.T.Burb.
 (Turcz.) Nied.
 (Turcz.) Oliv.
 (Turcz.) Ostenf.
 (Turcz.) P.S.Short
 (Turcz.) Paul G.Wilson
-(Turcz.) Paul G.Wilson - Phebalium tuberculosum (F.Muell.) Benth.
+(Turcz.) Peter G.Wilson
 (Turcz.) R.K.Jansen
 (Turcz.) Rye
 (Turcz.) Sch.Bip.
+(Turcz.) Tanaka
 (Turcz.) Toelken
-(Turcz.) Toelken x Kunzea micromera Schauer
-(Turcz.) Toelken x Kunzea recurva Schauer
 (Turcz.) Turcz.
 (Turcz.) Voss
 (Turner & Borrer ex Sm.) Almb.
 (Turner & Borrer) Duby
 (Turner & Borrer) Tibell
 (Turner & Sm.) Migula
 (Turner) A.Massal.
@@ -20327,15 +20586,18 @@
 (Turra) B.D.Jacks.
 (Turrill) Pedley
 (Turton) Nägeli
 (Tuyama) Fukuy.
 (Tzvelev) E.B.Alexeev
 (Tzvelev) Soreng, L.J.Gillespie & S.W.L.Jacobs
 (Tzvelev) Á.Löve
-(U.Braun) V.P.Gelyuta
+(U.Braun & Crous) J.A.Simpson
+(U.Braun & Crous) U.Braun & Crous
+(U.Braun) Heluta
+(U.Braun) P.-L.Qiu & S.-Y.Liu
 (Uden & Kolip.) S.A.Mey. & Yarrow
 (Uebelm.) S.F.Chen & C.Y.Chien
 (Ulbr.) A.J.Scott
 (Ulbr.) Borss.Waalk.
 (Umphlett) Sv.Nilsson
 (Underw.) C.Chr.
 (Underw.) Hennipman & M.C.Roos
@@ -20345,18 +20607,18 @@
 (Unger) Lemmerm.
 (Upton) D.L.Jones & M.A.Clem.
 (Upton) M.A.Clem. & D.L.Jones
 (Upton) Szlach.
 (Urb.) Anderb.
 (Usacev) Proshk.-Lavr.
 (V.Brig.) Singer
-(V.G.Rao & A.S.Patil) Alcorn
+(V.Brig.) Vizzini
 (V.J.Chapm.) Papenf. & K.C.Fan ex Papenf.
 (V.J.Cook) Soják
-(V.S.White) G.Moreno, J.E.Wright & Altés
+(V.S.White) J.E.Wright, G.Moreno & Altés
 (Vahl) Andersen
 (Vahl) Benth.
 (Vahl) Bisch. ex Boiss.
 (Vahl) Boeckeler
 (Vahl) Bor
 (Vahl) Brongn.
 (Vahl) Børgesen
@@ -20369,15 +20631,14 @@
 (Vahl) Endl.
 (Vahl) F.Ballard
 (Vahl) F.Muell.
 (Vahl) G.Brückn.
 (Vahl) G.Hirsch
 (Vahl) Gale
 (Vahl) Gillet
-(Vahl) Gray
 (Vahl) Greene
 (Vahl) Griseb.
 (Vahl) Hallier f.
 (Vahl) Henr.
 (Vahl) Herter
 (Vahl) Kosterm.
 (Vahl) Kunth
@@ -20385,14 +20646,15 @@
 (Vahl) Kük.
 (Vahl) L.A.S.Johnson
 (Vahl) Larridon
 (Vahl) Lye
 (Vahl) Lynge
 (Vahl) Masam.
 (Vahl) Merr.
+(Vahl) Michelang.
 (Vahl) Nees
 (Vahl) Nees ex C.B.Clarke
 (Vahl) Ohwi
 (Vahl) P.Karst.
 (Vahl) P.Kumm.
 (Vahl) P.Royen
 (Vahl) Palla
@@ -20416,17 +20678,15 @@
 (Vahl) Wettst.
 (Vahl) Wight
 (Vahl) Wight ex Steud.
 (Vahl) Wikstr.
 (Vahl) Wipff
 (Vahl) Á.Löve & D.Löve
 (Vahl) É.Desv.
-(Vaill. : Fr.) Link
-(Vaill.) Fr.
-(Vaill.) Link
+(Vahl) Örstadius & E.Larss.
 (Vain. ex Rasanen) Dombr.
 (Vain.) A.W.Archer
 (Vain.) A.W.Archer & Elix
 (Vain.) Aptroot
 (Vain.) Aptroot, Lücking & G.Thor
 (Vain.) Aptroot, M.P.Nelsen & Lücking
 (Vain.) Articus
@@ -20447,15 +20707,14 @@
 (Vain.) Gotth.Schneid.
 (Vain.) Gyeln.
 (Vain.) Hale
 (Vain.) Hale ex Sipman
 (Vain.) Kalb
 (Vain.) Kernst.
 (Vain.) Kirika, Divakar & Lumbsch
-(Vain.) Krog & Swinscow
 (Vain.) Lendemer & R.C.Harris
 (Vain.) Llano
 (Vain.) Lynge
 (Vain.) Lücking & Sérus.
 (Vain.) Marbach
 (Vain.) Marbach, Elix & Kalb
 (Vain.) Motyka
@@ -20470,15 +20729,14 @@
 (Vain.) Swinscow & Krog
 (Vain.) Søchting, Frödén & Arup
 (Vain.) Tibell
 (Vain.) Vain.
 (Vain.) Vězda
 (Vain.) Vězda & Poelt
 (Vain.) W.A.Weber
-(Vain.) W.L.Culb. & C.F.Culb.
 (Vain.) Y.S.Park & Hale
 (Vain.) Zahlbr.
 (Valck.Sur.) Kük.
 (Valeton) J.Everett
 (Valeton) Merr. & L.M.Perry
 (Valeton) Moldenke
 (Valeton) N.C.Duke
@@ -20488,27 +20746,27 @@
 (Van Goor) Meffert
 (Van Heurck) F.W.Mills
 (Van Heurck) Hoban
 (Van Heurck) R.M.Patrick
 (Van der Byl) Ryvarden
 (Vand.) Wettst.
 (Vanhöffen) Balech
-(Vanhöffen) Ostenf.
+(Vanhöffen) Jørg.
+(Varga & Samson) Samson, Varga, Visagie & Houbraken
 (Varsavsky & Ajello) Oorschot
 (Vassal) Vassal
 (Vaucher ex Gomont) Anagn. & Komárek
 (Vaucher) Bréb. & Godey
 (Vaucher) C.Agardh
 (Vaucher) DC.
 (Vaucher) Desv.
 (Vaucher) Harv.
-(Vaucher) Kütz
 (Vaucher) Kütz.
 (Vaucher) Thur.
-(Veldkamp) H.P.Linder
+(Vaughan-Mart., Kurtzman, S.A.Mey. & E.B.O'Neill) Kurtzman & M.Suzuki
 (Velen.) Nannf. & L.Holm
 (Velen.) S.E.Carp.
 (Vell.) A.H.Gentry
 (Vell.) Briq.
 (Vell.) C.Presl
 (Vell.) H.S.Irwin & Barneby
 (Vell.) J.M.A.Braga
@@ -20522,15 +20780,14 @@
 (Vent.) Andrews
 (Vent.) B.L.Burtt
 (Vent.) Baill.
 (Vent.) Benth.
 (Vent.) Blume ex A.Juss.
 (Vent.) Byng & Christenh.
 (Vent.) DC.
-(Vent.) DC. x Ozothamnus diotophyllus (F.Muell.) Anderb.
 (Vent.) Daveau
 (Vent.) Decne.
 (Vent.) Desf.
 (Vent.) Desv.
 (Vent.) Domin
 (Vent.) Druce
 (Vent.) Dum.Cours.
@@ -20539,14 +20796,15 @@
 (Vent.) G.Don
 (Vent.) Gasp.
 (Vent.) Goldblatt
 (Vent.) Heynh.
 (Vent.) Hook.
 (Vent.) Hook.f.
 (Vent.) J.L.Parm.
+(Vent.) Jackes & Trias-Blasi
 (Vent.) Kunth
 (Vent.) Kuntze
 (Vent.) L.A.S.Johnson
 (Vent.) Laun.
 (Vent.) Link
 (Vent.) Maiden & Betche
 (Vent.) Miq.
@@ -20565,16 +20823,18 @@
 (Vent.) Steenis
 (Vent.) Sweet
 (Vent.) Tratt.
 (Vent.) Tzvelev
 (Vent.) Voss
 (Vent.) Willd.
 (Verdon) Otálora, P.M.Jørg. & Wedin
+(Vernes, Danks & T.Lebel) Niskanen & Liimat.
 (Verona) A.R.Liu, T.Xu & L.D.Guo
 (Verwoerd & du Plessis) Crous
+(Verwoerd & du Plessis) Thambug. & K.D.Hyde
 (Vest) Comes
 (Vezda & Malcolm) Malcolm
 (Viala & G.Boyer) Prill. & Delacr.
 (Vickers) Børgesen
 (Vickers) Woelk.
 (Vickery) A.C.Sm.
 (Vickery) A.J.Br.
@@ -20607,15 +20867,14 @@
 (Vido) Sacc.
 (Vieill. ex E.Fourn.) C.Chr.
 (Vill.) Asch.
 (Vill.) Brenan
 (Vill.) C.Presl
 (Vill.) Gams ex D.Hawksw.
 (Vill.) Heukels
-(Vill.) Kraichak, Lucking & Lumbsch
 (Vill.) Kraichak, Lücking & Lumbsch
 (Vill.) Norman
 (Vill.) Nyman
 (Vill.) Schinz & Thell.
 (Vill.) Schischk.
 (Vill.) Soják
 (Vill.) Thell.
@@ -20627,47 +20886,52 @@
 (Vis.) Charrel
 (Vis.) Rehder
 (Vittad.) De Toni
 (Vittad.) Kreisel
 (Vittad.) Lloyd
 (Vittad.) M.Lange
 (Vittad.) M.M.Moser ex Bon
-(Vittad.) Morgan
 (Vittad.) P.D.Orton
 (Vittad.) Peck
 (Vittad.) Quél.
+(Vittad.) Redhead
 (Vittad.) Sacc.
 (Vittad.) Schild
 (Vittad.) Singer
-(Vittad.) T.W.May
 (Vittad.) Tul. & C.Tul.
 (Vittad.) Vellinga
 (Viv.) A.Berger
 (Viv.) Gillet
 (Viv.) H.S.Irwin & Barneby
 (Viv.) Kuntze
 (Viv.) Ricken
 (Viv.) Runemark ex Melderis
 (Vize ex Cooke) Y.X.Chen
-(Viégas) Begerow, Oberw., R.Bauer & A.Nagler
+(Vizzini, Contu & Justo) Murrill
+(Viégas) R.Bauer, Begerow, A.Nagler & Oberw.
 (Vogel) Benth.
 (Vogel) H.S.Irwin & Barneby
 (Vogel) Hassl.
 (Vogel) Randell
 (Vogel) Walp.
 (Voglino) Priest
 (Voit) Lindb.
 (Voit) Warnst.
 (Vouaux) D.Hawksw.
 (Vouaux) D.J.Galloway
 (Vuill.) Tirab.
+(Vánky & A.A.Mitch.) McTaggart & R.G.Shivas
 (Vánky & C.Vánky) Vánky
-(Vánky & Websdane) Vánky
-(Vánky) Begerow, Oberw. & M.Stoll
+(Vánky & McKenzie) McTaggart & R.G.Shivas
+(Vánky & McKenzie) Vánky
+(Vánky & R.G.Shivas) McTaggart & R.G.Shivas
+(Vánky) M.Stoll, Begerow & Oberw.
+(Vánky) McTaggart & R.G.Shivas
 (Vánky) Vánky
+(Vánky, C.Vánky & R.G.Shivas) McTaggart & R.G.Shivas
 (Vězda & Farkas) Kalb & Lücking
 (Vězda) Brusse
 (Vězda) D.Hawksw.
 (Vězda) H.Harada
 (Vězda) Kalb & Lücking
 (Vězda) Lücking
 (Vězda) Lücking & Aptroot
@@ -20703,15 +20967,14 @@
 (W.Bull) Dowe
 (W.Bull) Dugand
 (W.Bull) Schlittler
 (W.Bull) Sprague ex Steenis
 (W.C.Ko) N.C.Duke & X.J.Ge
 (W.Conrad) Hub.-Pest.
 (W.Conrad) Skvortsov
-(W.Curtis : Fr.) Fr.
 (W.D.J.Koch) Arcang.
 (W.Fitzg. ex Ewart & Jean White) P.S.Short
 (W.Fitzg. ex Ewart & Jean White) Pedley
 (W.Fitzg.) A.J.Scott
 (W.Fitzg.) A.T.Lee
 (W.Fitzg.) B.G.Briggs
 (W.Fitzg.) B.G.Briggs & L.A.S.Johnson
@@ -20729,14 +20992,15 @@
 (W.Fitzg.) Domin
 (W.Fitzg.) Dunlop
 (W.Fitzg.) F.D.Wilson
 (W.Fitzg.) Farmar
 (W.Fitzg.) Guymer
 (W.Fitzg.) H.Eichler
 (W.Fitzg.) Halford & W.K.Harris
+(W.Fitzg.) Hershk.
 (W.Fitzg.) Hislop & Puente-Lel.
 (W.Fitzg.) Hislop, Crayn & Puente-Lel.
 (W.Fitzg.) J.D.Briggs & Leigh
 (W.Fitzg.) J.Schust.
 (W.Fitzg.) J.W.Green
 (W.Fitzg.) J.W.Grimes
 (W.Fitzg.) K.D.Hill & L.A.S.Johnson
@@ -20759,14 +21023,15 @@
 (W.Fitzg.) Trudgen
 (W.G.Sm.) Baker
 (W.G.Sm.) Earle
 (W.G.Sm.) Gillet
 (W.G.Sm.) McAlpine
 (W.G.Sm.) P.Karst.
 (W.G.Sm.) Sacc.
+(W.Gams & Sivasith.) L.W.Hou, L.Cai & Crous
 (W.Greg. ex Grev.) Hust.
 (W.Greg.) Chunlian Li, Ashworth & Witkowski
 (W.Greg.) Cleve
 (W.Greg.) Cleve & Grunow
 (W.Greg.) D.G.Mann
 (W.Greg.) D.G.Mann & A.J.Stickle
 (W.Greg.) Danielidis & D.G.Mann
@@ -20783,21 +21048,21 @@
 (W.Greg.) M.Garcia-Baptista
 (W.Greg.) Pelletan
 (W.Greg.) Playfair
 (W.Greg.) R.Ross & Hartley
 (W.Greg.) Rabenh.
 (W.Greg.) Ralfs
 (W.Greg.) Round & D.G.Mann
+(W.Greg.) Ruck & Nakov
 (W.Greg.) Van Heurck
 (W.Greg.) Witkowski
 (W.Hartley) Lazarides
 (W.Hill & F.Muell.) F.Muell.
 (W.Hill & F.Muell.) P.H.Weston & Crisp
 (W.Hill & F.Muell.) Sleumer
-(W.Hill) Burret
 (W.Hill) F.M.Bailey
 (W.Hill) F.Muell.
 (W.Hill) Hook.f. ex Becc.
 (W.Hill) J.Schust.
 (W.Hill) Kuntze
 (W.Hill) L.H.Bailey
 (W.Hill) M.A.Clem. & D.L.Jones
@@ -20807,14 +21072,15 @@
 (W.Koch) W.J.de Wilde
 (W.L.Culb.) Hale
 (W.M.Curtis) D.A.Cooke
 (W.M.Curtis) D.L.Jones & M.A.Clem.
 (W.M.Curtis) P.S.Short
 (W.M.Curtis) Seberg
 (W.M.Curtis) W.R.Barker
+(W.M.Pitt, Úrbez-Torr. & Trouillas) Tao Yang & Crous
 (W.Martin & E.A.Hodgs.) J.J.Engel & R.M.Schust.
 (W.Martin & E.A.Hodgs.) R.M.Schust.
 (W.N.Takeuchi & Pipoly) D.L.Jones & B.Gray
 (W.Phillips & Plowr.) Sacc.
 (W.Phillips ex Cooke) S.E.Carp.
 (W.Phillips) Dennis
 (W.Phillips) Massee
@@ -20838,15 +21104,14 @@
 (W.Sm.) Cleve
 (W.Sm.) D.G.Mann & A.J.Stickle
 (W.Sm.) D.M.Williams & Round
 (W.Sm.) E.Morales & C.E.Wetzel
 (W.Sm.) F.Meister
 (W.Sm.) Grunow
 (W.Sm.) Grunow & Eulenstein
-(W.Sm.) H.Perag. & M.Perag.
 (W.Sm.) Hendey
 (W.Sm.) Hust.
 (W.Sm.) J.W.Griff. & Henfr.
 (W.Sm.) Kirchner
 (W.Sm.) Krammer
 (W.Sm.) Lagerst.
 (W.Sm.) Lange-Bert.
@@ -20857,52 +21122,57 @@
 (W.Sm.) Reimer
 (W.Sm.) Round & Bukht.
 (W.Sm.) Stickle & D.G.Mann
 (W.Sm.) Van Heurck
 (W.T.Aiton) Druce
 (W.T.Aiton) Herb.
 (W.T.Aiton) J.Gay
-(W.T.Aiton) J.Gay x Thomasia solanacea (Sims) J.Gay
 (W.Voss) Sacc.
 (W.West & G.S.West) Playfair
 (W.Weston & Uppal) C.G.Shaw
 (W.Weston) C.G.Shaw
+(W.Weston) Telle & Thines
 (W.Yamam.) Hansf.
 (Wahlenb.) A.Massal.
 (Wahlenb.) Fr.
 (Wahlenb.) Hedenäs
 (Wahlenb.) Kindb.
 (Wahlenb.) Körb.
 (Wahlenb.) Leight.
 (Wahlenb.) Limpr.
+(Wahlenb.) Lindb.
 (Wahlenb.) M.Choisy ex Scheid. & H.Mayrhofer
 (Wahlenb.) Norman
 (Wahlenb.) Nägeli ex Uloth
 (Wahlenb.) Röhl.
+(Wahlenb.) Schimp.
 (Wahlenb.) Sommerf.
 (Wahlenb.) Th.Fr.
+(Wahlenb.) Tuom. & T.J.Kop.
 (Wahlenb.) Wagenitz & Greuter
 (Wahlenb.) Wahlenb.
 (Wailes) M.Lefèvre
 (Wakef.) Boidin & Lanq.
 (Wakef.) Burds.
 (Wakef.) Corner
-(Wakef.) Crous & Denman
 (Wakef.) D.A.Reid
+(Wakef.) Denman & Crous
 (Wakef.) G.Cunn.
 (Wakef.) Ginns
 (Wakef.) Hansf.
 (Wakef.) Hjortstam
 (Wakef.) Hjortstam & Ryvarden
 (Wakef.) Jülich
 (Wakef.) K.L.Wilson
 (Wakef.) Nakasone
 (Wakef.) Nakasone & Gilb.
+(Wakef.) Redhead, Vizzini, Drehmel, & Contu
 (Wakef.) S.L.Thrower
 (Wakef.) Trotter
+(Wakef.) Vizzini & Contu
 (Wakker) Boedijn
 (Wakker) Sacc.
 (Waldst. & Kit.) Cout.
 (Waldst. & Kit.) F.Nyl.
 (Wall. ex Benth.) Kuntze
 (Wall. ex Cambess.) Hook.
 (Wall. ex DC.) R.K.Jansen
@@ -20932,14 +21202,15 @@
 (Wall.) Adema
 (Wall.) Alston
 (Wall.) B.D.Jacks.
 (Wall.) Baill. ex Müll.Arg.
 (Wall.) Baker
 (Wall.) Benth.
 (Wall.) Brongn.
+(Wall.) C.B.Clarke
 (Wall.) Choisy
 (Wall.) DC.
 (Wall.) F.Muell.
 (Wall.) H.Hara
 (Wall.) Hand.-Mazz.
 (Wall.) Hutch.
 (Wall.) Kazmi
@@ -20956,24 +21227,26 @@
 (Wallr.) Flot.
 (Wallr.) Fuckel
 (Wallr.) G.Winter
 (Wallr.) Gren.
 (Wallr.) Mansf.
 (Wallr.) Rabenh.
 (Wallr.) Rabenh. ex Fuckel
+(Wallr.) Rossman & K.D.Hyde
 (Wallr.) Rostaf.
 (Wallr.) Sacc.
 (Wallr.) Shoemaker
 (Wallr.) U.Braun
 (Wallr.) U.Braun & S.Takam.
 (Wallr.) Zahlbr.
 (Wallr.) de Bary
 (Wallroth) A.Beguinot & L.Formiggini
 (Wallroth) J.Groves
 (Wallroth) Kütz.
+(Wallwork & Spooner) Crous & W.Gams
 (Walp.) Baill.
 (Walp.) Benth.
 (Walp.) Domin
 (Walp.) Druce
 (Walp.) F.Muell.
 (Walp.) J.Everett
 (Walp.) Kosterm.
@@ -20994,19 +21267,19 @@
 (Warb.) J.Sinclair
 (Warb.) Kaneh.
 (Warb.) Lauterb. & K.Schum.
 (Warb.) Merr. & L.M.Perry
 (Warb.) Ooststr.
 (Warb.) Perkins
 (Warb.) W.J.de Wilde
+(Warcup & P.H.B.Talbot) Liberta
 (Warnst.) Rodway
 (Warnst.) Warnst.
 (Wartm.) Chodat
 (Wartm.) Gomont
-(Watling & Høil.) T.W.May & A.E.Wood
 (Watts) Christenh.
 (Watts) Copel.
 (Watts) D.L.Jones
 (Watts) Domin
 (Watts) N.A.Wakef.
 (Watts) Parris
 (Watts) S.B.Andrews
@@ -21039,15 +21312,16 @@
 (Weber Bosse) Stegenga
 (Weber Bosse) Weber Bosse
 (Weber Bosse) Woelk.
 (Weber Bosse) Womersley
 (Weber Bosse) Yamada
 (Weber Bosse) Yamada & Tak.Tanaka
 (Weber) Ach.
-(Weber) Hasle
+(Websdane & Vánky) Vánky
+(Websdane, Sivasith., K.W.Dixon & Pate) Vánky
 (Webster) Chinnock
 (Wedd.) Arup, Frödén & Søchting
 (Wedd.) Benth.
 (Wedd.) Chew
 (Wedd.) Friis & Wilmot-Dear
 (Wedd.) Kuntze
 (Wedd.) P.S.Green
@@ -21065,19 +21339,26 @@
 (Weigel) P.Kumm.
 (Weing.) Backeb.
 (Weing.) Borg
 (Weinm.) Cooke ex G.Cunn.
 (Weinm.) Fr.
 (Weinm.) G.Cunn.
 (Weinm.) Gillet
+(Weinm.) Matheny & Esteve-Rav.
 (Weinm.) P.Kumm.
 (Weinm.) Quél.
 (Weir ex Rodway & Cleland) G.Cunn.
 (Weis) Humb.
 (Weisse) F.Stein
+(Welti & Courtec.) Welti & Courtec.
+(Welw. & Curr.) A.L.Sm.
+(Welw. & Curr.) Cooke
+(Welw. & Curr.) D.Hawksw.
+(Welw. & Curr.) Sacc.
+(Welw. ex Carrière) Byng & Christenh.
 (Wernham ex S.Moore) Markgr.
 (Wernham) Markgr.
 (Wernham) Pichon
 (Wernham) S.Moore ex Markgr.
 (West & G.S.West ex N.Carter) J.R.Stein
 (West & G.S.West) A.M.Scott & Grönblad
 (West & G.S.West) A.M.Scott & Prescott
@@ -21114,22 +21395,24 @@
 (West) W.West & G.S.West
 (West) West & G.S.West
 (West) Willi Krieg.
 (Westend.) O.E.Erikss.
 (Westend.) Sacc.
 (Weston) Duchesne ex Rozier
 (Wettst.) W.R.Barker
+(Whalley & Watling) M.Stadler & Læssøe
 (Whedon & Kof.) A.R.Loebl. & L.A.Loebl.
 (Whedon & Kof.) Balech
 (Whedon & Kof.) F.J.R.Taylor
 (Whibley) Pedley
 (Whiffen) Sparrow
 (Wick.) Kurtzman
 (Wick.) Kurtzman & M.Suzuki
 (Wick.) Minter
+(Wick., Kurtzman & Herman) Van der Walt & Arx
 (Wiegand) Fernald & Griscom
 (Wiegand) Jauzein
 (Wiegand) Rydb.
 (Wiegand) Shinners
 (Wight & Arn.) Baker
 (Wight & Arn.) Benth.
 (Wight & Arn.) Benth. & Hook.f.
@@ -21145,15 +21428,14 @@
 (Wight & Arn.) P.I.Forst.
 (Wight & Arn.) Pax & K.Hoffm.
 (Wight & Arn.) Seem.
 (Wight & Arn.) Takeda ex Dunn
 (Wight & Arn.) Verdc.
 (Wight & Arn.) Walp.
 (Wight & Arn.) Wilmot-Dear
-(Wight) Baill.
 (Wight) Benth.
 (Wight) Benth. & Hook.f.
 (Wight) Decne.
 (Wight) Engl.
 (Wight) F.M.Bailey
 (Wight) H.Hara
 (Wight) Jean F.Brunel
@@ -21220,14 +21502,15 @@
 (Willd.) Gillot & Lucand
 (Willd.) Graebn.
 (Willd.) Greuter
 (Willd.) H.Ito
 (Willd.) H.J.Lam
 (Willd.) H.Ohashi & K.Ohashi
 (Willd.) Hale
+(Willd.) Hartm.
 (Willd.) Haw.
 (Willd.) Holub
 (Willd.) Hook.
 (Willd.) Hook.f.
 (Willd.) I.C.Nielsen
 (Willd.) J.Jacq.
 (Willd.) J.M.Black
@@ -21316,27 +21599,27 @@
 (Willi Krieg.) Thomasson
 (Willi Krieg.) Willi Krieg. & Gerloff
 (Willk.) Rech.f.
 (Willoughby & Townley) D.R.Simmons
 (Willoughby) A.Batko
 (Willoughby) Willoughby
 (Wills & J.J.Bruhl) Wills & J.J.Bruhl
-(Wilson & Hook.f.) M.Fleisch.
-(Wilson & Hook.f.) Paris
-(Wilson & Hook.f.) Wilson
 (Wilson) A.Jaeger
 (Wilson) Broth.
 (Wilson) Dixon
 (Wilson) E.F.Warb.
+(Wilson) Fife
 (Wilson) I.G.Stone
+(Wilson) Ignatov & Vanderp.
 (Wilson) J.H.Willis
 (Wilson) Jur.
 (Wilson) Kindb.
 (Wilson) Mitt.
 (Wilson) Müll.Hal.
+(Wilson) Ochyra & Seppelt
 (Wilson) Paris
 (Wilson) Schiffn.
 (Wilson) Schimp.
 (Wilson) Wijk & Margad.
 (Wiltshire) S.Hughes
 (Wimm. & Grab.) Arcang.
 (Wimm. & Grab.) Petr. ex P.H.Davis & Parris
@@ -21351,27 +21634,29 @@
 (With.) J.R.Laundon
 (With.) Junge
 (With.) Lilj.
 (With.) Lutzoni
 (With.) M.Choisy
 (With.) Otálora, P.M.Jørg. & Wedin
 (With.) Pers.
+(With.) R.H.Zander
 (With.) Roze & Richon
 (With.) Tzvelev
 (With.) Á.Löve & D.Löve
 (Witkowski & Lange-Bert.) Sabbe & Vyverman
 (Wittr.) Cushman
 (Wittr.) Hansg.
 (Wittr.) Hochr.
 (Wittr.) J.Roy
 (Wittr.) Kirchn.
 (Wittr.) Nordst.
 (Woelk.) Garbary
 (Wolf) Endl.
 (Wolfe & Bougher) Halling & N.A.Fechner
+(Wolfe & Bougher) Y.C.Li & Zhu L.Yang
 (Wolfg. ex Hoffm.) Hook.f.
 (Wolle) A.D.Hardy
 (Wolle) F.E.Drouet
 (Wolle) G.M.Sm.
 (Wolle) Gerrath
 (Wolle) Playfair
 (Wolle) Teiling
@@ -21401,21 +21686,21 @@
 (Woodw.) J.Agardh
 (Woodw.) J.V.Lamour.
 (Woodw.) M.Howe
 (Woolls & F.Muell.) F.M.Bailey
 (Woolls & F.Muell.) F.Muell.
 (Wooton) Britton & Rose
 (Wooton) Sarg.
+(Wooton) Standl.
+(Worapong, Strobel & W.M.Hess) Samarak., Thongbai, K.D.Hyde & M.Stadler
 (Woronichin) Willi Krieg.
 (Wujek & Kristiansen) K.H.Nicholls
-(Wulfen : Fr.) P.D.Orton & Watling
 (Wulfen ex Hoppe) Asch. & Graebn.
 (Wulfen ex Hoppe) Batt.
 (Wulfen ex Hoppe) Boiss.
-(Wulfen ex Roth) J.Agardh
 (Wulfen) A.Massal.
 (Wulfen) Ach.
 (Wulfen) C.Agardh
 (Wulfen) Dalla Torre & Sarnth.
 (Wulfen) Fr.
 (Wulfen) Harv.
 (Wulfen) Hertel
@@ -21423,32 +21708,32 @@
 (Wulfen) J.Agardh
 (Wulfen) J.Schröt.
 (Wulfen) J.V.Lamour.
 (Wulfen) Körb.
 (Wulfen) Lloyd
 (Wulfen) Maire
 (Wulfen) Nyl.
+(Wulfen) P.D.Orton & Watling
 (Wulfen) P.Karst.
 (Wulfen) P.Kumm.
-(Wulfen) Poetsch
 (Wulfen) Quél.
 (Wulfen) Schaer.
 (Wulfen) Schumach.
 (Wulfen) Singer
 (Wulfen) Trevis.
-(Wulfen) Watling & P.D.Orton
 (Wulfen) Wünsche
 (Y.Ling & T.L.Chen) Vánky
 (Y.M.Ju & J.D.Rogers) Y.M.Ju, J.D.Rogers & H.M.Hsieh
-(Y.Miyake & T.Komin. ex M.Oda) G.I.Hansen & Moestrup
 (Y.Nisik. & C.Miyake) Shoemaker
 (Y.Nisik.) Drechsler ex Dastur
 (Y.Nisik.) Shoemaker
 (Y.Nisik.) Subram. & B.L.Jain
+(Y.Nomura) U.Braun & S.Takam.
 (Y.Ohmura) Articus
+(Y.S.Chang & A.K.Mills) Y.S.Chang, A.K.Mills, G.M.Gates & Ratkowsky
 (Y.Saito & Womersley) Garbary & J.T.Harper
 (Y.Saito & Womersley) K.W.Nam
 (Y.Saito) K.W.Nam
 (Y.V.Rolle) Deflandre
 (Y.W.Ho) Y.W.Ho
 (Yamada & Tak.Tanaka) Itono & Yoshiz.
 (Yamada & Tak.Tanaka) Kobara & Chihara
@@ -21460,18 +21745,23 @@
 (Yamada) R.E.Norris
 (Yamada) S.Berger, Fettweiss, Gleissberg, L.B.Liddle, U.Richt., Sawitzky & Zuccarello
 (Yamada) Schnetter & Bula Meyer
 (Yamada) Yamada
 (Yamam.) M.Hiroe
 (Yamam.) Makino
 (Yamash.) T.E.Brooks & H.W.Keller
+(Yanna & K.D.Hyde) Yanna & K.D.Hyde
 (Yasuda) D.D.Awasthi
+(Yasuda) Spatafora, Hywel-Jones & Luangsa-ard
 (Yendo) K.C.Fan & Y.P.Fan
 (Yendo) Yendo
 (Z.Q.Yuan & Kile) A.E.Paulin, T.C.Harr. & McNew
+(Z.Q.Yuan & Kile) Z.W.de Beer, T.A.Duong & M.J.Wingf.
+(Z.Q.Yuan, Wardlaw & C.Mohammed) Crous
+(Zach.) Jørg.
 (Zacharias) Iwanoff
 (Zahlbr.) A.Crespo, Divakar & Elix
 (Zahlbr.) Aptroot & Lücking
 (Zahlbr.) Asahina
 (Zahlbr.) Blaha & H.Mayrhofer
 (Zahlbr.) Brako
 (Zahlbr.) C.W.Dodge
@@ -21482,15 +21772,14 @@
 (Zahlbr.) Elix & Hale
 (Zahlbr.) Elix & J.Johnst.
 (Zahlbr.) Elix, Lumbsch & Lücking
 (Zahlbr.) Essl.
 (Zahlbr.) Frisch
 (Zahlbr.) Frisch & Kalb
 (Zahlbr.) G.Salisb.
-(Zahlbr.) Gyeln.
 (Zahlbr.) H.Magn.
 (Zahlbr.) H.Mayrhofer
 (Zahlbr.) H.Mayrhofer & Elix
 (Zahlbr.) Hale
 (Zahlbr.) Hertel
 (Zahlbr.) Hertel & Kilias
 (Zahlbr.) I.M.Lamb
@@ -21534,47 +21823,58 @@
 (Zanardini) Papenf.
 (Zanardini) Setch. & N.L.Gardner
 (Zanardini) Solms
 (Zanardini) Sond.
 (Zanardini) Womersley
 (Zanardini) Zanardini
 (Zanon) Hust.
+(Zanten) L.T.Ellis
+(Zeller & C.W.Dodge) A.H.Sm.
+(Zeller & C.W.Dodge) E.Horak
+(Zeller & C.W.Dodge) G.Cunn.
+(Zeller & C.W.Dodge) G.W.Beaton, Pegler & T.W.K.Young
+(Zeller & C.W.Dodge) Peintner & M.M.Moser
 (Zeller & C.W.Dodge) Singer & A.H.Sm.
+(Zeller & C.W.Dodge) T.Lebel
 (Zeller) Cribb
 (Zeller) Vellinga
 (Zenker) Hale
 (Zenker) Zahlbr.
 (Zhao, Hsu & Sun) Wei
 (Zimm.) Boedijn
 (Zimm.) Deighton
 (Zimm.) Höhn.
 (Zipp. ex Lév.) G.Cunn.
 (Zipp. ex Lév.) Núñez
 (Zipp. ex Miq.) Planch.
 (Zipp.) Kuntze
 (Zipp.) Radlk.
+(Zmitr. & Malysheva) Berk.
 (Zoll. & Moritzi) C.V.Morton
 (Zoll. & Moritzi) Corner
 (Zoll. & Moritzi) H.Ohashi & K.Ohashi
 (Zoll. & Moritzi) Kuntze
 (Zoll. & Moritzi) R.H.Petersen
 (Zoll. & Moritzi) Schodde
 (Zoll. & Moritzi) Seidenf.
 (Zoll.) Hartog
+(Zoll.) Ooststr.
 (Zopf) A.Fisch.
 (Zopf) Letcher
 (Zopf) M.W.Dick
 (Zopf) Sacc.
 (Zuccagni) Trotter
+(Zuccaro & M.Weiss) M.Weiss, F.Waller, Zuccaro & Selosse
 (Zukal) Anagn. & Komárek
 (Zukal) C.R.Benj.
 (Zukal) Forti
 (Zukal) G.W.Martin
 (Zundel) L.Guo
 (Zundel) Langdon & Full.
+(Zundel) McTaggart & R.G.Shivas
 (Zundel) Vánky
 (d'Urv.) Hook.f.
 (d'Urv.) K.F.Chung
 (d'Urv.) P.W.Ball
 (de Bary & Rostaf.) G.Lister
 (de Bary & Woronin) A.E.Johanson
 (de Bary & Woronin) A.Fisch.
@@ -21583,16 +21883,19 @@
 (de Bary) Lütkem.
 (de Bary) Mark A.Spencer
 (de Bary) Playfair
 (de Bary) Rostaf.
 (de Bary) Savile
 (de Bary) W.Archer
 (de Bary) Willi Krieg.
+(de Hoog & G.A.de Vries) R.T.Moore
+(de Hoog & G.A.de Vries) Sigler
+(de Hoog & G.A.de Vries) Z.W.de Beer, Begerow & R.Bauer
 (de Hoog) Subram. & Sudha
-(de Hoog, E.Guého & M.T.Sm.) de Hoog & M.T.Sm.
+(de Hoog, M.T.Sm. & E.Guého) de Hoog & M.T.Sm.
 (de Vriese) Benth.
 (de Vriese) Carolin
 (de Vriese) D.A.Morrison
 (de Vriese) Domin
 (de Vriese) Druce
 (de Vriese) E.Pritz.
 (de Vriese) F.Muell. ex Hook.f.
@@ -21612,24 +21915,29 @@
 (Østrup) Hust.
 (Østrup) Krasske
 (Østrup) R.M.Crawford
 (Østrup) Witkowski, Lange-Bert. & Metzeltin
 (Øvstedal) Elix
 A.A.Burb.
 A.A.Fisch.Waldh.
+A.A.Francis & Bougher
 A.A.Ham.
+A.A.Holland & Pegler
 A.A.Padhye & Ajello
 A.A.Padhye, Ajello & McGinnis
+A.A.Wynns
 A.B.Costin
+A.B.Costin, M.Gray, Totterdell & Wimbush
 A.B.Frank
 A.B.Jacks.
 A.B.Joly & Pinheiro
 A.B.Joly & Yam.-Tomita
 A.B.Joly & Yam.-Tomita ex A.B.Joly
 A.B.Rchb.
+A.B.Sharma & Dearnaley
 A.Batko
 A.Baumann & N.Baumann
 A.Benn.
 A.Berger
 A.Bloxam ex Berk. & Broome
 A.Blytt
 A.Br. ex Magnus
@@ -21652,44 +21960,33 @@
 A.Cabral, Rego & Crous
 A.Camus
 A.Cels
 A.Cels & J.F.Cels
 A.Chev.
 A.Child
 A.Cleve
-A.Cleve ex Åke Berg
 A.Crespo, Divakar & Elix
 A.Crespo, Ferencova & Divakar
 A.Cunn.
 A.Cunn. & C.Fraser ex Hook.
 A.Cunn. & Hook.
 A.Cunn. ex A.DC.
 A.Cunn. ex A.Gray
 A.Cunn. ex Benth.
-A.Cunn. ex Benth. x Acacia celsa Tindale
-A.Cunn. ex Benth. x Acacia crassicarpa A.Cunn. ex Benth.
-A.Cunn. ex Benth. x Acacia decora Rchb.
-A.Cunn. ex Benth. x Acacia disparrima M.W.McDonald & Maslin
-A.Cunn. ex Benth. x Acacia midgleyi M.W.McDonald & Maslin
-A.Cunn. ex Benth. x Acacia polystachya A.Cunn. ex Benth.
-A.Cunn. ex Benth. x Acacia tindaleae Pedley
 A.Cunn. ex Brongn.
+A.Cunn. ex C.Fraser & Hook.
 A.Cunn. ex DC.
 A.Cunn. ex Decne.
 A.Cunn. ex Domin
 A.Cunn. ex Don
 A.Cunn. ex Endl.
 A.Cunn. ex Ettingsh.
 A.Cunn. ex F.Muell.
 A.Cunn. ex Fenzl
 A.Cunn. ex G.Don
-A.Cunn. ex G.Don x Acacia macradenia Benth.
-A.Cunn. ex G.Don x Acacia neriifolia A.Cunn. ex Benth.
-A.Cunn. ex G.Don x Acacia perangusta (C.T.White) Pedley
-A.Cunn. ex G.Don x Hovea impressinerva I.Thomps.
 A.Cunn. ex Heward
 A.Cunn. ex Hook.
 A.Cunn. ex Hook.f.
 A.Cunn. ex J.M.Black
 A.Cunn. ex J.Oxley
 A.Cunn. ex Jacques
 A.Cunn. ex Juss.
@@ -21705,118 +22002,115 @@
 A.Cunn. ex Moq.
 A.Cunn. ex Mudie
 A.Cunn. ex Otto & A.Dietr.
 A.Cunn. ex Planch.
 A.Cunn. ex Putt.
 A.Cunn. ex Puttock
 A.Cunn. ex R.Br.
-A.Cunn. ex R.Br. x Persoonia stradbrokensis Domin
-A.Cunn. ex R.Br. x Persoonia tenuifolia R.Br.
-A.Cunn. ex R.Br. x Persoonia volcanica P.H.Weston & L.A.S.Johnson
 A.Cunn. ex R.T.Baker & H.G.Sm.
 A.Cunn. ex Schauer
-A.Cunn. ex Schauer x Eucalyptus prava L.A.S.Johnson & K.D.Hill
 A.Cunn. ex Sims
 A.Cunn. ex Steetz
 A.Cunn. ex Steud.
 A.Cunn. ex T.Mitch.
 A.Cunn. ex Tul.
 A.Cunn. ex Vogel
 A.Cunn. ex W.Hill
 A.Cunn. ex Walp.
 A.Cunn. ex Wedd.
 A.Cunn. ex Woolls
-A.Cunn. x Dendrobium linguiforme Sw.
-A.Cunn. x Dendrobium mortii F.Muell.
-A.Cunn. x Dendrobium striolatum Rchb.f.
-A.Cunn. x Dendrobium striolatum Rchb.f.) x Dendrobium pugioniforme A.Cunn.
-A.Cunn. x Dendrobium tenuissimum Rupp
-A.Cunn. x Dendrobium teretifolium R.Br.
-A.Cunn. x Dendrobium teretifolium var. fairfaxii F.M.Bailey
 A.D.Chapm.
 A.D.Chapm. ex Engelm.
 A.D.Hardy
 A.D.Hawkes
 A.D.Hocking
 A.D.Hocking & Pitt
 A.D.Hocking & Whitelaw
+A.D.Orb.
+A.D.Webb, L.T.Monks &Wege
 A.DC.
 A.DC. ex Meisn.
+A.David & Rajchenb.
 A.Dietr.
 A.E.Bell
 A.E.Bell & Mahoney
 A.E.Bell & N.Lundq.
 A.E.Freeman
 A.E.Holland
 A.E.Holland & D.W.Butler
 A.E.Holland & E.J.Thomps.
 A.E.Holland & R.Butcher
 A.E.Holland & S.T.Reynolds
 A.E.Holland & T.P.Boyle
 A.E.Johanson
 A.E.Kelly, Napier & Hopper
 A.E.Wood
-A.E.Wood & B.J.Rees
 A.Eddy ex M.Menzel
 A.Ernst
 A.Evans
 A.F.Bartsch
 A.F.Peters
 A.Fisch.
 A.G.Eliasson
+A.G.Floyd
 A.G.Ham.
 A.G.Henckel
 A.Gaertn.
 A.Gaertn. ex D.J.S.Barr
 A.García
 A.Gepp
 A.Gepp & E.Gepp
+A.Giraldo & Crous
 A.Gray
 A.Gray ex Benth.
 A.Gray ex Kunth
-A.Gray x Indigofera australis Willd.
 A.H.Moore
 A.H.S.Lucas
 A.H.Sm.
 A.H.Sm. & D.A.Reid
 A.H.Sm. & Hesler
-A.H.Sm. & M.Lange
-A.H.Sm. & Mazzer
 A.H.Sm. & Singer
 A.H.Sm. & Thiers
 A.Hansen & Sunding
 A.Hay
 A.Hay & S.Taylor
 A.Hay, M.D.Barrett & R.L.Barrett
 A.Heller
 A.Hempel
 A.Henry
+A.Hern.Gut. & B.Sutton
 A.J.Alverson, S.H.Kang & E.C.Theriot
 A.J.Br.
 A.J.Br. & N.G.Walsh
 A.J.Ford
 A.J.Ford & Duretto
 A.J.Ford & Halford
 A.J.Ford & P.H.Weston
 A.J.Ford & Peter G.Wilson
 A.J.Ford, Craven & Brophy
 A.J.Ford, Craven & J.Holmes
 A.J.G.Wilson
 A.J.G.Wilson & Hislop
+A.J.Inman & Sivan.
 A.J.L.Phillips
+A.J.L.Phillips & Luque
+A.J.L.Phillips, A.Alves & Crous
+A.J.L.Phillips, Slippers, Boissin & Crous
 A.J.Paton
 A.J.Perkins
+A.J.Rea, Stukely & T.Jung
 A.J.Richards
 A.J.Schill.
 A.J.Scott
 A.J.Whalen & B.J.Conn
 A.Jaeger
 A.Jaeger ex A.Jaeger
 A.Juss.
 A.Jörg.
+A.K.Gibbs & Ladiges
 A.K.Irvine
 A.K.Kop.
 A.K.Sarbhoy
 A.Kalotas
 A.Keller
 A.Kern.
 A.L.Curtis & K.R.Thiele
@@ -21842,14 +22136,15 @@
 A.M.Prescott
 A.M.Scott
 A.M.Scott & Grönblad
 A.M.Scott & Prescott
 A.M.Scott ex Croasdale
 A.M.Young
 A.M.Young & A.K.Mills
+A.M.Young & K.Syme
 A.M.Young & N.A.Fechner
 A.M.Young, R.Kearney & E.Kearney
 A.Mann
 A.Massal.
 A.Massal. & De Not.
 A.Massal. ex Kremp.
 A.Maxwell
@@ -21888,29 +22183,28 @@
 A.R.Bean & Brooker
 A.R.Bean & Henwood
 A.R.Bean & Jessup
 A.R.Bean & Jobson
 A.R.Bean & M.T.Mathieson
 A.R.Bean & P.I.Forst.
 A.R.Bean & Sharpe
-A.R.Bean x Pterocaulon serrulatum (Montrouz.) Guillaumin
-A.R.Bean x Pterocaulon verbascifolium (Benth.) F.Muell.
-A.R.Bean x Solanum nemophilum F.Muell.
+A.R.Caval. & T.W.Johnson
 A.R.Chapm.
 A.R.Chapm. & Maslin
 A.R.Davis
 A.R.Delile ex A.Braun
 A.R.Field
 A.R.Field & Bostock
 A.R.Loebl.
 A.R.Loebl. & Tappan
 A.R.Loebl., Sherley & R.J.Schmidt
 A.R.Mast & K.R.Thiele
 A.R.Patil, T.M.Patil & M.S.Patil
 A.R.Paul
+A.R.Paul & Parbery
 A.R.Penfold & J.L.Willis
 A.R.Penfold & M.B.Welch
 A.R.Sm.
 A.R.Williams
 A.Rea, Stukely & T.Jung
 A.Rich.
 A.Rich. ex DC.
@@ -21929,29 +22223,29 @@
 A.S.Harv. & Woelk.
 A.S.Markey
 A.S.Markey & R.A.Meissn.
 A.S.Markey & R.Butcher
 A.S.Markey, S.J.Dillon & R.M.Barker
 A.S.Mitch.
 A.S.Mitch. ex Craven & Fryxell
+A.S.Patil & V.G.Rao
 A.S.Rob., A.T.Cross, Meisterl & A.Fleischm.
 A.Schimp.
 A.Schimp. & Vanhöffen
 A.Schimp. ex G.Karst.
 A.Schmidt
 A.Schott ex Engelm.
 A.St.-Hil.
 A.St.-Hil. ex Gray
 A.St.-Hil., A.Juss. & Cambess.
 A.Stokes
 A.T.Cross & Adamec
 A.T.Lee
-A.T.Lee - Crotalaria mitchellii Benth.
-A.T.Lee x Xanthorrhoea latifolia (A.T.Lee) D.J.Bedford
 A.T.Webb
+A.T.Webb, Birch & R.L.Barrett
 A.Terracc.
 A.V.Bobrov & Melikyan
 A.V.Jennings
 A.V.V.Iyengar
 A.V.V.Iyengar ex A.V.V.Iyengar
 A.Vilm.
 A.W.Archer
@@ -21968,21 +22262,23 @@
 A.W.Hill ex J.M.Black
 A.W.Howitt
 A.W.Phillips
 A.W.Ramaley
 A.Wallace
 A.Wulff
 Aa
+Abad, De Cock, K.Bala, Robideau, A.M.Lodhi & Lévesque
 Abbayes
+Abdel-Wahab & E.B.G.Jones
+Abdollahz., Javadi & A.J.L.Phillips
 Abedin
 Aberdeen
 Abrom.
 Ach.
 Ach. ex Flot.
-Ach. ex Michx.
 Ach. ex Pers.
 Ach. ex Schaer.
 Adachi & Fukuyo
 Adamson
 Adamson & Sprague
 Adans.
 Adans. ex Fr.
@@ -22004,65 +22300,65 @@
 Afzel. ex Urb.
 Agerer
 Aghighi, G.E.St.J.Hardy, J.K.Scott & T.I.Burgess
 Ahmad
 Ahti
 Ahti & Kashiw.
 Ahti & P.James
-Ahti, Elix & Ovstedal
 Ainsw.
 Airy Shaw
 Airy Shaw & B.Hyland
 Airy Shaw & G.L.Webster
 Airy Shaw & Turrill
-Airy Shaw x Croton dockrillii Airy Shaw
 Aitch.
 Aitch. & Hemsl.
 Aiton
 Aiton ex A.Cunn.
 Aiton ex Hook.
 Aiton ex Steud.
 Ajello
-Ajello & McGinnis
 Ajello & S.L.Cheng
 Ajello, Georg & C.J.K.Wang
 Akagi ex Sugita, A.Nishikawa & Shinoda
+Al-Hatmi, S.A.Ahmed & de Hoog
+Al-Shehbaz
 Alarcon, Aldasoro, C.Navarro & C.Aedo
 Alas.
 Alb. & Schwein.
 Albert
 Albr.
 Albr. & A.R.Bean
 Albr. & B.L.Rye
 Albr. & Chinnock
 Albr. & Cowie
+Albr. & J.G.West
 Albr. & Lally
 Albr. & N.G.Walsh
 Albr. & Paul G.Wilson
 Albr. & R.W.Jobson
 Alcoba-Flórez, Méndez-Álv., Cano, Guarro, Pérez-Roth & M.P.Arévalo
 Alcorn
 Alcorn & J.A.G.Irwin
+Alcorn & J.Walker
+Alcorn & P.F.Cannon
+Alcorn & P.M.Kirk
 Alcorn & R.G.Shivas
 Alcorn & S.M.Francis
 Alcorn & Sivan.
-Alcorn, R.G.Shivas & Sivan.
 Aldasoro, Aedo, C.Navarro & L.Sáez
 Alderw.
 Aleem & Hust.
 Alef.
 Alexander ex H.E.Moore
 Alexop.
 Alexop. & Beneke
 Alford
 Ali
 Ali & Robbr.
 All.
-All. x Aloe parvibracteata Schönland
-All. x Aloe striata Haw.
 Allan
 Allen
 Allender & G.T.Kraft
 Alles, M.Nörpel & Lange-Bert.
 Allesch.
 Allison
 Allorge & Jovet-Ast
@@ -22075,36 +22371,37 @@
 Amos & H.L.Barnett
 An.Kumar, Bajpai, A.K.Mishra, N.Sahu, S.Behera & L.B.Chaudhary
 Anagn. & Komárek
 Anand
 Anastasiou
 Anderb.
 Anderb. & Haegi
-Anderb., B.Stahl & Kallersjo
+Anderb., B.Stahl & Källersjö
 Anders
 Andersson
 Andjic & P.A.Barber
 Andjic & S.Jacks.
 Andjic & T.I.Burgess
 Andjic, Carnegie & P.A.Barber
 Andjic, P.A.Barber & T.I.Burgess
+Andjic, T.I.Burgess & A.Maxwell
 Andrews
-Andrews x Daviesia wyattiana F.M.Bailey
 Andrz.
 Andrz. ex Besser
 André
 Angstr.
 Anisimova
 Annesley
 Anon.
 Anth.Bishop
 Antoine
 Anzi
 Apfelbaum
 Apinis
+Apinis & R.G. Rees
 Apstein
 Aptekar
 Aptroot
 Aptroot & Chaves
 Aptroot & Lücking
 Aptroot & M.Cáceras
 Aptroot & Sipman
@@ -22118,46 +22415,48 @@
 Ardiss. & J.Straff.
 Ardiss. & J.Straff. ex Gomont
 Ardré
 Arechav.
 Arenes
 Aresch.
 Aresch. ex J.Agardh
-Argüello & A.Crespo
 Argüello & Crespo
 Ariati
+Arifin, Reiter, T.W.May & C.C.Linde
+Arifin, T.W.May & C.C.Linde
+Ariy. & K.D.Hyde
 Arn.
 Arn. ex Grev.
 Arn. ex Harv.
-Arn. ex Hook.f.
 Arn. ex Hust.
 Arn. ex Nees
 Arn. ex R.Br.
 Arn. ex Ralfs
 Arnell
 Arnell & J.Perss.
 Arnold
 Arnoldi
 Arnolds
 Arriaga & Barkworth
 Arrigoni
 Art.Mey.
 Arthur
+Arthur & Cummins
 Arts
 Arup, Frödén & Søchting
 Arup, Søchting & Frödén
 Arv.
 Arv. & D.J.Galloway
 Arx
 Arx & Constant.
 Arx & D.L.Olivier
 Arx & E.Müll.
 Arx & J.S.F.Barker
-Arx & Van der Walt
-Arx & de Hoog
+Arzanlou & Crous
+Arzanlou, W.Gams & Crous
 Asahina
 Asch.
 Asch. & Graebn.
 Ashby
 Ashford
 Ashton & McCrae
 Ashwin
@@ -22170,29 +22469,33 @@
 Athanas., Garbary & Vanderm.
 Athanassopoulos
 Atienza & D.Hawksw.
 Aubl.
 Aubrév.
 Audas
 Audas & P.Morris
+Audet
 Auersw.
 Auersw. ex Fuckel
 Auersw. ex Heiberg
 Auersw. ex Rabenh.
 Aug.DC.
 Augier ex Post & Kuntze
 Auriv.
 Ausfeld
 Austin
 Australian National Herbarium
 Aveskamp, Gruyter & Verkley
 Avé-Lall.
+Aylward, Marinc. & M.J.Wingf.
 B-E.van Wyk
+B.Archer & Maroske
 B.Boivin
-B.C.Ho & G.T.P.Vo
+B.C.Paulus, Gadek & K.D.Hyde
+B.C.Paulus, M.E.Barr & K.D.Hyde
 B.C.Stone
 B.C.Tan
 B.C.Tan, W.B.Schofield & H.P.Ramsay
 B.C.Wilde & R.L.Barrett
 B.C.Zhang & Minter
 B.Chandler
 B.D.Jacks.
@@ -22205,15 +22508,14 @@
 B.Eichler & Racib.
 B.F.Osorio
 B.G.Baldwin
 B.G.Briggs
 B.G.Briggs & Ehrend.
 B.G.Briggs & H.P.Linder
 B.G.Briggs & L.A.S.Johnson
-B.G.Briggs & L.A.S.Johnson x Lepyrodia verruculosa B.G.Briggs & L.A.S.Johnson
 B.G.Briggs & Makinson
 B.G.Briggs, B.Hyland & L.A.S.Johnson
 B.G.Briggs, Carolin & Pulley
 B.G.Thomson
 B.Gray
 B.Gray & D.L.Jones
 B.Gray & Y.W.Low
@@ -22241,70 +22543,74 @@
 B.J.Conn & K.A.Sheph.
 B.J.Conn & K.M.Proft
 B.J.Conn & P.G.Richards
 B.J.Conn & Quirico
 B.J.Conn & T.C.Wilson
 B.J.Conn & Tame
 B.J.Conn & Tozer
+B.J.Croft & M.W.Dick
 B.J.Keighery & Keighery
 B.J.Mole
 B.J.Rees
+B.J.Rees & A.E.Wood
+B.J.Rees & K.Syme
+B.J.Rees & Lepp
 B.J.Sm. & Sivasith.
 B.K.Cui & Shun Liu
 B.K.Cui & Xing Ji
 B.K.Cui & Y.F.Sun
+B.K.Cui, H.J.Li & Y.C.Dai
+B.K.Cui, M.L.Han & Y.C.Dai
+B.K.Cui, Shun Liu & Y.C.Dai
 B.K.Nayar
 B.K.Simon
 B.K.Simon & C.M.Weiller
 B.K.Simon & Cowie
-B.K.Simon x Arundinella montana S.T.Blake
 B.L.Burtt
 B.L.Jain
 B.L.Linden
 B.L.Turner
 B.L.Webber
 B.Leadb. & J.D.Dodge
 B.Lindeb.
 B.M.Anderson
 B.M.Anderson & M.D.Barrett
 B.M.Horton & Crayn
 B.M.Thiers
 B.M.Thiers & Gradst.
 B.M.Thiers ex L.Söderstr. & A.Hagborg
 B.Mathew
+B.Mishler, N.E.Bell & P.J.Dalton
 B.Nord.
 B.R.Paterson
 B.S.Fisher & Schweick.
 B.S.Mehrotra & Baijal
+B.S.Weir & P.R.Johnst.
 B.S.Williams
 B.Sutton
-B.Sutton & A.Hern.Gut.
 B.Sutton & Alcorn
-B.Sutton & Bhat
-B.Sutton & D.E.Shaw
 B.Sutton & E.M.Davison
 B.Sutton & Ganap.
+B.Sutton & H.J.Swart
 B.Sutton & Hodges
 B.Sutton & P.M.Kirk
 B.Sutton & Pascoe
 B.Sutton & Pollack
 B.Sutton & R.Campb.
 B.Sutton & Sankaran
 B.Sutton & Shaw
-B.Sutton, Muthumary & Abbas
 B.Vogel
 B.W.Horn, I.Carbone & Ram.-Prado
 B.W.van Ee, P.I.Forst. & P.E.Berry
 B.Xue & R.M.K.Saunders
 B.de Lesd.
 B.Øllg.
 Baardseth
 Baarud
 Bab.
-Bab. ex Planch.
 Babc. & Stebbins
 Babeva & Reshetova
 Bacc.
 Bach.Pyl.
 Bachm.
 Backeb.
 Backer
@@ -22312,19 +22618,20 @@
 Backh. ex Hook.f.
 Backh. ex Planch.
 Baehni
 Bagl.
 Baijnath
 Bailey
 Bailey & Ralfs
+Bailey ex Berk. & Broome
+Bailey ex L.W.Bailey
 Bailey ex Ralfs
 Baill.
 Baill. ex Franch.
 Baill. ex Müll.Arg.
-Baill. x Croton stigmatosus F.Muell.
 Bain
 Bainier
 Bainier & Sartory
 Bainier ex Thom
 Bakalin
 Baker
 Baker ex Benth.
@@ -22345,14 +22652,15 @@
 Balech ex A.R.Loebl.
 Balech ex Loebl. & A.R.Loebl.
 Balech ex Matsuoka, Sa.Kobay. & G.Gains
 Baleeiro & R.W.Jobson
 Baleeiro, R.W.Jobson & R.L.Barrett
 Balf.
 Balgooy
+Balgooy & de Vogel
 Balletto
 Balsamo
 Bando
 Bange
 Banka & Barfod
 Banker
 Banks
@@ -22362,64 +22670,71 @@
 Banks & Sol. ex DC.
 Banks & Sol. ex G.Forst.
 Banks & Sol. ex Gaertn.
 Banks & Sol. ex Hiern
 Banks & Sol. ex Hook.f.
 Banks & Sol. ex Knight
 Banks & Sol. ex R.Br.
+Banks & Sol. ex Rees
 Banks ex Andrews
 Banks ex DC.
 Banks ex Gaertn.
 Banks ex K.D.Koenig
 Banks ex Lam.
 Banks ex Lowe
 Banks ex Murray
 Banks ex R.Br.
 Banks ex Sims
-Banks ex Vesque
 Banwell
 Banyard & S.H.James
 Baral
+Baral & E.Weber
 Baral & G.Marson
+Baral, G.Marson & E.Weber
+Baral, Quijada & R.Tena
+Baral, S.F.Li, J.W.Guo, Z.F.Yu & G.Marson
 Baran.
 Barbier
 Barclay
 Barfod & Dowe
 Barkworth & D.R.Dewey
 Barkworth & S.W.L.Jacobs
 Barla
 Barlow
 Barlow ex Craven
-Barlow x Melaleuca nervosa (Lindl.) Cheel
 Barneby & J.W.Grimes
 Barneby & Krukoff
 Barneoud
 Barnhart
 Barros
 Barros ex H.Pfeiff.
+Barrs, van Doorn, Varga & Samson
 Bartel & R.A.Price
 Barthol.
 Barthol.-Began
 Bartl.
 Bartl. & H.L.Wendl.
 Bartl. ex Bisch.
 Bartl. ex DC.
 Bartl. ex Lindl.
+Bartrop, R.G.Shivas, Bishop-Hurley & Y.P.Tan
 Bas
 Bassi ex L.
 Bastard
 Bastow
 Bat.
 Bat. & A.F.Vital
 Bat. & C.A.A.Costa
 Bat. & Cif.
 Bat. & H.Maia
+Bat. & J.L.Bezerra
 Bataille
 Bateman ex Lindl.
 Bateman ex Rchb.f.
+Bathgate, M.E.Barr & B.L.Shearer
 Batsch
 Batsch ex Borkh.
 Batt.
 Battarra
 Battarra ex Kuntze
 Batters
 Baum.-Bod. ex Doweld
@@ -22427,14 +22742,15 @@
 Baumg.
 Baxter
 Baxter ex A.Dietr.
 Baxter ex R.Br.
 Baxter ex Sweet
 Bayl.Ell. & O.P.Stansf.
 Bayly
+Bayly & R.Fowler
 Beal
 Bean
 Beard
 Beauverd
 Beauverd ex Steph.
 Beauvis.
 Becc.
@@ -22443,88 +22759,89 @@
 Becc. ex Oliv.
 Beck
 Becker & Lücking
 Beckett
 Bedd.
 Beeby
 Beeli
+Beenken
 Beesley
 Beever, Castellano & T.Lebel
-Begerow, Oberw. & M.Piepenbr.
-Begerow, Oberw., R.Bauer & A.Nagler
 Behr
 Behr & F.Muell.
 Behr & F.Muell. ex Miq.
 Behr & F.Muell. ex Sond.
 Behr ex Baker
 Behr ex Benth.
 Behr ex J.M.Black
 Behre
 Behrend
 Beier & Thulin
 Beij.
 Beilharz & Cunningt.
+Beilharz & Pascoe
+Beilharz, Cunningt. & Pascoe
+Beilharz, Mayers & Pascoe
+Beilharz, Pascoe & Parbery
+Beilharz, Pascoe, M.J.Wingf. & Crous
 Bek.
 Belcher
 Belcher & Albr.
 Belcher ex I.Thomps.
 Bellynck
 Beltr.
+Bender
 Bendiksby & Timdal
 Benedix
 Benj.
 Benl
 Benl & H.Eichler
 Benn.
 Benn. & R.Br.
+Bensch, Crous & U.Braun
+Bensch, Summerell, Crous & U.Braun
+Bensch, U.Braun & Crous
 Benth.
 Benth. & Hook.f.
 Benth. & Hook.f. ex Drake
-Benth. - Atriplex eardleyae Aellen
-Benth. - Atriplex pseudocampanulata Aellen
 Benth. ex A.Gray
 Benth. ex Baker
+Benth. ex DC.
 Benth. ex Ewart
 Benth. ex Guilf.
 Benth. ex H.B.Will.
 Benth. ex Harv.
 Benth. ex Hook.f.
 Benth. ex Jacques
 Benth. ex Lindl.
 Benth. ex Morrison
 Benth. ex Oliv.
 Benth. ex Seem.
-Benth. subsp. loxophleba x Eucalyptus spathulata Hook.
-Benth. x Acacia torulosa Benth.
-Benth. x Eucalyptus melanophloia F.Muell.
-Benth. x Eucalyptus melliodora A.Cunn. ex Schauer
-Benth. x Eucalyptus microcarpa (Maiden) Maiden
-Benth. x Eucalyptus rudis Endl.
-Benth. x Marsdenia viridiflora R.Br.
-Benth. x Nemesia versicolor E.Mey. ex Benth.
+Benwell
 Bercht. & J.Presl
 Berdan
 Berenger
 Berg
 Berggr.
 Bergh
 Bergius
 Bergmans
 Bergmans ex J.W.Ingram
 Bergon
 Berhaut
 Berk.
 Berk. & Broome
-Berk. & Broome ex C.W.Dodge & Zeller
 Berk. & Broome ex Cooke
 Berk. & Broome ex F.Muell.
 Berk. & Broome ex G.Cunn.
 Berk. & Broome ex Massee
 Berk. & Broome ex W.Phillips
+Berk. & Broome ex Zeller & C.W.Dodge
 Berk. & Cooke
+Berk. & Corda
 Berk. & Desm.
 Berk. & F.Muell.
 Berk. & Harv.
 Berk. & Harv. ex Hirn
 Berk. & Hook.f.
 Berk. & M.A.Curtis
 Berk. & M.A.Curtis ex Cooke
@@ -22550,27 +22867,29 @@
 Berk. ex Rifai
 Berk. ex Rostaf.
 Berk. ex Sacc.
 Berkhout
 Berl.
 Berl. & Sacc.
 Bernard
+Berndt
 Bernh.
 Bernh. ex C.Krauss
 Bernh. ex Rchb.
 Bernh. ex Willd.
 Berrie
 Bertault
 Bertault & Malençon
 Bertault ex Contu
 Bertel
 Bertero
 Bertero ex Mont.
 Bertero ex Savi
 Berthold
+Bertier, H.Brouwer & De Cock
 Bertol.
 Bertuch
 Besch.
 Besch. & C.Massal.
 Bess
 Besser
 Besser ex Rchb.
@@ -22579,20 +22898,20 @@
 Betts
 Beuzev. & C.T.White
 Beuzev. & M.B.Welch
 Beverw.
 Bews
 Bharadwaja
 Bhashyakarla Rao
+Bhat & B.Sutton
 Bhat & W.B.Kendr.
 Bialosuknia
 Biasol.
 Bibby
 Bidwill ex Lindl.
-Bidwill ex Lindl. x Dendrobium speciosum Sm.
 Biecheler
 Biedenf.
 Biehler
 Bigelow
 Biourge
 Birdsey
 Bisch.
@@ -22618,40 +22937,34 @@
 Blaha, H.Mayrhofer & Elix
 Blake
 Blakely
 Blakely & Beuzev.
 Blakely & C.T.White
 Blakely & H.Steedman
 Blakely & Jacobs
-Blakely & Jacobs - Eucalyptus microtheca F.Muell.
-Blakely & Jacobs x Eucalyptus crebra F.Muell.
-Blakely & Jacobs x Eucalyptus melanophloia F.Muell.
-Blakely & Jacobs x Eucalyptus populnea F.Muell.
-Blakely & Jacobs x Eucalyptus whitei Maiden & Blakely
 Blakely & McKie
 Blakely & McKie ex Blakely
 Blakely ex C.T.White
 Blakely ex Court
-Blakely x Eucalyptus microcarpa (Maiden) Maiden
 Blanch.
 Blanchon
 Blanchon & Bannister
 Blanco
+Blanco-Dios
 Blandow ex Voit
 Blatt. & McCann
 Blaxell
 Blaxell & K.D.Hill
 Bleisch
 Bliding
 Bloemb.
 Blum & Womersley
 Blume
 Blume & T.Nees
 Blume ex A.Juss.
-Blume ex Blume
 Blume ex Decne.
 Blume ex Endl.
 Blume ex Korth.
 Blume ex Kunze
 Blume ex Miq.
 Blume ex Nees
 Blume ex Raspail
@@ -22662,15 +22975,14 @@
 Blytt
 Blytt ex Andersson
 Bobrov ex Airy Shaw
 Bock
 Bodegom
 Boeckeler
 Boeckeler ex Schinz
-Boedeker
 Boedijn
 Boehm.
 Boenn.
 Boenn. ex Rchb.
 Boerema, Gruyter & Kesteren
 Boerema, Gruyter & P.Graaf
 Boerema, Loer. & Hamers
@@ -22710,16 +23022,18 @@
 Bondartsev
 Bondartsev & Singer
 Bong.
 Bonito, K.Hameed, Aime & Vilgalys
 Bonord.
 Bonord. ex Sacc.
 Bonpl.
+Bonthond, Sand.-Den. & Crous
 Boom
 Boomsma
+Boonmee & K.D.Hyde
 Booth
 Boott
 Boott ex C.B.Clarke
 Boott ex Hook.f.
 Bor
 Borbás
 Boreau
@@ -22764,81 +23078,85 @@
 Bostock & A.E.Holland
 Bostock & Spokes
 Bosw.
 Bosw. ex Paris
 Botes, Sym & G.C.Pitcher
 Boucher ex DC.
 Boud.
+Boud. & Pat.
 Boud. & Torrend
 Boud. ex Cooke
 Bougher
 Bougher & A.A.Francis
 Bougher & A.M.Young
 Bougher & Castellano
 Bougher & K.Syme
-Bougher & Matheny
-Bougher & Matheny ex Bougher & Matheny
 Bougher & R.N.Hilton
 Bougher & T.Lebel
 Bougher & Thiers
 Bougher & Trappe
-Bougher & Verbeken
+Bougher, E.M.Davison & Giustiniano
 Bougher, Fuhrer & E.Horak
-Bougher, O.K.Mill. & Matheny
-Bougher, O.K.Mill. & Matheny ex Bougher, O.K.Mill. & Matheny
+Bougher, Tommerup & Malajczuk
 Boulos
 Bourdot
 Bourdot & Galzin
 Bourg. ex Nyman
+Bouriquet ex Crous
+Bourke & A.S.Rob.
 Bourr.
 Boursier
 Bouton ex DC.
 Bower
 Bowie ex Hook.
 Bowman
+Boxshall, Broadbridge & T.Lebel
 Boyland
 Boyland & A.E.Holland
 Braarud
 Braaten, Bougher, & Matheny
 Brack.
 Brady
 Braid
 Braid & C.T.White
 Brako
 Brand
 Brandegee
 Brandt
+Branwhite
 Brasier, Sánch.Hern. & S.A.Kirk
 Breb.
 Breda
 Breda de Haan
 Bref.
-Bref. & Tavel
+Breistr.
 Breiter
 Bremek.
 Bremek. & Oberm.
-Bremek. var. australiensis - Pavetta granitica F.Muell. ex Bremek.
+Bremer & Petr.
 Brenan
 Brenan & Brummitt
 Brennan
 Brennan & Cowie
 Brennan, Martine & Symon
 Brenner
 Bres.
+Bres. & Henn. ex Sacc.
+Bres. & Pat.
 Bres. & Schulzer
 Bres. & Torrend
 Bres. ex Lloyd
 Bresinsky
 Bresinsky & Jarosch
 Bresinsky & Manfr.Binder
 Bressan
 Breton
 Breton & Faurel
+Breton, Bernalier, Bonnemoy, Fonty, B.Gaillard, & Gouet
 Breton, Bernalier, Dusser, Fonty, B.Gaillard & J.Guillot
-Breton, Bernalier, Fonty, B.Gaillard, Bonnemoy & Gouet
 Brett
 Breuss
 Breyne ex Kuntze
 Brick
 Brid.
 Brid. ex Bonner
 Brid. ex F.M.Bailey
@@ -22853,24 +23171,23 @@
 Brinsley
 Briosi & Cavara
 Briot
 Briq.
 Brittan
 Britten
 Britten & S.Moore
-Britten & S.Moore ex S.Moore
 Brittleb.
 Brittleb. & D.B.Adam
 Britton
 Britton & Killip
 Britton & Rose
 Britton & Rose ex Britton & Killip
 Britton, Sterns & Poggenb.
 Britzelm.
-Brizi
+Broadbridge, Boxshall & T. Lebel
 Broady
 Broch
 Brockm.
 Brockmann
 Brogli
 Bromhead
 Brond.
@@ -22880,32 +23197,21 @@
 Brongn. ex Neumann
 Bronn
 Brook & Hine
 Brooker
 Brooker & A.R.Bean
 Brooker & Blaxell
 Brooker & Done
-Brooker & Done x Eucalyptus pruinosa Schauer
 Brooker & Dunlop
 Brooker & Edgecombe
 Brooker & Hopper
-Brooker & Hopper - Eucalyptus perangusta Brooker
-Brooker & Hopper subsp. arachnaea x Eucalyptus orthostemon D.Nicolle & Brooker
-Brooker & Hopper x Eucalyptus dorrienii Domin
-Brooker & Hopper x Eucalyptus platypus subsp. congregata Brooker & Hopper
-Brooker & Hopper x Eucalyptus sporadica Brooker & Hopper
-Brooker & Hopper x Eucalyptus suggrandis L.A.S.Johnson & K.D.Hill
 Brooker & Kleinig
 Brooker & M.W.McDonald
-Brooker & M.W.McDonald x Eucalyptus platyphylla F.Muell.
 Brooker & P.J.Lang
 Brooker & Slee
-Brooker - Eucalyptus olivina Brooker & Hopper
-Brooker - Eucalyptus salicola Brooker
-Brooker x Eucalyptus xanthoclada Brooker & A.R.Bean
 Brooker, Boland & Kleinig
 Brooker, Connors & Slee
 Brooker, Slee & J.D.Briggs
 Brooker, Slee, Connors & Duffy
 Brot.
 Brot. ex Hornem.
 Broth.
@@ -22948,26 +23254,26 @@
 Bruch ex De Not.
 Bruch ex Schimp.
 Brugger
 Bruhne
 Brullo
 Brumh.
 Brumm.
+Brumm., Korf & Rifai
 Brummitt
 Brumpt
 Brun
 Brunaud
 Brundrett
 Bruner
 Brunken
 Brunnth.
 Brusse
 Brusse & C.H.Dickinson
 Bryhn
-Bryhn ex Warnst.
 Brândză
 Bréb.
 Bréb. & Arn. ex Kitton
 Bréb. & Kitton
 Bréb. & Ralfs
 Bréb. ex Bornet & Flahault
 Bréb. ex Cleve & Grunow
@@ -22998,27 +23304,28 @@
 Buchanan
 Buchenau
 Buchet
 Buchinger ex Hochst.
 Bucholtz
 Buchwalder & Wanke
 Buckley
+Buddin & Wakef.
 Buell
 Buetschli
 Bugnic.
 Buirchell & A.P.Br.
-Bukhtiyarova & Round
+Bukht. & Round
 Bula-Meyer
 Bull.
 Bull. & Vent.
-Bull. : Pers. ex Pers.
 Bull. ex Juss.
 Buller
 Bullock
 Bulnh.
+Bundhun, Tennakoon, Phookamsak & K.D.Hyde
 Bungartz
 Bungartz & U.Grube
 Bunge
 Bunge ex Ung.-Sternb.
 Burch.
 Burch. ex DC.
 Burchard
@@ -23046,26 +23353,23 @@
 Burnside
 Burret
 Burrill
 Bursa
 Burt
 Burt ex Rolfs
 Burtt Davy
-Busch
 Buse
 Buse ex de Vriese
 Butin
 Butters
 Butzin
 Buxb.
 Buyck & V.Hofst.
 Byng & Christenh.
 Byrnes
-Byrnes x Kunzea opposita F.Muell.
-Byrnes x Kunzea parvifolia Schauer
 Bég.
 Bél.
 Böcher
 Böhm
 Børgesen
 Büdel
 Büdel & Elix
@@ -23092,17 +23396,21 @@
 C.A.Gardner ex Olde & Marriott
 C.A.Gardner ex P.H.Weston
 C.A.Gardner ex P.J.Lang
 C.A.Gardner ex R.S.Cowan & Maslin
 C.A.Gardner ex Rajput & Carolin
 C.A.Gardner ex Rye
 C.A.Gardner ex Rye & Hislop
-C.A.Gardner subsp. formanii - Eucalyptus formanii subsp. circulata D.Nicolle & M.E.French
-C.A.Gardner x Eucalyptus platypus Hook.
+C.A.Gardner ex Strid & Keighery
 C.A.Mey.
+C.A.Pearce & K.D.Hyde
+C.A.Pearce, K.D.Hyde & R.G.Shivas
+C.A.Pearce, Reddell & K.D.Hyde
+C.A.Quandt, Kepler & Spatafora
+C.A.Rosa, Lachance, Starmer, J.S.F.Barker, J.M.Bowles & Schlag-Edl.
 C.A.Weber
 C.Agardh
 C.Agardh ex Bornet & Flahault
 C.Agardh ex Bruzelius
 C.Agardh ex Gomont
 C.Agardh ex Hirn
 C.Agardh ex J.Agardh
@@ -23119,42 +23427,48 @@
 C.B.Shang
 C.B.Shang & X.P.Li
 C.Bab.
 C.Bab. & Mitt.
 C.Bailey
 C.Bayer, M.W.Chase & M.F.Fay
 C.Bernard
+C.Boed.
 C.Booth
 C.Booth & C.Prior
+C.Booth & D.E.Shaw
 C.Booth & R.H.Stover
+C.Booth & Shipton
+C.Boucher, T.S.Nguyen & P.Silar
 C.Brockman
+C.C. Chen & Sheng H. Wu
 C.C.Berg
 C.C.Gmel.
 C.C.Jao
 C.C.Jao & Wei Yinxin
+C.C.Linde & T.W.May
 C.C.Robin
 C.Chr.
 C.Chr. & Ching
 C.Chr. & Ostenf.
 C.Clarke & R.Kruger
+C.Crane & T.I.Burgess
 C.Cusset & G.Cusset
 C.D.K.Cook
 C.D.Moon & Schardl
 C.D.Moon, C.O.Miles & Schardl
 C.DC.
 C.DC. & F.Muell.
 C.E.Anderson
 C.E.Britton
 C.E.C.Fisch.
 C.E.Chadwick
 C.E.Cramer
 C.E.Cramer ex Hirn
 C.E.Hubb.
 C.E.Hubb. ex N.T.Burb.
-C.E.Hubb. x Iseilema vaginiflorum Domin
 C.E.Marks
 C.E.O.Jensen
 C.F.Chang & B.M.Xia
 C.F.Chang & E.Z.Xia
 C.F.Gaertn.
 C.F.Ludw. ex Tepper
 C.F.Reed
@@ -23164,15 +23478,14 @@
 C.F.Wilkins & L.M.Copel.
 C.F.Wilkins & Sandiford
 C.F.Wilkins & Trudgen
 C.F.Wilkins & Whitlock
 C.F.Wilkins, Orthia & Crisp
 C.Fraser
 C.Fraser ex Graham
-C.Fraser ex Graham x Hibiscus heterophyllus Vent.
 C.Fraser ex Hook.
 C.G.Rogers
 C.H.Bernard
 C.H.Bridges & C.W.Emmons
 C.H.G.Pouchet
 C.H.Mill.
 C.H.Mill. & J.G.West
@@ -23203,17 +23516,17 @@
 C.Knight ex Müll.Arg.
 C.Knight ex Shirley
 C.Knight.
 C.L.Armstr. & Banniza
 C.L.Gross
 C.L.Gross & B.Hyland
 C.L.Gross & P.H.Weston
-C.L.Schoch & Crous
 C.L.Tso
 C.Lippert
+C.Lock, Vitelli, Holdom, Y.P.Tan & R.G.Shivas
 C.M.Chr., Papav. & C.R.Benj.
 C.M.Weiller
 C.M.Weiller & Lazarides
 C.M.Weiller & N.G.Walsh
 C.M.Weiller & Stajsic
 C.Massal.
 C.Moore
@@ -23222,32 +23535,35 @@
 C.Moore ex Benth.
 C.Moore ex F.Muell.
 C.Moore ex Maiden
 C.Moore ex Parl.
 C.Morren
 C.N.Forbes
 C.N.Page
+C.Nakash. & Crous
+C.Nakash., Videira & Crous
 C.Norman
 C.P.Robin
 C.Presl
 C.Presl ex Copel.
 C.Presl ex F.M.Bailey
 C.Presl ex M.R.Schomb.
 C.Presl ex Mett.
 C.Presl ex Rothm.
 C.Presl ex Steud.
 C.Presl ex Wettst.
 C.R.Benj.
 C.R.Carter
-C.R.Huxley & Jebb
 C.R.Marsden
 C.R.Marsden & Chinnock
 C.R.P.Andrews
 C.Ramírez
 C.Riviere
+C.Rost
+C.Rost & Thines
 C.S.P.Foster & B.J.Conn
 C.S.P.Foster & Henwood
 C.S.P.Parish
 C.S.P.Parish & Rchb.f.
 C.S.P.Parish ex Bedd.
 C.Sm. ex DC.
 C.Stuart ex Benth.
@@ -23260,59 +23576,56 @@
 C.T.White ex M.Jacobs
 C.T.White ex R.J.F.Hend.
 C.T.White ex S.T.Blake
 C.V.Morton
 C.W.Dodge
 C.W.Dodge & E.D.Rudolph
 C.W.Dodge & G.E.Baker
-C.W.Dodge & Zeller
 C.W.Schneid. & Reading
 C.W.Schneid., C.E.Lane & G.W.Saunders
 C.W.Thomson
 C.W.Thomson ex Murray
 C.Walker
-C.Walker & A.Schüßler
+C.Walker & A.Schüssler
 C.Walker & F.E.Sanders
 C.Walker & L.H.Rhodes
 C.Walter
 C.Wright
 C.Y.Wu
 C.Yen & J.L.Yang
 C.Z.Wang
 CHAH
 Cabrera
 Cabrera & Ragonese
 Cachon & Cachon-Enj.
 Cady
 Cain
 Cain & J.H.Mirza
-Cain & K.P.Jain
 Cain & Luck-Allen
-Cain, Luck-Allen & Kimbr.
 Calado & Moestrup
 Calandron ex de Hoog & Tintelnot
 Caldesi
 Calest.
 Caley ex Corda
 Caley ex D.Don
 Caley ex DC.
 Caljon
 Callm. & Buerki
 Callm., Buerki & Gallaher
 Cambage
 Cambage ex Maiden
-Cambage x Eucalyptus leptophleba F.Muell.
-Cambage x Eucalyptus melanophloia F.Muell.
 Cambess.
 Cambridge & J.Kuo
 Cameron
 Campb.
 Campd.
 Canals, Hern.-Mar., Gómez-Bolea & Llimona
 Cand. & Sulmont
+Cano, L.B.Pitarch & Guarro
+Cano, M.Solé & Guarro
 Canter
 Capdev.
 Capuron
 Cardot
 Cardot & Dixon
 Carey ex Herb.
 Cargill
@@ -23325,14 +23638,15 @@
 Carmich.
 Carmich. ex Berk.
 Carmich. ex Gomont
 Carmich. ex Harv.
 Carne
 Carnegie
 Carnegie & Beilharz
+Carnegie & G.S.Pegg
 Carnegie & Keane
 Carnegie & M.J.Wingf.
 Carnegie, Andjic & P.A.Barber
 Caro
 Carolin
 Carolin & Hewson
 Carolin & L.W.Sage
@@ -23347,44 +23661,39 @@
 Carruth.
 Carter
 Carter & Cannon
 Carty
 Carty & El.R.Cox
 Caruel
 Carus
-Casanova
 Cashmore
 Casp.
 Cass.
 Cass. ex Bercht. & J.Presl
 Cassel
 Castagne
 Castell
 Castell.
 Castellano & Beever
 Castellano & Trappe
 Castellano & Verbeken
-Castellano, Trappe & Amar.
 Castellano, Trappe & Malajczuk
-Castellano, Trappe & Malajczuk ex Kantvilas & Y.S.Chang
 Castellano, Trappe & T.Lebel
 Castellano, Trappe & Vernes
 Castl. & Carris
 Castle
 Castrac.
 Catanei
 Catches.
 Catches. & I.G.Stone
 Catches. & J.-P.Frahm
 Catches. ex J.R.Spence & H.P.Ramsay
 Catt.
 Cav.
 Cav. ex DC.
-Cav. x Banksia robur Cav.
-Cavalier & Sechier
 Cavalier & Séchier
 Cavalier-Smith
 Cavara
 Cavender, Vadell, J.C.Landolt & S.L.Stephenson
 Cavers
 Cavolini
 Cayzer & F.W.Wakef.
@@ -23392,14 +23701,16 @@
 Cedergren
 Cejp
 Celak.
 Celan
 Cels ex Link
 Cerv.
 Ces.
+Ces. & De Not.
+Ces. & De Not. ex Fuckel
 Ces. ex Rabenh.
 Chaillet ex Fr.
 Chaix
 Chalaud
 Cham.
 Cham. & Schltdl.
 Cham. & Schltdl. ex DC.
@@ -23425,18 +23736,22 @@
 Chaudhury & P.N.Rao
 Chauv.
 Chauv. ex Duby
 Cheek
 Cheel
 Cheel & C.T.White
 Cheel & M.B.Welch
-Cheel x Telopea oreades F.Muell.
 Cheeseman
 Cheesman
+Cheew. & Crous
 Cheew., M.J.Wingf. & Crous
+Cheew., Summerell & Crous
+Chen Chen, Verkley & Crous
+Chengdong Zhang & B.C.Ferrari
+Chengdong Zhang, Sirijovski, L.Adler & B.C.Ferrari
 Cherm.
 Cherm. ex Kük.
 Cherry
 Chester
 Chesters & Greenh.
 Chev.
 Chevall.
@@ -23452,14 +23767,15 @@
 Chiov.
 Chiov. & A.Vacc.
 Chippend.
 Chirgwin
 Chirgwin & K.D.Hill
 Chivers
 Chodat
+Chodat & F.Chodat
 Chodat & Hassl.
 Chodat ex Anon.
 Choisy
 Choisy ex Engl.
 Cholnoky
 Chopinet
 Christ
@@ -23467,43 +23783,39 @@
 Christ ex Maiden
 Christ ex Nakai
 Christen
 Christenh.
 Christenh. & Byng
 Christenh. & H.Schneid.
 Christenh. & M.W.Chase
-Christenh. - Blechnum rupestre (Kaulf. ex Link) Christenh.
-Christenh. x Blechnum medium (R.Br.) Christenh.
 Christm.
 Chrtek & Chrtkova
 Chrtek, Slavikova & Studnicka
 Chupov
 Churchill
 Churchill, T.B.Muir & Sinkora
 Cibot ex L.f.
 Cienk.
 Cienkowski
 Cif.
 Cif. & Ashford
 Cif. & Bat.
-Cif. & Gonz.Frag.
 Cif. & Montemart.
 Cif. & Tomas.
 Cirillo
 Cl.Roux
 Claasen
 Claassen
 Clap. & J.Lachm.
 Claridge
 Claridge, Trappe & Castellano
 Clarion ex P.Beauv.
 Clauzade & Cl.Roux ex D.Hawksw.
 Clayton
 Clayton & J.R.Harlan
-Clayton & J.R.Harlan x Cynodon nlemfuensis Vanderyst
 Clayton & Renvoize
 Cleland
 Cleland & Cheel
 Cleland & Cheel ex E.-J.Gilbert
 Cleland & E.-J.Gilbert
 Cleland & G.Cunn.
 Cleland & J.R.Harris
@@ -23543,18 +23855,16 @@
 Colden
 Colebr.
 Colebr. ex G.Don
 Coleby
 Colella ex Reveal & Doweld
 Colenso
 Colenso ex Hook.
-Colenso x Asplenium hookerianum Colenso
 Colla
 Colla ex C.Presl
-Colla x Musa balbisiana Colla
 Collad.
 Collins
 Collins & Herv.
 Colozza
 Colsm.
 Colvill
 Colvill ex Sweet
@@ -23570,35 +23880,33 @@
 Comm. ex M.Roem.
 Comm. ex Poir.
 Comm. ex R.Br.
 Comm. ex Schkuhr
 Compton
 Compère & C.E.M.Bicudo
 Connor & Edgar
-Connor & Molloy
 Conran
 Conran & Clifford
 Conran & Lowrie
 Conran & M.W.Chase
 Conran & P.I.Forst.
 Conran, P.I.Forst. & Donnon
 Const.
 Constant.
 Constant. & R.Sant.
+Constant. & Thines
 Contu
 Coode
 Cook
 Cooke
 Cooke & Balf.f.
 Cooke & Balf.f. ex Massee
 Cooke & Ellis
 Cooke & Harkn.
-Cooke & Kalchbr.
 Cooke & Massee
-Cooke & Massee ex Bailey
 Cooke & Massee ex Coker
 Cooke & Massee ex W.B.Cooke
 Cooke & Morgan
 Cooke & Peck
 Cooke & W.Phillips
 Cooke & W.R.Gerard
 Cooke & Wills
@@ -23607,27 +23915,27 @@
 Cooke ex F.M.Bailey
 Cooke ex F.Muell.
 Cooke ex G.Cunn.
 Cooke ex Massee
 Cooke ex Pilát
 Cooke ex W.Phillips
 Cookson
+Cooney & R.Emers.
 Copel.
 Copley
 Coppejans & Prud'homme
 Coppens & V.E.Barney
 Coppins
 Coppins & Aptroot
 Coppins & Fryday
 Coppins & Kantvilas
 Coppins & Purvis
 Coppins & S.Y.Kondr.
 Coppins & van den Boom
 Corda
-Corda & Berk.
 Corda ex Korshikov
 Corda ex Ralfs
 Cordem.
 Corner
 Corner & E.Horak
 Corner & Hawker
 Cornu
@@ -23656,15 +23964,14 @@
 Court ex Maslin & D.J.Murphy
 Courtois
 Couté & Preisig
 Couté & Tell
 Covas
 Cowie
 Cowie & Albr.
-Cowie & Brennan
 Cowie & G.M.Wightman
 Cowie & Guymer
 Cowie & R.A.Kerrigan
 Cowie & R.Butcher
 Cowling, G.T.Kraft & J.A.West
 Crabbe, Jermy & Mickel
 Cragin
@@ -23709,15 +24016,14 @@
 Crisp & Brooker
 Crisp & G.Chandler
 Crisp & J.M.Taylor
 Crisp & J.R.Wheeler
 Crisp & L.G.Cook
 Crisp & Mollemans
 Crisp & P.H.Weston
-Crisp x Daviesia mimosoides R.Br.
 Croasdale
 Croasdale & Flint
 Croizat
 Cromb.
 Cron
 Cronberg & B.Hickel
 Cronquist
@@ -23726,72 +24032,80 @@
 Crooks
 Croome & Fabbro
 Croome & P.A.Tyler
 Croome, Durrschm. & P.A.Tyler
 Croome, H.U.Ling & P.A.Tyler
 Croome, Hallegr.& P.A.Tyler
 Croome, Kristiansen & P.A.Tyler
-Crosby & E.J.F.Wood
 Crous
 Crous & A.D.Hocking
-Crous & Arzanlou
+Crous & Alfenas
+Crous & C.L.Schoch
 Crous & C.Mohammed
+Crous & C.Nakash.
 Crous & Carnegie
 Crous & Cheew.
 Crous & D.Victor
 Crous & Denman
+Crous & Hern.-Restr.
 Crous & J.K.Stone
 Crous & Jacq.Edwards
-Crous & Joanne E.Taylor
-Crous & L.Swart
+Crous & Jol.Roux
+Crous & K.D.Hyde
+Crous & L.Lombard
 Crous & M.E.Palm
 Crous & M.J.Wingf.
+Crous & P.A.Barber
+Crous & P.R.Johnst.
 Crous & R.G.Shivas
+Crous & Seifert
 Crous & Slippers
 Crous & Summerell
+Crous & T.I.Burgess
+Crous & Trakun.
 Crous & U.Braun
+Crous & Van Niekerk
 Crous & Verkley
+Crous & W.Gams
 Crous & de Hoog
-Crous, Arzanlou & W.Gams
-Crous, B.Sutton & C.L.Lennox
-Crous, B.Sutton, M.J.Wingf. & Marasas
-Crous, Bensch & U.Braun
-Crous, Bensch, Summerell & U.Braun
+Crous, Alfenas & M.J.Wingf.
+Crous, C.L.Lennox & B.Sutton
+Crous, H.Sm.ter & M.J.Wingf.
+Crous, Hern.-Restr. & M.E.Palm
+Crous, Hern.-Restr. & M.J.Wingf.
 Crous, I.J.Porter & Jacq.Edwards
 Crous, Jacq.Edwards & P.W.J.Taylor
 Crous, Jacq.Edwards & Pascoe
+Crous, K.Schub. & U.Braun
 Crous, M.J.Wingf. & Alfenas
-Crous, M.J.Wingf. & H.Sm.ter
-Crous, M.J.Wingf. & Slippers
 Crous, M.J.Wingf. & W.B.Kendr.
-Crous, M.J.Wingf. & W.J.Swart
+Crous, M.J.Wingf., Marasas & B.Sutton
+Crous, Montaño-Mata & García-Jim.
 Crous, Pascoe & Jacq.Edwards
 Crous, Pascoe, I.J.Porter & Jacq.Edwards
 Crous, R.G.Shivas & McTaggart
 Crous, R.G.Shivas & Summerell
 Crous, Slippers & A.J.L.Phillips
-Crous, Summerb. & L.Mostert
+Crous, Summerb. & Summerell
 Crous, Summerell & Romberg
-Crous, Summerell & Summerb.
-Crous, U.Braun & K.Schub.
-Crous, W.Gams & L.Mostert
+Crous, U.Braun & C.F.Hill
 Crowden
 Crowden & Menadue
 Croxall
 Cuatrec.
 Cuatrec. & Lourteig
 Cuccuina & Nepi
 Cuff
 Cufino
 Cummins
-Cummins & Arthur
 Cunningt.
+Cunningt., Beilharz & Pascoe
+Cunningt., R.G.Shivas & Vánky
 Cupp
 Curr.
-Curr. & Welw.
 Currah
 Curreli
 Curtis
 Curzi
 Cuvier
 Czern.
 Czerw. & Warsz.
@@ -23813,91 +24127,82 @@
 D.A.Saunders
 D.A.Sm.
 D.A.Sm. ex Tindale
 D.A.Stewart
 D.A.Sutton
 D.B.Scott & Stolk
 D.B.Scott & Van der Walt
-D.B.Scott, Van der Walt & Klift
 D.B.Ward
 D.Ballant.
 D.Beardsell & C.Beardsell
 D.C.Bhardwaj
 D.C.Eaton
 D.C.Hassall
-D.C.Linds.
 D.D.Awasthi
 D.D.Cunn.
 D.D.Sokoloff & Remizowa
 D.D.Sokoloff, I.Marques, T.D.Macfarl., Rudall & S.W.Graham
 D.D.Sokoloff, Remizowa, T.D.Macfarl. & Rudall
+D.D.de Silva, R.G.Shivas & P.W.J.Taylor
 D.Delaroche
 D.Dietr.
 D.Don
-D.Don - Bauera rubioides Andrews
 D.Don ex G.Don
 D.Don ex Hook. & Arn.
 D.E.Bradley
 D.E.Mey.
 D.E.Shaw
 D.E.Shaw & Alcorn
-D.E.Shaw & C.Booth
+D.E.Shaw & B.Sutton
 D.F.Austin & Staples
 D.F.Brunt., G.Kantvilas & M.Garrett
 D.F.Cutler & Airy Shaw
 D.G.Drury
 D.G.Griffin & W.R.Buck
 D.G.Long
 D.G.Mann
 D.G.Mann & A.J.Stickle
 D.G.Mann & E.J.Cox
 D.G.Mann & Stickle
 D.G.Müll., E.R.Parodi & A.F.Peters
 D.G.Williams
-D.H.Ashton & R.F.McCrea
 D.H.Kim
 D.H.Norris & H.Rob.
 D.H.Scott
 D.Hawksw.
 D.Hawksw. & B.Sutton
 D.Hawksw. & Dieder.
-D.Hawksw. & Dyko
 D.Hawksw. & H.Y.Yip
 D.Hawksw. & Poelt
 D.Hawksw. & Punith.
 D.Hawksw. & R.Sant.
-D.Hawksw. & S.Y.Kondr.
-D.Hawksw. & Váczi
-D.Hawksw., Coppins & Sherwood
 D.I.Morris
 D.I.Morris & Duretto
 D.J.B.Wheeler, S.W.L.Jacobs & R.D.B.Whalley
 D.J.Bedford
 D.J.Carr
 D.J.Carr & S.G.M.Carr
-D.J.Carr & S.G.M.Carr subsp. conferruminata x Eucalyptus cornuta Labill.
-D.J.Carr & S.G.M.Carr x Eucalyptus setosa Schauer
 D.J.Carr ex Schelpe
 D.J.Carr, S.G.M.Carr & B.Hyland
 D.J.Dixon
 D.J.Galloway
 D.J.Galloway & Kantvilas
 D.J.Galloway & P.James
-D.J.Galloway & P.M.Jorg.
 D.J.Galloway & P.M.Jørg.
 D.J.Galloway, Hafellner & Elix
 D.J.Hibberd
 D.J.Middleton
+D.J.Midgley & Tran-Dinh
 D.J.Ohlsen
 D.J.Ohlsen, Perrie, E.L.May & Bayly
 D.J.Read
 D.J.S.Barr
 D.J.S.Barr, K.J.Cheng, H.Kudo & Jakober
-D.J.S.Barr, Longcore & Désauln.
 D.J.Sullivan, Western., K.A.Haynes, Dés.E.Benn. & D.C.Coleman
+D.Johnson, G.H.Sung, Hywel-Jones & Spatafora
 D.König
 D.L.Anderson & N.L.Gibson
 D.L.Jones
 D.L.Jones & B.Gray
 D.L.Jones & Bostock
 D.L.Jones & C.J.French
 D.L.Jones & D.P.Banks
@@ -23909,24 +24214,16 @@
 D.L.Jones & L.M.Copel.
 D.L.Jones & Lavarack
 D.L.Jones & M.A.Clem.
 D.L.Jones & P.I.Forst.
 D.L.Jones & R.C.Nash
 D.L.Jones & R.J.Bates
 D.L.Jones & T.B.Muir
-D.L.Jones - Macrozamia pauli-guilielmi W.Hill & F.Muell.
 D.L.Jones ex Jeanes
 D.L.Jones ex M.T.Mathieson
-D.L.Jones x Diuris orientis D.L.Jones
-D.L.Jones x Diuris palustris Lindl.
-D.L.Jones x Diuris pardina Lindl.
-D.L.Jones x Diuris semilunulata Messmer
-D.L.Jones x Diuris sulphurea R.Br.
-D.L.Jones x Macrozamia moorei F.Muell.
-D.L.Jones x Macrozamia pauli-guilielmi W.Hill & F.Muell.
 D.L.Jones, B.Gray & M.A.Clem.
 D.L.Jones, B.Gray, M.A.Clem. & J.J.Wood
 D.L.Jones, C.J.French & M.A.Clem.
 D.L.Jones, M.A.Clem. & D.P.Banks
 D.L.Jones, M.A.Clem. & I.K.Sharma
 D.L.Jones, M.A.Clem. & Molloy
 D.L.Jones, M.A.Clem., I.K.Sharma, A.M.Mack. & Molloy
@@ -23934,99 +24231,78 @@
 D.L.Schulz
 D.Legrand
 D.Löve & Á.Löve
 D.M.Britton & D.F.Brunt.
 D.M.Crayn, E.A.Br. & J.M.Powell
 D.M.Macedo, O.L.Pereira & R.W.Barreto
 D.M.Moore
+D.M.Robinson, M.H.Laurence, E.C.Y.Liew & Summerell
 D.M.Williams & Round
 D.Mohr
 D.Mohr & F.Weber
 D.Morris
 D.Mull.-Doblies & U.Mull.-Doblies
 D.Nicolle
 D.Nicolle & Brooker
-D.Nicolle & Brooker - Eucalyptus suggrandis subsp. promiscua D.Nicolle & Brooker
-D.Nicolle & Brooker - Eucalyptus vegrandis L.A.S.Johnson & K.D.Hill
-D.Nicolle & Brooker x Eucalyptus suggrandis L.A.S.Johnson & K.D.Hill
-D.Nicolle & Brooker x Eucalyptus vegrandis L.A.S.Johnson & K.D.Hill
-D.Nicolle & Brooker x Eucalyptus wandoo Blakely
-D.Nicolle & Brooker x Eucalyptus xanthonema Turcz.
 D.Nicolle & Kleinig
 D.Nicolle & L.A.S.Johnson
 D.Nicolle & M.E.French
-D.Nicolle & M.E.French - Eucalyptus olivina Brooker & Hopper
-D.Nicolle & M.E.French - Eucalyptus rigidula subsp. interior D.Nicolle & M.E.French
-D.Nicolle & M.E.French x Eucalyptus incrassata Labill.
-D.Nicolle & M.E.French x Eucalyptus loxophleba Benth.
-D.Nicolle & M.E.French x Eucalyptus megacornuta C.A.Gardner
-D.Nicolle & M.E.French x Eucalyptus orthostemon D.Nicolle & Brooker
-D.Nicolle & M.E.French x Eucalyptus salubris F.Muell.
-D.Nicolle & M.E.French x Eucalyptus sporadica Brooker & Hopper
-D.Nicolle & M.E.French x Eucalyptus tenera L.A.S.Johnson & K.D.Hill
-D.Nicolle & M.E.French x Eucalyptus tetraptera Turcz.
-D.Nicolle & M.E.French x Eucalyptus victrix L.A.S.Johnson & K.D.Hill
 D.Nicolle & R.L.Barrett
-D.Nicolle - Eucalyptus distuberosa D.Nicolle
-D.Nicolle - Eucalyptus kondininensis Maiden & Blakely
-D.Nicolle - Eucalyptus spreta L.A.S.Johnson & K.D.Hill
-D.Nicolle subsp. canescens x Eucalyptus vokesensis D.Nicolle & L.A.S.Johnson
-D.Nicolle subsp. distuberosa - Eucalyptus tenuis Brooker & Hopper
 D.Nicolle, B.M.Potts & McKinnon
 D.Nicolle, M.E.French & McQuoid
 D.O.Cross & Vickery
 D.P.Banks
 D.P.Cheney
 D.P.Rogers
 D.P.Thomas
 D.Parodi
+D.Q.Dai & K.D.Hyde
 D.Quandt, N.E.Bell & Stech
 D.R.Norris, Bomber & Balech
 D.R.Reynolds
 D.R.Reynolds & G.S.Gilbert
 D.R.Simmons
 D.Rao & P.Rag.Rao
 D.Ratkowsky & A.Ratkowsky
 D.Royen
 D.Royen ex L.
 D.S.Mitch.
 D.Stubbe & Verbeken
+D.W. Li
 D.W.Mitch.
 D.W.Stev.
 D.Wall
 D.Y.Hong
 DC.
-DC. & F.Desp.
 DC. & Spreng.
-DC. - Eriostemon scaber subsp. latifolius Paul G.Wilson
 DC. ex A.DC.
 DC. ex Bercht. & J.Presl
 DC. ex Collad.
 DC. ex Decne.
 DC. ex Dunal
 DC. ex F.Rudolphi
 DC. ex Gomont
 DC. ex Gray
 DC. ex Hook.
 DC. ex Koch
 DC. ex P.Beauv.
 DC. ex Perleb
 DC. ex Schnizl.
 DC. ex Sweet
-DC. subsp. aspera x Hibbertia empetrifolia (DC.) Hoogland
-DC. x Acacia sclerosperma F.Muell.
-DC. x Acacia verniciflua A.Cunn.
 Daday
 Dade
 Dahlst.
 Dalla Torre & Harms
 Dallim. & A.B.Jacks.
 Dalman
 Dalzell
 Dalzell ex C.B.Clarke
+Damm & P.F.Cannon
+Damm, P.F.Cannon & Crous
+Damm, P.F.Cannon, Crous, P.R.Johnst. & B.S.Weir
 Dammer
 Dandy
 Daniker
 Danks, T.Lebel & Vernes
 Danquah
 Danser
 Danthoine ex Lam. & DC.
@@ -24038,66 +24314,62 @@
 Dasz.
 Daveau
 Davoodian
 Davoodian & Halling
 Davoodian, Bougher & Halling
 Davoodian, Bougher, N.A.Fechner & Halling
 Davoodian, N.A.Fechner & Halling
+Dayar., Fryar & K.D.Hyde
 De Clerck & Coppejans
 De Cock & Man in 't Veld
 De Cock, L.Mend., A.A.Padhye, Ajello & Kaufman
 De Nardi
 De Nardi ex B.K.Simon
 De Not.
-De Not. & Ces.
-De Not. & Ces. ex Fuckel
 De Not. ex Rabenh.
 De Seynes
 De Stefano & D.Marino
 De Toni
 De Toni & Levi
 De Toni & Levi-Morenos
 De Wild.
 De Winter
 DeBuhr
+Dearnaley, Hidmi & C.C.Linde
+Dearnaley, T.W.May & C.C.Linde
 Deason
 Deason & Ed.R.Cox
 Deb
 Debbert
 Deby
 Decne.
 Decne. & Planch.
-Decne. ex Endl.
 Decne. ex Harv.
 Decne. ex Kütz.
 Decne. ex Miq.
 Decne. ex Müll.Arg.
 Dedecek
 Deflandre
 Degel.
 Dehnh.
 Dehnh. ex Miq.
-Dehnh. x Eucalyptus amygdalina Labill.
-Dehnh. x Eucalyptus exserta F.Muell.
-Dehnh. x Eucalyptus platyphylla F.Muell.
-Dehnh. x Eucalyptus tereticornis Sm.
 Deighton
 Delile
 Delile ex DC.
 Delile ex De Seynes
 Delise
-Delise ex Duby
 Delise ex Nyl.
 Delitsch
 Dell
 Dellow
 Delponte
 Delépine & Asensi
-Dema & I.Telford
+Denchev
 Denizot
+Denman & Crous
 Dennis
 Dennst.
 Dennst. ex Endl.
 Dennst. ex Sleumer
 Derbes & Solier
 Derbès & Solier
 Derera
@@ -24109,15 +24381,14 @@
 Desf. ex J.F.Gmel.
 Desf. ex Juss.
 Desf. ex Lehm.
 Desf. ex Link
 Desf. ex Paxton
 Desf. ex Pers.
 Desf. ex Poir.
-Desf. ex Poir. x Senecio hispidulus A.Rich.
 Desf. ex Redouté
 Desf. ex Vent.
 Desikachary
 Desm.
 Desm. ex Bornet & Flahault
 Desm. ex Gomont
 Despr. ex Nyl.
@@ -24138,32 +24409,30 @@
 Diddens & Lodder
 Died.
 Dieder.
 Diederich
 Diederich & Etayo
 Diederich & Lawrey
 Diederich, Aptroot & Sérus.
-Diederich, Ertz, U.Braun & Heuchert
-Diederich, Lawrey & Van den Broeck
 Diederich, Sérus. & Aptroot
-Diederich, U.Braun & Heuchert
 Diehl & E.B.Lamb.
 Diels
 Diels & E.Pritz.
 Diels & E.Pritz. ex De Wild.
 Diels & Loes.
 Diels & O.Schwarz ex O.Schwarz
 Diels ex Blakely
 Diels ex Reveal
-Diels x Kunzea preissiana Schauer
 Dierckx
+Dierickx & De Crop
 Diesing
 Diesing ex Endl.
 Diesing ex Schauer
 Dietel
+Dietel & Ellis
 Dietel & Holw.
 Dill. ex Fr.
 Dill. ex Pers.
 Dillwyn
 Diment, Humphries, Newington & Shaugnessy
 Dimon & M.A.M.Renner
 Ding Hou
@@ -24179,37 +24448,28 @@
 Dixon & Watts
 Dixon ex H.P.Ramsay
 Dixon ex H.P.Ramsay & J.Seur
 Dixon ex H.P.Ramsay, W.B.Schofield & B.C.Tan
 Dixon ex Malta
 Dixon ex Sainsbury
 Dixon, R.A.Kerrigan & Cowie
+Dixon-Stew.
 Dockrill
 Dockrill & St.Cloud
 Dode
 Dogiel
 Dogma
 Doidge
 Domański
 Dombey ex A.Juss.
 Dombey ex Lam.
 Dombrain
 Domin
-Domin - Persoonia media R.Br.
-Domin - Persoonia stradbrokensis Domin
-Domin - Persoonia tenuifolia R.Br.
-Domin - Persoonia virgata R.Br.
 Domin ex F.M.Bailey
 Domin ex Velen.
-Domin x Eucalyptus obesa Brooker & Hopper
-Domin x Eucalyptus pruinosa Schauer
-Domin x Iseilema vaginiflorum Domin
-Domin x Persoonia tenuifolia R.Br.
-Domin x Persoonia virgata R.Br.
-Domin x Zieria smithii Andrews
 Domke
 Don
 Donadini & G.Riousset
 Donat & Ruttner
 Donati
 Donk
 Donkin
@@ -24217,28 +24477,29 @@
 Donn ex Andrews
 Donn ex F.Dietr.
 Donn ex Haw.
 Donn ex Ker Gawl.
 Donn ex Sm.
 Donn ex Willd.
 Donn.Sm.
-Dorfelt
 Dorogin
 Dorr.Sm.
 Doty
 Doty & B.C.Stone
 Doty & Meñez
 Doty ex P.C.Silva
+Douch, L.Tegart, L.J.Vaughan & T.Lebel
 Douglas
 Douglas ex D.Don
 Douglas ex Hook.
 Douglas ex Lehm.
 Douglas ex Lindl.
 Douglas ex Loudon
 Douin
+Doungsa-ard, McTaggart, Geering & R.G.Shivas
 Doust & B.J.Conn
 Dovaston
 Dowding
 Dowe
 Dowe & A.K.Irvine
 Dowe & Barfod
 Dowe & D.L.Jones
@@ -24251,15 +24512,14 @@
 Dozy & Molk.
 Dragesco
 Drake
 Drap. ex DC.
 Drayton
 Drebes & D.Schulz
 Drechsler
-Drechsler, Meier & E.D.Eddy
 Drege
 Drejer
 Drezep.
 Drezepolski
 Dring
 Druce
 Drude
@@ -24310,14 +24570,15 @@
 Duretto & Heslewood
 Duretto & K.L.Durham
 Duretto & P.I.Forst.
 Duretto & P.R.Alvarez
 Duretto, F.J.Edwards & P.G.Edwards
 Durie & Frey
 Durieu
+Durieu & Mont.
 Durán & G.W.Fisch.
 Dusén
 Duthie
 Duval
 Duval-Jouve
 Duvau
 Duyfjes
@@ -24325,40 +24586,44 @@
 Dyko & D.Hawksw.
 Döbbeler
 Döbbeler & Poelt
 Döbbeler & Triebel
 Döll
 Dörfelt
 Dürrschm.
+D’souza, Boonmee, Bhat & K.D.Hyde
 E.'t Hart
 E.-J.Gilbert
+E.-J.Gilbert & Cleland
 E.A.Br.
 E.A.Br. & M.A.M.Renner
 E.A.Br. & N.Streiber
 E.A.Br. & Pócs
 E.A.Flint
 E.A.Flint & H.Ettl
 E.A.Hodgs.
 E.A.Hodgs. & Allison
 E.A.Hodgs. & Herzog
 E.A.Shaw
+E.Azevedo, P.Correia & M.F.Caeiro
 E.B.Alexeev
 E.B.Bartram
 E.B.Bartram & Dixon
 E.B.Bartram ex Dixon
-E.B.G.Jones & Abdel-Wahab
 E.B.G.Jones & Camp.-Als.
-E.B.G.Jones & K.L.Pang
+E.B.G.Jones & K.D.Hyde
 E.B.G.Jones & R.A.Eaton
-E.B.G.Jones, S.T.Moss & R.G.Johnson
+E.B.G.Jones, R.G.Johnson & S.T.Moss
+E.B.Knox
 E.Beer & H.J.Lam
 E.Bodin ex Guég.
 E.C.Berry
 E.C.Hall
 E.C.Hansen
+E.C.Keirnan, M.H.Laurence, R.G.Shivas & Y.P.Tan
 E.C.McDonald
 E.C.Nelson
 E.C.Nelson & D.J.Bedford
 E.Coleman
 E.D.Br.
 E.D.Clarke
 E.D.Cooper
@@ -24374,96 +24639,95 @@
 E.G.Jørg.
 E.G.Pringsh.
 E.G.Simmons
 E.G.Simmons & Alcorn
 E.G.Simmons & C.F.Hill
 E.G.Simmons, Alcorn & C.F.Hill
 E.Guého & M.T.Sm.
+E.H.Giglioli
 E.H.Lombard & Capon
 E.H.Wilson ex A.Grove
 E.Horak
 E.Horak & Desjardin
 E.Horak & G.M.Taylor
 E.Horak & M.M.Moser
-E.Horak & O.K.Mill.
 E.Horak, Peintner, M.M.Moser & Vilgalys
 E.Hübner
 E.J.Butler
-E.J.Butler, Syd. & P.Syd.
 E.J.Cox
 E.J.Durand
 E.J.Durand ex Thaxt.
 E.J.F.Wood
-E.J.Gilbert
-E.J.Gilbert & Cleland
 E.J.Hickman & Hopper
 E.J.Lowe
 E.J.Schmidt
 E.J.Thomps.
 E.J.Thomps. & B.K.Simon
 E.Jahn
 E.K.Cash & A.M.J.Watson
 E.L.Robertson
 E.L.Stewart & Trappe
 E.Liebet.
 E.M.Benn.
 E.M.Benn. & K.A.Sheph.
 E.M.Davison
+E.M.Davison & Giustiniano
+E.M.Davison & R.G.Shivas
+E.M.Davison, Giustiniano & Bougher
+E.M.Davison, Giustiniano, McGurk & E.L.J.Watkin
 E.M.Davison, P.J.N.Davison, M.D.Barrett & R.L.Barrett
 E.M.Johnson & Valleau
 E.M.Ross
-E.M.Ross x Macarthuria neocambrica F.Muell.
 E.M.Watson
 E.M.Woll.
 E.M.Woll. & Womersley
 E.Mackinnon
 E.Martinez & Ramos
 E.Mey.
 E.Mey. ex Arn.
 E.Mey. ex Bartl. & H.L.Wendl.
-E.Mey. ex Benth.
 E.Mey. ex DC.
 E.Mey. ex Drege
 E.Mey. ex Fenzl
 E.Mey. ex Harv. & Sond.
 E.Mey. ex Kunth
 E.Mey. ex Naudin
 E.Mey. ex Sond.
 E.Miege
 E.Murray
 E.Müll.
-E.Müll., Samuels & Petrini
 E.Nielsen
 E.Otto
 E.P.Bicknell
 E.Phillips
 E.Post
 E.Pritz.
 E.Pritz. ex Hemsl.
-E.Pritz. x Acacia tumida var. pilbarensis M.W.McDonald
 E.R.Farr, Leussink & Stafleu
 E.R.L.Johnson
 E.Reichardt
 E.S.Barton
 E.S.Salmon & Stolk
 E.Takah.
 E.Thurst.
+E.Thynne, M.C.McDonald, M.Evans, Wallwork, S.M.Neate & P.S.Solomon
 E.V.Abbott
 E.W.Cooper
 E.W.Cross
 E.W.Cross & Orchard
+E.W.Mason & M.B.Ellis
 E.Walker
 E.Wimm.
 E.Y.Dawson
 E.Y.Haw.
 E.Y.Haw. & P.A.Tyler
 E.Young
+E.Yuill
 Eardley
 Earle
-Earle & Tracy
 Eastw.
 Eaton
 Eckblad
 Eckl.
 Eckl. & Zeyh.
 Eckl. ex C.H.Wright
 Eckl. ex Klatt
@@ -24471,20 +24735,23 @@
 Edees & A.Newton
 Edgar
 Edgar & A.P.Druce
 Edgar & Molloy
 Edgew.
 Edginton
 Edginton & E.J.Thomps.
+Edginton, Al-Shehbaz & Lysak
 Edson
 Edward
 Edyvane
 Edyvane & Womersley
 Egea & Torrente
+Eggertson & Lévesque
 Eggli & Nyffeler
+Egunyomi & Olar.
 Ehrenb.
 Ehrenb. & Hempr. ex Asch. & Schweinf.
 Ehrenb. & Hemprich ex Ralfs
 Ehrenb. ex Asch.
 Ehrenb. ex Cleve
 Ehrenb. ex Fr.
 Ehrenb. ex Gomont
@@ -24541,17 +24808,16 @@
 Elix, Louwhoff & M.Molina
 Elix, O.Blanco & A.Crespo
 Elix, S.Y.Kondr. & Kärnefelt
 Eliz.George & A.S.George
 Elkan
 Elliott
 Ellis & Barthol.
-Ellis & Dietel
 Ellis & Everh.
-Ellis & Everh. ex H.S.Jacks. & D.P.Rogers
+Ellis & Everh. ex D.P.Rogers & H.S.Jacks.
 Ellis & G.Martin
 Ellis & Galloway
 Ellis & Halst.
 Ellis & Holw.
 Ellis & Kellerm.
 Ellis & Langl.
 Ellis & N.Pierce
@@ -24574,35 +24840,29 @@
 Endl. & Lehm.
 Endl. ex Meisn.
 Endl. ex Mildbr.
 Endl. ex Miq.
 Endl. ex Schnizl.
 Endl. ex Steud.
 Endl. ex Walp.
-Endl. x Eucalyptus dorrienii Domin
-Endl. x Eucalyptus ecostata (Maiden) D.Nicolle & M.E.French
-Endl. x Eucalyptus lane-poolei Maiden
-Endl. x Eucalyptus petrensis Brooker & Hopper
-Endl. x Eucalyptus virginea Hopper & Ward.-Johnson
-Endl. x Tribonanthes brachypetala Lindl.
-Endl. x Tribonanthes longipetala Lindl.
 Engelm.
 Engelm. & A.Gray
 Engelm. & J.M.Bigelow
 Engelm. ex A.Berger
 Engelm. ex Boiss.
 Engelm. ex Hegelm.
 Engelm. ex J.G.Sm.
 Engl.
 Engl. & Gilg
 Engl. & K.Krause
 Engl. & Warb.
 Engl. ex D.Legrand
 Enroth
 Enroth & S.He
+Enroth, Huttunen, Tangney, M.Stech & D.Quandt
 Entwisle
 Entwisle & Foard
 Entwisle & S.Skinner
 Entwisle & Vis
 Entz
 Er.Köhler
 Er.Lindem.
@@ -24613,14 +24873,15 @@
 Ertz, Diederich, Christnach & Wedin
 Eschsch.
 Eschw.
 Esper
 Espinosa
 Essig
 Essl.
+Esteve-Rav. & Matheny
 Etayo & Breuss
 Etchells & T.A.Bell
 Ettingsh.
 Everist
 Everist ex R.J.F.Hend.
 Ew.Gerhardt
 Ewart
@@ -24658,147 +24919,133 @@
 F.C.Quinn
 F.C.Quinn ex Craven
 F.Cels
 F.Cels ex Jacques
 F.D.Wilson
 F.D.Wilson & Byrnes
 F.Delaroche
+F.Desp. & DC.
 F.Dietr.
 F.Ducell.
 F.E.Briggs ex Mulligan
 F.E.Burbury
 F.E.Drouet
 F.E.Drouet & J.C.Strickland
 F.E.Drouet & W.A.Daily
 F.E.Fritsch
 F.E.Fritsch & M.F.Rich
 F.E.Fritsch & R.P.John
+F.E.Guard
 F.E.Guard, M.D.Barrett & Farid
+F.E.Guard, McMull.-Fish., J.van Wyk, T.Lebel, & Halling
+F.E.Guard, T.Lebel & Dearnaley
 F.E.Havil.
 F.E.Lloyd
 F.Fricke
 F.G.Davies
 F.Gay
+F.Gómez
 F.Gómez & Artigas
 F.Gómez, D.Moreira & P.López-Garcia
 F.H.Møller
 F.H.Wigg.
 F.Henkel
 F.Herm.
 F.J.Herm.
+F.J.Jiménez & M.Talavera
 F.J.MacEntee, H.C.Bold & P.A.Archibald
 F.J.R.Taylor
 F.J.Walker & Hafellner
 F.L.Bauer ex Benth.
 F.L.Erickson
 F.L.Erickson & J.H.Willis
 F.L.Tai
+F.Lara, Garilleti & Goffinet
+F.Liu, L.Cai & Crous
 F.Ludw.
 F.M.Anderson
 F.M.Bailey
 F.M.Bailey & F.Muell.
-F.M.Bailey & F.Muell. ex F.M.Bailey
 F.M.Bailey & Tenison-Woods
 F.M.Bailey ex B.K.Simon
-F.M.Bailey x Acacia monticola J.M.Black
-F.M.Bailey x Dendrobium racemosum (Nicholls) Clemesha & Dockrill
 F.M.Forbes
 F.M.Jarrett
 F.M.Knuth
 F.M.Leight.
 F.Meehan & H.C.Murphy
 F.Meister
 F.Muell.
 F.Muell. & A.Benn.
 F.Muell. & Baker
 F.Muell. & Behr
-F.Muell. & Behr ex F.Muell.
 F.Muell. & C.Stuart ex Meisn.
 F.Muell. & F.M.Bailey
-F.Muell. & F.M.Bailey ex F.M.Bailey
 F.Muell. & Fitzg.
 F.Muell. & Harv.
-F.Muell. & Harv. ex Harv.
 F.Muell. & Holtze
 F.Muell. & J.E.Br.
 F.Muell. & Kalchbr.
 F.Muell. & Kraenzl.
-F.Muell. & Kraenzl. ex Kraenzl.
 F.Muell. & Maiden
 F.Muell. & Miq.
 F.Muell. & O'Shanesy
 F.Muell. & Rodway
 F.Muell. & Scort.
 F.Muell. & Scort. ex Scort.
 F.Muell. & Sond.
-F.Muell. & Sond. ex Sond.
 F.Muell. & Tate
 F.Muell. & Tate ex Ewart
 F.Muell. & Tate ex Ewart & Cookson
 F.Muell. & Tate ex Ewart & Jean White
 F.Muell. & Tate ex J.M.Black
-F.Muell. & Tate ex Tate
-F.Muell. - Eucalyptus odontocarpa F.Muell.
-F.Muell. - Eucalyptus tectifica F.Muell.
-F.Muell. - Eucalyptus whitei Maiden & Blakely
+F.Muell. & Thüm.
 F.Muell. ex A.Braun
 F.Muell. ex A.E.Holland & S.T.Reynolds
 F.Muell. ex A.Gray
 F.Muell. ex A.S.Mitch.
 F.Muell. ex A.T.Lee
 F.Muell. ex Airy Shaw
 F.Muell. ex Baill.
 F.Muell. ex Becc.
 F.Muell. ex Belcher
 F.Muell. ex Benth.
-F.Muell. ex Benth. x Acacia paraneura Randell
-F.Muell. ex Benth. x Eucalyptus melanophloia F.Muell.
-F.Muell. ex Benth. x Eucalyptus populnea F.Muell.
-F.Muell. ex Benth. x Eucalyptus shirleyi Maiden
-F.Muell. ex Benth. x Eucalyptus sinuosa D.Nicolle, M.E.French & McQuoid
-F.Muell. ex Benth. x Lepyrodia cryptica B.G.Briggs & L.A.S.Johnson
-F.Muell. ex Benth. x Lepyrodia oligocolea B.G.Briggs & L.A.S.Johnson
-F.Muell. ex Benth. x Lepyrodia scariosa R.Br.
 F.Muell. ex Berk.
 F.Muell. ex Blakely
 F.Muell. ex Boeckeler
 F.Muell. ex Boiss.
 F.Muell. ex Bremek.
 F.Muell. ex Burtt Davy
 F.Muell. ex C.B.Clarke
 F.Muell. ex C.Moore
 F.Muell. ex C.T.White
 F.Muell. ex Cogn.
+F.Muell. ex Cooke
 F.Muell. ex Corner
 F.Muell. ex Craven
 F.Muell. ex D.Dietr.
 F.Muell. ex De Toni
 F.Muell. ex Diels
 F.Muell. ex Diels & E.Pritz.
 F.Muell. ex Domin
 F.Muell. ex Drude
 F.Muell. ex E.Pritz.
 F.Muell. ex Ewart
 F.Muell. ex Ewart & B.Rees
-F.Muell. ex Ewart & Jean White
 F.Muell. ex Ewart & O.B.Davies
 F.Muell. ex Ewart & Sharman
 F.Muell. ex Ewart, Jean White & B.Rees
-F.Muell. ex Ewart, Jean White & B.Wood
 F.Muell. ex F.L.Erickson & J.H.Willis
 F.Muell. ex F.M.Bailey
-F.Muell. ex F.M.Bailey x Astrebla lappacea (Lindl.) Domin
 F.Muell. ex Fitzg.
 F.Muell. ex French
 F.Muell. ex G.Taylor
 F.Muell. ex H.B.Will.
 F.Muell. ex H.Walter
 F.Muell. ex H.Wendl. & Drude
 F.Muell. ex Hallier f.
-F.Muell. ex Hampe
 F.Muell. ex Hannaford
 F.Muell. ex Harv.
 F.Muell. ex Hazlewood
 F.Muell. ex Hiern
 F.Muell. ex Hieron.
 F.Muell. ex Hochr.
 F.Muell. ex Hollós
@@ -24817,14 +25064,15 @@
 F.Muell. ex Kurz
 F.Muell. ex Kütz.
 F.Muell. ex L.A.S.Johnson
 F.Muell. ex Lange
 F.Muell. ex Luerss.
 F.Muell. ex Maiden
 F.Muell. ex Maiden & Betche
+F.Muell. ex Massee
 F.Muell. ex McGill.
 F.Muell. ex Meisn.
 F.Muell. ex Miq.
 F.Muell. ex Mitt.
 F.Muell. ex Müll.Arg.
 F.Muell. ex N.A.Wakef.
 F.Muell. ex N.Snow & Guymer
@@ -24851,88 +25099,37 @@
 F.Muell. ex Tod.
 F.Muell. ex Triana
 F.Muell. ex Vesque
 F.Muell. ex W.Archer
 F.Muell. ex W.Fitzg.
 F.Muell. ex Watts & Whitel.
 F.Muell. ex Wettst.
-F.Muell. subsp. bowmanii - Eremophila bowmanii subsp. nutans Chinnock
-F.Muell. subsp. bowmanii x Eremophila latrobei F.Muell.
-F.Muell. subsp. fibrosa x Eucalyptus moluccana Roxb.
-F.Muell. subsp. sclerosperma x Acacia sclerosperma subsp. glaucescens A.R.Chapm. & Maslin
-F.Muell. x Acacia dealbata A.Cunn.
-F.Muell. x Acacia decurrens Willd.
-F.Muell. x Acacia leucoclada Tindale
-F.Muell. x Acacia monticola J.M.Black
-F.Muell. x Caladenia pulchra Hopper & A.P.Br.
-F.Muell. x Callitris preissii subsp. verrucosa (A.Cunn. ex Endl.) J.Garden
-F.Muell. x Callitris verrucosa (A.Cunn. ex Endl.) F.Muell.
-F.Muell. x Correa reflexa (Labill.) Vent.
-F.Muell. x Dendrobium jonesii Rendle
-F.Muell. x Dendrobium pugioniforme A.Cunn.
-F.Muell. x Dendrobium schoeninum Lindl.
-F.Muell. x Dendrobium speciosum Sm.
-F.Muell. x Dendrobium speciosum var. grandiflorum F.M.Bailey
-F.Muell. x Dendrobium tenuissimum Rupp
-F.Muell. x Dodonaea viscosa Jacq.
-F.Muell. x Eremophila latrobei F.Muell.
-F.Muell. x Eucalyptus amygdalina Labill.
-F.Muell. x Eucalyptus decorticans (F.M.Bailey) Maiden
-F.Muell. x Eucalyptus fibrosa F.Muell.
-F.Muell. x Eucalyptus fibrosa subsp. nubilis (Maiden & Blakely) L.A.S.Johnson
-F.Muell. x Eucalyptus leptophleba F.Muell.
-F.Muell. x Eucalyptus leucophylla Domin
-F.Muell. x Eucalyptus marginata Donn ex Sm.
-F.Muell. x Eucalyptus melanophloia F.Muell.
-F.Muell. x Eucalyptus melliodora A.Cunn. ex Schauer
-F.Muell. x Eucalyptus microcarpa (Maiden) Maiden
-F.Muell. x Eucalyptus microtheca F.Muell.
-F.Muell. x Eucalyptus moluccana Roxb.
-F.Muell. x Eucalyptus normantonensis Maiden & Cambage
-F.Muell. x Eucalyptus obliqua L'Hér.
-F.Muell. x Eucalyptus obstans L.A.S.Johnson & K.D.Hill
-F.Muell. x Eucalyptus odontocarpa F.Muell.
-F.Muell. x Eucalyptus orgadophila Maiden & Blakely
-F.Muell. x Eucalyptus peninsularis D.Nicolle
-F.Muell. x Eucalyptus persistens L.A.S.Johnson & K.D.Hill
-F.Muell. x Eucalyptus platyphylla F.Muell.
-F.Muell. x Eucalyptus populnea F.Muell.
-F.Muell. x Eucalyptus portuensis K.D.Hill
-F.Muell. x Eucalyptus pruinosa Schauer
-F.Muell. x Eucalyptus shirleyi Maiden
-F.Muell. x Eucalyptus siderophloia Benth.
-F.Muell. x Eucalyptus tereticornis Sm.
-F.Muell. x Eucalyptus thozetiana (F.Muell. ex Maiden) R.T.Baker
-F.Muell. x Eucalyptus whitei Maiden & Blakely
-F.Muell. x Eucalyptus xanthoclada Brooker & A.R.Bean
-F.Muell. x Gossypium nelsonii Fryxell
-F.Muell. x Gossypium sturtianum J.H.Willis
-F.Muell. x Leptospermum microcarpum Cheel
-F.Muell. x Rubus parvifolius L.
 F.N.Williams
 F.Patt.
 F.Petit
 F.R.Jones bis
 F.Rudolphi
 F.Schill.
 F.Schmidt
 F.Schmitz
 F.Schmitz & Falkenb.
 F.Schmitz ex Batters
 F.Schmitz ex Falkenb.
 F.Schmitz ex Mazza
 F.Schütt
 F.Schütt ex De Toni
+F.Sklenář, S.W.Peterson & Hubka
 F.Stein
-F.Stein ex Jörg.
+F.Stein ex Jørg.
 F.Stevens
 F.Stevens & Dalbey
 F.Stevens & E.Young
 F.Stevens & Manter
 F.Stevens & Tehon
+F.Sulman
 F.T.Benn.
 F.T.Hubb.
 F.Turner
 F.Voigt
 F.W.Lewis
 F.W.Schmidt
 F.W.Schultz
@@ -24940,14 +25137,15 @@
 F.W.Wakef.
 F.Weber
 F.Weber & D.Mohr
 F.Wilson
 F.Wilson ex A.W.Archer
 F.Wilson ex Filson
 F.Wilson ex H.Magn.
+F.Y.Bai & Q.M.Wang
 F.Šmarda
 Fabr.
 Fabre
 Fabre-Dom.
 Faden
 Fagundez & Izco
 Fahey & Fensham
@@ -24958,34 +25156,33 @@
 Farkas & Vězda
 Farl.
 Farl. & Burt
 Farl. ex Gomont
 Farl. ex Murrill
 Farmar
 Farw.
-Faurel & Schotter
 Fauré-Frem.
 Fautrey
 Fautrey & Lambotte
 Fautrey & Roum.
 Fawc.
 Fay
 Fayod
 Febiger ex Cleve & Jos.D.Möller
 Fedde
+Fedosov, M.Stech & Ignatov
 Feinbrun
 Feldm.-Maz.
 Feldmann
 Feldmann & Hamel
 Fennell & Raper
 Fenzl
 Fenzl ex Endl.
 Fenzl ex Harv.
 Ferd. & Winge
-Fern.-Brime, Gaya, Llimona
 Fern.-Vill.
 Fernald
 Ferraris
 Ferrington, Hayford & Lichtw.
 Fiasson & Niemelä
 Ficinus & C.Schub.
 Fiddian
@@ -25007,28 +25204,21 @@
 Fisch. ex DC.
 Fisch. ex Fisch. & C.A.Mey.
 Fisch. ex Gaudich.
 Fisch. ex Koehne
 Fisch. ex Steud.
 Fitzg.
 Fitzg. ex Nicholls
-Fitzg. x Dendrobium gracilicaule F.Muell.
-Fitzg. x Dendrobium kingianum Bidwill ex Lindl.
-Fitzg. x Dendrobium speciosum Sm.
-Fitzg. x Pterostylis nutans R.Br.
 Fitzh.
 Fitzp.
-Flakus & Lucking
 Flakus & Lücking
 Flann
 Flicker
 Flint
 Florin
-Florke
-Florke ex Sommerf.
 Flot.
 Flot. & Körb. ex A.Massal.
 Flot. ex Nyl.
 Flörke
 Flüggé
 Focke
 Focke ex Nordst.
@@ -25056,21 +25246,19 @@
 Foslie & M.Howe
 Fott
 Foug.
 Fourr.
 Foust
 Fr.
 Fr. & Hök
-Fr. & Nordholm
 Fr. : Fr.
 Fr. ex Berk.
 Fr. ex Bonord.
 Fr. ex Klotzsch
 Fr. ex P.Karst.
-Frances, Sigler & C.Panter
 Francey
 Franch.
 Franch. & Rochebr. ex Crep.
 Franch. & Sav.
 Franco
 Franco & P.C.Silva
 Franco & Vasc.
@@ -25089,14 +25277,17 @@
 Fritsch
 Frodin
 Frodin ex B.Hyland & A.G.Floyd
 Frohne & U.Jensen ex Reveal
 From.
 Frood
 Frost
+Fryar & D.E.A.Catches.
+Fryar & K.D.Hyde
+Fryar, D.E.A.Catches. & Réblová
 Fryar, Haelew. & D.E.A.Catches.
 Fryday
 Fryday & A.Knight
 Fryday & Kantvilas
 Fryday, Printzen & S.Ekman
 Fryxell
 Fryxell & Craven
@@ -25112,73 +25303,69 @@
 Fulford & Hatcher
 Fulford & J.Taylor
 Funck
 Furtado
 Furtado & Montien
 Fée
 Fürnr.
+G.A.Forbes, Windels & L.W.Burgess
 G.A.Fryxell & Sëmina
 G.A.Klebs
 G.A.M.Scott & D.C.Pike
 G.A.M.Scott & D.C.Pike ex Cargill
-G.A.M.Scott & I.G.Stone
 G.A.M.Scott & K.G.Beckm.
 G.A.de Vries
-G.A.de Vries & de Hoog
 G.Armstr.
 G.Arnaud
 G.Arnaud & Bitanc.
 G.Arnaud ex M.B.Ellis
 G.Arnaud ex MacGarvie
 G.Arnaud ex S.Hughes
 G.Arnaud ex Samson
 G.B.McGregor
 G.B.Ownbey
 G.Benn.
 G.Brockman & C.J.French
 G.Brückn.
+G.C.Adams & M.J.Wingf.
 G.C.Wall.
 G.C.Wall. ex W.B.Turner
 G.Chandler & Crisp
-G.Chandler & Crisp x Daviesia wyattiana F.M.Bailey
 G.Chandler, Crisp & R.J.Bayer
 G.Cochet ex Sigler & J.W.Carmich.
 G.Cunn.
 G.Cunn. ex P.K.Buchanan & Ryvarden
 G.D.Rowley
 G.De Toni
 G.Don
 G.Don & D.Don
 G.Don ex Loudon
 G.Don ex W.D.J.Koch
-G.Don x Dodonaea viscosa subsp. cuneata (Sm.) J.G.West
 G.E.Haglund
 G.E.Haglund & Markl.
 G.E.Sm.
 G.F.Atk.
 G.F.Laundon
-G.F.Orr & Kuehn
 G.F.Seidel
 G.F.Walsh
 G.Forst.
 G.Forst. ex Baill.
 G.Forst. ex Biehler
 G.Forst. ex Hook.f.
 G.Forst. ex Sparrm.
 G.Forst. ex Spreng.
 G.Forst. ex Willd.
-G.Forst. subsp. didymum - Jasminum didymum subsp. racemosum (F.Muell.) P.S.Green
-G.Forst. subsp. flaccidum x Asplenium gracillimum Colenso
-G.Forst. x Asplenium obtusatum subsp. northlandicum Brownsey
 G.Gaertn., B.Mey. & Scherb.
 G.Goeze
+G.H.Boo & L.Le Gall
+G.H.Boo, L.Le Gall, K.A.Mill. & S.M.Boo
 G.H.Otth
 G.H.Otth ex P.Karst.
-G.I.Hansen & Moestrup
 G.J.Allman
+G.J.D.Sm., K.D.Hyde, & Whalley
 G.J.Harden
 G.J.Harden & L.J.Murray
 G.J.Howell
 G.J.Jellis & Punith.
 G.J.Leach
 G.J.Leach & C.C.Towns.
 G.J.Leach & Cheek
@@ -25186,44 +25373,47 @@
 G.J.Lewis ex L.Bolus
 G.K.Sutherl.
 G.Karst.
 G.Kirchn.
 G.L.Barron
 G.L.Barron & L.V.Busch
 G.L.Davis
-G.L.Davis - Brachyscome tetrapterocarpa G.L.Davis
 G.L.Mey.
 G.L.Nesom
 G.L.Sm.
 G.L.Stout
 G.L.Webster
 G.Lister
 G.Lister & Cran
-G.Lister & Lister
+G.Lister & Petch
 G.Lister ex Meyl.
 G.Lodd.
 G.Lodd. ex Benth.
 G.Lodd. ex Drapiez
 G.Lodd. ex G.Don
 G.Lodd. ex J.Forbes
 G.Lodd. ex Lindl.
 G.M.Cunn., W.E.Mulham, P.L.Milthorpe & J.H.Leigh
 G.M.Gates & Noordel.
+G.M.Gates, B.M.Horton & Noordel.
+G.M.Gates, Caboň & Jančovič.
 G.M.Gates, Ševčíková & Borovička
 G.M.Plunkett & Lowry
 G.M.Sm.
 G.M.Sm. & Klyver
 G.Martens
 G.Martens ex Asch.
 G.Merr. ex R.Sant.
 G.Merr. ex Sandst.
 G.Mey.
-G.Moreno & Manjón
 G.Moreno & Martin
 G.Moreno & S.L.Stephenson
+G.Moreno, D.W.Mitch. & S.L.Stephenson
+G.Moreno, López-Vill., S.L.Stephenson & A.Castillo
+G.Moreno, Rosing, D.W.Mitch. & S.L.Stephenson
 G.Murray
 G.Murray & De Toni
 G.Murray & Kof.
 G.Murray & Whitting
 G.N.Backh.
 G.N.Backh. & Jeanes
 G.N.Backh., R.J.Bates, A.P.Br. & L.M.Copel.
@@ -25235,33 +25425,35 @@
 G.Norman ex Grev.
 G.Norman ex Ralfs
 G.P.Agarwal & V.P.Sahni
 G.P.Clinton
 G.P.Clinton & Ricker
 G.Perry ex B.J.Conn
 G.Piper
+G.Pérez & Carnegie
 G.R.Guerin
 G.R.Guerin & Wege
 G.R.Hasle
 G.R.Hasle & P.A.Sims
 G.R.Hend.
 G.R.Hend. & Chappill
 G.R.W.Arnold
 G.Roth
+G.S.Li, M.Poulsen & Z.W.de Beer
+G.S.Pegg & Carnegie
 G.S.Varad. & Gilmartin
 G.S.West
 G.Salisbury
 G.Schellenb.
 G.Schmid
 G.Schneid.
 G.Simpson & J.S.Thomson
 G.Sinclair
 G.Sjöstedt
 G.Sm.
-G.Sm. & Olliver
 G.Stev.
 G.Stev. & G.M.Taylor
 G.T.Kraft
 G.T.Kraft & A.Millar
 G.T.Kraft & I.A.Abbott
 G.T.Kraft & J.L.Olsen
 G.T.Kraft & J.M.Noble
@@ -25276,56 +25468,56 @@
 G.T.Plunkett & R.L.Barrett
 G.T.Plunkett, J.J.Bruhl & K.L.Wilson
 G.Thor
 G.Thor, Lücking & Matsumoto
 G.Valet
 G.W.Andrews
 G.W.Beaton
+G.W.Beaton & M.B.Ellis
 G.W.Beaton & Malajczuk
 G.W.Beaton & Weste
 G.W.Beaton, Pegler & T.W.K.Young
 G.W.Carr
 G.W.Carr & P.F.Horsfall
 G.W.F.Carlson
 G.W.Fisch.
 G.W.Gillett
 G.W.Lawson & D.M.John
 G.W.Martin
 G.W.Martin ex G.W.Martin
 G.W.Martin, K.S.Thind & Rehill
 G.W.Saunders
 G.W.Saunders & G.T.Kraft
+G.W.Saunders & Huisman
 G.W.Wilson
 G.Watt
 G.Winter
-G.Winter & Plowr.
 G.Zeller
 Gaarder
+Gadgil & M.A.Dick
 Gaertn.
 Gaertn. ex DC.
 Gagnebin
 Gagnep.
 Gagnep. & Tardieu
 Gagnep. ex Reveal & Hoogland
 Gaillard
 Gaillon
 Gain
 Galeotti
-Gams & H.-B.Jansson
 Gamundí
 Gamundí, Aramb. & Giaiotti
 Gand.
 Ganguly
 Garay
 Garay & Christenson
 Garcia & Casanova
 Garcke
 Garden ex L.
 Gardner
-Gardner ex Strid & Keighery
 Garima Singh, H.T. Lumbsch & I. Schmitt
 Garn.-Jones
 Garnet
 Garov.
 Garsault
 Gary W.Wilson & S.Venter
 Gasp.
@@ -25336,17 +25528,15 @@
 Gassin
 Gatty
 Gauba
 Gaudich.
 Gaudich. ex C.Agardh
 Gaudich. ex DC.
 Gaudich. ex Decne.
-Gaudich. x Adriana quadripartita (Labill.) Müll.Arg.
 Gaudin
-Gaum.
 Gaussen
 Gauth.-Lievre
 Gauth.-Lièvre
 Gay
 Gebelein
 Gebert
 Gedoelst
@@ -25361,50 +25551,52 @@
 Geh. ex M.Fleisch.
 Geh. ex Thér.
 Geh. ex Watts & Whitel.
 Gehrm.
 Geiseler
 Geitler
 Geitler ex Komárek
+Gelardi, Simonini & Vizzini
 Genev.
 Genth
 Gentilli
 Gentilli ex Bas
 Georg & Maechling
 Georgi
 Geras.
 Geras. ex Symon
 Gerbaulet
-Gerd. & T.H.Nicolson
+Gerd. & Trappe
 Gerlach & L.Nilsson
 Gerloff
 Germain
 Gerneck
-Gerome
 Gerr.-Corn. & J.A.Simpson
+Gert Hansen & Moestrup
 Geyl.
 Ghafoor
 Ghesq. & Henrard
 Giachini, Castellano, Trappe & V.L.Oliveira
 Giacom.
+Gibas, Sigler & Currah
 Gibbs
 Gibelli & Belli
 Gibert
 Gideon
 Gideon F.Sm., E.Laguna, Verloove & P.P.Ferrer
 Giesen
 Giffen
-Giglioli
 Gilb. & Nakasone
 Gilchrist & W.R.Stokes
 Gilg
 Gilg & Gilg-Ben.
 Gilg & Werderm.
 Gilg-Ben.
 Gilgado, Cano, Gené & Guarro
+Gilgado, Gené, Cano & Guarro
 Gilib.
 Gilkey
 Gill.K.Br. & Bayly
 Gill.K.Br. & Bostock
 Gillet
 Gilli
 Gillies & Hook.
@@ -25423,34 +25615,39 @@
 Gled.
 Gled. ex Scop.
 Gledhill
 Glenn, C.W.Bacon & Hanlin
 Glenny
 Gloxin
 Gluck
+Gminder
 Gobi
 Gobi ex F.Schmitz
 Godey
 Godr.
 Godr. & Gren.
 Goebel
 Goffinet
 Goffinet & W.R.Buck
 Goffinet, Wickett, O.Werner, Ros, A.J.Shaw & C.J.Cox
+Gogorza Gondra, J.Kruse, McTaggart, Boekhout & R.G.Shivas
 Goh & K.D.Hyde
+Goh, K.D.Hyde & W.H.Ho
+Goh, W.H.Ho, K.D.Hyde & K.M.Tsui
 Goid.
 Gojdics
 Goldberg
 Goldblatt
 Goldring
 Golovin ex Speer
 Golubić
 Gomes
 Gomes ex DC.
 Gomont
+Gonz.Frag. & Cif.
 Gonz.Sierra, Pezez Morales, Penes & Rivas Mart.
 Gonzalves
 Gooden.
 Goodsp.
 Goor
 Goos, R.D.Brooks & Lamore
 Gooss.
@@ -25460,14 +25657,15 @@
 Gordon-Mills & A.Millar
 Gordon-Mills & E.M.Woll.
 Gordon-Mills & G.T.Kraft
 Gordon-Mills & Womersley
 Goreau & E.A.Graham
 Gorozh.
 Gorski
+Goto
 Gottsb.
 Gottsche
 Gottsche & F.Muell.
 Gottsche ex Besch.
 Gottsche ex Castle
 Gottsche ex F.Muell.
 Gottsche ex Gottsche, Lindenb. & Nees
@@ -25490,33 +25688,32 @@
 Gradst. & Terken
 Graebn.
 Graeffer ex Ten.
 Graham
 Graham ex Benth.
 Graham ex Hook.
 Graham ex Wight
-Graham x Hibiscus heterophyllus Vent.
+Gramaje, T.I.Burgess & Armengol
 Gran
 Gran & Angst
 Gran & Braarud
 Gratel.
 Gratel. ex Bory
 Gray
 Gray ex Lindb.
 Grayling & Brooker
-Grayling & Brooker x Eucalyptus loxophleba Benth.
 Greenall
 Greene
 Greenm.
 Grelet
 Gren. & Billot
 Gren. & Godr.
+Gresl., Nakasone & Rajchenb.
 Greuet
 Greuter
-Grev
 Grev.
 Grev. & Arn.
 Grev. & C.Agardh
 Grev. & C.Agardh ex Sond.
 Grev. & Harv.
 Grev. ex A.W.F.Schmidt
 Grev. ex Gomont
@@ -25538,15 +25735,14 @@
 Grilli
 Grimwade
 Griseb.
 Griseb. ex Doweld & Reveal
 Grobbelaar, Z.W.de Beer & M.J.Wingf.
 Grobéty
 Groen.
-Groenh.
 Grolle
 Grolle & Tixier
 Grolle ex L.Söderstr. & A.Hagborg
 Gronov.
 Groover & H.C.Bold
 Grose & Marink.
 Grosse-Veldmann & Wiegend
@@ -25558,14 +25754,15 @@
 Grove ex Cannon
 Grube
 Grube & Hafellner
 Gruby
 Gruith.
 Grunow
 Grunow & Rabenh.
+Grunow ex A.W.F.Schmidt
 Grunow ex Bornet & Flahault
 Grunow ex C.Zimm.
 Grunow ex Cleve
 Grunow ex De Toni
 Grunow ex G.Murray & Boodle
 Grunow ex Hust.
 Grunow ex Mereschk.
@@ -25576,17 +25773,17 @@
 Gruyter, Aveskamp & Verkley
 Gryzenh. & M.J.Wingf.
 Grönblad
 Grönblad & A.M.Scott
 Grüning
 Grütz
 Guagl.
-Guarro, Cano & L.B.Pitarch
-Guarro, Cano & M.Solé
-Guarro, Cano, Gené & Gilgado
+Guarro & Punsola
+Guarro, Deanna A. Sutton, Wickes & Rajeev
+Guatim., R.W.Barreto & Crous
 Guba
 Guderley & Lumbsch
 Guerber & J.C.Correll
 Guers. ex DC.
 Guett.
 Gugerli
 Guiler
@@ -25618,23 +25815,24 @@
 Guzmán & F.Tapia
 Guzmán & Watling
 Guég.
 Gyeln.
 Gyeln. ex Anders
 Géneau
 Gérard
+Gérôme
+Gérôme & Labroy
 Gürke
 Güssow
 Güssow & Foster
 H.-M.Wheeler
 H.A.Crum
 H.A.Mill.
 H.A.Möller
 H.Akiy.
-H.Akiyama, T.Yamag. & M.Mohamed
 H.B.Carter
 H.B.Lee, J.A.Lewis, G.T.Kraft & I.K.Lee
 H.B.P.Upadhyay
 H.B.Will.
 H.B.Will. ex J.M.Black
 H.Bachm.
 H.Bruggen
@@ -25645,30 +25843,23 @@
 H.C.Gilbert
 H.C.Greene
 H.C.Wood
 H.C.Wood ex Bornet & Flahault
 H.Chick
 H.Deane
 H.Deane & Maiden
-H.Deane & Maiden x Eucalyptus aggregata H.Deane & Maiden
-H.Deane & Maiden x Eucalyptus crebra F.Muell.
-H.Deane & Maiden x Eucalyptus fibrosa subsp. nubilis (Maiden & Blakely) L.A.S.Johnson
-H.Deane & Maiden x Eucalyptus melanophloia F.Muell.
-H.Deane & Maiden x Eucalyptus saligna Sm.
-H.Deane & Maiden x Eucalyptus viminalis Labill.
 H.E.K.Hartmann
 H.E.K.Hartmann & Liede
 H.E.Moore
 H.E.Petersen
 H.Eichler
 H.Eichler ex Henwood
 H.Eichler ex Jeanes
 H.Eichler ex R.M.Barker
 H.Eichler ex W.T.Wang
-H.Eichler x Ranunculus sessiliflorus R.Br. ex DC.
 H.Ettl
 H.F.Comber
 H.F.Copel.
 H.Finch-Hatton
 H.G.Choi, G.T.Kraft & G.W.Saunders
 H.Gross
 H.Groves & J.Groves
@@ -25685,21 +25876,21 @@
 H.J.Clark
 H.J.Huds.
 H.J.Lam
 H.J.Lam & B.Meeuse
 H.J.P.Winkl.
 H.J.Schrad.
 H.J.Swart
-H.J.Swart & B.Sutton
 H.J.Swart & D.A.Griffiths
 H.J.Swart & J.Walker
 H.J.Swart & M.A.Will.
 H.J.Veitch
 H.Jacq.
 H.K.Orel
+H.K.Orel & Duretto
 H.K.Walter
 H.Karst.
 H.Karst. ex Schnizl.
 H.Klinggr.
 H.L.Li
 H.L.Sm.
 H.L.Wendl.
@@ -25748,25 +25939,26 @@
 H.S.Randhawa & R.S.Sandhu
 H.S.Yates
 H.Schaef.
 H.Schneid.
 H.Scholz
 H.Shang
 H.St.John
-H.Takay. & Adachi
+H.Takay. & M.Adachi
 H.Turner
 H.U.Ling & P.A.Tyler
 H.Vilm.
 H.Vilm. ex Trab.
 H.W.Anderson
 H.W.Bisch. & H.C.Bold
 H.W.Graham
 H.W.Graham & Bronik.
 H.W.Howard & Manton
 H.W.Johans. & Womersley
+H.W.Keller & T.E.Brooks
 H.Wakab.
 H.Walter
 H.Wendl.
 H.Wendl. & Drude
 H.Wendl. & Drude ex Hook.f.
 H.Wendl. ex Benth. & Hook.f.
 H.Wendl. ex H.J.Veitch
@@ -25789,27 +25981,26 @@
 Haeckel
 Haegi
 Haegi & P.S.Short
 Hafellner
 Hafellner & Bellem.
 Hafellner & Calat.
 Hafellner & Cl.Roux
-Hafellner & Grube
 Hafellner & Kalb
 Hafellner & Nav.-Ros.
 Hafellner & R.W.Rogers
 Hafellner & Vězda
 Hafellner, Poelt & Vězda
 Hafellner, S.Y.Kondr. & Kärnefelt
 Hagelst.
+Hagem
 Hagend, Soest & Zevenb.
 Hagstr.
 Haines
 Hajsig
-Hakul.
 Hale
 Hale & A.Fletcher
 Hale & Kurok.
 Hale ex Sipman
 Hale, Elix & J.Johnst.
 Halford
 Halford & A.J.Ford
@@ -25825,16 +26016,19 @@
 Haller ex Kuntze
 Haller ex Zinn
 Haller f.
 Hallier f.
 Hallier f. ex K.Krause
 Halling
 Halling & N.A.Fechner
+Halling, N.A.Fechner & Davoodian
 Halling, Osmundson & M.A.Neves
 Ham.
+Hamam.
+Hamam., Sugiy. & Komag.
 Hamel
 Hamel & A.Hamel
 Hamlin
 Hampe
 Hampe & Broth.
 Hampe & Broth. ex Watts
 Hampe & Geh.
@@ -25854,15 +26048,14 @@
 Hampe ex F.M.Bailey
 Hampe ex F.Muell.
 Hampe ex Geh.
 Hampe ex Kindb.
 Hampe ex Mitt.
 Hampe ex Müll.Hal.
 Hampe ex Paris
-Hampe ex Sond.
 Hampe ex Watts & Whitel.
 Hampe ex Wijk, Margad. & Florsch.
 Hance
 Hance ex Walp.
 Hand.-Mazz.
 Hanelt
 Hanin
@@ -25870,14 +26063,15 @@
 Hansf.
 Hansf. & Deighton
 Hansg.
 Hanst.
 Hantzsch
 Hantzsch ex Rabenh.
 Har.
+Har. & Pat.
 Hara
 Hardouin
 Hardy
 Hargraves & Guillard
 Harkn.
 Harley & J.F.B.Pastore
 Harm.
@@ -25887,35 +26081,36 @@
 Harting
 Hartm.
 Hartog
 Hartw. ex Gordon
 Harv.
 Harv. & Bailey
 Harv. & F.Muell.
-Harv. & F.Muell. ex F.Muell.
 Harv. & Gray
 Harv. & Grev.
 Harv. & Hook.f.
 Harv. & Sond.
 Harv. ex Calvo-Pérez, Molinari & Guiry
 Harv. ex E.P.Wright
 Harv. ex F.Schmitz & Hauptfl.
+Harv. ex Gomont
 Harv. ex Grunow
 Harv. ex Hook.
 Harv. ex J.Agardh
 Harv. ex J.E.Gray
 Harv. ex Kütz.
 Harv. ex Womersley
 Harwood
 Harz
 Haskins & J.F.T.Spencer
 Hasle
 Hasle & Fryxell
 Hasle & Guillard
 Hasle & Heimdal
+Hasle, Medlin & Syvertsen
 Hasle, Stosch & Syvertsen
 Hassall
 Hassall ex Ralfs
 Hassall ex West & G.S.West
 Hasselbr.
 Hasselq.
 Hasselq. ex L.
@@ -25924,41 +26119,39 @@
 Hastings
 Hatch
 Hatcher ex J.J.Engel
 Hattaway & D.H.Norris
 Hauck
 Hauman
 Hauptfl.
-Hauskn. & Ryvarden
 Hausskn.
 Haw.
 Haw. ex Willd.
-Haw. x Aloe maculata All.
 Hawke ex Messina
 Hawkeswood
 Hawkeswood & Mollemans
 Hayas.
 Hayata
 Hayek
 Hayne
 Haywood & Steid.
 Haywood, Steid. & L.Mack.
 Hazen
 Hazsl.
 He-Nygren, Juslen, Ahonen, Glenny & Piipo
 Heads
+Healy & M.E.Sm.
 Hebenstr.
 Heckel
 Hector
 Hedenäs
 Hedgc.
 Hedl.
 Hedw.
 Hedw. ex Brid.
-Hedw. ex Sm.
 Hedw. ex Wijk, Margad. & Florsch.
 Heeg
 Heenan & de Lange
 Hegelm.
 Heib.
 Heiberg
 Heiden
@@ -25991,21 +26184,21 @@
 Hend. ex R.Hogg
 Hendey
 Hendey & P.A.Sims
 Henfr.
 Henkel & Hochst.
 Henkel & W.Hochst.
 Henn.
-Henn. & Bres. ex Sacc.
 Henn. & E.Nyman
 Henn. & Lindau
 Henn. ex G.Cunn.
 Henn. ex McAlpine
 Henn. ex Sacc. & D.Sacc.
 Henneberg
+Hennebert
 Hennebert & B.G.Desai
 Hennipman
 Henrard
 Hensch.
 Hensen
 Hensl.
 Henssen
@@ -26019,21 +26212,25 @@
 Hepp ex Leight.
 Hepp ex Stein
 Hepp ex Th.Fr.
 Hepper & P.-M.L.Jaeger
 Herb.
 Herb. ex Lindl.
 Herb. ex Sweet
-Herbert
 Herdman
 Hereman
 Hering
 Hering & G.Martens
 Herink
 Herm.
+Hern.-Restr.
+Hern.-Restr. & Crous
+Hern.-Restr., Crous & M.J.Wingf.
+Hern.-Restr., J.Mena & Gené
+Hern.-Restr., R.F.Castañeda & Gené
 Herndon
 Hernández-Becerril & Meave del Castillo
 Herre
 Herrera-Campos & Lücking
 Herrm.
 Hershk.
 Hertel
@@ -26078,14 +26275,15 @@
 Hilse & Rabenh.
 Hindm. & Blaxell
 Hindák
 Hinode
 Hirasaka
 Hirats.f.
 Hirn
+Hirooka, Tanney & Seifert
 Hirschh.
 Hislop
 Hislop & A.J.G.Wilson
 Hislop & A.R.Chapm.
 Hislop & Albr.
 Hislop & Cranfield
 Hislop & K.A.Sheph.
@@ -26098,40 +26296,42 @@
 Hislop, Wege & A.D.Webb
 Hitchc.
 Hitchc. & Chase
 Hitchc. & Chase ex Pilg.
 Hjortstam
 Hjortstam & P.Roberts
 Hjortstam & Ryvarden
+Hjortstam & Spooner
+Hjortstam, P.Roberts & Spooner
 Hnatiuk
 Hochr.
 Hochr. ex Britten
-Hochr. x Hibiscus splendens C.Fraser ex Graham
 Hochst.
 Hochst. & Steud.
 Hochst. ex A.Braun
 Hochst. ex A.Rich.
 Hochst. ex C.Krauss
 Hochst. ex Chiov.
 Hochst. ex Dunal
 Hochst. ex Gürke
-Hochst. ex Hook.f.
+Hochst. ex Jaub. & Spach
 Hochst. ex R.E.Fr.
 Hochst. ex Steud.
-Hocking
 Hodel & Dowe
 Hodges & D.E.Gardner
 Hoffm.
 Hoffm. ex Brid.
 Hoffm. ex Funck
 Hoffmanns.
 Hoffmanns. & Link
 Hoffmanns. & Link ex Dumort.
 Hogg ex Sweet
 Hohen.
+Hol.-Jech. & Hennebert
+Hol.-Jech. & Mercado
 Holdom, Y.P.Tan & R.G.Shivas
 Hollenb.
 Hollenb. ex W.R.Taylor
 Hollerb., Kossinsk. & Poljansky
 Hollós
 Holmb.
 Holmes
@@ -26156,15 +26356,14 @@
 Hongo & A.K.Mills
 Honigm.
 Hood
 Hoogland
 Hooibr. ex Endl.
 Hook.
 Hook. & Arn.
-Hook. & Arn. x Peperomia tetraphylla Hook. & Arn.
 Hook. & B.D.Jacks.
 Hook. & Baker
 Hook. & Grev.
 Hook. & Harv.
 Hook. & Lindl.
 Hook. & Lindl. ex Duby
 Hook. & Taylor
@@ -26173,19 +26372,14 @@
 Hook. ex Graham
 Hook. ex Harv.
 Hook. ex Hook.f.
 Hook. ex Planch.
 Hook. ex Steetz
 Hook. ex T.Moore
 Hook. ex Walp.
-Hook. subsp. platypus x Eucalyptus spathulata Hook.
-Hook. subsp. platypus x Eucalyptus suggrandis L.A.S.Johnson & K.D.Hill
-Hook. subsp. spathulata x Eucalyptus tenera L.A.S.Johnson & K.D.Hill
-Hook. x Eucalyptus peltata Benth.
-Hook. x Pittosporum undulatum Vent.
 Hook.f.
 Hook.f. & Harv.
 Hook.f. & Taylor
 Hook.f. & Thomson
 Hook.f. & Wilson
 Hook.f. & Wilson ex Burges
 Hook.f. & Wilson ex Dixon
@@ -26195,49 +26389,34 @@
 Hook.f. & Wilson ex Mitt.
 Hook.f. & Wilson ex Paris
 Hook.f. & Wilson ex Watts & Whitel.
 Hook.f. & Wilson ex Wilson
 Hook.f. ex A.Gray
 Hook.f. ex Benth.
 Hook.f. ex Boeckeler
-Hook.f. ex Domin
 Hook.f. ex E.A.Shaw
 Hook.f. ex Hook.
 Hook.f. ex Kirk
 Hook.f. ex Kütz.
 Hook.f. ex Planch.
 Hook.f. ex Raoul
 Hook.f. ex T.Anderson
-Hook.f. x Eucalyptus amygdalina Labill.
-Hook.f. x Eucalyptus dalrympleana Maiden
-Hook.f. x Eucalyptus globulus Labill.) x Eucalyptus johnstonii Maiden
-Hook.f. x Eucalyptus johnstonii Maiden
-Hook.f. x Eucalyptus subcrenulata Maiden & Blakely
 Hope
 Hoppaugh
 Hoppe
 Hoppenr.
 Hopper
 Hopper & A.P.Br.
 Hopper & A.P.Br. ex A.P.Br. & G.Brockman
 Hopper & A.P.Br. ex Jeanes
-Hopper & A.P.Br. x Caladenia harringtoniae Hopper & A.P.Br.
-Hopper & A.P.Br. x Caladenia horistes Hopper & A.P.Br.
-Hopper & A.P.Br. x Caladenia infundibularis A.S.George
-Hopper & A.P.Br. x Caladenia longicauda Lindl.
-Hopper & A.P.Br. x Caladenia polychroma Hopper & A.P.Br.
-Hopper & A.P.Br. x Caladenia rhomboidiformis (E.Coleman) M.A.Clem. & Hopper
-Hopper & A.P.Br. x Caladenia roei Benth.
-Hopper & A.P.Br. x Caladenia vulgata Hopper & A.P.Br.
 Hopper & D.Nicolle
 Hopper & McQuoid
 Hopper & R.L.Barrett
 Hopper & Ward.-Johnson
 Hopper, S.J.van Leeuwen, A.P.Br. & S.J.Patrick
-Hora
 Hora ex Hora
 Horan.
 Horik.
 Horik. & Nog.
 Horkel ex Schleid.
 Horne ex Baker
 Hornem.
@@ -26255,14 +26434,21 @@
 Hortob.
 Hosok.
 Host
 Host ex Gaudin
 Host ex Roem.
 Hotchk.
 Hotchk. & Imahori
+Houbraken
+Houbraken & Pitt
+Houbraken & Quaedvl.
+Houbraken, Frisvad & Samson
+Houbraken, Visagie & Pitt
+Houbraken, Visagie & Samson
+Houbraken, Visagie, Samson & Seifert
 Houk & Klee
 Houlston
 Houtt.
 Howe
 Howell
 Hoyt
 Hu ex Cronquist
@@ -26275,14 +26461,15 @@
 Huebener
 Hughes
 Huijsman ex P.D.Orton
 Huisman
 Huisman & A.Millar
 Huisman & Borow.
 Huisman & G.T.Kraft
+Huisman & G.W.Saunders
 Huisman & Gordon-Mills
 Huisman, A.R.Sherwood & I.A.Abbott
 Huisman, De Clerck, Prud'homme & Borow.
 Huisman, Foard & G.T.Kraft
 Huisman, G.W.Saunders & A.R.Sherwood
 Huisman, I.A.Abbott & A.R.Sherwood
 Huitf.-Kaas
@@ -26301,91 +26488,100 @@
 Humphrey
 Huneycutt
 Huneycutt ex M.W.Dick
 Hunger
 Hurus.
 Hust.
 Hust. ex Simonsen
+Hustad & A.N.Mill.
+Hustad, A.N.Mill., Dentinger & P.F.Cannon
 Hutch.
 Hutch. & Dalziel
 Huth
+Huttunen & Ignatov
 Hy
 Hyl.
 Hyl. ex Vaar.
 Hyvonen & Piippo
 Härk.
 Hässel
 Hérib.
 Hérincq
-Hérincq ex Lavallee
+Hérincq ex Lavallée
 Höhn.
 Höhn. & Litsch.
 Höhn. ex Falck
 Höhnk
+Hösterm. & Laubert
+Høil. & Watling
 Hübner
 Hügel
 Hügel ex Benth.
 Hügel ex Endl.
 Hügel ex Ettingsh.
 Hügel ex Jacques
 Hügel ex Lindl.
 Hügel ex Rousselon
 I.A.Abbott
 I.A.Abbott & Huisman
 I.A.Abbott & Magruder
 I.A.N.Lucas
+I.Barnes & M.J.Wingf.
 I.C.Nielsen
 I.G.Stone
 I.G.Stone & Catches.
 I.G.Stone & G.A.M.Scott
+I.H.Boas
 I.Hagen
 I.Holliday
+I.Hutton
 I.Hutton & P.S.Green
 I.I.Tav.
 I.J.Wright & Ladiges
 I.Johans. & Ryvarden
 I.M.Johnst.
 I.M.Lamb
 I.M.Turner
 I.M.Wilson
 I.Miyake
 I.O.Cook & Ladiges
 I.P.Price & P.H.B.Talbot
 I.R.Hall
 I.R.Hall & L.K.Abbott
-I.R.Hall & W.N.Becker
 I.R.Price, Huisman & Borow.
 I.Schmitt, Kalb & Lumbsch
 I.Telford
 I.Telford & C.R.Marsden
 I.Telford & J.J.Bruhl
 I.Telford & L.M.Copel.
 I.Telford & Naaykens
 I.Telford & P.Sebastian
 I.Telford & R.L.Barrett
 I.Telford, Clugston & R.L.Barrett
 I.Thomps.
 I.Thomps. & J.H.Ross
-I.Thomps. x Hovea heterophylla A.Cunn. ex Hook.f.
-I.Thomps. x Hovea planifolia (Domin) J.H.Ross
-I.Thomps. x Hovea tholiformis I.Thomps.
 I.Verd.
 I.Williams
 Iamonico & Mosyakin
 Idrees & J.M.H.Shaw
+Ignatov & Fedosov
+Ignatov & Huttunen
+Ignatov & Ignatova
+Ignatov & Vanderp.
 Ihlenf., Schwantes & Straka
 Iljin
 Iltis
 Imahori
 Imazeki
 Imazeki & Toki
 Imhof
 Imshaug ex Kantvilas
 Indel. & A.R.Loebl.
 Ing
+Ing & Nann.-Bremek.
 Ingold
 Inoue
 Inoue & Fukuyo
 Inoue & Grolle
 Inoue & R.M.Schust.
 Irmisch ex Asch.
 Irwin ex Hatch
@@ -26396,36 +26592,36 @@
 Itono
 Itono & Tak.Tanaka
 Itono & Yoshiz.
 Itzigs.
 Itzigsohn
 Ivanjuk. & Doronina
 Iwanoff
-J.-E.Gilbert
 J.-F.Leroy
 J.-P.Frahm
 J.A.Armstr.
 J.A.Armstr. ex Duretto & P.I.Forst.
 J.A.Bever., Fensham & P.I.Forst.
+J.A.Cooper
+J.A.Crouch
 J.A.Crouch, B.B.Clarke, J.F.White & B.I.Hillman
 J.A.Davidson, D.Hartley, Priest, Krysinska-Kaczm., Herdina, A.McKay & E.S.Scott
 J.A.Duke
 J.A.G.Irwin
-J.A.G.Irwin, Shoemaker & C.E.Babc.
+J.A.Hall & Sivan.
 J.A.Lackey
 J.A.Lewis & G.T.Kraft
 J.A.Lewis & Womersley
 J.A.McDonald & R.Ismail
 J.A.Mey. & Nicot
 J.A.Petterson
 J.A.Phillips
 J.A.Simpson
 J.A.Simpson & C.Stone
 J.A.Simpson & Grgur.
-J.A.Simpson, Wollw. & M.Stadler
 J.A.West & Zuccarello
 J.Agardh
 J.Agardh ex A.Gepp & E.Gepp
 J.Agardh ex Aresch.
 J.Agardh ex Bornet & Flahault
 J.Agardh ex Gomont
 J.Agardh ex Grunow
@@ -26460,43 +26656,45 @@
 J.Barker
 J.Bausch
 J.Berggr. & Wahlenb.
 J.Bommer
 J.Buchholz & N.E.Gray
 J.C.David
 J.C.David & D.Hawksw.
-J.C.David & T.Y.Zhang
 J.C.F.Hopkins
 J.C.Fisch.
 J.C.Gilman & E.V.Abbott
 J.C.Jang & T.Chen
 J.C.Lindq. & Alippi
 J.C.Manning & Goldblatt
 J.C.Mikan
 J.C.Paula & De Clerck
 J.C.Schmidt
 J.C.Wendl.
 J.C.Wendl. ex Hornem.
 J.C.Wendl. ex Link
 J.C.Wendl. ex Pfeiff.
+J.C.Zamora
+J.Calvert, McTaggart & R.G.Shivas
+J.Campb., J.L.Anderson & Shearer
 J.Clayton
 J.Compton & Schrire
 J.D.Briggs & Crisp
 J.D.Briggs & J.A.Armstr.
 J.D.Briggs & Leigh
 J.D.Dodge
 J.D.Dodge & Hermes
 J.D.Godfrey
-J.D.Rogers, W.J.Kaiser & B.C.Wang
 J.D.Rogers, Y.M.Ju & F.San Martín
 J.Drumm.
 J.Drumm. ex Berk.
 J.Drumm. ex Harv.
 J.Drumm. ex Lindl.
 J.E.Br.
+J.E.Chilton
 J.E.Gray
 J.E.Jacques
 J.E.Lange
 J.E.Lange ex Herink
 J.E.Mackinnon, Ferrada & Montem.
 J.E.Reid, Ward.-Johnson & Maslin
 J.E.Wright
@@ -26523,35 +26721,38 @@
 J.F.Mill.
 J.F.Redhead ex T.H.Nicholson & N.C.Schenck
 J.F.White & P.V.Reddy
 J.Forbes
 J.Forbes ex Otto & A.Dietr.
 J.Fröhl. & K.D.Hyde
 J.Fröhl., K.D.Hyde & Aptroot
+J.Fröhl., K.D.Hyde & D.I.Guest
 J.Fröhl., K.D.Hyde & Joanne E.Taylor
+J.Fröhl., Lowen & K.D.Hyde
+J.Fröhl., Raga, Philemon & K.D.Hyde
 J.G.Bruce
 J.G.Gmel. ex Hohen.
 J.G.Klein ex Link
 J.G.Klein ex Willd.
 J.G.Kühn
 J.G.Sm.
 J.G.Sm. ex C.Mohr
 J.G.West
+J.G.West & Albr.
 J.Garden
 J.Garden & L.A.S.Johnson
 J.Gay
 J.Gay ex DC.
 J.Gay ex Guss.
 J.Gay ex Kunth
 J.Gay ex Laharpe
 J.Gay ex Poir.
 J.Graham
 J.Groves
 J.Groves ex Filarszky
-J.H.Boas
 J.H.Haines & Dumont
 J.H.Johnston
 J.H.Kirkbr.
 J.H.Mill.
 J.H.Mill., Giddens & A.A.Foster
 J.H.Mirza & Cain
 J.H.Ross
@@ -26565,26 +26766,29 @@
 J.H.Willis & B.Boivin
 J.H.Willis & Court
 J.H.Willis ex G.L.Davis
 J.H.Willis ex McGill.
 J.Heyward
 J.Hobson
 J.J.Bruhl & I.Telford
+J.J.Ellis & Hesselt.
 J.J.Engel
 J.J.Engel & G.L.Merr.
 J.J.Engel & Glenny
 J.J.Engel & R.M.Schust.
 J.J.Gold
 J.J.Halford & Jessup
 J.J.Lee, C.W.Reimer & McEnery
 J.J.Lee, Reimer & McEnery
+J.J.Muchovej
 J.J.Riley
 J.J.Rodr.
 J.J.Sm.
 J.J.Verm.
+J.J.Zhou & Kohlm.
 J.Jacq.
 J.Jacq. ex Spreng.
 J.John
 J.K.Bartlett & Vitt
 J.Kalb & K.Kalb
 J.Kern
 J.Kerner
@@ -26592,46 +26796,43 @@
 J.Koenig
 J.Koenig ex Gras
 J.Koenig ex L.
 J.Koenig ex Ridl.
 J.Koenig ex Roxb.
 J.Koenig ex Wight & Arn.
 J.Kost.
+J.Kruse, M.Lyons, McTaggart & R.G.Shivas
+J.Kruse, R.G.Shivas & McTaggart
+J.Kruse, Ryley, Y.P.Tan, Thines & R.G.Shivas
 J.Kuo
 J.Kuo & Cambridge
+J.L.Bezerra & Kimbr.
 J.L.Crane & Schokn.
 J.L.Crane & Shearer
+J.L.Cunn.
 J.L.Mulder
 J.L.Olsen & J.A.West
 J.L.Walsh, L.W.Burgess, E.C.Y.Liew & Summerell
+J.L.Walsh, M.H.Laurence, L.W.Burgess, E.C.Y.Liew & Summerell
 J.L.Walsh, Sangal., L.W.Burgess, E.C.Y.Liew & Summerell
-J.L.Yuill
 J.Larsen
 J.Larsen & D.J.Patt.
 J.Lloyd
 J.Lloyd ex Billot
 J.Lowe
 J.Luo & N.Zhang
 J.Léonard
 J.M.B.Sm. & Pillai
 J.M.B.Sm., Jolly, Georg & Connole
 J.M.Black
 J.M.Black & E.L.Robertson
-J.M.Black - Atriplex intermedia R.H.Anderson
-J.M.Black - Atriplex pseudocampanulata Aellen
 J.M.Black ex E.L.Robertson
 J.M.Black ex Eardley
 J.M.Black ex J.H.Willis
 J.M.Black ex N.G.Walsh
-J.M.Black x Acacia phlebocarpa F.Muell.
-J.M.Black x Acacia trachycarpa E.Pritz.
-J.M.Black x Acacia tumida var. kulparn M.W.McDonald
-J.M.Black x Acacia tumida var. pilbarensis M.W.McDonald
-J.M.Black x Cassinia tegulata Orchard
-J.M.Black x Hibbertia villifera Tepper ex Toelken
 J.M.Coult.
 J.M.H.Shaw
 J.M.Hart
 J.M.Hart & Henwood
 J.M.Mend.
 J.M.Noble
 J.M.Noble & G.T.Kraft
@@ -26653,15 +26854,18 @@
 J.N.Gagul & Crayn
 J.N.Rai, J.P.Tewari & Mukerji
 J.N.Rai, Wadhwani & J.P.Tewari
 J.O.Sousa, Baseia & M.P.Martín
 J.P.Bull
 J.P.Bull, S.J.Dillon & Brearley
 J.P.Ellis
+J.P.M.Araújo, Abell, Marney, R.G.Shivas, H.C.Evans & D.P.Hughes
+J.P.M.Araújo, R.G.Shivas, Abell, Marney, H.C.Evans & D.P.Hughes
 J.P.Roux
+J.P.Samp., M.Weiss & R.Bauer
 J.Palmer
 J.Palmer & Mowatt
 J.Phillipson
 J.Pickard
 J.Poiss.
 J.Presl
 J.Presl & C.Presl
@@ -26687,29 +26891,27 @@
 J.Raynal
 J.Remy
 J.Roy
 J.Roy & Bisset
 J.Roy & Bissett
 J.Roy ex Hirn
 J.S.Davis & Toml.
-J.S.F.Barker & M.W.Mill.
-J.S.F.Barker, M.W.Mill., Phaff, Starmer & M.Miranda
-J.S.F.Barker, Starmer, Lachance & J.M.Bowles
-J.S.F.Barker, Starmer, Lachance, J.M.Bowles, C.A.Rosa & Schlag-Edl.
 J.S.McCulloch
+J.S.Monteiro, S.M.Leão, Gusmão, P.M.Kirk & R.F.Castañeda
 J.S.Muell.
 J.S.Murray
+J.S.Oliveira
 J.S.Turner, Smithers & Hoogland
 J.Sadler
 J.Schiller
 J.Schiller & Diskus
 J.Schiller ex F.J.R.Taylor
-J.Schrot.
 J.Schröt.
 J.Schröt. & Henn.
+J.Schröt. ex Höhn. & Litsch
 J.Schust.
 J.Shaw
 J.Sinclair
 J.Sm.
 J.Sm. ex C.Chr.
 J.Sm. ex Hook.
 J.Sm. ex Hook.f.
@@ -26718,15 +26920,15 @@
 J.Steiner
 J.Steiner & Zahlbr.
 J.Steiner ex Fritsch
 J.T.Hunter
 J.T.Hunter & J.J.Bruhl
 J.T.Johanss.
 J.T.Palmer
-J.T.Queckett
+J.T.Quekett
 J.T.Simmons
 J.Taylor
 J.Traill
 J.V.Almeida & Sousa da Câmara
 J.V.Lamour.
 J.V.Lamour. ex C.Agardh
 J.V.Lamour. ex Duby
@@ -26737,81 +26939,83 @@
 J.W.Dawson
 J.W.G.Lund
 J.W.Green
 J.W.Green ex Rye
 J.W.Griff.
 J.W.Griff. & Henfr.
 J.W.Grimes
+J.W.Groves & Skolko
 J.W.Horn
 J.W.Loudon
 J.W.Mathews & L.Bolus
 J.W.Moore
 J.W.Walker ex Takht.
 J.Walker
 J.Walker & A.M.Sm.bis
-J.Walker & Alcorn
 J.Walker & Bertus
 J.Walker & Kile
 J.Walker & M.M.van der Merwe
 J.Walker & N.H.White
 J.Walker & Priest
 J.Walker & R.G.Shivas
 J.Walker & Stovold
 J.Walker & Vánky
-J.Walker, Pascoe & B.Sutton
-J.Walker, Priest, Pascoe & Beilharz
+J.Walker, B.Sutton & Pascoe
+J.Walker, Beilharz, Pascoe & Priest
 J.Wen, Kiapranis & Lovave
 J.White
-J.White x Eucalyptus tereticornis Sm.
 J.Williams
 J.Wrigley & Fagg
 J.Z.Weber
 J.Z.Weber & R.J.Bates
 J.Z.Weber ex Jeanes
 J.Zahlbr.
+J.de Wet, Slippers & M.J.Wingf.
 Jaag
 Jaap
 Jabl.
 Jack
 Jack ex Wall.
 Jackes
+Jackes & Trias-Blasi
 Jacks.
 Jacob-Makoy ex Heynh.
 Jacobi
 Jacobsen
 Jacq.
 Jacq. ex L.
 Jacq. ex Willd.
-Jacq. x Rosa moschata Herrm.
-Jacq. x Rosa multiflora Thunb. ex Murray
 Jacques
+Jacques & Hérincq
 Jacz.
 Jagadeesh Ram & G.P.Sinha
 Jagger
+Jan Kučera & Ignatov
 Jancey
 Janch.
 Janisch
 Janisch & Rabenh.
 Janisch.
+Janošík & Döbbeler
 Jansen
 Jansen & Wacht.
 Jansen & Wacht. ex B.K.Simon
 Jansen ex Renvoize
 Jao
 Jariangpr. & Elix
 Jariangprasert
 Jarman
 Jarosch & Besl
 Jatta
 Jaub. & Spach
 Jauhar & Joshi
+Jayasiri, E.B.G.Jones & K.D.Hyde
 Jean F.Brunel
 Jean White
 Jeanes
-Jeanes x Thelymitra gregaria D.L.Jones & M.A.Clem.
 Jedwabn.
 Jeng & J.C.Krug
 Jenkins
 Jenkins & Bitanc.
 Jenner ex Ralfs
 Jeps.
 Jermy
@@ -26820,46 +27024,43 @@
 Jessop
 Jessup
 Jessup & Bygrave
 Jessup & Guymer
 Jessup & W.J.de Wilde
 Jian Wang ter
 Jian Wang ter & A.R.Bean
+Joanne E.Taylor & Crous
 Joanne E.Taylor & K.D.Hyde
-Joanne E.Taylor & S.J.Lee
 Joanne E.Taylor, J.Fröhl. & K.D.Hyde
 Joanne E.Taylor, K.D.Hyde & E.B.G.Jones
 Jobson
 Jobson & P.H.Weston
 Jobson & Whiffin
 Johan-Olsen
 Johanson
+Johanssen, J.L.Walsh, M.H.Laurence, L.W.Burgess, E.C.Y.Liew & T.Petrović
 Johnson
 Jolycl.
 Jones ex R.Br.
-Jones ex Roxb.
 Jonker
 Jord.
 Jord. ex Boreau
 Joshua
 Joss.
 Joss. ex Dennis
 Jost
 Jousé
 Jovet & Guedes
 Jovet-Ast
 Joy Thomps.
 Joy Thomps. & L.A.S.Johnson
-Joy Thomps. & L.A.S.Johnson - Callitris verrucosa (A.Cunn. ex Endl.) F.Muell.
-Joy Thomps. & L.A.S.Johnson x Callitris verrucosa (A.Cunn. ex Endl.) F.Muell.
 Joyce & R.Butcher
 Judz.
 Juel
 Jul.Schäff.
-Julich
 Junfu Zhang & I.A.Abbott
 Jungh.
 Junius ex L.
 Jur.
 Jurilj
 Juss.
 Juss. ex Aubl.
@@ -26873,106 +27074,83 @@
 Juss. ex R.Br.
 Juss. ex Roussel
 Juss. ex Steud.
 Juss. ex Thouars
 Justo
 Juswara
 Juswara & Craven
-Jörg
-Jörg.
+Jørg.
 Jørg.Koch
 Jülich
 K.-D.Kemp & Paddock
 K.A.Ford
 K.A.Sheph.
 K.A.Sheph. & A.D.Crawford
 K.A.Sheph. & C.F.Wilkins
 K.A.Sheph. & Hislop
 K.A.Sheph. & K.R.Thiele
+K.A.Sheph. & Lepschi
 K.A.Sheph. & M.Lyons
 K.A.Sheph. & Paul G.Wilson
 K.A.Sheph. & R.A.Meissn.
 K.A.Sheph. & R.M.Barker
 K.A.Sheph. & Rye
 K.A.Sheph. & S.J.van Leeuwen
 K.A.Sheph. & Trudgen
 K.A.W.Williams
 K.Ahlner
 K.Ando
+K.Ando & Pitt
+K.Ando & Tubaki
 K.Bakker
 K.Brandt
 K.Byrne & Zucarello
 K.C.Fan
 K.C.Fan & Y.P.Fan
 K.C.Fan & Yung C.Wang
 K.C.Fan, Yung C.Wang & Kuo Y.Pan
 K.C.Landon
 K.D.Hill
 K.D.Hill & D.L.Jones
 K.D.Hill & L.A.S.Johnson
-K.D.Hill & L.A.S.Johnson - Corymbia dallachiana (Benth.) K.D.Hill & L.A.S.Johnson
 K.D.Hill & L.A.S.Johnson ex D.Nicolle & M.E.French
-K.D.Hill & L.A.S.Johnson x Corymbia confertiflora (Kippist) K.D.Hill & L.A.S.Johnson
-K.D.Hill & L.A.S.Johnson x Corymbia terminalis (F.Muell.) K.D.Hill & L.A.S.Johnson
-K.D.Hill & L.A.S.Johnson x Eucalyptus obesa Brooker & Hopper
-K.D.Hill & L.A.S.Johnson x Eucalyptus semiglobosa (Brooker) L.A.S.Johnson & K.D.Hill
 K.D.Hill ex D.Nicolle & M.E.French
-K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus foecunda Schauer
-K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus horistes L.A.S.Johnson & K.D.Hill
-K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus latens Brooker
-K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus lunata D.Nicolle & M.E.French
-K.D.Hill x Cycas platyphylla K.D.Hill
 K.D.Hyde
 K.D.Hyde & Aptroot
 K.D.Hyde & Borse
 K.D.Hyde & C.A.Pearce
-K.D.Hyde & Crous
-K.D.Hyde & E.B.G.Jones
 K.D.Hyde & Goh
 K.D.Hyde & J.Fröhl.
 K.D.Hyde & Nakagiri
+K.D.Hyde & P.F.Cannon
 K.D.Hyde & Rappaz
-K.D.Hyde & S.J.Stanley
 K.D.Hyde & S.W.Wong
 K.D.Hyde & Seifert
-K.D.Hyde & Shearer
-K.D.Hyde & Yanna
-K.D.Hyde, B.C.Paulus & Gadek
-K.D.Hyde, C.A.Pearce & Læssøe
-K.D.Hyde, C.A.Pearce & Reddell
-K.D.Hyde, Crous, W.Gams, L.Mostert, Vijaykr. & Jeewon
-K.D.Hyde, E.B.G.Jones & S.W.Wong
 K.D.Hyde, E.B.G.Jones, Læssøe & Whalley
 K.D.Hyde, Goh & Umali
+K.D.Hyde, Goh, Joanne E.Taylor & J.Fröhl.
 K.D.Hyde, J.Fröhl. & Aptroot
-K.D.Hyde, J.Fröhl. & D.I.Guest
 K.D.Hyde, J.Fröhl. & Joanne E.Taylor
-K.D.Hyde, J.Fröhl. & Lowen
-K.D.Hyde, J.Fröhl., Goh & Joanne .E.Taylor
-K.D.Hyde, J.Fröhl., Joanne E.Taylor & Goh
-K.D.Hyde, J.Fröhl., Raga & Philemon
 K.D.Hyde, Joanne E.Taylor & J.Fröhl.
-K.D.Hyde, K.M.Tsui & Hodgkiss
-K.D.Hyde, M.E.Barr & B.C.Paulus
-K.D.Hyde, S.W.Wong, W.H.Ho & S.J.Stanley
-K.D.Hyde, W.H.Ho & Goh
+K.D.Hyde, S.W.Wong & E.B.G.Jones
 K.D.Hyde, W.H.Ho & K.M.Tsui
-K.D.Hyde, W.H.Ho, K.M.Tsui & Hodgkiss
-K.D.Hyde, W.H.Ho, Yanna & McKenzie
-K.D.Hyde, Whalley & G.J.D.Sm.
+K.D.Hyde, W.H.Ho, E.B.G.Jones, K.M.Tsui & S.W.Wong
 K.D.Koenig
 K.D.Koenig & Sims
 K.D.Koenig ex L.
 K.D.Koenig ex Retz.
 K.D.Koenig ex Roxb.
+K.D.W.Busch
 K.D.Whitney
 K.D.Whitney & H.W.Keller
 K.E.Lohmann & G.W.Andrews
 K.F.Chung
+K.F.Rodrigues & Samuels
 K.G.Grell & Wohlf.-Botterm.
+K.G.Rivera, Houbraken & Seifert
 K.H.Nicholls
 K.H.Walther
 K.Harris & D.E.Bradley
 K.Hiray., Kaz.Tanaka & Shearer
 K.Hübner
 K.I.Goebel
 K.Iwats.
@@ -26995,70 +27173,73 @@
 K.L.Gibbons
 K.L.Gibbons & S.J.Dillon
 K.L.Gibbons, B.J.Conn & Henwood
 K.L.McDougall
 K.L.McDougall & C.J.Hook
 K.L.McDougall & G.T.Wright
 K.L.McDougall & N.G.Walsh
+K.L.Pang & E.B.G.Jones
 K.L.Vinogr.
 K.L.Wilson
 K.L.Wilson & D.I.Morris
 K.L.Wilson & Makinson
 K.L.Wilson, J.J.Bruhl & R.L.Barrett
 K.Lewin
 K.M.Curtis
 K.M.Drew
-K.M.Drew & Ron.Ross
 K.M.Putterill
 K.M.Taylor, T.I.Burgess & G.E.Hardy
+K.M.Tsui, Hodgkiss & K.D.Hyde
 K.M.Wong
-K.M.Zalessky
-K.M.Zalessky.
 K.Miura
 K.Möbius
-K.Möbius : Entwisle
 K.P.Jain & Cain
 K.P.Singh & D.D.Awasthi
 K.R.G.Nair
 K.R.Peterson, Desjardin & Hemmes
 K.R.Thiele
 K.R.Thiele & Cockerton
 K.R.Thiele & E.E.Schill.
 K.R.Thiele & G.R.Guerin
 K.R.Thiele & K.A.Sheph.
 K.R.Thiele & Ladiges
 K.R.Thiele & Nge
 K.R.Thiele & Prober
+K.R.Thiele & R.W.Davis
+K.R.Thiele & T.Hammer
 K.R.Thiele ex Kellermann
 K.R.West & P.H.Raven
+K.Schub. & U.Braun
+K.Schub., U.Braun & R.G.Shivas
+K.Schub., Zalar, Crous & U.Braun
 K.Schum.
 K.Schum. & K.Krause
 K.Schum. & Lauterb.
 K.Schum. & Warb.
 K.Schum. ex Markgr.
 K.Stachura-Suchoples & D.M.Williams
 K.Strøm
 K.Syme
-K.Syme & A.M.Young
-K.Syme & B.J.Rees
 K.Syme & T.Lebel
+K.Syme, Bonito, T.Lebel, N.A.Fechner & Halling
 K.T.Picard
 K.Taylor, P.A.Barber & T.I.Burgess
 K.Toyoda & D.M.Williams
 K.U.Kramer
 K.U.Kramer & Tindale
 K.W.Dixon
 K.W.Dixon & B.G.Briggs
 K.W.Dixon & Batty
 K.W.Dixon & Christenh.
 K.W.Dixon & Meney
 K.W.Dixon & R.L.Barrett
 K.W.Nam & Y.Saito
 K.Wilh.
 K.Yamada
+K.Zaleski
 Kabiersch
 Kabát & Bubák
 Kaiser
 Kajim.
 Kakudidi
 Kakudidi, Lazarides & Carnahan
 Kalb
@@ -27083,20 +27264,20 @@
 Kalchbr. ex Bres.
 Kalchbr. ex Cooke
 Kalchbr. ex F.Muell.
 Kalchbr. ex G.Cunn.
 Kalchbr. ex Massee
 Kalchbr. ex Thüm.
 Kalkman
-Kallersjo
 Kalm ex L.
 Kaltenb.
 Kamg.Nkuek., Jol.Roux & Z.W.de Beer
 Kamg.Nkuek., K.Jacobs & M.J.Wingf.
 Kamg.Nkuek., M.J.Wingf. & Jol.Roux
+Kamgan & Jol.Roux
 Kamienski
 Kamptner
 Kaneh.
 Kaneh. & Hatus.
 Kanis
 Kanis ex J.Palmer
 Kanitz
@@ -27108,32 +27289,28 @@
 Kantvilas & Grube
 Kantvilas & Kukwa
 Kantvilas & Lumbsch
 Kantvilas & Messuti
 Kantvilas & P.M.McCarthy
 Kantvilas & Printzen
 Kantvilas & S.Y.Kondr.
-Kantvilas & Sochting
 Kantvilas & Søchting
-Kantvilas & Van den Boom
-Kantvilas & Vezda
 Kantvilas & Vězda
 Kantvilas & Wedin
 Kantvilas & van den Boom
 Kantvilas, Elix & A.W.Archer
 Kantvilas, Elix & P.James
 Kantvilas, Hafellner & Elix
 Kantvilas, Lumbsch & Elix
 Kantvilas, Rivas Plata & Lücking
 Kapil ex Takht.
 Kar. & Kir.
-Karajeva
+Karaeva
 Karling
 Karling ex Letcher
-Karnefelt
 Karsten
 Kaschik
 Kashiw.
 Katzn. & F.H.W.Morley
 Kauffman
 Kaulf.
 Kaulf. ex C.Presl
@@ -27143,14 +27320,15 @@
 Kavulak
 Kaz.Tanaka & K.Hiray.
 Kazandj. & Peter G.Wilson
 Keck
 Keighery
 Keighery & Cranfield
 Keighery & N.G.Marchant
+Keighery & Olde
 Keighery & Rye
 Keighery & T.D.Macfarl.
 Keighery ex Henwood
 Keighery, K.W.Dixon & R.L.Barrett
 Keilin
 Keissl.
 Kellermann
@@ -27175,39 +27353,40 @@
 Kerch.
 Kerr
 Kerr ex Barnett
 Kerrigan
 Kers
 Keuch.
 Keyserl.
+Khaliq & T.I.Burgess
 Khalk.
-Khodos., Vondrak & Soun
+Khemmuk, Geering & R.G.Shivas
+Khmelnitsky
+Khmelnitsky & Halling
 Khokhr. & Gornostaĭ
 Kiaer ex F.M.Bailey
 Kickx
 Kiffer
+Kijporn. & Aime
 Kile & Watling
-Kile, Læssøe & Whalley
 Kill.
 Kimbr.
-Kimbr. & J.L.Bezerra
 Kimbr. & Korf
 Kimbr. & M.Lenz
+Kimbr., Luck-Allen & Cain
 Kindb.
-Kindb. ex Streimann & Curn.
 King
 King & Gamble
 King & Pantl.
 King ex Hook.f.
 Kinney
 Kippist
 Kippist & Meisn.
 Kippist ex Lindl.
 Kippist ex Meisn.
-Kippist x Eucalyptus papuana F.Muell.
 Kirchn.
 Kirchner ex Bornet & Flahault
 Kirk
 Kirkp.
 Kirp.
 Kirschl.
 Kirschner, H.Øllg. & Štěpánek
@@ -27217,16 +27396,14 @@
 Kit.
 Kitaura & A.P.Lorenz
 Kitt.
 Kitton
 Kitton & Grove ex Rattray
 Kjellm.
 Klatt
-Klatt subsp. leichtlinii x Freesia leichtlinii subsp. alba (G.L.Mey.) J.C.Manning & Goldblatt
-Klatt x Freesia refracta (Jacq.) Klatt
 Kleb.
 Klein ex Willd.
 Klinge
 Kloot
 Klopotek
 Klopper & Gideon F.Sm.
 Klotzsch
@@ -27241,19 +27418,19 @@
 Klöcker
 Kneuck.
 Kniep
 Knight
 Knight & Perry ex Gordon
 Knight & T.A.Perry
 Knight ex Paxton
-Knight x Grevillea sessilis C.T.White & W.D.Francis
 Knobl.
 Knowles & Westc.
 Knuth
 Kny
+Kobayasi
 Kobayasi & Imazeki
 Koch
 Koch ex Schultz
 Kochman
 Koczwara
 Kodela
 Kodela & G.J.Harden
@@ -27271,24 +27448,20 @@
 Kof. & Skogsb.
 Kof. & Swezy
 Kof. ex Poche
 Koh
 Koh ex Womersley
 Kohlm.
 Kohlm. & E.Kohlm.
-Kohlm. & J.J.Zhou
-Kohlm. & Meyers
 Kohlm. & S.Schatz
 Kohlm. & Vittal
 Kohlm. & Volkm.-Kohlm.
 Kohlm., I.Schmidt & N.B.Nair
 Kohlm., Volkm.-Kohlm., Suetrong, Sakay. & E.B.G.Jones
 Koidz.
-Koidz. x (Salix matsudana Koidz. x Salix alba L.
-Koidz. x Salix alba L.
 Koker, Burds. & B.J.H.Janse
 Kol
 Kom.
 Komark.-Legn.
 Komiya
 Komárek
 Komárek & Anagn.
@@ -27296,18 +27469,14 @@
 Konrad
 Konrat & Braggins
 Konstant. & Melikyan
 Koord.
 Koord. & Valeton
 Kores
 Korf
-Korf & Kimbr.
-Korf & W.Y.Zhuang
-Korf, Brumm. & Rifai
-Korf, Rifai & Chin S.Yang
 Korneva
 Kornmann
 Kornmann & Sahling
 Korshikov
 Korth.
 Korth. ex Miq.
 Kosky
@@ -27323,45 +27492,46 @@
 Kotl. & Pouzar
 Kotschy ex Schweinf.
 Kottek
 Kovács, Trappe & Claridge
 Kozak.
 Kraenzl.
 Kraenzl. ex Guillaumin
-Kraichak, Lucking & Lumbsch
 Kraichak, Lücking & Lumbsch
 Kraisit., Pfister & M.E.Sm.
 Kramina & D.D.Sokoloff
 Krammer
 Krapov. & Cristobal
 Krapov. & W.C.Greg.
 Krasske
 Krasske ex Hust.
 Krause
 Kreger-van Rij
 Kreisel
-Kreisel ex P.M.Kirk, P.F.Cannon & J.C.David
+Kreisel & D.Krüger
 Kremp.
 Kremp. ex F.Wilson
 Kremp. ex Gyeln.
 Krestovsk.
 Kriesel
 Krock.
 Krog
 Krog & Swinscow
 Krombh.
 Krosnick & A.J.Ford
 Kruijt & Gradst.
+Krwanji
 Krzemien. & Badura
 Kubitzki
 Kuchel
 Kuck.
 Kuck. & Skottsb.
 Kuck. ex Oltm.
 Kuehn
+Kuehn & G.F.Orr
 Kuetz. ex Bornet & Flahault
 Kuff.
 Kuhlm.
 Kuhn
 Kuiter
 Kukkonen
 Kukwa & Pérez-Ortega
@@ -27389,156 +27559,133 @@
 Kunze ex Schwägr.
 Kuprian.
 Kurok.
 Kurok. & Elix
 Kurok. & Filson
 Kurok. & Moon
 Kurok. ex Elix
-Kurok. ex Elix & J.Johnst.
 Kurt Först.
 Kurtzman
 Kurtzman & M.Suzuki
+Kurtzman & Robnett
 Kurtzman, Robnett & Basehoar-Powers
-Kurtzman, Vaughan-Mart., S.A.Mey. & E.B.O'Neill
-Kurtzman, Wick. & Herman
 Kurz
 Kuthub. & Nawawi
 Kuwah.
+Kuyper
 Kylin
+Källersjö
 Kärnefelt
 Kõljalg & Dunstan
 Körb.
 Körn.
 Körn. ex Fuckel
 Körn. ex Müll.Berol.
+Küchenm. & Rabenh.
 Kühner
 Kühner & Lamoure
 Kühner & Maire
 Kühner ex Donk
 Kühner ex Singer
 Kühner ex Wasser
 Kük.
 Kük. & S.T.Blake
 Kük. ex Cheeseman
 Kük. ex Hochr.
 Kük. ex S.T.Blake
-Kütz
 Kütz.
 Kütz. ex Anagn. & Komárek
 Kütz. ex Bornet & Flahault
 Kütz. ex Entwisle & Foard
 Kütz. ex Gomont
-Kütz. ex Gomont.
 Kütz. ex Hirn
 Kütz. ex Ralfs
 Kütz. ex W.D.J.Koch
 L'Hér.
 L'Hér. ex DC.
 L'Hér. ex Hook.f.
 L'Hér. ex Pers.
 L'Hér. ex Vent.
-L'Hér. x Eucalyptus regnans F.Muell.
 L.
-L. - Tribulus terrestis J.W.Green
 L. ex G.Forst.
-L. ex Hedw.
 L. ex Jolycl.
 L. ex Kuntze
 L. ex Pall.
 L. ex Rottb.
 L. ex de Vriese
-L. subsp. cinerea x Salix x reichardtii A.Kern.
-L. x (Salix matsudana Koidz. x Salix alba L.
-L. x Avena sativa L.
-L. x Lolium rigidum Gaudin
-L. x Onopordum illyricum L.
-L. x Phalaris arundinacea L.
-L. x Psidium guineense Sw.
-L. x Rubus parvifolius L.
-L. x Rumex obtusifolius L.
-L. x Rumex pulcher L.
-L. x Salix nigra Marshall
-L. x Salix viminalis L.
-L. x Salix x fragilis L.
 L.A.Harper, M.C.Derbyshire, Lopez-Ruiz
 L.A.Nilsson
 L.A.S.Johnson
 L.A.S.Johnson & B.G.Briggs
 L.A.S.Johnson & Blaxell
-L.A.S.Johnson & Blaxell x Eucalyptus ovata Labill.
 L.A.S.Johnson & D.F.Cutler
 L.A.S.Johnson & D.I.Morris
 L.A.S.Johnson & K.D.Hill
 L.A.S.Johnson & K.D.Hill ex Brooker
 L.A.S.Johnson & K.D.Hill ex D.Nicolle & Brooker
 L.A.S.Johnson & K.D.Hill ex D.Nicolle & M.E.French
-L.A.S.Johnson & K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus horistes L.A.S.Johnson & K.D.Hill
-L.A.S.Johnson & K.D.Hill ex D.Nicolle & M.E.French - Eucalyptus olivina Brooker & Hopper
-L.A.S.Johnson & K.D.Hill subsp. suggrandis - Eucalyptus suggrandis subsp. promiscua D.Nicolle & Brooker
-L.A.S.Johnson & K.D.Hill x Eucalyptus pruinosa Schauer
-L.A.S.Johnson & K.D.Hill x Eucalyptus shirleyi Maiden
-L.A.S.Johnson & K.D.Hill x Eucalyptus sieberi L.A.S.Johnson
-L.A.S.Johnson & K.D.Hill x Eucalyptus thozetiana (F.Muell. ex Maiden) R.T.Baker
-L.A.S.Johnson & K.D.Hill x Eucalyptus xanthoclada Brooker & A.R.Bean
 L.A.S.Johnson & McGill.
 L.A.S.Johnson & O.D.Evans
-L.A.S.Johnson & O.D.Evans x Restio fimbriatus L.A.S.Johnson & O.D.Evans
 L.A.S.Johnson & P.H.Weston
-L.A.S.Johnson - Juncus polyanthemus Buchenau
 L.A.S.Johnson ex Brooker
 L.A.S.Johnson ex Brooker & Slee
 L.A.S.Johnson ex G.J.Leach
 L.A.S.Johnson ex K.L.Wilson
-L.A.S.Johnson subsp. alexandri x Juncus laeviusculus L.A.S.Johnson
-L.A.S.Johnson x Allocasuarina littoralis (Salisb.) L.A.S.Johnson
-L.A.S.Johnson x Juncus continuus L.A.S.Johnson
-L.A.S.Johnson x Juncus laeviusculus L.A.S.Johnson
-L.A.S.Johnson x Juncus radula Buchenau
-L.A.S.Johnson x Juncus usitatus L.A.S.Johnson
-L.A.S.Johnson x Macrozamia macleayi Miq.
 L.A.Shuttlew., E.C.Y.Liew & D.I.Guest
+L.A.Shuttlew., K.Scarlett, Entwistle & R.Daniel
 L.A.Shuttlew., K.Scarlett, R.Daniel & D.I.Guest
 L.Becker ex E.Fisch.
 L.Bolus
+L.C.Lane & Shearer
 L.D.Benson
 L.D.Pipes, P.A.Tyler & Leedale
-L.D.Pryor
 L.D.Pryor & J.H.Willis
 L.D.Pryor & L.A.S.Johnson
 L.D.Pryor & L.A.S.Johnson ex Brooker
 L.D.Pryor & L.A.S.Johnson ex Brooker & Slee
+L.E.Parkinson, E.K.Dann & R.G.Shivas
 L.E.Phillips
 L.E.Phillips & W.A.Nelson
 L.E.Phillips, H.G.Choi, G.W.Saunders & G.T.Kraft
 L.E.Rodin
 L.G.Adams
 L.G.Clark, Wendel & Craven
 L.Gentil
 L.H.Bailey
 L.H.Bailey ex D.Fairchild
 L.H.Crosby & E.J.F.Wood
 L.H.Crosby, E.J.F.Wood & Cassie
 L.H.Huang & Backus
 L.Hoffm.
 L.I.Savicz & Smirnova
+L.J.Vaughan, L.Tegart, Douch & T.Lebel
 L.K.Jones
+L.Kiss & Vaghefi
+L.Kiss, L.Kelly & Vaghefi
 L.L.Zhou, Y.C.F.Zu & R.M.K.Saunders
 L.Ling
+L.Lombard
 L.Lombard & Crous
+L.Lombard & Sand.-Den.
+L.Lombard, Crous & W.Gams
+L.Lombard, M.J.Wingf. & Crous
 L.Léger & Duboscq
 L.Léger & M.Gauthier
 L.M.Copel.
 L.M.Copel. & I.Telford
 L.M.Copel., J.Holmes & G.Holmes
 L.M.Kohn
 L.M.Lu & Jackes
 L.Mangin
+L.Mangin & Pat.
 L.Marchand
 L.McDougall & Porteners
 L.Moewus
+L.Mostert, Summerb. & Crous
+L.Mostert, W.Gams & Crous
 L.N.Johnson
 L.Neumann
 L.O.Williams
 L.P.Johnson
 L.Plate
 L.Preiss
 L.Preiss ex Endl.
@@ -27552,70 +27699,57 @@
 L.S.Olive
 L.S.Olive & Spiltoir
 L.S.Olive & Stoian.
 L.S.Sm.
 L.S.Sm. ex P.I.Forst.
 L.S.Sm. ex S.T.Reynolds
 L.S.Tai & Skogsb.
+L.Swart & Crous
 L.T.Ellis
-L.W.Burgess & Sangal.
-L.W.Burgess, G.A.Forbes & Windels
+L.V.Alvarez & Crous
 L.W.Burgess, P.E.Nelson & Toussoun
 L.W.Cayzer & Crisp
 L.W.Cayzer & D.L.Jones
 L.W.Cayzer, Crisp & I.Telford
 L.W.Hou & Yarden
+L.W.Hou, Crous & L.Cai
+L.W.Hou, L.Cai & Crous
 L.W.Sage
 L.W.Sage & Albr.
 L.W.Sage & Cranfield
 L.W.Sage & J.P.Pigott
 L.W.Sage & K.A.Sheph.
 L.W.Sage & K.W.Dixon
 L.W.Sage & M.D.Barrett
 L.W.Sage & S.J.van Leeuwen
+L.W.Zhou & S.L.Liu
+L.W.Zhou, S.L.Liu & T.W.May
+L.W.Zhou, Tedersoo & Y.C.Dai
+L.W.Zhou, Y.C.Dai & Sheng H.Wu
 L.Watson
 L.Watson & T.D.Macfarl.
 L.Watson ex Doweld & Reveal
 L.Weber
 L.Winter ex A.Berger
 L.f.
 L.f. ex Aiton
 L.f. ex Poir.
-L.f. x Mesembryanthemum haeckeliana A.Berger
 La Llave
 La Llave & Lex.
+La Touche
 Labiak, Sundue & R.C.Moran
 Labill.
 Labill. ex DC.
 Labill. ex Juss.
 Labill. ex Vent.
-Labill. x Eucalyptus barberi L.A.S.Johnson & Blaxell
-Labill. x Eucalyptus coccifera Hook.f.
-Labill. x Eucalyptus cordata Labill.
-Labill. x Eucalyptus dalrympleana Maiden
-Labill. x Eucalyptus globulus Labill.
-Labill. x Eucalyptus lehmannii (Schauer) Benth.
-Labill. x Eucalyptus lehmannii subsp. parallela D.Nicolle & M.E.French
-Labill. x Eucalyptus linearis Dehnh.
-Labill. x Eucalyptus nitida Hook.f.
-Labill. x Eucalyptus ovata Labill.
-Labill. x Eucalyptus pauciflora Sieber ex Spreng.
-Labill. x Eucalyptus pulchella Desf.
-Labill. x Eucalyptus risdonii Hook.f.
-Labill. x Eucalyptus rubida H.Deane & Maiden
-Labill. x Eucalyptus sieberi L.A.S.Johnson
-Labill. x Eucalyptus sieberiana F.Muell.
-Labill. x Eucalyptus simmondsii Maiden
-Labill. x Eucalyptus urnigera Hook.f.) x Eucalyptus johnstonii Maiden
-Labill. x Eucalyptus viminalis Hook.
-Labill. x Eucalyptus viminalis Labill.
-Labill. x Prostanthera spinosa F.Muell.
 Labour.
 Lace
+Lachance, C.A.Rosa & E.J.Carvajal
 Lachance, C.A.Rosa, Starmer, Schlag-Edl., J.S.F.Barker & J.M.Bowles
+Lachance, J.M.Bowles, Starmer & J.S.F.Barker
 Lack
 Lack & S.Holzapfel
 Ladiges & Whiffin
 Ladiges, Humphries & Brooker
 Lag.
 Lag. & Rodr.
 Lag. ex DC.
@@ -27633,33 +27767,31 @@
 Laird
 Laird ex Laird
 Lally
 Lam.
 Lam. & DC.
 Lam. ex P.Beauv.
 Lam. ex Poir.
-Lam. x Lolium perenne L.
 Lamb.
 Lambotte
 Lambotte & Fautrey
 Lammers
 Lamont
 Lamotte
 Lamoure
 Lander
-Lander & Barry
 Lander & L.A.S.Johnson
 Lander & N.G.Walsh
 Lander & P.J.H.Hurter
+Lander & R.Barry
 Landolt
 Landsb.
 Langdon
 Langdon & Boughton
 Langdon & Full.
-Langdon & Tommerup
 Lange
 Lange-Bert.
 Lange-Bert. & Bonik
 Lange-Bert. & E.Reichardt
 Lange-Bert. & Krammer
 Lange-Bert. & Metzeltin
 Lange-Bert., Fuhrmann & Werum
@@ -27670,29 +27802,28 @@
 Lapinpuro
 Large, Braggins & P.S.Green
 Largent
 Largent & Abell-Davis
 Largent & Bergemann
 Largent & R.G.Benedict
 Largent & Sk.Moore
-Largent & Skye Moore
 Larkum
 Lasch
 Latz
 Latz & Albr.
 Laubert
 Lauder
 Laun.
 Launert
 Launert & Paiva
 Laurer
 Lauterb.
 Lauterb. & K.Schum.
 Lauterborn
-Lavallee
+Lavallée
 Lavarack
 Lavarack & B.Gray
 Lavarack & Dockrill
 Lavarack & P.J.Cribb
 Laveran
 Lavrov
 Laxa
@@ -27705,14 +27836,16 @@
 Le Gal ex Le Gal
 Le Gal ex Rifai
 Le Jol.
 Le Prévost
 Le Texnier
 Leaney
 Leberle
+Lebert
+Lechat & P.-A.Moreau
 Lecoq & Juill.
 Ledeb.
 Ledeb. ex Link
 Leenh.
 Leers
 Lees ex Leight.
 Leeson & Rozefelds
@@ -27753,61 +27886,68 @@
 Lenorm. ex Kütz.
 Lenorm. ex Rosanoff
 Lenorm. ex Sauv.
 Lenorm. ex W.Archer
 Lentz
 Lenz
 Leonard
+Leontyev, C.Rojas, T. van der Heul, Kochergina & Schnittler
 Leontyev, Schnittler, G.Moreno, S.L.Stephenson, D.W.Mitch. & C.Rojas
-Lepp & B.J.Rees
+Leontyev, Schnittler, T.E. dela Cruz, M.F.B.Eloreta & T. van der Heul
+Lepr. & Mont.
 Lepschi
 Lepschi & Trudgen
 Lepschi & Wege
 Les & D.J.Crawford
 Lesc.
 Lesch.
 Lesch. ex A.DC.
 Lesp. & Thevenau
 Less.
 Less. ex Baker
 Less. ex Ledeb.
 Lest-Garl.
 Letcher
 Letcher & M.J.Powell
+Letcher, Longcore and M.J.Powell
 Lettau
 Leud.-Fort.
 Leud.-Fortm.
 Levander
 Levier
+Levkov, Metzeltin & A.Pavlov
 Levring
 Levyns
 Lewington & Maslin
 Lewton
 Leyb.
 Leyss.
 Lhotsky
 Lhotsky ex Meisn.
 Li Bing Zhang & K.W.Xu
 Li Bing Zhang, L.D.Sheph., D.K.Chen, X.M.Zhou & H.He
 Lib.
+Liber & Bonito
 Libert
 Libosch.
 Lichtw.
 Lichtw. & M.C.Williams
 Lichtw., Ferrington & López-Lastra
 Lickey
 Liddle & P.I.Forst.
 Liebm.
 Liede
 Lightf.
 Lightf. ex Turner
+Liimat.
 Lilj.
 Lilja
 Lillick
 Lillo
+Limbongan, Anth.J.Young, S.Campbell, Galea & Y.P.Tan
 Limpr.
 Lincz.
 Lind
 Lindau
 Lindauer
 Lindauer ex V.J.Chapm.
 Lindb.
@@ -27833,27 +27973,15 @@
 Lindl. ex Benth.
 Lindl. ex Boeckeler
 Lindl. ex Hook.
 Lindl. ex Meisn.
 Lindl. ex Oliv.
 Lindl. ex Paxton
 Lindl. ex Planch.
-Lindl. x Bursaria tenuifolia F.M.Bailey
-Lindl. x Dendrobium antennatum Lindl.
-Lindl. x Dendrobium johannis Rchb.f.
-Lindl. x Dendrobium linguiforme Sw.
-Lindl. x Dendrobium nindii W.Hill
-Lindl. x Dendrobium pugioniforme A.Cunn.
-Lindl. x Dendrobium sect. Phalaenanthe Schltr.
-Lindl. x Dendrobium semifuscum (Rchb.f.) Lavarack & P.J.Cribb
-Lindl. x Dendrobium teretifolium var. aureum F.M.Bailey
-Lindl. x Diuris corymbosa Lindl.
-Lindl. x Epidendrum secundum Jacq.
-Lindl. x Thelymitra ixioides Sw.
-Lindl. x Tribonanthes brachypetala Lindl.
+Lindl. ex Steud.
 Lindm.
 Lindner & Genoud
 Lindr.
 Lindsay
 Lindt
 Lingelsh.
 Link
@@ -27866,26 +27994,31 @@
 Link ex Hirn
 Link ex Schauer
 Link ex Spreng.
 Linnem.
 Liou & H.C.Cheng
 Liro
 Lister
+Lister & G.Lister
 Lister ex Minakata
 Litsch.
 Litsch. ex Pilát
 Livera
 Lizano & Lücking
 Lloyd
-Lloyd ex E.K.Cash & J.A.Stev.
 Lloyd ex G.Cunn.
+Lloyd ex J.A.Stev. & E.K.Cash
 Lloyd ex J.E.Wright
 Lloyd ex Torrend
+Lobban
+Lobban & Emm.S.Santos
+Lobban & S.Blanco
 Lobik
 Loconte
+Locq. ex A.Hashim. & Kaz.Tanaka
 Locq. ex E.Horak
 Locq. ex Singer
 Lodd.
 Lodd. ex DC.
 Lodd. ex G.Don
 Lodd. ex Hook.
 Lodd. ex Kuntze
@@ -27894,26 +28027,28 @@
 Lodd., G.Lodd. & W.Lodd.
 Lodd., G.Lodd. & W.Lodd. ex Courtois
 Lodd., G.Lodd. & W.Lodd. ex DC.
 Lodd., G.Lodd. & W.Lodd. ex Loudon
 Lodd., G.Lodd. & W.Lodd. ex Steud.
 Lodder
 Lodder & Kreger-van Rij
+Lodge, Vizzini, Ercole & Boertm.
 Lodha & K.R.C.Reddy
 Loebl. & A.R.Loebl.
 Loefl.
 Loefl. ex L.
 Loes.
 Loes. ex Harms
 Loeske
 Lohmann
 Loisel.
 Long & S.Ahmad
 Long ex G.P.Clinton
 Longcore
+Longcore, D.J.S.Barr & Désauln.
 Longcore, Pessier & D.K.Nichols
 Longyear
 Loomis
 Loos
 Lorb. ex Mull.Frib.
 Lorch
 Lorentz
@@ -27931,14 +28066,16 @@
 Lowrie & Carlquist
 Lowrie & Conran
 Lowrie & Kenneally
 Lowrie & N.G.Marchant
 Lowrie, A.H.Burb. & Kenneally
 Lowrie, Cowie & Conran
 Lowrie, D.J.Coates & Kenneally
+Luangsa-ard, Hywel-Jones & Spatafora
+Luangsa-ard, Hywel-Jones, Houbraken & Samson
 Ludw.
 Ludw. ex Kuntze
 Luehm.
 Luehm. ex Ewart
 Luehm. ex Maiden
 Luerss.
 Lumbsch
@@ -27953,27 +28090,27 @@
 Lumn.
 Lundb.
 Lundholm & Moestrup
 Lundholm, Moestrup & Hasle
 Lunell
 Lush.
 Luttr.
-Lutzoni, Redhead, Moncalvo & Vilgalys
 Lye
 Lyle
 Lyne
 Lyne & Crisp
 Lyngb.
 Lynge
 Lyon
 Lázaro Ibiza
+Læssøe & Spooner
+Læssøe, C.A.Pearce & K.D.Hyde
 Léman
 Lév.
 Lév. & Durieu
-Lév. & Moug.
 Löhne, Wiersema & Borsch
 Lücking
 Lücking & Aptroot
 Lücking & Barillas
 Lücking & Sipman
 Lücking & Vězda
 Lücking, Aptroot, Kalb & Elix
@@ -28000,47 +28137,51 @@
 M.A.Lawson
 M.A.M.Renner
 M.A.M.Renner & E.A.Br.
 M.A.M.Renner & Glenny
 M.A.M.Renner & P.H.Weston
 M.A.M.Renner & Pócs
 M.A.M.Renner & R.L.Barrett
+M.A.M.Renner & Towle
 M.A.M.Renner, P.H.Weston & S.Clarke
 M.A.Millar, Byrne, Nuberg & Sedgley
+M.A.Salam & P.N.Rao
 M.B.Ellis
-M.B.Ellis & E.W.Mason
-M.B.Ellis & G.W.Beaton
 M.B.MacDon. & Hotchk.
 M.B.Moss
 M.B.Scott
 M.B.Scott & Hutch.
 M.B.Thomas & W.J.McDonald
 M.B.Walters
 M.B.Williams
 M.Bartolome
 M.Bieb.
 M.Bieb. ex Willd.
 M.Brand, van den Boom & Sérus.
+M.C.Barreto, Frisvad & Samson
 M.C.Johnst.
 M.C.Williams & Lichtw.
 M.Choisy
 M.Choisy ex Scheid. & H.Mayrhofer
 M.D.Barrett
 M.D.Barrett & Craven
 M.D.Barrett & D.D.Sokoloff
 M.D.Barrett & Handasyde
 M.D.Barrett & Makinson
+M.D.Barrett & P.-L.de Kock
 M.D.Barrett & R.L.Barrett
+M.D.Barrett & S.J.Dillon
+M.D.Barrett & Spirin
+M.D.Barrett, Albr. & Fensham
 M.D.Barrett, Craven & R.L.Barrett
 M.D.Barrett, M.L.Moody & R.L.Barrett
+M.D.Barrett, R.L.Barrett & K.W.Dixon
 M.Dingley
 M.E.Barr
 M.E.Barr & E.G.Simmons
-M.E.Barr & Z.Q.Yuan
-M.E.Barr, Bathgate & B.L.Shearer
 M.E.Britton
 M.E.French & D.Nicolle
 M.E.Jansen
 M.E.Johnst. & J.H.Webber
 M.E.Lawr.
 M.E.Palm, W.Gams & Nirenberg
 M.F.Jørg. & Sh.Murray
@@ -28057,28 +28198,28 @@
 M.Gauthier ex Manier & Lichtw.
 M.Gray
 M.Gray & Given
 M.Gray & H.P.Linder
 M.Gray & P.W.Michael
 M.Greenway
 M.Guilf.
+M.H.Laurence & Summerell
+M.H.Laurence, E.C.Y.Liew, L.A.Shuttlew. & L.W.Burgess
+M.H.Laurence, Summerell & E.C.Y.Liew
 M.Harrison & Corrigan
 M.Henry
 M.Hiroe
 M.Hodgs. & R.Paine
 M.Howe
 M.J.Br.
 M.J.Cannon & Cannon
 M.J.Larsen & Zak
 M.J.Parsons
 M.J.Parsons & Womersley
-M.J.Wingf. & G.C.Adams
-M.J.Wingf. & I.Barnes
-M.J.Wingf., Slippers & J.de Wet
-M.J.Wingf., Slippers & Mohali
+M.J.Wingf., Crous & W.J.Swart
 M.J.Wynne
 M.J.Wynne & D.L.Ballant.
 M.J.Wynne & G.T.Kraft
 M.J.Wynne, A.Millar & G.T.Kraft
 M.J.Wynne, I.R.Price & D.L.Ballant.
 M.Kamiya
 M.Kamiya & R.J.King
@@ -28090,79 +28231,80 @@
 M.L.Farr
 M.L.Hicks
 M.L.Mend. & Cabioch
 M.L.Moody
 M.L.Moody & Les
 M.L.So
 M.L.Williams, Drinnan & N.G.Walsh
+M.Lange & A.H.Sm.
 M.Lebour
 M.Lefèvre
 M.Lyons & Keighery
 M.M.Moser
-M.M.Moser, E.Horak, Peintner & Vilgalys
 M.Martens & Galeotti
 M.Massey
 M.Mayrhofer
 M.McKeown, Sundue & Barrington
 M.Mizush.
 M.Morelet
+M.Niranjan & V.V.Sarma
 M.Nörpel
 M.Nörpel & Lange-Bert.
 M.Nörpel, Lange-Bert. & Alles
 M.O.P.Iyengar
 M.O.P.Iyengar & Bai
 M.O.P.Iyengar & Kanth.
 M.P.Christ.
 M.P.Christ. & Hauerslev
+M.P.S.Câmara, M.E.Palm & A.W.Ramaley
 M.P.Simmons
 M.P.Zhurbenko & U.Braun
 M.P.de Vos
 M.Piepenbr.
+M.Piepenbr. & R.Bauer
+M.Piepenbr., Begerow & Oberw.
 M.R.Schomb.
 M.Roem.
 M.Roser & H.R.Hamasha
 M.Rossignol
 M.S.Kim & I.K.Lee
 M.S.Patil
 M.Schultz, Porembski & Büdel
 M.Schultze
-M.T.Casanova & J.L.Porter
+M.Stoll, Begerow & Oberw.
 M.T.Mathieson
 M.T.Sm., Van der Walt & Johannsen
 M.Taylor
+M.Venter & M.J.Wingf.
 M.Voigt
 M.W.Chase & Christenh.
 M.W.Chase & Reveal
 M.W.Chase, Christenh. & Schuit.
 M.W.Chase, Dodsworth & Christenh.
 M.W.Chase, Kumar & Schuit.
 M.W.Chase, M.F.Fay & Christenh.
 M.W.Chase, Palsson & Christenh.
 M.W.Chase, Reveal & M.F.Fay
 M.W.Dick
-M.W.Dick & B.J.Croft
 M.W.Dick & Mark A.Spencer
-M.W.Dick & P.Wong
 M.W.Gardner
 M.W.McDonald
 M.W.McDonald & Maslin
+M.W.Mill. & J.S.F.Barker
 M.Watan., S.Suda, I.Inouye, Sawag. & Chihara
 M.Wilde & A.J.Eames
 M.Wilson, Noble & E.G.Gray
 M.van Wyk & M.J.Wingf.
 Maas Geest.
 Maasen ex Claussen
 Mabb.
-Mabb. x Hibiscus superbus C.A.Gardner
 Mabille
 MacGarvie
 MacKee
 MacLeay ex Lindl.
-MacLeay ex Lindl. x Dendrobium bowmanii Benth.
-MacLeay ex Lindl. x Dendrobium linguiforme Sw.
 MacOwan
 MacOwan ex Baker
 MacRaild & Womersley
 Macarthur & C.Moore
 Macartney
 Macfad.
 Mack. & Bush
@@ -28171,59 +28313,26 @@
 Macreight
 Maerkl.
 Maesen
 Maffei
 Magnus
 Maguire & Pires
 Maguire & Steyerm.
-Maheu & A.Gillet
+Maharachch. & K.D.Hyde
+Maharachch., K.D.Hyde & Crous
 Maheu & A.Gillett
 Maiden
 Maiden & Betche
-Maiden & Betche - Macadamia tetraphylla L.A.S.Johnson
 Maiden & Betche ex Maiden
-Maiden & Betche x Kunzea capitata subsp. seminuda Toelken
-Maiden & Betche x Kunzea obovata Byrnes
-Maiden & Betche x Kunzea parvifolia Schauer
 Maiden & Blakely
-Maiden & Blakely x Acacia citrinoviridis Tindale & Maslin
-Maiden & Blakely x Acacia pustula Maiden & Blakely
-Maiden & Blakely x Acacia rhodophloia Maslin
-Maiden & Blakely x Acacia trachycarpa E.Pritz.
-Maiden & Blakely x Acacia tumida F.Muell. ex Benth.
-Maiden & Blakely x Acacia tumida var. pilbarensis M.W.McDonald
-Maiden & Blakely x Eucalyptus gunnii Hook.f.
 Maiden & Cambage
-Maiden & Cambage - Eucalyptus persistens L.A.S.Johnson & K.D.Hill
-Maiden & Cambage - Eucalyptus populnea F.Muell.
-Maiden & Cambage x Eucalyptus crebra F.Muell.
-Maiden & Cambage x Eucalyptus drepanophylla F.Muell. ex Benth.
-Maiden & Cambage x Eucalyptus melanophloia F.Muell.
-Maiden & Cambage x Eucalyptus persistens L.A.S.Johnson & K.D.Hill
-Maiden & Cambage x Eucalyptus populnea F.Muell.
 Maiden & Camfield
 Maiden & J.M.Black
 Maiden & R.T.Baker
 Maiden ex Brooker
-Maiden x Acacia falciformis DC.
-Maiden x Acacia harpophylla F.Muell. ex Benth.
-Maiden x Acacia macradenia Benth.
-Maiden x Acacia shirleyi Maiden
-Maiden x Acacia stellaticeps Kodela, Tindale & D.Keith
-Maiden x Eucalyptus amygdalina Labill.
-Maiden x Eucalyptus citriodora Hook.
-Maiden x Eucalyptus globulus Labill.) x Eucalyptus urnigera Hook.f.
-Maiden x Eucalyptus gunnii Hook.f.
-Maiden x Eucalyptus maculata Hook.
-Maiden x Eucalyptus melanophloia F.Muell.
-Maiden x Eucalyptus microcarpa (Maiden) Maiden
-Maiden x Eucalyptus populnea F.Muell.
-Maiden x Eucalyptus relicta Hopper & Ward.-Johnson
-Maiden x Eucalyptus tereticornis Sm.
-Maiden x Eucalyptus viminalis Labill.
 Maiden, Blakely & Simmonds
 Mains
 Maire
 Maire & Duvernoy
 Maire & Malençon
 Maire, Weiller & Wilczek
 Makhija & Patw.
@@ -28234,51 +28343,55 @@
 Makinson & Albr.
 Makinson & M.D.Barrett
 Makinson & Olde
 Malajczuk & Beaton
 Malcolm & Vězda
 Malcolm, P.M.McCarthy & Kantvilas
 Malcolm, Vězda, P.M.McCarthy & Kantvilas
-Malencon
 Malençon
 Malençon & Bertault
+Malençon & R.Heim
 Mallinson
 Malloch & Cain
 Malloch & Salkin
 Malme
 Malmsten
-Maloch & Cain
 Malta
+Manamgoda, L.Cai & K.D.Hyde
+Mancini & Sacc.
 Mangold
 Mangold & Lumbsch
 Mangold, Elix & Lumbsch
 Mangold, Lücking & Lumbsch
 Manguin
 Manguin ex Kociolek & Reviers
 Manier & F.Coste
 Manier, Rioux & Whisler
 Manier, Rioux & Whisler ex Manier, Rioux & Whisler
 Maniotis
+Manjón & G.Moreno
 Mansf.
 Mantell
+Mapook & K.D.Hyde
+Mapperson, Bransgr., R.G.Shivas & Dearnaley
 Marais
-Marasas, P.E.Nelson & Rheeder
-Marasas, P.S.van Wyk & Knox-Dav.
-Marasas, P.S.van Wyk, P.E.Nelson & Toussoun
+Marasas, P.E.Nelson, Toussoun & P.S.van Wyk
 Marasas, Rheeder, Lampr., K.A.Zeller & J.F.Leslie
 Maratti
 Marbach
 Marbach & Kalb
 Marc.-Berti
+Marcelino & Gouli
 Marchal
 Marchand
 Marginson & Ladiges
 Marignoni
 Markgr.
 Marloth
+Marney
 Marnock
 Marohasy & P.I.Forst.
 Marquand
 Marquis
 Marr
 Marr & D.E.Stuntz
 Marriott & G.W.Carr
@@ -28299,14 +28412,15 @@
 Mart. ex Thell.
 Mart.Schmidt
 Martelli
 Martine
 Martine & Frawley
 Martine & J.Cantley
 Martine & McDonnell
+Martine & T.M.Williams
 Martine, J.Cantley & L.M.Lacey
 Martinez
 Martinov
 Martyn
 Marvanová
 Marvanová & S.H.Iqbal
 Maréchal, Mascherpa & Stainier
@@ -28321,18 +28435,14 @@
 Maslin & Cowie
 Maslin & D.J.Murphy
 Maslin & J.E.Reid
 Maslin & L.A.J.Thomson
 Maslin & M.W.McDonald
 Maslin & R.L.Barrett
 Maslin & Whibley
-Maslin x Acacia bivenosa DC.
-Maslin x Acacia pyrifolia DC.
-Maslin x Acacia sclerosperma F.Muell.
-Maslin x Acacia sibirica S.Moore
 Maslin, M.D.Barrett & R.L.Barrett
 Massart
 Massee
 Massee & Crossl.
 Massee & E.S.Salmon
 Massee & Rodway
 Massee ex Cheel
@@ -28341,16 +28451,27 @@
 Massee ex W.B.Cooke
 Massey
 Masson
 Mast.
 Mast. & Linden
 Matheny
 Matheny & Bougher
+Matheny & Bougher ex Bougher & Matheny
+Matheny & Esteve-Rav.
+Matheny & Watling
 Matheny, Bougher & G.M.Gates
+Matheny, Bougher & Halling
+Matheny, Bougher & Lepp
 Matheny, Bougher & M.D.Barrett
+Matheny, Bougher & Ryberg
+Matheny, Bougher, R.Rob. & K.Syme
+Matheny, O.K.Mill. & Bougher
+Matheny, O.K.Mill. & Bougher ex Matheny, O.K.Mill. & Bougher
+Matheny, Trappe & Bougher
+Matheny, Trappe & Bougher ex Matheny, Trappe & Bougher
 Mathias & Constance
 Maton
 Matr.
 Matsum.
 Matsuoka, Sa.Kobay. & G.Gains
 Matsush.
 Mattei
@@ -28375,57 +28496,62 @@
 Maxim. ex Meinh.
 Maxon
 Mayer
 Maynard & Crayn
 Mayor
 Mayrhofer & Sheard
 Mazel ex J.Houz.
-McAlpin
+Mazzer
+Mazzer & A.H.Sm.
 McAlpine
 McAlpine & Tepper
 McAlpine ex Hansf.
 McAulay & Brett
 McCalla ex Harv.
 McClain
 McClure ex Soderstr.
 McComb
 McDermid
 McGee
 McGee & A.Cooper
 McGee & Pattinson
 McGill.
+McGinnis & Ajello
 McGinnis & Schell
-McGinnis & W.Gams
+McGinty
 McGurk, E.M.Davison & E.L.J.Watkin
 McKenzie
 McKenzie & D.Matthews
-McKenzie & Vánky
 McKibbin
 McKinney
+McLay & Albr.
 McLay & S.J.Dillon
 McLennan
 McLennan & Cookson
 McLennan & Ducker
 McLennan & F.Halsey
 McLennan & Hoëtte
+McMull.-Fish., T.Lebel & Senn-Irlet
 McNabb
 McQuoid & Hopper
 McQuoid & M.E.French
 McTaggart & R.G.Shivas
 McTaggart, R.G.Shivas & U.Braun
 McTaggart, Y.Ono, Berndt & R.G.Shivas
 Me.Lemoine
 Meagher
+Meagher & Cairns
 Meagher & Pócs
 Medik.
 Medlar
 Medlin
 Meerb.
 Meeuwen
 Meffert
+Meier, Drechsler & E.D.Eddy
 Meijden
 Meikle
 Meikle & Hewson
 Meinsh.
 Meisn.
 Meisn. ex Benth.
 Meisn. ex Regel
@@ -28447,18 +28573,20 @@
 Menegh. ex Ralfs
 Menegh. ex de Bary
 Meney & K.W.Dixon
 Meney & K.W.Dixon ex R.L.Barrett
 Meney & Pate
 Meney, K.W.Dixon & Pate
 Menge
+Menkins
 Menzies ex Hook.
 Menzies ex Lindenb.
 Merat
-Mercado & Hol.-Jech.
+Mercado
+Mercado & R.F.Castañeda
 Meredith
 Mereschk.
 Merr.
 Merr. & L.M.Perry
 Merr. & Rolfe
 Merr. ex Moldenke
 Mert.
@@ -28467,46 +28595,48 @@
 Mert. ex C.Agardh
 Mert. ex Gomont
 Mert. ex Roth
 Mert. ex Turner
 Messik.
 Messina
 Messmer
-Messmer x Pterostylis baptistii Fitzg.
 Mett.
 Mett. ex A.B.Frank
 Mett. ex F.M.Bailey
 Mett. ex Kuhn
 Mett. ex Prantl
 Meunier
 Meve & Liede
 Meyen
 Meyen & Flot.
 Meyen & Walp.
 Meyen ex E.C.Hansen
 Meyen ex Ralfs
 Meyers
+Meyers & Kohlm.
 Meyers & R.T.Moore
-Meyers, Orpurt, Boral & Simms
 Meyl.
 Mez
 Mhaskar & V.G.Rao
 Mich.
 Mich.J.Parsons
 Michaelis
 Micheli
 Micheli ex Raddi
 Michx.
+Michx. ex Adans.
 Michx. ex DC.
 Mieg
 Miers
 Miers ex Bureau
 Miers ex Hook.f. & Thomson
+Miettinen
 Miettinen & K.H.Larss.
 Miettinen & Rajchenb.
+Miettinen & Spirin
 Mig.
 Migl. & Coccia
 Mihaich
 Miki
 Mildbr.
 Mildbr. & Burret
 Milde
@@ -28518,55 +28648,55 @@
 Millan
 Millardet
 Millott & K.L.McDougall
 Millsp.
 Milne & Cargill
 Min-Thein & Womersley
 Minden
+Minnis & D.L.Lindner
 Minoura & T.Muroi
 Minoura, Morinaga & T.Muroi
 Minter
 Minter & B.C.Zhang
 Miq.
-Miq. - Macrozamia mountperriensis F.M.Bailey
 Miq. ex Bartl.
 Miq. ex Gagnep.
-Miq. x Casuarina glauca Sieber ex Spreng.
 Mirb.
 Mirb. ex Bercht. & J.Presl
 Mirb. ex DC.
 Mishra
 Mitch.
 Mitford
 Mitra
 Mitt.
 Mitt. ex Burges
 Mitt. ex Cardot
 Mitt. ex Dixon
 Mitt. ex Dozy & Molk.
 Mitt. ex F.Muell.
 Mitt. ex Geh.
-Mitt. ex Hampe
 Mitt. ex Hardy
 Mitt. ex Hook.f.
-Mitt. ex M.Fleisch.
 Mitt. ex Paris
 Mitt. ex Steph.
 Mitt. ex Watts & Whitel.
 Mitt. ex Wijk, Margad. & Florsch.
 Miura
 Miyabe
 Miyake
+Miyake & Komin. ex M.Oda
 Mizut.
 Moberg
 Moberg & Purvis
+Moc. & Sessé ex DC.
 Moebius
 Moench
 Moestrup, Hakanen, Gert Hansen, Daugbjerg & M.Ellegaard
 Moezel
+Mohali, Slippers & M.J.Wingf.
 Mohamed
 Mohamed & Damanhuri
 Mohlenbr.
 Mohlo, Bodo, W.L.Culb. & C.F.Culb.
 Mohr
 Moldenke
 Molero & Monts.
@@ -28575,31 +28705,28 @@
 Molloy, D.L.Jones & M.A.Clem.
 Molyneux
 Molyneux & Forrester
 Molyneux & Olde
 Molyneux & Rule
 Molyneux & Stajsic
 Monach.
-Monach. x Alstonia spectabilis R.Br.
 Monks & A.K.Mills
 Mont.
 Mont. & Berk.
 Mont. & Bory
 Mont. & Bosch
 Mont. & C.P.Robin
 Mont. & Desm.
 Mont. & Durieu
 Mont. & Fr.
-Mont. & Lepr.
 Mont. & Millardet
 Mont. & Nees
 Mont. ex Gomont
 Mont. ex Kütz.
 Mont. ex Lehm.
-Mont. ex Okamura
 Mont. ex Steph.
 Montin
 Montressor, Procaccani & Stoecker
 Montrouz.
 Moodie
 Moon
 Moore
@@ -28607,49 +28734,51 @@
 Moore ex Ralfs
 Moq.
 Moq. ex Benth.
 Morat
 Mordue
 Moreau & R.Moreau ex W.Gams
 Morelet
-Morelet x Pinus elliottii Engelm.
 Moretti
 Morgado, G.M.Gates & Noordel.
 Morgan
 Morgan-Jones
 Morgan-Jones & J.F.White
 Morgan-Jones & W.Gams
 Moris
 Moris & De Not.
+Moriwaki, Toy.Sato & Tsukib.
 Morong
 Morren
 Morrison
 Moss
 Moss ex Fourc.
+Mossebo & Ambit
+Mostowf. & T.I.Burgess
 Mosyakin
 Motyka
-Mouch. & W.Gams
 Moug.
+Moug. & Lév.
 Mouill.
-Mrak & Recca
 Mrozińska
 Muasya & D.A.Simpson
 Mudie
 Muehlenpf.
+Mugambi & Huhndorf
 Muhl.
 Muhl. ex Elliott
 Muhl. ex Willd.
-Mukerji & T.N.Lakh.
 Mull.Frib.
 Mull.Frib. & Herzog
 Mull.Frib. ex Fulford & Hatcher
 Mull.Frib. ex Grolle
 Mun.-Chalm.
 Mundk.
 Mundk. & Khesw.
+Mundk. & Thirum.
 Munir
 Munk
 Munro
 Munro ex Hook.f.
 Munt.-Cvetk.
 Munz
 Murb.
@@ -28658,14 +28787,15 @@
 Murr & Thell.
 Murray
 Murray ex G.Forst.
 Murrill
 Muschl.
 Musili & J.J.Bruhl
 Muss.Puschk. ex Willd.
+Muthumary, Abbas & B.Sutton
 Mutis ex L.
 Mutis ex L.f.
 Myint
 Myint & D.B.Ward
 Métrod
 Möller
 Møller
@@ -28676,15 +28806,14 @@
 Müll.Hal.
 Müll.Hal. & Broth.
 Müll.Hal. & Hampe
 Müll.Hal. & Hampe ex Paris
 Müll.Hal. & Kindb.
 Müll.Hal. & Warnst.
 Müll.Hal. ex A.Jaeger
-Müll.Hal. ex Berthier
 Müll.Hal. ex Besch.
 Müll.Hal. ex Bosch & Sande Lac.
 Müll.Hal. ex Broth.
 Müll.Hal. ex Burges
 Müll.Hal. ex C.C.S.Clarke
 Müll.Hal. ex Cardot
 Müll.Hal. ex Dixon
@@ -28701,29 +28830,29 @@
 Müll.Hal. ex Mitt.
 Müll.Hal. ex Paris
 Müll.Hal. ex Rodway
 Müll.Hal. ex Schlieph. & Geh.
 Müll.Hal. ex Stirl.
 Müll.Hal. ex Tadgell
 Müll.Hal. ex Thér.
-Müll.Hal. ex Venturi
 Müll.Hal. ex W.Forsyth
 Müll.Hal. ex Warnst.
 Müll.Hal. ex Watts
 Müll.Hal. ex Watts & Whitel.
 Müll.Hal. ex Weymouth
 Müll.bis ex Hollós
 Münchh.
 N'Yeurt
 N.A.Brummitt & Utteridge
 N.A.Fechner & Halling
+N.A.Fechner, Bonito, T.Lebel & Halling
+N.A.Fechner, Bougher, Bonito & Halling
 N.A.Fechner, K.Syme, R.Rob., & Halling
 N.A.Goldberg & Huisman
 N.A.Wakef.
-N.A.Wakef. x Hypolepis rugosula (Labill.) J.Sm.
 N.C.Duke
 N.C.Duke & Hidet.Kudo
 N.C.W.Beadle
 N.C.W.Beadle, O.D.Evans & Carolin
 N.Carter
 N.E.Bell, A.E.Newton & D.Quandt
 N.E.Br.
@@ -28746,14 +28875,15 @@
 N.Gibson & Wege
 N.H.F.Desp.
 N.Hall
 N.Hallé
 N.Hoffman & A.P.Br.
 N.Holtze
 N.Jacques, S.Mallet & Casarég.
+N.K.Rao, Manohar. & Goos
 N.Kitag.
 N.Kitag. & Grolle
 N.L.Gardner
 N.Lundq.
 N.P.Balakr.
 N.P.Barker & H.P.Linder
 N.Pedersen
@@ -28766,49 +28896,53 @@
 N.Snow & Guymer
 N.Snow & J.Cantley
 N.Snow & J.McFadden
 N.Snow & J.P.Atwood
 N.Streiber & B.J.Conn
 N.T.Burb.
 N.T.Burb. & M.Gray
+N.T.Tran, Geering, Y.P.Tan & R.G.Shivas
 N.W.Simmonds
 N.Walters
 NE Herbarium
 NSW Herbarium
 NT Herbarium
 Na-Thalang
 Naccari
 Nadeaud
 Naeg.
 Nag Raj
+Nag Raj & W.B.Kendr.
+Nag Raj, DiCosmo & W.B.Kendr.
+Nagao, Udagawa & Bougher
 Nagarkar, Sethy & Patw.
 Nageli & Peter
+Najafz., V.A.Vicente, J.F.Sun, Meis & de Hoog
 Nakagiri & Tokura
 Nakai
 Nakai & Momose
 Nakai ex Doweld
 Nakai ex Reveal
 Nakai ex Tuyama
 Nakasone
 Nakasone & D.L.Lindner
-Nakasone, Rajchenb. & Gresl.
-Nan.-Bremek. & Y.Yamam.
+Nalim, Samuels & Geiser
 Nann.
 Nann.-Bremek.
 Nann.-Bremek. & D.W.Mitch.
-Nann.-Bremek. & Ing
 Nann.-Bremek. & Y.Yamam.
 Nann.-Bremek. ex Ing
 Nann.-Bremek., D.W.Mitch., T.N.Lakh. & R.K.Chopra
-Nann.-Bremek., Y.Yamam. & R.Sharma
+Nann.-Bremek., R.Sharma & Y.Yamam.
 Nannf.
 Nannf. & Korf
 Nardo
 Nash
 Nasr
+Natarajan & Raman
 Naudin
 Naudin ex Maiden
 Naumann
 Naurois & Roux
 Nav.-Ros. & Hafellner
 Navas
 Naveau
@@ -28834,15 +28968,14 @@
 Nees & Flot.
 Nees & Gottsche ex Lehm.
 Nees & Hornsch.
 Nees & Lindenb.
 Nees & Mart.
 Nees & Meyen
 Nees & Meyen ex Kunth
-Nees & Meyen ex Nees
 Nees & Meyen ex Wight
 Nees & Mont.
 Nees & T.Nees
 Nees ex B.D.Jacks.
 Nees ex Bartl.
 Nees ex Benth.
 Nees ex C.B.Clarke
@@ -28872,52 +29005,54 @@
 Neumann
 Nevski
 Newbigin & P.M.Waterh.
 Newman
 Newnham, Ladiges & Whiffin
 Nge & K.R.Thiele
 Nge & Keighery
+Ngugi
 Nicholls
 Nicholls & Goadby
-Nicholls x Caladenia pectinata R.S.Rogers
-Nicholls x Caladenia serotina Hopper & A.P.Br.
 Nickrent & Der
 Nickrent & Vidal-Russell
 Nicolson
 Nicolson & Sivad.
 Nicot
 Nied.
 Nielsen
 Niemelä
 Niessl
 Nieuwl.
 Night.
 Nikolaev
+Nimmo
 Nirenberg
+Nirenberg & O'Donnell
+Nirenberg & Samuels
 Nishih., Tsuda & Ueyama
 Nishim. & Miyaji
+Niskanen & Liimat.
 Nitschke
 Nitschke ex Arnold
 Nitschke ex Fuckel
-Nitschke ex G.Winter
 Nitzsch
 Nitzsch ex Ralfs
 Nizam.
 Nizam. & Womersley
 Nobles
 Nog.
 Nog. & Z.Iwats.
 Nois.
 Nois. ex Henkel & Hochst.
 Nois. ex Steud.
 Noordel.
 Noordel. & Co-David
+Noordel. & G.M.Gates
 Noordel. & Hauskn.
 Noordel., D.L.V.Co, G.M.Gates & Morgado
-Noordel., G.M.Gates & B.M.Horton
 Noot.
 Nordst.
 Nordst. & Hirn
 Nordst. ex De Toni
 Nordst. ex F.M.Bailey
 Nordst. ex Hirn
 Norl.
@@ -28928,35 +29063,34 @@
 Norstedt
 Noter
 Novak
 Novak ex Reveal
 Novak ex Takht.
 Nowak.
 Nubl.
+Nuhn, Manfr.Binder, A.F.S.Taylor, Halling & Hibbett
 Nuno
 Nutt.
 Nutt. ex Torr. & A.Gray
 Nygaard
 Nyl.
 Nyl. ex C.Bab. & Mitt.
 Nyl. ex Cromb.
 Nyl. ex Hue
 Nyl. ex Kremp.
 Nyl. ex Leight.
 Nyl. ex Müll.Arg.
-Nyl. ex Nyl.
 Nyl. ex Vain.
 Nyman
 Nádv.
 Nägeli
 Nägeli ex A.Braun
 Nägeli ex Bornet & Flahault
 Nägeli ex Kütz.
 O'Brien
-O'Donnell & Nirenberg
 O'Donnell, T.Aoki, Kistler & Geiser
 O'Gara
 O'Gorman, H.T.Fuller & P.S.Dyer
 O'Kelly ex R.W.Ricker
 O'Leary
 O'Leary & Maslin
 O'Meara
@@ -28975,14 +29109,15 @@
 O.F.Cook
 O.F.Cook & Doyle
 O.F.Müll.
 O.F.Müll. ex Vahl
 O.H.Sarg.
 O.Hoffm.
 O.K.Mill.
+O.K.Mill. & E.Horak
 O.K.Mill. & R.N.Hilton
 O.K.Mill., Hemmes & G.Wong
 O.Müll.
 O.Nazarova & Hislop
 O.Nilsson
 O.Prakash & A.P.Misra
 O.Rostr.
@@ -28992,19 +29127,21 @@
 O.Zacharias
 Obbens
 Obbens & J.G.West
 Obbens & L.P.Hancock
 Oberm.
 Obermayer
 Oberw.
+Oberw. & B.Metzler
 Oberw. & Bandoni
 Oberw. ex Parmasto
 Obrist
 Ochi
 Ochyra
+Ochyra & Seppelt
 Oeder
 Oerst.
 Oerst. ex Gomont
 Ohlend.
 Ohlsson
 Ohlsson ex Tibell
 Ohno
@@ -29012,122 +29149,126 @@
 Ohwi
 Ohwi & Yabuno
 Okamura
 Okamura & Nishikawa
 Okamura & Segawa
 Oken
 Okolodkov
+Oktalira, T.W.May & Linde
 Okuno
 Old & Z.Q.Yuan
 Olde
+Olde & Keighery
 Olde & Marriott
 Olde & Molyneux
 Oldfield & F.Muell.
-Oldfield & F.Muell. ex F.Muell.
 Oliv.
 Oliv. ex Benth.
 Olive
 Olliff
+Olliver & G.Sm.
+Oltra, G.Moreno & Illana
 Omvik
 Ooststr.
 Opat.
 Opiz
 Opiz ex L.Junell
 Orange
 Orange & Wolseley
 Orb.
 Orchard
 Orchard & J.B.Davies
 Orme & Duretto
 Ormerod
 Ornduff
+Orpurt, Meyers, Boral & Simms
 Orr
 Ortega
 Orthia
 Orthia & Chappill
 Orthia & Crisp
 Osbeck
 Oshio
 Ostaz.
 Ostenf.
 Ostenf. & E.J.Schmidt
-Osth. & P.James
 Ottaviani ex Badham
 Otto
 Otto & A.Dietr.
 Otto ex Rchb.
 Otto ex Walp.
 Oudem.
 Oudem. & Beij.
 Overeem
 Overh. & J.Lowe
 Overton
+O’Donnell, T.Aoki, Jacq.Edwards & Summerell
 O’Meara
+O’Rourke, M.H.Ryan, Hua Li, X.Ma, Sivasith., Fatehi & Barbetti
 P.A.Archibald
 P.A.Archibald & H.C.Bold
 P.A.Barber & Crous
 P.A.Butcher, M.W.McDonald & J.C.Bell
 P.A.Collier
 P.A.Dang.
 P.A.Gilbert
 P.A.Lemke
 P.A.Sims
+P.A.Sims & D.M.Williams
 P.A.Tandy
 P.A.Taylor, Pascoe & F.C.Greenh.
 P.A.Will.
 P.Archibald
 P.Baker
 P.Beauv.
-P.Beauv. ex Brid.
 P.Beauv. ex Mirb.
 P.Beauv. ex Nees
 P.Beauv. ex Roem. & Schult.
 P.Beauv. ex Steph.
 P.Beauv. ex T.Lestib.
 P.Bernhardt
 P.Browne
 P.Browne ex Gaertn.
 P.Browne ex L.
 P.C.Boyce & Bogner
 P.C.Chen
 P.C.Kao
 P.C.Misra
+P.C.Misra & P.H.B.Talbot
 P.C.Misra, K.J.Srivast. & Lata
 P.C.Reid
 P.C.Silva
 P.C.Silva & DeCew
 P.C.Silva & Womersley
 P.C.Silva, Chacana & Womersley
 P.C.Silva, K.Mattox & W.Blackwell
 P.C.Silva, Maggs & L.M.Irvine
 P.C.Tsoong
 P.Candargy
-P.Chaverri & Salgado
+P.Chaverri & C.G.Salgado
+P.Correia, E.Azevedo & M.F.Caeiro
 P.Crouan & H.Crouan
 P.D.Orton
 P.Delanoë & Delanoë
 P.Döbbeler
 P.Döbbeler, Poelt & Vězda
 P.E.Lim & H.Kawai
 P.E.Nelson & S.Wilh.
-P.E.Nelson, L.W.Burgess & Toussoun
+P.E.Nelson, Toussoun & L.W.Burgess
 P.E.S.Chr.
 P.F.Cannon
 P.F.Cannon & Alcorn
-P.F.Cannon & K.D.Hyde
 P.F.Horsfall & G.W.Carr
 P.F.Hunt & Summerh.
 P.F.Stevens
 P.Fourn.
 P.G.Neish
 P.G.Parkinson
 P.G.Richt.
 P.H.B.Talbot
-P.H.B.Talbot & P.C.Misra
-P.H.B.Talbot & Warcup
 P.H.Campb.
 P.H.Campbell
 P.H.Raven
 P.H.Raven & Engelhorn
 P.H.Weston
 P.H.Weston & A.R.Mast
 P.H.Weston & Crisp
@@ -29137,15 +29278,14 @@
 P.H.Weston & M.J.Turton
 P.H.Weston & N.P.Barker
 P.Horton
 P.I.Forst.
 P.I.Forst. & A.J.Paton
 P.I.Forst. & B.Gray
 P.I.Forst. & D.L.Jones
-P.I.Forst. & D.L.Jones - Macrozamia macleayi Miq.
 P.I.Forst. & E.J.Thomps.
 P.I.Forst. & Liddle
 P.I.Forst. & R.J.F.Hend.
 P.I.Forst. & Thongp.
 P.I.Forst., Liddle & I.M.Liddle
 P.J.Anderson
 P.J.Bergius
@@ -29154,40 +29294,43 @@
 P.J.Lang
 P.J.Lang & Brooker
 P.J.Lang & Maslin
 P.J.Lang & R.S.Cowan
 P.J.Mull. ex Boulay
 P.J.Mull. ex Genev.
 P.J.Sm.
+P.J.Wright
 P.James
 P.James & D.J.Galloway
 P.James & Henssen
 P.James & Kantvilas
 P.James & Kilias
 P.James & Vězda
 P.K.Buchanan
-P.K.Buchanan & Rajchenb.
 P.K.Buchanan & Ryvarden
 P.K.Endress, B.Hyland & Tracey
 P.Karst.
 P.Karst. & Har.
+P.Karst. & Roum.
 P.Kumm.
 P.L.J.Dang.
 P.Lawson & C.Lawson
+P.Leonard
+P.Leonard & Dearnaley
+P.Leonard & McMull.-Fish.
 P.Lewis & Summerh.
 P.Lundell
 P.M.Jørg.
 P.M.Jørg. & Aptroot
 P.M.Jørg. & D.J.Galloway
 P.M.Jørg. & Kantvilas
 P.M.Jørg. & P.James
 P.M.Jørg. & R.S.Poulsen
 P.M.Jørg. & Vězda
 P.M.Kirk
-P.M.Kirk & Alcorn
 P.M.Kirk & B.Sutton
 P.M.McCarthy
 P.M.McCarthy & Elix
 P.M.McCarthy & Filson
 P.M.McCarthy & Kantvilas
 P.M.McCarthy & Lücking
 P.M.McCarthy & P.N.Johnson
@@ -29200,68 +29343,73 @@
 P.M.Peterson
 P.M.Peterson & N.Snow
 P.M.Peterson & Romasch.
 P.M.Peterson, Romasch. & R.L.Barrett
 P.M.Scott & T.Jung
 P.M.Sm.
 P.M.Wells & R.S.Hill
+P.M.Will., Highet, W.Gams & Sivasith.
 P.Mann
 P.Metzner
 P.Micheli
 P.Micheli ex Adans.
 P.Micheli ex F.H.Wigg.
 P.Micheli ex Fr.
 P.Micheli ex Kuntze
 P.Micheli ex L.
 P.Micheli ex Link
 P.Micheli ex Pers.
 P.Morris
 P.N.Don
-P.N.Rao & M.A.Salam
 P.Palau
 P.Parm.
 P.Petit
 P.R.Alvarez & Duretto
 P.R.Johnst.
+P.R.Johnst., Baral & R.Galán
 P.Reinecke
 P.Roberts
 P.Royen
 P.Royen & Airy Shaw
 P.S.Catches. & D.E.A.Catches.
 P.S.Catches. & T.Lebel
+P.S.Catches., Vonow & D.E.A.Catches.
+P.S.Câmara
 P.S.Dixon
 P.S.Green
-P.S.Green ex I.Hutton
-P.S.Green x Jasminum simplicifolium subsp. suavissimum (Lindl.) P.S.Green
-P.S.Green x Jasminum suavissimum Lindl.
 P.S.Short
 P.S.Short & Hosking
 P.S.Short & Paul G.Wilson
 P.S.Short & Watan.
 P.S.Short, D.E.Albr., Cowie, D.L.Lewis & B.M.Stuckey
 P.S.Short, D.J.Dixon & Osterkamp Madsen
+P.S.van Wyk, Marasas & Knox-Dav.
 P.Sebastian & I.Telford
 P.Syd.
-P.Syd. & Sacc.
 P.Syd. & Syd.
 P.Syd. & Theiss.
 P.Taylor
 P.V.Heath
 P.W.Gabrielson & G.T.Kraft
 P.W.Michael
 P.W.Michael & Vickery
-P.W.Michael x Verbena litoralis Kunth
 P.Willemet
 P.Wong
 P.Wong & A.M.Stirling
+P.Wong & C.Dong
 P.Wong & M.L.Dickinson
+P.Wong & M.W.Dick
 P.Wong, Khemmuk & R.G.Shivas
 P.Wong, Y.P.Tan & R.G.Shivas
+P.Wong, Y.P.Tan, T.L.Weese & R.G.Shivas
 P.de la Varde
+Paap
+Paap & T.I.Burgess
 Paczk. & A.R.Chapm.
+Padwick
 Page
 Paine
 Pal
 Pall.
 Pall. ex Willd.
 Palla
 Palla ex Kneuck.
@@ -29275,15 +29423,14 @@
 Pant.
 Pantocsek
 Panz.
 Pančić ex A.Kern.
 Papendorf
 Papenf.
 Parbery
-Parbery & A.R.Paul
 Paris
 Paris & Broth.
 Paris & Schimp. ex Broth.
 Paris ex Dixon
 Parish ex Ridl.
 Parke
 Parke & D.Ballant.
@@ -29299,123 +29446,107 @@
 Parr-Sm.
 Parra-Os. & Ladiges
 Parris
 Partr. & Morgan-Jones
 Pascher
 Pascher & Jahoda
 Pascher & Ruttner
-Pascoe & Beilharz
 Pascoe & Crous
-Pascoe, Beilharz & Cunningt.
-Pascoe, Beilharz & Mayers
-Pascoe, Beilharz & Parbery
 Pasq.
 Pass.
+Pass. & Thüm.
 Pat.
-Pat. & Boud.
-Pat. & Bres.
 Pat. & C.F.Baker
 Pat. & Gaillard
 Pat. & Har.
-Pat. & L.Mangin
 Pat. & Lagerh.
 Pat. & Trab.
 Pate & Meney
 Paton
+Patricia McGee & Pascoe
 Patt.
 Patw. & Kulkarni
 Pau
 Paul G.Wilson
 Paul G.Wilson & M.A.Wilson
-Paul G.Wilson x Tegicornia uniflora Paul G.Wilson
 Paulet
 Paulsen
 Pauquy
 Paust
 Pav. ex Juss.
 Pav. ex Lindl.
 Pavgi
 Pavgi & Mundk.
 Pavill.
 Pavlic, T.I.Burgess & M.J.Wingf.
-Pavlic, T.I.Burgess, M.J.Wingf.
 Pax
 Pax & K.Hoffm.
 Paxton
-Paxton x Jasminum didymum subsp. racemosum (F.Muell.) P.S.Green
+Payak & Thirum.
 Payer
 Pazschke ex Henn.
 Pearson
+Peart & Y.P.Tan
+Peart, Anth.J.Young, S.Campbell & Y.P.Tan
 Peck
 Peck & Frost
 Peck ex V.S.White
 Pedley
 Pedley & Maslin
 Pedley & P.I.Forst.
-Pedley - Acacia fodinalis Pedley
-Pedley - Acacia leiocalyx (Domin) Pedley
 Pedley ex K.L.Gibbons
 Pedley ex Lithgow
 Pedley ex Maesen
 Pedley ex R.Butcher
-Pedley var. adoxa x Acacia spondylophylla F.Muell.
-Pedley x Acacia fodinalis Pedley
-Pedley x Acacia leiocalyx (Domin) Pedley
-Pedley x Acacia leptocarpa A.Cunn. ex Benth.
-Pedley x Acacia polystachya A.Cunn. ex Benth.
-Pedley x Acacia spirorbis Labill.
 Pegg & Alcorn
 Pegler
-Pegler & Holland
 Pegler & Lodge
 Peglion
 Peintner
 Peintner & M.M.Moser
+Peintner, E.Horak, M.M.Moser & Vilgalys
 Pellegr.
 Pellow & J.L.Porter
 Pellow, Henwood & Carolin
 Penard
 Pennant
 Pennell
 Pennycook & Samuels
 Penrose
 Penz.
 Penz. & Sacc.
 Perag.
 Perag. & Brun
 Perag. & Hérib.
+Percy-Bower & C.M.Parker
 Perest.
 Perkins
 Perleb
 Perman
 Perr.
 Perrie, D.J.Ohlsen & Brownsey
 Perrine
 Pers.
-Pers. : Fr.
-Pers. : Pers.
 Pers. ex Bercht. & J.Presl
 Pers. ex Berk.
 Pers. ex Cass.
 Pers. ex Hook.
 Pers. ex J.F.Gmel.
 Pers. ex Lév.
 Pers. ex Pat.
-Pers. ex Pers.
 Pers. ex Schleich.
 Pers. ex Steud.
 Persiel
 Perss.
 Perty
 Pesante
 Pescott
 Pescott & Nicholls
 Petagna
 Petch
-Petch & G.Lister
 Peter B.Adams
 Peter B.Adams, Jac.M.Burke & S.D.Lawson
 Peter B.Adams, S.D.Lawson & G.A.Paterson
 Peter G.Wilson
 Peter G.Wilson & B.Hyland
 Peter G.Wilson & J.T.Waterh.
 Peter G.Wilson & M.L.Moody
@@ -29425,33 +29556,32 @@
 Peterm.
 Peters
 Petersen
 Peterson, Varga & Samson
 Pethybr.
 Petit
 Petr.
-Petr. & Bremer
 Petr. & Cif.
 Petr. & Syd.
 Petri
 Petrie
 Petrovič
 Peyr.
 Peyronel
 Pfeiff.
 Pfitzer
 Phaff, Mrak & O.B.Williams
-Phaff, Starmer, Ganter & Lachance
 Phan, L.W.Burgess & Summerell
 Phil.
 Phil.Moore
 Philcox
 Philib.
 Philipson
 Philipson & Skipw.
+Phookamsak & K.D.Hyde
 Pic.Serm.
 Pic.Serm. ex Reveal
 Picc.
 Picc. & Grunow
 Pichon
 Pidopl.
 Pierre
@@ -29466,39 +29596,41 @@
 Pilát
 Pilát & Dermek
 Pilát ex Pilát
 Pinoy
 Piper
 Pire
 Piroz.
+Piroz. & Hodges
 Piroz. & Ichinoe
 Piroz. & S.D.Patil
 Pit.
 Pit. & Proust
 Pitschm.
 Pitt
-Pitt & K.Ando
+Pitt & A.D.Hocking
 Pittier
+Piątek & R.G.Shivas
 Plakidas & Edgerton ex Crane
 Plakidas & Edgerton ex J.L.Crane
 Planch.
 Planch. ex F.Muell.
 Planch. ex Gray
 Planch. ex Miq.
 Planch. ex Walp.
 Playfair
 Plenck
 Plowr.
+Plowr. & G.Winter
 Plum. ex L.
 Pochm.
 Podger & Chippend.
 Podp.
 Poelln.
 Poelt
-Poelt ex Elix
 Poetsch
 Pohl
 Poir.
 Poir. ex Lam.
 Poit.
 Pojark.
 Pole-Evans
@@ -29519,41 +29651,43 @@
 Pourr. ex Lag.
 Pourr. ex Lam.
 Pourr. ex Lapeyr.
 Pouzar
 Powell
 Prain
 Prantl
+Prasannath, Akinsanmi & R.G.Shivas
 Prassler
 Preisig
 Preisig & D.J.Hibberd
 Preisig & Hibberd
 Preiss ex Meisn.
 Preiss ex Schauer
 Prent.
 Prescott
 Prescott & A.M.Scott
 Prestoe
 Preuss
 Priest
 Priest & M.Lenz
-Priest & U.Braun
+Prihast., L.Cai & K.D.Hyde
 Prill. & Delacr.
 Prillinger, Lopandic & Sugita
 Pringsh.
 Pringsh. ex Hirn
 Printz
 Printzen
 Printzen & Kantvilas
 Probst
 Probst & Thell.
 Prokh.
 Prosk.
 Prowse
 Prud'homme & Lokhorst
+Prychid & J.J.Bruhl
 Pugsley
 Puiss.
 Pujals
 Punith.
 Purchas & Ley
 Pursh
 Purss
@@ -29561,62 +29695,68 @@
 Putt.
 Puttock
 Puttock & D.J.Ohlsen
 Puttock ex de Salas & Schmidt-Leb.
 Puymaly
 Pyck
 Pépin
+Pérez-Ort. & Etayo
 Pérez-Ortega & Etayo
 Pérez-Ortega & Kantvilas
 Pócs
 Pócs & Cairns
 Pócs & Ninh
 Pócs ex L.Söderstr. & A.Hagborg
+Q.Chen, Crous & L.Cai
+Q.M.Wang & F.Y.Bai
+Q.M.Wang, F.Y.Bai, M.Groenew. & Boekhout
+Qian Chen & L.Cai
 Qld Herbarium
 Quaedvl. & Crous
-Quel.
+Quaedvl., Carnegie & Crous
+Quaedvl., Summerell & Crous
+Quaedvl., Verkley & Crous
 Quinn
 Quél.
 Quél. ex Boud.
 Quél. ex P.Karst.
 R.A.Black
 R.A.Braune
 R.A.Dyer
+R.A.Eaton & E.B.G.Jones
 R.A.Howard
 R.A.Kerrigan
 R.A.Kerrigan & Albr.
+R.A.Krause & R.K.Webster
 R.A.Meissn.
 R.A.Meissn. & Rathbone
 R.A.Paterson
 R.A.Poiss.
 R.A.Towns.
 R.A.Towns. & Borow.
 R.A.Towns. & Huisman
 R.A.Towns., Keats & Y.M.Chamb.
 R.A.W.Herrm.
-R.Bauer & M.Piepenbr.
+R.B.Sanford
+R.Bauer, Begerow, A.Nagler & Oberw.
+R.Bauer, M.Lutz & Oberw.
+R.Benn. & Thines
 R.Blanch.
 R.Booth
 R.Booth & P.R.Sharpe
 R.Booth, D.J.Moore & Hodgon
 R.Br.
 R.Br. & Sims
-R.Br. - Alternanthera nodiflora R.Br.
-R.Br. - Atriplex spinibractea R.H.Anderson
-R.Br. - Cassinia longifolia R.Br.
-R.Br. - Cycas platyphylla K.D.Hill
-R.Br. - Myoporum boninense subsp. australe Chinnock
 R.Br. ex A.Braun
 R.Br. ex A.Juss.
 R.Br. ex A.Rich.
 R.Br. ex B.D.Jacks.
 R.Br. ex Bartl.
 R.Br. ex Benn.
 R.Br. ex Benth.
-R.Br. ex Benth. subsp. furfuracea - Zieria furfuracea subsp. gymnocarpa J.A.Armstr.
 R.Br. ex Bercht. & J.Presl
 R.Br. ex Blakely
 R.Br. ex Boeckeler
 R.Br. ex Braid
 R.Br. ex Brid.
 R.Br. ex Britten
 R.Br. ex Brongn.
@@ -29645,16 +29785,14 @@
 R.Br. ex Knuth
 R.Br. ex Lemon
 R.Br. ex Lindl.
 R.Br. ex Loudon
 R.Br. ex Maiden
 R.Br. ex Mart.
 R.Br. ex Meisn.
-R.Br. ex Mirb.
-R.Br. ex Nees
 R.Br. ex Pfeiff.
 R.Br. ex Planch.
 R.Br. ex Poir.
 R.Br. ex Pépin
 R.Br. ex R.T.Baker
 R.Br. ex R.T.Baker & H.G.Sm.
 R.Br. ex Rendle
@@ -29671,53 +29809,24 @@
 R.Br. ex T.Mitch.
 R.Br. ex T.Nees & Sinning
 R.Br. ex Tiegh.
 R.Br. ex Turner
 R.Br. ex Wall.
 R.Br. ex Walp.
 R.Br. ex Wight & Arn.
-R.Br. subsp. floribunda - Grevillea floribunda subsp. tenella Olde & Marriott
-R.Br. x Aristida vagans Cav.
-R.Br. x Asplenium (?) paleaceum R.Br.
-R.Br. x Asplenium paleaceum R.Br.
-R.Br. x Asplenium polyodon G.Forst.
-R.Br. x Caladenia hirta Lindl.
-R.Br. x Caladenia nana Endl.
-R.Br. x Caladenia patersonii R.Br.
-R.Br. x Caladenia reptans Lindl.
-R.Br. x Chenopodium cristatum (F.Muell.) F.Muell.
-R.Br. x Convolvulus erubescens Sims
-R.Br. x Cyperus centralis K.L.Wilson
-R.Br. x Dendrobium dicuphum F.Muell.
-R.Br. x Dendrobium discolor Lindl.
-R.Br. x Dendrobium johannis Rchb.f.
-R.Br. x Dendrobium kingianum Bidwill ex Lindl.
-R.Br. x Dendrobium linguiforme Sw.
-R.Br. x Dendrobium semifuscum (Rchb.f.) Lavarack & P.J.Cribb
-R.Br. x Diuris chrysantha D.L.Jones & M.A.Clem.
-R.Br. x Doodia media R.Br.
-R.Br. x Lepyrodia verruculosa B.G.Briggs & L.A.S.Johnson
-R.Br. x Myosotis exarrhena F.Muell.
-R.Br. x Notelaea ovata R.Br.
-R.Br. x Petrophile seminuda Lindl.
-R.Br. x Plectranthus parviflorus R.Br.
-R.Br. x Plectranthus suaveolens S.T.Blake
-R.Br. x Pterostylis reflexa var. intermedia Ewart
 R.Br.bis
-R.Br.ter.
 R.Butcher
 R.Butcher & Cockerton
 R.Butcher & Cowie
 R.Butcher & P.J.H.Hurter
 R.C.Harris
 R.C.Harris, Ladd & Printzen
 R.C.Keating & Takht.
 R.C.Y.Chou
 R.Chodat
-R.Chodat & F.Chodat
 R.Cunn.
 R.Cunn. ex A.Cunn.
 R.D.Arneson
 R.D.B.Whalley & J.J.Bruhl
 R.D.Spencer & Lumley
 R.D.Webster
 R.D.Wood
@@ -29733,80 +29842,91 @@
 R.E.Massey
 R.E.Massey ex Stapf
 R.E.Norris
 R.E.Norris & M.J.Wynne
 R.E.Sm. & E.H.Sm.
 R.E.Wyatt & A.H.Stoneb.
 R.Emers.
-R.Emers. & Cooney
 R.F.Bastow
 R.F.Castañeda
 R.F.Castañeda & Heredia
-R.F.Castañeda & Mercado
+R.F.Castañeda & W.B.Kendr.
 R.F.Castañeda & W.Gams
 R.F.Dykstra
 R.F.Park & Keane
 R.Fern. & Verdc.
 R.G.Bagn. & Sheridan
 R.G.Rees
 R.G.Shivas
 R.G.Shivas & A.J.Young
-R.G.Shivas & Crous
+R.G.Shivas & Alcorn
 R.G.Shivas & Cunningt.
-R.G.Shivas & E.M.Davison
 R.G.Shivas & J.Walker
 R.G.Shivas & L.Morin
 R.G.Shivas & McTaggart
 R.G.Shivas & Rodr.Mir.
 R.G.Shivas & Sivan.
 R.G.Shivas & Tree
 R.G.Shivas & U.Braun
 R.G.Shivas & Vánky
 R.G.Shivas & Y.P.Tan
+R.G.Shivas & Ying M.Li
 R.G.Shivas, A.J.Young & B.C.McNeil
 R.G.Shivas, A.J.Young & Crous
 R.G.Shivas, A.J.Young & Grice
+R.G.Shivas, A.J.Young & U.Braun
+R.G.Shivas, Akinsanmi & Y.P.Tan
 R.G.Shivas, Bathgate & Podger
 R.G.Shivas, Cother, G.J.Ash, Jane D.Ray & Vánky
-R.G.Shivas, Cunningt. & Vánky
+R.G.Shivas, G.F.Claridge & Y.P.Tan
 R.G.Shivas, Grice & A.J.Young
-R.G.Shivas, K.D.Hyde & C.A.Pearce
+R.G.Shivas, Grice & Y.P.Tan
+R.G.Shivas, J.G.Allen & P.M.Will.
+R.G.Shivas, Jacq.Edwards & Y.P.Tan
+R.G.Shivas, L.Morin, S.M.Thomps. & Y.P.Tan
 R.G.Shivas, M.D.Barrett, R.L.Barrett & McTaggart
-R.G.Shivas, M.J.Ryley, Telle & Thines
+R.G.Shivas, M.Lutz, McTaggart & Vánky
+R.G.Shivas, Marney & McTaggart
+R.G.Shivas, Marney & Y.P.Tan
+R.G.Shivas, Marney, Cunningt. & Y.P.Tan
 R.G.Shivas, McTaggart & Vánky
 R.G.Shivas, McTaggart, A.J.Young & Crous
-R.G.Shivas, P.M.Will. & J.G.Allen
+R.G.Shivas, Ryley & Y.P.Tan
+R.G.Shivas, Ryley, Telle & Thines
 R.G.Shivas, Ryley, Telle, Liberato & Thines
 R.G.Shivas, S.J.Pethybr. & S.J.Jones
-R.G.Shivas, U.Braun & A.J.Young
-R.G.Shivas, U.Braun & K.Schub.
+R.G.Shivas, S.M.Thomps. & A.J.Young
+R.G.Shivas, S.M.Thomps. & Y.P.Tan
 R.G.Shivas, Vawdrey & Y.P.Tan
 R.G.Shivas, Vánky & Athip.
-R.G.Shivas, Vánky & C.Vánky
 R.G.Shivas, Vánky & Cunningt.
+R.G.Shivas, Vánky, M.D.Barrett & M.Lutz
 R.G.Shivas, Y.P.Tan & Grice
+R.G.Shivas, Y.P.Tan & Ryley
+R.G.Shivas, Y.P.Tan & Thines
+R.G.Shivas, Y.P.Tan, Marney & Abell
+R.G.Shivas, Y.P.Tan, Telle & Thines
 R.H.Anderson
 R.H.Anderson & Aellen
 R.H.Archer
 R.H.Jones & J.J.Bruhl
 R.H.Jones & T.W.May
 R.H.Petersen
 R.H.Petersen & Bougher
 R.H.Petersen & Halling
 R.H.Petersen & M.D.Barrett
-R.H.Petersen, Kovalenko & O.Morozova
+R.H.Petersen & Watling
 R.H.Petersen, Kovalenko & O.V.Morozova
 R.H.Thomps.
 R.H.Thompson & D.E.Wujek
 R.H.Zander
 R.Hartig
 R.Hedw.
 R.Hedw. ex DC.
 R.Heim
-R.Heim & Malençon
 R.Heim ex R.Heim
 R.Hesse
 R.Hogg
 R.J.Bates
 R.J.Bates & D.L.Jones
 R.J.Bates & J.Z.Weber
 R.J.Bates ex Jeanes
@@ -29816,15 +29936,14 @@
 R.J.Davies
 R.J.Davies & Alford
 R.J.F.Hend.
 R.J.F.Hend. & Guymer
 R.J.F.Hend. & Halford
 R.J.F.Hend. & Mollemans
 R.J.F.Hend. & Sharpe
-R.J.F.Hend. x Dianella revoluta R.Br.
 R.J.G.Hertel
 R.J.King & Puttock
 R.J.Watson & Ladiges
 R.Jones & G.T.Kraft
 R.K.Benj.
 R.K.Jansen
 R.K.S.Lee
@@ -29839,24 +29958,26 @@
 R.L.Barrett & I.Telford
 R.L.Barrett & J.Palmer
 R.L.Barrett & K.L.Wilson
 R.L.Barrett & K.W.Dixon
 R.L.Barrett & M.D.Barrett
 R.L.Barrett & P.M.Peterson
 R.L.Barrett & Roalson
+R.L.Barrett & T.C.Wilson
 R.L.Barrett, G.B.Wells & K.W.Dixon
 R.L.Barrett, Hopper & T.D.Macfarl.
 R.L.Barrett, J.J.Bruhl & K.L.Wilson
 R.L.Barrett, K.L.Wilson & J.J.Bruhl
 R.L.Barrett, Keighery & T.D.Macfarl.
 R.L.Barrett, Kenneally & Lowrie
 R.L.Barrett, M.D.Barrett & Duretto
 R.L.Barrett, M.D.Barrett & Hopper
 R.L.Barrett, M.D.Barrett & K.W.Dixon
 R.L.Barrett, M.D.Barrett & Lowrie
+R.L.Barrett, M.D.Barrett & M.A.Clem.
 R.L.Giles
 R.L.Massey
 R.L.Mathur & B.L.Mathur
 R.L.Moe
 R.L.Taplin
 R.L.Taplin &P.J.Lang
 R.L.Zhu & L.Shu
@@ -29918,23 +30039,17 @@
 R.S.Williams
 R.Sant
 R.Sant & Tibell
 R.Sant.
 R.Sant. & Tibell
 R.Sant. ex Matzer & R.Sant.
 R.Sprague
+R.Sprague & Aar.G. Johnson
 R.T.Baker
 R.T.Baker & H.G.Sm.
-R.T.Baker x Acacia harpophylla F.Muell. ex Benth.
-R.T.Baker x Acacia tephrina Pedley
-R.T.Baker x Eucalyptus melanophloia F.Muell.
-R.T.Baker x Eucalyptus populnea F.Muell.
-R.T.Baker x Eucalyptus racemosa Cav.
-R.T.Baker x Eucalyptus sideroxylon A.Cunn. ex Woolls
-R.T.Baker x Eucalyptus viminalis Labill.
 R.T.Clausen
 R.T.Mill
 R.T.Moore
 R.T.Moore & Meyers
 R.Tucker
 R.V.Sm.
 R.V.Sm. & McGill.
@@ -29953,14 +30068,15 @@
 R.W.Davis & P.J.H.Hurter
 R.W.Davis & R.Butcher
 R.W.Davis & Rye
 R.W.Davis & T.Hammer
 R.W.Davis & Tauss
 R.W.Davis & Wege
 R.W.Davis, J.Palmer & T.Hammer
+R.W.Davis, K.R.Thiele & Cockerton
 R.W.Davis, Wege & Schmidt-Leb.
 R.W.Holmes
 R.W.Jobson
 R.W.Jobson & Baleeiro
 R.W.Jobson & Cherry
 R.W.Jobson & Davies-Colley
 R.W.Jobson & M.D.Barrett
@@ -29975,78 +30091,72 @@
 R.Wagner
 R.Wilczek
 R.Y.Roy & B.Rai
 R.Y.Roy, R.S.Dwivedi & R.R.Mishra
 R.Y.Zheng & G.Q.Chen
 Raam
 Rabenh.
-Rabenh. & Küchenm.
 Rabenh. ex Bornet & Flahault
-Rabenh. ex De Not. & Ces.
+Rabenh. ex Ces. & De Not.
 Rabenh. ex Fuckel
 Rabenh. ex Hilse
 Rabenh. ex J.Schröt.
 Racib.
 Racib. ex Theiss. & Syd.
 Racov.
 Radcl.-Sm.
 Radcl.-Sm. & Govaerts
 Raddi
 Raddi ex Spreng.
 Radlk.
-Radlk. x Jagera pseudorhus (A.Rich.) Radlk.
 Raeusch.
 Raf.
 Raf. ex Greene
 Rafarin
 Rafn
 Raghu Ram & Mallaiah
 Rahayu & I.H.Parbery
 Railons.
 Raithelh.
 Rajchenb.
-Rajchenb. & A.David
+Rajchenb. & J.E.Wright
+Rajchenb. & P.K.Buchanan
 Rajendren
 Rajput
 Rajput & Carolin
 Raleigh
 Ralfs
-Ralfs ex Bréb.
 Ralfs ex Ehrenb.
-Ralfs ex Kütz.
 Ralfs ex Meyen
 Ralph
 Ram.
-Raman & Natarajan
 Rambelli
 Rambold
 Rambold & Elix
 Rambold & H.Mayrhofer
 Rambold & Pietschm.
 Rambold & Triebel
 Ramond
 Ramond ex DC.
 Rampi
 Ramsay-Wright
 Ramsb.
 Randall
 Randell
-Randell x Ehretia membranifolia R.Br.
-Randell x Ehretia saligna R.Br.
 Randhawa
 Rands
 Rangel
 Rantonnet ex C.Morren
 Ranzoni
 Raoul
 Raoul ex Lehm.
 Raper
 Raper & Fennell
 Rapin
-Rasanen
+Rapley, Steinrucken, Vitelli, Holdom & Y.P.Tan
 Ratkowsky
 Rattray
 Raulings & Ladiges
 Raunk.
 Rauschert
 Ravenel ex Berk. & M.A.Curtis
 Raym.-Hamet
@@ -30061,31 +30171,33 @@
 Rchb. ex Kunze
 Rchb. ex Schauer
 Rchb. ex Spreng.
 Rchb.f.
 Rchb.f. & S.Moore
 Rchb.f. & Zoll.
 Rchb.f. ex Lindl.
-Rchb.f. x Caladenia pulchra Hopper & A.P.Br.
-Rchb.f. x Dendrobium discolor Lindl.
-Rchb.f. x Dendrobium teretifolium R.Br.
-Rchb.f. x Thelymitra macrophylla Lindl.
 Rea
 Reader
+Reannon L.Smith, Pascoe, T.W.May & Jacq.Edwards
 Rebent.
 Rebent. ex Kuntze
+Recca & Mrak
 Rech.
 Rech.f.
 Redhead
 Redhead & Ginns
 Redhead & Kroeger
+Redhead & Mullineux
 Redhead & Singer
 Redhead, Lutzoni, Moncalvo & Vilgalys
+Redhead, Moncalvo & Vilgalys
 Redhead, Moncalvo, Vilgalys & Lutzoni
+Redhead, Moncalvo, Vilgalys, Desjardin & B.A.Perry
 Redhead, Vilgalys & Hopple
+Redhead, Vizzini, Drehmel, & Contu
 Redinger
 Redouté
 Reeder
 Reedman & Womersley
 Rees, Zuccarello & Orlovich
 Reess
 Regel
@@ -30131,14 +30243,15 @@
 Reveal & Doweld
 Reveal & Hoogland
 Reveal & Zomlefer
 Reverdin
 Rex
 Rexer
 Reynolds
+Rheeder, Marasas & P.E.Nelson
 Ribaldi
 Ricard
 Rich
 Rich.
 Rich. & A.Rich.
 Rich. & A.Rich. ex Mirb.
 Rich. & Juss.
@@ -30157,18 +30270,20 @@
 Richon & Roze
 Rick
 Riddle
 Ridl.
 Ridl. ex C.B.Clarke
 Ridsdale
 Riebe
+Riebesehl & Langer
 Riedl
 Riess
 Rieth
 Rifai
+Rifai, Chin S.Yang & Korf
 Rikli
 Rilke
 Rilstone
 Rines & Hargraves
 Rintz
 Risso
 Ritgen
@@ -30188,32 +30303,34 @@
 Roberty
 Robill. & Castagne ex DC.
 Robins & G.T.Kraft
 Robyns
 Rodd
 Rodigas
 Rodr.Mir.
-Rodr.Mir. & Shivas
 Rodway
 Rodway & Cleland
-Rodway ex Kantvilas & Y.S.Chang
 Rodway ex W.M.Curtis
+Rodway ex Y.S.Chang & Kantvilas
 Roem. & Schult.
 Roep.
 Roezl ex Ortgies
+Rogerson & Samuels
 Rohde ex Loisel.
 Rohr
 Rohrb.
+Roiv.
 Rolfe
 Rolfe ex Downie
 Rolfe ex Hemsl.
 Rolland
 Romagn.
 Romell
 Romell ex Burt
+Roon.-Lath. & Crous
 Roper
 Rosanoff
 Roscoe
 Rose
 Rosenst.
 Rosenv.
 Roshkova
@@ -30234,15 +30351,14 @@
 Rottler
 Rottler ex Hook.f.
 Rottler ex Spreng.
 Rottler ex Willd.
 Roubal
 Roum.
 Roum. & Malbr.
-Roum. & P.Karst.
 Round
 Round & Basson
 Round & Bukht.
 Round & Crawford
 Round & D.G.Mann
 Round, Hallsteinsen & Paasche
 Roussel
@@ -30258,17 +30374,14 @@
 Roxb. ex Meisn.
 Roxb. ex Roth
 Roxb. ex Rottler
 Roxb. ex Schult.
 Roxb. ex Sm.
 Roxb. ex W.T.Aiton
 Roxb. ex Willd.
-Roxb. x Eucalyptus platyphylla F.Muell.
-Roxb. x Eucalyptus siderophloia Benth.
-Roxb. x Thunbergia laurifolia Lindl.
 Royle
 Roze
 Roze & Boud.
 Rozefelds
 Rozefelds & A.M.Buchanan
 Rozefelds & H.C.Hopkins
 Rozefelds & Pellow
@@ -30302,101 +30415,124 @@
 Rusby
 Ruttner
 Ruzicka
 Rydb.
 Rye
 Rye & Hislop
 Rye & K.A.Sheph.
+Rye & Keighery
 Rye & M.D.Barrett
 Rye & Peter G.Wilson
 Rye & T.D.Macfarl.
 Rye & Trudgen
 Rye & Wege
 Rye, Keighery & M.D.Barrett
 Rye, R.L.Barrett & M.D.Barrett
 Ryley & Langdon
+Ryley, Y.P.Tan & R.G.Shivas
 Ryvarden
+Ryvarden & Hauskn.
 Ryvarden & I.Johans.
 Räsänen
+Réblová & Hern.-Restr.
 Röhl.
 Röhl. ex Léman
 S.A.Day, R.P.Wickham, Entwisle & P.A.Tyler
 S.A.J.Bell
 S.A.J.Bell & D.Nicolle
 S.A.J.Bell & Driscoll
 S.A.J.Bell & L.M.Copel.
 S.A.J.Bell, Branwhite & Driscoll
+S.A.Rehner & Humber
 S.Archang. & G. Del Fueyo
 S.B.Andrews
 S.B.Saksena
 S.Berger, Fettweiss, Gleissberg, L.B.Liddle, U.Richt., Sawitzky & Zuccarello
 S.Blanco
 S.C.Jong & E.E.Davis
 S.C.Sommerfelt
 S.Chowdhury
+S.Craig, L.J.Vaughan & T.W.May
 S.D.Baker
 S.D.F.Patzak, M.A.M.Renner & Heinrichs
 S.D.F.Patzak, M.A.M.Renner, Schäf.-Verw. & Heinrichs
 S.D.Sharma & Shastry
+S.Dema & I.Telford
+S.E.Fawc. & A.R.Sm.
 S.Ekman & Froberg ex R.Sant.
 S.Ekman & M.Svennson
 S.F.Blake
 S.F.Gray
+S.F.Silveira, Alfenas, Crous & M.J.Wingf.
 S.Fraga & I.Bravo
 S.Fuentes & Borsch
 S.Fuentes, Uotila & Borsch
 S.G.Gmel.
 S.G.Gmel. ex Gugler
 S.G.M.Carr, D.J.Carr & A.S.George
 S.G.M.Fawc.
+S.H.He & Jiao Yang
+S.H.He & Y.C.Dai
 S.H.Iqbal
 S.H.Lewis
 S.H.Lin
 S.H.Sun
 S.H.Wright
 S.Hammer
+S.Handel, Tengfei Wang, Yurkov & H.König
 S.Hatt.
 S.Holzapfel
 S.Hughes
 S.Hughes & Piroz.
 S.Hughes & W.B.Kendr.
+S.Hughes, W.B.Kendr. & Shoemaker
 S.I.Ahmed & Cain
+S.I.Ahmed & M.Qureshi
 S.Imai
 S.Ito
 S.Ito & Kurib.
 S.Ito & S.Imai
 S.J.Dillon
 S.J.Dillon & A.S.Markey
 S.J.Dillon & K.A.Sheph.
 S.J.Forbes
 S.J.Forbes & D.I.Morris
+S.J.Lee & Joanne E.Taylor
 S.J.Lloyd, Leontyev & Dagamac
+S.J.Lloyd, Leontyev, G.Moreno, López-Vill. & Schnittler
 S.J.Patrick
+S.J.Stanley & K.D.Hyde
+S.K.Huang & K.D.Hyde
 S.Keller
+S.Konta & K.D.Hyde
 S.Krauss & L.A.S.Johnson
 S.L.F.Mey.
 S.L.Ghose
+S.L.Liu, Z.Q.Shen & L.W.Zhou
 S.L.Morton
+S.L.Stephenson & Novozh.
+S.L.Stephenson, Pu Liu, Yu Li & Y.Zou
+S.Luo, G.Dong & P.Wong
 S.M.D.FitzGerald
 S.M.Douglas & S.David
 S.M.F.Silva & Sant'Anna
 S.M.Francis
 S.M.Marshall
+S.M.Thomps., R.G.Shivas & Y.P.Tan
 S.M.Wilson & G.T.Kraft
 S.Moore
-S.Moore x Kunzea jucunda Diels
-S.Moore x Kunzea preissiana Schauer
 S.Morris
 S.Okamura
 S.Olsson, Enroth & D.Quandt
 S.Olsson, Enroth, Huttunen & D.Quandt
 S.P.Abbott
 S.P.Churchill
 S.R.Gilmore
 S.R.Hill
+S.R.Thomas, Dell & Trappe
 S.S.Prasad & R.A.B.Verma
 S.Schatz
 S.Schatz & Kohlm.
 S.Schauer
 S.Schauer ex Otto & A.Dietr.
 S.Skinner
 S.Skinner & Entwisle
@@ -30406,25 +30542,20 @@
 S.Stenroos, Pino-Bodas & Ahti
 S.Stenroos, Pino-Bodas, Lumbsch & Ahti
 S.Stringer & Conran
 S.T.Blake
 S.T.Blake ex Byrnes
 S.T.Blake ex Craven
 S.T.Blake ex J.Kern
-S.T.Blake x Cymbopogon refractus (R.Br.) A.Camus
-S.T.Blake x Eucalyptus pellita F.Muell.
-S.T.Blake x Iseilema vaginiflorum Domin
-S.T.Blake x Melaleuca saligna Schauer
-S.T.Blake x Plectranthus foetidus Benth.
-S.T.Blake x Plectranthus graveolens R.Br.
 S.T.Reynolds
 S.T.Reynolds & A.E.Holland
 S.T.Reynolds & P.I.Forst.
 S.T.Reynolds & Pedley
 S.T.Reynolds & R.J.F.Hend.
+S.Takam., Lebeda & M.Götz
 S.Venter
 S.Vidal
 S.Vogel
 S.W.Arnell
 S.W.Arnell ex Grolle
 S.W.L.Jacobs
 S.W.L.Jacobs & A.J.Br.
@@ -30432,25 +30563,25 @@
 S.W.L.Jacobs & J.Everett
 S.W.L.Jacobs & J.Pickard
 S.W.L.Jacobs & K.A.Frank
 S.W.L.Jacobs & Lapinpuro
 S.W.L.Jacobs & Les
 S.W.L.Jacobs, R.D.B.Whalley & D.J.Wheeler
 S.W.Peterson
+S.W.Peterson, Jurjević, Bills, Stchigel, Guarro & F.E.Vega
 S.W.Wong & K.D.Hyde
 S.W.Wong, K.D.Hyde & E.B.G.Jones
+S.W.Wong, K.D.Hyde, W.H.Ho & S.J.Stanley
 S.Wang ex S.W.L.Jacobs & Barkworth
 S.Watson
-S.Watson x Amaranthus quitensis Kunth
 S.Williams
 S.Wright
 S.Y.Hu
 S.Y.Kondr.
 S.Y.Kondr. & Alstrup
-S.Y.Kondr. & Coppins
 S.Y.Kondr. & D.Hawksw.
 S.Y.Kondr. & Elix
 S.Y.Kondr. & Kärnefelt
 S.Y.Kondr., Coppins & D.J.Galloway
 S.Y.Kondr., Elix & A.Thell
 S.Y.Kondr., Elix & Kärnefelt
 S.Y.Kondr., Elix, A.Thell & Hur
@@ -30472,16 +30603,16 @@
 Sacc. & Bizz.
 Sacc. & Briard
 Sacc. & Cub.
 Sacc. & D.Sacc.
 Sacc. & Ellis
 Sacc. & Fiori
 Sacc. & Magnus
-Sacc. & Mancini
 Sacc. & Marchal
+Sacc. & P.Syd.
 Sacc. & Penz.
 Sacc. & Roum.
 Sacc. & Speg.
 Sacc. & Traverso
 Sacc. & Trotter
 Sacc. ex Berl. & Voglino
 Sacc. ex Castell. & Chalm.
@@ -30489,21 +30620,23 @@
 Sacc., M.Rousseau & E.Bommer
 Saccas
 Sachs
 Sadeb.
 Sadler
 Saenger
 Saenger & E.M.Woll.
+Safaief., Mostowf., G.E.Hardy & T.I.Burgess
 Saff.
 Sahlin
 Sainsbury
 Saito
 Saito & M.Ota
 Sakai
 Sakai & T.Yoshida
+Sakalidis & T.I.Burgess
 Sakurai
 Saldarriaga & F.J.R.Taylor
 Saldivia
 Salisb.
 Salisb. ex Bercht. & J.Presl
 Salisb. ex Britton & P.Wilson
 Salisb. ex Endl.
@@ -30516,75 +30649,75 @@
 Salisb. ex Schult. & Schult.f.
 Salkin, M.A.Gordon, Sams. & Rieder
 Salm-Dyck
 Salm-Dyck ex Engelm.
 Salm-Dyck ex Webb & Berthel.
 Salomon
 Salzm. ex C.A.Mey.
+Samarak., Thongbai, K.D.Hyde & M.Stadler
 Samouts.
 Samson & Tansey
 Samson & W.Gams
+Samson, N.Yilmaz & Frisvad
 Samson, S.B.Hong & Varga
+Samson, Visagie & Houbraken
+Samson, W.Gams & H.C.Evans
 Samuel
-Samuel & T.Osborn
 Samuels
 Samuels & Druzhin.
-Samuels & K.F.Rodrigues
-Samuels & Nirenberg
-Samuels & Rogerson
-Samuels & Rossman
+Samuels & Jaklitsch
+Samuels & Seifert
+Samuels, E.Müll. & Petrini
+Sand.-Den., Guarro & Gené
 Sande Lac.
 Sander
 Sander ex André
 Sanderson
 Sandst.
+Sangal. & L.W.Burgess
+Sankaran & B.Sutton
 Santa & Simonn.
 Santel.
 Santel. & Hommers.
 Santi
 Santos
 Saporta
 Sarg.
 Sarma & Shyam
 Sarno & Kooistra
 Sarno & Zingone
-Sartory, J.Mey., R.Sartory & Weill
+Sartory, R.Sartory, Weill & J.Mey.
 Sata
 Sati & N.Tiwari
 Sattarian
+Satthaphorn
 Sauerb.
 Saut.
 Saut. ex Körb.
 Sauter ex Körb.
 Sauv.
+Sav.Verma, Aj.Varma, Rexer, G.Kost & P.Franken
 Savi
 Savigny
 Savile & Parmelee
 Sawada
 Sawada ex L.Ling
 Scarlett
 Sch.Bip.
 Sch.Bip. ex Benth.
 Schaarschm.
 Schaeff.
 Schaer.
-Schaer. ex D.Dietr.
 Schaer. ex Nyl.
 Scharapov
 Scharif
 Scharif ex A.Lam
 Schauer
 Schauer ex Otto & A.Dietr.
 Schauer ex Rchb.
-Schauer x Eucalyptus cloeziana F.Muell.
-Schauer x Eucalyptus radiata Sieber ex DC.
-Schauer x Kunzea montana (Diels) Domin
-Schauer x Kunzea preissiana Schauer
-Schauer x Kunzea recurva Schauer
-Schauer x Kunzea sulphurea Tovey & P.Morris
 Scheele
 Scheff.
 Schenk
 Schenk & Rauch
 Scherff.
 Scheuer
 Scheuerm.
@@ -30607,15 +30740,14 @@
 Schlauer
 Schlech
 Schleich. ex F.Weber & D.Mohr
 Schleich. ex Gaudin
 Schleich. ex Schwägr.
 Schleich. ex Sm.
 Schleid.
-Schlieph.
 Schlittler
 Schljakov
 Schlotth.
 Schltdl.
 Schltdl. & Cham.
 Schltdl. ex Link
 Schltdl. ex Spreng.
@@ -30627,15 +30759,14 @@
 Schltr. ex J.M.Wood
 Schltr. ex Kellermann
 Schmakov
 Schmarda
 Schmid & Curtman
 Schmidel
 Schmidle
-Schmidt
 Schmidt ex Tausch
 Schmidt-Leb.
 Schneev.
 Schnetter
 Schnizl.
 Schodde
 Schodde ex Philipson
@@ -30664,18 +30795,19 @@
 Schrad. ex Schult. & Schult.f.
 Schrank
 Schrank & Hoppe
 Schrank & Mart.
 Schreb.
 Schreb. ex Hedw.
 Schrenk
+Schroers, Gräfenhan & Seifert
 Schroers, O'Donnell, Baayen & Hooftman
+Schroers, Summerb., O'Donnell & Lampr.
 Schröd.
 Schröt.
-Schröt. ex Höhn. & Litsch
 Schuch.
 Schuit. & Peter B.Adams
 Schult.
 Schult. & Schult.f.
 Schult.f.
 Schultz
 Schultz Sch.
@@ -30709,15 +30841,15 @@
 Schönland
 Scop.
 Scribn.
 Scribn. & Merr.
 Sealy
 Searles
 Seaver
-Seaver ex Korf, C.S.Ramamurthi & L.R.Batra
+Seaver ex C.S.Ramamurthi, Korf & L.R.Batra
 Sebast. & Mauri
 Seberg
 Secr.
 Secr. ex Singer
 Seem.
 Seem. & H.Wendl.
 Seem. & J.A.Schmidt
@@ -30730,33 +30862,32 @@
 Seghers
 Segretain
 Segretain & Destombes
 Seidenf.
 Seifert & H.Boulay
 Seifert & N.L.Nick.
 Seifert & Okada
-Seifert & Samuels
-Seifert, Schroers & Gräfenhan
 Seigler & Ebinger
 Seithe
 Seligo
 Selling
 Sellow ex Schult.
 Sellow ex Wied-Neuw.
 Sendtn.
 Sendtn. ex Müll.Hal.
 Senft
 Senghas
 Sennen
+Senwanna, Phookamsak & K.D.Hyde
 Seppelt & H.A.Crum
 Ser.
 Ser. ex DC.
 Servett.
-Sesse & Moc.
 Sessé
+Sessé & Moc.
 Setch.
 Setch. & Estee
 Setch. & Gardner
 Setch. & L.R.Mason
 Setch. & N.L.Gardner
 Seub.
 Seward & E.Dale
@@ -30768,119 +30899,112 @@
 Sharpe
 Shaw
 Shear
 Shear & B.O.Dodge
 Shearer
 Shearer & J.Campb.
 Shearer & J.L.Crane
-Shearer & L.C.Lane
+Shearer & K.D.Hyde
 Shearer & M.A.Mill.
-Shearer, J.Campb. & J.L.Anderson
 Shepley & Womersley
 Sheppard ex Ker Gawl.
 Sherff
 Sherwood
 Sherwood, D.Hawksw. & Coppins
 Sheue, H.Y.Liu, C.C.Tsai & Yuen P.Yang
-Sheue, H.Y.Liu, C.C.Tsai & Yuen P.Yang x Ceriops tagal (Perr.) C.B.Rob.
 Shevejko
 Shihira & R.W.Krauss
 Shin Watan.
 Shipton
 Shipton & Booth
-Shipton & C.Booth
 Shipton & Schipper
 Shipunov
 Shipunov ex Reveal
 Shirai
 Shirley
+Shivas & Rodr.Mir.
 Shoemaker
-Shoemaker, S.Hughes & W.B.Kendr.
+Shoemaker, C.E.Babc. & J.A.G.Irwin
 Showe M.Lin & G.T.Kraft
 Shrubsole
 Shyam & Sarma
 Sibth.
 Sibth. & Sm.
 Sibth. ex Sm.
 Sidiyasa
 Sieber
 Sieber & Zucc.
 Sieber ex A.Juss.
 Sieber ex Baill.
 Sieber ex Benth.
 Sieber ex C.Presl
 Sieber ex DC.
-Sieber ex DC. subsp. radiata x Eucalyptus stricta DC.
-Sieber ex DC. x Pomaderris cinerea Benth.
 Sieber ex Endl.
 Sieber ex Fenzl
 Sieber ex Hook.f.
 Sieber ex Hoppe
 Sieber ex J.M.Black
 Sieber ex Kunth
 Sieber ex Lindl.
 Sieber ex Loudon
 Sieber ex N.A.Wakef.
 Sieber ex P.Morris & J.H.Willis
 Sieber ex R.Br.
 Sieber ex Rchb.
 Sieber ex Schult.
 Sieber ex Schult. & Schult.f.
-Sieber ex Schult. & Schult.f. x Persoonia levis (Cav.) Domin
 Sieber ex Sims
 Sieber ex Sond.
 Sieber ex Spreng.
-Sieber ex Spreng. x Eriostemon myoporoides DC.
-Sieber ex Spreng. x Eucalyptus amygdalina Labill.
 Sieber ex Steetz
 Sieber ex Steud.
 Sieber ex Toelken
 Sieber ex Trin.
 Siebert & Voss
 Siebold
 Siebold & Zucc.
 Siebold & Zucc. ex Steud.
 Siegesb. ex Kuntze
 Siegesmund, J.R.Johans. & Friedl
 Siemaszko
+Sieverd., G.A.Silva & Oehl
 Sigler
 Sigler & J.W.Carmich.
-Sigler, Currah & Gibas
 Sigler, Deanna A.Sutton, Gibas, Summerb. & Iwen
-Sigler, J.W.Carmich. & Tsuneda
+Sigler, Frances & C.Panter
+Sigler, Hambl. & Paré
+Sigler, Tsuneda & J.W.Carmich.
 Sikora
 Silba
 Silva Manso
+Simamora & T.I.Burgess
 Simmonds
 Simonet & Guin.
 Simonk.
 Simonsen
 Sims
-Sims x Dianella congesta R.Br.
 Singer
 Singer & A.H.Sm.
-Singer & Bondartsev
 Singer & Both
-Singer & Clémenc.
+Singer & Clémencon
 Singer ex Hora
 Singer ex P.D.Orton
 Sipman
 Sipman & Aptroot
 Sirisena, Conran & T.D.Macfarl.
 Sirisena, T.D.Macfarl. & Conran
 Sirodot
 Sitzenberger ex Gomont
 Sivan.
-Sivan. & A.J.Inman
+Sivan. & Alcorn
 Sivan. & B.Sutton
 Sivan. & H.S.Chang
-Sivan. & J.A.Hall
-Sivan., Wallwork & Lichon
+Sivan. & R.G.Shivas
+Sivan., Alcorn & R.G.Shivas
 Sivasith.
-Sivasith., Websdane, K.W.Dixon & Pate
 Skab.
 Skan
 Sked
 Skeels
 Skottsb.
 Skottsb. & Levring
 Skou
@@ -30889,31 +31013,28 @@
 Skuja
 Skuja ex Entwisle & Foard
 Skvortsov
 Skvortsov & C.I.Mey.
 Slabber
 Sledge
 Sleumer
+Slippers, Crous & M.J.Wingf.
 Slooten
 Sm.
-Sm. - Eriostemon scaber Paxton
 Sm. ex Andrews
-Sm. ex J.Houlst. & T.Moore
+Sm. ex Houlston & T.Moore
 Sm. ex Meisn.
 Sm. ex R.Br.
 Sm. ex Roem. & Schult.
 Sm. ex Vent.
 Sm. ex Walp.
 Sm. ex Willd.
-Sm. x Eriostemon myoporoides DC.
-Sm. x Eucalyptus planchoniana F.Muell.
-Sm. x Eucalyptus tereticornis Sm.
-Sm. x Sonneratia x gulngai N.C.Duke
 Sm.-White
 Small
+Small & Nash
 Smed.-Pet.
 Smejkal
 Snell
 Snowden
 Sobol.
 Sodamuk, Leavitt & Lumbsch
 Soderstr. & R.P.Ellis
@@ -30930,15 +31051,14 @@
 Sol. ex Britten
 Sol. ex Correa
 Sol. ex Curtis
 Sol. ex DC.
 Sol. ex F.Muell.
 Sol. ex G.Forst.
 Sol. ex Gaertn.
-Sol. ex Gaertn. x Metrosideros kermadecensis W.R.B.Oliv.
 Sol. ex Hemsl.
 Sol. ex Hook.f.
 Sol. ex Kite
 Sol. ex Lindl.
 Sol. ex Parkinson
 Sol. ex R.Br.
 Sol. ex Roxb.
@@ -30950,32 +31070,32 @@
 Sol. ex Sw.
 Sol. ex Willd.
 Soler.
 Solier
 Solms
 Sommerf.
 Sommier
+Somrith., E.B.G.Jones & K.L.Pang
 Sonck
 Sond.
 Sond. & F.Muell.
-Sond. & F.Muell. ex Sond.
 Sond. ex F.Muell. & Tate
 Sond. ex Grunow
 Sond. ex J.Agardh
 Sond. ex Kütz.
 Sond. ex Regel
 Sond. ex W.D.J.Koch
-Sonder
 Sonn.
 Soop
 Sopp
 Soreng, L.J.Gillespie & S.W.L.Jacobs
 Sorokīn
 Sosef & de Koning
 Soskov
+Sotome & T.Hatt.
 Soul.-Bod.
 Sournia
 South
 South & N.M.Adams
 South & Skelton
 Sovereign
 Sowerby
@@ -30985,27 +31105,25 @@
 Span. ex Miq.
 Spangler
 Sparrius
 Sparrius & Sipman
 Sparrius, Elix & A.W.Archer
 Sparrm.
 Sparrow
+Spatafora, Hywel-Jones & Luangsa-ard
 Spauld. & H.Schrenk
 Speare
 Specht
 Speg.
 Spenn.
 Spin
 Splitg.
 Spokes
 Spooner
-Spooner & Hjortstam
-Spooner & Læssøe
 Spooner & Suková
-Spooner, Hjortstam & P.Roberts
 Sprague
 Sprague & Hutch.
 Sprague & Summerh.
 Spreng.
 Spreng. ex Arn.
 Spreng. ex DC.
 Spreng. ex F.Rudolphi
@@ -31029,30 +31147,33 @@
 Staiger
 Staiger & Kalb
 Staiger & Matthes-Leicht
 Staiger, Kalb & Lücking
 Stajsic
 Stajsic & Molyneux
 Stajsic & R.F.Douglas
+Stajsic, Y.P.Tan & R.G.Shivas
 Standl.
 Stanley
 Stapf
 Stapf & C.E.Hubb.
 Stapf & Haines
 Stapf & J.R.Drumm.
-Stapf & Jess.
+Stapf & Jesson
 Stapf ex Blackall & Grieve
 Stapf ex D.A.Cooke
 Stapf ex N.G.Walsh
 Stapf ex Thell.
 Stapf ex Vickery
 Stapf ex W.Fitzg.
 Staples
 Starbäck
 Starke ex Röhl.
+Starmer, Phaff, Ganter & Lachance
+Starmer, Phaff, M.Miranda, M.W.Mill. & J.S.F.Barker
 Starr
 Stauffer
 Stearn
 Stech & W.Frey
 Steck
 Steele
 Steem.Niels.
@@ -31063,14 +31184,15 @@
 Steetz ex F.Muell.
 Steetz ex Sond.
 Steid. & Burkholder
 Steid., Landsb., P.L.Mason, Vogelb., P.A.Tester & Litaker
 Stein
 Steinecke
 Steinh.
+Steinrucken, Vitelli, Holdom, Y.P.Tan & R.G.Shivas
 Stell.-Dekk.
 Stent
 Steph.
 Steph. & Spruce
 Steph. & Watts
 Steph. ex A.Evans
 Steph. ex Besch.
@@ -31106,26 +31228,29 @@
 Stirt. ex Müll.Arg.
 Stizenb.
 Stizenb. ex Gomont
 Stockdale
 Stockdale, D.W.R.Mack. & Austwick
 Stocks ex Harv.
 Stokes
+Stolk & D.B.Scott
 Stolk & Dakin
 Stolk & G.F.Orr
 Stolk & Orr
+Stolk & Samson
 Stoll
 Stolterf.
 Stosch
 Stotler & Crand.-Stotl.
 Strasb.
 Streimann
 Strid
 Strid & Keighery
 Strother
+Strunecký, Bohunická, J.R.Johans. & Komárek
 Struwe & V.A.Albert
 Strömf.
 Stschegl.
 Stuchlik
 Stuck.
 Sturch
 Sturgis
@@ -31151,72 +31276,65 @@
 Suhr ex Jess.
 Suksd.
 Sull.
 Sull. & Lesq.
 Sull. ex A.Gray
 Sullivan
 Sulman
-Summerb., Schroers, O'Donnell & Lampr.
+Summerb., J.A.Scott, Guarro & Crous
 Summerell & L.W.Burgess
-Summerell, L.W.Burgess & C.A.Rugg
+Summerell, C.A.Rugg & L.W.Burgess
 Summerh.
 Summerh. & C.E.Hubb.
 Summerh. & H.F.Comber
 Summerh. ex H.F.Comber
 Sundaram
 Sunding
 Sundström
 Suringar
 Suriray
 Sv.Nilsson ex Marvanová & Sv.Nilsson
+Svantesson & T.W.May
 Sved.
 Sved. ex Kjellm. & Sved.
 Svenson
 Svenson ex J.Kern
 Svirenko
 Svrček
 Sw.
-Sw. ex Ach.
 Sw. ex Brid.
 Sw. ex F.Weber
 Sw. ex F.Weber & D.Mohr
 Sw. ex Hedw.
 Sw. ex Lehm.
 Sw. ex Poir.
 Sw. ex Schrad.
 Sw. ex Schreb.
 Sw. ex Thouars
 Sw. ex Wikstr.
 Sw. ex Willd.
-Sw. x Blechnum medium (R.Br.) Christenh.
-Sw. x Dendrobium teretifolium R.Br.
-Sw. x Doodia aspera R.Br.
-Sw. x Doodia media R.Br.
-Sw. x Lindsaea microphylla Sw.
 Swallen
 Swarbrick & R.Hart
-Swart
-Swart & D.A.Griffiths
 Sweeney
 Sweet
 Sweet ex Courtois
 Sweet ex G.Don
 Sweet ex Jacques
 Sweet ex Lindl.
 Swenson & K.Bremer
 Swift
 Swinb.
 Swingle
 Swinscow & Krog
 Syd.
 Syd. & P.Syd.
 Syd. & P.Syd. ex McAlpine
-Syd. & Sacc.
 Syd. ex Maire
 Syd., P.Syd. & Bubák
+Syd., P.Syd. & E.J.Butler
 Syd., P.Syd. & Theiss.
 Syeda
 Syeda & Carolin
 Syeda ex Obbens
 Sykes
 Syme ex Marquand
 Symon
@@ -31236,14 +31354,15 @@
 Søchting, Arup & Frödén
 Søchting, Frödén & Arup
 Søchting, Søgaard & Sancho
 T.A.Chr.
 T.A.James
 T.Anderson
 T.Anderson ex Hook.f.
+T.Aoki, Geering, Kasson, S.Freeman, Geiser & O’Donnell
 T.Aoki, Kistler, Geiser & O'Donnell
 T.B.Moore
 T.B.Muir
 T.Baines
 T.Baskerv.
 T.C.Chambers & P.A.Farrant
 T.C.Huang
@@ -31251,14 +31370,15 @@
 T.C.Wilson
 T.C.Wilson & B.J.Conn
 T.C.Wilson & Henwood
 T.C.Wilson & Hislop
 T.C.Wilson & P.I.Forst.
 T.C.Wilson & Radunz
 T.C.Wilson, P.I.Forst. & M.A.M.Renner
+T.C.Wilson, S.Rutherf. & S.M.Douglas
 T.Carruth., Huisman & D.I.Walker
 T.Carvalho & O.Mendes
 T.Cooke
 T.D.Macfarl.
 T.D.Macfarl. & A.L.Case
 T.D.Macfarl. & Conran
 T.D.Macfarl. & D.D.Sokoloff
@@ -31268,57 +31388,74 @@
 T.D.Macfarl. & S.J.van Leeuwen
 T.D.Macfarl. & Ward.-Johnson
 T.D.Macfarl., A.P.Br. & C.J.French
 T.D.Macfarl., C.J.French & Conran
 T.D.Macfarl., Conran & C.J.French
 T.Durand
 T.Durand & B.D.Jacks.
+T.E.Almeida & A.R.Field
 T.E.Brooks & H.W.Keller
 T.E.Hunt
 T.E.Hunt & Rupp
 T.E.T.Bond
 T.F.Elliot & Trappe
 T.F.Elliott, Bougher, O’Donnell & Trappe
 T.G.Hartley
 T.G.Hartley & B.Hyland
 T.G.Hartley & J.B.Williams
 T.G.Hartley & L.M.Perry
 T.H.Abé
 T.H.Abé ex Matsuoka
 T.H.Li
 T.H.Li & Watling
+T.H.Li, R.N.Hilton & Watling
+T.H.Li, Watling & N.M.Greg.
 T.H.Nash
+T.H.Nicolson & Gerd.
 T.H.Nicolson & N.C.Schenck
 T.Hammer
 T.Hammer & K.R.Thiele
 T.Hammer & R.W.Davis
+T.Hammer & Toelken
 T.Horig.
 T.Horig. & Chihara
 T.Horig. & Pienaar
 T.Horig. & Yoshiz.-Ebata
 T.I.Burgess
 T.I.Burgess & P.A.Barber
 T.I.Burgess & T.Jung
 T.I.Burgess, P.A.Barber & G.E.Hardy
-T.I.Burgess, P.A.Barber & G.Pegg
+T.I.Burgess, P.A.Barber & G.S.Pegg
 T.J.Baroni & G.M.Gates
+T.J.Baroni, N.A.Fechner & Peppel
+T.J.Baroni, V.Hofst. & Largent
 T.J.Kop.
 T.Jung & T.I.Burgess
+T.Jung, Stukely & T.I.Burgess
 T.Koyama
 T.Krueger & A.Fleischm.
+T.Krueger & A.S.Rob.
+T.Krueger & Bourke
+T.Krueger, A.Fleischm. & Bourke
 T.L.Collins
 T.L.Collins & I.Telford
 T.L.Collins & J.J.Bruhl
 T.L.Collins, R.L.Andrew & J.J.Bruhl
 T.L.Jahn & Shawhan
+T.L.Pearce, J.B.Scott, Crous, S.J.Pethybr. & F.S.Hay
 T.Lawr.
 T.Lebel
 T.Lebel & Castellano
+T.Lebel & L.Tegart
 T.Lebel & M.D.Barrett
+T.Lebel & Orihara
 T.Lebel & Vellinga
+T.Lebel, Boxshall & Broadbridge
+T.Lebel, Douch & L.J.Vaughan
+T.Lebel, Douch, L.Tegart & L.J.Vaughan
 T.Lestib.
 T.Lestib. ex Dumort.
 T.Liebe
 T.M.Bock
 T.M.Harris
 T.M.Salter
 T.M.Schust.
@@ -31326,32 +31463,36 @@
 T.Macbr.
 T.Mitch.
 T.Mitch. ex Lindl.
 T.Moore
 T.Moore ex Bosch
 T.Moore ex G.Schneid.
 T.Mori
+T.Muroi, Udagawa & Y.Otani
+T.N.Lakh. & Mukerji
 T.Nees
 T.Nees & Blume
 T.O.Cho, L.M.McIvor & S.M.Boo
 T.Ohta
+T.Osborn & Samuel
 T.Post & Kuntze
 T.S.Choo
 T.S.Hart
 T.S.Henshall
 T.S.Liu & W.D.Huang
 T.S.Ramakr. & K.Ramakr.
 T.Sprib. & Lumbsch
-T.W.Johnson & A.R.Caval.
+T.T.H.Vu, J.L.Walsh, M.H.Laurence, L.W.Burgess, E.C.Y.Liew & Summerell
 T.W.May
 T.W.May & A.E.Wood
 T.W.May & P.R.Johnst.
 T.W.Sheph.
 T.Wagner & M.Fisch.
 T.West
+T.Y.Zhang & J.C.David
 T.Yamag., Seppelt & Z.Iwats.
 T.Yoshida & Mikami
 Tadgell
 Tadul. & K.C.Jacob
 Tagawa
 Tak.Tanaka
 Tak.Tanaka & Chihara
@@ -31370,34 +31511,32 @@
 Tamblyn
 Tamura
 Tanaka
 Tandon & Bilgrami
 Tandon & Bilgrami ex M.B.Ellis
 Tanfani
 Tangney
+Tangney, D. Quandt, Huttunen & M. Stech
 Tansey & M.A.Jack
+Tao Yang & Crous
 Tardieu
 Targ.Tozz.
 Targ.Tozz. ex Kuntze
 Tas. Herbarium
 Tassi
 Tate
 Tate ex Domin
 Tate ex J.M.Black
-Tate x Acacia elachantha Maslin & M.W.McDonald
-Tate x Acacia gonoclada F.Muell.
-Tate x Acacia hammondii Maiden
-Tate x Acacia tropica (Maiden & Blakely) Tindale
 Tateoka ex S.D.Sharma & Shastry
 Taton
 Taub.
 Tausch
 Tausch ex A.Kern.
 Tauss
-Tav.
+Tauss & Rye
 Tavanti, A.Davidson, Gow, M.Maiden & Odds
 Taylor
 Taylor ex Broth.
 Taylor ex Burges
 Taylor ex C.Bab. & Mitt.
 Taylor ex Dixon
 Taylor ex Gottsche, Lindenb. & Nees
@@ -31413,42 +31552,44 @@
 Tehon
 Teijsm. & Binn.
 Teijsm. & Binn. ex Braid
 Teijsm. ex Hassk.
 Teiling
 Teixeira
 Tell
+Telle & Thines
 Temp.
 Ten.
+Teng
+Tennakoon, Camporesi, Phookamsak & K.D.Hyde
 Teodor.
 Tepper
 Tepper ex F.Ludw.
 Tepper ex Toelken
 Tereg
 Teschem.
 Teschner
 Testo & A.R.Field
 Th.Fr.
+Thambug. & K.D.Hyde
 Thaxt.
 Theiss.
 Theiss. & Sacc.
 Theiss. & Syd.
 Thell.
 Theophr. ex Wallr.
 Thibaud ex DC.
 Thiers
 Thiers & Ammirati
 Thines
 Thines & Y.J.Choi
 Thirum.
 Thirum. & M.J.O'Brien
-Thirum. & Mundk.
 Thirum. & Neerg.
-Thirum. & Payak
-Thirum., Payak & Pavgi
+Thirum., Pavgi & Payak
 Thivy
 Thiéb.-Bern. ex Pers.
 Thom
 Thomasson
 Thonn.
 Thore
 Thorne
@@ -31469,27 +31610,24 @@
 Thur. ex Bornet & Flahault
 Thur. ex Gomont
 Thuret
 Thuret ex Bornet & Flahault
 Thuret ex Gomont
 Thwaites
 Thwaites & F.Muell.
-Thwaites & F.Muell. ex F.Muell.
 Thwaites & Mitt.
 Thwaites & Ralfs
 Thwaites ex Gomont
 Thwaites ex Harv.
 Thwaites ex Merr.
 Thwaites ex Mitt.
 Thwaites ex W.Sm.
 Thér.
 Thér. & Dixon
 Thüm.
-Thüm. & F.Muell.
-Thüm. & Pass.
 Thüm. ex G.Cunn.
 Thüm. ex McAlpine
 Tibell
 Tibell & K.Ryman
 Tiegh.
 Tiegh. & G.Le Monn.
 Tiegh. ex Blakely
@@ -31509,20 +31647,18 @@
 Tindale & Bedward
 Tindale & Court
 Tindale & Craven
 Tindale & Herscovitch
 Tindale & Kodela
 Tindale & Maconochie
 Tindale & Maslin
-Tindale & Maslin x Acacia tumida var. pilbarensis M.W.McDonald
 Tindale & P.S.Green
 Tindale & S.J.Davies
 Tindale ex T.C.Chambers
 Tindale ex de Kok
-Tindale x Glycine clandestina J.C.Wendl.
 Tindale, Kodela & D.Keith
 Tineo & Guss.
 Tineo ex Guss.
 Tineo ex Lojac.
 Tintelnot
 Tippery & Les
 Tirveng.
@@ -31530,68 +31666,64 @@
 Tisdall
 Tiver
 Tixier
 Tobler
 Tod.
 Tod. ex Riccob.
 Tode
-Tode : Fr.
 Tode ex Sacc.
 Toelken
 Toelken & A.F.Rob.
 Toelken & D.Dean Cunn.
 Toelken & G.F.Craig
 Toelken & R.J.Bates
 Toelken & R.T.Mill.
 Toelken & de Lange
-Toelken x Hibbertia sericea (R.Br. ex DC.) Benth.
-Toelken x Kunzea ericifolia (Sm.) Heynh.
-Toelken x Kunzea jucunda Diels
-Toelken x Kunzea opposita F.Muell.
-Toelken x Kunzea parvifolia Schauer
-Toelken x Kunzea praestans Schauer
-Toelken x Kunzea recurva Schauer
 Togashi & Maki
 Tokida & T.Masaki
 Tomaschek
 Tomilin
 Toml. & Posl.
 Tomm. ex Freyn
-Tommerup, Bougher & Malajczuk
+Tommerup & Langdon
+Tomšovský
 Torr.
 Torr. & A.Gray
-Torr. x Prosopis velutina Wooton
 Torrend
+Torres-Garcia, Dania García & Gené
+Torres-Garcia, Gené & Cano-Lira
 Tortosa
-Tortosa x Discaria pubescens (Brongn.) Druce
 Tourn. ex Adans.
 Tourn. ex Medik.
 Tourn. ex Mill.
 Touw
 Tovey & P.Morris
 Traaen
 Trab.
 Trab. ex Grolle
 Tracy
+Tracy & Earle
 Trail
 Transeau
 Tranzschel
 Trappe
+Trappe & Castellano
 Trappe & Claridge
 Trappe & E.L.Stewart
 Trappe & G.W.Beaton
 Trappe & Gerd.
 Trappe & Malajczuk
-Trappe, Bougher & Matheny
-Trappe, Bougher & Matheny ex Trappe, Bougher & Matheny
+Trappe, Castellano & Amar.
 Trappe, Castellano & Giachini
+Trappe, Castellano & Malajczuk
+Trappe, Castellano & Malajczuk ex Y.S.Chang & Kantvilas
 Trappe, Claridge & Castellano
 Trappe, Claridge & Kovács
+Trappe, Desirò, M.E. Sm., Bonito & Bidartondo
 Trappe, Gerd. & I.Ho
-Trappe, S.R.Thomas & Dell
 Trappe, V.L.Oliveira, Castellano & Claridge
 Tratman ex Morrison
 Tratt.
 Traub
 Traub & L.S.Hannibal ex Traub
 Traub ex Reveal
 Trautv.
@@ -31617,14 +31749,15 @@
 Trinkaus & Elix
 Trinkaus, H.Mayrhofer & Elix
 Troll
 Tronchin
 Trono
 Tropova
 Trouillas, Sosnowski & Gubler
+Trouillas, W.M.Pitt & Gubler
 Trow
 Trudgen
 Trudgen & Keighery
 Trudgen & M.D.Barrett
 Trudgen & P.-L.de Kock
 Trudgen & Rye
 Trudgen ex Rye
@@ -31632,35 +31765,28 @@
 Tsang
 Tsch.-Woess & Poelt
 Tscherm.-Woess
 Tsiang
 Tsuda & Ueyama
 Tsumura
 Tubaki
-Tubaki & K.Ando
 Tubeuf
 Tuck.
 Tuck. ex Nyl.
 Tul.
 Tul. & C.Tul.
 Tul. ex G.H.Otth
 Tul. ex M.Raoul
+Tulloss
 Tulloss, A.M.Young & A.E.Wood
+Tuom. & T.J.Kop.
 Tupa
 Turconi
 Turcz.
-Turcz. - Phebalium maxwellii (F.Muell.) Engl.
-Turcz. - Phebalium tuberculosum subsp. megaphyllum (Ewart) Paul G.Wilson
 Turcz. ex Craven
-Turcz. subsp. erythronema x Eucalyptus salubris F.Muell.
-Turcz. subsp. erythronema x Eucalyptus tenera L.A.S.Johnson & K.D.Hill
-Turcz. subsp. erythronema x Eucalyptus tephroclada L.A.S.Johnson & K.D.Hill
-Turcz. var. erythronema x Eucalyptus orthostemon D.Nicolle & Brooker
-Turcz. x Eucalyptus retusa D.Nicolle, M.E.French & McQuoid
-Turcz. x Phebalium tuberculosum (F.Muell.) Benth.
 Turicchia, S.Ventura, Komárk.-Legn.& Komárek
 Turner
 Turner & Borrer
 Turpin
 Turpin ex Gomont
 Turpin ex Pers.
 Turra
@@ -31670,30 +31796,30 @@
 Tuyn
 Twining
 Tzvelev
 Tønsberg
 Tønsberg & A.Nordin
 U.B.Deshmukh
 U.Braun
-U.Braun & K.Schub.
+U.Braun & Crous
+U.Braun & Priest
+U.Braun & R.T.A.Cook
 U.Braun & Zhurb.
+U.Braun, C.Nakash., Videira & Crous
 U.Grube
 U.Grube & Elix
 U.Grube, H.Mayrhofer & Elix
 U.Hamann
 U.Scholz
 Udachin & Schachn.
 Udachin & Shakhm.
 Udagawa & Furuya
 Udagawa & Toyaz.
-Udagawa, Nagao & Bougher
-Udagawa, Y.Otani & T.Muroi
 Uden & Carmo Souza
 Uden & Kolip.
-Uden & Vidal-Leir.
 Udovicic & R.D.Spencer
 Uebelm.
 Uherk.
 Uittien
 Ulbr.
 Uline
 Ullstrup
@@ -31702,22 +31828,25 @@
 Underw. ex V.S.White
 Ung.-Sternb.
 Unger
 Upson & S.Andrews
 Upton
 Urb.
 Urb. & Ekman
+Urquhart & Douch
+Urquhart & Idnurm
+Urquhart, Coulon & Idnurm
 Usteri ex Roem.
 Utermöhl
 Uzuhashi, Tojo & Kakish.
 V.A.W.Graham
 V.Brig.
 V.D.Matthews
-V.G.Rao & A.S.Patil
 V.H.Blackman
+V.Hofst., Clémençon, Vilgalys & Redhead
 V.I.Krecz. & Bobrov
 V.J.Chapm.
 V.J.Chapm. & Dromgoole
 V.J.Cook
 V.J.Staněk
 V.Krishnam. & Sundararajan
 V.May
@@ -31726,37 +31855,44 @@
 V.Robert, B.Bonjean, Karutz, Paschold, W.Peeters & Wubbolts
 V.S.Poretzky & Anisimova
 V.S.White
 V.V.Mill.
 V.Wirth & Vězda
 V.Wirth & Vězda ex Coppins
 Vaartaja
+Vaghefi, B.Poudel & R.G.Shivas
 Vaghefi, S.J.Pethybr., Crous & P.W.J.Taylor
 Vahl
 Vahl ex Kunth
 Vahl ex Poir.
 Vaill.
 Vaill. ex L.
 Vain.
 Valck.Sur.
+Valenz.-Lopez, Crous, Cano, Guarro & Stchigel
+Valenz.-Lopez, Crous, Stchigel, Guarro & Cano
 Valeton
 Valeton ex Bremek.
 Van Eselt.
 Van Geel
 Van Goor
 Van Heurck
 Van Heurck & Müll.Arg.
 Van Houtte
 Van den Borre & Henwood
 Van der Byl
 Van der Walt
+Van der Walt & Arx
+Van der Walt, D.B.Scott & Klift
 VanLand.
 Vand.
 Vanden Berghen
 Vanden Berghen & Jovet-Ast
+Vandepol & Bonito
+Vanderpl.
 Vanderpoorten, Hedenäs, C.J.Cox & A.J.Shaw.
 Vanderyst
 Vanhoutte
 Vanhöffen
 Varga & Samson
 Varsavsky & Ajello
 Vasey
@@ -31765,36 +31901,34 @@
 Vasinger
 Vassal
 Vassiljevsky
 Vassilkov
 Vaucher
 Vaucher ex Bornet & Flahault
 Vaucher ex Gomont
+Vaughan-Mart., Kurtzman, S.A.Mey. & E.B.O'Neill
 Vavra & Joyon ex I.B.Heath
 Veill.
 Veitch
 Veldkamp
-Veldkamp x Perotis rara R.Br.
 Velen.
 Vell.
 Velley
 Vellinga
 Vellinga & Halling
 Vellinga & Lepp
 Venk.Rao
 Venk.Rao ex L.A.S.Johnson & B.G.Briggs
 Venkataram. & C.S.V.Ram
 Vent.
 Vent. ex Bercht. & J.Presl
 Vent. ex Juss.
-Vent. x Hibiscus meraukensis Hochr.
-Vent. x Hibiscus splendens C.Fraser ex Graham
 Venturi
 Venturi ex Broth.
-Venturi ex Watts & Whitel.
+Verbeken & Bougher
 Verd.
 Verdc.
 Verdon
 Verdon & Elix
 Verdon & Rambold
 Verdon ex G.J.Leach
 Verl.
@@ -31804,52 +31938,59 @@
 Verona & Negru ex Rogerson
 Verseghy
 Vershinin & S.L.Morton
 Verwoerd & du Plessis
 Vesque
 Vest
 Vestergr.
-Vezda & Kantvilas
 Vezda & Malcolm
 Viala & G.Boyer
 Viala & Ravaz
 Vic. Herbarium
 Vickers
 Vickery
 Vickery, S.W.L.Jacobs & J.Everett
+Vidal-Leir. & Uden
+Videira & Crous
+Videira, H.D.Shin & Crous
 Vieill.
 Vieill. ex Baill.
 Vieill. ex Brongn. & Gris
 Vieill. ex C.B.Clarke
 Vieill. ex E.Fourn.
 Vieill. ex Planch. & Triana
 Vienn.-Bourg.
 Vierh.
+Vijaykr., L.Mostert, Jeewon, W.Gams, K.D.Hyde & Crous
 Vilela, Humber, J.W.Taylor & L.Mend.
 Vilhelm
 Vill.
 Vill. ex Gochnat
 Villeret
 Vilm.
+Vincent, Seifert & Samson
 Vines
 Vink
 Virot
 Vis.
+Visagie, Houbraken & K.Jacobs
+Visagie, Seifert & Samson
+Visagie, Summerell, Shenoy & Seifert
 Vischer
 Vitman
 Vitt
 Vitt & Crosby
 Vitt & H.A.Mill.
 Vitt & H.P.Ramsay
-Vittad
 Vittad.
 Vittad. ex De Not. & Moris
 Viv.
 Vize ex Cooke
 Vizzini, Contu & Justo
+Vizzini, G.Moreno, P.Alvarado & Cons.
 Viégas
 Vogel
 Vogel ex Benth.
 Voglino
 Vogt & Oberpr.
 Voigt
 Voit
@@ -31863,102 +32004,103 @@
 Vyverman
 Vyverman & D.G.Mann
 Vyverman, K.Sabbe & R.Vyverman
 Váczi & D.Hawksw.
 Vánky
 Vánky & A.A.Mitch.
 Vánky & C.Vánky
+Vánky & McKenzie
 Vánky & R.G.Shivas
-Vánky & Websdane
+Vánky, C.Vánky & R.G.Shivas
 Vánky, M.Lutz & R.G.Shivas
 Vánky, M.Lutz, & Piątek
-Vánky, R.G.Shivas & C.Vanky
+Vánky, R.G.Shivas & C.Vánky
 Vánky, R.G.Shivas & M.Lutz
 Vězda
 Vězda & Hafellner
 Vězda & Kantvilas
 Vězda & Lumbsch
 Vězda & P.James
 Vězda & Pisut
 Vězda & Poelt
 Vězda & Thor
 Vězda & Vivant
 W.A.Baker & Morgan-Jones
+W.A.Dixon
 W.A.Nelson
 W.A.Nelson & K.G.Ryan
 W.A.Weber
-W.A.Weber ex Karnefelt
 W.A.Weber ex Kärnefelt
 W.Anderson ex R.Br.
 W.Archer
 W.Archer bis
 W.Archer bis & Mitt.
 W.Archer ex Playfair
 W.B.Cooke
 W.B.Kendr.
-W.B.Kendr. & Nag Raj
 W.B.Kendr. & R.F.Castañeda
-W.B.Kendr., Nag Raj & DiCosmo
 W.B.Turner
 W.Becker
 W.Bull
 W.Bull ex Hiern
 W.C.Barton & Ridd.
 W.C.Ko
 W.C.Potts & W.R.Barker
 W.C.R.Watson
 W.C.Shieh
 W.Conrad
 W.Conrad & Kuff.
 W.D.Buckley
 W.D.Francis
-W.D.H.Koch & Sond.
 W.D.J.Koch
+W.D.J.Koch & Sond.
 W.D.J.Koch ex Rchb.
 W.D.Jacks. & R.J.E.Wiltshire
 W.D.Reese
 W.Dietr.
-W.Dietr. x Oenothera stricta Ledeb. ex Link
 W.E.Cooper
 W.E.Cooper & A.J.Ford
-W.E.Cooper & F.A.Zich
+W.E.Cooper & Joyce
 W.E.Cooper & P.I.Forst.
+W.E.Cooper & Zich
 W.E.Hoffm. & Tilden
 W.E.Nicholson
 W.F.Chiu
 W.F.M.Drake
 W.Fitzg.
 W.Fitzg. ex Ewart & Jean White
 W.Fitzg. ex Jean White
 W.Fitzg. ex K.Krause
 W.Fitzg. ex Maiden
 W.Fitzg. ex Rendle
 W.Frey & M.Stech
 W.G.Jones, K.D.Hill & J.M.Allen
 W.G.Sm.
 W.Gams
+W.Gams & H.-B.Jansson
+W.Gams & McGinnis
+W.Gams & Mouch.
 W.Gams & Rozsypal
 W.Gams & Sivasith.
 W.Gams & Zare
 W.Gams, Crous & M.J.Wingf.
-W.Gams, Sivasith., P.M.Will. & Highet
+W.Gams, O'Donnell, Schroers & M.Chr.
 W.Greg.
 W.Greg. ex Grev.
 W.H.Adey
 W.H.Adey, R.A.Towns. & Boykins
 W.H.Baxter
+W.H.Ho, K.M.Tsui, Hodgkiss & K.D.Hyde
 W.Hartley
 W.Hill
 W.Hill & F.Muell.
 W.Hill ex Benth.
 W.Hill ex F.M.Bailey
-W.Hill x Dendrobium discolor Lindl.
-W.Hill x Eucalyptus pellita F.Muell.
-W.Hill x Eucalyptus robusta Sm.
 W.J.Gilbert
+W.J.Kaiser, B.C.Wang & J.D.Rogers
 W.J.Koch
 W.J.Kress
 W.J.de Wilde
 W.J.de Wilde & Duyfjes
 W.K.Harris
 W.K.Harris & G.Holmes
 W.K.Harris & W.J.McDonald
@@ -31967,19 +32109,22 @@
 W.Krüger
 W.L.Culb.
 W.L.Culb. & C.F.Culb.
 W.L.Wagner & Hoch
 W.L.Waterh.
 W.Lippert
 W.M.Curtis
+W.M.Pitt & Úrbez-Torr.
+W.M.Pitt, Úrbez-Torr. & Trouillas
 W.Martin
 W.Martin & E.A.Hodgs.
 W.Migula
 W.Mill. & N.Taylor
 W.Muell.
+W.N.Becker & I.R.Hall
 W.N.Takeuchi
 W.N.Takeuchi & Pipoly
 W.Phillips
 W.Phillips & Plowr.
 W.Phillips ex Cooke
 W.R.B.Oliv.
 W.R.Barker
@@ -31989,24 +32134,28 @@
 W.R.Barker & Hislop
 W.R.Barker & Kellermann
 W.R.Barker & M.D.Barrett
 W.R.Barker & R.M.Barker
 W.R.Barker & Rye
 W.R.Barker, R.M.Barker, Jessop & Vonow
 W.R.Barker, Y.S.Liang & Wannan
+W.R.Buck
 W.R.Buck & B.C.Tan
 W.R.Buck & H.A.Crum
 W.R.Buck & Ireland
 W.R.Buck & Vitt
 W.R.Buck, C.J.Cox, A.J.Shaw & Goffinet
+W.R.Buck, Goffinet & A.J.Shaw
+W.R.Buck, P.E.A.S.Câmara & Carv.-Silva
 W.R.Gerard
 W.R.Price
 W.R.Taylor
 W.Rossi
 W.Rossi & A.Weir
+W.Rossi & M.Leonardi
 W.Rossi & Santam.
 W.Schmidt
 W.Sm.
 W.Sm. ex Roper
 W.Sm. ex W.Greg.
 W.T.Aiton
 W.T.Aiton ex G.Don
@@ -32021,22 +32170,22 @@
 W.Watson
 W.West
 W.West & G.S.West
 W.Weston
 W.Weston & Uppal
 W.Wight
 W.Wight & Hedrich
+W.Y.Zhuang & Korf
 W.Yamam.
 WA Herbarium
 Wahlb.
 Wahlenb.
 Wailes
 Wakef.
 Wakef. & A.Pearson
-Wakef. & Buddin
 Wakker
 Wakker & Went
 Waldst. & Kit.
 Waldst. & Kit. ex Willd.
 Wall.
 Wall. ex A.DC.
 Wall. ex Airy Shaw
@@ -32069,17 +32218,19 @@
 Wall. ex Walp.
 Wall. ex Wight
 Wallander & V.A.Albert
 Wallman
 Wallr.
 Wallr. ex Rabenh.
 Wallroth
+Wallwork & Spooner
+Wallwork, Lichon & Sivan.
 Walp.
 Walter
-Walter x Ludwigia repens J.R.Forst.
+Wanas., E.B.G.Jones & K.D.Hyde
 Wannan
 Wannan & J.T.Waterh.
 Wapstra
 Warb.
 Warb. ex Becc.
 Warb. ex H.J.P.Winkl.
 Warb. ex H.Limpr.
@@ -32094,24 +32245,18 @@
 Warnst. ex Weymouth
 Wartm. ex Bornet & Flahault
 Wasser
 Wassh. & L.B.Sm.
 Watkins
 Watling
 Watling & A.M.Young
-Watling & Guzmán
-Watling & Høil.
 Watling & Kile
-Watling & Matheny
 Watling & N.M.Greg.
-Watling & R.H.Petersen
 Watling & T.H.Li
 Watling & T.W.May
-Watling, N.M.Greg. & T.H.Li
-Watling, R.N.Hilton & T.H.Li
 Watts
 Watts & Whitel.
 Watts & Whitel. ex G.Roth
 Watts & Whitel. ex Müll.Hal.
 Watts & Whitel. ex Wijk, Margad. & Florsch.
 Watts ex G.Roth
 Watts ex Watts & Whitel.
@@ -32120,22 +32265,23 @@
 Webb & Berthel.
 Webb ex Moq.
 Webb ex Sch.Bip.
 Weber
 Weber Bosse
 Weber ex F.H.Wigg.
 Weber-van Bosse
+Websdane & Vánky
 Websdane, Sieler, Sivasith. & K.W.Dixon
+Websdane, Sivasith., K.W.Dixon & Pate
 Webster
 Wedd & C.T.White
 Wedd.
 Wedin
 Wedin & Diederich
 Wedin, Ertz & Diederich
-Wedin, Ertz, Diederich & Christnach
 Weese
 Wege
 Wege & D.J.Coates
 Wege & Hislop
 Wege & K.R.Thiele
 Wege & Keighery
 Wege & Orchard
@@ -32155,17 +32301,20 @@
 Weihe & Boenn.
 Weihe & Nees
 Weing.
 Weinm.
 Weir ex Rodway & Cleland
 Weisse
 Weissenb.
+Weixia Wang, D.D.de Silva, and P.W.J.Taylor
+Welti & Courtec.
 Welw.
 Welw. & Curr.
 Welw. ex Baker
+Welw. ex Carrière
 Welw. ex Hegelm.
 Welw. ex Oliv.
 Welzen
 Wender.
 Wendker
 Went
 Wepfer & H.P.Linder
@@ -32181,65 +32330,63 @@
 Westling
 Weston
 Wetmore
 Wettst.
 Wetzel
 Whalley
 Whalley & Watling
+Whalley, Læssøe & Kile
 Whedon & Kof.
 Wheeler
 Whibley
 Whiffen
 Whiffen ex R.L.Seym.
 Whiffen ex W.H.Blackw. & M.J.Powell
 Whiffin
 Whitel.
 Whittaker & Margulis
 Whitton, K.D.Hyde & McKenzie
-Whitton, McKenzie & Hyde, K.D.
 Whitton, McKenzie & K.D.Hyde
 Whyte & Andjic
 Wibel
 Wick.
+Wick., Kurtzman & Herman
 Wickham
 Widjaja
 Wiegand
 Wight
 Wight & Arn.
 Wight & Arn. ex Chiov.
 Wight & Arn. ex Prain
 Wight & Arn. ex Steud.
 Wight ex Arn.
 Wight ex Hook.f.
+Wijayaw. & K.D.Hyde
 Wijk
 Wijk, Margad. & Florsch.
 Wiklund
 Wikstr.
 Wilbr.
 Wildsmith
 Wilks & Woelk.
 Will.
 Willd.
-Willd. - Cyperus cuspidatus Kunth
-Willd. - Schizaea dichotoma (L.) Sm.
 Willd. ex A.Juss.
 Willd. ex Bernh.
 Willd. ex Gaudin
 Willd. ex H.L.Wendl.
-Willd. ex Hedw.
 Willd. ex Klotzsch
 Willd. ex Kunth
 Willd. ex P.Beauv.
 Willd. ex Poir.
 Willd. ex Schkuhr
 Willd. ex Schult.
 Willd. ex Spreng.
 Willd. ex Trin.
 Willd. ex Vogel
-Willd. x Acacia polystachya A.Cunn. ex Benth.
 Wille
 Willi Krieg.
 Willi Krieg. & A.M.Scott
 Willis
 Willk.
 Willk. & Lange
 Willoughby
@@ -32248,15 +32395,14 @@
 Wills & J.J.Bruhl
 Wilmott
 Wilson
 Wilson & Hook.
 Wilson & Hook.f.
 Wilson ex A.Jaeger
 Wilson ex Bruch & Schimp.
-Wilson ex Kindb.
 Wilson ex Müll.Hal.
 Wilson ex Watts & Whitel.
 Wiltshire
 Wimm.
 Wimm. & Grab.
 Windler
 Wingate
@@ -32284,14 +32430,15 @@
 Wolfe & Bougher
 Wolfg.
 Wolfg. ex Hoffm.
 Wolle
 Wollenw.
 Wollenw. & Reinking
 Wollny
+Wollw., J.A.Simpson & M.Stadler
 Wolosz.
 Wolosz. & W.Conrad
 Woltz & Rouane
 Womersley
 Womersley & A.Bailey
 Womersley & E.Conway
 Womersley & G.T.Kraft
@@ -32314,93 +32461,164 @@
 Worapong, Strobel & W.M.Hess
 Woron.
 Woronichin
 Woronin
 Woronin ex J.Schröt.
 Woronow
 Wright
-Wright ex Watts & Whitel.
 Wujek
 Wulfen
 Wulfen ex Hoppe
 Wurmb
 X.C.Zhang
 X.C.Zhang & Christenh.
 X.J.Ge & N.C.Duke
+X.Wei Wang & Houbraken
+X.Wei Wang & L.W.Zhou
+Xin Zhan Liu, F.Y.Bai, M.Groenew. & Boekhout
 Y.-A.Utz & R.P.Gibson
 Y.Baba & Crayn
+Y.C.Dai & G.M.Gates
+Y.C.Dai & Jia J.Chen
+Y.C.Dai & L.W.Zhou
+Y.C.Dai, F.Wu & C.L.Zhao
 Y.C.Dai, F.Wu, G.M.Gates & R.Du
+Y.C.Dai, G.M.Gates, X.H.Ji & P.Du
+Y.C.Dai, Hai J.Li & Vlasák
+Y.C.Li & Zhu L.Yang
+Y.F.Sun & B.K.Cui
+Y.F.Sun, D.H.Costa & B.K.Cui
 Y.J.Yao
+Y.Jia, X.Wei Wang, S.L.Liu & L.W.Zhou
+Y.L.Yang, Zuo Y.Liu, K.D.Hyde & L.Cai
 Y.Ling
 Y.Ling & T.L.Chen
 Y.M.Chamb.
 Y.M.Ju & J.D.Rogers
 Y.M.Ju, J.D.Rogers & H.M.Hsieh
 Y.M.Ju, J.D.Rogers, H.M.Hsieh & Lar.N.Vassiljeva
-Y.Miyake & T.Komin. ex M.Oda
+Y.M.Li, R.G.Shivas, McTaggart & L.Cai
+Y.Marín & Crous
 Y.N.Yu & Z.Y.Zhang
 Y.Nakam.
 Y.Nisik.
+Y.Nisik. & C.Miyake
 Y.Ohara, Nonom. & Yunome ex Uden & H.R.Buckley
 Y.Ono
+Y.P.Tan
+Y.P.Tan & Bishop-Hurley
+Y.P.Tan & Dhileepan
+Y.P.Tan & G.S.Pegg
 Y.P.Tan & R.G.Shivas
+Y.P.Tan & Tran-Nguyen
+Y.P.Tan, Bishop-Hurley & Marney
+Y.P.Tan, Bishop-Hurley & R.G.Shivas
+Y.P.Tan, Bishop-Hurley & S.M.Thomps.
+Y.P.Tan, Bishop-Hurley, Bransgr. & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Dhileepan & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, E.Lacey & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, E.Lacey, Dhileepan & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, E.Lacey, Grice & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, L.Kelly & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Marney & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Marney, D.Teal & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Marney, E.Lacey & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Marney, Scharaschkin, E.Lacey & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, McTaggart & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, Pukallus & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, R.G.Shivas & Bransgr.
+Y.P.Tan, Bishop-Hurley, R.G.Shivas & Marney
+Y.P.Tan, Bishop-Hurley, Ryley & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, S.M.Thomps. & R.G.Shivas
+Y.P.Tan, Bishop-Hurley, T.Taylor, Comben & R.G.Shivas
+Y.P.Tan, Gogorza Gondra & R.G.Shivas
+Y.P.Tan, Grice & R.G.Shivas
+Y.P.Tan, Grice, Czislowski & R.G.Shivas
+Y.P.Tan, Grice, Trevorrow & R.G.Shivas
+Y.P.Tan, Grice, Trevorrow, Bishop-Hurley & R.G.Shivas
+Y.P.Tan, Grice, Trevorrow, I.Newton & R.G.Shivas
+Y.P.Tan, Marney & Bishop-Hurley
+Y.P.Tan, Marney & R.G.Shivas
+Y.P.Tan, Marney, Abell & R.G.Shivas
+Y.P.Tan, Marney, Hywel-Jones & R.G.Shivas
+Y.P.Tan, Pegg, A.G.Manners, A.W.Cooke & R.G.Shivas
+Y.P.Tan, Piggott & E.Lacey
+Y.P.Tan, R.G.Shivas & Marney
+Y.P.Tan, R.G.Shivas & Ryley
+Y.P.Tan, R.G.Shivas, Abell, Hywel-Jones & Marney
+Y.P.Tan, Sbaraini & C.Foster
+Y.P.Tan, Sbaraini & E.Lacey
 Y.S.Chang & A.K.Mills
 Y.S.Chang ex Ratkowsky & G.M.Gates
+Y.S.Paul & J.N.Kapoor
 Y.Saito
 Y.Saito & Womersley
 Y.Takano & T.Horiguchi
 Y.W.Ho
 Y.Yamada
 Y.Yamada, Tom.Suzuki, M.Matsuda & Mikata
 Y.Z.Ruan
 Yacubson
 Yakovlev
 Yamada
 Yamada & Tak.Tanaka
 Yamam.
 Yamash.
 Yan Liu bis, Kociolek & Q.X.Wang
+Yanna & K.D.Hyde
+Yanna, W.H.Ho, McKenzie & K.D.Hyde
 Yasuda
 Yee & A.Millar
 Yendo
 Yeo
 Yesilyurt & H.Schneider
+Yilmaz, Visagie & Frisvad
+Yin.Zhang, C.L.Schoch, J. Fourn., Crous & K.D.Hyde
+Ying M.Li & R.G.Shivas
 Yonesh.
 Yoshim.
 Yoshim. & Elix
 Yoshimatsu, Toriumi & J.D.Dodge
 Yoshino
 Yoshiz.
 Young
 Young ex Pers.
 Yunck.
 Z.G.Abad, J.A.Abad & Louws
+Z.G.Abad, J.A.Abad, T.I.Burgess & Mostowf.
+Z.G.Abad, W.Gut. & T.I.Burgess
 Z.Iwats.
-Z.Iwats. H.P.Ramsay & Fife
 Z.Kaplan, Fehrer & Hellq.
+Z.L.Luo, K.D.Hyde & Hong Y.Su
+Z.L.Luo, Maharachch. & K.D.Hyde
 Z.Q.Yuan
 Z.Q.Yuan & C.Mohammed
 Z.Q.Yuan & Kile
+Z.Q.Yuan & M.E.Barr
 Z.Q.Yuan & Old
-Z.Q.Yuan, C.Mohammed & Rudman
-Z.Q.Yuan, C.Mohammed & Wardlaw
+Z.Q.Yuan, Rudman & C.Mohammed
+Z.Q.Yuan, Wardlaw & C.Mohammed
 Z.Q.Yuan, de Little & C.Mohammed
+Z.W.de Beer, T.A.Duong & M.J.Wingf.
 Zach.
 Zacharias
 Zahlbr.
 Zalessky
 Zanardini
 Zanardini ex Bornet & Flahault
 Zanardini ex Frauenf.
 Zanardini ex Grunow
 Zanardini ex Kütz.
 Zaneveld
+Zaneveld & R.B.Sanford
+Zanten
 Zare & W.Gams
 Zeh
 Zeller
+Zeller & C.W.Dodge
 Zemann
 Zender
 Zenker
 Zich & A.J.Ford
 Zich & B.Gray
 Zikes
 Zimm.
@@ -32413,43 +32631,47 @@
 Zipp. ex Decne.
 Zipp. ex Kurz
 Zipp. ex Lév.
 Zipp. ex Miq.
 Zipp. ex Zoll.
 Ziz ex Bisch.
 Zmitr.
+Zmitr. & Kovalenko
+Zmitr. & Malysheva
 Zobel
 Zohary & Katzn.
 Zohary & Lerner
 Zohary & Waisel
 Zoll.
 Zoll. & Moritzi
 Zoll. ex Miq.
 Zopf
 Zotov
 Zschacke
 Zubcova
 Zucc.
 Zuccagni
 Zuccarello & J.A.West
+Zuccaro & M.Weiss
 Zukal
 Zuloaga
 Zundel
 Zwickel
 auct.
-d'Orbigny
 d'Urv.
 de Bary
 de Bary & Rostaf.
 de Bary & Woronin
 de Bary ex Hirn
 de Bary ex Jancz.
 de Hoog
+de Hoog & Arx
+de Hoog & G.A.de Vries
 de Hoog & H.C.Evans
-de Hoog, E.Guého & M.T.Sm.
+de Hoog, M.T.Sm. & E.Guého
 de Hoog, Mayser & Haase
 de Hoog, Oorschot & Hijwegen
 de Jonch. & Hennipman
 de Kok
 de Lange
 de Lange, Heenan & M.I.Dawson
 de Lange, R.O.Gardner, Sykes, Crowcroft, E.K.Cameron, F.Stalker, M.L.Christian & Braggins
@@ -32464,18 +32686,23 @@
 de Salas, Bolch, Botes & Hallegr.
 de Vriese
 de Vriese ex Benth.
 de Wet
 de Wet & J.R.Harlan
 de la Rosa & Messuti
 van Meel
+van Nieuwenh. & Samson
+van Nieuwenh., Miądl. & Samson
+van Nieuwenh., Miądl., Houbraken, Adan, Lutzoni & Samson
+van Nieuwenh., Miądl., Lutzoni & Samson
 Á.Löve
 Á.Löve & D.Löve
 Åke Berg
 Åke Berg ex A.Cleve
 Ångstr.
 Ångstr. ex F.M.Bailey
 É.Desv.
 É.J.Marchal
 É.Morren
+Örstadius & E.Larss.
 Østrup
 Øvstedal
```

### Comparing `hespi-0.4.2/hespi/data/family.txt` & `hespi-0.4.4/hespi/data/family.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 Achyranthaceae
 Acinetosporaceae
 Acmopylaceae
 Aconitaceae
 Acrasiaceae
 Acristaceae
 Acrobolbaceae
+Acrocalymmaceae
 Acrochaetiaceae
+Acrocladiaceae
 Acrospermaceae
 Acrostichaceae
 Acrosymphytaceae
 Acrotylaceae
 Actaeaceae
 Actinidiaceae
 Actiniopteridaceae
@@ -79,14 +81,15 @@
 Allioniaceae
 Allisoniaceae
 Allophylaceae
 Aloaceae
 Aloeaceae
 Alooideae
 Alopecuraceae
+Alphamycetaceae
 Alpiniaceae
 Alseuosmiaceae
 Alsinaceae
 Alsinastraceae
 Alsodeiaceae
 Alstroemeriaceae
 Amanitaceae
@@ -161,15 +164,14 @@
 Aphyllanthaceae
 Apiaceae
 Apiosporaceae
 Apocineae
 Apocynaceae
 Apodanthaceae
 Aponogetonaceae
-Aponogetonales
 Aporosaceae
 Aposeridaceae
 Apostasiaceae
 Aptandraceae
 Aquifoliaceae
 Aquilariaceae
 Aquilarinae
@@ -293,14 +295,15 @@
 Baueraceae
 Bauhiniaceae
 Baxteriaceae
 Begoniaceae
 Belangeraceae
 Bellerocheaceae
 Belloniaceae
+Beltraniaceae
 Belvisiaceae
 Bembiciaceae
 Bennettiaceae
 Berberidaceae
 Berberidopsidaceae
 Berkeleyaceae
 Berryaceae
@@ -313,19 +316,17 @@
 Betulideae
 Biatorellaceae
 Bicosoecaceae
 Biddulphiaceae
 Bifariaceae
 Bignoniaceae
 Bignoniae
-Bignoniales
 Bionectriaceae
 Bischofiaceae
 Bixaceae
-Bixales
 Bixinae
 Blakeaceae
 Blakwelliaceae
 Blandfordiaceae
 Blasiaceae
 Blastocladiaceae
 Blattiaceae
@@ -387,43 +388,45 @@
 Bryaceae
 Bryobartramiaceae
 Bryoniaceae
 Bryopsidaceae
 Buchneraceae
 Bucidaceae
 Bucklandiaceae
+Buckleyzymaceae
 Buddlejaceae
 Bueseraceae
 Buglossaceae
 Bulbocodiaceae
 Bulgariaceae
+Bulleraceae
 Bumeliaceae
 Bupleuraceae
 Burchardiaceae
 Burmanniaceae
 Burseraceae
 Butneriaceae
 Buttneriaceae
 Buxaceae
 Buxbaumiaceae
 Byblidaceae
 Byttneriaceae
-Byttneriales
 Cabombaceae
 Cacaoaceae
 Cactaceae
 Caesalpiniaceae
 Caladiaceae
 Calamaceae
 Calceolariaceae
 Calectasiaceae
 Calendulaceae
 Caliciaceae
 Callaceae
 Callicomaceae
+Callicostaceae
 Calliergonaceae
 Calligonaceae
 Callithamniaceae
 Callitrichaceae
 Callitrichinae
 Calochortaceae
 Calomniaceae
@@ -529,14 +532,15 @@
 Cereaceae
 Cerinthaceae
 Ceroxylaceae
 Cestraceae
 Chaconiaceae
 Chaetangiaceae
 Chaetocerotaceae
+Chaetomellaceae
 Chaetomiaceae
 Chaetopeltidaceae
 Chaetophoraceae
 Chaetosphaeriaceae
 Chaetosphaeridiaceae
 Chaetothyriaceae
 Chailletiaceae
@@ -576,14 +580,15 @@
 Chromulinaceae
 Chroococcaceae
 Chroococcidiopsidaceae
 Chroomonadaceae
 Chrysamoebaceae
 Chrysobalanaceae
 Chrysobalaneae
+Chrysoblastellaceae
 Chrysocapsaceae
 Chrysococcaceae
 Chrysophyceae familia incertae sedis
 Chrysosaccaceae
 Chrysospleniaceae
 Chrysotrichaceae
 Chytridiaceae
@@ -591,21 +596,21 @@
 Ciceraceae
 Cichoriaceae
 Cimicifugaceae
 Cinchonaceae
 Circaeaceae
 Cissaceae
 Cistaceae
-Cistales
 Cisti
 Citraceae
 Cladochytriaceae
 Cladoniaceae
 Cladophoraceae
 Cladopyxidaceae
+Cladoriellaceae
 Cladostephaceae
 Clastodermataceae
 Claustulaceae
 Clavariaceae
 Clavariadelphaceae
 Clavicipitaceae
 Clavulinaceae
@@ -626,14 +631,15 @@
 Coccodiniaceae
 Coccoideaceae
 Coccolithophyceae familia incertae sedis
 Coccomyxaceae
 Cocconeidaceae
 Coccotremataceae
 Cochicaceae
+Cochlearomycetaceae
 Cochlospermaceae
 Cochlospermeae
 Cocosaceae
 Codiaceae
 Codonosigaceae
 Coelomomycetaceae
 Coelosphaeriaceae
@@ -716,14 +722,15 @@
 Cryptomonadaceae
 Cubiculosporaceae
 Cucurbitaceae
 Cucurbitariaceae
 Cunninghamellaceae
 Cunoniaceae
 Cupressaceae
+Cupuliferae
 Curcumaceae
 Cuscutaceae
 Cuspariaceae
 Cutleriaceae
 Cyananthaceae
 Cyanastraceae
 Cyanellaceae
@@ -733,14 +740,15 @@
 Cyatheaceae
 Cyathodiaceae
 Cycadaceae
 Cyclantheraceae
 Cyclocheilaceae
 Cyclophoraceae
 Cydoniaceae
+Cylindriaceae
 Cylindrocapsaceae
 Cymatosiraceae
 Cymbellaceae
 Cymodoceaceae
 Cynanchaceae
 Cynaraceae
 Cynocrambaceae
@@ -812,21 +820,23 @@
 Dichapetaleae
 Dichondraceae
 Dichotomosiphonaceae
 Dicksoniaceae
 Dicksonieae
 Diclidantheraceae
 Dicranaceae
+Dicranellaceae
 Dicranemataceae
 Dicrastylidaceae
 Dictamnaceae
 Dictydiaethaliaceae
 Dictyoneidaceae
 Dictyonemataceae
 Dictyosphaeriaceae
+Dictyosporiaceae
 Dictyosteliaceae
 Dictyotaceae
 Didiereaceae
 Didymellaceae
 Didymiaceae
 Didymocarpaceae
 Didymosphaeriaceae
@@ -838,15 +848,14 @@
 Dinobryaceae
 Dinophyceae familia incertae sedis
 Dinophysaceae
 Dinosphaeraceae
 Dinotrichaceae
 Dionaeaceae
 Dioncophyllaceae
-Dioncophyllales
 Dioscoreaceae
 Dioscoreae
 Diosmaceae
 Diospyraceae
 Diphylleiaceae
 Diphysciaceae
 Diplaziopsidaceae
@@ -857,14 +866,15 @@
 Dipodascaceae
 Dipsacaceae
 Dipsaceae
 Dipteridaceae
 Dipterocarpaceae
 Disanthaceae
 Discinaceae
+Discosiaceae
 Discosporangiaceae
 Dissoconiaceae
 Distichiaceae
 Ditrichaceae
 Diversisporaceae
 Doassansiaceae
 Doassansiopsidaceae
@@ -961,14 +971,15 @@
 Erodiaceae
 Erpodiaceae
 Erratomycetaceae
 Erycibaceae
 Eryngiaceae
 Erysimaceae
 Erysiphaceae
+Erythrobasidiaceae
 Erythroniaceae
 Erythropalaceae
 Erythrospermaceae
 Erythrotrichiaceae
 Erythroxylaceae
 Erythroxyleae
 Escalloniaceae
@@ -999,14 +1010,15 @@
 Exobasidiaceae
 Exocarpaceae
 Exormothecaceae
 Fabaceae
 Fabroniaceae
 Fagaceae
 Fagineae
+Falcocladiaceae
 Faucheaceae
 Ferulaceae
 Festucaceae
 Ficaceae
 Filices
 Fissidentaceae
 Fistulinaceae
@@ -1037,14 +1049,15 @@
 Fugosiaceae
 Fumariaceae
 Funariaceae
 Fungi Family
 Funkiaceae
 Furcellariaceae
 Fuscideaceae
+Fusculinaceae
 Gaiadendraceae
 Gainiaceae
 Galanthaceae
 Galaxauraceae
 Galaxiaceae
 Galedupaceae
 Galeniaceae
@@ -1077,14 +1090,15 @@
 Gesnerieae
 Gethyllidaceae
 Gigartinaceae
 Gigaspermaceae
 Gigasporaceae
 Gilliesiaceae
 Ginalloaceae
+Gjaerumiaceae
 Gladiolaceae
 Glaucidiaceae
 Glaucocystaceae
 Glechomaceae
 Gleicheniaceae
 Glenodiniaceae
 Glenodiniopsidaceae
@@ -1188,15 +1202,14 @@
 Heisteriaceae
 Heleniaceae
 Heliamphoraceae
 Helianthaceae
 Helianthemaceae
 Helicobasidiaceae
 Heliconiaceae
-Helicophyllaceae
 Helicteraceae
 Heliopeltaceae
 Heliotropiaceae
 Helleboraceae
 Helminthosphaeriaceae
 Helminthostachyaceae
 Helosaceae
@@ -1210,14 +1223,15 @@
 Hemimeridaceae
 Hemiphylacaceae
 Henriqueziaceae
 Heppiaceae
 Herbertaceae
 Hericiaceae
 Hermanniaceae
+Hermatomycetaceae
 Hernandiaceae
 Herniariaceae
 Herpotrichiellaceae
 Hesperocallidaceae
 Heterantheraceae
 Heterocapsaceae
 Heterodeaceae
@@ -1285,27 +1299,27 @@
 Hygrophoraceae
 Hygrophoropsidaceae
 Hylocomiaceae
 Hymeneliaceae
 Hymenocardiaceae
 Hymenochaetaceae
 Hymenocladiaceae
+Hymenolomataceae
 Hymenophyllaceae
 Hymenophylleae
 Hymenophytaceae
 Hyoscyamaceae
 Hypecoaceae
 Hypericaceae
 Hyphochytriaceae
 Hypnaceae
 Hypneaceae
 Hypnodendraceae
 Hypnomonadaceae
 Hypocreaceae
-Hypogymniaceae
 Hyponectriaceae
 Hypopterygiaceae
 Hypoxidaceae
 Hypoxideae
 Hysterangiaceae
 Hysteriaceae
 Icacinaceae
@@ -1313,14 +1327,15 @@
 Idiospermaceae
 Ilicaceae
 Illecebraceae
 Illigeraceae
 Impatientaceae
 Imperatoriaceae
 Incertae sedis
+Induratiaceae
 Inkyuleeaceae
 Inocarpaceae
 Inocybaceae
 Inulaceae
 Iodaceae
 Iodosphaeriaceae
 Ionidiaceae
@@ -1406,16 +1421,16 @@
 Lejeuneaceae
 Lemaneaceae
 Lembophyllaceae
 Lemnaceae
 Lennoaceae
 Lentariaceae
 Lentibulariaceae
-Lentinaceae
 Lentiscaceae
+Lentitheciaceae
 Leoniaceae
 Leonticaceae
 Leotiaceae
 Lepicoleaceae
 Lepidocarpaceae
 Lepidocaryaceae
 Lepidocerataceae
@@ -1426,15 +1441,14 @@
 Leptodontaceae
 Leptolegniaceae
 Leptolegniellaceae
 Leptolyngbyaceae
 Leptosiraceae
 Leptospermaceae
 Leptosphaeriaceae
-Leptostomaceae
 Leptostomataceae
 Lepturaceae
 Lepyrodontaceae
 Leskeaceae
 Lessoniaceae
 Letrouitiaceae
 Leucobryaceae
@@ -1488,15 +1502,14 @@
 Lopeziaceae
 Lophiostomataceae
 Lophiraceae
 Lophocoleaceae
 Lophophytaceae
 Loranthaceae
 Lotaceae
-Lowiales
 Loxogrammaceae
 Lulworthiaceae
 Lunulariaceae
 Lupulaceae
 Luxemburgiaceae
 Luzuriagaceae
 Lychnidaceae
@@ -1530,15 +1543,14 @@
 Malpighiaceae
 Malpighiae
 Malvaceae
 Mangiaceae
 Manicariaceae
 Mapaniaceae
 Marantaceae
-Marantales
 Marasmiaceae
 Marathraceae
 Marattiaceae
 Marattiae
 Marchantiaceae
 Marsileaceae
 Martyniaceae
@@ -1558,14 +1570,15 @@
 Meesiaceae
 Megalariaceae
 Megalosporaceae
 Megasporaceae
 Melaleucaceae
 Melampsoraceae
 Melampyraceae
+Melanascomaceae
 Melanconidaceae
 Melanommataceae
 Melanotaeniaceae
 Melanthiaceae
 Melaspileaceae
 Melastomaceae
 Melastomae
@@ -1579,15 +1592,14 @@
 Melissaceae
 Melittidaceae
 Melochiaceae
 Melosiraceae
 Memecylaceae
 Mendonciaceae
 Menispermaceae
-Menispermales
 Menispermeae
 Menthaceae
 Menyanthaceae
 Menyanthideae
 Menziesiaceae
 Mercurialaceae
 Merenderaceae
@@ -1616,14 +1628,15 @@
 Microcoleaceae
 Microcystaceae
 Micropeltidaceae
 Microsporaceae
 Microthamniaceae
 Microtheliopsidaceae
 Microthyriaceae
+Mielichhoferiaceae
 Miliaceae
 Miltideaceae
 Milulaceae
 Mimosaceae
 Minuartiaceae
 Mirabilidaceae
 Mitteniaceae
@@ -1652,14 +1665,15 @@
 Moringaceae
 Moringeae
 Morosphaeriaceae
 Mortierellaceae
 Mouriraceae
 Moutabeaceae
 Muntingiaceae
+Murramarangomycetaceae
 Musaceae
 Mutisiaceae
 Mycenaceae
 Mychodeaceae
 Mychodeophyllaceae
 Mycoblastaceae
 Mycocaliciaceae
@@ -1671,15 +1685,17 @@
 Myoporinae
 Myriangiaceae
 Myricaceae
 Myriniaceae
 Myriophyllaceae
 Myristicaceae
 Myristiceae
+Myrmecridiaceae
 Myrobalanaceae
+Myrotheciomycetaceae
 Myrrhiniaceae
 Myrsinaceae
 Myrtaceae
 Myrti
 Mystropetalaceae
 Mytilinidiaceae
 Myuriaceae
@@ -1704,16 +1720,19 @@
 Neidiaceae
 Neilliaceae
 Nelsoniaceae
 Nelumbonaceae
 Nemacladaceae
 Nemastomataceae
 Neocallimastigaceae
+Neocelosporiaceae
 Neochloridaceae
+Neocrinulaceae
 Neohodgsoniaceae
+Neolauriomycetaceae
 Neoralfsiaceae
 Neotrichocoleaceae
 Neottiaceae
 Neozygitaceae
 Nepenthaceae
 Nepenthideae
 Nepetaceae
@@ -1735,34 +1754,36 @@
 Nonateliaceae
 Nopaleaceae
 Nostocaceae
 Nostochopsidaceae
 Notheiaceae
 Nothofagaceae
 Notothyladaceae
+Nowamycetaceae
 Nupharaceae
 Nuytsiaceae
 Nyctaginaceae
 Nyctanthaceae
 Nymphaeaceae
 Nypaceae
 Nyssaceae
 Obolariaceae
+Occultibambusaceae
 Ochnaceae
 Ochrolechiaceae
 Ochromonadaceae
 Octoblepharaceae
 Octoknemaceae
+Odontellaceae
 Odontotremataceae
 Oedogoniaceae
 Oenotheraceae
 Oftiaceae
 Olacaceae
 Olacinae
-Olacineae
 Oleaceae
 Oleandraceae
 Oleandreae
 Olpidiaceae
 Olpidiopsidaceae
 Olyraceae
 Omphalotaceae
@@ -1794,16 +1815,18 @@
 Orchideae
 Ornithogalaceae
 Ornithropaceae
 Orobanchaceae
 Orontiaceae
 Ortegaceae
 Orthodontiaceae
+Orthogonacladiaceae
 Orthorrhynchiaceae
 Orthoseiraceae
+Orthosticellaceae
 Orthotrichaceae
 Oryzaceae
 Oscillatoriaceae
 Osmundaceae
 Ostreobiaceae
 Osyridaceae
 Otteliaceae
@@ -1834,17 +1857,19 @@
 Pannariaceae
 Papaveraceae
 Papayaceae
 Papilionaceae
 Papillionaceae
 Pappophoraceae
 Papyraceae
+Paracladophialophoraceae
 Paracryphiaceae
 Paraliaceae
 Paraphysomonadaceae
+Pararamichloridiaceae
 Parataeniellaceae
 Parianaceae
 Parietariaceae
 Parkeriaceae
 Parmeliaceae
 Parmulariaceae
 Parodiellaceae
@@ -1902,15 +1927,14 @@
 Phacidiaceae
 Phacotaceae
 Phaeochoraceae
 Phaeophilaceae
 Phaeophyceae familia incertae sedis
 Phaeosphaeriaceae
 Phaeothamniaceae
-Phaeotrichaceae
 Phaffomycetaceae
 Phakopsoraceae
 Phalansteriaceae
 Phalaridaceae
 Phaleriaceae
 Phallaceae
 Phallogastraceae
@@ -1939,14 +1963,15 @@
 Phylicaceae
 Phyllachoraceae
 Phyllanthaceae
 Phyllocladaceae
 Phyllophoraceae
 Phyllopsoraceae
 Phyllosiphonaceae
+Phyllostictaceae
 Phymatocerotaceae
 Physalacriaceae
 Physaraceae
 Physciaceae
 Physodermataceae
 Phytelephantaceae
 Phytocrenaceae
@@ -2010,14 +2035,15 @@
 Pluteaceae
 Pneumocystidaceae
 Poaceae
 Podoaceae
 Podocarpaceae
 Podolampadaceae
 Podophyllaceae
+Podosporaceae
 Podostemaceae
 Podostemeae
 Polemonia
 Polemoniaceae
 Poliothyrsidaceae
 Polpodaceae
 Polycarpaeaceae
@@ -2037,14 +2063,15 @@
 Polytrichaceae
 Pongatiaceae
 Pontederiaceae
 Poranaceae
 Porantheraceae
 Porellaceae
 Porinaceae
+Porodiplodiaceae
 Porotheleaceae
 Porphyridiaceae
 Porpidiaceae
 Portulacaceae
 Portulacariaceae
 Portulaceae
 Posidoniaceae
@@ -2074,17 +2101,19 @@
 Psammodiscaceae
 Psathyrellaceae
 Pseliaceae
 Pseudanabaenaceae
 Pseudanthaceae
 Pseudocharaciopsidaceae
 Pseudocodiaceae
+Pseudodactylariaceae
 Pseudolepicoleaceae
 Pseudoperisporiaceae
 Pseudophoenicaceae
+Pseudosporidesmiaceae
 Pseudovalsaceae
 Psilotaceae
 Psiloteae
 Psiloxylaceae
 Psittacanthaceae
 Psoraceae
 Psychotriaceae
@@ -2107,14 +2136,15 @@
 Pucciniaceae
 Pucciniastraceae
 Pucciniosiraceae
 Pulchrinodaceae
 Punicaceae
 Puniceae
 Putranjivaceae
+Pylaisiaceae
 Pylaisiadelphaceae
 Pyraceae
 Pyramimonadaceae
 Pyrenomonadaceae
 Pyrenothricaceae
 Pyrenulaceae
 Pyrocystaceae
@@ -2145,14 +2175,15 @@
 Raveneliaceae
 Reaumuriaceae
 Repetobasidiaceae
 Requienellaceae
 Resedaceae
 Restionaceae
 Rhabdodendraceae
+Rhabdodontiaceae
 Rhabdonemataceae
 Rhabdoweisiaceae
 Rhachidosoraceae
 Rhacocarpaceae
 Rhamnaceae
 Rhamni
 Rhamphosporaceae
@@ -2184,18 +2215,18 @@
 Rhodophyta familia incertae sedis
 Rhodoraceae
 Rhodothamniellaceae
 Rhodotypaceae
 Rhodymeniaceae
 Rhoicospheniaceae
 Rhoipteleaceae
-Rhoipteleales
 Rhopalocarpaceae
 Rhopalodiaceae
 Rhopalosolenaceae
+Rhynchogastremaceae
 Rhynchomonadidae
 Rhynchostomataceae
 Rhytismataceae
 Ribesiaceae
 Ricciaceae
 Ricinaceae
 Ricinocarpaceae
@@ -2219,14 +2250,15 @@
 Rutaceae
 Rutstroemiaceae
 Sabalaceae
 Sabiaceae
 Sabiceaceae
 Sabulinaceae
 Saccharaceae
+Saccharataceae
 Saccharomycetaceae
 Saccharomycodaceae
 Saccifoliaceae
 Sagaceae
 Saginaceae
 Sagoneaceae
 Saksenaeaceae
@@ -2262,18 +2294,20 @@
 Sarcophytaceae
 Sarcoscyphaceae
 Sarcosomataceae
 Sarcospermataceae
 Sarcostigmataceae
 Sargassaceae
 Sargentodoxaceae
+Sarocladiaceae
 Sarraceniaceae
 Sarrameanaceae
 Saulomataceae
 Saurauiaceae
+Saururaceae
 Sauvagesiaceae
 Saxifragaceae
 Saxifragae
 Scabiosaceae
 Scaevolaceae
 Scandicaceae
 Scapaniaceae
@@ -2394,27 +2428,31 @@
 Sphenostemonaceae
 Sphinctrinaceae
 Spielmanniaceae
 Spigeliaceae
 Spinaciaceae
 Spiraeaceae
 Spiraeanthemaceae
+Spiridentaceae
 Spirulinaceae
 Spizellomycetaceae
 Splachnaceae
 Splachnidiaceae
 Splachnobryaceae
 Spondiadaceae
 Spondylomoraceae
 Spongomonadidae
 Sporastatiaceae
+Sporidesmiaceae
+Sporocadaceae
 Sporochnaceae
 Sporolithaceae
 Sporormiaceae
 Spyridiaceae
+Stachybotriaceae
 Stachydaceae
 Stackhouseae
 Stackhousiaceae
 Stangeriaceae
 Stanleyaceae
 Stapeliaceae
 Staticaceae
@@ -2431,15 +2469,14 @@
 Stereaceae
 Stereocaulaceae
 Stereophyllaceae
 Stictidaceae
 Stictodiscaceae
 Stigonemataceae
 Stilaginaceae
-Stilaginales
 Stipaceae
 Stratiotaceae
 Strelitziaceae
 Strelitziineae
 Streptochaetaceae
 Streptothecaceae
 Striatellaceae
@@ -2451,22 +2488,25 @@
 Stylideae
 Stylidiaceae
 Stylobasiaceae
 Stylococcaceae
 Stylonemataceae
 Stypheliaceae
 Stypocaulaceae
+Styracaceae
 Suessiaceae
 Suillaceae
 Sumachiaceae
+Superstratomycetaceae
 Surianaceae
 Surianeae
 Surirellaceae
 Swartziaceae
 Swieteniaceae
+Symmetrosporaceae
 Symphoremataceae
 Symphyodontaceae
 Symphyonemataceae
 Symplocaceae
 Symploceae
 Syncephalastraceae
 Synchytriaceae
@@ -2491,14 +2531,15 @@
 Tanacetaceae
 Taphrinaceae
 Tapinellaceae
 Targioniaceae
 Taxodiaceae
 Tecophilaeaceae
 Tectariaceae
+Teichosporaceae
 Telephiaceae
 Teloschistaceae
 Tepuianthaceae
 Teratosphaeriaceae
 Terebinthaceae
 Terminaliaceae
 Ternstroemiaceae
@@ -2549,14 +2590,15 @@
 Tithymalaceae
 Togniniaceae
 Tolypothrichaceae
 Tormentillaceae
 Tovelliaceae
 Toxariaceae
 Trachylomataceae
+Tracyllaceae
 Tradescantiaceae
 Tragiaceae
 Trapaceae
 Trapeliaceae
 Trapellaceae
 Trebouxiaceae
 Trebouxiophyceae familia incertae sedis
@@ -2583,14 +2625,15 @@
 Trichotemnomataceae
 Trichotheliaceae
 Tricyrtidaceae
 Trifoliaceae
 Triglochinaceae
 Trigoniaceae
 Trimeniaceae
+Trimorphomycetaceae
 Triplobaceae
 Triplostegiaceae
 Tripterellaceae
 Tristeginaceae
 Tristichaceae
 Triticaceae
 Triuridaceae
@@ -2681,19 +2724,21 @@
 Xanthonemataceae
 Xanthophyllaceae
 Xanthopyreniaceae
 Xanthorhaeaceae
 Xanthorhizaceae
 Xanthorrhoeaceae
 Xenasmataceae
+Xenospadicoidaceae
 Xeranthemaceae
 Xerotaceae
 Ximeniaceae
 Xiphidiaceae
 Xiphophoraceae
+Xyladictyochaetaceae
 Xylariaceae
 Xyridaceae
 Yuccaceae
 Zamiaceae
 Zannichelliaceae
 Zanoniaceae
 Zanthoxylaceae
@@ -2704,8 +2749,7 @@
 Zoopagaceae
 Zopfiaceae
 Zosteraceae
 Zoysiaceae
 Zygnemataceae
 Zygophyllaceae
 Zygophylleae
-[Family Not Recorded]
```

### Comparing `hespi-0.4.2/hespi/data/genus.txt` & `hespi-0.4.4/hespi/data/genus.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 Achnanthepyla
 Achnanthes
 Achnanthidium
 Achnatherum
 Achneria
 Achnophora
 Achras
+Achrochaeta
 Achromolaena
 Achrophyllum
 Achryanthes
 Achrysum
 Achyrantes
 Achyranthes
 Achyrodes
@@ -225,14 +226,15 @@
 Adiantum
 Adomia
 Adonis
 Adrastaea
 Adrastea
 Adriana
 Adriania
+Adustoporia
 Aecidium
 Aegagropila
 Aegerita
 Aegialinites
 Aegialites
 Aegialitis
 Aegiceras
@@ -281,14 +283,15 @@
 Agathomeris
 Agathosma
 Agathosoma
 Agati
 Agave
 Ageratina
 Ageratum
+Aggreflorum
 Agiortia
 Aglaia
 Aglaiopsis
 Aglaomorpha
 Aglaonema
 Aglaophyllum
 Aglaothamnion
@@ -298,14 +301,15 @@
 Agonimia
 Agonis
 Agonizanthos
 Agonomyrtus
 Agonon
 Agricolaea
 Agrimonia
+Agroathelia
 Agrocybe
 Agrophyllum
 Agropogon
 Agropyron
 Agropyrum
 Agrostema
 Agrostemma
@@ -325,38 +329,42 @@
 Ailantus
 Aillya
 Ainoa
 Aira
 Airopsis
 Aithaloderma
 Aitonia
+Aizoago
 Aizoon
 Ajuga
 Akalaphycus
 Akania
+Akanthomyces
 Akashiwo
 Akebia
 Alangium
 Alania
 Alaria
 Alatospora
 Albatrellus
 Albidella
 Albizia
 Albizzia
+Alboefibula
 Alboleptonia
 Albonectria
 Albuca
 Albugo
 Alcea
 Alchemilla
 Alchimilla
 Alchornea
 Alcicornium
 Alcicularia
+Alcornia
 Aldrovanda
 Aldrovandra
 Alectoria
 Alectrion
 Alectryon
 Alephia
 Alepyrum
@@ -368,14 +376,15 @@
 Aleurocorticium
 Aleurocystis
 Aleurodiscus
 Alexandrium
 Alexfloydia
 Alexgeorgea
 Alexgeorgia
+Alfaria
 Alga
 Algarobia
 Algogrunowia
 Alhagi
 Alisma
 Alismorchis
 Alismorkis
@@ -398,25 +407,28 @@
 Alliaria
 Allisonia
 Allisoniella
 Allittia
 Allium
 Allocarya
 Allocasuarina
+Allocryptovalsa
+Alloexidiopsis
 Allographa
 Allogyne
 Allomyces
 Allophylaria
 Allophyllus
 Allophylus
 Allopterigeron
 Allorgella
 Allosorus
 Allosyncarpia
 Alloteropsis
+Allotrechispora
 Alloxylon
 Almaleea
 Alnus
 Alobiella
 Alocasia
 Aloe
 Alogyne
@@ -527,15 +539,14 @@
 Amphidoma
 Amphiglottis
 Amphiloma
 Amphilophis
 Amphilothus
 Amphinema
 Amphineuron
-Amphinomium
 Amphipentas
 Amphipleura
 Amphiplexia
 Amphipogon
 Amphiprora
 Amphiroa
 Amphirosellinia
@@ -577,14 +588,15 @@
 Anademia
 Anadenanthera
 Anadenia
 Anadyomene
 Anaeromyces
 Anagallis
 Anagalloides
+Anagnostidinema
 Anagyris
 Ananas
 Anaphalis
 Anaphora
 Anaptychia
 Anarthria
 Anasser
@@ -712,14 +724,15 @@
 Anophora
 Anopterus
 Anorthoneis
 Anosporum
 Anotis
 Anotrichium
 Anredera
+Anteaglonium
 Antennaria
 Antennariella
 Antennospora
 Antennularia
 Antheidosorus
 Anthelepis
 Anthelia
@@ -743,14 +756,15 @@
 Anthosachne
 Anthostoma
 Anthostomella
 Anthotium
 Anthotroche
 Anthoxanthum
 Anthracobia
+Anthracocystis
 Anthracoidea
 Anthracophyllum
 Anthracothecium
 Anthriscus
 Anthrophyum
 Anthropodium
 Anthropomorphus
@@ -778,27 +792,29 @@
 Antrelloides
 Antrocentrum
 Antrodia
 Antrodiella
 Antromycopsis
 Antrophyum
 Antura
+Anungitea
 Anygosanthos
 Anygozanthes
 Anygozanthos
 Anzia
 Anzybas
 Aongstroemia
 Aotus
 Apalochlamys
 Apalodium
 Apargia
 Apatelantha
 Apatophyllum
 Apaturia
+Apectospermum
 Apera
 Apetalon
 Apetalum
 Aphananthe
 Aphanes
 Aphanizomenon
 Aphanoascus
@@ -814,27 +830,31 @@
 Aphanothece
 Aphelaria
 Aphelexis
 Aphelia
 Aphylax
 Aphyllodium
 Aphyllorchis
+Apinisia
 Apiocystis
+Apiognomonia
+Apioperdon
 Apiospora
 Apiothyrium
 Apium
 Apjohnia
 Aplochlamis
 Aplopappus
 Aplosporella
 Aplostellis
 Aplotaxis
 Aplozia
 Apluda
 Apocalathium
+Apocissus
 Apocopis
 Apodasmia
 Apodochloris
 Apodospora
 Apodytes
 Apogeton
 Apogloeum
@@ -876,14 +896,15 @@
 Arachne
 Arachniodes
 Arachnion
 Arachniopsis
 Arachniotus
 Arachnomyces
 Arachnopeziza
+Arachnophora
 Arachnorchis
 Aralia
 Araucaria
 Araujia
 Arbutus
 Arcangeliella
 Archaeolithothamnion
@@ -896,17 +917,19 @@
 Archidendropsis
 Archidium
 Archidondron
 Archilejeunea
 Archirhodomyrtus
 Archontophoenix
 Arctium
+Arctoa
 Arctomia
 Arctotheca
 Arctotis
+Arcuatospora
 Arcyria
 Ardhachandra
 Ardisia
 Ardissonea
 Arduina
 Areca
 Arecastrum
@@ -948,15 +971,14 @@
 Armatella
 Armillaria
 Armillariella
 Armitia
 Arnellia
 Arnhemia
 Arnica
-Arnium
 Arnocrinum
 Arnopogon
 Arnoseris
 Aromadendrum
 Aroramyces
 Arrhenatherum
 Arrhenechthites
@@ -992,14 +1014,15 @@
 Arthrosolen
 Arthrospira
 Arthrosprion
 Arthrostygma
 Arthrostyles
 Arthrostylis
 Arthrotaxis
+Arthrotrichium
 Arthrotrichum
 Artocarpus
 Artomyces
 Arum
 Aruncus
 Arundarbor
 Arundina
@@ -1043,15 +1066,14 @@
 Asperococcus
 Asperopilum
 Asperoporum
 Asperula
 Asphodelus
 Aspicilia
 Aspiciliopsis
-Aspidelia
 Aspidella
 Aspidistra
 Aspidium
 Aspidixia
 Aspidothelium
 Aspilia
 Asplenidictyum
@@ -1092,15 +1114,14 @@
 Asteromella
 Asteromenia
 Asteromphalus
 Asteromyrtus
 Asteronema
 Asterophlyctis
 Asterophora
-Asteropsis
 Asterostomella
 Asterostroma
 Asterostromella
 Asterotremella
 Asterotricha
 Asterotrichion
 Asterotrichon
@@ -1127,14 +1148,15 @@
 Atalaya
 Atelandra
 Atelocauda
 Athalamia
 Athallia
 Athelia
 Athelopsis
+Atheniella
 Atherocephala
 Atherosperma
 Athertonia
 Athrixia
 Athrodactylis
 Athroisma
 Athrotaxis
@@ -1142,15 +1164,15 @@
 Athyrium
 Atichia
 Atkinsonia
 Atractiella
 Atractobolus
 Atractocarpus
 Atractomorpha
-Atractylis
+Atrichopsis
 Atrichum
 Atriplex
 Atropa
 Atropis
 Atroporus
 Attheya
 Atylosia
@@ -1164,48 +1186,56 @@
 Aulaxina
 Auliscus
 Aulographum
 Aulosira
 Auranticarpa
 Aurantiosacculus
 Aurantiporus
+Aurantipostia
 Aurantium
 Auratiopycnidiella
 Aureobasidium
 Aureolejeunea
+Aureonarius
 Auricularia
 Auriculariopsis
 Aurificaria
 Auriscalpium
 Auritella
 Aurophora
 Austariella
+Austeria
 Austinia
 Australasia
 Australiaena
 Australiasca
 Australina
+Australocybe
 Australofilum
 Australohydnum
 Australopilus
 Australoporus
 Australopyrum
 Australorchis
+Australosphaerella
 Austrella
+Austroacremonium
+Austroafricana
 Austrobaeckea
 Austrobaileya
 Austrobassia
 Austroblastenia
 Austroblechnum
 Austroboletus
 Austrobryonia
 Austrobuxus
 Austrocallerya
 Austrochloris
 Austroclonium
+Austrocortinarius
 Austrocylindropuntia
 Austrocynoglossum
 Austrodanthonia
 Austroderia
 Austrodolichos
 Austroeupatorium
 Austrofestuca
@@ -1227,14 +1257,17 @@
 Austronereia
 Austroparmelina
 Austropaxillus
 Austropeltum
 Austrophyllis
 Austroplaca
 Austropleospora
+Austroporia
+Austropostia
+Austropuccinia
 Austroriella
 Austroscyphus
 Austrosmittium
 Austrosteenisia
 Austrostipa
 Austrothamnium
 Avellinia
@@ -1266,14 +1299,15 @@
 Baccharis
 Bachelotia
 Bacidia
 Bacidina
 Bacillaria
 Backhousea
 Backhousia
+Backusella
 Bacopa
 Bacteriastrum
 Bactridium
 Bactrilobium
 Bactrodesmium
 Bactrophora
 Bactrospora
@@ -1333,15 +1367,19 @@
 Bancksia
 Bangia
 Banisteria
 Banisterodes
 Banksea
 Banksia
 Banksiamyces
+Banksiophoma
+Banningia
+Bannoa
 Baobab
+Baobabopsis
 Baobabus
 Bapalmuia
 Barathranthus
 Baratranthus
 Barbaraea
 Barbarea
 Barbella
@@ -1428,17 +1466,19 @@
 Bellotia
 Belonia
 Belonidium
 Belonopsis
 Beloperone
 Beltrania
 Beltraniella
+Beltraniopsis
 Belvisia
 Benincasa
 Bennettella
+Benniella
 Benstonea
 Benthamia
 Benthamidia
 Benthamina
 Bentleya
 Berberidopsis
 Berberis
@@ -1516,27 +1556,29 @@
 Biophytum
 Bipolaris
 Biremis
 Bischoffia
 Bischofia
 Biscogniauxia
 Biserrula
+Bisifusarium
 Bisporella
 Bituminaria
 Bivallum
 Bixa
 Bjerkandera
 Blaberopus
 Blackallia
 Blackburnia
 Blackiella
 Blackstonia
 Blackwellia
 Bladhia
 Blainvillea
+Blakella
 Blakeochloa
 Blakwellia
 Blanca
 Blancoa
 Blandfordia
 Blandfortia
 Blasia
@@ -1711,14 +1753,15 @@
 Brachyspatha
 Brachysporiella
 Brachysporium
 Brachystachys
 Brachysteleum
 Brachystelma
 Brachystephium
+Brachytheciastrum
 Brachythecium
 Brachytrichia
 Brachyzema
 Brackenridgea
 Brackenridgia
 Bracteacoccus
 Bracteantha
@@ -1736,25 +1779,29 @@
 Brassiodendron
 Brathys
 Braunia
 Brayulinea
 Bredemeyera
 Breea
 Bremia
+Bresadolia
 Breutelia
 Brevianthus
+Brevicalcar
+Brevistachys
 Breweria
 Brewsteria
 Breynia
 Brianaria
 Bridelia
 Briedelia
 Brigantiaea
 Brillantaisia
 Briseis
+Brittonodoxa
 Briza
 Brizopyrum
 Brizula
 Brobdingnagia
 Brochosiphon
 Brockmania
 Brombya
@@ -1775,17 +1822,21 @@
 Bruchia
 Brugmansia
 Bruguiera
 Bruguieria
 Brunella
 Brunfelsia
 Brunneiapiospora
+Brunneocarpos
+Brunneofusispora
+Brunneospora
 Brunnipila
 Brunonia
 Brunoniella
+Brunswickiella
 Bryantea
 Bryantia
 Bryobartramia
 Bryobilimbia
 Bryobium
 Bryobrothera
 Bryochiton
@@ -1808,14 +1859,16 @@
 Bucetum
 Buchanania
 Bucheria
 Buchnera
 Bucholzia
 Buchwaldoboletus
 Buckinghamia
+Bucklandiella
+Buckleyzyma
 Budawangia
 Buddlea
 Buddleia
 Buddleja
 Budhanggurabania
 Buechnera
 Buechnica
@@ -1830,14 +1883,15 @@
 Bulbinopsis
 Bulbochaete
 Bulbophyllum
 Bulbostylis
 Bulbothrix
 Bulgaria
 Bulgariella
+Bullanockia
 Bullatina
 Bulliarda
 Bulweria
 Bumilleria
 Bunchosia
 Bunnya
 Bunochilus
@@ -1901,21 +1955,21 @@
 Caeomurus
 Caeruleum
 Caesalpina
 Caesalpinia
 Caesia
 Cahya
 Cailliea
+Cairneyella
 Cajan
 Cajanus
 Cajuputi
 Cakile
 Calaba
 Calacinum
-Calacodasya
 Caladenastrum
 Caladenia
 Caladeniastrum
 Caladium
 Calamagrostis
 Calamaria
 Calamintha
@@ -1944,19 +1998,21 @@
 Calenia
 Caleniopsis
 Calepina
 Caletia
 Caleya
 Caleyana
 Calibrachoa
+Caliciopsis
 Calicium
 Calicotome
 Calista
 Calla
 Calladium
+Callerascus
 Callerya
 Calliandra
 Calliblepharis
 Callicarpa
 Callicoma
 Callicomis
 Callicostella
@@ -2044,14 +2100,15 @@
 Calucechinus
 Calusparassus
 Calvatia
 Calvitimela
 Calycanthus
 Calycella
 Calycidium
+Calycofera
 Calycomis
 Calycomorphum
 Calycopeplus
 Calycothrix
 Calycotome
 Calyculosphaeria
 Calymella
@@ -2081,14 +2138,15 @@
 Calythropsis
 Calytrhix
 Calytrix
 Camara
 Camarophyllopsis
 Camarophyllus
 Camarosporium
+Camarosporula
 Camarotis
 Cambania
 Cambessedea
 Camelina
 Camellia
 Cameronia
 Camirium
@@ -2159,15 +2217,14 @@
 Cantuffa
 Capea
 Capillaria
 Capillipedium
 Capitoclavaria
 Capitorostrum
 Capitotricha
-Capitularia
 Capnodiastrum
 Capnodinula
 Capnodium
 Capnophyllum
 Capparis
 Capraella
 Capraria
@@ -2260,14 +2317,15 @@
 Cassiniola
 Cassutha
 Cassyta
 Cassytha
 Castagnea
 Castalia
 Castamospermum
+Castanediella
 Castanedomyces
 Castanocarpus
 Castanoclobus
 Castanospermum
 Castanospora
 Castilla
 Castilleja
@@ -2321,25 +2379,28 @@
 Caustis
 Cavinula
 Cavostelium
 Cayratia
 Ceanothus
 Cebatha
 Cebera
+Cecalyphum
 Cecarria
 Cecidiomyces
 Cecropia
 Cedrela
 Cedronella
 Cedrus
 Ceiba
 Celastrus
 Celeceras
+Celerioriella
 Celloniella
 Cellularia
+Cellulariella
 Celmisia
 Celosia
 Celothelium
 Celsia
 Celtis
 Cenacrum
 Cenangella
@@ -2359,14 +2420,15 @@
 Centosteca
 Centotheca
 Centranthera
 Centranthus
 Centratherum
 Centritractus
 Centroceras
+Centrochilus
 Centrodinium
 Centrolepidosporium
 Centrolepis
 Centromadia
 Centronella
 Centropappus
 Centrophorum
@@ -2397,14 +2459,15 @@
 Cephaloschoenus
 Cephalosorus
 Cephalosporiopsis
 Cephalosporium
 Cephalostigma
 Cephalotes
 Cephalotheca
+Cephalotrichum
 Cephalotrophis
 Cephalotus
 Cephalozia
 Cephaloziella
 Cepobaculum
 Cepsiclava
 Ceraceomerulius
@@ -2454,17 +2517,19 @@
 Cercidospora
 Cercis
 Cercodia
 Cercophora
 Cercospora
 Cercosporella
 Cercosporidium
+Cercostigmina
 Cereus
 Cerinosterus
 Cerion
+Cerioporus
 Ceriops
 Ceriospora
 Ceriosporopsis
 Ceriporia
 Ceriporiopsis
 Cerocorticium
 Ceropegia
@@ -2474,15 +2539,14 @@
 Cervicina
 Cesatia
 Cesia
 Cestichis
 Cestrum
 Ceterach
 Cetraria
-Cetrariastrum
 Cetrelia
 Ceuthospora
 Ceuthostoma
 Chadefaudia
 Chaelanthus
 Chaenomeles
 Chaenostoma
@@ -2598,14 +2662,15 @@
 Chenopodina
 Chenopodium
 Cheynia
 Cheyniana
 Chiastocaulon
 Chilianthus
 Chilocarpus
+Chilochista
 Chilodia
 Chiloglottis
 Chilomonas
 Chiloschista
 Chiloscyphus
 Chilosimpliglottis
 Chiloterus
@@ -2645,14 +2710,15 @@
 Chlorencoelia
 Chlorhormidium
 Chloridella
 Chloridium
 Chloris
 Chlorocharis
 Chlorociboria
+Chlorocillium
 Chloroclados
 Chlorocloster
 Chlorococcum
 Chlorocyperus
 Chlorodesmis
 Chlorogonium
 Chlorolobion
@@ -2795,14 +2861,15 @@
 Cinamomum
 Cincinalis
 Cineraria
 Cinna
 Cinnamomum
 Cinnamonum
 Cintractia
+Cintractiella
 Cionium
 Cionothrix
 Circinaria
 Circinella
 Circinotrichum
 Circulifolium
 Cirrenalia
@@ -2855,14 +2922,15 @@
 Cladotrichum
 Cladurus
 Clandarium
 Claopodium
 Claoxylon
 Clasmatocolea
 Clasterosporium
+Clastobryophilum
 Clastobryum
 Clastoderma
 Clathrella
 Clathrina
 Clathrocysta
 Clathrocystis
 Clathromorphum
@@ -2897,14 +2965,15 @@
 Cleidion
 Cleiostoma
 Cleisostoma
 Cleistanthus
 Cleistocalyx
 Cleistochloa
 Cleistoloranthus
+Cleistoma
 Clelandia
 Clematicissus
 Clematis
 Cleome
 Cleretum
 Clerodendron
 Clerodendrum
@@ -2922,27 +2991,29 @@
 Climacosphenia
 Clinopodium
 Clinostigma
 Cliostomum
 Clitandropsis
 Clitocybe
 Clitocybula
+Clitopiloides
 Clitopilus
 Clitoria
 Cloanthe
 Cloanthes
 Clohesyomyces
 Clohiesia
 Clompanus
 Cloniophora
 Clonostachys
 Closteridium
 Closteriopsis
 Closterium
 Clutia
+Clymene
 Clypea
 Clypeolella
 Clypeolum
 Clypeostroma
 Clytostoma
 Cnesmocarpon
 Cnicus
@@ -2961,14 +3032,15 @@
 Coccomyxa
 Cocconeiopsis
 Cocconeis
 Cocconema
 Coccostroma
 Coccotrema
 Cocculus
+Cochlearomyces
 Cochliobolus
 Cochlodinium
 Cochlospermum
 Cochranea
 Cocoicola
 Cocos
 Codariocalyx
@@ -3036,14 +3108,15 @@
 Colletia
 Colletogloeopsis
 Colletogloeum
 Colletotrichum
 Colloderma
 Collomia
 Collybia
+Collybiopsis
 Collyris
 Colmeiroa
 Colobandra
 Colobanthus
 Colocasia
 Colocynthis
 Cololejeunea
@@ -3058,14 +3131,15 @@
 Columnea
 Columnodontia
 Colura
 Colus
 Colutea
 Colymbea
 Colysis
+Coma
 Comaspermum
 Comatricha
 Combretum
 Comesperma
 Comespermea
 Commelina
 Commelyna
@@ -3164,15 +3238,14 @@
 Coriandrum
 Coridochloa
 Corinaldia
 Coringia
 Coriolopsis
 Coriolus
 Coriophyllum
-Coriscium
 Cornacchinia
 Corneohydnum
 Cornicularia
 Corniculariella
 Cornucopiella
 Cornularia
 Cornumyces
@@ -3348,14 +3421,15 @@
 Cryphaea
 Cryphia
 Cryphiacanthus
 Cryphidium
 Cryphonectria
 Crypsinus
 Crypsis
+Cryptachne
 Cryptandra
 Cryptanthemis
 Cryptanthus
 Crypthonia
 Crypticola
 Cryptocalyx
 Cryptocaria
@@ -3431,14 +3505,15 @@
 Cupanea
 Cupania
 Cupaniopsis
 Cuparilla
 Cuphea
 Cuphocybe
 Cuphonotus
+Cuphophyllus
 Cupi
 Cupia
 Cupressina
 Cupressus
 Cupulanthus
 Cupularia
 Curculigo
@@ -3457,17 +3532,19 @@
 Cyanicula
 Cyanidium
 Cyanisticta
 Cyanoarbor
 Cyanobacterium
 Cyanocarpus
 Cyanochlamys
+Cyanodermella
 Cyanolophocolea
 Cyanopulvis
 Cyanospermum
+Cyanosporus
 Cyanostegia
 Cyanothamnus
 Cyanothece
 Cyanotis
 Cyanotus
 Cyanthera
 Cyanthillium
@@ -3478,32 +3555,31 @@
 Cyathiscus
 Cyathochaeta
 Cyathochaete
 Cyathodes
 Cyathodium
 Cyathomiscus
 Cyathopappus
-Cyathophonum
 Cyathophorum
 Cyathopsis
 Cyathostemma
 Cyathostemon
 Cyathula
 Cyathus
 Cyatochaete
-Cyatophorum
 Cyatula
 Cybele
 Cyberlindnera
 Cycas
 Cyclaneusma
 Cyclanthera
 Cyclicodaphne
 Cyclocampe
 Cyclocarpa
+Cyclocybe
 Cycloderma
 Cyclodictyon
 Cyclographina
 Cyclogyne
 Cyclolejeunea
 Cycloloma
 Cyclomyces
@@ -3520,23 +3596,25 @@
 Cyclotheca
 Cycnogeton
 Cycnoseris
 Cydonia
 Cylicodaphne
 Cylindraxis
 Cylindrium
+Cylindroaseptospora
 Cylindrobasidium
 Cylindrocapsa
 Cylindrocarpon
 Cylindrocarpus
 Cylindrochytridium
 Cylindrocladiella
 Cylindrocladium
 Cylindrocolea
 Cylindrocystis
+Cylindromonium
 Cylindrophora
 Cylindropuntia
 Cylindropyxis
 Cylindrosorus
 Cylindrospermopsis
 Cylindrospermum
 Cylindrosporium
@@ -3574,14 +3652,15 @@
 Cynomorium
 Cynontodium
 Cynophallus
 Cynosurus
 Cyparissia
 Cyperochloa
 Cyperocymbidium
+Cyperorchis
 Cyperus
 Cyphanthera
 Cyphelium
 Cyphella
 Cyphellophora
 Cyphellopsis
 Cyphellostereum
@@ -3700,21 +3779,24 @@
 Dasyscyphella
 Dasyscyphus
 Dasystemon
 Dasystictella
 Dasythamniella
 Dasythamnion
 Datronia
+Datroniella
 Datura
 Daucus
 Davallia
 Davejonesia
 Davenportia
 Davidiella
+Davidiellomyces
 Davidsonia
+Davidsoniella
 Daviesia
 Daviesiu
 Davisoniella
 Dawsicola
 Dawsomyces
 Dawsonia
 Dawsoniella
@@ -3763,14 +3845,15 @@
 Dendriscocaulon
 Dendro-hypnum
 Dendro-leskea
 Dendrobates
 Dendrobium
 Dendroceros
 Dendrochaete
+Dendrochytridium
 Dendrocladium
 Dendrocnide
 Dendrocolla
 Dendroconche
 Dendrocoryne
 Dendrocryphaea
 Dendrodochium
@@ -3790,27 +3873,30 @@
 Dendropogon
 Dendrosarcus
 Dendrosporium
 Dendrothele
 Dendrotrophe
 Denea
 Denhamia
+Deniquelata
 Denisonia
 Dennisiella
 Dennisonia
 Dennstaedtia
 Denotarisia
 Densospora
 Dentella
 Denticella
 Denticula
 Denticulopsis
 Dentinum
+Dentipellicula
 Dentipellis
 Deparia
+Depazea
 Deplanchea
 Depremesnilia
 Derbesia
 Dermatea
 Dermatina
 Dermatocarpon
 Dermatodothis
@@ -3818,14 +3904,16 @@
 Dermatophlebium
 Dermatosorus
 Derminus
 Dermocybe
 Dermoloma
 Derris
 Derwentia
+Derxomyces
+Desarmillaria
 Deschampsia
 Descolea
 Descomyces
 Descurainia
 Desmanthus
 Desmarestia
 Desmatodon
@@ -3933,15 +4021,14 @@
 Dicranoweisia
 Dicranum
 Dicrastyles
 Dicrastylis
 Dicroglossum
 Dictydiaethalium
 Dictydium
-Dictymenia
 Dictymia
 Dictynia
 Dictyocephalos
 Dictyochaeta
 Dictyochloropsis
 Dictyodaphne
 Dictyogramma
@@ -3980,14 +4067,15 @@
 Didymellina
 Didymeria
 Didymium
 Didymobotryopsis
 Didymocarpus
 Didymochaeta
 Didymocheton
+Didymocyrtis
 Didymocystis
 Didymodon
 Didymoglossum
 Didymonema
 Didymopanax
 Didymoplexis
 Didymosperma
@@ -4019,14 +4107,15 @@
 Dilophus
 Dilwinia
 Dilwynia
 Dimelaena
 Dimeregramma
 Dimerella
 Dimeria
+Dimeriella
 Dimerina
 Dimerium
 Dimerosporium
 Dimetopia
 Dimocarpus
 Dimorphanthera
 Dimorphocalyx
@@ -4188,14 +4277,15 @@
 Distemma
 Distichium
 Distichlis
 Distichophyllum
 Distichostemon
 Distigma
 Distimake
+Distononappendiculata
 Distromium
 Distylis
 Diteilis
 Dithyrostegia
 Ditiola
 Ditoca
 Ditomostrophe
@@ -4221,14 +4311,15 @@
 Dolicholus
 Dolichos
 Dolichoscelis
 Dolichousnea
 Dombeya
 Domingoella
 Dominia
+Donacopsis
 Donatia
 Donella
 Donia
 Donkia
 Donkinia
 Doodia
 Dopatrium
@@ -4244,28 +4335,30 @@
 Doryopteris
 Doryphora
 Dothichloe
 Dothidasteroma
 Dothidasteromella
 Dothidea
 Dothidella
+Dothiora
 Dothiorella
 Dotyophycus
 Douglassia
 Dovyalis
 Doxantha
 Doxodasya
 Draba
 Drabastrum
 Dracaena
 Dracaenopsis
 Dracocephalum
 Dracontium
 Dracophyllum
 Drakaea
+Drakea
 Drakodenia
 Drakonorchis
 Draparnaldia
 Draparnaldiopsis
 Draparnandia
 Draparnaudia
 Drapetes
@@ -4360,14 +4453,15 @@
 Echinocactus
 Echinocarpus
 Echinocaulon
 Echinochaete
 Echinochloa
 Echinocolea
 Echinocroton
+Echinodiopsis
 Echinodium
 Echinodorus
 Echinolejeunea
 Echinophycus
 Echinoplaca
 Echinopogon
 Echinops
@@ -4400,34 +4494,35 @@
 Ehrartha
 Ehrartia
 Ehretia
 Ehrharta
 Eichhornia
 Eichlerago
 Eichleriella
+Eidernor
 Eidothea
 Eilemanthus
 Eilifdahlia
 Einadia
 Elachanthera
 Elachanthus
 Elachista
-Elachistea
 Elachocroton
 Elacholoma
 Elachopappus
 Elachopeltis
 Elachothamnos
 Elachothamnus
 Eladia
 Elaeagnus
 Elaeocarpus
 Elaeocharis
 Elaeodendron
 Elakatothrix
+Elaphanthera
 Elaphoblossum
 Elaphoglossum
 Elaphomyces
 Elasmomyces
 Elatine
 Elatostema
 Elatostemma
@@ -4517,14 +4612,15 @@
 Endoderma
 Endogenia
 Endogone
 Endohyalina
 Endomyces
 Endomycopsis
 Endophragmia
+Endophragmiella
 Endophyllum
 Endophyton
 Endoptychum
 Endoraecium
 Endosiphonia
 Endosira
 Endospermum
@@ -4549,15 +4645,17 @@
 Enteridium
 Enterodictyon
 Enterographa
 Enterolobium
 Enteromorpha
 Enteropogon
 Entocladia
+Entocybe
 Entodon
+Entodontopsis
 Entolasia
 Entoloma
 Entomoneis
 Entomophaga
 Entomophthora
 Entonaema
 Entopeltis
@@ -4604,15 +4702,14 @@
 Epidendroides
 Epidendrum
 Epidermophyton
 Epigloea
 Epiglossum
 Epilithon
 Epilobium
-Epimenia
 Epimeredi
 Epimeridi
 Epineuron
 Epipactis
 Epipellis
 Epiphanes
 Epiphloea
@@ -4633,14 +4730,15 @@
 Epitriche
 Epulo
 Epymenia
 Equisetum
 Eragrostiella
 Eragrostis
 Eranthemum
+Eraphthora
 Erechthites
 Erechtites
 Eremaea
 Eremaeopsis
 Eremastrella
 Eremocarpus
 Eremochloa
@@ -4678,14 +4776,15 @@
 Eriochilus
 Eriochiton
 Eriochlamys
 Eriochloa
 Eriochosma
 Eriocladium
 Eriocladus
+Eriocortex
 Erioderma
 Eriodon
 Erioglossum
 Erionema
 Eriopus
 Eriosciadium
 Eriosema
@@ -4717,14 +4816,15 @@
 Erysiphe
 Erythraea
 Erythranthe
 Erythranthera
 Erythricium
 Erythrina
 Erythrobarbula
+Erythrobasidium
 Erythrocarpus
 Erythrocladia
 Erythroclonium
 Erythrocolon
 Erythrodecton
 Erythromyces
 Erythronaema
@@ -4761,18 +4861,20 @@
 Ethuliopsis
 Etlingera
 Ettlia
 Euandra
 Euantennaria
 Euastrum
 Eubanksia
+Eucalyptoporia
 Eucalyptus
 Eucampia
 Eucamptodon
 Eucarya
+Eucasphaeria
 Eucheuma
 Euchilodes
 Euchilopsis
 Euchilos
 Euchilus
 Euchiton
 Euchlaena
@@ -4783,15 +4885,14 @@
 Euclidium
 Eucnemis
 Eucocconeis
 Eucosia
 Eucriphia
 Eucryphia
 Euctenodus
-Euctinodus
 Eucyperus
 Eudasycladus
 Eudesme
 Eudesmia
 Eudicranum
 Eudimeriolum
 Eudodia
@@ -4856,14 +4957,15 @@
 Eutacta
 Eutassa
 Eutaxia
 Euterpe
 Euthale
 Euthales
 Euthora
+Eutiarosporella
 Eutorulopsis
 Eutreptia
 Eutypa
 Eutypella
 Euxolus
 Euzoniella
 Evandra
@@ -4915,14 +5017,15 @@
 Fagara
 Fagaster
 Fagopyrum
 Fagraea
 Fagus
 Fairmaniella
 Falcataria
+Falcocladium
 Falkenbergia
 Falklandiella
 Fallacia
 Fallaciella
 Fallopia
 Faradaya
 Farnesia
@@ -4974,26 +5077,28 @@
 Filsoniana
 Fimbraria
 Fimbriaria
 Fimbristylis
 Fimetariella
 Finlaysonia
 Fioria
+Fiorinimazzantia
 Firmiana
 Fischera
 Fischerella
 Fissidens
 Fissistigma
 Fissurina
 Fistulina
 Fistulinella
 Fitchia
 Fitzalania
 Fitzgeraldia
 Fitzroya
+Fitzroyomyces
 Fitzwillia
 Flabellonema
 Flabellophora
 Flabellospora
 Flacourtia
 Flagellaria
 Flagelloscypha
@@ -5078,14 +5183,15 @@
 Fugomyces
 Fugosia
 Fuirena
 Fulgensia
 Fuligo
 Fulvifomes
 Fulvisporium
+Fumagopsis
 Fumagospora
 Fumaria
 Funalia
 Funaria
 Funckia
 Fungus
 Funicularius
@@ -5142,21 +5248,23 @@
 Galiella
 Galinsoga
 Galium
 Gallacea
 Gallaicolichen
 Gallionella
 Galphimia
+Gamarada
 Gambierdiscus
 Gamelythrum
 Gammamyces
 Gamochaeta
 Gamolepis
 Gamospora
 Gamozygis
+Gamsiella
 Gangliophora
 Ganitrus
 Ganoderma
 Ganonema
 Ganophyllum
 Garcinia
 Garckea
@@ -5178,32 +5286,35 @@
 Gastroglottis
 Gastrolobium
 Gastropila
 Gastrosuillus
 Gastrotylopilus
 Gattya
 Gaudinia
+Gaudium
 Gaultheria
 Gaultiera
 Gaura
 Gautieria
 Gaya
 Gayella
 Gayliella
 Gayralia
 Gazania
 Geastrum
 Geejayessia
+Geheebia
 Geijera
 Geissois
 Geissorhiza
 Geitlerinema
 Geitonoplesium
 Gela
 Gelasinospora
+Gelatoporia
 Geleznowia
 Gelibia
 Gelidiella
 Gelidiopsis
 Gelidium
 Gelinaria
 Gelineostroma
@@ -5222,14 +5333,15 @@
 Genea
 Genethyllis
 Genetyllis
 Genicularia
 Geniculosporium
 Geniostoma
 Genista
+Genolevuria
 Genoplesium
 Genorisis
 Genosiris
 Gentiana
 Gentianella
 Genus
 Genus (Aq247974)
@@ -5258,14 +5370,15 @@
 Geraniospermum
 Geranium
 Gerbera
 Germainia
 Germanea
 Germania
 Gerronema
+Gertrudiella
 Gessnerium
 Geum
 Geunsia
 Gevuina
 Gibasis
 Gibbera
 Gibberella
@@ -5292,14 +5405,15 @@
 Gingidia
 Gingidium
 Ginnania
 Gintarasia
 Giraudia
 Gironniera
 Githago
+Gjaerumia
 Glabraria
 Gladiolus
 Glandothamnus
 Glandularia
 Glaphyria
 Glaphyriopsis
 Glaphyrymenia
@@ -5315,25 +5429,29 @@
 Glenodiniopsis
 Glenodinium
 Glenospora
 Glensine
 Glinus
 Glioannellodochium
 Glioblastocladium
+Gliocephalotrichum
+Gliocladiopsis
 Gliocladium
 Gliomastix
 Gliophorus
 Gliricidia
 Glischrocaryon
 Globaria
 Globba
+Globisporangium
 Globomyces
 Globosphaeria
 Glochidion
 Gloeoactinium
+Gloeocalyx
 Gloeocapsa
 Gloeocapsopsis
 Gloeochaete
 Gloeococcus
 Gloeocystidiellum
 Gloeocystidium
 Gloeocystis
@@ -5349,19 +5467,19 @@
 Gloeothece
 Gloeotila
 Gloeotinia
 Gloeotrichia
 Gloiocladia
 Gloioderma
 Gloiohymenia
-Gloiophlaea
 Gloiophloea
 Gloiophyllis
 Gloiosaccion
 Gloiotrichus
+Gloioxanthomyces
 Glomerella
 Glomosporium
 Glomus
 Gloniella
 Gloniopsis
 Glonium
 Gloriosa
@@ -5370,14 +5488,15 @@
 Glossocardia
 Glossocarya
 Glossodia
 Glossogyne
 Glossophora
 Glossostigma
 Glotzia
+Glutinoglossum
 Glyaspermum
 Glyceria
 Glycine
 Glycocystis
 Glycorchis
 Glycosmis
 Glycyrrhiza
@@ -5427,14 +5546,15 @@
 Gomphotis
 Gomphraena
 Gomphrena
 Gomphus
 Gonapodya
 Gonatocarpus
 Gonatogenia
+Gonatophragmium
 Gonatopus
 Gonatozygon
 Gondwania
 Gongolaria
 Gongroceras
 Gongronella
 Gongronema
@@ -5532,14 +5652,15 @@
 Grona
 Gronophyllum
 Groutiella
 Grumilea
 Grumilia
 Grunowiella
 Grymania
+Grypothrix
 Guadelupa
 Guapeba
 Guatteria
 Guazuma
 Guembelia
 Guepinia
 Guepiniopsis
@@ -5647,15 +5768,17 @@
 Gyroporus
 Gyrosigma
 Gyrostemon
 Gyrostephium
 Gyrostomum
 Gyrothrix
 Gyrothyra
+Gyroweisia
 Habenaria
+Habenorkis
 Habranthus
 Habrophyllum
 Habrostictis
 Habrothamnus
 Hackelia
 Hackelochloa
 Haddowia
@@ -5720,20 +5843,22 @@
 Halteromyces
 Halurus
 Halydictyon
 Halymenia
 Halyseris
 Halysium
 Hamelia
+Hamigera
 Hampeella
 Hamulia
 Hancea
 Handkea
 Handroanthus
 Hanguana
+Hannaella
 Hannafordia
 Hanowia
 Hanseniaspora
 Hansenula
 Hansfordia
 Hansfordiella
 Hanslia
@@ -5747,19 +5872,21 @@
 Haplodasya
 Haplogloia
 Haplohymenium
 Haplomitrium
 Haplopappus
 Haploporus
 Haplopteris
+Haplostellis
 Haplostichanthus
 Haplostigma
 Haplostylis
 Haplotaenium
 Haplotaxis
+Hapsidospora
 Haptotrichion
 Haraldia
 Haraldiophyllum
 Hardenbergia
 Harknessia
 Harmogia
 Harmsiodoxa
@@ -5788,14 +5915,15 @@
 Hebe
 Hebejeebie
 Hebeloma
 Hebenstretia
 Hecatandra
 Hecatonema
 Hedaroma
+Hedenaesia
 Hedera
 Hederoma
 Hedraeanthera
 Hedraianthera
 Hedrianthera
 Hedwigia
 Hedwigidium
@@ -5851,15 +5979,14 @@
 Helminthocarpon
 Helminthocladia
 Helminthora
 Helminthosporium
 Helminthostachys
 Helminthotheca
 Helmintia
-Helmsia
 Helophyllum
 Helophytum
 Helopus
 Helosciadium
 Helospora
 Helothrix
 Helotiella
@@ -5879,14 +6006,15 @@
 Hemicarpha
 Hemicarpus
 Hemichroa
 Hemiclidia
 Hemicorynespora
 Hemicyatheon
 Hemicyclia
+Hemidesmas
 Hemidinium
 Hemidiscus
 Hemigenia
 Hemigrapha
 Hemigraphis
 Hemigymnia
 Hemileia
@@ -5930,14 +6058,15 @@
 Herdmania
 Hericium
 Heringia
 Herissantia
 Heritiera
 Hermanella
 Hermannia
+Hermatomyces
 Hermesia
 Herminium
 Hernandia
 Herniaria
 Herpestis
 Herpetineuron
 Herpetium
@@ -6005,16 +6134,18 @@
 Heterotextus
 Heterothamnion
 Heterotheca
 Heterothecium
 Heterothrichopsis
 Heterothrix
 Heterotolyposporium
+Heterotruncatella
 Heterozostera
 Heuzenroedera
+Hevansia
 Hevea
 Hewardia
 Hexaglottis
 Hexagonia
 Hexalepis
 Hexamita
 Hexasepalum
@@ -6103,14 +6234,15 @@
 Homeria
 Homoeocladia
 Homoeostrichus
 Homoeothrix
 Homoglossum
 Homogyne
 Homopholis
+Homophron
 Homoplitis
 Homoranthus
 Hookerella
 Hookeria
 Hookeriopsis
 Hookerochloa
 Hopkinsia
@@ -6163,19 +6295,21 @@
 Humaria
 Humata
 Humea
 Humicola
 Humidicutis
 Humulus
 Huneckia
+Huntiella
 Huperzia
 Husemannia
 Husseia
 Husseya
 Husseyella
+Husseyia
 Hutchinsia
 Huttia
 Huttoniella
 Huttum
 Huxleya
 Hyacinthoides
 Hyacinthus
@@ -6190,14 +6324,15 @@
 Hyalopus
 Hyaloscypha
 Hyalosira
 Hyalosperma
 Hyalospermum
 Hyalosynedra
 Hyalotheca
+Hyalozasmidium
 Hybanthera
 Hybanthus
 Hydatella
 Hydnangium
 Hydnellum
 Hydnobolites
 Hydnocarpus
@@ -6219,14 +6354,15 @@
 Hydrocleis
 Hydrocleys
 Hydrococcus
 Hydrocoleum
 Hydrocotyle
 Hydrodictyon
 Hydroglossum
+Hydrogonium
 Hydrolapatha
 Hydrolea
 Hydrolithon
 Hydronectria
 Hydropeltis
 Hydropisphaera
 Hydropuntia
@@ -6262,32 +6398,35 @@
 Hymenobolina
 Hymenobolus
 Hymenocallis
 Hymenocapsa
 Hymenochaeta
 Hymenochaete
 Hymenochaetella
+Hymenochaetopsis
 Hymenochilus
 Hymenocladia
 Hymenocladiopsis
 Hymenodon
 Hymenodontopsis
 Hymenogaster
 Hymenolepis
 Hymenolobus
+Hymenoloma
 Hymenopellis
 Hymenophyllum
 Hymenophyton
 Hymenoscypha
 Hymenoscyphus
 Hymenosporum
 Hymenostilbe
 Hymenostomum
 Hymenostylium
 Hymenotheca
+Hymenotorrendiella
 Hymenula
 Hyocomium
 Hyogeton
 Hyophila
 Hyoscyamus
 Hyoseris
 Hypaelyptum
@@ -6327,14 +6466,15 @@
 Hypochnus
 Hypochoeris
 Hypochoerus
 Hypocopra
 Hypocrea
 Hypocrella
 Hypocreopsis
+Hypodematium
 Hypodermella
 Hypoestes
 Hypoglossum
 Hypogymnia
 Hypolaena
 Hypolepis
 Hypolytrum
@@ -6349,43 +6489,47 @@
 Hypotrachyna
 Hypoxis
 Hypoxylon
 Hypsela
 Hypserpa
 Hypsizygus
 Hypsophila
+Hypsotheca
 Hyptiandra
 Hyptis
 Hyrtanandra
 Hysterangium
 Hysteria
 Hysterium
 Hysterobaeakea
 Hysterobaeckea
 Hysterogaster
 Hysterographium
 Hysteropezizella
 Hystrichosphaera
 Hystrix
+Hyweljonesia
 Ianthe
 Ibatiria
 Iberis
 Ibicella
 Ichnanthus
 Ichnocarpus
 Ichnostemma
 Ichthyocercus
 Ichthyodontum
 Ichthyostomum
 Icica
 Icmadophila
 Icmane
+Iconella
 Idiocercus
 Idiospermum
 Idriella
+Idriellomyces
 Ilea
 Ileodictyon
 Ileostylus
 Ilex
 Illecebrum
 Illigera
 Illipe
@@ -6401,53 +6545,57 @@
 Imperatia
 Imshaugia
 Incrustoporia
 Indagator
 Indigastrum
 Indigo
 Indigofera
+Induratia
 Ineffigiata
 Inesiosporium
 Inga
 Ingoldiomyces
 Ingvariella
 Inkyuleea
 Inocarpus
 Inocephalus
 Inocutis
 Inocybe
 Inocyclus
 Inoderma
 Inonotus
+Inosperma
 Insiticia
 Insolibasidium
 Interthamnion
 Intsia
 Inula
 Involucrana
 Involucraria
 Iodophanus
 Iodosphaeria
 Ionaspis
 Ionia
 Ionidium
 Ionomidotis
+Ionosporus
 Ionoxalis
 Iotasperma
 Ipheion
 Iphigenia
 Ipomaea
 Ipomoea
 Irene
 Irenepharsus
 Irenopsis
 Iresine
 Iria
 Iridaea
 Iridophycus
+Iridorchis
 Iridorkis
 Iriha
 Iris
 Irpex
 Irtugovia
 Irvingbaileya
 Irvingia
@@ -6474,14 +6622,16 @@
 Isolobus
 Isoloma
 Isomerium
 Isopaches
 Isophyllaria
 Isophysis
 Isopogon
+Isopterygiella
+Isopterygiopsis
 Isopterygium
 Isoschoenus
 Isostylis
 Isotachis
 Isothea
 Isothecium
 Isotoma
@@ -6536,30 +6686,34 @@
 Jasminanthes
 Jasminonerium
 Jasminum
 Jatropha
 Jeannerettia
 Jedda
 Jensenia
+Jensoa
 Jessenia
+Jimgerdemannia
 Johannesbaptistia
+Johnalcornia
 Johnsonia
 Jonesiopchis
 Jonesiopsis
 Jonesyella
 Jonidium
 Jonorchis
 Josephia
 Josephinia
 Jossinia
 Joycea
 Jubaea
 Jubula
 Juglans
 Julella
+Juncaceicola
 Juncella
 Juncellus
 Juncodes
 Juncoides
 Juncus
 Jungermannia
 Junghuhnia
@@ -6617,22 +6771,24 @@
 Kennedynella
 Kennyeda
 Kentia
 Kentranthus
 Kentrophora
 Kentrophyllum
 Kentropsis
+Keraliethelia
 Kerandrenia
 Keratinophyton
 Keratosphaera
 Keraudrenia
 Kerigomnia
 Kermadecia
 Kernera
 Kernkampella
+Kgaria
 Khaya
 Khuskia
 Kiaeria
 Kibara
 Kickxia
 Kikuyuochloa
 Kindbergia
@@ -6674,14 +6830,15 @@
 Komvophoron
 Koniga
 Kopsia
 Koralionastes
 Kordyana
 Korshikoviella
 Korthalsella
+Kraenzlinorchis
 Kraftia
 Kramasamuha
 Kraunhia
 Kreisigia
 Kretzschmaria
 Kreysigia
 Kreyssigia
@@ -6784,42 +6941,44 @@
 Lamprolobium
 Lamprospora
 Lamprothamnium
 Lamprothamnus
 Lancisia
 Landerolaria
 Landoltia
+Langdonia
 Langermannia
 Langloisula
 Lantana
 Lanzia
 Lapathum
 Lapeirousia
 Laphangium
 Laportea
 Lappa
 Lappago
 Lappagopsis
 Lappula
 Lapsana
 Lapula
+Lareunionomyces
 Laricifomes
 Larsenaikia
 Laschia
 Lasia
 Lasiandra
 Lasianthus
 Lasiobelonium
-Lasiobolidium
 Lasiobolus
 Lasiochloa
 Lasiodiplodia
 Lasioloma
 Lasiolytrum
 Lasionectria
+Lasionectriopsis
 Lasiopetalum
 Lasiosiphon
 Lasiospermum
 Lasiosphaeria
 Lasiosphaeris
 Lasiothalia
 Lasjia
@@ -6877,14 +7036,15 @@
 Lecanosticta
 Leccinum
 Lechenaultia
 Lechenautia
 Lecidea
 Lecidella
 Lecithites
+Lectera
 Lecythophora
 Ledebouria
 Ledelia
 Ledgeria
 Leea
 Leersia
 Leeuvenhookia
@@ -6895,36 +7055,39 @@
 Legeriomyces
 Legnephora
 Leguminosae (=RFK/2760)
 Leibleinia
 Leichardtia
 Leichhardtia
 Leifidium
+Leifiporia
 Leightoniella
 Leimonis
 Leioanthum
 Leiocarpa
 Leiocarya
 Leiocolea
 Leioderma
 Leiomitra
 Leionema
 Leiorreuma
 Leioscyphus
 Leiosporoceros
 Leiostoma
 Leiotheca
+Leiotrametes
 Lejeunea
 Lejeunia
 Lejolisia
 Lemanea
 Lembidium
 Lembophyllum
 Lembosia
 Lembosina
+Lembosiniella
 Lemmaphyllum
 Lemmermannia
 Lemmermanniella
 Lemna
 Lemnicola
 Lemnopsis
 Lemonniera
@@ -6953,27 +7116,27 @@
 Leopoldia
 Leotia
 Lepeostegeres
 Lepia
 Lepiactis
 Lepicolea
 Lepidagathis
+Lepidella
 Lepiderema
 Lepidium
 Lepidobolus
 Lepidocarpa
 Lepidocaulon
 Lepidocollema
 Lepidocoma
 Lepidoderma
 Lepidodinium
 Lepidogyna
 Lepidolaena
 Lepidolejeunea
-Lepidoleptogium
 Lepidoneuron
 Lepidopetalum
 Lepidopilum
 Lepidorhachis
 Lepidorrhachis
 Lepidosperma
 Lepidospora
@@ -7081,14 +7244,15 @@
 Leptotrichella
 Leptotrichum
 Leptoxyphium
 Lepturopetium
 Lepturus
 Lepyrodia
 Lepyrodon
+Leratia
 Leratiomyces
 Lerchia
 Leschenaultia
 Leskea
 Lesleigha
 Lespedeza
 Lespedezia
@@ -7134,23 +7298,25 @@
 Leucopogon
 Leucoporus
 Leucorchis
 Leucoscypha
 Leucosmia
 Leucospermum
 Leucothamnus
+Leucozoma
 Leuliisinea
 Leuwenhoekia
 Leuzea
 Levanderina
 Leveillea
 Levenhoekia
 Levenhookia
 Levieria
 Lewia
+Lewinskya
 Leycesteria
 Leymus
 Lhotskya
 Lhotzkya
 Lhotzseya
 Liagora
 Libartania
@@ -7214,24 +7380,26 @@
 Linealia
 Lineolata
 Linguella
 Lingulodinium
 Linkia
 Linkosia
 Linnaea
+Linnemannia
 Linocarpon
 Linochora
 Linociera
 Linociria
 Linospadix
 Linospora
 Linostoma
 Linosyris
 Linsaea
 Linschotenia
+Linteromyces
 Linum
 Liochlaena
 Lioloma
 Liparis
 Liparophyllum
 Lipoblepharis
 Lipocarpha
@@ -7255,14 +7423,15 @@
 Lithomyrtus
 Lithophyllum
 Lithoporella
 Lithospermum
 Lithothamnion
 Lithothamnium
 Lithothelium
+Lithotoma
 Lithoxylon
 Litobrochia
 Litocarpus
 Litsaea
 Litsea
 Livistona
 Livistonia
@@ -7333,14 +7502,15 @@
 Lophopyrum
 Lophosiphonia
 Lophospermum
 Lophostemon
 Lophothalia
 Lophothamnion
 Lophotocarpus
+Lophotrichus
 Lophozia
 Lophozonia
 Lophura
 Lophurella
 Lopidium
 Loranthus
 Lordhowea
@@ -7371,14 +7541,15 @@
 Lundquistia
 Lunularia
 Lunulina
 Lunulospora
 Luorea
 Lupinus
 Lupulus
+Luteocirrhus
 Luteolejeunea
 Luticola
 Luttrellia
 Luvunga
 Luzula
 Luzuriaga
 Luzuriago
@@ -7458,14 +7629,15 @@
 Macroglossum
 Macrohilum
 Macrohymenium
 Macrohyporia
 Macrolepiota
 Macromitrium
 Macrophoma
+Macrophomina
 Macropidia
 Macropiper
 Macroplethus
 Macropodia
 Macropogon
 Macropsychanthus
 Macropteranthes
@@ -7487,14 +7659,15 @@
 Macuna
 Macvicaria
 Madia
 Madrepora
 Madurella
 Maekawaea
 Maesa
+Magnaporthe
 Magnaporthiopsis
 Magnusiomyces
 Magoderna
 Mahernia
 Mahonia
 Maidenia
 Maireana
@@ -7518,14 +7691,15 @@
 Malaxis
 Malbranchea
 Malcolmia
 Malcolmiella
 Malcomia
 Malephora
 Malleostemon
+Mallocybe
 Mallomonas
 Mallomonopsis
 Mallophora
 Mallotus
 Malmidea
 Malocchia
 Malus
@@ -7580,14 +7754,15 @@
 Markhamia
 Marlea
 Maronea
 Maronina
 Marquartia
 Marquisia
 Marrattia
+Marrilea
 Marrubium
 Marsdenia
 Marsilea
 Marsilia
 Marssonia
 Marssonina
 Marsupella
@@ -7618,14 +7793,15 @@
 Mastodia
 Mastogloia
 Mastoneis
 Mastophora
 Mastophoropsis
 Mastosuke
 Mathiola
+Matourea
 Matricaria
 Matsushimiella
 Matthiola
 Mattirolomyces
 Mauchartia
 Maughania
 Maundia
@@ -7682,14 +7858,15 @@
 Meladenia
 Melalenca
 Melaleuca
 Melampilidium
 Melampodium
 Melampsora
 Melanamansia
+Melanascoma
 Melanconium
 Melancranis
 Melandrium
 Melandrum
 Melandryum
 Melanelia
 Melanelixia
@@ -7706,15 +7883,14 @@
 Melanophloea
 Melanophyllum
 Melanops
 Melanopsamma
 Melanopsichium
 Melanopus
 Melanoseris
-Melanospora
 Melanostachya
 Melanotaenium
 Melanotheca
 Melanotopelia
 Melanotrema
 Melanotus
 Melanthalia
@@ -7798,14 +7974,15 @@
 Meruliopsis
 Meruliporia
 Merulius
 Meryta
 Mesembrianthemum
 Mesembryanthemum
 Mesibovia
+Mesicera
 Mesocarpus
 Mesoceros
 Mesochaete
 Mesochlaena
 Mesodactylis
 Mesogloia
 Mesogloiopsis
@@ -7890,14 +8067,15 @@
 Microcybe
 Microcystis
 Microderis
 Microdictyon
 Microdiplodia
 Microdochium
 Microdus
+Microeurhynchium
 Microglaena
 Microglossum
 Microgongrus
 Microgonium
 Microgyne
 Microhilum
 Microlaena
@@ -7936,14 +8114,15 @@
 Microsporum
 Microstachys
 Microstegia
 Microstegium
 Microstemma
 Microstephium
 Microstrobos
+Microstroma
 Microstylis
 Microstylus
 Microtabella
 Microtatorchis
 Microthamnion
 Microthamnium
 Microthecium
@@ -7975,14 +8154,15 @@
 Miltidea
 Mimetes
 Mimosa
 Mimulus
 Mimusops
 Minidiscus
 Minimelanolocus
+Minivolcanus
 Minuartia
 Minuranthus
 Minuria
 Minuriella
 Minutocellus
 Minutoexcipula
 Mirabilis
@@ -8175,16 +8355,18 @@
 Munkiodothis
 Muntingia
 Muraltia
 Murchisonia
 Murdannia
 Muricia
 Muriella
+Murinectria
 Murracystis
 Murraea
+Murramarangomyces
 Murraya
 Murrayella
 Murtughas
 Murucuia
 Murucuja
 Musa
 Musaespora
@@ -8196,41 +8378,45 @@
 Mustelia
 Mutinus
 Myagrum
 Myceliophthora
 Mycena
 Mycenastrum
 Mycenella
+Mycetinis
 Mychodea
 Mychodeophyllum
 Mycoacia
 Mycoamaranthus
 Mycoarctium
 Mycobilimbia
 Mycoblastus
 Mycobonia
 Mycocalia
 Mycocalicium
 Mycocentrospora
 Mycoclelandia
 Mycoderma
+Mycodiella
 Mycoidea
 Mycoleptodiscus
 Mycoleptodon
 Mycomicrothelia
 Mycophycophila
 Mycoporellum
 Mycoporopsis
 Mycoporum
+Mycosarcoma
 Mycosphaerella
 Mycotorula
 Mycovellosiella
 Myelochroa
 Myeloconis
 Myelorrhiza
+Myiriogyne
 Mylitta
 Myoporum
 Myosotis
 Myosurus
 Myrcia
 Myriactis
 Myriactula
@@ -8256,20 +8442,23 @@
 Myrmecia
 Myrmecodia
 Myrmecophila
 Myrmecopteris
 Myrmecostylum
 Myrmecridium
 Myrobalanus
+Myrotheciomyces
 Myrothecium
 Myroxylon
 Myrsidrum
 Myrsine
 Myrsiphyllum
 Myrstiphyllum
+Myrtacremonium
+Myrtapenidiella
 Myrtella
 Myrtoleucodendron
 Myrtus
 Mystrosporium
 Mytilopsis
 Myurium
 Myxacium
@@ -8288,19 +8477,21 @@
 Naccaria
 Nadvornikia
 Naegeliella
 Naemacyclus
 Naemaspora
 Naematelia
 Naematoloma
+Naganishia
 Nageia
 Naias
 Nais
 Najas
 Nalagu
+Nalanthamala
 Nandina
 Nani
 Nania
 Nannizzia
 Nannizziopsis
 Nannochloris
 Nanobryum
@@ -8339,15 +8530,14 @@
 Negria
 Neidium
 Neiosperma
 Neisosperma
 Nelipus
 Nelitris
 Nellica
-Nelobesia
 Nelsonia
 Neltuma
 Nelumbium
 Nelumbo
 Nemacianthus
 Nemacystus
 Nemalion
@@ -8364,65 +8554,87 @@
 Nematopus
 Nematospora
 Nematostigma
 Nemcia
 Nemedra
 Nemesia
 Nemopogon
+Nemuranthes
 Nengella
 Neoachmandra
 Neoalsomitra
+Neoantrodia
+Neoanungitea
 Neoardissonea
 Neoareschougia
 Neoastelia
 Neobarya
 Neobassia
+Neoboletus
 Neobrownliella
 Neobulgaria
 Neobyrnesia
 Neocallimastix
 Neocallitropsis
+Neocalonectria
 Neocalyptrella
 Neoceis
+Neocelosporium
 Neoceratium
+Neoceratosperma
 Neochloris
 Neocolmeiroa
+Neoconiothyrium
 Neocosmospora
+Neocrinula
+Neocucurbitaria
 Neocupressus
 Neodasyscypha
 Neodetonia
+Neodevriesia
+Neodidymelliopsis
 Neodiplodina
+Neoerysiphe
+Neoeucasphaeria
 Neofabraea
 Neofabricia
+Neofavolus
+Neofomitella
 Neofranciella
 Neofuscelia
 Neofusicoccum
 Neogoniolithon
 Neogoodenia
 Neogrollea
 Neoguillauminia
 Neogunnia
 Neohodgsonia
 Neohuttonia
+Neohygrocybe
+Neokirramyces
 Neolamarckia
 Neolaria
+Neolauriomyces
 Neolentinus
 Neolentiporus
+Neolepidozia
 Neolindbergia
 Neolinocarpon
 Neolitsea
 Neololeba
 Neomarica
 Neomartensia
 Neomeris
 Neomonospora
 Neonauclea
 Neonectria
 Neonotonia
 Neopaxia
+Neopestalotiopsis
+Neophaeomoniella
 Neophoma
 Neophyllis
 Neophylum
 Neoplatylobium
 Neopreissia
 Neoprotoparmelia
 Neoralfsia
@@ -8431,43 +8643,51 @@
 Neoroepera
 Neosartorya
 Neosciadium
 Neoscytalidium
 Neosepicaea
 Neoseptorioides
 Neosiphonia
+Neosonderhenia
+Neospadicoides
+Neospermospora
 Neospongiococcum
+Neostemphylium
 Neostrearia
 Neostreptotheca
 Neotestudina
+Neothyriopsis
 Neotonia
 Neotrichocolea
+Neotrichosphaeria
 Neotrimmatostroma
 Neottia
 Neottiella
 Neottiospora
 Neottiosporina
 Neottopteris
 Neotyphodium
 Neotysonia
 Neovossia
 Neowollastonia
+Neoxylaria
 Neozygites
 Nepenthes
 Nepeta
 Nephelium
 Nephelolejeunea
 Nephrandra
 Nephrocytium
 Nephrodium
 Nephrolepis
 Nephroma
 Nephromium
 Neptunella
 Neptunia
+Neptunomyces
 Nereia
 Nereidea
 Nerine
 Nerium
 Nertera
 Nervilia
 Nesaea
@@ -8517,14 +8737,15 @@
 Nierembergia
 Niesslia
 Nigella
 Nigredo
 Nigrofomes
 Nigromnia
 Nigroporus
+Nigrosabulum
 Nigrospora
 Nigrovothelium
 Ninanga
 Nipa
 Niphobolus
 Nipholobus
 Nipicola
@@ -8533,14 +8754,15 @@
 Nitellopsis
 Nitidochapsa
 Nitophyllum
 Nitospinosa
 Nitraria
 Nitschkia
 Nitzschia
+Niveoporofomes
 Nizymenia
 Nizzophlaea
 Noahdendron
 Noctiluca
 Nodularia
 Nodulisporium
 Nolanea
@@ -8563,46 +8785,53 @@
 Nothoceros
 Nothochlaena
 Nothocissus
 Nothocladus
 Nothoclaena
 Nothocnide
 Nothodanthonnia
+Nothofagiporus
 Nothofagus
 Nothogenia
 Nothogymnomitrion
 Nothojafnea
 Notholaena
 Notholepiota
 Nothopanax
 Nothopanus
+Nothophoma
 Nothorites
 Nothoscordum
+Nothotrimmatostroma
 Notihydnum
 Notisia
 Notobasis
 Notochlaena
 Notochloe
 Notocladonia
 Notodanthonia
 Notogrammitis
+Notohypnum
 Notolecidea
 Notoleptopus
 Notoligotrichum
 Notonerium
 Notonia
 Notoparmelia
 Notoscyphus
 Notosolenus
+Notothamia
 Notothixos
 Notothlaspi
 Notothylas
 Notoxylinon
 Nowakowskiella
+Nowamyces
 Nowellia
+Nullicamyces
 Nummularia
 Nupela
 Nusuttodinium
 Nuttallanthus
 Nuytsia
 Nyctalis
 Nyctanthes
@@ -8618,14 +8847,15 @@
 Nyssanthes
 Nyssopsora
 Obba
 Obeliospora
 Oberonia
 Obione
 Oblea
+Oblongocollomyces
 Oceana
 Oceaniopteris
 Oceanitis
 Ocellularia
 Ochiobryum
 Ochlochaete
 Ochmapexus
@@ -8644,14 +8874,16 @@
 Octavianina
 Octoblepharum
 Octoclinis
 Octoclinus
 Octodiceras
 Octojuga
 Octospora
+Octosporella
+Oculimacula
 Ocymum
 Ocyricera
 Odixia
 Odontella
 Odontia
 Odontidium
 Odontolejeunea
@@ -8682,14 +8914,15 @@
 Oliganthemum
 Oligarrhena
 Oligocarpus
 Oligochaetochilus
 Oligoporus
 Oligostroma
 Oligotrichum
+Olivea
 Oliveonia
 Olivia
 Oloptum
 Olpidiopsis
 Olpidium
 Omalanthus
 Omalotheca
@@ -8733,14 +8966,15 @@
 Oospora
 Opanea
 Opegrapha
 Opephora
 Opercularia
 Operculina
 Ophelia
+Ophidiomyces
 Ophidocladus
 Ophiobolus
 Ophioceras
 Ophiocordyceps
 Ophiocytium
 Ophioderma
 Ophiodothella
@@ -8762,14 +8996,15 @@
 Oplotheca
 Opocunonia
 Opuntia
 Orania
 Oraniopsis
 Orbea
 Orbilia
+Orbiocrella
 Orcadella
 Orceolina
 Orchiastrum
 Orchiodes
 Orchipeda
 Orchis
 Orcularia
@@ -8803,14 +9038,15 @@
 Orobanche
 Orophea
 Orphniospora
 Orpinomyces
 Orthocarpus
 Orthoceras
 Orthodontium
+Orthogonacladia
 Orthogramma
 Orthomnion
 Orthomniopsis
 Orthoneis
 Orthopogon
 Orthorrhynchium
 Orthoseira
@@ -8834,14 +9070,15 @@
 Oschatzia
 Oscillatoria
 Osmia
 Osmoporus
 Osmunda
 Osmundaria
 Osmundea
+Ossicaulis
 Ossiella
 Osteina
 Osteocarpum
 Osteocarpus
 Osteospermum
 Ostiophyllum
 Ostracoderma
@@ -8874,14 +9111,15 @@
 Owenia
 Oxalis
 Oxera
 Oxilobium
 Oxleya
 Oxyanthera
 Oxybasis
+Oxychaete
 Oxychloris
 Oxycladium
 Oxydectes
 Oxydothis
 Oxylobium
 Oxymitra
 Oxymyrrhine
@@ -8933,14 +9171,15 @@
 Paecilomyces
 Paederia
 Paederota
 Paenula
 Paesia
 Pagetia
 Pagiantha
+Pakau
 Palaeophalacroma
 Palafoxia
 Palala
 Palaquium
 Palgianthus
 Palhinhaea
 Paliphora
@@ -8979,85 +9218,99 @@
 Panel
 Panellus
 Panicularia
 Paniculum
 Panicum
 Pannaria
 Pannoparmelia
-Pannularia
 Panope
 Panoxis
 Pantlingia
 Panus
 Papaver
 Papenfussiella
 Paphia
+Papiliotrema
 Papillaria
 Papillidiopsis
 Papillilabium
 Papistylus
 Pappochroma
 Pappophorum
 Papularia
 Papulaspora
 Papulipetalum
 Paquerina
 Parablechnum
 Paracaleana
+Paracamarosporium
 Paraceterach
+Paracladophialophora
+Paraconiothyrium
 Paracorokia
 Paracromastigum
 Paractaenum
 Paracynoglossum
 Paradennstaedtia
 Paraderris
 Paradiachea
 Paradiacheopsis
+Parafabraea
 Paragonis
 Paragoodia
 Parahebe
 Parahistioneis
 Parakeelya
 Paralia
 Paralinospadix
 Parallela
+Paraloratospora
 Paralstonia
 Paramapania
 Paramignya
 Paramycetinis
+Paramycosphaerella
+Paramyrothecium
+Paranannizziopsis
 Paranectria
 Paraneurachne
 Paranomus
 Paranotis
 Parantennaria
 Parapachygone
 Paraparmelia
 Parapenidiella
 Parapericonia
 Paraphaeosphaeria
 Parapholis
 Paraphoma
+Paraphysalospora
 Paraphysomonas
 Parapolystichum
 Paraporpidia
 Paraprasophyllum
+Parapyrenochaeta
+Pararamichloridium
 Pararchidendron
 Pararistolochia
 Parasamanea
 Parasarcochilus
+Parasarocladium
 Paraschistochila
 Parascutellinia
 Paraserianthes
 Parasiphula
 Parasola
 Paraspora
+Parastagonospora
 Parastigmatellina
 Parasympodiella
 Parataeniella
 Paratephrosia
+Parateratosphaeria
 Parathelium
 Paratrophis
 Paratropia
 Parberya
 Parduyna
 Parelion
 Parenterolobium
@@ -9137,14 +9390,15 @@
 Pedinopera
 Pedinophyllopsis
 Pedinophyllum
 Pedleya
 Pedobesia
 Peekeliopanax
 Peganum
+Peglionia
 Peirardia
 Peireskia
 Pelagorhynchus
 Pelargonium
 Pelekium
 Pelidnia
 Pellaea
@@ -9177,14 +9431,15 @@
 Pentachondra
 Pentacraspedion
 Pentacraspedon
 Pentadactylon
 Pentadynamis
 Pentaglottis
 Pentagonaster
+Pentagrostis
 Pentalepis
 Pentameris
 Pentapanax
 Pentapeltis
 Pentapetes
 Pentapharsodinium
 Pentapogon
@@ -9249,14 +9504,15 @@
 Perrottetia
 Perrya
 Persea
 Persicaria
 Persoonia
 Persooniella
 Perssoniella
+Perthomyces
 Pertusaria
 Pervinca
 Pesotum
 Pestalotia
 Pestalotiopsis
 Pestalozzia
 Petalandra
@@ -9275,15 +9531,14 @@
 Petasitis
 Peterjamesia
 Petermannia
 Petersenia
 Petractis
 Petraeomyrtus
 Petraeovitex
-Petriella
 Petrocarya
 Petroderma
 Petrodictyon
 Petroglossum
 Petromyces
 Petroneis
 Petrophila
@@ -9353,21 +9608,24 @@
 Phaeopyxis
 Phaeoramularia
 Phaeosclera
 Phaeoseptoria
 Phaeosphaera
 Phaeosphaerella
 Phaeosphaeria
+Phaeosphaeriopsis
 Phaeospora
 Phaeostalagmus
 Phaeotellus
 Phaeothamnion
 Phaeothecoidea
+Phaeothyriolum
 Phaeotrametes
 Phaeotrema
+Phaeotremella
 Phaeotrichoconis
 Phaeoxyphiella
 Phaeus
 Phaffomyces
 Phaius
 Phajus
 Phakopsora
@@ -9377,14 +9635,15 @@
 Phalangium
 Phalansterium
 Phalaris
 Phaleria
 Phallus
 Phanera
 Phanerandra
+Phanerina
 Phanerochaete
 Phanerophlebia
 Pharbitis
 Pharcidia
 Pharmacosycea
 Pharnaceum
 Pharochilum
@@ -9410,14 +9669,15 @@
 Phialea
 Phialemonium
 Phialocephala
 Phialocybe
 Phialomyces
 Phialophora
 Phialophorophoma
+Phialoseptomonium
 Phialosimplex
 Philadelphia
 Philadelphus
 Philidiostigma
 Philippia
 Philippiella
 Phillipsia
@@ -9446,14 +9706,15 @@
 Phlebothamnion
 Phlegmacium
 Phlegmariurus
 Phlegmatospermum
 Phleogena
 Phleum
 Phloeocaulon
+Phloeomana
 Phloeospora
 Phloeosporella
 Phloepeccania
 Phlogicylindrium
 Phloiocaulon
 Phlyctaena
 Phlyctella
@@ -9580,37 +9841,40 @@
 Physosporella
 Physostegia
 Physotium
 Physurus
 Phytoconis
 Phytolacca
 Phytophthora
+Phytopythium
 Piarimula
 Piaropus
 Piccolia
 Picea
 Pichia
 Pichonia
+Picipes
 Picnomon
 Picridium
 Picris
 Picrophyta
 Pictolejeunea
 Pigea
 Piggotia
 Pihiella
 Pilacre
-Pilaiella
+Pilaira
 Pilayella
 Pilbara
 Pilea
 Pileanthus
 Pileolaria
 Pilidiella
 Pilidiostigma
+Pilidium
 Pilinia
 Pilinophytum
 Piliocalyx
 Piliostigma
 Pilitis
 Pillera
 Pilobolus
@@ -9629,30 +9893,31 @@
 Pilularia
 Pimelea
 Pimelia
 Pimelodendron
 Pimpinella
 Pinalia
 Pinnatella
+Pinnatidendron
 Pinnularia
 Pinnunavis
 Pinus
 Piper
 Piptandra
 Piptatherum
 Piptocalyx
 Piptocephalis
 Piptochaetium
 Piptoclainia
 Piptomeris
 Piptoporus
-Piptospatha
 Piptostemma
 Pipturus
 Pircunia
+Piriformospora
 Piromonas
 Pisolithus
 Pisonia
 Pistachia
 Pistacia
 Pistaciovitex
 Pistia
@@ -9666,15 +9931,14 @@
 Pithomyces
 Pithophora
 Pithyopsis
 Pithyrodia
 Pittonia
 Pittosporoides
 Pittosporum
-Pityophycos
 Pityophykos
 Pityrodia
 Pityrogramma
 Pityrosporum
 Placella
 Placidiopsis
 Placidium
@@ -9718,16 +9982,18 @@
 Planktolyngbya
 Planktoniella
 Planktosphaeria
 Planktothrix
 Planocarpa
 Planophila
 Planothidium
+Plantaginorchis
 Plantago
 Plasmodiophora
+Plasmopara
 Platanocarpum
 Platanthera
 Platanus
 Platessa
 Platoma
 Platonia
 Platostoma
@@ -9742,14 +10008,15 @@
 Platygyrium
 Platyhypnidium
 Platyhypnum
 Platylobium
 Platyloma
 Platymenia
 Platyptelea
+Platypus
 Platysace
 Platysiphonia
 Platysma
 Platystomum
 Platytaenia
 Platythalia
 Platythamnion
@@ -9783,18 +10050,20 @@
 Plenotrichella
 Pleodorina
 Pleogibberella
 Pleogyne
 Pleolpidium
 Pleomele
 Pleonosporium
+Pleopassalora
 Pleopeltis
 Pleosphaeria
 Pleospora
 Pleotrichiella
+Pleotrichocladium
 Plerandra
 Pleroma
 Plesiagopus
 Plesioneuron
 Pleurandra
 Pleurandropsis
 Pleurandros
@@ -9804,25 +10073,27 @@
 Pleurocapsa
 Pleurocarpaea
 Pleurocitrus
 Pleurocladopsis
 Pleurocladula
 Pleurococcus
 Pleurocybella
+Pleurodesmospora
 Pleurodiscus
 Pleuroflammula
 Pleurogramma
 Pleurogramme
 Pleurolobus
 Pleuromanes
 Pleuropappus
 Pleuropedium
 Pleuropetalon
 Pleuropetalum
 Pleurophascum
+Pleurophoma
 Pleurophyllum
 Pleuroplitis
 Pleuroschisma
 Pleurosigma
 Pleurosira
 Pleurosorus
 Pleurostomophora
@@ -9855,14 +10126,15 @@
 Plumbago
 Pluteolus
 Pluteus
 Pneophyllum
 Pneumatopteris
 Pneumocystis
 Poa
+Poaceascoma
 Pocheina
 Pocillaria
 Pocockiella
 Pocsia
 Poculinia
 Podalyria
 Podanthe
@@ -9986,14 +10258,15 @@
 Polystigma
 Polystigmina
 Polytaenium
 Polythrinciopsis
 Polythrincium
 Polytoca
 Polytocha
+Polytretophora
 Polytrias
 Polytrichadelphus
 Polytrichastrum
 Polytrichum
 Polyzone
 Polyzonia
 Pomaderris
@@ -10011,27 +10284,29 @@
 Pongelia
 Pontania
 Pontederia
 Pontogeneia
 Pootia
 Popanax
 Popowia
+Populomyces
 Populus
 Porana
 Poranthera
 Porella
 Poria
 Porina
 Porinella
 Porinula
 Porobeltraniella
 Porocarpus
 Poroceratium
 Porocyphus
 Porodaedalea
+Porodiplodia
 Porodisculus
 Porogramme
 Porolithon
 Poronia
 Porophyllum
 Porospermum
 Porostereum
@@ -10042,14 +10317,15 @@
 Porphyra
 Porphyrellus
 Porphyridium
 Porphyropsis
 Porphyrosiphon
 Porpidia
 Porpoloma
+Porpolomopsis
 Porpomyces
 Porroteranthe
 Portenschlagia
 Porterandia
 Portieria
 Portphillipia
 Portulaca
@@ -10066,21 +10342,24 @@
 Poteriodendron
 Poterium
 Pothomorphe
 Pothos
 Potomorphe
 Potoromyces
 Potridiscus
+Pottera
 Pottia
 Pouchetia
 Pouteria
+Pouzarella
 Pouzaromyces
 Pouzolsia
 Pouzolzia
 Powellia
+Powelliopsis
 Powellomyces
 Pozoa
 Pozoopsis
 Pozopsis
 Praecoxanthus
 Prainea
 Prasiola
@@ -10153,14 +10432,15 @@
 Protopannaria
 Protoparmelia
 Protoperidinium
 Protopsis
 Protosiphon
 Protostegia
 Protostelium
+Protostropharia
 Prototremella
 Prototrichia
 Protoventuria
 Protoxerula
 Protubera
 Prumnopitys
 Prunella
@@ -10186,61 +10466,68 @@
 Pseudatalaza
 Pseudelephantopus
 Pseudendoclonium
 Pseudephebe
 Pseudephemerum
 Pseuderanthemum
 Pseuderiospora
+Pseudictyota
 Pseuditea
 Pseudixus
 Pseudo-eunotia
 Pseudoacrodictys
 Pseudoamauroascus
+Pseudoannulatascus
 Pseudoarachniotus
+Pseudoaustroboletus
 Pseudobaeospora
 Pseudobalsamia
 Pseudobeltrania
+Pseudoblindia
 Pseudobotrytis
 Pseudobrachiaria
 Pseudobryopsis
 Pseudocamptoum
 Pseudocarapa
 Pseudocephalozia
 Pseudocercospora
 Pseudocercosporella
 Pseudochaete
 Pseudochaetochloa
+Pseudochaetosphaeronema
 Pseudochlorococcum
 Pseudochlorodesmis
 Pseudochrosia
 Pseudoclitocybe
 Pseudococcomyxa
 Pseudocochliobolus
 Pseudocodium
 Pseudocolus
 Pseudocraterellus
 Pseudocrossidium
 Pseudocryptocarya
 Pseudocyphellaria
+Pseudodactylaria
 Pseudodiphasium
 Pseudodiplodia
-Pseudoendoclonium
+Pseudodiscosia
 Pseudoepicoccum
 Pseudofallacia
 Pseudofavolus
 Pseudofumaria
 Pseudofusicoccum
 Pseudogloiophloea
 Pseudognaphalium
 Pseudoguinardia
 Pseudohalonectria
 Pseudohansfordia
 Pseudohelotium
 Pseudohydnum
 Pseudohypnella
+Pseudoidium
 Pseudoidriella
 Pseudoinonotus
 Pseudolagarobasidium
 Pseudolembosia
 Pseudolepicolea
 Pseudoleskea
 Pseudoleskeopsis
@@ -10248,23 +10535,25 @@
 Pseudolithophyllum
 Pseudolpidium
 Pseudolycopodiella
 Pseudolycopodium
 Pseudolyophyllum
 Pseudomarsupidium
 Pseudomassaria
-Pseudombrophila
 Pseudomerulius
+Pseudomicrostroma
 Pseudomorus
 Pseudonitzschia
 Pseudopanax
 Pseudoparmelia
 Pseudopetrakia
+Pseudopeyronellaea
 Pseudopeziza
 Pseudophacidium
+Pseudophaeophleospora
 Pseudophalacroma
 Pseudophloeospora
 Pseudopholidia
 Pseudophormidium
 Pseudophycodrys
 Pseudopipturus
 Pseudoplagiostoma
@@ -10277,33 +10566,37 @@
 Pseudoramonia
 Pseudoraphis
 Pseudorhizoclonium
 Pseudosagedia
 Pseudoscinaia
 Pseudoscleropodium
 Pseudosolenia
+Pseudosperma
 Pseudosphaeria
 Pseudospiridentopsis
 Pseudospiropes
 Pseudostaurastrum
 Pseudostaurosira
+Pseudosydowia
 Pseudosymblepharis
 Pseudotaxiphyllum
 Pseudotetracystis
 Pseudotetraedron
 Pseudotis
 Pseudotomentella
 Pseudotracya
 Pseudotrebouxia
 Pseudotremellodendron
 Pseudotsuga
 Pseudovanilla
 Pseudoweinmannia
 Pseudowilloughbeia
+Pseudoxylomyces
 Pseudoxytenanthera
+Pseudozasmidium
 Pseuduvaria
 Psidiomyrtus
 Psidium
 Psilanthus
 Psilobotrys
 Psilocarya
 Psilocaulon
@@ -10338,14 +10631,15 @@
 Psychotrophum
 Psychrophila
 Psycrophila
 Psydrax
 Psylliostachys
 Pteridium
 Pteridoblechnum
+Pteridopassalora
 Pteridrys
 Pterigeron
 Pterigospermum
 Pterigynandrum
 Pteris
 Pternandra
 Pterobryella
@@ -10437,14 +10731,15 @@
 Punctelia
 Punctonora
 Punctularia
 Pungamia
 Punica
 Punicella
 Pupalia
+Purpureocillium
 Pursellia
 Pusaetha
 Pustula
 Pustularia
 Pustulina
 Pycnarrhena
 Pycnolachne
@@ -10504,15 +10799,14 @@
 Pyrus
 Pythiacystis
 Pythiogeton
 Pythiomorpha
 Pythium
 Pyxidaria
 Pyxidicula
-Pyxidiophora
 Pyxine
 Quadrigula
 Quadrispora
 Quambalaria
 Quamoclit
 Quamoclita
 Quasidiscus
@@ -10525,14 +10819,15 @@
 Quinetia
 Quinqueremulus
 Quintaria
 Quintinia
 Quisqualis
 Quoya
 Rabdochloa
+Rachicladosporium
 Raciborskiella
 Racodium
 Racomitrium
 Racopilum
 Racopsperma
 Racosperma
 Racospermyces
@@ -10600,24 +10895,26 @@
 Redeckera
 Reedia
 Reediella
 Reesia
 Regelia
 Rehmiellopsis
 Rehmiodothis
+Reholttumia
 Reichardia
 Reimnitzia
 Reinboldia
 Reineria
 Reinschiella
 Reinwardtia
 Relicina
 Relicinopsis
 Remirea
 Remispora
+Remotididymella
 Remototrachyna
 Remusatia
 Renanthera
 Rendlia
 Renealmia
 Reptataxis
 Reseda
@@ -10693,14 +10990,16 @@
 Rhizidium
 Rhizina
 Rhizoblepharia
 Rhizocarpon
 Rhizochaete
 Rhizoclonium
 Rhizoctonia
+Rhizocybe
+Rhizoglomus
 Rhizogonium
 Rhizolamellia
 Rhizomucor
 Rhizophagus
 Rhizophlyctis
 Rhizophora
 Rhizophydium
@@ -10718,14 +11017,16 @@
 Rhodochorton
 Rhodocladia
 Rhodocollybia
 Rhodocybe
 Rhododactylis
 Rhododendron
 Rhododiplobia
+Rhodofomes
+Rhodofomitopsis
 Rhodoglossum
 Rhodolophia
 Rhodomela
 Rhodomenia
 Rhodomonas
 Rhodomyrtus
 Rhodonema
@@ -10779,15 +11080,14 @@
 Rhyticaryum
 Rhytidandra
 Rhytidanthe
 Rhytidhysterium
 Rhytidiadelphus
 Rhytidochlamys
 Rhytidosporum
-Rhytileucoma
 Rhytisma
 Rhytispermum
 Ribes
 Ribesiodes
 Ricasolia
 Riccardia
 Riccia
@@ -10799,14 +11099,15 @@
 Richea
 Richoniella
 Richteriella
 Ricinocarpos
 Ricinocarpus
 Ricinus
 Rickenella
+Rickia
 Ridleia
 Riedelia
 Riedlea
 Riedleia
 Riedleja
 Riedleya
 Riedlia
@@ -10865,22 +11166,24 @@
 Roperia
 Rophostemon
 Roptrostemon
 Roridella
 Roridomyces
 Rorippa
 Rosa
+Rosbeeva
 Roschera
 Rosellinia
 Roselliniella
 Rosellinula
 Rosenscheldiella
 Rosenvingea
 Rosenvingiella
 Rosmarinus
+Rossbeevera
 Rossithidium
 Rossittia
 Rostafinskia
 Rostellaria
 Rostellularia
 Rostranthus
 Rostraria
@@ -10954,15 +11257,17 @@
 Saccobolus
 Saccogyna
 Saccogynidium
 Saccolabiopsis
 Saccolabium
 Saccomorpha
 Saccopetalum
+Saccothecium
 Sacidium
+Sagaranella
 Sagediopsis
 Sagenia
 Sagenidiopsis
 Sagenidium
 Sagenoma
 Sagenomella
 Sageretia
@@ -10973,14 +11278,15 @@
 Sagotia
 Sagrahamala
 Saguaster
 Saguerus
 Sagus
 Sahlingia
 Sainsburia
+Saitozyma
 Saksenaea
 Salacia
 Salacicratea
 Salacistis
 Salicornia
 Salisia
 Salix
@@ -10996,31 +11302,34 @@
 Samara
 Sambucus
 Samolus
 Sanchezia
 Sandfordia
 Sandoricum
 Sanfordia
+Sanguinoderma
 Sanguisorba
 Sanionia
 Sankowskia
 Sankowskya
 Sannantha
 Sanseverinia
+Sanseviera
 Sansevieria
 Santalodes
 Santaloides
 Santalum
 Santessoniella
 Santis
 Santolina
 Sapindus
 Sapium
 Saponaria
 Sapota
+Saproamanita
 Saprochaete
 Saprolegnia
 Sapromyces
 Saprosma
 Sarauia
 Sarcanthopsis
 Sarcanthus
@@ -11062,14 +11371,15 @@
 Sarcozona
 Sarcozygium
 Sarga
 Sargassopsis
 Sargassum
 Saribus
 Saritaea
+Sarmentypnum
 Sarojusticia
 Saropsis
 Sarotes
 Sarothamnus
 Sarracenia
 Sarrameana
 Sarsalisia
@@ -11214,14 +11524,15 @@
 Sciodaphyllum
 Scirpodendron
 Scirpoides
 Scirpus
 Scirrhia
 Scirrhodothis
 Scirrhophorus
+Sciuro-hypnum
 Sclerachne
 Sclerandrium
 Scleranthus
 Scleria
 Sclerobassia
 Scleroblitum
 Sclerocarya
@@ -11234,14 +11545,15 @@
 Sclerodontium
 Sclerogaster
 Scleroglossum
 Sclerogone
 Sclerolaena
 Scleroleima
 Scleromitrion
+Scleromyces
 Sclerophora
 Sclerophyton
 Sclerophytonomyces
 Scleropoa
 Scleropodium
 Scleroschoenus
 Sclerospora
@@ -11326,14 +11638,15 @@
 Seirospora
 Seismosarca
 Selaginella
 Selago
 Selenastrum
 Selenicereus
 Selenodesmium
+Selenodriella
 Selenophoma
 Selenosporella
 Selenosporium
 Selenothamnus
 Seligeria
 Selinia
 Sellaphora
@@ -11343,14 +11656,15 @@
 Semasperma
 Sematophyllum
 Semecarpus
 Semidelitschia
 Semifissispora
 Semigyalecta
 Seminavis
+Semiphajus
 Semnocarpa
 Senacia
 Senebiera
 Senecio
 Senegalia
 Senna
 Senniella
@@ -11393,27 +11707,29 @@
 Sestochilos
 Sesuvium
 Setameliola
 Setaria
 Setchelliogaster
 Setella
 Setiscapella
+Setophaeosphaeria
 Setophoma
 Setosa
 Setosphaeria
 Setosynnema
 Seuratia
 Severinia
 Seynesia
 Seynesiella
 Shawia
 Sheffieldia
 Shepleya
 Sherardia
 Shionodiscus
+Shirahamella
 Shivasia
 Shonia
 Shoutensia
 Shuteria
 Sicyos
 Sida
 Sidera
@@ -11444,28 +11760,30 @@
 Simonsenia
 Simpliglottis
 Simsia
 Simuliomyces
 Sinapis
 Sindora
 Singerella
+Singerocybe
 Singularybas
 Sinkoraena
 Sinoga
 Siona
 Siphonanthus
 Siphoneranthemum
 Siphonocladus
 Siphonodiscus
 Siphonodon
 Siphonogramen
 Siphonolejeunea
 Siphula
 Siphulastrum
 Siphulella
+Sirastachys
 Sirenophila
 Sirmuellera
 Sirobasidium
 Sirodotia
 Sirogonium
 Sirophysalis
 Sirosporium
@@ -11486,14 +11804,15 @@
 Skirrhophorus
 Skirrophorus
 Skitophyllum
 Skyttea
 Sloanea
 Smardaea
 Smilax
+Smithanthe
 Smithia
 Smittium
 Smyrnium
 Snowdenia
 Snowella
 Solandra
 Solanum
@@ -11509,14 +11828,15 @@
 Solenostigma
 Solenostoma
 Solidago
 Solieria
 Solitaria
 Soliva
 Sollya
+Solmsiella
 Solori
 Solorina
 Solosympodiella
 Solulus
 Sonchus
 Sondera
 Sonderella
@@ -11575,14 +11895,15 @@
 Spatoglossum
 Spatulodinium
 Speculantha
 Specularia
 Spegazzinia
 Speiropsis
 Spencerella
+Spencermartinsia
 Spergula
 Spergularia
 Spermacoce
 Spermatochnus
 Spermaxyrum
 Spermodon
 Spermothamion
@@ -11679,14 +12000,15 @@
 Spirocoleus
 Spiroconus
 Spirodela
 Spirodinium
 Spirogardnera
 Spirographa
 Spirogyra
+Spiromastigoides
 Spiromastix
 Spironema
 Spiropes
 Spirophycus
 Spiropodium
 Spirotaenia
 Spirulina
@@ -11728,14 +12050,15 @@
 Sporodum
 Sporoglossum
 Sporolithon
 Sporopodium
 Sporormia
 Sporormiella
 Sporoschisma
+Sporoschismopsis
 Sporothrix
 Sporotrichum
 Sprengalia
 Sprengelia
 Springalia
 Sprucea
 Spruceanthus
@@ -11745,15 +12068,14 @@
 Spyridia
 Spyridium
 Spyridum
 Squamacidia
 Squamarina
 Squamella
 Squamulea
-Stableria
 Stachybotrys
 Stachycarpus
 Stachygynandrum
 Stachylidium
 Stachylina
 Stachypitys
 Stachys
@@ -11761,14 +12083,16 @@
 Stachytarpheta
 Stackhousia
 Stadmannia
 Stadtmannia
 Stagonospora
 Stamnorchis
 Staninwardia
+Stanjehughesia
+Stanjemonium
 Stapelia
 Stapeliopsis
 Stapfiola
 Staphylotrichum
 Statice
 Staurastrum
 Staurocarpus
@@ -11802,14 +12126,16 @@
 Steiroglossa
 Stekhovia
 Stelbophyllum
 Stelechocarpus
 Stellaria
 Stellarima
 Stelligera
+Stellorchis
+Stellorkis
 Stellospora
 Stemaria
 Stemmacantha
 Stemmatophyllum
 Stemmodia
 Stemodia
 Stemodiacra
@@ -11824,15 +12150,14 @@
 Stenella
 Stenocarpus
 Stenochilus
 Stenochlaena
 Stenocladia
 Stenodiscus
 Stenogramma
-Stenogramme
 Stenolejeunea
 Stenolobium
 Stenolobus
 Stenoloma
 Stenopeltis
 Stenopetalum
 Stenophragma
@@ -11870,15 +12195,14 @@
 Stichococcus
 Sticta
 Stictina
 Stictis
 Stictocardia
 Stictodiscus
 Stictolejeunea
-Stictophyllium
 Stictophyllum
 Stictosiphonia
 Stictosporum
 Stictyosiphon
 Stigeoclonium
 Stigmaphyllon
 Stigmarota
@@ -11910,14 +12234,16 @@
 Stirtonia
 Stirtoniella
 Stizolobium
 Stobaea
 Stockwellia
 Stoechadomentha
 Stoechospermum
+Stollia
+Stolonochloa
 Stomarrhena
 Stomatogenella
 Stomiopeltis
 Stomoisia
 Stonea
 Stoneobryum
 Stonesiella
@@ -11965,14 +12291,15 @@
 Strombocarpa
 Strombomonas
 Strongylocaryum
 Strongylodon
 Strongylosperma
 Strongylospermum
 Stropharia
+Strophocaulon
 Strophostyles
 Strossmayeria
 Strumella
 Struthiopteris
 Struvea
 Strychnos
 Strzeleckia
@@ -12002,25 +12329,29 @@
 Stypandra
 Styphelia
 Stypocaulon
 Styponema
 Stypopodium
 Stysanus
 Suaeda
+Suberoteratosphaeria
 Submersisphaeria
 Subulicium
 Subulicystidium
 Subulispora
 Succowia
+Sugiyamaella
+Suillellus
 Suillus
 Sukunia
 Sulitia
 Sullivania
 Sundacarpus
 Sundstroemia
+Superstratomyces
 Suregada
 Surenus
 Suriana
 Suringaria
 Suringariella
 Surirella
 Surreya
@@ -12038,14 +12369,15 @@
 Sycios
 Sycomorus
 Sydowia
 Sylvipoa
 Symbiezidium
 Symbiodinium
 Symblepharis
+Symmetrospora
 Symonanthus
 Symphiobasis
 Symphionema
 Symphoricarpos
 Symphyobasis
 Symphyocladia
 Symphyogyna
@@ -12053,20 +12385,22 @@
 Symphyomera
 Symphyomyrtus
 Symphyonema
 Symphyopetalon
 Symphyopetalum
 Symphyotrichum
 Symphysocarpus
+Symphysodontella
 Symphytocarpus
 Symphytum
 Symplectrodia
 Symploca
 Symplocos
 Sympodophyllum
+Sympoventuria
 Synadenium
 Synalissa
 Synaphea
 Synaptantha
 Synarrhena
 Synarthrophyton
 Syncarpella
@@ -12079,17 +12413,20 @@
 Syncrypta
 Syndendrium
 Synechoblastus
 Synechococcus
 Synedra
 Synedrella
 Synedrellopsis
+Synedropsis
 Syngonium
 Syngramma
 Synima
+Synmeria
+Synnemellisia
 Synnotia
 Synostemon
 Synoum
 Syntherisma
 Syntrichia
 Synura
 Syracosphaera
@@ -12149,14 +12486,15 @@
 Tarennoidea
 Targionia
 Tarlmounia
 Tarrietia
 Tarzetta
 Taschneria
 Tasmania
+Tasmaniomyxa
 Tasmannia
 Tasmidella
 Tatea
 Taurantha
 Taurodium
 Taverniera
 Taxandria
@@ -12174,14 +12512,15 @@
 Tecomella
 Tectaria
 Tectella
 Tecticornia
 Tectona
 Teesdalia
 Tegicornia
+Teichospora
 Teilingia
 Tekel
 Tekelia
 Telanthera
 Telaranea
 Telimena
 Teline
@@ -12192,22 +12531,25 @@
 Temminckia
 Temninckia
 Temnoma
 Templetonia
 Tenaciphyllum
 Tenagocharis
 Tenarea
+Tenuipostia
 Tephrocybe
 Tephromela
 Tephrosea
 Tephrosia
 Teramnus
 Terana
 Teratophyllum
+Teratoramularia
 Teratosphaeria
+Teratosphaericola
 Terebinthina
 Terebraria
 Terfezia
 Terminalia
 Terminalis
 Termitaria
 Termitomyces
@@ -12274,14 +12616,15 @@
 Tetrasynandra
 Tetrathamnion
 Tetratheca
 Tetrathylax
 Tetrodon
 Teucridium
 Teucrium
+Teunia
 Thalamia
 Thalamnia
 Thalassia
 Thalassionema
 Thalassiosira
 Thalassiothrix
 Thalassodendron
@@ -12332,14 +12675,15 @@
 Thelopsis
 Thelotrema
 Thelychiton
 Thelymitra
 Thelypteris
 Themeda
 Theobroma
+Thermothielavioides
 Therogeron
 Therrya
 Thesium
 Thespesia
 Thespidium
 Thevetia
 Thielavia
@@ -12385,19 +12729,21 @@
 Thyridium
 Thyridolepis
 Thyrinula
 Thyrostroma
 Thyrsacanthus
 Thysananthus
 Thysanella
+Thysanochilus
 Thysanocladia
 Thysanolaena
 Thysanomitrion
 Thysanothecium
 Thysanothus
+Thysanotis
 Thysanotus
 Tiaridium
 Tiarophora
 Tiarosporella
 Tibellia
 Tibouchina
 Tieghemopanax
@@ -12430,18 +12776,20 @@
 Tittmannia
 Tmesipteris
 Tobira
 Todea
 Toechima
 Togninia
 Togula
+Toloxis
 Tolpis
 Tolypella
 Tolypellopsis
 Tolypiocladia
+Tolypocladium
 Tolypoderma
 Tolyposporidium
 Tolyposporium
 Tolypothrix
 Tomaculopsis
 Tomasellia
 Tomentella
@@ -12460,15 +12808,17 @@
 Torilis
 Tormentilla
 Torodinium
 Torpedospora
 Torquentidium
 Torrendia
 Torrendiella
+Torrentaria
 Torrenticola
+Torrentispora
 Torresia
 Torreya
 Tortella
 Tortula
 Torula
 Torulinium
 Torulomyces
@@ -12504,19 +12854,21 @@
 Trachypogon
 Trachypus
 Trachyrhizum
 Trachysphenia
 Trachystemon
 Trachystylis
 Trachythecium
+Tracylla
 Tradescantia
 Tragia
 Tragopogon
 Tragus
 Trametes
+Trametopsis
 Tranzschelia
 Tranzscheliella
 Trapa
 Trapelia
 Trapeliopsis
 Traponora
 Trebouxia
@@ -12561,14 +12913,15 @@
 Trichandrum
 Trichanthodium
 Trichaptum
 Tricharia
 Tricharina
 Trichelostyles
 Trichelostylis
+Tricherpodium
 Trichia
 Trichidium
 Trichilia
 Trichinium
 Trichinum
 Trichobasis
 Trichobelonium
@@ -12603,14 +12956,15 @@
 Trichonema
 Trichopeltis
 Trichopeltula
 Trichopeziza
 Trichophaea
 Trichophilus
 Trichophyton
+Trichopilus
 Trichormus
 Trichoryne
 Trichosanthes
 Trichoscypha
 Trichosiphon
 Trichosiphum
 Trichosolen
@@ -12658,14 +13012,15 @@
 Trimmatothelopsis
 Trinacrium
 Trinathotrema
 Trineuron
 Trinitaria
 Triodanis
 Triodia
+Triodiomyces
 Trioncinia
 Triosteum
 Tripetelus
 Triphasia
 Triphelia
 Triphragmium
 Triphysaria
@@ -12719,14 +13074,15 @@
 Trochocarpa
 Trocholejeunea
 Trogia
 Trogostolon
 Trollius
 Tropaeolum
 Trophis
+Tropicoporus
 Tropidia
 Tropidoneis
 Tropidoscyphus
 Tropilis
 Tropilus
 Troposporella
 Truellum
@@ -12740,14 +13096,15 @@
 Trymalium
 Trypetheliopsis
 Trypethelium
 Tryptomene
 Tryssglobulus
 Tsengia
 Tubaria
+Tubariomyces
 Tuber
 Tubercularia
 Tuberculina
 Tuberolabium
 Tubifera
 Tubularia
 Tubulicium
@@ -12785,14 +13142,15 @@
 Tylophoron
 Tylopilus
 Tylothallia
 Tylotus
 Tyndaridea
 Typha
 Typhonium
+Typhrasa
 Typhula
 Typtomene
 Tyrbastes
 Tyromyces
 Tysonia
 Tzvelevia
 Udora
@@ -12878,14 +13236,15 @@
 Ustulina
 Utania
 Uthatobasidium
 Utricularia
 Uva
 Uvaria
 Uvedalia
+Uwebraunia
 Vaccaria
 Vachellia
 Vacoparis
 Vacuolaria
 Vaginata
 Vaginatispora
 Vaginularia
@@ -12895,14 +13254,15 @@
 Valerianoides
 Valeriemaya
 Vallaris
 Vallisneria
 Valonia
 Valoniopsis
 Valsa
+Valsonectria
 Valvanthera
 Valvaria
 Van-royena
 Vanda
 Vandaisia
 Vandasia
 Vandasina
@@ -12929,43 +13289,49 @@
 Vauthiera
 Vavaea
 Veitchia
 Veleroa
 Veligaster
 Vella
 Velleia
+Velleja
 Vellereophyton
 Velleya
+Veloboletus
 Velutarina
 Veluticeps
 Venidium
 Ventenatia
 Ventilago
 Ventricaria
 Venturia
+Venturiella
 Vepris
 Veratrum
 Verbascum
 Verbena
 Verbesina
 Verdcourtia
 Verdoornia
 Vermicularia
 Vermiculariella
+Vermiculariopsiella
+Vermiculariopsis
 Vermisporium
 Vernicia
 Vernonia
 Veronaea
 Veronica
 Verreauxia
 Verrucalvus
 Verrucaria
 Verrucidens
 Verrucispora
 Verrucisporota
+Verrucoconiothyrium
 Verruculina
 Versiomyces
 Versipellis
 Vertebrata
 Verticicladiella
 Verticicladium
 Verticillium
@@ -12981,14 +13347,15 @@
 Vicia
 Vicinia
 Vidalia
 Viennotidia
 Vieusseuxia
 Vigna
 Vignea
+Vikalpa
 Vilfa
 Villaresia
 Villarsia
 Viminaria
 Vinassaella
 Vinca
 Vincetoxicum
@@ -12999,14 +13366,15 @@
 Vireya
 Virgilia
 Viridivellus
 Viridothelium
 Virotia
 Viscum
 Visenia
+Vishniacozyma
 Visum
 Vitalianthus
 Vitex
 Viticipremna
 Vitis
 Vittadinia
 Vittaria
@@ -13035,14 +13403,15 @@
 Waihonghopes
 Wailesia
 Waireia
 Waitea
 Waitzia
 Wakefieldia
 Walcottia
+Walkaminomyces
 Wallemia
 Wallrothia
 Walpersia
 Walshia
 Walsholaria
 Walteranthus
 Waltheria
@@ -13068,14 +13437,15 @@
 Websteria
 Weddellomyces
 Wedelia
 Wehlia
 Weihea
 Weinmannia
 Weinmanniaphyllum
+Weisiopsis
 Weissia
 Welchiodendron
 Wendlandia
 Wentiomyces
 Weraroa
 Westea
 Westella
@@ -13110,14 +13480,15 @@
 Willemetia
 Willeya
 Willkommlangea
 Wilsonaea
 Wilsonia
 Wilsoniella
 Windmannia
+Wingfieldomyces
 Winifredia
 Winika
 Winterana
 Winterania
 Winterella
 Wirtgenia
 Wissadula
@@ -13125,23 +13496,25 @@
 Wisteria
 Withania
 Witheringia
 Wittrockiella
 Wittsteinia
 Wodyetia
 Woessia
+Wojnowiciella
 Wolffia
 Wolfia
 Wollastonia
 Wollastoniella
 Wollea
 Wollemia
 Wollemiaster
 Woloszynskia
 Womersleya
+Wongia
 Woodia
 Woodsia
 Woodwardia
 Woollsia
 Wormia
 Woronichinia
 Woroninella
@@ -13183,25 +13556,31 @@
 Xanthostemon
 Xanthoxylon
 Xanthoxylum
 Xantolis
 Xantorrhoea
 Xenasma
 Xenasmatella
+Xenoanthostomella
 Xenodendron
+Xenogliocladiopsis
 Xenonectriella
+Xenopassalora
+Xenosonderhenia
 Xenostegia
 Xepicula
 Xeraea
 Xeranthemum
 Xerocarpa
 Xerocarpus
 Xerochloa
+Xerochrysium
 Xerochrysum
 Xerocomus
+Xerogeomyces
 Xerolirion
 Xeromesos
 Xeromphalina
 Xeromphis
 Xerosollya
 Xerotes
 Xerothamnella
@@ -13212,14 +13591,15 @@
 Ximenesia
 Ximenia
 Xiphion
 Xiphophora
 Xiphophyllanthus
 Xiphopteris
 Xuris
+Xyladictyochaeta
 Xylaria
 Xylobolus
 Xylocarpus
 Xylochlamys
 Xylococcus
 Xylodon
 Xylographa
@@ -13252,15 +13632,14 @@
 Zahlbrucknerella
 Zaleija
 Zalerion
 Zaleya
 Zaluzianskia
 Zaluzianskya
 Zamia
-Zamioculcas
 Zanardinia
 Zanardinula
 Zanclospora
 Zanichellia
 Zannichellia
 Zanonia
 Zantedeschia
@@ -13288,14 +13667,15 @@
 Zigmaloba
 Zignoella
 Zignoina
 Zingiber
 Zinnia
 Ziziphus
 Zizyphus
+Zodiomyces
 Zoellneria
 Zoisia
 Zonaria
 Zoochlorella
 Zoophthalmum
 Zoophthora
 Zoopsis
@@ -13316,15 +13696,14 @@
 Zygochloa
 Zygodesmus
 Zygodon
 Zygogonium
 Zygogynum
 Zygomenes
 Zygophyllum
-Zygopleurage
 Zygorhynchus
-Zygospermella
 Zygosporium
 Zymurgia
 Zythia
 Zythiostroma
-[Genus Not Recorded]
+aspera x queenslandica
+xAbacopterella
```

### Comparing `hespi-0.4.2/hespi/data/mk-lists.py` & `hespi-0.4.4/hespi/data/mk-lists.py`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/data/references.bib` & `hespi-0.4.4/hespi/data/references.bib`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/data/species.txt` & `hespi-0.4.4/hespi/data/species.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "Blesing" (J.R.Wheeler 461)
+"Cordillo Downs" (B.Lay 1487)
 "Kalpowar" (Fell 2969)
 "Lake Eyre" (K.Chorney 999)
 "Lake McDonald" (Bean 6770)
 "Linear segments" (K.Preiss 128)
 "Marree" (F.J.Badman 776)
 "Mt Garnet" (Myers s.n.)
 "Newcastle Bay" (Brass 18671)
@@ -210,25 +211,40 @@
 A89992 Wakaya Desert
 A90358 Walhallow Station
 A90679 Limestone (Sp. "B" FCA)
 A90788 Tobermorey Station
 A92973 Elliott
 A93357 Western Tanami
 A94522 long style
+Amanita  sp. 'LEM 35-2005'
+Amanita  sp. 'LEM 41-2005'
+Amanita  sp. 'LEM 6-2005'
+Amanita sp. 'EMD 15-1995'
+Amanita sp. 'EMD 54-1990'
+Amanita sp. 'EMD 7-1995'
+Amanita sp. 'EMD 8-2003'
+Amanita sp. 'LEM 13-2005'
+Amanita sp. 'LEM 19-2005'
+Amanita sp. 'LEM 8-2005'
+Amanita sp. 'MEL2151450' of Sawyer et al. in Genbank
+Amanita sp. 'persicina' sensu Bougher (2009)
 Annonaceae sp. (=RFK/1986)
 Annonaceae sp. (=RFK/2741)
 Annonaceae sp. (=RFK/3337)
 Annonaceae sp. (RFK/2741)
 B. Polyanthon
 Bastowii
 Bush Rebel
+Campanella sp. of Bougher (2007: Bougher E3689, PERTH)
 CandyCones
 Carmat
 Celastraceae sp. (Claudie River BH 21098V)
-Celtica (other taxa) Fl. Australia 2015 (A.C.Beauglehole 78369)
+Chytriomyces sp. '#1'
+Chytriomyces sp. 'Miller's Dentate'
+Chytriomyces sp. 'No. 2'
 Clearview Dwarf
 Clearview John
 Coral
 Coral Beauty
 Curtain Call
 D019989 Jabiru
 D123061 Goose Creek
@@ -296,19 +312,24 @@
 Dianella sp. Reservoir Hill (G.M.Cunningham 325)
 Euphorbiaceae sp. (=AFO/411)
 Euphorbiaceae sp. (=RFK/1080)
 Euphorbiaceae sp. (=RFK/1225)
 Euphorbiaceae sp. (=RFK/2817)
 Euphorbiaceae sp. (=RFK/3501)
 Flacourtiaceae sp. (=GS/517)
+Glomus sp. 'WUM 4' of Hall & Fish (1979)
+Glomus sp. 'WUM 5' of Hall & Fish (1979)
 Group 1 species
 Group A
 Haast Bluff Stn (P.K.Latz 7624)
 Hale
 Halosarcia x uniflora
+Heimiella sp. 'BRIP 9132'
+Hysterangium sp. '2'
+Hysterangium sp. '3'
 Litchfield entity
 Louisiana Hybrid Group
 Martini
 Monimiaceae Gen. Nov. sp. (Davies Creek LJW 6430)
 Monimiaceae Gen. nov. sp. (Davies Creek)
 Monimiaceae Gen. nov. sp. (McDowall Range)
 Monimiaceae Gen. nov. sp. (Mt Hemmant)
@@ -318,14 +339,16 @@
 Myrtaceae Gen. Nov. sp. (Boonjee BH 6589)
 Myrtaceae Gen. nov. sp. (Boonjee)
 Myrtaceae gen. nov. sp. (=RFK/2519)
 Nabarlek entity
 Neutral Junction entity
 Ninderry-Gold
 Pink SugarCandy
+Pisolithus sp. 'LJ30' of Anderson et al. (2001), Martin et al. (2002)
+Pisolithus sp. 'MH97' of Martin et al. (2002)
 Proteaceae sp. 'Devils Thumb'
 Proteaceae sp. (=RFK/2226)
 Proteaceae sp. (=RFK/3505)
 Proteaceae sp. (Mt Bartle Frere)
 Proteaceae sp. (RFK 3505)
 Proteaceae sp. Mt Bartle Frere
 Q2 (clipicola)
@@ -335,25 +358,28 @@
 Rubiaceae Gen. nov. sp. (Boonjee)
 Rubiaceae Gen. nov. sp. (Shute Harbour)
 Rubiaceae sp. (Sessile Fruits)
 Sapindaceae sp. (=AFO/70)
 Sapindaceae sp. (=RFK/2311)
 Sapindaceae sp. (Noah Creek BG 6026)
 Sapindaceae sp. (Noah Creek)
-Silver Plains (P.I.Forster PIF17005)
 Simaroubaceae sp. Mary River (I.D.Cowie 1454)
 Swan river
+Synchytrium sp. '2061' in ADW on <I>Hydrocotyle callicarpa</I>
+Tylopilus sp. '6 (BRIP 9175)' of Watling & Gregory (1989a)
 Ulmaceae sp. (=RFK/2534)
 Unnamed sp.
 Unnamed taxon
+Uredo sp. 'DAR57117' of Shivas (1989)
 Utricularia sp. Fanged (R.W.Jobson 2682)
 Victoria River entity
 W.L. 1. sensu Thomasson & P. Tyler (1971)
-Wangi (S.E.Pickering 20)
 [unknown]
+a sp. Bayswater (C.Andrews s.n. 11/1902)
+a sp. Kongorow Pool (M.D.Barrett & K.W.Dixon MDB 4556)
 abaphoides
 abaujensis
 abaxialis
 abbatiana
 abbatianum
 abblittiorum
 abbottiae
@@ -424,16 +450,18 @@
 abyssa
 abyssinica
 abyssinicum
 abyssus
 acaciae
 acaciae-mearnsii
 acaciaeformis
+acaciaformis
 acaciarum
 acaciformis
+acacigena
 acaciiformis
 acaciigena
 acaciodes
 acacioides
 acadiana
 acaenincola
 acanthaster
@@ -459,14 +487,15 @@
 acanthophora
 acanthophorum
 acanthophylla
 acanthophyllus
 acanthopoda
 acanthos
 acanthoscarpa
+acanthosperma
 acanthostachya
 acanthosyrinus
 acanthymenia
 acaricida
 acaridis
 acariformis
 acarinophila
@@ -562,14 +591,15 @@
 acinacea
 acinaceum
 acinacifolium
 acinaciforme
 acinaciformis
 acinaria
 aciniformis
+acinonychum
 acinorum
 acinus
 aciphylla
 aciphyllum
 acithecium
 ackeringae
 acmella
@@ -647,14 +677,15 @@
 actinoclada
 actinocladus
 actinodendron
 actinophora
 actinophylla
 actinophyllum
 actinoptychum
+actinoschoeni
 actinostachys
 actinostomus
 actinostrobus
 actinota
 actites
 actydrophila
 acuaria
@@ -674,24 +705,22 @@
 aculeolatus
 acuminata
 acuminata (narrow phyllode variant)
 acuminata (small seed variant)
 acuminata x balbisiana
 acuminatissima
 acuminatum
-acuminatum - australe
 acuminatus
 acuminiger
 acuminigera
 acupunctata
 acupunctatum
 acupunctatus
 acus
 acuta
-acuta x platyphylla
 acutangula
 acutangulum
 acutangulus
 acutata
 acutatum
 acutatus
 acutesquamosa
@@ -829,28 +858,26 @@
 adspersa
 adspersum
 adspersus
 adstrictum
 adsurgens
 adsurgens x rhodophloia
 adulterina
-adumbrans
 adunca
 adunca x neriifolia
 aduncum
 aduncus
 adusta
 adustum
 adustus
 advena
 advenus
 aecidiicola
 aecidiorum
 aegagropila
-aegagropiliodea
 aegagropiloidea
 aegeridantennata
 aegeridantennatus
 aegerita
 aegerrime
 aegialita
 aegiceras
@@ -933,14 +960,15 @@
 aestiva
 aestivale
 aestivalis
 aestivum
 aestuans
 aestuari
 aestuarii
+aestuarium
 aethalea
 aethiobola
 aethioboliza
 aethiopica
 aethiopicum
 aethiopicus
 aethiopicus x nlemfuensis
@@ -1343,37 +1371,40 @@
 affin. speciosa
 affin. trachycarpa
 affine
 affinis
 affinis x jucunda
 affinis x preissiana
 affirmata
+affixa
 affixus
 afra
 africana
+africana lutea
 africanoides
 africanum
 africanus
 afrorevoluta
 afrostricta
 afrum
 afzelii
 agallocha
+agapanthi
 agapetoides
 agardhiana
 agardhianum
 agardhii
 agaricicola
 agariciformis
 agaricoides
 agathidis
 agathosmoides
 agatiflora
 agatii
-agatii x microphylla
+agavacearum
 agelaeina
 agelaeoides
 agelaeotera
 aggeratum
 aggericola
 agglomerata
 agglutinospora
@@ -1407,17 +1438,20 @@
 agyrophylla
 ahlneriana
 ahtianum
 ailae
 ailantifolia
 aillya
 ainoae
+aiodonta
 aipolia
+airliensis
 airoides
 aithocheilum
+aitkeniae
 aitonis
 ajacis
 ajugacea
 ajugaceum
 ajugae
 ake-assii
 akrokomos
@@ -1446,14 +1480,15 @@
 alba x fragilis
 alba x gulngai
 alba x leichtlinii
 alba x matsudana x alba
 alba-compacta
 alba-odorata
 albata
+albella
 albellaria
 albellus
 albens
 albens x melanophloia
 albens x melliodora
 albens x microcarpa
 albert-smithii
@@ -1481,14 +1516,15 @@
 albidocapillaris
 albidocoeruleum
 albidoflava
 albidofusca
 albidoides
 albidoplumbea
 albidopunctata
+albidorosea
 albidosimulans
 albidula
 albidulum
 albidum
 albidus
 albifimbriata
 albiflora
@@ -1517,32 +1553,36 @@
 albocinereum
 alboconidia
 albocoronatum
 albofarinosa
 albofibrillosa
 alboflavescens
 alboflavicans
+albofloccosa
+albofoetidus
 albofuscus
 albogilvus
 alboglobospora
 albohirta
 alboihirta
 albolanata
 albolilacinum
 albolimbatum
 albolineata
 albomaculans
 albomagnum
 albomarginata
 albomarginatus
+albomontensis
 albomontis
 alboniger
 albonigra
 albonitens
 albonotata
+albopicri
 alboplumbea
 albopunctata
 albopurpurea
 alboranii
 alborimosa
 alborosella
 alborubens
@@ -1553,14 +1593,15 @@
 albosquamosus
 albostellatum
 albostraminea
 albostramineus
 albostriata
 albostriatus
 albostrigosa
+albostrigosum
 albostrigosus
 albotessellata
 albotexta
 albotextum
 albovaginatum
 albovaginatus
 alboverrucata
@@ -1630,23 +1671,25 @@
 alhagi
 alianuda
 alicae
 aliceae
 aliciae
 aliena
 alienata
+alienum
 aligera
 aligerum
 alilateralis
 alipes
 alismatis
 alismifolium
 alismoides
 alkalivirens
 alkekengi
+allaniae
 allanii
 allantoidea
 allantoides
 allantoideum
 allantoobliqua
 allantopus
 allantospora
@@ -1684,21 +1727,24 @@
 allomycis
 allophron
 alloplectus
 alloplectus x graveolens
 allorgei
 allosporoides
 allostraminea
+alloumbrina
+alloxyli
+allportiae
+almanense
 almbornii
 almum
 alneum
 alneus
 alni
 alnifolium
-alnus
 aloba
 alocophylla
 aloefolium
 aloides
 aloifolia
 alooides
 alopallonella
@@ -1718,14 +1764,15 @@
 alphitoniae
 alphitonioides
 alphitonioidos
 alphitonoides
 alphonsiana
 alpicola
 alpicolum
+alpicolus
 alpigena
 alpigenum
 alpina
 alpina (Beechworth)
 alpina (Black Range, west of the Grampians)
 alpina (Bright)
 alpina (Cardinia, Mt Dandenong Range)
@@ -1783,28 +1830,30 @@
 althaeifolia
 althaeina
 althaeoides
 althoferi
 althoferorum
 alticola
 alticolum
+altifrons
 altilamellosa
 altile
 altilis
 altimontana
 altior
 altisetum
 altisetus
 altissima
 altissimum
 altissimus
 altolimbatum
 alulata
 alumnus
 aluniticola
+aluta
 alutacea
 alutaceum
 alutaceus
 alutacia
 alutaria
 aluticolor
 alvearia
@@ -1815,15 +1864,14 @@
 alveolaris
 alveolarius
 alveolata
 alveolatum
 alveolatus
 alveolus
 alvesii
-alyconium
 alyssoides
 alyssum
 alyxia
 alyxiae
 alyxifolia
 alyxifolium
 alyxifolius
@@ -1856,19 +1904,18 @@
 amaurorachis
 amaurorhachis
 amaurus
 amazonensis
 amazonica
 amazonum
 ambasiensis
+amberina
 ambiens
 ambiens x rotundifolium
 ambigua
-ambigua x capitata
-ambigua x seminuda
 ambiguua
 ambiguum
 ambiguus
 ambiguus x queenslandicus
 ambita
 ambleia
 ambligona
@@ -1897,14 +1944,15 @@
 amblyphylla
 amblystegioides
 amblystoides
 amboinense
 amboinensis
 amboinicum
 amboinicus
+ambrosiae
 ambrosioides
 ambrozii
 ambusta
 ambustum
 ameliae
 amelum
 amentacea
@@ -1951,15 +1999,14 @@
 amorphum
 amorphus
 ampelina
 ampeloprasum
 ampelos
 ampeloscopia
 ampereae
-amphibela
 amphibia
 amphibiorum
 amphibium
 amphibius
 amphibola
 amphibolis
 amphibolum
@@ -2103,14 +2150,15 @@
 anceps (winged variant)
 anchusaefolia
 anchusaefolium
 anchusifolia
 anchusifolium
 ancistrocarpa
 ancistrocarpa x citrinoviridis
+ancistrocarpa x trachycarpa
 ancistrocarpum
 ancistroclada
 ancistrophylla
 ancistrophyllum
 ancistrophyllus
 ancistrosporelloides
 ancistrotricha
@@ -2148,14 +2196,15 @@
 androgynus
 andromedaeflora
 andromedaefolia
 andromediflora
 andromedifolia
 andromedifolia Small-leaved form
 andromedifolia Type form
+andropogonearum
 andropogonis
 andropogonis-aciculati
 andropogonis-micranthi
 androsacea
 androsaceum
 androsaceus
 androsaemifolia
@@ -2164,14 +2213,15 @@
 androsemaefolia
 androstemma
 aneba
 anebus
 aneirina
 aneirinus
 aneityense
+anemonefollia
 anemones
 anemoneus
 anemoniflorus
 anemonifolia
 anemonifolius
 anemonoides
 anemophilus
@@ -2203,27 +2253,29 @@
 anglicus
 anglocandicans
 angolense
 angolensis
 angophorae
 angophoroides
 angraeciflora
+angsiewkeeae
 anguillariae
 anguina
 anguinea
 anguinella
 anguineus
 anguivi
 angularis
 angulata
 angulata 'Golden-flowered form'
 angulata - eardleyae
 angulata - pseudocampanulata
 angulatum
 angulatus
+anguliobliqua
 angulispora
 angulisporus
 angulistipula
 angulosa
 angulosum
 anguria
 angusii
@@ -2260,14 +2312,17 @@
 angustisporum
 angustisporus
 angustissima
 angustissima x tholiformis
 angustissimum
 angustissimus
 angustissimus x erubescens
+angustiterminale
+angustoaristata
+angustoobliqua
 angustum
 angustus
 anidiophyllum
 anigozanthi
 anil
 animale
 animalis
@@ -2295,16 +2350,19 @@
 anisopogon
 anisostoma
 anisostomum
 anisotoma
 anisum
 anjutii
 annae
+annamaniae
+annamariae
 annamense
 annelida
+annellsiae
 annelsii
 annettae
 annonae
 annosa
 annosicaulis
 annosocaule
 annosocaulis
@@ -2328,15 +2386,14 @@
 annuus
 anodon
 anodonta
 anodontus
 anoectocolea
 anogrammoides
 anomaea
-anomaeus
 anomala
 anomalous
 anomalum
 anomalus
 anomoplexis
 anonyma
 anota
@@ -2354,15 +2411,14 @@
 antarcticus
 antarticum
 antecedens
 antecellens
 antediluviana
 antediluvianum
 antefossa
-antenaria
 antennaria
 antennarium
 antennarius
 antennaroidea
 antennata
 antennatum
 antennatus
@@ -2400,14 +2456,15 @@
 anthophila
 anthophilum
 anthostomelloidea
 anthoxanthi
 anthoxanthoides
 anthracina
 anthracinum
+anthracoideispora
 anthracoideisporum
 anthracophila
 anthracophilum
 anthracophilus
 anthropophagarum
 anthropophagorum
 anthyllidis
@@ -2432,14 +2489,15 @@
 antiquorum
 antiquum
 antirrhini
 antirrhiniflora
 antiscorbutica
 antleriformis
 antoinii
+antonovae
 antonschmidii
 antrea
 antrorsa
 antrorsum
 anulata
 anziana
 aokii
@@ -2520,14 +2578,15 @@
 apii-graveolentis
 apiicola
 apiifolium
 apilongissima
 apiospora
 apis
 apitectum
+aplacophylla
 aplectra
 apoa
 apocalypticum
 apocarpa
 apocarpum
 apocynifolia
 apoda
@@ -2597,16 +2656,16 @@
 apterantha
 apteropteridis
 aptogonum
 aptrootii
 apula
 apulum
 apus
+aquae-cooljarloo
 aquarii
-aquarum
 aquatica
 aquatica x arundinacea
 aquaticum
 aquaticus
 aquatile
 aquatilis
 aquea
@@ -2645,14 +2704,15 @@
 arachnanthe
 arachne
 arachnifera
 arachniformis
 arachnoidea
 arachnoides
 arachnoideum
+arachnoideus
 arachnopus
 araeophyllum
 arafurensis
 arafurica
 arafuricum
 aragoana
 araiorhachis
@@ -2691,29 +2751,30 @@
 arcana
 arcana x saligna
 arceuthos
 archaeoides
 archangelii
 archboldiana
 archboldianum
+archerae
 archeri
 archerian
 archeriana
 archerianum
 archibaldii
 archimedes
 archimedis
+archontophoenicicola
 archontophoenicis
 archytas
 arckaringensis
 arcohastata
 arcta
 arctica
 arcticum
-arcticus
 arctiflora
 arctii
 arctiscon
 arctotides
 arctotidis
 arctotis
 arcturi
@@ -2744,14 +2805,15 @@
 areira
 arenacea
 arenacolens
 arenaria
 arenariae
 arenariaeformis
 arenariobulbosa
+arenarioides
 arenarium
 arenarius
 arenastrum
 arenicola
 arenicolens
 arenicolor
 arenicolum
@@ -2760,14 +2822,15 @@
 arenitensis
 arenivaga
 arenosa
 arenosus
 arens
 arentii
 areolata
+areolatoimbricatum
 areolatoimbricatus
 areolatum
 areolatus
 areolifolia
 areomontana
 areschougii
 arfakense
@@ -2781,14 +2844,15 @@
 argentea
 argenteum
 argenteus
 argentia
 argentifolium
 argentifolius
 argentina
+argentinense
 argentinensis
 argentinus
 argillacea
 argillaceum
 argillaceus
 argillicola
 argocalla
@@ -2860,29 +2924,34 @@
 aristata
 aristata (Adelaide Hills)
 aristata x ixioides
 aristatula
 aristatulum
 aristatum
 aristatus
+aristibracteata
+aristidae
 aristidea
 aristidicola
 aristiferum
 aristifolius
 aristigera
 aristiglumis
+aristisepala
 aristispicula
 aristispiculum
 aristolochiicola
 aristotelea
+aristotelia
 aristulata
 aristulatum
 aristulosum
 aristum
 arizonica
+armarii
 armata
 armatisporus
 armatoides
 armatum
 armatus
 armbrustae
 armbrustiae
@@ -2901,31 +2970,30 @@
 armillare
 armillaris
 armillata
 armillata x orthostemon
 armillata x tenera
 armillatum
 armillatus
-armiti
 armitiana
 armitii
-armitti
 armittii
 armoraciae
 armorica
 armoricana
 armoricanus
 armourense
 armstrongiana
 armstrongii
 arnhemensis
 arnhemiaca
 arnhemica
 arnhemicum
 arnhemicus
+arnoldi
 arnoldii
 arnottiana
 arogoana
 aroha
 aromaphloia
 aromatica
 aromaticum
@@ -2977,16 +3045,18 @@
 arvense
 arvensis
 arvernensis
 arxii
 asahii
 asbolodes
 ascendens
+ascheae
 aschersoniana
 aschersonii
+asclepiadearum
 asclepiadeum
 ascoboloides
 ascocystophora
 ascoscypha
 ascripta
 asekii
 aselliformis
@@ -2995,15 +3065,17 @@
 asepalum
 aseptatospora
 aseroeformis
 asetosa
 ashbyae
 ashbyi
 ashtonii
+ashworthiae
 asiana
+asianum
 asiatica
 asiaticum
 asiaticus
 asinantum
 askania
 askenasyi
 aspalathodes
@@ -3088,15 +3160,14 @@
 asteliifolia
 asterella
 asterias
 asterichroma
 asteridiellae
 asterinarum
 asterinearum
-asteriodea
 asteriphila
 asteris
 asteriscophora
 asteriscophorum
 asteriscosa
 asteriscus
 asteriskos
@@ -3137,21 +3208,24 @@
 astrolasius
 astroloba
 astrolomioides
 astrolomoides
 astrophylla
 astropletha
 astrotricha
+astrotrichus
+astrovinosa
 asybosca
 asymmetrica
 asymmetricum
 asymmetriphyllum
 atacta
 atactica
 atala
+atalayense
 atamasco
 ataxiphylla
 ataxiphyllum
 atepalus
 ater
 aterrima
 aterrimum
@@ -3172,14 +3246,15 @@
 atkinsiana
 atkinsianum
 atkinsonae
 atkinsoni
 atkinsoniae
 atkinsoniana
 atkinsonii
+atkinsoniorum
 atlantica
 atlanticus
 atocioides
 atomaria
 atomatoides
 atomatum
 atomus
@@ -3213,14 +3288,15 @@
 atriplicifolia
 atriplicifolium
 atriplicifolius
 atriplicina
 atriplicinum
 atriplicis
 atrisola
+atrisquamosa
 atrivirida
 atro-virens
 atroalba
 atroalbus
 atroavellanea
 atrobarbatica
 atrobrunnea
@@ -3240,15 +3316,14 @@
 atrococcinea
 atrocoerulea
 atrocoeruleus
 atrocyanea
 atrocyaneus
 atroeffusum
 atroflavella
-atrofumosa
 atrofusca
 atrofuscum
 atrohispidus
 atrolilacina
 atrolucida
 atrolucidus
 atrolutea
@@ -3267,14 +3342,15 @@
 atropurpurea
 atropurpureum
 atropurpureus
 atroroseum
 atrorubens
 atrorubicans
 atrorubra
+atrorubripes
 atrorufa
 atrorufus
 atrosanguinea
 atrosanguineum
 atrosanguineus
 atrosphaerica
 atrosphaericum
@@ -3305,14 +3381,16 @@
 attenuifolia
 attescandens
 attingens
 attingens x infundibularis
 attingens x longicauda
 attleana
 atypa
+atypicola
+atypicolum
 atypus
 auberianum
 auberianus
 auberti
 aubertianum
 aubertii
 auburnense
@@ -3360,27 +3438,30 @@
 auraliae
 aurantia
 aurantiaca
 aurantiacafolia
 aurantiacopurpureum
 aurantiacum
 aurantiacus
+auranticarpum
 auranticus
 aurantifolia
 aurantii
 aurantiicola
 aurantiifolia
 aurantiocampanula
 aurantiocinnabarina
 aurantioides
 aurantioides vel. aff.
 aurantiolabes
 aurantiopallens
+aurantioruber
 aurantiospora
 aurantipes
+aurantirosea
 aurantiseta
 aurantium
 aurantius
 aurariae
 aurata
 auratiflora
 auratiflorum
@@ -3393,23 +3474,25 @@
 aureliae
 aurella
 aureo-nitens
 aureocinctum
 aureocorona
 aureocrinita
 aureocrinitum
+aureoelephanti
 aureofulva
 aureofulvum
 aureofulvus
 aureola
 aureolatum
 aureolum
 aureolus
 aureonitens
 aureopilea
+aureorimosa
 aureotomentosus
 aureoviride
 aurescens
 aureum
 aureus
 auricampa
 auricolor
@@ -3438,34 +3521,36 @@
 auriformis
 aurigera
 aurigerum
 auriorbis
 auripila
 auripilum
 aurita
+auritelloides
 auritum
 aurivella
 aurivellus
 auronitens
 aurora
 aurulenta
 ausfeldi
 ausfeldii
 aussiorum
 austaliensis
 austera
 austinensis
+australafricana
 australasia
 australasiaca
-australasiacum
 australasiae
 australasiaticum
 australasica
 australasicum
 australasicus
+australasiensis
 australasium
 australasius
 australe
 australe x nelsonii
 australe x sturtianum
 australense
 australensis
@@ -3476,27 +3561,29 @@
 australianus
 australiasicum
 australica
 australicum
 australiense
 australiensis
 australiensis - granitica
+australina
 australinum
 australis
 australis - caudata
 australis Form 2
 australis x brachypetala
 australis x clementii
 australis x exarrhena
 australis x exarrhenax
 australis x graveolens
 australis x linearis
 australis x longipetala
 australisense
 australopithecurus
+australpacifica
 austriaca
 austriacum
 austrigena
 austrigenus
 austrina
 austrina - olivina
 austrinum
@@ -3511,20 +3598,20 @@
 austroalpinum
 austroalpinus
 austroamericana
 austroamericanum
 austroamphibium
 austroapocarpa
 austroargenteum
+austroasianum
 austroaustraliense
 austrobrevipes
 austrobulbosa
 austrocaesia
 austrocaledonica
-austrocaledonicum
 austrocaledonicus
 austrocanescens
 austrocapense
 austrocarnea
 austrocausticus
 austrocetrata
 austrocetratum
@@ -3535,77 +3622,88 @@
 austrocongestum
 austroconiops
 austroconstrictans
 austrocrispa
 austrocrispum
 austrocyanescens
 austrocyanites
+austrocylindrica
+austrodensa
 austroedulis
 austroevernius
 austrofalcata
 austrofelleus
 austrofibrillosa
+austrofibrillosipes
 austrofilopes
 austroflaccida
 austrofragilis
 austrofunalis
 austrogeaster
-austrogeorgica
 austrogranulatus
 austrohemisphaerica
+austrohemisphaericum
 austrohygrophilum
 austrointumescens
 austrokoningii
 austroleprosa
 austrolitoralis
 austrolittoralis
 austrolutea
 austromaculata
+austrominimum
 austromontana
 austromontanum
 austromuralis
 austromuticum
 austronesophilus
+austronitens
 austronutans
+austroobtusispora
+austroocculta
 austropacifica
 austropacificum
 austropallescens
 austropalustre
 austropapillatus
 austropatens
 austrophalloides
 austrophlyctidospora
 austropiceum
 austropicreus
 austropiperatus
+austropleiomicrosoma
 austropratensis
 austroprunicolor
 austroprunulus
 austropulchella
 austropullata
 austropunctata
 austropusillum
 austropygmaeum
 austropyrenaica
 austroqueenslandica
 austroqueenslandicum
+austroregalis
 austrorhodocalyx
 austrororida
 austrororidus
 austroroseum
 austrorubi
 austroruralis
 austrosabulosum
 austrosaginus
 austrosapineus
+austrosarcitulum
 austroscoparium
 austroserpens
 austrosinense
 austrosinensis
 austrosorediosa
+austrosquarrosa
 austrostellaris
 austrostipae
 austrostraminea
 austrosubulatum
 austrosubulatus
 austrosudeticum
 austrosulcata
@@ -3617,34 +3715,41 @@
 austrounguiculata
 austrounguiculatula
 austrovaginatus
 austroveneta
 austrovenetus
 austrovinaceus
 austroviolaceus
+austrovirens
 austroviridis
 autmnale
 autochthonus
 autoicus
 autumnale
 autumnalis
 avecta
 avellana
+avellanea
+avellaneifolia
 avellaneum
 avellanus
 avenacea
 avenaceum
 avenaceus
 avenae
+avenoides
 aversa
 aversum
+aviaristata
 avicennae
 avicenniae
+aviceps
 avicula
 aviculare
+aviflagellata
 avium
 avonensis
 awabuki
 awestoniana
 awestonianum
 awestonii
 awhitu
@@ -3661,15 +3766,17 @@
 axillare
 axillaris
 axillibarba
 axilliflora
 axilliflorum
 axilliflorus
 axilliforum
+axillosa
 axonopodi
+axonopodicola
 ayensuensis
 ayersiana
 ayersianum
 ayersii
 ayresii
 aywerte
 azadirachtae
@@ -3719,14 +3826,15 @@
 bacillaris
 bacillata
 bacillifera
 bacillum
 backhouseana
 backhousei
 backhousi
+backhousiae
 backhousiana
 backhousii
 bactrodesmioides
 baculifera
 baculoides
 baculum
 badensis
@@ -3748,15 +3856,14 @@
 badyinbarus
 baeckeacea
 baeckeaceus
 baeckeoides
 baenzigeri
 baeomyceoides
 baeomycesica
-baeosporus
 baeticum
 baeticus
 baeuerleni
 baeuerlenii
 baeuerlenii (Armstrong 5087)
 bagleyi
 bagliettoana
@@ -3791,107 +3898,119 @@
 bakersana
 bakersiana
 balanites
 balanoides
 balanopelex
 balanophora
 balansae
+balansanum
 balantii
 balara
+balbakiae
 balbisii
 balcooa
 baldensis
 baldjikiana
 baldockii
 baldwinii
 balearica
 balearicum
 balekensis
+balenae
 balfouriana
 balfourii
 balfourniana
 balia
 baliboongarnang
 balica
 baliense
 balladoniense
 balladoniensis
 ballajupensis
 ballantinum
+ballerina
 balli
 balliae
 ballii
 ballinaensis
 ballinense
 ballinensis
 ballineus
 ballingalliae
 ballingalliana
-ballingallii
 ballioides
 ballonnesis
 balloui
 balls-headleyi
 ballythunnensis
 baloghioides
 balonense
 balonensis
 balonnensis
 baloskionis
+balpinea
 balpineum
 balsamea
 balsameum
 balsameus
 balsamica
 balsamicum
 balsamifera
 balsamina
 balsamona
 balsiformis
 baltica
 balticum
+bamagaensis
 bamagana
 bamagense
 bamagensis
 bambra
 bambrus
 bambusae
 bambusicola
 bambusifolia
 bambusifolium
 bambusina
 bambusoides
+bamuru
 banalo
+banati
 bancksii
 bancrofti
 bancroftiana
 bancroftii
 bancroftii x robusta
 bancroftiorum
 bancroftiorum x falciformis
 bancroftiorum x macradenia
 banfieldii
 bangmeiana
 banguioensis
+banksi
 banksiae
 banksiae-integrifoliae
+banksiae-repentis
 banksiaefolia
 banksiana
 banksianum
+banksianus
 banksii
-banksii x platyphylla
 banksiicola
 banksiifolia
+banksiigena
 bantaengensis
 bantamensis
 bantiana
 bantianum
 banyabba
+banzhao
 baouleensis
 baoulensis
+baptisti
 baptistii
 baptistii x nutans
 baracchiana
 baracchianum
 barakulense
 barakulensis
 barattense
@@ -3905,14 +4024,15 @@
 barbareaefolium
 barbarella
 barbarorum
 barbarossa
 barbarossae
 barbarum
 barbata
+barbatae
 barbatala
 barbatellum
 barbatica
 barbatum
 barbatus
 barbellata
 barbellatum
@@ -3941,30 +4061,33 @@
 barklyanus
 barklyensis
 barklyensis x pruinosa
 barklyi
 barleei
 barlowii
 barmedmanensis
+barnardiae
 barnardianum
 barnardii
 barnettii
 barneyense
 barodensis
 baronii
 barragensis
 barrelieri
 barrenfieldii
 barrettiae
 barrettiorum
 barrettorum
 barringtonense
 barringtonensis
+barringtoniae
 barronense
 barronfieldii
+barrowensis
 barryanum
 barssii
 bartayresiana
 bartayresii
 barteriana
 bartheriana
 barthlottii
@@ -4061,26 +4184,26 @@
 baumannii
 baumei
 bavaricum
 bawbawensis
 bawbawiensis
 baxteri
 baxteriana
-bayleyi
 beadleana
 beaglensis
 bealeyensis
 bealiana
 beaniana
 beardiana
 beardii
 beasleyana
 beasleyi
 beatonii
 beatricae
+beatricis
 beatrix
 beauchampiana
 beaudettei
 beaufortianum
 beaufortioides
 beaufortoides
 beaugleholei
@@ -4112,34 +4235,38 @@
 becklerii
 beckmanniae
 beckxiana
 beddomeana
 bedfordi
 bedfordii
 bedggoodiana
+beerburrumensis
 beeronensis
 beeveriae
 begaensis
 beharensis
 behen
+behri
 behriana
 behrianum
 behrianus
 behrii
 behrina
 beigehimenium
 beigelii
+beilharziae
 belangeri
 belangeriana
 belenophorus
 belense
 belgraveana
 bella
 bella x confertiflora
 belladonna
+bellae-mahoneyi
 bellairsiana
 bellairsiorum
 bellardi
 bellardii
 bellatula
 bellemerei
 bellenden-keriense
@@ -4212,14 +4339,15 @@
 bentonii
 benwellii
 beomiforme
 berardiana
 berarngutta
 berberifolia
 berberifolium
+berberifolius
 berberina
 bergeriana
 berggrenii
 berghii
 bergiana
 bergianus
 bergii
@@ -4244,14 +4372,15 @@
 bernicis
 bernieana
 berringbinensis
 berryana
 berryi
 berteri
 berteriana
+berteroae
 berteroana
 berteroanum
 berteroanus
 berteroi
 berteronianus
 berthae
 bertieri
@@ -4263,14 +4392,15 @@
 betaceum
 betae
 betcheanum
 betchei
 beticola
 betle
 betonica
+betonicaefolia
 betonicifolia
 bettyae
 bettzichiana
 betulae
 betulina
 betulinus
 beveridgei
@@ -4289,15 +4419,15 @@
 biangulata
 biangulatus
 biannulata
 biarmatum
 biarticulatum
 biasolettiana
 biasolettianum
-biatorina
+biatriispora
 biatriisporus
 biaurita
 biauritum
 bibas
 bibenda
 bibrachiatum
 bibracteata
@@ -4323,17 +4453,17 @@
 biciliatus
 bicincta
 bicinctulum
 bicinctum
 bicinctus
 bickertonensis
 bickfordiana
+bickfordianus
 bickii
 biclavatum
-biclavatum sensu A.M. Scott & Prescott (1958)
 biclavatus
 biclipea
 bicocca
 bicolor
 bicolor x undulatum
 bicolorans
 bicolorata
@@ -4458,14 +4588,15 @@
 bilocularis
 bilocularis x silvestris
 biloculata
 biloculatum
 biloelensis
 bilorbang
 bilunaris
+bilybara
 bimaculata
 bimarginatum
 bimberiensis
 bimorsum
 bimucronatum
 bimum
 binale
@@ -4530,14 +4661,15 @@
 bireflexus
 bireme
 biremis
 biretiforme
 biretum
 birgei
 birmanicum
+birmannicum
 birnbaumii
 birostris
 birrea
 birriliburu
 biruncinata
 bisaetosum
 bischlerae
@@ -4554,14 +4686,15 @@
 biserratus
 biserrula
 biserrulata
 biseta
 bisetulus
 bisetus
 bishii
+bishopiae
 bishopii
 bisimpressa
 bismolliuscula
 bispapillata
 bisphaericum
 bispinosa
 bispinosus
@@ -4569,14 +4702,15 @@
 bispora
 bisporalis
 bisporiger
 bisporigera
 bisporum
 bisporus
 bissellii
+bissilli
 bissillii
 bistratosus
 bistyla
 bisulca
 bisulcata
 bisulcatum
 bisumbellata
@@ -4596,25 +4730,28 @@
 bivaginata
 bivalve
 bivalvis
 bivenosa
 bivenosum
 bivestita
 bivillosa
+bizantiorum
 biziana
 bizzozeriana
 bjerkeana
 blackalli
 blackallii
 blackburnia
+blackburniae
 blackburniana
 blackdownensis
 blackei
 blacketii
 blackettii
+blacki
 blackiana
 blackianum
 blackii
 blackmani
 blackmanii
 blackmanni
 blackwelliana
@@ -4682,30 +4819,31 @@
 blepharophylla
 blepharosperma
 blepharospermus
 blepharospora
 bliklika
 blitum
 blochii
+blodgettiae
 blodgettii
 blomei
 blomianum
 blossfeldiana
 bloudowskyana
 bloxamii
 bloxsomei
 bloxsomei x citriodora
 bloxsomei x maculata
-bloxsomei x watsoniana
 blumeana
 blumeanum
 blumei
 blumii
 blyttii
 boanensis
+boardinghousense
 boardinghousensis
 bocconei
 bocconi
 bocconii
 bodalla
 boeckii
 boehmii
@@ -4725,23 +4863,26 @@
 bohmii orth. var.
 bohneri
 boidinii
 boivinii
 bokorensis
 bokotensis
 bolanderi
+bolayi
 bolbochaete
 boldtiana
 bolensis
 boletoides
 bolgartense
 bolida
 boliviana
 boliviensis
 boliviensis (Williams 89556)
+bolleana
+bolleanum
 bollei
 bolleyi
 boltonii
 bolusii
 bolyaiana
 bomba
 bombacifolia
@@ -4766,22 +4907,24 @@
 bonianum
 boninense
 boninensis
 boninsimae
 bonjeanii
 bonnemaisoniae
 bonnemaisonii
+bonneyae
 bonneyana
 bonneyanum
 bonneyi
 bonplandiae
 bonplandii
 bontei
 bonus-henricus
 bonwickii
+boodjera
 boodleoides
 boolaronga
 boolbunda
 booloola
 boomerangisporum
 boomerangum
 boomerangus
@@ -4799,15 +4942,15 @@
 boranupensis
 borbonica
 borbonicum
 bordiana
 borea
 boreale
 borealis
-borerri
+boreoaustralis
 borgeanum
 borgei
 borgenii
 borhidii
 boridiana
 borisianum
 borneense
@@ -4816,15 +4959,14 @@
 bornhardtiensis
 boroniaceum
 boroniacus
 boroniae
 boroniaefolia
 boronifolia
 boroniifolia
-boroniifolia x cuneata
 borowitzkae
 borreri
 borrichii
 borunastylis
 boryana
 boryanum
 boryanum sensu Entwisle 1989b
@@ -4842,14 +4984,15 @@
 bostockii
 bostrychiae
 boswellii
 botanense
 botanica
 botanicum
 botanocolpium
+bothae
 bothriochloae
 botriosa
 botrycephala
 botrydion
 botryocarpa
 botryocarpum
 botryoclada
@@ -4868,20 +5011,21 @@
 botuliforme
 bouchardatiae
 boucheana
 boucheanus
 boudieri
 boudouresquei
 bougainvilleana
-bougainvillense
 bougheri
+boughtoniae
 boulayi
 bouleyi
 boulindaensis
 bounites
+bounty
 bourellyanum
 bourgeanica
 bourjotiana
 bourlieri
 bourrellyana
 bourrellyi
 bouteillei
@@ -4938,38 +5082,40 @@
 brachyathera
 brachybotrya
 brachybotrya (Wirrabarra variant)
 brachybotrys
 brachybotryum
 brachycalyx
 brachycarpa
-brachycarpa x pedicellaris
 brachycarpa x plena
 brachycarpa x setosa
+brachycarpae
 brachycarpum
 brachycaulis
 brachycaulon
 brachycentra
 brachycephala
 brachycephalus
 brachyceras
 brachychaeta
 brachychaetum
+brachychitonis
 brachychlaenus
 brachyclada
 brachyclados
 brachycladulum
 brachycladum
 brachycladus
 brachycomes
 brachycomoides
 brachycorys
 brachycystidea
 brachydontia
 brachydontium
+brachygibbosum
 brachyglossa
 brachyglossus
 brachyglottis
 brachygona
 brachygonia
 brachygyne
 brachylaena
@@ -5047,14 +5193,15 @@
 bracteatum
 bracteatus
 bracteolaris
 bracteolata
 bracteolata x obovata
 bracteolatum
 bracteolatus
+bracteolosa
 bracteolosum
 bracteolosus
 bracteosa
 bracteosum
 bractescens
 bradburyae
 braddonii
@@ -5067,14 +5214,15 @@
 brandegeei
 brandenii
 branderhorstii
 brandiana
 brandtiae
 brandtii
 branwhitei
+branwhiteorum
 brasiliana
 brasilianum
 brasiliense
 brasiliensis
 brassiana
 brassiana x pellita
 brassianum
@@ -5094,15 +5242,14 @@
 brebissoniana
 brebissonii
 brebneri
 bredboensis
 brefeldianum
 brefeldii
 brekkaensis
-bremenensis
 bremensis
 bremerense
 brendannarum
 brennanii
 brentii
 bresadolae
 bresadoleanum
@@ -5111,14 +5258,15 @@
 breutelianum
 breutelii
 breve
 breviaculeata
 breviacuminata
 brevialata
 brevianthera
+breviappendiculata
 breviaristata
 breviarticulata
 breviarticulatum
 breviarticulatus
 brevibracteata
 brevibracteatus
 brevibracteosus
@@ -5127,14 +5275,15 @@
 brevicalycina
 brevicarinatum
 brevicauda
 brevicaudatus
 brevicaudum
 brevicaule
 brevicaulis
+brevicentra
 brevicentrum
 brevichila
 brevichilum
 brevicilia
 brevicilium
 brevicolle
 brevicollis
@@ -5158,14 +5307,15 @@
 brevifolium
 brevifolius
 breviglume
 breviglumis
 brevilabium
 brevilabre
 brevilabris
+brevilata
 brevilatum
 brevilimbatum
 brevilimbum
 brevilingueus
 breviloba
 brevilobata
 brevinerve
@@ -5174,15 +5324,14 @@
 brevipaniculata
 brevipaniculatum
 brevipapposus
 brevipedata
 brevipedatum
 brevipedicellatum
 brevipedunculata
-brevipedunculata x revoluta
 brevipedunculatus
 brevipes
 brevipes x microcarpum
 breviphora
 brevipila
 brevipilosa
 brevipinna
@@ -5190,16 +5339,16 @@
 breviracemosum
 breviradiata
 breviramosa
 breviramulosum
 brevirhachis
 brevirhiza
 brevirostra
-brevirostre
 brevirostris
+brevirostrum
 brevis
 breviscapa
 breviscapea
 breviscapis
 breviscapum
 brevisegmenta
 brevisepala
@@ -5242,17 +5391,19 @@
 briagolensis
 bridelii
 bridgesiana
 bridgesiana x viminalis
 brigalow
 brigalowensis
 briggsiae
+briggsiana
 brightiae
 brightwellii
 brigitteae
+brimsiorum
 brindabella
 brinkmannii
 brinsleyi
 brisbaneense
 brisbanense
 brisbanensis
 brisbanica
@@ -5317,14 +5468,15 @@
 broteri
 brotheri
 brotherusii
 broviniensis
 browneana
 browneanum
 brownei
+browni
 browniae
 browniana
 brownianum
 brownianus
 brownii
 brownii - populnea
 brownii x crebra
@@ -5342,25 +5494,28 @@
 bruhlii
 bruhnei
 brumale
 brumalis
 brumalis (incurved phyllode variant)
 brumalis (light land variant)
 brumalis (oblanceolate phyllode variant)
+brumptoniae
 bruneiensis
 brunellodes
 brunelloides
 bruniades
 bruniella
 brunii
 brunioides
+brunius
 brunkii
 brunnea
 brunneibulbosa
 brunneidens
+brunneidisca
 brunneiphylla
 brunneipurpureum
 brunneispora
 brunneistriatula
 brunneoadhaerens
 brunneoalbescens
 brunneoalbus
@@ -5368,19 +5523,21 @@
 brunneoatrum
 brunneocarpa
 brunneoceracea
 brunneocroceum
 brunneola
 brunneoleuca
 brunneoleucus
+brunneolorobustus
 brunneolum
 brunneolus
 brunneonigra
 brunneopictus
 brunneosorediata
+brunneospora
 brunneotingens
 brunnescens
 brunneum
 brunneus
 brunnthaleri
 brunonia
 brunoniae
@@ -5439,14 +5596,15 @@
 bularmialensis
 bulbicola
 bulbifera
 bulbiferum
 bulbigena
 bulbillifera
 bulbillosum
+bulbinella
 bulbinicola
 bulbipes
 bulbocodium
 bulbopilum
 bulborum
 bulbosa
 bulbosostolonifer
@@ -5479,14 +5637,15 @@
 bulweri
 bulwerii
 bunburyana
 bunburyanum
 bunburyense
 bunburyensis
 buncei
+bundaleer
 bundarus
 bundeica
 bundera
 bundeyana
 bundeyensis
 bungadinnia
 bungalbin
@@ -5516,15 +5675,15 @@
 burbidgeae
 burbidgeana
 burbidgeanum
 burbidgei
 burburiana
 burburianum
 burchardiae
-burchardtii
+burchardii
 burchellianum
 burchellii
 burckiana
 burdekense
 burdekensis
 burdettiana
 burdettii
@@ -5534,23 +5693,25 @@
 burgessiorum
 burgmaniana
 burianum
 burkei
 burkensis
 burkilii
 burkillii
+burkitti
 burkittii
 burleighensis
 burmanni
 burmanniana
 burmannii
 burmeisteri
 burmense
 burmensis
 burnettensis
+burnetti
 burnettii
 burneyensis
 burracoppinensis
 burraensis
 burragorang
 burrana
 burrowa
@@ -5578,14 +5739,15 @@
 busselliana
 bussellianus
 butcherense
 butcherensis
 butcheriana
 butleri
 butleriae
+butterlyi
 butyracea
 butyraceus
 butyrosum
 buubugujin
 buxbaumii
 buxeum
 buxifolia
@@ -5598,15 +5760,14 @@
 bynoeana
 bynoeanum
 bynoei
 byrneana
 byrnesiana
 byrnesii
 byronensis
-byrsaea
 byrsaeum
 byrsina
 byrsinum
 byrsinus
 byrsonimae
 byssacea
 byssicaule
@@ -5624,22 +5785,24 @@
 byssoideum
 byzantina
 byzantinus
 cabrerae
 cacalia
 cacao
 cacaobrunnea
+cacaocolor
 cacaotina
 cacatua
 cachemiriana
 cacomorpha
 cacomorphus
 cactacea
 cactifolia
 cactoides
+cacuminis
 cadamba
 cadelli
 cadellii
 cadens
 cadicola
 cadophora
 caduca
@@ -5661,20 +5824,22 @@
 caepicolorosa
 caereula
 caerulata
 caerulea
 caerulea x congesta
 caerulea, 'serrulata' variant
 caerulensis
+caeruleocaseus
 caeruleoeburneus
 caeruleoniger
 caeruleonigricans
 caerulescens
 caeruleum
 caeruleus
+caerulitunicatus
 caesaneura
 caesarea
 caesareum
 caesareus
 caesariata
 caesariatum
 caesia
@@ -5709,19 +5874,21 @@
 caespitulosus
 caespitulus
 cafferensis
 caffra
 caffrum
 cagiana
 cahillii
+cahuchucosa
 cahuchucosus
 cainito
 cairica
 cairicus
 cairnensis
+cairnsense
 cairnsensis
 cairnsiana
 cairnsiana x pulchra
 cairnsianum
 cairnsii
 cajan
 cajanensis
@@ -5859,14 +6026,15 @@
 callistemonea
 callistemonis
 callistos
 callistum
 callithamnium
 callitricha
 callitrichoides
+callitris
 callitrophila
 callitrophilis
 callitrophilum
 callium
 callochaetes
 callophylla
 callophyllis
@@ -5879,14 +6047,15 @@
 calobates
 caloblastoides
 caloblastum
 calobra
 calocarpa
 calocarpum
 calocarpus
+calocephala
 calocephalum
 calocera
 caloceroides
 calochlora
 calocoma
 calodendron
 calodictya
@@ -5898,14 +6067,15 @@
 calomelanos
 calomelas
 calopadiae
 calopedes
 calophleba
 calophylla
 calophylla x haematoxylon
+calophyllae
 calophyllantha
 calophyllum
 caloptera
 calopterum
 calopus
 calorhabdos
 calospora
@@ -5947,19 +6117,19 @@
 calyculus
 calyerup
 calyi
 calymega
 calymegum
 calymperaceum
 calymperidium
-calyptoglyphe
 calyptrata
 calyptratum
 calyptratus
 calyptrocalyx
+calyptroglyphe
 calyptroides
 calystegia
 calystegioides
 calyxhymenia
 camaldulensis
 camaldulensis x exserta
 camaldulensis x platyphylla
@@ -5971,16 +6141,16 @@
 cambageana x melanophloia
 cambageana x populnea
 cambagei
 cambagei x A
 cambagei x B
 cambagei x harpophylla
 cambagei x parvifolia
-cambagei x seminuda
 cambagei x tephrina
+cambagi
 cambessedesii
 cambewarrae
 cambewarrana
 cambewarranus
 cambodgensis
 cambogiense
 cambricum
@@ -6111,18 +6281,18 @@
 candolleanus
 candollei
 candolliana
 candollii
 canei
 canens
 canescens
-canescens x vokesensis
 cangaiense
 cangaiensis
 caniana
+canianus
 canicortex
 canina
 caninum
 caninus
 canis
 cannabina
 cannabinum
@@ -6159,14 +6329,15 @@
 capensis
 caperata
 caperatula
 caperatum
 caperatus
 capetribulense
 capetribulensis
+capilare
 capillacea
 capillaceum
 capillaceus
 capillare
 capillaripes
 capillaris
 capillata
@@ -6182,15 +6353,14 @@
 capillipes
 capillosa
 capillus-veneris
 capitanea
 capitaneum
 capitat
 capitata
-capitata x rupestris
 capitatoradiata
 capitatum
 capitatus
 capitellata
 capitellatum
 capitellatus
 capitis-york
@@ -6341,14 +6511,15 @@
 carlsoni
 carlsonii
 carlyleana
 carmeliana
 carmelii
 carminescens
 carminicolor
+carminorosea
 carnabyi
 carnarvonense
 carnarvonensis
 carnea
 carnea x racemosa
 carnegiei
 carnei
@@ -6415,26 +6586,29 @@
 carpodetoides
 carpoglossi
 carpoloma
 carpophila
 carpophilum
 carpophyllum
 carramarus
+carriae
 carrickiana
 carriemichelliae
 carriense
 carriensis
 carrii
 carroni
 carronii
 carronis
+carruthersi
 carruthersianus
 carruthersii
 carsei
 carsoni
+carsoniae
 carsonii
 carterae
 carteri
 carthagenense
 carthagenensis
 carthaginensis
 carthami
@@ -6445,15 +6619,17 @@
 cartilagineum
 cartilagineum x aspera
 cartilagineum x media
 cartilagineum x medium
 cartilagineus
 cartilaginipes
 cartilaginosa
+cartilaginum
 cartiliginea
+cartwrightiae
 carvi
 caryae
 carymbulosa
 caryophyllacea
 caryophyllaceus
 caryophyllea
 caryophylleae
@@ -6522,15 +6698,14 @@
 castorum
 castracanei
 castratus
 castrensis
 castrisinensis
 casuarina
 casuarinae
-casuarinarum
 casuarinoides
 casuarinophila
 catadromum
 catadromus
 catanduana
 catapastoides
 catapastum
@@ -6545,16 +6720,14 @@
 catarracticus
 catarractilis
 catasema
 catechu
 catenaeformis
 catenaria
 catenata
-catenatula
-catenatulum
 catenatum
 catenatus
 catenella
 catenemum
 cateniforme
 cateniformis
 catenula
@@ -6815,14 +6988,15 @@
 cervicula
 cervicularis
 cerviculatum
 cerviculatus
 cervifolia
 cervina
 cerviniicola
+cervinogilva
 cervinogilvum
 cervinogilvus
 cervinoleucus
 cervinoplumbeus
 cervinum
 cervinus
 cesatii
@@ -6834,23 +7008,20 @@
 cetrarioides
 cetrata
 cetratum
 cetratus
 ceuthocarpa
 ceylanica
 ceylanicum
-ceylanicus
 ceylonensis
 ceylonica
 ceylonicum
 cf. capilliforme
 cf. caprea
 cf. chelonoides
-cf. compacta
-cf. compressus
 cf. fonticola
 cf. francisiana
 cf. hispida
 cf. javanica
 cf. longicornua
 cf. luteola
 cf. micrococcus
@@ -6878,14 +7049,15 @@
 chailletii
 chalandei
 chalcedonia
 chalcedonica
 chalcedonium
 chalceum
 chalceus
+chalcoceps
 chalepensis
 chalkeri
 challengeroides
 challinorae
 chalmersii
 chalybaea
 chalybea
@@ -6920,26 +7092,29 @@
 chamelaea
 chamissoniana
 chamissonis
 chamomilla
 chamomillaefolia
 chamomillifolia
 championiae
+championii
 chandleri
+chantiae
 chapmaniana
 chapmanii
 chappilliae
 chara
 charadrodes
 charaeforme
 charantia
 charcotii
 charkowiensis
 charlesiana
 charlesii
+charlesworthii
 charlioi
 charnleyensis
 charoides
 charophyton
 charruana
 charsleyae
 chartaboma
@@ -6958,14 +7133,15 @@
 chatopodo
 chaunocoleus
 chaunorhiza
 chauviniana
 chauvinii
 cheeli
 cheelii
+cheesemaniae
 cheesemanii
 cheesemanniana
 cheesmanii
 cheilocarpa
 cheimonoceps
 cheiranthos
 cheiri
@@ -6984,14 +7160,15 @@
 cherticola
 chesapeakensis
 cheumatophila
 chevalieri
 chevallieri
 cheyneana
 chiapensis
+chiaroscuro
 chichesterensis
 chickrassa
 chiddarcoopingense
 chilense
 chilensis
 chillagoanum
 chillagoense
@@ -7056,24 +7233,22 @@
 chlorogrammus
 chlorolampra
 chlorolecanorica
 chloroleuca
 chloroloma
 chloromelas
 chloromelum
-chloromelus
 chlorophaea
 chlorophaeum
 chlorophana
 chlorophorum
 chlorophos
 chlorophylla
 chlorophylla x pruinosa
 chlorophyllosum
-chlorophyllus
 chloroplaca
 chloroptera
 chloropterum
 chlororhodon
 chlorosarca
 chlorosepala
 chlorospora
@@ -7177,14 +7352,15 @@
 chryseopsis x orientis
 chryseopsis x palustris
 chryseopsis x pardina
 chryseopsis x sulphurea
 chryseus
 chrysinocolla
 chrysites
+chrysitricis
 chrysoblephara
 chrysobotrya
 chrysobotrys
 chrysocalyx
 chrysocarpa
 chrysocarpum
 chrysocarpus
@@ -7208,14 +7384,15 @@
 chrysogaster
 chrysoglossa
 chrysoleuca
 chrysoleucus
 chrysomelinus
 chrysoneura
 chrysoneuron
+chrysoneurum
 chrysophaea
 chrysophaea Brisbane Ranges form
 chrysophaea Gippsland form
 chrysophaea Holey Plains form
 chrysophora
 chrysophthalma
 chrysophthalmus
@@ -7239,14 +7416,15 @@
 chrysotrycha
 chrystallina
 chrystenteron
 chrysus
 chthonocephala
 chthonocephalata
 chthonoplastes
+chuasooengiae
 chubutensis
 chudaei
 chudalupensis
 chudeaui
 chundra
 chunii
 chytraphora
@@ -7308,15 +7486,14 @@
 cineolifera
 cineramis
 cineraria
 cinerariifolium
 cinerarioides
 cinerascens
 cinerea
-cinerea x reichardtii
 cinereoannulosa
 cinereoargentea
 cinereoargenteum
 cinereoatra
 cinereocyaneus
 cinereofuscus
 cinereopallida
@@ -7327,15 +7504,14 @@
 cinereoumbrina
 cinereoviolacea
 cinereovirens
 cinerescens
 cinereum
 cinereus
 cinericolor
-cineroannulosa
 cingula
 cingulata
 cingulatus
 cingulum
 cinnabarina
 cinnabarinum
 cinnabarinus
@@ -7344,16 +7520,14 @@
 cinnamometorum
 cinnamomeum
 cinnamomeus
 cinnamomi
 cinnamomicola
 cinnamomifolia
 cinnamomipes
-cinnamonea
-cinnamoneobadius
 cinnamoneus
 cinnamopurpureum
 circaeoides
 circinale
 circinalis
 circinans
 circinata
@@ -7445,15 +7619,14 @@
 citrinoviridis
 citrinum
 citrinus
 citriobati
 citriocephala
 citriodora
 citriodora (Coveny 6590)
-citriodora x capillata
 citriodora x leichhardtii
 citriodora x peltata
 citriodora x torelliana
 citriodorum
 citroaurantius
 citrolens
 citronella
@@ -7529,19 +7702,19 @@
 clathroides
 clatritexta
 claucifolia
 claudei
 claudiana
 claudicans
 claudiensis
+claudopus
 clausa
 clausii
 clausum
 clauzadei
-clavaeforme
 clavaeformis
 clavarioides
 clavata
 clavatiramea
 clavatoflavus
 clavatoisidiata
 clavatum
@@ -7556,14 +7729,15 @@
 clavifer
 clavifera
 claviferum
 claviflora
 claviflorum
 clavifolia
 clavifolius
+claviforme
 claviformis
 claviger
 clavigera
 clavigerum
 clavinerve
 clavipetala
 claviseta
@@ -7594,14 +7768,15 @@
 cleistanthus
 cleistoblephara
 cleistocalyx
 cleistogama
 cleistogamoides
 cleistogamum
 clelandi
+clelandianum
 clelandii
 clelandiorum
 clellandii
 clematidea
 clematideum
 clematidis
 clematitis
@@ -7679,18 +7854,20 @@
 coalitus
 coangustata
 coangustatus
 coarctata
 coarctatum
 coarctatus
 coateana
+coatesiae
 coatesianum
 coatesii
 cobarensis
 cobbe
+cobbittiense
 coboni
 cobonii
 coccicola
 coccifera
 coccifera x amygdalina
 coccina
 coccinea
@@ -7698,14 +7875,15 @@
 coccineus
 coccinum
 coccocarpiae
 coccoidea
 coccoloba
 coccoloboides
 cocconeiformis
+coccophila
 coccophorum
 coccosporum
 coccotrypicola
 cocculifolia
 coccymelophyllus
 cochenill
 cochenillifer
@@ -7730,14 +7908,15 @@
 cochliocarpa
 cochlocarpa
 cochlocarpum
 cockaynei
 cockaynii
 cockertoniana
 cockertonii
+cocksii
 cocoes
 cocoina
 cocoparrana
 cocos
 cocosoides
 cocoës
 codiatile
@@ -7758,14 +7937,15 @@
 coelorachis
 coelosperma
 coelospermum
 coelothrix
 coenensis
 coenicola
 coenicolum
+coenophiala
 coenophialum
 coerulea
 coeruleo-punctata
 coeruleogracilis
 coeruleomagnum
 coeruleopunctatus
 coerulescens
@@ -7780,15 +7960,17 @@
 cognata
 cognatum
 cognatus
 cohaerans
 cohaerens
 cohglanii
 cohnii
+coicis
 colabense
+colbranii
 colchici
 coleae
 colei
 colemanae
 colemaniae
 colemaniarum
 colensoana
@@ -7803,29 +7985,32 @@
 collapsa
 collaris
 collata
 collatum
 collectorense
 collegialis
 colletioides
+colletotrichoides
 collicola
 collicolus
 colliculosa
 colliculosum
 colliei
 collierianum
 colligata
 collina
 collinoides
+collinsiae
 collinsiania
 collinsianum
 collinsii
 collinum
 collinus
 collodes
+collubrina
 collucera
 collum
 collybioides
 colmanae
 colobinoides
 colocasia
 colocasiae
@@ -7833,34 +8018,36 @@
 colocynthus
 coloensis
 colona
 coloneus
 colonorum
 colonum
 colonus
+colophon
 colophona
 colorans
 colorata
 coloratum
 coloratus
 colossea
 colossum
 colossus
-colpeteii
+colpeteorum
 colpopelta
 coltranei
 colubrina
 columbaria
 columbariensis
 columbarius
 columbetoides
 columbiana
 columbicolor
 columbina
 columbinum
+columboola
 columellaris
 columellaris inland race
 columellaris type race
 columellaris x verrucosa
 columellatum
 columellifera
 columnae
@@ -7892,14 +8079,15 @@
 comersonii
 comesperma
 cometae-vallis
 cometes
 comiramea
 comitae-vallis
 comitans
+commarosa
 commersonii
 commixta
 commixtum
 communalis
 commune
 communis
 commutabilis
@@ -8084,15 +8272,14 @@
 congrua
 congruens
 congruum
 congruus
 conica
 conica x crebra
 conica x melanophloia
-conica x nubilis
 conicobulbosa
 conicogrisea
 conicoides
 conicoverrucosa
 conicum
 conicus
 coniectum
@@ -8101,14 +8288,15 @@
 conifera
 coniferus
 coniifolia
 coniifolium
 coniocarpa
 coniochlora
 coniocraea
+coniogrammes
 coniophloia
 coniophora
 coniophorella
 coniophorus
 coniops
 conista
 conistea
@@ -8130,14 +8318,15 @@
 connatus
 connectens
 connerensis
 connexa
 conniana
 connianum
 connivens
+connolei
 connorsii
 conocarpa
 conocarpum
 conocephala
 conocephala x microphylla
 conocephalus
 conocladulum
@@ -8165,14 +8354,15 @@
 conranensis
 conranii
 consanguinea
 consanguineum
 consideneana
 consideniana
 considenianae
+considineana
 consimile
 consimilis
 consobrina
 consobrinum
 consocians
 consociata
 consociatum
@@ -8190,28 +8380,30 @@
 conspicua
 conspicuiflorum
 conspicuum
 conspicuus
 conspirans
 conspurcata
 constablei
+constancestoneae
 constanciae
 constans
 constellata
 constellatio
 constipata
 constricta
 constricta Narrow-leaved pubescent form
 constricta Pubescent form
 constricta Type Form
 constrictans
 constrictospora
 constrictum
 constrictus
 construens
+contaminatum
 contecta
 contectum
 contendens
 contenta
 contermina
 conterminus
 contexta
@@ -8248,14 +8440,15 @@
 conturba
 conturbata
 convallarioides
 convallis
 convallium
 conveniens
 convergens
+converta
 convexa
 convexella
 convexior
 convexiuscula
 convexula
 convexum
 convexus
@@ -8274,23 +8467,26 @@
 conwayensis
 conyzoides
 coogeeanum
 cookeana
 cookei
 cookeianum
 cookii
+cooksoniae
 coolabah
 coolabah - microtheca
 coolabah x crebra
 coolabah x melanophloia
 coolabah x populnea
 coolabah x whitei
+coolabuniensis
 coolaminica
 coolgardiense
 coolgardiensis
+cooljarloo
 coolminiana
 coolminianum
 cooloolae
 cooloolanus
 cooloomia
 coomae
 coomallo
@@ -8353,15 +8549,14 @@
 corallodendrum
 corallodesme
 coralloidea
 coralloides
 coralloides-cinerea
 coralloideum
 coralloideus
-corallophora
 corallorhiza
 corallum
 corbieri
 corchorifolia
 corcovadoensis
 cordanoides
 cordanum
@@ -8399,20 +8594,22 @@
 corifolia
 corifolium
 corifolius
 coriifolia
 coriifolium
 corinnae
 coriolus
+coriorum
 corium
 corkii
 cormiflora
 cormiflorum
 cornea
 corneliana
+cornerianum
 corneum
 corneus
 cornicina
 cornicularia
 corniculata
 corniculatum
 corniculatus
@@ -8461,14 +8658,15 @@
 coroniferum
 coroniforme
 coronilla
 coronillaefolia
 coronillifolia
 coronilloides
 coronillus
+coronohesperidea
 coronopifolia
 coronopifolius
 coronopus
 coronulata
 coronulatum
 coronum
 corpulenta
@@ -8510,14 +8708,15 @@
 corticatus
 corticicola
 corticiforme
 corticiformis
 corticola
 corticophilus
 corticosa
+corticosae
 corunnae
 corusca
 corvijuga
 coryli
 corylifolia
 corylifolium
 corylophilum
@@ -8528,14 +8727,15 @@
 corymbia
 corymbiae
 corymbifer
 corymbifera
 corymbiflora
 corymbiflorum
 corymbiformis
+corymbiicola
 corymbosa
 corymbosum
 corymbosus
 corymbulosa
 corynantha
 corynanthum
 corynelioides
@@ -8565,14 +8765,15 @@
 cosmopolites
 cossus
 costale
 costaricensis
 costata
 costatifructum
 costatifructus
+costatispora
 costatisporus
 costatum
 costatus
 costelloi
 costiglumis
 costinervis
 costiniana
@@ -8609,25 +8810,27 @@
 cowleana x gonoclada
 cowleana x hammondii
 cowleana x tropica
 cowleanum
 cowleyae
 cowleyana
 cowleyi
+coxeniae
+coxi
 coxii
+coyrecup
 crabro
 cracca
 cracens
 cracente
 cracentis
 craegii
 craggyensis
 craigiae
 craigiana
-craigii
 crameri
 cramesina
 cramesinus
 cranei
 cranfieldii
 cranfordi
 craniiformis
@@ -8644,14 +8847,15 @@
 crassicalyx
 crassicarpa
 crassicarpa x midgleyi
 crassicarpum
 crassicaudex
 crassicaulis
 crassichila
+crassicontexta
 crassicostata
 crassidens
 crassiflora
 crassiflorus
 crassifolia
 crassifolium
 crassifolius
@@ -8712,21 +8916,19 @@
 craynii
 crebea
 creber
 creberrima
 creberrimum
 crebra
 crebra x decorticans
-crebra x fibrosa
 crebra x leptophleba
 crebra x melanophloia
 crebra x melliodora
 crebra x microcarpa
 crebra x moluccana
-crebra x nubilis
 crebra x orgadophila
 crebra x populnea
 crebra x shirleyi
 crebra x siderophloia
 crebra x thozetiana
 crebra x whitei
 crebrecostatus
@@ -8737,14 +8939,15 @@
 crebriforme
 crebrinerve
 crebrinervis
 crebrispinum
 crebrum
 crechqueraultii
 creethae
+creethiae
 crematelloides
 cremea
 cremeoisabellinum
 cremeum
 cremiflora
 cremiflorum
 cremna
@@ -8765,14 +8968,15 @@
 crenulatocollis
 crenulatum
 crenulatus
 creperum
 crepidioides
 crepidis-japonicae
 crescens
+crescentiloba
 crescentium
 crespoae
 creswelli
 creswellii
 creta
 cretacea
 cretaceum
@@ -8848,14 +9052,15 @@
 crista
 crista-galli
 cristaefolium
 cristaspora
 cristata
 cristata x glauca
 cristatella
+cristatosporum
 cristatum
 cristatus
 cristifera
 cristiferum
 cristifolia
 cristiloba
 cristobalensis
@@ -8867,23 +9072,25 @@
 crithmifolius
 croajingolensis
 croasdaleae
 crocata
 crocatoides
 crocea
 croceella
+croceorrhizus
 croceum
 croceus
 crocicreas
 crocidens
 crociformis
 crociphylla
 crociphyllus
 crocodiliensi
 crocodiliensis
+crocodyli
 crocodyloides
 crocopeplum
 crocosmaeflora
 crocosmiaeflora
 crocosmiflora
 crocosmiiflora
 croftianus
@@ -8908,14 +9115,15 @@
 crotolariae
 crotonensis
 crotonis
 crouanii
 crouanioides
 crouchiana
 crowei
+crowfoothodgkiniae
 crowii
 crowleana
 crowleyae
 crowleyi
 croxfordiae
 croydonensis
 crozalsiana
@@ -9008,14 +9216,15 @@
 cryptostachys
 cryptostegiae
 cryptostemmae
 cryptostemmatis
 cryptostoma
 cryptothrix
 cryptotricha
+cryptovalsoidea
 cryptum
 crystalina
 crystallifera
 crystalligerus
 crystallina
 crystallinum
 crystallinus
@@ -9034,14 +9243,15 @@
 cucubalis
 cucubalus
 cucullata
 cucullatum
 cucullatus
 cucullifolia
 cuculligera
+cuculligerum
 cucumerifolius
 cucumerina
 cucumerinum
 cucumerinum x bowmanii
 cucumerinum x linguiforme
 cucumeris
 cucumis
@@ -9051,14 +9261,15 @@
 cucurbitella
 cucurbitinum
 cucurbitula
 cudraniae
 cuensis
 cujete
 culcitella
+culcullata
 culcutratum
 culicinum
 culisetae
 culleni
 cullenii
 cullenii x leptophleba
 cullenii x melanophloia
@@ -9165,14 +9376,18 @@
 curtispina
 curtistriata
 curtophylla
 curtum
 curtus
 curvata
 curvatiloba
+curvatimyriella
+curvatinavajoana
+curvatiobliqua
+curvativitalbae
 curvatocomosum
 curvatulus
 curvatum
 curvatus
 curvescens
 curviapicis
 curvicarpa
@@ -9181,27 +9396,25 @@
 curvicauda
 curvicaule
 curvicaulis
 curviceps
 curviclavia
 curvicollum
 curvicorne
-curvicornis
 curvicuspe
 curvidentata
 curviflora
 curvifolia
 curvifolius
 curvihirtum
 curviloba
 curvinervia
 curvipes
 curvirostra
-curvirostre
-curvirostris
+curvirostrum
 curviseriata
 curviseta
 curvisetum
 curvisetus
 curvispicatum
 curvispora
 curvistyla
@@ -9215,17 +9428,17 @@
 cuscutiflorus
 cuscutiformis
 cuspidata
 cuspidata x retusa
 cuspidatum
 cuspidatus
 cuspidicalyx
+cuspidifer
 cuspidifera
 cuspidiferum
-cuspidiferus
 cuspidifolia
 cuspidifolium
 cuspidifolius
 cuspidigera
 cuspidigerum
 cuspidilingue
 cuspidistipula
@@ -9254,30 +9467,34 @@
 cyanocarpus
 cyanocephala
 cyanoclada
 cyanococca
 cyanodiscalis
 cyanodiscus
 cyanogranulifer
+cyanogranulifera
 cyanoides
 cyanonioides
 cyanopetala
 cyanopetalus
 cyanophylla
 cyanophyllum
 cyanophyllus
 cyanopioides
 cyanoplectra
 cyanopora
 cyanosperma
 cyanospermus
+cyanotrichia
+cyanotrichium
 cyanoxantha
 cyanoxanthus
 cyanus
 cyatheae
+cyatheicola
 cyathicarpa
 cyathicarpum
 cyathicarpus
 cyathicola
 cyathifer
 cyathifera
 cyathiflora
@@ -9331,27 +9548,29 @@
 cycnocephalus
 cycnopotamica
 cycnorum
 cydonia
 cydoniae
 cydoniaefolia
 cydoniaefolius
+cydonifolius
 cydoniifolia
 cygna
 cygnea
 cygneus
 cygnicolla
 cygnisetum
 cygnopotamia
 cygnopotamica
 cygnopotamius
 cygnorum
 cygnus
 cylindracea
 cylindraceocampanulatus
+cylindraceum
 cylindraceus
 cylindrangia
 cylindrata
 cylindrica
 cylindricarpum
 cylindriceps
 cylindricoideum
@@ -9386,21 +9605,23 @@
 cymbalariifolius
 cymbalifer
 cymbalifera
 cymbaliferus
 cymbaria
 cymbelliformis
 cymbellus
+cymbidiicola
 cymbifolia
 cymbifolioides
 cymbifolium
 cymbiforme
 cymbiformis
 cymbonoti
 cymbophyllum
+cymbopogi
 cymbopogonis
 cymbopogonis-bombycini
 cymiferum
 cymiflora
 cymodoceae
 cymopoliae
 cymosa
@@ -9418,17 +9639,18 @@
 cynodontis
 cynodontoides
 cynosuroides
 cynthia
 cynurica
 cyparioides
 cyparissias
-cyparoides
 cypellocarpa
+cypellocarpae
 cypellomitrium
+cyperacearum
 cyperi
 cyperi-lucidi
 cypericola
 cyperina
 cyperinus
 cyperodes
 cyperoides
@@ -9537,25 +9759,26 @@
 dallachyanum
 dallachyanus
 dallachyi
 dallanneyi
 dalliana
 dalmatica
 dalmaticum
-dalmaticus
 dalmeniensis
 dalmiensis
 dalrympleana
 dalrympleana x gunnii
 dalrympleana x viminalis
+dalrympleanae
 dalrympliana
 daltoni
 daltonii
 dalveenica
 dalyana
+dalyelliae
 dalyellii
 damae-cornis
 damaecornis
 damannii
 damascena
 damasonium
 damasonum
@@ -9565,15 +9788,17 @@
 dammarae
 dammeri
 dammerianum
 damopsis
 dampierae
 dampieri
 dampierii
+danbullense
 danbullensis
+dandenongensis
 danesiana
 danesianum
 danesii
 dangarense
 dangarensis
 dangeardiana
 dangeardii
@@ -9584,35 +9809,38 @@
 danseyi
 dansie
 dansiei
 danthoniae
 danthoniae-frigidae
 danthonioides
 daphne
+daphneae
 daphnifolia
 daphnifolium
 daphnodes
 daphnoides
 dapperensis
 dapsilanthi
 darbyshirei
 dareicarpa
 dargilensis
 dargonia
 dargonius
 darjeelensis
 darleyenisis
+darliae
 darlingensis
 darlingiana
 darlingtonii
 daronensis
 darwinensis
 darwinianus
 darwinii
 darwinioides
+darwinoides
 dasaea
 dastuguei
 dasyae
 dasyantha
 dasycalyx
 dasycarpa
 dasyclada
@@ -9621,22 +9849,24 @@
 dasyphloia
 dasyphylla
 dasyphyllum
 dasyphyllus
 dasypleurum
 dasypoga
 dasypogoides
+dasypogonis
 dasypus
 dasyrrhache
 dasysperma
 dasystachys
 dasystylis
 dasyura
 dasyurum
 datil
+dauci
 daucinus
 daucoides
 davalianus
 davalliana
 davallianum
 davallioides
 davenporti
@@ -9655,19 +9885,22 @@
 davisiae
 davisiana
 davisii
 davisoniellae
 davurica
 daweana
 daweanum
+dawei
 dawsoni
 dawsonii
+dawsoniorum
 dayboroana
 dayi
 dayiana
+daymanianum
 daymannianum
 de beuzevillei
 dealbata
 dealbata x prava
 dealbatum
 dealbatus
 deaneanum
@@ -9685,28 +9918,28 @@
 debilicaulis
 debilior
 debilis
 debilissima
 debilissimum
 debilissimus
 debneyi
+debralockiae
 debyi
 decaisneana
 decaisneanum
 decaisnei
 decaisnii
 decalvans
 decalvatus
 decandra
 decandra x tagal
 decandrum
 decandrus
 decapetala
 decaptera
-decaryana
 decasetus
 decaspermoides
 decastes
 decazesii
 decedens
 decemcellulare
 decemcostata
@@ -9798,14 +10031,15 @@
 defossa
 defossum
 defungens
 degelii
 degenerans
 degenii
 deglubens
+degreyensis
 degreyi
 dehiscens
 dehoogii
 dejecta
 dejectum
 dejectus
 dekindtiana
@@ -9855,15 +10089,14 @@
 deltodeum
 deltoidea
 deltoiden
 deltoides
 deltoideum
 deltophylla
 delutula
-delvisoi
 demarzii
 dematioides
 dematium
 demersa
 demersum
 demethylbarbatica
 demethylmicrophyllinicum
@@ -9885,32 +10118,33 @@
 dendritica
 dendriticum
 dendriticus
 dendrobatidis
 dendrobia
 dendrobioides
 dendrocharis
-dendrographae
 dendroidea
 dendroides
 dendroideum
 dendroideus
 dendromerinx
 dendromorpha
 dendrosheath
 dendrospinosa
 dendrothrix
 denegans
 deneufvillei
 denhartogii
 denigrata
 denigratus
+denisoni
 denisonii
 denmarkica
 denmarkicus
+dennisiae
 dennisii
 dens
 dens-leonis
 densa
 densestriata
 densevestita
 densevestitum
@@ -9931,14 +10165,15 @@
 densivestitus
 densum
 densus
 dentata
 dentata x parasitica
 dentatifolia
 dentatifolius
+dentatim
 dentatum
 dentatus
 dentella
 dentellata
 dentex
 denticula
 denticulata
@@ -9947,14 +10182,15 @@
 denticulatus
 denticuliferum
 denticulosa
 denticulosum
 denticuspis
 dentifera
 dentiferum
+dentifolius
 dentigera
 dentigeroides
 dentilabellum
 dentistipulum
 dentosa
 denudata
 denudatum
@@ -10044,23 +10280,26 @@
 deuteroeburneum
 deuteroneura
 deuteroneurum
 develatula
 devexa
 devexum
 deviata
+devikae
 devilliersiana
 devitata
 devito
 devius
 devoniensis
 devriesii
 dewrangia
 dextropinea
+dharug
 dharugensis
+dhileepani
 diabolica
 diabolicum
 diabolophyllum
 diabolus
 diacantha
 diacanthum
 diacapsis
@@ -10090,15 +10329,14 @@
 dianellaceum
 dianellae
 dianellicola
 dianellincola
 diantha
 dianthifolia
 dianthifolium
-dianthifolium x racemosum
 dianthophorum
 dianthorum
 diaphaenenta
 diaphana
 diaphanoneuron
 diaphanophleba
 diaphanophlebia
@@ -10112,19 +10350,21 @@
 diastemata
 diatrypa
 diatrypelloidea
 diatrypeoides
 diatyches
 dibenzofuranica
 dicarpa
+dicarpon
 dicarpum
 dicephala
 diceratum
 dichaeta
 dichanthioides
+dichapetali
 dichasiale
 dichelachne
 dichohotomum
 dichondrae
 dichopetala
 dichopitys
 dichoptera
@@ -10250,15 +10490,14 @@
 diffractaica
 diffractella
 diffractum
 diffusa
 diffusum
 diffusus
 digitale
-digitalis
 digitaria
 digitariae
 digitata
 digitatum
 digitatus
 digitiformis
 digitoradiata
@@ -10288,14 +10527,15 @@
 dillwyniaefolia
 dillwyniaefolium
 dillwynifolia
 dillwynii
 dillwyniifolia
 dillwynioides
 dillwynoides
+dilophospora
 dilucida
 dilucidum
 diluta
 diluviana
 dimbulahensis
 dimenica
 dimerelloides
@@ -10323,14 +10563,15 @@
 dimorpholepis
 dimorphospora
 dimorphosporum
 dimorphotricha
 dimorphum
 dimorphus
 dimporphandra
+dindenense
 dindygulensis
 dineura
 dingleyae
 dinocalyx
 dinteri
 diococcum
 diodon
@@ -10421,14 +10662,15 @@
 discoideus
 discolor
 discolor x antennatum
 discolor x johannis
 discolor x nindii
 discolor x semifuscum
 discolorata
+discoloratum
 discophora
 discordans
 discorde
 discordis
 discors
 discrepans
 discreta
@@ -10447,14 +10689,15 @@
 disjungenda
 disoxyli
 dispar
 disparata
 disparilis
 disparipes
 disparrima
+disparrimae
 disparrimum
 disperma
 dispermum
 dispermus
 dispersa
 dispersogranulata
 dispersum
@@ -10536,14 +10779,15 @@
 ditassodes
 ditassoides
 ditatatum
 dithotoma
 ditopa
 ditopus
 ditricha
+ditrichi
 ditrichii
 ditrichum
 ditrigynus
 dittrichii
 diurna
 diurnum
 diuroides
@@ -10588,14 +10832,15 @@
 dixoniana
 dixonii
 dixsoni
 dixsonii
 djamor
 djerral
 djinda
+djirangnandiri
 dobagii
 dobreeanum
 dobsoni
 dobsonianum
 dobsonii
 dochmia
 dochmius
@@ -10609,14 +10854,15 @@
 dodonaeae
 dodonaeaefolia
 dodonaeifolia
 dodonaeifolia x paradoxa
 dodonaeifolium
 dodoneaefolia
 doellingeri
+doerrieniae
 doggrellii
 dohertyi
 dohrnii
 doidgeae
 doidgei
 dolabratus
 dolabriformis
@@ -10681,14 +10927,15 @@
 dominicana
 dominii
 donaldiana
 donaldsoni
 donaldsonii
 donalsonii
 donax
+donbarrettii
 dongarraensis
 dongicola
 donianus
 donneri
 donniana
 donnianum
 donnianus
@@ -10703,15 +10950,14 @@
 dorcadideus
 doreta
 dorisiana
 doronici
 dorothea
 dorotheae
 dorothyae
-dorothyi
 dorrien-smithii
 dorrienii
 dorrienii x obesa
 dorrigoensis
 dorsale
 dorsalisulcum
 dorsenna
@@ -10750,14 +10996,15 @@
 dracophylla
 dracophylloides
 drake-castilloi
 drakeoides
 drapetocoleus
 dregeana
 dregeanum
+drenthii
 drepanocarpa
 drepanocarpa (variant)
 drepanocarpum
 drepanocladum
 drepanophylla
 drepanophylla x melanophloia
 drepanophylla x populnea
@@ -10803,14 +11050,15 @@
 drymophila
 drymophilus
 dryophila
 dryophilus
 dryophylla
 drysdalensis
 dualis
+duaringa
 duarteana
 dubenii
 dubia
 dubiosa
 dubiosum
 dubitabilis
 dubitata
@@ -10820,24 +11068,26 @@
 dubius
 dubliniensis
 dubyi
 ducassei
 duchassaingiana
 duchassaingianus
 duckerae
+duclitan
 dudleyensis
 duerrenbergiana
 duffii
 dufourii
 dugulla
 duiganiae
 dulca
 dulcamara
 dulce
 dulcis
+dulitan
 dumastii
 dumeticola
 dumetorum
 dumetosa
 dumicola
 dumosa
 dumosiformis
@@ -10851,14 +11101,15 @@
 dundasi
 dundasiae
 dundasii
 dungarra
 dunlopiana
 dunlopianum
 dunlopii
+dunni
 dunnii
 dunstani
 dunstaniae
 dunstanii
 duoformis
 duomilia
 duomilius
@@ -10911,18 +11162,19 @@
 dysantha
 dysophylla
 dysophyllus
 dysoxyli
 dysoxylicola
 dysphanoides
 dysprosium
-e sp. Bonaparte Archipelago (A.A.Mitchell 4774)
 eachamensis
+eadesi
 eadesii
 eardleyae
+earlei
 earlii
 eartoxicus
 eastii
 eastoni
 eastonii
 eatoni
 eatoniae
@@ -11018,15 +11270,14 @@
 eclyptoides
 ecmocyna
 ecolumellata
 ecorne
 ecorniculata
 ecornis
 ecorollata
-ecoronata
 ecorticata
 ecostata
 ecostatum
 ecrassifolium
 ecristata
 ectadioclada
 ectanea
@@ -11047,24 +11298,26 @@
 edax
 edelfeltii
 edentata
 edentatum
 edentatus
 edentula
 edgeworthii
-ednaena
+ednaeana
 ednana
 ednieana
 edodes
 educta
 edule
 edulentum
 edulis
 edura
 edwardsii
+eelemani
+eendrachtslandiae
 eenii
 eerwah
 efflorescens
 efflorescens - horistes
 effodiendus
 effugiens
 effusa
@@ -11170,14 +11423,15 @@
 elatostipitatus
 elatum
 elatus
 elatus x oreophilus
 elderi
 elderiana
 eldridgei
+eleanorwilliamsiae
 electrospermum
 elegans
 elegans Fraser Road form (A.C.Burns 27)
 elegantior
 elegantissima
 elegantissimum
 elegantissimus
@@ -11192,35 +11446,41 @@
 eleusinis
 eleusinoides
 eleuterostachya
 eleuterostachyum
 eleutherostachya
 eleutherostachyum
 elevata
-elevativena
 elfvingii
 elginense
 elginensis
 eliae
-elicifolia
 elimbata
 elimbatum
 elimbatus
+elioniae
 eliosurum
 elisabethae
 elisabethiae
+elisabettae
 elisae
 elixia
 elixiana
 elixii
 elizabethae
+elizabethalexanderae
+elizabethandersoniae
+elizabethblackwelliae
+elizabethdatsoniae
 elizabethiae
+elizabethkenny
 elizae
 elkhartiense
 ellae
+ellenclarkiae
 elleniae
 elleryana
 elliffii
 elliotii
 elliottii
 ellipsicarpa
 ellipsoidea
@@ -11229,16 +11489,18 @@
 ellipsospora
 ellipsosporum
 elliptica
 elliptice
 ellipticifolia
 ellipticum
 ellipticus
+ellisi
 ellisia
 ellisii
+ellisrowaniae
 ellistoniae
 ellytes
 elmae
 elmeri
 elminthoides
 elobata
 elobatum
@@ -11284,14 +11546,15 @@
 emmenosperma
 emmenospermatus
 emmonsii
 emmottii
 emodensis
 empelioclada
 empeliocladum
+empetrifola
 empetrifolia
 empetriformis
 empetroides
 emphysopus
 emuina
 emuina x littoralis
 emulum
@@ -11350,16 +11613,18 @@
 endopurpurea
 endopyria
 endota
 endotheius
 endothrix
 endotricha
 endotrichum
+endotum
 endoxantha
 endoxanthum
+endrylaenoides
 eneabba
 eneabbensis
 enerve
 enervia
 enervifolia
 enervis
 enervium
@@ -11384,14 +11649,15 @@
 enodis
 enorme
 ensata
 ensatum
 ensifer
 ensifera
 ensiferum
+ensifoali
 ensifolia
 ensifolia x microphylla
 ensifolium
 ensifolius
 ensiforme
 ensiformis
 ensigera
@@ -11408,14 +11674,15 @@
 enteroxantha
 enthyle
 entochlora
 entocosmesis
 entodiaphana
 entodontoides
 entomogama
+entomophila
 entospora
 entrancensis
 entrichoma
 enypniastina
 enzenspergerianum
 enzenspergerianus
 eobalta
@@ -11431,14 +11698,15 @@
 epacridoides
 epacridoideum
 epacrioides
 epacroides
 epacrospora
 epactia
 epaleata
+epeduncularis
 epedunculata
 epedunculatum
 eperforata
 epheboides
 ephedraea
 ephedroides
 ephemera
@@ -11476,15 +11744,14 @@
 epilinteus
 epilinum
 epilobii
 epilobii-tetragoni
 epilobioides
 epilosa
 epimarta
-epimelaeana
 epimelaena
 epimicta
 epimyces
 epipacroides
 epipactoides
 epipastoides
 epiphylla
@@ -11504,14 +11771,15 @@
 episiliquosum
 epispora
 epitea
 epitephra
 epitephrum
 epitephrus
 epithele
+epitheloides
 epithemiae
 epithymum
 epitrema
 epixanthum
 epixanthus
 epizoa
 epruinata
@@ -11525,18 +11793,20 @@
 equisefolia
 equiseti
 equisetifolia
 equisetifolius
 equisetiformis
 equisetina
 equitans
+equitem
 equitum
 eradicata
 eradicatus
 eraemeum
+eragrosticola
 eragrostidis
 eragrostis
 eragrostoides
 eranthemodes
 eranthemoides
 eranthidis
 ercegovicii
@@ -11546,14 +11816,15 @@
 erecta
 erectifolia
 erectifolium
 erectiloba
 erectum
 erectus
 eremaea
+eremaeae
 eremaeum
 eremaeum x vaginiflorum
 eremaeus
 eremea
 eremica
 eremicola
 eremicus
@@ -11611,26 +11882,27 @@
 ericoides
 eriensis
 erifuga
 erigeroides
 erigona
 erikssonii
 erimae
-erimis
 erinacea
 erinaceum
 erinaceus
 erinoides
 erinus
 eriobotrya
 eriobotryae
 eriocalyx
 eriocarpa
 eriocarpus
 eriocaula
+eriocauli
+eriocaulis
 eriocaulum
 eriocephala
 eriocephalum
 eriocephalus
 eriochila
 eriochilum
 eriochilus
@@ -11642,14 +11914,15 @@
 eriocladus
 eriodes
 eriogena
 eriogenus
 eriogona
 eriolepis
 erioloma
+erionia
 eriophila
 eriophora
 eriophorum
 eriophorus
 eriophylla
 eriophyllum
 eriopoda
@@ -11785,14 +12058,15 @@
 esmeralda
 esperensis
 esperi
 esquamata
 esquamatum
 esquamatus
 esquirolii
+essexcoheniae
 essingtoniana
 esterhaziae
 estrophiolata
 estrophiolatum
 estuariale
 esulifolia
 esulifolium
@@ -11800,29 +12074,35 @@
 eta
 etchellsii
 etheira
 ethelae
 etheliana
 ethelium
 etheridgensis
+etinsideae
 etmanii
+etonensis
+euabalongensis
 euarcuatum
 euarcuatus
 euastroides
 eubenangeensis
 eubryani
 eucalypta
 eucalyptaceum
 eucalypti
+eucalyptica
 eucalypticola
 eucalypticum
 eucalyptifolia
 eucalyptifolius
 eucalyptiformis
 eucalyptigena
+eucalyptigenum
+eucalyptina
 eucalyptinus
 eucalyptodes
 eucalyptoides
 eucalyptophylla
 eucalyptorum
 eucamptodontoides
 eucentrica
@@ -11846,14 +12126,15 @@
 eugelii
 eugellii
 eugenea
 eugeneum
 eugeniae
 eugeniae-jamboloidis
 eugeniarum
+eugenieclarkiae
 eugeniodes
 eugenioides
 eugenum
 euglypta
 eugrammum
 eugrammus
 eulaliae
@@ -11870,14 +12151,15 @@
 eungellense
 eungellensis
 eunotia
 euodes
 euodiae
 euodiformis
 euodiiformis
+euonymicola
 eupatoria
 eupatorioides
 eupetraeoides
 euphaeus
 euphemiae
 euphleba
 euphlebia
@@ -11914,15 +12196,14 @@
 eurycarpa
 eurychordae
 euryloba
 eurylobos
 eurynema
 euryphylla
 euryphyllum
-eurysaca
 eurysacum
 euryspermus
 eurystoma
 eustachii
 eustephana
 eustomum
 eustyle
@@ -11951,29 +12232,29 @@
 evansii
 evasa
 evasum
 evecta
 evectum
 evenulosa
 evenulosum
-everadensis
 everardensis
 everettiana
 everistiana
 everistii
 evernica
 evernius
 eversa
 everta
 evexa
 eviscidula
 evodiiformis
 evolceanui
 evolutum
 evolvens
+ewarti
 ewartiana
 ewartianum
 ewartianus
 ewartii
 ewersii
 ewingii
 exacta
@@ -12012,15 +12293,14 @@
 excelsa
 excelsa x kermadecensis
 excelsior
 excelsum
 excelsus
 excentrica
 excentricum
-excentricus
 excentriporum
 excipulata
 excipulatus
 excisa
 excisifolia
 excisifolius
 excisula
@@ -12028,14 +12308,15 @@
 excludens
 excorians
 excoriata
 excoriatus
 excurrens
 exfimbriatus
 exfoliata
+exigens
 exigua
 exigua x gregaria
 exiguella
 exiguifolia
 exiguifolius
 exiguis
 exiguum
@@ -12223,20 +12504,23 @@
 farctus
 fareana
 farinacea
 farinaceum
 farinaceus
 farinicola
 farinosa
+farinosae
+farinosipes
 farinosum
 farinosus
 farinulenta
 farlowii
 farmeri
 farnesiana
+farnesianae
 farquharsonii
 farragei
 farrangei
 fascia
 fasciata
 fasciatum
 fasciatus
@@ -12256,14 +12540,15 @@
 fasciculosa
 fasciculum
 fascifolia
 fasciola
 fasciolum
 fastibile
 fastibilis
+fastidia
 fastidiosa
 fastidium
 fastigata
 fastigatum
 fastigiata
 fastigiatum
 fastigiatus
@@ -12309,14 +12594,15 @@
 federata
 fedtschenkoi
 feei
 feejeensis
 feliciennae
 felina
 felinum
+felis
 felleus
 felliana
 fellii
 fellowsii
 femina
 fenestrata
 fenestratum
@@ -12364,14 +12650,15 @@
 ferruginicincta
 ferruginiflora
 ferruginiflorus
 ferruginipes
 ferruginosa
 ferruginosus
 ferruma
+fertile
 fertilis
 fertillis
 ferulacea
 fervens
 festiva
 festivum
 festucacea
@@ -12381,24 +12668,26 @@
 feuereri
 fibrata
 fibriatus
 fibrilloides
 fibrillopes
 fibrillosa
 fibrillosibrunnea
+fibrillosipes
 fibrillosus
 fibrosa
 fibrosa x moluccana
 fibrosissima
 fibrosopileatum
 fibrosum
 fibrosus
 fibula
 fibulifera
 ficaria
+ficherai
 fici
 fici-orbispora
 ficicola
 ficifolia
 ficifolium
 ficifolius
 ficioides
@@ -12488,15 +12777,14 @@
 fimetarius
 fimeti
 fimicola
 fimiputris
 finalis
 finaustrina
 findlayi
-fineranii
 finetiana
 finetii
 finetti
 finitima
 finitimum
 finkii
 finlandicum
@@ -12505,14 +12793,15 @@
 finlaysoniana
 finlaysonianum
 finlaysonii
 finnica
 finniganense
 finniganensis
 finnisterrae
+fioriniae
 firma
 firmula
 firmum
 firmus
 firthii
 fischeri
 fischerianus
@@ -12537,14 +12826,15 @@
 fissistipus
 fissivalve
 fissivalvis
 fissofurcata
 fissum
 fissura
 fissurata
+fissuratum
 fissuristoma
 fistula
 fistulatum
 fistuloides
 fistulosa
 fistulosum
 fistulosus
@@ -12583,15 +12873,14 @@
 flaccidifolium
 flaccidisetum
 flaccidisetus
 flaccidissima
 flaccidissimum
 flaccidulum
 flaccidum
-flaccidum x gracillimum
 flaccidus
 flacida
 flagella
 flagellaceum
 flagellaceus
 flagellans
 flagellare
@@ -12602,15 +12891,15 @@
 flagellifer
 flagellifera
 flagelliferum
 flagelliferus
 flagelliforme
 flagelliformis
 flagelligera
-flagelliramus
+flagellirameus
 flagellispora
 flagellum
 flamabile
 flamabilis
 flamea
 flammans
 flammea
@@ -12627,14 +12916,15 @@
 flavelifolium
 flavella
 flavellum
 flaventior
 flaveolum
 flavescens
 flavescentireagens
+flavescentis
 flavicans
 flavicarinata
 flavicomum
 flavicomus
 flaviculmis
 flavicunda
 flavida
@@ -12659,21 +12949,23 @@
 flavimarina
 flavinervis
 flavipes
 flaviphylla
 flavipila
 flavipilum
 flavipora
+flaviporus
 flavispinum
 flavissima
 flavissimum
 flavistyla
 flavo-olivacea
 flavo-virens
 flavoalba
+flavoalbida
 flavoalbus
 flavoaurantiaca
 flavobrunnescens
 flavocaerulescens
 flavocostatus
 flavocrocea
 flavocroceus
@@ -12682,14 +12974,15 @@
 flavofaciens
 flavofuscum
 flavogenita
 flavoisidiata
 flavolimbata
 flavolurida
 flavomedullosum
+flavomucosus
 flavonigritus
 flavopallida
 flavopila
 flavopunctata
 flavopurpurea
 flavorubescens
 flavostraminea
@@ -12700,32 +12993,33 @@
 flavovirescens
 flavoviride
 flavoviridis
 flavum
 flavus
 fleckeri
 fletcheri
+fleuryana
 flexa
 flexella
 flexialabastra
 flexibilis
 flexicaule
 flexicaulis
 flexicollis
 flexifolia
 flexifolium
 flexifolius
 flexile
 flexilis
+fleximarginata
 flexinervis
 flexinutans
 flexipes
 flexipile
 flexispora
-flexomarginata
 flexuosa
 flexuosiformis
 flexuosissima
 flexuosum
 flexuosus
 flexusa
 flindersiana
@@ -12734,34 +13028,33 @@
 flindersiensis
 flindersii
 flintii
 floccipes
 floccoides
 floccopus
 floccosa
+floccosibrunnea
 floccosum
 floccosus
 flocculenta
 flocculiformis
 flocculosa
 flocculosus
 flocktonae
 flocktoniae
 floerkeana
-floerkiana
 floodii
 floralis
 florea
 floresia
 floresius
 floribunda
 floribunda 'delicate form'
 floribunda variant
 floribunda x leiocarpa
-floribunda x tetraphylla
 floribunda x woodsiana
 floribundum
 floribundus
 floriceps
 florida
 floridaensis
 floridana
@@ -12934,14 +13227,15 @@
 fornicatum
 fornicatus
 forresterae
 forrestiae
 forrestiana
 forrestianum
 forrestii
+forsbergii
 forskalii
 forskallii
 forstenii
 forsteri
 forsteriana
 forsterianum
 forsterii
@@ -12959,14 +13253,15 @@
 fortunae-hibernae
 fortunata
 fortuneana
 fortunei
 fosbergii
 fosliei
 fossa
+fossiculatum
 fossulata
 fossulicola
 fosteri
 fothergillii
 fournieri
 foustinellum
 foveata
@@ -13025,15 +13320,14 @@
 franklinianum
 franklinii
 fraserae
 fraserana
 fraseranum
 fraserensis
 fraseri
-fraseriae
 fraseriana
 fraserianum
 fraserianus
 fraterna
 fraternalis
 fraternus
 fratris
@@ -13042,35 +13336,39 @@
 fraudulenta
 fraudulentum
 frauenfeldiana
 frauenfeldianum
 frauenfeldii
 fraxinea
 fraxineum
+fraxini-angustifoliae
 fraxinifolia
 fraxinifolium
 fraxinifolius
 fraxinoides
 frazeri
 fredwoodii
+freelingi
 freelingii
 freemani
 freemanii
 frenchiana
 frenchii
 frequentans
 fretensis
 freyciana
+freycinetiae
 freycinetiana
 freycinetii
 friabilis
 frians
 fribrillosa
 frickei
-friderici-augusta
+friderici augusti
+friderici-augusti
 friedrichsthalii
 friesiana
 friesianum
 friesianus
 friesii
 frigescens
 frigida
@@ -13082,14 +13380,15 @@
 frohlichii
 frondicola
 frondosa
 frondosum
 frondosus
 frontalis
 frostii
+froudistii
 fructicola
 fructicosus
 fructigenum
 fructo-tecto
 fructoglabrum
 frugalis
 frumentacea
@@ -13125,14 +13424,15 @@
 fuciforme
 fuciformis
 fuckelii
 fucosa
 fucosus
 fuegianum
 fuellebornii
+fuernrohri
 fuernrohrii
 fugacissima
 fugax
 fugiens
 fugitivum
 fuhreri
 fuirenoides
@@ -13152,14 +13452,15 @@
 fuliginodes
 fuliginosa
 fuliginosum
 fuliginosus
 fullagari
 fullagarii
 fullageri
+fullertonii
 fullonum
 fulmen
 fulva
 fulvaster
 fulvastra
 fulvastrum
 fulvella
@@ -13170,15 +13471,15 @@
 fulviflorum
 fulvilubrica
 fulvo-olivacea
 fulvoatomatus
 fulvocinerea
 fulvoiubatus
 fulvotingens
-fulvoviolacea
+fulvotomentosa
 fulvula
 fulvum
 fulvus
 fumaginea
 fumana
 fumanum
 fumarprotocetrarica
@@ -13190,17 +13491,17 @@
 fumosa
 fumosella
 fumosopruinosum
 fumosula
 fumosum
 fumosus
 funafutiense
+funale
 funalis
 funckii
-funebris
 funerata
 funerea
 fungicola
 fungiforme
 fungoides
 fungosa
 funicola
@@ -13211,14 +13512,15 @@
 funiforme
 funiformis
 funigera
 furca
 furcata
 furcatifolia
 furcatifolium
+furcatispina
 furcatispinus
 furcatospermus
 furcatum
 furcatus
 furcellaria
 furcellariae
 furcellata
@@ -13290,14 +13592,15 @@
 fuscopurpureus
 fuscorufa
 fuscosorediata
 fuscosporum
 fuscosquamea
 fuscosquameus
 fuscosquamosa
+fuscosquarrosa
 fuscosubtile
 fuscosuccinea
 fuscoumbonatus
 fuscovinosum
 fuscoviolacea
 fuscoviolaceum
 fuscoviolaceus
@@ -13323,19 +13626,21 @@
 gaagudju
 gabrielae
 gabrieli
 gabrielis
 gabrielsonii
 gadgarrense
 gadgarrensis
+gadigal
 gaditjirrii
 gaertneri
 gageoides
 gahniae
 gahnianum
+gahniicola
 gahnioides
 gaillardianum
 gaillonii
 gaimardii
 gainii
 gairdnerianum
 galactina
@@ -13414,14 +13719,15 @@
 ganopoda
 gardineri
 gardneri
 gardnerianum
 gariepinum
 gariwerdensis
 garlandii
+garlbiwalawarda
 garrawayae
 garrawayi
 garretti
 garrettii
 garrolense
 garrowayi
 gascoynensis
@@ -13430,19 +13736,21 @@
 gasparriniae
 gasstroemi
 gasstroemii
 gasteenii
 gasteroidea
 gasterosteus
 gastonis
+gastroemi
 gastroemii
 gastroides
 gastrolobii
 gastromycetoides
 gastrum
+gatesiae
 gatesii
 gattyae
 gattyana
 gattyanum
 gatunense
 gaubae
 gaudichaudi
@@ -13463,16 +13771,18 @@
 gayana
 gayanum
 gayanus
 gayi
 gazellae
 geaster
 geeingwa
+geeringii
 geheebii
 gei
+geijerae
 geinitzi
 geissoloma
 geitonoplesii
 gelasina
 gelasinum
 gelatinifera
 gelatinosa
@@ -13495,14 +13805,15 @@
 gemelliparum
 gemellus
 gemina
 geminata
 geminatum
 geminatus
 geminella
+gemini
 geminiflora
 geminiflorum
 geminifolia
 geminifolium
 geminum
 gemma
 gemmata
@@ -13515,14 +13826,15 @@
 gemmiparus
 gendarussa
 generalis
 genethylloides
 genetylloides
 genevensis
 genevievae
+genevieveae
 genialis
 genianthum
 geniculata
 geniculatum
 geniculatus
 geniculosa
 genistaefolia
@@ -13608,14 +13920,15 @@
 gibberulosa
 gibberulosus
 gibberulum
 gibberulus
 gibberum
 gibberus
 gibbifolia
+gibbonsi
 gibbonsii
 gibbosa
 gibbosifolia
 gibbosum
 gibbosus
 gibbsiae
 gibbsoni
@@ -13640,14 +13953,15 @@
 gigaspora
 gigasporum
 gigasporus
 gilbertensis
 gilberti
 gilbertiana
 gilbertii
+gilesi
 gilesiana
 gilesianum
 gilesii
 gilfillaniorum
 gilgai
 gilgaiensis
 gilgiana
@@ -13656,22 +13970,24 @@
 gilleni
 gilleniae
 gillenii
 gillianus
 gilliesae
 gilliesii
 gillii
+gillingarra
 gillisonii
 gillivraei
 gillivrayi
 gilmorei
 gilmourii
 gilo
 gilruthiana
 gilva
+gilviceps
 gilvum
 gilvus
 ginninderrense
 gintarasii
 ginus
 gioisa
 giovanellae
@@ -13712,14 +14028,15 @@
 glabriflora
 glabriflorum
 glabriflorus
 glabrifolia
 glabrifoliatus
 glabrifolium
 glabrifolius
+glabrilimba
 glabripes
 glabripetala
 glabriscapa
 glabrisepala
 glabrisepalum
 glabrispiculus
 glabristyla
@@ -13744,14 +14061,15 @@
 gladiolus
 gladiosum
 glandicola
 glandifera
 glandulacea
 glandulaceus
 glandulaefolium
+glandulariae
 glandulicarpa
 glandulicarpum
 glandulifera
 glanduliferum
 glanduligera
 glandulosa
 glandulosa x velutina
@@ -13929,14 +14247,15 @@
 glossodioides
 glossodiphylla
 glossoides
 glossophylla
 glossosema
 glossostigma
 glossostigmum
+gloucesterense
 glumacea
 glumaceum
 glumaceus
 glumaris
 glutescens
 glutinifer
 glutinis
@@ -13982,20 +14301,22 @@
 godeffroyi
 godenowii
 godlewskii
 godofriediana
 godseffiana
 goebelii
 goeppertiana
+goeppertmayerae
 goetzeana
 goetzei
 goezeana
 goezeanus
 gogo
 goldiei
+goldingiae
 goldsackii
 goldsworthii
 gomontiana
 gomphispora
 gomphocarpum
 gomphocarpus
 gomphocephala
@@ -14041,27 +14362,30 @@
 goodeniicola
 goodenoughii
 goodenowii
 goodiae
 goodiaefolia
 goodii
 goodspeedii
+goodwini
 goodwiniae
 goodwinii
+goolgardi
 goonooensis
 goossensiae
 gorakhporense
 gordoni
 gordoniae
 gordoniana
 gordonii
 goreensis
 gorgonea
 gorgonina
 gossei
+gossiae
 gossypifolia
 gossypiifolia
 gossypina
 gossypinoannulata
 gossypinum
 gossypinus
 gossypiodes
@@ -14070,20 +14394,22 @@
 gottlandica
 gottscheana
 gottschei
 gouani
 goudeyi
 goulardi
 gouldii
+goulteri
 gourliei
 gourretii
 gourvilii
 goveniana
 goweri
 goyderi
+gracehopperae
 gracei
 gracilaria
 gracilarioides
 gracile
 gracilens
 gracilenta
 gracilentum
@@ -14101,20 +14427,20 @@
 gracilifolia
 gracilifolium
 graciliformis
 gracilior
 gracilipes
 gracilis
 graciliseta
+gracilissima
 gracilissimum
 gracilistipes
 gracilius
 gracillima
 gracillimum
-gracillimum x flaccidum
 gracillimum x hookerianum
 gracillimus
 graciloides
 gracilosum
 graciosus
 graeca
 graecizans
@@ -14267,42 +14593,48 @@
 grayana
 grayanum
 grayi
 grayii
 grayorum
 greavesii
 greeniana
+greevesi
 greevesii
 gregale
 gregalis
 gregantula
 gregaria
 gregaria x sp. aff. pauciflora (Short)
 gregarium
+gregata
 gregiflorus
+gregori
 gregoriensis
 gregorii
 gregoryensis
 gregsoni
 gregsoniana
 gregsonii
+greiderae
 grevilleae
 grevilleana
 grevillei
+grevilleicola
 grevillensis
 grevillensis x montana
 grevilleoides
 grevillii
 grevillina
 grevillioides
 grewiae
 grewiaefolia
 grewiifolia
 greyana
 greyi
+griceae
 grieveana
 grievei
 griffinianus
 griffinii
 griffithiana
 griffithianum
 griffithianus
@@ -14333,14 +14665,15 @@
 griseoramosa
 griseosquamulosum
 griseovelata
 griseovirens
 griseozonata
 griseum
 griseus
+groatii
 groeneri
 groenerii
 groenlandica
 groenlandicum
 grollei
 grossa
 grossealata
@@ -14388,14 +14721,15 @@
 guenter-grassii
 guentheri
 guepini
 guepinii
 guepinioides
 guerichianum
 guerinae
+gueriniae
 guernisacii
 guestrowiense
 guianense
 guianensis
 guibertii
 guicciardiniana
 guichensis
@@ -14415,14 +14749,16 @@
 gullicki
 gullickii
 gulliveri
 gulliverii
 gullweri
 gulngai
 gulungulana
+gulyae
+gumbaynggirr
 gummifera
 gummiferum
 gummosa
 gummosus
 gundarara
 gundermanica
 gunii
@@ -14454,14 +14790,15 @@
 gusukumai
 guthrieana
 guttata
 guttatum
 guttatus
 guttiforme
 guttula
+guttulatum
 guttulatus
 guttulifera
 guttuliferum
 gutwinskii
 guyanensis
 guyava
 guyeri
@@ -14518,14 +14855,15 @@
 gyropoda
 gyrostomoides
 gyrosum
 gysingensis
 haaboeliense
 haageana
 haagenii
+haastii
 habenarina
 habirshawii
 habra
 habrantha
 habrophyllus
 habrus
 hackeli
@@ -14551,14 +14889,16 @@
 haemantha
 haemanthum
 haemastoma
 haematica
 haematina
 haematites
 haematocephalus
+haematococca
+haematococcum
 haematodes
 haematommatum
 haematommona
 haematopus
 haematospermum
 haematospermus
 haematostachya
@@ -14589,14 +14929,15 @@
 hakeaefolia
 hakeaefolius
 hakeaeformis
 hakeicola
 hakeifolia
 hakeifolius
 hakeiformis
+hakeigena
 hakeodes
 hakeoides
 hakgallae
 hakonensis
 halata
 halei
 halepense
@@ -14628,14 +14969,15 @@
 halocarpa
 halocnemoides
 halodes
 halodytes
 halogenea
 halonia
 halonioides
+halopetalus
 halophila
 halophilicum
 halophilicus
 halophilioides
 halophilum
 halophilus
 haloragoides
@@ -14713,23 +15055,25 @@
 haplophylla
 haplophyllus
 haplorrhiza
 haplosciadea
 haplosciadia
 haplostemona
 hapsiphorus
+haptoclada
 haptocladus
 haptosporus
 haptotyla
 harae
 harcusiana
 hardenbergiae
 hardeniana
 hardmaniana
 hardyi
+harfordiae
 hariolorum
 hariotii
 harmala
 harmandiana
 harmandii
 harmanii
 harmannii
@@ -14770,15 +15114,14 @@
 hassallii
 hassellii
 hasseltii
 hasskarliana
 hassleriana
 hasta
 hastata
-hastata x stellulata
 hastatistipula
 hastatum
 hastatus
 hastieana
 hastiferum
 hastiferus
 hastifolia
@@ -14818,14 +15161,16 @@
 hayi
 haynaldii
 haysomii
 haywardiana
 haywardii
 haywardiorum
 hazeliae
+hazeniae
+healeyae
 healeyi
 healiana
 heardense
 heardensis
 heardii
 hearnii
 heatheriana
@@ -14853,22 +15198,22 @@
 hedleyi
 hedraiandra
 hedraiantheroides
 hedraiophylla
 hedraiophyllum
 hedycaryae
 hedychioides
+hedylamarr
 hedypnois
 hedysaroides
 heimansioides
 heimerlianum
 heimii
 heinari
 heinarii
-heinemanni
 heinemannii
 heintzelmaniana
 heironymi
 heisteria
 heleios
 helenae
 heleniae
@@ -14878,26 +15223,29 @@
 helferi
 heliantha
 helianthemi
 helianthemifolia
 helianthemifolium
 helianthemoides
 helianthi
+helianthicola
 helicandra
 helichrysantha
 helichrysi
 helichrysicola
 helichrysoides
 helichyrsodes
 helichyrsoides
 helicoides
 heliconiae
+helicoobliqua
 helicophylla
 helicophyllum
 helicosporum
+helicovinosa
 helidonica
 helikoides
 heliogiton
 heliophila
 heliophilus
 helioscopia
 heliosperma
@@ -14939,14 +15287,15 @@
 hemibapha
 hemibaphus
 hemibrunnea
 hemicardia
 hemicarpa
 hemicarpus
 hemichiton
+hemichrysus
 hemicyclodes
 hemicycloides
 hemicyclus
 hemiderma
 hemigenioides
 hemigenoides
 hemiglauca
@@ -14992,17 +15341,17 @@
 henryae
 henryi
 henryi x torelliana
 henshallii
 hensseniae
 henssenianus
 hepatica
-hepaticaefolia
-hepaticaefolium
 hepaticicola
+hepaticifolia
+hepaticifolium
 hepaticolor
 hepaticum
 hepaticus
 hepatochrous
 hepatotricha
 hepatotrichus
 heppii
@@ -15010,14 +15359,15 @@
 heptactis
 heptadactyla
 heptadactylus
 heptagona
 heptanthera
 heptaphylla
 heptaphyllum
+heptaseptatum
 heptemerus
 heptiflorum
 heptoneuron
 heraldense
 herbacea
 herbaceous
 herbaceum
@@ -15071,14 +15421,15 @@
 hesperidearum
 hesperidiiformis
 hesperidum
 hesperis
 hesperium
 hesperius
 hesperonotos
+hesseae
 heteracanthum
 heterandra
 heterandrum
 heterantha
 heteranthera
 heterantherus
 heteranthum
@@ -15126,14 +15477,15 @@
 heterophylla
 heterophylloides
 heterophyllum
 heterophyllus
 heterophyllus x meraukensis
 heterophyllus x splendens
 heteropleura
+heteropoda
 heteropodium
 heteropogonicola
 heteropogonis
 heteropogonis-contorti
 heteroporus
 heteroptera
 heteropus
@@ -15143,14 +15495,15 @@
 heterospora
 heterosporum
 heterosporus
 heterosticha
 heterostichum
 heterostriatum
 heterotricha
+hetheringtonii
 hetherophyllus
 hetieri
 heufleri
 heuflerii
 heveanensis
 hewardiana
 hewsoniae
@@ -15228,14 +15581,15 @@
 hildebrandii
 hildebrandtii
 hildebrandtioides
 hilderbrandii
 hilleana
 hillebrandi
 hillebrandii
+hilli
 hilliana
 hilliana x stellaticeps
 hillianum
 hillianus
 hillii
 hillii x parvifolius
 hillmanii
@@ -15245,14 +15599,15 @@
 hincksiae
 hindii
 hindii (Coveny 9906)
 hindmarchi
 hindmarchii
 hindsii
 hinnulea
+hinnuleum
 hinnuleus
 hinsbyi
 hippocastanum
 hippoglossa
 hippomanica
 hippopala
 hippoperoides
@@ -15339,16 +15694,16 @@
 hoipolloi
 holathera
 holcocarpa
 hollandiae
 hollandica
 hollandicus
 holleae
+holleanus
 hollenbergii
-hollianus
 hollidayi
 hollrungii
 holmesii
 holmiense
 holocarpa
 holocarpum
 holochila
@@ -15368,17 +15723,17 @@
 holopogonius
 holoptera
 holopterum
 holorubella
 holoschoenus
 holosclerus
 holosericea
+holosericeae
 holosericeum
 holosericeus
-holospoda
 holosteoides
 holostyla
 holotricha
 holotrichum
 holroydi
 holroydii
 holsatica
@@ -15428,15 +15783,16 @@
 homophylia
 homopilatum
 homoplastica
 homoplasticus
 homoranthoides
 homosekikaica
 homothallicus
-homuncula
+homunculus
+honeywilliae
 hongkongensis
 hoodii
 hoogendorfii
 hoogendorpii
 hooglandii
 hookerana
 hookeranus
@@ -15463,14 +15819,15 @@
 hopperi
 hopperiana
 hopperianum
 hopsonii
 hopwoodi
 hopwoodii
 hopwoodii x dixonii
+horakii
 horburyanum
 hordacea
 hordeacea
 hordeaceum
 hordeaceus
 hordei
 hordeiaustralica
@@ -15492,27 +15849,27 @@
 hornodermus
 hornschuchiana
 hornschuchianum
 hornschuchii
 hornseyi
 horologicalis
 horologium
-horrens
 horrescens
 horricomis
 horrida
 horridula
 horridulum
 horridum
 horridus
 horrifolia
 horsfallii
 horsfieldiana
 horsfieldii
 hortense
+hortensiae
 hortensis
 hortii
 hortiorum
 hortoniae
 hortorum
 hortulanum
 hortulanus
@@ -15530,14 +15887,15 @@
 houghtonii
 houseana
 houstonianum
 hoveae
 hoveaefolia
 hoveifolia
 hoveoides
+howardiae
 howardii
 howatharra
 howeana
 howeanum
 howeanus
 howei
 howei-insulae
@@ -15548,25 +15906,28 @@
 howettiana
 howii
 howinsula
 howitti
 howittiana
 howittii
 hteroneura
+huamulaniae
 hubbardiana
 hubbardianum
 hubbardii
 hubbsii
 huberana
 huberi
 huberiana
 hubregtseorum
+huegeli
 huegeliana
 huegelianum
 huegelii
+hueglei
 huerlimannii
 hugeliana
 hugelii
 hughani
 hughanii
 hughesii
 huismanii
@@ -15615,14 +15976,15 @@
 huronense
 hursthousei
 hurteri
 husemanii
 husseyana
 husseyanum
 hustedtii
+hustoniae
 hutchinsiae
 hutchinsioides
 hutonii T. Koyama
 huttensis
 hutti
 huttii
 huttoni
@@ -15634,15 +15996,14 @@
 hyacinthi
 hyacinthiflora
 hyacinthiflora-candidissima
 hyacinthoides
 hyalacanthum
 hyalina
 hyalinescens
-hyalinolimbata
 hyalinolimbatum
 hyalinum
 hyalinus
 hyaloneura
 hyaloneurum
 hyalosperma
 hyalospermum
@@ -15699,23 +16060,23 @@
 hylandiana
 hylandii
 hylobroma
 hylonoma
 hylonomum
 hymenachne
 hymenena
+hymenidermum
 hymenocallidicola
 hymenocarpa
 hymenocarpum
 hymenocladioides
 hymenocraspedum
 hymenocystis
 hymenodonta
 hymenodontioides
-hymenodontoides
 hymenoides
 hymenonema
 hymenophylla
 hymenosepalus
 hymenotheca
 hymenothecum
 hynesiana
@@ -15723,14 +16084,15 @@
 hyophilaceum
 hyophilus
 hypacanthum
 hypandra
 hypargyrea
 hyparrheniae
 hypata
+hypatia
 hypelytroides
 hypenantion
 hyperborea
 hyperelloides
 hyperellum
 hyperellus
 hypericifolia
@@ -15738,17 +16100,22 @@
 hypericina
 hypericoides
 hypericorum
 hyperion
 hyperleptalea
 hypermeces
 hypernota
+hyperommae
 hyperopta
 hyperostigma
+hyperparasiticum
 hypersporella
+hyphopodioides
+hypipamee
+hypipameeum
 hypipamensis
 hypispermis
 hypneoides
 hypni
 hypnodelphus
 hypnoides
 hypnorum
@@ -15859,27 +16226,29 @@
 ignescens
 igniaria
 igniarius
 ignobilis
 ignorabilis
 ignorata
 ignota
+iiodochrous
 ileticos
 ilex
 ilicifolia
 ilicifolium
 ilicifolius
 ilicina
 ilicincola
 ilicinum
 iliensis
 illecebroides
 illecebrosa
 illegitimus
 illiberalis
+illicifolia
 illicifolium
 illinita
 illinitus
 illita
 illitus
 illota
 illotus
@@ -15893,17 +16262,19 @@
 ilopangoensis
 imahorii
 imbecilla
 imbecille
 imbecillis
 imberbe
 imberbiflora
+imberbifolia
 imberbis
 imbricata
 imbricatula
+imbricatulum
 imbricatum
 imbricatus
 imitans
 imitatricoides
 imitatrix
 imlayensis
 immaculata
@@ -15916,14 +16287,15 @@
 immersella
 immersicans
 immersum
 immersus
 immixta
 immutabilis
 immutata
+impar
 imparile
 imparilis
 impatiens
 impatientis
 impendens
 impensa
 imperatae
@@ -15938,14 +16310,15 @@
 imperialis
 imperiosus
 impervia
 impetiginosa
 impetiginosus
 implana
 implexa
+implexae
 implexicoma
 implexum
 implexus
 implicata
 implicatum
 implicatus
 impolita
@@ -16104,14 +16477,15 @@
 indigoticoumbrinum
 indigotinum
 indira
 indistincta
 indistinctum
 indivisa
 indivisus
+indooroopillyensis
 inducta
 indumenta
 induplicata
 indurata
 induratum
 induratus
 indusiata
@@ -16159,14 +16533,15 @@
 inflexus
 informe
 infossum
 infracorticata
 infractum
 infractus
 inframediana
+infrapurpureum
 infrequens
 infundibulare
 infundibularis
 infundibuliforme
 infundibuliformis
 infusca
 infuscatulum
@@ -16198,14 +16573,16 @@
 innexa
 innominata
 innovans
 innoxia
 innoxium
 innubum
 innumera
+innumerum
+innuopurpureus
 inobvia
 inodora
 inodorum
 inodorus
 inolens
 inophloea
 inophloia
@@ -16230,14 +16607,15 @@
 inscripta
 insculpta
 insculptum
 insculptus
 insecticida
 insectifer
 insectifera
+insectum
 inselbergia
 insensitivum
 inserata
 inserta
 insidiosa
 insidiosum
 insidiosus
@@ -16272,14 +16650,15 @@
 insulanemorecincta
 insulare
 insulari-sylvatica
 insularicola
 insularis
 insularis x stigmatosus
 insularum
+insulinativitatis
 intactilis
 intangenda
 intangendus
 integer
 integerimum
 integerrima
 integerrimum
@@ -16298,15 +16677,14 @@
 integrum
 interanea
 interaneum
 intercalaris
 intercedens
 intercepta
 interceptus
-interhiascens
 interiore
 interioris
 interjacens
 interjecta
 interjectum
 interjuncta
 interlamellare
@@ -16388,16 +16766,18 @@
 inulifolium
 inuncta
 inundata
 inundatum
 inundatus
 inusta
 inutilis
+invadens
 invaginata
 invermaium
+inverness
 inversa
 inversiflorum
 inversum
 inversus
 investe
 investiens
 investita
@@ -16423,27 +16803,27 @@
 iodoformis
 iodolens
 iodostachys
 ioeca
 iogyna
 ionae
 ionantha
+ionocaulis
 ionoglossum
 ionthocarpa
 iophyta
 iotanum
 ipereniae
 iphthima
 ipsviciensis
 irbyana
 irbyi
 irbyiana
 ireneae
 iria
-irianense
 irianensis
 iridana
 iridescens
 iridiaustralis
 iridifolia
 iridifolium
 iridifolius
@@ -16463,35 +16843,37 @@
 irrigata
 irrigua
 irriguum
 irriguus
 irritabilis
 irritans
 irrorata
+irroratae
 irroratum
 irrubescens
 irukandjiana
 irukandjianum
 irvineae
 irvineanum
+irwinica
 isabelae
+isabellae
 isabellina
 isabellinus
 isantherum
 isantherus
 isatidea
 isatideum
 ischaemi
 ischaemi-rugosi
 ischaemoides
 ischaemum
 ischnobella
 ischnobellum
 ischnotricha
-ischyrhodon
 ischyrorhodon
 isdellensis
 iseilematis
 iseilematis-ciliati
 iseilematis-vaginiflori
 ishigakensis
 isiaca
@@ -16574,14 +16956,15 @@
 ixodiae
 ixoides
 ixoroides
 iyengarii
 iynx
 iyouta
 izonetae
+izuensis
 izunosimensis
 izziae
 jaagii
 jabiluka
 jabirabela
 jaboolum
 jacea
@@ -16608,14 +16991,15 @@
 jacquiniana
 jacquinii
 jacquinotii
 jaczewskii
 jadinianum
 jadinii
 jaernefeltii
+jagerae
 jagoanum
 jagonis
 jagorii
 jajaensis
 jalapa
 jamaicense
 jamaicense x mutabilis
@@ -16624,14 +17008,15 @@
 jamalinensis
 jambhiri
 jambolana
 jambolanum
 jamboolum
 jambos
 jambosoides
+jamesiae
 jamesiana
 jamesianum
 jamesii
 jamesiorum
 jamesoni
 jamesoniana
 jamesonianus
@@ -16678,46 +17063,48 @@
 jeanesii
 jeannerettii
 jebbiana
 jeckeri
 jecorinum
 jeffreyae
 jeleneckii
-jelineckii
 jelinkii
 jenensis
 jenisejense
 jenjiana
 jenkinsii
 jennerae
 jenneri
 jenniae
+jenningsiae
 jenolanensis
 jenseni
 jensenii
 jensziae
 jephcottii
 jerichoensis
 jerramungupensis
 jerseyana
 jesseni
 jessenii
 jessicae
+jetiae
 jibberdingense
 jibberdingensis
 jibbonense
 jibbonensis
 jillup
 jimberlanica
 jimiensis
 jingera
 jinksii
 jinungurdu
 jirovecii
 joadjense
+joanfreemaniae
 joanneae
 jobsonii
 jodoformicus
 joesmithii
 jofftii
 johannis
 johannis x discolor
@@ -16735,21 +17122,24 @@
 johnstonensis
 johnstoni
 johnstoniae
 johnstoniana
 johnstonianus
 johnstonii
 johnstonii x globulus x urnigera
+johnwestii
 johnwhinrayi
 johsonii
+joliotcurieae
 jolisiana
 jolla
-jollifei
 jolliffei
 jolliffii
+jollyi
+jonesi
 jonesianus
 jonesii
 jonkershoekensis
 jonquilla
 joshuae
 jourdani
 jourdanii
@@ -16766,15 +17156,14 @@
 jucunda x preissiana
 jucunda x pustula
 jucundum
 jucundus
 judaica
 judayi
 judithae
-judithiae
 judithiana
 juergensii
 jugalis
 jugicola
 jugispora
 juglandinus
 jugorum
@@ -16783,14 +17172,15 @@
 julacea
 julaceus
 juliana
 julianae
 julianeae
 julianetti
 julianettii
+juliannae
 julicaulis
 julietae
 julietiae
 julifera
 julifera x torulosa
 juliferum
 juliflora
@@ -16814,14 +17204,15 @@
 juncinum
 juncoides
 juncophila
 juncophilum
 juncta
 junctus
 jungermanniae
+jungermanniarum
 jungermannioides
 junghuhniana
 junghuhnii
 jungii
 jungquilianum
 juniperifolium
 juniperina
@@ -16925,50 +17316,54 @@
 karroo
 karroun
 karsense
 karsensis
 karsteniana
 karstenianum
 karstenii
+karstii
 kartana
+kartense
 kartzoffiana
 karvinskianum
 karvinskianus
 karwarrae
 karwinicola
 kashmiriana
 kaspar
 katabudjar
-katakata
 katatona
+katemensis
 katerae
 katerinae
 katjarra
 katjarranka
 kauaiense
 kauaiensis
 kaudernii
 kauki
 kavinae
 kaweaensis
 kayei
 kayseri
+keanei
 kearneyi
 keartlandi
 keartlandii
 kedumbensis
 keffordii
 kegelianus
 keigheryi
 keisak
 kekwickii
 kelanensis
 kelica
 kelleri
 kelloggii
+kelmanii
 kelsoi
 keltonii
 kempeana
 kempeanum
 kempei
 kempiana
 kemsleyi
@@ -16987,14 +17382,15 @@
 kennediicola
 kennedyae
 kennedyana
 kennedyensis
 kennedyi
 kennedyii
 kennyi
+kenpeggii
 kentiae
 kentrocaule
 kentropsidea
 keppelina
 keralensis
 keratinophila
 keratinophilum
@@ -17008,40 +17404,45 @@
 kerigomnensis
 kermadecense
 kermadecensis
 kermandii
 kermes
 kernianum
 keroblasta
+kerribeeensis
 kerrii
 kerryana
 kerryanum
 kershawii
 kerstenii
 kesselli
 kessellii
 kesslitzi
 kestervenii
 kestevenii
 kettlewelliae
 kevediana
 kevedianus
+kewarra
 keysii
 keysseri
 khasiana
 khasianum
 khatoonae
 khayae
 kiaeri
 kiaerii
 kiamae
+kiamaense
 kiambramensis
 kiamensis
 kiata
+kiataensis
 kiiensis
+kilaueaense
 kilcundaensis
 kilgourii
 kiliense
 killianii
 kilneri
 kilpanius
 kimberleyana
@@ -17051,19 +17452,22 @@
 kimberleyi
 kinahanii
 kincaidi
 kindelii
 kindyerracola
 kinearii
 kinghornii
+kingiae
 kingiana
 kingianum
 kingianum x speciosum
 kingianus
 kingii
+kinglakensis
+kingsiana
 kingsmilli
 kingsmillii
 kingwella
 kinneari
 kinnearii
 kioloensis
 kippistiana
@@ -17104,15 +17508,14 @@
 kleiniae DC.
 kleistobolus
 kleiwegii
 klementii
 klenzeana
 klenzeanus
 klinggraeffii
-klinggraefii
 klossii
 klotzchii
 klotzschii
 knappii
 kniepii
 knightiana
 knightianum
@@ -17125,32 +17528,35 @@
 koalae
 kochi
 kochiae
 kochiana
 kochianum
 kochii
 kochioides
+kochmanii
 kochummeniana
 koechlinii
 koehleri
 koenigii
 koerberiana
 koetjape
 kofoidi
 kofoidii
 koidzumii
+koikyennuruff
 koizumii
 kok-saghyz
 kolkwitzii
 kolleri
 kolya
 komarovianum
 kombolgiana
 kombolgiensis
 kondininensis
+kongii
 koniguruensis
 koningii
 konkinyerius
 konradii
 koobabbiensis
 koolgibberah
 koolpinensis
@@ -17159,27 +17565,30 @@
 koondrookensis
 koordana
 koordersii
 korewalensis
 korffense
 korijekup
 koronicarpus
-korothkevieziae
+kororoense
+korotkevicziae
 korra
 korrae
 korundensis
+korungensis
 kosciuskoa
 kosciuskoensis
 kosciuszkoensis
 kosteriana
 kotschyana
 kotschyanum
 kotschyi
 kouskosii
 kouytchense
+kovalevskayae
 kowenensis
 kowiense
 koyana
 koyanoides
 kozukensis
 kraehenbuehlii
 kraenzlinii
@@ -17197,23 +17606,25 @@
 kraussiana
 kraussianum
 kraussianus
 kraussii
 krebsiana
 krempelhuberi
 krempfii
+krichauffi
 krichauffianus
 krichauffii
+kriechauffi
 kriegeri
+kriegeriana
 krogiae
 krombholzii
 kroneanum
 kroombitensis
 kruseana
-kuborensis
 kuckuckii
 kuehliana
 kuehlianum
 kuehnii
 kuetzingiana
 kuetzingianum
 kuetzingii
@@ -17224,42 +17635,44 @@
 kumaoense
 kumaoensis
 kumaonense
 kumaonensis
 kumarinensis
 kumarlensis
 kumarlensis - salicola
+kumbius
 kumeraho
 kumpaja
 kunthiana
 kunthii
 kunzei
 kunzeoides
 kuranda
 kurandae
 kurandaensis
 kurandensis
 kurandica
 kurara
 kuringaiensis
 kuripanum
+kurodachikae
 kurramulla
 kurrangii
 kurriminensis
 kurzii
 kusanoi
 kusukusense
 kusukusensis
-kutubuensis
 kuurkacea
 kuwaitensis
 kuwanoanum
 kwangensis
 kwangsiense
 kwashotense
+kwolekiae
 kwongkanicola
 kybeanense
 kybeanensis
 kybeliona
 kydrense
 kydrensis
 kyeema
@@ -17355,25 +17768,28 @@
 lacor
 lacrimans
 lacryma
 lacryma-jobi
 lacrymabunda
 lacrymabundus
 lacrymans
+lacsalaria
 lactaria
 lactea
 lacteella
+lacteocoffeatum
 lacteola
 lacteolum
 lactescens
 lacteum
 lacteus
 lactiflora
 lactiflua
 lactifluus
+lactiglaucus
 lactinea
 lactineus
 lactivirens
 lactovirens
 lactuca
 lactucae
 lactucaefolia
@@ -17437,14 +17853,15 @@
 laeviuscula
 laeviusculum
 laeviusculus
 laevopinea
 lagaipensis
 lagapoides
 lagara
+lagarophylla
 lagarostrobi
 lagenacea
 lagenaceus
 lagenarioides
 lagenella
 lagenifera
 lageniforme
@@ -17474,14 +17891,15 @@
 lakei
 lalagoides
 lalitae
 lallemandii
 lamaense
 lamaensis
 lamaoensis
+lamarcheae
 lamarckiana
 lamarckii
 lambertiae
 lambertiana
 lambertianum
 lambertii
 lambica
@@ -17588,22 +18006,24 @@
 lanifolae
 laniger
 lanigera
 lanigeri
 lanigerum
 lanigerus
 lanipes
+laniscuspis
 lanosa
 lanosiflora
 lanosum
 lansdowneana
 lansium
 lantanifolia
 lantanoides
 lanterna
+lanternae
 lanternata
 lanternatus
 lantzschii
 lanuginophylla
 lanuginophyllum
 lanuginosa
 lanuginosum
@@ -17655,14 +18075,15 @@
 larkumii
 larnachiana
 larraeoides
 larreoides
 larsenii
 larvaespora
 larvale
+larvarum
 laseroni
 laseronii
 laserpitiifolium
 lasia
 lasiandra
 lasiandrum
 lasiangustata
@@ -17770,14 +18191,15 @@
 latisepaleum
 latisepalum
 latisepalus
 latisinensis
 latispicea
 latispinum
 latispora
+latisporus
 latisquamea
 latissima
 latissimum
 latissimus
 latitans
 latiuscula
 lativalve
@@ -17791,31 +18213,33 @@
 latrodectus
 latum
 latus
 latypizodes
 latzii
 laubatii
 laubertianum
-laucocanthum
 laudatus
 lauderi
 laufferianum
+lauracearum
 lauraceus
 laurana
 laurata
+laureata
 laurencei
 laurencia
 laurenciae
 laurencii
 laurentia
 laurentii
 laureola
 laureri
 laureriformis
 lauricassiae
+lauriflora
 laurifolia
 laurifolium
 laurifolius
 laurina
 laurinum
 laurinus
 laurocerasi
@@ -17846,14 +18270,15 @@
 lavata
 lavatum
 lavendocaeruleus
 lavendulense
 lavendulensis
 lavenia
 lawiana
+lawianus
 lawleri
 lawrenceana
 lawrencei
 lawrencella
 lawrencellum
 lawrencia
 lawrenciana
@@ -17896,20 +18321,20 @@
 leaiana
 leaianus
 leakeana
 leakeanum
 leari
 learii
 leathesiae
-leavis
 lebbeck
 lebbeckioides
 lebbek
 lebbekioides
 lebbekoides
+lebeliae
 lebelii
 lebourae
 lebouriae
 lecanantha
 lecannellieri
 lecanorae
 lecanorellum
@@ -17919,14 +18344,15 @@
 lechenaultiana
 lechenaultii
 lecideina
 lecideoides
 lecideola
 leclancheri
 lecomtei
+lecythiformis
 ledermanii
 ledermanniana
 ledermannii
 ledgeri
 ledgeriana
 ledgerii
 ledi
@@ -17947,14 +18373,15 @@
 leewenii
 lefevrei
 lefroyense
 lefroyensis
 lefvevrei
 leggeae
 leglerii
+legnephoricola
 legnota
 legnotum
 legrandii
 legumen
 leguminicola
 leguminum
 lehmanni
@@ -17970,28 +18397,29 @@
 leibleinii
 leichardi
 leichardiana
 leichardtiana
 leichardtii
 leichhardi
 leichhardii
-leichhardiitii
+leichharditii
 leichhardti
 leichhardtiana
 leichhardtianum
 leichhardtii
 leichhardtii (Cobar)
 leichhardtii x myoporoides
 leichhardtii x tessellaris
 leichtlinii
 leichtlinii x refracta
 leightoni
 leightonii
 leimonophilus
 leioblastus
+leiocalycis
 leiocalyx
 leiocarpa
 leiocarpella
 leiocarpum
 leiocarpus
 leiocaulis
 leiocaulon
@@ -18009,14 +18437,15 @@
 leioplaca
 leioplacella
 leioplacoides
 leiopyxe
 leiopyxis
 leiosperma
 leiospermum
+leiospora
 leiosporum
 leiosporus
 leiostachya
 leiostachys
 leiostachyum
 leiostyla
 leiotera
@@ -18107,16 +18536,16 @@
 lepidophyllus
 lepidopiloides
 lepidopoda
 lepidopodum
 lepidoptera
 lepidopus
 lepidorhiza
-lepidosperae
 lepidosperma
+lepidospermae
 lepidospermatis
 lepidospermoides
 lepidota
 lepidotum
 lepidotum - tuberculosum
 lepidotus
 lepidula
@@ -18176,14 +18605,15 @@
 leptocephalus
 leptoceras
 leptoceros
 leptochaete
 leptochila
 leptochilum
 leptochilus
+leptochlamys
 leptoclada
 leptoclados
 leptocladum
 leptocladus
 leptoclavia
 leptoclavium
 leptocylindrica
@@ -18308,14 +18738,15 @@
 lessoni
 lessonianus
 lessonii
 lesteri
 lesueurensis
 lesueurii
 leswellensis
+lethalis
 letrouitioides
 leucacanthum
 leucadendra
 leucadendri
 leucadendron
 leucaeana
 leucampyx
@@ -18417,29 +18848,29 @@
 leucostachya
 leucostachys
 leucostachyum
 leucostega
 leucostigma
 leucostoma
 leucostomoides
+leucotaenia
 leucothecium
 leucothelia
 leucothites
 leucothrix
 leucotos
 leucotricha
 leucotrichoides
 leucotrichum
 leucotylia
 leucoxantha
 leucoxanthum
 leucoxylon
 leuhmanni
 leuhmanniana
-leuhmannianum
 leuropoma
 levanderi
 levata
 levatum
 leve
 leveillei
 levicornua
@@ -18451,15 +18882,14 @@
 leviseta
 levispinum
 levispora
 levisporum
 levisporus
 levringii
 levynsiana
-lewellinae
 lewellini
 lewelliniae
 lewellinii
 lewisense
 lewisensis
 lewisiae
 lewisii
@@ -18509,39 +18939,41 @@
 lidii
 liebetruthii
 liebiana
 liebianum
 liebmannii
 lietzei
 lietzi
+liffmaniae
 liga
 ligans
 lightfootii
 lignatilis
+lignescens
 ligniaria
 lignicola
 lignicolor
 lignocarpa
 lignosa
 lignosus
 lignum-vitae
 lignyodes
-ligulaefolium
 ligulare
 ligularis
 ligulata
 ligulatulum
 ligulatum
 ligulatus
 ligulifolium
 ligustica
 ligusticum
 ligustrifolia
 ligustrifolium
 ligustrina
+ligustrinae
 ligustrinum
 lii
 liisae
 lilacea
 lilaceolamellata
 lilaceolamellatus
 lilacina
@@ -18566,17 +18998,19 @@
 liliifolia
 liliifolium
 lilioasphodelus
 liliputana
 liliputanobryoides
 liliputanoincurvus
 liliputanum
+lillianiae
 lillipillensis
 lilliputiana
 lilliria
+lillirium
 lima
 limacis
 limata
 limatum
 limbata
 limbata vel aff.
 limbatum
@@ -18604,14 +19038,15 @@
 limnophilum
 limnophylax
 limon
 limonella
 limonelle
 limoni
 limonia
+limoniforma
 limoniformis
 limonis
 limonisporus
 limonius
 limosa
 limosella
 limosellae
@@ -18647,16 +19082,18 @@
 lindleyi
 lindoniana
 lindsaea
 lindsayana
 lindsayanum
 lindsayoides
 lindseyana
+linear
 lineare
 lineare x rupestre
+linearefolium
 linearifolia
 linearifolia 'Unassigned 1' population (Angourie)
 linearifolia 'Unassigned 2'
 linearifolia 'Unassigned 3'
 linearifolia 'Unassigned 7'
 linearifolia 'race l' (Eyre Peninsula form)
 linearifolia 'race m' (Kangaroo Island form)
@@ -18672,15 +19109,14 @@
 lineariloba sp. B
 lineariloba sp. C
 lineariloba sp. D
 lineariloba sp. E
 linearioides
 linearis
 linearis x amygdalina
-linearis x compactus
 linearis x heterophylla
 linearis x planifolia
 linearoides
 lineata
 lineatoscaber
 lineatum
 lineatus
@@ -18701,21 +19137,21 @@
 linguiformis
 lingula
 lingulata
 lingulatus
 lingulifera
 linguus
 liniae
+linicola
 liniflora
 liniflorum
 linifolia
 linifolium
 linifolius
 linkii
-linkolae
 linnaeanum
 linnaei
 linnaeoides
 linneanum
 linnei
 linoides
 linophylla
@@ -18745,19 +19181,19 @@
 lissanthoides
 lissocarpa
 lissocarpha
 lissocarpus
 lissopleura
 lissosperma
 listeri
+litchiicola
 lithgowiae
 lithobius
 lithocola
 lithophila
-lithophilioides
 lithophiloides
 lithophilum
 lithophilus
 lithosperma
 lithospermoides
 lithospermum
 lithospermus
@@ -18779,14 +19215,15 @@
 littoralis x thalassoscopica
 littorea
 littorea x racemosa
 littoreum
 littoreus
 littoricola
 lituana
+lituanus
 liukiuensis
 livea
 liversidgei
 livida
 lividescens
 lividocarpa
 lividocinerea
@@ -18836,24 +19273,27 @@
 lobulata
 lobulatum
 lobuliflora
 lobuliflorum
 localis
 lochae
 lochiae
+lochii
 lockyeri
 loculata
 loculatus
 locusta
+loddigesi
 loddigesii
 loddigessii
 loderi
 lodgeana
 loeflingia
 loeflingiae
+loeflingii
 logaltyensis
 loganiacea
 loganii
 loganioides
 loganobaccus
 loganubaccus
 logiense
@@ -18903,14 +19343,15 @@
 longibractea
 longibracteata
 longibracteatum
 longibracteolata
 longibracteolatum
 longicarinata
 longicarpa
+longicatenatum
 longicauda
 longicaudata
 longicaudum
 longicaudus
 longicaulis
 longiceps
 longiciliata
@@ -18928,15 +19369,14 @@
 longicomum
 longicor
 longicorne
 longicornis
 longicornu
 longicurva
 longicurvum
-longicuspes
 longicuspis
 longidens
 longifimbriata
 longifissus
 longiflora
 longiflorum
 longiflorus
@@ -18950,15 +19390,14 @@
 longiloba
 longilobum
 longilumna
 longinode
 longinqua
 longinquus
 longinum
-longinus
 longior
 longipalea
 longipedata
 longipedicellata
 longipedicellatum
 longipedunculata
 longipedunculatum
@@ -18967,26 +19406,28 @@
 longipetalum
 longipetalus
 longipetiolata
 longipetiolatus
 longiphialidis
 longiphyllodinea
 longiphyllodineum
+longipila
 longipilosa
 longipilum
 longipilus
 longipinna
 longiracemosa
 longiradiatum
 longirostrata
 longirostrata x propinqua
 longirostratum
 longirostre
 longirostris
 longirostrum
+longirostrus
 longiscapa
 longiscypha
 longiscyphum
 longisepala
 longisepalum
 longiseta
 longisetacea
@@ -19021,24 +19462,24 @@
 longistipulis
 longistipulus
 longistriata
 longistyla
 longistylis
 longistylum
 longistylus
-longithecium
-longithecum
+longitheca
 longituba
 longitubea
 longitubum
 longitubus
 longitudinale
 longitudinalis
 longivalve
 longivalvis
+longmaniae
 longmanii
 longula
 longum
 longus
 lonicerodes
 loniceroides
 lopadii
@@ -19088,18 +19529,21 @@
 lotica
 lotifolia
 lotoides
 lotus
 loudoni
 loudonii
 louiseana
+louisecottisiae
+louisemackiae
 louisiana
 louisianica
 louisii
 loureiri
+lovelaceae
 lovellae
 lovelliae
 lovenii
 lowanense
 lowanensis
 lowei
 lowi
@@ -19135,23 +19579,25 @@
 lucida x macleayi
 lucidendroides
 lucidula
 luciduloides
 lucidulus
 lucidum
 lucidus
+lucifera
 lucifuga
 lucorum
 lucrusmiana
 luculenta
 lucyi
 ludens
 ludibunda
 ludoviciana
 ludovicianus
+ludwigianum
 ludwigii
 luehamanni
 luehmanii
 luehmanni
 luehmanniana
 luehmanniana x obstans
 luehmannianum
@@ -19229,16 +19675,18 @@
 luteoalbus
 luteoaurantiaca
 luteoaurantiacum
 luteoaurantium
 luteoaurantius
 luteobadia
 luteobadium
+luteobrunnea
 luteobrunneum
 luteobubalina
+luteobulbosa
 luteociliata
 luteocilium
 luteocincta
 luteocinctum
 luteocollum
 luteoconica
 luteocontextus
@@ -19249,24 +19697,26 @@
 luteolovelata
 luteolum
 luteolus
 luteonitens
 luteonitidus
 luteonotata
 luteoolivaceus
+luteorubrus
 luteosa
 luteostirpata
 luteoumbrina
 luteoumbrinus
 luteoviridis
 lutescens
 lutetiana
 luteum
 luteus
 luticola
+lutiteana
 lutosa
 lutosis
 lutosus
 luttrellii
 lux
 luxatum
 luxurians
@@ -19337,14 +19787,15 @@
 lythropsidis
 m'kayi
 mabacea
 mabellae
 mabelliae
 macachin
 macadamiae
+macalata
 macalpineana
 macalpineanum
 macalpinei
 macalpini
 macalpinianum
 macarangae
 macarthuri
@@ -19388,40 +19839,45 @@
 maceratus
 macfarlanei
 macgillivraei
 macgillivrayi
 macginnisii
 macgregorii
 machardiana
+machiavelliana
 machinii
 macilenta
 macilentum
 macilentus
 macilwraithense
 macilwraithensis
 macilwraithianum
+macintoshii
 macintyrei
 macintyrii
 macivorii
 mackaviense
 mackaviensis
 mackayense
 mackayensis
 mackayi
 mackeeanum
+mackellarae
 mackenziei
 mackenzii
+mackerrasiae
 mackeyana
 mackeyanum
 mackibbini
 mackibbinii
 mackinlayi
 mackinnoniana
 mackinnonianum
 mackintii
+mackintyi
 mackliniana
 maclanniae
 maclayana
 maclayanum
 macleanum
 maclearii
 macleayae
@@ -19443,17 +19899,17 @@
 maconochie
 maconochieana
 maconochieanum
 maconochiei
 macoorai
 macooraia
 macounii
-macowani
 macowanii
 macphersoni
+macphersoniae
 macphersonii
 macquariense
 macquariensis
 macquoidii
 macra
 macractenia
 macractenium
@@ -19476,16 +19932,18 @@
 macranthum
 macranthus
 macrarenula
 macrarthra
 macrathera
 macratherum
 macratherum x vaginiflorum
+macreana
 macrediana
 macredieana
+macredieanus
 macroblastum
 macrobotrya
 macrobotrys
 macrocalymma
 macrocalyx
 macrocarpa
 macrocarpoides
@@ -19507,14 +19965,15 @@
 macrocladum
 macroclavatum
 macroclavia
 macroclavium
 macrococcum
 macrococcus
 macrocurvum
+macrocystidia
 macrocystidium
 macrocystis
 macrodisca
 macrodonta
 macrodontum
 macrodontus
 macrodus
@@ -19616,21 +20075,23 @@
 macrourus
 macrozamia
 macrozamiae
 macrozyga
 macrum
 macsweeneyorum
 macta
+mactaggartii
 macula
 maculans
 maculare
 macularis
 maculata
 maculata x parvibracteata
 maculata x striata
+maculatissima
 maculatissimus
 maculatum
 maculatus
 maculiforme
 maculobulga
 maculosa
 maculosissima
@@ -19703,26 +20164,28 @@
 mahuianum
 maideni
 maideniana
 maidenianum
 maidenianus
 maidenii
 maierae
+mainiae
 maior
 maireana
 maireanae
 mairei
 maisonneuvei
 maisonneuvii
 maitlandi
 maitlandianum
 maitlandianus
 maitlandii
 maitlandii aciculiform variant
 majalis
+majewskii
 major
 majorae
 majoranaefolium
 majoranifolium
 majori
 majoriae
 majorii
@@ -19730,14 +20193,15 @@
 majus
 majuscula
 majusculum
 majusculus
 makarikariense
 makinoana
 makinoanum
+makinsoniae
 makinsonii
 maknoanum
 makoyana
 makoyanum
 makroklonion
 mala
 malabara
@@ -19785,39 +20249,43 @@
 malleatum
 malleeanus
 malleolacea
 malleus
 mallobolba
 malloclada
 mallocladum
+mallocyboides
+mallopoda
 mallota
 mallotoides
 malmei
 malthousei
 maluensis
 malus
 malvacea
 malvacearum
 malvaceus
 malvaefolia
 malvaefolium
 malvarum
 malvicola
+malvicolor
 malvifolia
 malvifolium
 malvina
 mamillana
 mamillaris
 mamillata
 mamillatum
 mamillatus
 mamillosa
 mamillosum
 mamillosus
 mammalis
+mammifera
 mammilla
 mammillatum
 mammillosus
 mammoidea
 mammosa
 mammosum
 mammosus
@@ -19889,24 +20357,27 @@
 marchantiorum
 marchesettioides
 marchica
 marchicum
 marcoana
 marcobotrys
 marduguru
+mareebaensis
 mareebensis
 marenitensis
 marescalchianum
 maretensis
 margacea
 margadinium
 margalefi
 margalefii
 margaretarum
+margaretflocktoniae
 margarethae
+margaretspencerae
 margarita
 margaritacea
 margaritaceum
 margaritaceus
 margaritae
 margaritatum
 margaritifer
@@ -19921,58 +20392,62 @@
 marginalis
 marginans
 marginata
 marginatta
 marginatum
 marginatus
 marginellum
-marginellus
 marginestriata
 marginifera
 marginiflexa
 marginulata
 mariae
 mariae-lebouriae
+mariamitchelliae
 mariana
 marianensis
 marianii
 marianna
 mariannensis
 mariannus
 marianthi
 marianum
 marianus
+mariehareliae
 mariei
 marielebourae
+marietelkes
 marifolia
 marilandica
 marina
+marinae
 marinospora
 marinum
 marinus
 marionense
 mariscus
 mariti
 maritima
 maritima (Hind 3092)
 maritimum
 maritimus
 maritinum
 marivelensis
+marjaniae
 marksiana
 marksii
 marliacea
 marliesiae
 marmelos
 marmorata
 marmoratum
 marmoratus
 marmorea
 marneffei
-marocana
+marneyi
 maroccana
 marquandii
 marradongense
 marramamba
 marrawalina
 marriottii
 marrubii
@@ -20006,22 +20481,29 @@
 martiniana
 martinicense
 martinicensis
 martinii
 martyana
 martyi
 maryae
+maryandersoniae
+maryelizabethiae
+maryellenpeartiae
+marykayhuntiae
 marylandica
+maryleeae
 maryonii
 mas
 maschalinus
 maschalocarpum
 masdevalliaceum
+masirevicii
 masliniana
 maslinianum
+maslinii
 masoni
 masoniae
 masonianum
 masonii
 massaicum
 massalongoi
 massariospora
@@ -20035,14 +20517,15 @@
 mastoidella
 mastoideum
 mastoideus
 mastophorizans
 mastopora
 mastoporum
 mastoporus
+mastotermitis
 mastothallina
 matanoensis
 matarankense
 mathewsii
 mathinnae
 mathinnicola
 mathuataense
@@ -20061,14 +20544,15 @@
 matthiolae
 mattiroloanum
 mattogrossensis
 matutina
 matutinum
 maugeana
 maunakeansis
+maundi
 maundii
 maura
 maurilabra
 mauritanica
 mauritanicus
 mauritiana
 mauritianum
@@ -20080,35 +20564,37 @@
 max
 maxgrayi
 maxillare
 maxillaris
 maxima
 maximum
 maximus
-maxweli
 maxwell
 maxwelli
 maxwellii
 mayae
 mayama
+maybankeae
 maydicum
 maydicus
 maydis
 mayeri
+mayi
 mayrhoferae
 mayrhoferi
 mays
 maytenifolia
 maytenifolius
 mazatlanense
 mazeliana
 mazlini
 mcalpinei
 mcclatchie
 mcclatchiei
+mcclintockiae
 mccomishii
 mccutcheonii
 mcdowalliana
 mcgillivrayi
 mcintyrensis
 mckieana
 mckiei
@@ -20117,14 +20603,15 @@
 mcnabbii
 mcnuttiana
 mcquoidii
 mea
 mearnsi
 mearnsii
 mearsii
+mebaldsii
 medeloides
 medeoloides
 media
 media - platyphylla
 mediale
 medialinermis
 medialis
@@ -20155,14 +20642,15 @@
 medulla-panis
 medullare
 medullaris
 medullosa
 medullosum
 medusa
 medusae
+medusoides
 medusula
 medusulina
 meeana
 meeboldii
 megacalyx
 megacantha
 megacanthum
@@ -20176,14 +20664,15 @@
 megadenia
 megadontus
 megaflora
 megaglomerulosa
 megaglomerulosum
 megaglossus
 megagonidia
+megahesperidea
 megalacantha
 megalantha
 megalanthum
 megalanthus
 megalocarpa
 megalocarpus
 megalocopa
@@ -20212,14 +20701,15 @@
 megalostegia
 megalotheca
 megalothecus
 megalotheles
 megalotis
 megalura
 meganotia
+megaocculta
 megaphlyctidioides
 megaphylla
 megaphyllum
 megaphyllus
 megapolitanum
 megapotamia
 megapotamica
@@ -20272,15 +20762,14 @@
 melaleucaphilus
 melaleucoides
 melaleucum
 melaleucus
 melaloma
 melambola
 melana
-melanacantha
 melananthum
 melancholicus
 melanema
 melanemum
 melanenta
 melanesica
 melaniceps
@@ -20313,16 +20802,16 @@
 melanophloia x normantonensis
 melanophloia x orgadophila
 melanophloia x persistens
 melanophloia x populnea
 melanophloia x whitei
 melanophloia x xanthoclada
 melanophloium
-melanophtalmum
 melanophthalma
+melanophthalmum
 melanopogon
 melanoporus
 melanoptera
 melanopum
 melanopus
 melanorrhiza
 melanosperma
@@ -20380,27 +20869,29 @@
 melinocarpa
 melinocaule
 melinoides
 meliolae
 melioloides
 melissifolia
 melissiodora
+melitenisis
 melitensis
 mellaria
 mellarium
 mellea
 melleicinctus
 melleobrunnea
 melleodora
 melleodorum
 melleum
 melleus
 mellina
 melliodora
 mellissii
+mellita
 mellorianum
 melo
 melobesioides
 melocarpa
 melodini
 melongena
 meloniformis
@@ -20417,35 +20908,38 @@
 membranicinctus
 membranifaciens
 membraniflorum
 membranifolia
 membranifolium
 membranifolius
 memoria-annae
+memorialis
 memphitica
 memphiticum
 menaiensis
 mendax
 mendellii
 meneghiniana
 meneghinii
 meneyae
 mengenensis
 meningiensis
+meniscoidea
 menisculus
 meniscus
 menispermacea
 menkeana
 mensalis
 mentagrophytes
 menthae
 mentiens
 menyanthicola
 menzeliae
 menzelii
+menziesi
 menziesiana
 menziesii
 meonantha
 meraukensis
 meraukensis x splendens
 merceri
 mercurialis
@@ -20455,14 +20949,15 @@
 meredithiae
 meredithiana
 merenia
 mereschkowskiana
 mereschkowskyi
 meriana
 meriania
+merianiae
 meridionale
 meridionalis
 meridithae
 meridonialis
 merikin
 merinthophora
 merinthophorum
@@ -20550,14 +21045,15 @@
 metcalfii
 metel
 meteleoides
 metelerkampiae
 meteloides
 meteori
 methoxymicareica
+methvenii
 methylbarbatica
 metrosideri
 metrosiderifolia
 metrosideros
 metulifer
 metuliferus
 metum
@@ -20584,27 +21080,27 @@
 micans
 micareoides
 michaelae
 michaeliana
 michaelii
 michaelis
 michelagoensis
+micheli
 micheliana
 michelianum
 michelianus
 michelii
 michelli
 michellii
 micheneri
 michieana
 michieanum
 michiei
 micholitzii
 michotii
-micklei
 micra
 micracantha
 micradenia
 micradenium
 micrairae
 micrairoides
 micramnia
@@ -20633,14 +21129,15 @@
 microcarpa
 microcarpa 'Adelaide Variant'
 microcarpa x ovata
 microcarpa x viridis
 microcarpella
 microcarpoides
 microcarpon
+microcarpos
 microcarpum
 microcarpus
 microcarya
 microcaryus
 microcephala
 microcephalum
 microcephalus
@@ -20703,17 +21200,17 @@
 micromorus
 micromyrtus
 micronesica
 micronesiense
 microneura
 microneurum
 micropachypoma
-micropachypomum
 micropetala
 micropetalum
+micropetata
 micropholis
 microphthalmum
 microphylla
 microphylla - rubioides
 microphyllina
 microphyllizans
 microphylloides
@@ -20824,14 +21321,15 @@
 millegrana
 millerae
 milleri
 milleriana
 millgar
 milligani
 milliganii
+millisiae
 milneana
 milnei
 milnerae
 milneri
 milnerii
 miltina
 miltinus
@@ -20849,19 +21347,21 @@
 mimosoides
 mimula
 mimuloides
 mimulum
 mimulus
 minahassae
 minarum
+minata
 mindanaense
 mindanaensis
 minderiana
 mindorense
 mindorensis
+miniaroides
 miniata
 miniatescens
 miniatocinctum
 miniatum
 miniatus
 miniglutinans
 minigwalica
@@ -20869,14 +21369,15 @@
 minima
 minimoides
 minimum
 minimus
 minispora
 minitula
 minniritchi
+minnsiorum
 minoensis
 minor
 minorata
 minormylittae
 minurioides
 minus
 minuscula
@@ -20900,35 +21401,38 @@
 minutirameum
 minutispora
 minutissima
 minutissimum
 minutissimus
 minutistipula
 minutoides
+minutoincanum
 minutoincanus
 minutula
 minutuliflora
 minutuliflorum
 minutulum
 minutulus
 minutum
 minutus
 minya
 minyma
+minysantha
 minyura
 minyura variant
 miqueli
 miqueliana
 miqueliana 'Mt Wellington form'
 miqueliana 'Typical form'
 miquelianum
 miquelii
 miquellii
 mira
 mirabile
+mirabiliaffinis
 mirabilis
 mirabilissima
 miraculosa
 miraculosum
 miraculosus
 miranda
 mirbeli
@@ -20936,14 +21440,15 @@
 mirbeliana
 mirbelianum
 mirbelii
 mirbelioides
 mireniana
 miriamae
 miriamiae
+miriciae
 mirificus
 mirramirildinum
 mirum
 mirus
 misaminensis
 miscella
 miscellus
@@ -20972,19 +21477,21 @@
 mitrata
 mitratum
 mitreola
 mitriformis
 mittagongensis
 mittenii
 mixta
+mixtilis
 mixtum
 mixtus
 miyabeana
 miyabeanus
 mjoebergii
+mnesitheae
 mniaroides
 mniatopodius
 mnioides
 mnoraifolius
 moabus
 mobergiana
 mobile
@@ -20994,26 +21501,26 @@
 modesta
 modestula
 modestulus
 modestum
 modestus
 moebii
 moebiusii
-moelkenboerii
 moelleri
 moelleriana
 moellerianus
 moesta
 moffatiana
 mogin
 mogrere
 mohii
 mohrii
 moirensis
 moirii
+mokarei
 mokusin
 molare
 molaris
 moldavica
 molesta
 molkenboeri
 molle
@@ -21120,14 +21627,15 @@
 monocystis
 monodon
 monogyna
 monogynum
 monoica
 monoicum
 monoicus
+monolina
 monopetala
 monopetalum
 monopetalus
 monophylla
 monophyllum
 monophyllus
 monoplocodes
@@ -21164,17 +21672,17 @@
 monspieliensis
 monstrosa
 monstrosita
 monstrosum
 monstrosus
 montagneana
 montagnei
-montaguei
 montana
 montana x recurva
+montanea
 montaneus
 montanum
 montanus
 montecolli
 montellicum
 montenegrensis
 montevidense
@@ -21231,14 +21739,15 @@
 mori
 morifolia
 morina
 morindae
 morindaefolia
 morindifolia
 moringa
+moriniae
 morinii
 morinum
 moriopsis
 moritziana
 moritzii
 morobensis
 moroides
@@ -21247,35 +21756,38 @@
 morphotype R2
 morphotype R3
 morphotype R4
 morphotype S
 morrallii
 morrisae
 morrisbyi
+morrisi
 morrisiae
 morrisiana
 morrisii
 morrisonensis
 morrisoni
 morrisoniana
 morrisonianus
 morrisonii
 morrissii
 morsa
 morsus-ranae
+morti
 mortii
 mortii x pugioniforme
 mortii x pugioniformis
 mortii x schoeninum
 mortoni
 mortoniana
 mortonii
 morula
 morulus
 morum
+morwellensis
 mosambicense
 mosambicensis
 moscaliana
 moscalianus
 moscalii
 moscata
 moschata
@@ -21372,14 +21884,16 @@
 mulligana
 mulliganensis
 mullinense
 mulpu
 multiacida
 multiamentula
 multiarticulata
+multiaustraliensis
+multiaustrocylindrica
 multibracteata
 multicapsulus
 multicarpelatus
 multicaule
 multicaulis
 multicaulis A
 multicaulis B
@@ -21393,14 +21907,15 @@
 multiclavia x pulchra
 multiclavium
 multicolor
 multicolorata
 multicorne
 multicostata
 multiculmis
+multicurvula
 multicuspidata
 multicuspidatum
 multidentatum
 multifaria
 multifera
 multifida
 multifidum
@@ -21429,22 +21944,25 @@
 multilacera
 multilaceroides
 multilamellata
 multilineata
 multiloba
 multilobatus
 multilobus
+multimorphosa
+multinanosoma
 multinerve
 multinervia
 multinervis
 multinervosa
 multinoda
 multinode
 multinodulosum
 multinodum
+multinucleata
 multiordinatum
 multipartita
 multipartitum
 multipedata
 multipedes
 multipenna
 multipennus
@@ -21478,16 +21996,18 @@
 multispina
 multistipulosa
 multistipulosum
 multistriata
 multistriatum
 multituberculatum
 multivalvis
+multivinosa
 multivora
 munda
+mundagurra
 mundak
 mundata
 mundijongensis
 mundroola
 mundula
 mundulum
 mungo
@@ -21537,23 +22057,23 @@
 murrayana
 murrayanum
 murrayanus
 murrayi
 murrumboensis
 musaceum
 musae
+musae-banksii
 musaiaensis
 musaria
 musarum
 muscae
 muscaria
 muscarius
 musci
 muscicola
-muscicolum
 musciforme
 musciformis
 muscigena
 muscipula
 muscoides
 muscolignosa
 muscorum
@@ -21622,47 +22142,61 @@
 myriantha
 myrianthum
 myrianthus
 myricaefolia
 myricaefolius
 myricifolius
 myricoides
+myriella
+myrioauris
+myrioaustraliensis
 myriobotrya
 myriocarpa
 myriocarpum
 myriocarpus
 myriocephala
 myriocephalum
 myrioclada
 myriocladum
 myriocladus
 myriococcum
 myriocodon
 myriocystum
 myriodesmae
+myrioeuonymi
+myriofusiclava
+myriofusoidea
+myriohesperidea
+myriolilacina
 myrioloba
 myriomera
+myriomuscula
+myrionamibica
+myrionanosoma
+myrioobliqua
 myriophylla
 myriophylloides
 myriophyllus
 myriopoda
 myrioporum
+myriopseudoregalis
 myriotrema
 myriotricha
 myriotylum
 myrmecoa
 myrmecophila
 myrmecophilum
 myrsinifolia
 myrsinitis
 myrsinocarpa
 myrsinodendron
 myrsinoides
 myrtacea
 myrtacearum
+myrtaceicola
 myrticola
 myrtifolia
 myrtifolium
 myrtifolius
 myrtiformis
 myrtillifolia
 myrtillina
@@ -21680,34 +22214,39 @@
 myurium
 myuros
 myurus
 myxa
 myxobasis
 naaykensii
 nabiacense
+nabiacensis
 nabonnandi
 nabonnandii
 naccarioides
 naegeliana
 naegelianum
 naegelii
 naevosa
 nagarensis
 nagasakiense
 nahui
+naiawu
 nakamurae
 nakamurai
 nakanisheana
 nakanishikii
 namadgi
 namadgiense
 namadgiensis
 nana
 nanana
 nanandra
+nanangensis
+nancybirdwaltoniae
+nancywakeae
 nandewarense
 nandewarica
 nanglei
 nannengae
 nanoarcuata
 nanobolax
 nanocarpa
@@ -21723,32 +22262,35 @@
 nanolineata
 nanolineatus
 nanopennatum
 nanopetala
 nanophylla
 nanopravissima
 nanopyxis
+nanosperma
 nanospora
 nanosporum
 nanostellata
 nanosubulata
 nanotorquescens
 nanotortuosa
 nanournigerum
 nanseni
 nanteuilii
 nanum
 nanus
+naomipierceae
 napalansis
 napalensis
 napiformis
 napipes
 napobrassica
 napus
 naqsii
+naracoortensis
 naranjus
 narayanaraoana
 narcissi
 narcissus
 nardiensis
 nardoides
 nardu
@@ -21790,20 +22332,23 @@
 naviculoideum
 naviculum
 navisporus
 nealensis
 neapolitana
 neapolitanum
 neapolitanus
+neatei
 nebularis
 nebulata
 nebulobrunneus
+nebuloides
 nebulosa
 nebulosus
 necator
+neclivorem
 necopinata
 necrophylla
 necrophyllum
 nectandrae
 nectarina
 nectrioideum
 neergaardii
@@ -21868,43 +22413,48 @@
 neobunyana
 neocaledonica
 neocaledonicum
 neocaledonicus
 neocalyptrata
 neocambrica
 neochilus
+neocomma
 neoconglomerata
 neocoprophila
 neoculata
 neocyanescens
+neocylindrospora
 neocymosa
 neodamaziana
 neodelisei
+neodilophospora
 neodissecta
+neofalcata
 neofoliata
 neoglaber
 neoglabrans
 neogoodenia
 neogracilis
 neoguineensis
 neohalonia
 neohibernicum
-neohollandica
 neohollandicum
 neohollandicum x medium
 neohoweana
 neoisidiata
 neokyrea
 neolenticula
 neoleucomelaena
 neolitseae
 neomajor
 neomexicana
 neomongaensis
+neomurina
 neonubila
+neoorbicularis
 neopertusariiformis
 neopolyphylla
 neopommeranica
 neopropagulifera
 neopustulatum
 neoqueenslandica
 neoquintaria
@@ -21915,14 +22465,15 @@
 neospectabile
 neotinctina
 neotriconica
 neotricosa
 neotropica
 neotucsonensis
 neotunicatum
+neowalkeri
 neozelandica
 neozelandicum
 nepalense
 nepalensis
 nepalica
 nepeanensis
 nepeta
@@ -21945,16 +22496,18 @@
 nereifolium
 neriella
 neriifolia
 neriifolium
 neriifolius
 neriiformis
 nermula
+nernsti
 nernstii
 nerrenensis
+nerrigaensis
 nerrigensis
 nertera
 nerterioides
 nerteroides
 nervata
 nervifolia
 nervilemma
@@ -21977,15 +22530,14 @@
 nesophila x spirorbis
 nesophilum
 nesophilus
 nesophylla
 nesophyllum
 nessorhina
 nestor
-neuhoffii
 neumanni
 neumanniana
 neumannii
 neupokojewi
 neurachnis
 neurachnoides
 neurivalvis
@@ -22004,21 +22556,25 @@
 newbeyana
 newbeyi
 newcastlianum
 newelliana
 newlingii
 newmanii
 newmannii
+newnesense
 newportii
+newtonturnerae
 nexosa
 nexosum
 neypergiana
+ngayawang
 nguba
 nhatragensis
 niagarae
+niallkiyoshii
 niaouli
 nicaeense
 nicaeensis
 nicaraguense
 nicholasii
 nicholi
 nicholii
@@ -22044,14 +22600,15 @@
 niedenzuana
 niei
 nieppergiana
 nietneri
 nigella
 nigellum
 niger
+nigeriana
 nigerrimus
 nightingaleae
 nigra
 nigrae-silvae
 nigraoleosa
 nigrapicus
 nigrata
@@ -22079,15 +22636,14 @@
 nigrocinctum
 nigrocinerea
 nigroclavata
 nigroflavum
 nigroflavus
 nigrofusca
 nigrolaccatus
-nigromarginata
 nigromontana
 nigromucronata
 nigropedata
 nigrorufa
 nigrosclerotium
 nigroseptatum
 nigroviolaceus
@@ -22116,15 +22672,14 @@
 niphodes
 niphopedium
 niphophila
 niphophilum
 niphophilus
 niphophloia
 nipponica
-nipponicum
 nirimbii
 niruri
 nissolia
 nitchaga
 nitella
 nitellarum
 nitens
@@ -22193,14 +22748,15 @@
 nodatum
 nodatus
 nodicoma
 nodiferum
 nodiflora
 nodiflorum
 nodiflorus
+nodorum
 nodosa
 nodosum
 nodosus
 nodularia
 nodularis
 nodulifera
 nodulifolium
@@ -22219,19 +22775,20 @@
 nonda
 nonparaphysata
 nonreagens
 nonscandens
 nonscriptus
 nonspecifica
 nontingens
+nooreniae
 noosaensis
 noosanus
+nootherensis
 norcapnodes
 norconvoluta
-norcrambidiocarpa
 nordstedtiana
 nordstedtianum
 nordstedtii
 nordtiana
 norfolkensis
 norfolkiana
 norfolkianum
@@ -22240,14 +22797,15 @@
 normalis
 normaloides
 normanbyana
 normanbyanum
 normanbyi
 normandina
 normanense
+normanensis
 normani
 normanii
 normantonensis
 normantonensis - persistens
 nornotatica
 nornotaticum
 norpraegnans
@@ -22275,20 +22833,25 @@
 notactites
 notarisii
 notata
 notatum
 notatus
 notelaeae
 notha
+nothescens
 notho-manihot
+nothoaprilis
+nothofagetorum
 nothofagi
 nothofagicola
 nothogeae
+nothopus
 nothorachodes
 nothostricta
+nothovinosa
 nothum
 nothus
 notiale
 notialis
 notibractea
 notochthona
 notochthonum
@@ -22315,24 +22878,21 @@
 novae-guineae
 novae-guineensis
 novae-hiberniae
 novae-hollandiae
 novae-seelandiae
 novae-semliae
 novae-valesiae
-novae-valisiae
 novae-walesiae
 novae-zealandiae
 novae-zeelandiae
 novae-zelandiae
 novaebritanniae
 novaeguineae
 novaehollandiae
-novaeseelandiae
-novaevalesiae
 novaezeelandiae
 novaezelandiae
 novazelandica
 novehollandiae
 novella
 novemnerve
 novi-belgii
@@ -22356,27 +22916,30 @@
 nubecula
 nubica
 nubicola
 nubicus
 nubigena
 nubila
 nubilis
+nubilosa
 nublingii
 nucifera
 nucipersica
 nuciseda
 nucisedus
 nucleata
 nucleatum
 nucula
 nuculastrum
 nuda
 nudata
+nudgee
 nudibaccatum
 nudibrachiatum
+nudicalycina
 nudicarpa
 nudicaule
 nudicaulis
 nudiflora
 nudiflorum
 nudipes
 nudiscapa
@@ -22392,14 +22955,16 @@
 nugentae
 nugentiae
 nugentii
 nulla
 nullanulla
 nullarborensis
 nullawarrensis
+nullicana
+nullicananum
 nullum
 nullumense
 nullumensis
 nullumiae
 numarium
 numerosa
 numinbahensis
@@ -22409,14 +22974,15 @@
 nummulariifolius
 nummularium
 nummularius
 nummulifolium
 nummuloides
 nunaginensis
 nungarinense
+nupera
 nuperrima
 nuperrimum
 nureliyum
 nurragi
 nutans
 nutrix
 nux-vomica
@@ -22470,30 +23036,33 @@
 oblanceoloideus
 oblata
 oblatiapicalis
 oblatum
 oblatus
 oblectans
 oblecythiformis
+obligomera
 oblimans
 oblinitum
 oblinitus
 obliqua
 obliqua x regnans
+obliquae
 obliqueberbe
 obliquiberbe
 obliquiberbis
 obliquicuspis
 obliquifolia
 obliquifolium
 obliquifolius
 obliquinervia
 obliquinervium
 obliquirostre
 obliquisepala
+obliquiseptatum
 obliquistigma
 obliquomucronatum
 obliquum
 obliquus
 oblitera
 obliterans
 obliterata
@@ -22514,33 +23083,33 @@
 oblongisporus
 oblongum
 oblongus
 obniger
 obovale
 obovalis
 obovata
-obovata x opposita
 obovata x parvifolia
 obovatifolia
 obovatum
 obovatus
 obovoidea
 obpyriformis
 obrienianum
 obrienii
 obscura
 obscurans
 obscurata
 obscuratum
 obscurecoccineus
+obscureogracile
 obscureorubeus
 obscureotenax
 obscurevirens
 obscurior
-obscurirete
+obscuriretis
 obscurum
 obscurus
 obseptum
 obsoleta
 obsoletum
 obsoletus
 obstans
@@ -22573,14 +23142,15 @@
 obtusidens
 obtusifida
 obtusiflora
 obtusiflorum
 obtusiflorus
 obtusifolia
 obtusifolia vel. aff.
+obtusifoliae
 obtusifolium
 obtusifolius
 obtusiloba
 obtusilobus
 obtusiplicatum
 obtusirameum
 obtusisepala
@@ -22603,18 +23173,18 @@
 occidentalis x B
 occidentalis x opposita
 occidentiaustralis
 occidentissima
 occidua
 occlusa
 occlusus
-occulata
 occulatum
 occulta
 occultans
+occultata
 occultiflora
 occultipetala
 occultiseta
 occultum
 occultus
 oceanica
 oceanicum
@@ -22640,15 +23210,14 @@
 ochraceum
 ochraceus
 ochrantha
 ochranthum
 ochreata
 ochreatus
 ochrocephala
-ochroceracea
 ochrochlora
 ochrochroa
 ochrochroum
 ochrocoleus
 ochrocrinitum
 ochrodigitula
 ochroflava
@@ -22682,16 +23251,19 @@
 ocreata
 ocreatus
 octaedricum
 octandra
 octandrum
 octandrus
 octo
+octoblephara
 octoblepharioides
 octoblepharum
+octoblepharus
+octocercocarpi
 octocorne
 octocornis
 octocostatus
 octodonta
 octodontum
 octofila
 octogibbosum
@@ -22704,37 +23276,41 @@
 octonarium
 octonarius
 octonervia
 octonervium
 octonum
 octopetala
 octophylla
+octoserpentina
 octosporum
 octotriginta
 octovalvis
 octoverrucosum
 oculata
 oculatum
 oculoides
 oculus-iridis
 ocymastrum
 ocymifolia
+odellii
 odgersii
 odiosa
 odiosum
 odocoileops
 odollam
 odonnellii
+odontata
 odontella
 odontites
 odontocalyx
 odontocarpa
 odontocarpum
 odontocarpus
 odontoclada
+odontoides
 odontolepis
 odontophyllum
 odontosoriae
 odontosperma
 odontospermum
 odora
 odorata
@@ -22745,21 +23321,22 @@
 odoratum Coastal Form
 odoratum Inland Form
 odoratus
 odorifer
 odorifera
 odorum
 odorus
+oecophyllae
 oederi
 oederoides
 oedineura
 oedipus
 oedithecium
 oedogonia
-oedogoniales
+oedogonioides
 oedogonium
 oelandicum
 oenanthum
 oenochila
 oenoplia
 oenopolia
 oenotheroides
@@ -22774,14 +23351,15 @@
 ogatae
 ogatai
 ogilvieanum
 ohiensis
 ohioense
 ohkuboana
 ohmeri
+ohnowa
 ohwii
 oiwakensis
 okamurae
 okamurai
 okaritana
 okaritanus
 olaefolia
@@ -22791,14 +23369,15 @@
 oldfiedii
 oldfieldi
 oldfieldiana
 oldfieldianum
 oldfieldianus
 oldfieldii
 oldhamii
+oldii
 oleae
 oleaefolia
 oleaefolium
 oleaginosa
 oleaginus
 oleander
 oleariae
@@ -22809,14 +23388,15 @@
 oleaster
 oleifera
 oleifolia
 oleifolium
 oleifolius
 olens
 oleoides
+oleoligni
 oleosa
 oleosum
 oleosus
 oleracea
 oleraceum
 oleraceus
 olgae
@@ -22877,16 +23457,18 @@
 oligotropha
 olitorius
 olivacea
 olivaceoalba
 olivaceoalbus
 olivaceobrunnea
 olivaceobrunneum
+olivaceoflava
 olivaceoflavidum
 olivaceoflavidus
+olivaceohinnulea
 olivaceolutea
 olivaceonigra
 olivaceoporus
 olivaceum
 olivaceus
 olivascens
 oliverana
@@ -22965,19 +23547,21 @@
 opegraphina
 opegraphoides
 operculariae
 opercularina
 operculata
 operculatum
 operculatus
+operculinae
 operculoides
 operta
 opertum
 ophelii
 ophiocephala
+ophiodiicola
 ophioglossa
 ophioglossifolius
 ophioglossoides
 ophioglossum
 ophiolithica
 ophiolithicum
 ophiolitica
@@ -23046,15 +23630,14 @@
 ordiana
 ordii
 ordinata
 ordinatum
 ordinifolia
 ordorata
 ordoratum Coastal Form
-oreadeoides
 oreades
 oreillyana
 oreillyanum
 oreina
 oreinoides
 orellana
 orenburgika
@@ -23083,25 +23666,27 @@
 ormocarpoides
 ormocarpum
 ormondi
 ormondii
 ornamentosum
 ornans
 ornata
+ornatipes
 ornatissimus
 ornatum
 ornatus
 ornithocephala
 ornithocephalum
 ornithocopreoides
 ornithogali
 ornithophora
 ornithopoda
 ornithopodioides
 ornithopodoides
+ornithopoides
 ornithopterae
 ornithorhynchi
 ornus
 oroboides
 oroflavum
 oroflavus
 orokonuiana
@@ -23157,20 +23742,22 @@
 oshanesii
 oshanesyana
 oshimensis
 osmera
 osmophila
 osmoxylon
 osmus
+osphranticarpa
 ossa
 osseoalba
 osseus
 ossicruentum
 osswaldi
 ostenfeldii
+ostentans
 osteocarpum
 osteospermi
 ostrea
 ostrearia
 ostrearius
 ostreata
 ostreatus
@@ -23376,37 +23963,37 @@
 pachystachyum
 pachystachyus
 pachystemon
 pachystomoides
 pachystylum
 pachytheca
 pachythecioides
-pachythecum
 pachythrix
 pachytricha
-pachytrix
 pacifica
 pacifica (Grace 946)
 pacificum
 pacificus
 packhamiae
 pactolus
 paddisoni
 paddisonii
+padulosum
 padwickii
 paedoglauca
 paeminosa
 paeninsularis
 paeninsularis x villifera
 paeoniaefolium
 paeoniifolium
 paeoniifolius
 pagetii
 pagetodes
 pagna
+pagodicystidiatus
 pagophila
 pagophilus
 pagorum
 pahiensis
 paisleyi
 paitensis
 pala
@@ -23439,22 +24026,24 @@
 pallescens
 pallida
 pallide-fusca
 pallide-fuscum
 pallide-virens
 pallidefuscum
 pallidella
+pallidiflavipes
 pallidiflora
 pallidiflorum
 pallidiflorus
 pallidifolia
 pallidifolium
 pallidifolius
 pallidifructus
 pallidifusca
+pallidinervis
 pallidipora
 pallidiramosa
 pallidissimum
 pallidissimus
 pallido-ochracea
 pallidoatra
 pallidobrunnea
@@ -23473,25 +24062,23 @@
 pallidovirens
 pallidula
 pallidulum
 pallidum
 pallidus
 palliolatis
 palliseri
-palludosa
 palmaceus
 palmae
 palmaefolium
 palmaeum
 palmarum
 palmata
 palmatula
 palmatum
 palmatus
-palmelioides
 palmensis
 palmeri
 palmeriae
 palmeriana
 palmerianus
 palmerstoni
 palmerstoniae
@@ -23510,24 +24097,26 @@
 palpera
 paludicola
 paludis
 paludosa
 paludosas
 paludosum
 paludosus
+palumana
 palumanus
 palumense
 palumensis
 palustre
 palustris
 pamela
 pamelae
 pamiae
 pampeana
 pampeanus
+pamphila
 pampliniana
 panaciformis
 panaeolum
 panaeolus
 panaetioides
 panamensis
 panaria
@@ -23549,24 +24138,27 @@
 pandanocarpa
 pandanophylla
 pandanophyllum
 pandanum
 pandorae
 pandorana
 pandorea
+pandrosion
 panduformis
 pandum
 pandura
-panduraefolia
-panduraefolium
 panduraeformis
 pandurata
 panduratus
+pandurifolia
+pandurifolium
 panduriforme
 panduriformis
+paneeroides
+panespora
 pangerangoensis
 pangorei
 panhesya
 panicea
 paniceum
 paniceus
 panici
@@ -23595,15 +24187,14 @@
 paniculata population (q)
 paniculata population (r) Busselton form
 paniculatum
 paniculatus
 paniculosa
 panicum
 pannarina
-pannarinum
 pannicola
 panniculata
 panniculus
 panniforme
 panniformis
 panniosum
 pannona
@@ -23680,62 +24271,74 @@
 papyriferum
 papyrina
 papyrinum
 papyrocarpa
 papyrocarpum
 papyrus
 para
-paraamoenum
 parabola
 parabolica
 parabolum
+paracastaneicola
+paracaudata
 parachromapes
 paracolpica
 paracrinitum
 paractaenum
 paractia
+paracylindrospora
 paradisi
 paradisiaca
 paraditopa
 paradoxa
 paradoxa x verniciflua
+paradoxae
 paradoxica
 paradoxides
 paradoxum
 paradoxus
+paraelegans
 paraexcentricum
+parafalcata
 paraformis
 paragibberosa
 paraguayense
 paraguayensis
 parahebicola
 parahypotropa
 parahypotropum
 paralata
+paraleptospermi
 paralia
 paralias
 paralimnetica
 paralinguus
 paralium
 paralius
 parallela
 parallelicuspis
 parallelinervis
 parallelum
+paramacrospora
 paramatha
 paramatta
 paramattense
 paramattensis
 paramecium
+paramelaleucae
 paramoenolens
+paramoenum
 paraneura
 paraneurachnis
 paraneurum
 paranthera
+paraobliqua
 paraparmeliformis
+parapenidielloides
+paraphysata
 paraphysiferus
 parapsilosis
 parasema
 parasemum
 parasitica
 parasiticum
 parasiticus
@@ -23773,36 +24376,34 @@
 parkinsonii
 parlatorei
 parmeliarum
 parmeliicola
 parmelina
 parmelinoides
 parmelioides
-parmeloides
 parnassifolia
 parnassifolium
 parnassiifolia
 parnassiifolium
 parnkalliana
 parochraceus
 parodii
+paroecandrum
 paronychia
-parooensis
 parqui
 parramattana
 parramattense
 parramattensis
 parrana
 parrisiae
 parrisiae (Armstrong 5091)
 parrisiae - rupestre
 parrisii
 parrumbala
 parrumbalus
-parsoniae
 parsonsiae
 partheneia
 parthenica
 parthenicus
 parthenium
 partimpatens
 partita
@@ -23820,24 +24421,27 @@
 parvicallum
 parvicalyx
 parvicalyx x planifolia
 parvicapsa
 parvicaruncula
 parvicaulis
 parviceps
+parviclava
+parvicylindrica
 parvidens
 parviflora
 parviflora 'Maroota-Berrilee form'
 parviflora 'Typical form'
 parviflorum
 parviflorus
 parvifolia
 parvifoliolata
 parvifolium
 parvifolius
+parvifulva
 parviloba
 parvinuclea
 parvinucleum
 parvipapillata
 parvipapillatus
 parvipetala
 parvipinnula
@@ -23849,29 +24453,32 @@
 parvispora
 parvisporum
 parvisporus
 parvistaminea
 parvistipa
 parvistipula
 parvitexta
+parviumbrus
 parvivallis
+parviverrucosum
 parviverrucosus
 parvizebrinum
 parvoclystoides
 parvoincerta
 parvula
 parvuliflorum
 parvulifolia
 parvulosporus
 parvulum
 parvulus
 parvum
 parvus
 pascheri
 pascoeana
+pascoei
 pascoensis
 pascua
 pascuicolum
 pascuinus
 pascuorum
 pascuum
 pascuus
@@ -23879,14 +24486,15 @@
 paspali-scrobiculati
 paspali-thunbergii
 paspalicola
 paspalidioides
 paspalina
 paspalodes
 paspaloides
+pasqualense
 passerina
 passerinianum
 passerinii
 passerinoides
 passiflorae
 pastinacae
 pastinacarpum
@@ -23920,38 +24528,42 @@
 patentifolia
 patentifolium
 patentiloba
 patentinervis
 patentiramea
 patentissima
 patericola
+pateritonsus
 patersoni
 patersonia
 patersoniana
 patersonianum
 patersonii
 patersonis
 patersonius
 patilii
 patinata
 patinatum
 patinifera
 patouillardii
 patriae
 patricia
+patriciamatherae
 patricium
 patrickae
 patrickiae
+patrickii
 patula
 patuliflorus
 patulifolia
 patulifolius
 patulum
 patulus
 pauca
+paucicolor
 paucicostata
 paucidentata
 paucidentatus
 pauciflora
 pauciflora x amygdalina
 pauciflorum
 pauciflorus
@@ -24009,30 +24621,33 @@
 pavonia
 pavonica
 pavonicus
 pavonina
 pavonius
 pavopennacea
 pawlikowskyana
+pawpawense
 paxii
 paxilli
 paxillifera
 paxilliformis
 paxteri
 paxtonii
+paynescottiae
 paynterae
 paynteri
 pazschkei
 peacockeana
 peacocki
 peacockiana
 peacockii
 peakallana
 peakalliana
 peakallii
+pearceae
 pearnii
 pearsonii
 pearsoniorum
 peasicarium
 peckhamii
 peckiana
 peckianum
@@ -24065,14 +24680,15 @@
 pedicellaris
 pedicellata
 pedicellatum
 pedicellatus
 pedicellosa
 pedicellosum
 pedicularioides
+pediculata
 pediculus
 pedimontana
 pedina
 pedinum
 pedinus
 pedleyanus
 pedleyi
@@ -24085,14 +24701,15 @@
 pedunculatus
 pedunculosa
 pedunculosum
 pedunculosus
 peekelii
 peeneri
 peerallyi
+peggii
 pegleri
 peguana
 peisleyi
 pelagia
 pelagica
 pelagicum
 pelargonii
@@ -24172,14 +24789,15 @@
 penicilliferum
 penicilliformis
 penicillioides
 penicula
 peniculata
 peniculum
 peniculus
+penidielloides
 peninsulare
 peninsularis
 peninsulensis
 peniocystis
 penium
 penna
 penna-marina
@@ -24256,14 +24874,15 @@
 pentzkeana
 pentzkeanum
 pentzkei
 peperocarpos
 pepingensis
 pepli
 peplidis
+peplis
 peploides
 peplus
 pepo
 peponicola
 peponicolum
 peponula
 pepricarpos
@@ -24333,22 +24952,22 @@
 perfoliati
 perfoliatum
 perfoliatus
 perforans
 perforata
 perforatum
 perforatus
-perfossa
 perfurcata
 pergamenum
 pergamenus
 perglandulosa
 pergracile
 pergracilis
 pergranulata
+perhamata
 perhumile
 perhumilis
 perialla
 peribambusina
 pericarpica
 pericava
 perichaetiale
@@ -24387,15 +25006,14 @@
 perlucida
 permagna
 perminuta
 perminutum
 permutata
 permutatum
 pernambucanus
-pernervosa x parvifolia
 perniciosa
 pernodii
 perobscurus
 perobtusus
 peroffkyana
 peroffskyana
 peronata
@@ -24451,14 +25069,15 @@
 persicarium
 persicarius
 persichii
 persiciflorum
 persicifolia
 persicifolius
 persicina
+persicinipes
 persicinum
 persicinus
 persicum
 persiehana
 persiehii
 persimile
 persimilis
@@ -24466,14 +25085,15 @@
 persistens x shirleyi
 persistens x thozetiana
 persistens x xanthoclada
 persistentifolium
 personata
 personatum
 personatus
+personensis
 personioides
 persooniae
 persoonii
 persoonioides
 persoonoides
 persplendidus
 persquamata
@@ -24556,19 +25176,21 @@
 petraeoides
 petraeum
 petrakii
 petrapendula
 petrei
 petrensis
 petricola
+petricolae
 petrieana
 petriei
 petriseda
-petrogale
 petrophila
+petrophiles
+petrophilicola
 petrophiliodes
 petrophiloides
 petrophilum
 petrophilus
 petrophyes
 petrosa
 petroselini
@@ -24616,15 +25238,15 @@
 phaeoderma
 phaeolasia
 phaeoleuca
 phaeoloma
 phaeomarginatum
 phaeomma
 phaeophthalma
-phaeophylla
+phaeophthalmum
 phaeosperma
 phaeospora
 phaeosporum
 phaeosticta
 phaeostoma
 phaeotricha
 phaeotrichum
@@ -24633,29 +25255,29 @@
 phaeton
 phaeum
 phaeus
 phalaenarum
 phalaenopsis
 phalaricola
 phalaridis
-phalaris
 phalarus
 phalenarum
 phalloidea
 phalloides
 phanerophlebia
 pharangites
 phascoides
 phaseolifolia
 phaseolina
 phaseolisporus
 phaseoloides
 phaseolus
 phasmatodes
 phasmoides
+phasoloides
 phathyrantha
 phebaliodes
 phebalioides
 phebalium
 phegopteris
 phelgmatocarpus
 phellandra
@@ -24679,14 +25301,15 @@
 phillipsiana
 phillipsii
 phillipsiorum
 phillyraefolia
 phillyraeoides
 phillyreifolia
 phillyreoides
+phillyrioides
 phillyroides
 philochalix
 philombros
 philonothum
 philonotis
 philonotoideum
 philonotum
@@ -24800,14 +25423,15 @@
 phylloidiae
 phyllophila
 phyllophilum
 phyllophilus
 phyllophora
 phyllophoroides
 phylloplana
+phylloplanum
 phylloplanus
 phyllopoda
 phylloporinae
 phylloptera
 phyllopterus
 phyllorhiza
 phyllorhizum
@@ -24818,14 +25442,15 @@
 phyllostachya
 phyllostachys
 phyllostegia
 phymatodea
 phymatodes
 phymatodeum
 phymatodeus
+phymatodispora
 phymatodisporum
 phymatosporum
 physalifolium
 physalodes
 physaloides
 physantha
 physanthus
@@ -24904,14 +25529,15 @@
 pilisepalus
 pillagaensis
 pillansii
 pilligaense
 pilligaensis
 pilocarina
 pilocystidiata
+pilocystidiatum
 pilonema
 pilopus
 pilosa
 pilosella
 pilosellodies
 piloselloides
 pilosellum
@@ -24934,29 +25560,29 @@
 pilularis x planchoniana
 pilulifer
 pilulifera
 piluliferum
 piluliforme
 piluliformis
 pilulis
+pilulosa
 pimbaensis
 pimeleae
 pimeleifolia
 pimeleoides
 pimelifolia
 pimelioides
 pimelodes
 pimeloides
 pimenteliana
 pimpamae
 pimpinellifolia
 pimpinellifolius
 pimpinelloides
 pimpiniana
-pinacolens
 pinaster
 pinastri
 pinastroides
 pindanica
 pindanicum
 pinea
 pineti
@@ -24973,14 +25599,15 @@
 pinguis
 pini
 pinicola
 pinicolens
 pinifolia
 pinifolium
 pinifolius
+piniforme
 pininana
 pinkiana
 pinnacula
 pinnaculata
 pinnaculum
 pinnafolium
 pinnata
@@ -24994,28 +25621,30 @@
 pinnatula
 pinnatum
 pinnatus
 pinnella
 pinnicola
 pinnulata
 pinodella
+pinodes
 pinoidea
 pinoides
 pinoniana
 pinonianus
 pinophilus
 pinsitus
 pinto
 pintoi
 piperata
 piperatum
 piperatus
 piperis
 piperita
 piperita entity 37 'apetala'
+piperitae
 piperitus
 piperoides
 piptomeris
 pirara
 piriforme
 piriformis
 pirilliformis
@@ -25034,14 +25663,15 @@
 pisi
 pisicarpa
 pisicarpum
 pisicolor
 pisiforme
 pisiformis
 pisiglarea
+pisiglareum
 pisinnum
 pisinnus
 pisocarpium
 pisoliticola
 pisoniae
 pistillaris
 pistillata
@@ -25099,14 +25729,15 @@
 planchonis
 planctonica
 planctonicum
 planeta
 planetophorus
 planicaulis
 planicola
+planiconvexa
 planiculmis
 planiflora
 planifolia
 planifolia x ramulosa
 planifolia x tholiformis
 planifolium
 planifolius
@@ -25163,14 +25794,15 @@
 platycena
 platycephala
 platycephalus
 platycerii
 platycerum
 platychaeta
 platycheiridia
+platycheiridion
 platychila
 platychilus
 platychlamys
 platyclada
 platyclados
 platycorne
 platycornis
@@ -25186,20 +25818,22 @@
 platyloba
 platylobii
 platylobioides
 platylobium
 platyloma
 platynema
 platynemus
+platyneura
 platyneuron
 platypetala
 platypetalum
 platyphylla
 platyphylla x tereticornis
 platyphyllaceum
+platyphyllae
 platyphyllos
 platyphyllus
 platypoda
 platypodos
 platypodum
 platyptera
 platypterus
@@ -25221,14 +25855,15 @@
 platythaliae
 platythamnos
 platytrema
 platytricha
 platytyrea
 platyzoma
 platyzomopsis
+platzii
 plautella
 plautellum
 playfairi
 playfairiana
 playfairii
 plebeia
 plebeium
@@ -25247,45 +25882,64 @@
 plectostachyus
 plectrachnoides
 plectroniae
 pleiadenia
 pleiadenium
 pleiantha
 pleigynia
+pleioaustraliensis
+pleioaustrocylindrica
 pleiocephala
 pleiocephalus
 pleiochaeta
 pleiochaetum
 pleioclada
 pleiococca
+pleiocoronohesperidea
+pleiocrescens
+pleioerythrostigma
 pleiogyna
 pleiogynum
 pleiogynus
+pleiohesperidea
+pleioobtusispora
 pleiopetala
 pleiopetalum
 pleiopterum
 pleiopyrenigerum
+pleioquaestiformis
 pleiorrhiza
+pleioserpens
 pleiosperma
 pleiospermus
 pleiostemoneus
 pleiostigma
+pleiostomachia
 pleiotera
+pleioungulata
+pleiovinosa
+pleiovitalbae
+pleistolilacina
+pleistoobliqua
 pleistophragmia
+pleistovitalbae
 plejocephala
 plemmellea
 plena
 plena x terminalis
 plenissima
+plenus
+pleomorpha
 pleomorphum
 plesiocoralloides
 pleurandroides
 pleurata
 pleurinervia
 pleurocarpa
+pleurocarpae
 pleuroceras
 pleurococcoides
 pleurocorys
 pleurogynoides
 pleuronectes
 pleuropappus
 pleurophylla
@@ -25346,31 +26000,34 @@
 pluriangulatus
 pluricallata
 pluricaulis
 pluriflora
 pluriflorus
 pluriglandulosa
 plurijuga
+plurililacina
 plurilocularis
 pluriloculata
 pluriloculatus
 plurimiseptata
 plurinervata
 plurinerve
 plurinervia
 plurinervis
 plurisegmenta
 plurisepala
 plurisepalea
 plurisepaleus
 plurisepalus
 pluriseta
+pluristomachia
 plurivora
 pluvialis
 pluviatilis
+pluviorum
 pluviosilvestris
 pluvisilvaticus
 pluvium
 poae
 poae-nemoralis
 poaeformis
 poaeoides
@@ -25388,34 +26045,37 @@
 podacanthum
 podagraria
 podagrica
 podagricum
 podalyriaefolia
 podalyrifolia
 podalyriifolia
+podalyriifoliae
 podalyriifolium
 podalyrina
 podantha
 podanthum
 podenzanae
 podiocarpa
 podistra
 podocarpa
+podocarpi
 podocarpifolia
 podocarpoides
 podolepideum
 podolepidis
 podolepidium
 podolepis
 podopetala
 podophylla
 podophyllum
 podperae
 podzolica
 podzolicus
+poecilometigena
 poecilophlebia
 poecilophlebium
 poeltii
 poeppigiana
 poeppigianum
 poeppigii
 poeticus
@@ -25423,19 +26083,20 @@
 pogonati-urnigeri
 pogonocalyx
 pogonocarpum
 pogonolepis
 pogonoloba
 pogonophora
 pogostoma
-pohliaecarpum
 pohliaeopsis
+pohliicarpum
 pohlmaniana
 pohlmaniana var. (Gilbert River C.T.White 1409)
 pohlmanianum
+pohlmannia
 pohlmanniana
 poicilum
 poiformis
 poimena
 poimenae
 poinciana
 poiretiana
@@ -25475,14 +26136,15 @@
 polospora
 polot
 polpha
 polyacantha
 polyacanthum
 polyacanthus
 polyacida
+polyactina
 polyadenia
 polyadenium
 polyadenos
 polyancistra
 polyandra
 polyandrum
 polyandrus
@@ -25498,17 +26160,19 @@
 polybotrya
 polybotrys
 polybotryum
 polybotryus
 polybractea
 polybracteata
 polycarpa
+polycarpae
 polycarpina
 polycarpoides
 polycarpon
+polycarpos
 polycarpum
 polycarpus
 polycaulon
 polycephala
 polycephala sensu A. Braun
 polycephalum
 polycephalus
@@ -25553,15 +26217,14 @@
 polygonata
 polygonati
 polygonatum
 polygoni-serrulati
 polygonifolius
 polygonoides
 polygramma
-polygrammoides
 polygrammus
 polygyna
 polygynum
 polygyra
 polyidis
 polyloba
 polymera
@@ -25592,14 +26255,15 @@
 polypori
 polyporoides
 polypterygia
 polypyllum
 polyrhiza
 polyrhizon
 polyrhizum
+polyrrhiza
 polyscia
 polysciada
 polyscium
 polyseta
 polysetum
 polysiphoniae
 polysora
@@ -25816,14 +26480,15 @@
 praefolia
 praegnans
 praelonga
 praelongata
 praelongatum
 praelongatus
 praelongipes
+praelongispora
 praelongum
 praelongus
 praelta
 praeltus
 praemollis
 praemonas
 praemorsa
@@ -25853,14 +26518,15 @@
 prasinastra
 prasinella
 prasinum
 prasinus
 prasiolitica
 pratense
 pratensis
+prati
 praticola
 pratioides
 prava
 pravifolia
 pravifolium
 pravissima
 pravissimum
@@ -25868,14 +26534,15 @@
 precatoria
 precatorius
 prehendens
 prehensilis
 preisii
 preissi
 preissiana
+preissianae
 preissianum
 preissianus
 preissii
 preminghana
 premnae
 premnanthoides
 premnea
@@ -25884,19 +26551,22 @@
 prenticei
 prescottii
 presliana
 preslii
 prethopodalis
 priceana
 priceanus
+prima
 primaria
 primitiva
+primogenitum
 primordialis
 primulacea
 primulaceus
+primulae
 primulaefolia
 primulaefolius
 primuliflora
 primuliflorum
 primulifolia
 primulifolius
 primulina
@@ -25971,14 +26641,15 @@
 profallax
 profunda
 profundum
 profusa
 profusum
 proiantha
 proianthum
+proiphydis
 prolata
 prolatum
 prolatus
 prolifer
 prolifera
 proliferata
 proliferum
@@ -26005,26 +26676,29 @@
 pronum
 propaguli
 propagulifera
 propaguliferum
 propebyssoides
 prophylla
 prophyllum
+prophyrocladus
 propingnum
 propinqua
 propinquior
 propinquum
 propinquus
 proponens
+propria
 propriorichromapes
 proprius
 propulagifera
 propullulans
 propulsator
 prorepens
+prorufa
 prosacris
 proserpinensis
 prosodea
 prospectum
 prospersa
 prostantherae
 prostantheroides
@@ -26034,14 +26708,15 @@
 prostratum
 prostratus
 protea
 proteacearum
 proteacium
 proteae
 proteaeoides
+protearum
 protecta
 protectum
 proteiformis
 proteiporus
 protena
 protendens
 protensa
@@ -26061,15 +26736,14 @@
 protosorediata
 protosulcata
 protothallina
 prototypa
 prototypica
 prototypum
 prototypus
-protovirens
 protracta
 protractum
 protractus
 protrudens
 protrusa
 protrusum
 protuberans
@@ -26137,19 +26811,22 @@
 pseudo-flavellata
 pseudo-neurachne
 pseudo-obducens
 pseudo-obscura
 pseudo-piperita
 pseudoacacia
 pseudoacrotricha
+pseudoacuta
+pseudoalata
 pseudoalpinum
 pseudoamoenum
 pseudoamphioxys
 pseudoamphixantha
 pseudoarbuscula
+pseudoarenaria
 pseudoarmatum
 pseudoatocion
 pseudoaugur
 pseudobarbatus
 pseudobiretum
 pseudobitteriana
 pseudoboscii
@@ -26163,14 +26840,15 @@
 pseudocandidum
 pseudocapsicum
 pseudochaetochloae
 pseudochina
 pseudociliata
 pseudociliatum
 pseudociliatus
+pseudocircinoseta
 pseudocladosporioides
 pseudoclaricolor
 pseudoclypeata
 pseudococcinea
 pseudococcodes
 pseudoconnatum
 pseudocoppinsii
@@ -26180,38 +26858,45 @@
 pseudocracca
 pseudocrassirostris
 pseudocratis
 pseudocretaceus
 pseudocrinitus
 pseudocrispa
 pseudocrispus
+pseudocryptogea
 pseudocurvisetus
 pseudocymosa
 pseudocyperus
 pseudocyphellariae
 pseudodactylina
+pseudodarliae
 pseudodecandra
 pseudodecandra x tagal
 pseudodecorata
 pseudodelicatissima
 pseudodemissum
 pseudodianae
 pseudodichotoma
+pseudodiospyri
 pseudodrummondii
 pseudoelegans
+pseudoeucalypti
 pseudoexanthismocarpa
 pseudoexigua
 pseudoextenuatum
+pseudofalcata
 pseudofastigiatum
 pseudofeei
 pseudoferrugineum
 pseudofischeri
 pseudoflabellata
 pseudoflacca
+pseudoflagellispora
 pseudofloccosa
+pseudoflocktoniae
 pseudofloribunda
 pseudofloridianum
 pseudofluitans
 pseudoforcipata
 pseudofoveolata
 pseudofulvella
 pseudofurcigerum
@@ -26264,19 +26949,21 @@
 pseudomuralis
 pseudomutica
 pseudonana
 pseudonarcissus
 pseudoneglecta
 pseudoneurachne
 pseudoniger
+pseudonigra
 pseudonilgherrense
-pseudonilgherrensis
 pseudonitidulum
 pseudonoctiluca
 pseudonordstedtii
+pseudonubilosa
+pseudoobtusa
 pseudopachydermum
 pseudopallescens
 pseudopallidella
 pseudopallidum
 pseudopallidus
 pseudopapillosum
 pseudoparadoxa
@@ -26305,14 +26992,15 @@
 pseudorhus
 pseudorobusta
 pseudorotundisporus
 pseudoruderale
 pseudorufescens
 pseudosaccatus
 pseudosacculatum
+pseudosamuelii
 pseudoscaber
 pseudoscenedesmus
 pseudoscutiformis
 pseudosebaldi
 pseudosenex
 pseudoseriata
 pseudosigma
@@ -26354,14 +27042,15 @@
 pseudotunbridgense
 pseudoturbinatum
 pseudouncinatum
 pseudovellea
 pseudovespa
 pseudovirens
 pseudovolvox
+pseudowalkeri
 psidii
 psidioides
 psilantha
 psilobasis
 psilocalyx
 psilocarpa
 psilocarpus
@@ -26404,14 +27093,15 @@
 psychotriaefolia
 psychotriaefolium
 psychotriifolia
 psychotriifolium
 psychotrioides
 psychotroides
 psychrocharis
+psychrophila
 psyllium
 ptarmicaeflorum
 ptarmicaefolia
 ptarmiciflorum
 ptarmicifolia
 ptarmicoides
 pteraneura
@@ -26457,14 +27147,15 @@
 pterostylis
 pteruloides
 pterygodes
 pterygosperma
 ptilota
 ptychocarpa
 ptychocarpon
+ptychocarpos
 ptychocarpum
 ptychoclada
 ptychocladum
 ptychodes
 ptychoides
 ptychomitrioides
 ptychophylla
@@ -26484,14 +27175,15 @@
 pubicosta
 pubicostum
 pubiflora
 pubiflorum
 pubiflorus
 pubifolia
 pubifolium
+pubifolius
 pubigera
 pubigerum
 pubinervis
 pubinodis
 pubirhachis
 pubisquama
 pubisquameum
@@ -26550,14 +27242,15 @@
 pullenii
 pullula
 pullulans
 pullus
 pulmonarius
 pulneyensis
 pulopenangensis
+pultenaea
 pultenaeiformis
 pultenaeum
 pulteneae
 pulverata
 pulverea
 pulvereus
 pulverulacea
@@ -26616,14 +27309,15 @@
 pungentium
 pungetium
 punicea
 puniceum
 puniceus
 punkapitiensis
 pupa
+pupatju
 pupula
 pura
 purdieae
 purdieana
 purdiei
 purpuascens
 purpurascens
@@ -26634,21 +27328,21 @@
 purpurea
 purpurea vel aff.
 purpurea x solanacea
 purpureapetala
 purpureaum
 purpureipetalum
 purpureo-caerulea
-purpureo-flava
 purpureo-olivaceus
 purpureo-sericeum
 purpureocaerula
 purpureocaulis
 purpureocolla
 purpureoflava
+purpureofuscum
 purpureonitens
 purpureopetala
 purpureopetalum
 purpureospora
 purpurescens
 purpureum
 purpureus
@@ -26672,14 +27366,15 @@
 pusiolus
 pustula
 pustulans
 pustulata
 pustulatum
 pustulatus
 pustulescens
+pustulifolia
 pustuliza
 pustulosa
 pustulum
 putaminosa
 putaminosus
 putaminum
 puteale
@@ -26716,14 +27411,15 @@
 pycnostachyum
 pycnostachyus
 pycnothelia
 pycnotricha
 pycnotrichum
 pyelodes
 pygmaea
+pygmaeformis
 pygmaeum
 pygmaeus
 pygmalum
 pygmea
 pymacum
 pyracanthae
 pyracanthon
@@ -26753,32 +27449,33 @@
 pyriferus
 pyrifolia
 pyrifolium
 pyriforme
 pyriformis
 pyrilobum
 pyrina
-pyrinus
 pyrispora
 pyrocarpa
 pyrochroa
 pyrogenus
 pyrophila
 pyrophilus
 pyrophora
 pyrophorum
 pyrophthalma
 pyrophthalmum
+pyropus
 pyrorum
 pyrothecium
 pyrrhanthes
 pyrrhocarpa
 pyrrhocreas
 pyrrhodasys
 pyrrhophila
+pyrrhopoda
 pyrrhum
 pyrrhus
 pyrrophylla
 pyrum
 pythara
 pyxidaria
 pyxidata
@@ -26906,30 +27603,29 @@
 queenslandianus
 queenslandica
 queenslandicum
 queenslandicus
 queenslandicus x refractus
 queletii
 quenda
-quercicola
 quercifolia
 quercifolium
 quercifolius
 quercina
 quercinum
 quercinus
 quercizans
 quercus
 querinae
-quezelii
 quiescens
 quietus
 quinata
 quinatus
 quindecim
+quini
 quiniflora
 quinii
 quinina
 quinkanensis
 quinniorum
 quinquangulare
 quinquangularis
@@ -26953,14 +27649,15 @@
 quinquepartita
 quinquepetalum
 quinquepetalus
 quinquescuspis
 quinqueseptatum
 quinquevulnera
 quinquifolia
+quintiniae
 quiricana
 quiricanus
 quisquilaris
 quisquiliare
 quisquiliarum
 quitensis
 quixote
@@ -26994,15 +27691,14 @@
 raciborskii
 racospermoides
 radiale
 radialis
 radians
 radiata
 radiata x serotina
-radiata x stricta
 radiatius
 radiatofissum
 radiatorugosus
 radiatum
 radiatus
 radicale
 radicalis
@@ -27022,25 +27718,27 @@
 radicosum
 radicosus
 radiculata
 radiculatum
 radiculosa
 radiculosum
 radicum
+radicus
 radinophylla
 radiodives
 radiofissile
 radiofissilis
 radiosa
 radiosafallax
 radiosum
 radonensis
 radula
 radulans
 raduliloba
+raduloides
 raetam
 raffii
 rafflesiana
 ragazziana
 ragazzianus
 raggedensis
 ragusina
@@ -27091,19 +27789,21 @@
 ramosii
 ramosissima
 ramosissimum
 ramosissimus
 ramosoradicatus
 ramosum
 ramosus
+ramotenellum
 rampoddense
 rampoddensis
 ramsayae
 ramsayana
 ramsayi
+ramsdenii
 ramuana
 ramuanus
 ramulans
 ramulare
 ramularis
 ramulentum
 ramulentus
@@ -27131,14 +27831,15 @@
 rangiferops
 rangiformis
 rangoonensis
 ranipes
 rankinensis
 rankingi
 rankingii
+rankiniae
 rantonnei
 rantonnetii
 ranuliferum
 ranunculacea
 ranunculaceum
 ranunculata
 ranunculi
@@ -27160,49 +27861,52 @@
 rappiana
 rapunculoides
 rara
 rariflora
 rariflorum
 rariflorus
 rarifolia
+rarihospitum
 raripila
 raripilus
 rarissima
 rarum
 rarus
 rasilis
 rasipes
 rata
 ratkowskiana
 ratkowskyanus
 rattanicola
 rattenburyi
 ratticauda
+ratticaudae
 rattrayi
 rauhii
 raunkiaeri
 rava
 ravenelii
 ravensthorpensis
 ravenstreetina
 raveretiana
 ravida
+ravinense
 ravum
 rawakense
 rawakensis
 rawsoniensis
+raybouldiae
 raybrownii
 raymundi
 raymundii
 raynalii
 raysmithii
-readeranum
 readeri
 readeriana
-readerii
+readerianum
 readii
 reagenella
 reagens
 rebeccae
 recedens
 rechingeri
 recipienda
@@ -27240,16 +27944,18 @@
 recurvicuspis
 recurvifolia
 recurvifolium
 recurvimucronata
 recurvipila
 recurvipilis
 recurvipilum
+recurvirostra
 recurvirostre
-recurvirostris
+recurvirostrum
+recurvirostrus
 recurvisepala
 recurvisepalus
 recurvistipula
 recurvistylis
 recurvula
 recurvulum
 recurvum
@@ -27261,22 +27967,22 @@
 reddellii
 redeckei
 redekei
 redimiculifera
 redita
 rediunta
 redolens
-reducens
 reducta
 reductum
 redunca
 reduncus
 reduplicata
 reduplicatum
 reesiae
+reesii
 reeuwykiana
 reeveanum
 reevesii
 reflectens
 reflexa
 reflexidens
 reflexifolia
@@ -27284,26 +27990,26 @@
 reflexistipula
 reflexum
 reflexus
 refracta
 refractum
 refractus
 refringens
-refringes
 refugia
 refulgens
 regalis
 regelii
 regia
 regina
 reginae
 regium
 regius
 regnans
 regnans x obliqua
+regnantis
 regnellii
 regnesii
 regulare
 regularis
 rehmanniana
 rehmannianus
 rehmannii
@@ -27335,15 +28041,14 @@
 reinwardtii
 reisiglii
 reissekii
 reissii
 relativa
 relaxa
 relaxum
-relicina
 relicinula
 relicta
 relictua
 religiosa
 reliqua
 remanella
 remanens
@@ -27371,14 +28076,15 @@
 reniformi
 reniformis
 reniloba
 renispora
 renitens
 reniverrucosus
 rennieana
+rennwickiana
 renschii
 renunculiflorus
 renwickiana
 repanda
 repandidentatus
 repandistipula
 repandodentatus
@@ -27403,14 +28109,15 @@
 reptatrix
 repullans
 repullulans
 requienii
 resa
 resectum
 resedanum
+resedanus
 resedifolia
 resedifolium
 reseminans
 resiliens
 resinaceum
 resinaceus
 resinicostata
@@ -27443,15 +28150,14 @@
 restituta
 restrictum
 resupina
 resupinata
 resupinatum
 rete
 retecta
-reteporus
 retevenia
 reticularis
 reticulata
 reticulata sensu Skvortsov (1926)
 reticulatum
 reticulatus
 reticulum
@@ -27469,14 +28175,15 @@
 retiruga
 retiruge
 retirugella
 retirugis
 retirugum
 retis
 retispora
+retisporum
 retisporus
 retitesta
 retivalve
 retivalvis
 retivenea
 retiveneum
 retivenia
@@ -27689,14 +28396,15 @@
 rhynchocarpum
 rhynchocephala
 rhynchocephalum
 rhyncholepis
 rhynchonema
 rhynchopetala
 rhynchosioides
+rhynchosporae
 rhynchotropis
 rhyncocarpa
 rhyncophorum
 rhyolitica
 rhyoliticum
 rhyparophora
 rhyparophorus
@@ -27828,14 +28536,15 @@
 rivicola
 riviniana
 rivinoides
 rivulare
 rivulare sensu Entwisle (1989b)
 rivularis
 rivularum
+rivulata
 rivulicola
 rivulosa
 rivulosum
 rivulosus
 rixosum
 robbii
 robbinsii
@@ -27849,15 +28558,15 @@
 robertsianum
 robertsianus
 robertsii
 robertsiorum
 robertsoni
 robertsoniae
 robertsonii
-robillardei
+robillardii
 robillardoides
 robinae
 robiniae
 robinsoni
 robinsoniae
 robinsoniana
 robinsonii
@@ -27873,15 +28582,14 @@
 robustiusculum
 robustula
 robustum
 robustus
 robyniae
 robynsianus
 roccellica
-rochelia
 rochesterensis
 rockinghamensis
 roddii
 roderickii
 rodneyanum
 rodriguesii
 rodwayana
@@ -27932,23 +28640,23 @@
 rosae
 rosaefolius
 rosaliae
 rosanoffii
 rosans
 rosarum
 rosatii
-rosaviolacea
 roscida
 roscidulum
 roscidum
 rosea
 rosea-alba
 rosea-major
 roseana
 rosei
+roseialbus
 roseiflora
 rosella
 rosellus
 rosemstromii
 rosenbergii
 rosenstromii
 rosenvingei
@@ -27984,14 +28692,15 @@
 rosmarinifolium
 rosmarinifolius
 rosmariniformis
 rosmarinoides
 rosmarinus
 rossei
 rosserae
+rossi
 rossiana
 rossii
 rostellata
 rostellatum
 rostellifera
 rostelliferum
 rostellum
@@ -28009,15 +28718,14 @@
 rosulans
 rosularis
 rosulata
 rosulatum
 rosulatus
 rotaeana
 rotala
-rotalilis
 rotalis
 rotata
 rotatilis
 rotatum
 rotatus
 rothae
 rothiana
@@ -28087,15 +28795,14 @@
 rubicunda
 rubicundum
 rubicundus
 rubida
 rubida x aggregata
 rubida x viminalis
 rubidae
-rubidula
 rubidum
 rubidus
 rubifolia
 rubiforme
 rubiformis
 rubiginascens
 rubigineoareolatum
@@ -28110,14 +28817,16 @@
 rubricalyx
 rubricarina
 rubricaule
 rubricaulis
 rubricentrum
 rubrichila
 rubricola
+rubricosa
+rubricosum
 rubriflora
 rubriflorum
 rubrigena
 rubrigenum
 rubrijuvenis
 rubrimolle
 rubrina
@@ -28155,57 +28864,58 @@
 rubrostoma
 rubrotincta
 rubrotinctum
 rubrotinctus
 rubroviolaceus
 rubroviridis
 rubrum
+rudallense
 rudallensis
 rudallii
 rudderi
 rude
 rudecta
 ruderale
 ruderalis
 rudericola
 rudgei
 rudicula
-rudior
 rudis
 rudiuscula
 rudolphii
 ruellii
 rueppellianum
 rufa
 rufescens
 rufibasis
 ruficarpa
 ruficaule
-ruficola
 rufida
 rufidulum
 rufiflora
 rufipes
 rufipogon
 rufiseta
 rufistylis
 rufitincta
 rufitinctus
 rufo-olivacea
 rufoaurea
 rufoaureum
+rufobadia
 rufobasis
 rufobrunnea
 rufocarnea
 rufocarneum
 rufocarneus
 rufociliata
 rufocornea
 rufocorneum
 rufocuprea
+rufoflavipes
 rufofulva
 rufolanosa
 rufolateritius
 rufopallidus
 rufopruinosa
 rufopruinosum
 rufopunctata
@@ -28223,26 +28933,29 @@
 rugatus
 rugiceps
 rugiferum
 rugiseta
 rugocephala
 rugocephalum
 rugosa
+rugosae
 rugosifolia
 rugosisporus
+rugosiviscosum
 rugosoannulata
 rugosoelegans
 rugosula
 rugosulum
 rugosum
 rugosus
 rugulata
 rugulosa
 rugulosarium
 rugulosella
+rugulostipitatus
 rugulosum
 rugulosus
 ruizensis
 rulingiae
 rulingioides
 rumicis-scutati
 ruminata
@@ -28282,27 +28995,31 @@
 russa
 russanowi
 russeliana
 russell-smithii
 russelliana
 russellii
 russeocinnamomeus
-russeocinnamoneus
 russeus
 russiceps
 russodes
 russula
+russulisporus
 russus
 rustica
+rustici
 rutabulum
 rutaefolia
 rutaefolium
 rutaefolius
 rutaeolens
 ruthenica
+ruthhalliae
+ruthsangerae
+rutidochlamys
 rutidoclamys
 rutidolepis
 rutidosea
 rutidosis
 rutidosperma
 rutidota
 rutifolia
@@ -28368,23 +29085,25 @@
 sacculum
 sacculus
 sacer
 sachalinense
 sachalinensis
 sachlanii
 sackettii
+sackstonii
 sacrata
 sacratum
 saddlensis
 saepiaria
 saepiarius
 safrolifera
 sagei
 sagenidii
 sagenomatis
+sagerae
 sageretiae
 sageretina
 saggicola
 saginata
 sagitallis
 sagittaefolium
 sagittarium
@@ -28396,28 +29115,30 @@
 sagittifolia
 sagittifolium
 sagittulatum
 sagraeaum
 sahayai
 saidana
 sainsburiana
+saintkilda
 saintpaulioides
 saintronanensis
 sajor-caju
 sake
 sakisimensis
 salahae
 salazinica
 salbundia
 salcrambidiocarpa
 salebrosa
 salebrosum
 salicaria
 salicariaefolia
 salicariifolia
+salicicola
 salicifolia
 salicifolium
 salicifolius
 saliciforme
 saliciformis
 salicina
 salicina x linearis
@@ -28430,14 +29151,15 @@
 salicorniae
 salicornioides
 salifex
 salifugus
 saligna
 saligna x tereticornis
 saligna x versicolor
+salignae
 salignum
 salignus
 salina
 salinarum
 salingnus
 salinum
 salinus
@@ -28475,14 +29197,15 @@
 salutare
 salvatrix
 salviaefolia
 salviaefolius
 salvifolia
 salviifolia
 salviifolius
+salviniae
 samaense
 samaensis
 saman
 samaria
 samariformis
 sambac
 sambuci
@@ -28501,23 +29224,23 @@
 sanctae-crucis
 sancti-angelii
 sanctum
 sanderi
 sanderiana
 sandersonii
 sandfordii
+sandichiana
 sandifordiae
 sandifordiana
 sandrae
 sandriana
 sandrianus
 sandvicense
 sandvicensis
 sandwicense
-sandwichense
 sandwithii
 sandyana
 sanfordiana
 sanfordii
 sanfuentes
 sanguifluum
 sanguifluus
@@ -28667,14 +29390,15 @@
 scabridorsum
 scabridula
 scabridulum
 scabridum
 scabridus
 scabrifolia
 scabrifolium
+scabrilemma
 scabripes
 scabrisina
 scabriuscula
 scabriusculum
 scabriusculus
 scabropustulata
 scabrosa
@@ -28688,14 +29412,15 @@
 scaevolina
 scaevolincola
 scalare
 scalariformis
 scalarirete
 scalariretis
 scalaris
+scalarium
 scalaroides
 scalena
 scalenum
 scalpelliforme
 scalpelliformis
 scalpellus
 scalproides
@@ -28720,15 +29445,15 @@
 scariosa x verruculosa
 scariosifolia
 scariosum
 scariosus
 scarlatina
 scarlatinus
 scarlettianum
-scategenus
+scarthjohnsoniae
 scatigena
 scatigenus
 scelerata
 sceleratus
 scenedesmus
 sceptrum
 schaeferi
@@ -28756,20 +29481,20 @@
 schindleri
 schinifolia
 schinoides
 schinziana
 schinzii
 schismoides
 schistacea
-schistaceae
 schistocarpa
 schistophila
 schistorhiza
 schistorhizum
 schistorrhiza
+schizachyrii
 schizandra
 schizantha
 schizanthum
 schizeilematis
 schizolepis
 schizolomum
 schizophylla
@@ -28870,20 +29595,23 @@
 scindica
 scindicum
 scintillans
 sciophana
 sciophanes
 sciophanus
 sciophila
+sciopifolia
 sciotostyla
 scirpi
 scirpi-nodosi
 scirpicola
 scirpifolia
+scirpifoliae
 scirpifolium
+scirpodendri
 scirpoidea
 scirpoideum
 scirpoideus
 scissa
 scissum
 scitaminea
 scitamineum
@@ -28905,15 +29633,14 @@
 scleroclada
 sclerocladum
 sclerococcus
 scleroderma
 sclerodermum
 scleroides
 sclerolaenae
-sclerolaenioides
 sclerolaenoides
 sclerophaeum
 sclerophylla
 sclerophyllarum
 sclerophyllum
 scleroplaca
 scleroprium
@@ -28922,19 +29649,22 @@
 sclerosperma
 sclerospermum
 sclerosycia
 sclerotianus
 scleroticola
 sclerotiformis
 sclerotii
+sclerotina
 sclerotinium
 sclerotinius
+sclerotinus
 sclerotioides
 sclerotiorum
 scleroxyla
+scleroxylon
 sclopetifera
 scobina
 scobinacea
 scobinaceus
 scobinella
 scoboideum
 scolecina
@@ -28977,14 +29707,15 @@
 scorodonia
 scorodonius
 scorodoprasum
 scorpioides
 scorpioides sensu Entwisle & Kraft (1984)
 scorpiurus
 scortea
+scortechini
 scortechiniana
 scortechinii
 scorteus
 scorzonerifolium
 scotica
 scoticus
 scotinum
@@ -29101,14 +29832,15 @@
 seemenianum
 seemenianus
 segetalis
 segetum
 segmentosa
 segregata
 sehimae
+sehimatis
 sehimicola
 seirosperma
 seitheae
 sejugata
 sejuncta
 sejunctum
 sekikaica
@@ -29187,14 +29919,15 @@
 semierectus
 semifertile
 semifertilis
 semiflexa
 semiflexus
 semifurcata
 semifuscum
+semigastroideus
 semiglabra
 semiglabrum
 semiglauca
 semiglaucum
 semiglobata
 semiglobatus
 semiglobosa
@@ -29223,15 +29956,14 @@
 semilunulata
 seminarii
 seminata
 seminerve
 seminiperda
 seminis-convolvuli
 seminuda
-seminuda x parvifolia
 seminudum
 seminudus
 seminulum
 semiocculta
 semiopacus
 semiopposita
 semioppositus
@@ -29249,15 +29981,14 @@
 semipilosa
 semipinnata
 semipinnatifidum
 semiplana
 semiplanus
 semiplena
 semipulchellum
-semipulchellus
 semirepanda
 semirepandus
 semirigida
 semirigidum
 semirubra
 semirufum
 semirufus
@@ -29306,14 +30037,15 @@
 senegalensis
 senegalioides
 senex
 senifolia
 senile
 senilis
 senlensis
+sennae-torae
 senniana
 sennoides
 senocionifolia
 senodictyon
 senseletii
 sensitiva
 sensu Croome & Fabbro 2005
@@ -29330,15 +30062,14 @@
 separinus
 sepiaceovelutinum
 sepiaceus
 sepiaria
 sepiarium
 sepiarius
 sepicanus
-sepikensis
 sepioides
 sepium
 seppeltii
 septemfida
 septemseptata
 septemtrionalis
 septentrionale
@@ -29352,14 +30083,15 @@
 septorioides
 septosior
 septosporus
 septuosa
 septuosum
 sepulchralis
 sepulcralis
+serafiniae
 serena
 serendipita
 sergeyana
 seriale
 serialis
 serians
 seriata
@@ -29404,14 +30136,15 @@
 sericostachyum
 sericostachyus
 sericothrix
 sericovexilla
 serifluus
 seriocarpa
 seriocoleopsis
+seriostachya
 seriphioides
 sermentosum
 serotina
 serotinax
 serotinum
 serotinus
 serpens
@@ -29435,14 +30168,15 @@
 serraensis
 serrata
 serratifolia
 serratifolium
 serratifolius
 serratiformis
 serratistipa
+serratoides
 serratomarginatus
 serratula
 serratulodes
 serratuloides
 serratulum
 serratum
 serratus
@@ -29467,14 +30201,15 @@
 sesameus
 sesamoides
 sesban
 seselifolia
 sesquiflora
 sesquiflorus
 sesquispicula
+sesquispiculus
 sessile
 sessiliceps
 sessiliflora
 sessiliflorum
 sessiliflorus
 sessilifolia
 sessilifoliola
@@ -29502,21 +30237,23 @@
 setifer
 setifera
 setiferum
 setiflora
 setifolia
 setifolium
 setifolius
+setiforme
 setiformis
 setiger
 setigera
 setigerum
 setigerus
 setiglumis
 setipes
+setipora
 setiporus
 setisquama
 setistyla
 setosa
 setosa-asperula
 setosoasperula
 setosum
@@ -29553,17 +30290,19 @@
 sharkoensis
 sharmae
 sharonae
 sharoniae
 sharpeana
 sharpei
 sharpii
+shawiae
 sheaffiana
 sheana
 sheareri
+shearii
 sheathiana
 sheathii
 sheoak
 shepherdi
 shepherdianum
 shepherdii
 shepleyana
@@ -29574,14 +30313,15 @@
 shiressii
 shirleyae
 shirleyana
 shirleyanum
 shirleyanus
 shirleyi
 shivasii
+shoemakeri
 shonae
 shraderi
 shultziae
 shumwayae
 shuttleworthiana
 shuttleworthii
 siamea
@@ -29630,14 +30370,15 @@
 sieberianum
 sieberianus
 sieberii
 siebertiana
 sieboldianum
 sieboldii
 sieboldtianum
+siemsseni
 siemssenia
 siemssenii
 sifton
 sigma
 sigmatella
 sigmatophylla
 sigmatophyllum
@@ -29779,23 +30520,25 @@
 sissoo
 sistotremoides
 sistrata
 sistratus
 sisymbriifolium
 situla
 siussii
+sivanesaniana
 sjoestedtii
 skagii
 skanderbegii
 skeatsiana
 skeatsianus
 skeleton
 skinneri
 skirrophora
 skirrophorum
+sklodowskacurieae
 skogsbergii
 skottsbergii
 skujae
 skyrinica
 sladeanum
 slateri
 sleei
@@ -29927,15 +30670,14 @@
 sophora
 sophorae
 sophorina
 sorbifolia
 sorbifolium
 sordentulus
 sordida
-sordide-virens
 sordidevirens
 sordideviride
 sordidobubalina
 sordidogrisea
 sordidum
 sordidus
 sordulenta
@@ -29957,15 +30699,14 @@
 sorghina
 sorghum
 sorifera
 soriferan
 soriferus
 soriformis
 sorocarpa
-sorocheila
 sorocheilum
 sorokiniana
 sorokinianum
 sorophylla
 sorophyllum
 sororia
 sororiella
@@ -29992,18 +30733,18 @@
 sp.  7 (Weipa)
 sp. "10" of Martin et al. (2002)
 sp. "371 post fire"  [PERTH7598394]
 sp. "5" of Martin et al. (2002)
 sp. "8" of Martin et al. (2002)
 sp. "A"
 sp. "Boyanup"
-sp. "Cordillo Downs" (B.Lay 1487)
 sp. "Gibraltar Range"
 sp. "H909" of AusFungi
 sp. "H909" of Justo et al. (2010)
+sp. "LC1" [Young 2188 in BRI]
 sp. "Long stout-pedicelled" (W.R.Barker 2481)
 sp. "Lyndoch" (R.Bates 5906)
 sp. "Marla" (W.R.Barker 3535)
 sp. "Mungilli" (K.J. Knight MC 154)
 sp. "Mylor" (R.Bates 3529)
 sp. "O"
 sp. "P"
@@ -30015,40 +30756,35 @@
 sp. "Slender Sun Orchid"
 sp. "South-west Swamps"
 sp. "U"
 sp. "aff. pilosella" (H4784 HO)
 sp. "brown to yellowish brown-capped" (P.B. Matheny 3217)
 sp. "torresia nom. prov." (PBM 2157, E6978)
 sp. "yellow" of Hubregtse & Hubregtse (2011)
-sp. '#1'
 sp. '1 U.S.' sensu Harrop (1869)
-sp. '2'
-sp. '2061' in ADW on <I>Hydrocotyle callicarpa</I>
-sp. '3'
 sp. '40 Mile Scrub' (B.Hyland 11638)
-sp. '6 (BRIP 9175)' of Watling & Gregory (1989a)
 sp. 'A'
 sp. 'ACT 1'
 sp. 'ACT 2'
 sp. 'ACT'
 sp. 'Abercrombie Caves'
 sp. 'Adelaide Hills'
 sp. 'Adelaide hills'
+sp. 'Albany Highway late'
 sp. 'Albury'
 sp. 'Alice River' (J.R.Clarkson 3765)
 sp. 'Alligator Gorge'
 sp. 'Anglesea'
 sp. 'Angourie'
 sp. 'Ararat hills'
 sp. 'Arkaroola'
+sp. 'Arrowsmith late'
 sp. 'Arrowsmith'
 sp. 'Arthurs Lake'
 sp. 'Augusta'
-sp. 'BM1' (Young 2098)
-sp. 'BRIP 9132'
 sp. 'Baal Gammon' (B.P.Hyland 10341)
 sp. 'Bald Rock'
 sp. 'Bamaga' (B.Hyland 10235)
 sp. 'Bamaga' (B.P.Hyland 2517)
 sp. 'Barakula' (H.Dillewaard 942)
 sp. 'Barakula' (V.Hando 378)
 sp. 'Barong' (B.Hyland 2519 RFK)
@@ -30081,14 +30817,15 @@
 sp. 'Boonjee' (B.Hyland 2139 RFK)
 sp. 'Boonjee' (B.Hyland 2199 RFK)
 sp. 'Boonjee' (B.Hyland 6764)
 sp. 'Boorhaman'
 sp. 'Boranup'
 sp. 'Border Ranges'
 sp. 'Boulia' (L.Pedley 5297)
+sp. 'Boyatup'
 sp. 'Boyd Plateau'
 sp. 'Boyup Brook'
 sp. 'Boyup'
 sp. 'Bradshaw Station'
 sp. 'Brigooda' (W.Power s.n. Sept 1954)
 sp. 'Brookton Highway'
 sp. 'Broughton River'
@@ -30107,37 +30844,38 @@
 sp. 'Cape Naturaliste'
 sp. 'Cape River' (A.K.Irvine 1912)
 sp. 'Carboor'
 sp. 'Cardwell' (A.Thorsborne 16)
 sp. 'Carnarvon and Taroom' (R.W.Johnson 2764)
 sp. 'Carnarvon'
 sp. 'Castle Tower' (M.Crisp 2753)
+sp. 'Chapman Valley'
 sp. 'Chapple Vale'
 sp. 'Chudalup'
 sp. 'Claire'
 sp. 'Clarencetown'
 sp. 'Claudie & Chester Rivers' (L.J.Brass 19658)
 sp. 'Claudie River' (B.Gray 3240)
 sp. 'Claudie River' (B.Hyland 13102)
 sp. 'Coaldale'
+sp. 'Cocklebiddy'
 sp. 'Colllie'
 sp. 'Colo River'
 sp. 'Colo River' (Weston 2423)
 sp. 'Conway Range' (P.R.Sharpe 4139)
 sp. 'Cooktown' (A.K.Irvine 2178)
 sp. 'Coomera Valley' (J.Roberts s.n. Sept 1986)
 sp. 'Coominglah' (A.Bean 236)
 sp. 'Coonabarabran'
 sp. 'Coonawarra'
 sp. 'Coorong'
 sp. 'Cordalba' (K.Sarnadsky s.n. Jan 1986)
 sp. 'Cowley Beach' (C.Puttock & A.Graham)
 sp. 'D'
 sp. 'D'Aguilar Range' (P.Young 611)
-sp. 'DAR57117' of Shivas (1989)
 sp. 'Daintree River' (B.Gray 3162)
 sp. 'Dale'
 sp. 'Dandenong Ranges'
 sp. 'Darling Range'
 sp. 'Darling Scarp'
 sp. 'Darwin Lawns'
 sp. 'Darwin'
@@ -30148,18 +30886,14 @@
 sp. 'Digby'
 sp. 'Dongara'
 sp. 'Dorrigo'
 sp. 'Dryander Creek' (P.R.Sharpe 4169)
 sp. 'Dundonnell'
 sp. 'Dunmore' (D.M.Gordon 84)
 sp. 'Dunsborough'
-sp. 'EMD 15-1995'
-sp. 'EMD 54-1990'
-sp. 'EMD 7-1995'
-sp. 'EMD 8-2003'
 sp. 'Earlston'
 sp. 'East Gippsland'
 sp. 'East Kangaloon'
 sp. 'Ebor Falls'
 sp. 'Ebor'
 sp. 'Edison Mill'
 sp. 'Eneabba'
@@ -30178,14 +30912,15 @@
 sp. 'Fleurieu Peninsula'
 sp. 'Flinders Island'
 sp. 'Flinders Ranges north 1'
 sp. 'Flinders Ranges north 2'
 sp. 'Flinders Ranges red'
 sp. 'Flinders Ranges'
 sp. 'Flinders'
+sp. 'Forrestania'
 sp. 'Fraser Island'
 sp. 'Gadgarra' (B.P.Hyland RFK 2011)
 sp. 'Gammon Range'
 sp. 'Genowlan Point' (NSW 417813)
 sp. 'Gibraltar Falls'
 sp. 'Gibraltar Range'
 sp. 'Gilbert River'
@@ -30235,45 +30970,37 @@
 sp. 'Jollys Falls'
 sp. 'K.'
 sp. 'Kakadu'
 sp. 'Kalbarri'
 sp. 'Kangaroo Island'
 sp. 'Kaniva Giant'
 sp. 'Kaniva'
+sp. 'Karridale'
 sp. 'Katherine Gorge'
 sp. 'Kellerberrin'
 sp. 'Kemerton'
 sp. 'Kenenup'
 sp. 'Keninup'
 sp. 'Kennedy River' (J.R.Clarkson 5645)
 sp. 'Kilkoy Creek'
 sp. 'Kilsyth South'
 sp. 'Kooyera'
 sp. 'Kybean Range'
-sp. 'LEM 13-2005'
-sp. 'LEM 19-2005'
-sp. 'LEM 35-2005'
-sp. 'LEM 41-2005'
-sp. 'LEM 6-2005'
-sp. 'LEM 8-2005'
-sp. 'LJ30' of Anderson et al. (2001), Martin et al. (2002)
 sp. 'Lake Muir'
 sp. 'Lakeland Downs' (J.R.Clarkson 6291)
 sp. 'Lappa, Sandy Tate River' (L.J.Brass 1745)
 sp. 'Lara'
 sp. 'Laura' (C.Puttock UNSW 15926)
 sp. 'Limbunya'
 sp. 'Little Annan River' (B.Gray 101)
 sp. 'Long peduncles'
 sp. 'Longreach' (D.Davidson s.n. Aug 1952)
 sp. 'Lower Palmerston' (L.Jessup 472)
 sp. 'Lumeah' (R.W.Purdie 2168)
 sp. 'Lyndoch'
-sp. 'MEL2151450' of Sawyer et al. in Genbank
-sp. 'MH97' of Martin et al. (2002)
 sp. 'Maldon'
 sp. 'Mallacoota'
 sp. 'Malua Bay'
 sp. 'Mambray Creek'
 sp. 'Mandurang'
 sp. 'Maryborough'
 sp. 'Maryborough' (T.D.Stanley 87)
@@ -30282,18 +31009,19 @@
 sp. 'McIvor River' (J.R.Clarkson 5201)
 sp. 'McIvor River' (J.R.Clarkson 5447)
 sp. 'McNamee Creek' (B.Hyland 3565 RFK)
 sp. 'McPherson Range' (G.P.Guymer 2000)
 sp. 'Meadows'
 sp. 'Mehinup'
 sp. 'Melville Is.'
+sp. 'Merivale'
 sp. 'Midlands'
 sp. 'Millaa Millaa' (L.W.Jessup 515)
-sp. 'Miller's Dentate'
 sp. 'Millers Point'
+sp. 'Mobrup'
 sp. 'Moggill' (G.P.Guymer 1990)
 sp. 'Mokota'
 sp. 'Monaro'
 sp. 'Monarto South'
 sp. 'Monogorilby' (P.Forster 1004)
 sp. 'Moodiarrup'
 sp. 'Moondarra'
@@ -30311,14 +31039,15 @@
 sp. 'Mount Spurgeon'
 sp. 'Mount Victoria Uranium Mine'
 sp. 'Mt Bartle Frere' (M.Godwin 2960)
 sp. 'Mt Bartle Frere' (M.Godwin C1158)
 sp. 'Mt Beerwah' (A.Bean 6)
 sp. 'Mt Bellenden Ker'
 sp. 'Mt Brockman'
+sp. 'Mt Cooke'
 sp. 'Mt Coolum' (P.R.Sharpe 3345)
 sp. 'Mt Dryander' (V.K.Moriarty 1901)
 sp. 'Mt Finnigan' (L.J.Brass 20129)
 sp. 'Mt Hemmant' (B.Hyland 3196 RFK)
 sp. 'Mt Hemmant' (B.Hyland RFK3338)
 sp. 'Mt Lewis & Mt Spurgeon' (K.A.Williams 82/194)
 sp. 'Mt Lewis' (B.Gray 2844)
@@ -30362,21 +31091,20 @@
 sp. 'Naturaliste'
 sp. 'New England batholith'
 sp. 'New England escarpment'
 sp. 'New England striped'
 sp. 'New England swamps'
 sp. 'New England'
 sp. 'Newcastle Bay' (L.J.Brass 18671)
+sp. 'Newdegate'
 sp. 'Newland Head'
-sp. 'No. 2'
 sp. 'Noah Creek' (B.Hyland 2786 RFK)
 sp. 'Noah Creek' (B.P.Hyland 5987)
 sp. 'Noorinbee'
 sp. 'Nora Creina'
-sp. 'Norfolk'
 sp. 'Northampton'
 sp. 'Northern Pilliga'
 sp. 'Northern Swamps'
 sp. 'Nowra'
 sp. 'Nunniong'
 sp. 'Nyabing'
 sp. 'Old Bar'
@@ -30417,17 +31145,19 @@
 sp. 'Red Gum waterholes'
 sp. 'Red Hummock' (R.D.Royce 10394)
 sp. 'Richmond River'
 sp. 'Riverina grasslands'
 sp. 'Roaring Meg Creek' (B.Hyland 10626)
 sp. 'Roaring Meg' (L.J.Brass 20326)
 sp. 'Rokeby' (J.R.Clarkson 7132)
+sp. 'Roleystone'
 sp. 'Rum Jungle'
 sp. 'Sarina, Proserpine' (G.P.Guymer 2005)
 sp. 'Scaddan'
+sp. 'Scott River'
 sp. 'Small brown bayonets'
 sp. 'Smokers Gap'
 sp. 'South coast'
 sp. 'Southern Pilliga'
 sp. 'Southport'
 sp. 'Spring Ridge'
 sp. 'St Andrews'
@@ -30446,26 +31176,25 @@
 sp. 'The Knoll'
 sp. 'Theda Station'
 sp. 'Thornton Peak' (H.Flecker s.n. Dec 1949)
 sp. 'Thornton Peak' J.R.Clarkson 5556)
 sp. 'Three Springs'
 sp. 'Thursday Island' (E.Cowley 10,29)
 sp. 'Tiwi'
+sp. 'Toolinna'
 sp. 'Top End'
 sp. 'Topaz' (G.Sankowsky+ 244)
 sp. 'Topperwein'
 sp. 'Torndirrup'
 sp. 'Torrington'
 sp. 'Torrington' (J.B.Williams s.n. 9 May 1965)
 sp. 'Towrana' (R.J.Cranfield 2183)
 sp. 'Toy Creek'
 sp. 'Urbenville'
 sp. 'Verran Tanks'
-sp. 'WUM 4' of Hall & Fish (1979)
-sp. 'WUM 5' of Hall & Fish (1979)
 sp. 'Wallagaraugh'
 sp. 'Wallangarra' (J.Boorman s.n. Nov 1904)
 sp. 'Walpole'
 sp. 'Wandoo'
 sp. 'Wandoo' (V.Crowley DKN700)
 sp. 'Wannamal'
 sp. 'Warialda'
@@ -30485,14 +31214,15 @@
 sp. 'Williams'
 sp. 'Williamson' (B.J.Keighery & N.Gibson 226)
 sp. 'Wilsons Promontory'
 sp. 'Wimmera woodlands'
 sp. 'Windsor Tableland' (B.Gray 2181)
 sp. 'Windsor Tableland' (B.Hyland 2309)
 sp. 'Windy Harbour'
+sp. 'Wongan Hills'
 sp. 'Woohlpooer'
 sp. 'Woolly Tea-tree'
 sp. 'Woopen Creek' (G. & N.Sankowsky 685)
 sp. 'Woronora Plateau'
 sp. 'Wyalkatchem'
 sp. 'Wyberba'
 sp. 'Wyvuri' (B.P.Hyland RFK2632)
@@ -30595,14 +31325,17 @@
 sp. 'large bracts'
 sp. 'large curved flowers'
 sp. 'large fawn'
 sp. 'large scented'
 sp. 'large striped flowers'
 sp. 'late coastal dunes'
 sp. 'late flowering'
+sp. 'late forests'
+sp. 'late northern'
+sp. 'late south coast'
 sp. 'late summer'
 sp. 'late swamps'
 sp. 'late'
 sp. 'limestone heath'
 sp. 'limestone mallee'
 sp. 'limestone sands'
 sp. 'limestone'
@@ -30627,24 +31360,24 @@
 sp. 'mountain bogs'
 sp. 'narrow lip'
 sp. 'needle points'
 sp. 'north-east Vic hills'
 sp. 'north-west mallee'
 sp. 'north-western wheatbelt'
 sp. 'northern granite'
+sp. 'northern laterite'
 sp. 'northern montane'
 sp. 'northern swamps'
 sp. 'northern thick sepals'
 sp. 'northern'
 sp. 'northwest'
 sp. 'orientalis'
 sp. 'ornate flowers'
 sp. 'oxy'
 sp. 'papillose'
-sp. 'persicina' sensu Bougher (2009)
 sp. 'pink lip'
 sp. 'plumed'
 sp. 'pointed flowers'
 sp. 'pse'
 sp. 'pte'
 sp. 'purple lip'
 sp. 'quartz'
@@ -30704,19 +31437,19 @@
 sp. 'upper Spencer Gulf'
 sp. 'wandoo'
 sp. 'waterholes'
 sp. 'western Murray Flats'
 sp. 'western Victoria'
 sp. 'western wheatbelt'
 sp. 'western woodlands'
+sp. 'white gums'
 sp. 'woodland'
 sp. 'woodlands'
 sp. 'wrinkled lateral sepals'
 sp. 'yellow'
-sp. ( Bridle LA P.I.Forster+ PIF17345)
 sp. ('red bark', D120590)
 sp. (1)
 sp. (10)
 sp. (11)
 sp. (12)
 sp. (12-15 leaflets)
 sp. (13)
@@ -31115,14 +31848,15 @@
 sp. (Boulders BG 6326)
 sp. (Boulders)
 sp. (Boulia L.Pedley 5297)
 sp. (Boyd Creek A.R.Bean 19248)
 sp. (Boynedale M.I.H.Brooker 9767)
 sp. (Brewer LA B.Hyland 13373)
 sp. (Bribie Island S.T.Blake 7089)
+sp. (Bridle LA P.I.Forster+ PIF17345)
 sp. (Bringalily P.I.Forster+ PIF11661)
 sp. (Brisbane B.K.Simon 3221)
 sp. (Brisbane River)
 sp. (Broad-leaved Form)
 sp. (Brolga Park A.R.Bean 1002)
 sp. (Brolga Park; A.R.Bean 1002)
 sp. (Bromley B.P.Hyland 9022)
@@ -31477,15 +32211,14 @@
 sp. (Fryerstown)
 sp. (G.J.Barrett 15.9.1989)
 sp. (G.J.Keighery 10990)
 sp. (G.J.Keighery 343)
 sp. (G.J.Keighery 8376)
 sp. (G.J.Keighery 901)
 sp. (G.J.McCutcheon s.n.)
-sp. (GJK & JA 1951)
 sp. (Gadgarra B.P.Hyland RFK2011)
 sp. (Gadgarra BH 2011RFK)
 sp. (Gadgarra BH 25231RFK)
 sp. (Gadgarra)
 sp. (Gap Creek L.S.Smith 11116)
 sp. (Gap Creek L.S.Smith 14419)
 sp. (Gap Creek L.W.Jessup 651)
@@ -31602,14 +32335,15 @@
 sp. (Inglewood C.T.White AQ142073)
 sp. (Inglewood J.M.Dalby 86/93)
 sp. (Inglewood P.Grimshaw+ PG846)
 sp. (Inglewood R.W.Johnson 2940)
 sp. (Innisfail live-bearing)
 sp. (Ipswich K.A.Williams 86020)
 sp. (Iron Mt D.J.Liddle AQ484361)
+sp. (Iron Range BH 16395)
 sp. (Iron Range BH 21158V)
 sp. (Iron Range D.G.Fell DF2321)
 sp. (Iron Range D.G.Fell DF2327)
 sp. (Iron Range G.Sankowsky+ 382)
 sp. (Iron Range G.Sankowsky+ 383)
 sp. (Iron Range GS 382)
 sp. (Iron Range H.Flecker NQNC8728)
@@ -31660,14 +32394,15 @@
 sp. (K.R.Newbey 5514)
 sp. (K.R.Newbey 5627)
 sp. (K.R.Newbey 6532)
 sp. (K.R.Newbey 6679)
 sp. (K.R.Newbey 8269)
 sp. (K.R.Newbey 9766)
 sp. (K.R.Newbey 9775)
+sp. (KFK 10453)
 sp. (KS/6)
 sp. (Ka Ka Mundi N.P.)
 sp. (Ka Ka Mundi NP A.R.Bean 2170)
 sp. (Ka Ka Mundi NP W.J.McDonald+ 4642)
 sp. (Kajabbi D.A.Halford Q994)
 sp. (Kalbarri) A.P.Brown 8.82
 sp. (Kallala S.L.Everist 3223)
@@ -31729,14 +32464,15 @@
 sp. (Lake Mueller R.J.Fensham 3476)
 sp. (Lakefield J.R.Clarkson+ 6971)
 sp. (Lakefield NP J.R.Clarkson+ 7010)
 sp. (Lakefield NP P.I.Forster+ PIF12943)
 sp. (Lamb Range)
 sp. (Lamington G.Leiper AQ502702)
 sp. (Lamington G.Leiper AQ633386)
+sp. (Lamington NP)
 sp. (Lamington W.J.McDonald 6176)
 sp. (Lamond Hill G.Sankowsky+ 382)
 sp. (Lappa P.I.Forster+ PIF18572)
 sp. (Larcom Gully N.Gibson 1057)
 sp. (Laura A.R.Bean 1807)
 sp. (Laura A.R.Bean 1863)
 sp. (Laura C.Dalliston CC18)
@@ -31813,14 +32549,15 @@
 sp. (Maria Island)
 sp. (Mariala C.Sandercoe 600)
 sp. (Marlborough Creek G.N.Batianoff+ MC9108006)
 sp. (Marlborough J.McCabe AQ659027)
 sp. (Marlborough P.I.Forster PIF12269A)
 sp. (Marlborough P.I.Forster+ PIF12269A)
 sp. (Marlborough)
+sp. (Marr Creek BH 16069)
 sp. (Marrett River J.A.Elsol+ 680)
 sp. (Maryborough A.E.Logan AQ673312)
 sp. (Maryborough T.Stanley 87)
 sp. (Maryborough)
 sp. (Massy Creek P.I.Forster +PIF10568)
 sp. (Massy Creek R.G.Coveny+ 7174)
 sp. (Mataranka)
@@ -31852,14 +32589,15 @@
 sp. (McPherson Range G.P.Guymer 2000)
 sp. (McPherson Range W.D.Francis AQ217480)
 sp. (Mekunga Creek J.R.Clarkson 4373)
 sp. (Melaleuca Creek Scrub P.I.Forster+ PIF7949)
 sp. (Melrose D.A.Halford Q1524)
 sp. (Melville Island R.J.Fensham 2909)
 sp. (Merapah B.S.Wannan 5240)
+sp. (Merluna BH 21374V)
 sp. (Messines L.Pedley 1521)
 sp. (Midlands Highway) M.I.H.Brooker 8734
 sp. (Miles E.J.Thompson EJT888)
 sp. (Miles S.T.Blake 7709)
 sp. (Millaa Millaa L.W.Jessup 515)
 sp. (Millaa Millaa LWJ 515)
 sp. (Millaa Millaa RJ 494)
@@ -32041,16 +32779,16 @@
 sp. (Mt Lewis L.S.Smith 10107)
 sp. (Mt Lewis L.W.Jessup 554)
 sp. (Mt Lewis L.W.Jessup+ GJM1574)
 sp. (Mt Lewis L.W.Jessup+ GJM228)
 sp. (Mt Lewis LSS 10107)
 sp. (Mt Lewis LWJ 554)
 sp. (Mt Lewis P.I.Forster PIF15614)
-sp. (Mt Lewis V.K.Moriarity 833)
 sp. (Mt Lewis V.K.Moriarty 2445)
+sp. (Mt Lewis V.K.Moriarty 833)
 sp. (Mt Lewis VKM 2445)
 sp. (Mt Lewis VKM 833)
 sp. (Mt Lewis)
 sp. (Mt Lewis/Thornton Range)
 sp. (Mt Lews BG 167)
 sp. (Mt Lindesay P.I.Forster PIF12173)
 sp. (Mt Margaret P.I.Forster PIF6753)
@@ -34162,14 +34900,15 @@
 sp. Basalt Woodland (M.D.Barrett 198)
 sp. Basaltica (H.Nicholls s.n. MEL 649396)
 sp. Bastion Range (A.A.Mitchell et al. AAM 10710)
 sp. Batavia Downs (J.R.Clarkson 8511)
 sp. Batchelor (I.D.Cowie+ 1384)
 sp. Bathurst Island (R.Fensham 1021)
 sp. Battle Hill (A.L.Payne 1006)
+sp. Bayswater (C.Andrews s.n. 11/1902)
 sp. Beagle Bay (K.F.Kenneally 10628)
 sp. Beaked Fruit (R.J.Chinnock 4011)
 sp. Bearded (R.W.Jobson 2308)
 sp. Beardmore Rd (A.R.Annels & R.W.Hearn 4409)
 sp. Beatrice Creek (L.S.Smith 10487)
 sp. Beatrice River (L.S.Smith 10487)
 sp. Beaufort (G.J.Keighery 6291B)
@@ -34178,26 +34917,29 @@
 sp. Beaufort River (G.J.Keighery 16554)
 sp. Bebo State Forest (J.Westaway 1311)
 sp. Beddome Range (D.E.Albrecht 5656)
 sp. Beechworth (J.Galbraith s.n., MEL 2117497)
 sp. Beeron (P.I.Forster 4673 & C.E.Wilkinson)
 sp. Beeron Holding (P.I.Forster 5753)
 sp. Belele (D.W.Goodall 3215)
+sp. Belele (D.W.Goodall 3417)
 sp. Belele Station (A.L.Payne 80)
 sp. Bellenden Ker (B.Gray 2868)
 sp. Bellenden Ker (B.Gray 2948)
 sp. Bellenden Ker (B.Hyland 12916)
 sp. Bellenden Ker (B.Hyland 5775)
 sp. Bellenden Ker (W.Sayer 45)
 sp. Bemboka (Telford 11565)
 sp. Bencubbin-Koorda (M.E.Trudgen 5421)
 sp. Bendering (B.Lullfitz s.n. July 1965)
+sp. Bendering (J.W.Horn 4101)
 sp. Bendering (T.J.Alford 110)
 sp. Bent (I.D.Cowie 9688)
 sp. Beringbooding (A.R.Main 11/9/1957)
+sp. Berkeley River (M.D.Barrett MDB 4766)
 sp. Berrook (J.A.Jeanes s.n., MEL 2154721)
 sp. Berry Springs (M.O.Parker 855)
 sp. Berry Springs (P.Horsfall 1042)
 sp. Berthier Dunes (R.L.Barrett RLB 5753)
 sp. Bethungra
 sp. Beverley (K.Kershaw KK 2438)
 sp. Beverley (M.Ochtman & D.Lynch 48)
@@ -34286,15 +35028,15 @@
 sp. Blyth Range (W.V.Fitzgerald s.n. 1898)
 sp. Bodallin (R.Cranfield & D.Kabay 9134)
 sp. Boddington (D.Halford 80746)
 sp. Boddington (K.Atkins 309)
 sp. Boddington (K.J.Atkins 309)
 sp. Boiler Rocks (R.D.Seppelt 12528)
 sp. Bolgart (C.A.Gardner 8700)
-sp. Bolgart (M.Hislop & F.Hort MH2486)
+sp. Bolgart (M.Hislop & F.Hort MH 2486)
 sp. Bolt Head (J.R.Clarkson+ 8805)
 sp. Bolt Head (P.I.Forster PIF8948)
 sp. Bonaparte Archipelago (A.A.Mitchell 4774)
 sp. Bond Springs (D.J.Nelson 2538)
 sp. Bonnie Hill (K.R.Newbey 9831)
 sp. Boolardy Station (P.Jayasekara 719-JHR-01)
 sp. Boolbunda Rock (K.M.Sparshott+ KMS623)
@@ -34593,15 +35335,15 @@
 sp. Carr Boyd Range (T.G.Hartley 14527)
 sp. Carracarrup Creek (S.Kern, R.Jasper, D.Brassington LCH 16738)
 sp. Carrarang (M.E.Trudgen 7420)
 sp. Carson Escarpment (A.S.George 13732)
 sp. Carson River (A.A.Mitchell 4387)
 sp. Carson River (I.Cowie & Wendell IC 4232)
 sp. Carson River (M.McDonald MM1890)
-sp. Cascade (R.Bruhn 20896)
+sp. Cascade (R.Bruhn 20896 CAS)
 sp. Cascade (W.Archer 212122)
 sp. Cascade Creek (R.L.Barrett & M.D.Barrett RLB 3738)
 sp. Cascades (M.Hislop 3693)
 sp. Cascades (R.Bruhn 24/899 CAS)
 sp. Cascades (R.Davis 11037)
 sp. Cascades (W.Archer 1110161)
 sp. Castle Tower (A.Bean 480)
@@ -34613,28 +35355,28 @@
 sp. Cataby (F.Hort 1779)
 sp. Cataby (F.Obbens & C.Godden 14. 16)
 sp. Cataby (G.J.Keighery 11009)
 sp. Cataby (G.J.Keighery 5151)
 sp. Cathedral Gorge (F.H.Mollemans 2420)
 sp. Cathedral Rock (K.A.Williams 95303)
 sp. Cattai (Gregson s.n. 28 Aug 1954)
+sp. Cattai (NSW 318983)
 sp. Central (P.K.Latz 17037)
 sp. Central Australia (J.Z.Weber 9460)
 sp. Central Ranges (D.J.Edinger et al. 2420)
 sp. Central Ranges (D.J.Edinger, B.Backhouse & G.Marsh DJE2128)
 sp. Central Wheatbelt (G.Brockman GBB 1161)
 sp. Central Wheatbelt (K.Dixon 861)
 sp. Central Wheatbelt (L.W.Sage, F.Hort, C.A.Hollister LWS2321)
 sp. Central Wheatbelt (M.N. & S.D.Lyons 2760)
 sp. Central ranges (P.K.Latz 8076)
 sp. Central wheatbelt (M.N. & S.D.Lyons 2760)
 sp. Chamaeclada (G.J.Keighery & N.Gibson 1224)
 sp. Chambigne NR (M.Fatemi 24)
 sp. Chandala (G.J.Keighery 17055)
-sp. Channar (M.E.Trudgen 4920)
 sp. Chapman Road (M.E.Trudgen MET 5446)
 sp. Chapple Vale (J.A.Jeanes 344)
 sp. Charles Darwin (J.L.Egan 5300)
 sp. Charmhaven
 sp. Charmhaven (NSW 896673)
 sp. Charnley River (M.D.Barrett MDB 5163)
 sp. Charters Towers (E.J.Thompson+ 347)
@@ -34749,14 +35491,15 @@
 sp. Coolibah Stn (R.Pullen+ 11182)
 sp. Cooljarloo (B.Backhouse s.n. 16/11/88)
 sp. Cooljarloo (B.J.Keighery 28 B)
 sp. Coolmunda (D.Halford Q1635)
 sp. Cooloomia (S.D.Hopper 1353)
 sp. Cooloomia (S.D.Hopper 3301)
 sp. Coolum Beach (P.R.Sharpe 2314)
+sp. Cooma (J.H.Maiden NSW642748)
 sp. Coomallo (L.Haegi 2677)
 sp. Coomallo (R.J.Cranfield 1457)
 sp. Coomberdale (M.E. & M.E.Trudgen MET 1724)
 sp. Coondewanna Flats (S.van Leeuwen 4684)
 sp. Coondewanna Flats (S.van Leeuwen 975)
 sp. Coonjimba Billabong (T.S.Henshall 3365)
 sp. Cooper Creek
@@ -34778,15 +35521,15 @@
 sp. Coraginaensis (K.R.Newbey 7477)
 sp. Cordata (J.Russell-Smith 7211)
 sp. Cordate-leaved (H.P.Vonow 810)
 sp. Cordifolia (C.A.Gardner 2712)
 sp. Cordillo Downs (B.Lay 1487)
 sp. Corky Bark
 sp. Corrigin (K.Kershaw & L.Kerrigan KK2091)
-sp. Corrigin (K.Kershaw KK2091)
+sp. Corrigin (K.Kershaw KK 2091)
 sp. Corrigin (T.Erickson TEE 308)
 sp. Corunna (D.E.Symon 17088)
 sp. Cotton Island (J.Russell-Smith 5050)
 sp. Coujinup (M.A.Burgman 1085)
 sp. Coujinup Hill (M.A.Burgman 1560)
 sp. Cowcowing (Wittwer W 1210)
 sp. Cowley Beach (C.Puttock & A.Graham UNSW14851)
@@ -34908,14 +35651,15 @@
 sp. Dave's Creek (P.I.Forster+ PIF15979)
 sp. Davenport Ranges (C.R.Dunlop 6042)
 sp. Davenport Ranges (D.E.Albrecht 10005)
 sp. Davies Creek (J.G.Tracey 14745)
 sp. Davies Creek (L.J.Webb+ 6430)
 sp. Davies Creek (R.L.Jago 3758)
 sp. De Grey (A.A.Mitchell PRP1940)
+sp. De Grey River (M.D. Barrett & B.M. Anderson MDB 4432)
 sp. Deaf Adder Gorge (C.R.Dunlop 4403)
 sp. Deaf Adder Gorge (C.R.Dunlop 4444)
 sp. Deception Hill (J.Warden & E.Ager LCH 31691)
 sp. Decipiens (G.J.Keighery 463)
 sp. Decipiens (Peter G.Wilson & J.Palmer PGW 1777)
 sp. Decumbent (P.Martensz 513)
 sp. Decussate (R.J.Chinnock 7735)
@@ -34980,14 +35724,15 @@
 sp. Douglas Springs (C.R.Michell 2787)
 sp. Douglas Springs (I.D.Cowie 9235)
 sp. Douglas-Denison (R.Schahinger HO526133)
 sp. Dowak (J.M.Fox 86/271)
 sp. Dowerin
 sp. Dowerin (G.Wiehl F 8004)
 sp. Dragon Rocks (A.M.Coates 2609)
+sp. Dragon Rocks (A.M.Coates 2875)
 sp. Dragon Rocks (J.A.Wege & K.A.Shepherd JAW 2054)
 sp. Dragon Rocks (K.Kershaw & L.Kerrigan KK 2180)
 sp. Dragon Rocks (K.Kershaw KK 2184)
 sp. Drajurk (D.T.Rouse 105)
 sp. Dryander Creek (P.R.Sharpe 4184)
 sp. Dryandra (D.M.Rose 397)
 sp. Dryandra (D.Rose 446)
@@ -35040,15 +35785,15 @@
 sp. Earaheedy (I.Kealley IEK 019)
 sp. East Alligator (J.Russell-Smith 8418)
 sp. East Fortescue (J.Bull & D.Roberts ONS A 27.01)
 sp. East Mulgrave River (R.L.Jago et al. 3696)
 sp. East Nabawa (M.E.Trudgen MET 21623)
 sp. East Northcliffe (E.M.Sandiford et al. 2174)
 sp. East Peak (E.D.Middleton EDM 43)
-sp. East Pilbara (A.R.Mitchell PRP 727) WA Herbarium
+sp. East Pilbara (A.R.Mitchell PRP 727)
 sp. East Yuna (A.C.Burns 6)
 sp. East Yuna (J.W.Green 4639)
 sp. East Yuna (R.Spjut & C.Edson 7077)
 sp. Eastern Goldfields (A.Williams 3)
 sp. Eastern Highlands (D.T.Rouse s.n., 2 Dec. 2000)
 sp. Eastern Wheatbelt (C. & D.Woolcock s.n. PERTH 00760846)
 sp. Ebor (P.C.Jobson 5318 & S.A.Mills)
@@ -35057,14 +35802,15 @@
 sp. Echidna (A.R.Annels ARA 5500)
 sp. Echo Point (M.Olsen 801)
 sp. Edaggee Station (T.E.H.Aplin 3208)
 sp. Edah (J. W.Green 1601)
 sp. Edel Land (F.Obbens FO 01/17)
 sp. Edgar Range (S.D.Hopper 1763)
 sp. Edgbaston (R.J.Fensham 3341)
+sp. Edgbaston (R.J.Fensham 5094)
 sp. Edith Falls (D.M.J.S.Bowman 468)
 sp. Edith Falls (K.G.Brennan 7668)
 sp. Edith River (M.Lazarides 124)
 sp. Edkins 3965
 sp. Edkins Range (R.L.Barrett & M.D.Barrett RLB661)
 sp. Edward River (S.Garnett AQ344221)
 sp. Eganu (S.Patrick 4537)
@@ -35118,26 +35864,25 @@
 sp. Eriophylla (J.Stretch s.n. (PERTH 05406110))
 sp. Erubescens (A.A.Mitchell 3371)
 sp. Esmeralda (A.R.Bean 13464)
 sp. Esmeralda Gorge (S.T.Blake 19640)
 sp. Esperance (A.Fairall 2431)
 sp. Esperance (A.G.Gunness AG 2435)
 sp. Esperance (G.Brockman 735)
-sp. Esperance (G.Brockman 735) WA Herbarium
 sp. Esperance (M.A.Burgman 1055 & S.McNee)
 sp. Esperance (M.A.Burgman 1833b)
 sp. Esperance (M.A.Burgman 4268A)
 sp. Esperance (M.E.French 1579)
 sp. Esperance (M.G.Corrick 9558)
 sp. Esperance (N.S.Lander 1080)
 sp. Esperance (P.G.Wilson 7904)
 sp. Esperance (R.J.Cranfield 1370)
 sp. Esperance (W.R.Archer 2512952)
 sp. Esperance Swamps (D.Voigt DLJ6699)
-sp. Eujinyn (J.Buegge D99)
+sp. Eujinyn (J.Buegge D 99)
 sp. Eulo (I.Tambling AQ123784)
 sp. Eulo (M.E.Ballingall MEB 2590)
 sp. Eungella (C.T.White 12994)
 sp. Eungella (W.J.McDonald 5131 & A.R.Bean)
 sp. Eungella NP (P.R.Sharpe+ 5052)
 sp. Eungella Range
 sp. Eurardy (D. & B.Bellairs 1649)
@@ -35242,14 +35987,15 @@
 sp. Fortescue Marsh (A.Markey & S.Dillon FM 9709)
 sp. Fortescue Marsh (K.A.Shepherd et al. 1055)
 sp. Fortescue Marsh (K.A.Shepherd et al. KS 1055)
 sp. Fortescue Valley (M.N.Lyons & R.A.Coppen FV 0760)
 sp. Forty Mile Scrub (B.Hyland 3883RFK)
 sp. Forty Mile Scrub (R.J.Fensham 1113)
 sp. Fractiflexa (S.van Leeuwen 3773)
+sp. Frank Hann (K.Newbey 10900)
 sp. Frank Hann (K.R.Newbey 11499)
 sp. Frank Hann (K.R.Newbey 6688)
 sp. Frankland (E.M.Sandiford EMS 896)
 sp. Frankland (W.Jackson BJ8)
 sp. Frankland National Park (T.D.Macfarlane 2238)
 sp. Fraser Island (P.Baxter 777)
 sp. Fraser Island NP (R.Crane 2063)
@@ -35358,17 +36104,17 @@
 sp. Gnangara (J.R.Wheeler 2329)
 sp. Gnarlbine Rocks (G.Barrett GRH 469)
 sp. Golden Grove (S.J.Patrick 2679)
 sp. Golden calyces glabrous fruit (H.N.Foote)
 sp. Golden calyces pubescent (G.J.Leach 1966)
 sp. Golden hairs (D. & B.Bellairs 1450 A)
 sp. Goldfields (H.Pringle 2188)
+sp. Goldfields (K.R. Newbey 6044)
 sp. Goldfields (P.G.Wilson 7183)
 sp. Goldfields (R.Davis 10796)
-sp. Goldfields Goldfields (K.R. Newbey 6044)
 sp. Goldfields Ranges (N.Gibson & K.Brown 3175)
 sp. Goldsborough Road (L.W.Jessup 748)
 sp. Goodlands (B.R.Maslin 7761)
 sp. Goomalling (A.G.Gunness et al. OAKP 10/63)
 sp. Goongarrie (F.Obbens, F.Hort & J.Hort FO 18/13)
 sp. Goonmirk Rocks (S.J.Forbes 1009)
 sp. Goonoowigall Bushland Reserve (G.J.White NE 66952)
@@ -35388,35 +36134,37 @@
 sp. Graniticola (A.Moscal 4210) Crowden
 sp. Grass Patch (A.J.G.Wilson 110)
 sp. Grass Patch (M.A.Burgman 4431)
 sp. Grassy (E.Gude & J.Harvey 250)
 sp. Graveside Gorge (V.J.Levitzke 806)
 sp. Great Sandy Desert (C.P.Campbell 3689)
 sp. Great Sandy Desert (D.E.Albrecht 10517)
-sp. Great Southern (R.S.Cowan A586)
+sp. Great Southern (R.S.Cowan A-586)
 sp. Great Victoria Desert
 sp. Great Victoria Desert (A.S.George 8219)
 sp. Great Victoria Desert (A.S.George 8406)
 sp. Great Victoria Desert (A.S.Weston 14813)
 sp. Great Victoria Desert (C.Tauss 2835)
 sp. Great Victoria Desert (D.J.Edinger 6212)
 sp. Great Victoria Desert (D.Nicolle & M.French DN 3877)
 sp. Great Victoria Desert (G.J.Keighery 7501)
+sp. Great Victoria Desert (J.Alford s.n. PERTH 09041567)
 sp. Great Victoria Desert (L.Cockram LAC 139)
 sp. Great Victoria Desert (N.Murdoch 44)
 sp. Great Victoria Desert (N.Murdock 44)
 sp. Great Victoria Desert (R.W.Davis 10621)
 sp. Green Bark (B.Hyland 25370RFK)
 sp. Green Hill (S.Paust 1322)
 sp. Greenough River (J.Docherty 169)
 sp. Greenvale (R.J.Fensham 1150)
 sp. Gregory (G.M.Wightman 2823)
 sp. Gregory (M.Hislop 3784)
 sp. Greta Creek (R.J.Lawn+ AQ532201)
 sp. Grey Rhizome (K.L.Wilson 2922)
+sp. Groote Eylandt (C.R.Dunlop 9300 & G.J.Leach)
 sp. Groote Eylandt (D.J.Dixon 1365 & I.D.Cowie)
 sp. Groote Eylandt (R.L.Specht 335)
 sp. Groote Eylandt (R.L.Specht 387)
 sp. Grooved (R.A.Kerrigan 1131)
 sp. Group 1 Fl. Victoria (A.C.Beauglehole 67529)
 sp. Group 2 (N.H.Scarlett 82-199)
 sp. Gunapin (F.Hort 308)
@@ -35452,15 +36200,15 @@
 sp. Hale River (B.G.Thomson 3395)
 sp. Hale River (P.K.Latz 12036)
 sp. Halls Creek (G.W.Carr 3503)
 sp. Halls Creek (L.A.Craven 8170)
 sp. Hamelin (A.M.Ashby 2196)
 sp. Hamelin (Trudgen 8000)
 sp. Hamelin Station (F.Obbens FO 02/20)
-sp. Hamelinensis (G.J.Keighery s.n. (PERTH 02391325))
+sp. Hamelinensis (G.J.Keighery s.n. PERTH 02391325)
 sp. Hamersley (A.S.Weston 8444)
 sp. Hamersley (M.E.Trudgen 11207)
 sp. Hamersley (M.E.Trudgen 11353)
 sp. Hamersley (M.Trudgen 17794)
 sp. Hamersley (M.Trudgen 2302)
 sp. Hamersley (N.McQuoid 379)
 sp. Hamersley Clay (A.A.Mitchell PRP 113)
@@ -35500,15 +36248,15 @@
 sp. Harvey (G.J.Keighery 16821)
 sp. Harvey (M.E.T.Trudgen & A.Tingay)
 sp. Hatter Hill (G.J.Barrett s.n. 15/9/1989)
 sp. Hatter Hill (K.R.Newbey 3284)
 sp. Hatter Hill (K.R.Newbey 6532)
 sp. Hawkesbury (B.J.Conn 2591)
 sp. Hay Flat Road (K.F.Kenneally 11408))
-sp. Hay River (Randino 14)
+sp. Hay River (Raudino 14)
 sp. Headland (G.J.Keighery 8501)
 sp. Heathlands (R.W.Johnson 5134)
 sp. Heathmont (J.C.Reid 2684)
 sp. Hedland
 sp. Helena & Aurora (B.J.Lepschi 2003)
 sp. Helena & Aurora (K.R.Newbey 8972)
 sp. Helena & Aurora Range (B.J.Lepschi 2077)
@@ -35682,15 +36430,15 @@
 sp. Junction Reserve (B.A.Piercey 62)
 sp. Junee Tableland (T.J.McDonald 553)
 sp. Junga (S.D.Hopper 1293)
 sp. Junga Dam (A.G.Gunness 2383 A)
 sp. Junga Dam (D.Bellairs 942)
 sp. Jurien (B.J.Conn 3885 & M.E.Tozer)
 sp. Jurien (G.Lullfitz s.n. 10/7/1986)
-sp. Jurien (R.J.Cranfield & P.Spencer RJC 8443)
+sp. Jurien (R.J.Cranfield & P.J.Spencer RJC 8443)
 sp. Jyndabinbin Rocks (K.R.Newbey 7689)
 sp. K
 sp. K (aff. lanceolatus)
 sp. K (aff. phlogopappa)
 sp. K (aff. semipapposum)
 sp. K Boorabbin (K.L.Wilson 2579)
 sp. K Kimberley Flora
@@ -35799,15 +36547,15 @@
 sp. Kennedy River (J.R.Clarkson 5645)
 sp. Kent River (B.G.Hammersley 1791)
 sp. Kentdale (G.J.Bourke 458)
 sp. Kenwick (G.J.Keighery 10905)
 sp. Kenwick (G.J.Keighery 5179)
 sp. Kettering
 sp. Keysbrook (R.Archer 17/11/99)
-sp. Kilcoy Creek (R.Crane 1286) Qld Herbarium
+sp. Kilcoy Creek (R.Crane 1286)
 sp. Killarney (C.R.Michell 2403)
 sp. Killawarra (A.D.J.Piesse 461)
 sp. Kilsyth South (G.S.Lorimer 1253)
 sp. Kimberley (A.S.George 13193)
 sp. Kimberley (K.F.Kenneally 4857)
 sp. Kimberley (M.D.Barrett 1036)
 sp. Kimberley (R.A.Kerrigan 1111)
@@ -35887,27 +36635,30 @@
 sp. L
 sp. L (A.M.Ashby 4202)
 sp. L (K.R.Newbey 7888)
 sp. L (aff. minimus)
 sp. L Kimberley Flora (A.S.George 13505)
 sp. L Kimberley Flora (E.Langfield 60)
 sp. L Kimberley Flora (K.F.Kenneally 11167)
+sp. L Kimberley Flora (T.G.Hartley 14569)
 sp. L Kimberley Flora (T.G.Hartley 1469)
 sp. Laglan Station (L.S.Smith 10302)
 sp. Laglan Station (L.S.Smith 10325)
+sp. Lajamanu (J.Egan 4317)
 sp. Lake Amadeus (C.L.Spencer 18/07/2000)
 sp. Lake Anneen (A.L.Payne 320)
 sp. Lake Broadwater (K.A.Williams AQ230829)
 sp. Lake Brown (E.Merrall s.n. 1889)
 sp. Lake Buchanan (E.J.Thompson+ BUC2128)
 sp. Lake Buchanan (J.Kemp+ 3384H)
 sp. Lake Buchanan (V.J.Neldner+ 3362)
 sp. Lake Cairlocup (K.Newbey 9834)
 sp. Lake Campion (A.Coates AC 2285)
 sp. Lake Carey (E.Mattiske LM 197)
+sp. Lake Carey (J. Paterson & J.Warden WB 40825)
 sp. Lake Cobham (K.Newbey 3262)
 sp. Lake Cronin (K.R.Newbey 9191)
 sp. Lake Disappointment (S.van Leeuwen 2865)
 sp. Lake Gregory (L.Thomson LXT1336A)
 sp. Lake Innes (D.L.Jones 4920 & M.A.Clements)
 sp. Lake Jasper (B.M.Hammersley 567)
 sp. Lake Johnson (N.Gibson & M.Lyons 1959)
@@ -36154,14 +36905,15 @@
 sp. Mataranka (S.T.Blake 17514)
 sp. Matt Wilson (I.D.Cowie 2446 & P.S.Brocklehurst)
 sp. Maud Creek (C.R.Michell 43)
 sp. Maules Creek (M.V.Robinson s.n., NSW1115296)
 sp. Maxwell River (S.J.Jarman HO314082)
 sp. Maya (R.Davis & P.Jobson RD 12235)
 sp. Maydon (S.Kern, R.Jasper, H.Hughes LCH 17844)
+sp. McArthur River (T.S.Henshall 1619)
 sp. McDermid Rock
 sp. McDermid Rock (A.P.Brown 3615)
 sp. McDonald Downs Station (R.A.Perry 3416)
 sp. McDowall Range (B.Hyland 3938)
 sp. McDowall Range (J.G.Tracey 14552)
 sp. McIlwraith
 sp. McIlwraith (B.Hyland 3295RFK)
@@ -36194,17 +36946,19 @@
 sp. Melville Island (C.R.Dunlop 4609)
 sp. Melville Island (C.R.Dunlop 6556)
 sp. Melville Island (D.T.Liddle et al. 3603)
 sp. Melville Island (J.Russell-Smith 2036)
 sp. Melville Island (J.Russell-Smith 2148)
 sp. Melville Island (N.B.Byrnes 666)
 sp. Melville Island (R.Fensham 1021)
+sp. Melville Island (R.J.Fensham 2909)
 sp. Menai (A.T.Fairley, 15 Dec 2004)
 sp. Menzies (F.Hort et al. FH 4100)
 sp. Merapah (J.R.Clarkson 7142)
+sp. Merluna (B.Hyland 21374V)
 sp. Merredin (B.R.Maslin 586)
 sp. Merredin (G.J.Keighery & N.Gibson 6320)
 sp. Merredin (K.R.Newbey 2506)
 sp. Merredin (M.B.Mills 11)
 sp. Merredin (M.Koch 2959)
 sp. Mertens Falls (K.F.Kenneally 7887)
 sp. Metamorphics (C.R.Michell 2557)
@@ -36285,14 +37039,15 @@
 sp. Morawa (G.J.Keighery & N.Gibson 6759)
 sp. Morawa (M.A.Langley MAL4177)
 sp. Morehead River (J.R.Clarkson+ 8086)
 sp. Moresby Range (A.S.George 14873)
 sp. Moresby Range (R.J.Cranfield 2751)
 sp. Moresby Range (S.Patrick 2614)
 sp. Morgan River (A.T.Cross ATC 62)
+sp. Morgan River (M.D.Barrett 1549)
 sp. Mornington Peninsula (K.Rule 210)
 sp. Mornington Peninsula (V.Stajsic 4293)
 sp. Mortlake (J.A.Jeanes 1892)
 sp. Mosquito Creek (A.A.Mitchell PRP1439)
 sp. Mosquito Creek (A.A.Mitchell et al. AAM 10795)
 sp. Mosquito Point (J.R.Clarkson+ 9991)
 sp. Mosquito Point (J.R.Clarkson+ 9994)
@@ -36303,14 +37058,16 @@
 sp. Mount Bomford (M.D.Barrett 423)
 sp. Mount Boss (P.Gilmour 7907)
 sp. Mount Brockman (R.C.Hinz 362)
 sp. Mount Bundey (C.R.Dunlop 8840)
 sp. Mount Canobolas (R.Coveny 4191b)
 sp. Mount Caroline (S.D.Hopper SDH 6381)
 sp. Mount Coot-tha (J.Conran s.n., 1983)
+sp. Mount Gibbs (G.F.Craig 6668-1)
+sp. Mount Gibson (B.H.Smith 883)
 sp. Mount Groper (R.Cranfield & D.Kabay 9157)
 sp. Mount Heywood (M.A.Burgman 1211)
 sp. Mount Hilditch (M.E.Trudgen 19134)
 sp. Mount House (P.A.Fryxell+ 3961)
 sp. Mount Howship (C.R.Dunlop 6656)
 sp. Mount Isa (L.A.Craven 8566)
 sp. Mount Lesueur (E.A.Griffin 1997)
@@ -36368,14 +37125,15 @@
 sp. Mt Burgess (A.A.Mitchell & P.H.Waddell 10499)
 sp. Mt Burrowa (V.Stajsic 3314 & W.M.Molyneux)
 sp. Mt Carbine (G.P.Guymer 885)
 sp. Mt Carbine (L.W.Jessup+ GJM995)
 sp. Mt Castletower (I.R.Telford 10112)
 sp. Mt Castletower (M.D.Crisp 2753)
 sp. Mt Caudan (N.Gibson & M.Lyons 2081)
+sp. Mt Channar (M.E.Trudgen 4920)
 sp. Mt Channar Range (C.Keating & M.E.Trudgen CK 408)
 sp. Mt Chester (S.Kern et al. LCH 16596)
 sp. Mt Clara (R.J.Cranfield 11693)
 sp. Mt Clara (R.J.Cranfield 11702)
 sp. Mt Clere (R.J.Dadd 5)
 sp. Mt Clifford (B.Severne 74002)
 sp. Mt Clifford (R.Cumming 1267)
@@ -36408,15 +37166,15 @@
 sp. Mt Frankland (L.Graham 2174)
 sp. Mt Fyfe (R.L.Barrett & M.D.Barrett RLB1526)
 sp. Mt Garnet (D.J.Carr+ 1672B)
 sp. Mt Garnet (R.J.Henderson H1690)
 sp. Mt Garnet (R.J.Myers AQ6301)
 sp. Mt Gibbs (G.F.Craig 6658)
 sp. Mt Gibbs (G.F.Craig 7031)
-sp. Mt Gibson (R.D.Hogland 12002)
+sp. Mt Gibson (R.D.Hoogland 12002)
 sp. Mt Gibson (R.Meissner & Y.Caruso 3)
 sp. Mt Gibson (S.Patrick 2098)
 sp. Mt Gilruth (D.L.Jones 1543)
 sp. Mt Glasse (P.G.Wilson 5717)
 sp. Mt Goonanaman (J.Randall 738)
 sp. Mt Goonaneman (J.Randall 738)
 sp. Mt Groper (K.Newbey 11808)
@@ -36445,15 +37203,14 @@
 sp. Mt Isa (P.L.Harris 699)
 sp. Mt Isa (R.L.Specht+ 49)
 sp. Mt Jackson
 sp. Mt Jackson (B.Ryan 176)
 sp. Mt Jackson (G.J.Keighery 4362)
 sp. Mt Jackson (G.J.Keighery 4372)
 sp. Mt Jackson (L.Mattiske 193-2/572)
-sp. Mt Jackson (R.J.Cranfield 7748)
 sp. Mt Johnston (A.R.Annels 5645)
 sp. Mt Kaputar (Jackson 2246)
 sp. Mt Kaputar (W.Schofield NE92414)
 sp. Mt Keith (G.Cockerton & G.O'Keefe 11017)
 sp. Mt King (S.van Leeuwen 3605)
 sp. Mt Kosciusko (B.Gott s.n., 1987)
 sp. Mt Kosciuszko (J.H.Maiden s.n. NSW149268)
@@ -36522,15 +37279,15 @@
 sp. Mt Norman (J.T.Hunter 3847)
 sp. Mt Pilot (A.D.Bishop J298/15-20, NSW 429728)
 sp. Mt Ragged (C.A.Gardner 2860)
 sp. Mt Ragged (K.Newbey 7858)
 sp. Mt Ragged (M.Goods GG 004)
 sp. Mt Ragged (S.Barrett 663)
 sp. Mt Ragged (T.E.H.Aplin 4349)
-sp. Mt Read (R.K.Crowden 0802 006) Tas Herbarium
+sp. Mt Read (R.K.Crowden 0802 006)
 sp. Mt Ridley (W.R.Archer 1210911)
 sp. Mt Ridley (W.R.Archer 510914)
 sp. Mt Robinson (G.Byrne 3537)
 sp. Mt Robinson (S.van Leeuwen 4109)
 sp. Mt Samaria (I.C.Clarke 2737)
 sp. Mt Sanford (R.Rowley 10/4/2002)
 sp. Mt Shadforth (I.R.Telford 11609)
@@ -36547,21 +37304,23 @@
 sp. Mt Success (G.J.Keighery 2299)
 sp. Mt Tinbeerwah (C.Sandercoe C1256)
 sp. Mt Tinbeerwah (C.Sandercoe C1286)
 sp. Mt Tinbeerwah (P.R.Sharpe 4781)
 sp. Mt Tozer (J.R.Clarkson 2196)
 sp. Mt Tozer (L.J.Brass 19348)
 sp. Mt Tozer (L.J.Brass 19483)
+sp. Mt Vernon Station (T.L.Setter 427)
 sp. Mt Walsh (P.I.Forster+ PIF7477)
 sp. Mt White (P.I.Forster 14415)
 sp. Mt Windell (S.van Leeuwen 846)
 sp. Mt Windsor Tableland (L.W.Jessup+ GJM1374)
 sp. Mt Zeil (G.Griffin 05/Oct/91)
 sp. Mt Zero (V.Stajsic 4204)
 sp. Mt. Barney (J.M.Powell 1050)
+sp. Mt. Jackson (R.J.Cranfield 7748)
 sp. Mt. Lewis (B.Hyland 14048)
 sp. Mt. Lewis (B.P.Hyland 579)
 sp. Mt. Mulligan (J.R.Clarkson 5768)
 sp. Mt. Mulligan (J.R.Clarkson 5775)
 sp. Muchea (B.J.Keighery 2458)
 sp. Muddarning Hill (S.D.Hopper 4013)
 sp. Muddy Bay (P.I.Forster+ PIF15313)
@@ -36652,14 +37411,15 @@
 sp. Nalgi (N.T.Burbidge 1317)
 sp. Nambung (R.Spjut & R.Smith s.n. 22/09/1992)
 sp. Nanga (A.S.George 11346)
 sp. Nannup (P.A.Jurjevich 1133)
 sp. Nannup (R.D.Royce 3978)
 sp. Nantglyn (P.I.Forster+ PIF5741)
 sp. Nanutarra (F.Obbens FO 08/18)
+sp. Nanutarra (S. van Leeuwen 5037)
 sp. Napier (D.E.Symon 7015)
 sp. Napier Range (R.L.Barrett et al. RLB 2186 A)
 sp. Narbalek (Hinz 467)
 sp. Narembeen (G.J.Keighery & N.Gibson 3010)
 sp. Narembeen (W.E.Blackall s.n. /09/1929)
 sp. Narkal (B.H.Smith 1440)
 sp. Narrabarba Hill (J.Miles 16-10)
@@ -36711,14 +37471,15 @@
 sp. Ninghan (M.G.Corrick 9332)
 sp. Ninghan Station (A.A.Mitchell 1161)
 sp. Nitmiluk (C.R.Michell 2648)
 sp. Nitmiluk (C.R.Michell 3293)
 sp. Nitmiluk (C.R.Michell 3482)
 sp. Nitmiluk (C.R.Michell 3803)
 sp. Nitmiluk (L.A.Craven 6728)
+sp. Nitmiluk (P.A.Fryxell 4220 & L.A.Craven)
 sp. Nitmiluk large (C.R.Michell 4186)
 sp. Nitmiluk small (C.R.Michell 4181)
 sp. Noccundra (P.Warhurst s.n. Aug 1987)
 sp. Nolba (E.Place s.n. Jan. 1964)
 sp. Nolba (M.E.Trudgen MET21632)
 sp. Nookawarra Station (S.J.J.Davies s.n. 1/3/1960)
 sp. Nooloo Breakaway
@@ -36767,14 +37528,15 @@
 sp. Nullagine (B.R.Maslin 8510)
 sp. Nullo Mountain
 sp. Nullo Mountain (M.A.M.Renner et al. 9034)
 sp. Nundle
 sp. Nunniong (J.R.Turner 1156)
 sp. Nuytsland (A.P.Brown s.n.)
 sp. Nuytsland (G.J.Keighery & J.J.Alford 522)
+sp. Nyabing (A.Coates & J.Ward AC 6030)
 sp. Nymphaea (K.L.Lemson KLL 215)
 sp. O
 sp. O (J.Palmer)
 sp. O (Lochiel)
 sp. O Kimberley Flora
 sp. O Kimberley Flora (B.K.Symon 10226)
 sp. O.T. Station (S.T.Blake 17659)
@@ -36813,14 +37575,15 @@
 sp. Ormeau (L.H.Bird AQ435851)
 sp. Ormiston (H.D.V.Prendegast 66)
 sp. Ostrina (M.Officer 164)
 sp. Otway Coast (D.T.Rouse 96)
 sp. Otway Ranges (D.T.Rouse 113)
 sp. Overlander (M.E.Trudgen 12138)
 sp. Overlander (P.S.Short 2096)
+sp. Oxley Wild Rivers (T.M.Collins 924)
 sp. Oxley Wild Rivers N.P. (L.M.Copeland 3863)
 sp. P
 sp. P (aff. chrysantha)
 sp. P Kimberley Flora (A.J.Ewart s.n.)
 sp. P Kimberley Flora (G.W.Carr 3107 & A.C.Beauglehole 46867)
 sp. P1 small head (M.D.Tindale 166A)
 sp. P122 (B.R.Maslin 4918)
@@ -37060,15 +37823,15 @@
 sp. Q6 (filicaulis ms)
 sp. Q8 (olida Lazarides ms Latz 2015)
 sp. Q9 aff. C. bidwillii
 sp. Qld (Iron Range to Mission Beach, Dunk Island)
 sp. Qld (Iron Range)
 sp. Qld (tropical open forest & dry scrubs)
 sp. Quairading (W.E.Blackall 3261)
-sp. Quartzite (A.M.Buchanan 16828) Tas. Herbarium
+sp. Quartzite (A.M.Buchanan 16828)
 sp. Queen Victoria Rock (K.R.Newbey 6103)
 sp. Queen Victoria Spring (D.Nicolle 524)
 sp. Queen Victoria Springs (D.J.Pearson 2212)
 sp. Quindalup (H.Cole & D.Carter 577)
 sp. Quindanning (K.Smith & P.Johns 231)
 sp. Quobba (H.Demarz 3858)
 sp. Quorrobolong (S.Lewer 40)
@@ -37084,15 +37847,15 @@
 sp. RR
 sp. Rabbit Flat (B.J.Carter 626)
 sp. Rabbit Flat (P.K.Latz 12326)
 sp. Rabbit Flat (P.K.Latz 4530)
 sp. Rabbit Flat (R.B.Major 158)
 sp. Raby Bay (J.Elsol AQ462423)
 sp. Ragged (W.Archer 1509903)
-sp. Rainbow Falls (P.I.Forster PIF13786) Qld Herbarium
+sp. Rainbow Falls (P.I.Forster PIF13786)
 sp. Rainbow Valley (A91207)
 sp. Rainbow Valley (D.E.Albrecht 6601)
 sp. Rainbow Valley (T.S.Henshall 1181)
 sp. Ramingining (J.Russell-Smith 2585)
 sp. Ravensthorpe (A.S.George 616)
 sp. Ravensthorpe (C.F.Craig 6309)
 sp. Ravensthorpe (D.B.Foreman 1207)
@@ -37267,15 +38030,15 @@
 sp. Shark Bay (T.E.H.Aplin 3335)
 sp. Sharp Point (J.R.Clarkson 2101)
 sp. Shaw Island (G.N.Batianoff+ 3360)
 sp. Shay Gap (B.Cook 7)
 sp. Shay Gap (K.R.Newby 10293)
 sp. Shay Gap (L.A.Craven 7558)
 sp. Sheoak Hill (K.R.Newbey 8003A)
-sp. Sheoaks Rocks (M.E.Trudgen MET5452)
+sp. Sheoaks Rocks (M.E.Trudgen MET 5452)
 sp. Sherwood Breakaways (R.J.Cranfield 6771)
 sp. Shiptons Flat
 sp. Shiptons Flat (L.W.Jessup+ GJD3200)
 sp. Shoemaker Levy (L.Ang & O.Davies 10815)
 sp. Short Calyx (S.T.Blake 20451)
 sp. Short inflorescence (R.A.Kerrigan 595)
 sp. Short leaf (J.Russell-Smith 5193)
@@ -37293,14 +38056,15 @@
 sp. Silver Plains (P.I.Forster PIF17005)
 sp. Silvergrass (P.-L.de Kock BES 00808)
 sp. Simple-haired calyx (D.E.Symon 8875)
 sp. Simpson Desert NP (R.G.Atherton 8)
 sp. Simpson Desert dunes (P.K.Latz 18008)
 sp. Single NP (L.M.Copeland 2009)
 sp. Sinuate (T.G.Hartley 14337)
+sp. Skeleton (A.A.Mitchell 915)
 sp. Slate (D.L.Jones 16267)
 sp. Slate Buds (R.Bates 64092)
 sp. Slender Snail Orchid (G.J.Keighery 14516)
 sp. Slender Sun Orchid (A.R.Annels 2884)
 sp. Small Flower (B.Gray 5657)
 sp. Small Red-leaved Wattle (J.B.Williams 95033)
 sp. Small lobes (R.A.Kerrigan 754)
@@ -37334,35 +38098,36 @@
 sp. South Molle Island (J.A.Gresty AQ208995)
 sp. South Obelisk (A.S.Benwell 204)
 sp. South Percy Island (G.N.Batianoff+ 11444)
 sp. South West (G.J.Keighery 343)
 sp. South West (K.L.Wilson & K.Frank KLW 9266)
 sp. South Wubin
 sp. South Wubin (R.Davis 10648)
+sp. South coast (G.Byrne 5133)
 sp. South coast (R.Davis 10239)
 sp. South-east Highlands (N.G.Walsh 811)
 sp. South-west Swamps (A.C.Beauglehole 22255)
 sp. South-west swamps (B.G.Hammersley 1010)
 sp. South-west swamps (D.T.Rouse 126)
 sp. Southeast (R.Bates 66283)
 sp. Southern Coast (A.S.George 289)
 sp. Southern Cross (D.Nicolle & M.French DN 3480)
 sp. Southern Cross (G.Cockerton et al. WB 38518)
 sp. Southern Forests (B.G.Hammersley 1000)
 sp. Southern Goldfields (D.Nicolle & M.French DN 3652)
-sp. Southern Granite (E.D.Middleton EDM266)
+sp. Southern Granite (E.D.Middleton EDM 266)
 sp. Southern Granites (W.Jackson BJ256)
 sp. Southern Wheatbelt (C.A.Gardner & W.E.Blackall 1412)
 sp. Southern smooth-bark (D.Nicolle & M.French DN 6916)
 sp. Southern wheatbelt (D.Nicolle & M.French DN 5507)
 sp. Southport (W.M.Curtis 5/12/58)
 sp. Southwest (G.J.Keighery 5677)
 sp. Spade-leaf (I.Crawford 5473)
 sp. Sparkle Hill (M.A.Burgman 2690)
-sp. Sparse pinnae (C.R.Michel 2202)
+sp. Sparse pinnae (C.R.Michell 2202)
 sp. Spear Hill (B.R.Maslin 5266)
 sp. Spicata
 sp. Spirit Hills
 sp. Spirit Hills (D.J.Dixon 1632)
 sp. Spirit Hills (R.K.Harwood 548)
 sp. Splitters Creek 1 (W.Molyneux 30 Apr. 1986)
 sp. Splitters Creek 2 (J.H.Willis 3 Dec. 1962)
@@ -37412,23 +38177,23 @@
 sp. Style-topped fruit (M.Maier BES MM 1017)
 sp. Subalpine (N.G.Walsh 5149)
 sp. Subdecumbens (G.J.Keighery 5390)
 sp. Subglabriphylla (N.Lothian 5277)
 sp. Subteretifolia (K.R.Newbey 10924)
 sp. Subulata (T.R.Lally & B.J.Lepschi 1091)
 sp. Sudley (A.Gunness 1886)
-sp. Sugarloaf (A.Moscal 8301) Tasmanian Herbarium
+sp. Sugarloaf (A.Moscal 8301)
 sp. Suggan Buggan (J.Turner 211)
 sp. Sullivan Soak (D.Nicolle & M.French DN 5503)
 sp. Summerdell (E.R.Anderson 3696)
 sp. Sunrise Hill (M.A.Burgmann 4484)
 sp. Sunshine Lake (K.A.Shepherd et al. KS 867)
 sp. Suplejack Station (P.K.Latz 8184)
+sp. Suplejack Station (T.S.Henshall 2345)
 sp. Supplejack Station (P.K.Latz 8184)
-sp. Supplejack Station (T.S.Henshall 2345)
 sp. Swallow Rock (K.R.Newbey 9677)
 sp. Swamp (D.E.Murfet 1950b)
 sp. Swamp (N.M.Smith 3022)
 sp. Swamp Form (N.Gibson & M.Lyons 544)
 sp. Swan Reach (R.Bates 21370)
 sp. Swan Region (G.B.Brockman 1082)
 sp. Sweet Webb (R.J.Chinnock 8266)
@@ -37455,24 +38220,26 @@
 sp. Tanami (D.E.Albrecht 6176)
 sp. Tanami (P.K.Latz 11904)
 sp. Tanami (P.K.Latz 8218)
 sp. Tanami (P.K.Latz 9906)
 sp. Tanguin Hill (K.R.Newbey 10501)
 sp. Tanumbirini (B.A.Wilson 187)
 sp. Tara (D.Halford Q2259)
+sp. Taravale (J.E.Kemp+ 20074),
 sp. Tarin Rock (D.Nicolle & M.French DN 3759)
 sp. Tarin Rock (E.J.Croxford 2118)
 sp. Tarin Rock (E.J.Croxford 5251)
 sp. Tarin Rock (H.Demarz 1041)
 sp. Tarin Rock (W.E.Blackall 1315)
 sp. Tasmania (J.R.Hosking 1551)
 sp. Tasmania (N.Brittan s.n.)
 sp. Tasmania aff. oblonga (A.M.Gray 22495)
 sp. Tathra (M.A.Langley & J.M.Harvey 1873)
 sp. Tathra (M.Hislop 2900)
+sp. Tawallah Ck (P.K.Latz 14542)
 sp. Tea Tree Road (O.Davies OD 171)
 sp. Tee Dee Hills (P.S.Brocklehurst 606)
 sp. Telford CBG7702560
 sp. Tempe Downs (P.K.Latz 15623)
 sp. Temple Bay (J.R.Clarkson 2175)
 sp. Temple Bay (P.I.Forster PIF8975)
 sp. Temple Bay (P.I.Forster PIF8980)
@@ -37491,15 +38258,17 @@
 sp. Theda (K.Menkhorst s.n. 18/04/1988)
 sp. Theda (M.D.Barrett & R.L.Barrett MDB 2144)
 sp. Theda (M.D.Barrett 1575)
 sp. Theda (M.D.Barrett 1578 B)
 sp. Theda (M.D.Barrett MDB 2056)
 sp. Theda (M.D.Barrett MDB 2063)
 sp. Theda (M.D.Barrett MDB1661)
+sp. Theda (R.L.Barrett & M.D.Barrett RLB 3220)
 sp. Theda (R.L.Barrett et al. RLB 6158)
+sp. Theda Station (R.L.Barrett & M.D.Barrett RLB 3285)
 sp. Thevenard Island (M.White 050)
 sp. Thick sepals (A.E.Orchard 1547)
 sp. Thomas River (A.Case & B.Cole 58)
 sp. Thornton Peak (L.J.Brass+ 249)
 sp. Thornton Peak (S.F.Kajewski 1492)
 sp. Thredbo River Gorge (L.A.S.Johnson & E.F.Constable s.n., 19 Jan 1951)
 sp. Three Springs (D.Jones s.n.)
@@ -37520,14 +38289,15 @@
 sp. Tinaroo Hills (S.T.Blake 14752A)
 sp. Tinaroo Range (V.K.Moriarty 302)
 sp. Tingoora (A.R.Bean 10311)
 sp. Tiny white (R.Bates 41056)
 sp. Tipperary (C.S.Robinson 297)
 sp. Tipperary (G.J.Leach 2152)
 sp. Tiwi Islands (J.Russell-Smith 8240)
+sp. Tobermorey (B.G.Thomson 2360)
 sp. Tobermorey Station (D.E.Albrecht 6322)
 sp. Todd River (G.Chippendale 482)
 sp. Tolmer (C.R.Dunlop 6787)
 sp. Tom Price (M.E. Trudgen 11246)
 sp. Tomoulin (J.R.Clarkson 5122)
 sp. Toodyay (F.Hort 2689)
 sp. Toodyay (G.J.Keighery & N.Gibson 2918)
@@ -37548,14 +38318,15 @@
 sp. Torrington (L.M.Copeland Feb/1997)
 sp. Tortile (G.J.Keighery 3767)
 sp. Tower LA (P.I.Forster+ PIF14846)
 sp. Tozer Gap (L.J.Brass 19441)
 sp. Tozer Range (L.J.Brass 19393)
 sp. Tozer's Gap (L.J.Brass 19024)
 sp. Trayning (A.M.George 97)
+sp. Trayning (W. Johnston WJ 071)
 sp. Tree form (J.B.Williams NE7973)
 sp. Treeton (B.J.Keighery & N.Gibson 564)
 sp. Trent River (K.F.Kenneally 11701)
 sp. Triangolensis (D.F.Blaxell 2059 & L.A.S.Johnson)
 sp. Trichopoda (J.H.Maiden & J.L.Boorman s.n. 40290)
 sp. Trigwell Bridge (R.Smith s.n. 20.6.1989)
 sp. Trigwell Bridge (R.Smith s.n., 20/6/1989)
@@ -37612,23 +38383,26 @@
 sp. Varley (M.Hislop 3659)
 sp. Vasse (C.Wilkins & K.Shepherd CW581)
 sp. Veined Leaf (R.J.Bates 59781)
 sp. Veneta (R.J.Chinnock 8250) R.Chinnock
 sp. Vernicosa (W.E.Blackall 3937)
 sp. Victoria (J.Coleby-Williams 99)
 sp. Victoria Desert (R.Davis et al. RD 11611)
+sp. Victoria Range (J.A.Jeanes 2095 & D.Naqvi)
 sp. Victoria Range (V.Stajsic 4207)
 sp. Victoria River
+sp. Victoria River (I.D.Cowie 5058)
 sp. Victoria River (I.D.Cowie 9193)
 sp. Vigintimilia (P.G.Wilson 7940)
 sp. Violet Town (C.Findlay & G.Backhouse s.n. 26/9/1999)
 sp. Virolens (G.J.Keighery 12000)
 sp. Volcanic Lakes (V.Stajsic 3453)
 sp. Volcanic Plain (V.Stajsic 3673)
 sp. W
+sp. W Hamersley Range (S.Colwill & B.Duncan LCR99-01)
 sp. W Kimberley Flora (C.A.Gardner 10260)
 sp. WL 1 sensu Thomasson & Tyler 1971
 sp. Waaje (A.Bean 19)
 sp. Wadbilliga (Rodd 6168)
 sp. Wade Creek (C.A.Gardner 1534)
 sp. Wagerup (L.Johnson 9127 & B.Briggs)
 sp. Wagga Wagga (G.Burrows 13)
@@ -37660,16 +38434,17 @@
 sp. Wandana (M.E.Trudgen 22016)
 sp. Wandering (F. & J.Hort 3181)
 sp. Wandering (F.Hort 3273)
 sp. Wandering (F.Hort 419)
 sp. Wandoo (F. & J.Hort 2441)
 sp. Wandoo (F.Hort 153B)
 sp. Wandoo (G.Brockman GBB 671)
-sp. Wandoo (V.Crowley DKN700)
+sp. Wandoo (V.Crowley DKN 700)
 sp. Wandoo Beard Orchid (D.M.Rose 344)
+sp. Wangi (S.E.Pickering 20)
 sp. Wanna
 sp. Wanna (M.J.Greeve & J.D.Start D7 44)
 sp. Wanna Munna Flats (S.van Leeuwen 4662)
 sp. Wanneroo (G.J.Keighery 16705)
 sp. Waratah trig (J.B.Williams NE85940)
 sp. Warburton (A.A.Munir 5209)
 sp. Warburton (A.S.George 8164)
@@ -37690,28 +38465,30 @@
 sp. Warren (M.McCallum Webster 23/2/1979)
 sp. Warren Road (M.N.Lyons 2710)
 sp. Warriedar (A.P.Brown & S.Patrick APB 1100)
 sp. Warriedar (F.Obbens 04/09)
 sp. Warriedar (G.J.Keighery 12448)
 sp. Warriedar (P.G.Wilson 12267)
 sp. Warriedar (S.Patrick 1978A)
+sp. Warwick (F.M.Bailey AQ89020)
 sp. Watalgan (A.R.Bean 8611)
 sp. Watarrka (A.C.Beauglehole 20471)
 sp. Watarrka (D.E.Albrecht 8672)
 sp. Watchimbark (P.Gilmour 7938)
 sp. Waterholes (R.Bates 9037) R.J.Bates
 sp. Waterhouse Range (S.McAlpine s.n.)
 sp. Waterloo (G.J.Keighery 13724)
 sp. Watheroo (D.Foreman 477)
 sp. Watheroo (I.R.McGill 20)
 sp. Watheroo (K.M.Allan 57)
 sp. Watheroo (K.Shepherd & C.Wilkins KS 220)
 sp. Watheroo (R.D.Royce 9616)
 sp. Watheroo (R.D.Royce 9625)
 sp. Watheroo (R.J.Cranfield & P.J.Spencer 8183)
+sp. Watheroo (S.D.Hopper 7668)
 sp. Watheroo (S.Hancocks 4)
 sp. Watson River (J.R.Clarkson 4075A)
 sp. Watsonville (P.I.Forster PIF6259)
 sp. Waychinicup (D.Davidson s.n. PERTH 01486527)
 sp. Waychinicup (E.M.Sandiford EMS 1336)
 sp. Weam Reserve (M.Hislop 2755)
 sp. Weelarrana (M.N.Lyons & S.D.Lyons 3050)
@@ -37774,16 +38551,16 @@
 sp. White Mountains (R.J.Cumming+ 19025)
 sp. Whitfield Range (R.Jago 17)
 sp. Whitsundays (W.J.McDonald+ 5831)
 sp. Whoogarup Range (A.S.George 1910)
 sp. Whyanbeel
 sp. Whyanbeel (B.P.Hyland RFK1106)
 sp. Whyanbeel (G.P.Guymer 2059)
-sp. Wiakli (G.M.Storr s.n. 4/10/1958)
 sp. Wialki (B.H.Smith 482)
+sp. Wialki (G.M.Storr s.n. 4/10/1958)
 sp. Wiangaree SF, NSW, P.Hind 2568
 sp. Wiangaree SF, NSW, P.Hind 2750
 sp. Widgiemooltha (F.Obbens & E.Reid FO 9/05)
 sp. Wielangta (M.Wapstra 934)
 sp. Wielangta (M.Wapstra 935)
 sp. Wildflower Show (?A.M.Coates S 4407)
 sp. Wilgie Mia (D.Coultas & G.Woodman AW 03-Opp1)
@@ -37881,14 +38658,15 @@
 sp. Yalgorup (B.J.Keighery & N.Gibson 897)
 sp. Yalgorup (G.Brockman GBB463)
 sp. Yalgorup (G.J.Keighery 14455)
 sp. Yalgorup (M.E.Trudgen 12196)
 sp. Yalgorup (M.E.Trudgen)
 sp. Yalgorup National Park (G.J.Keighery 14449)
 sp. Yampi (A.N.Start per R.L.Barrett RLB 2291)
+sp. Yampi Peninsula (A.J.M.Hopkins BA 0248)
 sp. Yampi Peninsula (R.L.Barrett & A.N.Start RLB 2280)
 sp. Yanchep (G.J.Keighery 11242)
 sp. Yanchep (M.Hislop 1986)
 sp. Yanchep (R.Davis 11129)
 sp. Yandanooka (M.Hislop 2507)
 sp. Yandanooka (R.Soullier 421)
 sp. Yandanooka (R.Soullier 646)
@@ -38043,14 +38821,15 @@
 sp. aff. T. laxiflora
 sp. aff. T. livescens
 sp. aff. abbreviatum
 sp. aff. acicularis (Maiden 1904)
 sp. aff. aciculiformis
 sp. aff. aciculiformis (Beechworth)
 sp. aff. aciculiformis (Stawell)
+sp. aff. acmenoides
 sp. aff. acradenia
 sp. aff. acutangula (S.T.Blake 17630)
 sp. aff. affinis
 sp. aff. affinis (Nunniong Plateau)
 sp. aff. alata (Coastal)
 sp. aff. alata (New England)
 sp. aff. alata (Woronora Plateau)
@@ -38072,25 +38851,25 @@
 sp. aff. angustum
 sp. aff. apetala (Coastal)
 sp. aff. aphylla
 sp. aff. aquifolium (Anglesea)
 sp. aff. armigera
 sp. aff. arrectum (Mt Kaputar)
 sp. aff. atrox (Kirramingly N.R., L.M.Copeland 4422)
-sp. aff. attenuata
 sp. aff. australasica (Qld)
 sp. aff. australiensis
 sp. aff. australis
 sp. aff. australis (Berrigan)
 sp. aff. axillaris
 sp. aff. axillaris (Wimmera)
 sp. aff. baxteri (Grampians)
 sp. aff. bialata
 sp. aff. bicolor
 sp. aff. bicolor (Woorndoo)
+sp. aff. bidwillii
 sp. aff. bioculatum
 sp. aff. biserratus (Montane)
 sp. aff. biseta (Grampians)
 sp. aff. biseta (Lara)
 sp. aff. biseta (Pink Lakes)
 sp. aff. biseta (Striped)
 sp. aff. biseta (Wimmera River)
@@ -38289,14 +39068,15 @@
 sp. aff. lacunarius
 sp. aff. lamellate
 sp. aff. lanceolata
 sp. aff. lanceolata (Derrinallum)
 sp. aff. lanceolata (Laverton)
 sp. aff. lanceolata (Wonnangatta)
 sp. aff. lanuginosa (Mornington Peninsula)
+sp. aff. lasioclada
 sp. aff. lawrencei (Goonmirk Rocks)
 sp. aff. leiophylla
 sp. aff. lenticulare
 sp. aff. lindleyana (Beechworth)
 sp. aff. linearis
 sp. aff. linifolia (Grampians)
 sp. aff. longifolia (Benambra)
@@ -38459,15 +39239,14 @@
 sp. aff. pentandra (Koolan Island)
 sp. aff. pentandra (Mitchell Plateau)
 sp. aff. petilum
 sp. aff. petilum 1
 sp. aff. petilum 2
 sp. aff. picta
 sp. aff. pinifolia
-sp. aff. pisum
 sp. aff. placosporum
 sp. aff. plagiostomum
 sp. aff. plumosa (Anglesea)
 sp. aff. plumosa (Mallee)
 sp. aff. plumosa (Sydney)
 sp. aff. plumosa (Woodland)
 sp. aff. plumosa 1
@@ -38741,20 +39520,24 @@
 sp. nov. 'Belowra'
 sp. nov. 'Nullica'
 sp. nov. 'Yowaka'
 sp. nov. 'costata'
 sp. nov. 'longiflorum' [E.A.Brown et al], ms. (E.A.Brown 97/51)
 sp. nov. (A.S.Mitchell, 1976)
 sp. nov. (Bankstown Airport)
+sp. nov. (Crystal Creek)
 sp. nov. (Dome Mountain)
+sp. nov. (Dorrigo)
 sp. nov. (East Gippsland)
+sp. nov. (GJK/J. Alford 1951)
 sp. nov. (Little Desert)
 sp. nov. (Mt William)
 sp. nov. (NG & ML 1776)
 sp. nov. (New England NP)
+sp. nov. (New England)
 sp. nov. (Nightcap Range)
 sp. nov. (P. gilesii)
 sp. nov. (P.H.Weston 2464)
 sp. nov. (Willi Willi)
 sp. nov. (aff. laurina)
 sp. nov. 1
 sp. nov. ?
@@ -38796,15 +39579,14 @@
 sp. nova aff. heterophylla
 sp. nova aff. lissocarpha
 sp. nova aff. petiolaris
 sp. nova aff. propinqua
 sp. nova aff. spinulosa (Cockleshell Gully)
 sp. nova aff. spinulosa (Newdegate/Lake King)
 sp. oblong (C.R.Dunlop 3260)
-sp. of Bougher (2007: Bougher E3689, PERTH)
 sp. on <I>Heteropogon contortus</I> of Langdon & Parbery (1963).
 sp. ornate labellum (A.P.Brown 869)
 sp. outer wheatbelt (M.Hislop 30)
 sp. papillose leaves (K.R.Newbey 11110)
 sp. prostrate (L.A.Craven 5850)
 sp. red flowered (W.Jackson BJ269)
 sp. ridged papillate (M.Hislop & E.Hudson MH161)
@@ -38824,29 +39606,28 @@
 sp. sensu Croome et Fabbro
 sp. sensu Dingley 2001
 sp. sensu M.Dingley 2001
 sp. sessile leaf (J.L.Robson 657)
 sp. short sepals (W.Jackson BJ259)
 sp. short style (S.Barrett 1578)
 sp. silver leaf (T.E.H.Aplin 6300)
-sp. skeleton (A.A.Mitchell 915)
 sp. small flowers (K.F.Kenneally 7705)
 sp. small fruits (Symon 2338)
 sp. small stature (W.Jackson BJ303)
 sp. smooth culms (Newbey 7823)
 sp. smooth seed (C.R.Michell 2286)
 sp. south coast (P.S.Short 3895)
 sp. south coast (R.T.Wills 1423)
 sp. south coast (T.R.Lally 1576 & I.P.Lally)
 sp. south-coast variant (M.Carter 180)
 sp. southern (L.A.Orthia 39)
 sp. southern granites (G.J.Keighery 11266)
 sp. southern gypsum (M.N.Lyons 2964)
 sp. southern ranges (T.E.H.Aplin 2108)
-sp. sparse pinnae (C.R.Michel 2202)
+sp. sparse pinnae (C.R.Michell 2202)
 sp. spiciform panicles (E.Leyland s.n. 14/8/1990)
 sp. spinifex dweller (I.Morris 6/4/02 ex CANB)
 sp. staminodes (A.Strid 21584)
 sp. star calyx (M.Lazarides 9135)
 sp. stellate (A.Strid 21885)
 sp. striped sepal greenhood (G.Brockman GBB355)
 sp. thickened testa (I.D.Cowie 2472)
@@ -38857,15 +39638,16 @@
 sp. viscid (K.M.Manning 16/June/87)
 sp. wandoo (J. & F.Hort 456)
 sp. white (C.A.Gardner s.n.)
 sp. wing tips (M.E.Trudgen 12044)
 sp. woolly culms (P.K.Latz 10065)
 sp. wrinkled seed (F.Mueller s.n.)
 sp. yellow eared (W.Jackson BJ359)
-sp.' LC1' (Young 2188)
+sp. ‘Clade 5’ sensu Telle et al. (2011)
+sp. ‘Clade 8’ sensu Telle et al. (2011)
 sp.' Russell River' (S.Johnson s.n. 1892)
 sp.'inland'
 sp., No. 264
 sp., Pine Creek (Australia)
 sp.1 sensu Sullivan et al (1988)
 sp.12 (Mount Victoria Uranium Mine; R.Bates 167)
 sp.16 (Arthur River; DLJ13668 ex L.Rubenach s.n.)
@@ -38884,23 +39666,26 @@
 spanogheanum
 spanomerus
 sparagosa
 sparassoides
 spareopsis
 spargenosa
 sparkesii
+sparksii
+sparmanni
 sparmannii
 sparrmanii
 sparrmanni
 sparsa
 sparshottiorum
 sparsicoma
 sparsiflora
 sparsiflorum
 sparsifolia
+sparsifoliae
 sparsifolium
 sparsisora
 sparsisorum
 sparsum
 sparsus
 spartea
 spartella
@@ -38917,14 +39702,15 @@
 spathacei
 spathaceus
 spatheus
 spathularia
 spathulata
 spathulatum
 spathulatus
+spathuliappendiculata
 spathulifera
 spathulifolia
 spathulifolium
 spathulifolius
 spathuliloba
 spathulistipa
 spathulistipus
@@ -38959,29 +39745,30 @@
 spectabile
 spectabilis
 spectablis
 spectatissima
 spectatrix
 spectra
 spectrum
+speewahensis
 spegazziniana
 spegazzinianum
 speirea
 speireus
 speirostega
 speirostichellum
 speirostichum
 spelaeus
 speleotis
 speluncae
+spenceae
 spencerana
 spenceri
 spenceriana
 spencerianus
-spencerii
 spergula
 spergulacea
 spergularina
 spergularinum
 spermacocea
 spermacociodes
 spermacocoides
@@ -39030,14 +39817,16 @@
 sphaerospora
 sphaerosporum
 sphaerosporus
 sphaerostachya
 sphaerostachyum
 sphaerotheca
 sphaerula
+sphagneti
+sphagneticolae
 sphagni
 sphagnicola
 sphagnophila
 sphalerostichum
 sphenandra
 sphenandrum
 spheniscispora
@@ -39132,14 +39921,15 @@
 spinulosperma
 spinulosum
 spinulosus
 spirafolia
 spirale
 spiralis
 spirifolia
+spirillospora
 spiripennatum
 spiritus
 spiroda
 spirographidis
 spirogyra
 spirogyrae
 spiroides
@@ -39159,14 +39949,15 @@
 spitzbergense
 splachnicarpa
 splachnicarpon
 splachnifolius
 splachnirima
 splachnirimus
 splachnoides
+splattiae
 splendens
 splendens x heterophyllus
 splendida
 splendidula
 splendidulum
 splendidum
 splendidus
@@ -39199,17 +39990,19 @@
 spongipes
 spongolitica
 spongoliticum
 sponiae
 spontaneum
 spooneri
 sporadica
+sporadicae
 sporadicus
 sporadotrichum
 sporoboli
+sporobolicola
 sporoboloides
 sporobolus
 sporodochiale
 spp.
 spp. aff. biseta
 spp. sensu Croome et Fabbro 2005
 spraguei
@@ -39228,15 +40021,17 @@
 spumosa
 spumosum
 spumosus
 spurcus
 spuria
 spurium
 spurius
+spyridicola
 spyridii
+spyridiicola
 spyridioides
 sqarrosus
 squalida
 squalidum
 squallidiusculum
 squamaeformis
 squamaria
@@ -39336,17 +40131,17 @@
 stanthorpensis
 stantonii
 stapfiana
 stapfii
 staphylea
 staphyleoides
 staphylioides
+starckeana
+starckeanum
 staringii
-starkeana
-starkeanum
 starkei
 starmachii
 starteorum
 startii
 startiorum
 staticiformis
 statteranum
@@ -39356,28 +40151,30 @@
 stauroglossa
 stauroneiformis
 staurophora
 staurophorum
 staurophylla
 staurophyllum
 stauroptera
+stawelli
 stawellii
 stebbinsii
 steedmani
 steedmanii
 steenisii
 steereana
 steetziana
 steetzianum
 steetzii
 steezii
 stegasauroides
 steiglitziana
 steinii
 steinmanni
+stellae
 stellapilis
 stellarioides
 stellaris
 stellata
 stellaticeps
 stellatifolium
 stellatisporus
@@ -39391,14 +40188,15 @@
 stelligerum
 stelligerus
 stellinum
 stellulata
 stellulatum
 stellulatus
 stelluligera
+stemaria
 stemonea
 stenandra
 stenandrus
 stenanthum
 stenobotrya
 stenocalyx
 stenocarpa
@@ -39500,15 +40298,14 @@
 stichodonta
 stictaeformis
 stictathecium
 stictica
 sticticum
 sticticus
 stictideum
-stictoideus
 stictophylla
 stictus
 stigma
 stigmaea
 stigmatea
 stigmatella
 stigmaticum
@@ -39585,14 +40382,15 @@
 stoloniferus
 stolterfothii
 stomarrhena
 stomatophora
 stoneae
 stoneana
 stonei
+stonesiae
 stoniella
 stopfordi
 stopfordii
 storckii
 storyi
 stoschii
 stoveae
@@ -39753,14 +40551,15 @@
 stuntzii
 stupefactum
 stuposa
 stuposum
 stuposus
 stupposa
 sturgissiana
+sturti
 sturtianum
 sturtii
 stutzeri
 stygia
 stygiodes
 stygium
 stygius
@@ -39773,33 +40572,34 @@
 styliformis
 stylobates
 stylophora
 stylophorus
 stylorum
 stylosa
 stylosanthoides
+stylospora
 stylosum
 stylosus
 stylotricha
 styotricha
 styotrichum
 stypandroides
 stypheleoides
 stypheliodes
 styphelioides
+stypheloides
 stypophylla
 styriaca
 suaderis
 suaedacea
 suaedae
 suaedae-australis
 suaedaefolium
 suaedifolia
 suaedifolium
-suatinum
 suave
 suaveolens
 suaveolensis
 suaveolente
 suavis
 suavissima
 suavissimum
@@ -39823,14 +40623,15 @@
 subaggregans
 subaggregatum
 subalaris
 subalatum
 subalatus
 subalbicans
 subalbida
+subalbovinosa
 subalbula
 subalopecuroides
 subalpina
 subalternans
 subalutacea
 subalutaceum
 subammophila
@@ -39873,14 +40674,15 @@
 subarticulata
 subarvinaceus
 subasbolodes
 subascendens
 subassentiens
 subasterospora
 subastroidea
+subasymmetrica
 subathallina
 subatomoides
 subatrata
 subatratus
 subatropurpureum
 subattenuata
 subattenuatus
@@ -40045,22 +40847,20 @@
 subdentata
 subdentatum
 subdentatus
 subdenticulata
 subdenticulatum
 subdepressa
 subdepressum
-subdescendens
 subdichotomum
 subdigitata
 subdimidiatum
 subdiscordans
 subdiscreta
 subdispersum
-subdissecta
 subdisticha
 subdistichum
 subdistorta
 subdita
 subdividens
 subdomokosii
 subdryophila
@@ -40078,44 +40878,48 @@
 suber
 suberadicata
 suberea
 suberecta
 suberectum
 suberectus
 subericinum
+subericola
 suberosa
 suberosum
 suberosus
 suberythrocarpulum
 suberythrocarpum
 subexasperata
 subexcisa
 subexigua
 subexilis
 subexserens
 subextenuatum
+subfabacearum
 subfalcata
 subfalcatulum
 subfalcatum
 subfalcatus
 subfallens
 subfarcinata
 subfarcinatus
 subfarinosa
 subfascicularis
 subfasciculata
 subfasciculatum
 subfasciculatus
 subfatiscens
+subferruginea
 subflaccida
 subflaccidum
 subflava
 subflavidum
 subflavidus
 subflavifolium
+subflavospora
 subflavovirens
 subflavus
 subflexuosa
 subflexuosum
 subflexuosus
 subfloccosa
 subfloccosus
@@ -40175,14 +40979,15 @@
 subhexagona
 subhirsuta
 subhirtella
 subhorizontalis
 subhuelphersianum
 subhumile
 subhumilis
+subiculata
 subiculosum
 subimitatrix
 subimmergens
 subimmersa
 subimmixta
 subincarnata
 subincarnatum
@@ -40230,14 +41035,15 @@
 sublargus
 sublateralis
 sublateritium
 sublatifolium
 sublatum
 sublatus
 sublaxus
+subleptorhynchoides
 subleptorrhynchoides
 subleptothecium
 sublesta
 sublestis
 sublestus
 subleucoblepharum
 sublilacina
@@ -40270,32 +41076,35 @@
 submagellanicus
 submalvinae
 submamilliferum
 submanfeldtii
 submarginale
 submarginalis
 submarginata
+submarginatus
 submarina
 submarinum
 submarinus
 submaritima
 submaxima
 submeleagris
 submembranacea
 submerrillii
 submersa
 submersiporum
 submersum
+submersus
 submexicana
 submicrostachyus
 subminima
 subminuscula
 subminutifolium
 subminutifolius
 subminutula
+submodesta
 submolliculum
 submollusca
 submoniliferum
 submontana
 submontanus
 submonticulosum
 submultiplinervis
@@ -40323,15 +41132,14 @@
 subocculta
 subocellata
 subocellatum
 subocellatus
 subochreata
 subochreatum
 suboculata
-suboeneum
 subolivaceum
 subolivaceus
 subopposita
 suboppositus
 suborbiculare
 suborbicularis
 suborbiculata
@@ -40372,30 +41180,33 @@
 subplanaica
 subplanum
 subplicata
 subplicatula
 subporosa
 subporosum
 subporosus
+subporotrichoides
 subpremnea
 subproducta
 subprolixa
 subpromiscua
 subprona
 subpronum
 subpronus
 subproposita
 subprostans
 subprotumidum
 subpseudotriquetrum
 subpuberula
 subpubescens
 subpulcella
+subpulverulenta
 subpulverulentus
 subpumila
+subpunctata
 subpunctiformis
 subpunctulatum
 subpungens
 subpurpurascens
 subpurpurea
 subpustulifera
 subpygmaeus
@@ -40404,14 +41215,15 @@
 subquaripara
 subquercinum
 subracemosa
 subracemosum
 subradians
 subradiata
 subradiatum
+subramanianii
 subramosum
 subramulosum
 subreagens
 subreducta
 subregularis
 subrelaxa
 subrelaxum
@@ -40419,14 +41231,15 @@
 subremotus
 subreniforme
 subreniformis
 subrepanda
 subrepandra
 subrepens
 subrepleta
+subreticulosporum
 subretusa
 subrhodotropa
 subrhombifolia
 subrhynchocephala
 subrigida
 subrigidum
 subrobustum
@@ -40441,15 +41254,14 @@
 subrubellum
 subrudecta
 subrufescens
 subrugata
 subrugatum
 subrugosa
 subrugulosa
-subrupta
 subrutilans
 subsaccata
 subsalina
 subsalsa
 subsalsum
 subscabrum
 subsciorophyllus
@@ -40458,14 +41270,15 @@
 subsecundata
 subsecundum
 subsecundus
 subsejunctus
 subserialis
 subseriata
 subseriatum
+subseriatus
 subserpens
 subserpentina
 subserratum
 subsessile
 subsessiliflora
 subsessilifolia
 subsessilis
@@ -40599,14 +41412,15 @@
 subvelutinum
 subventosa
 subventricosum
 subverrucella
 subversus
 subverticillata
 subvicariella
+subvictoriense
 subvillifera
 subvillosa
 subvillosus
 subvinaceipallidus
 subvincta
 subvinctus
 subvinosum
@@ -40643,14 +41457,15 @@
 succirubrum
 succisa
 succisae
 succisus
 succosum
 succulenta
 succulentum
+succuneata
 sucina
 sudanense
 sudans
 sudetica
 sudeticum
 suecica
 suecicum
@@ -40767,14 +41582,15 @@
 surrepens
 surreyana
 surrogatum
 sursum
 suspensum
 sussuela
 sutherlandi
+sutherlandiae
 sutherlandii
 suttonensis
 suttoni
 suttonii
 suvorovii
 suworowii
 swainii
@@ -40803,14 +41619,15 @@
 sylvatica
 sylvaticum
 sylvaticus
 sylvatrix
 sylvestor
 sylvestre
 sylvestris
+sylviaearle
 sylvicola
 sylvicultrix
 symeae
 symmetrica
 symmetricum
 symmetricus
 symmicta
@@ -40849,39 +41666,44 @@
 syringaefolia
 syringifolia
 syrmatica
 syrmaticum
 syrtica
 syrticola
 syrticolus
+systema-solare
 systena
 systenum
 systremma
 systyla
 sytnikii
-syvashica
 syzygii
+szostakii
 tabacina
 tabacinum
 tabacinus
 tabacum
 tabascana
+tabeijunko
+tabeijunkoae
 tabellaria
 tabernaemontani
 tabernaemontanoides
 tabescens
 tabidus
+taboriae
 tabula
 tabulaeformis
 tabularis
 tabulata
 tabulatum
 tabuliplagae
 taccada
 tachyglossoides
+tactilis
 tadgellianum
 tadgellii
 taeda
 taekeri
 taeniaeformis
 taeniata
 taenicola
@@ -40910,14 +41732,15 @@
 talbotianum
 talbotii
 talcophila
 talingka
 tallangattensis
 tallowa
 talpae
+taluna
 talyuberlup
 tamala
 tamarense
 tamarensis
 tamarindi
 tamarinii
 tamarisci
@@ -40941,26 +41764,29 @@
 tandonis
 tanegana
 tanensis
 tanganyikae
 tangaroae
 tangatensis
 tangerinum
+tangneyae
 tankarvilleae
 tankervillaea
 tankervilleae
 tankervilliae
 tannensis
 tanumbirinense
 tanumbirinensis
 tanythrix
+tanyunxianiae
 tanzanica
 tapeinosporum
 tapes
 taphanyx
+tapputi
 taquetii
 taractica
 tararaensis
 taraxaci
 taraxacifolia
 taraxacoides
 taraxacum
@@ -40973,40 +41799,43 @@
 tardum
 tardus
 tarik
 tarinensis
 tarkinea
 tarkinensis
 tarminiana
+tarrabulga
 tarrietiae
 tarriettiae
 tartarea
 tasmacamphoratus
 tasmanensis
 tasmaniae
 tasmaniana
 tasmanica
 tasmanica 'B'
 tasmanicum
 tasmanicus
 tasmaniense
 tasmaniensis
+tasmanniae
 tasmannica
 tasmannicum
 tassiana
 tateana
 tateanus
 tatei
 tatjanae
 tatrae
 tatrana
 tatricum
 tattoniana
 tattonianum
 tatula
+tauntonensis
 tauntoniensis
 tauphorum
 tauricum
 taurina
 taurus
 tavaresii
 tawa
@@ -41024,32 +41853,33 @@
 taxifolium 'narrow-leaved form'
 taxifolium 'type form'
 taxifolius
 taxiforme
 taxiformis
 taxirameum
 taxirameus
-taxmanica
 taxophila
 taxophilus
 taylori
 tayloriana
 taylorianum
 taylorii
 tazetta
 tchupalensis
 teakleana
+tealii
 teckiana
 tecomatis
 tecta
 tectanthera
 tectiascus
 tectifica
 tectificae
 tectipora
+tectonae
 tectorius
 tectorum
 tectum
 tectus
 tedmoorei
 tef
 tegens
@@ -41064,24 +41894,24 @@
 telephioides
 telfairiae
 telfairii
 telfordii
 tellemanii
 telmata
 telmatiaea
-telmaticum
 telmatophila
 telmatum
 telmica
 telmicum
 telopeae
 temnomoides
 tempeltonii
 temperatum
 temperei
+templetoniae
 temulenta
 temulentum
 temulentus
 tenacella
 tenacis
 tenacissima
 tenacissimus
@@ -41120,14 +41950,15 @@
 tentaculata
 tentaculatum
 tentaculifera
 tentaculum
 tentaculus
 tentans
 tenuatum
+tenuatum x xanthopetalum
 tenue
 tenuicalyx
 tenuicarpum
 tenuicauda
 tenuicaule
 tenuicaulis
 tenuicorne
@@ -41259,14 +42090,15 @@
 terneraeflora
 terneriflora
 ternifolia
 ternifolium
 ternifolius
 terra-guilelmii
 terracina
+terrae-australis
 terrae-novae
 terrae-reginae
 terrae-victoriae
 terraereginae
 terraneum
 terrareginalense
 terrena
@@ -41347,14 +42179,15 @@
 tetragonoloba 'race c'
 tetragonoloba 'race d'
 tetragonoloba 'race e'
 tetragonoloba race 'a'
 tetragonoloba race 'b'
 tetragonolobus
 tetragonophylla
+tetragonophyllae
 tetragonophyllum
 tetragonum
 tetragonus
 tetragyna
 tetragynum
 tetragynus
 tetrahit
@@ -41435,15 +42268,14 @@
 thalia
 thaliana
 thalianum
 thalictroides
 thalliferum
 thallina
 thamesis
-thamnidiella
 thamnochortoides
 thamnoides
 thamnolica
 thamnophora
 thanatophora
 thapsina
 thapsus
@@ -41488,14 +42320,15 @@
 thermometrus
 thermophila
 therophilus
 thesaurum
 thesiifolia
 thesiodes
 thesioides
+thesoides
 thespesioides
 thespidioides
 thevetia
 thieleana
 thieleanum
 thienemanni
 thienemannii
@@ -41514,14 +42347,15 @@
 thoermeri
 tholicarpus
 tholifera
 tholiforme
 tholiformis
 tholocarpa
 thoma
+thomae
 thomasiae
 thomasiana
 thomasii
 thomasioides
 thominii
 thompsoniae
 thompsoniana
@@ -41573,14 +42407,15 @@
 thurberi
 thuretii
 thurni
 thurnii
 thuyoides
 thwaitesiana
 thwaitesii
+thwiaitesi
 thylax
 thymafolia
 thymifolia
 thymifolium
 thymifolius
 thymodes
 thymoides
@@ -41617,14 +42452,15 @@
 tibiiformis
 tichbonii
 tichospora
 tidbillensis
 tierneyana
 tierneyanum
 tierneyi
+tietkensi
 tietkensii
 tiffanyanum
 tigrina
 tigrinum
 tigrinus
 tildeniae
 tiliacea
@@ -41645,14 +42481,15 @@
 timorense
 timorensis
 timoriana
 timoriense
 timoriensis
 timothyi
 tinara
+tinarooa
 tinarooense
 tinarooensis
 tinasporoides
 tincta
 tinctina
 tinctoria
 tinctorium
@@ -41671,30 +42508,34 @@
 tingitanum
 tingitanus
 tingoorense
 tingoorensis
 tinifolia
 tinifolium
 tinkeri
+tinkyukuku
 tinosporoides
 tintinnans
 tinus
 tipa
 tipu
 tirucalli
 tisdallii
 tisserantii
 tissotii
 titania
 tithymaloides
 titubans
+tiwiana
 tiwiense
 tiwiensis
+tjaetaba
 tjaetabensis
 tjapukaiensis
+tjaynera
 tjibenongense
 tjibodensis
 toccoae
 toddii
 todtiana
 tofftii
 tofus
@@ -41713,14 +42554,15 @@
 tomasinianum
 tomatillo
 tomentella
 tomentellus
 tomentifera
 tomentilla
 tomentillus
+tomentipes
 tomentosa
 tomentosolilacinum
 tomentosum
 tomentosus
 tomentulosus
 tomlinsii
 tomnashii
@@ -41733,22 +42575,24 @@
 tonquinensis
 tonsa
 tonsum
 tonsurata
 toodyay
 toogaadyalis
 toolbrunupensis
+tooloomensis
 toona
 toondulya
 tooram
 toowoombae
 toowoombense
 toowoombensis
 topazense
 topazensis
+tophacea
 tophaceum
 tophaceus
 topiro
 toppii
 tora
 torelliana
 toressae
@@ -41898,56 +42742,63 @@
 transversalis
 transversum
 trapeza
 trapeziforme
 trapeziformis
 trapezioides
 trapezoidea
+trapezoides
 trappei
 tratmaniana
 tratmanianum
 tratmanni
 tratmannii
 trattinickiana
 traunsteineri
+traversi
+traversiae
 traversiana
 traversii
 trayningensis
 tremandrae
 tremandroides
 trematis-orientalis
 tremelloides
 tremellosa
 tremellosus
 tremula
 tremulae
 tremulans
+tremulentum
 tremulus
 trentepohlii
 trentepohlioides
 trepida
 trepidus
 treubii
 treueriana
 trevelyana
 trevethensis
+trevorrowii
+treyvaudi
 treyvaudii
 triacantha
 triacanthos
 triacanthus
 triacros
 trialata
 trialatus
 triandra
 triandrum
 triandrus
 triangolensis
 triangulare
 triangularis
 triangulatum
+triangulispora
 triangulum
 triantha
 trianthemi
 triapiculata
 triappendiculata
 triaristata
 triartha
@@ -42082,14 +42933,15 @@
 trifidus
 trifilla
 trifilum
 triflora
 triflorum
 triflorus
 trifolia
+trifolia var. trifoliolata
 trifoliastrum
 trifoliata
 trifoliatum
 trifoliatus
 trifolii
 trifoliolata
 trifoliolatum
@@ -42101,14 +42953,15 @@
 trifurcata
 trifurcatum
 trifurcatus
 trigastrocarya
 trigastrotheca
 trigenea
 trigibba
+triginocaulis
 triglochinicola
 triglochinoides
 trigona
 trigonis
 trigonocardia
 trigonocarpa
 trigonocarpum
@@ -42239,14 +43092,15 @@
 tristachya
 tristachyos
 tristachys
 tristachyum
 tristachyus
 tristanensis
 tristaniae
+tristaniopsidis
 tristaniopsis
 triste
 tristicha
 tristichum
 tristichus
 tristicula
 tristiculum
@@ -42257,14 +43111,15 @@
 trisulca
 trita
 triternata
 triticea
 triticeum
 triticeus
 tritici
+tritici-australis
 tritici-repentis
 triticiformis
 triticoides
 triumphalis
 triumvirorum
 triuncialis
 triuniae
@@ -42277,17 +43132,19 @@
 trixago
 trizonatus
 trochocarpae
 trochocarpoides
 trochoidea
 trochoideum
 troedelii
+troedelli
 troglodytica
 tropaeoli
 tropica
+tropicae
 tropicale
 tropicalis
 tropicum
 tropicus
 tropidiiflora
 tropidiifolia
 truculenta
@@ -42307,14 +43164,15 @@
 truncatoapocarpa
 truncatoapocarpum
 truncatula
 truncatum
 truncatus
 truncorum
 truncospora
+trunculata
 truxillensis
 tryblionella
 trygvei
 trygvii
 trymalioides
 tryoni
 tryonii
@@ -42325,14 +43183,15 @@
 tryphera
 trypherus
 tryptococca
 tryssa
 tschirchiana
 tsinglanensis
 tsotsi
+tsudae
 tuba
 tubaeforme
 tubaeformis
 tubaestylis
 tubaraoense
 tubata
 tuber-regium
@@ -42341,14 +43200,15 @@
 tuberculata
 tuberculata (Armstrong 743)
 tuberculatella
 tuberculatum
 tuberculatus
 tuberculifera
 tuberculiformis
+tuberculipilosa
 tuberculosa
 tuberculosum
 tuberculosus
 tuberiferum
 tuberiformis
 tuberigena
 tuberivora
@@ -42417,14 +43277,15 @@
 turbatus
 turberculata
 turbidulus
 turbinata
 turbinatum
 turbinatus
 turbinipes
+turbinispora
 turbinospora
 turbo
 turbynei
 turcica
 turcicum
 turczaninovi
 turczaninovii
@@ -42468,16 +43329,18 @@
 tuscula
 tusculus
 tutelata
 tuticorinense
 tutulata
 tuuwuulensis
 tuvara
+tuyouyou
 tweediana
 tweedianum
+tyalla
 tyallus
 tyleri
 tylicolor
 tylimanthoidea
 tylophorus
 tyloplaca
 tylosa
@@ -42589,14 +43452,15 @@
 umbrawarrensis
 umbriceps
 umbricola
 umbricolus
 umbrina
 umbrinella
 umbrinelloides
+umbrinellum
 umbrinoalutaceum
 umbrinocarnosa
 umbrinum
 umbrinus
 umbrorum
 umbrosa
 umbrosum
@@ -42742,14 +43606,15 @@
 urceolaris
 urceolata
 urceolatum
 urceolatus
 urceolatus (hairy-leafed form)
 uredinicola
 uredinis
+urenae
 ureniae
 urens
 urinamans
 urinaria
 urna
 urnalis
 urniformis
@@ -42760,14 +43625,15 @@
 urodon
 uroglossum
 uromycoides
 urophorum
 urophylla
 urophyllum
 urophyllus
+urosperma
 ursiniae
 ursinus
 urticae
 urticaefolia
 urticaefolius
 urticifolia
 urticoides
@@ -42837,27 +43703,29 @@
 vacuolatum
 vadorum
 vaga
 vagabunda
 vagabunde
 vagabundum
 vagans
+vagata
 vagens
 vaginale
 vaginalis
 vaginans
 vaginata
 vaginatum
 vaginatus
 vaginiflora
 vaginiflorum
 vaginula
 vagum
 vagus
 vahlii
+vaileae
 vaillantii
 vainioi
 valantoides
 valdentata
 valdestriata
 valdeta
 valdiviana
@@ -42909,14 +43777,15 @@
 vanderystii
 vangeertii
 vanheurckii
 vanhoffeni
 vanhouttei
 vankyi
 vanleeuwenii
+vanoverberghii
 vansittartense
 vansittartensis
 vansteenisii
 vanuatensis
 vaporalis
 vaporaria
 vaporarius
@@ -42946,14 +43815,15 @@
 variolatum
 variolosa
 variolosum
 variolosus
 variostriata
 variostromatica
 variotii
+varipunctata
 varium
 varius
 vascosilvae
 vasculum
 vaseyanum
 vasiformis
 vasinfecta
@@ -42998,14 +43868,15 @@
 velleioides
 vellerea
 vellereum
 vellereus
 velleum
 velleyanum
 velleyoides
+veloci
 velorum
 velox
 veluticeps
 velutina
 velutinella
 velutinellum
 velutinifolia
@@ -43013,26 +43884,28 @@
 velutinosus
 velutinum
 velutinus
 velutipes
 velveta
 venablesii
 venator
+venatus
 venefica
 veneficum
 venenifica
 venenificum
 veneris
 veneta
 venetus
 venezuelense
 veniciae
 venosa
 venosum
 venosus
+ventenati
 ventenatii
 venter
 ventosus
 ventrecta
 ventricosa
 ventricosum
 ventricosus
@@ -43057,14 +43930,15 @@
 verbascifolius
 verbascina
 verbenaca
 verbenae
 verbesinodes
 verbesinoides
 verdcourtii
+verdoni
 verdonii
 verecunda
 verecundum
 verecundus
 vereenae
 verior
 verisidiosa
@@ -43090,40 +43964,43 @@
 verniciflua (Southern variant)
 verniciflua (common variant)
 vernicifluum
 vernicifluus
 vernicosa
 vernicosum
 vernicosus
+vernoni
 vernonii
 vernum
 vernus
 veronabrunnea
 veronabrunneus
 veronense
 veronensis
 veronica
 veronicae
 veronicaefolia
 veronicea
 veronicifolia
 veroniciformis
 veronicoides
+verreauxi
 verreauxii
 verricula
 verriculum
 verrucaeformis
 verrucaria
 verrucarium
 verrucarius
 verrucata
 verrucatum
 verrucella
 verruciformis
 verrucipes
+verrucispora
 verrucisporum
 verrucisporus
 verrucitesta
 verrucosa
 verrucosa sensu Playfair (1915a)
 verrucosporum
 verrucosum
@@ -43150,14 +44027,15 @@
 versteegii
 vertebrale
 vertebralis
 vertebratum
 vertex
 verticale
 verticellata
+verticiclada
 verticillare
 verticillaris
 verticillata
 verticillatum
 verticillatus
 verticillifera
 verticilliflorum
@@ -43175,14 +44053,15 @@
 vescum
 vesicaria
 vesicarium
 vesicarius
 vesicata
 vesicatoria
 vesicatum
+vesiculare
 vesicularis
 vesiculata
 vesiculifera
 vesiculifolia
 vesiculifolium
 vesiculifolius
 vesiculiforme
@@ -43197,14 +44076,15 @@
 vespertilio
 vespertilionis
 vespertina
 vespertinus
 vespillonea
 vespilloneum
 vestifici
+vestipedes
 vestita
 vestitoides
 vestitum
 vestitus
 vesuvianum
 vesuvius
 vexans
@@ -43243,15 +44123,15 @@
 victorae
 victori
 victoria
 victoriae
 victoriae 'ACT form'
 victoriae 'Canberra form'
 victoriae 'Lake Mountain form'
-victoriae 'Mallacoota Inlet''
+victoriae 'Mallacoota Inlet'
 victoriae 'Unassigned 3'
 victoriae 'Unassigned 5'
 victoriae 'Unassigned 6'
 victoriae 'race 1'
 victoriae 'race a'
 victoriae 'race b'
 victoriae 'race c'
@@ -43259,35 +44139,37 @@
 victoriae 'race e'
 victoriae 'race f (Victorian populations)'
 victoriae 'race f'
 victoriae 'race g'
 victoriae 'race h'
 victoriae 'race j'
 victoriae 'race k'
+victoriaensis
 victorialis
 victoriana
 victorianum
 victoriense
 victoriensis
 victorii
 victrix
 vidaliana
+vidmadera
 vidovichii
 vieiardii
 vieillardi
 vieillardii
 viennotii
 vigilans
 vigintimilia
 vignae
 vigorosum
 vilhelmii
 vilior
-villaricense
 villaticus
+villepreuxpowerae
 villicaulis
 villiceps
 villifer
 villifera
 villiferus
 villiflora
 villiflorum
@@ -43325,38 +44207,42 @@
 vinaceorosea
 vinaceum
 vinaceus
 vincae
 vincaeflora
 vincentia
 vincentii
-vincentina
 vinciflora
 vincta
 vinctus
+vinea-gemmae
 vineale
 vinealis
 vinicolor
 vinifera
 vinnula
 vinnulum
 vinosa
 vinosipes
 vinosobrunnea
 vinosum
 vinosus
 violacea
 violaceocaulis
+violaceocoeruleum
 violaceohinnuleus
 violaceolamellatus
 violaceolivida
 violaceonigrum
+violaceotinctum
 violaceum
 violaceus
 violae
+violae-faustae
+violae-faustiae
 violascens
 violea
 violescens
 violeus
 violicola
 violifolia
 violifolium
@@ -43387,14 +44273,15 @@
 virgatus entity B
 virgatus entity C
 virginae
 virginea
 virgineoides
 virgineum
 virgineus
+virginiahalliae
 virginiana
 virginianum
 virginica
 virginicum
 virginicus
 virgulacolens
 virgulata
@@ -43428,40 +44315,43 @@
 viridiloculare
 viridilocularis
 viridimagentea
 viridinsularis
 viridinutans
 viridipallens
 viridipallidus
+viridipes
 viridireagens
 viridirufa
 viridis
 viridiseda
 viridissima
 viridissimum
 viridissimus
 viridistellata
 viridomarginata
 viridomarginatum
 viridosoredians
 viridula
 viridulum
+viridulus
 viridus
 viriosa
 viriosum
 viriosus
 virolens
 virosa
 virosus
 virusanum
 visci
 viscida
 viscidibrunnea
 viscidichromapes
 viscidocruenta
+viscidoviridis
 viscidula
 viscidulum
 viscidulus
 viscidum
 viscidus
 visciflua
 viscifolia
@@ -43478,15 +44368,17 @@
 vitalba
 vitellina
 vitellinella
 vitellinula
 vitellinum
 vitellinus
 viticifolia
+viticis
 viticoides
+viticola
 viticulosa
 viticulosoides
 vitiense
 vitiensis
 vitiflora
 vitifolia
 vitifolius
@@ -43567,14 +44459,15 @@
 vultur
 vulturiensis
 vulvaria
 vulvarifolia
 vuyckii
 waddelliae
 wadjukiorum
+wadsworthi
 wadsworthii
 wadulawitu
 waeberi
 wagenitzii
 wagiribuanum
 wagneri
 wahlbergii
@@ -43590,21 +44483,23 @@
 waitzia
 waitzioides
 wakefieldiae
 wakefieldiana
 wakefieldianus
 wakoolica
 waksmanii
+walalbai
 walchottianum
 walcottianum
 walcottii
 walesiana
 walhallae
 walkerae
 walkeri
+walkerianum
 walkingtoni
 walkingtonii
 wallabyensis
 wallaceanum
 wallachi
 wallamanense
 wallamanensis
@@ -43633,25 +44528,29 @@
 waltonii
 walyunga
 wamanguana
 wandoo
 wandooana
 wangariensis
 wangiensis
+wangzhenyi
 wanjurum
 wankaensis
 wannanii
+wannerooensis
 wannooensis
 wanosa
 wanosum
 wanyu
 wapstrarum
 wapstreorum
 wapu
 waralya
+warambiense
+warambiensis
 warangensis
 warburgiana
 warburgii
 warburtonensis
 warcupii
 wardellense
 wardellii
@@ -43663,14 +44562,15 @@
 wariatodes
 warmingii
 warneckeana
 warnesii
 warnieri
 warningensis
 warocqueana
+warraberensis
 warramaba
 warrenensis
 warrenii
 warriedarense
 warrumbunglensis
 warszewiczii
 wassellii
@@ -43767,16 +44667,18 @@
 wesenbergii
 westeae
 westermannii
 westii
 westoni
 westoniana
 westonii
+westrale
 westraliense
 westraliensis
+westralis
 westresii
 westringiaefolia
 westringiaefolium
 westringiaeformis
 westringifolia
 westringiifolia
 westringiifolium
@@ -43784,41 +44686,43 @@
 wetarense
 wetarensis
 wettsteinii
 weymouthi
 weymouthiana
 weymouthianus
 weymouthii
+whamiae
 whanii
 wheelerae
 wheeleri
 whelani
 whelanii
 whewellii
 whibleyana
 whibleyanum
 whicherae
 whicheranus
 whicherense
 whicherensis
 whiffiniana
+whileyi
 whinrayi
 whipplei
 whitackeri
 whiteae
 whiteana
 whiteanum
+whitehaneyae
 whiteheadii
 whitei
 whiteii
 whiteleggeana
 whiteleggeanum
 whiteleggeanus
 whiteleggei
-whiteleggii
 whiteochloae
 whitii
 whittakeri
 whittakerii
 whitteronii
 whittingae
 whittingehamei
@@ -43833,14 +44737,15 @@
 wichurae
 wichuraiana
 wichurana
 wichuriana
 wickhami
 wickhamiana
 wickhamii
+wielangtae
 wiemansii
 wierzejskii
 wiesneri
 wigghii
 wightiana
 wightii
 wilbergi
@@ -43962,14 +44867,16 @@
 wollastoniana
 wollastonianum
 wollastonii
 wolleanum
 wollei
 wollemiae
 wollemiensis
+wollemiicola
+wollsianus
 wollumbina
 wolseleyi
 woltereckii
 womersleyi
 wondraczekii
 wongabelensis
 wonganense
@@ -43986,14 +44893,15 @@
 woodsii
 woodwardi
 woodwardia
 woodwardii
 woolcockiorum
 woolhopensis
 woolhousiae
+woollsi
 woollsiana
 woollsianum
 woollsianus
 woollsii
 woolsiana
 woolsii
 woombye
@@ -44008,25 +44916,28 @@
 wratislaviensis
 wratislawiensis
 wrayae
 wrightii
 wrixoni
 wubabulna
 wubinensis
+wuchienshiung
 wudjariensis
 wuerthii
 wuhanense
 wulasiensis
 wulfenii
 wurdemannii
 wurmbeae
 wurthii
 wurunuran
+wusaulan
 wuthiana
 wuttkei
+wuzetian
 wyalongensis
 wyattiana
 wyattii
 wyberbensis
 wycherleyi
 wynaadense
 wynaadensis
@@ -44053,20 +44964,22 @@
 xanthocephalus
 xanthochila
 xanthochilum
 xanthochlora
 xanthochymus
 xanthoclada
 xanthocladum
+xanthocystis
 xanthodactylina
 xanthoderma
 xanthodermus
 xanthofarinosa
 xanthogloea
 xantholaema
+xantholaemus
 xantholeuca
 xantholeucum
 xantholeucus
 xanthomelaena
 xanthomelana
 xanthomelanoides
 xanthominuta
@@ -44107,24 +45020,26 @@
 xanthoxylon
 xanthum
 xanthus
 xanti
 xela
 xenicum
 xenismota
+xenosuberosa
 xerampelina
 xerampelinum
 xerampelinus
 xerica
 xerocarpa
 xerocarpum
 xerocarpus
 xerocephalum
 xerochloa
 xerochloae
+xerofasciculata
 xerofasciculatum
 xerophila
 xerophilum
 xerophilus
 xerophylla
 xerophyllum
 xerophyllus
@@ -44163,17 +45078,19 @@
 yaeyamensis
 yagobiei
 yakirrae
 yakuensis
 yalatensis
 yalgensis
 yalgorensis
+yallundae
 yalna
 yalwalensis
 yamblaensis
+yambulla
 yammeraensis
 yandina
 yandinense
 yandinga
 yangoura
 yapensis
 yapukaratja
@@ -44187,14 +45104,15 @@
 yarromerensis
 yarrowmerensis
 yarun
 yassensis
 yatesae
 yatesiae
 yeelirrie
+yelarbonense
 yemensis
 yendoi
 yeoi
 yerilla
 yerillus
 yilgarnense
 yilgarnensis
@@ -44214,16 +45132,18 @@
 yorkrakinense
 yorkrakinensis
 youmani
 youmanii
 youngiae
 youngiana
 youngii
+yourkae
 yowaensis
 yucatanensis
+yugambeh
 yuin
 yuleensis
 yumbarrana
 yunnanensis
 yunnaniana
 yuroogurrum
 yuulongicola
@@ -44234,14 +45154,15 @@
 zahlbruckneri
 zahlbruckneriana
 zahlbrucknerianus
 zaleae
 zamiaefolium
 zamiifolium
 zanardinii
+zaneveldii
 zanzibarensis
 zanzibarica
 zapota
 zarae
 zasuminensis
 zatrichota
 zatrichotum
@@ -44275,26 +45196,28 @@
 zeylandica
 zeylanensis
 zeylanica
 zeylanicum
 zeylanicus
 zeylanoides
 zeylonensis
+zhivanae
 zichii
 ziegeleri
 zierioides
 zigzagia
 zingiber
 zinniae
 zippeliana
 zippelianum
 zippelianus
 zippelii
 ziwolki
 zizanioides
+zlotorzyckae
 zmiewika
 zoanthogyne
 zodiacus
 zoeae
 zoexylocarya
 zollingeri
 zollingerianum
```

### Comparing `hespi-0.4.2/hespi/download.py` & `hespi-0.4.4/hespi/download.py`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/main.py` & `hespi-0.4.4/hespi/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 
 console = Console()
 
 app = typer.Typer()
 
 @app.command()
 def detect(
-    images: List[str] = typer.Argument(..., help="A list of images to process."),
+    images: List[str] = typer.Argument(..., help="A list of images to process. The images can also be URLs."),
     output_dir: Path = typer.Option(
-        ...,
+        "hespi-output",
         help="A directory to output the results.",
-        prompt="Please specify a directory for the results",
     ),
     gpu: bool = typer.Option(True, help="Whether or not to use a GPU if available."),
     fuzzy: bool = typer.Option(
         True, help="Whether or not to use fuzzy matching from teh reference database."
     ),
     fuzzy_cutoff: float = typer.Option(
         0.8, min=0.0, max=1.0, help="The threshold for the fuzzy matching score to use."
     ),
     htr: bool = typer.Option(
         True,
         help="Whether or not to do handwritten text recognition using Microsoft's TrOCR.",
     ),
     trocr_size: TrOCRSize = typer.Option(
-        TrOCRSize.BASE.value,
+        TrOCRSize.LARGE.value,
         help="The size of the TrOCR model to use for handwritten text recognition.",
         case_sensitive=False,
     ),
     sheet_component_weights: str = typer.Option(
         DEFAULT_SHEET_COMPONENT_WEIGHTS, 
         help="The path to the sheet component model weights.",
         envvar="HESPI_SHEET_COMPONENT_WEIGHTS",
```

### Comparing `hespi-0.4.2/hespi/ocr.py` & `hespi-0.4.4/hespi/ocr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
-from transformers import TrOCRProcessor, VisionEncoderDecoderModel
 from PIL import Image
 from enum import Enum
 from pathlib import Path
 import pytesseract
 
 
+
 class TrOCRSize(Enum):
     SMALL = "small"
     BASE = "base"
     LARGE = "large"
 
     def __str__(self):
         return str(self.value)
@@ -18,26 +18,25 @@
 class OCR:
     def get_text(self, image_path: Path) -> str:
         raise NotImplementedError
 
 
 class TrOCR(OCR):
     def __init__(self, size: TrOCRSize = TrOCRSize.BASE):
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-
-            print("Getting TrOCRProcessor")
-            self.processor = TrOCRProcessor.from_pretrained(
-                f"microsoft/trocr-{size}-handwritten"
-            )
-
-            print("Getting VisionEncoderDecoderModel")
-            self.model = VisionEncoderDecoderModel.from_pretrained(
-                f"microsoft/trocr-{size}-handwritten"
-            )
+        import transformers
+        from transformers import TrOCRProcessor, VisionEncoderDecoderModel
+        transformers.utils.logging.set_verbosity_error()
+
+        self.processor = TrOCRProcessor.from_pretrained(
+            f"microsoft/trocr-{size}-handwritten"
+        )
+
+        self.model = VisionEncoderDecoderModel.from_pretrained(
+            f"microsoft/trocr-{size}-handwritten",
+        )
 
     def get_text(self, image_path: Path) -> str:
         image = Image.open(image_path)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
             pixel_values = self.processor(
```

### Comparing `hespi-0.4.2/hespi/report.py` & `hespi-0.4.4/hespi/report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import jinja2
 from pathlib import Path
 import pandas as pd
 from typing import Dict
 
-from .util import label_fields
-
+from .util import console, ocr_result_str, label_fields
 
 def write_report(output:Path, component_files:Dict, ocr_df:pd.DataFrame):
     """
     Writes an HTML report of the detection found.
 
     Args:
         output (Path): The path to write the output HTML.
@@ -20,34 +19,50 @@
 
     def relative_to_output(path):
         try:
             return Path(path).relative_to(output.parent)
         except Exception:
             return path
 
+    def get_field_images(row, field, relative=True):
+        images = []
+        i = 1
+        while True:
+            suffix = f"_{i}" if i > 1 else ""
+            image = row.get(f"{field}_image{suffix}")
+            if image is None:
+                break
+            if relative:
+                image = relative_to_output(image)
+            images.append(image)
+            i += 1
+        return images
+
     def get_classification(path):
         return Path(path).name.split(".")[-2].replace("_", " ").title()
 
     def truncate(string):
         if len(string) < 30:
             return string
         return f"{string[:30]}..."
 
     env = jinja2.Environment(
         loader=loader,
         autoescape=jinja2.select_autoescape()
     )
     env.globals['relative_to_output'] = relative_to_output
     env.globals['get_classification'] = get_classification
+    env.globals['get_field_images'] = get_field_images
+    env.globals['ocr_result_str'] = ocr_result_str
     env.globals['len'] = len
     env.globals['truncate'] = truncate
     template = env.get_template("report-template.html")
 
     result = template.render(
         component_files=component_files,
         label_fields=label_fields,
         ocr_df=ocr_df,
     )
     with open(str(output), 'w') as f:
-        print(f"Writing result to {output}")
+        console.print(f"Writing HTML report to '{output}'")
         f.write(result)
```

### Comparing `hespi-0.4.2/hespi/templates/assets/css/bootstrap.hespi.min.css` & `hespi-0.4.4/hespi/templates/assets/css/bootstrap.hespi.min.css`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/templates/assets/img/favicon.svg` & `hespi-0.4.4/hespi/templates/assets/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/templates/assets/img/hespi-favicon.png` & `hespi-0.4.4/hespi/templates/assets/img/hespi-favicon.png`

 * *Files identical despite different names*

### Comparing `hespi-0.4.2/hespi/yolo.py` & `hespi-0.4.4/hespi/yolo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import tempfile
 from shutil import move
 from pathlib import Path
 from PIL import Image
-from collections import defaultdict
+from collections import defaultdict, Counter
 from rich.console import Console
-
-
-try:
-    from ultralytics.models.yolo.detect.predict import DetectionPredictor
-except ImportError: # pragma: no cover
-    from ultralytics.yolo.v8.detect.predict import DetectionPredictor # pragma: no cover
-
+from rich.table import Column, Table
 
 console = Console()
 
 from .util import get_stub
 
 def predictions_filename(stub):
-    return f"{stub}-predictions.jpg"
+    return f"{stub}.all.jpg"
 
 
 def yolo_output(model, images, output_dir, tmp_dir_prefix=None, batch_size=4, res=1280):
+    try:
+        from ultralytics.models.yolo.detect.predict import DetectionPredictor
+    except ImportError: # pragma: no cover
+        from ultralytics.yolo.v8.detect.predict import DetectionPredictor # pragma: no cover
+
     if not model.predictor:
         model.predictor = DetectionPredictor()
         model.predictor.setup_model(model=model.model)
 
     tmp_dir = tempfile.TemporaryDirectory(prefix=tmp_dir_prefix)
     tmp_dir_path = Path(tmp_dir.name)
     console.print(f"Using temporary directory '{tmp_dir_path}'")
@@ -32,43 +31,56 @@
     model.predictor.save_dir = tmp_dir_path
 
     results = model.predict(source=images, show=False, save=True, batch=batch_size, imgsz=res)
     output_files = defaultdict(list)
 
     output_dir = Path(output_dir)
 
-    for index, (image, predictions) in enumerate(zip(images, results)):
+    for image, predictions in zip(images, results):
         stub = get_stub(image)
         image_output_dir = output_dir / stub
         image_output_dir.mkdir(exist_ok=True, parents=True)
         prediction_path = image_output_dir / predictions_filename(stub)
 
         prediction_path_tmp_location = Path(model.predictor.save_dir)/image.name
         assert prediction_path_tmp_location.exists()
 
-        console.print(
-            f"Saving sheet component predicitons with bounding boxes to '{prediction_path}'"
+        table = Table(
+            Column(header="Category", justify="middle"),
+            Column(header=f"File in directory '{image_output_dir}'", justify="left", style="green"),
+            title=f"Saving predicitons for: '{stub}'",
         )
+        table.add_row("All", prediction_path.name)
+
         move(prediction_path_tmp_location, prediction_path)
 
-        for prediction_index, boxes in enumerate(predictions.boxes):
+        counter = Counter()
+
+        for _, boxes in enumerate(predictions.boxes):
             category_index = int(boxes.cls.cpu().item())
             category = (
                 model.names[category_index].replace(" ", "_").replace(":", "").strip()
             )
 
             assert len(boxes.xyxy) == 1
             x0, y0, x1, y1 = boxes.xyxy.cpu().numpy()[0]
 
             # open image
             im = Image.open(image)
             im_crop = im.crop((x0, y0, x1, y1))
+            counter.update([category])
+
+            counter_suffix = f"-{counter[category]}" if counter[category] > 1 else ""
+            
             output_path = (
-                image_output_dir / f"{stub}.{prediction_index}.{category}.jpg"
+                image_output_dir / f"{stub}.{category}{counter_suffix}.jpg"
             )
-            console.print(f"Saving {category} to '{output_path}'")
+            table.add_row(category, output_path.name)
+
             im_crop.convert('RGB').save(output_path)
             output_files[stub].append(output_path)
 
     tmp_dir.cleanup()
 
+    console.print(table)
+
     return output_files
```

### Comparing `hespi-0.4.2/pyproject.toml` & `hespi-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hespi"
-version = "0.4.2"
+version = "0.4.4"
 description = "HErbarium Specimen sheet PIpeline"
 authors = ["Robert Turnbull <robert.turnbull@unimelb.edu.au>"]
 license = "Apache-2.0"
 readme = "README.rst"
 exclude = ["hespi/data/plants.csv"]
 homepage = "https://rbturnbull.github.io/hespi/"
 repository = "https://github.com/rbturnbull/hespi"
@@ -27,14 +27,15 @@
 pytesseract = ">=0.3.10"
 transformers = ">=4.21.3"
 appdirs = ">=1.4.4"
 jinja2 = ">=3.1.2"
 ultralytics = ">=8.1.0"
 
 [tool.poetry.dev-dependencies]
+rcssmin = "^1.1.2"
 pytest = "^6.2.5"
 ipykernel = "^6.6.1"
 coverage = "^5.5"
 autopep8 = "^1.5.7"
 Sphinx = "^4.2.0"
 nbsphinx = "^0.8.7"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `hespi-0.4.2/PKG-INFO` & `hespi-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hespi
-Version: 0.4.2
+Version: 0.4.4
 Summary: HErbarium Specimen sheet PIpeline
 Home-page: https://rbturnbull.github.io/hespi/
 License: Apache-2.0
 Keywords: herbarium,object detection,OCR,HTR,specimen,handwritten text recognition
 Author: Robert Turnbull
 Author-email: robert.turnbull@unimelb.edu.au
 Requires-Python: >=3.8,<3.12
@@ -131,14 +131,24 @@
 .. start-credits
 
 Robert Turnbull, Emily Fitzgerald, Karen Thompson and Jo Birch from the University of Melbourne.
 
 This research was supported by The University of Melbourne’s Research Computing Services and the Petascale Campus Initiative. 
 The authors thank collaborators Niels Klazenga, Heroen Verbruggen, Nunzio Knerr, Noel Faux, Simon Mutch, Babak Shaban, Andrew Drinnan, Michael Bayly and Hannah Turnbull.
 
+Plant refererence data obtained from the `Australian National Species List (auNSL) <https://biodiversity.org.au/nsl>`_, as of March 2024, using the:
+
+- Australian Plant Name Index (APNI)
+- Australian Bryophyte Name Index (AusMoss)
+- Australian Fungi Name Index (AFNI) 
+- Australian Lichen Name Index (ALNI) 
+- Australian Algae Name Index (AANI)
+
+
+
 This pipeline depends on `YOLOv8 <https://github.com/ultralytics/ultralytics>`_, 
 `torchapp <https://github.com/rbturnbull/torchapp>`_,
 Microsoft's `TrOCR <https://www.microsoft.com/en-us/research/publication/trocr-transformer-based-optical-character-recognition-with-pre-trained-models/>`_.
 
 Logo derived from artwork by `ka reemov <https://thenounproject.com/icon/plant-1386076/>`_.
 
 .. end-credits
```

