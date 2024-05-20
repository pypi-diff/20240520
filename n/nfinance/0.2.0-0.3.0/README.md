# Comparing `tmp/nfinance-0.2.0-py3-none-any.whl.zip` & `tmp/nfinance-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 7217 bytes, number of entries: 11
--rw-r--r--  2.0 unx      100 b- defN 24-May-16 11:17 nfinance/__init__.py
--rw-r--r--  2.0 unx     1368 b- defN 24-May-16 11:17 nfinance/nfinance.py
--rw-r--r--  2.0 unx      481 b- defN 24-May-16 11:17 nfinance/rsi.py
--rw-r--r--  2.0 unx     3123 b- defN 24-May-16 11:17 nfinance/stock_listing.py
--rw-r--r--  2.0 unx       45 b- defN 24-May-16 11:17 tests/__init__.py
--rw-r--r--  2.0 unx     2979 b- defN 24-May-16 11:17 tests/test_nfinance.py
--rw-r--r--  2.0 unx     1064 b- defN 24-May-16 11:19 nfinance-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3334 b- defN 24-May-16 11:19 nfinance-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 11:19 nfinance-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-16 11:19 nfinance-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      848 b- defN 24-May-16 11:19 nfinance-0.2.0.dist-info/RECORD
-11 files, 13449 bytes uncompressed, 5793 bytes compressed:  56.9%
+Zip file size: 8878 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      284 b- defN 24-May-20 05:30 nfinance/__init__.py
+-rw-r--r--  2.0 unx     1368 b- defN 24-May-20 05:29 nfinance/nfinance.py
+-rw-r--r--  2.0 unx      481 b- defN 24-May-20 05:30 nfinance/rsi.py
+-rw-r--r--  2.0 unx     1727 b- defN 24-May-20 05:39 nfinance/stock_data.py
+-rw-r--r--  2.0 unx     3123 b- defN 24-May-20 05:30 nfinance/stock_listing.py
+-rw-r--r--  2.0 unx       45 b- defN 24-May-20 05:30 tests/__init__.py
+-rw-r--r--  2.0 unx     2979 b- defN 24-May-20 05:29 tests/test_nfinance.py
+-rw-r--r--  2.0 unx     1485 b- defN 24-May-20 05:39 tests/test_stock_data.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-20 05:41 nfinance-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3239 b- defN 24-May-20 05:41 nfinance-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 05:41 nfinance-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-20 05:41 nfinance-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1008 b- defN 24-May-20 05:41 nfinance-0.3.0.dist-info/RECORD
+13 files, 16910 bytes uncompressed, 7210 bytes compressed:  57.4%
```

## zipnote {}

```diff
@@ -3,32 +3,38 @@
 
 Filename: nfinance/nfinance.py
 Comment: 
 
 Filename: nfinance/rsi.py
 Comment: 
 
+Filename: nfinance/stock_data.py
+Comment: 
+
 Filename: nfinance/stock_listing.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_nfinance.py
 Comment: 
 
-Filename: nfinance-0.2.0.dist-info/LICENSE
+Filename: tests/test_stock_data.py
+Comment: 
+
+Filename: nfinance-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: nfinance-0.2.0.dist-info/METADATA
+Filename: nfinance-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: nfinance-0.2.0.dist-info/WHEEL
+Filename: nfinance-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: nfinance-0.2.0.dist-info/top_level.txt
+Filename: nfinance-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nfinance-0.2.0.dist-info/RECORD
+Filename: nfinance-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nfinance/__init__.py

```diff
@@ -1,3 +1,7 @@
-from .nfinance import nfinance
 from .rsi import compute_rsi
 from .stock_listing import StockListing
+from .stock_data import StockDataDownloader
+
+def download(ticker, start_date, end_date, interval='day'):
+    downloader = StockDataDownloader(ticker, start_date, end_date, interval)
+    return downloader.download()
```

## Comparing `nfinance-0.2.0.dist-info/LICENSE` & `nfinance-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nfinance-0.2.0.dist-info/METADATA` & `nfinance-0.3.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,59 +23,62 @@
 
 # nfinance
 ```
 nfinance/
 │
 ├── nfinance/
 │   ├── __init__.py
-│   └── nfinance.py
+│   └── stock_data.py
 │   └── stock_listing.py
 │   └── rsi.py
 │
 ├── tests/
 │   ├── __init__.py
-│   └── test_nfinance.py
+│   └── test_stock_data.py
 │
 ├── .gitignore
 ├── LICENSE
 ├── README.md
 ├── requirements.txt
 └── setup.py
 ```
 
 ## 1. 설명
