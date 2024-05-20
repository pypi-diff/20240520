# Comparing `tmp/ku_of_fuzzy-0.1.5.tar.gz` & `tmp/ku_of_fuzzy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ku_of_fuzzy-0.1.5.tar", last modified: Wed May 15 12:08:32 2024, max compression
+gzip compressed data, was "ku_of_fuzzy-0.1.6.tar", last modified: Mon May 20 15:02:19 2024, max compression
```

## Comparing `ku_of_fuzzy-0.1.5.tar` & `ku_of_fuzzy-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:08:32.023227 ku_of_fuzzy-0.1.5/
--rw-rw-rw-   0        0        0     1089 2024-05-13 01:06:36.000000 ku_of_fuzzy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    17181 2024-05-15 12:08:32.021850 ku_of_fuzzy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    16610 2024-05-15 11:57:34.000000 ku_of_fuzzy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:08:32.017678 ku_of_fuzzy-0.1.5/ku_of_fuzzy/
--rw-rw-rw-   0        0        0        2 2024-05-13 01:06:36.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy/__init__.py
--rw-rw-rw-   0        0        0    37779 2024-05-15 11:53:51.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy/fuzzy_calculate.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:08:32.020826 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/
--rw-rw-rw-   0        0        0    17181 2024-05-15 12:08:31.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-15 12:08:31.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:08:31.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-15 12:08:31.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 12:08:31.000000 ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 12:08:32.023227 ku_of_fuzzy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-05-15 11:52:28.000000 ku_of_fuzzy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:02:19.435773 ku_of_fuzzy-0.1.6/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 01:06:36.000000 ku_of_fuzzy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    17181 2024-05-20 15:02:19.434776 ku_of_fuzzy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16610 2024-05-15 11:57:34.000000 ku_of_fuzzy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 15:02:19.429505 ku_of_fuzzy-0.1.6/ku_of_fuzzy/
+-rw-rw-rw-   0        0        0        2 2024-05-13 01:06:36.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0    38453 2024-05-20 14:53:12.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy/fuzzy_calculate.py
+drwxrwxrwx   0        0        0        0 2024-05-20 15:02:19.432689 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0    17181 2024-05-20 15:02:19.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-20 15:02:19.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 15:02:19.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 15:02:19.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 15:02:19.000000 ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 15:02:19.435773 ku_of_fuzzy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-05-20 14:59:47.000000 ku_of_fuzzy-0.1.6/setup.py
```

### Comparing `ku_of_fuzzy-0.1.5/LICENSE` & `ku_of_fuzzy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ku_of_fuzzy-0.1.5/PKG-INFO` & `ku_of_fuzzy-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku_of_fuzzy
-Version: 0.1.5
+Version: 0.1.6
 Summary: 用于模糊数学计算的Python库
 Home-page: https://github.com/YueorLekai/ku_of_fuzzy
 Author: Yuekai
 Author-email: 1977269004@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ku_of_fuzzy-0.1.5/README.md` & `ku_of_fuzzy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ku_of_fuzzy-0.1.5/ku_of_fuzzy/fuzzy_calculate.py` & `ku_of_fuzzy-0.1.6/ku_of_fuzzy/fuzzy_calculate.py`

 * *Files 2% similar despite different names*

```diff
@@ -811,31 +811,34 @@
         返回两个的内积
     """
     if not isinstance(A, pd.Series) or not isinstance(B, pd.Series):
         raise ValueError("必须是pd.Series对象")
     n = len(A)
     if n != len(B):
         raise ValueError("必须具有相同的长度")
-    # 计算模糊集的内积
-    return A.combine(B, min).max()
+
+    # 使用 .iloc[pos] 来按位置访问Series对象中的值
+    inner_product = pd.Series([min(A.iloc[i], B.iloc[i]) for i in range(n)]).max()
+    return inner_product
 
 
 # 模糊集外积
 def fuzzy_outer_product(A, B):
     """
         A和B为两个pd.Series表示的模糊集
         返回两个的外积
     """
     if not isinstance(A, pd.Series) or not isinstance(B, pd.Series):
         raise ValueError("必须是pd.Series对象")
     n = len(A)
     if n != len(B):
         raise ValueError("必须具有相同的长度")
     # 计算模糊集的外积
-    return A.combine(B, max).min()
+    outer = pd.Series([max(A.iloc[i], B.iloc[i]) for i in range(n)]).min()
+    return outer
 
 
 # 计算两个模糊集的格贴近度
 def lattice_proximity(A, B):
     """
         A和B为两个pd.Series表示的模糊集
         返回的时格贴近度
