# Comparing `tmp/hyrule-0.5.0.tar.gz` & `tmp/hyrule-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyrule-0.5.0.tar", last modified: Fri Jan  5 15:27:20 2024, max compression
+gzip compressed data, was "hyrule-0.6.0.tar", last modified: Mon May 20 20:12:14 2024, max compression
```

## Comparing `hyrule-0.5.0.tar` & `hyrule-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-01-05 15:27:20.765118 hyrule-0.5.0/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4453 2023-07-02 12:55:15.000000 hyrule-0.5.0/AUTHORS
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1053 2024-01-05 15:18:16.000000 hyrule-0.5.0/LICENSE
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1248 2024-01-05 15:27:20.765118 hyrule-0.5.0/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      723 2023-07-02 12:55:15.000000 hyrule-0.5.0/README.rst
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-01-05 15:27:20.765118 hyrule-0.5.0/hyrule/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      399 2024-01-05 15:24:27.000000 hyrule-0.5.0/hyrule/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7155 2023-08-27 12:38:40.000000 hyrule-0.5.0/hyrule/anaphoric.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4836 2023-10-12 17:46:20.000000 hyrule-0.5.0/hyrule/argmove.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    11188 2023-07-02 12:55:15.000000 hyrule-0.5.0/hyrule/collections.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    14392 2023-11-13 18:04:44.000000 hyrule-0.5.0/hyrule/control.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    14883 2023-07-02 12:55:15.000000 hyrule-0.5.0/hyrule/destructure.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      362 2023-08-27 12:40:49.000000 hyrule-0.5.0/hyrule/hy_init.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    12832 2023-07-02 12:55:15.000000 hyrule-0.5.0/hyrule/hypprint.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2941 2023-07-02 12:55:15.000000 hyrule-0.5.0/hyrule/iterables.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     5757 2023-11-13 18:04:44.000000 hyrule-0.5.0/hyrule/macrotools.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7880 2023-11-13 18:04:44.000000 hyrule-0.5.0/hyrule/misc.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4189 2023-07-02 12:55:15.000000 hyrule-0.5.0/hyrule/sequences.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-01-05 15:27:20.765118 hyrule-0.5.0/hyrule.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1248 2024-01-05 15:27:20.000000 hyrule-0.5.0/hyrule.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      416 2024-01-05 15:27:20.000000 hyrule-0.5.0/hyrule.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2024-01-05 15:27:20.000000 hyrule-0.5.0/hyrule.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       17 2024-01-05 15:27:20.000000 hyrule-0.5.0/hyrule.egg-info/requires.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        7 2024-01-05 15:27:20.000000 hyrule-0.5.0/hyrule.egg-info/top_level.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2024-01-05 15:27:20.765118 hyrule-0.5.0/setup.cfg
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1522 2024-01-05 15:25:08.000000 hyrule-0.5.0/setup.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 20:12:14.495064 hyrule-0.6.0/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4471 2024-05-10 20:19:59.000000 hyrule-0.6.0/AUTHORS
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1053 2024-03-26 16:54:34.000000 hyrule-0.6.0/LICENSE
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1400 2024-05-20 20:12:14.495064 hyrule-0.6.0/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      836 2024-04-21 11:10:30.000000 hyrule-0.6.0/README.rst
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 20:12:14.495064 hyrule-0.6.0/hyrule/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      399 2024-05-20 20:11:29.000000 hyrule-0.6.0/hyrule/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6265 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/anaphoric.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4175 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/argmove.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7651 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/collections.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    13407 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/control.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    14783 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/destructure.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      362 2024-03-26 16:54:34.000000 hyrule-0.6.0/hyrule/hy_init.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    11578 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/hypprint.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2528 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/iterables.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    11117 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/macrotools.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7907 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/misc.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3454 2024-05-10 20:19:59.000000 hyrule-0.6.0/hyrule/sequences.hy
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-05-20 20:12:14.495064 hyrule-0.6.0/hyrule.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1400 2024-05-20 20:12:14.000000 hyrule-0.6.0/hyrule.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      416 2024-05-20 20:12:14.000000 hyrule-0.6.0/hyrule.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2024-05-20 20:12:14.000000 hyrule-0.6.0/hyrule.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       17 2024-05-20 20:12:14.000000 hyrule-0.6.0/hyrule.egg-info/requires.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        7 2024-05-20 20:12:14.000000 hyrule-0.6.0/hyrule.egg-info/top_level.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2024-05-20 20:12:14.495064 hyrule-0.6.0/setup.cfg
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1560 2024-05-20 20:11:29.000000 hyrule-0.6.0/setup.py
```

### Comparing `hyrule-0.5.0/AUTHORS` & `hyrule-0.6.0/AUTHORS`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 * James King <james@agentultra.com>
 * Julien Danjou <julien@danjou.info>
 * Nicolas Dandrimont <nicolas.dandrimont@crans.org>
 * Gergely Nagy <algernon@madhouse-project.org>
 * Konrad Hinsen <konrad.hinsen@fastmail.net>
 * Vladimir Gorbunov <vsg@suburban.me>
 * John Jacobsen <john@mail.npxdesigns.com>
-* rogererens <roger.erens@e-s-c.biz>
+* Roger Erens <roger.erens@e-s-c.biz>
 * Thomas Ballinger <thomasballinger@gmail.com>
 * Morten Linderud <mcfoxax@gmail.com>
 * Guillermo Vayá <guivaya@gmail.com>
 * Bob Tolbert <bob@tolbert.org>
 * Ralph Möritz <ralph.moeritz@outlook.com>
 * Josh McLaughlin <josh@phear.cc>
 * Berker Peksag <berker.peksag@gmail.com>
 * Henrique Carvalho Alves <hcarvalhoalves@gmail.com>
 * Joe Hakim Rahme <joehakimrahme@gmail.com>
 * Kenan Bölükbaşı <kenanbolukbasi@gmail.com>
-* Abhishek L <abhishek.lekshmanan@gmail.com>
+* Abhishek Lekshmanan <abhishek.lekshmanan@gmail.com>
 * Christopher Browne <cbbrowne@ca.afilias.info>
 * Clinton N. Dreisbach <crnixon@gmail.com>
-* D. Joe <deejoe+castanea@etrumeus.com>
 * Duncan McGreggor <duncan.mcgreggor@rackspace.com>
 * E. Anders Lannerback <anders@lannerback.net>
-* Jack <jackjrabbit+github@gmail.com>
+* Jack Laxson <jackjrabbit+github@gmail.com>
 * Johan Euphrosine <proppy@google.com>
 * Kevin Zita <kzita@kent.edu>
 * Matt Fenwick <mfenwick100@gmail.com>
 * Sean B. Palmer <sean@miscoranda.com>
 * Thom Neale <twneale@gmail.com>
 * Tuukka Turto <tuukka.turto@oktaeder.net>
 * Vasudev Kamath <kamathvasudev@gmail.com>
 * Yuval Langer <yuval.langer@gmail.com>
 * Fatih Kadir Akın <fka@fatihak.in>
 * Jack Hooper <contact.jhooper@gmail.com>
 * Brian McKenna <brian@brianmckenna.org>
 * Halit Alptekin <info@halitalptekin.com>
 * Richard Parsons <richard.lee.parsons@gmail.com>
-* han semaj <sangho.nah@gmail.com>
+* Sangho Na <sangho.nah@gmail.com>
 * Ryan Gonzalez <rymg19@gmail.com>
 * Brendan Curran-Johnson <brendan@bcjbcj.ca>
 * Ivan Kozik <ivan@ludios.org>
 * Allison Kaptur <allison.kaptur@gmail.com>
 * Matthew Wampler-Doty <matthew.wampler.doty@gmail.com>
 * Tianon Gravi <admwiggin@gmail.com>
 * Ian Denhardt <ian@zenhack.net>
@@ -86,15 +85,15 @@
 * Rob Day <rkd@rkd.me.uk>
 * Eric Kaschalk <ekaschalk@gmail.com>
 * Yoan Tournade <yoan@ytotech.com>
 * Simon Gomizelj <simon@vodik.xyz>
 * Yigong Wang <wang@yigo.ng>
 * Oskar Kvist <oskar.kvist@gmail.com>
 * Brandon T. Willard <brandonwillard@gmail.com>
-* Andrew R. M. <nixy@nixy.moe>
+* Andrew Miller <nixy@nixy.moe>
 * Tristan de Cacqueray <tdecacqu@redhat.com>
 * Sören Tempel <soeren@soeren-tempel.net>
 * Noah Snelson <noah.snelson@protonmail.com>
 * Adam Porter <adam@alphapapa.net>
 * Gábor Lipták <gliptak@gmail.com>
 * Raymund MARTINEZ <zhaqenl@protonmail.com>
 * Zepeng Zhang <redraiment@gmail.com>
@@ -105,7 +104,8 @@
 * Joshua Munn <public@elysee-munn.family>
 * Peter Andreev <appa@gmx.co.uk>
 * Sunjay Cauligi <scauligi@eng.ucsd.edu>
 * David Tscheppen <david.tscheppen@gmail.com>
 * Gabriel F. C. Pereira <empresagabriel@gmail.com>
 * Daniel Nagy <danielnagy@posteo.de>
 * John Blundell <jlobblet@jlobblet.co.uk>
+* Artur Wroblewski <wrobell@riseup.net>
```

