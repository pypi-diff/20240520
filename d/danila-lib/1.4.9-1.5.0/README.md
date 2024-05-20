# Comparing `tmp/danila-lib-1.4.9.tar.gz` & `tmp/danila-lib-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.4.9.tar", last modified: Mon May 20 08:58:25 2024, max compression
+gzip compressed data, was "danila-lib-1.5.0.tar", last modified: Mon May 20 09:07:06 2024, max compression
```

## Comparing `danila-lib-1.4.9.tar` & `danila-lib-1.5.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.762041 danila-lib-1.4.9/
--rw-rw-rw-   0        0        0     9615 2024-05-20 08:58:25.762041 danila-lib-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.637079 danila-lib-1.4.9/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.4.9/danila/__init__.py
--rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.4.9/danila/danila.py
--rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.4.9/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.4.9/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10693 2024-05-14 12:37:43.000000 danila-lib-1.4.9/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.652687 danila-lib-1.4.9/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-20 08:58:25.000000 danila-lib-1.4.9/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-20 08:58:25.000000 danila-lib-1.4.9/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:58:25.000000 danila-lib-1.4.9/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-20 08:58:25.000000 danila-lib-1.4.9/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 08:58:25.000000 danila-lib-1.4.9/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.652687 danila-lib-1.4.9/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.4.9/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.699565 danila-lib-1.4.9/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.4.9/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.4.9/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.4.9/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.4.9/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.4.9/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.9/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.4.9/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-20 08:57:19.000000 danila-lib-1.4.9/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.4.9/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4337 2024-05-20 08:55:37.000000 danila-lib-1.4.9/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:58:25.746428 danila-lib-1.4.9/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.4.9/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.4.9/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.4.9/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.4.9/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.4.9/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.4.9/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.4.9/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.4.9/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.4.9/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.4.9/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.4.9/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-20 08:58:25.762041 danila-lib-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-20 08:58:21.000000 danila-lib-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.865047 danila-lib-1.5.0/
+-rw-rw-rw-   0        0        0     9615 2024-05-20 09:07:06.865047 danila-lib-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.833806 danila-lib-1.5.0/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.0/danila/__init__.py
+-rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.5.0/danila/danila.py
+-rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.0/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.0/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10693 2024-05-14 12:37:43.000000 danila-lib-1.5.0/danila/danila_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.849443 danila-lib-1.5.0/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-20 09:07:06.000000 danila-lib-1.5.0/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-20 09:07:06.000000 danila-lib-1.5.0/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:07:06.000000 danila-lib-1.5.0/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-20 09:07:06.000000 danila-lib-1.5.0/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 09:07:06.000000 danila-lib-1.5.0/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.849443 danila-lib-1.5.0/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.0/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.849443 danila-lib-1.5.0/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.0/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.0/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.0/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.0/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.5.0/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.0/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.0/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-20 08:57:19.000000 danila-lib-1.5.0/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.0/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 09:06:42.000000 danila-lib-1.5.0/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:07:06.865047 danila-lib-1.5.0/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.0/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.0/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.0/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.0/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.0/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.0/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.0/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.0/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.0/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.0/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.0/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:07:06.865047 danila-lib-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-20 09:07:01.000000 danila-lib-1.5.0/setup.py
```

### Comparing `danila-lib-1.4.9/PKG-INFO` & `danila-lib-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.9
+Version: 1.5.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.9/README.md` & `danila-lib-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila/danila.py` & `danila-lib-1.5.0/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila/danila_v1.py` & `danila-lib-1.5.0/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila/danila_v2.py` & `danila-lib-1.5.0/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila/danila_v3.py` & `danila-lib-1.5.0/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.5.0/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.4.9
+Version: 1.5.0
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.4.9/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.5.0/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/danila_lib.egg-info/requires.txt` & `danila-lib-1.5.0/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/Letters_recognize.py` & `danila-lib-1.5.0/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/Rama_classify_class.py` & `danila-lib-1.5.0/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/Rama_detect_class.py` & `danila-lib-1.5.0/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.5.0/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/Text_detect_class.py` & `danila-lib-1.5.0/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/letters_in_image.py` & `danila-lib-1.5.0/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/models.py` & `danila-lib-1.5.0/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/objs_in_image.py` & `danila-lib-1.5.0/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/neuro/text_recognize_yolo.py` & `danila-lib-1.5.0/data/neuro/text_recognize_yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string
 
     def work_image_cuts(self, number_image_cuts, l, h, w):
         """for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string """
         str = ''
         for number_image_cut in number_image_cuts:
             # cv2.imwrite('data/neuro_classes/cut.jpg', number_image_cut)
-            cur_str = self.work_img_word(number_image_cut, h, w)
+            cur_str = self.work_img_word(number_image_cut, l, h, w)
             if len(cur_str) == l:
                 return cur_str
             if len(cur_str) > len(str):
                 str = cur_str
         return str
 
         # main_method takes all image_text_areas from image_rama_cut and recognize text
@@ -63,17 +63,18 @@
         year = self.work_image_cuts(year_image_cuts, year_l, year_h, year_w)
         label_area = Label_area()
         label_area.labels[Class_text.number] = number
         label_area.labels[Class_text.prod] = prod
         label_area.labels[Class_text.year] = year
         return label_area
 
-    def work_img_word(self, number_image_cut, number_h, number_w):
+    def work_img_word(self, number_image_cut, l, number_h, number_w):
         h, w = number_image_cut.shape[:2]
         cv2.imwrite('img.jpg', number_image_cut)
+        self.model.max_det = l
         results = self.model(['img.jpg'], size=(number_h, number_w))
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
         img_letters = Letters_In_Image.get_letters_in_image_from_yolo_json(res2)
         img_letters.sort_letters()
         img_letters.delete_intersections()
         os.remove('img.jpg')
```

### Comparing `danila-lib-1.4.9/data/result/Image_text_areas.py` & `danila-lib-1.5.0/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/result/Rect.py` & `danila-lib-1.5.0/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/result/Text_area.py` & `danila-lib-1.5.0/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/data/result/Yolo_label_rect.py` & `danila-lib-1.5.0/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.4.9/setup.py` & `danila-lib-1.5.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.4.9',
+  version='1.5.0',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

