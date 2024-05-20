# Comparing `tmp/MPSPEnv-0.0.9.tar.gz` & `tmp/mpspenv-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MPSPEnv-0.0.9.tar", last modified: Sat Feb 24 11:20:35 2024, max compression
+gzip compressed data, was "mpspenv-0.1.0.tar", last modified: Mon May 20 17:36:35 2024, max compression
```

## Comparing `MPSPEnv-0.0.9.tar` & `mpspenv-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134986 MPSPEnv-0.0.9/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MANIFEST.in
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.132253 MPSPEnv-0.0.9/MPSPEnv/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       27 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/__init__.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.131425 MPSPEnv-0.0.9/MPSPEnv/c/
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134432 MPSPEnv-0.0.9/MPSPEnv/c/src/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2833 2024-01-17 21:40:27.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/array.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      589 2024-01-17 21:40:30.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/array.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7131 2024-01-18 09:17:31.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/bay.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      533 2024-01-18 09:12:54.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/bay.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4379 2024-02-05 17:19:30.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/env.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      541 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/env.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1522 2024-01-18 09:19:11.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/random.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      229 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/random.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)      660 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/sort.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/sort.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     5893 2024-01-30 22:33:00.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      934 2024-01-16 19:28:34.000000 MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1653 2024-02-05 17:20:47.000000 MPSPEnv-0.0.9/MPSPEnv/c_interface.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     8690 2024-02-24 11:18:57.000000 MPSPEnv-0.0.9/MPSPEnv/env.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4922 2024-02-04 21:34:43.000000 MPSPEnv-0.0.9/MPSPEnv/visualizer.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-02-24 11:20:35.134604 MPSPEnv-0.0.9/MPSPEnv.egg-info/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)      552 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/SOURCES.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/dependency_links.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/requires.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-02-24 11:20:35.000000 MPSPEnv-0.0.9/MPSPEnv.egg-info/top_level.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3800 2024-02-24 11:20:35.134803 MPSPEnv-0.0.9/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3410 2024-02-14 10:07:42.000000 MPSPEnv-0.0.9/README.md
--rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-02-24 11:20:35.135032 MPSPEnv-0.0.9/setup.cfg
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1065 2024-02-24 11:20:28.000000 MPSPEnv-0.0.9/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.404058 mpspenv-0.1.0/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.0/MANIFEST.in
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.399380 mpspenv-0.1.0/MPSPEnv/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.0/MPSPEnv/__init__.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.397675 mpspenv-0.1.0/MPSPEnv/c/
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.402848 mpspenv-0.1.0/MPSPEnv/c/src/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.0/MPSPEnv/c/src/array.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.0/MPSPEnv/c/src/array.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.0/MPSPEnv/c/src/bay.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.0/MPSPEnv/c/src/bay.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     9914 2024-05-20 17:22:44.000000 mpspenv-0.1.0/MPSPEnv/c/src/env.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      620 2024-05-20 17:04:20.000000 mpspenv-0.1.0/MPSPEnv/c/src/env.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.0/MPSPEnv/c/src/random.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.0/MPSPEnv/c/src/random.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.0/MPSPEnv/c/src/sort.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.0/MPSPEnv/c/src/sort.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1911 2024-05-20 17:05:13.000000 mpspenv-0.1.0/MPSPEnv/c_interface.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7910 2024-05-20 17:21:01.000000 mpspenv-0.1.0/MPSPEnv/env.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.0/MPSPEnv/visualizer.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.403661 mpspenv-0.1.0/MPSPEnv.egg-info/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/requires.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/top_level.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-20 17:36:35.403861 mpspenv-0.1.0/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.0/README.md
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-20 17:36:35.404110 mpspenv-0.1.0/setup.cfg
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-20 17:36:15.000000 mpspenv-0.1.0/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.403134 mpspenv-0.1.0/tests/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1237 2024-05-20 11:15:35.000000 mpspenv-0.1.0/tests/test_env.py
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c/src/array.c` & `mpspenv-0.1.0/MPSPEnv/c/src/array.c`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,34 @@
     for (int i = 0; i < array.n; i++)
     {
         printf("%d ", array.values[i]);
     }
     printf("\n");
 }
 
+Array null_array()
+{
+    Array array;
+    array.values = NULL;
+    array.n = 0;
+    return array;
+}
+
+Array copy_array(Array array)
+{
+    Array copy;
+    copy.values = (int *)calloc(array.n, sizeof(int));
+    copy.n = array.n;
+    for (int i = 0; i < array.n; i++)
+    {
+        copy.values[i] = array.values[i];
+    }
+    return copy;
+}
+
 void print_matrix(Array array, int w, int h)
 {
     assert(array.n == w * h);
     for (int i = 0; i < h; i++)
     {
         for (int j = 0; j < w; j++)
         {
@@ -77,14 +97,46 @@
     }
     for (int i = array.n - n_shifts; i < array.n; i++)
     {
         array.values[i] = 0;
     }
 }
 
+void fill_array(Array array, int value)
+{
+    for (int i = 0; i < array.n; i++)
+    {
+        array.values[i] = value;
+    }
+}
+
+int get_max(Array array)
+{
+    assert(array.n > 0);
+    int max = array.values[0];
+    for (int i = 1; i < array.n; i++)
+    {
+        if (array.values[i] > max)
+        {
+            max = array.values[i];
+        }
+    }
+    return max;
+}
+
+int get_sum(Array array)
+{
+    int sum = 0;
+    for (int i = 0; i < array.n; i++)
+    {
+        sum += array.values[i];
+    }
+    return sum;
+}
+
 Array array_from_ints(int *values, int n)
 {
     Array array;
     array.values = (int *)calloc(n, sizeof(int));
     array.n = n;
     for (int i = 0; i < n; i++)
     {
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c/src/bay.c` & `mpspenv-0.1.0/MPSPEnv/c/src/bay.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "bay.h"
 #include "sort.h"
 #include <assert.h>
 #include <stdio.h>
+#include <stdlib.h>
 
 int containers_in_column(Bay bay, int column)
 {
     return bay.column_counts.values[column];
 }
 
 int is_column_empty(Bay bay, int column)
@@ -14,28 +15,30 @@
 }
 
 int is_full_column(Bay bay, int column)
 {
     return containers_in_column(bay, column) == bay.R;
 }
 
-void update_column_mask(Bay bay, int column)
+Bay copy_bay(Bay bay)
 {
-    // Add mask
-    bay.mask.values[column] = !is_full_column(bay, column);
-    // Remove mask
-    bay.mask.values[column + bay.C] = !is_column_empty(bay, column);
-}
-
-void insert_mask(Bay bay)
-{
-    for (int i = 0; i < bay.C; i++)
-    {
-        update_column_mask(bay, i);
-    }
+    Bay copy;
+    copy.R = bay.R;
+    copy.C = bay.C;
+    copy.N = bay.N;
+    copy.right_most_added_column = malloc(sizeof(int));
+    *copy.right_most_added_column = *bay.right_most_added_column;
+    copy.left_most_removed_column = malloc(sizeof(int));
+    *copy.left_most_removed_column = *bay.left_most_removed_column;
+    copy.added_since_sailing = malloc(sizeof(int));
+    *copy.added_since_sailing = *bay.added_since_sailing;
+    copy.matrix = copy_array(bay.matrix);
+    copy.min_container_per_column = copy_array(bay.min_container_per_column);
+    copy.column_counts = copy_array(bay.column_counts);
+    return copy;
 }
 
 int find_min_container_in_column(Bay bay, int column)
 {
     int min = bay.N;
     const int start_row = bay.R - containers_in_column(bay, column);
 
@@ -54,15 +57,15 @@
 int *min_container_ref(Bay bay, int column)
 {
     return &bay.min_container_per_column.values[column];
 }
 
 // Checks bottom up for containers going to current port (always 1)
 // If container is 1, then it is offloaded, and so are all the containers above it
-void offload_column(Bay bay, int j, Array offloaded_containers)
+void offload_column(Bay bay, int j, Array offloaded_containers, Env *env)
 {
     int offload_column_rest = 0;
     const int min_row = bay.R - containers_in_column(bay, j);
     const int max_row = bay.R - 1;
     for (int i = max_row; i >= min_row; i--)
     {
         const int index = i * bay.C + j;
@@ -80,20 +83,20 @@
     }
     if (offload_column_rest)
     {
         *min_container_ref(bay, j) = find_min_container_in_column(bay, j);
     }
 }
 
-Array bay_offload_containers(Bay bay)
+Array bay_offload_containers(Bay bay, Env *env)
 {
     Array offloaded_containers = get_zeros(bay.N);
     for (int j = 0; j < bay.C; j++)
     {
-        offload_column(bay, j, offloaded_containers);
+        offload_column(bay, j, offloaded_containers, env);
     }
 
     return offloaded_containers;
 }
 
 void decrement_bay(Bay bay)
 {
@@ -105,156 +108,176 @@
             bay.matrix.values[index]--;
         }
         if (containers_in_column(bay, j) > 0)
             bay.min_container_per_column.values[j]--;
     }
 }
 
+void reset_right_most_added_column(Bay bay)
+{
+    *bay.right_most_added_column = bay.C;
+}
+
+void reset_pointer_values(Bay bay)
+{
+    reset_right_most_added_column(bay);
+    *bay.left_most_removed_column = -1;
+    *bay.added_since_sailing = 0;
+}
+
+void update_left_most_removed_column(Bay bay, int column)
+{
+    if (column > *bay.left_most_removed_column)
+        *bay.left_most_removed_column = column;
+    else
+        assert(0);
+}
+
+void update_right_most_added_column(Bay bay, int column)
+{
+    if (column < *bay.right_most_added_column)
+        *bay.right_most_added_column = column;
+    else
+        assert(0);
+}
+
+void sorted_rows_order(Bay bay, Array column_order, int first_affected_row)
+{
+    for (int i = bay.R - 1; i >= first_affected_row; i--)
+    {
+        int *row_values = bay.matrix.values + i * bay.C;
+        Array row_array = array_from_ints_shallow_copy(row_values, bay.C);
+        sort_indexes_using_values(column_order, row_array);
+    }
+}
+
+Array get_column_order(Bay bay)
+{
+    Array column_order = get_range(0, bay.C);
+    sorted_rows_order(bay, column_order, bay.R - get_max(bay.column_counts));
+    return column_order;
+}
+
+void reorder_bay(Bay bay)
+{
+    Array new_column_order = get_column_order(bay);
+
+    reorder_matrix_columns(bay.matrix, bay.C, bay.R, new_column_order);
+    reorder_array(bay.min_container_per_column, new_column_order);
+    reorder_array(bay.column_counts, new_column_order);
+
+    free_array(new_column_order);
+}
+
 // Offloads all containers going to current port (always 1)
 // Returns reshuffled containers
-Array bay_sail_along(Bay bay)
+Array bay_sail_along(Bay bay, Env *env)
 {
-    Array reshuffled = bay_offload_containers(bay);
+    Array reshuffled = bay_offload_containers(bay, env);
     decrement_bay(bay);
     // Ignore 1s, as they are offloaded
     reshuffled.values[1] = 0;
     // And also decrement the reshuffled containers
     shift_array_left(reshuffled, 1);
-    insert_mask(bay);
+    reset_pointer_values(bay);
+    reorder_bay(bay);
+
     return reshuffled;
 }
 
 Bay get_bay(int R, int C, int N)
 {
     Bay bay;
     bay.R = R;
     bay.C = C;
     bay.N = N;
+    bay.right_most_added_column = malloc(sizeof(int));
+    bay.left_most_removed_column = malloc(sizeof(int));
+    bay.added_since_sailing = malloc(sizeof(int));
     bay.matrix = get_zeros(R * C);
     // Initialize to max value + 1
     bay.min_container_per_column = get_full(C, N);
     bay.column_counts = get_zeros(C);
-    bay.mask = get_zeros(2 * bay.C);
-    insert_mask(bay);
+    reset_pointer_values(bay);
 
     return bay;
 }
 
 void free_bay(Bay bay)
 {
+    free(bay.right_most_added_column);
+    free(bay.left_most_removed_column);
+    free(bay.added_since_sailing);
     free_array(bay.matrix);
     free_array(bay.min_container_per_column);
     free_array(bay.column_counts);
-    free_array(bay.mask);
 }
+
 void update_min_post_insertion(Bay bay, int column, int container)
 {
     if (container < *min_container_ref(bay, column))
     {
         *min_container_ref(bay, column) = container;
     }
 }
 
-void insert_container_into_column(Bay bay, int column, int container)
+void insert_containers_into_column(Bay bay, int column, int amount, int container)
 {
-    int row = bay.R - containers_in_column(bay, column) - 1;
-    bay.matrix.values[row * bay.C + column] = container;
-    bay.column_counts.values[column]++;
-}
-
-Array get_lexicographic_column_order(Bay bay, int first_affected_row)
-{
-    Array column_order = get_range(0, bay.C);
-
-    // You only need to check the first affected row and down
-    for (int i = first_affected_row; i < bay.R; i++)
+    for (int i = 0; i < amount; i++)
     {
-        int *row_values = bay.matrix.values + i * bay.C;
-        Array row_array = array_from_ints_shallow_copy(row_values, bay.C);
-        sort_indexes_using_values(column_order, row_array);
+        int row = bay.R - containers_in_column(bay, column) - 1 - i;
+        bay.matrix.values[row * bay.C + column] = container;
     }
-
-    return column_order;
+    bay.column_counts.values[column] += amount;
 }
 
-void reorder_mask(Bay bay, Array correct_column_order)
-{
-    Array add_mask = array_from_ints_shallow_copy(bay.mask.values, bay.C);
-    Array remove_mask = array_from_ints_shallow_copy(bay.mask.values + bay.C, bay.C);
-    reorder_array(add_mask, correct_column_order);
-    reorder_array(remove_mask, correct_column_order);
-}
-
-void reorder_bay(Bay bay, int first_affected_row)
-{
-    Array correct_column_order = get_lexicographic_column_order(bay, first_affected_row);
-
-    reorder_matrix_columns(bay.matrix, bay.C, bay.R, correct_column_order);
-    reorder_array(bay.min_container_per_column, correct_column_order);
-    reorder_array(bay.column_counts, correct_column_order);
-    reorder_mask(bay, correct_column_order);
-
-    free_array(correct_column_order);
-}
-
-void bay_add_container(Bay bay, int column, int container)
+void bay_add_containers(Bay bay, int column, int container, int amount)
 {
     assert(column >= 0 && column < bay.C);
-    assert(containers_in_column(bay, column) < bay.R);
-    insert_container_into_column(bay, column, container);
+    assert(containers_in_column(bay, column) + amount <= bay.R);
+    insert_containers_into_column(bay, column, amount, container);
     update_min_post_insertion(bay, column, container);
-    update_column_mask(bay, column);
-    int first_affected_row = bay.R - containers_in_column(bay, column);
-    reorder_bay(bay, first_affected_row);
+    *bay.added_since_sailing = 1;
+    update_right_most_added_column(bay, column);
+    reorder_bay(bay);
 }
 
-int get_top_container(Bay bay, int column)
+Array pop_containers_from_column(Bay bay, int column, int amount)
 {
-    assert(column >= 0 && column < bay.C);
-    assert(containers_in_column(bay, column) > 0);
-    int row = bay.R - containers_in_column(bay, column);
-    int index = row * bay.C + column;
-    return bay.matrix.values[index];
-}
+    Array reshuffled = get_zeros(bay.N);
+    for (int i = 0; i < amount; i++)
+    {
+        int row = bay.R - containers_in_column(bay, column) + i;
+        int index = row * bay.C + column;
+        int container = bay.matrix.values[index];
 
-int pop_container_from_column(Bay bay, int column)
-{
-    int row = bay.R - containers_in_column(bay, column);
-    int index = row * bay.C + column;
-    int container = bay.matrix.values[index];
+        reshuffled.values[container]++;
 
-    bay.matrix.values[index] = 0;
-    bay.column_counts.values[column]--;
+        bay.matrix.values[index] = 0;
+    }
 
-    return container;
+    bay.column_counts.values[column] -= amount;
+    return reshuffled;
 }
 
 // Assumes the container would be placed at the top of the column
 int is_container_blocking(Bay bay, int column, int container)
 {
     return container > *min_container_ref(bay, column);
 }
 
-void update_min_post_removal(Bay bay, int column, int container)
+void update_min_post_removal(Bay bay, int column)
 {
-    if (*min_container_ref(bay, column) < container)
-        return;
-
-    if (containers_in_column(bay, column) == 0)
-    {
-        *min_container_ref(bay, column) = bay.N;
-        return;
-    }
-
     *min_container_ref(bay, column) = find_min_container_in_column(bay, column);
 }
 
-void bay_pop_container(Bay bay, int column)
+Array bay_pop_containers(Bay bay, int column, int amount)
 {
     assert(column >= 0 && column < bay.C);
-    assert(containers_in_column(bay, column) > 0);
-    int container = pop_container_from_column(bay, column);
-    update_min_post_removal(bay, column, container);
-    update_column_mask(bay, column);
-    int first_affected_row = bay.R - containers_in_column(bay, column) - 1;
-    reorder_bay(bay, first_affected_row);
+    assert(containers_in_column(bay, column) - amount >= 0);
+    Array reshuffled = pop_containers_from_column(bay, column, amount);
+    update_min_post_removal(bay, column);
+    update_left_most_removed_column(bay, column);
+    reorder_bay(bay);
+
+    return reshuffled;
 }
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c/src/random.c` & `mpspenv-0.1.0/MPSPEnv/c/src/random.c`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 #include <stdio.h>
 
 void set_seed(int seed)
 {
     srand(seed);
 }
 
