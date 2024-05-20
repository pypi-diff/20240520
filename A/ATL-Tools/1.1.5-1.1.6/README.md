# Comparing `tmp/atl_tools-1.1.5.tar.gz` & `tmp/atl_tools-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.1.5.tar", last modified: Mon May  6 03:17:50 2024, max compression
+gzip compressed data, was "atl_tools-1.1.6.tar", last modified: Mon May 20 07:29:50 2024, max compression
```

## Comparing `atl_tools-1.1.5.tar` & `atl_tools-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/ATL_Tools/
--rw-rw-r--   0 atl       (1002) atl       (1002)    30727 2024-05-06 02:59:37.000000 atl_tools-1.1.5/ATL_Tools/ATL_gdal.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.5/ATL_Tools/ATL_path.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.5/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     5049 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     5049 2024-05-06 03:17:50.219870 atl_tools-1.1.5/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)     4750 2024-05-06 03:07:18.000000 atl_tools-1.1.5/README.md
--rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-05-06 03:02:11.000000 atl_tools-1.1.5/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-05-06 03:17:50.219870 atl_tools-1.1.5/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    33181 2024-05-20 07:19:50.000000 atl_tools-1.1.6/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.6/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2844 2024-05-20 07:20:13.000000 atl_tools-1.1.6/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-20 07:29:50.667467 atl_tools-1.1.6/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     5272 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-05-20 07:29:50.000000 atl_tools-1.1.6/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     5272 2024-05-20 07:29:50.667467 atl_tools-1.1.6/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4973 2024-05-20 07:27:23.000000 atl_tools-1.1.6/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-05-20 07:23:25.000000 atl_tools-1.1.6/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-05-20 07:29:50.667467 atl_tools-1.1.6/setup.cfg
```

### Comparing `atl_tools-1.1.5/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.6/ATL_Tools/ATL_gdal.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
             Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
             raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
             crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
             crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan,支持alpha
             Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
             resample_image,      # ✔使用GDAL对图像进行重采样
             shp_to_geojson,      # ✔将shp文件转为geojson文件
+            cut_image_with_overlap, # 将大图裁切为小图，支持重叠
+
         )
                             
     ________________________________________________________________
     >>> # 示例1-读取影像为数组并返回信息
     >>> img = read_img_to_array_with_info(img_path) # 读取图片，并输出图片信息
     ________________________________________________________________
     >>> # 示例2-读取影像为数组
@@ -802,13 +804,71 @@
         output_geojson,    # 输出文件路径
         input_shp   # 输入Shapefile文件路径
     ]
 
     # 调用ogr2ogr工具执行转换
     subprocess.run(ogr2ogr_cmd)
 
-    
+def cut_image_with_overlap(input_file, output_dir, tile_size=5000, overlap=500):
+    """将大图裁切成小图，以供GPU可以进行推理
+    Args:
+        input_file (str): 输入图像路径
+        output_dir (str): 输出图像路径
+        tile_size (int): 图像块的大小，默认为5000
+        overlap (int): 图像块的重叠大小，默认为500
 
+    Returns: 
+        None, 保存裁切后的图像至指定目录。
+    """
+    # 打开输入图像
+    dataset = gdal.Open(input_file)
+    if not dataset:
+        raise FileNotFoundError(f"Unable to open {input_file}")
+
+    # 获取图像尺寸
+    width = dataset.RasterXSize
+    height = dataset.RasterYSize
+
+    # 获取投影和地理变换信息
+    projection = dataset.GetProjection()
+    geotransform = dataset.GetGeoTransform()
+
+    # 计算图像块的步长（减去重叠部分）
+    step_size = tile_size - overlap
+
+    # 计算图像块的数量
+    x_tiles = (width + step_size - 1) // step_size
+    y_tiles = (height + step_size - 1) // step_size
+    print(f'正在裁切 {input_file} ...')
+    print(f'该图像将被裁切为 {x_tiles*y_tiles} 个 {tile_size}x{tile_size} 的小图....')
+
+    for i in range(x_tiles):
+        for j in range(y_tiles):
+            # 计算图像块的像素范围
+            x_offset = i * step_size
+            y_offset = j * step_size
+
+            # 计算实际读取的像素范围
+            x_size = min(tile_size, width - x_offset)
+            y_size = min(tile_size, height - y_offset)
+
+            # 计算输出的地理范围
+            minx = geotransform[0] + x_offset * geotransform[1] + y_offset * geotransform[2]
+            maxy = geotransform[3] + x_offset * geotransform[4] + y_offset * geotransform[5]
+            maxx = minx + x_size * geotransform[1] + y_size * geotransform[2]
+            miny = maxy + x_size * geotransform[4] + y_size * geotransform[5]
+
+            # 裁切图像块
+            output_img_path = os.path.join(output_dir,f'{os.path.basename(input_file).split(".")[0]}_{i}_{j}.tif')
+            gdal.Translate(
+                output_img_path,
+                dataset,
+                srcWin=[x_offset, y_offset, x_size, y_size],
+                format='GTiff',
+                outputSRS=projection,
+                outputBounds=[minx, miny, maxx, maxy]
+            )
+    print(f"{input_file} 已经裁切完成")
```

### Comparing `atl_tools-1.1.5/ATL_Tools/ATL_path.py` & `atl_tools-1.1.6/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.5/ATL_Tools/__init__.py` & `atl_tools-1.1.6/ATL_Tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
             Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
             Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
             raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
             crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
             crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
             Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-            resample_image      # ✔使用GDAL对图像进行重采样
+            resample_image,      # ✔使用GDAL对图像进行重采样
+            shp_to_geojson,      # ✔将shp文件转为geojson文件
+            cut_image_with_overlap, # 将大图裁切为小图，支持重叠
         )
 
 ---
 示例程序：
 ----       
 示例1-根据json批量裁切影像根据矢量批量裁切影像
```

### Comparing `atl_tools-1.1.5/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.6/ATL_Tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.5
+Version: 1.1.6
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
+最新版本 v1.1.6
 ## 0. 简介
 ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
 如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
 ## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
@@ -33,14 +34,15 @@
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image,      # ✔使用GDAL对图像进行重采样
     shp_to_geojson,      # ✔将shp文件转为geojson文件
+    cut_image_with_overlap, # 将大图裁切为小图，支持重叠
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -88,7 +90,8 @@
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
 - 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
+- 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
```

### Comparing `atl_tools-1.1.5/PKG-INFO` & `atl_tools-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.5
+Version: 1.1.6
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
+最新版本 v1.1.6
 ## 0. 简介
 ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
 如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
 ## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
@@ -33,14 +34,15 @@
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image,      # ✔使用GDAL对图像进行重采样
     shp_to_geojson,      # ✔将shp文件转为geojson文件
+    cut_image_with_overlap, # 将大图裁切为小图，支持重叠
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -88,7 +90,8 @@
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
 - 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
+- 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
```

### Comparing `atl_tools-1.1.5/README.md` & `atl_tools-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # ATL_Tools 使用指南
+最新版本 v1.1.6
 ## 0. 简介
 ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
 如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
 ## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
@@ -25,14 +26,15 @@
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image,      # ✔使用GDAL对图像进行重采样
     shp_to_geojson,      # ✔将shp文件转为geojson文件
+    cut_image_with_overlap, # 将大图裁切为小图，支持重叠
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -79,8 +81,9 @@
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
-- 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
+- 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
+- 2024-05-20 v1.1.6 ATL_gdal 中 增加 `cut_image_with_overlap()`支持将大图裁切成指定尺寸的小图，并带有坐标。
```

