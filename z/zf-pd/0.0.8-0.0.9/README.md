# Comparing `tmp/zf-pd-0.0.8.tar.gz` & `tmp/zf-pd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zf-pd-0.0.8.tar", last modified: Mon Dec 25 00:11:39 2023, max compression
+gzip compressed data, was "zf-pd-0.0.9.tar", last modified: Mon Dec 25 03:36:01 2023, max compression
```

## Comparing `zf-pd-0.0.8.tar` & `zf-pd-0.0.9.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.785466 zf-pd-0.0.8/
--rw-r--r--   0 muqsit     (501) staff       (20)     1065 2023-12-24 23:56:56.000000 zf-pd-0.0.8/LICENSE
--rw-r--r--   0 muqsit     (501) staff       (20)      434 2023-12-24 23:56:56.000000 zf-pd-0.0.8/MANIFEST.in
--rw-r--r--   0 muqsit     (501) staff       (20)     7527 2023-12-25 00:11:39.785266 zf-pd-0.0.8/PKG-INFO
--rw-------   0 muqsit     (501) staff       (20)     7154 2023-12-24 23:49:21.000000 zf-pd-0.0.8/README.md
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.775858 zf-pd-0.0.8/pd/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)      832 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/__main__.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.776066 zf-pd-0.0.8/pd/config/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/config/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)    11114 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/config/config.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.776211 zf-pd-0.0.8/pd/config/templates/
--rw-r--r--   0 muqsit     (501) staff       (20)      357 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/config/templates/zshrc.j2
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.777097 zf-pd-0.0.8/pd/conv/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/conv/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)     3746 2023-12-24 23:49:01.000000 zf-pd-0.0.8/pd/conv/conv.py
--rw-r--r--   0 muqsit     (501) staff       (20)      621 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/conv/m4a.py
--rw-r--r--   0 muqsit     (501) staff       (20)      776 2023-12-24 23:47:59.000000 zf-pd-0.0.8/pd/conv/mov.py
--rw-r--r--   0 muqsit     (501) staff       (20)      592 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/conv/mp3.py
--rw-r--r--   0 muqsit     (501) staff       (20)      452 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/conv/mp4.py
--rw-r--r--   0 muqsit     (501) staff       (20)      795 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/conv/png.py
--rw-r--r--   0 muqsit     (501) staff       (20)      781 2023-12-25 00:00:28.000000 zf-pd-0.0.8/pd/conv/webm.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.777308 zf-pd-0.0.8/pd/ec2/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/ec2/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)     7655 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/ec2/ec2.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.777551 zf-pd-0.0.8/pd/env/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/env/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)     1109 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/env/env.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.777724 zf-pd-0.0.8/pd/init/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)     4209 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/init.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.777896 zf-pd-0.0.8/pd/init/templates/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/__init__.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.778596 zf-pd-0.0.8/pd/init/templates/pd-fastapi/
--rw-r--r--   0 muqsit     (501) staff       (20)       51 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/.gitignore
--rw-r--r--   0 muqsit     (501) staff       (20)     1387 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/README.md
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/__init__.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.778693 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.778899 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/apis/
--rw-r--r--   0 muqsit     (501) staff       (20)       25 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/apis/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)      125 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/apis/api.py
--rw-r--r--   0 muqsit     (501) staff       (20)      714 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/main.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.779113 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/model/
--rw-r--r--   0 muqsit     (501) staff       (20)       27 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/model/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)       72 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/model/model.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.779318 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/routers/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/routers/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)      633 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/routers/home.py
--rw-r--r--   0 muqsit     (501) staff       (20)      635 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/package-lock.json
--rw-r--r--   0 muqsit     (501) staff       (20)      178 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/package.json
--rw-r--r--   0 muqsit     (501) staff       (20)      252 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/requirements.txt
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.779998 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780095 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/css/
--rwxr-xr-x   0 muqsit     (501) staff       (20)      461 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/css/index.css
--rw-r--r--   0 muqsit     (501) staff       (20)    15406 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/favicon.ico
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780197 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/fonts/
--rw-r--r--   0 muqsit     (501) staff       (20)    77280 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/fonts/Rosario-Regular.ttf
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780353 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/img/
--rw-r--r--   0 muqsit     (501) staff       (20)    79233 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/img/pd.png
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780508 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/js/
--rw-r--r--   0 muqsit     (501) staff       (20)       62 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/js/index.js
--rw-r--r--   0 muqsit     (501) staff       (20)    13742 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/logo192.png
--rw-r--r--   0 muqsit     (501) staff       (20)    34750 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/logo512.png
--rw-r--r--   0 muqsit     (501) staff       (20)      498 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/manifest.json
--rw-r--r--   0 muqsit     (501) staff       (20)       66 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/robots.txt
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780612 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/ts/
--rw-r--r--   0 muqsit     (501) staff       (20)       47 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/ts/index.ts
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.780908 zf-pd-0.0.8/pd/init/templates/pd-fastapi/templates/
--rw-r--r--   0 muqsit     (501) staff       (20)      558 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/templates/head.html
--rw-r--r--   0 muqsit     (501) staff       (20)      337 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/templates/index.html
--rw-r--r--   0 muqsit     (501) staff       (20)       79 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/templates/logo.html
--rw-r--r--   0 muqsit     (501) staff       (20)      266 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-fastapi/tsconfig.json
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.781805 zf-pd-0.0.8/pd/init/templates/pd-react/
--rw-r--r--   0 muqsit     (501) staff       (20)      310 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/.gitignore
--rw-r--r--   0 muqsit     (501) staff       (20)     1016 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/README.md
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)   762015 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/package-lock.json
--rw-r--r--   0 muqsit     (501) staff       (20)     1038 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/package.json
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.782513 zf-pd-0.0.8/pd/init/templates/pd-react/public/
--rw-r--r--   0 muqsit     (501) staff       (20)    15406 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/favicon.ico
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.782611 zf-pd-0.0.8/pd/init/templates/pd-react/public/fonts/
--rw-r--r--   0 muqsit     (501) staff       (20)    77280 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/fonts/Rosario-Regular.ttf
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.782765 zf-pd-0.0.8/pd/init/templates/pd-react/public/img/
--rw-r--r--   0 muqsit     (501) staff       (20)    79233 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/img/pd.png
--rw-r--r--   0 muqsit     (501) staff       (20)      680 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/index.html
--rw-r--r--   0 muqsit     (501) staff       (20)    13742 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/logo192.png
--rw-r--r--   0 muqsit     (501) staff       (20)    34750 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/logo512.png
--rw-r--r--   0 muqsit     (501) staff       (20)      494 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/manifest.json
--rw-r--r--   0 muqsit     (501) staff       (20)       67 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/public/robots.txt
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.783294 zf-pd-0.0.8/pd/init/templates/pd-react/src/
--rw-r--r--   0 muqsit     (501) staff       (20)      391 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/App.tsx
--rw-r--r--   0 muqsit     (501) staff       (20)      399 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/Error.tsx
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.783396 zf-pd-0.0.8/pd/init/templates/pd-react/src/apis/
--rw-r--r--   0 muqsit     (501) staff       (20)       63 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/apis/api.tsx
--rw-r--r--   0 muqsit     (501) staff       (20)      595 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/index.css
--rw-r--r--   0 muqsit     (501) staff       (20)      731 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/index.tsx
--rw-r--r--   0 muqsit     (501) staff       (20)      425 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/reportWebVitals.ts
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.783500 zf-pd-0.0.8/pd/init/templates/pd-react/src/routes/
--rw-r--r--   0 muqsit     (501) staff       (20)      814 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/src/routes/Home.tsx
--rw-r--r--   0 muqsit     (501) staff       (20)      535 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/init/templates/pd-react/tsconfig.json
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.783690 zf-pd-0.0.8/pd/model/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/model/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)      565 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/model/model.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.783891 zf-pd-0.0.8/pd/nginx/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/nginx/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)     1889 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/nginx/nginx.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.784178 zf-pd-0.0.8/pd/nginx/templates/
--rw-r--r--   0 muqsit     (501) staff       (20)      326 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/nginx/templates/example.com
--rw-r--r--   0 muqsit     (501) staff       (20)      326 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/nginx/templates/simple.com
--rw-r--r--   0 muqsit     (501) staff       (20)      613 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/nginx/templates/static.com
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.784374 zf-pd-0.0.8/pd/sync/
--rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/sync/__init__.py
--rw-r--r--   0 muqsit     (501) staff       (20)      309 2023-12-24 23:56:56.000000 zf-pd-0.0.8/pd/sync/sync.py
--rw-r--r--   0 muqsit     (501) staff       (20)       22 2023-12-25 00:10:20.000000 zf-pd-0.0.8/pd/version.py
--rw-r--r--   0 muqsit     (501) staff       (20)       38 2023-12-25 00:11:39.785505 zf-pd-0.0.8/setup.cfg
--rw-r--r--   0 muqsit     (501) staff       (20)     1603 2023-12-24 23:56:56.000000 zf-pd-0.0.8/setup.py
-drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 00:11:39.784998 zf-pd-0.0.8/zf_pd.egg-info/
--rw-r--r--   0 muqsit     (501) staff       (20)     7527 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/PKG-INFO
--rw-r--r--   0 muqsit     (501) staff       (20)     2996 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/SOURCES.txt
--rw-r--r--   0 muqsit     (501) staff       (20)        1 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/dependency_links.txt
--rw-r--r--   0 muqsit     (501) staff       (20)       40 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/entry_points.txt
--rw-r--r--   0 muqsit     (501) staff       (20)       54 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/requires.txt
--rw-r--r--   0 muqsit     (501) staff       (20)        3 2023-12-25 00:11:39.000000 zf-pd-0.0.8/zf_pd.egg-info/top_level.txt
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.257576 zf-pd-0.0.9/
+-rw-r--r--   0 muqsit     (501) staff       (20)     1065 2023-12-24 23:56:56.000000 zf-pd-0.0.9/LICENSE
+-rw-r--r--   0 muqsit     (501) staff       (20)      434 2023-12-24 23:56:56.000000 zf-pd-0.0.9/MANIFEST.in
+-rw-r--r--   0 muqsit     (501) staff       (20)     7560 2023-12-25 03:36:01.257370 zf-pd-0.0.9/PKG-INFO
+-rw-------   0 muqsit     (501) staff       (20)     7187 2023-12-25 03:35:22.000000 zf-pd-0.0.9/README.md
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.218889 zf-pd-0.0.9/pd/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      832 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/__main__.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.219098 zf-pd-0.0.9/pd/config/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/config/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)    11114 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/config/config.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.219368 zf-pd-0.0.9/pd/config/templates/
+-rw-r--r--   0 muqsit     (501) staff       (20)      357 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/config/templates/zshrc.j2
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.220883 zf-pd-0.0.9/pd/conv/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/conv/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)     3835 2023-12-25 03:35:06.000000 zf-pd-0.0.9/pd/conv/conv.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      621 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/conv/m4a.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      776 2023-12-24 23:47:59.000000 zf-pd-0.0.9/pd/conv/mov.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      592 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/conv/mp3.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      452 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/conv/mp4.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      795 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/conv/png.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      781 2023-12-25 00:00:28.000000 zf-pd-0.0.9/pd/conv/webm.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.221275 zf-pd-0.0.9/pd/ec2/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/ec2/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)     7655 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/ec2/ec2.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.221588 zf-pd-0.0.9/pd/env/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/env/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)     1109 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/env/env.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.222122 zf-pd-0.0.9/pd/init/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)     4209 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/init.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.222324 zf-pd-0.0.9/pd/init/templates/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/__init__.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.226408 zf-pd-0.0.9/pd/init/templates/pd-fastapi/
+-rw-r--r--   0 muqsit     (501) staff       (20)       51 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/.gitignore
+-rw-r--r--   0 muqsit     (501) staff       (20)     1387 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/README.md
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/__init__.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.226616 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.227199 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/apis/
+-rw-r--r--   0 muqsit     (501) staff       (20)       25 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/apis/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      125 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/apis/api.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      714 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/main.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.227575 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/model/
+-rw-r--r--   0 muqsit     (501) staff       (20)       27 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/model/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)       72 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/model/model.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.227873 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/routers/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/routers/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      633 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/routers/home.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      635 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/package-lock.json
+-rw-r--r--   0 muqsit     (501) staff       (20)      178 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/package.json
+-rw-r--r--   0 muqsit     (501) staff       (20)      252 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/requirements.txt
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.233719 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.233850 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/css/
+-rwxr-xr-x   0 muqsit     (501) staff       (20)      461 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/css/index.css
+-rw-r--r--   0 muqsit     (501) staff       (20)    15406 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/favicon.ico
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.233980 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/fonts/
+-rw-r--r--   0 muqsit     (501) staff       (20)    77280 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/fonts/Rosario-Regular.ttf
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.235838 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/img/
+-rw-r--r--   0 muqsit     (501) staff       (20)    79233 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/img/pd.png
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.237873 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/js/
+-rw-r--r--   0 muqsit     (501) staff       (20)       62 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/js/index.js
+-rw-r--r--   0 muqsit     (501) staff       (20)    13742 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/logo192.png
+-rw-r--r--   0 muqsit     (501) staff       (20)    34750 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/logo512.png
+-rw-r--r--   0 muqsit     (501) staff       (20)      498 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/manifest.json
+-rw-r--r--   0 muqsit     (501) staff       (20)       66 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/robots.txt
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.238056 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/ts/
+-rw-r--r--   0 muqsit     (501) staff       (20)       47 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/ts/index.ts
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.238682 zf-pd-0.0.9/pd/init/templates/pd-fastapi/templates/
+-rw-r--r--   0 muqsit     (501) staff       (20)      558 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/templates/head.html
+-rw-r--r--   0 muqsit     (501) staff       (20)      337 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/templates/index.html
+-rw-r--r--   0 muqsit     (501) staff       (20)       79 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/templates/logo.html
+-rw-r--r--   0 muqsit     (501) staff       (20)      266 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-fastapi/tsconfig.json
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.243409 zf-pd-0.0.9/pd/init/templates/pd-react/
+-rw-r--r--   0 muqsit     (501) staff       (20)      310 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/.gitignore
+-rw-r--r--   0 muqsit     (501) staff       (20)     1016 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/README.md
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)   762015 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/package-lock.json
+-rw-r--r--   0 muqsit     (501) staff       (20)     1038 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/package.json
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.247754 zf-pd-0.0.9/pd/init/templates/pd-react/public/
+-rw-r--r--   0 muqsit     (501) staff       (20)    15406 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/favicon.ico
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.247930 zf-pd-0.0.9/pd/init/templates/pd-react/public/fonts/
+-rw-r--r--   0 muqsit     (501) staff       (20)    77280 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/fonts/Rosario-Regular.ttf
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.248181 zf-pd-0.0.9/pd/init/templates/pd-react/public/img/
+-rw-r--r--   0 muqsit     (501) staff       (20)    79233 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/img/pd.png
+-rw-r--r--   0 muqsit     (501) staff       (20)      680 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/index.html
+-rw-r--r--   0 muqsit     (501) staff       (20)    13742 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/logo192.png
+-rw-r--r--   0 muqsit     (501) staff       (20)    34750 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/logo512.png
+-rw-r--r--   0 muqsit     (501) staff       (20)      494 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/manifest.json
+-rw-r--r--   0 muqsit     (501) staff       (20)       67 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/public/robots.txt
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.253115 zf-pd-0.0.9/pd/init/templates/pd-react/src/
+-rw-r--r--   0 muqsit     (501) staff       (20)      391 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/App.tsx
+-rw-r--r--   0 muqsit     (501) staff       (20)      399 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/Error.tsx
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.253249 zf-pd-0.0.9/pd/init/templates/pd-react/src/apis/
+-rw-r--r--   0 muqsit     (501) staff       (20)       63 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/apis/api.tsx
+-rw-r--r--   0 muqsit     (501) staff       (20)      595 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/index.css
+-rw-r--r--   0 muqsit     (501) staff       (20)      731 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/index.tsx
+-rw-r--r--   0 muqsit     (501) staff       (20)      425 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/reportWebVitals.ts
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.253382 zf-pd-0.0.9/pd/init/templates/pd-react/src/routes/
+-rw-r--r--   0 muqsit     (501) staff       (20)      814 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/src/routes/Home.tsx
+-rw-r--r--   0 muqsit     (501) staff       (20)      535 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/init/templates/pd-react/tsconfig.json
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.253604 zf-pd-0.0.9/pd/model/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/model/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      565 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/model/model.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.253835 zf-pd-0.0.9/pd/nginx/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/nginx/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)     1889 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/nginx/nginx.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.256128 zf-pd-0.0.9/pd/nginx/templates/
+-rw-r--r--   0 muqsit     (501) staff       (20)      326 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/nginx/templates/example.com
+-rw-r--r--   0 muqsit     (501) staff       (20)      326 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/nginx/templates/simple.com
+-rw-r--r--   0 muqsit     (501) staff       (20)      613 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/nginx/templates/static.com
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.256361 zf-pd-0.0.9/pd/sync/
+-rw-r--r--   0 muqsit     (501) staff       (20)        0 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/sync/__init__.py
+-rw-r--r--   0 muqsit     (501) staff       (20)      309 2023-12-24 23:56:56.000000 zf-pd-0.0.9/pd/sync/sync.py
+-rw-r--r--   0 muqsit     (501) staff       (20)       22 2023-12-25 03:34:14.000000 zf-pd-0.0.9/pd/version.py
+-rw-r--r--   0 muqsit     (501) staff       (20)       38 2023-12-25 03:36:01.257621 zf-pd-0.0.9/setup.cfg
+-rw-r--r--   0 muqsit     (501) staff       (20)     1603 2023-12-24 23:56:56.000000 zf-pd-0.0.9/setup.py
+drwxr-xr-x   0 muqsit     (501) staff       (20)        0 2023-12-25 03:36:01.257084 zf-pd-0.0.9/zf_pd.egg-info/
+-rw-r--r--   0 muqsit     (501) staff       (20)     7560 2023-12-25 03:36:00.000000 zf-pd-0.0.9/zf_pd.egg-info/PKG-INFO
+-rw-r--r--   0 muqsit     (501) staff       (20)     2996 2023-12-25 03:36:01.000000 zf-pd-0.0.9/zf_pd.egg-info/SOURCES.txt
+-rw-r--r--   0 muqsit     (501) staff       (20)        1 2023-12-25 03:36:01.000000 zf-pd-0.0.9/zf_pd.egg-info/dependency_links.txt
+-rw-r--r--   0 muqsit     (501) staff       (20)       40 2023-12-25 03:36:01.000000 zf-pd-0.0.9/zf_pd.egg-info/entry_points.txt
+-rw-r--r--   0 muqsit     (501) staff       (20)       54 2023-12-25 03:36:01.000000 zf-pd-0.0.9/zf_pd.egg-info/requires.txt
+-rw-r--r--   0 muqsit     (501) staff       (20)        3 2023-12-25 03:36:01.000000 zf-pd-0.0.9/zf_pd.egg-info/top_level.txt
```

### Comparing `zf-pd-0.0.8/LICENSE` & `zf-pd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/PKG-INFO` & `zf-pd-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zf-pd
-Version: 0.0.8
+Version: 0.0.9
 Summary: pd supercharges your development workflows
 Author: zeffmuks
 Author-email: zeffmuks@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: click