-void set_random_seed()
-{
-    srand(time(NULL));
-}
-
 int random_int()
 {
     return rand();
 }
 
 // Returns a random float in the range [0, 1)
 float random_float()
@@ -48,14 +43,26 @@
 void swap(int *a, int *b)
 {
     int temp = *a;
     *a = *b;
     *b = temp;
 }
 
+void shuffle(int *array, int n)
+{
+    for (int i = 0; i < n; i++)
+    {
+        int j = random_uniform_int(i, n);
+        if (i != j)
+        {
+            swap(&array[i], &array[j]);
+        }
+    }
+}
+
 // v is randomly partitioned into b integers
 int *random_partition(int v, int b)
 {
     int *x = (int *)malloc(b * sizeof(int));
     if (b == 1)
     {
         x[0] = v;
@@ -82,10 +89,12 @@
     x[0] = y[0] - 1;
     for (int i = 1; i < b - 1; i++)
     {
         x[i] = y[i] - y[i - 1] - 1;
     }
     x[b - 1] = v + b - 1 - y[b - 2];
 
+    shuffle(x, b);
+
     free(y);
     return x;
 }
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.c` & `mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.c`

 * *Files 10% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 
 void increment_matrix_and_port(Transportation_Info *T, int port, int container, int n_containers)
 {
     T->matrix.values[port * T->N + container] += n_containers;
     T->containers_per_port.values[port] += n_containers;
 }
 
-void decrement_matrix_and_port(Transportation_Info *T, int port, int container)
+void decrement_matrix_and_port(Transportation_Info *T, int port, int container, int n_containers)
 {
-    T->matrix.values[port * T->N + container] -= 1;
-    T->containers_per_port.values[port] -= 1;
+    T->matrix.values[port * T->N + container] -= n_containers;
+    T->containers_per_port.values[port] -= n_containers;
 }
 
 void insert_containers(Transportation_Info *T, int container, int n_containers)
 {
     increment_matrix_and_port(T, 0, container, n_containers);
     update_last_non_zero_column(T, container);
 }
@@ -156,28 +156,42 @@
 }
 
 int no_containers_at_port(Transportation_Info *T)
 {
     return T->containers_per_port.values[0] == 0;
 }
 
-int transportation_pop_container(Transportation_Info *T)
+int transportation_pop_n_containers(Transportation_Info *T, int n_containers)
 {
     assert(!is_last_port(T));
     assert(!no_containers_at_port(T));
     assert(T->last_non_zero_column >= 0);
+    assert(T->matrix.values[T->last_non_zero_column] >= n_containers);
 
     int container = T->last_non_zero_column;
 
-    decrement_matrix_and_port(T, 0, T->last_non_zero_column);
+    decrement_matrix_and_port(T, 0, T->last_non_zero_column, n_containers);
     insert_last_non_zero_column(T);
 
     return container;
 }
 
+Transportation_Info *copy_transportation_info(Transportation_Info *T)
+{
+    Transportation_Info *copy = malloc(sizeof(Transportation_Info));
+    copy->N = T->N;
+    copy->seed = T->seed;
+    copy->matrix = copy_array(T->matrix);
+    copy->containers_per_port = copy_array(T->containers_per_port);
+    copy->last_non_zero_column = T->last_non_zero_column;
+    copy->current_port = T->current_port;
+
+    return copy;
+}
+
 Transportation_Info *get_empty_transportation_matrix(
     int N)
 {
     Transportation_Info *T = malloc(sizeof(Transportation_Info));
 
     T->N = N;
     T->seed = random_int();
@@ -211,15 +225,14 @@
     Transportation_Info *T = get_empty_transportation_matrix(N);
     insert_seeded_transportation_matrix(T, bay_capacity);
     insert_containers_per_port(T);
     insert_last_non_zero_column(T);
 
     return T;
 }
-
 Transportation_Info *get_specific_transportation_matrix(
     int N,
     int *T_matrix)
 {
     assert(N > 0);
 
     Transportation_Info *T = get_empty_transportation_matrix(N);
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c/src/transportation_matrix.h` & `mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.h`

 * *Files 11% similar despite different names*

```diff
@@ -18,21 +18,23 @@
     int N,
     int bay_capacity);
 
 Transportation_Info *get_specific_transportation_matrix(
     int N,
     int *T_matrix);
 
+Transportation_Info *copy_transportation_info(Transportation_Info *T);
+
 int is_last_port(Transportation_Info *T);
 
 void free_transportation_matrix(Transportation_Info *T);
 
 void transportation_sail_along(Transportation_Info *T);
 
-int transportation_pop_container(Transportation_Info *T);
+int transportation_pop_n_containers(Transportation_Info *T, int n_containers);
 
 void transportation_insert_container(Transportation_Info *T, int container);
 
 void transportation_insert_reshuffled(Transportation_Info *T, Array reshuffled);
 
 int no_containers_at_port(Transportation_Info *T);
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/c_interface.py` & `mpspenv-0.1.0/MPSPEnv/c_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ctypes
-from ctypes import POINTER, c_int, Structure
+from ctypes import POINTER, c_int, Structure, c_char
 import os
 import glob
 
 
 class Array(Structure):
     _fields_ = [
         ("values", POINTER(c_int)),
@@ -12,18 +12,20 @@
 
 
 class Bay(Structure):
     _fields_ = [
         ("R", c_int),
         ("C", c_int),
         ("N", c_int),
+        ("right_most_added_column", POINTER(c_int)),
+        ("left_most_updated_column", POINTER(c_int)),
+        ("added_since_sailing", POINTER(c_int)),
         ("matrix", Array),
         ("min_container_per_column", Array),
         ("column_counts", Array),
-        ("mask", Array),
     ]
 
 
 class Transportation_Info(Structure):
     _fields_ = [
         ("matrix", Array),
         ("containers_per_port", Array),
@@ -34,17 +36,20 @@
     ]
 
 
 class Env(Structure):
     _fields_ = [
         ("T", POINTER(Transportation_Info)),
         ("bay", Bay),
-        ("one_hot_bay", Array),
         ("flat_T_matrix", Array),
-        ("skip_last_port", c_int),
+        ("mask", Array),
+        ("auto_move", c_int),
+        ("total_reward", POINTER(c_int)),
+        ("containers_left", POINTER(c_int)),
+        ("containers_placed", POINTER(c_int)),
     ]
 
 
 class StepInfo(Structure):
     _fields_ = [
         ("is_terminal", c_int),
         ("reward", c_int),
@@ -67,10 +72,9 @@
 c_lib.get_random_env.restype = Env
 
 c_lib.get_specific_env.argtypes = [c_int, c_int, c_int, POINTER(c_int), c_int]
 c_lib.get_specific_env.restype = Env
 
 c_lib.free_env.argtypes = [Env]
 
-c_lib.set_random_seed.argtypes = []
-
-c_lib.set_seed.argtypes = [c_int]
+c_lib.copy_env.argtypes = [Env, c_int]
+c_lib.copy_env.restype = Env
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/env.py` & `mpspenv-0.1.0/MPSPEnv/env.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,145 +1,182 @@
-from MPSPEnv.c_interface import c_lib
+from MPSPEnv.c_interface import c_lib, Env as c_Env
 import numpy as np
-from gymnasium import spaces
 import gymnasium as gym
 from MPSPEnv.visualizer import Visualizer
 import warnings
-from ctypes import POINTER, c_int
+import ctypes
+
+
+class ActionNotAllowed(Exception):
+    pass
+
+
+class LazyNdarray:
+    def __init__(self, env: c_Env, attributes: list[str], shape: tuple[int, int]):
+        self.env = env
+        self.attributes = attributes
+        self.shape = shape
+        self.store = None
+
+    @property
+    def ndarray(self):
+        if self.store is None:
+            self._build_store()
+
+        return self.store
+
+    def _build_store(self):
+        self.store = self.env
+        for attr in self.attributes:
+            self.store = getattr(self.store, attr)
+
+        self.store = np.ctypeslib.as_array(self.store.values, shape=self.shape)
 
 
 class Env(gym.Env):
     """
     Gym environment for the Multi-Port Stowage Planning Problem (MPSP).
     The environment is defined by the following parameters:
     - R: number of rows in the bay
     - C: number of columns in the bay
     - N: number of ports
-    - skip_last_port: whether to terminate episodes at the second to last port (default: False)
-    - take_first_action: whether to automaticlly place the first container of every episode (default: False)
-    - strict_mask: whether to break when an invalid action is taken. Otherwise a penalty of -10 is given (default: False)
     """
 
     def __init__(
         self,
         R: int,
         C: int,
         N: int,
-        skip_last_port: bool = False,
-        take_first_action: bool = False,
-        strict_mask: bool = False,
+        auto_move: bool = False,
+        speedy: bool = False,
     ):
         super().__init__()
         assert R > 0, f"R must be positive but was {R}"
         assert C > 0, f"C must be positive but was {C}"
         assert N > 0, f"N must be positive but was {N}"
         self.R = R
         self.C = C
         self.N = N
         self._env = None
         self.visualizer = None
-        self.skip_last_port = skip_last_port
-        self.take_first_action = take_first_action
-        self.strict_mask = strict_mask
-        self.action_probs = None
-        self.total_reward = 0
-
-        self._set_gym_interface()
-
-    def _set_gym_interface(self):
-        self.render_mode = "human"
-        self.action_space = spaces.Discrete(2 * self.C)
-        one_hot_bay_def = spaces.Box(
-            low=0, high=1, shape=(self.N - 1, self.R, self.C), dtype=np.int32
-        )
-        flat_T__def = spaces.Box(
-            low=0,
-            high=self.R * self.C,
-            shape=(self.N * (self.N - 1) // 2,),
-            dtype=np.int32,
-        )
-        self.observation_space = spaces.Dict(
-            {
-                "one_hot_bay": one_hot_bay_def,
-                "flat_T": flat_T__def,
-            }
-        )
+        self.auto_move = auto_move
+        self.speedy = speedy
 
     def step(self, action: int):
-        assert (
-            0 <= action < 2 * self.C
-        ), f"Action must be in the range [0, 2C). The first C actions correspond to adding a container into the respective column, the last C actions correspond to removing a container from the respective column."
-        if self.strict_mask:
-            assert (
-                self._mask[action] == 1
-            ), f"The action {action} is not allowed. The mask is {self._mask}"
-
-        reward = -10
-        is_terminal = False
-
-        if self._mask[action] == 1:
-            step_info = c_lib.step(self._env, action)
-            reward = step_info.reward
-            is_terminal = bool(step_info.is_terminal)
+        assert self._env is not None, "The environment must be reset before stepping."
+        self._check_action(action)
 
-        self.total_reward += reward
-        self.steps += 1
+        step_info = c_lib.step(self._env, action)
+        reward = step_info.reward
+        self.terminal = bool(step_info.is_terminal)
 
-        return (
-            self._get_observation(),
-            reward,
-            is_terminal,
-            False,
-            {},
-        )
+        if self.speedy:
+            return None
+        else:
+            return (
+                self._get_observation(),
+                reward,
+                self.terminal,
+                False,
+                {},
+            )
 
-    def _reset_random_c_env(self, seed: int = None):
-        if self._env is not None:
-            c_lib.free_env(self._env)
+    def copy(self):
+        new_env = Env(
+            R=self.R,
+            C=self.C,
+            N=self.N,
+            auto_move=self.auto_move,
+            speedy=self.speedy,
+        )
+        new_env._env = c_lib.copy_env(self._env)
+        new_env.terminal = self.terminal
+        new_env._set_stores()
 
-        if seed is not None:
-            c_lib.set_seed(seed)
-        else:
-            c_lib.set_random_seed()
+        return new_env
 
-        self._env = c_lib.get_random_env(
-            self.R, self.C, self.N, int(self.skip_last_port)
-        )
-        self._set_numpy_views()
+    def reset(self, seed: int = None, options=None):
+        self._reset_random_c_env(seed)
+        self._set_stores()
+        self.terminal = False
 
-    def _reset_specific_c_env(self, transportation: np.ndarray):
-        if self._env is not None:
-            c_lib.free_env(self._env)
+        if self.speedy:
+            return None
+        else:
+            return self._get_observation(), {}
 
-        self._env = c_lib.get_specific_env(
-            self.R,
-            self.C,
-            self.N,
-            transportation.ctypes.data_as(POINTER(c_int)),
-            int(self.skip_last_port),
-        )
-        self._set_numpy_views()
+    def reset_to_transportation(self, transportation: np.ndarray):
+        self._assert_transportation(transportation)
+        self._reset_specific_c_env(transportation)
+        self._set_stores()
+        self.terminal = False
+
+        if self.speedy:
+            return None
+        else:
+            return self._get_observation(), {}
 
     def render(self):
         if self.visualizer == None:
             self.visualizer = Visualizer(self.R, self.C, self.N)
 
-        return self.visualizer.render(
-            self.bay, self.T, self.total_reward, self.action_probs
-        )
+        return self.visualizer.render(self.bay, self.T, self.total_reward)
 
-    def reset(self, seed: int = None, options=None):
-        self._reset_random_c_env(seed)
-        self.total_reward = 0
-        self.steps = 0
+    def close(self):
+        if self._env is not None:
+            c_lib.free_env(self._env)
+            self._env = None
 
-        if self.take_first_action:
-            self.step(0)
+    def _check_action(self, action: int):
+        if 0 > action or action >= 2 * self.C * self.R:
+            raise ActionNotAllowed
+        if self.mask_store.ndarray[action] != 1:
+            raise ActionNotAllowed
 
-        return self._get_observation(), {}
+    @property
+    def total_reward(self) -> int:
+        return self._env.total_reward.contents.value
+
+    @property
+    def containers_left(self) -> int:
+        return self._env.containers_left.contents.value
+
+    @property
+    def containers_placed(self) -> int:
+        return self._env.containers_placed.contents.value
+
+    @property
+    def remaining_ports(self) -> int:
+        return self.N - 1 - self._env.T.contents.current_port
+
+    @property
+    def bay(self) -> np.ndarray:
+        return self.bay_store.ndarray.copy()
+
+    @property
+    def T(self) -> np.ndarray:
+        return self.T_store.ndarray.copy()
+
+    @property
+    def flat_T(self) -> np.ndarray:
+        return self.flat_T_store.ndarray.copy()
+
+    @property
+    def mask(self) -> np.ndarray:
+        return self.mask_store.ndarray.copy()
+
+    def _set_stores(self):
+        self.bay_store = LazyNdarray(self._env, ["bay", "matrix"], (self.R, self.C))
+        self.T_store = LazyNdarray(
+            self._env, ["T", "contents", "matrix"], (self.N, self.N)
+        )
+        self.flat_T_store = LazyNdarray(
+            self._env, ["flat_T_matrix"], ((self.N - 1) * self.N // 2,)
+        )
+        self.mask_store = LazyNdarray(self._env, ["mask"], (2 * self.C * self.R,))
 
     def _assert_transportation(self, transportation: np.ndarray):
         assert (
             transportation.dtype == np.int32
         ), f"Transportation matrix must be of type np.int32 but was {transportation.dtype}"
         assert transportation.shape == (
             self.N,
@@ -167,110 +204,58 @@
                 for j in range(i + 1, self.N):
                     total += transportation[k, j]
             if total > capacity:
                 return False
 
         return True
 
-    def reset_to_transportation(self, transportation: np.ndarray):
-        self._assert_transportation(transportation)
-        self._reset_specific_c_env(transportation)
-        self.total_reward = 0
-
-        if self.take_first_action:
-            self.step(0)
-
-        return self._get_observation(), {}
-
     def _get_observation(self):
         return {
-            "one_hot_bay": self.one_hot_bay,
-            "flat_T": self.flat_T / (self.R * self.C),  # Normalize to [0, 1]
+            "bay": self.bay / self.remaining_ports,
+            "flat_T": self.flat_T / (self.R * self.C),
+            "mask": self.mask,
+            "containers_left": self.containers_left,
         }
 
-    def action_masks(self):
-        return self._mask.copy()
-
-    @property
-    def bay(self):
-        return self._bay.copy()
-
-    @property
-    def one_hot_bay(self):
-        return self._one_hot_bay.copy()
-
-    @property
-    def T(self):
-        return self._T.copy()
+    def _reset_random_c_env(self, seed: int = None):
+        if self._env is not None:
+            c_lib.free_env(self._env)
 
-    @property
-    def flat_T(self):
-        return self._flat_T.copy()
+        if seed is not None:
+            c_lib.set_seed(seed)
+        else:
+            c_lib.set_seed(np.random.randint(0, 2**32))
 
-    def print(self):
-        print("Bay:")
-        print(self._bay)
-        print("T:")
-        print(self._T)
-        print("Mask:")
-        print(self._mask)
-        print()
+        self._env = c_lib.get_random_env(self.R, self.C, self.N, int(self.auto_move))
 
-    def close(self):
+    def _reset_specific_c_env(self, transportation: np.ndarray):
         if self._env is not None:
             c_lib.free_env(self._env)
-            self._env = None
+
+        self._env = c_lib.get_specific_env(
+            self.R,
+            self.C,
+            self.N,
+            transportation.ctypes.data_as(ctypes.POINTER(ctypes.c_int)),
+            int(self.auto_move),
+        )
 
     def __del__(self):
         if self._env is not None:
             warnings.warn(
                 "Env was not closed properly. Please call .close() to avoid memory leaks."
             )
             self.close()
 
     def __hash__(self):
-        return hash(self.bay.tobytes() + self.flat_T.tobytes())
-
-    def __eq__(self, other):
-        return np.array_equal(self.bay, other.bay) and np.array_equal(
-            self.flat_T, other.flat_T
+        return hash(
+            self.bay_store.ndarray.tobytes()
+            + self.flat_T_store.ndarray.tobytes()
+            + self.mask_store.ndarray.tobytes()
         )
 
-    def _set_numpy_views(self):
-        # The following numpy arrays are views of the underlying C arrays
-        # You should always .copy() them before using them
-        self._bay = np.ctypeslib.as_array(
-            self._env.bay.matrix.values, shape=(self.R, self.C)
-        )
-        self._T = np.ctypeslib.as_array(
-            self._env.T.contents.matrix.values, shape=(self.N, self.N)
-        )
-        self._mask = np.ctypeslib.as_array(
-            self._env.bay.mask.values, shape=(2 * self.C,)
-        )
-        self._flat_T = np.ctypeslib.as_array(
-            self._env.flat_T_matrix.values, shape=((self.N - 1) * self.N // 2,)
-        )
-        self._one_hot_bay = np.ctypeslib.as_array(
-            self._env.one_hot_bay.values, shape=(self.N - 1, self.R, self.C)
-        )
-
-    def copy(self):
-        new_env = Env(
-            self.R,
-            self.C,
-            self.N,
-            self.skip_last_port,
-            self.take_first_action,
-            self.strict_mask,
+    def __eq__(self, other: "Env"):
+        return (
+            np.array_equal(self.bay_store.ndarray, other.bay_store.ndarray)
+            and np.array_equal(self.flat_T_store.ndarray, other.flat_T_store.ndarray)
+            and np.array_equal(self.mask_store.ndarray, other.mask_store.ndarray)
         )
-        new_env.reset()
-        new_env._bay[...] = self._bay
-        new_env._T[...] = self._T
-        new_env._mask[...] = self._mask
-        new_env._flat_T[...] = self._flat_T
-        new_env._one_hot_bay[...] = self._one_hot_bay
-        new_env.total_reward = self.total_reward
-        new_env.steps = self.steps
-        new_env.action_probs = self.action_probs
-
-        return new_env
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv/visualizer.py` & `mpspenv-0.1.0/MPSPEnv/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 if Bay[i, j] < min_in_column:
                     min_in_column = Bay[i, j]
                 elif Bay[i, j] > min_in_column:
                     blocking_containers[i, j] = 1
 
         return blocking_containers
 
-    def render(self, Bay, T, sum_reward, action_probs):
+    def render(self, Bay, T, sum_reward, action_probs=None):
         pygame.event.pump()
         self.screen.fill((255, 255, 255))
         self._render_bay(Bay)
         self._render_T(T)
         self._render_reward(sum_reward)
         self._render_action_probs(action_probs)
         pygame.display.flip()
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv.egg-info/PKG-INFO` & `mpspenv-0.1.0/MPSPEnv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.0.9
+Version: 0.1.0
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
@@ -14,34 +14,31 @@
 This package implements the mathematical model of the "Multi Port Stowage Planning" (MPSP) problem, introduced in [Avriel et al. 1998](https://www.researchgate.net/publication/242916342_Stowage_planning_for_container_ships_to_reduce_the_number_of_shifts), as a reinforcement learning environment using the [Gymnasium API](https://gymnasium.farama.org/api/env/).
 
 The Env class has the following input parameters:
 
 - **R** (int): number of rows
 - **C** (int): number of columns
 - **N** (int): number of ports
-- **skip_last_port** (boolean): if true, the environment will terminate at the second to last port. This is useful for speeding up training, as the last port is trivial to solve.
-- **take_first_action** (boolean): if true, the environment automaticlly places the first container of every episode. This is useful for speeding up training, as the first action is trivial.
-- **strict_mask** (boolean): if true, the environment will break when an invalid action is taken. Otherwise a penalty of -10 is given, and no change is made to the state.
 
 The env observations consist of a dictionary with the one hot encoded bay, and the upper triangular part of the transportation matrix as a flattened array.
 
 ![](https://raw.githubusercontent.com/hojmax/MPSPEnv/main/env.png)
-*Screenshot from the environment. The left matrix is the bay, and the right matrix is the transportation matrix. "x" denotes blocking containers. The reward decreases by one for each reshuffle necessitated by the agents stowage plan.*
+_Screenshot from the environment. The left matrix is the bay, and the right matrix is the transportation matrix. "x" denotes blocking containers. The reward decreases by one for each reshuffle necessitated by the agents stowage plan._
 
 Note that since the mathematical model disregards any stability constraints, the env automatically swaps the column order in a lexocographic manor, based on the containers in the columns. This reduces the state space, by a factor of almost $C!$. Furthmore, the transportation matrix, is reshifted up and to the left, for each port, to reduce the state space even further. This means that from the point of view of the agent, it never leaves the first port.
 
 When using the environment, you should call `env.close()` before exiting your program, to avoid memory leaks.
 
 Minimal usage with [Stable Baselines](https://stable-baselines.readthedocs.io/en/master/):
 
 ```python
 from MPSPEnv import Env
 from sb3_contrib.ppo_mask import MaskablePPO
 
-train_env = Env(R=8, C=4, N=5, skip_last_port=True)
+train_env = Env(R=8, C=4, N=5)
 
 model = MaskablePPO(
     "MultiInputPolicy",
     train_env
 )
 
 model.learn(
```

### Comparing `MPSPEnv-0.0.9/MPSPEnv.egg-info/SOURCES.txt` & `mpspenv-0.1.0/MPSPEnv.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 MPSPEnv/c/src/env.c
 MPSPEnv/c/src/env.h
 MPSPEnv/c/src/random.c
 MPSPEnv/c/src/random.h
 MPSPEnv/c/src/sort.c
 MPSPEnv/c/src/sort.h
 MPSPEnv/c/src/transportation_matrix.c
-MPSPEnv/c/src/transportation_matrix.h
+MPSPEnv/c/src/transportation_matrix.h
+tests/test_env.py
```

### Comparing `MPSPEnv-0.0.9/PKG-INFO` & `mpspenv-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.0.9
+Version: 0.1.0
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
@@ -14,34 +14,31 @@
 This package implements the mathematical model of the "Multi Port Stowage Planning" (MPSP) problem, introduced in [Avriel et al. 1998](https://www.researchgate.net/publication/242916342_Stowage_planning_for_container_ships_to_reduce_the_number_of_shifts), as a reinforcement learning environment using the [Gymnasium API](https://gymnasium.farama.org/api/env/).
 
 The Env class has the following input parameters:
 
 - **R** (int): number of rows
 - **C** (int): number of columns
 - **N** (int): number of ports
-- **skip_last_port** (boolean): if true, the environment will terminate at the second to last port. This is useful for speeding up training, as the last port is trivial to solve.
-- **take_first_action** (boolean): if true, the environment automaticlly places the first container of every episode. This is useful for speeding up training, as the first action is trivial.
-- **strict_mask** (boolean): if true, the environment will break when an invalid action is taken. Otherwise a penalty of -10 is given, and no change is made to the state.
 
 The env observations consist of a dictionary with the one hot encoded bay, and the upper triangular part of the transportation matrix as a flattened array.
 
 ![](https://raw.githubusercontent.com/hojmax/MPSPEnv/main/env.png)
-*Screenshot from the environment. The left matrix is the bay, and the right matrix is the transportation matrix. "x" denotes blocking containers. The reward decreases by one for each reshuffle necessitated by the agents stowage plan.*
+_Screenshot from the environment. The left matrix is the bay, and the right matrix is the transportation matrix. "x" denotes blocking containers. The reward decreases by one for each reshuffle necessitated by the agents stowage plan._
 
 Note that since the mathematical model disregards any stability constraints, the env automatically swaps the column order in a lexocographic manor, based on the containers in the columns. This reduces the state space, by a factor of almost $C!$. Furthmore, the transportation matrix, is reshifted up and to the left, for each port, to reduce the state space even further. This means that from the point of view of the agent, it never leaves the first port.
 
 When using the environment, you should call `env.close()` before exiting your program, to avoid memory leaks.
 
 Minimal usage with [Stable Baselines](https://stable-baselines.readthedocs.io/en/master/):
 
 ```python
 from MPSPEnv import Env
 from sb3_contrib.ppo_mask import MaskablePPO
 
-train_env = Env(R=8, C=4, N=5, skip_last_port=True)
+train_env = Env(R=8, C=4, N=5)
 
 model = MaskablePPO(
     "MultiInputPolicy",
     train_env
 )
 
 model.learn(
```

### Comparing `MPSPEnv-0.0.9/setup.py` & `mpspenv-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from setuptools import setup, Extension
+import glob
 
 ext_modules = Extension(
     "MPSPEnv.c_lib",
-    sources=[
-        "MPSPEnv/c/src/array.c",
-        "MPSPEnv/c/src/bay.c",
-        "MPSPEnv/c/src/env.c",
-        "MPSPEnv/c/src/random.c",
-        "MPSPEnv/c/src/sort.c",
-        "MPSPEnv/c/src/transportation_matrix.c",
-    ],
+    sources=glob.glob("MPSPEnv/c/src/*.c"),
     extra_compile_args=["-O3", "-DNDEBUG"],
     extra_link_args=["-O3", "-DNDEBUG"],
     include_dirs=["MPSPEnv/c/src"],
     language="c",
 )
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MPSPEnv",
-    version="0.0.9",
+    version="0.1.0",
     author="Axel Højmark",
     author_email="axelhojmark@gmail.com",
     description="A reinforcement learning environment for the Multi Port Stowage Planning problem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[ext_modules],
     packages=["MPSPEnv"],
```

