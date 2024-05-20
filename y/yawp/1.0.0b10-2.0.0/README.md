# Comparing `tmp/yawp-1.0.0b10.tar.gz` & `tmp/yawp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yawp-1.0.0b10.tar", last modified: Thu May 18 16:14:55 2023, max compression
+gzip compressed data, was "yawp-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yawp-1.0.0b10.tar` & `yawp-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,52 @@
--rw-r--r--   0        0        0    13951 2023-05-18 15:02:43.510753 yawp-1.0.0b10/README.md
--rwxr-xr-x   0        0        0      807 2023-01-23 10:24:56.324823 yawp-1.0.0b10/pyproject.toml
--rwxr-xr-x   0        0        0    32580 2023-05-18 15:02:41.402757 yawp-1.0.0b10/yawp/__init__.py
--rwxr-xr-x   0        0        0    98271 2023-05-18 14:39:13.246607 yawp-1.0.0b10/yawp/__main__.py
--rw-r--r--   0        0        0   232685 2023-05-03 07:29:14.608193 yawp-1.0.0b10/yawp/docs/.test.pdf
--rw-r--r--   0        0        0   125254 2023-05-12 12:19:25.432197 yawp-1.0.0b10/yawp/docs/.yawp.pdf
--rw-r--r--   0        0        0   125697 2023-05-18 16:12:47.720089 yawp-1.0.0b10/yawp/docs/yawp.pdf
--rw-r--r--   0        0        0    14727 1970-01-01 00:00:00.000000 yawp-1.0.0b10/PKG-INFO
+-rw-r--r--   0        0        0    17144 2024-05-20 09:29:24.908001 yawp-2.0.0/README.md
+-rwxr-xr-x   0        0        0      834 2024-03-27 20:18:17.646923 yawp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    41858 2024-03-04 16:36:03.611071 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.04-17.36.03.back
+-rw-r--r--   0        0        0    41889 2024-03-06 09:28:02.962522 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-10.28.02.back
+-rw-r--r--   0        0        0    43552 2024-03-06 09:49:37.700852 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-10.49.37.back
+-rw-r--r--   0        0        0    42692 2024-03-06 10:45:33.797259 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-11.45.33.back
+-rw-r--r--   0        0        0    42092 2024-03-06 16:10:20.484525 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-17.10.20.back
+-rw-r--r--   0        0        0    42843 2024-03-06 16:23:19.356332 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-17.23.19.back
+-rw-r--r--   0        0        0    42875 2024-03-07 12:33:58.206084 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.07-13.33.58.back
+-rw-r--r--   0        0        0    42852 2024-03-07 18:50:50.315296 yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.07-19.50.50.back
+-rw-r--r--   0        0        0        0 2024-03-08 04:43:42.749094 yawp-2.0.0/yawp/.yawp.__init__.py.args
+-rw-r--r--   0        0        0    10257 2024-03-07 18:50:50.315296 yawp-2.0.0/yawp/.yawp.__init__.py.log
+-rw-r--r--   0        0        0   103562 2024-03-04 16:23:29.647385 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.04-17.23.29.back
+-rw-r--r--   0        0        0   103636 2024-03-04 16:26:40.456318 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.04-17.26.40.back
+-rw-r--r--   0        0        0   103640 2024-03-06 09:56:11.170776 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-10.56.11.back
+-rw-r--r--   0        0        0   103823 2024-03-06 10:02:24.240599 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.02.24.back
+-rw-r--r--   0        0        0   103739 2024-03-06 10:05:41.477564 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.05.41.back
+-rw-r--r--   0        0        0   103739 2024-03-06 10:07:27.258081 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.07.27.back
+-rw-r--r--   0        0        0   103738 2024-03-06 10:08:17.002324 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.08.16.back
+-rw-r--r--   0        0        0   103738 2024-03-06 10:08:57.250521 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.08.57.back
+-rw-r--r--   0        0        0   103738 2024-03-06 10:13:42.247914 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.13.42.back
+-rw-r--r--   0        0        0   103718 2024-03-06 10:14:32.836161 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.14.32.back
+-rw-r--r--   0        0        0   103718 2024-03-06 10:16:10.108637 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.16.10.back
+-rw-r--r--   0        0        0   103718 2024-03-06 10:18:56.865452 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.18.56.back
+-rw-r--r--   0        0        0   103718 2024-03-06 10:20:55.678033 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.20.55.back
+-rw-r--r--   0        0        0   103738 2024-03-06 10:24:28.571074 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.24.28.back
+-rw-r--r--   0        0        0   103738 2024-03-06 10:25:56.443503 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.25.56.back
+-rw-r--r--   0        0        0   103737 2024-03-06 10:30:06.920728 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.30.06.back
+-rw-r--r--   0        0        0   103737 2024-03-06 10:52:44.855367 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.52.44.back
+-rw-r--r--   0        0        0   104406 2024-03-06 10:53:51.903694 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.53.51.back
+-rw-r--r--   0        0        0   104404 2024-03-06 10:56:28.636460 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-11.56.28.back
+-rw-r--r--   0        0        0   104377 2024-03-06 11:03:08.618416 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-12.03.08.back
+-rw-r--r--   0        0        0   104378 2024-03-06 11:05:03.702978 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-12.05.03.back
+-rw-r--r--   0        0        0   104378 2024-03-06 11:07:45.171768 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-12.07.45.back
+-rw-r--r--   0        0        0   104378 2024-03-06 11:10:04.768450 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-12.10.04.back
+-rw-r--r--   0        0        0   104403 2024-03-06 13:01:28.481125 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-14.01.28.back
+-rw-r--r--   0        0        0   104151 2024-03-06 13:52:43.120156 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-14.52.43.back
+-rw-r--r--   0        0        0   104443 2024-03-06 14:29:45.251020 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-15.29.45.back
+-rw-r--r--   0        0        0   104217 2024-03-06 14:38:53.349699 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-15.38.53.back
+-rw-r--r--   0        0        0   104306 2024-03-06 14:44:41.619402 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-15.44.41.back
+-rw-r--r--   0        0        0   104405 2024-03-06 15:11:51.883372 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-16.11.51.back
+-rw-r--r--   0        0        0   104433 2024-03-06 16:10:35.104596 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-17.10.35.back
+-rw-r--r--   0        0        0   104488 2024-03-07 16:44:57.390375 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.07-17.44.57.back
+-rw-r--r--   0        0        0   104668 2024-03-07 18:50:42.207256 yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.07-19.50.42.back
+-rw-r--r--   0        0        0        0 2024-03-07 18:50:44.839269 yawp-2.0.0/yawp/.yawp.__main__.py.args
+-rw-r--r--   0        0        0    33869 2024-03-07 18:50:42.207256 yawp-2.0.0/yawp/.yawp.__main__.py.log
+-rwxr-xr-x   0        0        0    46582 2024-05-20 09:29:23.047992 yawp-2.0.0/yawp/__init__.py
+-rwxr-xr-x   0        0        0   113897 2024-05-17 15:44:03.854416 yawp-2.0.0/yawp/__main__.py
+-rw-r--r--   0        0        0    51559 2024-04-25 14:48:16.902196 yawp-2.0.0/yawp/docs/YAWP 2.0.0 Cheat Sheet.txt.pdf
+-rw-r--r--   0        0        0   388850 2024-05-20 09:33:57.709334 yawp-2.0.0/yawp/docs/YAWP 2.0.0 User Manual.txt.pdf
+-rw-r--r--   0        0        0   363430 2024-05-15 06:42:02.916905 yawp-2.0.0/yawp/docs/copy.txt.pdf
+-rw-r--r--   0        0        0    17949 1970-01-01 00:00:00.000000 yawp-2.0.0/PKG-INFO
```

### Comparing `yawp-1.0.0b10/pyproject.toml` & `yawp-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core >=3.9,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "yawp"
 authors = [{name = "Carlo Alessandro Verre", email = "carlo.alessandro.verre@gmail.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: POSIX :: Linux"]
 requires-python = ">=3.6"
-dependencies = ["PySimpleGui","pdfrw"]
+dependencies = ["PySimpleGUI==4.60.5", "pdfrw==0.4"]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://pypi.org/project/yawp"
 
 [project.scripts]
 yawp = "yawp.__main__:main"
```

### Comparing `yawp-1.0.0b10/yawp/__init__.py` & `yawp-2.0.0/yawp/.yawp.__init__.py.2024.03.06-11.45.33.back`

 * *Files 21% similar despite different names*

```diff
@@ -1,187 +1,312 @@
 #!/usr/bin/env python3
 
-'''Yet Another Word Processor, a word processor for text files, with PDF export
+'''Yet Another Word Processor, a WP for plain text files, with PDF export
 
-"YAWP" here means Yet Another Word Processor, and YAWP is a pure-Python Linux-only
-word  processor  for plain text files, with PDF export. If you really need all the
-features  of  a  full-fledged  WYSIWYG  word processor (with italic bold fonts etc
-etc)  as LibreOffice Writer, YAWP is not for you. But if you just want to create a
-draft or a simple quick-and-dirty no-frills document, give YAWP a try.
+"YAWP"  here means Yet Another Word Processor, and YAWP is a pure-Python Linux-only
+word  processor  for  plain text files, with PDF export. If you really need all the
+endless  features  of  a full-fledged WYSIWYG word processor as LibreOffice Writer,
+YAWP  is  not  for  you.  But  if  you  just  want  to  create  a draft or a simple
+quick-and-dirty no-frills document, give YAWP a try.
 
-Main features are:
+YAWP's main features are:
 
     • YAWP has a GUI interface, but can be used as a CLI command too
-    • YAWP  processes  in  place a single plain text file, hereinafter referred to
+    • YAWP  processes  in  place  a single plain text file, hereinafter referred to
       simply as the "text file"
-    • YAWP  before  rewriting the text file creates a timestamped backup, allowing
+    • YAWP  before  rewriting  the text file creates a timestamped backup, allowing
       Undo operation
     • YAWP justifies text at left and right in:
         • unindented paragraphs
         • dot-marked indented paragraphs (as this one)
-    • YAWP  justification  is driven by the text in the text file and by arguments
+    • YAWP  justification  is  driven by the text in the text file and by arguments
       only, not by commands or tags embedded in text
-    • YAWP  accepts  unjustified  pictures  (as schemas, tables and code examples)
+    • YAWP  accepts  unjustified  pictures  (as  schemas, tables and code examples)
       freely intermixed with text
-    • YAWP  performs  automatic multi-level renumbering of chapters and inserts an
+    • YAWP  performs  automatic  multi-level renumbering of chapters and inserts an
       automatic Contents chapter in the text file
-    • YAWP  recognizes  relevant subjects (quoted by '"') and inserts an automatic
+    • YAWP  recognizes  relevant  subjects (quoted by '"') and inserts an automatic
       Index chapter in the text file
-    • YAWP  performs  automatic  multi-level  renumbering  of  figure captions and
+    • YAWP  performs  automatic  multi-level  renumbering  of  figure  captions and
       inserts an automatic Figures chapter in the text file
-    • YAWP  cuts  the  text  file  in  pages, by inserting two-lines page headers,
-      allowing  page  numbering  control  and  insertion of initial Roman-numbered
-      pages
-    • YAWP also has some graphic features, you can sketch pictures with horizontal
-      and vertical segments (by '`') and arrowheads (by '^'), YAWP redraws them by
-      suitable Unicode graphic characters
-    • YAWP  exports  the text file in PDF format, with control over character size
-      and  page  layout,  and  lets  you  browse  the generated PDF file, allowing
-      preview and printing
-    • YAWP keeps a distinct argument set for each text file
-    • YAWP  in GUI mode saves the last processed text file and restores it at next
-      invocation
-    • YAWP in GUI mode saves a list of the 20 most recent processed text files and
-      allows to select one at next invocation
-    • YAWP  tries  to  correct  errors  made  by CUPS-PDF about font size and page
-      margins,  you  can  use default corrections or redefine them by a correction
+    • YAWP  cuts  the  text  file  in  pages,  by inserting two-lines page headers,
+      allowing page numbering control and insertion of initial Roman-numbered pages
+    • YAWP  also  has  some  graphics  capabilities,  you  can sketch pictures with
+      horizontal  and  vertical  segments  (by  '`')  and arrowheads (by '^'), YAWP
+      redraws them by suitable Unicode graphic characters
+    • YAWP  exports  the  text file in PDF format, with control over character size
+      and page layout, and lets you browse the generated PDF file, allowing preview
+      and printing
+    • YAWP  can  export  2,  4 or 8 pages on each paper sheet side, allowing you to
+      create in folio, in quarto and in octavo booklets
+    • YAWP writes information and error messages on terminal and on the log file of
+      the text file
+    • YAWP  tries  to  correct  errors  made  by  CUPS-PDF about font size and page
+      margins,  you  can  use  default corrections or redefine them by a correction
       file
-    • YAWP  writes  messages  about  processing on terminal and into a timestamped
-      session log file
-    • YAWP  locks the text file to  be processed in order to avoid interference by
-      other concurrent YAWP executions
-    • YAWP  is  stable,  if  after a YAWP execution you run YAWP again on the same
-      file with the same arguments, the text file content does not change
-    • believe  or  not,  YAWP   has   been  kept as simple as possible, about 3000
-      lines of Python code  (plus 3000 lines of this YAWP User Manual)
-
-In  order to install YAWP, we assume that your Linux belongs to the Debian family.
-Type at terminal:
-
-    │ $ sudo apt-get update
-    │ $ sudo apt-get purge printer-driver-cups-pdf
-    │ $ sudo apt-get install printer-driver-cups-pdf idle python3-pip
-    │ $ pip3 install yawp
+    • YAWP   locks  text  files  while  they  are  processed,  in  order  to  avoid
+      interference by other concurrent YAWP executions
+    • YAWP in GUI mode keeps a distinct arguments file for each text file
+    • YAWP  in GUI mode saves the name of the last processed text file and restores
+      it at next invocation
+    • YAWP  in  GUI  mode  saves a list of the 25 most recent processed text files,
+      among which you can select the next current text file
+    • if  after  a YAWP execution you run YAWP again on the same file with the same
+      arguments,  the  text  file  content  does  not  change (except of course the
+      time-dependent data in the page headers)
 
-Imagine your user name is 'xxxx'. If you see a message like this:
+As an example of CLI usage, the YAWP User Manual has been generated as
 
-    WARNING: The script yawp is installed in '/home/xxxx/.local/bin'
-    which is not on PATH
+    'YAWP 1.1.0 User Manual.txt.pdf'
 
-you can fix the problem by typing:
+from the text file
 
-    │ $ echo 'PATH=$PATH:/home/xxxx/.local/bin' >> /home/xxxx/.bashrc
+    'YAWP 1.1.0 User Manual.txt'
+
+by typing at terminal:
+
+    │ $ yawp -M f -v -w 95 -p c -n -4 -X e -L 3cm 'YAWP 1.1.0 User Manual.txt'
+
+where arguments mean:
+
+    • -M f: run YAWP in CLI Format mode
+    • -v: write messages not only into log file but also on terminal
+    • -w 95: set 95 characters per line
+    • -p c: insert a page header on page full, on picture break and before level-1 chapters
+    • -n -4: first four pages are numbered by Roman numbers
+    • -X e: export in PDF format
+    • -L 3cm: set left margins on odd pages and right margins on even pages to 3 cm
+    • 'YAWP 1.1.0 User Manual.txt': set the text file to process
+
+To install YAWP, if your Linux belongs to the Debian family, type at terminal:
+
+    │ $ sudo apt install idle atril printer-driver-cups-pdf pipx
+
+On other platforms you will use the specific installer instead:
+
+    │ $ sudo yum install ...        # on RHEL/CentOS/Fedora/Rocky/AlmaLinux
+    │ $ sudo emerge -a sys-apps/... # on Gentoo Linux
+    │ $ sudo apk add ...            # on Alpine Linux
+    │ $ sudo pacman -S ...          # on Arch Linux
+    │ $ sudo zypper install ...     # on OpenSUSE Linux
+
+Then run:
+
+    │ $ pipx ensurepath
+    │ $ pipx install yawp
+
+Later you can type:
+
+    │ $ pipx install --upgrade yawp
+
+in order to upgrade YAWP to a later version.
 
 Now you can close the terminal, open another one, and call YAWP. Syntax is:
 
-    │ $ yawp -h # show a help message and exit
-    │ $ yawp -V # show program's version number and exit
-    │ $ yawp -H [-Y pdf_browser] # browse the PDF YAWP User Manual and exit
-    │ $ yawp -M e [-y text_editor] text_file # run YAWP in CLI Edit mode
-    │ $ yawp -M f [...arguments...] text_file # run YAWP in CLI Format mode
-    │ $ yawp -M n [...arguments...] text_file # run YAWP in CLI Noformat mode
-    │ $ yawp -M u [...arguments...] text_file # run YAWP in CLI Undo mode
-    │ $ yawp text_file # run YAWP in GUI mode, explicit text file, no arguments
-    │ $ yawp # run YAWP in GUI mode, text file from previous session, no arguments
-
-This is the GUI Main window:
-
- ┌───┬───────────────────────────────────────────────────────────────────┬───┬───┐
- │   │                              YAWP - Main                          │ _ │ x │
- ├───┴───────────────────────────────────────────────────────────────────┴───┴───┤
- │ -v --verbose         □                                                        │
- │ -y --text-editor    [idle............] -g --graphics        □                 │
- │ -w --chars-per-line [0...............] -l --just-left-only  □                 │
- │ -c --contents-title [contents........] -i --index-title    [index...........] │
- │ -f --figures-title  [figures.........] -F --caption-prefix [figure..........] │
- │ -p --page-headers    ◎ n=no  ○ f=fullpage  ○ p=picture  ○ c=chapter           │
- │ -e --even-left      [%n/%N...........] -E --even-right     [%F %Y-%m-%d.....] │
- │ -o --odd-left       [%c..............] -O --odd-right      [%n/%N...........] │
- │ -n --page-offset    [0...............] -a --all-pages-E-e   □                 │
- │ -X --export-pdf      □                                                        │
- │ -Y --pdf-browser    [xdg-open........] -P --file-pdf       [%P%f.pdf........] │
- │ -W --char-width     [0...............] -A --char-aspect    [3/5.............] │
- │ -S --paper-size     [A4..............] -Z --landscape       □                 │
- │ -L --left-margin    [2cm.............] -R --right-margin   [2cm.............] │
- │ -T --top-margin     [2cm.............] -B --bottom-margin  [2cm.............] │
- │ -C --correct-sizes   ○ n=no  ◎ d=default  ○ f=file    -K --fake-margins □     │
- │ text_file           [.......................................................] │
- │ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ │
- │ │   New    │ │   Open   │ │  Recent  │ │  Saveas  │ │   Help   │ │   Exit   │ │
- │ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ │
- │ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ │
- │ │   Edit   │ │  Format  │ │ Noformat │ │   Undo   │ │   Log    │ │  Correct │ │
- │ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘ │
- └───────────────────────────────────────────────────────────────────────────────┘
+    • $ yawp -h               # show a help message and exit
+    • $ yawp -V               # show program's version number and exit
+    • $ yawp -H […arguments…] # browse the PDF YAWP User Manual and exit
+
+    • $ yawp text_file # GUI mode, explicit text file, no other arguments
+    • $ yawp           # GUI mode, text file from previous session, no arguments
+
+    • $ yawp -M e […arguments…] text_file # CLI Edit mode
+    • $ yawp -M f […arguments…] text_file # CLI Format mode
+    • $ yawp -M n […arguments…] text_file # CLI Noformat mode
+    • $ yawp -M u […arguments…] text_file # CLI Undo mode
+
+This is the GUI Main window, with default argument values:
+
+┌───┬───────────────────────────────────────────────────────────────────────────────┬───┬───┐
+│   │                                    YAWP - Main                                │ _ │ x │
+├───┴───────────────────────────────────────────────────────────────────────────────┴───┴───┤
+│ Format    -y --text-editor    [idle………………………………]                                          │
+│           -w --chars-per-line [0………………………………………]   -g --graphics       □                  │
+│           -u --lines-per-page [0………………………………………]   -l --just-left-only □                  │
+│ Chapters  -c --contents-title [Contents……………………]   -i --index-title    [Index……………………………] │
+│           -f --figures-title  [Figures………………………]   -F --caption-prefix [Figure…………………………] │
+│           -m --chapter-offset [0………………………………………]                                          │
+│ Pages     -p --page-headers  ◎ no ○ fullpage ○ picture ○ chapter ○ double                 │
+│           -e --even-left      [%n……………………………………]   -E --even-right     [%f……………………………………] │
+│           -o --odd-left       [%c……………………………………]   -O --odd-right      [%n……………………………………] │
+│           -n --page-offset    [0………………………………………]   -a --all-pages-E-e  □                  │
+│           -s --second-line  ○ no ○ blanks ○ points ○ dashes ◎ solid                       │
+│ Export    -X --export-pdf  ◎ no ○ export ○ browse  -C --correct  ○ no ◎ default ○ file    │
+│           -Y --pdf-browser    [atril……………………………]   -P --file-pdf       [%f%e.pdf……………………] │
+│           -W --char-width     [0………………………………………]   -A --char-aspect    [3/5…………………………………] │
+│           -S --sheet-size     [A4……………………………………]   -Z --landscape      □                  │
+│           -L --left-margin    [2cm…………………………………]   -R --right-margin   [2cm…………………………………] │
+│           -T --top-margin     [2cm…………………………………]   -B --bottom-margin  [2cm…………………………………] │
+│           -I --multi-pages    ◎ 1 ○ 2 ○ 4 ○ 8      -J --multi-sheets   [0………………………………………] │
+│ Text File ………………………………………………………………………………………………………………………………………………………………………………………………………………… │
+│ ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐ │
+│ │    New     │ │    Open    │ │   Recent   │ │   SaveAs   │ │    Help    │ │    Exit    │ │
+│ └────────────┘ └────────────┘ └────────────┘ └────────────┘ └────────────┘ └────────────┘ │
+│ ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐ ┌────────────┐                │
+│ │    Edit    │ │   Format   │ │  NoFormat  │ │    Undo    │ │    Log     │                │
+│ └────────────┘ └────────────┘ └────────────┘ └────────────┘ └────────────┘                │
+└───────────────────────────────────────────────────────────────────────────────────────────┘
 
 These are the buttons in GUI Main window:
 
-    • 4 buttons dedicated to the selection of the text file:
-        • New button: create a new empty text file
-        • Open button: browse the file system to select the text file
-        • Recent button: browse the list of recent files to select the text file
-        • Saveas button: clone current text file into a new target text file
-    • Help button: browse the YAWP Manual through the PDF browser defined by -Y
-    • Exit button: save current text file with its arguments and finish
-    • 4 buttons dedicated to the processing of the text file:
-        • Edit button: edit the text file through the text editor defined by -y
-        • Format button: process the text file by formatting it
-        • Noformat button: process the text file without formatting it
-        • Undo button: restore the text file to its previous content
-    • Log button: browse the log file through the text editor defined by -y
-    • Correct button: manage the correction file (Edit Reset or Undo)
+    • 4 buttons to the select the text file:
+        • New: create a new empty text file
+        • Open: browse the file system to select the text file
+        • Recent: browse the list of recent files to select the text file
+        • Saveas: clone current text file into a new target text file
+    • Help: browse the YAWP Manual by the PDF browser defined by -Y
+    • Exit: save current text file with its arguments and finish
+    • 4 buttons to process the text file:
+        • Edit: edit the text file by the text editor defined by -y
+        • Format: process the text file by formatting it
+        • Noformat: process the text file without formatting it
+        • Undo: restore the text file to its previous content
+    • Log: browse the log file by the text editor defined by -y
 
 '''
 
-__version__ = '1.0.0b10'
+#----- constants -----
+
+__version__ = '1.1.0' # YAWP present version
+VERSION_DATE = '2024-02-17' # 'YYYY-mm-dd' date of YAWP present version
+ECHO = True # echo at console the commands passed to shell() (debug only)
+ROUND = 5 # decimal digits in float representation
+phi = 1.618033988749895 # golden ratio
+STRIP_CHARS = ' \n\r\t' # chars for *strip(), no other whitespace as formfeed '\f' no-break space '\xa0' etc.
 
 #----- imports -----
 
 from fnmatch import fnmatchcase
 from glob import glob
-from os import chdir, lstat, popen, sep as path_sep
-from os.path import split as splitpath, abspath, expanduser, normpath, splitext, exists, isfile, isdir, basename, dirname
+from itertools import count
+from os import chdir, lstat, makedirs, rename, popen, remove, sep as pathsep
+from os.path import split as splitpath, abspath, expanduser, getmtime, getsize, normpath, splitext, exists, isfile, isdir, basename, dirname
+from shutil import copy2
 from subprocess import run, PIPE
 from sys import exit, stdout, stderr
-from time import localtime, sleep
+from time import localtime, sleep, time
 import readline
 
+#----- two-chars functions -----
+
+def cd(path):
+    'change directory to path, if existing'
+    if isdir(path):
+        chdir(path)
+
+def cp(file, file2):
+    'copy file into file2, if existing, else remove file2'
+    if isfile(file):
+        copy2(file, file2)
+    elif isfile(file2):
+        remove(file2)
+
+def md(path):
+    'make directory, if not existing'
+    makedirs(path, exist_ok=True)
+
+def mv(file, file2):
+    'move file into file2, if existing'
+    if isfile(file):
+        rename(file, file2)
+
+def rm(file):
+    'remove file, if existing'
+    if isfile(file):
+        remove(file)
+
+#----- various functions -----
+
+def tryfunc(func, *args):
+    'try: return func(*args); except: return None'
+    try:
+        return func(*args)
+    except:
+        return None
+
+def timefunc(n, func, *args):
+    'howmany seconds to call func(*args) n times?'
+    t0 = time()
+    for j in range(n):
+        func(*args)
+    return time() - t0
+
+def check(assertion):
+    'if not assertion: raise ValueError'
+    if not assertion:
+        raise ValueError
+
+def types(*args):
+    '>>> types(var1, typ1, var2, (typ2a, typ2b))'
+    check(len(args) % 2 == 0)
+    for j in range(0, len(args), 2):
+        var, typs = args[j:j+2]
+        if not isinstance(var, typs):
+            raise TypeError
+
 #----- string functions -----
 
-def hold(string, charpattern, default=''):
+def hold(string, charpattern, default='', joinby=''):
     'hold charpattern-matching chars in string and replace not matching chars with default'
-    return ''.join(char if fnmatchcase(char, charpattern) else default for char in string)
+    return joinby.join(char if fnmatchcase(char, charpattern) else default for char in string)
 
-def take(string, charset, default=''):
+def take(string, charset, default='', joinby=''):
     'take chars in string found in charset and replace not found chars with default'
-    return ''.join(char if char in charset else default for char in string)
+    return joinby.join(char if char in charset else default for char in string)
 
-def drop(string, charset, default=''):
+def drop(string, charset, default='', joinby=''):
     'drop chars in string found in charset and replace not found chars with default'
-    return ''.join(default if char in charset else char for char in string)
+    return joinby.join(default if char in charset else char for char in string)
 
 def chars(charpattern):
     'return a sorted string of all charpattern-matching characters'
     kernel = charpattern[1:-1]
     a, z = ord(min(kernel)), ord(max(kernel)) + 1
     return ''.join(chr(j) for j in range(a, z) if fnmatchcase(chr(j), charpattern))
 
+def line2stmt(line):
+    """return stripped statement, removing '#'-comments,
+but preserving '#' quoted by "'" or '"' or '\…' """
+    auto = 0; value = ''
+    for char in line:
+        if auto == 0:
+            if char == '#': break
+            elif char == '\\': value += char; auto = 10
+            elif char == "'": value += char; auto = 1
+            elif char == '"': value += char; auto = 2
+            else: value += char
+        elif auto == 1:
+            if char == '\\': value += char; auto = 11
+            elif char == "'": value += char; auto = 0
+            else: value += char
+        elif auto == 2:
+            if char == '\\': value += char; auto = 12
+            elif char == '"': value += char; auto = 0
+            else: value += char
+        elif auto == 10:
+            value += char; auto = 0
+        elif auto == 11:
+            value += char; auto = 1
+        elif auto == 12:
+            value += char; auto = 2
+    return value.strip()
+
 def ispattern(string):
     'is string a fnmatch pattern?'
     return bool(take(string, '?*['))
 
 def split_lines(string):
-    "split_lines('aaa\nbbb\n') -> ['aaa', 'bbb'], split_lines('') -> []"
-    string = string.rstrip()
-    return [] if not string else [line.rstrip() for line in string.split('\n')]
+    "split_lines('aaa \nbbb \n') -> ['aaa', 'bbb'], split_lines('') -> []"
+    string = rstrip(string)
+    return [] if not string else [rstrip(line) for line in string.split('\n')]
 
 def replace(string, *oldsnews):
     'replace(string, a, b, c, d, ...) == string.replace(a, b).replace(c, d)...'
-    for j in range(0, len(oldsnews), 2):
-        string = string.replace(oldsnews[j], oldsnews[j+1])
+    for old, new in slices(oldsnews, 2):
+        string = string.replace(old, new)
     return string
 
 def evalchar(string, olds, news, char='%'):
     '''for old, new in zip(olds, news): string = string.replace(char + old, new)
 on error raise ValueError('%x')'''
     trans = {old: new for old, new in zip(olds, news)}
     trans[char] = char # char + char --> char
@@ -198,34 +323,17 @@
             else:
                 j += 1
         else:
             value += charj
         j += 1
     return value
 
-def shrink(string, joinby=' ', splitby=None):
-    'eliminate from string all leading, multiple and trailing blanks'
-    return joinby.join(string.split(splitby))
-
-def adjust(string, length, align='!'):
-    "adjust string, align: '<'=left, '!'=center, '>'=right"
-    return (string.ljust(length) if align == '<' else
-            string.rjust(length) if align == '>' else
-            string.center(length))
-
-def frame(lines, align='!'):
-    "frame around lines, align: '<'=left, '!'=center, '>'=right"
-    if isinstance(lines, str):
-        lines = lines.split('\n')
-    length = max(len(line) for line in lines)
-    updown = (length + 2) * '─'
-    result = [f'┌{updown}┐']
-    for line in lines:
-        result.append(f'│ {adjust(line, length, align)} │')
-    return '\n'.join(result + [f'└{updown}┘'])
+def just(string, length, align='^'):
+    "align: '<'=left, '^'=center, '>'=right"
+    return {'<': str.ljust, '^': str.center, '>': str.rjust}[align](string, length)
 
 def expand(string, width):
     "insert blanks into string until len(string) == width, on error return ''"
     string = shrink(string)
     if len(string) == width:
         return string
     if ' ' not in string[1:] or len(string) > width:
@@ -253,99 +361,43 @@
         if fnmatchcase(char, pattern):
             return j
     else:
         return -1
 
 def prevchar(char):
     """>>> prevchar('b')
-'a'
-"""
+'a'"""
     return chr(ord(char) - 1)
 
 def nextchar(char):
     """>>> nextchar('a')
-'b'
-"""
+'b'"""
     return chr(ord(char) + 1)
 
-def chrs(list):
+def chrs(jj):
     """>>> chrs([97, 98, 99])
-'abc'
-"""
-    return ''.join(chr(j) for j in list)
+'abc'"""
+    return ''.join(chr(j) for j in jj)
 
-def ords(string):
+def ords(s):
     """>>> ords('abc')
-[97, 98, 99]
-"""
-    return [ord(char) for char in string]
-
-def unqupper(string, quotes='"'):
-    '''uppercase unquoted chars in string
-'''
-    result = ''; quote = ''
-    for char in string:
-        if quote:
-            result += char
-            if char == quote:
-                quote = ''
-        else:
-            result += char.upper()
-            if char in quotes:
-                quote = char
-    return result
-
-def unqlower(string, quotes='"'):
-    '''lowercase unquoted chars in string'''
-    result = ''; quote = ''
-    for char in string:
-        if quote:
-            result += char
-            if char == quote:
-                quote = ''
-        else:
-            result += char.lower()
-            if char in quotes:
-                quote = char
-    return result
-
-def unqtitle(string, quotes='"'):
-    '''titlecase unquoted chars in string'''
-    result = ''; quote = ''; first = True
-    for char in string:
-        if quote:
-            result += char
-            first = True
-            if char == quote:
-                quote = ''
-        elif char.isalpha():
-            result += char.upper() if first else char.lower()
-            first = False
-        else:
-            result += char
-            first = True
-            if char in quotes:
-                quote = char
-    return result
-
-def equivalent(string, string2):
-    'return titlecase(shrink(string)) == titlecase(shrink(string2))'
-    return titlecase(shrink(string)) == titlecase(shrink(string2))
+[97, 98, 99]"""
+    return [ord(c) for c in s]
 
 def plural(num, sing, plur=''):
     '''return f'1 {sing}' if num == 1 else f'{num} {plur}' if plur else f'{num} {sing}s'
->>> print(plural(1, 'cat'))
+>>> plural(1, 'cat')
 1 cat
->>> print(plural(3, 'cat'))
+>>> plural(3, 'cat')
 3 cats
->>> print(plural(1, 'mouse'))
+>>> plural(1, 'mouse')
 1 mouse
->>> print(plural(3, 'mouse'))
+>>> plural(3, 'mouse')
 3 mouses
->>> print(plural(3, 'mouse', 'mice'))
+>>> plural(3, 'mouse', 'mice')
 3 mice
 '''
     return f'1 {sing}' if num == 1 else f'{num} {plur}' if plur else f'{num} {sing}s'
 
 def edit(item, width=0, ndig=None, right=False):
     if isinstance(item, int):
         return str(item).rjust(width)
@@ -353,90 +405,239 @@
         string = str(item if ndig is None else round(item, ndig))
         return (string[:-2] if string.endswith('.0') else string).rjust(width)
     elif right:
         return str(item).rjust(width)
     else:
         return str(item).ljust(width)
 
-def table(head, body, ndig=None):
-    '''
->>> for line in table(('n', 'n2', 'n3'),
-    [(n, n * n, n ** 3) for n in range(11)]):
-    print(f'    {line}')
-
-    ┌──┬───┬────┐
-    │N │ N2│ N3 │
-    ├──┼───┼────┤
-    │ 0│  0│   0│
-    │ 1│  1│   1│
-    │ 2│  4│   8│
-    │ 3│  9│  27│
-    │ 4│ 16│  64│
-    │ 5│ 25│ 125│
-    │ 6│ 36│ 216│
-    │ 7│ 49│ 343│
-    │ 8│ 64│ 512│
-    │ 9│ 81│ 729│
-    │10│100│1000│
-    └──┴───┴────┘
-'''
-    head = [name.upper() for name in head]
-    widths = [len(name) for name in head]
-    lenhead = len(head)
-    result = []
-    for jrow, row in enumerate(body):
-        row = tuple(row[:lenhead]) + (lenhead - len(row)) * ('',)
-        for jcol, item in enumerate(row):
-            widths[jcol] = max(widths[jcol], len(edit(item, 0, ndig)))
-        body[jrow] = row
-    result.append('┌' + '┬'.join(width * '─' for width in widths) + '┐')
-    result.append('│' + '│'.join(name.center(width) for name, width in zip(head, widths)) + '│')
-    result.append('├' + '┼'.join(width * '─' for width in widths) + '┤')
-    for row in body:
-        result.append('│' + '│'.join(edit(item, width, ndig) for item, width in zip(row, widths)) + '│')
-    result.append('└' + '┴'.join(width * '─' for width in widths) + '┘')
-    return result
+#----- roman numbers -----
 
 def int2roman(number):
-    '''
->>> int2roman(0)
+    """>>> int2roman(0) # min
 ''
->>> int2roman(3999)
+>>> int2roman(3888) # longest (15 chars)
+'mmmdccclxxxviii'
+>>> int2roman(3999) # max
 'mmmcmxcix'
-'''
-    if number not in range(4000):
-        raise ValueError
+>>> all(n == roman2int(int2roman(n)) for n in range(4000))
+True"""
+    check(number in range(4000))
     m, c, x, i = [int(digit) for digit in f'{number:04}']
     return (['','m','mm','mmm'][m] +
             ['','c','cc','ccc','cd','d','dc','dcc','dccc','cm'][c] +
             ['','x','xx','xxx','xl','l','lx','lxx','lxxx','xc'][x] +
             ['','i','ii','iii','iv','v','vi','vii','viii','ix'][i])
 
-#----- path & file functions -----
+def roman2int(roman):
+    """>>> roman2int('') # min
+0
+>>> roman2int('mmmdccclxxxviii') # longest (15 chars)
+3888
+>>> roman2int('mmmcmxcix') # max
+3999
+>>> all(n == roman2int(int2roman(n)) for n in range(4000))
+True"""
+    num = 0
+    for char in replace(roman.strip().lower(), 'cd','cccc', 'cm','dcccc',
+                                               'xl','xxxx', 'xc','lxxxx',
+                                               'iv','iiii', 'ix','viiii'):
+        try:
+            num += {'m':1000, 'd':500, 'c':100, 'l':50, 'x':10, 'v':5, 'i':1}[char]
+        except KeyError:
+            raise ValueError
+    return num
+
+#----- *strip split shrink* eq/ne_upper() -----
+
+def lstrip(string):
+    'strip leading STRIP_CHARS'
+    return string.lstrip(STRIP_CHARS)
+
+def rstrip(string):
+    'strip trailing STRIP_CHARS'
+    return string.rstrip(STRIP_CHARS)
+
+def strip(string):
+    'strip leading and trailing STRIP_CHARS'
+    return string.strip(STRIP_CHARS)
+
+def split(string):
+    "split string into a list of notempty words separated by space ' ' and tab '\t'"
+    return [word for word in string.replace('\t',' ').split(' ') if word]
+
+def shrink(string):
+    "strip leading trailing and intermediate multiple space ' ' and tab '\t' chars"
+    return ' '.join(split(string))
+
+def shrink_alphaupper(string):
+    'shrink and uppercase alphabetic words'
+    return ' '.join(word.upper() if word.isalpha() else word for word in split(string))
+
+def shrink_alphalower(string):
+    'shrink and lowercase alphabetic words'
+    return ' '.join(word.lower() if word.isalpha() else word for word in split(string))
+
+def shrink_alphatitle(string):
+    'shrink and titlecase alphabetic words'
+    return ' '.join(word.title() if word.isalpha() else word for word in split(string))
+
+def eq_alphaupper(string, string2):
+    'return shrink_alphaupper(string) == shrink_alphaupper(string2)'
+    return shrink_alphaupper(string) == shrink_alphaupper(string2)
+
+def ne_alphaupper(string, string2):
+    'return shrink_alphaupper(string) != shrink_alphaupper(string2)'
+    return shrink_alphaupper(string) != shrink_alphaupper(string2)
+
+#----- frame xframe table xtable -----
+
+def frame(lines, align='^'):
+    """lines is a list of strings or a single string
+align is '<', '^' or '>'
+return frame as a single string"""
+    return '\n'.join(xframe(lines, align=align))
+
+def xframe(lines, align='^'):
+    """lines is a list of strings or a single string
+align is '<', '^' or '>'
+yield frame as strings"""
+    if isinstance(lines, str):
+        lines = lines.split('\n')
+    length = max(len(line) for line in lines)
+    updown = (length + 2) * '─'
+    yield f'┌{updown}┐'
+    for line in lines:
+        yield f'│ {just(line, length, align)} │'
+    yield f'└{updown}┘'
+
+def table(head, body):
+    '''head is a tuple of column names, optionally followed by ':' and format
+body is a list of tuples of items
+an item is bool int float or str
+return table as a single string
+>>> print(table(('N', 'N/7:.3f'), [(n, n/7) for n in range(11)]))
+┌──┬─────┐
+│N │ N/7 │
+├──┼─────┤
+│ 0│0.000│
+│ 1│0.143│
+│ 2│0.286│
+│ 3│0.429│
+│ 4│0.571│
+│ 5│0.714│
+│ 6│0.857│
+│ 7│1.000│
+│ 8│1.143│
+│ 9│1.286│
+│10│1.429│
+└──┴─────┘'''
+    return '\n'.join(xtable(head, body))
+
+def xtable(head, body):
+    '''head is a tuple of column columns,
+    optionally followed by ':' and format
+body is a list of tuples of items
+an item is bool int float or str
+yield table as strings'''
+    convert = lambda value, formatj, length: (str.ljust if isinstance(value, str) else str.rjust)(format(value, formatj), length)
+    columns = [word.split(':')[0] for word in head]
+    formats = [(word+':').split(':')[1] for word in head]
+    lengths = [len(column) for column in columns]
+    for values in body:
+        values = values[:len(head)] + (len(head) - len(values)) * ('',)
+        for jcol, (value, formatj) in enumerate(zip(values, formats)):
+            lengths[jcol] = max(lengths[jcol], len(format(value, formatj)))
+    yield '┌' + '┬'.join(length * '─' for length in lengths) + '┐'
+    yield '│' + '│'.join(column.center(length) for column, length in zip(columns, lengths)) + '│'
+    yield '├' + '┼'.join(length * '─' for length in lengths) + '┤'
+    for values in body:
+        yield '│' + '│'.join(convert(value, formatj, length) for value, formatj, length in zip(values, formats, lengths)) + '│'
+    yield '└' + '┴'.join(length * '─' for length in lengths) + '┘'
+
+#----- time functions -----
+
+def now(seconds=None):
+    "return 'YYYY-mm-dd HH:MM:SS' from seconds or current time'"
+    Y, m, d, H, M, S = localtime(seconds)[:6]
+    return f'{Y:04d}-{m:02d}-{d:02d} {H:02d}:{M:02d}:{int(S):02d}'
+
+def get_YmdHMS(seconds=None):
+    "return ('YYYY','mm','dd','HH','MM','SS') from seconds or current time"
+    Y, m, d, H, M, S = localtime(seconds)[:6]
+    return tuple(f'{Y:04d} {m:02d} {d:02d} {H:02d} {M:02d} {S:02d}'.split())
+
+def is_leap_year(Y):
+    """
+is Y a leap year? (proleptic gregorian calendar)
+>>> [y for y in range(1000, 3001, 100) if is_leap_year(y)]
+[1200, 1600, 2000, 2400, 2800]
+>>> [y for y in range(1980, 2021) if is_leap_year(y)]
+[1980, 1984, 1988, 1992, 1996, 2000, 2004, 2008, 2012, 2016, 2020]
+"""
+    return Y % 4 == 0 and (Y % 100 != 0 or Y % 400 == 0)
+
+def year_days(Y):
+    "number of days in year Y (proleptic gregorian calendar)"
+    return 365 + is_leap_year(Y)
+
+def month_days(Y, m):
+    "number of days in month m of year Y (proleptic gregorian calendar)"
+    return [31, 28 + is_leap_year(Y), 31, 30, 31, 30, 31, 31, 30, 31, 30, 31][m - 1]
+
+def is_date_time(Y, m, d, H=0, M=0, S=0, Ymin=0, Ymax=9999):
+    "is date (and time) correct?"
+    return (Ymin <= Y <= Ymax and 1 <= m <= 12 and 1 <= d <= month_days(Y, m) and
+            0 <= min(H, M, S) <= max(H, M, S) <= 59)
+
+def easter_month_day(Y):
+    """return Easter date of year Y as (month, day)
+>>> for Y in range(2020, 2030): print(Y, easter_month_day(Y))
+2020, (4, 12)
+2021, (4, 4)
+2022, (4, 17)
+2023, (4, 9)
+2024, (3, 31)
+2025, (4, 20)
+2026, (4, 5)
+2027, (3, 28)
+2028, (4, 16)
+2029, (4, 1)
+"""
+    a = Y % 19
+    b = Y // 100
+    c = Y % 100
+    d = (19 * a + b - b // 4 - ((b - (b + 8) // 25 + 1) // 3) + 15) % 30
+    e = (32 + 2 * (b % 4) + 2 * (c // 4) - d - (c % 4)) % 7
+    f = d + e - 7 * ((a + 11 * d + 22 * e) // 451) + 114
+    return f // 31, f % 31 + 1
 
-def join_path(*paths):
-    '''
->>> join_path('/a/b/', '/c/d.e')
-'/a/b/c/d.e'
->>> join_path('/a/b', 'c/d.e')
-'/a/b/c/d.e'
-''' 
-    return normpath(path_sep.join(paths))
+#----- path & file functions -----
 
-def long_path(path='.'):
-    path = (path or '').strip()
+def filesize(file):
+    'return size of file in bytes'
+    return getsize(file)
+
+def filetime(file):
+    "return last modification time of file in 'YYYY-mm-dd HH:MM:SS' format"
+    return now(getmtime(file))
+
+def longpath(path):
+    'return abspath(expanduser(path))'
+    path = path.strip()
     return '' if not path else abspath(expanduser(path))
 
-def short_path(path='.'):
-    path, home = long_path(path), long_path('~')
-    return '' if not path else '~' + path[len(home):] if path.startswith(home) else path
+def shortpath(path):
+    "return '~/...' if applicable"
+    path = longpath(path)
+    home = longpath('~')
+    return '~' + path[len(home):] if path.startswith(home) else path
 
 def get_files(pattern):
     "return a list of absolute paths to pattern-matching files ('**' in path is allowed)"
-    return [file for file in glob(long_path(pattern), recursive=True) if isfile(file)]
+    return sorted(file for file in glob(longpath(pattern), recursive=True) if isfile(file))
 
 def get_file(pattern):
     "return unique pattern-matching file, or '' if not found or ambiguous"
     files = get_files(pattern)
     return files[0] if len(files) == 1 else ''
 
 def get_lines(file):
@@ -455,46 +656,44 @@
     "return the newest path_file among matching path_files, or raise FileNotFoundError if not found"
     files = get_files(pattern)
     if files:
         return max((lstat(file).st_mtime, file) for file in files)[1]
     else:
         raise FileNotFoundError
 
-def get_PpfFeYmdHMS(file):
-    '''return (P, p, f, F, e, Y, m, d, H, M, S), where:
-    • P is long path to file, without final '/'
-    • p is short path to file, without final '/'
-    • f is file name, with no extension
-    • F is file name, with no extension, spaced and titlecased
-    • e is file extension, starting with '.'
-    • Y is 4-digit current year
-    • m, d, H, M, S are 2-digit current month, day, hour, minute, second'''
-    P, f_e = splitpath(long_path(file))
-    p = short_path(P)
-    f, e = splitext(f_e)
-    F = hold(f, '[a-zA-Z0-9]', ' ').title()
-    return (P, p, f, F, e) + get_YmdHMS()
-
 def new_file(pattern, char='%'):
     'return not existing expanded pathfile, initialize file as empty'
     while True:
-        file = long_path(evalchar(pattern, 'YmdHMS', get_YmdHMS(), char=char))
+        file = longpath(evalchar(pattern, 'YmdHMS', get_YmdHMS(), char=char))
         if char in pattern and isfile(file):
             sleep(0.1)
         else:
             open(file, 'w').write('')
             return file
-        
+
+def PpfeYmdHMS_of(file):
+    '''return (P, p, f, e, Y, m, d, H, M, S), where:
+    • P is long path to file, without final '/'
+    • p is short path to file, without final '/'
+    • f is file name, with no extension
+    • e is file extension, starting with '.'
+    • Y is 4-digit current year
+    • m, d, H, M, S are 2-digit current month day hour minute and second'''
+    P, fe = splitpath(longpath(file))
+    p = shortpath(P)
+    f, e = splitext(fe)
+    return (P, p, f, e) + get_YmdHMS()
+
 def local_file(pathfile):
     'return absolute path of a package relative pathfile'
     return normpath(f'{dirname(__file__)}/{pathfile}')
 
 def get_dirs(pattern):
     "return a list of absolute paths to pattern-matching dirs ('**' in path is allowed)"
-    return [path for path in glob(long_path(pattern), recursive=True) if isdir(path)]
+    return [path for path in glob(longpath(pattern), recursive=True) if isdir(path)]
 
 def get_dir(pattern):
     "return unique pattern-matching dir, or '' if not found or ambiguous"
     dirs = get_dirs(pattern)
     return dirs[0] if len(dirs) == 1 else ''
 
 def chdir2(pattern='~'):
@@ -505,165 +704,253 @@
     elif len(paths) > 1:
         print(f'cd: path {pattern!r} is ambiguous', file=stderr)
     else:
         chdir(paths[0])
 
 #----- sequence functions -----
 
-def retroenum(sequence):
-    'like enumerate(sequence), but backwards from last to first item'
-    for j in range(len(sequence) - 1, -1, -1):
-        yield j, sequence[j]
-
-def find(sequence, item):
-    'return index of first item found in sequence, or -1 if not found'
-    for j, itemj in enumerate(sequence):
-        if itemj == item:
+def find(xx, x):
+    'find min j such that xx[j] == x, return -1 if not found'
+    for j, xj in enumerate(xx):
+        if xj == x:
             return j
     else:
         return -1
 
-def rfind(sequence, item):
-    'return index of last item found in sequence, or -1 if not found'
-    for j, itemj in retroenum(sequence):
-        if itemj == item:
+def rfind(xx, x):
+    'find max j such that xx[j] == x, return -1 if not found'
+    jok = -1
+    for j, xj in enumerate(xx):
+        if xj == x:
+            jok = j
+    return jok
+
+def finddup(xx):
+    'find min j such that xx[j] == xx[i] for some i < j, return -1 if not found'
+    xset = set()
+    for j, xj in enumerate(xx):
+        if xj in xset:
             return j
+        xset.add(xj)
     else:
         return -1
 
-def index(sequence, item):
-    'return index of first item found in sequence, or raise ValueError if not found'
-    for j, itemj in enumerate(sequence):
-        if itemj == item:
-            return j
-    else:
-        raise ValueError('item not found')
+def rfinddup(xx):
+    'find max j such that xx[j] == xx[i] for some i < j, return -1 if not found'
+    xset = set()
+    jok = -1
+    for j, xj in enumerate(xx):
+        if xj in xset:
+            jok = j
+        else:
+            xset.add(xj)
+    return jok
 
-def rindex(sequence, item):
-    'return index of last item found in sequence, or raise ValueError if not found'
-    for j, itemj in retroenum(sequence):
-        if itemj == item:
-            return j
-    else:
-        raise ValueError('item not found')
+def findmin(xx):
+    'find min j such that xx[j] == min(xx), return -1 if not found'
+    jmin = -1
+    for j, xj in enumerate(xx):
+        if j == 0 or xj < xmin:
+            jmin = j
+            xmin = xj
+    return jmin
+
+def rfindmin(xx):
+    'find max j such that xx[j] == min(xx), return -1 if not found'
+    jmin = -1
+    for j, xj in enumerate(xx):
+        if j == 0 or xj <= xmin:
+            jmin = j
+            xmin = xj
+    return jmin
+
+def findmax(xx):
+    'find min j such that xx[j] == max(xx), return -1 if not found'
+    jmax = -1
+    for j, xj in enumerate(xx):
+        if j == 0 or xj > xmax:
+            jmax = j
+            xmax = xj
+    return jmax
+
+def rfindmax(xx):
+    'find max j such that xx[j] == max(xx), return -1 if not found'
+    jmax = -1
+    for j, xj in enumerate(xx):
+        if j == 0 or xj >= xmax:
+            jmax = j
+            xmax = xj
+    return jmax
+
+def slices(xx, n):
+    """>>> list(slices('0123456789', 2)) # str
+['01', '23', '45', '67', '89']
+>>> list(slices(list('0123456789'), 2)) # list
+[['0', '1'], ['2', '3'], ['4', '5'], ['6', '7'], ['8', '9']]
+>>> list(slices(tuple('0123456789'), 2)) # tuple
+[('0', '1'), ('2', '3'), ('4', '5'), ('6', '7'), ('8', '9')]
+>>> list(slices((str(j) for j in range(10)), 2)) # generator
+[['0', '1'], ['2', '3'], ['4', '5'], ['6', '7'], ['8', '9']]"""
+    check(n > 0)
+    func = tuple if isinstance(xx, tuple) else (lambda yy: ''.join(yy)) if isinstance(xx, str) else (lambda yy: yy)
+    slice = []
+    for jx, x in enumerate(xx):
+        slice.append(x)
+        if len(slice) == n:
+            yield func(slice)
+            slice = []
+    check((jx + 1) % n == 0)
+
+def retroenum(xx):
+    'like enumerate(xx), but backwards from last to first item'
+    if '__getitem__' not in dir(xx):
+        xx = list(xx)
+    for j in range(len(xx) - 1, -1, -1):
+        yield j, xx[j]
 
 def get(xx, j, default=None):
     'return xx[j] if 0 <= j < len(xx) else default'
     return xx[j] if 0 <= j < len(xx) else default
 
 def unique(xx):
-    'return copy of list xx with no duplicates'
-    olds = set()
-    result = []
+    'return a list of items in xx discarding duplicates'
+    zz = set()
+    yy = []
     for x in xx:
-        if x not in olds:
-            olds.add(x)
-            result.append(x)
-    return result
+        if x not in zz:
+            zz.add(x)
+            yy.append(x)
+    return yy
 
 #----- shell functions -----
 
-def shell(command, echo=False):
+def shell(line, echo=ECHO, stdout=False):
+    'execute shell command in line, print errors into stderr, return output as list of strings'
     if echo:
-        print('--> ' + command)
-    nocomment = command.split('#')[0].strip()
-    if nocomment == 'exit' or nocomment.startswith('exit '):
+        print('--> ' + line)
+    command = line2stmt(line)
+    if command == 'exit':
         raise SystemExit
-    elif nocomment == 'cd' or nocomment.startswith('cd '):
-        where = nocomment[3:].strip() or '~'
-        paths = glob(long_path(where))
+    elif command == 'cd' or command.startswith('cd '):
+        where = command[3:].strip() or '~'
+        paths = glob(longpath(where))
         if not paths:
             print(f'cd: {where!r}: No such file or directory', file=stderr)
         elif len(paths) > 1:
             print(f'cd: too many arguments', file=stderr)
         else:
             chdir(paths[0])
         return []
     else:
-        result = run(command.strip(), shell=True, text=True, capture_output=True)
+        result = run(command, shell=True, text=True, capture_output=True)
         for line in split_lines(result.stderr):
             print(line, file=stderr)
         return split_lines(result.stdout)
 
 def term():
-    print(frame('term - minimalistic terminal'))
+    "minimalistic terminal, type 'exit' to exit"
+    print(50 * '<')
     while True:
         try:
-            command = input(f"{abspath('.')} $ ")
+            inline = input(f"{shortpath('.')} $ ")
             try:
-                for line in shell(command):
-                    print(line)
+                for outline in shell(inline):
+                    print(outline)
             except SystemExit:
-                break
+                print(50 * '>')
+                return
         except KeyboardInterrupt:
             print('^C')
-    print(frame("term - terminated by 'exit'"))
 
 def command_exists(command):
     return bool(shell(f'which {command}'))
 
-#----- metric functions -----
+#----- conversion functions -----
 
 in2in = lambda In: float(In) # inch converters
 in2pt = lambda In: In * 72.0
 pt2in = lambda pt: pt / 72.0
 in2cm = lambda In: In * 2.54
 cm2in = lambda cm: cm / 2.54
 in2mm = lambda In: In * 25.4
 mm2in = lambda mm: mm / 25.4
+cc2in = {'pt': pt2in, 'in': in2in, 'mm': mm2in, 'cm': cm2in}
 
-def inch2str(inch, digits):
+def inch2str(inch, digits=ROUND):
     'convert float inch into a multi-unit human-readable string'
-    in2xx = {'pt': in2pt, 'in': in2in, 'mm': in2mm, 'cm': in2cm}
-    return ' = '.join(f"{in2xx[unit](inch):.{digits}f}{unit}" for unit in ['pt','in','mm','cm'])
+    return ' = '.join(str(round(in2cc(inch), digits)) + unit for in2cc, unit in [(in2pt, 'pt'), (in2in, 'in'),(in2mm, 'mm'),(in2cm, 'cm')])
 
 def str2inch(string):
-    "convert '{float}{suffix}' into an inch float value"
-    string = replace(string,' ','',',','.')
-    try:
-        assert float(string) == 0.0
+    "convert unsigned '{float}{suffix}' into float, on error raise ValueError"
+    check('-' not in string)
+    string = replace(string, ',', '.')
+    if tryfunc(float, string) == 0.0:
         return 0.0
-    except:
-        xx2in = {'pt': pt2in, 'in': in2in, 'mm': mm2in, 'cm': cm2in}
-        try:
-            value = xx2in[string[-2:]](float(string[:-2]))
-            assert value >= 0.0
-            return value
-        except:
-            raise ValueError
+    else:
+        x, cc = string[:-2], string[-2:]
+        check(cc in cc2in)
+        return cc2in[cc](float(x))
 
 def str2inxin(string):
-    "convert '{float}x{float}{suffix}' into two inch float values"
-    try:
-        a, b = string.split('x')
-        x, y = str2inch(a + b[-2:]), str2inch(b)
-        return (x, y)
-    except:
-        raise ValueError
-
-def ratio(string):
-    '''convert '{float}/{float}' or '{float}' into a float
-float value(s) must be positive
-'''
-    string = replace(string,' ','',',','.')
-    try:
-        r = float(string)
-        assert r > 0
-        return r
-    except (ValueError, AssertionError):
-        try:
-            a, b = string.split('/')
-            a, b = float(a), float(b)
-            assert a > 0 < b
-            return a / b
-        except (ValueError, AssertionError):
-            raise ValueError
+    "convert unsigned '{float}x{float}{suffix}' into (float, float), on error raise ValueError"
+    check('-' not in string)
+    string = replace(string, ',', '.')
+    xy, cc = string[:-2], string[-2:]
+    check(cc in cc2in)
+    x, y = [float(s) for s in xy.split('x')]
+    check(x > 0.0 < y)
+    return (cc2in[cc](x), cc2in[cc](y))
+
+def str2ratio(string):
+    "convert unsigned '{float}' or '{float}/{float}' into float, on error raise ValueError"
+    check('-' not in string)
+    string = replace(string, ',', '.')
+    if '/' not in string:
+        return float(string)
+    else:
+        x, y = [float(s) for s in string.split('/')]
+        check(x > 0.0 < y)
+        return x / y
+
+def str2int(string, min=0):
+    "convert '{int}' into int, on error raise ValueError"
+    n = int(string)
+    check(n >= min)
+    return n
 
 #----- numeric functions -----
 
+def is_perm(xx):
+    'is xx a permutation of list(range(len(xx)))?'
+    return sorted(xx) == list(range(len(xx)))
+
+def ceildiv(x, y):
+    'return ceil(x / y) # but by integer arithmetic only'
+    q, r = divmod(x, y)
+    return q + bool(r)
+
+def prod(xx):
+    'product of all x in xx'
+    p = 1
+    for x in xx:
+        p *= x
+    return p
+
+def fact(n):
+    'factorial'
+    return prod(range(2, n + 1)) if n >= 0 else 0
+
+def disp(n, k):
+    'dispositions'
+    return prod(range(n - k + 1, n + 1)) if 0 <= k <= n else 0
+
+def comb(n, k):
+    'combinations = binomial coefficient'
+    return disp(n, k) // fact(k) if 0 <= k <= n else 0
+
 def frange(start, stop=None, step=1.0, first=True, last=False):
     """float range
 >>> list(frange(0, 1, 1/3, last=True))
 [0.0, 0.3333333333333333, 0.6666666666666666, 1.0]
 >>> list(frange(1, 0, -1/3, last=True))
 [1.0, 0.6666666666666667, 0.33333333333333337, 0.0]"""
     if stop is None:
@@ -673,22 +960,36 @@
         yield start
     for j in range(1, round((stop - start) / step)):
         yield start + j * step
     if last:
         yield stop
 
 def difs(xx):
+    '''return [xx[0], xx[1] - xx[0], xx[2] - xx[1], ...]
+difs(sums(xx)) == sums(difs(xx)) == xx'''
     return [xj - xx[j-1] if j else xj for j, xj in enumerate(xx)]
-            
+
 def sums(xx):
+    '''return [xx[0], xx[0] + xx[1], xx[0] + xx[1] + xx[2], ...]
+difs(sums(xx)) == sums(difs(xx)) == xx'''
     yy = xx[:]
     for j in range(1, len(yy)):
         yy[j] += yy[j - 1]
     return yy
 
+def plus(xx, yy):
+    '''return [xx[0] + yy[0], xx[1] + yy[1], xx[2] + yy[2], ...]'''
+    check(len(xx) == len(yy))
+    return [(x + y) for x, y in zip(xx, yy)]
+
+def mins(xx, yy):
+    '''return [xx[0] - yy[0], xx[1] - yy[1], xx[2] - yy[2], ...]'''
+    check(len(xx) == len(yy))
+    return [(x - y) for x, y in zip(xx, yy)]
+
 def broken_line(xyxy, x):
     '''linear interpolation by broken line
 xyxy = [(x0, y0), (x1, y1), (x2, y2),...]
 0.0 <= x0 < x1 < x2 ...
 0.0 <= y0 < y1 < y2 ...'''
     n = len(xyxy)
     if n == 0: # straight line by [(0.0, 0.0), (1.0, 1.0)]
@@ -705,143 +1006,105 @@
         return a * x + b
     else: # broken line by [(x0, y0), (x1, y1), (x2, y2),...]
         for j, (x0, y0) in enumerate(xyxy):
             x1, y1 = xyxy[j + 1]
             if j >= n - 2 or x <= x1:
                 return y0 + (x - x0) * (y1 - y0) / (x1 - x0)
 
-def least_squares_line(xyxy, x):
+def least_squares_line(xyxy, x=None):
     '''linear interpolation by least-squares straight line
-xyxy = [(x0, y0), (x1, y1), (x2, y2),...]
-for j > 0: x[j] > x[j - 1] and y[j] > y[j -1 ]'''
+xyxy = [(x0, y0), (x1, y1), (x2, y2),...]'''
     n = len(xyxy)
     if n == 0: # straight line by [(0.0, 0.0), (1.0, 1.0)]
-        return  x
+        a, b = 1.0, 0.0
     elif n == 1: # straight line by [(0.0, 0.0), (x0, y0)]
         x0, y0 = xyxy[0]
-        return (y0 / x0) * x
+        a, b = y0 / x0, 0.0
     elif n == 2: # straight line by [(x0, y0), (x1, y1)]
         x0, y0 = xyxy[0]
         x1, y1 = xyxy[1]
         d = x1 - x0
         a = (y1 - y0) / d
         b = (y0 * x1 - y1 * x0) / d
-        return a * x + b
     else: # least-squares straight line by [(x0, y0), (x1, y1), (x2, y2),...]
         sx = sum(x for x, y in xyxy)
         sx2 = sum(x * x for x, y in xyxy)
         sy = sum(y for x, y in xyxy)
         sxy = sum(x * y for x, y in xyxy)
         d = n * sx2 - sx * sx
         a = (n * sxy - sx * sy) / d
         b = (sx2 * sy - sx * sxy) / d
-        return a * x + b
+    return (a, b) if x is None else a * x + b
 
 def moving_means(xx, n=7):
     """return [yy[j] = sum(xx[j+1-n:j+1]) / n]
 >>> moving_means(list(range(10)))
 [0.0, 0.5, 1.0, 1.5, 2.0, 2.5, 3.0, 4.0, 5.0, 6.0]
 >>> moving_means(list(range(10)), 3)
 [0.0, 0.5, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]
 """
     return [sum(xx[max(0, j + 1 - n): j + 1]) / min(n, j + 1) for j in range(len(xx))]
 
-#----- other functions -----
-
-def now():
-    "return 'YYYY-mm-dd HH:MM:SS'"
-    Y, m, d, H, M, S = localtime()[:6]
-    return f'{Y:04d}-{m:02d}-{d:02d} {H:02d}:{M:02d}:{S:02d}'
-
-def today():
-    "return 'YYYY-mm-dd'"
-    Y, m, d = localtime()[:3]
-    return f'{Y:04d}-{m:02d}-{d:02d}'
-
-def get_YmdHMS():
-    "return ('YYYY','mm','dd','HH','MM','SS')"
-    Y, m, d, H, M, S = localtime()[:6]
-    return tuple(f'{Y:04d} {m:02d} {d:02d} {H:02d} {M:02d} {S:02d}'.split())
-    
-def get_Ymd():
-    "return ('YYYY','mm','dd')"
-    Y, m, d = localtime()[:3]
-    return tuple(f'{Y:04d} {m:02d} {d:02d}'.split())
-    
-def try_func(func, args, on_error=None):
-    'try: return func(*args); except: return on_error'
-    try:
-        return func(*args)
-    except:
-        return on_error
-
-def try_func1(func, arg, on_error=None):
-    'try: return func(arg); except: return on_error'
-    try:
-        return func(arg)
-    except:
-        return on_error
-
-def idem(x):
-    'return x'
-    return x
-
-def dump(object, undertoo=False):
-    items = sorted((key, value) for key, value in object.__dict__.items() if undertoo or not key.startswith('_'))
-    length = max((len(key) for key, value in items), default=0)
-    for key, value in items:
-        value = (inch2str if isinstance(value, float) else str)(value)
-        print(f'    {edit(key, length)}\t = {value!r}')
-
-def show(names):
-    '''
->>> a, b, c = 'xyz'; show('a, b, c')
-a = 'x'
-b = 'y'
-c = 'z'
+def zerofunc(f, xa, xz, max_iter=100, trace=False):
+    '''return x such that f(x) = 0 by regula falsi
+f in [xa, xz] interval must:
+    1. be continuous and monotonic
+    2. have one and only one zero
+>>> zerofunc(lambda x: 1 / x - (x - 1), 0.5, 2.0) # golden ratio, 1 / x = x - 1
+1.618033988749895
+>>> zerofunc(lambda x: 1 / x - (x + 1), 0.5, 2.0) # inverse of golden ratio, 1 / x = x + 1
+0.6180339887498948
 '''
-    names = [name.strip() for name in names.split(',')]
-    for name in names:
-        var = eval(name)
-        if isinstance(var, tuple):
-            if not var:
-                print(name, '= ()')
-            else:
-                print(name, '= (')
-                for j, v in enumerate(var):
-                    print(f'    {v!r},')
-                print('    )')
-        elif isinstance(var, list):
-            if not var:
-                print(name, '= []')
-            else:
-                print(name, '= [')
-                for j, v in enumerate(var):
-                    print(f'    {v!r},')
-                print('    ]')
-        elif isinstance(var, dict):
-            if not var:
-                print(name, '= {}')
-            else:
-                print(name, '= {')
-                for j, (k, v) in enumerate(sorted(var.items())):
-                    print(f'    {k!r}: {v!r},')
-                print('    }')
-        elif isinstance(var, (set, frozenset)):
-            if not var:
-                print(name, '= set()')
-            else:
-                print(name, '= {')
-                for j, v in enumerate(sorted(var)):
-                    print(f'    {v!r},')
-                print('    }')
+    ya = f(xa); yz = f(xz); xh0 = None
+    for iter in range(max_iter):
+        xh = xa - ya * (xz - xa) / (yz - ya)
+        if xh == xh0:
+            return xh
+        xh0 = xh
+        yh = f(xh)
+        if trace:
+            print(f'x = {xh}, y = {yh}')
+        if yh == 0.0:
+            return xh
+        if yh * yz < 0.0:
+            xz = xh; yz = yh
         else:
-            print(f'{name} = {var!r}')
+            xa = xh; ya = yh
+    raise ValueError(f'Convergence not reached after {max_iter} iterations')
 
-#----- dict subclasses -----
+#----- dict functions and classes -----
+
+def sorted_items(dic, by_value=False, reverse=False):
+    'return dic.items() = [(key, value), ...] sorted by value if by_value else by key'
+    types(dic, dict)
+    key = (lambda kv: (kv[1], kv[0])) if by_value else None
+    return sorted(dic.items(), key=key, reverse=reverse)
+
+class IntDict(dict):
+    'dictionary of integers'
+
+    def __init__(getitem, keys=[]):
+        'initialize intdict by a sequence of keys'
+        for key in keys:
+            intdict.add(key)
+
+    def __getitem__(intdict, key):
+        'return intdict[key] if key in intdict else 0'
+        return intdict.get(key, 0)
+
+    def add(intdict, key):
+        'add a key to intdict'
+        if key not in intdict:
+            intdict[key] = 0
+        intdict[key] += 1
+
+    def extend(intdict, keys):
+        'extend intdict by a sequence of keys'
+        for key in keys:
+            intdict.add(key)
 
 class ListDict(dict):
     'dictionary of lists'
 
     def __getitem__(listdict, key):
         return listdict.get(key, [])
 
@@ -859,29 +1122,42 @@
     def add(setdict, key, value):
         if key not in setdict:
             setdict[key] = set()
         setdict[key].add(value)
 
 #----- PySimpleGUI-related functions -----
 
-def get_radio(window, start, chars):
+def get_radio(window, start, domain):
     ntrue = 0
-    for j, charj in enumerate(chars):
+    for j, valuej in enumerate(domain):
         if window[start + j].get():
             ntrue += 1
-            char = charj
-    if ntrue != 1:
-        raise ValueError
-    return char
+            value = valuej
+    check(ntrue == 1)
+    return value
+
+def get_radios(window, domains):
+    start = 0
+    for domain in domains:
+        yield get_radio(window, start, domain)
+        start += len(domain)
 
-def put_radio(window, start, chars, char):
+def put_radio(window, start, domain, value):
     ntrue = 0
-    for j, charj in enumerate(chars):
-        if charj == char:
+    for j, valuej in enumerate(domain):
+        if valuej == value:
             ntrue += 1
             window[start + j].update(True)
         else:
             window[start + j].update(False)
-    if ntrue != 1:
-        raise ValueError
- 
+    check(ntrue == 1)
+
+def put_radios(window, domains, values):
+    start = 0
+    for domain, value in zip(domains, values):
+        put_radio(window, start, domain, value)
+        start += len(domain)
+
 #----- end -----
+
+
+
```

### Comparing `yawp-1.0.0b10/yawp/__main__.py` & `yawp-2.0.0/yawp/.yawp.__main__.py.2024.03.06-12.03.08.back`

 * *Files 9% similar despite different names*

```diff
@@ -1,133 +1,130 @@
 #!/usr/bin/env python3
+'''
+                                ┌───────────────────────────────────┐
+                                │                                   ├─┐
+                                │      │   │ ┌───┐ │   │ ┌───┐      │ │
+                                │      │   │ │   │ │   │ │   │      │ │
+                                │      └─┬─┘ ├───┤ │ │ │ ├───┘      │ │
+                                │        │   │   │ │ │ │ │          │ │
+                                │        │   │   │ └─┴─┘ │          │ │
+                                │                                   │ │
+                                └─┬─────────────────────────────────┘ │
+                                  └───────────────────────────────────┘
+'''
 
 #----- imports -----
 
 from .__init__ import *
 from .__init__ import __version__ as VERSION, __doc__ as DESCRIPTION
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
-from fnmatch import fnmatchcase
-from glob import glob
-from os import makedirs as md, remove as rm, rename as mv, chdir as cd
-from pdfrw import PdfReader, PdfWriter
-from shutil import copy2 as cp
-from sys import argv, stderr
-from time import localtime, sleep
+from pdfrw import PdfReader, PdfWriter, PageMerge
+from sys import argv, stderr, stdout, platform
+from time import localtime, sleep, time
+from traceback import format_exc
 from warnings import simplefilter
 import PySimpleGUI as sg
 
 #----- constants -----
 
-EMPT, CODE, TEXT, PICT, CONT, FIGU, CAPT, INDX, CHP1, CHP2, HEA1, HEA2 = range(12) # line kinds
+EMPT, TEXT, PICT, CONT, FIGU, CAPT, INDX, CHP1, CHP2, HEA1, HEA2 = range(11) # line kinds in buf.buffer[KIND]
 
-KINDS = 'EMPT, CODE, TEXT, PICT, CONT, FIGU, CAPT, INDX, CHP1, CHP2, HEA1, HEA2'.split(', ')
-    # values in buf.buffer[KIND]
-    # EMPT empty line
-    # CODE Python code line
-    # TEXT text line
-    # PICT picture line
-    # CONT contents chapter line
-    # FIGU figure chapter line
-    # CAPT figure caption line
-    # INDX index chapter line
-    # CHP1 numbered chapter line, level == 1
-    # CHP2 numbered chapter line, level > 1
-    # HEA1 page header, first line
-    # HEA2 page header, second line
+KINDS = 'EMPT, TEXT, PICT, CONT, FIGU, CAPT, INDX, CHP1, CHP2, HEA1, HEA2'.split(', ')
+    # values in buf.buffer[KIND]:
+        # EMPT empty line
+        # TEXT text line
+        # PICT picture line
+        # CONT contents chapter line
+        # FIGU figure chapter line
+        # CAPT figure caption line
+        # INDX index chapter line
+        # CHP1 numbered chapter line, level == 1
+        # CHP2 numbered chapter line, level > 1
+        # HEA1 page header, first line
+        # HEA2 page header, second line
 
 JINP, KIND, JPAG, LPIC, LINE = range(5) # positions in buf.buffer
     # JINP line index in input file
     # KIND line kind, see before
     # JPAG page number
     # LPIC number of lines in picture
     # LINE content of line
 
 LABL, TITL, JOUT = range(3) # positions in buf.contents and buf.captions
-    # LABL chapter label, as '1.' in buf.contents or '1.a.' in buf.captions
+    # LABL chapter label, like '1.' in buf.contents or '1.a.' in buf.captions
     # TITL chapter title
     # JOUT line index in buf.buffer
 
+# characters
+INDENT = 4 * ' ' # standard indentation
 HORIZTAB = '\t' # horizontal tab, replaced by INDENT in input lines
-LINEFEED = '\n' # line separator
+LINEFEED = '\n' # line feed, standard Linux line separator
 CARRIAGE = '\r' # carriage return
-FORMFEED = '\f' # first character of first line of page headers
-MACRON = '¯' # characters of second line of page headers
-ZEROWIDTHSPACE = '\u200b' # character to be removed from input
-ZEROWIDTHNONJOINER = '\u200c' # character to be removed from input
-ZEROWIDTHJOINER = '\u200d' # character to be removed from input
+FORMFEED = '\f' # form feed, first character of first line of page headers
+NO_BREAK_SPACE = '\xa0' # characters of second line of page headers if -s = 'b' (blank)
+DOT_ABOVE = '˙' # characters of second line of page headers if -s = 'p' (point)
+MACRON = '¯'    # characters of second line of page headers if -s = 'd' (dash)
+OVERLINE = '‾'  # characters of second line of page headers if -s = 's' (solid)
+HEADER_CHARS = frozenset(FORMFEED + NO_BREAK_SPACE + DOT_ABOVE + MACRON + OVERLINE) # first chars of 1st and 2nd header lines
+SECOND_LINE_CHARS = {'b': NO_BREAK_SPACE, 'p': DOT_ABOVE, 'd': MACRON, 's': OVERLINE} # first chars in second header lines
+ZERO_WIDTH_CHARS = frozenset('\u200b\u200c\u200d') # to be discarded from input
+
+# status indicators
+WAITING = '?'
+RUNNING = '…'
+
+# scale factors when -I > 1
+SCALE_2 = 0.5 ** 0.5 # -I = 2
+SCALE_4 = 0.5        # -I = 4
+SCALE_8 = 0.5 ** 1.5 # -I = 8
+
+# PySimpleGUI
+THEME = 'Default1' # window colour theme
+TSIZE = 15 # text size
+FSIZE = 33 # field size
+
+# files
+MS_WINDOWS = platform.lower().startswith('win')
+YAWP_PATH = longpath('~/.config/yawp') # yawp's directory, create if does not exist
+md(YAWP_PATH) # create if not exists
+PDF_PATH = longpath('~/PDF') # directory for temporary PDF files
+md(PDF_PATH) # create if not exists
+CORR_FILE = longpath(f'{YAWP_PATH}/yawp.corr') # correction file
+HIST_FILE = longpath(f'{YAWP_PATH}/yawp.hist') # file of history of recent files (GUI mode only)
+SESS_FILE = longpath(f'{YAWP_PATH}/yawp.sess') # session file containing pathfile of last text file of previous session (GUI mode only)
+MANUAL_FILE = local_file(f'docs/YAWP {VERSION} User Manual.txt.pdf') # YAWP User Manual
+
+# radio buttons
+NON_RADIO_CHARS = 'ywgulcifFmeEoOnaYPWASZLRTBJt' # chars of non-radio arguments
+RADIO_CHARS = 'psXCI' # chars of radio arguments
+RADIO_DICT = {'p': list('nfpcd'), # domains of radio arguments, as a dict…
+              's': list('nbpds'),
+              'X': list('neb'),
+              'C': list('ndf'),
+              'I': list('1248')}
+RADIO_LIST = [RADIO_DICT[c] for c in RADIO_CHARS] # …and as a list
+SECOND_LINE = ''.join(RADIO_DICT['s']) # display domain of -s argument
+MULTI_PAGES = '/'.join(RADIO_DICT['I']) # display domain of -I argument
+
+# various
+ERROR = 1 # error return code
+USAGE_MODES = list('gefnu') # domain of arg.usage_mode
 QUOTES = "'" + '"' # single and double quotation marks
-INDENT = 4 * ' ' # standard indentation
-MIN_MARGIN = '2cm' # margin < MIN_MARGIN is deprecated
-MAX_QUALITY = 5 # max lp/lpr print quality
-ROUND = 6 # rounding factor in display of floats
-MAX_HIST = 20 # max number of items in history of recent files
-
-YAWP_ROOT = long_path('~/.yawp') # yawp's hidden directory
-md(YAWP_ROOT, exist_ok=True) # create if not exists
-YAWP_CORR = long_path('~/.yawp/.yawp.corr') # correction file
-YAWP_HIST = long_path('~/.yawp/.yawp.hist') # file of history of recent files (GUI mode only)
-YAWP_SESS = long_path('~/.yawp/.yawp.sess') # session file containing last text file of previous session (GUI mode only)
-YAWP_LOG = new_file('~/.yawp/.yawp.%Y.%m.%d-%H.%M.%S.log') # timestamped log file
-YAWP_PDF = local_file('docs/.yawp.pdf') # manual file
-
-SGTS = 16 # PySimpleGUI text size
-SGAS = 32 # PySimpleGUI argument size
-SGFS = 84 # PySimpleGUI file size
-SGBS = 12 # PySimpleGUI button size
-
-BUTTON_TOOLTIP = { # tooltips for buttons in GUI main window
-    'New':      'create a new empty text file',
-    'Open':     'browse the file system\nto select the text file',
-    'Recent':   'browse the list of recent files\nto select the text file',
-    'Saveas':   'clone current text file into a target text file',
-    'Help':     'browse the yawp-generated YAWP Manual\nthrough the PDF browser defined by -Y',
-    'Exit':     "save arguments and finish",
-    'Edit':     'edit the text file\nthrough the text editor defined by -y',
-    'Format':   'process the text file in Format mode',
-    'Noformat': 'process the text file in Noformat mode',
-    'Undo':     'restore the text file to its previous content',
-    'Log':      'browse the log file\nthrough the text editor defined by -y',
-    'Correct':  'manage the correction file\n(edit reset or restore)'}
-
-PAPERSIZE = { # format names for -S --paper-size
-    'HALF-LETTER':  '5.5x8.5in',
-    'LETTER':       '8.5x11.0in',
-    'LEGAL':        '8.5x14.0in',
-    'JUNIOR-LEGAL': '5.0x8.0in',
-    'LEDGER':       '11.0x17.0in',
-    'TABLOID':      '11.0x17.0in',
-    'A0':  '841x1189mm',
-    'A1':  '594x841mm',
-    'A2':  '420x594mm',
-    'A3':  '297x420mm',
-    'A4':  '210x297mm',
-    'A5':  '148x210mm',
-    'A6':  '105x148mm',
-    'A7':  '74x105mm',
-    'A8':  '52x74mm',
-    'A9':  '37x52mm',
-    'A10': '26x37mm',
-    'B0':  '1000x1414mm',
-    'B1':  '707x1000mm',
-    'B1+': '720x1020mm',
-    'B2':  '500x707mm',
-    'B2+': '520x720mm',
-    'B3':  '353x500mm',
-    'B4':  '250x353mm',
-    'B5':  '176x250mm',
-    'B6':  '125x176mm',
-    'B7':  '88x125mm',
-    'B8':  '62x88mm',
-    'B9':  '44x62mm',
-    'B10': '31x44mm'}
-
-CORRECTORS = '''
-# ┌────────────────────┐
-# │ ~/.yawp/.yawp.corr │
-# └────────────────────┘
+MAX_QUALITY = 5 # max lp print quality
+LP_SLEEP = 0.5 # sleep seconds in wait_lp_completion()
+ROUND = 6 # rounding factor in float display
+MAX_HISTORY = 25 # max number of items in history of recent files
+UNITS = ", unit: pt/in/mm/cm" # units in argument helps
+THIS_SESSION = now() # session timestamp, used as a session signature by lock
+
+# default correction file
+CORR_DEFAULT = '''
+# ┌──────────────────────────┐
+# │ ~/.config/yawp/yawp.corr │
+# └──────────────────────────┘
 
 plm 0mm 6mm # portrait left margin
 plm 10mm 16mm
 plm 20mm 24mm
 plm 30mm 35mm
 plm 40mm 43mm
 plm 50mm 52mm
@@ -184,15 +181,15 @@
 ptm 60mm 59mm
 ptm 70mm 68mm
 ptm 80mm 77.5mm
 ptm 90mm 87mm
 ptm 100mm 96mm
 
 ltm 0mm 2mm # landscape top margin
-ltm 5mm 7mm 
+ltm 5mm 7mm
 ltm 10mm 11mm
 ltm 20mm 20.5mm
 ltm 30mm 30mm
 ltm 40mm 39mm
 ltm 50mm 48.5mm
 ltm 60mm 57.5mm
 ltm 70mm 67mm
@@ -230,102 +227,220 @@
 lcw 100mm 92.200mm # landscape character width
 
 pch 100mm 94.358mm # portrait character height
 
 lch 100mm 92.647mm # landscape character height
 '''
 
-#----- yawp-specific functions -----
+tooltips = { # tooltips in GUI main window, others will be added later by get_arguments()
+    'New':      'Create a new empty text file',
+    'Open':     'Browse the file system\nto select the text file',
+    'Recent':   'Browse the list of recent files\nto select the text file',
+    'SaveAs':   'Clone current text file into a target text file',
+    'Help':     'Browse the yawp-generated YAWP Manual\nby the PDF browser defined by -Y',
+    'Exit':     'Save arguments and finish',
+    'Edit':     'Edit the text file\nby the text editor defined by -y',
+    'Format':   'Process the text file in Format mode',
+    'NoFormat': 'Process the text file in NoFormat mode',
+    'Undo':     'Restore the text file to its previous content',
+    'Log':      'Browse the log file\nby the text editor defined by -y'}
 
-def inform(message):
-    'information message'
-    log.print(message)
-    if arg.verbose:
-        print(message, file=stderr)
+PAPERSIZE = { # paper format names for -S --sheet-size
+    'A0':  '841x1189mm',
+    'A1':  '594x841mm',
+    'A2':  '420x594mm',
+    'A3':  '297x420mm',
+    'A4':  '210x297mm',
+    'A5':  '148x210mm',
+    'A6':  '105x148mm',
+    'A7':  '74x105mm',
+    'A8':  '52x74mm',
+    'A9':  '37x52mm',
+    'A10': '26x37mm',
+    'B0':  '1000x1414mm',
+    'B1':  '707x1000mm',
+    'B1+': '720x1020mm',
+    'B2':  '500x707mm',
+    'B2+': '520x720mm',
+    'B3':  '353x500mm',
+    'B4':  '250x353mm',
+    'B5':  '176x250mm',
+    'B6':  '125x176mm',
+    'B7':  '88x125mm',
+    'B8':  '62x88mm',
+    'B9':  '44x62mm',
+    'B10': '31x44mm',
+    'C0':  '917x1297mm',
+    'C1':  '648x917mm',
+    'C2':  '458x648mm',
+    'C3':  '324x458mm',
+    'C4':  '229x324mm',
+    'C5':  '162x229mm',
+    'C6':  '114x162mm',
+    'C7':  '81x114mm',
+    'C8':  '57x81mm',
+    'C9':  '40x57mm',
+    'C10': '28x40mm',
+    'C11': '22x32mm',
+    'C12': '16x22mm',
+    'HALF-LETTER':  '5.5x8.5in',
+    'LETTER':       '8.5x11.0in',
+    'LEGAL':        '8.5x14.0in',
+    'JUNIOR-LEGAL': '5.0x8.0in',
+    'LEDGER':       '11.0x17.0in',
+    'TABLOID':      '11.0x17.0in'}
 
-def strfile_inform(strfile, title):
-    'information message about a file read as a string'
-    inform(title)
-    inform(f'    {strfile.count(LINEFEED)+1} lines')
-    inform(f'    {len(strfile)} chars')    
-
-def warning(message):
-    'warning message'
-    inform('WARNING: ' + message)
-
-def error(message, jline=None, line=None):
-    'error message'
-    message = message[0].upper() + message[1:]
-    message = f'ERROR: {message}' if jline is None else f'ERROR: {message}:\nLINE {jline+1}: {line}'
-    log.print(message)
-    if var.gui:
-        print(message, file=stderr)
-        raise YawpError(message)
+#----- YAWP-specific functions -----
+
+def inform(lines):
+    'information lines'
+    log_lines(lines)
+    if not var.gui_mode and arg.verbose:
+        for line in lines:
+            print(line)
+
+def error(message, jline=None, line=None, ask=False):
+    message = f'ERROR: {message}'
+    if jline:
+        message += f'\n[{jline+1}] {line!r}'
+    log_lines([message])
+    if var.gui_mode and ask:
+        if not ask_yes('YAWP - ERROR', f'{message}\nDo you want to continue anyway?', 'continue'):
+            raise YawpError
+    elif var.gui_mode:
+        ask_ok('YAWP - ERROR', message)
+        raise YawpError
     else:
-        log.close()
-        exit(message)
+        print(message, file=stderr)
+        exit_button(ERROR)
 
-def yield_lines(file):
-    'yield lines read from a file'
-    file = file.strip()
+def open_file(file, mode='r'):
+    'like open(), but check file for undefined error and directory not found error'
+    process = {'r':'read', 'w':'writ', 'a':'append'}[mode[0]]
+    file = strip(file)
     if not file:
-        error(f'text file is undefined')
-    file = long_path(file)
-    path = dirname(file)
-    if not isdir(path):
-        error(f'directory {path!r} not found')
-    if not exists(file):
-        error(f'file {file!r} not found')
-    if not isfile(file):
-        error(f'file {file!r} exists but is not a file')
+        error(f"Undefined file error {process}ing file {file!r}")
+    file = longpath(file)
+    if not isdir(dirname(file)):
+        error(f"Directory not found error {process}ing file {file!r}")
+    return open(file, mode)
+
+def except_file(file, mode='r'):
+    'redirect I/O exception to error()'
+    process = {'r':'read', 'w':'writ', 'a':'append'}[mode[0]]
+    for line in format_exc().split('\n'):
+        if 'Error:' in line:
+            message = '' # 'FileNotFoundError: ... ' -> 'File not found error'
+            for jchar, char in enumerate(line.split(':')[0]):
+                if jchar > 0 and char.isupper():
+                    message += ' ' + char.lower()
+                else:
+                    message += char
+            error(f'{message} {process}ing file {file!r}')
+    else:
+        error(f'Undefined error {process}ing file {file!r}')
+
+def read_lines(text_file):
+    'yield lines in text_file'
+    try:
+        for line in open_file(text_file):
+            yield rstrip(''.join(
+                INDENT if char == HORIZTAB else '' if char in ZERO_WIDTH_CHARS else char for char in line))
+    except:
+        except_file(text_file)
+
+def max_line_length_in(text_file):
+    max_length = 0
     try:
-        for line in open(file):
-            yield ''.join(INDENT if char == HORIZTAB else '' if ZEROWIDTHSPACE <= char <= ZEROWIDTHJOINER else char for char in line).rstrip()
-    except UnicodeDecodeError:
-        error(f'file {file!r} is not correctly UTF8-encoded')
-    except Exception as exception:
-        error(f'{exception} reading file {file!r}')
+        for line in open_file(text_file):
+            max_length = max(max_length, len(rstrip(''.join(
+                INDENT if char == HORIZTAB else '' if char in ZERO_WIDTH_CHARS else char for char in line))))
+    except:
+        except_file(text_file)
+    else:
+        return max_length
 
-def get_lock_file(text_file):
-    'create a (not timestamped) filename for lock file of text_file'
+def write_lines(text_file, lines=[]):
+    'write lines into text_file'
+    try:
+        with open_file(text_file, 'w') as output:
+            for line in lines:
+                print(rstrip(line), file=output)
+    except:
+        except_file(text_file, 'w')
+
+def append_lines(text_file, lines):
+    'append lines to text_file'
+    try:
+        with open_file(text_file, 'a') as output:
+            for line in lines:
+                print(rstrip(line), file=output)
+    except:
+        except_file(text_file, 'a')
+
+def log_lines(lines):
+    if isfile(arg.text_file):
+        append_lines(log_file_of(arg.text_file), lines)
+
+def lock_file_of(text_file):
+    'create a filename for lock file of text_file'
     if not text_file:
         return ''
-    path, name = splitpath(long_path(text_file))
+    path, name = splitpath(longpath(text_file))
     return normpath(f'{path}/.yawp.{name}.lock')
 
-def get_args_file(text_file):
-    'create a (not timestamped) filename for args file of text_file'
+def log_file_of(text_file):
+    'create a filename for log file of text_file'
+    if not text_file:
+        return ''
+    path, name = splitpath(longpath(text_file))
+    return normpath(f'{path}/.yawp.{name}.log')
+
+def args_file_of(text_file):
+    'create a filename for args file of text_file'
     if not text_file:
         return ''
-    path, name = splitpath(long_path(text_file))
+    path, name = splitpath(longpath(text_file))
     return normpath(f'{path}/.yawp.{name}.args')
 
-def get_temp_file(text_file):
-    'create a (not timestamped) filename for temp file of text_file'
+def temp_file_of(text_file):
+    'create a filename for temp file of text_file'
     if not text_file:
         return ''
-    path, name = splitpath(long_path(text_file))
+    path, name = splitpath(longpath(text_file))
     return normpath(f'{path}/.yawp.{name}.temp')
 
-def new_back_file(text_file):
-    'create a timestamped filename for backup file of file'
+def new_back_file_of(text_file):
+    'create a timestamped filename for backup file of text_file'
     if not text_file:
         return ''
-    path, name = splitpath(long_path(text_file))
+    path, name = splitpath(longpath(text_file))
     return new_file(f'{path}/.yawp.{name}.%Y.%m.%d-%H.%M.%S.back')
 
-def old_back_file(text_file):
+def last_back_file_of(text_file):
     "return filename of the newest timestamped backup of file, or raise FileNotFoundError if not found"
     if not text_file:
         return ''
-    path, name_ext = splitpath(long_path(text_file))
+    path, name_ext = splitpath(longpath(text_file))
     return max_file(f'{path}/.yawp.{name_ext}.[2-9][0-9][0-9][0-9].[01][0-9].[0-3][0-9]-[0-2][0-9].[0-5][0-9].[0-5][0-9].back')
 
+def back_files_of(text_file):
+    "return list of filenames of all timestamped backups of text_file"
+    if not text_file:
+        return []
+    path, name_ext = splitpath(longpath(text_file))
+    return get_file(f'{path}/.yawp.{name_ext}.[2-9][0-9][0-9][0-9].[01][0-9].[0-3][0-9]-[0-2][0-9].[0-5][0-9].[0-5][0-9].back')
+
+def is_reserved(file):
+    'is file a YAWP-reserved file?'
+    path, name = splitpath(shortpath(file))
+    return path.startswith('~/.config/yawp') or name.startswith('.yawp.')
+
 def chapter_level(prefix):
-    "level of a chapter prefix: '0.' -> 1, '0.0.' -> 2, ..., else -> 0"
+    "level of a chapter prefix: '0.' -> 1, '0.0.' -> 2, …, else -> 0"
     status = 0; level = 0
     for char in prefix:
         if status == 0:
             if char.isdecimal():
                 status = 1
             else:
                 return 0
@@ -336,555 +451,531 @@
                 level += 1
                 status = 0
             else:
                 return 0
     return level if status == 0 else 0
 
 def figure_level(prefix):
-    "level of a figure caption: 'x.' -> 1, '0.x.' -> 2, '0.0.x.' -> 3, ..., else -> 0"
+    "level of a figure caption: 'x.' -> 1, '0.x.' -> 2, '0.0.x.' -> 3, …, else -> 0"
     if fnmatchcase(prefix, '[a-z].'):
         return 1
     elif not fnmatchcase(prefix, '*[a-z].'):
         return 0
     else:
         chaplevel = chapter_level(prefix[:-2])
         return 0 if chaplevel == 0 else chaplevel + 1
 
 def page_number(number, page_offset):
     'display page number, possibly by a Roman number'
     return int2roman(number) if number <= -page_offset else str(number + page_offset)
 
 def max_len_page_number(max_number, page_offset):
-    'max length of display page numbers from 1 until max_number'
-    arab = len(str(max_number + page_offset))
-    roma = 0 if page_offset >= 0 else max((len(int2roman(n)) for n in range(min(max_number, -page_offset) + 1)))
-    return max(arab, roma)
+    'max length of display page numbers from 1 until max_number, including Roman numbers'
+    arab_len = len(str(max_number + page_offset))
+    roma_len = 0 if page_offset >= 0 else max((len(int2roman(n)) for n in range(min(max_number, -page_offset) + 1)))
+    return max(arab_len, roma_len)
 
 def ask_yes(title, question, tooltip_yes, tooltip_no=''):
-    "show a question (Yes/No) window and return True if 'Yes', False if 'No' or alt-F4 or 'x' button"
+    "show a Yes/No window and return True if 'Yes', False if 'No' or alt-F4 or 'x' button"
     lines = question.split('\n')
-    text_width = max(len(line) for line in lines)
+    text_width = max(FSIZE, max(len(line) for line in lines))
     text_height = len(lines)
     layout = [[sg.Text(question, size=(text_width, text_height))],
-              [sg.Button('Yes', tooltip=tooltip_yes, size=SGBS),
-               sg.Button('No', tooltip=tooltip_no or f"do not {tooltip_yes}", size=SGBS)]]
+              [sg.Button('Yes', tooltip=tooltip_yes.title(), size=BSIZE),
+               sg.Button('No', tooltip=tooltip_no or f"Do not {tooltip_yes.lower()}", size=BSIZE)]]
     return sg.Window(title, layout).read(close=True)[0] == 'Yes'
 
-def ask_ok(button, message):
-    "show an error message window, exit by 'OK' or alt-F4 or 'x' button"
-    title = f'YAWP - {button} - ERROR'
-    lines = message.split('ERROR: ')[-1].split('\n')
-    message = '\n'.join(lines)
-    text_width = max(SGAS, max(len(line) for line in lines))
+def ask_ok(title, message):
+    "show a window, exit by 'OK' or alt-F4 or 'x' button"
+    lines = message.split('\n')
+    text_width = max(FSIZE, max(len(line) for line in lines))
     text_height = len(lines)
     layout = [[sg.Text(message, size=(text_width, text_height))],
-              [sg.Button('OK', tooltip='go back', size=SGBS)]]
+              [sg.Button('OK', tooltip='go on', size=BSIZE)]]
     sg.Window(title, layout).read(close=True)
 
+def read_sess_file():
+    'read path and name of text file from session file, if possible'
+    try:
+        return rstrip(open(SESS_FILE).read())
+    except:
+        return ''
+
+def write_sess_file(text_file):
+    if arg.usage_mode == 'g':
+        write_lines(SESS_FILE, [text_file])
+
+def wait_lp_completion():
+    previous = None
+    while True:
+        current = shell(f'ls -al {PDF_PATH!r} 2>/dev/null')
+        if previous == current:
+            return
+        previous = current
+        sleep(LP_SLEEP)
+
 #----- class YawpError -----
 
 class YawpError(Exception): pass # error control in GUI mode
 
 #----- class Variables -----
 
-class Variables: pass # global not-arguments scalar variables
+class Variables: pass # global not-argument scalar variables
 
 var = Variables()
 
 #----- class Arguments -----
 
 class Arguments:
 
     def __init__(arg):
-        arg.name_default = {} # {name: default} filled by get__arguments()
-        arg.letter_tooltip = {} # {letter: tooltip} button tooltips (argument tooltips added later by get_arguments())
-        arg.LETTERS = 'vygwlcifFeEoOnaXYPWASZLRTBKt' # letters in main window, all but radio -p and -C
-        arg.BLACKLIST = {'help','view_manual','version','usage_mode','text_file'} # do not read/write from/into args file
-        arg.shorts_longs = [] # [(short, long), ...]
-
-    def dump(arg):
-        show('arg.__dict__, arg.name_default, arg.letter_tooltip, arg.LETTERS, arg.BLACKLIST')
- 
+        arg.name_default = {} # {name: default} filled by get_arguments()
+        arg.blacklist = {'help','view_manual','version','usage_mode','verbose','text_file'} # do not read/write from/into args file
+        arg.shorts_longs = [] # [(short, long), …]
+
     def read_from_argv(arg, argv):
         parser = ArgumentParser(prog='yawp', formatter_class=RawDescriptionHelpFormatter, description=DESCRIPTION)
-        UNITS = ", unit: 'pt' 'in' 'mm' or 'cm'"
         #
         def varg(short, long, version):
             'version argument'
-            # no need for arg.name_default arg.letter_tooltip arg.letters arg shorts_longs
-            parser.add_argument(short, long, action='version', version=VERSION)
+            # no need for arg.name_default tooltip NON_RADIO_CHARS arg shorts_longs
+            parser.add_argument(short, long, action='version', version=f'YAWP {VERSION}')
         #
         def barg(short, long, help):
             'boolean argument'
             name = long[2:].replace('-','_')
             arg.name_default[name] = False
             letter = short[1]
-            tooltip = help.replace(' (','\n(').replace(', ',',\n')
-            arg.letter_tooltip[letter] = tooltip
+            tooltips[letter] = help.replace(' (','\n(').replace(', ',',\n')
             help=help.replace('%','%%')
             parser.add_argument(short, long, action='store_true', help=help)
             arg.shorts_longs.append((short, long))
         #
         def sarg(short, long, default, help, note=''):
             'string argument'
             name = long[2:].replace('-','_')
             arg.name_default[name] = default
             letter = short[1]
             help = f"{help} (default: {default!r}{note})"
-            tooltip = help.replace(' (','\n(').replace(', ',',\n')
-            arg.letter_tooltip[letter] = tooltip
+            tooltips[letter] = help.replace(' (','\n(').replace(', ',',\n')
             help=help.replace('%','%%')
             parser.add_argument(short, long, default=default, help=help)
             arg.shorts_longs.append((short, long))
         #
         def parg(name, nargs, help):
             'positional argument'
             arg.name_default[name] = ''
             letter = name[0]
-            tooltip = help.replace(' (','\n(').replace(', ',',\n')
-            arg.letter_tooltip[letter] = tooltip
+            tooltips[letter] = help.replace(' (','\n(').replace(', ',',\n')
             help=help.replace('%','%%')
             parser.add_argument(name, nargs=nargs, help=help)
             arg.shorts_longs.append(('', name))
         #
         # usage arguments
-        barg('-H', '--view-manual',     'browse the yawp-generated PDF Yawp Manual and exit')
         varg('-V', '--version',         'yawp' + VERSION)
-        barg('-v', '--verbose',         'write all messages on stderr (default: write errors only)')
-        sarg('-M', '--usage-mode',      'g', "run yawp in this usage mode", " = GUI, 'e' = Edit, 'f' = Format, 'n' = Noformat, 'U' = undo")
+        barg('-H', '--browse-manual',   'browse the PDF YAWP User Manual and exit')
+        barg('-v', '--verbose',         'write all messages on stderr (CLI modes only, default: write errors only)')
+        sarg('-M', '--usage-mode',      'g', "run yawp in this usage mode", " = GUI, 'e' = CLI Edit, 'f' = CLI Format, 'n' = CLI NoFormat, 'u' = CLI Undo")
         # format arguments
         sarg('-y', '--text-editor',     'idle', "editor for text files")
-        barg('-g', '--graphics',        "redraw '`'-segments and '^'-arrowheads")
         sarg('-w', '--chars-per-line',  '0', 'line width in characters per line', ' = automatic')
+        barg('-g', '--graphics',        "redraw '`'-segments and '^'-arrowheads")
+        sarg('-u', '--lines-per-page',  '0', 'page height in lines per page', ' = automatic')
         barg('-l', '--just-left-only',  'justify text lines at left only (default: at left and right)')
-        sarg('-c', '--contents-title',  'contents', "title of contents chapter")
-        sarg('-i', '--index-title',     'index', "title of index chapter")
-        sarg('-f', '--figures-title',   'figures', "title of figures chapter")
-        sarg('-F', '--caption-prefix',  'figure', "first word of figure captions")
-        # paging arguments:
-        sarg('-p', '--page-headers',    'n', "insert page headers", " = no, 'f' = on full page, 'p' = and on broken pictures, 'c' = and on level-1 chapters")
-        sarg('-e', '--even-left',       '%n/%N', "headers of even pages, left")
-        sarg('-E', '--even-right',      '%F %Y-%m-%d', "headers of even pages, right")
-        sarg('-o', '--odd-left', '%c',  "headers of odd pages, left")
-        sarg('-O', '--odd-right',       '%n/%N', "headers of odd pages, right")
-        sarg('-n', '--page-offset',     '0', 'offset of page numbers', ", min: '-3999', if negative it is count of initial Roman numbers")
+        # chapter arguments
+        sarg('-c', '--contents-title',  'Contents', "title of Contents chapter")
+        sarg('-i', '--index-title',     'Index', "title of Index chapter")
+        sarg('-f', '--figures-title',   'Figures', "title of Figures chapter")
+        sarg('-F', '--caption-prefix',  'Figure', "first word of figure captions")
+        sarg('-m', '--chapter-offset',  '0', 'offset of level-1 numbered chapters', ', min: -1')
+        # paging arguments
+        sarg('-p', '--page-headers',    'n', "insert page headers",
+             " = no, 'f' = on full page, 'p' = and on broken pictures, 'c' = and on level-1 chapters, 'd' = double if level-1 on even page")
+        sarg('-e', '--even-left',       '%n', "first line of headers of even pages, left")
+        sarg('-E', '--even-right',      '%f', "first line of headers of even pages, right")
+        sarg('-o', '--odd-left',        '%c', "first line of headers of odd pages, left")
+        sarg('-O', '--odd-right',       '%n', "first line of headers of odd pages, right")
+        sarg('-n', '--page-offset',     '0', 'offset of page numbers', ", min: -3999, if < 0: Roman numbers")
         barg('-a', '--all-pages-E-e',   "put in all page headers -E at left and -e at right")
+        sarg('-s', '--second_line',     's', 'second line of page headers', " = solid, 'n' = no, 'b' = blanks, 'p' = points, 'd' = dashes")
         # export arguments
-        barg('-X', '--export-view-pdf', "after processing export and browse PDF file")
-        sarg('-Y', '--pdf-browser',     'xdg-open', "browser for PDF files")
-        sarg('-P', '--pdf-file',        '%f.pdf', "exported PDF file")
+        sarg('-X', '--export-pdf',      'n', 'export and browse PDF file', " = no, 'e' = export, 'b' = export and browse")
+        sarg('-C', '--correct',         'd', "correct character size and page margins", " = by default values, 'n' = no, 'f' = by correction file")
+        sarg('-Y', '--pdf-browser',     'atril', "browser for PDF files")
+        sarg('-P', '--pdf-file',        '%f%e.pdf', "exported PDF file")
         sarg('-W', '--char-width',      '0', "character width", " = automatic" + UNITS)
-        sarg('-A', '--char-aspect',     '3/5', "character aspect ratio = char width / char height", ", '1' = square grid")
-        sarg('-S', '--paper-size',      'A4', "portrait paper size width x height", " = '210x297mm'" + UNITS)
+        sarg('-A', '--char-aspect',     '3/5', "character aspect ratio = width / height", ", 1 = square grid")
+        sarg('-S', '--sheet-size',      'A4', "portrait paper size width x height", " = '210x297mm'" + UNITS)
         barg('-Z', '--landscape',       "turn page by 90 degrees (default: portrait)")
         sarg('-L', '--left-margin',     '2cm', "left margin", UNITS)
         sarg('-R', '--right-margin',    '2cm', "right margin", UNITS)
         sarg('-T', '--top-margin',      '2cm', "top margin", UNITS)
         sarg('-B', '--bottom-margin',   '2cm', "bottom margin", UNITS)
-        sarg('-C', '--correct-sizes',   'd', "correct character size and page margins", " = by default values, 'n' = no, 'f' = by correction file")
-        barg('-K', '--fake-margins',    'get left margin by blanks and top margin by empty lines')
+        sarg('-I', '--multi-pages',     '1', 'pages on each side of paper sheets', ", values: 1/2/4/8")
+        sarg('-J', '--multi-sheets',    '0', 'paper sheets gathered together', " = export sequentially")
         # file argument
-        parg('text_file', '?', 'text file to be processed, ASCII or UTF8-encoded')
-        # arguments ──▷ arg.*
+        parg('text_file', '?', 'text file to process, ASCII or UTF-8-encoded Unicode')
+        # arguments → arg.*
         parser.parse_args(argv[1:], arg)
         # text_file
-        arg.text_file = long_path(arg.text_file or '') # None ──▷ ''
+        arg.text_file = longpath(arg.text_file) if arg.text_file else '' # None → ''
         # -h is managed by ArgumentParser
         # -V is managed by ArgumentParser
         # -H
-        if arg.view_manual:
+        if arg.browse_manual:
             arg.check_pdf_browser()
-            shell(f'{arg.pdf_browser} {YAWP_PDF}')
+            shell(f'{arg.pdf_browser} {MANUAL_FILE!r}')
             exit(0)
         # -M
-        if arg.usage_mode not in set('gefnu'):
-            error(f"wrong -M {arg.usage_mode!r}, it must be 'g' 'e' 'f' 'n' or 'u'")    
+        if arg.usage_mode not in USAGE_MODES:
+            error(f"Wrong -M {arg.usage_mode!r}, it must be in {USAGE_MODES}")
         # text_file
-        arg.text_file = (arg.text_file or '').strip()
-        if arg.usage_mode == 'g': # text_file optional, other arguments forbidden
+        arg.text_file = strip(arg.text_file or '')
+        if arg.text_file:
+            arg.text_file = longpath(arg.text_file)
+        if arg.usage_mode == 'g': # GUI mode, text_file optional, other arguments forbidden
+            arg.verbose = False
             if len(argv) != 1 + bool(arg.text_file):
-                error(f"in GUI mode no argument is allowed, except possibly text_file")
+                error(f"In GUI mode no argument is allowed, except possibly text_file")
             if not arg.text_file:
-                arg.read_text_file_from_sess_file(YAWP_SESS)
-        else:
-            if not arg.text_file: # text_file mandatory, other arguments optional
-                error(f'in CLI mode (-M {arg.usage_mode!r}) the text_file argument is mandatory')
-        if arg.text_file:        
-            dir_of_text_file = dirname(arg.text_file)
-            if not isdir(dir_of_text_file):
-                error(f'path {dir_of_text_file!r} of text_file {arg.text_file!r} not found')
-            if exists(arg.text_file) and not isfile(arg.text_file):
-                error(f'text_file {arg.text_file!r} exists but is not a file')
-            if not isfile(arg.text_file):
-                if arg.usage_mode == 'e':
-                    open(arg.text_file, 'w').write('')
-                elif arg.usage_mode == 'u': 
-                    pass
-                else:
-                    error(f'text_file {arg.text_file!r} not found')
-        arg.open_text_file(arg.text_file)
+                arg.text_file = read_sess_file()
+            arg.read_from_args_file_of(arg.text_file)
+        else: # CLI modes, text_file mandatory, other arguments optional
+            if not arg.text_file:
+                error(f'In CLI mode (-M {arg.usage_mode!r}) the text_file argument is mandatory')
+        if isfile(arg.text_file):
+            hist.add(arg.text_file)
+            cd(dirname(arg.text_file))
 
     def inform(arg):
-        inform('Arguments:')
-        inform('    -h --help = False')
-        inform('    -V --version = False')
+        lines = ['Non-default arguments:']
         for short, long in arg.shorts_longs:
-            name = long.replace('--','').replace('-','_')
-            value = eval(name, arg.__dict__, arg.__dict__)
-            inform(f'    {short} {long} = {value!r}')
-            
-    def read_from_args_file_of(arg, text_file):
-        arg.set_default()
-        if text_file:
-            args_file = get_args_file(text_file)
-            if isfile(args_file):
-                lines = list(yield_lines(args_file))
-                try:
-                    for jline, line in enumerate(lines):
-                        line = line.split('#')[0].strip()
-                        if line:
-                            name, value = line.split('=')
-                            name = name.strip()
-                            if name in arg.name_default and name not in arg.BLACKLIST:
-                                setattr(arg, name, eval(value.strip(), {}, {}))
-                except:
-                    error(f'in argument file, syntax error', jline, line)
+            name = replace(long, '--', '', '-', '_')
+            if name not in arg.blacklist or name == 'verbose':
+                value = eval(name, arg.__dict__, arg.__dict__)
+                default = arg.name_default[name]
+                if value != default:
+                    lines.append(f'    {name} = {value!r}')
+        inform(lines)
 
-    def write_into_args_file_of(arg, text_file):
-        if text_file:
-            args_file = get_args_file(text_file)
-            with open(args_file, 'w') as output:
-                for name in sorted(arg.name_default.keys()):
-                    if name not in arg.BLACKLIST:
-                        print(f'{name} = {getattr(arg, name)!r}', file=output)
-
-    def read_text_file_from_sess_file(arg, sess_file):
-        arg.text_file = ''
-        if isfile(sess_file):
-            text_file = long_path(open(sess_file).read())
+    def read_from_args_file_of(arg, text_file):
+        '''if args_file_of(text_file) not found, all args get their default values
+on error reading an arg, arg maintains its default value'''
+        if arg.usage_mode == 'g':
+            arg.set_default()
             if isfile(text_file):
-                arg.text_file = text_file
+                args_file = args_file_of(text_file)
+                if isfile(args_file):
+                    for line in read_lines(args_file):
+                        stmt = line2stmt(line)
+                        if stmt:
+                            try:
+                                name, value = stmt.split('=')
+                                name, value = strip(name), strip(value)
+                                if name in arg.name_default and name not in arg.blacklist:
+                                    setattr(arg, name, eval(value, {}, {}))
+                            except:
+                                pass
 
-    def write_text_file_into_sess_file(arg, sess_file):
-        open(sess_file, 'w').write(arg.text_file)
+    def write_into_args_file_of(arg, text_file):
+        if arg.usage_mode == 'g' and isfile(text_file):
+            lines = []
+            for short, long in arg.shorts_longs:
+                name = long.replace('--','').replace('-','_')
+                if name not in arg.blacklist:
+                    value = eval(name, arg.__dict__, arg.__dict__)
+                    if value != arg.name_default[name]:
+                        lines.append(f'{name} = {value!r}')
+            write_lines(args_file_of(text_file), lines)
 
     def read_from_window(arg, window):
-        (arg.verbose, arg.text_editor, arg.graphics, arg.chars_per_line, arg.just_left_only,
-         arg.contents_title, arg.index_title, arg.figures_title, arg.caption_prefix,
+        (arg.text_editor, arg.chars_per_line, arg.graphics, arg.lines_per_page, arg.just_left_only,
+         arg.contents_title, arg.index_title, arg.figures_title, arg.caption_prefix, arg.chapter_offset,
          arg.even_left, arg.even_right, arg.odd_left, arg.odd_right, arg.page_offset, arg.all_pages_E_e,
-         arg.export_view_pdf, arg.pdf_browser, arg.pdf_file, arg.char_width, arg.char_aspect, arg.paper_size, arg.landscape,
-         arg.left_margin, arg.right_margin, arg.top_margin, arg.bottom_margin, arg.fake_margins, arg.text_file) = [
-             window[char].get() for char in arg.LETTERS]
-        arg.page_headers = get_radio(window, 0, 'nfpc')
-        arg.correct_sizes = get_radio(window, 4, 'ndf')
+         arg.pdf_browser, arg.pdf_file, arg.char_width, arg.char_aspect, arg.sheet_size, arg.landscape,
+         arg.left_margin, arg.right_margin, arg.top_margin, arg.bottom_margin, arg.multi_sheets,
+         arg.text_file) = [window[char].get() for char in NON_RADIO_CHARS]
+        arg.page_headers, arg.second_line, arg.export_pdf, arg.correct, arg.multi_pages = get_radios(window, RADIO_LIST)
 
     def write_into_window(arg, window):
-        for letter, value in zip(arg.LETTERS,
-            (arg.verbose, arg.text_editor, arg.graphics, arg.chars_per_line, arg.just_left_only,
-             arg.contents_title, arg.index_title, arg.figures_title, arg.caption_prefix,
+        for letter, value in zip(NON_RADIO_CHARS,
+            (arg.text_editor, arg.chars_per_line, arg.graphics, arg.lines_per_page, arg.just_left_only,
+             arg.contents_title, arg.index_title, arg.figures_title, arg.caption_prefix, arg.chapter_offset,
              arg.even_left, arg.even_right, arg.odd_left, arg.odd_right, arg.page_offset, arg.all_pages_E_e,
-             arg.export_view_pdf, arg.pdf_browser, arg.pdf_file, arg.char_width, arg.char_aspect, arg.paper_size, arg.landscape,
-             arg.left_margin, arg.right_margin, arg.top_margin, arg.bottom_margin, arg.fake_margins, arg.text_file)
-            ): window[letter].update(value)
-        put_radio(window, 0, 'nfpc', arg.page_headers)
-        put_radio(window, 4, 'ndf', arg.correct_sizes)
+             arg.pdf_browser, arg.pdf_file, arg.char_width, arg.char_aspect, arg.sheet_size, arg.landscape,
+             arg.left_margin, arg.right_margin, arg.top_margin, arg.bottom_margin, arg.multi_sheets,
+             arg.text_file)):
+            window[letter].update(value)
+        put_radios(window, RADIO_LIST, (arg.page_headers, arg.second_line, arg.export_pdf, arg.correct, arg.multi_pages))
         window.refresh()
 
+    def shrink_all(arg):
+        for name, default in arg.name_default.items():
+            if name not in arg.blacklist:
+                value = getattr(arg, name)
+                if isinstance(value, str):
+                    setattr(arg, name, shrink(value))
+
     def set_default(arg):
         for name, default in arg.name_default.items():
-            if name not in arg.BLACKLIST:
+            if name not in arg.blacklist:
                 setattr(arg, name, default)
 
     def set_default_if_empty(arg):
         for name, default in arg.name_default.items():
-            if name not in arg.BLACKLIST:
+            if name not in arg.blacklist:
                 value = getattr(arg, name)
-                if isinstance(value, str) and not value.strip():
+                if isinstance(value, str) and not strip(value):
                     setattr(arg, name, default)
 
-    def print(arg):
-        for name, default in sorted(arg.name_default.items()):
-            print(f'{name} = {getattr(arg, name)!r} # default = {default!r}')
-
     def check(arg):
-        arg.inform()
+        arg.shrink_all()
         # -y
         arg.check_text_editor()
         # -w
         try:
-            var.chars_per_line = int(arg.chars_per_line)
-            assert var.chars_per_line >= 0
-        except (ValueError, AssertionError):
+            var.chars_per_line = str2int(arg.chars_per_line, min=0)
+        except ValueError:
             error(f'Wrong -w --chars-per-line {arg.chars_per_line!r}, it must be an integer ≥ 0')
+        # -u
+        try:
+            var.lines_per_page = str2int(arg.lines_per_page, min=0)
+        except ValueError:
+            error(f'Wrong -u --lines-per-page {arg.lines_per_page!r}, it must be an integer ≥ 0')
         # -c
-        var.contents_title = unqupper(shrink(arg. contents_title))
+        var.contents_title = shrink_alphaupper(arg.contents_title)
         if not var.contents_title:
-            error(f"wrong -c --contents-title '', it cannot be empty")
+            error(f"Wrong -c --contents-title '', it cannot be empty")
         # -i
-        var.index_title = unqupper(shrink(arg. index_title))
+        var.index_title = shrink_alphaupper(arg.index_title)
         if not var.index_title:
-            error(f"wrong -i --index-title '', it cannot be empty")
+            error(f"Wrong -i --index-title '', it cannot be empty")
         # -f
-        var.figures_title = unqupper(shrink(arg. figures_title))
+        var.figures_title = shrink_alphaupper(arg.figures_title)
         if not var.figures_title:
-            error(f"wrong -f --figures-title '', it cannot be empty")
+            error(f"Wrong -f --figures-title '', it cannot be empty")
         # -c -i -f
         if len(set([var.contents_title, var.index_title, var.figures_title])) < 3:
             error(f'Wrong -c -i -f, they must be all different')
         # -F
-        var.caption_prefix = unqupper(shrink(arg. caption_prefix))
+        var.caption_prefix = shrink_alphaupper(arg.caption_prefix)
         if not var.caption_prefix:
-            error(f"wrong -F --caption-prefix '', it cannot be empty")
+            error(f"Wrong -F --caption-prefix '', it cannot be empty")
         if ' ' in var.caption_prefix:
-            error(f"wrong -F --caption-prefix {arg.caption_prefix!r}, it cannot contain blanks")
+            error(f"Wrong -F --caption-prefix {arg.caption_prefix!r}, it cannot contain blanks")
+        # -m
+        try:
+            var.chapter_offset = str2int(arg.chapter_offset, min=-1)
+        except ValueError:
+            error(f'Wrong -m --chapter-offset {arg.chapter_offset!r}, it must be an integer ≥ -1')
         # -p
-        if arg.page_headers not in list('nfpc'):
-            error(f"wrong -p --page-headers {arg.page_headers!r}, it must be 'n' 'f' 'p' or 'c'")
+        if arg.page_headers not in RADIO_DICT['p']:
+            error(f"Wrong -p --page-headers {arg.page_headers!r}, it must be in {RADIO_DICT['p']}")
         # -e
         try:
-            evalchar(arg.even_left, 'PpfFeYmdHMSnNc', 'PpfFeYmdHMSnNc', '%')
+            evalchar(arg.even_left, 'PpfeYmdHMSnNc', 'PpfeYmdHMSnNc', '%')
         except ValueError as illegal:
             error(f'Wrong -e --even-left {arg.even_left!r}, illegal {str(illegal)!r}')
         # -E
         try:
-            evalchar(arg.even_right, 'PpfFeYmdHMSnNc', 'PpfFeYmdHMSnNc', '%')
+            evalchar(arg.even_right, 'PpfeYmdHMSnNc', 'PpfeYmdHMSnNc', '%')
         except ValueError as illegal:
             error(f'Wrong -E --even-right {arg.even_right!r}, illegal {str(illegal)!r}')
         # -o
         try:
-            evalchar(arg.odd_left, 'PpfFeYmdHMSnNc', 'PpfFeYmdHMSnNc', '%')
+            evalchar(arg.odd_left, 'PpfeYmdHMSnNc', 'PpfeYmdHMSnNc', '%')
         except ValueError as illegal:
             error(f'Wrong -o --odd-left {arg.odd_left!r}, illegal {str(illegal)!r}')
         # -O
         try:
-            evalchar(arg.odd_right, 'PpfFeYmdHMSnNc', 'PpfFeYmdHMSnNc', '%')
+            evalchar(arg.odd_right, 'PpfeYmdHMSnNc', 'PpfeYmdHMSnNc', '%')
         except ValueError as illegal:
             error(f'Wrong -O --odd-right {arg.odd_right!r}, illegal {str(illegal)!r}')
         # -n
         try:
-            var.page_offset = int(arg.page_offset)
-            assert var.page_offset >= -3999
-        except (ValueError, AssertionError):
+            var.page_offset = str2int(arg.page_offset, min=-3999)
+        except ValueError:
             error(f'Wrong -n --page-offset {arg.page_offset!r}, it must be an integer ≥ -3999')
+        # -s
+        if arg.second_line not in RADIO_DICT['s']:
+            error(f"Wrong -s --second-line {arg.second_line!r}, it must be in {SECOND_LINE!r}")
+        var.page_header_lines = 0 if arg.page_headers == 'n' else 1 if arg.second_line == 'n' else 2
+        # -X
+        if arg.export_pdf not in RADIO_DICT['X']:
+            error(f"Wrong -X --export-view-pdf {arg.export_pdf!r}, it must be in {RADIO_DICT['X']}")
+        # -C
+        if arg.correct not in RADIO_DICT['C']:
+            error(f"Wrong -C --correct {arg.correct!r}, it must be in {RADIO_DICT['C']}")
         # -Y
         arg.check_pdf_browser()
         # -P
         try:
-            evalchar(arg.pdf_file, 'PpfFeYmdHMS', 'PpfFeYmdHMS', '%')
+            evalchar(arg.pdf_file, 'PpfeYmdHMS', 'PpfeYmdHMS', '%')
         except ValueError as illegal:
             error(f'Wrong -P --file-pdf {arg.pdf_file!r}, illegal {str(illegal)!r}')
         if not arg.pdf_file.endswith('.pdf'):
-            error(f"wrong -P --file-pdf {arg.pdf_file!r}, not ending with '.pdf'")
+            error(f"Wrong -P --file-pdf {arg.pdf_file!r}, not ending with '.pdf'")
         # -W
         try:
             var.char_width = str2inch(arg.char_width)
-            assert var.char_width >= 0.0
-        except (ValueError, AssertionError):
-            error(f"wrong -W --char-width {arg.char_width!r}, it must be zero (as '0' or 0.0')\nor value + 'in'/'pt'/'cm'/'mm' (as '0.5pt'), value ≥ 0")
+        except ValueError:
+            error(f"Wrong -W --char-width {arg.char_width!r}, it must be zero or unsigned float + 'in'/'pt'/'cm'/'mm'")
         # -A
         try:
-            var.char_aspect = ratio(arg.char_aspect)
-        except ValueError:
-            error(f"wrong -A --char-aspect {arg.char_aspect!r}, it must be a value (as '0.6')\nor value1 + '/' + value2 (as '3/5'), values > 0")
+            var.char_aspect = str2ratio(arg.char_aspect)
+        except (ValueError, AssertionError):
+            error(f"Wrong -A --char-aspect {arg.char_aspect!r}, it must be unsigned float or unsigned float + '/' + unsigned float ")
         # -S
         try:
-            var.paper_width, var.paper_height = str2inxin(PAPERSIZE.get(arg.paper_size.upper(), arg.paper_size))
-            assert 0.0 < var.paper_width <= var.paper_height
-        except (ValueError, AssertionError):
-            error(f"wrong -S --paper-size {arg.paper_size!r}, it must be a paper format name (as 'A4')\nor width + 'x' + height + 'in'/'pt'/'cm'/'mm' (as '210x297mm'), 0 < width ≤ height")
+            var.sheet_width, var.sheet_height = str2inxin(PAPERSIZE.get(arg.sheet_size.upper(), arg.sheet_size))
+        except ValueError:
+            error(f"Wrong -S --sheet-size {arg.sheet_size!r}, it must be a format name or width x height in/pt/cm/mm")
         # -Z
         if arg.landscape:
-            var.paper_width, var.paper_height = var.paper_height, var.paper_width
+            var.sheet_width, var.sheet_height = var.sheet_height, var.sheet_width
         # -L
-        min_margin = str2inch(MIN_MARGIN)
         try:
             var.left_margin = str2inch(arg.left_margin)
         except ValueError:
-            error(f"wrong -L --left-margin {arg.left_margin!r}, it must be float + 'in'/'pt'/'cm'/'mm', value ≥ '0'")
-        if var.left_margin < min_margin:
-            warning(f"-L --left-margin {arg.left_margin!r} < {MIN_MARGIN}, it may give unexpected results")
+            error(f"Wrong -L --left-margin {arg.left_margin!r}, it must be zero or unsigned float in/pt/cm/mm")
         # -R
         try:
             var.right_margin = str2inch(arg.right_margin)
         except ValueError:
-            error(f"wrong -R --right-margin {arg.right_margin!r}, it must be float + 'in'/'pt'/'cm'/'mm', value ≥ '0'")
-        if var.left_margin < min_margin:
-            warning(f"-L --left-margin {arg.left_margin!r} < {MIN_MARGIN}, it may give unexpected results")
+            error(f"Wrong -R --right-margin {arg.right_margin!r}, it must be zero or unsigned float in/pt/cm/mm")
         # -T
         try:
             var.top_margin = str2inch(arg.top_margin)
         except ValueError:
-            error(f"wrong -T --top-margin {arg.top_margin!r}, it must be float + 'in'/'pt'/'cm'/'mm', value ≥ '0'")
-        if var.top_margin < min_margin:
-            warning(f"-L --top-margin {arg.top_margin!r} < {MIN_MARGIN}, it may give unexpected results")
+            error(f"Wrong -T --top-margin {arg.top_margin!r}, it must be zero or unsigned float in/pt/cm/mm")
         # -B
         try:
             var.bottom_margin = str2inch(arg.bottom_margin)
         except ValueError:
-            error(f"wrong -B --bottom-margin {arg.bottom_margin!r}, it must be float + 'in'/'pt'/'cm'/'mm', value ≥ '0'")
-        if var.left_margin < min_margin:
-            warning(f"-L --left-margin {arg.left_margin!r} < {MIN_MARGIN}, it may give unexpected results")
-        # -C
-        if arg.correct_sizes not in list('ndf'):
-            error(f"wrong -C --correct-sizes {arg.correct_sizes!r}, it must be 'n' 'd' or 'f'")
-
-    def check_text_file(arg, must_exist=True):
-        arg.text_file = (arg.text_file or '').strip()
-        if not arg.text_file:
-            error('text file is undefined')
-        arg.text_file = long_path(arg.text_file)
-        path = dirname(arg.text_file)
-        if not isdir(path):
-            error('directory {path!r} of text file {arg.text_file!r} not found')
-        if exists(arg.text_file) and not isfile(arg.text_file):
-            error('text file {arg.text_file!r} exists but is not a file')
-        if must_exist and not exists(arg.text_file):
-            error('text file {arg.text_file!r} not found')
+            error(f"Wrong -B --bottom-margin {arg.bottom_margin!r}, it must be zero or unsigned float in/pt/cm/mm")
+        # -I
+        if arg.multi_pages not in RADIO_DICT['I']:
+            error(f"Wrong -I --multi_pages {arg.multi_pages}, it must be in {MULTI_PAGES}")
+        var.multi_pages = int(arg.multi_pages)
+        if arg.page_headers == 'n' and var.multi_pages > 1:
+            error(f"Wrong -I --multi_pages {arg.multi_pages}, it must be 1 when -p is 'n'")
+        # -J
+        try:
+            var.multi_sheets = str2int(arg.multi_sheets, min=0)
+        except ValueError:
+            error(f"Wrong -J --many-sheets {arg.multi_sheets!r}, it must be an integer ≥ 0")
+        if var.multi_pages == 1:
+            var.multi_sheets = 0
+        elif var.multi_pages == 2 and arg.landscape and var.multi_sheets > 1:
+            var.multi_sheets = 1
+        # text_file
+        arg.text_file = strip(arg.text_file)
+        if arg.text_file:
+            arg.text_file = longpath(arg.text_file)
 
     def check_text_editor(arg):
         if not command_exists(arg.text_editor):
             error(f'Wrong -y --text-editor {arg.text_editor!r}, command not found')
 
     def check_pdf_browser(arg):
         if not command_exists(arg.pdf_browser):
             error(f'Wrong -Y --pdf-browser {arg.pdf_browser!r}, command not found')
-            
-    def open_text_file(arg, new_text_file):
-        new_text_file = long_path(new_text_file or '')
-        if isfile(new_text_file):
-            arg.text_file = new_text_file
-            lock.seize(arg.text_file)
-            hist.add(arg.text_file)
-            if arg.usage_mode == 'g':
-                arg.read_from_args_file_of(arg.text_file)
-            var.PpfFeYmdHMS = get_PpfFeYmdHMS(arg.text_file)
-            cd(dirname(arg.text_file))
-
-    def close_text_file(arg):
-        if isfile(arg.text_file):
-            arg.write_into_args_file_of(arg.text_file)
-            lock.release(arg.text_file)
-            
-    def swap_text_file(arg, new_text_file):
-        arg.close_text_file()
-        arg.open_text_file(new_text_file)
 
 arg = Arguments()
 
 #----- class History -----
 
 class History:
 
     def __init__(hist, max_files, file):
         hist.max_files = max_files
-        hist.file = long_path(file)
+        hist.file = longpath(file)
         hist.files = []
- 
+
     def read(hist):
         if isfile(hist.file):
-            hist.files = [file.strip() for file in yield_lines(hist.file) if isfile(file.strip())]
+            hist.files = list(read_lines(hist.file))
         else:
             hist.files = []
 
     def write(hist):
-        open(hist.file, 'w').write('\n'.join(unique([file.strip() for file in hist.files if file.strip() and isfile(file.strip())])[:hist.max_files]))
+        write_lines(hist.file, hist.files)
 
     def clear(hist):
-        open(hist.file, 'w').write('')
+        write_lines(hist.file)
 
     def add(hist, file):
-        if arg.usage_mode == 'g' and isfile(file):
+        if arg.usage_mode == 'g':
             hist.read()
             if not (hist.files and hist.files[0] == file):
-                hist.files = [file] + hist.files
+                hist.files = unique([file] + hist.files)[:hist.max_files]
                 hist.write()
 
     def select(hist):
         hist.read()
         if not hist.files:
-            error(f'list of recent files is empty')
-        layout = [[sg.Text(f'{jfile+1:2}.'), sg.Button(file, size=0, tooltip='select this file as the text file to be processed')] for jfile, file in enumerate(hist.files)] + [
-            [sg.Button('Clear', size=SGBS, tooltip='clear the list of recent files'),
-             sg.Button('Cancel', size=SGBS, tooltip='exit with no selection')]]
+            error(f'List of recent files is empty')
+        layout = [[sg.Text(f'{jfile+1:2}.'), sg.Button(file, size=0,
+                    tooltip='Select this file as the current text file')]
+                  for jfile, file in enumerate(hist.files)] + [
+                      [sg.Button('Clear', size=BSIZE, tooltip='Clear the list of recent files'),
+                       sg.Button('Cancel', size=BSIZE, tooltip='Exit with no selection')]]
         window = sg.Window(f'YAWP - Recent', layout)
         while True:
             event, values = window.read()
             if event in [None, 'Cancel']:
                 window.close()
-                return None
+                return ''
             elif event == 'Clear':
-                if ask_yes('YAWP - Recent', 'History of recent text files will be lost\nDo you want to clear history?', 'clear'):
+                if ask_yes('YAWP - Recent', 'History of recent text files will be lost.\nDo you want to clear history?', 'clear'):
                     hist.clear()
                     var.ok_message = ', list of recent files is empty'
                     window.close()
                     return ''
-                else:
-                    continue
             else:
-                file = event
-                if not (hist.files and hist.files[0] == file):
-                    hist.files = [file] + hist.files
-                    hist.write()
+                file = longpath(event)
+                hist.add(file)
                 window.close()
                 return file
 
-hist = History(MAX_HIST, YAWP_HIST)
-
-#----- class Log -----
-
-class Log:
-
-    def __init__(log):
-        log.output = None
-
-    def open(log):
-        log.output = open(YAWP_LOG, 'w')
-
-    def print(log, line):
-        print(line, file=log.output)
-
-    def close(log):
-        log.output.close()
-        log.output = None
-
-    def reopen(log):
-        log.output = open(YAWP_LOG, 'a')
-
-    def browse(log):
-        log.close()
-        shell(f'{arg.text_editor} {YAWP_LOG}')
-        log.reopen()
-
-log = Log()
+hist = History(MAX_HISTORY, HIST_FILE)
 
 #----- class Lock -----
 
 class Lock:
+    'seize and release files'
 
     def __init__(lock):
-        lock.files = set()
+        lock.locked_file = None
 
     def seize(lock, file):
-        if isfile(file):
-            lock_file = get_lock_file(file)
-            if isfile(lock_file):
-                if open(lock_file).read() == YAWP_LOG: # file is already locked by me
-                    return
-                else: # file is already locked by another YAWP instance
-                    error(f'file {file!r} is locked by another YAWP instance')
-            else: # file is not locked, lock it
-                open(lock_file, 'w').write(YAWP_LOG)
-                lock.files.add(file)
+        "seize file"
+        if not file:
+            error(f'File {file!r} is undefined')
+        if not isdir(dirname(longpath(file))):
+            error(f'Directory of file {file!r} not found')
+        if not isfile(file):
+            error(f'File {file!r} not found')
+        lock_file = lock_file_of(file)
+        if not isfile(lock_file):
+            pass
+        elif list(read_lines(lock_file)) == [THIS_SESSION]:
+            return
+        else:
+            error(f'File {file!r} is locked.', ask=True)
+        lock.release(lock.locked_file)
+        write_lines(lock_file, [THIS_SESSION])
+        lock.locked_file = file
 
     def release(lock, file):
-        if file in lock.files:
-            lock_file = get_lock_file(file)
-            if isfile(lock_file) and open(lock_file).read() == YAWP_LOG:
+        "release file, if it's locked by this session"
+        if file:
+            lock_file = lock_file_of(file)
+            if isfile(lock_file) and list(read_lines(lock_file)) == [THIS_SESSION]:
                 rm(lock_file)
-                lock.files.remove(file)
 
 lock = Lock()
 
 #----- class Paragraph -----
 
 class Paragraph:
 
@@ -895,427 +986,577 @@
 
     def assign(par, string, jinp, indent):
         assert not par.string
         par.string = shrink(string)
         par.jinp = jinp
         par.indent = indent
         if indent > var.chars_per_line // 2:
-            error(f"indent of indented paragraph = {indent} > -w / 2 = {var.chars_per_line // 2}", jinp, '• ' + string)
+            error(f"Indent of indented paragraph = {indent} > -w / 2 = {var.chars_per_line // 2}", jinp, '• ' + string)
 
     def append(par, string):
         assert par.string
         par.string += ' ' + shrink(string)
 
     def flush(par, buffer2):
         if not par.string:
             return
         prefix = (par.indent - 2) * ' ' + '• ' if par.indent else ''
         while len(par.string) > var.chars_per_line - par.indent:
             jchar = rfind(par.string[:var.chars_per_line-par.indent+1], ' ')
             if jchar <= 0:
-                error(f'impossible to left-justify', par.jinp, par.string)
+                error(f'Impossible to left-justify', par.jinp, par.string)
             string, par.string = par.string[:jchar], par.string[jchar+1:]
             if not arg.just_left_only:
                 try:
                     string = expand(string, var.chars_per_line - par.indent)
                 except ValueError:
-                    error(f'impossible to right-justify', par.jinp, string)
+                    error(f'Impossible to right-justify', par.jinp, string)
             buffer2.append([par.jinp, TEXT, 0, 0, prefix + string])
             prefix = par.indent * ' '
-        if  par.string:
+        if par.string:
             buffer2.append([par.jinp, TEXT, 0, 0, prefix + par.string])
             par.string = ''
 
 par = Paragraph()
 
 #----- class Correction -----
 
 class Correction:
 
     def __init__(corr):
-        corr.points = {k: [] for k in 'plm llm prm lrm ptm ltm pbm lbm pcw lcw pch lch'.split()}
+        KEYS = 'plm llm prm lrm ptm ltm pbm lbm pcw lcw pch lch'.split()
+        corr.points = {k: [] for k in KEYS}
         # read correction points from YAWP_CORR
-        if arg.correct_sizes != 'n':
-            for jline, line in enumerate(yield_lines(YAWP_CORR) if arg.correct_sizes == 'f' else CORRECTORS.split('\n')):
-                stmt = line.split('#')[0].strip()
+        if arg.correct != 'n':
+            for jline, line in enumerate(read_lines(YAWP_CORR) if arg.correct == 'f' else CORR_DEFAULT.split('\n')):
+                stmt = line2stmt(line)
                 if stmt:
                     kyx = stmt.split()
                     if len(kyx) != 3:
-                        error(f'in correction file, found {len(kyx)} values instead of 3', jline, line)
+                        error(f'In correction file, found {len(kyx)} values instead of 3', jline, line)
                     k, sy, sx = kyx
                     if k not in corr.points:
-                        error(f'in correction file, wrong key {k!r}', jline, line)
+                        error(f'In correction file, wrong key {k!r}', jline, line)
                     try:
                         x = str2inch(sx)
                         assert x >= 0.0 and (not corr.points[k] or x > corr.points[k][-1][0])
                     except (ValueError, AssertionError):
-                        error(f'in correction file, wrong x-value {sx!r}, must be ', jline, line)
+                        error(f'In correction file, wrong x-value {sx!r}, must be ', jline, line)
                     try:
                         y = str2inch(sy)
-                        assert y >= 0.0 and (not corr.points[k] or x > corr.points[k][-1][1]) 
+                        assert y >= 0.0 and (not corr.points[k] or x > corr.points[k][-1][1])
                     except (ValueError, AssertionError):
-                        error(f'in correction file, wrong y-value {sy!r}', jline, line)
+                        error(f'In correction file, wrong y-value {sy!r}', jline, line)
                     corr.points[k].append((x, y))
-            for k in 'plm llm prm lrm ptm ltm pbm lbm pcw lcw pch lch'.split():
+            for k in KEYS:
                 corr.points[k].sort()
-        # nonprintable borders in paper sheet
-        var.left_border =   [corr.points['plm'][0][0] if corr.points['plm'] and corr.points['plm'][0][1] == 0.0 else 0.0,
-                             corr.points['llm'][0][0] if corr.points['llm'] and corr.points['llm'][0][1] == 0.0 else 0.0]
-        var.right_border =  [corr.points['prm'][0][0] if corr.points['prm'] and corr.points['prm'][0][1] == 0.0 else 0.0,
-                             corr.points['lrm'][0][0] if corr.points['lrm'] and corr.points['lrm'][0][1] == 0.0 else 0.0]
-        var.top_border =    [corr.points['ptm'][0][0] if corr.points['ptm'] and corr.points['ptm'][0][1] == 0.0 else 0.0,
-                             corr.points['ltm'][0][0] if corr.points['ltm'] and corr.points['ltm'][0][1] == 0.0 else 0.0]
-        var.bottom_border = [corr.points['pbm'][0][0] if corr.points['pbm'] and corr.points['pbm'][0][1] == 0.0 else 0.0,
-                             corr.points['lbm'][0][0] if corr.points['lbm'] and corr.points['lbm'][0][1] == 0.0 else 0.0]
-        
+
 #----- class Pdf -----
 
 class Pdf:
 
-    def text2temp(pdf, text_file, temp_file, left_blanks, top_lines):
-        'copy text_file into temp_file, adding left_blanks blanks and top_lines LINEFEED'
-        assert text_file != temp_file
-        left_string = left_blanks * ' '
-        top_string = top_lines * LINEFEED
-        with open(temp_file, 'w') as temp:
-            print(top_string, file=temp)
-            for jline, line in enumerate(open(text_file)):
-                line = line.rstrip()
-                if (arg.page_headers == 'n'):
-                    if jline and (jline % var.lines_per_page == 0):
-                        print(FORMFEED + top_string, end='', file=temp)
-                else:
-                    if line.startswith(FORMFEED):
-                        print(FORMFEED + top_string, end='', file=temp)
-                        line = line[1:]
-                print(left_string + line, file=temp)
-
-    def text2pdf(pdf, text_file, pdf_file=None, left=0, right=0, top=0, bottom=0):
-        '''export text_file into pdf_file and return pdf_file name,
-        if pdf_file is None return original ~/PDF/*.pdf written by lpr'''
-        shell(f'lpr -P PDF ' # export
+    def zoom(pdf, pdf_file):
+
+        def upside_down(page):
+            page.Rotate = (int(page.inheritable.Rotate or 0) + 180) % 360
+
+        def p20(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_2 * i for i in pages.xobj_box[2:])
+            for jx, page in enumerate(pages):
+                page.scale(SCALE_2)
+                page.x = jx * dx
+                page.y = 0
+            yield pages.render()
+
+        def p40(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_4 * i for i in pages.xobj_box[2:])
+            for k, page in enumerate(pages):
+                page.scale(SCALE_4)
+                jy, jx = divmod(k, 2)
+                page.x = jx * dx
+                page.y = (1 - jy) * dy
+            yield pages.render()
+
+        def p80(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_8 * i for i in pages.xobj_box[2:])
+            for k, page in enumerate(pages):
+                page.scale(SCALE_8)
+                jy, jx = divmod(k, 4)
+                page.x = jx * dx
+                page.y = (1 - jy) * dy
+            yield pages.render()
+
+        def p21(pages_pages):
+            n = len(pages_pages)
+            swap = [n - 1, 0, 1, n - 2]
+            while len(swap) < n:
+                for step in [-2, 2, 2, -2]:
+                    swap.append(swap[-4] + step)
+            pages_pages = [pages_pages[i] for i in swap]
+            for i in range(0, n, 2):
+                pages = pages_pages[i:i+2]
+                pages = PageMerge() + pages
+                dx, dy = (SCALE_2 * i for i in pages.xobj_box[2:])
+                for jx, page in enumerate(pages):
+                    page.scale(SCALE_2)
+                    page.x = jx * dx
+                    page.y = 0
+                yield pages.render()
+
+        def p41(pages_pages):
+            n = len(pages_pages)
+            h = n // 2
+            swap = [h, h - 1, n - 1, 0, h - 2, h + 1, 1, n - 2]
+            while len(swap) < n:
+                for step in [2, -2, -2, 2, -2, 2, 2, -2]:
+                    swap.append(swap[-8] + step)
+            pages_pages = [pages_pages[i] for i in swap]
+            for i, page in enumerate(pages_pages):
+                if i % 4 < 2:
+                    upside_down(page)
+            for i in range(0, n, 4):
+                pages = pages_pages[i:i+4]
+                pages = PageMerge() + pages
+                dx, dy = (SCALE_4 * i for i in pages.xobj_box[2:])
+                for j, page in enumerate(pages):
+                    page.scale(SCALE_4)
+                    jy, jx = divmod(j, 2)
+                    page.x = jx * dx
+                    page.y = (1 - jy) * dy
+                yield pages.render()
+
+        def p81(pages_pages):
+            n = len(pages_pages)
+            swap = [4, n - 5, n - 8, 7, 3, n - 4, n - 1, 0, 6, n - 7, n - 6, 5, 1, n - 2, n - 3, 2]
+            while len(swap) < n:
+                for step in 4 * [8, -8, -8, 8]:
+                    swap.append(swap[-16] + step)
+            pages_pages = [pages_pages[i] for i in swap]
+            for i, page in enumerate(pages_pages):
+                if i % 8 < 4:
+                    upside_down(page)
+            for i in range(0, n, 8):
+                pages = pages_pages[i:i+8]
+                pages = PageMerge() + pages
+                dx, dy = (SCALE_8 * i for i in pages.xobj_box[2:])
+                for j, page in enumerate(pages):
+                    page.scale(SCALE_8)
+                    jy, jx = divmod(j, 4)
+                    page.x = jx * dx
+                    page.y = (1 - jy) * dy
+                yield pages.render()
+
+        def l20(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_2 * i for i in pages.xobj_box[2:])
+            for jy, page in enumerate(pages):
+                page.scale(SCALE_2)
+                page.x = 0
+                page.y = (1 - jy) * dy
+            yield pages.render()
+
+        def l40(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_4 * i for i in pages.xobj_box[2:])
+            for i, page in enumerate(pages):
+                page.scale(SCALE_4)
+                jy, jx = divmod(i, 2)
+                page.x = jx * dx
+                page.y = (1 - jy) * dy
+            yield pages.render()
+
+        def l80(pages):
+            pages = PageMerge() + pages
+            dx, dy = (SCALE_8 * i for i in pages.xobj_box[2:])
+            for i, page in enumerate(pages):
+                page.scale(SCALE_8)
+                jy, jx = divmod(i, 2)
+                page.x = jx * dx
+                page.y = (3 - jy) * dy
+            yield pages.render()
+
+        def l21(pages_pages):
+            n = len(pages_pages)
+            pages_pages = [pages_pages[i] for i in [3, 0, 2, 1]]
+            for i, page in enumerate(pages_pages):
+                if i % 2 == 0:
+                    upside_down(page)
+            for i in range(0, n, 2):
+                pages = pages_pages[i:i+2]
+                pages = PageMerge() + pages
+                dx, dy = (SCALE_2 * i for i in pages.xobj_box[2:])
+                for jy, page in enumerate(pages):
+                    page.scale(SCALE_2)
+                    page.x = 0
+                    page.y = (1 - jy) * dy
+                yield pages.render()
+
+        l41 = p41
+
+        def l81(pages_pages):
+            n = len(pages_pages)
+            swap = [n - 4, 3, n - 5, 4, n - 8, 7, n - 1, 0, 2, n - 3, 5, n - 6, 6, n - 7, 1, n - 2]
+            while len(swap) < n:
+                for step in 4 * [-8, 8] + 4 * [8, -8]:
+                    swap.append(swap[-16] + step)
+            pages_pages = [pages_pages[i] for i in swap]
+            for i, page in enumerate(pages_pages):
+                if i % 4 < 2:
+                    upside_down(page)
+            for i in range(0, n, 8):
+                pages = pages_pages[i:i+8]
+                pages = PageMerge() + pages
+                dx, dy = (SCALE_8 * i for i in pages.xobj_box[2:])
+                for j, page in enumerate(pages):
+                    page.scale(SCALE_8)
+                    jy, jx = divmod(j, 2)
+                    page.x = jx * dx
+                    page.y = (3 - jy) * dy
+                yield pages.render()
+
+        if var.multi_pages > 1:
+            yield_pages = {'p20': p20, 'p40': p40, 'p80': p80, 'p21': p21, 'p41': p41, 'p81': p81,
+                           'l20': l20, 'l40': l40, 'l80': l80, 'l21': l21, 'l41': l41, 'l81': l81}[
+                          f"{'pl'[arg.landscape]}{var.multi_pages}{min(1, var.multi_sheets)}"]
+            pages = PdfReader(pdf_file).pages # read pdf_file
+            writer = PdfWriter(pdf_file) # rewrite pdf_file
+            for jpage in range(0, len(pages), var.len_pages_pages):
+                for page in yield_pages(pages[jpage:jpage + var.len_pages_pages]):
+                    writer.addpage(page)
+            writer.write()
+
+    def text2text(pdf, text_file, text_file2):
+        '''copy text_file into text_file2 adding final FORMFEED chars if needed'''
+        if not isfile(text_file):
+            error(f'Text file {text_file!r} not found')
+        num_pages = 1
+        lines = list(read_lines(text_file))
+        num_pages = 1 + sum(line.startswith(FORMFEED) for line in lines)
+        var.min_multi_sheets = min(var.multi_sheets, ceildiv(num_pages, 2 * var.multi_pages))
+        var.len_pages_pages = var.multi_pages if var.min_multi_sheets == 0 else 2 * var.multi_pages * var.min_multi_sheets
+        while num_pages % var.len_pages_pages:
+            lines.append(FORMFEED + NO_BREAK_SPACE)
+            num_pages += 1
+        write_lines(text_file2, lines)
+
+    def text2pdf(pdf, text_file, lp_page_left):
+        'export text_file into pdf_file and return pdf_file name'
+        shell(f'lp -d PDF ' # export
               f'-o print-quality={MAX_QUALITY} '
-              f'-o media=Custom.{in2pt(var.paper_width)}x{in2pt(var.paper_height)} '
-              f'-o cpi={var.chars_per_inch2} '
-              f'-o lpi={var.lines_per_inch2} '
-              f'-o page-top={in2pt(top)} '
-              f'-o page-left={in2pt(left)} '
-              f'-o page-right={in2pt(right)} '
-              f'-o page-bottom={in2pt(bottom)} '
+              f'-o media=Custom.{in2pt(var.sheet_width)}x{in2pt(var.sheet_height)} '
+              f'-o cpi={pdf.lp_chars_per_inch} '
+              f'-o lpi={pdf.lp_lines_per_inch} '
+              f'-o page-top={in2pt(pdf.lp_page_top)} '
+              f'-o page-left={in2pt(lp_page_left)} '
+              f'-o page-right=0 '
+              f'-o page-bottom=0 '
               f'{text_file!r}')
-        while any(line.startswith('active') for line in shell(f'lpq -P PDF')): # wait lp completion
-            sleep(0.1)
-        sleep(1)
-        pattern = '~/PDF/.*.pdf' if basename(text_file).startswith('.') else '~/PDF/*.pdf' # hidden or not
+        wait_lp_completion()
+        dot = basename(text_file).startswith('.') * '.' # hidden or not?
         try:
-            last_pdf = last_file(pattern) # seek the most recent one
+            last_pdf = last_file(f'{PDF_PATH}/{dot}*.pdf') # find the most recent one
         except FileNotFoundError:
-            error(f'exported PDF file not found')
-        if pdf_file is None:
-            return last_pdf
-        else:
-            mv(last_pdf, pdf_file)
-            return pdf_file
+            error(f'Exported PDF file not found')
+        return last_pdf
 
     def pdfpdf2pdf(pdf, even_pdf_file, odd_pdf_file, pdf_file):
         'merge even pages from even_pdf_file with odd pages from odd_pdf_file into pdf_file'
         even_pages = PdfReader(even_pdf_file).pages
         odd_pages = PdfReader(odd_pdf_file).pages
         pdf_writer = PdfWriter()
         for jpage, (even_page, odd_page) in enumerate(zip(even_pages, odd_pages)):
             pdf_writer.addpage(even_page if jpage % 2 else odd_page)
         pdf_writer.write(var.pdf_file)
 
+    def correct(pdf):
+        'compute parameters of lp commands, corrected following -C'
+        corr = Correction()
+        pl = 'pl'[arg.landscape]
+        pdf.lp_page_left      = least_squares_line(corr.points[f'{pl}lm'], var.left_margin)
+        pdf.lp_page_right     = least_squares_line(corr.points[f'{pl}rm'], var.right_margin)
+        pdf.lp_page_top       = least_squares_line(corr.points[f'{pl}tm'], var.top_margin)
+        pdf.lp_page_bottom    = least_squares_line(corr.points[f'{pl}bm'], var.bottom_margin)
+        if pdf.lp_page_left < 0.0:
+            error(f'-L --left-margin {arg.left_margin} is too small, PDF file may be wrong', ask=True)
+            pdf.lp_page_left = 0.0
+        if pdf.lp_page_right < 0.0:
+            error(f'-R --right-margin {arg.right_margin} is too small, PDF file may be wrong', ask=True)
+            pdf.lp_page_right = 0.0
+        if pdf.lp_page_top < 0.0:
+            error(f'-T --top-margin {arg.top_margin} is too small, PDF file may be wrong', ask=True)
+            pdf.lp_page_top = 0.0
+        if pdf.lp_page_bottom < 0.0:
+            error(f'-B --bottom-margin {arg.bottom_margin} is too small, PDF file may be wrong', ask=True)
+            pdf.lp_page_bottom = 0.0
+        pdf.lp_page_left_odd_pages  = pdf.lp_page_left
+        pdf.lp_page_left_even_pages = pdf.lp_page_left if arg.all_pages_E_e else pdf.lp_page_right
+        pdf.lp_char_width     = least_squares_line(corr.points[f'{pl}cw'], var.char_width)
+        if pdf.lp_char_width <= 0.0:
+            error(f'Character width is too small, corrected value ≤ 0')
+        pdf.lp_char_height    = least_squares_line(corr.points[f'{pl}ch'], var.char_height)
+        if pdf.lp_char_height <= 0.0:
+            error(f'Character height is too small, corrected value ≤ 0')
+        pdf.lp_chars_per_inch = 1.0 / pdf.lp_char_width
+        pdf.lp_lines_per_inch = 1.0 / pdf.lp_char_height
+        # inform
+        inform(['Corrections:',
+            f'    left_margin = {inch2str(pdf.lp_page_left, ROUND)}',
+            f'    right_margin = {inch2str(pdf.lp_page_right, ROUND)}',
+            f'    top_margin = {inch2str(pdf.lp_page_top, ROUND)}',
+            f'    bottom_margin = {inch2str(pdf.lp_page_bottom, ROUND)}',
+            f'    char_width = {inch2str(pdf.lp_char_width, ROUND)}',
+            f'    char_height = {inch2str(pdf.lp_char_height, ROUND)}',
+            f'    chars_per_inch = {round(pdf.lp_chars_per_inch, ROUND)}',
+            f'    lines_per_inch = {round(pdf.lp_lines_per_inch, ROUND)}'])
+
     def export_and_browse(pdf, text_file):
-        var.pdf_file = long_path(evalchar(arg.pdf_file, 'PpfFeYmdHMS', var.PpfFeYmdHMS, '%'))
+        var.pdf_file = longpath(evalchar(arg.pdf_file, 'PpfeYmdHMS', var.PpfeYmdHMS, '%'))
         if not isdir(dirname(var.pdf_file)):
             error(f'Wrong -P --file-pdf {arg.pdf_file!r}, directory {dirname(var.pdf_file)!r} not found')
-        if isfile(var.pdf_file):
-            rm(var.pdf_file)
-        if var.left_margin == var.right_margin or arg.all_pages_E_e: # export directly into var.pdf_file
-            if arg.fake_margins: # text -> temp -> pdf
-                temp_file = get_temp_file(arg.text_file)
-                pdf.text2temp(arg.text_file, temp_file, var.left_blanks, var.top_lines)
-                pdf.text2pdf(temp_file, var.pdf_file)
-                rm(temp_file)
-            else:                # text -> pdf
-                pdf.text2pdf(arg.text_file, var.pdf_file, left=var.left_margin2, right=var.right_margin2, top=var.top_margin2, bottom=var.bottom_margin2)
-        else: # export into var.pdf_file through even_pdf_file and odd_pdf_file
-            if arg.fake_margins: # text -> temp -> even; text -> temp -> odd; even, odd -> pdf
-                temp_file = get_temp_file(arg.text_file)
-                pdf.text2temp(arg.text_file, temp_file, var.left_blanks, var.top_lines)
-                even_pdf_file = pdf.text2pdf(temp_file)
-                pdf.text2temp(arg.text_file, temp_file, var.right_blanks, var.top_lines)
-                odd_pdf_file = pdf.text2pdf(temp_file)
-                rm(temp_file)
-                pdf.pdfpdf2pdf(even_pdf_file, odd_pdf_file, var.pdf_file)
-            else:                # text -> even; text -> odd; even, odd -> pdf
-                even_pdf_file = pdf.text2pdf(arg.text_file, left=var.left_margin2, right=var.right_margin2, top=var.top_margin2, bottom=var.bottom_margin2)
-                odd_pdf_file = pdf.text2pdf(arg.text_file, left=var.left_margin3, right=var.right_margin3, top=var.top_margin2, bottom=var.bottom_margin2)
-                pdf.pdfpdf2pdf(even_pdf_file, odd_pdf_file, var.pdf_file)
-        inform(f'Export:  {arg.text_file!r} ──▷')
-        inform(f'         {var.pdf_file!r}')
-        shell(f'{arg.pdf_browser} {var.pdf_file!r}') # browse
+        rm(var.pdf_file)
+        pdf.correct()
+        temp_file = temp_file_of(text_file)
+        pdf.text2text(arg.text_file, temp_file)
+        even_pdf_file = pdf.text2pdf(temp_file, pdf.lp_page_left_even_pages)
+        odd_pdf_file = pdf.text2pdf(temp_file, pdf.lp_page_left_odd_pages)
+        if temp_file.endswith('.temp'):
+            rm(temp_file)
+        pdf.pdfpdf2pdf(even_pdf_file, odd_pdf_file, var.pdf_file)
+        rm(even_pdf_file)
+        rm(odd_pdf_file)
+        if var.multi_pages > 1:
+            pdf.zoom(var.pdf_file)
+        inform([f'Export:',
+            f'    {arg.text_file!r} →',
+            f'    {var.pdf_file!r}'])
+        if arg.export_pdf == 'b':
+            shell(f'{arg.pdf_browser} {var.pdf_file!r}') # browse
 
 pdf = Pdf()
 
 #----- class Buffer -----
 
 class Buffer:
 
-    def __init__(buf, file=None):
-        buf.buffer = [] # [[jinp, kind, jpag, lpic, line]] # output buffer
+    def __init__(buf, file=''):
+        buf.buffer = [] # [[jinp, kind, jpage, lpic, line]] # output buffer
         # jinp: line index in buf.input
-        # kind: kind of line: CODE, TEXT, PICT, CONT, INDX, FIGU, CHP1, CHP2, HEA1, HEA2
-        # jpag: page number
+        # kind: kind of line: TEXT, PICT, CONT, INDX, FIGU, CHP1, CHP2, HEA1, HEA2
+        # jpage: page number
         # lpic: lines in picture (in first line of pictures only, else 0)
         # line
         buf.contents = [] # [[pref, titl, jout]], if words == line.split():
-        # pref: words[0], chapter numbering as '1.', '1.1.'...
+        # pref: words[0], chapter numbering as '1.', '1.1.'…
         # titl: ' '.join(words[1:])
         # jout: position of chapter line in buf.buffer
         buf.contents_found = False # file contains a contents chapter line?
         buf.contents_jout = -1 # position of contents chapter line in output
         buf.qsub_jouts = SetDict() # {subject: {jout}}
         # subject: subject between double quotes
         # jout: position of subject in buf.buffer
         buf.uqsub_jouts = SetDict() # {subject: {jout}}
         # subject: subject not between double quotes
         # jout: position of subject in buf.buffer
         buf.index_found = False # file contains an index chapter line?
         buf.index_jout = -1 # position of index chapter line in output
         buf.subjects = set()
         buf.figures_found = False # file contains a figures chapter line?
-        buf.figures_jout = -1 # position  of figures chapter line in buf.buffer
-        buf.figures = [] # [[pref, titl, jout]] , if words == line.split() ...
+        buf.figures_jout = -1 # position of figures chapter line in buf.buffer
+        buf.figures = [] # [[pref, titl, jout]] , if words == line.split() …
         # words[0] == var.figures_title
-        # pref: words[1], figure numbering as 'a.', '1.b.', '1.1.c.'...
+        # pref: words[1], figure numbering as 'a.', '1.b.', '1.1.c.'…
         # titl: ' '.join(words[2:])
         # jout: position of caption line in buf.buffer
-        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_chars_per_line, buf.num_pages = 0, 0, 0, 0, 1
-        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_chars_per_line = 0, 0, 0, 0
-        if file:
+        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_line_length, buf.num_pages = 0, 0, 0, 0, 1
+        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_line_length = 0, 0, 0, 0
+        if isfile(file):
+            if filesize(file) == 0:
+                error(f'File empty reading file {file!r}')
             buf.read_from_file(file)
 
     def read_from_file(buf, file):
         buf.buffer = []
-        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_chars_per_line, buf.num_pages = 0, 0, 0, 0, 1
-        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_chars_per_line = 0, 0, 0, 0
-        for jinp, line in enumerate(yield_lines(file)):
+        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_line_length, buf.num_pages = 0, 0, 0, 0, 1
+        buf.hea2_num_lines, buf.hea2_chars, buf.hea2_words, buf.hea2_max_line_length = 0, 0, 0, 0
+        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_line_length = 0, 0, 0, 0
+        for jinp, line in enumerate(read_lines(file)):
             buf.buffer.append([jinp, PICT, 1, 0, line])
             if line.startswith(FORMFEED):
                 buf.head_chars += len(line) - 1
                 buf.head_words += len(line[1:].split())
-                buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line) - 1)
+                buf.head_max_line_length = max(buf.head_max_line_length, len(line) - 1)
                 buf.head_num_lines += 1
                 buf.num_pages += 1
-            elif line.startswith(MACRON):
-                buf.head_chars += len(line)
-                buf.head_words += len(line.split())
-                buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line))
-                buf.head_num_lines += 1
+            elif line and line[0] in HEADER_CHARS:
+                buf.hea2_chars += len(line)
+                buf.hea2_words += len(line.split())
+                buf.hea2_max_line_length = max(buf.head_max_line_length, len(line))
+                buf.hea2_num_lines += 1
             else:
                 buf.body_chars += len(line)
                 buf.body_words += len(line.split())
-                buf.body_max_chars_per_line = max(buf.body_max_chars_per_line, len(line))
+                buf.body_max_line_length = max(buf.body_max_line_length, len(line))
                 buf.body_num_lines += 1
-           
+
     def write_into_file(buf, file):
-        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_chars_per_line, buf.num_pages = 0, 0, 0, 0, 1
-        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_chars_per_line = 0, 0, 0, 0
-        with open(file, 'w') as file_w:
-            for reco in buf.buffer:
-                line = reco[LINE]
-                print(line, file=file_w)
+        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_line_length, buf.num_pages = 0, 0, 0, 0, 1
+        buf.hea2_num_lines, buf.hea2_chars, buf.hea2_words, buf.hea2_max_line_length = 0, 0, 0, 0
+        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_line_length = 0, 0, 0, 0
+        with open(file, 'w') as output:
+            for record in buf.buffer:
+                line = record[LINE]
                 if line.startswith(FORMFEED):
                     buf.head_chars += len(line) - 1
                     buf.head_words += len(line[1:].split())
-                    buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line) - 1)
+                    buf.head_max_line_length = max(buf.head_max_line_length, len(line) - 1)
                     buf.head_num_lines += 1
                     buf.num_pages += 1
-                elif line.startswith(MACRON):
-                    buf.head_chars += len(line)
-                    buf.head_words += len(line.split())
-                    buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line))
-                    buf.head_num_lines += 1
+                elif line and line[0] in HEADER_CHARS:
+                    buf.hea2_chars += len(line)
+                    buf.hea2_words += len(line.split())
+                    buf.hea2_max_line_length = max(buf.head_max_line_length, len(line))
+                    buf.hea2_num_lines += 1
                 else:
                     buf.body_chars += len(line)
                     buf.body_words += len(line.split())
-                    buf.body_max_chars_per_line = max(buf.body_max_chars_per_line, len(line))
+                    buf.body_max_line_length = max(buf.body_max_line_length, len(line))
                     buf.body_num_lines += 1
+                print(line, file=output)
 
     def copy(buf):
         buf2 = Buffer()
-        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_chars_per_line, buf.num_pages = 0, 0, 0, 0, 1
-        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_chars_per_line = 0, 0, 0, 0
-        for reco in buf.buffer:
-            rec2 = reco[:] # deep copy
+        buf.head_num_lines, buf.head_chars, buf.head_words, buf.head_max_line_length, buf.num_pages = 0, 0, 0, 0, 1
+        buf.hea2_num_lines, buf.hea2_chars, buf.hea2_words, buf.hea2_max_line_length = 0, 0, 0, 0
+        buf.body_num_lines, buf.body_chars, buf.body_words, buf.body_max_line_length = 0, 0, 0, 0
+        for record in buf.buffer:
+            rec2 = record[:] # deep copy
             buf2.buffer.append(rec2)
             line = rec2[LINE]
             if line.startswith(FORMFEED):
                 buf.head_chars += len(line) - 1
                 buf.head_words += len(line[1:].split())
-                buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line) - 1)
+                buf.head_max_line_length = max(buf.head_max_line_length, len(line) - 1)
                 buf.head_num_lines += 1
                 buf.num_pages += 1
-            elif line.startswith(MACRON):
+            elif line and line[0] in HEADER_CHARS:
                 buf.head_chars += len(line)
                 buf.head_words += len(line.split())
-                buf.head_max_chars_per_line = max(buf.head_max_chars_per_line, len(line))
+                buf.head_max_line_length = max(buf.head_max_line_length, len(line))
                 buf.head_num_lines += 1
             else:
                 buf.body_chars += len(line)
                 buf.body_words += len(line.split())
-                buf.body_max_chars_per_line = max(buf.body_max_chars_per_line, len(line))
+                buf.body_max_line_length = max(buf.body_max_line_length, len(line))
                 buf.body_num_lines += 1
         return buf2
 
     def inform(buf, title):
         'write informations about buf after last buf.read_from_file() or last buf.write_into_file() or buf.copy()'
-        inform(title)
-        inform(f"    header: {plural(buf.head_num_lines, 'line')}, "
-               f"{plural(buf.head_words, 'word')}, {plural(buf.head_chars, 'char')}, "
-               f"max {plural(buf.head_max_chars_per_line, 'char')} per line, {plural(buf.num_pages, 'page')}")
-        inform(f"    body:   {plural(buf.body_num_lines, 'line')}, "
-               f"{plural(buf.body_words, 'word')}, {plural(buf.body_chars, 'char')}, "
-               f"max {plural(buf.body_max_chars_per_line, 'char')} per line")
-        inform(f"    total:  {plural(buf.head_num_lines + buf.body_num_lines, 'line')}, "
-               f"{plural(buf.head_words+buf.body_words, 'word')}, {plural(buf.head_chars+buf.body_chars, 'char')}, "
-               f"max {plural(max(buf.head_max_chars_per_line, buf.body_max_chars_per_line), 'char')} per line")
+        inform([title,
+            f"    header1: {plural(buf.head_num_lines, 'line')}, "
+            f"{plural(buf.head_words, 'word')}, {plural(buf.head_chars, 'char')}, "
+            f"max {plural(buf.head_max_line_length, 'char')} per line, {plural(buf.num_pages, 'page')}",
+            f"    header2: {plural(buf.hea2_num_lines, 'line')}, "
+            f"{plural(buf.hea2_words, 'word')}, {plural(buf.hea2_chars, 'char')}, "
+            f"max {plural(buf.hea2_max_line_length, 'char')} per line",
+            f"    body:   {plural(buf.body_num_lines, 'line')}, "
+            f"{plural(buf.body_words, 'word')}, {plural(buf.body_chars, 'char')}, "
+            f"max {plural(buf.body_max_line_length, 'char')} per line",
+            f"    total:  {plural(buf.head_num_lines + buf.body_num_lines, 'line')}, "
+            f"{plural(buf.head_words+buf.hea2_words+buf.body_words, 'word')}, {plural(buf.head_chars+buf.hea2_chars+buf.body_chars, 'char')}, "
+            f"max {plural(max(buf.head_max_line_length, buf.hea2_max_line_length, buf.body_max_line_length), 'char')} per line"])
 
     def __eq__(buf, buf2):
+        'text lines in buf.buffer == text lines in buf2.buffer?'
         return len(buf.buffer) == len(buf2.buffer) and all(record[LINE] == record2[LINE] for record, record2 in zip(buf.buffer, buf2.buffer))
 
-    def char(buf, jout, jchar):
-        "return buf.buffer[jout][LINE][jchar], if not PICT or on IndexError return '*', used by redraw_segments() and redraw_arroheads()"
+    def char(buf, jout, jchar, default='*'):
+        "return buf.buffer[jout][LINE][jchar], if not PICT or on IndexError return default, used by redraw_segments() and redraw_arroheads()"
         if jout < 0 or jchar < 0:
-            return '*'
+            return default
         else:
             try:
                 line = buf.buffer[jout][LINE]
-                return line[jchar] if buf.buffer[jout][KIND] == PICT else '*'
+                return line[jchar] if buf.buffer[jout][KIND] == PICT else default
             except IndexError:
-                return '*'
+                return default
 
-    def compute_and_correct_sizes(buf):
-        if buf.body_max_chars_per_line == 0:
-            error(f'text file is empty')
-        # set correction parameters depending on arg.correct_sizes
-        corr = Correction()
-        # free space
-        inform(f'Compute: page width {inch2str(var.paper_width, ROUND)}')
-        inform(f'Compute: page height {inch2str(var.paper_height, ROUND)}')
-        var.free_width = var.paper_width - var.left_margin - var.right_margin
-        inform(f'Compute: free width {inch2str(var.free_width, ROUND)}')
-        if var.free_width <= 0:
+    def compute(buf):
+        var.print_width = var.sheet_width - var.left_margin - var.right_margin
+        var.print_height = var.sheet_height - var.top_margin - var.bottom_margin
+        if var.print_width <= 0.0:
             error(f'-L and/or -R too large, no horizontal space on paper')
-        var.free_height = var.paper_height - var.top_margin - var.bottom_margin
-        inform(f'Compute: free height {inch2str(var.free_height, ROUND)}')
-        if var.free_height <= 0:
+        if var.print_height <= 0.0:
             error(f'-T and/or -B too large, no vertical space on paper')
-        # corrected -L -R -T -B
-        var.left_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'lm'], var.left_margin))
-        var.right_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'rm'], var.right_margin))
-        var.top_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'tm'], var.top_margin))
-        var.bottom_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'bm'], var.bottom_margin))
-        # compute automatic -w -W
-        if var.chars_per_line and not var.char_width: # if -w and not -W == 0: -W = f(-w)
-            var.char_width = var.free_width / var.chars_per_line
-            inform(f'Compute: -W --char-width {inch2str(var.char_width, ROUND)}')
-            if var.char_width <= 0:
-                error(f'Wrong -W --char-width {inch2str(var.char_width, ROUND)} ≤ 0')
-        elif not var.chars_per_line and var.char_width: # if not -w and -W: -w = f(-W)
-            var.chars_per_line = int(var.free_width / var.char_width)
-            inform(f'Compute: -w --chars-per-line {var.chars_per_line}')
-            if var.chars_per_line <= 0:
-                error(f'Wrong -w --chars-per-line {inch2str(var.chars_per_line, ROUND)} ≤ 0')
-        elif not var.chars_per_line and not var.char_width: # if not -w and not -W: -w = f(file); -W = f(-w)
-            var.chars_per_line = buf.body_max_chars_per_line # set by read_file()
-            inform(f'Compute: -w --chars-per-line {var.chars_per_line}')
-            if var.chars_per_line <= 0:
-                error(f'Wrong -w --chars-per-line {inch2str(var.chars_per_line, ROUND)} ≤ 0')
-            var.char_width = var.free_width / var.chars_per_line
-            inform(f'Compute: -W --char-width {inch2str(var.char_width, ROUND)}')
-            if var.char_width <= 0:
-                error(f'Wrong -W --char-width {inch2str(var.char_width, ROUND)} ≤ 0')
-        # correct -L -R -T -B -W
-        if arg.correct_sizes == 'n':
-            var.left_margin2 = var.left_margin
-            var.right_margin2 = var.right_margin
-            var.left_margin3 = var.right_margin # swapped for even pages
-            var.right_margin3 = var.left_margin # swapped for even pages
-            var.top_margin2 = var.top_margin
-            var.bottom_margin2 = var.bottom_margin
-            var.char_width2 = var.char_width
+        def w2W(chars_per_line): return var.print_width / chars_per_line
+        def u2W(lines_per_page): return var.print_height * var.char_aspect / lines_per_page
+        def W2w(char_width): return int(var.print_width / char_width)
+        def W2u(char_width): return int(var.print_height * var.char_aspect / char_width)
+        if var.char_width == 0.0:
+            if var.lines_per_page == 0:
+                if var.chars_per_line == 0:
+                    var.chars_per_line = max_line_length_in(arg.text_file)
+                    if var.chars_per_line == 0:
+                        error(f'Text file {arg.text_file} is empty or contains empty lines only.')
+                    var.char_width = w2W(var.chars_per_line)
+                    var.lines_per_page = W2u(var.char_width)
+                else:
+                    var.char_width = w2W(var.chars_per_line)
+                    var.lines_per_page = W2u(var.char_width)
+            else:
+                if var.chars_per_line == 0:
+                    var.char_width = u2W(var.lines_per_page)
+                    var.chars_per_line = W2w(var.char_width)
+                else:
+                    var.char_width = min(w2W(var.chars_per_line), u2W(var.lines_per_page))
         else:
-            var.char_width2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'cw'], var.char_width))
-            inform(f'Correct: -W --char-width {inch2str(var.char_width2, ROUND)}')
-            var.right_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'rm'], var.right_margin))
-            var.left_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'lm'], var.left_margin))
-            if var.left_margin == var.right_margin or arg.all_pages_E_e:
-                inform(f'Correct: -L --left-margin {inch2str(var.right_margin2, ROUND)} (all pages)')
-                inform(f'Correct: -R --right-margin {inch2str(var.left_margin2, ROUND)} (all pages)')
+            if var.lines_per_page == 0:
+                if var.chars_per_line == 0:
+                    var.chars_per_line = W2w(var.char_width)
+                    var.lines_per_page = W2u(var.char_width)
+                else:
+                    var.char_width = min(var.char_width, w2W(var.chars_per_line))
+                    var.lines_per_page = W2u(var.char_width)
             else:
-                inform(f'Correct: -L --left-margin {inch2str(var.right_margin2, ROUND)} (odd pages)')
-                inform(f'Correct: -R --right-margin {inch2str(var.left_margin2, ROUND)} (odd pages)')
-                var.right_margin3 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'rm'], var.left_margin))
-                inform(f'Correct: -L --left-margin {inch2str(var.right_margin3, ROUND)} (even pages)')
-                var.left_margin3 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'lm'], var.right_margin))
-                inform(f'Correct: -R --right-margin {inch2str(var.left_margin3, ROUND)} (even pages)')
-            var.top_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'tm'], var.top_margin))
-            inform(f'Correct: -T --top-margin {inch2str(var.top_margin2, ROUND)} (all pages)')
-            var.bottom_margin2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'bm'], var.bottom_margin))
-            inform(f'Correct: -B --bottom-margin {inch2str(var.bottom_margin2, ROUND)} (all pages)')
-        # compute char_height, chars_per_inch, lines_per_inch, lines_per_page
+                if var.chars_per_line == 0:
+                    var.char_width = min(var.char_width, u2W(var.lines_per_page))
+                    var.chars_per_line = W2w(var.char_width)
+                else:
+                    var.char_width = min(var.char_width, w2W(var.chars_per_line), u2W(var.lines_per_page))
         var.char_height = var.char_width / var.char_aspect
-        inform(f'Compute: char height {inch2str(var.char_height, ROUND)}')
-        var.chars_per_inch = 1.0 / var.char_width
-        inform(f'Compute: chars per inch {round(var.chars_per_inch, ROUND)}')
-        var.lines_per_inch = 1.0 / var.char_height
-        inform(f'Compute: lines per inch {round(var.lines_per_inch, ROUND)}')
-        # correct char_height, chars_per_inch, lines_per_inch
-        if arg.correct_sizes == 'n':
-            var.char_height2 = var.char_height
-            var.chars_per_inch2 = var.chars_per_inch
-            var.lines_per_inch2 = var.lines_per_inch
-        else:
-            var.char_height2 = max(0.0, broken_line(corr.points['pl'[arg.landscape] + 'ch'], var.char_height))
-            inform(f'Correct: char height {inch2str(var.char_height2, ROUND)}')
-            var.chars_per_inch2 = 1.0 / var.char_width2
-            inform(f'Correct: chars per inch {round(var.chars_per_inch2, ROUND)}')
-            var.lines_per_inch2 = 1.0 / var.char_height2
-            inform(f'Correct: lines per inch {round(var.lines_per_inch2, ROUND)}')
-        # compute lines_per_page
-        var.lines_per_page = int(var.lines_per_inch * var.free_height) - 2 * (arg.page_headers != 'n') - 1
-        inform(f'Compute: lines per page {var.lines_per_page}')
-        # compute fake margins
-        if arg.fake_margins:
-            var.left_blanks = int((var.left_margin - var.left_border[arg.landscape]) / var.char_width)
-            var.right_blanks = int((var.right_margin - var.left_border[arg.landscape]) / var.char_width) # sic
-            var.top_lines = int((var.top_margin - var.top_border[arg.landscape]) / var.char_height)
-            inform(f'Fake: left blanks {var.left_blanks}')
-            inform(f'Fake: right blanks {var.right_blanks}')
-            inform(f'Fake: top empty lines {var.top_lines}') 
+        var.PpfeYmdHMS = PpfeYmdHMS_of(arg.text_file)
+        inform(['Computations:',
+            f'    print_width = {inch2str(var.print_width, ROUND)}',
+            f'    print_height = {inch2str(var.print_height, ROUND)}',
+            f'    chars_per_line = {var.chars_per_line}',
+            f'    lines_per_page = {var.lines_per_page}',
+            f'    char_width = {inch2str(var.char_width, ROUND)}',
+            f'    char_height = {inch2str(var.char_height, ROUND)}',
+            f'    chars_per_inch = {round(1.0/var.char_width, ROUND)}',
+            f'    lines_per_inch = {round(1.0/var.char_height, ROUND)}'])
 
     def remove_page_headers(buf):
-        buf.buffer = [record for record in buf.buffer if not (record[LINE].startswith(FORMFEED) or record[LINE].startswith(MACRON))]
+        buf.buffer = [record for record in buf.buffer if not record[LINE] or record[LINE][0] not in HEADER_CHARS]
 
     def justify_lines(buf):
         buffer2 = []
         for jinp, x, x, x, line in buf.buffer:
             if not line: # empty line
                 par.flush(buffer2)
                 buffer2.append([jinp, EMPT, 0, 0, ''])
             else:
                 jdot = findchar(line, '[! ]')
                 if jdot >= 0 and line[jdot:jdot+2] in ['• ','. ']: # dot line
                     if jdot + 2 > var.chars_per_line:
-                        error('Dot line indentation {jdot+2} > chars per line {var.chars_per_line}')
+                        error(f'Dot line indentation {jdot+2} > chars per line {var.chars_per_line}')
                     par.flush(buffer2)
-                    par.assign(line[jdot+2:].strip(), jinp, jdot + 2)
+                    par.assign(strip(line[jdot+2:]), jinp, jdot + 2)
                 elif line[0] == ' ': # indented line
                     if par.string:
                         par.append(line)
                     else:
                         buffer2.append([jinp, PICT, 0, 0, line])
                 elif par.string: # unindented line
                     par.append(line)
@@ -1324,62 +1565,66 @@
         par.flush(buffer2)
         buf.buffer = buffer2
 
     def redraw_segments(buf):
         charstr = '`─│┐│┘│┤──┌┬└┴├┼'
         #          0123456789ABCDEF
         charset = frozenset(charstr)
-        for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+        for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
             if kind == PICT:
                 chars = list(line)
                 for jchar, char in enumerate(chars):
                     if char in charset:
-                        kchar = (1 * (buf.char(jout, jchar - 1) in charset) +
+                        kchar = (    (buf.char(jout, jchar - 1) in charset) +
                                  2 * (buf.char(jout + 1, jchar) in charset) +
                                  4 * (buf.char(jout - 1, jchar) in charset) +
                                  8 * (buf.char(jout, jchar + 1) in charset))
                         if kchar:
-                            chars[jchar] = charstr[kchar]    
+                            chars[jchar] = charstr[kchar]
                 buf.buffer[jout][LINE] = ''.join(chars)
 
     def redraw_arrowheads(buf):
         charstr = '^▷△^▽^^^◁^^^^^^^'
         #          0123456789ABCDEF
         charset = frozenset(charstr)
-        for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+        for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
             if kind == PICT:
                 chars = list(line)
                 for jchar, char in enumerate(chars):
                     if char in charset:
-                        kchar = (1 * (buf.char(jout, jchar - 1) == '─') +
+                        kchar = (    (buf.char(jout, jchar - 1) == '─') +
                                  2 * (buf.char(jout + 1, jchar) == '│') +
                                  4 * (buf.char(jout - 1, jchar) == '│') +
                                  8 * (buf.char(jout, jchar + 1) == '─'))
                         if kchar:
-                            chars[jchar] = charstr[kchar]    
+                            chars[jchar] = charstr[kchar]
                 buf.buffer[jout][LINE] = ''.join(chars)
 
+    def redraw(buf):
+        buf.redraw_segments()
+        buf.redraw_arrowheads()
+
     def renumber_chapters(buf):
-        levels = []; max_level = 1; nout = len(buf.buffer)
-        for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+        levels = [var.chapter_offset]; max_level = 1; nout = len(buf.buffer)
+        for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
             prev_line = buf.buffer[jout-1][LINE] if jout > 0 else ''
             next_line = buf.buffer[jout+1][LINE] if jout + 1 < nout else ''
             if kind == TEXT and line and not prev_line and not next_line:
                 words = line.split()
                 level = chapter_level(words[0])
-                title = unqupper(line)
+                title = shrink_alphaupper(line)
                 if level > 0: # numbered chapter line
                     if level > max_level:
-                        error(f'numbered chapter level is {level} > {max_level}', jinp)
+                        error(f'Numbered chapter level is {level} > {max_level}', jinp)
                     elif level == len(levels) + 1:
                         levels.append(1)
                     else:
                         levels = levels[:level]
                         levels[-1] += 1
-                    title = unqupper(' '.join(words[1:]))
+                    title = shrink_alphaupper(' '.join(words[1:]))
                     buf.buffer[jout][KIND] = CHP1 if level == 1 else CHP2
                     buf.buffer[jout][LINE] = '.'.join(str(level) for level in levels) + '. ' + title
                     max_level = len(levels) + 1
                 elif title == var.contents_title: # contents chapter line
                     buf.buffer[jout][KIND] = CONT
                     buf.buffer[jout][LINE] = title
                     max_level = 1
@@ -1390,75 +1635,73 @@
                 elif title == var.index_title: # index chapter line
                     buf.buffer[jout][KIND] = INDX
                     buf.buffer[jout][LINE] = title
                     max_level = 1
                 else: # no chapter line
                     title = ''
 
-    def add_chapters_to_contents(buf):
-        for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+    def add_chapters_to_contents_chapter(buf):
+        for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
             if kind == CONT:
                 if buf.contents_found:
-                    error(f'more than one contents line in text file', jinp)
+                    error(f'More than one contents line in text file', jinp)
                 buf.contents_found = True
                 # contents chapter doesn't list itself
             elif kind == FIGU:
                 if buf.figures_found:
-                    error(f'more than one figures line in text file', jinp)
+                    error(f'More than one figures line in text file', jinp)
                 buf.figures_found = True
-                buf.contents.append(['', unqtitle(var.figures_title), jout])
+                buf.contents.append(['', shrink_alphatitle(var.figures_title), jout])
             elif kind == INDX:
                 if buf.index_found:
-                    error(f'more than one index line in text file', jinp)
+                    error(f'More than one index line in text file', jinp)
                 buf.index_found = True
-                buf.contents.append(['', unqtitle(var.index_title), jout])
+                buf.contents.append(['', shrink_alphatitle(var.index_title), jout])
             elif kind in [CHP1, CHP2]:
                 prefix, title = (line.split(None, 1) + [''])[:2]
-                buf.contents.append([prefix, unqtitle(title), jout])
+                buf.contents.append([prefix, shrink_alphatitle(title), jout])
 
-    def add_captions_to_figures(buf):
+    def add_captions_to_figures_chapter(buf):
         if buf.figures_found:
             seek = False
-            max_len_caption = 0
             chapter = ''
             letter = prevchar('a')
             for jout, record in enumerate(buf.buffer):
-                jinp, kind, jpag, lpic, line = record
+                jinp, kind, jpage, lpic, line = record
                 if kind in [CONT, INDX, FIGU]:
                     seek = True
                 elif kind in [CHP1, CHP2]:
                     seek = False
                     chapter = line.split()[0]
                     letter = prevchar('a')
                 elif not seek and kind == PICT and (
                     jout == 0 or buf.buffer[jout-1][KIND] == EMPT) and (
                     jout == len(buf.buffer) - 1 or buf.buffer[jout+1][KIND] == EMPT):
-                    words = unqtitle(line).split()
+                    words = shrink_alphatitle(line).split()
                     if len(words) >= 2:
-                        prefix, label, *title = unqtitle(line).split()
-                        title = ' '.join(title)
+                        prefix, label, *leftovers = words
+                        title = ' '.join(leftovers)
                         if prefix.upper() == var.caption_prefix and figure_level(label.lower()) > 0:
                             if letter == 'z':
                                 error(f'in text file, more than 26 figure captions in a single chapter', jinp, line)
                             letter = nextchar(letter)
                             label = f'{chapter}{letter}.'
                             caption = f'{prefix} {label} {title}'
-                            max_len_caption = max(max_len_caption, len(caption))
                             blanks = (var.chars_per_line - len(caption)) // 2 * ' '
                             buf.figures.append((label, title, jout))
                             record[LINE] = blanks + caption
                             record[KIND] = CAPT
                             if jout >= 2 and buf.buffer[jout - 2][KIND] == PICT:
                                 buf.buffer[jout - 1][KIND] = PICT # paste caption with previous picture
 
-    def add_quoted_subjects_to_index(buf):
+    def add_quoted_subjects_to_index_chapter(buf):
         if buf.index_found:
             buf.qsub_jouts = SetDict() # {subject: jout}
             quote = False; subject = ''; seek = True
-            for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+            for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
                 if kind in [CONT, FIGU, INDX]:
                     seek = False
                 elif kind in [CHP1, CHP2]:
                     seek = True
                 elif seek and kind == TEXT:
                     for jchar, char in enumerate(line + ' '):
                         if quote:
@@ -1466,88 +1709,89 @@
                                 subject = shrink(subject)
                                 buf.qsub_jouts.add(subject, jout)
                                 buf.subjects.add(subject)
                                 quote = False
                             else:
                                 subject += char
                                 if len(subject) > var.chars_per_line // 2:
-                                    error(f'length of subject "{subject}..." > -w / 2 = {var.chars_per_line // 2}')
+                                    error(f'Length of subject "{subject}…" > -w / 2 = {var.chars_per_line // 2}')
                         elif (char == '"' and get(line, jchar-1, ' ') not in QUOTES and get(line, jchar+1, ' ') not in QUOTES):
                             subject = ''
                             quote = True
                 else:
                     if quote:
-                        error(f'unpaired \'"\' found while filling the index')
+                        error(f'Unpaired \'"\' found while filling the index')
             if quote:
-                error(f'unpaired \'"\' found while filling the index')
+                error(f'Unpaired \'"\' found while filling the index')
 
-    def add_unquoted_subjects_to_index(buf):
+    def add_unquoted_subjects_to_index_chapter(buf):
         if buf.index_found:
             buf.uqsub_jouts = SetDict() # {subject: jout}
             charset = set(chars('[a-zA-Z0-9]') + ''.join(buf.qsub_jouts.keys()))
             word_jouts = [] # [(word, jout)]
             seek = True
-            for jout, (jinp, kind, jpag, lpic, line) in enumerate(buf.buffer):
+            for jout, (jinp, kind, jpage, lpic, line) in enumerate(buf.buffer):
                 if kind in [CONT, FIGU, INDX]:
                     seek = False
                 elif kind in [CHP1, CHP2]:
                     seek = True
                 elif seek and kind == TEXT:
                     for word in take(line, charset, ' ').split():
                         word_jouts.append((word, jout))
             sub0_subws = ListDict() # {subject.word[0]: subject.word[1:]}
             for subject in buf.qsub_jouts.keys():
-                subjectwords = subject.split()
+                subjectwords = split(subject)
                 sub0_subws.append(subjectwords[0], subjectwords[1:])
             for jword_jouts, (sub0, jout) in enumerate(word_jouts):
                 if sub0 in sub0_subws:
                     for subw in sub0_subws[sub0]:
                         subject = sub0 + ' ' + ' '.join(subw) if subw else sub0
                         if subject == ' '.join(w for w, j in word_jouts[jword_jouts: jword_jouts + len(subw) + 1]):
                             buf.uqsub_jouts.add(subject, jout)
                             buf.subjects.add(subject)
 
     def insert_contents_figures_and_index_chapters(buf):
 
         def append_contents_to(buffer2):
             jinp = buffer2[-1][JINP]
             buffer2.append([jinp, TEXT, 0, 0, ''])
-            fmt_labl = max((len(labl) for labl, titl, jpag in buf.contents), default=0)
-            fmt_titl = max((len(titl) for labl, titl, jpag in buf.contents), default=0)
-            for labl, titl, jpag in buf.contents:
-                line = f'{INDENT}• {edit(labl, fmt_labl)} {edit(titl, fmt_titl)}'
-                if len(line.rstrip()) > var.chars_per_line:
-                    error(f'length of contents chapter line {line!r} is {len(line.rstrip())} > -w = {var.chars_per_line}')
+            fmt_labl = max((len(labl) for labl, titl, jpage in buf.contents), default=0)
+            fmt_titl = max((len(titl) for labl, titl, jpage in buf.contents), default=0)
+            for labl, titl, jpage in buf.contents:
+##                line = f'{INDENT}• {edit(labl, fmt_labl)} {edit(titl, fmt_titl)}'
+                line = f'{INDENT}• {edit(labl, fmt_labl)} {titl}'
+##                if len(strip(line)) > var.chars_per_line:
+##                    error(f'Length of Contents chapter line is {len(strip(line))} > -w = {var.chars_per_line}', jinp, strip(line))
                 buffer2.append([jinp, TEXT, 0, 0, line])
             buffer2.append([jinp, TEXT, 0, 0, ''])
 
         def append_figures_to(buffer2):
             jinp = buffer2[-1][JINP]
             buffer2.append([jinp, TEXT, 0, 0, ''])
-            fmt_labl = max((len(labl) for labl, titl, jpag in buf.figures), default=0)
-            fmt_titl = max((len(titl) for labl, titl, jpag in buf.figures), default=0)
-            for labl, titl, jpag in buf.figures:
+            fmt_labl = max((len(labl) for labl, titl, jpage in buf.figures), default=0)
+            fmt_titl = max((len(titl) for labl, titl, jpage in buf.figures), default=0)
+            for labl, titl, jpage in buf.figures:
                 line = f'{INDENT}• {edit(labl, fmt_labl)} {edit(titl, fmt_titl)}'
-                if len(line.rstrip()) > var.chars_per_line:
-                    error(f'length of figures chapter line {line!r} is {len(line.rstrip())} > -w = {var.chars_per_line}')
+                if len(strip(line)) > var.chars_per_line:
+                    error(f'Length of Figures chapter line is {len(strip(line))} > -w = {var.chars_per_line}', jinp, strip(line))
                 buffer2.append([jinp, TEXT, 0, 0, line])
             buffer2.append([jinp, TEXT, 0, 0, ''])
 
         def append_index_to(buffer2):
             jinp = buffer2[-1][JINP]
             buffer2.append([jinp, TEXT, 0, 0, ''])
             room = max((len(subject) for subject in buf.subjects), default=0) + 1
             for subject in sorted(buf.subjects):
                 line = f'{INDENT}• {edit(subject, room)}'
-                if len(line.rstrip()) > var.chars_per_line:
-                    error(f'length of index chapter line {line!r} is {len(line.rstrip())} > -w = {var.chars_per_line}')
+                if len(strip(line)) > var.chars_per_line:
+                    error(f'Length of Index chapter line is {len(strip(line))} > -w = {var.chars_per_line}', jinp, strip(line))
                 buffer2.append([jinp, TEXT, 0, 0, line])
             buffer2.append([jinp, TEXT, 0, 0, ''])
 
-        buffer2 = [] 
+        buffer2 = []
         copy = True
         for record in buf.buffer:
             kind = record[KIND]
             if kind == CONT:
                 buf.contents_jout = len(buffer2)
                 buffer2.append(record)
                 append_contents_to(buffer2)
@@ -1567,508 +1811,461 @@
                 copy = True
             elif copy:
                 buffer2.append(record)
         buf.buffer = buffer2
 
     def check_line_lengths(buf):
         for jinp, kind, zero, lpic, line in buf.buffer:
-            if kind != CODE and len(line) > var.chars_per_line:
-                error(f'in text file, line length {len(line)} > -w --chars-per-line {var.chars_per_line} in text file', jinp, line)
+            if len(strip(line)) - line.startswith(FORMFEED) > var.chars_per_line:
+                error(f'Line length {len(line)} > -w --chars-per-line {var.chars_per_line} in text file', jinp, line)
 
     def count_picture_lines(buf):
         jpic = 0
         for jout, record in retroenum(buf.buffer):
             if record[KIND] in [PICT, CAPT]:
                 jpic += 1
                 if jout == 0 or buf.buffer[jout-1][KIND] not in [PICT, CAPT]:
                     buf.buffer[jout][LPIC] = jpic
             else:
                 jpic = 0
 
     def count_pages(buf):
-        jpag, jpagline = 1, 0
+        jpage, jpagline = 1, 0
         for jout, (jinp, kind, zero, lpic, line) in enumerate(buf.buffer):
-            if (arg.page_headers in 'fpc' and jpagline >= var.lines_per_page or
-                arg.page_headers in 'pc' and lpic < var.lines_per_page and jpagline + lpic >= var.lines_per_page or
-                arg.page_headers == 'c' and kind in [CONT, INDX, FIGU, CHP1] and not (jout >= 2 and not buf.buffer[jout-1][LINE] and buf.buffer[jout-1][JPAG] > buf.buffer[jout-2][JPAG])):
-                jpag += 1
+            if (arg.page_headers in 'fpcd' and jpagline >= var.lines_per_page - var.page_header_lines or
+                arg.page_headers in 'pcd' and lpic < var.lines_per_page and jpagline + lpic >= var.lines_per_page or
+                arg.page_headers in 'cd' and kind in [CONT, INDX, FIGU, CHP1] and not (
+                    jout >= 2 and not buf.buffer[jout-1][LINE] and buf.buffer[jout-1][JPAG] > buf.buffer[jout-2][JPAG])):
+                jpage += 1 + (arg.page_headers == 'd' and kind in [CONT, INDX, FIGU, CHP1] and jpage % 2 == 1)
                 jpagline = 0
             else:
                 jpagline += 1
-            buf.buffer[jout][JPAG] = jpag
+            buf.buffer[jout][JPAG] = jpage
 
-    def add_page_numbers_to_contents(buf):
+    def add_page_numbers_to_contents_chapter(buf):
         if buf.contents_jout > -1:
             width = max_len_page_number(buf.buffer[-1][JPAG], var.page_offset) + 1
             for jcontents, (prefix, titl, jout) in enumerate(buf.contents):
                 line = buf.buffer[buf.contents_jout + 2 + jcontents][LINE] + edit(page_number(buf.buffer[jout][JPAG], var.page_offset), width, right=True)
-                if len(line) > var.chars_per_line:
-                    error(f'length of contents chapter line {line!r} is {len(line)} > -w = {var.chars_per_line}')
+##                if len(line) > var.chars_per_line:
+##                    error(f'Length of Contents chapter line is {len(line)} > -w = {var.chars_per_line}', jinp, line)
                 buf.buffer[buf.contents_jout + 2 + jcontents][LINE] = line
 
-    def add_page_numbers_to_index(buf):
+    def add_page_numbers_to_index_chapter(buf):
         if buf.index_jout > -1:
-            qsub_jpags = SetDict() # {quoted_subject: {jpag}}
+            qsub_jpags = SetDict() # {quoted_subject: {jpage}}
             for subject, jouts in buf.qsub_jouts.items():
                 for jout in jouts:
                     qsub_jpags.add(subject, buf.buffer[jout][JPAG])
-            uqsub_jpags = SetDict() # {unquoted_subject: {jpag}}
+            uqsub_jpags = SetDict() # {unquoted_subject: {jpage}}
             for subject, jouts in buf.uqsub_jouts.items():
                 for jout in jouts:
-                    jpag = buf.buffer[jout][JPAG]
-                    if jpag not in qsub_jpags[subject]:
-                        uqsub_jpags.add(subject, jpag)
+                    jpage = buf.buffer[jout][JPAG]
+                    if jpage not in qsub_jpags[subject]:
+                        uqsub_jpags.add(subject, jpage)
             for jindex, subject in enumerate(sorted(buf.subjects)):
-                jpag_strjs = sorted((jpag, f'"{page_number(jpag, var.page_offset)}"'
-                                     if jpag in qsub_jpags[subject] else page_number(jpag, var.page_offset))
-                    for jpag in (qsub_jpags[subject] | uqsub_jpags[subject])) # [(jpag, str(jpag))]
-                line = buf.buffer[buf.index_jout + 2 + jindex][LINE] + ', '.join(strj for jpag, strj in jpag_strjs)
+                jpag_strjs = sorted((jpage, f'"{page_number(jpage, var.page_offset)}"'
+                                     if jpage in qsub_jpags[subject] else page_number(jpage, var.page_offset))
+                    for jpage in (qsub_jpags[subject] | uqsub_jpags[subject])) # [(jpage, str(jpage))]
+                line = buf.buffer[buf.index_jout + 2 + jindex][LINE] + ', '.join(strj for jpage, strj in jpag_strjs)
                 if len(line) > var.chars_per_line:
-                    warning(f"Index line for {subject!r} longer than -w --chars-per-line {var.chars_per_line}, truncated")
                     while True:
                         line = line[:line.rfind(',')]
-                        if len(line) + 5 <= var.chars_per_line:
+                        if len(line) + 3 <= var.chars_per_line:
                             break
-                    line += ', ...'
+                    line += ', …'
+                if len(line) > var.chars_per_line:
+                    error(f'Length of Index chapter line is {len(line)} > -w = {var.chars_per_line}', jinp, line)
                 buf.buffer[buf.index_jout + 2 + jindex][LINE] = line
 
-    def add_page_numbers_to_figures(buf):
+    def add_page_numbers_to_figures_chapter(buf):
         if buf.figures_jout > -1:
             width = max_len_page_number(buf.buffer[-1][JPAG], var.page_offset) + 1
             for jfigures, (prefix, title, jout) in enumerate(buf.figures):
                 line = buf.buffer[buf.figures_jout + 2 + jfigures][LINE] + edit(page_number(buf.buffer[jout][JPAG], var.page_offset), width, right=True)
                 if len(line) > var.chars_per_line:
-                    error(f'length of figures chapter line {line!r} is {len(line)} > -w {var.chars_per_line}')
+                    error(f'Length of Figures chapter line is {len(line)} > -w = {var.chars_per_line}', jinp, line)
                 buf.buffer[buf.figures_jout + 2 + jfigures][LINE] = line
 
     def insert_page_headers(buf):
-        if buf.buffer:
-            jout = 0; jpag0 = 1; chapter = ''; npag = buf.buffer[-1][JPAG]
-            header2 = var.chars_per_line * MACRON
-            while jout < len(buf.buffer):
-                jinp, kind, jpag, lpic, line = buf.buffer[jout]
+
+        def header1(jinp, jpage, npages, chapter):
+            left, right = ((arg.even_right, arg.even_left) if arg.all_pages_E_e else
+                           (arg.odd_left, arg.odd_right) if jpage % 2 else
+                           (arg.even_left, arg.even_right))
+            PpfeYmdHMSnNc = var.PpfeYmdHMS + (page_number(jpage, var.page_offset), str(npages), chapter)
+            left = evalchar(left, 'PpfeYmdHMSnNc', PpfeYmdHMSnNc, '%')
+            right = evalchar(right, 'PpfeYmdHMSnNc', PpfeYmdHMSnNc, '%')
+            blanks = ' ' * max(1, (var.chars_per_line - len(left) - len(right)))
+            header = left + blanks + right
+            return [jinp, HEA1, jpage, lpic, FORMFEED + header]
+
+        def header2(jinp, jpage, npages, chapter):
+            second_line = var.chars_per_line * SECOND_LINE_CHARS[arg.second_line]
+            return [jinp, HEA2, jpage, lpic, second_line]
+
+        if buf.buffer: # insert page headers
+            buffer2 = []; jpag0 = 1; chapter = ''; npages = buf.buffer[-1][JPAG]
+            for record in buf.buffer:
+                jinp, kind, jpage, lpic, line = record
                 if kind in [CONT, INDX, FIGU, CHP1]:
-                    chapter = unqtitle(line)
-                if jpag > jpag0:
-                    left, right = ((arg.even_right, arg.even_left) if arg.all_pages_E_e else
-                                   (arg.odd_left, arg.odd_right) if jpag % 2 else
-                                   (arg.even_left, arg.even_right))
-                    PpfFeYmdHMSnNc = var.PpfFeYmdHMS + (page_number(jpag, var.page_offset), str(npag), chapter)
-                    left = evalchar(left, 'PpfFeYmdHMSnNc', PpfFeYmdHMSnNc, '%')
-                    right = evalchar(right, 'PpfFeYmdHMSnNc', PpfFeYmdHMSnNc, '%')
-                    blanks = ' ' * (var.chars_per_line - len(left) - len(right))
-                    if not blanks:
-                        header1 = f'{left} {right}'
-                        error(f"length of header {header1!r} is {len(header1)} > -w {var.chars_per_line}")
-                    header1 = f'{FORMFEED}{left}{blanks}{right}'
-                    buf.buffer.insert(jout, [0, HEA2, jpag, 0, header2])
-                    buf.buffer.insert(jout, [0, HEA1, jpag, 0, header1])
-                    jout += 2
-                    jpag0 = jpag
-                elif jout >= 3 and not buf.buffer[jout-1][LINE] and buf.buffer[jout-3][LINE].startswith(FORMFEED):
-                    left, right = ((arg.even_right, arg.even_left) if arg.all_pages_E_e else
-                                   (arg.odd_left, arg.odd_right) if jpag % 2 else
-                                   (arg.even_left, arg.even_right))
-                    PpfGeYmdHMSnNc = var.PpfFeYmdHMS + (str(jpag), str(npag), chapter)
-                    left = evalchar(left, 'PpfFeYmdHMSnNc', PpfFeYmdHMSnNc, '%')
-                    right = evalchar(right, 'PpfFeYmdHMSnNc', PpfFeYmdHMSnNc, '%')
-                    blanks = ' ' * (var.chars_per_line - len(left) - len(right))
-                    if not blanks:
-                        header1 = f'{left} {right}'
-                        error(f"length of header {header1!r} is {len(header1)} > -w --chars-per-line {var.chars_per_line}")
-                    buf.buffer[jout-3][LINE] = f'{FORMFEED}{left}{blanks}{right}'
-                jout += 1
+                        chapter = shrink_alphatitle(line)
+                if jpage == jpag0 + 2:
+                    buffer2.append(header1(jinp, jpage - 1, npages, chapter))
+                    if arg.second_line != 'n':
+                        buffer2.append(header2(jinp, jpage - 1, npages, chapter))
+                if jpage > jpag0:
+                    buffer2.append(header1(jinp, jpage, npages, chapter))
+                    if arg.second_line != 'n':
+                        buffer2.append(header2(jinp, jpage, npages, chapter))
+                jpag0 = jpage
+                buffer2.append(record)
+            buf.buffer = buffer2
 
 #----- main window -----
 
-def main_window():
-    'main window of GUI mode'
-    sg.theme('Python')
+def gui_main_window():
+    sg.theme(THEME)
     button = 'Main'
-    while True: # loop after 'x' button or Alt-F4 error
-        layout = [
-            # format arguments
-            [sg.Text('-v --verbose',         size=SGTS), sg.Checkbox('', default=arg.verbose,         key='v', tooltip=arg.letter_tooltip['v'])],
-            [sg.Text('-y --text-editor',     size=SGTS), sg.Input(arg.text_editor, size=SGAS,         key='y', tooltip=arg.letter_tooltip['y']),
-             sg.Text('-g --graphics',        size=SGTS), sg.Checkbox('', default=arg.graphics,        key='g', tooltip=arg.letter_tooltip['g'])],
-            [sg.Text('-w --chars-per-line',  size=SGTS), sg.Input(arg.chars_per_line, size=SGAS,      key='w', tooltip=arg.letter_tooltip['w']),
-             sg.Text('-l --just-left-only',  size=SGTS), sg.Checkbox('', default=arg.just_left_only,  key='l', tooltip=arg.letter_tooltip['l'])],
-            [sg.Text('-c --contents-title',  size=SGTS), sg.Input(arg.contents_title, size=SGAS,      key='c', tooltip=arg.letter_tooltip['c']),
-             sg.Text('-i --index-title',     size=SGTS), sg.Input(arg.index_title, size=SGAS,         key='i', tooltip=arg.letter_tooltip['i'])],
-            [sg.Text('-f --figures-title',   size=SGTS), sg.Input(arg.figures_title, size=SGAS,       key='f', tooltip=arg.letter_tooltip['f']),
-             sg.Text('-F --caption-prefix',  size=SGTS), sg.Input(arg.caption_prefix, size=SGAS,      key='F', tooltip=arg.letter_tooltip['F'])],
-            # paging arguments
-            [sg.Text('-p --page-headers',    size=SGTS),
-                sg.Radio('n=no',       'p',  default=arg.page_headers=='n', tooltip="do not insert page headers"),
-                sg.Radio('f=fullpage', 'p',  default=arg.page_headers=='f', tooltip="insert page headers on full page"),
-                sg.Radio('p=picture',  'p',  default=arg.page_headers=='p', tooltip="...and on broken picture"),
-                sg.Radio('c=chapter',  'p',  default=arg.page_headers=='c', tooltip="...and before level-1 chapters")],
-            [sg.Text('-e --even-left',       size=SGTS), sg.Input(arg.even_left, size=SGAS,           key='e', tooltip=arg.letter_tooltip['e']),
-             sg.Text('-E --even-right',      size=SGTS), sg.Input(arg.even_right, size=SGAS,          key='E', tooltip=arg.letter_tooltip['E'])],
-            [sg.Text('-o --odd-left',        size=SGTS), sg.Input(arg.odd_left, size=SGAS,            key='o', tooltip=arg.letter_tooltip['o']),
-             sg.Text('-O --odd-right',       size=SGTS), sg.Input(arg.odd_right, size=SGAS,           key='O', tooltip=arg.letter_tooltip['O'])],
-            [sg.Text('-n --page-offset',     size=SGTS), sg.Input(arg.page_offset, size=SGAS,         key='n', tooltip=arg.letter_tooltip['n']),
-             sg.Text('-a --all-pages-E-e',   size=SGTS), sg.Checkbox('', default=arg.all_pages_E_e,   key='a', tooltip=arg.letter_tooltip['a'])],
-            # export arguments
-            [sg.Text('-X --export-view-pdf', size=SGTS), sg.Checkbox('', default=arg.export_view_pdf, key='X', tooltip=arg.letter_tooltip['X'])],
-            [sg.Text('-Y --pdf-browser',     size=SGTS), sg.Input(arg.pdf_browser, size=SGAS,         key='Y', tooltip=arg.letter_tooltip['Y']),
-             sg.Text('-P --file-pdf',        size=SGTS), sg.Input(arg.pdf_file, size=SGAS,            key='P', tooltip=arg.letter_tooltip['P'])],
-            [sg.Text('-W --char-width',      size=SGTS), sg.Input(arg.char_width, size=SGAS,          key='W', tooltip=arg.letter_tooltip['W']),
-             sg.Text('-A --char-aspect',     size=SGTS), sg.Input(arg.char_aspect, size=SGAS,         key='A', tooltip=arg.letter_tooltip['A'])],
-            [sg.Text('-S --paper-size',      size=SGTS), sg.Input(arg.paper_size, size=SGAS,          key='S', tooltip=arg.letter_tooltip['S']),
-             sg.Text('-Z --landscape',       size=SGTS), sg.Checkbox('', default=arg.landscape,       key='Z', tooltip=arg.letter_tooltip['Z'])],
-            [sg.Text('-L --left-margin',     size=SGTS), sg.Input(arg.left_margin, size=SGAS,         key='L', tooltip=arg.letter_tooltip['L']),
-             sg.Text('-R --right-margin',    size=SGTS), sg.Input(arg.right_margin, size=SGAS,        key='R', tooltip=arg.letter_tooltip['R'])],
-            [sg.Text('-T --top-margin',      size=SGTS), sg.Input(arg.top_margin, size=SGAS,          key='T', tooltip=arg.letter_tooltip['T']),
-             sg.Text('-B --bottom-margin',   size=SGTS), sg.Input(arg.bottom_margin, size=SGAS,       key='B', tooltip=arg.letter_tooltip['B'])],
-            [sg.Text('-C --correct-sizes',   size=SGTS),
-                sg.Radio('n=no',      'C',   default=arg.correct_sizes=='n', tooltip="do not correct char size and page margins"),
-                sg.Radio('d=default', 'C',   default=arg.correct_sizes=='d', tooltip="correct char size and page margins\nby default values"),
-                sg.Radio('f=file',    'C',   default=arg.correct_sizes=='f', tooltip="correct char size and page margins\nby correction file"),
-             sg.Text('', size=0),
-             sg.Text('-K --fake-margins',    size=SGTS), sg.Checkbox('', default=arg.fake_margins,     key='K', tooltip=arg.letter_tooltip['K'])],
-            # text_file argument, read-only
-            [sg.Text('text_file',            size=SGTS), sg.Text(arg.text_file, size=SGFS, key='t', tooltip=arg.letter_tooltip['t'])],
-            # action buttons
-            [sg.Button(button, tooltip=BUTTON_TOOLTIP[button], size=SGBS) for button in ['New','Open','Recent','Saveas','Help','Exit']],
-            [sg.Button(button, tooltip=BUTTON_TOOLTIP[button], size=SGBS) for button in ['Edit','Format','Noformat','Undo','Log','Correct']]]
-        window = sg.Window(f'YAWP - Main', layout, finalize=True)
-        while True: # window.read() loop
-            try:
-                if not arg.text_file:
-                    arg.read_text_file_from_sess_file(YAWP_SESS)
-                    arg.read_from_args_file_of(arg.text_file)
-                    arg.write_into_window(window)
-                button, values = window.read()
-                if not button: # 'x' button or Alt-F4 error
-                    message = "ERROR: You cannot close YAWP by typing alt-F4 or clicking the 'x' button\nClick the 'Exit' button instead"
-                    log.print(message)
-                    print(message, file=stderr)
-                    ask_ok('Main', message)
-                    break
-                inform(frame(f'{button:<10} {now()}'))
-                arg.read_from_window(window)
-                arg.set_default_if_empty()
-                arg.write_into_window(window)
-                old_text_file = arg.text_file
-                var.ok_message = ''
-                {'New':      New_button,
-                 'Open':     Open_button,
-                 'Recent':   Recent_button,
-                 'Saveas':   Saveas_button,
-                 'Correct':  Correct_button,
-                 'Help':     Help_button,
-                 'Exit':     Exit_button,
-                 'Edit':     Edit_button,
-                 'Format':   Format_button,
-                 'Noformat': Noformat_button,
-                 'Undo':     Undo_button,
-                 'Log':      Log_button}[button]()
-                arg.text_file = long_path(arg.text_file)
-                var.PpfFeYmdHMS = get_PpfFeYmdHMS(arg.text_file)
-                path = dirname(arg.text_file)
-                if isdir(path):
-                    cd(path)
-                if old_text_file != arg.text_file: # altered by New/Open/Recent/Saveas?
-                    if isfile(old_text_file):
-                        arg.write_into_args_file_of(old_text_file)
-                    arg.read_from_args_file_of(arg.text_file)
-                    cd(dirname(arg.text_file))
+    space = lambda size=0: sg.Text(size=size)
+    block = lambda title='': sg.Text(title, size=7)
+    layout = [
+        [block('Format'), sg.Text('-y --text-editor',     size=TSIZE), sg.Input(arg.text_editor, size=FSIZE,         key='y', tooltip=tooltips['y']),
+         space(40), sg.Text('Status'), sg.Text(WAITING, key='Status', tooltip=f"status indicator ({WAITING!r} or {RUNNING!r})")],
+        [block(),         sg.Text('-w --chars-per-line',  size=TSIZE), sg.Input(arg.chars_per_line, size=FSIZE,      key='w', tooltip=tooltips['w']), space(),
+         sg.Text('-g --graphics',        size=TSIZE), sg.Checkbox('', default=arg.graphics,         key='g', tooltip=tooltips['g'])],
+        [block(),         sg.Text('-u --lines-per-page',  size=TSIZE), sg.Input(arg.lines_per_page, size=FSIZE,      key='u', tooltip=tooltips['u']), space(),
+         sg.Text('-l --just-left-only',  size=TSIZE), sg.Checkbox('', default=arg.just_left_only,   key='l', tooltip=tooltips['l'])],
+        [block('Chapters'),sg.Text('-c --contents-title',  size=TSIZE), sg.Input(arg.contents_title, size=FSIZE,      key='c', tooltip=tooltips['c']), space(),
+         sg.Text('-i --index-title',     size=TSIZE), sg.Input(arg.index_title, size=FSIZE,         key='i', tooltip=tooltips['i'])],
+        [block(),         sg.Text('-f --figures-title',   size=TSIZE), sg.Input(arg.figures_title, size=FSIZE,       key='f', tooltip=tooltips['f']), space(),
+         sg.Text('-F --caption-prefix',  size=TSIZE), sg.Input(arg.caption_prefix, size=FSIZE,      key='F', tooltip=tooltips['F'])],
+        [block(),         sg.Text('-m --chapter-offset',  size=TSIZE), sg.Input(arg.chapter_offset, size=FSIZE,      key='m', tooltip=tooltips['m'])],
+        [block('Pages'),         sg.Text('-p --page-headers',    size=TSIZE),
+            sg.Radio('no',       'p', default=arg.page_headers=='n', tooltip='do not insert page headers'),
+            sg.Radio('fullpage', 'p', default=arg.page_headers=='f', tooltip='insert page headers on full page'),
+            sg.Radio('picture',  'p', default=arg.page_headers=='p', tooltip='…and on broken picture'),
+            sg.Radio('chapter',  'p', default=arg.page_headers=='c', tooltip='…and before level-1 chapters'),
+            sg.Radio('double',   'p', default=arg.page_headers=='d', tooltip='…and double if level-1 on even page'),],
+        [block(),         sg.Text('-e --even-left',       size=TSIZE), sg.Input(arg.even_left, size=FSIZE,           key='e', tooltip=tooltips['e']), space(),
+         sg.Text('-E --even-right',      size=TSIZE), sg.Input(arg.even_right, size=FSIZE,          key='E', tooltip=tooltips['E'])],
+        [block(),         sg.Text('-o --odd-left',        size=TSIZE), sg.Input(arg.odd_left, size=FSIZE,            key='o', tooltip=tooltips['o']), space(),
+         sg.Text('-O --odd-right',       size=TSIZE), sg.Input(arg.odd_right, size=FSIZE,           key='O', tooltip=tooltips['O'])],
+        [block(),         sg.Text('-n --page-offset',     size=TSIZE), sg.Input(arg.page_offset, size=FSIZE,         key='n', tooltip=tooltips['n']), space(),
+         sg.Text('-a --all-pages-E-e',   size=TSIZE), sg.Checkbox('', default=arg.all_pages_E_e,    key='a', tooltip=tooltips['a'])],
+        [block(),         sg.Text('-s --second_line',     size=TSIZE),
+            sg.Radio('no',       's', default=arg.second_line=='n', tooltip='no second line in page header'),
+            sg.Radio('blanks',   's', default=arg.second_line=='b', tooltip='blank second line in page header'),
+            sg.Radio('points',   's', default=arg.second_line=='p', tooltip='dotted second line in page header'),
+            sg.Radio('dashes',   's', default=arg.second_line=='d', tooltip='dashed second line in page header'),
+            sg.Radio('solid',    's', default=arg.second_line=='s', tooltip='solid second line in page header')],
+        [block('Export'), sg.Text('-X --export-pdf',      size=TSIZE),
+            sg.Radio('no',       'X', default=arg.export_pdf=='n', tooltip='do not export'),
+            sg.Radio('export',   'X', default=arg.export_pdf=='e', tooltip='export PDF file'),
+            sg.Radio('browse',   'X', default=arg.export_pdf=='b', tooltip='export and browse PDF file'), space(4),
+         sg.Text('-C --correct', size=TSIZE),
+            sg.Radio('no',       'C', default=arg.correct=='n', tooltip='do not correct char size and page margins'),
+            sg.Radio('default',  'C', default=arg.correct=='d', tooltip='correct char size and page margins by default values'),
+            sg.Radio('file',     'C', default=arg.correct=='f', tooltip='correct char size and page margins by correction file')],
+        [block(),         sg.Text('-Y --pdf-browser',     size=TSIZE), sg.Input(arg.pdf_browser, size=FSIZE,         key='Y', tooltip=tooltips['Y']), space(),
+         sg.Text('-P --file-pdf',        size=TSIZE), sg.Input(arg.pdf_file, size=FSIZE,            key='P', tooltip=tooltips['P'])],
+        [block(),         sg.Text('-W --char-width',      size=TSIZE), sg.Input(arg.char_width, size=FSIZE,          key='W', tooltip=tooltips['W']), space(),
+         sg.Text('-A --char-aspect',     size=TSIZE), sg.Input(arg.char_aspect, size=FSIZE,         key='A', tooltip=tooltips['A'])],
+        [block(),         sg.Text('-S --sheet-size',      size=TSIZE), sg.Input(arg.sheet_size, size=FSIZE,          key='S', tooltip=tooltips['S']), space(),
+         sg.Text('-Z --landscape',       size=TSIZE), sg.Checkbox('', default=arg.landscape,        key='Z', tooltip=tooltips['Z'])],
+        [block(),         sg.Text('-L --left-margin',     size=TSIZE), sg.Input(arg.left_margin, size=FSIZE,         key='L', tooltip=tooltips['L']), space(),
+         sg.Text('-R --right-margin',    size=TSIZE), sg.Input(arg.right_margin, size=FSIZE,        key='R', tooltip=tooltips['R'])],
+        [block(),         sg.Text('-T --top-margin',      size=TSIZE), sg.Input(arg.top_margin, size=FSIZE,          key='T', tooltip=tooltips['T']), space(),
+         sg.Text('-B --bottom-margin',   size=TSIZE), sg.Input(arg.bottom_margin, size=FSIZE,       key='B', tooltip=tooltips['B'])],
+        [block(),         sg.Text('-I --multi-pages',     size=TSIZE),
+            sg.Radio('1',        'I', default=arg.multi_pages=='1', tooltip=f"export 1 page per side of paper sheets"),
+            sg.Radio('2',        'I', default=arg.multi_pages=='2', tooltip=f"export 2 pages per side of paper sheets"),
+            sg.Radio('4',        'I', default=arg.multi_pages=='4', tooltip=f"export 4 pages per side of paper sheets"),
+            sg.Radio('8',        'I', default=arg.multi_pages=='8', tooltip=f"export 8 pages per side of paper sheets"), space(8),
+         sg.Text('-J --multi-sheets',    size=TSIZE), sg.Input(arg.multi_sheets, size=FSIZE,        key='J', tooltip=tooltips['J'])],
+        [block('Text File'), sg.Text(arg.text_file, key='t', tooltip=tooltips['t'])],
+        # action buttons
+        [sg.Button('New',      tooltip=tooltips['New']),
+         sg.Button('Open',     tooltip=tooltips['Open']),
+         sg.Button('Recent',   tooltip=tooltips['Recent']),
+         sg.Button('SaveAs',   tooltip=tooltips['SaveAs']), space(),
+         sg.Button('Edit',     tooltip=tooltips['Edit']),
+         sg.Button('Format',   tooltip=tooltips['Format']),
+         sg.Button('NoFormat', tooltip=tooltips['NoFormat']),
+         sg.Button('Undo',     tooltip=tooltips['Undo']),space(),
+         sg.Button('Log',      tooltip=tooltips['Log']),
+         sg.Button('Help',     tooltip=tooltips['Help']),
+         sg.Button('Exit',     tooltip=tooltips['Exit'])]]
+
+##        [sg.Button(button, tooltip=tooltips[button], size=BSIZE) for button in ['New','Open','Recent','SaveAs','Edit','Format','NoFormat','Undo','Log','Help','Exit']]]
+    window = sg.Window(f'YAWP - Main', layout, finalize=True)
+    while True: # window.read() loop
+        try:
+            window['Status'].update(WAITING)
+            window.refresh()
+            button, values = window.read()
+            arg.read_from_window(window)
+            button = button or 'Exit'
+            if button != 'Exit':
+                window['Status'].update(RUNNING)
+                arg.shrink_all()
                 arg.write_into_window(window)
-            except YawpError as yawp_error:
-                ask_ok(button, f'{button}: {yawp_error}')
-            else:
-                inform(f'{button}: OK')
-
-#----- buttons, first line: New Open Recent Saveas Help Exit -----
-
-def New_button():
-    'create a new empty text file, which becomes the new text file'
-    new_file = long_path(sg.popup_get_file('', no_window=True, save_as=True))
+            var.ok_message = ''
+            {'New':      new_button,
+             'Open':     open_button,
+             'Recent':   recent_button,
+             'SaveAs':   saveas_button,
+             'Help':     help_button,
+             'Exit':     exit_button,
+             'Edit':     edit_button,
+             'Format':   format_button,
+             'NoFormat': noformat_button,
+             'Undo':     undo_button,
+             'Log':      log_button}[button]()
+            arg.write_into_window(window)
+        except YawpError:
+            pass
+
+#----- buttons, first line: New Open Recent SaveAs Help Exit -----
+
+def new_button():
+    'create a new empty text file with default arguments, which becomes the new current text file'
+    old_text_file = arg.text_file
+    new_text_file = sg.popup_get_file('', no_window=True, save_as=True)
     # if new file aready exists, confirmation window is issued by sg.PopupGetFile() itself
-    if new_file:
-        dir_of_new_file = dirname(new_file)
-        if not isdir(dir_of_new_file):
-            error(f'directory {dir_of_new_file!r} of new file {new_file!r} not found')
-        if exists(new_file) and not isfile(new_file):
-            error(f'new text file {new_file!r} exists but is not a file')
-        open(new_file, 'w').write('') # create empty new file
-        new_file_args = get_args_file(new_file)
-        if exists(new_file_args):
-            rm(new_file_args) # virtually set args of new file to default values
-        arg.swap_text_file(new_file)
-        inform(f'New: new text file {new_file!r} created')
-    else:
-        inform('New: new text file NOT created')
-
-def Open_button():
-    'browse file system and select the text file to be processed'
-    new_file = long_path(sg.PopupGetFile('', no_window=True, save_as=False))
-    # if new_file doesn't exist, error window is issued by sg.PopupGetFile() itself
-    if new_file:
-        if exists(new_file) and not isfile(new_file):
-            error('target file exists but is not a file')
-        arg.swap_text_file(new_file)
-        inform('Open: text file {new_file!r} selected')
-    else:
-        inform('Open: text file NOT selected')
-
-def Recent_button():
-    'browse list of recent files and select the text file to be processed'
-    new_file = long_path(hist.select())
-    if new_file:
-        arg.swap_text_file(new_file)
-        inform('Recent: text file {new_file!r} selected')
-    else:
-        inform('Recent: text file NOT selected')
-
-def Saveas_button():
-    'clone current text file into a copy, which becomes the new text file'
-    new_file = long_path(sg.popup_get_file('', no_window=True, save_as=True))
+    if new_text_file:
+        new_text_file = longpath(new_text_file)
+        if arg.text_file == new_text_file:
+            error(f'The new text file can not be the current text file')
+        arg.write_into_args_file_of(old_text_file) # save old arguments
+        open(new_text_file, 'w').close() # empty file…
+        rm(args_file_of(new_text_file)) # …with default arguments…
+        arg.set_default()
+        rm(log_file_of(new_text_file)) # …with no log…
+        for back_file in back_files_of(new_text_file):
+            rm(back_file) # …and no backups
+        hist.add(new_text_file)
+        cd(dirname(new_text_file))
+        arg.text_file = new_text_file
+        lock.release(old_text_file)
+
+def open_button():
+    'browse file system and select the new current text file'
+    old_text_file = arg.text_file
+    new_text_file = sg.PopupGetFile('', no_window=True, save_as=False)
+    # if new_text_file doesn't exist, error window is issued by sg.PopupGetFile() itself
+    if new_text_file:
+        new_text_file = longpath(new_text_file)
+        if arg.text_file == new_text_file:
+            error(f'The selected text file can not be the current text file')
+        arg.write_into_args_file_of(old_text_file)
+        arg.read_from_args_file_of(new_text_file) # update arguments
+        hist.add(new_text_file)
+        cd(dirname(new_text_file))
+        arg.text_file = new_text_file
+        lock.release(old_text_file)
+
+def recent_button():
+    'browse list of recent existing files and select the new current text file'
+    old_text_file = arg.text_file
+    new_text_file = hist.select()
+    # if list of recent files is empty, error window is issued by hist.select() itself
+    if new_text_file:
+        new_text_file = longpath(new_text_file)
+        if arg.text_file == new_text_file:
+            error(f'The selected text file can not be the current text file')
+        arg.write_into_args_file_of(old_text_file)
+        arg.read_from_args_file_of(new_text_file) # update arguments
+        hist.add(new_text_file)
+        cd(dirname(new_text_file))
+        arg.text_file = new_text_file
+        lock.release(old_text_file)
+
+def saveas_button():
+    'clone current text file (and its args file) into a copy, which becomes the new current text file'
+    old_text_file = arg.text_file
+    new_text_file = sg.popup_get_file('', no_window=True, save_as=True)
     # if target file aready exists, confirmation window is issued by sg.PopupGetFile() itself
-    if new_file:
-        if arg.text_file == new_file:
-            error('you cannot save a text file into itself')
-        if exists(new_file) and not isfile(new_file):
-            error('target file exists but is not a file')
-        cp(arg.text_file, new_file) # copy text file
-        text_file_args = get_args_file(arg.text_file)
-        if isfile(text_file_args):
-            new_file_args = get_args_file(new_file)
-            cp(text_file_args, new_file_args) # copy args file, if any
-        arg.swap_text_file(new_file)
-        inform(f'Saveas: {arg.text_file!r} ──▷')
-        inform(f'        {new_file!r}')
-    else:
-        inform('Saveas: target text file NOT selected')
+    if new_text_file:
+        new_text_file = longpath(new_text_file)
+        if old_text_file == new_text_file:
+            error(f'The target text file can not be the current text file')
+        arg.write_into_args_file_of(old_text_file)
+        cp(old_text_file, new_text_file) # cloned text file…
+        cp(args_file_of(old_text_file), args_file_of(new_text_file)) # …with cloned arguments…
+        rm(log_file_of(new_text_file)) # …with no log…
+        for back_file in back_files_of(new_text_file):
+            rm(back_file) # …and no backups
+        hist.add(new_text_file)
+        cd(dirname(new_text_file))
+        arg.text_file = new_text_file
+        lock.release(old_text_file)
 
-def Help_button():
+def help_button():
     'show colophon and possibly browse the YAWP User Manual'
     if ask_yes('YAWP - Help', f'''
-                        YAWP {VERSION}
-             Yet Another Word Processor
-                          2023-05-18
-             https://pypi.org/project/yawp
-                 Carlo Alessandro Verre
-         carlo.alessandro.verre@gmail.com
+                          YAWP {VERSION}
+              Yet Another Word Processor
+                           {VERSION_DATE}
+              https://pypi.org/project/yawp
+                  Carlo Alessandro Verre
+          carlo.alessandro.verre@gmail.com
 
 Do you want to browse the YAWP User Manual?''', 'browse'):
         arg.check_pdf_browser()
-        shell(f'{arg.pdf_browser} {YAWP_PDF}')
+        shell(f'{arg.pdf_browser} {MANUAL_FILE!r}')
 
-def Exit_button():
+def exit_button(return_code=0):
     'terminate execution'
-    if isfile(arg.text_file):
-        arg.close_text_file()
-        if arg.usage_mode == 'g':
-            arg.write_text_file_into_sess_file(YAWP_SESS)
-    log.close()
-    exit()
+    if var.gui_mode:
+        arg.write_into_args_file_of(arg.text_file)
+        write_sess_file(arg.text_file)
+    lock.release(lock.locked_file)
+    exit(return_code)
 
-#----- buttons, second line: Edit Format Noformat Undo Log Correct -----
+#----- buttons, second line: Edit Format NoFormat Undo Log -----
 
-def Edit_button():
+def edit_button():
     'edit current text file'
-    arg.check_text_file()
-    arg.check_text_editor()
+    inform([frame(f'Edit - {now()}')])
+    arg.check()
+    arg.inform()
+    if not isfile(arg.text_file):
+        if ask_yes(f'YAWP - Edit', f'File {arg.text_file!r} does not exist.\nDo you want to create it as an empty file?', 'create'):
+            write_lines(arg.text_file) # new file…
+            rm(args_file_of(arg.text_file)) # …with default arguments…
+            arg.set_default()
+            for back_file in back_files_of(arg.text_file):
+                rm(back_file) # …and no backups
+        else:
+            return
+    lock.seize(arg.text_file)
     old = Buffer(arg.text_file)
     old.inform('Before:')
-    shell(f'{arg.text_editor} {arg.text_file}')
+    shell(f'{arg.text_editor} {arg.text_file!r}')
     new = Buffer(arg.text_file)
     if old == new:
-        inform('Edit: text file NOT altered, backup NOT performed')
+        inform(['Backup:\n    Text file not altered, backup not performed'])
     else:
-        back_file = new_back_file(arg.text_file)
+        back_file = new_back_file_of(arg.text_file)
         old.write_into_file(back_file)
-        inform(f'Backup:  {arg.text_file!r} ──▷')
-        inform(f'         {back_file!r}')
+        inform([f'Backup:',
+            f'    {arg.text_file!r} →',
+            f'    {back_file!r}'])
         new.inform('After:')
-        inform('Edit: text file altered, backup performed')
 
-def Format_button(format=True):
-    'format current text file, and export in PDF format'
-    arg.check_text_file()
-    button = ['Noformat','Format'][format]
+def format_button(format=True):
+    'format current text file, run graphics if -g, and export and browse in PDF format following -X'
+    button = ["NoFormat","Format"][format]
+    inform([frame(f'{button} - {now()}')])
+    if format and is_reserved(arg.text_file):
+        error(f'Format of reserved file\n{arg.text_file!r}\nis not allowed.')
     arg.check()
+    arg.inform()
+    lock.seize(arg.text_file)
     old = Buffer(arg.text_file)
-    inform(f'Read:    YAWP ◁── {arg.text_file}')
-    old.compute_and_correct_sizes()
+    inform([f'Read:\n    YAWP ← {arg.text_file!r}'])
     old.inform('Before:')
+    old.compute()
     new = old.copy()
-    if format:
+    if format: # -M f?
         new.remove_page_headers()
         new.justify_lines()
     if arg.graphics: # -g ?
-        new.redraw_segments()
-        new.redraw_arrowheads()
-    if format:
+        new.redraw()
+    if format: # -M f?
         new.renumber_chapters()
-        new.add_chapters_to_contents()
-        new.add_captions_to_figures()
-        new.add_quoted_subjects_to_index()
-        new.add_unquoted_subjects_to_index()
+        new.add_chapters_to_contents_chapter()
+        new.add_captions_to_figures_chapter()
+        new.add_quoted_subjects_to_index_chapter()
+        new.add_unquoted_subjects_to_index_chapter()
         new.insert_contents_figures_and_index_chapters()
-        new.check_line_lengths()
         if arg.page_headers != 'n': # -p ?
             new.count_picture_lines()
             new.count_pages()
-            new.add_page_numbers_to_contents()
-            new.add_page_numbers_to_figures()
-            new.add_page_numbers_to_index()
+            new.add_page_numbers_to_contents_chapter()
+            new.add_page_numbers_to_figures_chapter()
+            new.add_page_numbers_to_index_chapter()
             new.insert_page_headers()
+        new.check_line_lengths()
     if (not format and not arg.graphics) or old == new:
-        inform(f'{button}: text file NOT altered, backup NOT performed')
+        inform([f'Backup:\n    text file not altered, backup not performed'])
     else:
-        back_file = new_back_file(arg.text_file)
+        back_file = new_back_file_of(arg.text_file)
         old.write_into_file(back_file)
-        inform(f'Backup:  {arg.text_file!r} ──▷')
-        inform(f'         {back_file!r}')
+        inform([f'Backup:',
+            f'    {arg.text_file!r} →',
+            f'    {back_file!r}',
+            f'Rewrite:\n    YAWP → {arg.text_file!r}'])
         new.write_into_file(arg.text_file)
-        inform(f'Rewrite: YAWP ──▷ {arg.text_file!r}')
         new.inform('After:')
-        inform(f'{button}: text file altered, backup performed')
-    if arg.export_view_pdf: # -X ?
+    if arg.export_pdf != 'n': # -p n?
         pdf.export_and_browse(arg.text_file)
 
-def Noformat_button():
-    'do not format current text file, but run graphics, and export in PDF format'
-    Format_button(format=False)
-    
-def Undo_button():
+def noformat_button():
+    'do not format current text file, but anyway run graphics if -g, and export and browse in PDF format following -X'
+    format_button(format=False)
+
+def undo_button():
     'restore current text file to its previous version'
-    arg.check_text_file(must_exist=False)
+    inform([frame(f'Undo - {now()}')])
+    arg.check()
+    arg.inform()
     try:
-        back_file = old_back_file(arg.text_file)
+        back_file = last_back_file_of(arg.text_file)
     except FileNotFoundError:
-        error(f'backup file for text file {arg.text_file!r} not found')
+        error(f'Backup file for text file {arg.text_file!r} not found')
     if not isfile(back_file):
-        error(f'backup file {back_file!r} for text file {arg.text_file!r} exists but is not a file')
+        error(f'Backup file {back_file!r} for text file {arg.text_file!r} exists but is not a file')
     if arg.usage_mode == 'u' or not isfile(arg.text_file) or ask_yes('YAWP - Undo',
-            'Current content will be lost\nDo you want restore previous content?','restore'):
+            'Current content will be lost.\nDo you want restore previous content?','restore'):
+        lock.seize(arg.text_file)
         old = Buffer(arg.text_file)
         old.inform('Before:')
         rm(arg.text_file)
         mv(back_file, arg.text_file)
-        inform(f'Restore: {arg.text_file!r} ◁──')
-        inform(f'         {back_file!r}')
+        inform([f'Restore:',
+            f'    {arg.text_file!r} ←',
+            f'    {back_file!r}'])
         new = Buffer(arg.text_file)
         if old != new:
             new.inform('After:')
-            inform('Undo: text file altered')
+            inform(['Undo:\n    Text file altered'])
         else:
-            new.compute_and_correct_sizes()
-            inform('Undo: text file NOT altered')
-        if arg.export_view_pdf: # -X ?
+            inform(['Undo:\n    Text file not altered'])
+        if arg.export_pdf != 'n':
+            new.compute()
             pdf.export_and_browse(arg.text_file)
 
-def Log_button():
+def log_button():
     'browse current log file'
     arg.check_text_editor()
-    log.browse()
-
-def Correct_button():
-    'manage correction file'
-
-    def Correct_Edit_button():
-        'edit correction file'
-        arg.check_text_editor()
-        lock.seize(YAWP_CORR)
-        old = open(YAWP_CORR).read()
-        strfile_inform(old, 'Before:')
-        shell(f'{arg.text_editor} {YAWP_CORR}')
-        new = open(YAWP_CORR).read()
-        if old == new:
-            inform('Correct - Edit:correction file NOT altered, backup NOT performed')
-        else:
-            back_file = new_back_file(YAWP_CORR)
-            open(back_file, 'w').write(old)
-            inform(f'Backup:  {YAWP_CORR!r} ──▷')
-            inform(f'         {back_file!r}')
-            strfile_inform(new, 'After:')
-            inform('Correct - Edit: correction file altered, backup performed')
-
-    def Correct_Reset_button():
-        'reset correction file to default values'
-        lock.seize(YAWP_CORR)
-        old = open(YAWP_CORR).read()
-        strfile_inform(old, 'Before:')
-        open(YAWP_CORR, 'w').write(CORRECTORS)
-        new = CORRECTORS
-        if old == new:
-            inform('Correct - Reset: correction file NOT altered, backup NOT performed')
-        else:
-            back_file = new_back_file(YAWP_CORR)
-            open(back_file, 'w').write(old)
-            inform(f'Backup:  {YAWP_CORR!r} ──▷')
-            inform(f'         {back_file!r}')
-            strfile_inform(new, 'After:')
-            inform('Correct - Reset: correction file altered, backup performed')
-    
-    def Correct_Undo_button():
-        'restore correction file to the previous version'
-        try:
-            back_file = old_back_file(YAWP_CORR)
-        except FileNotFoundError:
-            error(f'backup file for correction file not found')
-        if not isfile(back_file):
-            error(f'backup file {back_file!r} for correction file exists but is not a file')
-        if ask_yes('YAWP - Correct - Undo','Current content will be lost\nDo you want to restore previous content?','restore'):
-            lock.seize(YAWP_CORR)
-            old = open(YAWP_CORR).read()
-            strfile_inform(old, 'Before:')
-            rm(YAWP_CORR)
-            mv(back_file, YAWP_CORR)
-            inform(f'Restore: {YAWP_CORR!r} ◁──')
-            inform(f'         {back_file!r}')
-            new = open(YAWP_CORR).read()
-            if old == new:
-                inform('Correct - Undo: correction file NOT altered')
-            else:
-                strfile_inform(new, 'After:')
-                inform('Correct - Undo: correction file altered')
-    
-    layout = [[sg.Text('edit reset or restore the correction file?')],
-        [sg.Button('Edit',   size=SGBS, tooltip='edit correction file\nthrough the text editor defined by -y'),
-         sg.Button('Reset',  size=SGBS, tooltip='reset correction file\nto default values'),
-         sg.Button('Undo',   size=SGBS, tooltip='restore correction file\nto its previous content'),
-         sg.Button('Cancel', size=SGBS, tooltip='do nothing and go back')]]
-    window = sg.Window(f'YAWP - Correct', layout)
-    event, values = window.read(close=True)
-    if event and event != 'Cancel':
-        {'Edit': Correct_Edit_button,
-         'Reset': Correct_Reset_button,
-         'Undo': Correct_Undo_button}[event]()
+    if isfile(arg.text_file):
+        shell(f'{arg.text_editor} {log_file_of(arg.text_file)!r}')
+    else:
+        error('Log file not found')
 
 #----- main -----
 
 def main():
-    try:
-        var.gui = False
-        simplefilter('ignore')
-        if not exists(YAWP_CORR):
-            open(YAWP_CORR, 'w').write(CORRECTORS)
-        log.open()
-        arg.read_from_argv(argv)
-        inform(frame(YAWP_LOG))
-        if arg.usage_mode == 'g':
-            var.gui = True
-            main_window()
-        elif arg.usage_mode == 'e':
-            inform(frame(f'{"Edit":<10} {now()}'))
-            Edit_button()
-        elif arg.usage_mode == 'f':
-            inform(frame(f'{"Format":<10} {now()}'))
-            Format_button()
-        elif arg.usage_mode == 'n':
-            inform(frame(f'{"Noformat":<10} {now()}'))
-            Noformat_button()
-        else: # arg.usage_mode == 'u'
-            inform(frame(f'{"Undo":<10} {now()}'))
-            Undo_button()
-        Exit_button()
-    except KeyboardInterrupt:
-        Exit_button()
+    var.gui_mode = False
+    simplefilter('ignore')
+    if not isfile(CORR_FILE):
+        open(CORR_FILE, 'w').write(CORR_DEFAULT)
+    arg.read_from_argv(argv)
+    if arg.usage_mode == 'g':
+        var.gui_mode = True
+        gui_main_window()
+    elif arg.usage_mode == 'e':
+        edit_button()
+    elif arg.usage_mode == 'f':
+        format_button()
+    elif arg.usage_mode == 'n':
+        noformat_button()
+    else: # arg.usage_mode == 'u'
+        undo_button()
+    exit_button()
 
 if __name__ == '__main__':
     main()
 
 #----- end -----
```

### Comparing `yawp-1.0.0b10/yawp/docs/.test.pdf` & `yawp-2.0.0/yawp/docs/copy.txt.pdf`

 * *Files 24% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,5951 +1,11817 @@
-7
-
-
-
+┌───────────────────────────────────┐
 │
- │
-
+├─┐
 │
 │
-│ 
-│ 
+│ ┌───┐ │
+│ ┌───┐
+│ │
 │
 │
 │ │
 │ │
 │ │
 │
+│ │
 │
-     │ │ │  
+└─┬─┘ ├───┤ │ │ │ ├───┘
+│ │
 │
 │
 │
 │ │ │ │ │
+│ │
 │
 │
 │
-│    │
+│ └─┴─┘ │
+│ │
 │
+│ │
+│ │
 │
-   
+  
+
+
 │
-   
+│ │
+    
+│ │
 │
-2023-04-27
+
+│ │
 │
-https://pypi.org/project/yawp
+   !
 │
-  !
-│ carlo.alessandro.verre@gmail.com
+│ │
+"     # 
+│     $ %& & │ │
 │
+│ │
+└─┬─────────────────────────────────┘ │
+└───────────────────────────────────┘
 
- 
-
+I 
 
-
- 
+ & '
 
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
-│ │
- │
+'   ! $ 
+  &
 
-
+( (  ! ld
 
-I sound my barbaric yawp over the roofs of the world
+ii
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+"C  
 
-W"
+iii
+ 
+ ! 
+iii
+ 
+I   
+iii
+ 
+I   
+ 
+   
+$
+ 
+ 
+$
+ 
+
+ 
+  
+
+ 
+
+ 
+ 
+I 
+
+ 
+
+ 
+  ( 
+
+  !
+
+
+  C
+
+
+    
+
+  "
+
+
+  $
+
+
+   
+
+
+ 
+    
+
+   
+   &  
+  ( & 
+   
+
+  
+
+ 
+C  
+   
+   
+I I ( &         
+ 
+
+ 
+"I 
+
+ 
+" 
+
+ 
+$ 
+ 
+
+ 
+
+   
+
+ 
+ &  
+
+  
+( & 
+
+     
+
+ 
+"I I ( &      
+
+ 
+   
+ &
+
+ 
+  
+
+ 
+
+ 
+"  
+& " 
+
+ 
+&'  "  
+
+ 
+
+ 
+&  "  
+
+ 
+"   " 
+
+ 
+I  " 
+
+ 
+  " 
+ 
+
+ 
+ 
+
+ 
+   
+
+ 
+   & 
+
+ 
+
+ 
+ 
+& 
+
+ 
+  
+
+ 
+  
+
+ 
+  
+
+ 
+ $ 
+
+ 
+
+ 
+    
+  
+
+ 
+   
+
+ 
+"    "  
+
+ 
+ &  
+ &  
+
+ 
+     
+    
+
+  
+   
+
+  
+
+ 
+&
+ 
+
+ 
+&
+   
+
+ 
+( ! 
+
+ 
+#  
+
+ 
+&  
+
+ 
+
+
+ 
+" 
+& &
+
+ 
+
+  
+  &
+ 
+
+  
+
+ 
+"  
+
+ 
+"  
+
+
+ 
+
+
+I 
 
-ii/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-CONTENTS
-• 1.
-Forewords
-• 1.1.
-Introduction
-• 1.2.
-Installation
-• 1.3.
-Glossary
-• 2.
-Usage Modes
-• 2.1.
-"GUI" Mode
-• 2.1.1.
-Text File Selection
-• 2.1.1.1. New Button
-• 2.1.1.2. Open Button
-• 2.1.1.3. Recent Button
-• 2.1.1.4. Saveas Button
-• 2.1.2.
-Correct Button
-• 2.1.3.
-Help Button
-• 2.1.4.
-Exit Button
+  ! 
 
-
+iii
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+ C C
 
- W W
-
-• 2.1.5.1. Edit Button
-• 2.1.5.2. Format Button
-• 2.1.5.3. Noformat Button
-• 2.1.5.4. Undo Button
-• 2.1.6.
-Log Button
-• 2.2.
-"CLI" Modes
-• 2.2.1.
-Edit Mode
-• 2.2.2.
-Format Mode
-• 2.2.3.
-Noformat Mode
-• 2.2.4.
-Undo Mode
-• 3.
-Justification
-
- 
- 
-
-• 4.
-• 4.1.
-• 4.2.
+
 
+ I  C "IC
+
+
+  & 
+     ,
+        (  
+   !    (    (, !     I(      
+  (   ( ( (  I  !     ' C((   ,    (
+& s    (   & , $
+ 
+ (    !       ( 
+  
+Y &  ( 
+
+
+
+
+
+  
+I   ( , '   '   "I &&  
+     
+     (,   ( (   &  
+ (
+!      (     
+ Y (   
+  
+  '(  !     (    & & '  , !     
+   (   (
+   
+      
+ &     
+      
+        $ '      (  '  &   ,  '
+&&     &'  
+ 
+
+ (     &,  '
+   & (    &
+! 
+ &'   (   
+   ( &
+&  & $
+   
+& 
+"        (
+    $   ' s  ' Y Y
+   
+&  I    
+  (
+   ( &
+&  & $  &'   ( (    
+   
+& 
+       (
+      (   , '     !      , !   
+&'     
+    (    &  &'   
+     &     ',      !    
+
+$   &  ' YvY
+  ! & '   '  
+
+!  ' YY ,
+    
+      (    ( & , !    $ 
+ 
+     ,
+   ' !       (, !   $!
+    
+     ,            , !        (,
+ s     $ '
+  !   ( & 
+   &    & 
+    ( (   (
+
+          &  ' "  '  (      &  ,  
+(      (  & '
+  (
+    ( !    ,     $   (   ' 
+       
+   I & 
+   &  ( (    (
+   I &  $  & (       (
+     
+ $ 
+   I &  $  (   &      (, &  ! 
+        (
+   
+      & ( !   &  & , 
+ ( (
+ (    
+    (    &        
+  
+
 
 
-
+
 
-W"
- W
-
-Chapters
-Nameless Chapter
-Numbered Chapters
+ & ( "I
 
-"W  
+ , 
 
-iii
-iii
-iii
-iv
-1
-1
-2
-2
-3
-3
-4
-4
-5
-5
+ 
 
-
+   '    
 
-5
-5
-5
-6
-6
-6
-6
-6
-6
-6
-7
+Y   
 
-
-
-9
-9
-9
+(Y
 
-
+( &   (
+Y   
 
-• 4.3.1.
-• 4.3.2.
-• 4.3.3.
-
-Contents Chapter
-Index Chapter
-Figures Chapter
+Y
 
-10
-11
-12
+'     & 
+ !  ( $ !    
 
-• 6.
+│
 
-Graphics
+! 
 
-15
+    & Y   
 
-• 8.
+Y
 
-Reserved Files
+ &  & 
 
-20
+  "I  &  &
+  (
+ $ !  &        ( '     & 
+ !          
+             ( ,    '  
+ '(  $   
+ &'  ' &
+&' 
+   (  (  
+        ( & 
+  &  ( &      
+  &    $     &
+Y   (   
+ Y   
+ I   IC
+I( 
 
- 
- 
+  '    '
+│
 
- 
- 
-  
- 
-  
-  
-  
-  
- 
-
-• 9.1.
-• 9.2.
-• 9.3.
-• 9.4.
-
-  
-• 10.
-• 11.
-•
-•
+C
 
-W
+( &,    & 
 
-
+      ! 
 
- W
+  ( &  !
+│
+│
+│
+│
+│
 
-W  W W
-   W W
-W  W W
-   W
-"  " W
-   W
- W  "  W
-    W
-
+$   
 
-
+      $  ( 
 
-
+  (      , (
 
-
-
-
-
+ 
 
-
-
-
-
+
 
-Versions
-Credits
-Homonyms
-License
-
-27
-27
-27
-28
-
-Unicode Characters
-Cheat Sheet
-Figures
-Index
-
-29
-30
-31
-32
+   &    
+  " C   &
+  &          
+    
+     
+   &
+ 
+ 
+  
+      
+  C   
 
-"
+ 
 
-
+$
 
-1. Forewords
-iii/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-1 1
+
 
-1.1. INTRODUCTION
+
 
-"  "     
-W  n  Wn  
- W  W W    f         n 
-f l
-   W1 W W
-W  for you. But if you just want to create a draft or
-a simple quick-and-dirty no-frills document as thi  Ws
- 
-"
+    
+     !
 
-Y "W
-
-
+│
+│
 
-file"
+! 
+ 
 
- 
-  lf W       f command too
- W   W W  We, hereinafter referred to simply as the "text
+   &
 
-  WW   W   Wmestamped backup, allowing Undo operation
-W W      W W
+
+ 
 
-
-
+, 
 
-• unindented paragraphs
-• dot-marked indented paragraphs (as this one)
-W WW W Ws    in the text file and by arguments only, not by
-
-commands or tags embedded in text
-  W W
-
-W  "s, tables and code examples) freely intermixed
-with text
- " "W "Wns "W of chapters and inserts an automatic Contents
-
-chapter in the text file
-W s    '"') and inserts an automatic Index chapter in
-
-the text file
- " "W "Wns "Wng of figure captions and inserts an automatic
-
-Figures chapter in the text file
-   W W   WW wo-lines page headers, allowing page numbering
-
-control and insertion of initial Roman-Numbered pages
-  "  W
-  n sketch pictures with horizontal and vertical
-
-segments (by '`') and arrowheads (by '^'), Y
- "  W W  W
-characters
-    W W  " Wh control over character size and page layout,
-
-       W Wng preview and printing
-
-W lf " s     ile and restores it at next invocation
-
-   WW "     file
-
-W lf " s  W    " cent processed text files and allows to select
-one at next invocation
-W    "   n  about font size and page margins, you can use
-
-default corrections or redefine them by a correction file
-W "  W  "Wl and into a timestamped session log file
-
+  ,
 
- 
+
 
-
+ 
 
-W  
+ I"0 
+ 
 
- W   sW W    
+,   (
 
-executions
-• yawp is stable, if after a yawp execution you run yawp again on the same file with the same
-arguments, the text file content does not change
+  
 
-
+
+
 
-W
-
- 
+│
 
-typing:
+  
 
-     W"   W   W 
- 
+  
 
-"  
+  
 
-f
+ 
 
- W
+ 
 
- 
+   !
 
-  W 
+$  
 
- nual has been created as yawp.pdf from yawp.txt by
+
+   Y  
 
-│ $ yawp -M f -v -w 90 -p c -n -5 -E 'yawp 1.0.0b7 User Manual' -X -L 2.5cm yawp.txt
-where arguments mean:
+      
 
- n
+
 
- 
+        
+   "      
+  I &
+  
+ !
 
-W f " "
+│
 
-• -v: write information messages not only into log file but also on terminal
-• -w 90: set 90 characters per line
-• -p c: insert a page header on page full, on picture break and before level-1 chapters
-• -n -5: first five pages are Numbered by Roman numbers
-• -E 'yawp 1.0.0b7 User Manual': set the title to the right of even page headers
+ '
 
- n    sW W
+  
 
-
+ & 
 
-"
+ 
 
-• -L 2.5cm: set left margins on odd pages and right margins on even pages to 2.5 cm
-• yawp.txt: this is the text file to be processed
+'  
 
-Other examples are scattered below.
+ C
+I
 
-f   f1
-In the following we assume that your Linux belongs to the Debian family. Type at terminal:
-│ $ sudo apt-get update
-│ $ sudo apt-get purge printer-driver-cups-pdf
-│ $ sudo apt-get install printer-driver-cups-pdf IDLE python3-pip
-│ $ pip3 install yawp
- Y 
- WY
-
-│
-
-Imagine your user name is 'xxxx'. If you see a message like this:
+
 
-fl  W 
+  &  (
+ & '  
+ !
+&& &  
 
-W W W Y " 
+
 
- WY W W  
+  
 
-
+ &
 
-you can fix the problem by typing:
-│
+ '
 
- Y 
+  YiY '
 
- " 
+        '
+         ' 
+i !
+ s   ( '     
+  '   &
+  
+Y
 
- WY
+ 
 
-me/xxxx/.bashrc
+(
 
-The 'sudo apt-get purge printer-driver-cups-pdf' command is recommended because on some Linux
-systems (as MX) printer-driver-cups-pdf is pre-installed but it doesn't seem to work out of the box,
-while it works if it is uninstalled and reinstalled.
-Now you can close the terminal, open another one,  
+
 
-  W
+
 
-iv/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ $ yawp -H # show a help message and exit
-│ $ yawp -V # show program's version number and exit
-   Wt
-│ $ yawp -H [-Y pdf_   
-
-│ $ yawp text_ W  
-W lf "  WW  W o arguments
-│
-  
-W lf "  W " evious session, no arguments
-│ $ yawp -M e [-y text_editor] text_ W  
-W f W "
-│ $ yawp -M f [...arguments...] text_ W  
-W f " "
-│ $ yawp -M n [...arguments...] text_ W  
-W f  " "
-│ $ yawp -M u [...arguments...] text_ W  
-W f  "
-Later you can type:
-│ $ pip3 install --upgrade yawp
+ 
 
-W    
- l1
+&$,
 
-   sW
+
 
-
+Y → Y  (Y
 
-Some terms here have a different meaning from that commonly in use.
-To "shrink" a character string means:
-• to strip away all leading and trailing blanks, and
-• to reduce each internal group of consecutive blanks to a single blank
-For instance, the string:
+         '
+  i !  !  &  (  '     
+          , !  !       &        
+(
+  I    &,  !  Y Y     '        
+  YY
+Y  (Y → Y  Y
+       '  i ! ,   !  &  (  '   
+ 
+   
+ ,  (    
+   
+  &      
+     &   , !  !       &         (
+   &
+Y  (Y → Y  (Y
+  
+    ' s $  i ( ! ' 
+!  
+ &,  !    s $  i
+'&   & 
+ 
 
 Y
+'
 
- 
+ '   , !
 
-
+
 
-""
+i
 
-Y
+
 
-if shrunk, becomes:
+(
 
-Y   ""Y
-To "uppercase" a character string means to uppercase all characters in it, except characters quoted
-by double quote '"', which remain unchanged.
-For instance, the string:
+Y  Y 
 
-Y   ""Y
-if uppercased, becomes:
+(
 
 Y
 
- ""Y
+  i, '& Y  Y
 
-To "titlecase" a character string means to uppercase the first character of each word in it, and to
-lowercase all the others, except the characters quoted by double quote '"', which remain unchanged.
-For instance, the string:
+i
 
-Y   ""Y
-if titlecased, becomes:
+
 
-Y   ""Y
-Two strings
-the strings:
+  i 
 
-  Y
-y = '
+  
 
-are said to be "equivalent" if, shrunk and uppercased, they become equal. For instance
+1
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
- 
+  
 
-
+   C 
+(     , 
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
 
-aaa
+
 
-""
-BBB
+ & 
 
-Y
+
 
-"cCc"'
+,    
 
-are equivalent because:
+ ! 
+ !
+ &   
+&'
+ ! #
+ !   &Y $ 
+ 
+
+ !    &   ' !     
+ 
+  I &,   (,  
+ ! _( 
+ & 
+  I &,  ( ( &  $   ,   & 
+ !
+
+  "I " &
+ !     &  _(  _( 
+  "I $ &
+ !  &   &  _(  _( 
+  "I  &
+ !     &  _(
+
+  "I  &
+
+ !     &  _(
+  "I  &  &
+
+ !  (   &  _(
+  "I ( & &
+
+ ! 
+  &  _(
+  "I   &
+ ! 
+  &  _(
+
+   I $    
 
- Wuu  Y
+
+  I &
+   ' $
+
+
+
+
+
 
- ""Y   se(shrink(y))
+  
 
-Other terms will be explained when they will be used.
+  "I &,
 
-2. Usage Modes
-1/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
 
- l
+  
 
-1
+ & 
 
-General behaviour is controlled by the following arguments:
-• "-h, --help": show a help message and exit
+ 
 
- "n nnsWn"" sW 
+i
 
-n
+ & 
 
-   W
+    '  (! 
 
-
+ ,   !
+ &   
+# , $   !   &Y $ 
+&'
+ 
+ , ' !&
+  ' !        
+
+ 
+$ , $ '  !   ( &  &      "I &  
+ ,   & 
+     & (  YYdI, YYd"I ", Y&Yd"I
+$, YYd"I , YYd"I , Y(Yd"I  & , Y Yd"I ( &, Y Yd"I  
+
+  
+  
+(  
+   
+
+ &     _(, !      (    I 
+I &, &     "I &       '  
+ $   ,
+       YY    &&  '   &     (
+"II   , 
+        
+$ & 
+
+& 
+
+s   (  , 
+ ( 
+ '    &     ( 
+ 
+$   !  &,       &  
+
+  
 
-• "-V, --version": show program's version number and exit
-• "-v, --verbose": write all messages on stderr (default: write errors only)
- "n nnn"" 
-W W  " (default: 'g' = GUI, 'e' = CLI Edit, 'f' = CLI
-Format, 'n' = CLI Noformat, 'U' = CLI Undo) The -y argument defines the text editor to be
-used:
-
-    n W  W  n
-
-
-
- .).
-
-Usage modes defined by -M are five:
-• one GUI mode, the default one (see 2.2.)
-• four CLI modes:
-• Edit mode (-M e, see 2.1.1.)
-• Format mode (-M f, see 2.1.2.)
-• Noformat mode (-M n, see 2.1.3.)
-• Undo mode (-M u, see 2.1.4.)
-In all usage modes, after processing the text fi      sW W
--X argument (see 7.).
+   (
 
-
+ &   _( 
 
-"  
+s    " & 
 
-W
-is the positional argument text_file, which indicates the text file to be processe
-(absolute or relative to current directory) W  W
-Y Y W W "" 
- "  W  W
-ff rs, or any other Unicode UTF8-encoded character.
-Last
-path
+
 
-
-W  ted by line terminators. The text file is read in
-W W   
-"universal newlines" mode, so three line terminators are accepted:
- "W "  YY WnWn
+
 
-u
+   ( Y Y    
+ 
+ 
+  
+Y Y    C  C
+ 
+  
+   ( Y  Y   !
+   ( 
 
-• "carriage return" + "line feed" = '\r\n' (Micros n Wu
-  1 n1 X)
- "W "  YY 
+!  ,     &  
 
-  
+!  Y Y
 
-W W W  W "Wor is always '\n'.
+   IC
+ 
+ & 
 
-   W  
+  ,  
 
-   can choose your preferred ones. To define the text
+ 
 
-editor, set the argument:
+ (     (     ,  
 
-• "-y, --text-editor": editor for text files (default: 'idle')
-Such an editor is used:
-• to edit the text file by the Edit button
-• to edit the correction file by Correct button
-• to browse the session log file by Log button
-If you use
-clicking:
+  ,    (  ( (
+ 
 
-IDLE,
+
 
-the
+
 
-default
+ Y! Y
 
- Configure IDLE
+
 
-Options
+     ( ' I  '  ,  ' "I  &
+  ' !   ( (      ( ' I  ' 
+   & ' ! &&  
+    ( $       , ' 
+  ,    $ $& & 
+   $   ''       ,
+     ,   
+'       ' &   &  '! !  
+│
 
-  W 
+ ! 
 
- Shell/Ed
+       ! 
 
- Show line numbers in new windows
+   !
 
-    "
+! 
 
- "n  nn  n" 
- 
+    !    ! !, ' 
 
-text editor, you can view the line numbers at left of the text by
+  ! ! ! !   '  
 
-
+0!  ! 
+   
 
-
+ '    Y  $  ( &   ( !,
+ ('   
 
-W  ult: 'xdg-open')
+  
 
-  W 
+ (  ,
 
-    
-   W
+I(     ! ,  (  &         (  
+      (       , 
 
-W    "  "at and Undo buttons
-    
+   
 
-The default value 'xdg-open'
-further details, type:
+  
+ " (  0 
+   
+   
+    #    
+    
+      
+ C0
+  $
+ "
+I
 
-causes you view t
+     ! Y   , 
+ 
+  
+ &  
+!   ! 
 
-
+" 
+
+" (C
+
+   (( 
 
-W   "  
+
 
-  
+    ( 
 
-│ $ man xdg-open
-2.1. "GUI" MODE
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+             (
+   ( & "       ( &  
+ "      ((     
+
+
+
+I
 
-W W lf " W 
+  
 
-   
+
 
-Y f " f lf "  _file
+C 
 
-argument is optional and the other arguments are not allowed.
+
+I & 
+
+  
+  (    '!
+ "I & I
+ &       
+ &    !
+_(
+│
 │
-If
 
-
+ 
+ 
 
-"    
+ ! _( 
+ !
+
 
-text_file
+I & 
 
-W lf " W explicit text_file argument
+I &,   (,  
+ & 
+I &,  ( ( &  $   , 
+ & 
 
-is not given, path and name of the text file to be processed are read from a reserved
-WW   sW
-Y ecution.
+& (   (       ( & 
+I( _(   $ ,   
+(, ! 
+   (  $  Y    I(  
+(   ( ,   ( 
+    ( 
+I(   ( 
+, '   !
+ 
+ 
+ & 
+(   ( ,
 
-W W 
-│
+(        '   ,    $ 
+      's     ,
+&   &   ( &
+
 
-
+   ( &   $ (,   !   ( I(  
+ &      (  $  
 
- 
+   '  
 
-W lf " W _file inherited from the previous session
+
 
-Then the other arguments are read from another reserved file, associated with the text file (if such
-a file is not found, arguments silently get their default values).
-For further details about reserved files, see chapter 8.
-Then the Main window appears.
+(
 
-2/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
 
-
+
 
-│
+
 
-
+! !
 
-
+
+
+ &  (,  
+
+
+
+ 
 
-n W
+
 
+┌───┬─────────────────────────────────────────────────────────────────────────────────┬───┬───┐
+│ _ │  │
+│
+│
+  
+├───┴─────────────────────────────────────────────────────────────────────────────────┴───┴───┤
+│  & 
+ 
+ (  
+ │
+! 
+!     
+    
+│
+│
+│
+              (      │
 │
+│ "       "  
+  
+I 
+( ( 
+    (  
+│
+│
+ 
+│
+│
+&   (( 
+        (           '
+│  
+│
+│
+│
+ $ (
+ $  
+
+(
+│
+│
+ (
+C  
+
+
+  ((
+
+    
+│
+│
+│
+│
+   
+   '         
+  (
+      ' !
+"      (   ( │
+│  
+│
+│
+ (' !
+ ((
+ 
+( (
+  !
+
+   
+
+│
+│
+ 
+
+   
+
+│
+│
+│
+│
+ (& 
+&
+  & 
+&
+ & 
+&
+ '&& 
+&
+│
+│
+│
+│
+I &  
+       
+ & 
+
+│    │
+│┌────┐┌─────┐┌──────┐┌─────┐┌─────┐┌──────┐┌─────┐┌──────┐┌──────┐┌─────┐┌────┐┌─────┐┌─────┐│
+││ ! ││C ││  ││" ││ $ ││  ││ ││ & ││ ( &││  ││ ││ ││ ││
+│└────┘└─────┘└──────┘└─────┘└─────┘└──────┘└─────┘└──────┘└──────┘└─────┘└────┘└─────┘└─────┘│
+└─────────────────────────────────────────────────────────────────────────────────────────────┘
+
+   
+
+
+ ! 
+
+( 
+
+ &  #  
+
+ ! !    
+    ! 
+ & , (  
+'
+ '
+ &    
+  ,   '   ((, '    
+  (( ' ( 
+  ' 
+ &      "  I
+ (
+ &      
+  !  
+  _(
+   (  
+
+ &  
+'   ' !
+C   "  $ '  ,    '  ' 
+  !   '  ,       
+
+   ( &
+  ( (  
+! &  (
+ !   
+   (
+ C  ' !  ( &  
+   (
+   ' !   (   (  
+ "       ( !   &  (
+ $ &$      ( !   &    '   (
+   ( !   &    '   (
+    
+  (   
+        ( '    (  ' 
+   (   !         
+  &  ( &   
+ ( &  Y ( &      ( '   !         
+          (    $         
+  ' !   ( (     ( '    (  ' 
+   
+  
+
+ '    ' ! (  ' 
+  ' ! 
+  s  
+      
+   !$     
+     (  (  ' 
+   ,   s    YY
+  , !   (    s 
+  
+!
+ '  
+' 
+  ' ,  ( & 
+s  '  
+  !
+
 
-
+   
+
 
-
+
 
-
+
 
-
+
 
-
+!  &  
 
-
+( 
 
-
+' 
+
+
+
+I & ' '
+
+ 
+
+ , 
+
+    !
+
+  , !  & 
+
+
+
+
+
+  
+
+3
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-│ _ │ x │
+ &$ ! ! ( , ( !  '  ', ' !  ' ( '
+ ! (   
+(  & ,    $  
+ ! (   
+'
+ & ,     '    
+ ((
+ ! (   
+ '  ,     '  
+ 
+ 
+ '  ((
+ ! (   
+ '  ,     '       
+   
+ !  !    ( & ,  
+
+  I I IIC
+
+
+
+
+C
+
+"  
+
+! &  (
+
+    ( &               (, ' !  ( &
+   $ '   (   !  (
+  ! ( & 
+ &   , '  (     
+  (  ( & 
+ 
+  ! (  Y '      (
+ &   ' 
+ &$
+ 
+ &  
+ '   ( (
+
+& ( ! ( 
+  !  (     
+ & 
+  !  ( '&      (
+  !    "  '    '  !   
+ 
 
-│ -v --verbose
+
+
+┌───┬─────────────────────────────────┬───┬───┬───┐
 │
-│ -y --text-editor
-[idle............] -g --graphics
 │
-│ -w --chars-per-line [0...............] -l --just-left-only
+│ _ │  │  │
+ $ 
+├───┴─────────────────────────────────┴───┴───┴───┤
+│    
+ │
 │
-│ -c --contents-title [Contents........] -i --index-title
-[index...........] │
-│ -f --figures-title [figures.........] -F --caption-prefix [figure..........] │
-n=no  f=fullpage  p=picture  c=chapter
-│
-│ -p --page-headers
-│ -e --even-left
-[%n/%N...........] -E --even-right
-[%F %Y-%m-%d.....] │
-│ -o --odd-left
-[%c..............] -O --odd-right
-[%n/%N...........] │
-│ -n --page-offset
-[0...............] -a --all-pages-E-e
-│
-│ -X --export-pdf
-│
-│ n nn  n
-[%f.pdf........] │
-n 
-n nn W-pdf
-│ n nnnW
-[3/5.............] │
-
-n nn-aspect
 │
-│ n nn  nW
-n nnscape
-│ -L --left-margin
-[2cm.............] -R --right-margin
-[2cm.............] │
-│ -T --top-margin
-[2cm.............] -B --bottom-margin [2cm.............] │
-│ -C --correct-sizes
-d=default  f=file
+│  
 │
- n=no
+│  sss
 │
--K --fake-margins
 │
-......................................................... │
-│ text_file
- 
- 
- 
- 
- 
- │
-│ 
-│ │
-New
-│ │
-Open
-│ │ Recent │ │ Saveas │ │
-Help
-│ │
-Exit
-│ │
-│ 
- 
- 
- 
- 
- 
- │
- 
- 
- 
- 
- 
- │
-│ 
+│ 
+│
+│
+
+│  │
+│
+┌────────┤
+&  │  $ │
+│ 
+│
+├────────┤
+ 
+ii,i  │ "  │
+│  ( 
+└────────────────────────────────────────┴────────┘
+
+   !
+
+
+
+ ,
+
+! 
+
+(   !
+
+┌───┬─────────────────────────────────────┬───┬───┐
+│
+│
+│  │  │
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│
+│    
+│   !   $ !  
+│
+│ ┌────────────┐┌────────────┐
+│
+
 │ │
-Edit
-│ │ Format │ │ Noformat │ │
-Undo
-│ │
-Log
-│ │ Correct │ │
- 
- 
- 
- 
- 
- │
-│ 
+││
+│
+│
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-
+
+ C
 
-
+ ' !
 
- W W
+ , C$ !   " ( &   !
 
-W
-The Main window contains:
+C
 
-• 16 lines, containing a subset of CLI arguments, of three types:
-• "boolean arguments" (-v -g -l -a -X and -Z), all turned off by default
-• "radio button arguments" (-p and -C)
-• "field arguments" (all the others), they can never be null, if they are set to null string
-by the user, they are automatically reset to their default value
-• 1 line, containing the current text_file argument as a read-only field, it can be changed by
-New Open Recent and Saveas buttons
-• 2 lines, containing 12 "action buttons", each corresponding to an action:
-• 4 buttons dedicated to the selection of the text file:
-• New button: create a new empty text file
-• Open button: browse the file system to select the text file
-• Recent button: browse the list of recent files to select the text file
-• Saveas button: clone current text file into a new target text file
-
- 
-
-  
-
-  
-
-   W  n
-
-• Exit button: save current text file with its arguments and finish
-• 4 buttons dedicated to the processing of the text file:
-• Edit button: edit the text file through the text editor defined by -y
-• Format button: process the text file by formatting it
-• Noformat button: process the text file without formatting it
-• Undo button: restore the text file to its previous content
-• Log button: browse the log file through the text editor defined by -y
-• Correct button: manage the correction file (Edit Reset or Undo)
-By touching a field or a button with the mouse cursor, the associated help tooltip will appear.
-
-   
-
-W lf "   , without mouse:
-
-• move window's focus, forward by Tab key, backward by Shift+Tab key
-• when focus is on a boolean argument, press Space bar to toggle it on and off
-• when focus is on a radio button, press Space bar to turn it on and turn all its siblings off
-• when focus is on an action button, press Space bar to trigger the associated action
-In case of error an error window will appear, click the 'OK' button to close and go back.
+!  ( &  
 
-
+   (
 
+    ( &               (, ' !  ( &
+  (
+  C '   
+   (  Y '      (  &   ' 
+   (
+   ( '&  ! 
+  !    "  '    '  !   
+ 
+┌───┬─────────────────────────────────┬───┬───┬───┐
+│
 │
+│ _ │  │  │
+C
+├───┴─────────────────────────────────┴───┴───┴───┤
+│    
+ │
+│
+│
+│  
+│
+│  sss
+│
+│
+│ 
+│
+│
+
+│  │
+│
+┌────────┤
+&  │ C │
+│ 
+│
+├────────┤
+  ii,i
+│  ( 
+ │ "  │
+└────────────────────────────────────────┴────────┘
 
-
+
+
 
-
+" 
 
-n
+   C
 
-│
+ ,    ow
 
-
+C
 
-n 
+!   (
 
-
+  (  
 
-
+   (
 
-
+ $!   ( &      ( &  ,  &      
+  (:
+  ( '   
+   (  Y '      (  &   ' 
+   (
+   ( '&  ! 
+  !   " '     (  ( &    (   (
 
-
+
 
-
+4
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+  !    "  ' 
 
-│ _ │ x │
+  '  !   
 
-│ ............................................ │
-
-│ 
+   ( 
+   ( 
+ '  
+       (    (,  
+
+ 
+
+( 
+
+  '    (
+
+┌───┬─────────────────────────────────────┬───┬───┐
+│ _ │  │
 │
-│ │
-OK
 │
+   
+├───┴─────────────────────────────────────┴───┴───┤
 │
-│ 
+┌──────────────────────┐
 │
-
+│
+│  │ &   │
+│
+└──────────────────────┘
+│
+│
+┌──────────────────────────────────────────┐ │
+│  │ &  
+'''' │ │
+│
+└──────────────────────────────────────────┘ │
+│
+┌────────────────────────────────┐
+│
+│
+│  │ &  ssss
+ │
+│
+└────────────────────────────────┘
+│
+│ ┌────────────┐┌────────────┐
+│
+││
+│
+│
+│ │
+"
+" 
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-
+   
 
-
+ 
 
-W
+ ,  
 
-
+ndow
 
-
+┌───┬─────────────────────────────────────┬───┬───┐
+│ _ │  │
+│
+│
+   
+├───┴─────────────────────────────────────┴───┴───┤
+│   (   ( ! ' 
+│
+│
+│   !   
+ 
+│ ┌────────────┐┌────────────┐
+│
+│ │
+││
+│
+│
+
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-W
+  '  
+ "C
 
-2.1.1. TEXT FILE SELECTION
+" ( & 
 
-
+ !
 
-1
+C
+   (  
 
-• create a new empty text file, with default argument set
-• if new text file already exists, ask for confirmation
-• the new text file becomes the current text file
-
-2. Usage Modes
-3/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+"  
 
-
+ , "
 
-
+! 
 
-
+  (
 
-
+   ( &     ' 
+  
+   (, ' !  ( & 
+    ( &           
+   $ '       (:
+    ( &   &   , '  (     
+  (  ( & 
+ 
+  ! (  Y '      (  &   ' 
+      (      (
+ 
+ &  ( (     (  
+ &  ( (    (
+       (    $ (    
+     ( '&  !     (, !   (   '  
+(
+  !    "  '    '  !     
+
+
+I    (   ( &    (
 
+  
+
+┌───┬─────────────────────────────────┬───┬───┬───┐
+│
+│
+│ _ │  │  │
+ $ 
+├───┴─────────────────────────────────┴───┴───┴───┤
+│    
+ │
+│
+│
+│
+│  
+│  sss
+│
 │
+│ 
+│
+│
+
+│  │
+│
+┌────────┤
+│ 
+&  │  $ │
+│
+├────────┤
+ 
+ii,i  │ "  │
+│  ( 
+└────────────────────────────────────────┴────────┘
+
+    "
+
+ ,   
+
+( 
 
-s
+ !
 
+┌───┬─────────────────────────────────────┬───┬───┐
+│
+│
+│  │  │
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│
+│    
+│   !   $ !  
+│
+│ ┌────────────┐┌────────────┐
+│
+
+│ │
+││
+│
 │
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-
+  ' "
+
 
-
+C#
 
-
+$ 
 
-
+   (  
 
-
+  
 
-
+ , C$ !   " ( & 
 
-
+C
+! 
 
-
+  (:
 
-
+   ( &  
+
+
+
+ ' 
 
-│ _ │
+ !
 
-│ x │
+  
 
-│ Directory: [...........................] [] │
+5
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+    ( &               (, ' !  ( &
+
+   $ '       (:
+    ( &   &   , (     
+  (  ( & 
+ 
+  ! (  Y '      (
+ &   ' 
+ &$     (     (
+   (    &  
+ &$
+ &  
+ '   ( ( 
+ '  
+( (    (, (     $ ! 
+   (    &  
+   
+ '   (    
+     ( '&  !     (
+  !    "  '    '  !   
+ 
+
+
+
+I    (   ( &  &$  (
+
+
+
+ &$
+
+┌───┬─────────────────────────────────┬───┬───┬───┐
 │
 │
+│ _ │  │  │
+ $ 
+├───┴─────────────────────────────────┴───┴───┴───┤
+│    
+ │
 │
-ppp
 │
+│  
 │
-qqq
 │
+│  sss
 │
-rrr
+│ 
 │
 │
-.....
+
+│  │
 │
-│  ......................................... │
+┌────────┤
+│ 
+&  │  $ │
 │
-
-
-│ File name: [......................] │ Save │
-
+├────────┤
+ 
+ii,i  │ "  │
+│  ( 
+└────────────────────────────────────────┴────────┘
+
+
+
+   $
+
+ , 
+
+ 
+
+(   !
+
+┌───┬─────────────────────────────────────┬───┬───┐
 │
-
- W 
-│ W   
- u] │ Cancel │
+│
+│  │  │
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│    
+│
+│
+│   !   $ !  
+│ ┌────────────┐┌────────────┐
+│
+
+│ │
+││
+│
+│
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-
+
+ 
+ &
 
-
+
 
-
+ '
+
+$
+
+ , C$ !   " ( &   !
+
+C
 
-W
+     ( !  
 
-Figure 2.1.1.1.a. New Button, New File Definition
+  (
 
+      ( &   &   , '  (    &   ' 
+  (  ( & 
+ 
+       ( ( 
+    &   
+ '   (
+       (  ( 
+ I  
+( $ 
 
 
-
+
 
-
+ 
 
-
+
 
-
+ '
 
-
+ ,   (
 
-
+I    (   ( &    (
 
-
+ 
 
-
+ $ (
 
-
+ 
 
-│
+  
 
+┌───┬─────────────────────────────────────┬───┬───┐
+  
+│ _ │  │
 │
-
 │
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│ ! '  &   
+│
+│
+│ !     (
+│   !    
+│
+│ ┌────────────┐┌────────────┐
+│
+││
+│
+│
+│ │
+
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
+
+
 
-│ x │
+   
 
-│ File ....................... already exists. │
-│ Do you want to overwrite it?
+
+
+ ,
+
+ " ( &   !
+
+  I  C"I 
+  I
+  
+
+C
+   ( '    (  ' 
+
+      ( & 
+ &   
+ (  ,  &   ' 
+
+&  ( ! ( 
+ (    ,      (  ( & 
+ & 
+       ( '    (  ' 
+ (   (   '  , '            & &  
+
+
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌───┬─────────────────────────────────────┬───┬───┐
+│ _ │  │
 │
-│ 
 │
- 
-
-│ │
-Yes
+  
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│
+│   
+& (
+│   !       
+│
+│ ┌────────────┐┌────────────┐
+│
+
 │ │
-No
+││
 │
 │
- 
-
-│ 
+
+│ └────────────┘└────────────┘
 │
+└─────────────────────────────────────────────────┘
 
-
+    
+ C
 
-
+ C
+
+ &   
+
+   (
+
+
+
+
+
+!
+
+ , "  
+
+
+
+
+" ( & 
+
+ 
+
+ !
+
+    
+
+   (    &  
+  
+     (, &       
+       ' YY   ,     ' ( ' 
+    ! 
+  Y 'Y, Y Y  Y Y
+     ' 
+ ( &    (   
+ &$          (
+&     "   I    
+  (    
+ (    Y Y,     (   , '     !      ,
+!   
+&'          (    &  &'     
+  ( &
+&  & $  &'   (   
+ ( (  
+&  "        (  
+   $   '  ( (  
+&  I     
+ (  
+  ( & &  & $  &'   ( (      ( (  
+&         (  
+ (    ,  !      $   &  
+!  '   '  
+      
+ (   Y Y,     (     
+ 
+ (    '
+  $   $     (   (  
+& & '   (  
+ !    (
+ (   Y Y
+     (      (  
+ (  d Y'Y
+ ' !    ( '    ' ! (  ' 
+
+
+CC
+
+ Y ( &  
+
+C
+   ( '  
+
+!
+
+
+
+  
+
+    
+
+   (    &  
+  
+     (, &       
+       ' YY   ,     ' ( ' 
+   ! 
+  Y 'Y, Y Y  Y Y
+     ' 
+   ( &    (   
+ (    ,  !      $   &  
+!  '   '  
+      
+ (   Y Y,    (  (     
+  '   $   on:
+ (    '
+  $   $     (   (  
+& & '   (  
+ !    (
+ (   Y Y
+     (      (  
+ (  d Y'Y
+ ' !    ( '    ' ! (  ' 
+ 
 
-Figure 2.1.1.1.b. New Button, Overwriting ConfirmaW
+C C
 
-W
+    (    $    
 
-1  1
-• browse the file system, starting from the current directory
-• click the Open button (of the below window) to select the text file to be processed
-• if not found, open an error window
-• click the "Cancel" button to exit with no selection
+    
 
+      (  '   & 
+ &   , (  ,  (
+ ( & 
+ (  ( &,        (    $  $  ( &  &  
+'   (
+ (   Y Y
+     (      (  
+ (  d Y'Y
+ ' !    ( '    ' ! (  ' 
 
 
-
+I         '
+        ( $ 
+ &  ( (  (  
 
-
+ ,   (  '    
 
-
+  
 
-│
+(
+
+
+
+&  $ 
+
+  '  '   (  
 
+  
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌───┬─────────────────────────────────────┬───┬───┐
+│
+│
+│ _ │  │
+   
+├───┴─────────────────────────────────────┴───┴───┤
+│   │
+│
+│ , 
+     ! ' 
+│   !      $    
+│
+│ ┌────────────┐┌────────────┐
+│
+
+│ │
+││
 │
+│
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-Open
+    
 
-
+
+ C
 
-
+ ,
 
-
+  " ( &   !
 
-
+C
 
-
+!   ( (  
+C  " $ 
+'   (   
+ C
 
-
+"IC 
 
-
+ 
 
-
+C
+
+   ( '   
+
+  & 
+
+(  ( &  , ' ! 
+ Y ! Y 
 
-│ _ │
+( &  
 
-│ x │
+  
 
-│ Directory: [...........................] [] │
+ 
+
+(  ' 
+
+ 
+
+ 
+
+   (
+
+ '    ' !
+
+
+
+ 
+
+(  ' 
+
+┌───┬─────────────────────────────────────┬───┬───┐
+│ _ │  │
 │
 │
+  
+├───┴─────────────────────────────────────┴───┴───┤
 │
-ppp
 │
-qqq
+ 
 │
 │
 │
-rrr
 │
+
+    
 │
-.....
 │
-│  ......................................... │
+
 │
-
-
-│ File name: [......................] │ Open │
 │
-
-
- W 
-│ W   
- u] │ Cancel │
+   !
+│
+│
+"     # 
+│
+│
+    $ %& &
+│
+│
+│
+│   !   ' ! 
+ 
+
+│ ┌────────────┐┌────────────┐
+│
+│ │
+││
+│
+│
+
+
+│ └────────────┘└────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-
+
+ I
 
-
+   
 
-
+ ,
 
-W
+ " ( &   !
 
-
+C
 
-1   W
+
 
-
+ 
 
-
+   (   ,  (    ( & 
+  $  &  ( (     (
+   (
+  
+ !    (  (    (
+  &  ! !
+ (    
+ 
+  
 
-
+s 
 
-
+   & (( '    YY ' 
+  ' 
 
-
+ I I C
 
-
+IC  
 
-
+I I &,  ( &  
+  ( (  (
 
-
+I 
+
+ &  ! !Y 
+
+ 
 
 
 
-
+ '
 
-│
+ C 
 
-│
+'   (   
+   !
+  & 
+   !        
 
+ !   
+
+     ! &  !  !  
+  ! ! !  
+     
+' 
+ ,   YC0Y '        ,  (   &( 
+    '   &  ! !
+┌───┬─────────────────────────────────────┬───┬───┐
+   C
+│
+│
+│ _ │  │
+├───┴─────────────────────────────────────┴───┴───┤
+│  C   │
+│ ┌────────────┐
+│
+│ │
 │
+│
+C0
+│ └────────────┘
+│
+└─────────────────────────────────────────────────┘
 
-W
+
+!
+
 
-Wow
+   
 
-│ x │
+  !
 
-│ File ....................... does not exist. │
-
+  ! &  !  !   '    
+  
+!
+  ! ! ! ! '    , 
+
+ !    
+
+  Y Y '            !
+
+   Y Y '        ,  (   &(
+   !
+
+     ' 
+
+
+
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌───┬─────────────────────────────────────┬───┬───┐
+│ _ │  │
+│
 │
+   I 
+├───┴─────────────────────────────────────┴───┴───┤
 │ 
+I   │
+│
+│   !     
+! 
+│ ┌────────────┐┌────────────┐
+│
 │ │
-OK
+││
+│
 │
+
+
+│ └────────────┘└────────────┘
 │
-│ 
+└─────────────────────────────────────────────────┘
+
+  ' 
+   &Y 
+
+
+"I
+
+ ! 
+
+ 
+
+s 
+
+   !
+
+!  
+
+C 
+
+ &   &      
+ &    
+ & 
+I "I &  _(
+   &&      (  $  , 
+ &  (    
+"I &
+
+        I '  , '  !    ( &  s 
+ "C
+
+C 
+ !  
+
 │
+
+" _(   
+
+ &  _( 
+
 
 
-
+_(, 
+
+_(
+
+ &  (
+
+! 
+
+ _( &     ' 
+  _( &   &   , '  (  
+  &   ' 
+     $ ! 
+
+
+C#
+
+C 
+ !  
+
+│
+
+$ _(   
+
+ &  _( 
+
+
+
+_(, 
+
+ &  
+
+! 
+
+_(
+ '   (
+
+ _( &     ' 
+   _( &   &   , '  (  
+  &   ' 
+     $ ! 
+
+
+
+
+C 
+ !  
+
+│
+
+ &      ( !
+
+ & 
 
 
 
-Figure 2.1.1.2.b. Open Button, File Not Found Erro
+ 
+
+_(
+
+ &   
+
+ '   (
+
+ _( &   &   , '  (  
+  &   ' 
+     
+  I
+
+C 
+ !  
+
+│
+
+ & 
+
+
 
-W
+_(
 
-2.1.1.3. RECENT BUTTON
-• view the list of most recently processed text files (max 20, the most recent one on top)
-• click a file button to select the text file to be processed
-• click the "Clear" button to clear (after confirmation) the list of recent files
-• click the "Cancel" button to exit with no selection
-
-4/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+   ( '    (  ' y:
+ _( &  
+( 
+ & 
+ C
 
 
 
+ &   
+
+& 
+
+CC
+
+   (
+
 │
 
-
+ ! 
 
-
+( 
+
+
+
+
+
+
+
+!
+
+ ! 
+
+   ( '  
+
+ _( &  
+
+
+
+ 
+
+
+
+ & 
+
+!
+
+
+
+    
+
+
+
+ & 
+
+
+
+_(
+ 
+
+    
+
+C 
+ ! 
+
+    (    $    
+ _(  '  
+&   '   (
+"I
 
-n 
+_(
 
+ ' 
+
+
 │
 
-
+
 
-
+ & 
 
-
+C 
 
-
+ Y ( &   
+C
 
-
+& ( !
 
-
+ ' 
+
+
+│
+
+  
 
 
 
-│ _ │ x │
+C 
+
+ _( &  
+ 
+
+ , '  (       
+
+I C
+
+IC 
 
-
 
+
+& 
+
+ & 
+
+_(
+
+    
+ ,
+
+!     
+
+  ( & 
+
+C 
+
+I "I &,  ( &   '   (   
+( (     (, (  & 
+
+ 
+
+
+
+& 
+
+ ! 
+
+  
+
+  
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+  !     ! 
+   & 
+  !        
+  ( &  & 
+
+I "I
+( 
+
+&, !
+    ,
+      &Y 
+
+    &  &
+     (  
+
+ $  
+
+    (    
+      ,  
+       
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+ 
+
+
+I" 
+
+C I
+
+   '( ,   &  &            '
+  &$ ( &    
+(   &    '   '     (  (
+
+  
+&   (       
+       '       
+   ! ,   $              '  '&
+&  
+  
+  !
+   ( Y  &    !
+    &  '  Y Y
+
+   , !  '
+
+'  &    YY, 
+
+&    YY  !    ' YY  (  !  
+ '  Y Y
+
+ '   
+  
+  !
+     ( Y  &
+   ! ' 
+  
+  !
+     (   !
+ '  
+
+
+
+ (
+ &  
+
+  
+
+ ( &  
+
+
+
+   &      ( ( ! 
+
+
+
+ &,  $ '      ,   '!
+
+    , !          !   
+
+   , !      
+ &    
+ ( 
+ !        
+
+
+
+
+ 
+
+ 
+
+(
+
+
+
+!  
+
+  
+   ' ((
+
+&  ,
+    
+! 
+
+(
+
+    ,
+    
+ 
+
+┌────────────┐
+┌────────────┐
 │
 │
-│ 1. │ /home/xxxx/yyyyy.txt │
 │
-
-
 │
 │
+┌──────┴──────┐
+┌──────┴──────┐
 │
-
- │
-│ 2. │ /home/xxxx/aaaa/bbbb/cccc/dddd/xy.txt │ │
+    ,    
+
+
+├─────────────────────────────
 
- │
+
+
 │
-
-
 │
 │
-│ 3. │ /home/xxxx/pppp/qqqq/rrrrr.txt │
 │
+ 
+
+ 
+&   ( , !  │
+ 
 │
 │
-
-
- 
+│
+
+──────────────────┤
+
 
-│ 
+
+
+└──────┬──────┘
+└───┬─────┬───┘
+│
 │
-│ │ Clear
-│ │ Cancel │
 │
-│ 
+│  │
+│( ,
 │
- 
+  ( (│
+  ( (│
+
+│
+│ 
+│
+( ,  │
+└─────────┘
+
+
+
 
 
-
+
 
-
+     &    
+            I
 
-W
-
+ 
 
-│
+&
 
-
+  , (     
 
-
+&   
+         !     
+           ,
+   
+  ' ,    
+
+i         ' (( , 
+  (         
+
+         ,
+      ' ,     
+i 
+       ' (( , 
+  (          (
+    
+   !
+   (    (      
+
+
 
-    W W Wndow
+
 
-n 
+ 
 
-│
+!
 
-
+  , (       
 
-
+&    
+  ' ((  (   (, !     & ,  
+ '      ,  &    !   
+
+   
+         
+i      
+  ' ((
+!      ,     
+
+      ' ((  ( ,
+i
+       ' (( , 
+
+  (          (
+    
+   !
+   (    (    ' ((  ( ,      
+
 
-
+&'
 
 
+
+!
+
+
 
-
+( 
 
-
+! ,
 
-│ _ │ x │
+&  '
+!, 
+$  
+
 
-│ history of recent files will be lost!
-│ shure to clear history?
- 
-
-│ 
-│ │
-Yes
-│ │
-No
-│
- 
-
-│ 
+ ,
 
-
+
+
+  
+
+      'y:
+
+      ! 
+
+
+
+  
+
+  (
+
+ d
+
+& 
+
+     
+    ( ,          
+      
+ (   '
+        
+  & , 
+ 
+(    (     (   (
+
+  (
+
+ 
 
+I( ! 
+   &       
+& , !    ( & &       
+ (,             , ! 
+     !    
+$   ! ,     ! ( &   
+ !  ,   (  
 
 
+ & (  &  ( & !, ! &   
 │
 │
-│
+
+
+
+ ! 
 │
 │
 
-
+  ' '
 
-Figure 2.1.1.3.b. Recent Button, Clear Confirmatio
+
 
-W
+'
 
-For further details about backup files, see 8.8.
+
 
-!
+   
+
+ 
 
-1
+!    '
+  '
+
 
-• browse the file system, starting from the current directory
-• save current text file into target text file, together with its argument set
-• if target text file already exists, ask for confirmation
-• target text file becomes the current text file
+
 
-
+ 
 
-│
+ 
 
-
+   &,  d Y Y, ! d YY
 
-
+ 
 
-│
+11
+  
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+      '   d Y Y, '     ( '
+! '
+   Y
+ Y,         
+
+ (     
+
+   "I"
+(  & 
+
+! ! 
+
+    
+
+  (! !
+
+    (
+
+    '
+
+&  
+   '
+   '
+    
+    '    
+    
+&   '  '   
+   '
+I   
+
+
+
+   '
+
+   '   (
+ 
+    '    ' (    !  '
+    '    
+    
+&    '    
+   '
+
+
+
+
+   '
+&  
+   '
+        '       
+&   '  '
+   '
+     
+
+&'     
+
+ 
 
 
 
-s 
+ && , '   
 
-
+'
 
-
+  
 
-
+'    ' 
+
+  ( 
+   
+   
+ 
+
+  '  , ' 
+
+
+
+ '  
+
+
+
+ " I   
+
+
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+ "  
+
+      '  
+ ,   ! :
+
+  ( 
+' 
+       
+
+   
+
+ 
+
+ 
+
+&  '
+
+&  
+   (      (     '
+&  
+         (   (! '
+ 
+ &  
+   !
+ '   
+      (       '    ,     &'
+&' (          
+ ($  (   
+ s   
+
+(   
+
+&   ,  (   , ( & (   
+ 
+ (     
+&'    ,    
+ 
+ 
+&    , &   &  ( '  &   
+  "     ,   (   
+  I    ,   (  '
+      ,   ( (    
+┌────────┬─────┬─────────┬────────┬──────────┬────────────┬───────────┬─────────┬──────┐
+│  
+│"  I  │I "C   │C
+│"  │#│ C I"│C
+ │  │
+
+
 
 
 
-
+│ &│ d  │ 
+│&    │(  │ 
+│ 
+│ 
+│ │
+│  &│$ !  │
+│
+│
+│ │
+│ &'  │ d  │ 
+ │ 
+│ &'  │
+│  &│$ !  │
+│
+│ 
+│ │
+│&    │$ !  │
+│ 
+│
+│ │
+│"  │ d  │
+│ d  │
+│&    │$ !  │
+│
+│
+│ │
+│I 
+│  │ d  │
+│&    │$ !  │
+│
+│
+│ │
+└────────┴─────┴─────────┴────────┴──────────┴────────────┴───────────┴─────────┴──────┘
+
+    " 
+&  
+$
+
+ $, $ (
+
+    (   ,  
+   ,  
+   
+
+&'     
+
+&'   , 
+
+&  , & 
+
+
+
+'  
+
+& ,
+
+&    
+
+
+
+ &  
+
+  
+
+$ ! 
+
+ 
+
+   ,
+
+   ,  
+  
+
+&  
+
+ $     
+
+( & ( (   YY 
+
+
+
+
+
+  "     (,
 
 
 
+ (
+
+
+  
+
+ 
+
+ '
+
+ "  
+
+YY
+
+ " 
+
+
+
+
+&     (  (   (,   ( &  (      
+
+     IY     "         
+(   
+,   '  $ (   & 
+
+
+
+
+
+"  
+
+ 
+
+&'     &  '
+&'          
+  (
+  (        &  '   ! , ( !  (    
+ 
+ ' , &  '    &      ,   &  '
+
+&' 
+ 
+
+    &  &   YYYY
+   &    YY
+ (!  ! , (
+$ (
+
+
+
+ 
+ 
+ 
+
+,
+
+&'   
+$
+$
+$
+
+&'   
+
+   
+
+
+
+    
+
+&'  " 
+&'  " 
+&'  " 
+
+  &  (!
+
+  ( s  '$  s  
+
+&'    
+ ( 
+  ( 
+$ &'   
+  &  '
+&'           $
+ 
+ $       , '   & 
+&'   
+
+  ',  &
+
+ (     
+
+
+
+
+
+&'   
+
+ $ '!
+
+ 
+
+
+& 
+
+  $ ( 
+
+
+
+
+
+ 
+i    i !   
+ 
+i   i !   
+   "    
+        ' Y Y  
+
 
 
-
+&'        &  ,
+   & '    ,    $ &   
+ (        
+!        ,  ! '
+&  
+&' 
+
+$  
+
+
+& ,
 
-│ _ │
+ 
 
-│ x │
+'
 
-│ Directory: [...........................] [] │
+&'  
+
+'   &  '
+
+  ((  (( ( $
+
+&'     (
+
+(  !
+
+(
+
+  ( 
+
+ 
+
+ 
+
+ , &  
+
+ &  
+
+  
+
+ "  
+
+13
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+I( 
+ 
+
+!
+
+&'    
+   
+&' 
+  !
+
+( & , & 
+
+' , ' 
+
+ , ' 
+
+ $
+
+ &
+│
+    
+│ 
+│
+│  ''' ''' '''
+│
+│    
+│
+│    
+│
+│    
+│
+│  ((( ((( (((
+│
+ !  ( !    
+│
+    
+│ 
+│
+│ 
+│
+│  """ """ """
+│
+│ 
+│
+│    
+│
+│    
+│
+ !  ( !  &    
+│
+    
+│ 
+│
+│ 
+│
+│  """ """ """
+│
+│ 
+│
+│    
+│
+│    
+│
 │
 │
 │
-ppp
 │
 │
-qqq
 │
 │
-rrr
 │
 │
-.....
 │
-│  ......................................... │
-
-
 │
-│ File name: [......................] │ Save │
 │
-
-
-│ W   
- W 
- u] │ Cancel │
 
-
+ !  ( !  &
+    
+
 
-
+  
+
+
+ """ """ """
+
+   
+   
+
+
+       &
+
+ C I" "  
+"  , I 
+
+ 
+
+   
 
 
 
-Figure 2.1.1.4.a. Saveas Button, Target File DefinWW
+&    ,  & 
 
-
+   (      &     &    (   (    
+       (  &             
+  
+    '       
+ 
+( (
+
+  !       &      (     
+   Y Y   ,     
+(          , (
+'  !    &'  
+ I 
+    
+      
+ (
 
-│
+    ,  
+&    
 
-
+  &' ,
+    
+s ,  !   ,
 
-
+         (  (,  (
+  '    $  $  '    
+
+
+
+ "C   " 
+ "     ! &
+&           (   ,    (
+
+, ' !  &' (     '   &,  "     !
+ 
+&'    ,  I   
+      , '   ! Y  
+ &     "     (
+ "           "    
+
+ (  ' 
 
+  ,      ( "     (
 │
 
-
+ !  Y (   Y 
 
-
+ & 
 
-
+ Y"  Y ,  &
 
-
+14
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+ 
 
-
+  
 
-│
+ 
+ 
 
-
+  ( Y s $  i    
+
+"    
 
-W
+  
 
-│ x │
+   i !   
+  i !           ' Y Y  
 
-│ File ....................... already exists. │
-│ Do you want to overwrite it?
+i
+i
+
+ &
 │
- 
-
-│ 
+    
+│   
 │
-│ │
-Yes
-│ │
-No
 │
+   $    
 │
+( "    
 │
-│ 
- 
-
+! ' 
+│
+│ 
+│
+│  ''' ''' '''
+│
+│    
+│
+│    
+│
+│    
+│
+│  ((( ((( (((
+│
+ !  ( !    
+│
+    
+│ "C  
+│
+│
+ 
+│
+ 
+'' '' ''
+│
+ 
+" " "
+│
+ 
+  
+│
+ 
+  
+│
+  (( (( ((
+│
+│ 
+│
+│ 
+│
+│  """ """ """
+│
+│ 
+│
+│    
+│
+│    
 
-
+        &
+
 
-
+ & ( "    
 
-Figure 2.1.1.4.b. Saveas Button, Overwriting Confi"W
+     ( 
 
-W
+
+
+ I  " 
+ ' 
+
+I   
+! &
+&          (  ', 
+  , ' !  !      '     '         ,
+ ' 
+ (                
+ 
+
+s   ' ( Y    (! '  ' s  Y Y '   ' s 
+  s  Y  '   ' s  Y Y    
+  
+(! '
+   ,     !    Y Y  Y  
+
+s   '  !
+
 
-2.1.2. CORRECT BUTTON
-• click the Edit button to edit the correction file, by the text editor defined by -y
-• click the Reset button to reset the correction file to default values
-• click the Undo button to restore the correction file to its previous version
-• click the Cancel button to exit with no action
-For further details see 8.3.
+ s   '    $ !  (   (             
+s   ' &!        
+      
+$  ' !
+contain:
 
-
+&'  (
+ s  ' Y Y
+ 
+          &  s     ( 
+ '      & 
+s    
+&'  (           & 
+
+s   
+s     (   ' 
+  s    
+ '   
+& 
+ I   
+
 
-│
+ ,
 
-
+ '   
+  
 
-
+ ( ( !
 
+   I   
+
+ & , !
+
+ '
+
+ (  ' 
+
+ & 
+
+    ( I   
 │
 
-
+ 
 
-n 
+
 
-
+  
 
-
+I   
 
-
+(
 
-
+
 
-
+
 
-
+&  
 
-│ _ │ x │
+ YI Y ,  &
 
-│ edit reset or restore the correction file?
- 
- 
- 
-│ 
-│ │
-Edit
-│ │ Reset
-│ │
-Undo
-│ │ Cancel
-│ 
- 
- 
- 
+ !  Y (  'Y 
+  ( Y s $  i    
 
-
+  
 
-W
+ 
+i    i !   
+ 
+i   i !   
+    "    
+        ' Y Y  
+
 
-
+     ,
 
- 
+ ' 
 
-│
+   &  
 
- │
-│ │
+    
 
- │
-
-W W Wow
+ I       (
 
-2. Usage Modes
-5/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+ "  
 
-
+15
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+ '
+ 
 
-
+
 
-
+ (    &   
+ 
+ YY
+  &  '
 
-│
+ & ( I   
+
+      I   
+
+     ( 
+
+   , Y
 
-n  n 
+
 
+ I  " 
+ ( (    ,   
+     ! &
+&        
+( 
+, ' !  !              ' (!
+'
+  ,
+   !      &   ,  !   
+(  
+  (! '
+  
+
+
+
+       ' (
+    (  ' (
+
+ 
+
+ ( , (
+
+   (
+
+   ( 
 │
 
-│ current content will be lost!
-│ shure to restore previous content?
- 
-
-│ 
-│ │
-Yes
-│ │
-No
+    
+ 
+ 
+
+
+
+
+ &   
+
+ ! ( Y ( (
+
+     
+
+ Y
+
+  
+
+Y ,  &
+
+Y 
+
+     ( Y s $  i  (  
+
+  
+
+i
+   i !   
+i
+  i !   
+    "    
+        ' Y Y  
+
+ 
+
+(
+
+  
+
+' 
+
+  ,    (  (  !  ( (
 │
-│ 
- 
+
+ &  '
+
+  ! , 
+
+  
+
+   
+
+    (
+
+ Y
+
+Y ,  &
+
+ !  Y& Y 
+
+ !   
+
+   
+
+'
+
+
+
+(
+
+    ,   ! 
+&  
+   (     (  Y   '
+&  
+        (  Y (! '
+ 
+ &      ! ' 
+     !  &  '   ! , ( ! hich:
+  (     s $  i  
+      
+   '     
+&        YY
+   ' (          ' (
+
+  $ !    Y YYY, &           
+ 
+ &    YY
+    
+  (!  ! , (
+,
+ 
+
+ & (     
+ 
+ 
+ 
+ 
+
+
+
+
+
+
+
+
+    "  I  & " 
+    "  I " 
 
+'    "  I "  
+    "  I "  
 
-
+   
+ '
+
+
+
+
+
+  
+
+&  
 
 
 
-
+   ,   (
+
+  
+
+ $ (
+        ( &       ',    s
+$ (            
+       ' &  '
+    ' 
+:
+&         "   
+ 
+ 
+
+
+
+'
+
+, (
+
+  
+  (
+
+! 
+
+&   !     ((   '! 
+
+    ,  , (  ' (,        
+    , & , (  ' ,       
+
+ & ( 
+
+   
+
+    ( 
+
+
+
+  
+
+ $,  ! '
+
+i  i
+    !   
+i
+  i !       
+
+  ' 
+
+(  
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+  
+
+I ( &  &         
+
+    (   & 
+
+
+ ,
+' 
 
 
 
+&   , 
+
+ 
+
+'
+
+   
+
+             (  Y Yd , Y(Yd (   , YYd
+ , YYd   $   , YYd ' ( $  $  
+
+ 
+
+
+ ! Y Y,          ,   (  !   &      
+( & 
+(,  
+ &   ! Y Y
+ ! Y (Y,          !        (       
+ ! Y Y,           '$  !        (  
+    
+     '$  !       $ 
+ ! Y Y,     
+&     
+$ 
+ ! Y Y,           '$  !
+&   
+$  ,     
+      
+    '        
+     $ 
+&        
+  
+   ,
+I(   YY YY  YY, !
+       (    
+   
+&  , &  '    !   $
+(  !   $  , 
+ '
+          ,  
+ 
+ (
+       
+   
+&' (   
 
+   '
+
+
+ ,
+
+ &  '
+
+ 
+
+      
+
+        
+
+  
+
+!   (      , (
+  (  d
 
+
+
+
+
+& 
+
+    
+
+I( ! 
+   &       
+& , !    ( & &       
+ (,             , ! 
+     !    
+$   ! ,     ! ( &   
+ !  ,   (  
+   ,   (   ,   ( '
+      (     &' (
+&' (                 &  (    !
+   s   
+   
+  (     ,    !
+( & ( Y(Y 
+ ,          (
+&,  
+&' ,     (    C 
+,  , &   
+ 
+ & 
+          , !     ,  
+  (     
+(     ,  (  ' 
+ & 
+  ( 
+
+ &&   ( & (    
+  '   '  
+    '   ,  (  Y     ! &           
 
+
+  ,  
+'  $' 
+
+!   YY 
+! s  YY
+ s   YY
+! YY  YY !    
+ I  $
+
+$   
+ ,
 
-│ _ │ x │
+
+(
 
-
+    ( (   
+
+
+
+
+
+ ,
+ ,
+ ,
+C ,
+
+   !
+( & ( 
+
+  &  &  
+
+'       '$ 
+  !    
 
+      '    C 
+
+ 
+
+
+
+ & 
+
+$ (  (    (    ( $  , ( (  Y Y
+$    (    (    ( $  ,  (  Y (Y
+(  (    (    (   , ( (  Y Y
+   (    (    (   ,  (  Y Y
+
+ 
+   $  ' 
+$  '  !
+
+ (     
+
+   $ 
+
+
+
+ (!,  
+
+┌────┬──────────────────────────────────────────────┐
+│
+│ # │
+# 
+──┤
+
+│Y Y│Y Y
+│
 │
+│Y Y│
+    I
+│Y Y│ (    , ! (  YY
 │
 │
+│Y Y│ (    , ! (  YY
 │
+│Y (Y│ (
+&, !   
+│Y Y│ (   , (
+, !    YY │
 │
+│Y Y│
+   ,  
+  & ,  
+│Y &Y│
+│
+│
+│Y Y│
+   ,  
+   ,  
+│
+│Y Y│
+  & ,  
+│Y Y│
+│
+│
+│Y Y│
+   ,  
+  &  , 
+│Y Y│
+│
+│
+│Y Y│
+   
+&'
+&' (  
+│Y Y│ 
+│
+  $"   I    │
+│Y Y│
+└────┴──────────────────────────────────────────────┘
 
-
+       #  '
+I( (
 
-Figure 2.1.2.b. Correct Button, Restore Confirmati
+&  
 
-  
+    
 
-1
+   ( 
+&  !!!
 
-    W"W
+  
 
- W
+  
 
-n
+
 
-defined by -Y (like 'yawp -H')
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+ ! 
+ Y Y → Y&  Y
+ Y Y → Y Y
+ Y (Y → Y!!!Y
+ Y Y → YY
+ Y  ( Y → Y&  !!!Y
+ Y  ( Y → Y !!!Y
+ $   ( Y
 
-
+
 
-
+ 
 
-
+Y  (( '
 
-│
+,  ((  (( (  
 
-W
+&'  (
 
-n 
+ , (
 
-│
+ $
 
-
+&' 
 
-
+&
 
+┌───────────────────────────────────────────┐
+│
+│
+  ((
+
+
 
+│ │ │  │ │ │  │  │ │  │ │ │ │
+
+
+│ │ │ │ │ │ │  │ │ │  │ │
+│
+│
+│
+│  │ │ │ │ │  │  │ │  │  │
+│
+│ │
+│  │iii│iii│iii│ │  │ │ │  │
+│ │ $│ $ │ │ │ │  │ │
+│
+│ │ │
+│
+│ │ │ │
+│ │ $│  │ │ │  │  │
+│ │ │  │ │ │  │
+│
+│ │ │ │ │
+│
+│ │ │  │ │ │
+│ │ │ │ │ │
+│
+│ │ │  │  │ │ │
+│ │ │  │ │
+│ │ │  │
+│
+│ │ │ │  │  │ │ │
+│
+│ │ │  │ │  │ │ │ │
+││ │
 
-
+└────┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┘
 
-
+
+ 
 
-
+ '
+
+#   C
+
+ 
+
+   C
+
+
+
+ & 
+
+
+
+
+
+ ( 
+ &      (  ,  &'        ,  (    
+YY,     YY,
+  
+   &  '  ,  
+ (   &    ,   &' 
+' (  (  
+   &    &
+( 
+  (
+&' ( !   &  &'    s    ' 
+ ( 
+  
+ ,
+$   (    
+' &'   
+
+
+
+
+Y
+
+Y     
+
+
+
+I( 
+
+ 
+
+ 
+ 
+
+
+
 
- 
+ $ $  , ' 
+&'
 
-│ _ │ x │
+&
 
+(    &
+
+ &  
+ ( 
+ ( 
+
+ 
+
+ 
+
+ 
+
+!
+
+ (( '  
+
+ 
+
+        (
+
+   &      
+
+
+$
+
+
+
+
+
+ &
+
+
+
+  
+
+'
+
+  
+
+ , 
+
+C((
+
+┌─────────────┐
+
+│
 │
- 
 │
+‾‾‾‾‾‾‾‾‾‾│
 │
-   
+··········│
 │
-https://pypi.org/project/yawp
-  !
+··········│
 │
+··········│
 │
-carlo.alessandro.verre@gmail.com
+·······│
 │
-│   
- 
-│ 
- 
-
-│ │
-Yes
-│ │
-No
+··· ···│
 │
- 
-
-│ 
+··········│
+│
+··········│
+│
+··········│
+│
+··········│
+└─────────────┘
 
-
+  
+  
 
-W
+ $  
+   
+
+┌─────────────┐
+│
+
+C│
+│
+‾‾‾‾‾‾‾‾‾‾│
+│
+··········│
+│
+··········│
+│
+··········│
+│
+·······│
+│
+··· ···│
+│
+··········│
+│
+··········│
+│
+··········│
+│
+··········│
+└─────────────┘
 
-   
+┌─────────────┐
+
+│
+│
+│
+‾‾‾‾‾‾‾‾‾‾│
+│
+·········· │
+│
+·········· │
+│
+·········· │
+│
+···$ ··· │
+│
+··· ··· │
+│
+·········· │
+│
+·········· │
+│
+·········· │
+│
+········· │
+└─────────────┘
 
- 
+
 
-
+
 
+  !  '! 
+
+ !  !   
+  &  
+ &   &      ' $
+┌─────────────┐
+│
+ │
+│‾‾‾‾‾‾‾‾‾‾
 │
+│··········
 │
 │
+│··········
+│··········
 │
 │
+│···$ ···
+│··· ···
 │
 │
+│··········
 │
+│··········
+│··········
 │
 │
-│
+│··········
+└─────────────┘
 
-
+ , 
 
-   W"W
+  
 
-indow
+   
 
-2.1.4. EXIT BUTTON
-• save argument file and session file
-• close main window
-• close log file
-
- WW
-
-W
-
-  W by mouse the 'x' button in main window's top right
-fl W   "W
-   n   " "t may lose its value, use always the 'Exit' button
-instead.
-
-
-
-  f
-
-1
-
-fl
-
-2.1.5.1. EDIT BUTTON
-• edit the text file through the text editor defined by -y
-• if the text file has been altered, backup its original content into a timestamped copy
-The text file to be edited must exist. This behavior is different from that of CLI Edit mode, where
-if the text file does not exist it is automatically created as an empty file.
-
-
-
-1  1
-
-• read the text file, eliminating:
-• "horizontal tab" '\t' in lines, each replaced by four blanks
-• trailing blanks in lines
-• format the text file content:
-• remove page headers and content of automatic chapters
-• justify the text (see 3.)
-• perform automatic multi-level renumbering of chapters and refill (if needed) the automatic
-Contents chapter in the text file (see 4.3.1.)
-• recognize relevant subjects and refill (if needed) the automatic Index chapter in the text
-file (see 4.3.2.)
-• perform automatic multi-level renumbering of figure captions and refill (if needed) the
-automatic Figures chapter in the text file (see 4.3.3.)
-• if -p  'n', cut the text file in pages, by inserting two-lines page headers, allowing
-page numbering control and insertion of initial Roman-Numbered pages (see 5.)
-• if -g is on, redraw horizontal and vertical segments and arrowheads by suitable Unicode
-graphic characters (see 6.)
-• if text has been altered:
-• backup the text file into a timestamped copy
-• rewrite the text file
-• if -X is on:
-
-     W W   W   u
-    W      W y -Y
-
-The text file to be processed must exist.
-
- 
-
-11  1
-
-• read the text file, eliminating:
-• "horizontal tab" '\t' in lines, each replaced by four blanks
-• trailing blanks in lines
-• do not format the text file content
-• if -g is on, redraw horizontal and vertical segments and arrowheads by suitable Unicode
-graphic characters (see 6.)
-
-6/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-• if text has been altered:
-• backup the text file into a timestamped copy
-• rewrite the text file
-• if -X is on:
-
-     W W 
- W
-  
- W  
-   W y -Y
-
-The text file to be processed must exist.
-2.1.5.4. UNDO BUTTON
-• restore the text file to its previous version
-• if -X is on:
-
-     W W 
- W
-  
- W  
-   W y -Y
+ ((  ( &  
 
-
+ ((, (
+  , (
 
-│
+C(   ( 
 
-
+'
 
-
+Y&&&&Y  
 
-n 
+ (  '     , 
 
-│
+,       
+ Y
 
-
+&'     
 
-
+ , 
 
-
+$  ,
 
-
+C
+ $
 
-
+   
+
+
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+    (     
+
+
+    '
+
+ ,         (      (
+YYd , YYd 
+
+ YYd, Y Yd , Y'Yd' ,
+
+
+ (  d Y Y,        ! 
+ (  d Y'Y,       '   , &  ( '        Y
+ (  d YY,         , &  (  '$    YY
+ (  d YY,          , &  ( &      YaaaaaY
+ (  d YY,         , &  ( $      Y‾‾‾‾‾Y
+
+Y
+
+ 
+
+
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+ I" 
+I
+
+ & 
+&&' 
+
+( &
+
+
+
+  ,
+
+
+
+&( 
+
+
+
+
+
+ ' 
+
+ 
+
+ & , ' 
+
+   &    , 
+                
+    (    
+ 
+( &   ,      (         ,   
+ 
+       (
+ I"  
+
+I"
+
+    & 
+ !    
+
+ ( 
+
+ 
+
+
+
+ 
+
+ ! '  '
+
+
+
+! ' !
+
+ '  s  YvY   !    
+ $   & 
+   &(   YY  & 
+! 
+I(  
+
+ 
+
+ & 
+
+  ,  
+
+ 
 
+ ! YvY& 
+
+ !  !    '
+
+      (   
+
+ YY
+
+! 
+
+     ! 
+  !   ' 
+  (  '$  '! 
+
+ &
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+   
+vvvvvvvvvvvvv
+v   
+v
+ v
+vvvvvvvvvvvvv
+v
+v    v v
+vvvvvvvvvvvvv v 
+v
+   v
+vvvvvvvvvvvvv
+vvvvv
+vvvvv
+vvvvvv
+vvvvvv vvvvvv
+vvvvv
+vvvvv
+
+v
+v
+v
+v
 
+vvvvv
+vvvvv
+vvvvvv
+vvvvvv " vvvvvv
+vvvvv
+vvvvv
 
-│ _ │ x │
+vvvvvv
+vv v
+vvvvvv
+vv v
+vv v
+vv v
+vv v
+vv v
+vvv
+v v v
+v vv
+vv v
+vvv
+vvvvvv
 
-│ current content will be lost!
-│ shure to restore previous content?
- 
 
-│ 
+v
+ vvvvvvv 
+v
+ 
+
+v
+
+v
+
+v
+
+v
+
+v
+
+v
+
+v
+
+v
+
+v
+
+
+vvvvvvvvvvvvvvv
+     
+ 
+
+vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv
+v v v v v v v v v v v v v v v v v v v v v v v v v
+v v v v v v v v v v v v v v v v v v v v v v v v v
+v v v v v v v v v v v v v v v v v v v v v v v v v
+v vvv vvv v vvv vvv vvv v vvv vvv v vvv vvv vvv v
+v v
+v v v v
+v v v
+v v v v
+v v
+vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv
+
+
+
+
+
+
+
+
+
+vvv d vvv  vvv  vvv  vvv  vvv   d  vvvvvvvv
+
+
+
+
+
+ d    
+vvv
+v v
+v v
+v v
+vvv
+
+v
+v
+v
+v
+v
+
+vvv
+v
+vvv
+v
+vvv
+
+vvv
+v
+vvv
+v
+vvv
+
+v v
+v v
+vvv
+v
+v
+
+vvv
+v
+vvv
+v
+vvv
+
+vvv
+v
+vvv
+v v
+vvv
+
+vvv
+v
+v
+v
+v
+
+vvv
+v v
+vvv
+v v
+vvv
+
+vvv
+v v
+vvv
+v
+vvv
+
+vvvvv vvvv vvvvv vvvv vvvvv vvvvv vvvvv v v
+v v v v v
+v vv v
+v
+v
+v v
+vvvvv vvvvv v
+v
+v vvvvv vvvvv v vv vvvvv
+v v v
+v v
+v vv v
+v
+v v v v
+v v vvvvv vvvvv vvvv vvvvv v
+vvvvv v v
+
+vvv
+v
+v
+v
+vvv
+
+v
+v
+v
+v v
+vvvvv
+
+v v v
+vvvvv vvv v vvvvv vvvvv vvvvv vvvvv vvvvv vvvvv
+v vvv v
+v v v v v v v v v
+v v v v v v
+v
+vvv v
+v v v v v v v v vvvvv v v vvvvv vvvvv v
+v vvv v
+v v v v v v v v
+v v v v
+v v
+v v vvvvv v v v vvv vvvvv v
+vvvvv v vvv vvvvv v
+v
+v v v
+v v v v
+v v v vvvvv
+v v v
+v v v vvvvv v v
+v
+v v v
+v v v v v
+vvvvv vvvvv
+v v vv vv v v v vvvvv v v
+vvvvv vvv vvvvv v
+v v vvvvv
+
+  ,
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+│
+ !  (   
+│
+   
+│
+┌───────────┐
+│
+│   
+│
+
+│
+┌─┬──┐
+│
+
+ │ 
+ 
+ 
+│
+│
+│    │
+│
+│t│ │
+│
+│ 
+│
+
+
+
+
+│
+│
+││ │
+   │
+ 
+
+│
+└───────────┘
+│1│ │
+│
+
+│
+│
+││ │
+
+│
+│
+┌───┐
+┌───┐
+│3│  │
+
+│
+│4│ │
+ 
+ 
+
+│
+
+│
+│
+└───┘
+└─┬─┘
+│5││
+
+│
+│
+│ │ │
+│
+
+
+│
+│
+│
+│
+│ │ │
+
+│
+│
+│ │ │
+│
+
+
+│
+┌─┴─┐
+┌───┐
+│ ││
+│
+
+
+ 
+ " 
+ ─
+
+│ 
+└─┴──┘
+│
+└───┘
+└───┘
+     
+ 
+│
+│ ┌──┬─┬─┬─┬──┬──┬─┬─┬─┬─┬─┬──┬──┬─┬─┬─┬──┬──┬─┬─┬─┬─┬─┬──┐
+│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
+│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
+│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
+│ │ └┬┘ └┬┘ │ └┬┘ └┬┘ └┬┘ │ └┬┘ └┬┘ │ └┬┘ └┬┘ └┬┘ │
 │ │
-Yes
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│ └───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┘
+│
+
+│
+
+
+
+
+
+
+
+
+
+│ ─── d ───  ───  ───  ───  ───   d
+────────
+│
+
+
+
+
+
+ d    
+│
+│
+┌─┐
+│
+──┐
+──┐
 │ │
-No
+┌──
+┌──
+──┐
+┌─┐
+┌─┐
 │
-│ 
- 
-
-
-
-
-
-
+│ │
+│
+│
+│
+│ │
+│
+│
+│
+│ │
+│ │
+│
+│ │
+│
+┌─┘
+──┤
+└─┤
+└─┐
+├─┐
+│
+├─┤
+└─┤
+│
+│ │
+│
+│
+│
+│
+│
+│ │
+│
+│ │
+│
+│
+└─┘
+│
+└──
+──┘
+│
+──┘
+└─┘
+│
+└─┘
+──┘
+│
+│ ┌───┐ ┌──┐ ┌──── ┌──┐ ┌──── ┌──── ┌──── │
+│ ─┬─
+│
+│ │
+│ │ │ │
+│ └┐ │
+│
+│
+│
+│
+│
+│
+│ ├───┤ ├──┴┐ │
+│
+│ ├──── ├──── │ ─┐ ├───┤
+│
+│
+│ │
+│ │
+│ │
+│ ┌┘ │
+│
+│
+│ │
+│
+│
+│
+│
+│ │
+│ └───┘ └──── └──┘ └──── │
+└───┘ │
+│ ─┴─ └───┘
+│
+│ │
+│ │
+┌─┬─┐ ┌─┐ │ ┌───┐ ┌───┐ ┌───┐ ┌───┐ ┌──── ──┬──
+│ │ ┌─┘ │
+│ │ │ │ │ │ │
+│ │
+│ │
+│ │
+│ │
+│
+│ ├─┤
+│
+│ │ │ │ │ │ │
+│ ├───┘ │
+│ ├─┬─┘ └───┐
+│
+│ │ └─┐ │
+│
+│ │ │ │ │
+│ │
+│
+│ │ │
+│
+│
+│ │
+│ └──── │
+│ │ └─┘ └───┘ │
+└─┬─┘ │ └── ────┘
 │
 │
 │
+│ │
+│ │
+│ │
+│ │
+│ │
+│ ────┐
+│ │
+│ │
+│ │
+│ └─┬─┘ │
+│
 │
+│ │
+│ │
+│ │ │ │
+│
+└─┬─┘ ┌───┘
+│ │
+│ └┐ ┌┘ │ │ │ ┌─┴─┐
 │
+│
+│ └───┘ └─┘ └─┴─┘ │
+│
+│
+└────
 
-
+       &,  C
+   
 
-Figure 2.1.5.4.a. Undo Button, Restore Confirmatio
+
 
-W
+
 
-fl   W      file goes back to the penultimate version and the
+ &   !  ! Y
+  ,
+ ! 
+(     
 
-last one is lost forever.
-The text
-exist.
+     ,    ! ( 
 
-file
+   
 
-to
+ ! !    (
+Y ,   
+'   '   (
+     ( &   (  
+    
+( & &  !
+   &, ! !     
+&  '  & & 
 
-be
+ Y Y  $  ( &    (  , '   '      ( & '  YY
+    (
+ (  Y! Y
+ Y Y &         $  '   '! ( 
+ &  
+
+ Y Y  ( &     s   ' (,  '      
+   s  ' , '  & 
+ 
+│
+  ' 
+│ vvvvvvvvvvvvvvvvv
+│ v vv vv vv vv
+│ vvvvvvvvvvvvvvvvv
+│ vv vv vv vv v
+│ vvvvvvvvvvvvvvvvv
+│ v vv vv vv vv
+│ vvvvvvvvvvvvvvvvv
+│ vv vv vv vv v
+│ vvvvvvvvvvvvvvvvv
+│ v vv vv vv vv
+│ vvvvvvvvvvvvvvvvv
+│ vv vv vv vv v
+│ vvvvvvvvvvvvvvvvv
+│ v vv vv vv vv
+│ vvvvvvvvvvvvvvvvv
+│ vv vv vv vv v
+│ vvvvvvvvvvvvvvvvv
+
+ 
+
+
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+     ' 
+│
+ ! 
+│
+  ' 
+│ ┌─┬─┬─┬─┬─┬─┬─┬─┐
+│ │ ││ ││ ││ ││
+│ 
+
+│ ││ ││ ││ ││ │
+│ 
+
+│ │ ││ ││ ││ ││
+│ 
+
+│ ││ ││ ││ ││ │
+
+│ 
+│ │ ││ ││ ││ ││
+
+│ 
+│ ││ ││ ││ ││ │
+
+│ 
+│ │ ││ ││ ││ ││
+│ 
+
+│ ││ ││ ││ ││ │
+│ └─┴─┴─┴─┴─┴─┴─┴─┘
 
-restored
+
+ I"  I
+
 
-may or may not exist, while of course a suitable backup file must
+ ' '
 
-2.1.6. LOG BUTTON
-• browse the current session log file (see 8.4.) through the text editor defined by -y
-2.2. "CLI" MODES
-In CLI modes the text_file argument is mandatory and the other arguments a  W
-set in command line get their default values.
+  &,  C , 
 
-" 
+d Y Y, 
 
-The CLI modes correspond one-to-one to the four GUI buttons dedicated to the processing of the text
-file.
-2.2.1. EDIT MODE
-│ $ yawp -M e [...arguments...] text_file
+d 
 
-W W W    W  W lf mode (see 2.1.5.1.) with an exception: if the text
-file does not exists, it is silently created as an empty file, while in GUI mode this is an error.
-1  1
-│ $ yawp -M f [...arguments...] text_file
+ 
 
-W W W  
-
+   ( 
 
- "  W lI mode (see 2.1.5.2.).
+' ( (
 
-11  1
+
 
-│ $ yawp -M n [...arguments...] text_file
+ 
 
-W W W  
+ (  Y Yd , YYd(, YYd  , Y Yd 
 
-  "  W GUI mode (see 2.1.5.3.).
+  ,   
 
-2.2.4. UNDO MODE
-│ $ yawp -M u [...arguments...] text_file
+
 
-W W W  
+
 
-   W lf mode (see 2.1.5.4.).
+,      ! (  ' !
 
-3. Justification
-7/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
+  (
+ ! Y Y  
+ (  , '          '
+ ! Y Y  
+   &    $ (  's     
+   
+ ! Y Y  
+   
+ ! Y Y  
+  (!   &
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
 
- 3 ff f1
-
+ 
 
-l1f
+(
 
- W   W " "   " W" W 
+  &  s
 
-  u W "s " 
+vvvvv
+v v
+vvvvv
+
 
-input file. Each remaining "body line" belongs to one of these four types:
+vvvvvvvvvvv
+v
+v
+v
+v
+v
+v
+v
+v
+vvvvvvvvvvv
+  ' s
 
-• a line is an "empty line" if it contains no characters (all trailing blanks in input lines are
-stripped away, hence every input line containing only blanks becomes an empty line)
-• otherwise a line is a "dot line" if it's not empty and starts with:
-• zero or more blanks ' '
-• a "dot character", which can be:
-• a "black small circle" '•', or
-• a "decimal point" '.' (always replaced by '•' on output)
-• a blank ' '
-• otherwise a line is an "indented line" if it's not empty and starts with a blank
-• otherwise a line is an "unindented line" if starts with a non-blank character
-The formatting algorithm, driven by the input lines, oscillates between two states:
-• "picture state", where input lines are directly written out as they are
-• "text state", where input lines are accumulated into a paragraph
-justification and writing at paragraph end
-empty line,
-indented line:
-write
+(
 
-
+ !  ( !    
 
-
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+
+
+ 
+
+ 
 
+┌───┐
 │
 │
+└───┘
 
-
-
+
 
-
+ 
+
+ 
+
+
+
+  &  s
 
 
 
+┌─────────┐
+│
+│
+│
+│
 │
 │
 │
+│
+└─────────┘
 
-start
+ '
 
-
+
 
-│
+ s
 
-picture
-state
+
 
-
-
+      &,  C ,  d YY
+ !  ( !      
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
 
-buffer
+ 
 
-for further
+ 
 
-unindented line,
-indented line:
-append
+
 
-unindented line, dot line:
- assign
-
+┌───┐
+│
+│
+└───┘
 
-
+  &  s
+
+
 
+┌─────────┐
 │
+│
+│
+│
+│
+│
+│
+│
+└─────────┘
 
-
+
 
-
+ '
+
+ s
 
 
 
-text
+  (    ,
 
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 │
 
-state
+ ! 
 
-
+  '
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
 
-
+
 
-
+,   
 
-end of file:│
-stop
-│
+
 
+ 
+
+   &,  C ,  d YY
+
+   
+
+ 
+
+┌───┐
 │
+│
+└───┘
 
-empty line: flush, write │
+ &  s
 
+
+┌─────────┐
+│
 │
 │
+│
+│
+│
+│
+│
+└─────────┘
 
-
+  '  s
 
-
+  
+ 
 
-
+( !   
+
+
+
+   &,  C ,  d Y Y
+
+!    
+
+  
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+ C 
+
+(  & 
+   (
+
+( &
+
+    ,   ( 
 
 
 
-│
-end of file:│
-flush, stop │
+  ,  ( 
+ ' !
 
-
+ 
 
-
-
+ ' !   ( (
 
-
+'       ( & ,
 
-│
+
 
-
+ Y Yd , YYd , Y'Yd 
 
-│
-│
+
+ ! Y Y,          
+ ! Y Y,   (        (
+ ! Y 'Y,   (        (,
+   ' ! (  '  &  
+ (     ' ! ,  
+ 
 
-
-
+  
 
-
+  (  ' ! '
 
-
-
+ & 
 
-
+, (' !  ' ! (   ( (
 
-│
-│
-│
+ Y  Y
 
-
+'    
+    &      ' ! 
+    ( $   
+$  ( (      ' !     ' !  
+' ! ,     
+ ' 
+ &     
+ (   
 
-│
-│
+& (      (,  
 
-
+
 
-dot line: flush, assign
+  , ((      ( (
 
-Figure 3.1.a. Formatting State Diagram
-The picture state is the initial state. In this state, if the input is:
-• an empty line or an indented line: the line is written out as is
-• an unindented line: text state is entered, an "unindented paragraph" begins, the line is
-shrunk and assigned to the paragraph buffer, paragraph left indentation is set to zero
-• a dot line: text state is entered, an "indented paragraph" begins, the line is shrunk and
-assigned to the paragraph buffer, paragraph left indentation is set to the position of initial
-dot character plus two
-• at end of input file: processing is ended
+ & 
 
-   W   W  W  W W
-• an empty line: the paragraph buffer is flushed (justified, written out and emptied), state
-goes back to picture state, the empty line is written out
-• an indented or unindented line: the line is shrunk and appended to the paragraph buffer
-• a dot line: paragraph buffer is flushed, a new paragraph is started, the line is shrunk and
-assigned to the paragraph buffer, paragraph left indentation is set to the position of initial
-dot plus two
-• at end of input file: paragraph buffer is flushed, processing is ended
-Max length of text lines can be controlled by:
-• "-w, --chars-per-line": line width in characters per line (default: '0' = automatic)
+ Y ( (Y
 
- n  n  Wu     "automatic", namely:
- W n W "W  n W  n W "  " n
- W n W "W  n W  n W "  from -w
- W  n  n  "W
+   $  '  
+ $        (   , '  Y Y Y Y
+ 
+ Y Y
+ ' ! '  $   &   
+ '
+  ! Y Y
+ Y Y
+   ( & &    ! !   Y(Y
+&  '  ( '     I(    $ ,  &   I(
+    (
+    $ ,               (   &
+I(    (    ,     $ !  
+ C 
+   (  ' 
 
-• -w is deduced from max body line length in file (page headers are not considered)
+ 
 
- n
+  ,  !  
 
-W " 
+ ! (
 
-" n
+"
 
-Indentation of indented paragraphs cannot be greater than half of -w argument, whether set by user
-or automatically computed.
+#   
 
-  "   n
-│
+   
 
-"  " n  W"  e character per line only:
+ YY (
+ Y Y (
+ Y&&Y (
+ Y&Y (
+ (
 
-     
+ 
 
-│ $ yawp -M n -w 1 -X banner.txt
-│ $ cat banner.txt
-│   
+ & 
+ d & ,
 
-W 
-Now
+ (    (! '
 
-banner.txt
+     d  
+ 
+&& 
+ & 
 
-is
+  &&&
 
-
+!  
 
-"  W "n  n "
+  ((
 
-not altered because the '-M n', but the exported file 'banner.pdf' contains the
+  
 
-W Y  Y   
+   $   & $   (    
 
- 
+  
+  
+  &&
+  &
+&  $
 
-8/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-Line justification in text is controlled by -l argument:
-• "-l, --just-left-only": justify text lines at left only (default: at left and right)
+      (     ,
 
-
+ 
 
-"W
+ 
 
-• groups of consecutive empty lines between text paragraphs are reduced to a single empty line
-• groups of consecutive empty lines in contact with a picture are left unchanged
+&&
 
-
+Y,Y  &  
 
-
+Y         
+
+ , Y,&Y  Y&Y
+
+  
+ ( 
+,   ((  &    C    $           
+ ((, '  (    d  d && d & 
+  $   (  &  & 
+    
+
+"
+
+
+ (  '
+
+ 
+
+,     
+
+
+
+,   
+
+
+
+
+
+d! (
+
+&   (   
+   (  '( 
+
+,  
+ (  ' 
+
+  ,    
+  &&&
+ $   
+
+'
+
+, 
+
+  
+
+'
 
-  f
+   $    (        
+  ! $    (   ,   '
 
-Now we can define some "best practices" to follow when editing the text file.
-Unindented paragraphs should be:
-• preceded by an empty line
-• started by an unindented line
-• continued by indented or unindented lines
-• ended by an empty line (better) or by a dot line
-Indented paragraphs should be:
-• preceded by a line of any type
-• initiated by a dot line (better if starting with 4-8-12-... blanks)
-• continued by indented or unindented lines
-• ended by an empty line or by another dot line
+ &    
 
-W  
-• preceded by an empty line
-• initiated and continued by indented lines only
-• ended by an empty line (better) or by an unindented line or by a dot line
-Numbered intented paragraphs are not implemented, but they can be created by hand:
-• 1. first...
-• 2. second...
-• 3. third...
+ , ds
 
-4. Chapters
-9/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+ 
 
-  
+  &&  
 
-The text file can be partitioned in chapters by chapter lines. There are five types of chapter:
-• the Nameless chapter, the first one, from first line until first chapter line
-• the Numbered chapters, as this one
-• the automatic chapters, automatically emptied and refilled:
-• the Contents chapter, the list of chapters
-• the Index chapter, the list of subjects
-• the Figures chapter, the list of figure captions
+    , !   (
 
+ !  ! 
+
+  ( & 
+
+
+
+  YY    
+
+ '    
+
+
+
+& ,   (!   '
+
+
+
+ &   
+
+ Y YY &&Y,
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌────────────┬───────────┬──────┬────────┬────────┐
+
+│C
+│  │&W │ W │
+ d ────────
 
-│
+ │
+# 
 
+┤
+!
+│  │
+││  │
+  │
+│
+││
+│
+│ │
+ d !  
+ │ │
+│ 
+│
+│  │
+│ │  │
+│ IC  │
+│
+│ 
+│ 
+││  │  │
+│ 
+││  │  │
+│ CI
+│&& ││ │ │
+│ 
+│
+│ 
+│&& ││ │
+│&& ││ │   │
+│ 
+│ 
+│ && ││  │ │
+│ && ││
+│ 
+ │   │
+ │
+│&& ││ │
+│ 
+│
+│&& ││ │
+│
+│ &&
+││
+│
+ │
+│
+│
+ │
+│ 
+│ &&
+││
+│ &&
+││
+│ 
+│
+│
+│
+│ 
+│  &&
+││
+ │
+│&&│││  │
+│ 
+│  && ││  │ │
+│ 
+│ 
+│ && │ │ │ │
+│  && ││ │  │
+│ 
+│ 
+│ && │ │  │ │
+│&& │ │  │  │
+│ 
+│&& ││ │   │
+│ 
+│
+│ 
+│ && ││ │
+│ && ││ │
+│
+│
+ │
+│
+│&&
+││ │
+│ &&
+││
+│ 
+ │
+ │
+ │
+│
+│ &&
+││
+│ 
+│ 
+│&&
+││
+ │
+│
+│  && │││ │
+│"
+│"
+│  && ││  │ │
+│ && ││  │  │
+│"
+│"
+│&& │ │ │ │
+│&& ││
+│"
+ │ │
+│ && │ │  │
+│"
+ │
+ │
+│"
+│ && ││  │
+│&&
+│ │
+│"
+│
+│
+  │
+ │
+│"
+│ &&
+││
+│ &&
+││
+│"
+│
+│
+│
+ │
+│&&
+│ │
+│"
+│
+│
+│"
+│&&
+││
+│ &&
+│ │
+│"
+│
+│
+└────────────┴───────────┴──────┴────────┴────────┘
+
+ 
+
+   
+
+ & 
+
+& 
+
+
+
+&
+    $ Y Y  Y Y , !  YY 
+
+  $   &  ' !  
+ 
+
+  
+
+ ,
+
+    
+
+
+
+    ' &
+ ,
+ ,
+ ,
+ ,
 
-
-
-
-  │ 1 f│1   │
-
-
-
+
+
+
+
+ 
+(
 
-│Nameless│no
-│Numbered│no
-│Contents│yes
-│Index
-│yes
-│Figures │yes
+' 
 
-
+!
 
- 
+ 
 
-
+
 
-│
+ !   
 
-
+
 
-│max one │file top │no
-│no limit│everywhere│yes
-│max one │everywhere│yes
-│max one │everywhere│yes
-│max one │everywhere│yes
+ 
 
-
+  (( 
 
-
+'  
 
-
+  '  (    
+
+   
 
+
+
+    '
+
+(&   ( &  (  &,   &&&
+ &    &  (  &,   &&&
+&    &  (  &,   &&&
+'&&   '& &  (  &,   &&&
+
+   
+
+  &
+
+ 
+
+    &&    & 
 
 
-
-
-
-
-  fNE│IN Contents│EJECT IF -p c│ SEE │
-
+(( ' 
+
+    '$
+
+ & :
+
+ (   ((, (   &    !   $      
+ (    , (   &         
+ $      
+I( ! 
+   &       
+& , !    ( & &       
+ (,             , ! 
+     !    
+$   ! ,    
+! ( &     !  ,  !  $ r d  '
+ ,  ! '  (!    
+
+  
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+│ (
+& _! !, ,  
+│
+   !, ,  d & _! !, , 
+│
+ !        ( & !
+ & 
+│
+        ( & 
+ & 
+│
+   !    ( & 
+ & 
+  d !   ( & 
+│
+  
+ & 
+│
+ !    !    ( &   & 
+│
+         ( &   & 
+│
+  ( &     ( &   & 
+│
+ 
+ &     ( & 
+ & 
+│
+   &     ( & 
+ & 
+│
+  '& &     ( & 
+ & 
+│
+! d !        !   
+│
+ d            
+│
+( !!  
+!  !
+  $  !  
+│
+(   
+ i
+
+  $ 
+ 
+│
+( !  
+ !  
+  $    !
+│
+(    
+  i     $   
+│
+(  dd 
+ dd 
+ ! dd 
+│
+! d & __ _ _ _(
+│
+ d !!
+│
+d  
+(  dd 
+
+│
+ dd 
+ !
+│
+ d !!
+│
+d  
+│
+(  dd 
 
+
+ ! dd 
+ d 
+│
+│
+! d !
+│
+(  dd 
 
+
+ ! 
+ d & !! , 
+│
+│
+(  
+
+dd 
+ ! dd 
+│
+! d !
+│
+d  
+│
+(  
+
+dd 
+ ! 
+ d & , !!
+│
+│
+d  
+(  
 
-│no
-│yes
-│no
-│yes
-│yes
+│
+
+ ! dd 
+│
+ d & , 
+│
+! d !
+  
+
+
+│
+
+ ! 
+│
+ d & , !! , 
+
+!, , 
+│
 
 
 
-│no
-│4.1. │
-│level-1 only │4.2. │
-│yes
-│4.3.1.│
-│yes
-│4.3.2.│
-│yes
-│4.3.3.│
+
+
+'
+
+&  ! 
+
+ 
+
+ I  
+ 
+
+   &  
 
+    
+
+    ,
+
+
+
+   ( !
+
+ & 
+
+ I , &          (    (  , $   
+  , &          (  d  s   
+I
+   ! !   Y Y  &  '
+     I(  d ,   
 
+   s       C !,   
+  ((  ' $ 
+   
+        $         (  ,
+ !   ( 
+  '
+      '(   '   I      (  ! &  
+   !     I(    ,   &       & & &
+   &&    
+I
+
+ (!  !  
+    (      '
+    (   '   ( 
+  ' '    ( , 
+  $
+
+'  
 
+
+
+ 
+
+     
+
+  
+ ! YI Y,    (   (     ,   (   , ( (   
+ 
+     ,      $
+ ! YI Y,    (   (     ,   (   , ( (   
+
+     ,      $
+ ! YI Y,    (   (     ,   (   , ( (
 
+        ,      $
+  ( I
 
-
+,   '
+
+  !
+
+
+──────────────
 
-Figure 4.a. Chapter Types
+!
 
-      "   
+  !  
 
- no more than once in the file.
+&' &
 
-      "  "   everywhere and in any order, and are started by a
-chapter line. Chapter lines share some properties, each chapter line:
-• is the first line in text file or is preceded by an empty line
-• is the last line in text file or is followed by an empty line
-• is a not empty line and starts with a non-blank character
-Therefore we can say that a chapter line must be a one-line unindented text paragraph.
+ '
 
-  
+  YiY
 
-   "   he Contents one itself, are listed in the Contents
+             ,  
 
-  
+_
+ d 
+     ! 
+ 
 
-   "    not-level-1 Numbered ones, trigger a page break if
+((
 
-chapter.
+ 
 
-argument -p is 'c' (see 5.).
+  
 
-  
+ ,
 
-
+ (!
 
- 
+ C  I
+I( I
+  
 
- W    ""  " W  Wrst of the text file, and goes from the first line
-(included) until the first chapter line (excludeu fY  W W    
- W
-this User Manual, it can be the cover of the document.
- 
+d 
 
-
+  !   I
 
- 
+
 
-Start of a "Numbered chapter" is marked by a Nu"   W
-chapter line" if contains one or more blank-separated words, of which:
+  d ,   
 
-  W W  ""
+ s       
 
-• the first one is a "chapter label", made by one or more "int-dot couples", each made by:
-• one or more decimal digits, between '0' and '9'
-• a "decimal point" '.'
-• the following words, if any, are the chapter title
-The "level" of a Numbered chapter line is the count of int-dot couples in its label, examples:
-• 12345. a level-1 Numbered chapter line
-• 1.345. a level-2 Numbered chapter line
-• 0.0.0. a level-3 Numbered chapter line
-Numbered chapter lines must follow a couple of quite obvious sequence rules:
-• first Numbered chapter in the text file and any Numbered chapter next to an automatic chapter
-must be a level-1 chapter
-• any Numbered chapter next to another one can have any level between 1 and the level of the
-previous one plus one, but no more
-Numbered chapter titles are:
-• shrunk and uppercased where they are
-• shrunk and titlecased when inserted:
-• into Contents chapter
-• into page headers by '%c' (see 5.)
+
 
-" W W    "
+
 
-are free
-Example:
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-  " by the right ones, only the level matters. So you
-to create destroy or swap chapters as you like it, they will be automatically reNumbered.
+   (  
+(  
+' 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+(
+
 
-10/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ $ cat chapters.txt
-│       
+
+
+│
 │
-│ 32.33. bBb bBb 'bBb'
 │
-│ 0.0. cCc "cCc" cCc
 │
-│ 0. 'dDd dDd' dDd
 │
-│ 0.0. eEe 'eEe' "eEe"
 │
-│ 9.9.9. 'fFf fFf fFf'
 │
-│ 0.0. "gGg gGg gGg"
-│ $ yawp -M f -w 32 chapters.txt
-│ $ cat chapters.txt
 │
 │
-│ 1.1. BBB BBB 'BBB'
 │
-│ 1.2. CCC "cCc" CCC
 │
-│ 2. 'DDD DDD' DDD
+
+
+
+ 
+
+│
+│
+│
+│
 │
-│ 2.1. EEE 'EEE' "eEe"
 │
-│ 2.1.1. 'FFF FFF FFF'
 │
-│ 2.2. "gGg gGg gGg"
-Figure 4.2.a. Example Of Chapter Renumbering
 
 
 
-1 f   
+ 
+
 
-Contents, Index and Figures chapters are "automatic chapters", this means:
-• the file cannot contain more than one automatic chapter for each of the three types
-• all input lines after the automatic chapter line until the next chapter line (or until end of
-file) are supposed to be the old chapter content and are deleted
-• the new chapter content is automatically inserted after the chapter line
+│
+│
+│
+│
+│
 
-W
+
+
+│
+│
+│
+│
+│
 
-Yn Y   u
+
 
-chapter is
-example.
+ 
 
-fl
+│
+│
+│
 
-requested,
+│
+
+│
+│
+│
 
-  W
+│
 
-    Wed and pages are not Numbered. So, if an automatic
-it
+
 
-will
+
 
-still appear, but without page numbers aside, as in the following
+
 
-
+
 
-   W
+│
 
- 
+' 
 
- W 
+  
 
- W   
+C((, I d ,  ! 
 
-processing check the result and if needed go back to previous version by Undo mode.
+' 
 
-"W      n nW n  -F arguments, which must all be non-null strings.
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
+
+(
+
 
-Furthermore
-blanks.
+│
+│
+│
+│
 
 
 
--c
+
+│
+│
+│
+│
+│
+│
+│
 
-1 
+
 
--f
+┌─────────┬─────────┐
+│
+│
+├
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+└─────────┴─────────┘
 
-and
+
 
--i
+│
 
-must
+' 
 
-have,
+C((, I d ,  d 
+
 
-if uppercased, all distinct values, and -F cannot contain
+┌──────┬──────┐
+│
+│
+├
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+
+├─
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+├
+│
+│
+└──────┴──────┘
 
-  
+│
+│
+│
+│
+│
 
-For "Contents chapter" we mean an automatic chapter containing the list of chapters, in order of
-appearance, possibly with the number of the page they begin on. Namely, the Contents chapter will
-list all Numbered chapters, the Index chapter and the Figures chapter, but it won't list either the
-Nameless chapter or the Contents chapter itself.
-The Contents chapter line starting the Contents chapter is defined by -c argument:
-• "-c, --contents-title": title of Contents chapter (default: 'contents'), example:
-│ $ yawp -c 'list of chapters' ...
+
+│
 
-  W W     W W WY equivalent to -c. Such a line is:
-• shrunk and uppercased where it is
-• shrunk and titlecased when inserted into page headers by '%c' (see 5.)
-Example:
+ 
 
-4. Chapters
-11/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ $ cat Contents.txt
-│ Contents
 │
 │
-(any previous content
 │
-of Contents chapter
 │
-will be deleted)
+
+
+
+
+
 │
-│       
+
+' 
+C((, I d ,  d 
+
+   (  
+(  
+' 
+
+│ │
+
+│ │ │
 │
-│ 32.33. bBb bBb 'bBb'
 │
-│ 0.0. cCc "cCc" cCc
 │
-│ 0. 'dDd dDd' dDd
 │
-│ 0.0. eEe 'eEe' "eEe"
 │
-│ 9.9.9. 'fFf fFf fFf'
+
 │
-│ 0.0. "gGg gGg gGg"
-│ $ yawp -M f -w 32 Contents.txt
-│ $ cat Contents.txt
-│ Contents
 │
-  
 │
-
 │
-• 1.1.
-Bbb Bbb 'Bbb'
 │
-• 1.2.
-Ccc "cCc" Ccc
+
+
 │
-• 2.
-'Ddd Ddd' Ddd
 │
-• 2.1.
-Eee 'Eee' "eEe"
+ │ │ │
 │
-• 2.1.1. 'Fff Fff Fff'
 │
-• 2.2.
-"gGg gGg gGg"
 │
 │
 │
-│ 1.1. BBB BBB 'BBB'
+
 │
-│ 1.2. CCC "cCc" CCC
 │
-│ 2. 'DDD DDD' DDD
 │
-│ 2.1. EEE 'EEE' "eEe"
 │
-│ 2.1.1. 'FFF FFF FFF'
 │
-│ 2.2. "gGg gGg gGg"
-Figure 4.3.1.a. Example Of Contents Chapter
-
- "      W   
+
+
+
+
 
+
+
+
+(
+
+ 
+
+┌─────────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────────┘
 
-f
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
 
-of this Manual.
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
+
+(
+
 
-   
+
 
-For "Index chapter" we mean an automatic chapter containing a list of subjects, in alphabetical
-order, possibly showing which pages each "subject" is on. Subjects are sought in text lines only,
-therefore neither in pictures nor in captions nor W   W
-   
-• as a "quoted subject" if it's preceded and followed by a "double quote" '"' (but double quotes
-preceded or followed by a "single quote" "'" or by another double quote '"' are not taken into
-account, in order to allow things like '"' in text)
-• an "unquoted subject" otherwise
-Unquoted subjects are recognized everywhere if the text file contains at least one corresponding
-quoted subject somewhere. Hence in index chapter the line relating to a given subject will contain:
-• quoted (by '"') page numbers for pages containing one or more quoted instances of the subject
-(and zero or more unquoted instances)
-• unquoted page numbers for pages containing one or more unquoted instance of the subject and
-zero quoted instances
-Subject length
-computed.
+
 
-can
+
+│
 
-not
+ 
 
-be greater than half of -w argument, whether set by user or automatically
+
+│
+│
+│
 
-The Index chapter line starting the Index chapter is defined by -i argument:
-• "-i, --index-title": title of Index chapter (default: 'index'), example:
-│ $ yawp -i 'list of subjects' ...
+
+ │
+│
+│
 
-  W W  f   W W WY uivalent to -i. Such a line is:
-• shrunk and uppercased where it is
-• shrunk and titlecased when inserted:
-• into the Contents chapter
-• into page headers by '%c' (see 5.)
-For technical reasons, a subject cannot occupy more than one line in the Index chapter. Hence if a
-subject is referenced in many pages and the resulting line is longer than -w argument, then it's
-truncated and terminated by '...' with a warning message.
+
 
-12/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
- "   f   W   "  is Manual.
+┌────┬────┬────┬────┐
+├
+│ │ │ │
+├
+│
+│
+│
+│
+├
+│
+│
+│
+│
+
+├─
+├
+│
+│
+│
+│
+├
+│
+│
+│
+│
+├
+│
+│
+│
+│
+└────┴────┴────┴────┘
 
- 
+
 
-  
+│
 
-fl
+' 
 
-For "Figures chapter" we mean an automatic chapter containing a list of figure captions, in order of
-appearance, possibly showing which page a "caption" is on. Not all pictures need to be followed by a
-caption, and a caption without a picture does not make sense, so we can say a "figure" is a picture
-followed by a caption.
-Figures chapter is controlled by -f and -F arguments. The Figures chapter line starting the Figures
-chapter is defined by -f:
-• "-f, --figures-title": title of Figures chapter (default: 'figures'), example:
-│ $ yawp -f 'list of figures' ...
+C((, I d ,  d 
 
-  W W  W   W W WY quivalent to -f. Such a line is:
-• shrunk and uppercased where it is
-• shrunk and titlecased when inserted:
-• into the Contents chapter
-• into page headers by '%c' (see 5.)
+,     !   ' $             
+I( I   
+$         (   I( I d    d ,       ,
+   
+(
+( &   ( &        ' (   $  
+ 
 
-W  W  W  n
-• "-F, --caption-prefix": first word of figure captions (default: 'figure')
--F must be a single word, in other words it cannot contain blanks.
+  
 
-W W  " W  W W" W 
-• is a one-line picture, in other words:
-• is the first line in file or it's preceded by an empty line
-• is the last line in file or it's followed by an empty line
-• is a not empty line and starts with blank
-• contains two or more blank-separated words, of which:
-• the first one is equivalent to -F
-• the second one is a "caption label" containing:
-• the label of the containing chapter (label of Nameless chapter is null string '')
-• a progressive lowercase letter between 'a' and 'z', meaning caption position in the
-containing chapter
-• a decimal point '.'
-• the following words, if any, are the figure title
-Examples of caption labels are:
-• 'a.' (the first caption in the Nameless chapter)
-• '7.c.' (the third caption in the '7.' chapter)
-• '7.9.b.' (the second caption in the '7.9.' chapter)
-• '7.9.8.z.' (the 26th caption in the '7.9.8.' chapter)
+
 
-W    W "    Won lines, one for each letter of english alphabet.
-The input
-lines are:
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-caption
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
+
+
+│
+(
+(
+
 
-label
+
 
-can
+│
+│
+│
+│
+│
+│
+│
 
-be any, of any level, it's automatically updated on output. Caption
+
 
-• shrunk titlecased and centered where they are
-• shrunk and titlecased when listed in the Figures chapter
-The label letter always remains lowercase. Notice the difference between:
-• the Figures chapter line, one, defined by -f, starting the Figures chapter
-• the figure caption lines, many, defined by -F, listed in the Figures chapter
+  
 
-  
+
 
-
+
+│
 
-W
+┌─────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────┘
 
- W W W nected with previous picture, so, when applicable,
+│
+│
+│
+│
+│
+│
 
-figure caption lines are logically
-caption split across two pages.
+
 
- "  
+
 
-pasted
+│
 
-W   W   " 
+' 
 
-with
+C((, I d ,  d 
 
-previous picture, in order to avoid figure and
+I( I d 
+  , !  &  (  '    !     I
+( &     (     
+' (   $
+   
+
 
-this Manual.
+│
+│
+│
+│
+│
+│
+│
 
-13/37
-W
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
 
+(   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
 
+(
+
+
+
+
+┌───
+│
+│
+│
+│
+│
+│
+│
+└───
+
+│
+│
+│
+│
+│
+│
+│
+
+
+
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
 
+(
+
+
+┌─────────┬─────────┐   
+│
+│
+│
+│ ┌───────┴─┬───────┴─┐  
+│ │
+│
+│
+│ │
+│
+│
+│ │
+│
+│
+│ │
+│
+│
+│ │
+│
+│
+└─┤
+│
+│
+│
+│
+│
+└─────────┴─────────┘
+
+
+
+│
+
+  &,
+
+
+│
+│
+│
+│
+│
+│
+│
 
-lfl
+
 
-In format mode page headers in input are automatically deleted, then they can be reinserted (or not)
-under control of -p argument:
-• -p, --page-headers: insert page headers (default: 'n' = no, 'f' = on full page, 'p' = and on
-broken pictures, 'c' = and on level-1 Numbered Contents index or Figures chapters)
+┌─────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────┘
 
-W   Yn Y     Wed. So, if you want to eliminate page headers from
- W  
-W " " W Yn Y     W" "
-W Yn
+
 
-Y    W  t line does not fit into current page
+│
 
-W Yn
+$  (
+
 
-Y    W 
+
 
-• current line does not fit into current page
-• current picture does not fit into current page
+' 
 
-W Yn
+ ( 
 
-Y    W 
+C((, I d ,  d 
 
-• current line does not fit into current page
-• current picture does not fit into current page
-• current line is a level-1 Numbered or Contents or figures or Index chapter line
+I(  !   (    !    ,    $   $   I  
+ &,   (       ,
+ !  $      ,  i  d    
+   !     d  ,
+   &     ( &      
+&  ( ,
+
+' (  
+    I(  &' (      '
+ $   &' ( '    !   $ '  
+┌─────────┬─────────┐  
+│
+│
+│
+│ ┌───────┴─┬───────┴─┐  
+│
+│ │
+│
+│ │ ┌───────┴─┬───────┴─┐   
+ │
+│
+│ │ │
+│ │ │ ┌───────┴─┬───────┴─┐   
+│
+│
+│ │ │ │
+└─┤ │ │ ┌───────┴─┬───────┴─┐  
+│ │ │ │
+ │
+│
+└─┤ │ │
+│
+│
+│
+│
+│ │ │
+└─┤ │
+│
+│
+│
+│
+│ │
+└─┤
+│
+│
+│
+│
+│
+└─────────┴─────────┘
 
-W Yn
-Y  Yn Y W  W W  long to fit into the current page, a page eject is
-forced. But if the picture is higher than one page, such a page eject is useless and does not take
-place, see for example the figure 8.3.a.
-Each page, except the first one, is prefixed by a page header. Therefore the total number of pages
-is equal to the number of page headers plus one. Each page header is made up of two header lines:
-• first header line, starting with a "form feed" '\f' character, containing data such as file
-name, chapter title, date, time or page number
-• second header line, a separation line made of "macron" '¯' characters, which form a kind of
-dashed underline under the first header line
-The form feed character causes a page break but is a non-printable character, therefore it's not
-considered when measuring line lengths. Depending on your editor, it can appear as a quarter musical
-note or as a small rectangle.
+
 
-fl s  
+│
 
-line would disappear.
+$  (
+
 
- 
+
 
-fW
+   , 
 
- W W 
-W 
+┌─────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────┘
 
-'.py', -p is silently set to 'n'.
+
 
-
+│
 
-"
+' 
+C((, I d ,  d 
 
-   "    
+I( I d 
+  d ,       ,     ,   
+( &   ( &       
+' (   $
+   
 
-  
+ s
 
-W  not make sense, so if the text file name ends with
+
 
-The content of first header line is controlled by -e -E -o -O -n and -a arguments:
-• "-e, --even-left": headers of even pages, left (default: '%n/%N')
-• "-E, --even-right": headers of even pages, right (default: '%F %Y-%m-%d')
-• "-o, --odd-left": headers of odd pages, left (default: '%c')
-• "-O, --odd-right": headers of odd pages, right (default: '%n/%N')
-Each "percent variable" is evaluated as follows, no other percent variable is allowed.
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
 
-
-│!  │
-! 
-
-
-│Y' Y│text file "long path", without final '/'
 
-
-
+│
+│
+│
+│
+│i
+
+
+
+(
+
+│
+│
+│
+│
+│
 
 
 
-
+   (  
+(  
+' 
+
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+│i
+│ i
+i
+
+│
+
+│
+│
+│
+
+│
+│
+
+│
+│
+
+│
+│
+
+
+
+
+
+(
+
+ 
+
+
 
 │
+│
+│
+│
+│
+
+
+
+│
+│
+│
+│
+│
+
+
 
+ 
+
+┌──────┬──────┐
+│
+│
 │
-│'%p'│text file "short path", without final '/'
 │
-│'%f'│text file name, with no extension
 │
-│'%F'│text file name, with no extension, altered
 │
-│'%e'│text file extension, if any, with initial '.' │
-│'%Y'│current year, 4 digits
 │
-│'%m'│current month, 2 digits
 │
-│'%d'│current day, 2 digits
 │
-│'%H'│current hour, 2 digits
 │
-│'%M'│current minute, 2 digits
 │
-│'%S'│current second, 2 digits
 │
-│'%n'│current page number
 │
-│'%N'│total number of pages
 │
-│'%c'│current level-1/Contents/Figures/Index chapter│
-│'%%'│'%'
 │
+└──────┴──────┘
 
-
+
 
-W  
+
 
- !W
+
 
-  " " Y' Yu  " " Y' Y) mean? If for instance the current text
-file is '~/yyyy/zzz.www.txt' and the user is 'xxxx' then we get:
- Y' Y nn
+(
 
-Y "  Y
+' 
 
- Y'Y nn
+│
 
-Y  Y
+
 
-• '%p' --> '~/yyyy'
-• '%f' --> 'zzz.www'
-• '%e' --> '.txt'
+│
+│
+│
+│
+│i
 
- Y'
+
 
-' 'Y nn
+│
+│
+│
+│
+│
+
+
+
+$  
+ (
+
+┌──────┬──────┐   
+│
+│
+│
+│ ┌────┴─┬────┴─┐  
+│ │
+│
+│
+│ │
+│
+│
+│1│
+│
+│
+├─┤
+│
+│
+││i
+│i
+│
+
+
+
+
+
+ │
+│
+│ │
+│ │
+│
+│
+│ │
+│
+│
+└─┤
+│
+│
+│
+│
+│
+└──────┴──────┘
+
+C((, I d ,  d 
+
+ 
+
+┌──────┬──────┐
+ │
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+└──────┴──────┘
+
+
 
-Y "     Y
+│
+├
+├
+│
+├
+│
+├
+│
+├
+│
+└──────┘
 
-• '%p/%f%e' --> '~/yyyy/zzz.www.txt'
+
 
-  " W "" Y'Yu " We name is altered by '%F' as follows:
-• any special character is replaced by a blank
+(
 
-14/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-• resulting words are titlecased
+' 
 
- s 
+cut
 
-Y'Y W   
+│
 
-• "-n, --page-offset": offset of page numbers (default: '0', min: '-3999', if negative it is the
-count of initial Roman numbers)
+C((, I d ,  d 
+,    
+   
 
+   (  
+(  
+' 
 
+
+
+┌────┬────┐
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│i │i │i │i  i │i │i │ i │
+│i │i │
+
+
+ (──
+
+│ │  │
+
+│ │ │  │
+│
+│
+│  │
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+└────┴────┘
+
+
+
+
+
+
+
+
+
+
 
-
 │
+(
+(
+
+ 
+
+
 
- 
- 
- 
-l │ -5│ -4│ -3│ -2│ -1│
+
+
+I( I d 
+  d ,       ,    
+( &   ( &        ' (   $
+
+ 
+
+    I 
+   
+
+   (  
+(  
+' 
+
+┌──────┬──────
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+│i
+│ i
+│i
+│
+i
 
- 
- 
- 
+
+
+│
+│
+
+│
+ │
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+│
+│
+│
+│
+
+└──────┴──────
+
+
+
+(
+
+
+│
+
+ 
 
-0│
+cut
 
+│
+
+, !  &  (  '  '    !
+I( I d 
+ 
+  &, ( &     (      ' (   $
+(   (  
+(  
+' 
+
+
+│
+│
+│
+
+│
+│
+│
+
+│
+│
+│
+
+│
+│
+│
+
+│i
+│i
+│
+ i
+
+
+ │
+
+│
+│
+│
+│
+│
+
+│
+│
+│
+
+│
+│
+│
+
+│
+│
+│
+
+
+
 
+
+
+(
+
 
-
+
 
+│
+├
+├
+│
+├
+│
+├
 │
+├
+│
+└──────┘
 
-│ 1st│ i│ i│ i│ i│
-│ 2nd│ ii│ ii│ ii│ ii│
-│ 3rd│iii│iii│iii│ 1│
-│ 4th│ iv│ iv│ 1│ 2│
-│ 5th│ v│ 1│ 2│ 3│
-│ 6th│ 1│ 2│ 3│ 4│
-│ 7th│ 2│ 3│ 4│ 5│
-│ 8th│ 3│ 4│ 5│ 6│
-│ 9th│ 4│ 5│ 6│ 7│
-│10th│ 5│ 6│ 7│ 8│
+ $
 
-
+ 
+│
 
-
+┌────┬────┐
+│
+│  │
+│
+│
+│
+│
+│
+│
+└────┴────┘
 
--n, --page-offset
+
 
-
+├
+├
+│
+├
+│
+└────┘
 
-
+
 
-
+
 
-
+(
 
-
+' 
 
-
+│
 
-
+
+
+│
 
-1│
+cut
 
-
+│
 
-
+C((, I d ,  d 
 
-
+, !  &  (  '  '    !     I 
+I( 
+( &     (      ' (   $    
 
-2│
+  &,
 
-3│
+  
 
-
+
 
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+(   (  
+(  
+' 
+
+
+
+┌────┬────┐
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│i │i │i │i  i │ i │ i │ i │
+│i │i │
+
+
+
+ (─ 
+│ │ │  │ │  │ │
+│
+│
+│ │
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+└────┴────┘
+
+
+
+
+
+
+
+
+
+
+
+│
+(
+(
+
+   (  
+(  
+' 
+
+
+
+┌────┬────┐
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│ i │ i │
+│i │i │ i │ i i │i │i │i │
 
+
+ (─ 
+
+│  │ │ │
+│ │
+ │ │  │  │
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+└────┴────┘
+
+
+
+
+
+
+
+
+
+
+
+│
+(
+(
+
 
-
+cut
 
-4│
+│
+├
+├
+│
+├
+│
+└────┘
 
-
+
+
+
 
 │
 
-
+$    (
 
-5│
+I( I
+  
 
-
+
+
 
-i│ 1│ 2│ 3│ 4│ 5│ 6│
-1│ 2│ 3│ 4│ 5│ 6│ 7│
-2│ 3│ 4│ 5│ 6│ 7│ 8│
-3│ 4│ 5│ 6│ 7│ 8│ 9│
-4│ 5│ 6│ 7│ 8│ 9│ 10│
-5│ 6│ 7│ 8│ 9│ 10│ 11│
-6│ 7│ 8│ 9│ 10│ 11│ 12│
-7│ 8│ 9│ 10│ 11│ 12│ 13│
-8│ 9│ 10│ 11│ 12│ 13│ 14│
-9│ 10│ 11│ 12│ 13│ 14│ 15│
+
 
-
+│
 
-
+ 
 
-
+┌────┬────┐
+│  │
+│
+│
+│
+│
+│
+│
+│
+└────┴────┘
 
-
+cut
+│
 
-
+┌────┬────┐   
+│  │ │
+│ ┌──┴─┬──┴─┐  
+│
+│ │  │
+└─┤
+│
+│
+│
+│
+│
+└────┴────┘
 
-
+
+
+┌────┬────┐
+│
+│  │
+│
+│
+│
+│
+│
+│
+└────┴────┘
+
+' 
+
+  
+
+C((, I d ,  d 
+
+" 
+d 
+
+  !   I
+
+
 
-W   "'" ! 1   W 1 "n" "
-   
-• if -n argument is zero (the default), the numbering is the natural one, the first page is '1',
-the second is '2', and so on
-• if -n is more than zero, page numbers are incremented by -n, this can be useful if the text
-file is only a chapter of a larger document
-• if -n is less than zero, a number of lowercase-"Roman"-Numbered pages equal to the absolute
-
-s 
-
-n   " W"n"
-
-
-
-n W   "W
-Y "   take negative values. -n cannot be less than -3999
-because 3999 = 'mmmcmxcix' is the maximum standard Roman number.
-'%N' is still the total number of pages (Roman plu
-
-Wu  W      n "
-
-If you do not need front-back printing, set:
-• "-a, --all-pages-E-e": put in all page headers -E at left and -e at right
-and so you'll get the same header layout on even and odd pages. Notice the swap between -e and -E.
-
-" n   W      "W n d right margin -R:
-• if -a is off, left and right margins are swapped with each other on even pages
-• if -a is on, left and right margins stay in place on odd and even pages
+  d ,   
 
+   (  
+(  
+' 
+
+
+
+
+
+
+
+
+
 
+(
+
 
-
+
+
+│
+│
+│
+│
+│
+│
+│
+
+
+
+
+
+
+│
+│
+│
+│
+│
+
+
+
+│
+│
+│
+│
+│
 
 
 
 
 
-│-e
--E
-│¯¯¯¯¯¯¯¯
-│........
-│........
-│..even..
-│..page..
-│........
-│........
+
 
-W  
+
+│
+│
+│
+│
+│
+│
+│
+
+
+
+┌───────────────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└───────────────────┘
+
+
+
+│
+
+' 
+
+   C , I d ,  ! 
+
+   (  
+(  
+' 
+
+
+
+
+
+
+
+
+
+
+
+
+
 
+(
+
+
+
+ s       
+
+
+│
+
+┌─────────────┐
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+├─────────────┤
+│
+├
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────────┘
 
 │
 │
 │
 │
+
+
+│
+│
 │
 │
 │
+
+
+
+
+
 │
 
+' 
+
+'  C , I d ,  d 
+
+
+
+
+
+
+
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+│
+│
+
+
+│
+
+│
+│
+│
+
+│
+│
+
 
+
+
+
+(
+
 
-W  
+
 
 │
 │
 │
+
+
+
+│
 │
 │
+
+
+
+
+
 │
 │
 │
 
 
+│
 
--o
--O│
-¯¯¯¯¯¯¯¯│
-........│
-........│
-..odd...│
-..page..│
-........│
-........│
+
+
+│
+│
+
+
+
+│
+│
+
+
+
+│
+│
+
+
+
+│
+│
+
+
+
+
 
 
 
-  W "n"
-
+
 
--E
--e│
-¯¯¯¯¯¯¯¯│
-........│
-........│
-..even..│
-..page..│
-........│
-........│
+│
+│
+├
+├
+│
+│
+├
+│
+│
+└─────────┴─────────┘
 
-
+│
+│
+
+
+
+│
+
+' 
+
+   
+   (  
+(  
+' 
+
+│
+
+│
+│
+│
+
+
+│
+
+│
+│
+│
+
+
+│
+│
+
+│
+│
+
+
+
+│
+│
+│
+│
+
+
+
+
+
+(
+
 
-"n"
+┌─────────┬─────────┐
+├
+│
+│
+├
+│
+│
+├
+│
+│
 
- "n" Off
+C , I d ,  d 
 
-"n"
+
+│
+
+┌──────┬──────┐
+├
+│
+│
+├
+│
+│
+
+├─
+├
+│
+│
+├
+│
+│
+├─
+
+│
+├
+│
+├
+│
+│
+├─
+
+│
+├
+│
+├
+│
+│
+└──────┴──────┘
 
- "n" On
+│
 
 
+│
+│
 
--E
--e│
-¯¯¯¯¯¯¯¯│
-........│
-........│
-..odd...│
-..page..│
-........│
-........│
+
+│
+│
 
-
+
 
-  W "n"
+ │
+│
 
-6. Graphics
-15/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
 
- l f
+
 
-  " W"W  W
+│
 
-two "draw characters":
+' 
 
-
+   
 
- an sketch pictures with boxes arrows and tables by
+C , I d ,  d 
 
-• "back quote" '`' to draw horizontal and vertical "segments"
-• "circumflex accent" '^' to mark "arrowheads"
-If you turn on the argument:
-• "-g, --graphics": redraw '`'-segments and '^'-arrowheads
+,     !   ' $             
+I( I   
+$         (   I( I d    d ,       
+,  
+ ( &        ' (   $     I( I d   
+  &  
+
 
-W   W   W  
-and usage mode is Format or Noformat, then Y
-characters with suitable graphic ones, depending on the other four characters around (left right
-above and below). Standalone draw characters are not replaced.
-This feature works:
-• in Format mode: in picture lines only, but not in text lines
-• in Noformat mode: in all lines of the text file
+(
 
- " 
-│ $ cat graphics.txt
 │
-`````````````
-N
 │
-` x - y
-`
-^
 │
-x `
-`````````````
-````````
-`
 │
-`
-` x & y `
-`
-`N `N2 `
+│i
+
+
+
+│
 │
-`````````````
-` y
-````````
-`
 │
-`
-y - x `
-` 0` 0`
-^
 │
-`````````````
-` 1` 1`
-^ u
-S
 │
-` 2` 4`
-`
+
+
+
+   (  
+(  
+' 
+
+
+
+
+
+i
+
+
+
+
+
+
+
+
+(
+
+   
+
+I( I d    d , 
+ ' (   $
+
+
+│
+( │
 │
-`````
-`````
-` 3` 9`
-7`
-•••
+│i
+
+
+
+
+
 │
-
-
-
 │
-`````
-`````
-` 5` 25`
-5`
-••
-•
-••
 │
-^
-`
-` 6` 36`
-4` • •
-•
+
+
+
+    
+   
+
+
+
 │
-`
-`
-` 7` 49`
-3•••
-•
-•
 │
-`
-^
-` 8` 64`
-2`
-•••
 │
-`````
-`````
-` 9` 81`
-1`
-t
 │
-^`````` D `^````` C `^````` `10`100`
-0````````````````````^
 │
-`````
-`````
-````````
-0 1 2 3 4 5 6 7 8 9
+
+
+│
+
+
+
 │
 │
-`````````````````````````````````````````````````````````
 │
-` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` `
 │
-` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` `
+
+
+
+  ( 
+
+cut
+
+
+
 │
-` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` ` `
+
+' 
+C , I d ,  ! 
+
+,    
+
+   (  
+(  
+' 
+
 │
-` ``` ``` ` ``` ``` ``` ` ``` ``` ` ``` ``` ``` `
 │
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
-`
+
 │
-`````````````````````````````````````````````````````````
 │
-i
-1
-1
-1
-1
-1
-(-1)
+
+│i
+│ i
+i
+
+│
+
+│
 │
-
-
 │
-``` = ``` - ``` + ``` - ``` + ``` - ... =
-````````
-
+
 │
-4
-1
-3
-5
-7
-9
-i = 0 2i + 1
-│
-│
-```
-`
-```
-```
-` `
-```
-```
-```
-```
-```
-│
-` `
-`
-`
-`
-` `
-`
-`
-`
-` `
-` `
-│
-` `
-`
-```
-```
-```
-```
-```
-`
-```
-```
-│
-` `
-`
-`
-`
-`
-`
-` `
-`
-` `
-`
-│
-```
-`
-```
-```
-`
-```
-```
-`
-```
-```
-│
-│
-````` ```` ````` ```
-````` ````` ````` `
-` ```
-`
-│
-`
-` ` ` `
-` `` `
-`
-`
-`
-`
-`
-`
-│
-````` ````` `
-` `` ````` ````` ` `` `````
-`
-`
-│
-`
-` `
-` `
-`
-` `
-`
-`
-` `
-`
-`
-`
-`
-│
-`
-` ````` ````` ````` ````` `
-````` `
-` ``` `````
-│
-│
-`
-` `
-````` ``` ` ````` ````` ````` ````` ````` `````
-│
-` ``` `
-` ` ` ` ` ` `
-` `
-` `
-` `
-` `
-`
-│
-```
-`
-` ` ` ` ` ` `
-` ````` `
-` ````` `````
-`
-│
-` ``` `
-`
-` ` ` ` `
-` `
-`
-` ` `
-`
-`
-│
-`
-` ````` `
-` ` ``` ````` `
-````` ` ``` `````
-`
-│
-`
-│
-`
-` `
-` `
-` `
-` `
-` `````
-````` `````
-│
-`
-` `
-` `
-` ````` `
-`
-`
-` ` ` `````
-│
-`
-` `` `` ` ` `
-`
-````` `````
-````` `````
-│
-`
-` ` ` ` ` ` `````
-`
-`
-` ` ` `````
-│
-````` ``` ````` `
-`
-`
-`````
-````` `````
-│ $ yawp -M f -g graphics.txt
-
-16/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ $ cat graphics.txt
 │
-N
+
+
+
+
 
+(
+
+
+
+
+├
+│
+├
+│
+├
+│
+├
+│
+├
+│
+└─────────────┘
+
+  ( &    
+
+ 
+
 
+
 │
-│ x - y
 │
-
+│
+
+
+
+│
+│
+│
+
+
+
+┌─────────┬─────────┐
+│
+│
+│
+│
+│
+│
+│
+│
+│
+└─────────┴─────────┘
+
 
-  
+
+
+
+├
+│
+├
+│
+├
 │
-x │
+└─────────┘
+
+
+
+
+
+(
+
+' d
+
+│
+
+cut
+
 │
- 
+
+C , I d ,  d 
+
+, !  &  (  '  '    !
+I( I d 
+ 
+  &, ( &     (      ' (   $
+
+    I 
+   
+
+31
+  
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+(   (  
+(  
+' 
+
 │
 │
-│ x & y │
+
 │
-│N │N2 │
-
-  E
- 
-
 │
-│ y
+
+│i
+│i
+ i
+
+ │
+
+│
 │
-  
 │
+
 │
-y - x │
-│ 0│ 0│
-
 │
-│ 1│ 1│
-S
+
 
-
- u
+
+
+
+(
+
+
+
+
 │
-│ 2│ 4│
 │
- 
- 
-│ 3│ 9│
-7│
-│
-│
-6│
-•••
- 
- B 
- │ 4│ 16│
-│
-│ 5│ 25│
-5│
-••
-•
-••
- 
-  
-│
-│
-│ 6│ 36│
-4│ • •
-•
-
+│i
+
+
+
 │
 │
 │
-│ 7│ 49│
-3•••
-•
-•
+
+
+
+$  
+ (
+
+
+
 │
 │
-│ 8│ 64│
-2│
-•••
-
-│ 9│ 81│
-1│
-t
 │
-  
- 
- D 
- C 
+
 
+│
 │
-│10│100│
-0
-
- 
- 
-  
 │
-0 1 2 3 4 5 6 7 8 9
+
+
+
+┌────
 │
 │
-                        
+│i
+├────
 │
-│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
 │
-│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
 │
-│ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │ │
+└────
+
+┌─────────┬─────────┐   
+│
+│
+│
+│ ┌───────┴─┬───────┴─┐  
+│1│
+│
 │
-│   │    │   │ └   │
+├─┤
 │
 │
+│ │i
+│i
 │
+
+
+
+
+
+ │
+│
+│ │
+└─┤
 │
 │
+│
 │
 │
+└─────────┴─────────┘
+
+   (  
+(  
+' 
+
 │
 │
+
 │
 │
+
+│ i
+│i
+i
+
+│
+
+│
 │
 │
+
 │
 │
+
+
+
+
+
+(
+
+
+┌─────────┬─────────┐
+ │
+│
 │
-   
 │
- 
- 
- 
-  
- 
 │
 │
-i
 │
-1
-1
-1
-1
-1
-(-1)
-
-
 │
-=
-+
-+
-- ... =
-
 │
-4
-1
-3
-5
-7
-9
-i = 0 2i + 1
+└─────────┴─────────┘
+
+
+
 │
+
+
+
 │
 │
- 
-
- │ │
-
+
+
+
+
+
+│
+├
+├
+│
+├
+│
+└─────────┘
+
+cut
+
+
+
+' 
+
+     ( &      
+
+   (  
+(  
+' 
 
+
 
-   
 │
-│ │
 │
 │
 │
-│ │
+
+│i
+│i
+│i
 │
+i
+
+
+
+│
+
+ │
 │
+( │
 │
-│ │
-│ │
- 
-  
-   
 │
-│ │
 │
 │
-   
 │
-│ │
+
+
+
+┌──────┬──────┐
+ 
 │
 │
 │
+│ ( │
 │
 │
+
+│i
+│i
 │ │
+│i
+│i
+│
+│i
+ i
+
+
+  
+─┤
+│
+1│
+│
+ │
+
+│
+ │
+ │
 │
-│ │
 │
 │
 │
 │
 │
- 
+│
+
+└──────┴──────┘
+
+
+
 
 
-
- 
- 
-
-│
-
-   
- 
 
+(
+
+
+
+
+│
+
+  C , I d ,  d 
+
+I( I d    d ,       , 
+
+' (   $
+   
+
+
+
+│
+│
+│
+
+│
+
+(
+
+
 
+
+
+
 
-
+
+
+│
+
+cut
+
+
+
+
+
+
+
+
+cut
+
+(
+
+' 
+
+┌──────┬──────┐
 │
+ │
+│
 │
 │
 │
+└──────┴──────┘
 │
+
+├
+├
+
 │
-│ │ │ │
-│  │
+
 │
+
+  C , I d ,  d 
+
+I( I d 
+  , !  &  (  '  '    !     I
+  &, ( &     (     
+' (   $
+   
+(   (  
+(  
+' 
+
+
+
 │
 │
 │
 │
+
+│i
+│i
+│i
 │
+i
+
+
+
+│
+
+ │
 │
-│  
 │
 │
 │
-   │
-  
-
-
 │
 │
-│ │
-│ │
+
+┌──────┬──────┐
+
+
+( 
 │
-│ │
 │
 │
-│ │
 │
 │
 │
 │
- 
-  
-  │ │ 
- 
+
+│i
+│ i
 │
+│i
+│i
 │
-│ 
+│i
+ i
+
+
+ ( 
+───┤
 │
 │
+│
+
+│
+│
+│
+│
 │
 │
-│ │
-     │     
-   
-
 │
-│   │
-│ │ │ │ │ │ │
-│ │
-│ │
-│ │
-│ │
 │
- │
- │
 │
 │
-│ │ │ │ │ │ │
-│ 
-│    
- 
 │
-│   │
+
+└──────┴──────┘
+
+
+
+
+
+
+(
+
+
+┌──────┬──────┐
 │
-│ │ │ │ │
-│ │
+│
+│
 │
-│ │ │
 │
 │
+└──────┴──────┘
+
+
+
+
+
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+(
+
+   (  
+(  
+' 
+
+
+
 │
 │
-│ 
 │
-│ │   
 │
- │
-  │ 
-
+
+│i
+│i
+i │i │
+
+
+
+│
+│
+
+│
+ │
+│
 │
+│
+│
+
+
+
 
-   
 │
 │
-│ │
-│ │
-│ │
-│ │
 │
 │
+
+│ i
+│ i
+i │i │
+
+
+ (
+│
+│
+ │
 │
-│ │
-│ │
-│    │
+
 │
 │
-│ │ │ 
 │
 │
-│ │
-│ │ │ │
+
+
+
+
+
+
+
+(
+
+
+┌──────┬──────┐   
+│
+│
+│
+│ ┌────┴─┬────┴─┐  
+│
+│
+└─┤
+│
+│
+│
+└──────┴──────┘
+
+
+
+│
+
+$    (
+   
+
+┌──────┬──────┐
 │
-    
-   
 │
 │
-│   │ │ │   
+│ i
+│ i
 │
+───┤
+
+│
 │
-│ │ │ 
-       │
+│
+│
+│
+│
+└──────┴──────┘
+
+
+
+
+│
+
+cut
+
 
-   
+
+
+
+
+cut
+
+├
+├
+
 │
+
 │
+
+' 
+C , I d ,  d 
+
+┌──────┬──────┐
+│
 │
+│
+│
+│
+│
+└──────┴──────┘
 
-W  
+33
+  $ 
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-"  W "n"
+  # I
 
-" n  W Yn Y     draw picture files without the need for a blank at
-WW   W  W
-W  "  W
-    W  " "
-  W W  W W   example, we want to print a small chessboard. Some
+  
+ 
+Y   
 
-remarks:
+  
 
-• '-M n' prevents formatting the file as text, but the backup is still performed because '-g'
-alters the text file
-   Yn Y  Yn Y "  W  up all available space between left and right
-margins
+
 
- Yn
+   (
 
-Y  "  W  W      WW W  
+'  
 
-you get a square chessboard of about 18x18cm, 7x7in
+ $ ( !   
 
-│ $ cat chessboard.txt
-│ `````````````````
-│ ` `X` `X` `X` `X`
-│ `````````````````
-│ `X` `X` `X` `X` `
-│ `````````````````
-│ ` `X` `X` `X` `X`
-│ `````````````````
-│ `X` `X` `X` `X` `
-│ `````````````````
-│ ` `X` `X` `X` `X`
-│ `````````````````
-│ `X` `X` `X` `X` `
-│ `````````````````
-│ ` `X` `X` `X` `X`
-│ `````````````````
-│ `X` `X` `X` `X` `
-│ `````````````````
+┌───────────────┬─────────────────────────────────────────────┬───┬───┬────┐
+│I │"I │ │
 │
+I   │
+I  
+
 
- n  n n
+
+
+
 
-n  
+│ (
+│  ( ! !
+│ │ C ││
+│  ( ! !
+│ │ C ││
+│  (
+│  (│  ( ! !
+│ │ ││
+│ │ C ││
+│  &  ( │  ! (  
+│'   (
+│  ! (   &    ' 
+│ │ ││
+│  ! ( 
+│ │ │ │
+│ (
+│  ! ( 
+│ │ │ │
+│ (
+│&
+│ │ ││
+ ( │   !   &     &
+│&   ( │   !   &     &i(│ │ ││
+└───────────────┴─────────────────────────────────────────────┴───┴───┴────┘
 
-
+
 
-6. Graphics
-17/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ $ cat chessboard.txt
-│         
-│ │ │X│ │X│ │X│ │X│
-│         
-│ │X│ │X│ │X│ │X│ │
-│         
-│ │ │X│ │X│ │X│ │X│
-│         
-│ │X│ │X│ │X│ │X│ │
-│         
-│ │ │X│ │X│ │X│ │X│
-│         
-│ │X│ │X│ │X│ │X│ │
-│         
-│ │ │X│ │X│ │X│ │X│
-│         
-│ │X│ │X│ │X│ │X│ │
-│         
+
+   (
 
-W  
+ $ 
 
-" 
+  (     (
 
-W "n  n n
+   $  '
+    (
+ ,  
 
-"
+ 
 
-18/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+
+
 
 
 
-  1fl
+  
 
-In Format Noformat and Undo mode the text file is   W 
-• "-X, --export-pdf": after processing export and 
+ &  (
 
-
+ (
 
-
+  , Y Y Y (Y
 
-
+   I & ' 
 
-W W
+ Y Y
 
-preview and print.
+( (    
 
-  W
+  "I &
 
- 
+   (,  $ (  '   '  (,     '  
+    ' ( &         , !   (    (
+ &     $ (  $ !
+ IC 
 
-  " 
+IC
 
- sW  
+I
 
-  
+  I & 
+       ,    &, & 
+   
+(
+ (    & (     (,    ,   $  
+s  
+(
+ ( ! !
+
 
- "n  nn Wn  "  
+   $  I &  
 
- W W
+  
 
-" n W 
+' 
 
- W
+   ( 
+   $ ! _(  & ,   Y !  &Y, 
+ (
+     ( &   & 
+   ( 
+ (  !    $ !  _(  & ,   Y !Y, 
+     ( &   $   $  ( (   (   ( , 
+  
+    (,      ( &  
+( ,
+ ! 
+ ' (  ' ! C    " '   '(  '    '   & 
+( &    '  
+C(  , (  
 
-   W sW  u  
+ &   
 
- W set the argument:
+ 
 
- W   Y'f.pdf')
+  ,   
 
- sW W n  s   Wned in figure 5.c., but '%n' '%N' and '%c' are not
- W    Y' Y  Y' Y  th allowed but give the same result. The resulting
+ !     ! !
 
-file name must end with lowercase '.pdf'.
+│
 
-The resulting file name can be prefixed by a path or not. If path is given, it must exist, otherwise
-the directory containing text_file is assumed.
+  (     (   ( ! '  &  '  
+I
 
-f 
+"I &  _(
 
- W  W W W W srwritten.
+ &   &
 
- W W  W  n
+   ( 
 
- n "
+  
 
- "n  nnnW"  W   Y' = automatic, unit: 'pt' 'in' 'mm' or 'cm')
-Value is an integer or float literal followed by a lowercase unit suffix:
-• 'pt' for points (1 inch = 72 points)
-• 'in' for inches
-• 'mm' for millimeters
-• 'cm' for centimeters
-so for instance these are all equivalent, giving a value of one inch:
+   
 
- n  
-W
- n
- n  ""
- n
- "
-You can also use comma ',' as decimal separator, '2,54cm' = '2.54cm'.
-There is no default unit, the suffix is mandatory. Only a zero value (as '0' or '0.0') can lack the
-suffix, because of course 0pt = 0in = 0mm = 0cm. B   s  n " ""W"
+
 
- n   Wu    ence automatic, namely:
+
 
- n
- W
- W
- W
+ &$   (, 
+&
 
-n W "W  n W  n W "  " n
-n W "W  n W  n W "  from -w
- n  n  "W
+│
 
-• -w is deduced from max body line length in file (page headers are not considered)
+
 
- n W "  " n
+ (
+ " 
 
-Character proportions are defined by:
+ & 
 
- "n  nnn "    W  har width / char height (default: '3/5', '1' =
-square grid)
+C
 
-n W  W  W  
-• a positive integer or float literal (as '1' or '0.6')
-• two positive integer or float literals, separated by a "slash" '/' (as '3/5')
-Dimensions
+IC
 
- n
+ ( ! !
 
-of
+ I  $   
 
-the paper sheet, expressed in points inches millimeters or centimeters (as explained
+   ( ! '
 
- u   W  n 
+( 
 
-• "-S, --paper-size": portrait paper size width x W   Y
-'mm' or 'cm')
+I
 
-Y  Y  ""Y Y Y YWY
+  I & (    '    &  
+ (         (
 
-Format is portrait, in other words must width cannot be greater than height.
-Values
+( & 
 
-can
+   ,  
 
-Y Y 
+
 
-be
+& (
 
-paper
+
 
-format
+& 
 
-names too, see the following table. These names are case-insensitive
+ ( ! !
+    
+& ( 
 
-Y Y W  "u W  YY  tor and the unit suffix in the explicit value must
+ &
 
-be lowercase.
+ $     , 
 
-19/37
-   W
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+    '   
+   
+    (,  
+I
 
-
-
-
-│1    │
+"I &    ( 
+
+
+
+         ,
+
+    
+
+  (   , 
+
+
+
+ &$    (, 
 │
-! 
-
-
-
-│ n   │5.5x8.5in │
-│LETTER
-│8.5x11.0in │
-│ l 
-│8.5x14.0in │
-│3f1n l │5.0x8.0in │
-│LEDGER
-│11.0x17.0in│
-│ 1f
-│11.0x17.0in│
-│ 
-│841x1189mm │
-│
-│594x841mm │
-│
-│420x594mm │
-│ 
-│297x420mm │
+
+ (
+
+
+
+ "C
+
+"IC 
+
+&
+
+ ( ! !
+
+ I  $    (
+"C
+
+  ( ! ' &
+
+"IC I
+
+  (    (   ( & ' " $     &&
+      $  
+ & , &  !
+  d  &' ( 
+
+  
+
+ , (
+
+d
+
+ &      '
+
+34
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+  d  &' (     , ( d
+   (d (   &  , $     
+    d     &  , $     
+
+   d    &  , $     
+   '&d '&   &  , $     
+  
+
+
+
+ &  
+
+  &
+
+ , '   
+
+(  & (
+
+    
+
+!!!&  &  &
+ ( 
+, '        (     '$     , ' 
+&
+(( '  '      &&    &     
+   &      ,     '  
+   !     ,     '   
+ 
+  
+            ((  ,   
+((  
+
+
+
+   &  '
+
+& & 
+            $   '   (  ( 
+ Y Y d Y &&Y, '       , 
+ C((       
+ 
+
+( &  
+     &   ((    ,    &   ((  
+   
+"
+
+ 
+
+
+    ' "
+
+ & 
+
+" ,
+     
+$  , Y Yd , Y(Yd'   (
+
+ '  
+
+
+
+
+
+
+
+   &   (
+
+ YYd' (
+
+
+
+( Y  ( ! ! Y, 
+
+ ! Y" Y,
+  (
+ ! Y" Y, 
+ ! Y" (Y, 
+
+ 
+
+
+
+ 
+ 
+
+   ,  
+
+(   &   &   ( 
+
+  ( & ' (  $  
+  ( & ' $     ( & 
+
+
+
+(
+
+(  $    $ '  !  (     Y Y d Y &&Y, '   
+ C((         ( &  
+   , 
+     &  
+((    ,    &   ((     $      (,  
+ (
+( 
+'   '
 │
-│210x297mm │
-│ 
-│148x210mm │
-│105x148mm │
-│ 
-│ 
-│74x105mm
+
+  
+
+ !
+
+ ( ! !
+
+'
+
+  '   ' 
+    ' ( & ' 
+      $     '   
+ !
+
+ 
+
+  & , ( 
+
+ $ (,   &    
+&$  
+
+
 │
-│ 
-│52x74mm
+
+  ! '
+ & ( 
+
+ton
+
+&
+
+(
+ ( ! !
+
+&      (
+
+
+( (!, 
+
+!
+
+   
+
+ 
+
+     (
+
+  $  
+
+ 
+
 │
-│ 
-│37x52mm
+   ( ! !
+│
+│  ┌──────────────────────────┐
+│
+│  │  ( ! !
+│  └──────────────────────────┘
+│
+│ & && &&     ( & 
+│ & &&  &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│
+│ & && &&     ( & 
+│ & &&  &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & &&  &&
+│ & &&
+&&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│
+│  & && &&      & 
+
+ 
+
+35
+  $ 
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│
+│  & && &&     ( & 
+│  & &&  &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+│  & && &&
+&&
+│  & &&
+│  & &&  &&
+│  & &&  &&
+│  & && &&
 │
-│ 
-│26x37mm
+│ & && &&      & 
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & &&
+&&
+│ & &&  &&
+│ & &&  &&
 │
-│B0
-│1000x1414mm│
-│B1
-│707x1000mm │
-│B1+
-│720x1020mm │
-│B2
-│500x707mm │
-│B2+
-│520x720mm │
-│B3
-│353x500mm │
-│B4
-│250x353mm │
-│B5
-│176x250mm │
-│B6
-│125x176mm │
-│B7
-│88x125mm
+│ & && &&      & 
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & && &&
+│ & &&  &&
+&&
+│ & &&
+│ & &&
+&&
+│ & && &&
+│ & && &&
 │
-│B8
-│62x88mm
+│ '& &&  &&     '& & 
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
 │
-│B9
-│44x62mm
+│ '& && &&     '& & 
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& && &&
+│ '& &&  &&
 │
-│B10
-│31x44mm
+│ ! &&  &&     
+ !
 │
+│ ! && &&     
+ !
+│
+│  && &&     
+ 
+│
+│  &&   &&     
+ 
 
-
+
 
-
+   "
 
-
+  
 
-Figure 7.a. Symbolic Names For "-S"
+(
 
-  W  W    W  other by -Z:
-• "-Z, --landscape": turn page by 90 degrees (default: portrait)
-Unprintable margins around the paper sheet are controlled by:
-• "-L, --left-margin": left margin (default: '2cm' = min, unit: 'pt' 'in' 'mm' or 'cm')
-• "-R, --right-margin": right margin (default: '2cm' = min, unit: 'pt' 'in' 'mm' or 'cm')
-• "-T, --top-margin": top margin (default: '2cm' = min, unit: 'pt' 'in' 'mm' or 'cm')
-• "-B, --bottom-margin": bottom margin (default: '2cm' = min, unit: 'pt' 'in' 'mm' or 'cm')
-Margins are expressed in points inches millimeters or centimeters as explained above.
-Left and right margins are affected by -a argument:
-• if -a is off, left and right margins are swapped with each other on even pages
-• if -a is on, left and right margins stay in place on odd and even pages
-Computations about geometry of characters and p  W W 
-characters per line is automatic, it has to be computed from the character width:
-chars-per-line =
+ #  
 
-  " 
+   ,      YY&& 
+   (    
+ &  
+(              ( & Y  Y, ! 
+  !    &  
+  
+ Y&Y    ( & 
+ Y &Y     & 
+ Y&Y     & 
 
-page-width - left-margin - right-margin
-char-width
+! $  
 
-   W W "W W   e computed from the number of characters per line:
-char-width =
+
 
-page-width - left-margin - right-margin
-chars-per-line
+
 
-Now we can compute the character height and the number of lines per page:
-char-height =
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-char-width
-char-aspect
+ Y'&Y    '& &
+ Y!Y    
+
 
-lines-per-page =
+
+!
 
-page-height - top-margin - bottom-margin
-char-height
+ YY    
+ 
+ Y&Y    ( & 
+ Y &Y     & 
+ Y&Y     & 
+ Y'&Y    '& & 
+ Y!Y      !
+ YY      
+     $        &&    & 
+  
+'   $        &&    & 
+   , Y    (     , Y& && &&Y  &   , '    
+  
+  !  ((, " d Y Y,   d Y&&Y  d && , !  $ &   '  
+  &   ( &  ( &&     d &&   (  ( ! !
+  &  
+( & 
+( &&     d && , !   $   && 
+ &  Y  (Y
+s $    &&  d &&  , $
+ (    
+!  ( &   
+ 
+ , !            (( , !   (   d (&
+   !   &    $  
+
 
-20/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-8. RESERVED FILES
+  ,   Y&Y, ! 
+   
 
-W 
+
 
-    W   
+ $  ,  , ! 
 
-technicalities about these files.
+&  
 
-
+
 
-
+ ,
 
-f 
+&
 
-│
+ 
 
-
+ ,  
 
-f
+ d (& d 
+, 
+    
+ ,  
+   ' , 
+ ,  
 
-│
+,  
 
-
+(   $
 
-
+'     
 
-hidden reserved files, and this chapter ilustrates
+
+ d (& d  ────
+
+,  , ,
+ !  
+ ,  
+       '  !  
 
-  
+,  
 
-
+
 
-
+( 
 
-
+ $
 
-
+' 
 
-
+  
 
-
+ d (& d     
 
-│SEE │
+─────────
 
-│session file
-│~/.yawp/.yawp.sess
-│8.1.│
-│history file
-│~/.yawp/.yawp.hist
-│8.2.│
-│correction file│~/.yawp/.yawp.corr
-│8.3.│
-│log files
-│~/.yawp/.yawp.%Y.%m.%d-%H.%M.%S.log │8.4.│
-│argument files │'
-│8.5.│
- ' ' 
-│lock files
-│'
-│8.6.│
- ' ' 
-│temporary files│'
-│8.7.│
- ' ' "
-│backup files
-│'
- ' ' ' '" 'n' ' ' ack│8.8.│
+  
 
-
+    &     ,   ,  , ,  , ,  ,  ,   ( 
+ d (&   &  '   s    (  '   ,  , ,  ,
+,  , 
+
 
-
+, (      
 
-Figure 8.a. Hidden Reserved Files
+ 
 
- sW
+   
+&  ,
+ ( !
+ !   I &,    (   
+s  &    ' '  ,    !    
+, ( ! 
+ ,  (&             
+  & 
+ ,       
+ !
+  & 
+  !      !   
+ !
+ !        ,  ! '
+
 
-text file.
+&$  
 
-
+
 
-f1
+(, 
+│
 
-
+
+   I  $ 
+(    
+
 
-
+  
 
- W W W    Y' Y Y' Y  Y'Y   
+  ' (& 
 
-   
+&
 
-f1 f
+ ( ! !
+
 
- W 
- W
-
+ 
 
-file:
+&     
 
-
+( ! '
 
-W lf " W  "Won". Each session can process, one at a time, more
-"     We, at session end, is saved into an unique session
+ 
 
-~/.yawp/.yawp.sess
+! 
 
-
+   I
 
-W Ws W lf " W   ssion begins:
-W Ws W _file
-processed is taken from the argument
+I I &, ( 
 
- W
+ (  (  &
+ &
 
-argument,
+
 
-as
+
 
-in
+ 
 
-'yawp exemple.txt', text file to be
+ & 
 
-W
-W Ws W _file argument, as in 'yawp', text file to be
-processed is taken from the previously saved '~/.yawp/.yawp.sess' file, if any
+  $  
+ ! &
 
- W
+
 
-In CLI modes the session file is not used.
+ & 
 
-
+
 
-   1 
+
 
-f 1
+   ( &
+ &  (    , (  (  ! 
+ &  (   ( ,
+ &      (  $  
+  
+  $  
+ &  (    ( & 
+ &  ( ! $  
+( '&   
+  $  
+ &  (  Y  
+    
+ &     '!
+   (   &  (
+C 
 
-f
+ &  !
 
- W lf "  W W   W  ormat or Noformat or Undo action, path and name of
+I "I &
+
 
-the file are recorded into the history file
-~/.yawp/.yawp.hist
+&$
 
-Such entries are managed avoiding duplications, in descending chronological order, until a max limit
-of 20.
-You can access history in order to select the next text file to be processed, or clear the history
-file, by the Recent button, see 2.2.2.
-In CLI modes the history file is not used.
+ (
 
- 
+ & 
+
 
-1 f1
+
 
-
+ $  
 
-1 f1 f
+I    (
 
-
-  
- W W  "  
-W   sW "
+$
 
-sWa the "lp" Unix command. Geometry is controlled by
+ (
 
-• -o cpi=N (number of characters per inch, default=10)
-• -o lpi=N (number of lines per inch, default=6)
-• -o page-left=N (left page margin, value in points)
-• -o page-right=N (right page margin, value in points)
-• -o page-top=N (top page margin, value in points)
-• -o page-bottom=N (bottom page margin, value in points)
-These options are undocumented in the lp man page, but you can find them for instance in:
-https://www.computerhope.com/unix/ulp.htm
+ 
 
-   WW 
-    WW 
+ !  
 
- W  paper the above options are not respected, but are
-W " " ""and the same thing happens. Namely:
+  ( &  "I   ( 
 
-• page margins are enlarged, so they need to be reduced
-• character width and height are reduced, so they need to be enlarged
-• in portrait and landscape orientation errors are different, and so corrections must be
-different
+ &  ( ( &  
 
-W    . This device has been tuned for the default paper
-"W" W
-W Y Y  Y  ""Y  W      n  1 W   W
-W  "   W  " t different results, and so you may need different
-correction points.
+ 
 
-Corrections are controlled by -C argument:
-• "-C, --correct-sizes": correct character
-values, 'n' = no, 'f' = by correction file)
+    , 
+│
 
-size
+&  !i
 
-and page margins (default: 'd' = by default
+
 
-and by the correction file '~/.yawp/.yawp.corr', if exists:
+ &  (  
 
-8. Reserved Files
-21/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-• if -C is 'n', no correction takes place, and we can make experiments in order to define
-content of correction file
-• if -C is 'd', the default corrections are applied
-• if -C is 'f', correction point are read from correction file
+
 
- "   W
+ I
 
-W   ing to the default corrections:
+  $ 
 
-│ # 
-
-│ # │ ~/.yawp/.yawp.corr │
-
-│ # 
-│
-│ plm 0mm 7mm # portrait left margin
-│ plm 10mm 16mm
-│ plm 20mm 24mm
-│ plm 30mm 35mm
-│ plm 40mm 43mm
-│ plm 50mm 52mm
-│ plm 60mm 62mm
-│ plm 70mm 72.5mm
-│ plm 80mm 83mm
-│ plm 90mm 92mm
-│ plm 100mm 101mm
-│
-│ llm 5mm 16mm # landscape left margin
-│ llm 10mm 20.5mm
-│ llm 20mm 29.5mm
-│ llm 30mm 39mm
-│ llm 40mm 48mm
-│ llm 50mm 57mm
-│ llm 60mm 66.5mm
-│ llm 70mm 75.5mm
-│ llm 80mm 84.5mm
-│ llm 90mm 94mm
-│ llm 100mm 104mm
-│
-│ prm 0mm 7mm # portrait right margin
-│ prm 10mm 15mm
-│ prm 20mm 25.5mm
-│ prm 30mm 34.5mm
-│ prm 40mm 44.5mm
-│ prm 50mm 54.5mm
-│ prm 60mm 64.5mm
-│ prm 70mm 72mm
-│ prm 80mm 81mm
-│ prm 90mm 91.5mm
-│ prm 100mm 100mm
-│
-│ lrm 5mm 17mm # landscape left margin
-│ lrm 10mm 22mm
-│ lrm 20mm 30mm
-│ lrm 30mm 40mm
-│ lrm 40mm 49.5mm
-│ lrm 50mm 58mm
-│ lrm 60mm 68mm
-│ lrm 70mm 77.5mm
-│ lrm 80mm 86mm
-│ lrm 90mm 96mm
-│ lrm 100mm 104mm
-│
-│ ptm 0mm 2mm # portrait top margin
-│ ptm 10mm 11.5mm
-│ ptm 20mm 21mm
-│ ptm 30mm 30.5mm
-│ ptm 40mm 39.5mm
-│ ptm 50mm 49mm
-│ ptm 60mm 59mm
-│ ptm 70mm 68mm
-│ ptm 80mm 77.5mm
-│ ptm 90mm 87mm
-│ ptm 100mm 96mm
-│
-│ ltm 5mm 7mm # landscape top margin
-│ ltm 10mm 11mm
-│ ltm 20mm 20.5mm
-│ ltm 30mm 30mm
-│ ltm 40mm 39mm
-│ ltm 50mm 48.5mm
-│ ltm 60mm 57.5mm
-│ ltm 70mm 67mm
-│ ltm 80mm 76mm
-│ ltm 90mm 85mm
-│ ltm 100mm 95mm
-│
-│ pbm 0mm 16mm # portrait bottom margin
-│ pbm 10mm 24mm
-│ pbm 20mm 34mm
-│ pbm 30mm 43mm
-│ pbm 40mm 52.5mm
-│ pbm 50mm 62mm
-│ pbm 60mm 71mm
-│ pbm 70mm 81mm
-
-22/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-│ pbm 80mm 90mm
-│ pbm 90mm 100mm
-│ pbm 100mm 109.5mm
-│
-│ lbm 5mm 19mm # landscape bottom margin
-│ lbm 10mm 24mm
-│ lbm 20mm 32mm
-│ lbm 30mm 42mm
-│ lbm 40mm 52mm
-│ lbm 50mm 60mm
-│ lbm 60mm 70mm
-│ lbm 70mm 80mm
-│ lbm 80mm 88mm
-│ lbm 90mm 99mm
-│ lbm 100mm 107mm
-│
-│ pcw 100mm 94.674mm # portrait character width
-│
-│ lcw 100mm 92.200mm # landscape character width
-│
-│ pch 100mm 94.358mm # portrait character height
-│
-│ lch 100mm 92.647mm # landscape character height
-Figure 8.3.a. Example Of Correction File
-
-     W YYn""  "pty lines are accepted. The file contains a set of
-correction points, in ascending order. Each "correction point" has the form 'k y x', where:
-• k is a 3-letters lowercase "key" among 12 allowed values:
-• 'plm' portrait left margin
-• 'prm' portrait right margin
-• 'ptm' portrait top margin
-• 'pbm' portrait bottom margin
-• 'pcw' portrait character width
-• 'pch' portrait character height
-• 'llm' landscape left margin
-• 'lrm' landscape right margin
-• 'ltm' landscape top margin
-• 'lbm' landscape bottom margin
-• 'lcw' landscape character width
-• 'lch' landscape character height
-• y is a "wanted value" in points inches millimeters or centimeters
-• x is an "obtained value" in points inches millimeters or centimeters
-
-  W " "W W "
-• For each key, first y value must be not less than zero, and each next y value must be strictly
-greater than the previous one
-• For each key, first x value must be not less than zero, and each next x value must be strictly
-greater than the previous one
-For instance, let's take the first correction point, 'plm 10mm 16mm'. This means that, by trying to
-print a page with -Z off, -C n, and -L 10mm (y = 10mm), we have empirically obtained an actual
-measured left margin of 16mm on paper (x = 16mm). Therefore if we wish an actual measured left
-margin of 16mm on paper (x = 16mm), we should give to lp command an argument '-o page-left'
-equivalent to 10mm (y = 10mm). So, given a wanted measure x and a set of corresponding correction
-points, which is the function y = f(x) telling us what argument y provide to lp?
-For each key, we can have zero, one, two or more correction points, namely:
-• zero correction points: no correction, y = f(x) = x, the straight line passing by (0, 0) and
-(1, 1)
-• one correction point, say [(y0, x0)], the straight line passing by (0, 0) and (x0, y0): y =
-f(x) = (y0 / x0) * x
-• two correction points, say [(y0, x0), (y1, x1)], the straight line passing by points (x0, y0)
-and (x1, y1): y = f(x) = y0 + (x - x0) * (y1 - y0) / (x1 - x0)
-• three or more correction points, say [(y0, x0), (y1, x1), (y2, x2), ...], y = f(x) is
-approximated by the broken line defined by points (x0, y0), (x1, y1), (x2, y2), ...
-Finally, if the result is less than zero, it's forced to zero.
-
-8. Reserved Files
-23/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
- y = f(x)
-│
-•
-│
-•
-│
-•
-y3 ···························•
-│
-• :
-y2 ·····················•
-:
-│
-• :
-:
-│
-•
-:
-:
-y1 ···············•
-:
-:
-│
-•:
-:
-:
-│
-• :
-:
-:
-│
-• :
-:
-:
-│
-•
-:
-:
-:
-│
-•
-:
-:
-:
-:
-:
-:
-y0 ·········•
-│
-•:
-:
-:
-:
-│
-• :
-:
-:
-:
-│
-• :
-:
-:
-:
-│
-•
-:
-:
-:
-:
-x
-
-
-
-
-
-0 ••••••
-0
-x0
-x1
-x2
-x3
+
 
-W   
-In
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-W W
+ 
 
- W   W
+
 
-W
+ I  $ 
 
-GUI
+     !  (
 
-mode the correction file can be edited, reset to default values, or restored by the Correct
-
-
-W   W  e correction archive is managed in the same way as
-the text archives. Namely:
+  (   
 
-
+ $  
 
-• if
+I(       & !  
+ (  '   '  !,   &   &  ! 
+ &   &    ,  
+    &  (    ( !   
+(    (   & ,    (!   &
+│
+   ! & 
+│ 
+ &  ( (  &
+│
+│  _(_  d    '
+ & , &   ' s 
+│  _ _  d Y Y 
+&   & , &  ' s 
+│   _ ( d YI& Y    
+ & , &  ' s 
 
-
+
+  
+, YY&& 
+'    
 
-the
+    & C(
+ '
 
-Edit
+  
 
-Restore or Undo buttons are clicked, the correction file is locked until end of
+ &  
 
-W  W  
+     &   &     
 
-W W
+&,       &  & !    YY
+  
+ & 
+   YY   ' Y_Y,  & Y ( Y → Y _(_ Y
+
+YdY 
+ $  
+
+s  $       (
+' '
+ & 
+ $   s  ' Y     
 
-~/.yawp/.yawp..yawp.corr.%Y.%m.%d-%H.%M.%S.lock
-and released at session end
-• if the Edit or Restore buttons are clicked and the correction file is actually modified, its
-original content is saved in a backup file like:
-~/.yawp/.yawp..yawp.corr.%Y.%m.%d-%H.%M.%S.back
+&$
 
-
+
 
-
+
 
-l
+"0
 
- 1l f
+
 
-W W
+"0 I
 
- W sW    "essages on the log file:
+  (  '   !   
+     &   (
 
-• an initial frame containing the log file name
-• frames containing the operation performed and a datetime timestamp
-• "information messages" saying what's going on
+& &  '   (,       &
 
- "W ""
+ &
+! ' '    
 
-W W Y
+'   ( (   
+ ! &  &  
 
-flYu W  "   
+ ' 
 
-W
+ '        (
+    &  ( &      (
+I
+   $  (  (  '   (,  '     ( &   ( 
+ &  ( &           (   (
+ &$  '   ( ( &  
 
-continues
-• "error messages" (starting with 'ERROR:') saying what's wrong, they can be:
-• "argument error messages", when an argument pass 
-W   WW
-• "correction error messages", when an error in correction file is found
-• "processing error messages", when an error raises during processing of the text file
+    , 
+&  !i' 
 
-Information and warning messages are displayed on stderr only if -v argument is on, except the
-initial frame containing the log file name, which is displayed anyway.
-In case of an error message, file backup and reWW   
-processing is terminated, while in GUI mode processing continues.
+│
 
- f f  "
+
 
-Correction error
-correction file.
+
 
-of the offending line in the
+  $ 
 
-messages
+   
 
-are
+C I
 
-followed
+
 
-W  " 
+
+ 
 
-processed text file.
+  
 
-by
+
 
-position
+(   
 
-and
+     !
 
-content
+  
 
- 
+    
+&   
+     (    & &,     
+(  $     ( I(   (  (  &
+ &
+     ( ! '
+ ! &
+   
 
-osition
+ 
 
-and
+!  !  ( & 
 
-content of the offending line in the
+   &     ! Y C Y    ! Y !     
+ 
+  ( &  &          ! Y         & 
+   
+  "I
+ I &,  & 
+' ' ! '   '  
+I
 
-     "  W  
- "  ns W   
+I &,
+ &   !       
+ ,           ,  
 
-GUI execution, of the type:
+"I &, 
+ !  
+& ,  
 
-u  W to a timestamped log file, unique for each CLI or
+I
 
-~/.yawp/.yawp.%Y.%m.%d-%H.%M.%S.log
-In GUI mode such a log file can be browsed through the Log button (see 2.2.2.).
+ !     ( I
 
-" WW  
- "  
+I &  
 
-W " W  Wtten on output, for further inspection.
+ I   (  
+  !  
 
- W ns 
+( &
 
-
+
 
-24/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-  User Manual" -X -L 2.5cm yawp.txt
-│
- n
-ns n  n  n n n "
-│ 
-
-│ │ /home/xxxx/.yawp/.yawp.2023.03.10-15.44.17.log │
-
-│ 
-
-│ 
-│ │ Format
-2023-04-01 15:44:17 │
-│ 
-
-│ "
-│
--h --help = False
-│
--V --version = False
-│
--H --view-manual = False
-│
--v --verbose = True
-│
--M --usage-mode = 'f'
-│
--y --text-editor = 'idle'
+ ( 
+  ! !
+
+ !  !    , ! !
+ & 
+ 
+  ( &  & 
+  
+,     $  &    (( 
+   
+ & 
+  (   
+
+ & (
+
+    (
+
+! $    (!,      &   s      
+
+
+
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+Y
 │
--g --graphics = False
+ !  ( $ !         & Y   
+│ ┌──────────────────────────────┐
+│ │  &     │
+│ └──────────────────────────────┘
+│  ( 
+ & 
 │
--w --chars-per-line = '90'
+ _ _  d Y Y
 │
--l --just-left-only = False
+ _   d YY
 │
--c --contents-title = 'contents'
+ _((
+d YY
 │
--i --index-title = 'index'
+ _(
+d Y'Y
 │
--f --figures-title = 'figures'
+(_(
+d Y ! ( (Y
+(_& 
 │
--F --caption-prefix = 'figure'
+d Y&Y
+│  
+ # Y&   !   
+Y
 │
--p --page-headers = 'c'
+│ ( 
+  , &       ,   
 │
--e --even-left = '%n/%N'
+     ,  ! ,
 │
--E --even-right = 'yawp 1.0.0b7 User Manual'
+ ! ,
+  , &       
+     ,
 │
--o --odd-left = '%c'
+   ,  ! ,    , &       
+'
 │
--O --odd-right = '%n/%N'
+     ,  ! ,    , &       
+│ "&   
 │
--n --page-offset = '-5'
+  _!
+d   d  d  && d  &
 │
--a --all-pages-E-e = False
+  _ d   d  d  && d  &
 │
--X --export-pdf = True
+ _ _  d 
+ _ _  d 
 │
--Y --pdf-browser = 'xdg-open'
- Y
 │
-n nn  n W  Y' '
+&& d 
+ _!
+d   d     d 
+&
+&& d 
+&
 │
-n nnnW  YY
+ _
+d    d   d 
 │
-n nnn   Y Y
+ _ _  d 
+ _ _  d 
 │
-n nn  nW  Y Y
 │
--Z --landscape = False
+ 
 │
--L --left-margin = '2.5cm'
+Y →
+Y&   !   
+' Y
 │
--R --right-margin = '2cm'
+Y&   ! !   
+│ ! 
+ → Y&   !   
+Y
 │
--T --top-margin = '2cm'
+│ ( 
 │
--B --bottom-margin = '2cm'
+  , &       ,   
+     ,  ! ,
+ ! ,
+  , &       
 │
--C --correct-sizes = 'd'
+     ,
 │
-text_file = '/home/xxxx/pypi/yawp/yawp.txt'
-│ 
-/home/xxxx/pypi/yawp/yawp.txt
-
-│ "  n nnnW Y      Wn = 1.833333mm = 0.183333cm'
-│  n nnnW        W = 1.936470mm = 0.193647cm
-│ Correct: -L 41.844769pt = 0.581177in = 14.761905mm = 1.476190cm (even pages)
-│ Correct: -R 59.269864pt = 0.823193in = 20.909091mm = 2.090909cm (even pages)
-│ Correct: -L 55.343082pt = 0.768654in = 19.523810mm = 1.952381cm (odd pages)
-│ Correct: -R 42.519685pt = 0.590551in = 15.000000mm = 1.500000cm (odd pages)
-│ Correct: -T 53.709076pt = 0.745959in = 18.947368mm = 1.894737cm
-│ Correct: -B 14.173228pt = 0.196850in = 5.000000mm = 0.500000cm
-│ Compute: char height 8.661417pt = 0.120297in = 3.055556mm = 0.305556cm
-│ Compute: chars per inch 13.854545
-│ Compute: lines per inch 8.312727
-│ Correct: char height 9.179314pt = 0.127490in = 3.238258mm = 0.323826cm
-│ Correct: chars per inch 13.116652
-│ Correct: lines per inch 7.843723
-│ Compute: lines per page 81
-│ Before:
+   ,  ! ,    , &       
+'
 │
-header: 74 lines, 186 words, 6660 chars, max 90 chars per line, 38 pages
+     ,  ! ,    , &       
+│ "  
 │
-body:
-2687 lines, 15777 words, 108239 chars, max 90 chars per line
+(_& 
+d  d    d  && d  &
 │
-total: 2761 lines, 15963 words, 114899 chars, max 90 chars per line
+_& 
+d  d   d   && d   &
 │
-fl f W  Y WY   -w --chars-per-line 90, truncated
+_& 
+d    d    d  && d  &
 │
-fl f W  Y Y   n nnchars-per-line 90, truncated
-
-│ Backup: '/home/xxxx/pypi/yawp/yawp.txt'
+'&_&  d    d   d  && d  &
 │
-'/home/xxxx/pypi/yawp/.yawp.yawp.txt.2023.03.10-15.44.17.back'
-│ W
- '/home/xxxx/pypi/yawp/yawp.txt'
-
+ _!
+d   d   d   && d  &
 │
+ _
+d  d  d  && d  &
 │
-header: 76 lines, 191 words, 6840 chars, max 90 chars per line, 39 pages
+ _ _  d 
 │
-body:
-2682 lines, 15771 words, 108147 chars, max 90 chars per line
+ _ _  d  
+│  
 │
-total: 2758 lines, 15962 words, 114987 chars, max 90 chars per line
-│ Export: '/home/xxxx/pypi/yawp/yawp.txt'
-
+Y →
+Y&   !   
+(Y
 │
-'/home/xxxx/pypi/yawp/yawp.pdf'
-Figure 8.4.a. Example Of Verbose Output
-This output has been written on terminal, thanks to -v argument, and recorded into:
-/home/xxxx/.yawp/.yawp.2023.03.10-15.44.17.log
-If for any reason you want to remove all log files, type:
-│ $ rm -fv ~/.yawp/.yawp.*.log
+Y&   ! !   
 
- 
+ 
+      '
 
-l 
+! 
 
-
+
 
-l  f
+    & C( # ' C  
 
-If your text file is for example:
-~/example.txt
-then the associated arguments are saved into:
+ &
 
-8. Reserved Files
-25/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-~/.yawp.example.txt.args
-In CLI mode the arguments are:
-• not loaded from a file but taken from the CLI interface at startup
-• saved into .args file at finish
-In GUI mode the arguments are:
-• loaded from .args file at startup, if any (if otherwise the .args file is not found, arguments
-silently get their default values)
-• saved into .args file and reloaded from another .args file whenever the current text file
-becomes another one
-• saved into .args file at finish
-This ensures argument
-the same text file:
+, 
 
-continuity from a processing of a given text file to the next processing of
+  $
 
-• from CLI mode to GUI mode
-• and from GUI mode to GUI mode
-but not:
-• from CLI mode to CLI mode
-• or from GUI mode to CLI mode
+ & ,
 
-  18
-Both
+    (
 
-in
+
 
- 18 f
-CLI
+&   ! ! !
+
 
-and
+&$
 
-in
+  ( ( &  
 
-GUI
+    , 
+&  !i
 
-mode,
+│
 
-W  "  
+
+ 
+&  (
+  C"0
 
-the
+
 
-text
+I  $ 
 
-file
+ 
 
-is
+
 
-locked
+( 
 
-Ws. Namely:
+ 
 
-before processing in order to avoid
+     ! !
 
-• in CLI mode the text file is locked before processing and unlocked at processing end
-• in GUI mode any processed text file (by Edit Format Noformat or Undo action) is locked before
-processing, and stays locked until session end, so a single session can keep multiple text
-files locked at same time
-Locking
-file:
+C"0 I
 
-takes
+I &,   (   '(     
+ 
+"I
+ 
+&
+  (   ( &         
 
-place
+ 
 
-through
+
 
-the creation of a lock file. For instance, in order to lock the text
+$
 
-~/yyyy/example.txt
-a temporary hidden file:
-~/yyyy/.yawp.example.txt.lock
-is generated in the same directory and is removed 
+      
+"I &   (   '(     
+I &
+ (   !    $   &  ( &    
+&    !       ,  
+ ,
+
+   (  
+ ( 
+  , 
+
 
-Y 
+ 
+ 
 
-  " 
-
-W  W W he lock file, this acts as a session signature and
- 
-W  WWW W  ck files from those of others.
-  
+      '    
 
-W 
+ ( 
 
-fl   
+(
 
-s  
+  , 
 
-the same text file.
-application.
+ 
 
-  he same time two distinct text files, but not both
-W " W "W W    n
+    (
 
-
-
-fl 
-W  rrection file '~/.yawp/.yawp.corr'
-'~/.yawp/.yawp.sess' and '~/.yawp/.yawp.hist' are not lock-protected.
+ &
+&
 
-only,
+ 
 
-while
+(     
 
-It shouldn't happen, but if for any reason one or more text files in a given directory remain locked
- "   W   :
+
 
-  W
+
 
-│ $ rm -fv .yawp.*.lock
+      
 
-   8  lf
+  &   
 
-   1  f
+ ! &
+I  
 
- " n  n8     DF file is generated from the text file through an
-intermediate temporary file. This file contains empty lines at the top of the pages and blanks on
-the left of text lines, in order to simulate the top margin and the left margin respectively. For
-example the text file
-~/yyyy/example.txt
-will generate a temporary file:
-~/yyyy/.yawp.example.temp
-The temporary file is deleted when
-reason one or more temporary files
-directory and type:
+   
 
-it is no longer needed. It shouldn't happen, but if for any
-remain in  Ws W   W
- "  
+s    
 
-│ $ rm -fv .yawp.*.temp
+
 
- 
+     ( &  Y 
 
- 8
+ & 
 
-  8 f
+  
 
-The text file is backed up when needed into a timestamped hidden backup file, created in the same
-directory. For example the text file
-~/yyyy/example.txt
-will be backed up into a backup file of this kind:
+Y,  &
 
-26/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-~/yyyy/.yawp.example.txt.%Y.%m.%d-%H.%M.%S.back
-Such a backup can take place after any operation likely to alter the text file, namely:
-• GUI mode:
-• Edit button
-• Format button
-• Noformat button
-• CLI modes:
-• Edit mode (yawp -M e)
-• Format mode (yawp -M f)
-• Noformat mode (yawp -M n)
-In order to avoid proliferation of useless backup files, the backup is performed only if the
-Edit/Format/Noformat operation actually altered the content of the text file.
-If for any
-and type:
+│
+   ! &
+│    
 
-reason you want to remove all backup files in a given directory, jump to the directory
+ 
+       !  ( ( &  (  ,  !    
+    
+     & & !    (, '   '   & 
+(
 
-│ $ rm -fv .yawp.*.back
+
+
 
-27/37
-
-
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+I   
 
-
+  $ 
 
-  1
+
 
-9.1. VERSIONS
-• version 1.0.0b7 - 2023-04-27 - on test.pypi.org
-• something fixed
-• version 1.0.0b6 - 2023-04-18 - on test.pypi.org
-• something fixed
-• version 1.0.0b5 - 2023-04-02 - on test.pypi.org
-• something fixed
-• version 1.0.0b4 - 2023-04-01 - on test.pypi.org
-• something fixed
-• version 1.0.0b3 - 2023-04-01 - on test.pypi.org
-• updated installation instructions
-• version 1.0.0b2 - 2023-04-01 - on test.pypi.org
-• moved mkdir between constants
-• version 1.0.0b1 - 2023-04-01 - on test.pypi.org
-• GUI mode, added and set as default usage mode
-• CLI Edit mode, added
-• several other additions and changes, too many to list here
-• version 0.7.1 - 2022-06-25
-• experimental obsolete and deprecated
-• version 0.6.1 - 2022-05-06
-• experimental obsolete and deprecated
-• version 0.5.4 - 2022-04-04
-• experimental obsolete and deprecated
-• version 0.5.3 - 2022-04-02
-• experimental obsolete and deprecated
-• version 0.5.2 - 2022-04-02
-• experimental obsolete and deprecated
-• version 0.5.1 - 2022-03-19
-• experimental obsolete and deprecated
-• version 0.4.2 - 2022-01-04
-• experimental obsolete and deprecated
-• version 0.4.1 - 2022-01-03
-• first version on https://pypi.org
-• experimental obsolete and deprecated
-9.2. CREDITS
+
 
-   s W
+(
 
-u
+( & '  &( '
 
-" W  nix command "fmt", for details type:
+  
 
-│ $ man fmt
+ 
 
-       "  W W.
-  s   
+  $ 
 
-
+
 
-http://www.xubuntu.org
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-      f    Y f
+  
 
-
+  
 
-https://www.python.org
+  (   !    (    I  
+ &$   ( ( &       , 
 
-" Ws  
+
 
-nW  W W
+, ' 
 
-  W 
+     (     ( &   (   
+  &  &
+'      '      , ! ( &  Y   !   &    
+(  &
 
- f 
+ (
+&Y,
 
-W  
+&  !i
 
-  3.6.
+│
 
-
+  C
 
-https://pypi.org/project/flit
+Y '
 
- lf W    W" "  
- 
+I
 
- W  
+  !  &
+   
+& &
 
-ySimpleGUI 4.60.1:
+s  ,  &
 
- W" lf
+ ( &        I
 
-  n    n   W
+ &$ ! 
+  &  (
+ &$  &
+ (, 
+│
 
-
+  C
 
-W e:
+ 
 
-https://www.cups-pdf.de
+
 
-
+  
 
-  
+&   
 
- "W 
+
 
-
+ I  
 
-W 
+ '
 
-https://pypi.org/project/pdfrw
+
 
-
+, ' 
 
-  W 
+&   !i&
 
- W W
+I
+
+I
+   '       (,    ! &
+   (
+Y   !   &     &i(Y, (  &
+
+   , ! ( & 
+
+  !  &___('_(
+  &    (
+'   &$  &
+
+ &$ ! 
+   (, 
+│
+
+
 
-6.0:
+  
 
-https://wiki.mate-desktop.org/mate-desktop/applications/atril
-9.3. HOMONYMS
+&   !i(
 
-28/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-There are several homonyms online, with which this project has nothing to do. Some examples:
+ I    ' 
 
+,
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+
+
+ C 
+
+ # IC 
+ $          '
+ I  ' 
+ "I  &, 
+ I "  '  , &$
+
+ &      , 
+
+ &      , 
+
+ &  &   ((, 
 
+ &     , 
 
+ &  I &  , 
 
+ &   & , 
 
+ &      ,  YY 
 
+ &    (,   Y Y YY
+ Y'Y 
 
+ &  $ $ ', &$ ( & I &  ! dow
 
+ &  0 ( &  , &$
+  I &  ! !,    (, 
+ &$  (    &      (, 
+ &
+ & , !
+   &  ( (   (,  
+  (  (,  
+  (   (,  
+  ( &  (,  
+ &  ! !     ! ! &  ,   (      '
+&' ( &    (   (,  ( &   
+ & 
+  (      ( & Y  !Y  Y  ( !Y
+   (
+, !       
+ 
+ &   
+& &
+ &I $  ,      '  &I  s    
+ (    ,   ( & I   0 
+ '   !  ,  &    '   ( (  (  !  ( &  '
+&$, (
+ '  
+"  , 
+ '   ( (  (  !  ( &  '
+&$, (
+ '   &  (      & , (
+ '  
+ s   &&        $     '  ,  
+$ '  &&   '
+  ( 
+ 
+ '  &
+   ( &  ' &$, (
+ '  Y ! Y          (   (, (
+ &  &  s  , (
+  ' & ' !  $  $   "I    $  Y Y   Y 'Y
+ $ 
 
-  W 
-   
-   
-   
-   
-  WW "
- W " WW
+        '
 
- W W  
+ $  '    '  
+ I &, 
+   (    &
+ "I  &, 
+   ((  & , 
+ $       ,  &     
+  & ' !  $  $  
+ $ 
 
-  W   s://pypi.org.
+       &  
 
-9.4. LICENSE
-This
+ $ 
 
-program
+      &  
 
-is free software, you can redistribute it and/or modify it under the terms of the GNU
-W    Software Foundation, either version 3, or (at your
-option) any later version.
-This
+ $ 
 
-program
+     &  
 
-l
+ $ 
 
-W W 
-is
+     &  
 
-distributed in the hope that it W    
+ $ 
 
-s  W" W  
-   ff
-l W W  " W
+     &  
 
-
+ $ 
 
-You should have received a copy of the GNU Gener
-text file LICENSE), if not, see:
+     &  
 
-f
+ $ 
 
-1
+     &  
 
-f1 
-   W
-  l
-f   1
+ $ 
 
-W W  W W
+    (  $ 
 
-"  
+
 
-https://www.gnu.org/licenses/
-or
+
 
-contact
+    &  
 
- 
+I  IC 
+┌───────────┬─────┬─────┬──────┐
+│I │C  │"  │
+│
+ 
 
-1 
+
 
-
+
+ │  │ │  │
+│  ││ │
+
+
+│C 
+│ │ ││
+│
+│
 
-Free
+└───────────┴─────┴─────┴──────┘
 
-
+   
+
 
-
+&   C(
 
-
+   
 
-
+
 
-
+&&      (             
+ &  '    '       $  (
+ 
 
-
+  ' 
 
-│ 1 │
+ &&  '
+
 
-Software Foundation, Inc., 51 FW
+ "  I
 
- W     
+&  
+   $
 
-
+%& &
 
- fl
+     (,
 
-│
+41
+ ( ! 
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-
+  '  $  ((  
+
+&     &&
+
+ 
 
-│ ff │ "W    f "W fterchange│
-│CLI
-│Command Line Interface
-│
-│"" W WW "
-│
-│
-│GNU
-│Gnu is Not Unix
-│
-│GUI
-│Graphic User Interface
-│
-│IDE
-│Integrated Development Environment
-│
-│IDLE
-│Integrated Development and Learning Environment
-│
-│  W W "
-│
-│ 
-│  f
-│   f
-│
-│ 
-│"  "
-│
-│
-│W  
-│
-"W
-│UTF8
-│Unicode Transformation Format 8 bits
-│
-│
-│
-f l│    f   l
-│
-│    
 │
 
-
+
 
-W   
+
 
-"
+
 
-n 
+ (
 
-10. Unicode Characters
-29/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
+!
 
- f1
-
+(&
 
-│
+'
 
-
+
 
-   
+
+ 
 
-     
+!!!'
+' 
 
-
-
-
-
-│ │HEX │DEC │
-
-
-
-
+ 
 
-│horizontal tab
-│'\t'│0009│
-9│
-│line feed
-│'\n'│000a│ 10│
-│form feed
-│'\f'│000c│ 12│
-│carriage return
-│'\r'│000d│ 13│
-│space (or blank)
-│' ' │0020│ 32│
-│exclamation mark
-│'!' │0021│ 33│
-│quotation mark (or double quote)
-│'"' │0022│ 34│
-│number sign (or hash or pound)
-│'#' │0023│ 35│
-│dollar sign
-│'$' │0024│ 36│
-│percent sign
-│'%' │0025│ 37│
-│ampersand
-│'&' │0026│ 38│
-│apostrophe (or single quote)
-│"'" │0027│ 39│
-│left parenthesis
-│'(' │0028│ 40│
-│right parenthesis
-│')' │0029│ 41│
-│asterisk
-│'*' │002a│ 42│
-│plus sign
-│'+' │002b│ 43│
-│comma
-│',' │002c│ 44│
-│hyphen (or minus sign)
-│'-' │002d│ 45│
-│decimal point (or full stop)
-│'.' │002e│ 46│
-│slash
-│'/' │002f│ 47│
-│digit zero
-│'0' │0030│ 48│
-│...
-│... │ ...│ ...│
-│digit nine
-│'9' │0039│ 57│
-│colon
-│':' │003a│ 58│
-│semicolon
-│';' │003b│ 59│
-│less-than sign
-│'<' │003c│ 60│
-│equal sign
-│'=' │003d│ 61│
-│greater-than sign
-│'>' │003e│ 62│
-│question mark
-│'?' │003f│ 63│
-│at sign
-│'@' │0040│ 64│
-│Y Y │0041│ 65│
-│W  W 
-│...
-│... │ ...│ ...│
-│latin capital letter Z
-│'Z' │005a│ 90│
-│left square bracket
-│'[' │005b│ 91│
-│back slash
-│'\\'│005c│ 92│
-│right square bracket
-│']' │005d│ 93│
-│circumflex accent
-│'^' │005e│ 94│
-│low line (or underscore)
-│'_' │005f│ 95│
-│back quote (or grave accent)
-│'`' │0060│ 96│
-│latin small letter a
-│'a' │0061│ 97│
-│...
-│... │ ...│ ...│
-│latin small letter z
-│'z' │007a│ 122│
-│left curly bracket
-│'{' │007b│ 123│
-│vertical bar
-│'|' │007c│ 124│
-│right curly bracket
-│'}' │007d│ 125│
-│tilde
-│'~' │007e│ 126│
-│macron
-│'¯' │00af│ 175│
-│middle dot
-│'·' │00b7│ 183│
-│greek capital letter sigma
-│'' │03a3│ 931│
-│greek small letter pi
-│'' │03c0│ 960│
-│black small circle
-│'•' │2022│8226│
-│infinity
-│'' │221e│8734│
-│not equal sign
-│'' │2260│8800│
-│less than or equal sign
-│'≤' │2264│8804│
-│greater than or equal sign
-│'≥' │2265│8805│
-│box drawings light horizontal
-│'─' │2500│9472│
-│box drawings light vertical
-│'│' │2502│9474│
-│box drawings light down and right
-│'┌' │250c│9484│
-│box drawings light down and left
-│'┐' │2510│9488│
-│box drawings light up and right
-│'└' │2514│9492│
-│box drawings light up and left
-│'┘' │2518│9496│
-│box drawings light vertical and right
-│'├' │251c│9500│
-│box drawings light vertical and left
-│'┤' │2524│9508│
-│box drawings light down and horizontal
-│'┬' │252c│9516│
-│box drawings light up and horizontal
-│'┴' │2534│9524│
-│box drawings light vertical and horizontal│'┼' │253c│9532│
-│white square
-│'□' │25a1│9633│
-│white up-pointing triangle
-│'△' │25b3│9651│
-│white right-pointing triangle
-│'▷' │25b7│9655│
-│white down-pointing triangle
-│'▽' │25bd│9661│
-│white left-pointing triangle
-│'◁' │25c1│9665│
-│white circle
-│'○' │25cb│9675│
-│bullseye
-│'◎' │25ce│9678│
-└──────────────────────────────────────────┴────┴────┴────┘
-Figure 10.a. Unicode Characters
-
-30/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-
-
-
- 
-
-
-
-  n     n  s://pypi.org/project/yawp
-
-   ! n   sgmail.com
-Usage syntax:
-│ $ yawp -H # show a help message and exit
-│ $ yawp -V # show program's version number and exit
-   Wt
-│ $ yawp -H [-Y pdf_   
-
-│ $ yawp text_ W  
-W lf "  WW  W o arguments
-│
-  
-W lf "  W " evious session, no arguments
-│ $ yawp -M e [-y text_editor] text_ W  
-W f W "
-│ $ yawp -M f [...arguments...] text_ W  
-W f " "
-│ $ yawp -M n [...arguments...] text_ W  
-W f  " "
-│ $ yawp -M u [...arguments...] text_ W  
-W f  "
-Buttons in GUI Main window:
-• 4 buttons dedicated to the selection of the text file:
-• New button: create a new empty text file
-• Open button: browse the file system to select the text file
-• Recent button: browse the list of recent files to select the text file
-• Saveas button: clone current text file into a new target text file
-
- 
-
-  
-
-  
-
-   W  n
-
-• Exit button: save current text file with its arguments and finish
-• 4 buttons dedicated to the processing of the text file:
-• Edit button: edit the text file through the text editor defined by -y
-• Format button: process the text file by formatting it
-• Noformat button: process the text file without formatting it
-• Undo button: restore the text file to its previous content
-• Log button: browse the log file through the text editor defined by -y
-• Correct button: manage the correction file (Edit Reset or Undo)
-
-Usage arguments:
-• -h, --help: show a help message and exit
-• -V, --version: show program's version number and exit
+  
 
- n nnsWn" sW 
+& (   
 
-n
+   
 
-
+    ' $
 
-   W
+&
 
-• -v, --verbose: write all messages on stderr (default: write errors only)
- n nnn" 
-W W  " (default: 'g' = GUI, 'e' = CLI Edit, 'f' = CLI
-Format, 'n' = CLI Noformat, 'U' = CLI Undo)
-Format arguments:
-• -y, --text-editor: editor for text files (default: 'idle')
-• -g, --graphics: redraw '`'-segments and '^'-arrowheads
-• -w, --chars-per-line: line width in characters per line (default: '0' = automatic)
-• -l, --just-left-only: justify text lines at left only (default: at left and right)
-• -c, --contents-title: title of Contents chapter (default: 'contents')
-• -i, --index-title: title of Index chapter (default: 'index')
-• -f, --figures-title: title of Figures chapter (default: 'figures')
-• -F, --caption-prefix: first word of figure captions (default: 'figure')
-
-W "
-• -p, --page-headers: insert page headers (default: 'n' = no, 'f' = on full page, 'p' = and on
-broken pictures, 'c' = and on level-1 chapters)
-• -e, --even-left: headers of even pages, left (default: '%n/%N')
-• -E, --even-right: headers of even pages, right (default: '%F %Y-%m-%d')
-• -o, --odd-left: headers of odd pages, left (default: '%c')
-• -O, --odd-right: headers of odd pages, right (default: '%n/%N')
-• -n, --page-offset: offset of page numbers (default: '0', min: '-3999', if negative it is the
-count of initial Roman numbers)
-• -a, --all-pages-E-e: put in all page headers -E at left and -e at right
-Export arguments:
-• -X, --export-pdf: after processing export and br
- W
- n  nn  n  
- W  t: 'xdg-open')
- n  nn Wn    
- W   Y' pdf')
- n  nnnW  W   YY = automatic, 'pt' 'in' 'mm' or 'cm')
- n  nnn     W  har width / char height (default: '3/5', '1' =
-
-square grid)
-• -S, --paper-size: portrait paper size width x W   Y Y  Y  ""Y Y Y YWY
-'mm' or 'cm')
-• -Z, --landscape: turn page by 90 degrees (default: portrait)
-• -L, --left-margin: left margin (default: '2cm' = min, 'pt' 'in' 'mm' or 'cm')
-• -R, --right-margin: right margin (default: '2cm' = min, 'pt' 'in' 'mm' or 'cm')
-• -T, --top-margin: top margin (default: '2cm' = min, 'pt' 'in' 'mm' or 'cm')
-• -B, --bottom-margin: bottom margin (default: '2cm' = min, 'pt' 'in' 'mm' or 'cm')
-• -C, --correct-sizes: correct character size and page margins (default: 'd' = by default
-values, 'n' = no, 'f' = by correction file)
-• -K, --fake-margins: build left margin by blanks and top margin by empty lines
-
-File argument:
-• text_ W 
-
-W   
-
-ff  nncoded
-
-Figures
-31/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-FIGURES
+ (&, (
 
-
-
-
+ !  ,   Y I  
+!!!  
 
-
-
+'  & & &
 
-
+s   
 
-W W
- W
-   W  WWW
+  
 
-2
-2
-3
+   '  '  I ' ( 
+  (
+ I   (    '
 
-Ww
+&&     &I  
+  &I 
 
-
+    '     ' C $ 
+&I , ! s    
 
-W
-1   W W W
-1   W    Wdow
-  W W W
-    W"W Wdow
-• 2.1.1.4.a. Saveas Button, Target File Definition W
-• 2.1.1.4.b. Saveas Button, Overwriting Confirmati W
-
-  W W W
+( &I,
+
+ 
+
+ 
+
+ 
+
+      $  (   !    (, 
+!!! (
+  ( !   &
+
+     (, 
+  ( !
+
+(
+
+
+
+Y  
+
+ ! 
+  ! 
+
+(
+
+
+
+Y   ' !
+
+
+
+ 
+
+!&  &      
+ C C
+ 
+
+
+
+
+
+
+
+
+
+
+
 
-• 2.1.2.b.
-Correct Button, Restore Confirmation W
- 
 
-    W"W Wow
 
-      W"W Wdow
-• 2.1.1.1.b. New Button, Overwriting Confirmation
-
-
-
- 
- 
-
 
 
 
 
 
-• 3.1.a.
+
 
-Formatting State Diagram
+ $  & &   , ! !     
 
-• 4.a.
-• 4.2.a.
-• 4.3.1.a.
+    &  &
 
-Chapter Types
-Example Of Chapter Renumbering
-Example Of Contents Chapter
+   !   
+
+   
+
+    
+
+    &
+
+ '  
+
+ '    
+
+ '   && 
+
+ ' $  $
+
+ '   
+
+    
+
+    '&
+
+   (   
+
+    
+
+    ' 
+
+     
+         &
+ 
+' &    
+    !
 
- 
+! ,   
+  " C
 
-
+ 
+
+
+
+(  
+
+ 
+
+
+
+ (!   ' !
+
+  &      
+
+ 
+
+
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌───────┬──────────────────────────────────────────────────┐
+│
+│
+│ " C
+ I 
+
+─────────┤
+│ "II │ & 
+   " ( I ( &  I   │
+│"&&    I  ( 
+│
+│"I
+│"
+│"&&       &
+│
+│   ' 
+│
+│ 
+│C
+│ 
+│
+ C   (! 
+│  (!    
+│
+│
+│
+│
+│ 
+   
+│
+│    '  
+│
+│   I  ( 
+│
+│I
+│
+│!  
+│
+│I   $&   $  & 
+│
+│I 
+│I   $& 
+│
+│I 
+     $  & 
+│0 
+│0   $  & 
+│
+│  (
+│
+│ 
+│ 
+│  '  &   & 
+│
+│  I  (
+│
+│I
+│I
+│    I 
+│
+│
+│
+│
+&  & 
+│     (
+│
+│
+│
+│      (
+│
+│
+│  │      (
+│
+│    ( & 
+│
+│
+│ │  
+( &   &   '
+│   
+│
+│
+│ I │    I    
+│
+│ & "&&  $  & 
+│
+│"
+│ 
+│ 
+│
+    
+└───────┴──────────────────────────────────────────────────┘
 
-  
-  
-  
-  
-  
-  
-
-• 7.a.
-• 8.a.
-• 8.3.a.
+    
 
-   
+  &
 
-" 
+  I" 
+ '   
+   &  (  (! ,  
+      '     ' '    (!  
+ 
+   $  
 
-4
+&(     & ( 
+  ,  $  ,   
 
 
+   &   '        ! ' ( , '  IC
+$  & !
+ I"  C
+ (  "  II  I  C
+     
 
-5
-6
-7
-7
-9
-10
-11
-13
+  '   (
 
-W "n  n "
+ , ! 
 
- !W
-"'" ! 1   W 1 "n" "
-  W "n" "n"  "n" Off
-  W "n" "n"  "n" On
-"  W "n"
-"  W "n  n n "
-Symbolic Names For "-S"
-Hidden Reserved Files
-Example Of Correction File
+&   
 
-W W
+   $ $
+
+ (     
+  ( I"  , ( , 
 
- W   W
+  '  
 
-• 8.4.a.
+  !   
 
-Example Of Verbose Output
+& 
 
-• 10.a.
+!!!   
+      (!  
+ 
+ "
 
-Unicode Characters
+  , I ,  
 
-   
+
 
-3
-3
-4
-4
+ , (  ,  ,
+
+
+
+" 
+
+I( 
+!        
+ ( &         , '   $ 
+&    '   
+&         '  ( &  ,  
+  
+& 
+
+  
+'           &   , &      
+$  !   $ , ! ! & 
+ &  
+   " (
+    &    (  
+    
+
+ ,
+
+& Y Y, 
+
+& Y Y
+
+  &  
+  
+    
+
+! ,     
+ 
+ 
+    &  
+ (, '    
+  ((
+    '    ,  (   
+
+ ! 
+ (
+
+&'   '
+ (!   ' !  ( $  
+ &   &  ( & 
+
+ , ! 
+
+     & 
+
+43
+ ( ! 
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌─────────────────────────────────────────────┬────────┬────┬────┬────┐
+│ "
+│ │ " │ C│
+│
+" "
+
+
+
+
+
+
+│  
+│YY
+│ │
+│
+
+│
+│ 
+│
+│
+│
+│ │
+│'
+│Y Y
+│ │
+│
+│
+│Y'Y
+││
+│
+│'  
+│
+│     '   '
+│YY
+││
+│
+│
+│Y Y
+│ │  │
+│
+│  (
+│Y$Y
+│'│  │
+│
+│$    '
+│( & (
+│Y(Y
+││  │
+│
+│Y Y
+││ │
+│
+│
+  
+│
+│ 
+│
+│
+│ │
+│Y Y
+│ │  │
+│
+│   ' 
+│Y'Y
+│ │ │
+│
+│ &  & 
+│s   &    ' s 
+│Y Y
+│ │  │  │
+│YY
+││  │
+│
+│ &'         
+│
+│Y Y
+│ │  │
+│
+│Y Y
+│ │  │
+│
+│  
+│ &  
+│YY
+│ │ │
+│
+│ Y
+│ │ │
+│
+│      s 
+│YY
+││  │
+│
+│(   
+│    
+│Y Y
+││  │
+│
+│YiY
+│ │  │
+│
+│  
+│ 
+│YY
+│'│ │
+│
+│Y,Y
+││  │
+│
+│&&
+│YY
+││  │
+│
+│  & 
+│&          (   │YY
+││  │  │
+│YY
+│( │  │
+│
+│    
+│  
+│YY
+│ │ │
+│
+│ 
+│
+│
+│
+│ │
+│YY
+││  │
+│
+│  
+│
+│YY
+│ │ │
+│
+│Y Y
+│'│ │
+│
+│&
+│
+│ 
+│YY
+││
+│
+│YdY
+││
+│
+│s 
+│
+│
+│   
+│Y Y
+││
+│
+│Y Y
+│( │
+│
+│s  & 
+│
+│Y%Y
+│ │
+│
+│ 
+│
+│
+│     
+│Y Y
+│ │
+│
+│ 
+│
+│
+│
+│ │
+│     
+│Y Y
+│ │  │
+│
+│Y Y
+│'│  │
+│
+│( s
+ ' 
+│YY
+││  │
+│
+│'   
+ ' 
+│  s
+│Y Y
+││ │
+│
+│YY
+││  │  │
+│  &(  
+│!   
+│Y_Y
+│(│  │
+│
+  
+│YvY
+│  │  │  │
+│'  s    $  
+│  &  
+│Y Y
+│  │  │
+│
+│ 
+│
+│
+│
+│ │
+│YY
+│ │  │
+│
+│  &   
+│(   ' 
+│YY
+│ '│ │
+│
+│YY
+│ │  │
+│
+│$   '
+│    ' 
+│YY
+│ │  │
+│
+│Y Y
+│ │  │
+│
+│
+│Y  (Y│ ( │  │
+│
+│   
+' 
+└─────────────────────────────────────────────┴────────┴────┴────┴────┘
+
+ s   '
+      
+    
+
+
+  
+
+"II
+
+"
+
+ 
+
+44
+copy
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+┌─────────────────────────────────────────────┬────────┬────┬────┬────┐
+│ "
+│ │ " │ C│
+│
+"
+"
+
+
+
+
+
+
+│ '   
+s       (  │Y  Y│ │  │  │
+│YaY
+│ (│  │  │
+│&  
+│ 
+│YY
+│'│  │
+│
+│YWY
+│'│  │
+│
+│    !
+│     
+│YrY
+│'│  │
+│
+│Y·Y
+│' │ │
+│
+│&     
+│YY
+││ │  │
+│ '$    
+│      &
+│YY
+│ │ │
+│
+│YY
+││  │
+│
+│  &   
+│  !  
+│Y 'Y│'││
+│
+│Y Y│││
+│
+│  !   
+│Y Y│││
+│
+│  !  
+│'  &     ' 
+│YY
+││ │  │
+│YY
+│ ││
+│
+│      
+│$  
+│Y ‾Y
+│││  │
+│Y#Y
+│││
+│
+│(! 
+!
+│ ! 
+│Y →Y
+│││
+│
+!
+│YY
+│ │ │
+│
+│s
+ 
+│YY
+││ │
+│
+│ ( 
+│ & s 
+│Y Y
+││
+│
+│
+│YY
+│ ││
+│
+│  s 
+│    s $       
+│YY
+│ ││
+│
+│Y$Y
+│ ││
+│
+│ 
+ s 
+│Y!Y
+│ ││
+│
+│   
+ s 
+│'  !      
+│Y ─Y
+││ │  │
+│Y │Y
+││ │  │
+│'  !   $  
+│'  !          
+│Y%Y
+││ │
+│
+│YY
+│ ││
+│
+│'  !   s     $  
+│Y ┌Y
+│││  │
+│'  !   !
+ 
+│'  !   !
+│Y ┐Y
+│││  │
+ (
+│Y └Y
+│││  │
+│'  !   
+ 
+│'  !   
+│Y ┘Y
+││ │  │
+ (
+│Y ├Y
+│││  │
+│'  !   $  
+ 
+│'  !   $  
+│Y ┤Y
+│││  │
+ (
+│Y ┬Y
+││ │  │
+│'  !   !
+    
+│Y ┴Y
+│││  │
+│'  !   
+    
+│'  !   $  
+│Y Y
+│││  │
+    
+│YY
+│ │ │
+│
+│'  s
+
+
+│! s
+│YY
+│ │ │
+│
+│YY
+│ (│  │
+│
+│! $    
+│YY
+│'│ │  │
+│!      
+│!      
+│YY
+│' │ │  │
+│YY
+│'│ │  │
+│! !      
+│! (     
+│YY
+││ │  │
+│YY
+│'│ │
+│
+│!  
+│' 
+│YY
+││ │
+│
+│YY
+│ ││
+│
+│s
+
+
+└─────────────────────────────────────────────┴────────┴────┴────┴────┘
+
+    
+ 
+    
+     (     
+  ' C
+
+  "
+
+ 
+
+45
+ "  
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+ "  
+
+    
+           !
+ "     #       $ %& &
+    
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+│
+
+ ! 
+ !
+ &   
+&'
+ ! #
+ ! Y $ 
+ 
+
+ !    &   ' !     
+ 
+  I &,   (,  
+ ! _( 
+ & 
+  I &,  ( ( &  $   ,   & 
+ !
+
+  "I " &
+ !     &  _(  _( 
+  "I $ &
+ !  &   &  _(  _( 
+  "I  &
+
+ !     &  _(
+  "I  &
+
+ !     &  _(
+  "I  &  &
+
+ !  (   &  _(
+  "I ( & &
+ ! 
+  &  _(
+
+  "I   &
+ ! 
+  &  _(
+
+
+   I
+ ! !
+! &  (
+ !   
+   (
+ C  ' !  ( &  
+   (
+   ' !   (   (  
+ "       ( ! 
+ &  (
+ $ &$      ( ! 
+ &  
+ '   (
+   ( !   &  
+    
+ '   (
+        ( '    (  ' 
+   (   !
+  &  ( &   
+   
+    
+ ( &  Y ( &      ( '   !
+   
+    
+          (    $    
+  ' !   ( (     ( '    (  ' 
+ '    ' ! (  ' 
+  ' !     
+  s  
+ & 
+  
+ ,  !
+ &   
+&'
+ #, $   !  $ 
+ 
+ ' !        
+
+ , ' !&
+ 
+ $, $ ' !   ( &  &      "I &  
+     & (  YYdI, YYd"I ", Y&Yd"I
+  ,   &
+$, YYd"I , YYd"I , Y(Yd"I  & , Y Yd"I ( &, Y Yd"I  
+  & 
+ ,    (  ( (  Y! Y
+ , (   (     (   (   (
+ 
+ !,       !        (  d & 
+ ,     ! YvY& 
+ YY
+! 
+  ,              (  d & 
+ ,        (  Y Yd , YYd(, YYd  , Y Yd 
+ "  
+ ,     ( "     (  Y"  Y
+ ,    ( I    (  YI Y
+ (, (   (     (  Y Y
+ ,    ( (  !  ( (     (  Y Y
+ &,   (( (( ( $ &'     (  , &  
+  
+ ,             (  Y Yd , Y(Yd (   , YYd  
+'   , YYd   $   , YYd ' ( $  $  
+ , $ ( (    (    ( $  , ( (  Y Y
+ , $   (    (    ( $  ,  (  Y (Y
+ , ( (    (    (   , ( (  Y Y
+ C,   (    (    (   ,  (  Y Y
+&' 
+  ,  (( (( (   &'  (  , (  $ &
+  ,               (
+   
+ ,        (      (  YYd, Y Yd , Y'Yd' ,
+YYd , YYd 
+  
+ ,  (  
+ ' !   ( (  Y Yd , YYd , Y'Yd 
+ ' !
+ ",       
+   &   (  YYd' (  $  ,
+Y Yd , Y(Yd'   (
+  , (' !  ' ! (   ( (  Y  Y
+ , ((     ( (  Y ( (Y
+ ,  !   ! (  YYd & ,
+  &&&
+  
+  ,    
+ 
+d! (  , ds
+ ,        , !   (  Y YY &&Y,
+  &&&
+  ,    
+  '  (    
+ , (&   ( &  (  &,
+  &&&
+  ,  &    &  (  &,
+  &&&
+ , &    &  (  &,
+  &&&
+  , '&&   '& &  (  &,
+  &&&
+ I, &         (    (  , $   
+ , &         (  d  s   
+  
+ _(  (   , "II     
+  _(    (, ( "I "  
+ "I $  &  
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+I 
+
+  
+I $    
+  
+  !  ( 
+ &  #  
+   !
+ , !  (   !
+ ' !
+ , C$ !   " ( &   !
+   C
+ ,    !
+      ,    !
+ '    , "
+" ( &   !
+   "
+ ,    (   !
+ ' "
+ , C$ !   " ( &   !
+   $
+ ,    (   !
+ ' $
+ , C$ !   " ( &   !
+    
+ ,  " ( &   !
+     , "   " ( &   !
+    
+ ,   " ( &   !
+ " ( &   !
+     ,
+      !
+    !
+ '
+  
+ &       &
+   &,  d Y Y, ! d YY
+ '
+'
+  
+"  
+  
+    &
+       &
+   #  '
+  
+ '
+#   C      C 
+ & 
+  ,  C((
+ 
+  ,  C
+ 
+  
+   &,  C
+ '
+'   &,  C ,  d Y Y,  d 
+   &,  C ,  d YY
+  
+   &,  C ,  d YY
+ '
+   &,  C ,  d Y Y
+ 
+   &  &  
+  
+ '
+&  ! 
+ 
+ C((, I d ,  ! 
+  
+ C((, I d ,  d 
+ '
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ (
+  ,  C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C((, I d ,  d 
+ 
+ C , I d ,  ! 
+  
+ C , I d ,  d 
+ '
+ C , I d ,  d 
+ 
+ C , I d ,  d 
+ 
+ C , I d ,  ! 
+ 
+ C , I d ,  d 
+ (
+ C , I d ,  d 
+ 
+ C , I d ,  d 
+ 
+ C , I d ,  d 
+ 
+ $ 
+  
+  
+"    (  #  
+  
+ & C(
+ &  
+   
+ & C( # ' C  
+   
+  
+&   C(
+   
+  &
+  
+"II "
+ 
+ '
+C   "  
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+I 
+
+
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 
-"
+I
 
-W
+
 
-14
-14
-16
-17
-19
-20
-22
-
-
-
-24
-28
-29
-
-32/37
-   
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-INDEX
-
- n  nnn 
-
-" " 
-
- n  nn Wn 
-
-" " 
-
- n  nnnW
-
-" " 
-
- W
-
-" "
-
-• -B, --bottom-margin
-• -C, --correct-sizes
-• -E, --even-right
-• -F, --caption-prefix
-• -H, --view-manual
-• -L, --left-margin
-• -M, --usage-mode
-• -O, --odd-right
-• -R, --right-margin
-• -S, --paper-size
-• -T, --top-margin
-• -V, --version
-• -X, --export-pdf
-• -Y, --pdf-browser
-• -Z, --landscape
-• -a, --all-pages-E-e
-• -c, --contents-title
-• -e, --even-left
-• -f, --figures-title
-• -g, --graphics
-• -h, --help
-• -i, --index-title
-• -l, --just-left-only
-• -n, --page-offset
-• -o, --odd-left
-• -v, --verbose
-• -w, --chars-per-line
-• -y, --text-editor
-• Cancel
-• Clear
-• Contents chapter
-• Figures chapter
-• Index chapter
-• Nameless chapter
-• Numbered chapter
-• Numbered chapter line
-• Roman
-
-"19", 30
-"20", 30
-"13", 30
-"12", 30
-"1", 30
-"19", 30
-"1", 30
-"13", 30
-"19", 30
-"18", 30
-"19", 30
-"1", 30
-"18", 30
-"1", 30
-"19", 30
-"14", 30
-"10", 30
-"13", 30
-"12", 30
-"15", 30
-"1", 30
-"11", 30
-"8", 30
-"14", 30
-"13", 30
-"1", 30
-"7", 30
-"1", 30
-
-"3", 4
-"3"
-iii, 5, 9, "10", 11, 12, 30
-iii, 5, "12", 30
-iii, 5, 10, "11", 12, 13, 30
-"9", 10, 12
-"9"
-"9"
-iii, "14", 30
-
-"WWW" Ws     9, 10, 12, 13, 14, 15, 16, 20, 23, 25, ...
-• action buttons
-"2"
-• altered file name
-"13"
-• argument error messages
-"23"
-• arrowheads
-iii, 5, "15"
-• automatic
-iii, 5, "7", 9, 10, 11, 12, "18", 30
-• automatic chapters
-5, "10"
-• back quote
-"15"
-• best practices
-"8"
-• black small circle
-"7"
-• body line
-"7", 18
-• boolean arguments
-"2"
-• caption
-"12"
-• caption label
-"12"
-• carriage return
-"1"
-• chapter label
-"9", 12
-• circumflex accent
-"15"
-• correction error messages "23"
-• correction point
-21, "22"
-• decimal point
-"7", "9", 12
-• dot character
-"7"
-• dot line
-"7", 8
-• double quote
-iv, "11"
-• draw characters
-"15"
-• empty line
-"7", 8, 9, 12
-• equivalent
-"iv", 10, 11, 12, 22
-• error messages
-"23"
-• field arguments
-"2"
-• figure
-iii, 5, 9, "12", 13, 18, 20, 30
-• figure caption line
-"12"
-• fmt
-"27"
-• form feed
-"13"
-• header line
-"7", 13
-• horizontal tab
-"5"
-• in ascending order
-"22"
-• indented line
-"7"
-• indented paragraph
-"7"
-• information messages
-iii, "23"
-• int-dot couples
-"9"
-• key
-2, "22"
-• level
-"9"
-• line feed
-"1"
-• lp
-"20", 22
-• lpr
-"20"
-• macron
-"13"
-• obtained value
-"22"
-• percent variable
-"13"
-• picture state
-"7"
-
-Index
-33/37
-¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
-• processing error messages "23"
-• quoted subject
-"11"
-• radio button arguments
-"2"
-• segments
-iii, 5, "15"
-• session
-iii, 1, 5, 6, "20", 23, 25
-• shrink
-"iv"
-• single quote
-"11"
-• slash
-"18"
-• subject
-"11"
-• text file
-"iii", 1, 2, 3, 4, 5, 6, 8, 9, 11, 13, 14, 15, 16, 18, 20, 23, ...
-• text state
-"7"
-• titlecase
-"iv"
-• unindented line
-"7", 8
-• unindented paragraph
-"7"
-• universal newlines
-"1"
-• unquoted subject
-"11"
-• uppercase
-"iv"
-• wanted value
-"22"
-• warning messages
-"23"
+      , , 
+     , 
+ , 
+ '&& 
+  , 
+ ' !&
+    (  , 
+   ((  , , 
+ , 
+   
+ , 
+  !
+      , 
+     , 
+
+  
+ , 
+ $ (
+ , 
+ $  
+ , , 
+  (
+ (   , 
+     , 
+ , 
+ 
+ , 
+  
+ , 
+   
+ , 
+ (& 
+ (   , 
+      , , 
+ , , 
+ &  
+ , , 
+ & 
+ , 
+ (
+ , 
+  
+ , , 
+    
+ , , 
+  ((
+ , 
+ (' !
+ , 
+ ((
+ , 
+  & 
+ , , 
+   
+ , 
+ 
+ , 
+ 
+ , 
+ & 
+ , 
+   &
+ , , 
+ $ '
+ , 
+ $ 
+,  , 
+ 
+ , 
+ 
+,  ,  , 
+ "
+ ,  , 
+ 
+ , 
+ 
+ , , , 
+ 
+,  ,  ,  , , , , , , 
+ I
+ ,  ,  , , , , , , 
+ 
+ 
+,  ,  ,  , 
+ 
+,  , , , 
+ , 
+ C
+ , 
+ 
+ ,  , 
+ 
+ , 
+ 
+ , 
+ 
+ , 
+ #
+,  , ,  , , 
+ 
+ 
+, , ,  , , 
+, , ,  , 
+ 
+,  , ,  , 
+ 
+,  ,  , , 
+ 
+ , , 
+ 
+ ,  , 
+ 
+ , 
+ (
+, ,  , , 
+ 
+ , 
+ 
+ , 
+ 
+, , ,  , , 
+ 
+,  , 
+ 
+ , ,  , , 
+ &
+ 
+, ,  ,  , , 
+ , , ,  , 
+ 
+ 
+, , , , ,  , , , 
+,  ,  , , 
+ 
+,  , , , 
+ 
+ $
+,  , ,  , , , 
+ !
+,  , ,  , , , , 45
+ , , , , , 
+ 
+ 
+ , $, , , , , , , , , ,  , , , , , ,  , 
+
+ '  
+
+    '
+
+    
+ , , 
+  & 
+ , 
+    '
+ , , , , 
+    
+
+  
+
+ , 
+   
+  !    
+ , , , , 
+ &  
+ s $  i
+$ , , 
+ ( 
+, , ,  , , , ,  5
+
+copy
+
+‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
+
+  (
+, 
+   $
+, 
+  s 
+, 
+ , , 
+  
+
+     
+     
+ , 
+ $
+ , , 
+ && 
+ , , 
+ '    
+        , 
+    $  ' 
+
+    
+, ,  , , , , ,  , , 
+  
+ 
+i
+$ , , , , , 
+
+      
+  (
+ , , , , , , , , , , , , , , ,  ,  , , , 
+
+   
+  i
+$ , , , 
+ , 
+     
+   i
+$ , , , 
```

