# Comparing `tmp/iconmatch-0.0.1.tar.gz` & `tmp/iconmatch-0.0.2.tar.gz`

## Comparing `iconmatch-0.0.1.tar` & `iconmatch-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/IconMatch.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/__init__.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/box.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/helpers.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/manual_test.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/rectangle.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 iconmatch-0.0.1/IconMatch/weighted_quick_unionUF.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 iconmatch-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 iconmatch-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 iconmatch-0.0.1/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 iconmatch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 iconmatch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/IconMatch.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/__init__.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/box.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/helpers.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/manual_test.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/rectangle.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 iconmatch-0.0.2/IconMatch/weighted_quick_unionUF.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 iconmatch-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 iconmatch-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 iconmatch-0.0.2/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 iconmatch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 iconmatch-0.0.2/PKG-INFO
```

### Comparing `iconmatch-0.0.1/IconMatch/manual_test.py` & `iconmatch-0.0.2/IconMatch/manual_test.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from PIL import ImageGrab
-from pynput import mouse
-import IconMatch
-from IconMatch.helpers import run_sift, save_img
-
-
-def main():
-    """
-    Manual test is an interactive screen shot tool that will perform SIFT on the image.
-    todo: Add more options for edge detection algorithm and options on where to save image.
-    todo: Add functionality for previewing before saving an image.
-    """
-    print("Choose the top left and bottom right coordinates of your box.")
-
-    button_presses = []
-
-    # Stream of events
-    with mouse.Events() as events:
-        for event in events:
-            if hasattr(event, "button") and event.pressed:
-                print(
-                    "The {0} button was {1} at the following coordinates: x:{2}, y:{3}".format(
-                        event.button,
-                        "pressed" if event.pressed else "released",
-                        event.x,
-                        event.y,
-                    )
-                )
-                button_presses.append(event)
-            if len(button_presses) == 2:
-                break
-
-    screen_shot = ImageGrab.grab(
-        bbox=(
-            button_presses[0].x,
-            button_presses[0].y,
-            button_presses[1].x,
-            button_presses[1].y,
-        )
-    )
-
-    save_img(screen_shot, "pre")
-    run_sift(screen_shot)
-    save_img(screen_shot, "post")
-
-
-if __name__ == "__main__":
-    main()
+from PIL import ImageGrab
+from pynput import mouse
+import IconMatch
+from IconMatch.helpers import run_sift, save_img
+
+
+def main():
+    """
+    Manual test is an interactive screen shot tool that will perform SIFT on the image.
+    todo: Add more options for edge detection algorithm and options on where to save image.
+    todo: Add functionality for previewing before saving an image.
+    """
+    print("Choose the top left and bottom right coordinates of your box.")
+
+    button_presses = []
+
+    # Stream of events
+    with mouse.Events() as events:
+        for event in events:
+            if hasattr(event, "button") and event.pressed:
+                print(
+                    "The {0} button was {1} at the following coordinates: x:{2}, y:{3}".format(
+                        event.button,
+                        "pressed" if event.pressed else "released",
+                        event.x,
+                        event.y,
+                    )
+                )
+                button_presses.append(event)
+            if len(button_presses) == 2:
+                break
+
+    screen_shot = ImageGrab.grab(
+        bbox=(
+            button_presses[0].x,
+            button_presses[0].y,
+            button_presses[1].x,
+            button_presses[1].y,
+        )
+    )
+
+    save_img(screen_shot, "pre")
+    run_sift(screen_shot)
+    save_img(screen_shot, "post")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `iconmatch-0.0.1/IconMatch/rectangle.py` & `iconmatch-0.0.2/IconMatch/rectangle.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import math
-import sys
-
-from typing import List, Tuple
-
-
-class Rectangle:
-    """
-    Representation of a rectangle in two dimensional space.
-
-    Note: Keep in mind that due to OpenCV's representation of the screen, y increases from top to bottom!
-                            0 - x +
-                            |
-                            y
-                            +
-    Where top, bottom, left and right are named relative to cartesian coordinates. The below
-    diagram shows what this entails.
-                           Top
-                        --------
-                        |      |
-                   Left |      | Right
-                        |      |
-                        --------
-                         Bottom
-    """
-
-    def __init__(self, top: int, left: int, bottom: int, right: int):
-        """
-        Create a rectangle in Cartesian notation
-        """
-
-        self.top = top
-        self.left = left
-        self.bottom = bottom
-        self.right = right
-
-        # stored for cached initialization
-        self.area = None
-
-    @staticmethod
-    def intersect(rect_a: 'Rectangle', rect_b: 'Rectangle') -> bool:
-        """
-        Determine if rect_a, rect_b intersect.
-        Modified slightly from:
-        https://stackoverflow.com/questions/306316/determine-if-two-rectangles-overlap-each-other#306332
-        """
-
-        ret = (
-                rect_a.left < rect_b.right
-                and rect_a.right > rect_b.left
-                and rect_a.top < rect_b.bottom
-                and rect_a.bottom > rect_b.top
-        )
-        return ret
-
-    @staticmethod
-    def merge_rects(rects: List['Rectangle']) -> 'Rectangle':
-        """
-        Merge a list of rectangles into one conglomerate rect in Cartesian representation.
-        """
-
-        ans = Rectangle(sys.maxsize, sys.maxsize, 0, 0)
-
-        for rect in rects:
-            if rect.left < ans.left:
-                ans.left = rect.left
-            if rect.top < ans.top:
-                ans.top = rect.top
-            if rect.bottom > ans.bottom:
-                ans.bottom = rect.bottom
-            if rect.right > ans.right:
-                ans.right = rect.right
-
-        return ans
-
-    @staticmethod
-    def rect_cv_to_cartesian(rect: Tuple[int, int, int, int]) -> 'Rectangle':
-        """
-        Convert a rectangle from CV representation to cartesian coordinates.
-        """
-        new_rect = Rectangle(rect[0], rect[1], rect[0] + rect[2], rect[1] + rect[3])
-        return new_rect
-
-    @staticmethod
-    def rect_cartesian_to_cv(rect: 'Rectangle') -> tuple:
-        """
-        Convert rectangle from Cartesian representation back to CV tuple representation
-        """
-        new_rect = (rect.top, rect.left, rect.bottom - rect.top, rect.right - rect.left)
-        return new_rect
-
-    def __eq__(self, other: 'Rectangle') -> bool:
-        if isinstance(other, Rectangle):
-            return (
-                    self.top == other.top
-                    and self.left == other.left
-                    and self.right == other.right
-                    and self.bottom == other.bottom
-            )
-        return False
-
-    def __lt__(self, other: 'Rectangle') -> bool:
-        # todo: Ideate a more absolute definition of "less than"
-        if self.get_area() > other.get_area():
-            return True
-        return False
-
-    def get_area(self) -> int:
-        """
-        Return the area taken up by this rectangle.
-        """
-        if self.area is None:
-            self.area = (self.right - self.left) * (self.bottom - self.top)
-        return self.area
-
-    def contains_point(self, point: Tuple[int, int]) -> bool:
-        """
-        Given a Tuple representing a point, return whether the point is within this rectangle.
-        """
-        if self.distance_to_point(point) == 0.0:
-            return True
-        return False
-
-    def distance_to_point(self, point: tuple) -> float:
-        """
-        Determine the distance from a rectangle to a point. If the point is within a rectangle, zero will be returned.
-        https://stackoverflow.com/questions/5254838/calculating-distance-between-a-point-and-a-rectangular-box-nearest-point
-        """
-        dx = max(self.left - point[0], 0, point[0] - self.right)
-        dy = max(self.top - point[1], 0, point[1] - self.bottom)
-
-        if dx == 0 and dy == 0:
-            return 0.0
-
-        # potentially problematic due to using floats
-        return math.sqrt(dx ** 2 + dy ** 2)
-
-    def __str__(self):
-        return "({1},{0}), ({3},{2})".format(self.top, self.left, self.bottom, self.right)
+import math
+import sys
+
+from typing import List, Tuple
+
+
+class Rectangle:
+    """
+    Representation of a rectangle in two dimensional space.
+
+    Note: Keep in mind that due to OpenCV's representation of the screen, y increases from top to bottom!
+                            0 - x +
+                            |
+                            y
+                            +
+    Where top, bottom, left and right are named relative to cartesian coordinates. The below
+    diagram shows what this entails.
+                           Top
+                        --------
+                        |      |
+                   Left |      | Right
+                        |      |
+                        --------
+                         Bottom
+    """
+
+    def __init__(self, top: int, left: int, bottom: int, right: int):
+        """
+        Create a rectangle in Cartesian notation
+        """
+
+        self.top = top
+        self.left = left
+        self.bottom = bottom
+        self.right = right
+
+        # stored for cached initialization
+        self.area = None
+
+    @staticmethod
+    def intersect(rect_a: 'Rectangle', rect_b: 'Rectangle') -> bool:
+        """
+        Determine if rect_a, rect_b intersect.
+        Modified slightly from:
+        https://stackoverflow.com/questions/306316/determine-if-two-rectangles-overlap-each-other#306332
+        """
+
+        ret = (
+                rect_a.left < rect_b.right
+                and rect_a.right > rect_b.left
+                and rect_a.top < rect_b.bottom
+                and rect_a.bottom > rect_b.top
+        )
+        return ret
+
+    @staticmethod
+    def merge_rects(rects: List['Rectangle']) -> 'Rectangle':
+        """
+        Merge a list of rectangles into one conglomerate rect in Cartesian representation.
+        """
+
+        ans = Rectangle(sys.maxsize, sys.maxsize, 0, 0)
+
+        for rect in rects:
+            if rect.left < ans.left:
+                ans.left = rect.left
+            if rect.top < ans.top:
+                ans.top = rect.top
+            if rect.bottom > ans.bottom:
+                ans.bottom = rect.bottom
+            if rect.right > ans.right:
+                ans.right = rect.right
+
+        return ans
+
+    @staticmethod
+    def rect_cv_to_cartesian(rect: Tuple[int, int, int, int]) -> 'Rectangle':
+        """
+        Convert a rectangle from CV representation to cartesian coordinates.
+        """
+        new_rect = Rectangle(rect[0], rect[1], rect[0] + rect[2], rect[1] + rect[3])
+        return new_rect
+
+    @staticmethod
+    def rect_cartesian_to_cv(rect: 'Rectangle') -> tuple:
+        """
+        Convert rectangle from Cartesian representation back to CV tuple representation
+        """
+        new_rect = (rect.top, rect.left, rect.bottom - rect.top, rect.right - rect.left)
+        return new_rect
+
+    def __eq__(self, other: 'Rectangle') -> bool:
+        if isinstance(other, Rectangle):
+            return (
+                    self.top == other.top
+                    and self.left == other.left
+                    and self.right == other.right
+                    and self.bottom == other.bottom
+            )
+        return False
+
+    def __lt__(self, other: 'Rectangle') -> bool:
+        # todo: Ideate a more absolute definition of "less than"
+        if self.get_area() > other.get_area():
+            return True
+        return False
+
+    def get_area(self) -> int:
+        """
+        Return the area taken up by this rectangle.
+        """
+        if self.area is None:
+            self.area = (self.right - self.left) * (self.bottom - self.top)
+        return self.area
+
+    def contains_point(self, point: Tuple[int, int]) -> bool:
+        """
+        Given a Tuple representing a point, return whether the point is within this rectangle.
+        """
+        if self.distance_to_point(point) == 0.0:
+            return True
+        return False
+
+    def distance_to_point(self, point: tuple) -> float:
+        """
+        Determine the distance from a rectangle to a point. If the point is within a rectangle, zero will be returned.
+        https://stackoverflow.com/questions/5254838/calculating-distance-between-a-point-and-a-rectangular-box-nearest-point
+        """
+        dx = max(self.left - point[0], 0, point[0] - self.right)
+        dy = max(self.top - point[1], 0, point[1] - self.bottom)
+
+        if dx == 0 and dy == 0:
+            return 0.0
+
+        # potentially problematic due to using floats
+        return math.sqrt(dx ** 2 + dy ** 2)
+
+    def __str__(self):
+        return "({1},{0}), ({3},{2})".format(self.top, self.left, self.bottom, self.right)
```