@@ -952,15 +955,15 @@
 
 # 第五部分：模糊综合评判
 
 # 主因素决定型
 def principal_factor_determination_evaluation(A, R):
     """
         A为pd.Series表示的权重向量
-        R为pd.Dataframe表示的综合评价矩阵
+        R为pd.DataFrame表示的综合评价矩阵
         返回主因素决定型评价向量
     """
     # 确保A是一个Series，R是一个DataFrame
     if not isinstance(A, pd.Series) or not isinstance(R, pd.DataFrame):
         raise ValueError("A必须是pd.Series对象，R必须是pd.DataFrame对象")
     # 创建一个空的Series来保存内积结果
     inner_products = pd.Series(dtype=float)
@@ -979,101 +982,107 @@
 # 主因素突出型
 def principal_factor_prominent_evaluation(A, R):
     """
         A为pd.Series表示的权重向量
         R为pd.Dataframe表示的综合评价矩阵
         返回主因素突出型评价向量
     """
-    # 确保A是一个Series，R是一个DataFrame
-    if not isinstance(A, pd.Series) or not isinstance(R, pd.DataFrame):
-        raise ValueError("A必须是pd.Series对象，R必须是pd.DataFrame对象")
-
-    # 创建一个空的Series来保存每个对象的综合评价值
-    B = pd.Series(dtype=float)
-
-    # 遍历R的每一列，即每个对象
-    for j in R.columns:
+    # 使用.values获取A和R的纯数值数组
+    A_values = A.values
+    R_values = R.values
+    # 创建一个空的列表来保存每个对象的综合评价值
+    B_values = []
+    # 遍历R_values的每一列，即每个对象
+    for j in range(R_values.shape[1]):
         # 计算每个因素的权重与评价值的乘积
-        products = A * R[j]
+        products = A_values * R_values[:, j]
         # 取乘积的最大值作为对象的综合评价值
-        B[j] = products.max()
-
+        B_values.append(products.max())
+    # 将结果转换为Series，不指定索引
+    B = pd.Series(B_values,index=R.columns)
     # 返回包含所有对象综合评价值的Series
     return B
 
 
 # 加权平均型
 def weighted_sum_evaluation(A, R):
     """
         A为pd.Series表示的权重向量
-        R为pd.Dataframe表示的综合评价矩阵
+        R为pd.DataFrame表示的综合评价矩阵
         返回加权平均型评价向量
     """
+    A_values = A.values
+    R_values = R.values
     # 确保A是一个Series，R是一个DataFrame
     if not isinstance(A, pd.Series) or not isinstance(R, pd.DataFrame):
         raise ValueError("A必须是pd.Series对象，R必须是pd.DataFrame对象")
 
     # 创建一个空的Series来保存每个对象的综合评价值
     B = pd.Series(dtype=float)
 
-    # 遍历R的每一列，即每个对象
-    for j in R.columns:
+    # 使用enumerate遍历R的每一列，即每个对象
+    for idx, j in enumerate(R.columns):
         # 计算每个因素的权重与评价值的乘积之和