-`nfinance`는 네이버 파이낸스의 데이터를 가져오는 Python 라이브러리입니다.
-`rsi`는 Relative Strength Index를 구하는 Python 라이브러리입니다.
+`stock_data.py`는 네이버 파이낸스의 데이터를 가져오는 Python 라이브러리입니다.
+`stock_listing.py`는 네이버 파이낸스의 종목 list를 가져오는 Python 라이브러리입니다.
+`rsi.py`는 Relative Strength Index를 구하는 Python 라이브러리입니다.
 
 ## 2. 설치 방법
 pip install nfinance
 
 ## 3-1. 사용 예제
 ```python
-from nfinance import nfinance
+import nfinance as nf
 
-# Correctly calling a class method
-data_day = nfinance.download(ticker="005930", start_date="2022-01-01", end_date="2022-1-31", interval="day")
-data_week = nfinance.download(ticker="005930", start_date="2022-01-01", end_date="2022-3-31", interval="week")
-data_month = nfinance.download(ticker="005930", start_date="2022-01-01", end_date="2022-12-31", interval="month")
-print(data_day)
-print(data_week)
-print(data_month)
+ticker = '005930'  # Samsung Electronics Co., Ltd
+start_date = '2023-01-01'
+end_date = '2023-05-01'
+
+try:
+    data = nf.download(ticker, start_date, end_date)
+    print(data.head())
+except Exception as e:
+    print(e)
 ```
 ## 3-2. 사용 예제
 ```python
-import nfinance
+import nfinance as nf
 
 # 코스피 전체 주식 목록 가져오기
-stocks_kospi = nfinance.StockListing('KOSPI')
+stocks_kospi = nf.StockListing('KOSPI')
 df_kospi = stocks_kospi.fetch_stocks()
 print(df_kospi)
 
 # 코스닥 전체 주식 목록 가져오기
-stocks_kosdaq = nfinance.StockListing('KOSDAQ')
+stocks_kosdaq = nf.StockListing('KOSDAQ')
 df_kosdaq = stocks_kosdaq.fetch_stocks()
 print(df_kosdaq)
 
 ```
 
 ## 4. LICENSE
```

## Comparing `nfinance-0.2.0.dist-info/RECORD` & `nfinance-0.3.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-nfinance/__init__.py,sha256=jk5_co-EtpzRvYjsPW3Dm-dn6PvH8AoLcolkVb3fA8g,100
+nfinance/__init__.py,sha256=xVmEAx0JxMpvrM3h49GKGkKjtEEMktZ6hj7e8Wsznv4,284
 nfinance/nfinance.py,sha256=OuzdeujEjuHSeAmmyD-gaIOCl4dve1mTpjVMYWHla0Y,1368
 nfinance/rsi.py,sha256=aNaV5DNpCdEiZeY2-RnIwTOIf7wt1G8Kafz9aMr9JdY,481
+nfinance/stock_data.py,sha256=gQ9MSVZ_QMqbQslkE-vCplw_CH2-U1skKJDr8TAq_TE,1727
 nfinance/stock_listing.py,sha256=UCnjRdCzT3KytWBukgIon0rQjZkN3InuYNqtcOKS28E,3123
 tests/__init__.py,sha256=PG_aDJEGJwy2Ls4tNVDssNXIARlEqzKc4hB7FAEE31g,45
 tests/test_nfinance.py,sha256=d7-dD3BRqqhv-r9Cd1qykhhhiZryp0DCqLWyIG1pKR0,2979
-nfinance-0.2.0.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
-nfinance-0.2.0.dist-info/METADATA,sha256=l8jLuMyV1gyujXBPWEGtlT0UUGuN0q_Wjh2gSp3cY0I,3334
-nfinance-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nfinance-0.2.0.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
-nfinance-0.2.0.dist-info/RECORD,,
+tests/test_stock_data.py,sha256=nobDuOLwlap9sPzyyIFKb05um2mbVrYOAlzeRqjO-jE,1485
+nfinance-0.3.0.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
+nfinance-0.3.0.dist-info/METADATA,sha256=JodzV-MCwA25RbZKckTOZh5mS09WlBa6-zkmMkfvgI4,3239
+nfinance-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nfinance-0.3.0.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
+nfinance-0.3.0.dist-info/RECORD,,
```