### Comparing `iconmatch-0.0.1/IconMatch/weighted_quick_unionUF.py` & `iconmatch-0.0.2/IconMatch/weighted_quick_unionUF.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-class WeightedQuickUnionUF:
-    """
-    Weighted Quick Union UF is a Python conversion of the algorithm as implemented by Kevin Wayne and Robert Sedgewick
-    for their Algorithms 1 course on Coursera.
-
-    https://algs4.cs.princeton.edu/code/javadoc/edu/princeton/cs/algs4/WeightedQuickUnionUF.html
-    """
-
-    def __init__(self, n: int, entries):
-        """
-        Initializes an empty union–find data structure with n sites
-        0 through n-1. Each site is initially in its own
-        component.
-
-        Within the parent list, each entry is a tuple that contains the "parent"
-        index, as well as the object holding that specific entry (generic)
-        """
-        self._parent = [(0, None)] * n
-        self._size = [1] * n
-        self._count = n
-        for i in range(n):
-            self._parent[i] = (i, entries[i])
-
-    def count(self):
-        """
-        Returns the number of components.
-        """
-        return self._count
-
-    def find(self, p: int):
-        """
-        Returns the component identifier for the component containing site p.
-        """
-        self._validate(p)
-        while p != self._parent[p][0]:
-            # path compression (make every other node in path point to its grandparent)
-            self._parent[p] = (self._parent[self._parent[p][0]][0], self._parent[p][1])
-
-            p = self._parent[p][0]
-
-        return p
-
-    def _validate(self, p: int):
-        """
-        Validate that p is a valid index.
-        """
-        n = len(self._parent)
-        if p is None or p < 0 or p >= n:
-            raise ValueError("index {0} is not between 0 and {1}".format(p, n - 1))
-
-    def connected(self, p: int, q: int):
-        """
-        Returns true if the the two sites are in the same component.
-        """
-        return self.find(p) == self.find(q)
-        pass
-
-    def union(self, p: int, q: int):
-        """
-        Merges the component containing site p with the component containing site q.
-        """
-        root_p = self.find(p)
-        root_q = self.find(q)
-        if root_p == root_q:
-            return
-
-        # make smaller root point to larger one
-        if self._size[root_p] < self._size[root_q]:
-            self._parent[root_p] = (root_q, self._parent[root_p][1])
-            self._size[root_q] = self._size[root_q] + self._size[root_p]
-        else:
-            self._parent[root_q] = (root_p, self._parent[root_q][1])
-            self._size[root_p] = self._size[root_p] + self._size[root_q]
-
-        self._count = self._count - 1
-        pass
-
-    def get_unions(self):
-        """
-        Retrieves and returns all groups, according to their parent
-        """
-        components = {}
-        for index_element in range(len(self._parent)):
-            # get parent component
-            index_parent = self.find(index_element)
-            parent = self._parent[index_parent][1]
-            child = self._parent[index_element][1]
-
-            # add it to the mapping, or add the current component to its list
-            if index_parent not in components:
-                if index_element == index_parent:
-                    components[index_parent] = [
-                        child,
-                    ]
-                else:
-                    components[index_parent] = [
-                        parent,
-                        child,
-                    ]
-            else:
-                parent_list = components[index_parent]
-                parent_list.append(child)
-                components[index_parent] = parent_list
-
-        return components
+class WeightedQuickUnionUF:
+    """
+    Weighted Quick Union UF is a Python conversion of the algorithm as implemented by Kevin Wayne and Robert Sedgewick
+    for their Algorithms 1 course on Coursera.
+
+    https://algs4.cs.princeton.edu/code/javadoc/edu/princeton/cs/algs4/WeightedQuickUnionUF.html
+    """
+
+    def __init__(self, n: int, entries):
+        """
+        Initializes an empty union–find data structure with n sites
+        0 through n-1. Each site is initially in its own
+        component.
+
+        Within the parent list, each entry is a tuple that contains the "parent"
+        index, as well as the object holding that specific entry (generic)
+        """
+        self._parent = [(0, None)] * n
+        self._size = [1] * n
+        self._count = n
+        for i in range(n):
+            self._parent[i] = (i, entries[i])
+
+    def count(self):
+        """
+        Returns the number of components.
+        """
+        return self._count
+
+    def find(self, p: int):
+        """
+        Returns the component identifier for the component containing site p.
+        """
+        self._validate(p)
+        while p != self._parent[p][0]:
+            # path compression (make every other node in path point to its grandparent)
+            self._parent[p] = (self._parent[self._parent[p][0]][0], self._parent[p][1])
+
+            p = self._parent[p][0]
+
+        return p
+
+    def _validate(self, p: int):
+        """
+        Validate that p is a valid index.
+        """
+        n = len(self._parent)
+        if p is None or p < 0 or p >= n:
+            raise ValueError("index {0} is not between 0 and {1}".format(p, n - 1))
+
+    def connected(self, p: int, q: int):
+        """
+        Returns true if the the two sites are in the same component.
+        """
+        return self.find(p) == self.find(q)
+        pass
+
+    def union(self, p: int, q: int):
+        """
+        Merges the component containing site p with the component containing site q.
+        """
+        root_p = self.find(p)
+        root_q = self.find(q)
+        if root_p == root_q:
+            return
+
+        # make smaller root point to larger one
+        if self._size[root_p] < self._size[root_q]:
+            self._parent[root_p] = (root_q, self._parent[root_p][1])
+            self._size[root_q] = self._size[root_q] + self._size[root_p]
+        else:
+            self._parent[root_q] = (root_p, self._parent[root_q][1])
+            self._size[root_p] = self._size[root_p] + self._size[root_q]
+
+        self._count = self._count - 1
+        pass
+
+    def get_unions(self):
+        """
+        Retrieves and returns all groups, according to their parent
+        """
+        components = {}
+        for index_element in range(len(self._parent)):
+            # get parent component
+            index_parent = self.find(index_element)
+            parent = self._parent[index_parent][1]
+            child = self._parent[index_element][1]
+
+            # add it to the mapping, or add the current component to its list
+            if index_parent not in components:
+                if index_element == index_parent:
+                    components[index_parent] = [
+                        child,
+                    ]
+                else:
+                    components[index_parent] = [
+                        parent,
+                        child,
+                    ]
+            else:
+                parent_list = components[index_parent]
+                parent_list.append(child)
+                components[index_parent] = parent_list
+
+        return components
```

### Comparing `iconmatch-0.0.1/README.md` & `iconmatch-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,141 @@
-<h1 align="center">
-	IconMatch
-</h1>
-
-<p align="center">
-	<i>Easily select icons on the screen in any environment.</i>
-</p>
-
-<p align="center">
-  <a href="https://luiszugasti.me">
-    <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/screenshot.png" alt="Showcasing bounding boxes and original image"/>
-  </a>
-  <a href="https://luiszugasti.me">
-    <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/nearest_box.gif" alt="Showcasing candidate boxes functionality"/>
-  </a>
-  <a href="https://luiszugasti.me">
-    <img src="https://github.com/NativeSensors/IconMatch/assets/40773550/ebc5aa2e-50b3-464a-a033-7c54b7615eeb" alt="Showcasing realtime demo"/>
-  </a>
-</p>
-
-  
-This is part of the Hands Free Computing project. Built with [OpenCV 3.12](https://opencv.org) and [Python 3.8](https://python.org).
-
-## Table of Contents
-
-
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [API](#api)
-  - [Roadmap](#roadmap)
-  - [Contributing](#contributing)
-  - [License](#license)
-  - [Contact](#contact)
-
-
-## Installation 
-
-1. Clone the repo and open it locally:
-```
-$ git clone https://github.com/luiszugasti/IconMatch/
-$ cd IconMatch
-```
-
-2. Install the [requirements](https://github.com/luiszugasti/IconMatch/blob/main/requirements.txt):
-```
-$ pip install -r requirements.txt
-```
-
-## Usage
-
-You can use the functions as shown in [demo.py](https://github.com/luiszugasti/IconMatch/blob/main/icondetection/demo/demo.py) as a default entry point.
-
-In the below example, the main set of functions is called within a callback function, as this allows the threshold value
-to be controlled from a GUI in OpenCV.
-
-Image Scanner:
-
-```python
-import cv2 as cv
-
-import IconMatch.IconMatch from ImageScanner
-
-src = cv.imread("source to your image file")
-scanner = ImageScanner(thersh = 100)
-
-detected_rectangles = scanner.scan(src)
-# list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
-
-```
-
-Screen Scanner:
-
-```python
-import cv2 as cv
-
-import IconMatch.IconMatch from ScreenScanner
-
-src = cv.imread("source to your image file")
-scanner = ScreenScanner(thersh = 100)
-
-detected_rectangles = scanner.scan(bbox = (x,y,w,h))
-# list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
-
-```
-
-RealTime demo:
-```bash
-python rt_demo.py
-```
-
-## Key Features
-
-- Detection of areas with a high likelihood of being clickable icons.
-- Detection of closest rectangle to point of interest (be it gaze, or mouse as in the examples)
-
-## API
-
-The current available APIs encompass what your image processing pipeline should contain. Both APIs are 
-currently still experimental as I learn more about OpenCV and optimize code.
-
-### ImageScanner
-> Performs Canny detection on passed images and group overlapping rectangles 
-
-### ScreenScanner
-> Scans your display, take screnshoots and call ImageScanners
-
-## Roadmap
-
-- [x] Detect regions of interest with moderate accuracy
-- [x] Detect candidate region based on proximity
-- [x] Detect icon-like objects on the screen
-- [?] Context provision into regions of interest
-
-
-## Contributing
-
-Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **genuinely appreciated**.
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-## Contact
-
-Original Creator: Luis Zugasti - [@luis\_\_zugasti](https://twitter.com/luis__zugasti)
-
-Current Maintainer: Piotr Walas - [@Piotr\_\_Walas](https://twitter.com/PW4ltz)
-
-Project Link: [https://github.com/NativeSensors/IconMatch](https://github.com/NativeSensors/IconMatch)
+<h1 align="center">
+	IconMatch
+</h1>
+
+<p align="center">
+	<i>Easily select icons on the screen in any environment.</i>
+</p>
+
+<p align="center">
+  <a href="">
+    <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/screenshot.png" alt="Showcasing bounding boxes and original image"/>
+  </a>
+  <a href="">
+    <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/nearest_box.gif" alt="Showcasing candidate boxes functionality"/>
+  </a>
+  <a href="">
+    <img src="https://github.com/NativeSensors/IconMatch/assets/40773550/ebc5aa2e-50b3-464a-a033-7c54b7615eeb" alt="Showcasing realtime demo"/>
+  </a>
+</p>
+
+
+This is part of the Hands Free Computing project. Built with [OpenCV 3.12](https://opencv.org) and [Python 3.8](https://python.org).
+
+### 💜 Sponsors: 
+
+```
+Sponsor us and we can add your link, banner or other promo materials!
+```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+<!-- POLAR-END id=eizdelwu -->
+
+### 💜 Follow NativeSensors: 
+
+<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+
+## Table of Contents
+
+
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [API](#api)
+  - [Roadmap](#roadmap)
+  - [Contributing](#contributing)
+  - [License](#license)
+  - [Contact](#contact)
+
+
+## Installation 
+
+1. Install from PyPI:
+```
+$ pip install iconmatch
+```
+
+## Usage
+
+You can use the functions as shown in [demo.py](https://github.com/luiszugasti/IconMatch/blob/main/icondetection/demo/demo.py) as a default entry point.
+
+In the below example, the main set of functions is called within a callback function, as this allows the threshold value
+to be controlled from a GUI in OpenCV.
+
+Image Scanner:
+
+```python
+import cv2 as cv
+
+import IconMatch.IconMatch from ImageScanner
+
+src = cv.imread("source to your image file")
+scanner = ImageScanner(thersh = 100)
+
+detected_rectangles = scanner.scan(src)
+# list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
+
+```
+
+Screen Scanner:
+
+```python
+import IconMatch.IconMatch from ScreenScanner
+
+scanner = ScreenScanner(thersh = 100)
+
+detected_rectangles = scanner.scan(bbox = (x,y,w,h))
+# list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
+
+```
+
+RealTime demo:
+```bash
+python rt_demo.py
+```
+
+## Key Features
+
+- Detection of areas with a high likelihood of being clickable icons.
+- Detection of closest rectangle to point of interest (be it gaze, or mouse as in the examples)
+
+## API
+
+The current available APIs encompass what your image processing pipeline should contain. Both APIs are 
+currently still experimental as I learn more about OpenCV and optimize code.
+
+### ImageScanner
+> Performs Canny detection on passed images and group overlapping rectangles 
+
+### ScreenScanner
+> Scans your display, take screnshoots and call ImageScanners
+
+## Roadmap
+
+- [x] Detect regions of interest with moderate accuracy
+- [x] Detect candidate region based on proximity
+- [x] Detect icon-like objects on the screen
+- [?] Context provision into regions of interest
+
+
+## Contributing
+
+Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **genuinely appreciated**.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Original Creator: Luis Zugasti - [@luis\_\_zugasti](https://twitter.com/luis__zugasti)
+Original Creator blog: [https://luiszugasti.me](https://luiszugasti.me)
+
+Current Maintainer: Piotr Walas - [@Piotr\_\_Walas](https://twitter.com/PW4ltz)
+
+Project Link: [https://github.com/NativeSensors/IconMatch](https://github.com/NativeSensors/IconMatch)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iconmatch-0.0.1/PKG-INFO` & `iconmatch-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: IconMatch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for detecting Icons from images or screen
 Project-URL: Homepage, https://github.com/NativeSensors/IconMatch
 Project-URL: Issues, https://github.com/NativeSensors/IconMatch/Issues
 Author-email: Piotr Walas <piotr.walas@eyegestures.com>
 Maintainer-email: Piotr Walas <piotr.walas@eyegestures.com>
 License: MIT License
         
@@ -40,51 +40,59 @@
 </h1>
 
 <p align="center">
 	<i>Easily select icons on the screen in any environment.</i>
 </p>
 
 <p align="center">
-  <a href="https://luiszugasti.me">
+  <a href="">
     <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/screenshot.png" alt="Showcasing bounding boxes and original image"/>
   </a>
-  <a href="https://luiszugasti.me">
+  <a href="">
     <img src="https://raw.githubusercontent.com/luiszugasti/IconMatch/main/images/nearest_box.gif" alt="Showcasing candidate boxes functionality"/>
   </a>
-  <a href="https://luiszugasti.me">
+  <a href="">
     <img src="https://github.com/NativeSensors/IconMatch/assets/40773550/ebc5aa2e-50b3-464a-a033-7c54b7615eeb" alt="Showcasing realtime demo"/>
   </a>
 </p>
 
-  
+
 This is part of the Hands Free Computing project. Built with [OpenCV 3.12](https://opencv.org) and [Python 3.8](https://python.org).
 
+### 💜 Sponsors: 
+
+```
+Sponsor us and we can add your link, banner or other promo materials!
+```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+<!-- POLAR-END id=eizdelwu -->
+
+### 💜 Follow NativeSensors: 
+
+<a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
+
 ## Table of Contents
 
 
   - [Installation](#installation)
   - [Usage](#usage)
   - [API](#api)
   - [Roadmap](#roadmap)
   - [Contributing](#contributing)
   - [License](#license)
   - [Contact](#contact)
 
 
 ## Installation 
 
-1. Clone the repo and open it locally:
-```
-$ git clone https://github.com/luiszugasti/IconMatch/
-$ cd IconMatch
-```
-
-2. Install the [requirements](https://github.com/luiszugasti/IconMatch/blob/main/requirements.txt):
+1. Install from PyPI:
 ```
-$ pip install -r requirements.txt
+$ pip install iconmatch
 ```
 
 ## Usage
 
 You can use the functions as shown in [demo.py](https://github.com/luiszugasti/IconMatch/blob/main/icondetection/demo/demo.py) as a default entry point.
 
 In the below example, the main set of functions is called within a callback function, as this allows the threshold value
@@ -104,19 +112,16 @@
 # list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
 
 ```
 
 Screen Scanner:
 
 ```python
-import cv2 as cv
-
 import IconMatch.IconMatch from ScreenScanner
 
-src = cv.imread("source to your image file")
 scanner = ScreenScanner(thersh = 100)
 
 detected_rectangles = scanner.scan(bbox = (x,y,w,h))
 # list of [(x,y,w,h),(x,y,w,h), ... , (x,y,w,h)]
 
 ```
 
@@ -162,11 +167,12 @@
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 ## Contact
 
 Original Creator: Luis Zugasti - [@luis\_\_zugasti](https://twitter.com/luis__zugasti)
+Original Creator blog: [https://luiszugasti.me](https://luiszugasti.me)
 
 Current Maintainer: Piotr Walas - [@Piotr\_\_Walas](https://twitter.com/PW4ltz)
 
 Project Link: [https://github.com/NativeSensors/IconMatch](https://github.com/NativeSensors/IconMatch)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