@@ -139,15 +139,16 @@
 Available conversions:
   video
     mp4,webm,mov -> mp3
   audio
     m4a -> wav, mp3
     mp3 -> wav, m4a
   image
-    jpg, jpeg, png -> mp4
+    jpg, jpeg, webp -> png
+    jpg, jpeg, webp, png -> mp4
 ```
 
 **Example**
 
 You can convert a mp4 video file into an audio file by running:
 
 ```bash
```

### Comparing `zf-pd-0.0.8/README.md` & `zf-pd-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 Available conversions:
   video
     mp4,webm,mov -> mp3
   audio
     m4a -> wav, mp3
     mp3 -> wav, m4a
   image
-    jpg, jpeg, png -> mp4
+    jpg, jpeg, webp -> png
+    jpg, jpeg, webp, png -> mp4
 ```
 
 **Example**
 
 You can convert a mp4 video file into an audio file by running:
 
 ```bash
```

### Comparing `zf-pd-0.0.8/pd/__main__.py` & `zf-pd-0.0.9/pd/__main__.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/config/config.py` & `zf-pd-0.0.9/pd/config/config.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/conv/conv.py` & `zf-pd-0.0.9/pd/conv/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     print("Available conversions:")
     print("  video")
     print("    mp4,webm,mov -> mp3")
     print("  audio")
     print("    m4a -> wav, mp3")
     print("    mp3 -> wav, m4a")
     print("  image")