-        weighted_sum = (A * R[j]).sum()
+        weighted_sum = (A_values * R_values[:, idx]).sum()
         # 将计算结果作为对象的综合评价值
         B[j] = weighted_sum
 
     # 返回包含所有对象综合评价值的Series
     return B
 
 
 # 取小上界和型
 def min_sum_evaluation(A, R):
     """
         A为pd.Series表示的权重向量
-        R为pd.Dataframe表示的综合评价矩阵
+        R为pd.DataFrame表示的综合评价矩阵
         返回取小上界和型评价向量
     """
     # 确保A是一个Series，R是一个DataFrame
     if not isinstance(A, pd.Series) or not isinstance(R, pd.DataFrame):
         raise ValueError("A必须是pd.Series对象，R必须是pd.DataFrame对象")
 
     # 创建一个空的Series来保存每个选项的综合评价值
     B = pd.Series(dtype=float)
 
     # 遍历R的每一列，即每个选项
-    for j in R.columns:
+    for j in range(len(R.columns)):
         # 计算每个因素的权重与评价值的最小值之和
-        min_sum = (A.combine(R[j], min)).sum()
+        min_sum = sum(min(a_val, r_val) for a_val, r_val in zip(A, R.iloc[:, j]))
         # 取和与1之间的最小值作为选项的综合评价值
-        B[j] = min(min_sum, 1)
+        B[R.columns[j]] = min(min_sum, 1)
 
     # 返回包含所有选项综合评价值的Series
     return B
 
 
 # 均衡平均型
 def balanced_average_evaluation(A, R):
     """
         A为pd.Series表示的权重向量
-        R为pd.Dataframe表示的综合评价矩阵
+        R为pd.DataFrame表示的综合评价矩阵
         返回均衡平均型向量
     """
     # 确保A是一个Series，R是一个DataFrame
     if not isinstance(A, pd.Series) or not isinstance(R, pd.DataFrame):
         raise ValueError("A必须是pd.Series对象，R必须是pd.DataFrame对象")
 
     # 创建一个空的Series来保存每个选项的综合评价值
     B = pd.Series(dtype=float)
 
     # 计算每个选项的评价值之和
     r_j_sum = R.sum()
 
     # 遍历R的每一列，即每个选项
-    for j in R.columns:
-        # 计算每个因素的权重与评价值比值的最小值之和
-        normalized_weighted_sum = (A.combine(R[j] / r_j_sum[j], min)).sum()
+    for j in range(len(R.columns)):
+        # 如果这一列的和不为零，则计算normalized_weighted_sum
+        if r_j_sum[R.columns[j]] != 0:
+            # 计算每个因素的权重与评价值比值的最小值之和
+            normalized_weighted_sum = sum(min(a_val, r_val) for a_val, r_val in zip(A, R.iloc[:, j] / r_j_sum[R.columns[j]]))
+        else:
+            # 如果这一列的和为零，则将normalized_weighted_sum设置为0
+            normalized_weighted_sum = 0
         # 将计算结果作为选项的综合评价值
-        B[j] = normalized_weighted_sum
+        B[R.columns[j]] = normalized_weighted_sum
 
     # 返回包含所有选项综合评价值的Series
     return B
```

### Comparing `ku_of_fuzzy-0.1.5/ku_of_fuzzy.egg-info/PKG-INFO` & `ku_of_fuzzy-0.1.6/ku_of_fuzzy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ku_of_fuzzy
-Version: 0.1.5
+Version: 0.1.6
 Summary: 用于模糊数学计算的Python库
 Home-page: https://github.com/YueorLekai/ku_of_fuzzy
 Author: Yuekai
 Author-email: 1977269004@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ku_of_fuzzy-0.1.5/setup.py` & `ku_of_fuzzy-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ku_of_fuzzy',
-    version='0.1.5',
+    version='0.1.6',
     author='Yuekai',
     author_email='1977269004@qq.com',
     description='用于模糊数学计算的Python库',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/YueorLekai/ku_of_fuzzy',
     packages=find_packages(),
```