### Comparing `hyrule-0.5.0/LICENSE` & `hyrule-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyrule-0.5.0/PKG-INFO` & `hyrule-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: hyrule
-Version: 0.5.0
+Version: 0.6.0
 Summary: A utility library for the Hy programming language
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
 Project-URL: Documentation, https://hyrule.readthedocs.io
 Project-URL: Source, https://github.com/hylang/hyrule
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Hy
 License-File: LICENSE
 License-File: AUTHORS
 
 Hyrule is a utility library for the `Hy <http://hylang.org>`_ programming language. It can be thought of as the Hy equivalent, or addition, to Python's standard library. While intended primarily for Hy programs, its functions and classes can be used in Python as with any other Python library; just ``import hyrule``. Hyrule's macros, on the other hand, are only really usable in Hy.
 
-All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``.
+All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``, as in ``(require hyrule [branch])``. The specific submodule an object belongs to may not be stable between releases.
 
-`Hyrule's documentation can be read online on Read the Docs. <https://hyrule.readthedocs.io>`_
+`Hyrule's documentation can be read online on Hylang.org. <http://hylang.org/hyrule/doc>`_
 
 You can run Hyrule's test suite with the command ``pytest`` and build its documentation with ``( cd docs; sphinx-build . _build -b html )``.
```

### Comparing `hyrule-0.5.0/hyrule/anaphoric.hy` & `hyrule-0.6.0/hyrule/anaphoric.hy`

 * *Files 14% similar despite different names*

```diff
@@ -1,163 +1,109 @@
-;;; Hy anaphoric macros
-"The anaphoric macros module makes functional programming in Hy very
-concise and easy to read.
-
-    An anaphoric macro is a type of programming macro that
-    deliberately captures some form supplied to the macro which may be
-    referred to by an anaphor (an expression referring to another).
+"Hyrule's anaphoric macros can make functional programming more concise and
+easier to read. An anaphoric macro assigns values to designated symbols
+(typically ``it``) that may be used in the code passed to the macro."
 