-    print("    jpg, jpeg, png -> mp4")
+    print("    jpg, jpeg, webp -> png")
+    print("    jpg, jpeg, webp, png -> mp4")
     return
 
 
 @conv.command(help="Convert a video to another format")
 @option('-p', '--path', type=str, required=True, prompt=True,
         help="Path to the video file (e.g. /path/to/file)")
 @option('-f', '--format', type=str, required=True, prompt=True,
@@ -130,12 +131,14 @@
     src_path = path
 
     dst_format = format
     dst_path = f"{src_filename}.{dst_format}"
 
     if src_format != 'png':
         src_path = to_png(src_path)
+    if dst_format == 'png':
+        return
 
     logger.debug(f"Converting {src_path} to {dst_path}")
 
     png(src_path, dst_path, duration)
     return
```

### Comparing `zf-pd-0.0.8/pd/conv/m4a.py` & `zf-pd-0.0.9/pd/conv/m4a.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/conv/mov.py` & `zf-pd-0.0.9/pd/conv/mov.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/conv/mp3.py` & `zf-pd-0.0.9/pd/conv/mp3.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/conv/png.py` & `zf-pd-0.0.9/pd/conv/png.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/conv/webm.py` & `zf-pd-0.0.9/pd/conv/webm.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/ec2/ec2.py` & `zf-pd-0.0.9/pd/ec2/ec2.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/env/env.py` & `zf-pd-0.0.9/pd/env/env.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/init.py` & `zf-pd-0.0.9/pd/init/init.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/README.md` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/README.md`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/main.py` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/main.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/app/routers/home.py` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/app/routers/home.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/package-lock.json` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/package-lock.json`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/favicon.ico` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/fonts/Rosario-Regular.ttf` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/fonts/Rosario-Regular.ttf`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/img/pd.png` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/img/pd.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/logo192.png` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/logo192.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/static/logo512.png` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/static/logo512.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-fastapi/templates/head.html` & `zf-pd-0.0.9/pd/init/templates/pd-fastapi/templates/head.html`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/README.md` & `zf-pd-0.0.9/pd/init/templates/pd-react/README.md`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/package-lock.json` & `zf-pd-0.0.9/pd/init/templates/pd-react/package-lock.json`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/package.json` & `zf-pd-0.0.9/pd/init/templates/pd-react/package.json`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/favicon.ico` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/fonts/Rosario-Regular.ttf` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/fonts/Rosario-Regular.ttf`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/img/pd.png` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/img/pd.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/index.html` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/index.html`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/logo192.png` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/logo192.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/public/logo512.png` & `zf-pd-0.0.9/pd/init/templates/pd-react/public/logo512.png`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/src/index.css` & `zf-pd-0.0.9/pd/init/templates/pd-react/src/index.css`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/src/index.tsx` & `zf-pd-0.0.9/pd/init/templates/pd-react/src/index.tsx`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/src/routes/Home.tsx` & `zf-pd-0.0.9/pd/init/templates/pd-react/src/routes/Home.tsx`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/init/templates/pd-react/tsconfig.json` & `zf-pd-0.0.9/pd/init/templates/pd-react/tsconfig.json`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/model/model.py` & `zf-pd-0.0.9/pd/model/model.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/nginx/nginx.py` & `zf-pd-0.0.9/pd/nginx/nginx.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/pd/nginx/templates/static.com` & `zf-pd-0.0.9/pd/nginx/templates/static.com`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/setup.py` & `zf-pd-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `zf-pd-0.0.8/zf_pd.egg-info/PKG-INFO` & `zf-pd-0.0.9/zf_pd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zf-pd
-Version: 0.0.8
+Version: 0.0.9
 Summary: pd supercharges your development workflows
 Author: zeffmuks
 Author-email: zeffmuks@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: click
@@ -139,15 +139,16 @@
 Available conversions:
   video
     mp4,webm,mov -> mp3
   audio
     m4a -> wav, mp3
     mp3 -> wav, m4a
   image
-    jpg, jpeg, png -> mp4
+    jpg, jpeg, webp -> png
+    jpg, jpeg, webp, png -> mp4
 ```
 
 **Example**
 
 You can convert a mp4 video file into an audio file by running:
 
 ```bash
```

### Comparing `zf-pd-0.0.8/zf_pd.egg-info/SOURCES.txt` & `zf-pd-0.0.9/zf_pd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