-    -- Wikipedia (https://en.wikipedia.org/wiki/Anaphoric_macro)"
 
 (require
   hyrule.macrotools [defmacro!]
   hyrule.argmove [->])
 
 
-(defmacro ap-if [test-form then-form [else-form None]]
-  "As :ref:`if <if>`, but the result of the test form is named ``it`` in
-  the subsequent forms. The else-clause is optional.
-
-  Examples:
-    ::
-
-       => (import os)
-       => (ap-if (.get os.environ \"PYTHONPATH\")
-       ...   (print \"Your PYTHONPATH is\" it))
-  "
-  `(let [it ~test-form]
-     (if it ~then-form ~else-form)))
+(defmacro ap-if [test true-value [false-value None]]
+  #[[As :hy:func:`if`, but the result of the test form is named ``it`` in
+  the subsequent forms, and the else-clause is optional. ::
+
+      (import os)
+      (ap-if (.get os.environ "PYTHONPATH")
+         (print "Your PYTHONPATH is" it))]]
+  `(let [it ~test]
+     (if it ~true-value ~false-value)))
 
 
 (defmacro ap-each [xs #* body]
-  "Evaluate the body forms for each element ``it`` of ``xs`` and return ``None``.
-
-  Examples:
-    ::
+  "Evaluate the body forms for each element ``it`` of ``xs`` and return
+  ``None``. ::
 
-       => (ap-each [1 2 3] (print it))
-       1
-       2
-       3"
+    (ap-each [1 2 3] (print it))"
   `(let [it None] (for [it ~xs] ~@body)))
 
 
 (defmacro ap-each-while [xs form #* body]
-  "As ``ap-each``, but the form ``pred`` is run before the body forms on
-  each iteration, and the loop ends if ``pred`` is false.
-
-  Examples:
-    ::
+  "As :hy:func:`ap-each`, but the form ``pred`` is run before the body forms on
+  each iteration, and the loop ends if ``pred`` is false. ::
 
-       => (ap-each-while [1 2 3 4 5 6] (< it 4) (print it))
-       1
-       2
-       3"
+    (ap-each-while [1 2 3 4 5 6] (< it 4) (print it))
+      ; Prints only 1, 2, and 3"
   `(let [it None]
     (for [it ~xs]
       (when (not ~form)
         (break))
       ~@body)))
 
 
 (defmacro ap-map [form xs]
   "Create a generator like :py:func:`map` that yields each result of ``form``
-  evaluated with ``it`` bound to successive elements of ``xs``.
+  evaluated with ``it`` bound to successive elements of ``xs``. ::
 
-  Examples:
-    ::
-
-       => (list (ap-map (* it 2) [1 2 3]))
-       [2 4 6]"
+    (list (ap-map (* it 2) [1 2 3]))  ; => [2 4 6]"
   `(gfor  it ~xs  ~form))
 
 
 (defmacro ap-map-when [predfn rep xs]
-  "As ``ap-map``, but the predicate function ``predfn`` (yes, that's a
-  function, not an anaphoric form) is applied to each ``it``, and the
-  anaphoric mapping form ``rep`` is only applied if the predicate is true.
-  Otherwise, ``it`` is yielded unchanged.
-
-  Examples:
-    ::
-
-       => (list (ap-map-when (fn [x] (% x 2)) (* it 2) [1 2 3 4]))
-       [2 2 6 4]
-
-    ::
-
-       => (list (ap-map-when (fn [x] (= (% x 2) 0)) (* it 2) [1 2 3 4]))
-       [1 4 3 8]"
+  "As :hy:func:`ap-map`, but the predicate function ``predfn`` (yes, that's a
+  function, not an anaphoric form) is applied to each ``it``, and the anaphoric
+  mapping form ``rep`` is only applied if the predicate is true. Otherwise,
+  ``it`` is yielded unchanged. ::
+
+    (list (ap-map-when (fn [x] (% x 2)) (* it 2) [1 2 3 4]))
+      ; => [2 2 6 4]
+    (list (ap-map-when (fn [x] (= (% x 2) 0)) (* it 2) [1 2 3 4]))
+      ; => [1 4 3 8]"
   `(gfor  it ~xs  (if (~predfn it) ~rep it)))
 
 
 (defmacro ap-filter [form xs]
-  "The :py:func:`filter` equivalent of ``ap-map``.
+  "The :py:func:`filter` equivalent of :hy:func:`ap-map`.
 
-  Examples:
-    ::
+  ::
 
-       => (list (ap-filter (> (* it 2) 6) [1 2 3 4 5]))
-       [4 5]"
+    (list (ap-filter (> (* it 2) 6) [1 2 3 4 5]))
+      ; => [4 5]"
   `(gfor  it ~xs  :if ~form  it))
 
 
 (defmacro ap-reject [form xs]
-  "Equivalent to ``(ap-filter (not form) xs)``.
-
-  Examples:
-    ::
-
-       => (list (ap-reject (> (* it 2) 6) [1 2 3 4 5]))
-       [1 2 3]"
+  "Shorthand for ``(ap-filter (not form) xs)``. See :hy:func:`ap-filter`."
   `(gfor  it ~xs  :if (not ~form)  it))
 
 
 (defmacro ap-dotimes [n #* body]
-  "Equivalent to ``(ap-each (range n) body…)``.
-
-  Examples:
-    ::
-
-       => (setv n [])
-       => (ap-dotimes 3 (.append n it))
-       => n
-       [0 1 2]"
+  "Shorthand for ``(ap-each (range n) body…)``. See :hy:func:`ap-each`."
   `(let [it None]
     (for [it (range ~n)]
       ~@body)))
 
 
 (defmacro ap-first [form xs]
   "Evaluate the predicate ``form`` for each element ``it`` of ``xs``. When
   the predicate is true, stop and return ``it``. If the predicate is never
-  true, return ``None``.
-
-  Examples:
-    ::
+  true, return ``None``. ::
 
-       => (ap-first (> it 5) (range 10))
-       6"
+    (ap-first (> it 5) (range 10))  ; => 6"
   `(next
     (gfor  it ~xs  :if ~form  it)
     None))
 
 
 (defmacro ap-last [form xs]
-  "Usage: ``(ap-last form list)``
-
-  Evaluate the predicate ``form`` for every element ``it`` of ``xs``.
+  "Evaluate the predicate ``form`` for every element ``it`` of ``xs``.
   Return the last element for which the predicate is true, or ``None`` if
-  there is no such element.
+  there is no such element. ::
 
-  Examples:
-    ::
-
-       => (ap-last (> it 5) (range 10))
-       9"
+    (ap-last (> it 5) (range 10))  ; => 9"
   (setv x (hy.gensym))
   `(let [it None]
     (setv ~x None)
     (for  [it ~xs  :if ~form]
       (setv ~x it))
     ~x))
 
@@ -170,89 +116,64 @@
     second, and evaluate ``form``.
   - Bind ``acc`` to the result, bind ``it`` to the third value of ``xs``,
     and evaluate ``form`` again.
   - Bind ``acc`` to the result, and continue until ``xs`` is exhausted.
 
   If ``initial-value`` is supplied, the process instead begins with
   ``acc`` set to ``initial-value`` and ``it`` set to the first element of
-  ``xs``.
-
-  Examples:
-    ::
+  ``xs``. ::
 
-       => (ap-reduce (+ it acc) (range 10))
-       45"
+    (ap-reduce (+ it acc) (range 10))  ; => 45"
   `(let [acc None  it None]
     (setv acc ~(if (is initial-value None)
       `(do
         (setv ~g!xs (iter ~g!xs))
         (next ~g!xs))
       initial-value))
     (for [it ~g!xs]
       (setv acc ~form))
     acc))
 
 (defmacro ap-when [test-form #* body]
-  "As :ref:`when <when>`, but the result of the test form is named ``it`` in
-  the subsequent forms.
+  #[[As :hy:func:`when <hy.core.macros.when>`, but the result of the test
+  form is named ``it`` in the subsequent forms. ::
 
-  Examples:
-    ::
-
-       => (import os)
-       => (ap-when (.get os.environ \"PYTHONPATH\")
-       ...   (print \"Your PYTHONPATH is\" it)
-       ...   it)
-  "
+    (setv variable -1)
+    (ap-when (+ variable 2)
+      (setv result it)
+      (print it))
+    (print result)]]
   `(let [it ~test-form]
      (when it ~@body)))
 
 (defmacro ap-with [form #* body]
-  "As :ref:`with <with>`, but the result of the form is named ``it`` in
-  the subsequent forms.
-
-  Examples:
-    ::
-
-       => (ap-with (open \"/proc/cpuinfo\")
-       ...   (lfor line it line))
-  "
+  "Shorthand for ``(with [it form] body…)``. See :hy:func:`with`."
   `(with [it ~form]
      ~@body))
 
 (defreader %
-  "Makes an expression into a function with an implicit ``%`` parameter list.
-
-  A ``%i`` symbol designates the (1-based) *i* th parameter (such as ``%3``).
-  Only the maximum ``%i`` determines the number of ``%i`` parameters--the
-  others need not appear in the expression.
-  ``%*`` and ``%**`` name the ``#*`` and ``#**`` parameters, respectively.
-
-  Examples:
-    ::
+  "Define an anonymous function with an implicit parameter list,
+  similarly to Clojure's literal anonymous functions. A single form is
+  read and interpreted as the body of the function. The first
+  parameter is named ``%1``, the second ``%2``, and so on. ::
 
-       => (#%[%1 %6 42 [%2 %3] %* %4] 1 2 3 4 555 6 7 8)
-       [1 6 42 [2 3] #(7 8) 4]
+    (list (map #%(+ %1 3) (range 5)))  ; => [3 4 5 6 7]
 
-    ::
+  The number of parameters is set by the largest ``%i`` symbol that
+  appears in the code::
 
-       => (#% %** :foo 2)
-       {\"foo\" 2}
+    (setv f #%(+ %1 %3))
+    (f 1 10 100)  ; => 101
 
-    When used on an s-expression,
-    ``#%`` is similar to Clojure's anonymous function literals--``#()``::
+  Use ``%*`` for a ``#* args`` parameter and ``%**`` for a ``#**
+  kwargs`` parameter::
 
-       => (setv add-10 #%(+ 10 %1))
-       => (add-10 6)
-       16
+    (#%[%1 %*] 1 2 3)  ; => [1 #(2 3)]
 
-  .. note::
-    ``#%`` determines the parameter list by the presence of a ``%*`` or ``%**``
-    symbol and by the maximum ``%i`` symbol found *anywhere* in the expression,
-    so nesting of ``#%`` forms is not recommended."
+  The implementation searches the input recursively for ``%``-symbols and doesn't attempt to detect nested ``#%`` calls, so nested calls are of limited value."
   (import hyrule [flatten inc])
   (setv expr (.parse-one-form &reader))
   (setv %symbols (sfor a (flatten [expr])
                        :if (and (isinstance a hy.models.Symbol)
                                 (.startswith a '%))
                        (-> a
                            (.split "." :maxsplit 1)
```

### Comparing `hyrule-0.5.0/hyrule/argmove.hy` & `hyrule-0.6.0/hyrule/argmove.hy`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,153 @@
+"This module provides macros similar to Clojure's threading macros,
+also known as arrow macros."
+
+
 (import
-  hyrule.iterables [rest])
+  hyrule.iterables [rest]
+  itertools [chain])
 
 
 (eval-and-compile
   (defn _dotted [node]
     "Helper function to turn '.name forms into '(.name) forms"
     (if (and (isinstance node hy.models.Expression)
              (= (get node 0) '.))
       `(~node)
       node)))
 
 
 (defmacro -> [head #* args]
-  "Thread `head` first through the `rest` of the forms.
 
-  ``->`` (or the *threading macro*) is used to avoid nesting of expressions. The
-  threading macro inserts each expression into the next expression's first argument
-  place. The following code demonstrates this:
-
-  Examples:
-    ::
-
-       => (defn output [a b] (print a b))
-       => (-> (+ 4 6) (output 5))
-       10 5
-  "
+  #[[Evaluate the first :ref:`expression <hy:expressions>` in ``args``
+  with ``head`` inserted as the second argument, then the next
+  expression with that result as its second argument, then the next
+  expression with *that* result as its second argument, and so on. In
+  other words, ::
+
+    (-> x (foo a b) (bar c d))
+
+  is equvalent to ::
+
+    (do
+      (setv value x)
+      (setv value (foo value a b))
+      (setv value (bar value c d))
+      value)
+
+  but without actually using an intermediate variable. For example::
+
+    (-> (+ 4 6) (print 5))
+      ; Prints "10 5"
+
+  Arguments of the form ``.foo`` are automatically expanded to ``(.foo)``::
+
+    (-> " hello " .upper .strip)  ; => "HELLO"
+
+  And if an argument ``arg`` isn't an expression, it's expanded to
+  ``(arg)``::
+
+   (-> "0" int bool)  ; => False]]
+
   (setv ret head)
   (for [node args
        :setv node (_dotted node)]
     (setv ret (if (isinstance node hy.models.Expression)
                   `(~(get node 0) ~ret ~@(rest node))
                   `(~node ~ret))))
   ret)
 
 
 (defmacro ->> [head #* args]
-  "Thread `head` last through the `rest` of the forms.
+  #[[As :hy:func:`->`, but each result is placed as the last argument of
+  each expression instead of the second. ::
 
-  ``->>`` (or the *threading tail macro*) is similar to the *threading macro*, but
-  instead of inserting each expression into the next expression's first argument,
-  it appends it as the last argument. The following code demonstrates this:
-
-  Examples:
-    ::
-
-       => (defn output [a b] (print a b))
-       => (->> (+ 4 6) (output 5))
-       5 10
-  "
+    (->> "a" (+ "b" "c"))  ; => "bca" ]]
   (setv ret head)
   (for [node args
        :setv node (_dotted node)]
     (setv ret (if (isinstance node hy.models.Expression)
                   `(~@node ~ret)
                   `(~node ~ret))))
   ret)
 
 
 (defmacro as-> [head name #* rest]
-  "Beginning with `head`, expand a sequence of assignments `rest` to `name`.
 
-  Each assignment is passed to the subsequent form. Returns the final assignment,
-  leaving the name bound to it in the local scope.
+  #[[Assign ``head`` to the symbol ``name`` and evaluate each form in
+  ``rest``. After each evaluation, the result is reassigned to
+  ``name``. ::
+
+    (as-> "a" it
+          (+ "b" it "c")
+          (.upper it)
+          (print it))
+      ; Prints "BAC".
+
+  Thus ``as->`` is analogous to e.g. :hy:func:`->`, but the threading
+  point is set per form by name, rather than always being the second
+  argument.
+
+  Here's a more complex example, which prints a sentence from a Project
+  Gutenberg e-book::
+
+    (import
+      re
+      urllib.request [urlopen])
+
+    (as-> (urlopen "https://www.gutenberg.org/ebooks/219.txt.utf-8") it
+          (.read it)
+          (.decode it "UTF-8")
+          (re.search r"\. ([^.]+ paw-strokes [^.]+\.)" it)
+          (.group it 1)
+          (.replace it "\r\n" " ")
+          (print it))]]
 
-  This behaves similarly to other threading macros, but requires specifying
-  the threading point per-form via the name, rather than fixing to the first
-  or last argument.
-
-  Examples:
-    example how ``->`` and ``as->`` relate::
-
-       => (as-> 0 it
-       ...      (inc it)
-       ...      (inc it))
-       2
-
-    ::
-
-       => (-> 0 inc inc)
-       2
-
-    create data for our cuttlefish database::
-
-       => (setv data [{:name \"hooded cuttlefish\"
-       ...             :classification {:subgenus \"Acanthosepion\"
-       ...                              :species \"Sepia prashadi\"}
-       ...             :discovered {:year 1936
-       ...                          :name \"Ronald Winckworth\"}}
-       ...            {:name \"slender cuttlefish\"
-       ...             :classification {:subgenus \"Doratosepion\"
-       ...                              :species \"Sepia braggi\"}
-       ...             :discovered {:year 1907
-       ...                          :name \"Sir Joseph Cooke Verco\"}}])
-
-    retrieve name of first entry::
-
-       => (as-> (get data 0) it
-       ...      (:name it))
-       \"hooded cuttlefish\"
-
-    retrieve species of first entry::
-
-       => (as-> (get data 0) it
-       ...      (:classification it)
-       ...      (:species it))
-       \"Sepia prashadi\"
-
-    find out who discovered slender cuttlefish::
-
-       => (as-> (filter (fn [entry] (= (:name entry)
-       ...                           \"slender cuttlefish\")) data) it
-       ...      (get it 0)
-       ...      (:discovered it)
-       ...      (:name it))
-       \"Sir Joseph Cooke Verco\"
-
-    more convoluted example to load web page and retrieve data from it::
-
-       => (import urllib.request [urlopen])
-       => (as-> (urlopen \"http://docs.hylang.org/en/stable/\") it
-       ...      (.read it)
-       ...      (.decode it \"utf-8\")
-       ...      (lfor  x it  :if (!= it \"Welcome\")  it)
-       ...      (cut it 30)
-       ...      (.join \"\" it))
-       \"Welcome to Hy’s documentation!\"
-
-  .. note::
-
-    In these examples, the REPL will report a tuple (e.g. `('Sepia prashadi',
-    'Sepia prashadi')`) as the result, but only a single value is actually
-    returned.
-  "
   `(do (setv
          ~name ~head
          ~@(sum (gfor  x rest  [name x]) []))
      ~name))
 
 
+(defmacro some-> [head #* args]
+  #[[As :hy:func:`->`, but if an intermediate result is ``None``, all
+  further forms are ignored. ::
+
+    (defn lookup [char]
+      (.get {"a" 1 "b" 2} char))
+    (some-> "q" lookup (print "is the value"))
+      ; Prints nothing, since `(lookup "q")` returns `None`.]]
+  (setv val (hy.gensym))
+  `(cond (is (setx ~val ~head) None) None
+         ~@(chain.from_iterable (gfor node args
+           [`(is (setx ~val (hy.R.hyrule.-> ~val ~node)) None) None]))
+         True ~val))
+
+
 (defmacro doto [form #* expressions]
-  "Perform possibly mutating `expressions` on `form`, returning resulting obj.
 
-  ``doto`` is used to simplify a sequence of method calls to an object.
+  "As :hy:func:`->`, but instead of the return value of each expression being
+  passed to the next, a single object (obtained by evaluating the orignial
+  first argument ``form``) is used every time. In other words, ::
+
+    (doto x (foo a b) (bar c d))
+
+  is equvalent to ::
 
-  Examples:
-    ::
+    (do
+      (setv value x)
+      (foo value a b)
+      (bar value c d)
+      value)
 
-       => (doto [] (.append 1) (.append 2) (.reverse))
-       [2 1]
+  Thus, ``doto`` is useful when ``value`` is an object that gets mutated by
+  each expression::
 
-    ::
+    (doto [] (.append 1) (.append 2) (.reverse))  ; => [2 1]"
 
-       => (setv collection [])
-       => (.append collection 1)
-       => (.append collection 2)
-       => (.reverse collection)
-       => collection
-       [2 1]
-  "
   (setv f (hy.gensym))
   (defn build-form [expression]
     (setv expression (_dotted expression))
     (if (isinstance expression hy.models.Expression)
       `(~(get expression 0) ~f ~@(rest expression))
       `(~expression ~f)))
   `(do
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hyrule-0.5.0/hyrule/control.hy` & `hyrule-0.6.0/hyrule/control.hy`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 (require
-  hyrule.macrotools [defmacro/g! defmacro!])
+  hyrule.macrotools [defmacro!])
 (import
   hyrule.collections [prewalk by2s]
   hyrule.iterables [coll?]
   hyrule.misc [inc])
 
 
 (defmacro branch [tester #* rest]
@@ -131,72 +131,47 @@
         (if (= test-value 'else)
           'True
           `(= ~x ~test-value))
         result])
       []))))
 
 
-(defmacro cfor [f #* generator]
-  #[[syntactic sugar for passing a ``generator`` expression to the callable ``f``
-
-  Its syntax is the same as :ref:`generator expression <py:genexpr>`, but takes
-  a function ``f`` that the generator will be immedietly passed to. Equivalent
-  to ``(f (gfor ...))``.
-
-  Examples:
-
-  ::
-     => (cfor tuple x (range 10) :if (% x 2) x)
-     #(1 3 5 7 9)
-
-  The equivalent in python would be:
-
-     >>> tuple(x for x in range(10) if x % 2)
-
-  Some other common functions that take iterables::
-
-     => (cfor all x [1 3 8 5] (< x 10))
-     True
-
-     => (with [f (open "AUTHORS")]
-     ...  (cfor max
-     ...        author (.splitlines (f.read))
-     ...        :setv name (.group (re.match r"\* (.*?) <" author) 1)
-     ...        :if (name.startswith "A")
-     ...        (len name)))
-     20 ;; The number of characters in the longest author's name that starts with 'A'
-  ]]
-  `(~f (gfor ~@generator)))
+(defmacro cfor [f #* gfor-args]
+  #[[Shorthand for ``(f (gfor …))``. See
+  :hy:func:`gfor`. ::
+
+     (cfor tuple
+       x (range 10)
+       :if (% x 2)
+       x)           ; => #(1 3 5 7 9)]]
+  `(~f (gfor ~@gfor-args)))
 
 
 (defn _do-n [count-form body]
   (setv count (hy.gensym))
   `(do
     (setv ~count ~count-form)
     (for [~(hy.gensym)
         (if (= ~count Inf)
           (hy.I.itertools.repeat None)
           (range ~count))]
       ~@body)))
 
 
 (defmacro do-n [count-form #* body]
-  #[[Execute `body` a number of times equal to `count-form` and return
+  #[[Execute ``body`` a number of times equal to ``count-form`` and return
   ``None``. (To collect return values, use :hy:macro:`list-n`
   instead.)
 
   The macro is implemented as a :hy:func:`for` loop over a
-  :func:`range` call, with the attendent consequences for negative
+  :py:class:`range` call, with the attendent consequences for negative
   counts, :hy:func:`break`, etc. As an exception, if the count is
-  `Inf`, the loop is run over an infinite iterator instead. ::
+  ``Inf``, the loop is run over an infinite iterator instead. ::
 
-     => (do-n 3 (print "hi"))
-     hi
-     hi
-     hi]]
+     (do-n 3 (print "hi"))]]
 
   (_do-n count-form body))
 
 
 (defmacro defmain [args #* body]
   #[[Define a function to be called when :attr:`__name__` equals ``"__main__"``
   (see :mod:`__main__`). ``args`` is the function's lambda list, which will be
@@ -207,42 +182,35 @@
   allowed, but ignored.
 
   If the defined function returns an :class:`int`, :func:`sys.exit` is called
   with that integer as the return code.
 
   If you want fancy command-line arguments, you can use the standard Python
   module :mod:`argparse` in the usual way, because ``defmain`` doesn't change
-  ``sys.argv``. See also :hy:func:`parse-args <hyrule.misc.parse-args>`.
-  ::
+  ``sys.argv``. See also :hy:func:`parse-args`. ::
+
+    (defmain [program-name argument]
+      (print "Welcome to" program-name)
+      (print "The answer is" (* (float argument) 2)))]]
 
-      (import argparse)
-      (defmain []
-        (setv parser (argparse.ArgumentParser))
-        (.add-argument parser "STRING"
-          :help "string to replicate")
-        (.add-argument parser "-n" :type int :default 3
-          :help "number of copies")
-        (setv args (.parse-args parser))
-        (print (* args.STRING args.n))
-        0)]]
   (setv retval (hy.gensym)
         restval (hy.gensym))
   `(when (= __name__ "__main__")
      (import sys)
      (setv ~retval ((fn [~@(or args `[#* ~restval])] ~@body) #* sys.argv))
      (when (isinstance ~retval int)
        (sys.exit ~retval))))
 
 
 (defmacro lif [#* args]
   #[[A "Lispy if" similar to :hy:func:`if` and :hy:func:`cond
   <hy.core.macros.cond>`. Its most notable property is that it tests
   the condition with ``(is-not condition None)`` instead of ``(bool
   condition)``, so values such as the integer 0, the empty string, and
-  :py:keyword:`False` are considered true, not false. The general
+  ``False`` are considered true, not false. The general
   syntax is
   ::
 
       (lif
         condition1 result1
         condition2 result2
         …
@@ -268,26 +236,24 @@
 
 
 (defmacro list-n [count-form #* body]
   "Like :hy:macro:`do-n`, but the results are collected into a list.
 
   ::
 
-    => (setv counter 0)
-    => (list-n 5 (+= counter 1) counter)
-    [1 2 3 4 5]
-  "
+    (setv counter 0)
+    (list-n 5 (+= counter 1) counter)  ; => [1 2 3 4 5]"
   (setv l (hy.gensym))
   `(do
     (setv ~l [])
     ~(_do-n count-form [`(.append ~l (do ~@body))])
     ~l))
 
 
-(defmacro/g! loop [bindings #* body]
+(defmacro! loop [bindings #* body]
   "The loop/recur macro allows you to construct functions that use
   tail-call optimization to allow arbitrary levels of recursion.
 
   ``loop`` establishes a recursion point. With ``loop``, ``recur``
   rebinds the variables set in the recursion point and sends code
   execution back to that recursion point. If ``recur`` is used in a
   non-tail position, an exception is raised. which
@@ -348,16 +314,17 @@
 
 (defmacro block [#* body]
   #[[A macro that allows you to jump outside of a list of forms, like
   the Common Lisp special operator of the same name. The body forms
   are executed until ``(block-ret VALUE)`` is reached. The block
   returns ``VALUE``, or the value of the last form, if execution
   reached the end instead of being terminated by ``block-ret``.
-  ``VALUE`` is optional and defaults to ``None``. One use of ``block``
-  is to jump out of nested loops::
+  ``VALUE`` is optional and defaults to ``None``.
+
+  One use of ``block`` is to jump out of nested loops::
 
       (block (for [x (range 5)]
         (setv y x)
         (while y
           (print x y)
           (when (and (= x 3) (= y 1))
             (block-ret))
@@ -386,18 +353,18 @@
   ``:foo`` is an error. Inner blocks names shadow outer blocks of the
   same name, so ``block-ret`` will apply to the innermost of a series
   of nested anonymous blocks.
 
   There are no macros or functions named ``block-ret`` or
   ``block-ret-from``, since these forms are processed entirely by
   ``block``. ``block-ret`` and ``block-ret-from`` should not be
-  confused with Hy's built-in ``return``, which produces a true Python
+  confused with Hy's built-in :hy:func:`return`, which produces a true Python
   return statement. ``block`` is implemented with exception-handling
-  rather than functions, so it doesn't create a new scope as ``fn``
-  and ``defn`` do.]]
+  rather than functions, so it doesn't create a new scope as :hy:func:`fn`
+  and :hy:func:`defn` do.]]
   (block-f body {} (hy.gensym "br") True))
 
 (defn block-f [body tags BR [top False]]
 
   (setv tag 'None)
   (when (and body (or
       (= (get body 0) 'None)
```

### Comparing `hyrule-0.5.0/hyrule/destructure.hy` & `hyrule-0.6.0/hyrule/destructure.hy`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 ;;; Hy destructuring bind
 "
 This module is heavily inspired by destructuring from Clojure and provides very
 similar semantics. It provides several macros that allow for destructuring within
 their arguments.
 
-Introduction
-============
-
-Destructuring allows one to easily peek inside a data structure and assign names to values within. For example,
-
-.. code-block:: hy
+Destructuring allows one to easily peek inside a data structure and assign names to values within. For example, ::
 
     (setv+ {[{name :name [weapon1 weapon2] :weapons} :as all-players] :players
             map-name :map
             :keys [tasks-remaining tasks-completed]}
            data)
 
-would be equivalent to
-
-.. code-block:: hy
+would be equivalent to ::
 
     (setv map-name (.get data ':map)
           tasks-remaining (.get data ':tasks-remaining)
           tasks-completed (.get data ':tasks-completed)
           all-players (.get data ':players)
           name (.get (get all-players 0) ':name)
           weapon1 (get (.get (get all-players 0) ':weapons) 0)
           weapon2 (get (.get (get all-players 0) ':weapons) 1))
 
-where ``data`` might be defined by
-
-.. code-block:: hy
+where ``data`` might be defined by ::
 
     (setv data {:players [{:name Joe :weapons [:sword :dagger]}
                           {:name Max :weapons [:axe :crossbow]}]
                 :map \"Dungeon\"
                 :tasks-remaining 4})
 
 This is similar to unpacking iterables in Python, such as ``a, *b, c = range(10)``, however it also works on dictionaries, and has several special options.
 
 .. warning::
-   Variables which are not found in the expression are silently set to ``None`` if no default value is specified. This is particularly important with ``defn+`` and ``fn+``.
-
-   .. code-block:: hy
+   Variables which are not found in the expression are silently set to ``None`` if no default value is specified. This is particularly important with ``defn+`` and ``fn+``. ::
 
       (defn+ some-function [arg1
                             {subarg2-1 \"key\"
                              :or {subarg2-1 20}
                              :as arg2}
                             [subarg3-1
                              :& subargs3-2+
@@ -64,75 +53,71 @@
 
       (some-function)
       ; => {\"arg1\" None  \"arg2\" None  \"arg3\" None
       ;     \"subarg2-1\" 20  \"subarg3-1\" None  \"subargs3-2+\" None}
 
    Note that variables with a default value from an ``:or`` special option will fallback to their default value instead of being silently set to ``None``.
 
-Patterns
-========
+Pattern types
+~~~~~~~~~~~~~
 
-Dictionary Pattern
-------------------
+Several kinds of patterns are understood.
 
-Dictionary patterns are specified using dictionaries, where the keys corresponds to the symbols which are to be bound, and the values correspond to which key needs to be looked up in the expression for the given symbol.
+Dictionary patterns
+-------------------
 
-.. code-block:: hy
+Dictionary patterns are specified using dictionaries, where the keys corresponds to the symbols which are to be bound, and the values correspond to which key needs to be looked up in the expression for the given symbol. ::
 
     (setv+ {a :a b \"b\" c #(1 0)} {:a 1 \"b\" 2 #(1 0) 3})
     [a b c] ; => [1 2 3]
 
 The keys can also be one of the following 4 special options: ``:or``, ``:as``, ``:keys``, ``:strs``.
 
 - ``:or`` takes a dictionary of default values.
 - ``:as`` takes a variable name which is bound to the entire expression.
 - ``:keys`` takes a list of variable names which are looked up as keywords in the expression.
 - ``:strs`` is the same as ``:keys`` but uses strings instead.
 
-The ordering of the special options and the variable names doesn't matter, however each special option can be used at most once.
-
-.. code-block:: hy
+The ordering of the special options and the variable names doesn't matter, however each special option can be used at most once. ::
 
     (setv+ {:keys [a b] :strs [c d] :or {b 2 d 4} :as full} {:a 1 :b 2 \"c\" 3})
     [a b c d full] ; => [1 2 3 4 {:a 1 :b 2 \"c\" 3}]
 
 Variables which are not found in the expression are set to ``None`` if no default value is specified.
 
-List Pattern
-------------
+List patterns
+-------------
 
 List patterns are specified using lists. The nth symbol in the pattern is bound to the nth value in the expression, or ``None`` if the expression has fewer than n values.
 
 There are 2 special options: ``:&`` and ``:as``.
 
 - ``:&`` takes a pattern which is bound to the rest of the expression. This pattern can be anything, including a dictionary, which allows for keyword arguments.
 - ``:as`` takes a variable name which is bound to the entire expression.
 
-If the special options are present, they must be last, with ``:&`` preceding ``:as`` if both are present.
-
-.. code-block:: hy
+If the special options are present, they must be last, with ``:&`` preceding ``:as`` if both are present. ::
 
     (setv+ [a b :& rest :as full] (range 5))
     [a b rest full] ; => [0 1 [2 3 4] [0 1 2 3 4]]
 
     (setv+ [a b :& {:keys [c d] :or {c 3}}] [1 2 :d 4 :e 5]
     [a b c d] ; => [1 2 3 4]
 
 Note that this pattern calls ``list`` on the expression before binding the variables, and hence cannot be used with infinite iterators.
 
-Iterator Pattern
-----------------
+Iterator patterns
+-----------------
 
 Iterator patterns are specified using round brackets. They are the same as list patterns, but can be safely used with infinite generators. The iterator pattern does not allow for recursive destructuring within the ``:as`` special option.
 "
 
 (require
   hyrule.argmove [->>]
   hyrule.control [unless branch]
-  hyrule.macrotools [defmacro/g!])
+  hyrule.macrotools [defmacro!])
 (import
   itertools [starmap chain count]
   functools [reduce]
   hy.pyops *
   hyrule.iterables [rest]
   hyrule.collections [by2s])
 
@@ -341,49 +326,49 @@
 (defn _expanded-setv [actual args kwargs]
   (hy.macroexpand
     `(setv+ ~actual (+ (list ~args)
                           (lfor [k v] (.items ~kwargs)
                                 s [(hy.models.Keyword k) v]
                             s)))))
 
-(defmacro/g! defn+ [fn-name args #* doc+body]
+(defmacro! defn+ [fn-name args #* doc+body]
   "Define function `fn-name` with destructuring within `args`.
 
   Note that `#*` etc have no special meaning and are
   intepretted as any other argument.
   "
   (setv [doc body] (if (isinstance (get doc+body 0) str)
                      [(get doc+body 0) (rest doc+body)]
                      [None doc+body]))
   `(defn ~fn-name [#* ~g!args #** ~g!kwargs]
      ~doc
      ~(_expanded-setv args g!args g!kwargs)
      ~@body))
 
-(defmacro/g! fn+ [args #* body]
+(defmacro! fn+ [args #* body]
   "Return anonymous function with destructuring within `args`
 
   Note that `*`, `/`, etc have no special meaning and are
   intepretted as any other argument.
   "
   `(fn [#* ~g!args #** ~g!kwargs]
      ~(_expanded-setv args g!args g!kwargs)
      ~@body))
 
-(defmacro/g! defn/a+ [fn-name args #* doc+body]
+(defmacro! defn/a+ [fn-name args #* doc+body]
   "Async variant of ``defn+``."
   (setv [doc body] (if (isinstance (get doc+body 0) str)
                      [(get doc+body 0) (rest doc+body)]
                      [None doc+body]))
   `(defn/a ~fn-name [#* ~g!args #** ~g!kwargs]
      ~doc
      ~(_expanded-setv args g!args g!kwargs)
      ~@body))
 
-(defmacro/g! fn/a+ [args #* body]
+(defmacro! fn/a+ [args #* body]
   "Async variant of ``fn+``."
   `(fn/a [#* ~g!args #** ~g!kwargs]
      ~(_expanded-setv args g!args g!kwargs)
      ~@body))
 
 (defmacro let+ [args #* body]
   "let macro with full destructuring with `args`"
```

### Comparing `hyrule-0.5.0/hyrule/hypprint.hy` & `hyrule-0.6.0/hyrule/hypprint.hy`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,69 @@
-"``hyrule.pprint`` is a port of python's built-in ``pprint`` that can pretty
-print objects using Hy syntax.
+"Hyrule provides various tools for pretty-printing objects in Hy syntax. The
+interface is largely compatible with Python's own :mod:`pprint`, with two
+cosmetic differences:
+
+- :py:func:`isreadable <pprint.isreadable>` becomes :hy:func:`readable?
+  <hyrule.readable?>`.
+- :py:func:`isrecursive <pprint.isrecursive>` becomes :hy:func:`recursive?
+  <hyrule.recursive?>`.
+
+Much of the work is done by :hy:func:`hy.repr`, and thus Hyrule's
+pretty-printing can be extended to new types with :hy:func:`hy.repr-register`.
+
+Since Hy lacks :ref:`implicit concatenation of string literals
+<py:string-concatenation>`, strings (and bytestrings) are broken up using
+:hy:func:`+ <hy.pyops.+>`."
 
-Hy ``pprint`` leverages ``hy.repr`` for much of it's pretty printing and
-therefor can be extended to work with arbitrary types using
-``hy.repr-register``. Like Python's ``pprint`` and ``hy.repr``, Hy ``pprint``
-attempts to maintain round-trippability of it's input where possible. Unlike
-Python, however, Hy does not have `string literal concatenation`_,
-which is why strings and bytestrings are broken up using the form ``(+ ...)``.
-
-.. _string literal concatenation: https://docs.python.org/3/reference/lexical_analysis.html#string-literal-concatenation
-
-The API for Hy ``pprint`` is functionally identical to Python's ``pprint``
-module, so be sure to reference the Python `pprint`_
-docs for more on how to use the module's various methods and arguments.
-
-.. _pprint: https://docs.python.org/3/library/pprint.html
-
-The differences that do exist are as follows:
-
-- ``isreadable`` becomes ``readable?``
-- ``isrecursive`` becomes ``recursive?``
-- Passing ``False`` to the ``PrettyPrinter`` arg ``sort-dicts`` in Python
-  versions < 3.8 will raise a ``ValueError``
-"
 ;; Adapted from: https://github.com/python/cpython/blob/3.9/Lib/pprint.py
 
 (require
-  hyrule.collections [assoc]
   hyrule.control [unless])
 
 (import sys
         re
         collections
         pprint [PrettyPrinter :as PyPrettyPrinter
                 _recursion
                 _safe-tuple
                 _safe-key]
         hy.core.hy-repr
-        hy._compat [PY3_10]
+        hyrule.collections [assoc]
         hyrule.misc [inc dec constantly])
 
 (export [pprint pformat saferepr PrettyPrinter readable? recursive? pp])
 
-(if PY3_10
+(if (>= sys.version-info #(3 10))
   (defn _safe-py-repr [object context maxlevels level sort-dicts]
     (._safe-repr (PyPrettyPrinter :sort-dicts sort-dicts)
       object context maxlevels level))
   (import pprint [_safe-repr :as _safe-py-repr]))
 
 (defn pprint [object #* args #** kwargs]
-  "Pretty-print a Python object to a stream [default is sys.stdout].
-
-  Examples:
-    ::
-
-       => (pprint {:name \"Adam\" :favorite-foods #{:apple :pizza}
-                     :bio \"something very important\"}
-             :width 20)
-        {:name \"Adam\"
-         :bio (+ \"something \"
-                 \"very \"
-                 \"important\")
-         :favorite-foods #{:apple
-                           :pizza}}
-  "
+  "Pretty-print the object to a stream."
   (.pprint (PrettyPrinter #* args #** kwargs) object))
 
 (defn pformat [object #* args #** kwargs]
-  "Format a Python object into a pretty-printed representation."
+  "Format an object into a pretty-printed representation. Return a string."
   (.pformat (PrettyPrinter #* args #** kwargs) object))
 
 (defn pp [object [sort-dicts False] #* args #** kwargs]
-  "Pretty-print a Python object"
+  "As :hy:func:`pprint`, but with ``sort-dicts`` defaulting to ``False``."
   (pprint object #* args :sort-dicts sort-dicts #** kwargs))
 
 (defn saferepr [object]
-  "Version of (repr) which can handle recursive data structures."
+  "As :hy:func:`hy.repr`, but with a different approach to recursive objects."
   (get (_safe-repr object {} None 0 True) 0))
 
 (defn readable? [object]
-  "Determine if (saferepr object) is readable by (hy.eval)."
+  "Determine if ``(saferepr object)`` is readable by Hy's parser."
   (get (_safe-repr object {} None 0 True) 1))
 
 (defn recursive? [object]
-  "Determine if object requires a recursive representation."
+  "Determine if the object requires a recursive representation."
   (get (_safe-repr object {} None 0 True) 2))
 
 (defn _safe-repr [object context maxlevels level [sort-dicts True]]
   (setv typ (type object)
         r (getattr typ "__repr__" None))
 
   ;; Level and recursive protected dict hy-repr
@@ -179,25 +155,16 @@
         (do (when current (yield (hy.repr current)))
             (setv current part))
         (setv current candidate)))
   (when current
     (yield (hy.repr current))))
 
 (defclass PrettyPrinter [PyPrettyPrinter]
-  "Handle pretty printing operations onto a stream using a set of
-   configured parameters.
-
-   Args:
-     indent: Number of spaces to indent for each level of nesting.
-     width: Attempted maximum number of columns in the output.
-     depth: The maximum depth to print out nested structures.
-     stream: The desired output stream.  If omitted (or false), the standard
-       output stream available at construction will be used.
-     compact: If true, several items will be combined in one line.
-     sort-dicts: If True, dict keys are sorted. (only available for python >= 3.8)"
+  "Handle pretty-printing operations onto a stream using a set of
+  configured parameters. See :py:class:`pprint.PrettyPrinter`."
   (defn __init__ [self [indent 1] [width 80] [depth None] [stream None]
                   * [compact False] [sort-dicts True]]
     (setv self._sort-dicts True)
     (.__init__ (super)
                :indent indent
                :width width
                :depth depth
```

### Comparing `hyrule-0.5.0/hyrule/misc.hy` & `hyrule-0.6.0/hyrule/misc.hy`

 * *Files 12% similar despite different names*

```diff
@@ -1,191 +1,125 @@
 (require
-  hyrule.macrotools [defmacro/g!])
+  hyrule.macrotools [defmacro!])
 
 (import
+  sys
+  importlib.util
   hy.scoping [ScopeLet]
   hyrule.collections [by2s])
 
 
 (defmacro comment [#* body]
-  "Ignores body and always expands to None
 
-  The ``comment`` macro ignores its body and always expands to ``None``.
-  Unlike linewise comments, the body of the ``comment`` macro must
-  be grammatically valid Hy, so the compiler can tell where the comment ends.
-  Besides the semicolon linewise comments,
-  Hy also has the ``#_`` discard prefix syntax to discard the next form.
-  This is completely discarded and doesn't expand to anything, not even ``None``.
+  #[=[Ignore any arguments and expand to ``None``. ::
 
-  Examples:
-    ::
-
-        => (print (comment <h1>Surprise!</h1>
-        ...                <p>You'd be surprised what's grammatically valid in Hy</p>
-        ...                <p>(Keep delimiters in balance, and you're mostly good to go)</p>)
-        ...        \"Hy\")
-        None Hy
-
-    ::
+    (setv x ["a"
+             (comment <h1>Surprise!</h1>
+                      You might be surprised what's lexically valid in Hy
+                      (keep delimiters balanced and you're mostly good to go))
+             "b"])
+     x  ; => ["a" None "b"]
+
+  Contrast with Hy's built-in semicolon comments and :ref:`discard
+  prefix <hy:discard-prefix>`::
+
+    (setv x [1 ; 2 3
+               3])
+    x  ; => [1 3]
+    (setv x [1 #_ 2 3])
+    x  ; => [1 3]
+    (setv x [1 (comment 2) 3])
+    x  ; => [1 None 3]]=]
 
-        => (print #_(comment <h1>Surprise!</h1>
-        ...                  <p>You'd be surprised what's grammatically valid in Hy</p>
-        ...                  <p>(Keep delimiters in balance, and you're mostly good to go)</p>))
-        ...        \"Hy\")
-        Hy"
   None)
 
 
 (defn constantly [value]
-  "Create a new function that always returns `value` regardless of its input.
-
-  Create a new function that always returns the given value, regardless of
-  the arguments given to it.
-
-  Examples:
-    ::
+  "Return a constant function, which ignores its arguments and always
+  returns ``value``. ::
 
-        => (setv answer (constantly 42))
-        => (answer)
-        42
-
-    ::
-
-        => (answer 1 2 3)
-        42
-
-    ::
-
-        => (answer 1 :foo 2)
-        42
-  "
+    (setv answer (constantly 42))
+    (answer)           ; => 42
+    (answer 1 :foo 2)  ; => 42"
   (fn [#* args #** kwargs]
     value))
 
 
 (defn dec [n]
-  "Decrement `n` by 1.
-
-  Returns one less than *x*. Equivalent to ``(- x 1)``. Raises ``TypeError``
-  if *x* is not numeric.
-
-  Examples:
-    ::
-
-        => (dec 3)
-        2
-
-    ::
-
-        => (dec 0)
-        -1
-
-    ::
-
-        => (dec 12.3)
-        11.3
-  "
+  #[[Shorthand for ``(- n 1)``. The name stands for "decrement".]]
   (- n 1))
 
 
 (defn inc [n]
-  "Increment `n` by 1.
-
-  Returns one more than *x*. Equivalent to ``(+ x 1)``. Raises ``TypeError``
-  if *x* is not numeric.
-
-  Examples:
-    ::
-
-       => (inc 3)
-       4
-
-    ::
-
-       => (inc 0)
-       1
-
-    ::
-
-       => (inc 12.3)
-       13.3
-  "
+  #[[Shorthand for ``(+ n 1)``. The name stands for "increment".]]
   (+ n 1))
 
 
-(defmacro of [base #* args]
-  "Shorthand for indexing for type annotations.
-
-  If only one arguments are given, this expands to just that argument. If two arguments are
-  given, it expands to indexing the first argument via the second. Otherwise, the first argument
-  is indexed using a tuple of the rest.
-
-  ``of`` has three forms:
-
-  - ``(of T)`` will simply become ``T``.
-  - ``(of T x)`` will become ``(get T x)``.
-  - ``(of T x y ...)`` (where the ``...`` represents zero or more arguments) will become
-    ``(get T #(x y ...))``.
-
-  Examples:
-    ::
-
-       => (of str)
-       str
-
-    ::
+(defn import-path [path [name None]]
 
-       => (of List int)
-       List[int]
-
-    ::
+  #[[Import the Python or Hy source code at ``path`` as a module with
+  :func:`importlib.util.spec_from_file_location`, per Python's documentation.
+  Return the new module object. ``name`` defaults to ``(str (hy.gensym
+  "import-file"))``. ::
+
+    (setv p (hy.I.pathlib.Path "mymodule.hy"))
+    (.write-text p "(setv foo 3)")
+    (setv m (import-path p))
+    (print m.foo)  ; => 3]]
+
+  (when (is name None)
+    (setv name (str (hy.gensym "import-file"))))
+  (when (in name sys.modules)
+    (raise (ValueError f"The name {(hy.repr name)} is already in use in `sys.modules`.")))
+
+  ; Translated from https://github.com/python/cpython/blob/408e127159e54d87bb3464fd8bd60219dc527fac/Doc/library/importlib.rst?plain=1#L1584
+  (setv spec (importlib.util.spec-from-file-location name path))
+  (setv m (importlib.util.module-from-spec spec))
+  (setv (get sys.modules name) m)
+  (.loader.exec-module spec m)
 
-       => (of Set int)
-       Set[int]
+  m)
 
-    ::
-
-       => (of Dict str str)
-       Dict[str, str]
-
-    ::
 
-       => (of Tuple str int)
-       Tuple[str, int]
+(defmacro of [base #* args]
 
-    ::
+  "Shorthand for type annotations with indexing. If only one argument
+  is given, the macro expands to just that argument. If two arguments are
+  given, it expands to indexing the first argument with the second.
+  Otherwise, the first argument is indexed using a tuple of the rest. Thus:
+
+  - ``(of T)`` becomes ``T``.
+  - ``(of T x)`` becomes ``(get T x)``.
+  - ``(of T x y z)`` becomes ``(get T #(x y z))``.
+
+  Here are some Python equivalents of example uses:
+
+  - ``(of str)`` → ``str``
+  - ``(of List int)`` → ``List[int]``
+  - ``(of Callable [int str] str)`` → ``Callable[[int, str], str]``"
 
-       => (of Callable [int str] str)
-       Callable[[int, str], str]
-  "
   (if
     (not args) base
     (if (= (len args) 1)
         `(get ~base ~@args)
         `(get ~base #(~@args)))))
 
 
 (defn parse-args [spec [args None] #** parser-args]
-  "Return arguments namespace parsed from *args* or ``sys.argv`` with
-  :py:meth:`argparse.ArgumentParser.parse_args` according to *spec*.
 
-  *spec* should be a list of arguments which will be passed to repeated
-  calls to :py:meth:`argparse.ArgumentParser.add_argument`.  *parser-args*
-  may be a list of keyword arguments to pass to the
-  :py:class:`argparse.ArgumentParser` constructor.
+  #[=[Shorthand for typical uses of :py:mod:`argparse`. ``spec`` is a list of arguments to pass in repeated calls to :py:meth:`ArgumentParser.add_argument <argparse.ArgumentParser.add_argument>`. ``args``, defaulting to :data:`sys.argv`, will be used as the input arguments. ``parser-args``, if provided, will be passed on to the constructor of :py:class:`ArgumentParser <argparse.ArgumentParser>`. The return value is that of :py:meth:`parse_args <argparse.ArgumentParser.parse_args>`.
 
-  Examples:
-    ::
+  ::
+
+    (parse-args :spec [["strings" :nargs "+" :help "Strings"]
+                       ["-n" "--numbers" :action "append" :type int :help "Numbers"]]
+                :description "Parse strings and numbers from args"
+                :args ["a" "b" "-n" "1" "-n" "2"])
+       ; => Namespace(strings=['a', 'b'], numbers=[1, 2])]=]
 
-       => (parse-args [[\"strings\" :nargs \"+\" :help \"Strings\"]
-       ...             [\"-n\" \"--numbers\" :action \"append\" :type int :help \"Numbers\"]]
-       ...            [\"a\" \"b\" \"-n\" \"1\" \"-n\" \"2\"]
-       ...            :description \"Parse strings and numbers from args\")
-       Namespace(numbers=[1, 2], strings=['a', 'b'])
-  "
   (import argparse)
   (setv parser (argparse.ArgumentParser #** parser-args))
   (for [arg spec]
     (setv positional-arguments []
           keyword-arguments []
           value-of-keyword? False)
     (for [item arg]
@@ -215,15 +149,15 @@
   `(do
      (import pycallgraph [PyCallGraph]
              pycallgraph.output [GraphvizOutput])
      (with [(PyCallGraph :output (GraphvizOutput))]
            ~@body)))
 
 
-(defmacro/g! profile/cpu [#* body]
+(defmacro! profile/cpu [#* body]
   "Profile a bit of code
 
   Examples:
     ::
 
        => (require hyrule.contrib.profile [profile/cpu])
        => (profile/cpu (print \"hey there\"))
@@ -252,28 +186,49 @@
      (setv ~g!hy-s (StringIO))
      (setv ~g!hy-ps
            (.sort-stats (pstats.Stats ~g!hy-pr :stream ~g!hy-s)))
      (.print-stats ~g!hy-ps)
      (print (.getvalue ~g!hy-s))))
 
 
+(do-mac (do
+  (setv code "
+      (cond
+        (< x 0) -1
+        (> x 0)  1
+        (= x 0)  0
+        True     (raise TypeError))")
+
+  `(defn sign [x]
+    ~f"Return -1 for negative ``x``, 1 for positive ``x``, and 0 for
+    ``x`` equal to 0. The implementation is exactly ::
+
+    {code}
+
+    with the corresponding consequences for special cases like negative
+    zero and NaN."
+
+      ~(hy.read code))))
+
+
 (defn xor [a b]
-  "Perform exclusive or between `a` and `b`.
 
-  ``xor`` performs the logical operation of exclusive OR. It takes two arguments.
-  If exactly one argument is true, that argument is returned. If neither is true,
-  the second argument is returned (which will necessarily be false). Otherwise,
-  when both arguments are true, the value ``False`` is returned.
+  "A logical exclusive-or operation.
 
-  Examples:
-    ::
+  - If exactly one argument is true, return it.
+  - If neither is true, return the second argument (which will
+    necessarily be false).
+  - Otherwise (that is, when both arguments are true), return
+    ``False``.
+
+  ::
+
+    [(xor 0 0) (xor 0 1) (xor 1 0) (xor 1 1)]
+      ; => [0 1 1 False]"
 
-       => [(xor 0 0) (xor 0 1) (xor 1 0) (xor 1 1)]
-       [0 1 1 False]
-  "
   (if (and a b)
     False
     (or a b)))
 
 (defmacro smacrolet [_hy_compiler bindings #* body]
   "symbol macro let.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hyrule-0.5.0/hyrule.egg-info/PKG-INFO` & `hyrule-0.6.0/hyrule.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: hyrule
-Version: 0.5.0
+Version: 0.6.0
 Summary: A utility library for the Hy programming language
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
 Project-URL: Documentation, https://hyrule.readthedocs.io
 Project-URL: Source, https://github.com/hylang/hyrule
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Hy
 License-File: LICENSE
 License-File: AUTHORS
 
 Hyrule is a utility library for the `Hy <http://hylang.org>`_ programming language. It can be thought of as the Hy equivalent, or addition, to Python's standard library. While intended primarily for Hy programs, its functions and classes can be used in Python as with any other Python library; just ``import hyrule``. Hyrule's macros, on the other hand, are only really usable in Hy.
 
-All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``.
+All of Hyrule's contents can be imported or required directly from the top-level module ``hyrule``, as in ``(require hyrule [branch])``. The specific submodule an object belongs to may not be stable between releases.
 
-`Hyrule's documentation can be read online on Read the Docs. <https://hyrule.readthedocs.io>`_
+`Hyrule's documentation can be read online on Hylang.org. <http://hylang.org/hyrule/doc>`_
 
 You can run Hyrule's test suite with the command ``pytest`` and build its documentation with ``( cd docs; sphinx-build . _build -b html )``.
```

### Comparing `hyrule-0.5.0/setup.py` & `hyrule-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,21 @@
                     invalidation_mode=py_compile.PycInvalidationMode.CHECKED_HASH,
                 )
 
 
 # both setup_requires and install_requires
 # since we need to compile .hy files during setup
 requires = [
-    'hy >= 0.28.0, < 0.29'
+    'hy >= 0.29.0, < 0.30'
 ]
 
 
 setuptools.setup(
     name = 'hyrule',
-    version = '0.5.0',
+    version = '0.6.0',
     setup_requires=['wheel'] + requires,
     install_requires=requires,
     packages = setuptools.find_packages(exclude = ["tests*"]),
     package_data={'': ['*.hy']},
     author = "Paul Tagliamonte",
     author_email = "tag@pault.ag",
     description = 'A utility library for the Hy programming language',
@@ -45,9 +45,10 @@
         Documentation = 'https://hyrule.readthedocs.io',
         Source = 'https://github.com/hylang/hyrule'),
     platforms = ['any'],
     classifiers = [
         "Development Status :: 4 - Beta",
         "License :: DFSG approved",
         "License :: OSI Approved :: MIT License",  # Really "Expat". Ugh.
-        "Operating System :: OS Independent"],
+        "Operating System :: OS Independent",
+        "Programming Language :: Hy"],
     cmdclass={'install': install})
```

