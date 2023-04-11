# Comparing `tmp/starfishX-0.155555.tar.gz` & `tmp/starfishX-0.155556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfishX-0.155555.tar", last modified: Sat Mar 11 04:02:14 2023, max compression
+gzip compressed data, was "starfishX-0.155556.tar", last modified: Tue Apr 11 15:02:28 2023, max compression
```

## Comparing `starfishX-0.155555.tar` & `starfishX-0.155556.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.314380 starfishX-0.155555/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11846 2023-03-11 04:02:14.313063 starfishX-0.155555/PKG-INFO
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11466 2021-11-04 08:06:30.000000 starfishX-0.155555/README.rst
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       38 2023-03-11 04:02:14.314499 starfishX-0.155555/setup.cfg
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1245 2023-03-11 04:01:26.000000 starfishX-0.155555/setup.py
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.301617 starfishX-0.155555/starfishX/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8812 2020-02-19 23:32:22.000000 starfishX-0.155555/starfishX/AD.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4762 2019-06-07 20:21:16.000000 starfishX-0.155555/starfishX/DividendDiscountModel.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7483 2019-07-22 21:24:16.000000 starfishX-0.155555/starfishX/DuPontROE.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5675 2020-06-13 19:53:26.000000 starfishX-0.155555/starfishX/EYG.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1176 2019-10-30 20:54:04.000000 starfishX-0.155555/starfishX/Elder.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7116 2020-05-05 04:45:24.000000 starfishX-0.155555/starfishX/InterestBearingDebt.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5827 2020-06-19 23:59:20.000000 starfishX-0.155555/starfishX/Ke.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4210 2020-12-04 07:28:08.000000 starfishX-0.155555/starfishX/ShareholdersNow.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8084 2023-03-11 04:01:14.000000 starfishX-0.155555/starfishX/__init__.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5349 2020-02-19 23:56:32.000000 starfishX-0.155555/starfishX/checkServices.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       52 2019-10-23 06:36:20.000000 starfishX-0.155555/starfishX/config.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        0 2019-07-25 02:52:00.000000 starfishX-0.155555/starfishX/dashFn.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2701 2021-08-19 08:07:52.000000 starfishX-0.155555/starfishX/depreciationAndAmortisation.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5494 2021-02-04 05:51:12.000000 starfishX-0.155555/starfishX/findMarketCap.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1187 2019-10-17 04:48:50.000000 starfishX-0.155555/starfishX/findSector.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      774 2021-11-04 01:02:16.000000 starfishX-0.155555/starfishX/getDW.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     9048 2020-03-28 22:56:16.000000 starfishX-0.155555/starfishX/getEVEBITDA.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2879 2022-06-30 02:33:18.000000 starfishX-0.155555/starfishX/getFundamentalInSector.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      900 2020-05-28 01:51:26.000000 starfishX-0.155555/starfishX/getProfitAbility.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5131 2021-10-10 19:19:26.000000 starfishX-0.155555/starfishX/getWarrant.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     9375 2021-10-10 01:38:06.000000 starfishX-0.155555/starfishX/greek.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2360 2020-02-14 21:45:28.000000 starfishX-0.155555/starfishX/helpers.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2732 2020-11-20 20:44:20.000000 starfishX-0.155555/starfishX/holidayMarket.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4952 2020-03-29 21:58:48.000000 starfishX-0.155555/starfishX/incomestatement.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      235 2019-06-17 23:30:54.000000 starfishX-0.155555/starfishX/indexMarket.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2609 2020-02-19 23:35:10.000000 starfishX-0.155555/starfishX/indicator.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3333 2020-11-30 01:37:02.000000 starfishX-0.155555/starfishX/ipoStat.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2868 2019-10-14 22:14:26.000000 starfishX-0.155555/starfishX/listSecurities.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3255 2021-10-10 22:24:16.000000 starfishX-0.155555/starfishX/loadHistData_v2.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5130 2020-02-19 23:24:46.000000 starfishX-0.155555/starfishX/marketValueDaily.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7110 2020-06-17 22:38:02.000000 starfishX-0.155555/starfishX/marketview.py
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.304719 starfishX-0.155555/starfishX/markminervini/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      302 2022-10-31 01:46:52.000000 starfishX-0.155555/starfishX/markminervini/__init__.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5718 2022-10-31 01:56:59.000000 starfishX-0.155555/starfishX/markminervini/trendtemplate.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3960 2020-02-19 23:34:00.000000 starfishX-0.155555/starfishX/moc.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     6437 2020-05-28 03:37:50.000000 starfishX-0.155555/starfishX/morningstarGetfn.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4686 2022-11-09 16:47:07.000000 starfishX-0.155555/starfishX/news_api.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5951 2020-07-27 00:12:32.000000 starfishX-0.155555/starfishX/npl_fn.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3826 2021-05-02 19:02:22.000000 starfishX-0.155555/starfishX/nvdr.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4262 2021-02-15 07:19:08.000000 starfishX-0.155555/starfishX/openInterest.py
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.311091 starfishX-0.155555/starfishX/peterlynch/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2051 2021-12-03 07:03:30.000000 starfishX-0.155555/starfishX/peterlynch/__init__.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    12043 2021-08-19 08:50:42.000000 starfishX-0.155555/starfishX/peterlynch/balancesheet.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      385 2020-05-11 01:51:12.000000 starfishX-0.155555/starfishX/peterlynch/condition.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5102 2021-12-03 07:01:38.000000 starfishX-0.155555/starfishX/peterlynch/fcf.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1189 2020-05-02 21:56:32.000000 starfishX-0.155555/starfishX/peterlynch/iaa.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4252 2021-04-18 03:42:48.000000 starfishX-0.155555/starfishX/peterlynch/industrial.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1266 2020-05-14 03:00:02.000000 starfishX-0.155555/starfishX/peterlynch/longtermdebt.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1318 2020-05-20 02:32:56.000000 starfishX-0.155555/starfishX/peterlynch/pehistory.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2195 2020-05-13 04:50:44.000000 starfishX-0.155555/starfishX/peterlynch/peproxy.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8767 2020-11-01 00:54:10.000000 starfishX-0.155555/starfishX/peterlynch/r59.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1534 2020-05-02 03:54:32.000000 starfishX-0.155555/starfishX/peterlynch/shareholders.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      701 2020-06-05 21:45:16.000000 starfishX-0.155555/starfishX/peterlynch/sixclass.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    10234 2020-05-18 23:48:54.000000 starfishX-0.155555/starfishX/peterlynch/strategy.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2604 2020-07-12 02:50:14.000000 starfishX-0.155555/starfishX/peterlynch/sumofthepart.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     6722 2020-04-17 01:41:50.000000 starfishX-0.155555/starfishX/risk_kit.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1186 2020-07-23 22:00:20.000000 starfishX-0.155555/starfishX/sentimentAnalysis.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3665 2020-02-19 23:33:36.000000 starfishX-0.155555/starfishX/shortsale.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7417 2019-10-09 21:55:58.000000 starfishX-0.155555/starfishX/squarify.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    90111 2022-10-23 14:49:25.000000 starfishX-0.155555/starfishX/starfishXfn.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7318 2023-03-11 03:59:40.000000 starfishX-0.155555/starfishX/utilHelpers.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1376 2020-04-11 02:16:24.000000 starfishX-0.155555/starfishX/utility.py
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.312391 starfishX-0.155555/starfishX/volatility/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       90 2020-09-22 03:32:34.000000 starfishX-0.155555/starfishX/volatility/__init__.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       41 2020-09-22 02:27:40.000000 starfishX-0.155555/starfishX/volatility/typevol.py
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5187 2020-09-22 04:01:08.000000 starfishX-0.155555/starfishX/volatility/vol.py
-drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-03-11 04:02:14.303736 starfishX-0.155555/starfishX.egg-info/
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11846 2023-03-11 04:02:13.000000 starfishX-0.155555/starfishX.egg-info/PKG-INFO
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1932 2023-03-11 04:02:14.000000 starfishX-0.155555/starfishX.egg-info/SOURCES.txt
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        1 2023-03-11 04:02:13.000000 starfishX-0.155555/starfishX.egg-info/dependency_links.txt
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        1 2023-03-01 03:49:45.000000 starfishX-0.155555/starfishX.egg-info/not-zip-safe
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      135 2023-03-11 04:02:13.000000 starfishX-0.155555/starfishX.egg-info/requires.txt
--rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       10 2023-03-11 04:02:14.000000 starfishX-0.155555/starfishX.egg-info/top_level.txt
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.791244 starfishX-0.155556/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11810 2023-04-11 15:02:28.790603 starfishX-0.155556/PKG-INFO
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11466 2021-11-04 08:06:30.000000 starfishX-0.155556/README.rst
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       38 2023-04-11 15:02:28.791433 starfishX-0.155556/setup.cfg
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1245 2023-04-11 14:57:02.000000 starfishX-0.155556/setup.py
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.767852 starfishX-0.155556/starfishX/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8812 2020-02-19 23:32:22.000000 starfishX-0.155556/starfishX/AD.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4762 2019-06-07 20:21:16.000000 starfishX-0.155556/starfishX/DividendDiscountModel.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7483 2019-07-22 21:24:16.000000 starfishX-0.155556/starfishX/DuPontROE.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5675 2020-06-13 19:53:26.000000 starfishX-0.155556/starfishX/EYG.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1176 2019-10-30 20:54:04.000000 starfishX-0.155556/starfishX/Elder.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7116 2020-05-05 04:45:24.000000 starfishX-0.155556/starfishX/InterestBearingDebt.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5827 2020-06-19 23:59:20.000000 starfishX-0.155556/starfishX/Ke.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4210 2020-12-04 07:28:08.000000 starfishX-0.155556/starfishX/ShareholdersNow.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8084 2023-04-11 14:56:44.000000 starfishX-0.155556/starfishX/__init__.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5349 2020-02-19 23:56:32.000000 starfishX-0.155556/starfishX/checkServices.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       52 2019-10-23 06:36:20.000000 starfishX-0.155556/starfishX/config.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        0 2019-07-25 02:52:00.000000 starfishX-0.155556/starfishX/dashFn.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2701 2021-08-19 08:07:52.000000 starfishX-0.155556/starfishX/depreciationAndAmortisation.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5494 2021-02-04 05:51:12.000000 starfishX-0.155556/starfishX/findMarketCap.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1187 2019-10-17 04:48:50.000000 starfishX-0.155556/starfishX/findSector.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      774 2021-11-04 01:02:16.000000 starfishX-0.155556/starfishX/getDW.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     9048 2020-03-28 22:56:16.000000 starfishX-0.155556/starfishX/getEVEBITDA.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2879 2022-06-30 02:33:18.000000 starfishX-0.155556/starfishX/getFundamentalInSector.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      900 2020-05-28 01:51:26.000000 starfishX-0.155556/starfishX/getProfitAbility.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5131 2021-10-10 19:19:26.000000 starfishX-0.155556/starfishX/getWarrant.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     9375 2021-10-10 01:38:06.000000 starfishX-0.155556/starfishX/greek.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2360 2020-02-14 21:45:28.000000 starfishX-0.155556/starfishX/helpers.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2732 2020-11-20 20:44:20.000000 starfishX-0.155556/starfishX/holidayMarket.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4952 2020-03-29 21:58:48.000000 starfishX-0.155556/starfishX/incomestatement.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      235 2019-06-17 23:30:54.000000 starfishX-0.155556/starfishX/indexMarket.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2609 2020-02-19 23:35:10.000000 starfishX-0.155556/starfishX/indicator.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3333 2020-11-30 01:37:02.000000 starfishX-0.155556/starfishX/ipoStat.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2868 2019-10-14 22:14:26.000000 starfishX-0.155556/starfishX/listSecurities.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3255 2021-10-10 22:24:16.000000 starfishX-0.155556/starfishX/loadHistData_v2.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5130 2020-02-19 23:24:46.000000 starfishX-0.155556/starfishX/marketValueDaily.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7110 2020-06-17 22:38:02.000000 starfishX-0.155556/starfishX/marketview.py
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.772440 starfishX-0.155556/starfishX/markminervini/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      302 2022-10-31 01:46:52.000000 starfishX-0.155556/starfishX/markminervini/__init__.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5718 2022-10-31 01:56:59.000000 starfishX-0.155556/starfishX/markminervini/trendtemplate.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3960 2020-02-19 23:34:00.000000 starfishX-0.155556/starfishX/moc.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     6437 2020-05-28 03:37:50.000000 starfishX-0.155556/starfishX/morningstarGetfn.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4686 2022-11-09 16:47:07.000000 starfishX-0.155556/starfishX/news_api.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5951 2020-07-27 00:12:32.000000 starfishX-0.155556/starfishX/npl_fn.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3826 2021-05-02 19:02:22.000000 starfishX-0.155556/starfishX/nvdr.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4262 2021-02-15 07:19:08.000000 starfishX-0.155556/starfishX/openInterest.py
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.787446 starfishX-0.155556/starfishX/peterlynch/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2051 2021-12-03 07:03:30.000000 starfishX-0.155556/starfishX/peterlynch/__init__.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    12043 2021-08-19 08:50:42.000000 starfishX-0.155556/starfishX/peterlynch/balancesheet.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      385 2020-05-11 01:51:12.000000 starfishX-0.155556/starfishX/peterlynch/condition.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5102 2021-12-03 07:01:38.000000 starfishX-0.155556/starfishX/peterlynch/fcf.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1189 2020-05-02 21:56:32.000000 starfishX-0.155556/starfishX/peterlynch/iaa.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     4252 2021-04-18 03:42:48.000000 starfishX-0.155556/starfishX/peterlynch/industrial.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1266 2020-05-14 03:00:02.000000 starfishX-0.155556/starfishX/peterlynch/longtermdebt.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1318 2020-05-20 02:32:56.000000 starfishX-0.155556/starfishX/peterlynch/pehistory.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2195 2020-05-13 04:50:44.000000 starfishX-0.155556/starfishX/peterlynch/peproxy.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     8767 2020-11-01 00:54:10.000000 starfishX-0.155556/starfishX/peterlynch/r59.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1534 2020-05-02 03:54:32.000000 starfishX-0.155556/starfishX/peterlynch/shareholders.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      701 2020-06-05 21:45:16.000000 starfishX-0.155556/starfishX/peterlynch/sixclass.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    10234 2020-05-18 23:48:54.000000 starfishX-0.155556/starfishX/peterlynch/strategy.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     2604 2020-07-12 02:50:14.000000 starfishX-0.155556/starfishX/peterlynch/sumofthepart.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     6722 2020-04-17 01:41:50.000000 starfishX-0.155556/starfishX/risk_kit.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1186 2020-07-23 22:00:20.000000 starfishX-0.155556/starfishX/sentimentAnalysis.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     3665 2020-02-19 23:33:36.000000 starfishX-0.155556/starfishX/shortsale.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7417 2019-10-09 21:55:58.000000 starfishX-0.155556/starfishX/squarify.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    90111 2022-10-23 14:49:25.000000 starfishX-0.155556/starfishX/starfishXfn.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     7318 2023-04-11 14:54:34.000000 starfishX-0.155556/starfishX/utilHelpers.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1376 2020-04-11 02:16:24.000000 starfishX-0.155556/starfishX/utility.py
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.789611 starfishX-0.155556/starfishX/volatility/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       90 2020-09-22 03:32:34.000000 starfishX-0.155556/starfishX/volatility/__init__.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       41 2020-09-22 02:27:40.000000 starfishX-0.155556/starfishX/volatility/typevol.py
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     5187 2020-09-22 04:01:08.000000 starfishX-0.155556/starfishX/volatility/vol.py
+drwxr-xr-x   0 nattapatattiratanasunthron   (501) staff       (20)        0 2023-04-11 15:02:28.770960 starfishX-0.155556/starfishX.egg-info/
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)    11810 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/PKG-INFO
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)     1932 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/SOURCES.txt
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        1 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/dependency_links.txt
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)        1 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/not-zip-safe
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)      135 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/requires.txt
+-rw-r--r--   0 nattapatattiratanasunthron   (501) staff       (20)       10 2023-04-11 15:02:28.000000 starfishX-0.155556/starfishX.egg-info/top_level.txt
```

### Comparing `starfishX-0.155555/PKG-INFO` & `starfishX-0.155556/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: starfishX
-Version: 0.155555
+Version: 0.155556
 Summary: Get data of stock exchange thailand (SET)
 Home-page: https://github.com/tapattan/starfishX
 Author: nattapat attiratanasunthron
 Author-email: tapattan@gmail.com
-License: UNKNOWN
 Keywords: starfishx,finance,การลงทุน,หุ้น,peterlynch
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Library สำหรับประมวลข้อมูลตลาดหุ้นไทย Stock Exchange of Thailand https://www.set.or.th และการจัดการ Portfolio
 
 พื้นฐานที่ต้องการ
 
     $ conda install -c conda-forge matplotlib
@@ -209,8 +207,7 @@
 - 6.Yang-Zhang (Open-High-Low-Close + จัดการราคาที่ไม่เปลี่ยนแปลงได้ + จัดการราคาที่มีการเปิดกระโดดได้)
 
 ติดต่อฉัน แจ้ง BUG แจ้ง Error ได้ที่
 
  Facebook : https://www.facebook.com/Superstarman-1464755373546185/
 
  Email    : tapattan@จีเมล์ดอทคอม
-
```

### Comparing `starfishX-0.155555/README.rst` & `starfishX-0.155556/README.rst`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/setup.py` & `starfishX-0.155556/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup#, find_namespace_packages
 def readme():
     with open('README.rst', encoding='utf-8') as f:
         return f.read()
 
 setup(
      name='starfishX',   # This is the name of your PyPI-package.
-     version='0.155555',  # Update the version number for new releases
+     version='0.155556',  # Update the version number for new releases
      author='nattapat attiratanasunthron',
      author_email='tapattan@gmail.com',
      url='https://github.com/tapattan/starfishX',
      #packages=['starfishX'],
      packages=['starfishX','starfishX.peterlynch','starfishX.volatility','starfishX.markminervini'],
      #package_data={'starfishX': ['sa_model.h5','dictionary.json']},
      #packages=find_namespace_packages(include=['starfishX','starfishX.peterlynch']),
```

### Comparing `starfishX-0.155555/starfishX/AD.py` & `starfishX-0.155556/starfishX/AD.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/DividendDiscountModel.py` & `starfishX-0.155556/starfishX/DividendDiscountModel.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/DuPontROE.py` & `starfishX-0.155556/starfishX/DuPontROE.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/EYG.py` & `starfishX-0.155556/starfishX/EYG.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/Elder.py` & `starfishX-0.155556/starfishX/Elder.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/InterestBearingDebt.py` & `starfishX-0.155556/starfishX/InterestBearingDebt.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/Ke.py` & `starfishX-0.155556/starfishX/Ke.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/ShareholdersNow.py` & `starfishX-0.155556/starfishX/ShareholdersNow.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/__init__.py` & `starfishX-0.155556/starfishX/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,10 +209,10 @@
 exec("from "+prefix+"greek import EuropeanCall")
 exec("from "+prefix+"greek import EuropeanCallRolling")
 
 #exec("from "+prefix+"utilHelpers import rankWithRange")
 #exec("from "+prefix+"utilHelpers import HistStockPrice")
  
 
-__version__ = 0.155555  #21 Feb 2023 update 0.155549
+__version__ = 0.155556  #21 Feb 2023 update 0.155549
 
 __doc__ = """starfishX Version จัดเตรียมข้อมูลสำหรับประมวลผลการลงทุนในตลาดหุ้นไทย """
```

### Comparing `starfishX-0.155555/starfishX/checkServices.py` & `starfishX-0.155556/starfishX/checkServices.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/depreciationAndAmortisation.py` & `starfishX-0.155556/starfishX/depreciationAndAmortisation.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/findMarketCap.py` & `starfishX-0.155556/starfishX/findMarketCap.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/findSector.py` & `starfishX-0.155556/starfishX/findSector.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/getDW.py` & `starfishX-0.155556/starfishX/getDW.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/getEVEBITDA.py` & `starfishX-0.155556/starfishX/getEVEBITDA.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/getFundamentalInSector.py` & `starfishX-0.155556/starfishX/getFundamentalInSector.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/getProfitAbility.py` & `starfishX-0.155556/starfishX/getProfitAbility.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/getWarrant.py` & `starfishX-0.155556/starfishX/getWarrant.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/greek.py` & `starfishX-0.155556/starfishX/greek.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/helpers.py` & `starfishX-0.155556/starfishX/helpers.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/holidayMarket.py` & `starfishX-0.155556/starfishX/holidayMarket.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/incomestatement.py` & `starfishX-0.155556/starfishX/incomestatement.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/indicator.py` & `starfishX-0.155556/starfishX/indicator.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/ipoStat.py` & `starfishX-0.155556/starfishX/ipoStat.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/listSecurities.py` & `starfishX-0.155556/starfishX/listSecurities.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/loadHistData_v2.py` & `starfishX-0.155556/starfishX/loadHistData_v2.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/marketValueDaily.py` & `starfishX-0.155556/starfishX/marketValueDaily.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/marketview.py` & `starfishX-0.155556/starfishX/marketview.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/markminervini/trendtemplate.py` & `starfishX-0.155556/starfishX/markminervini/trendtemplate.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/moc.py` & `starfishX-0.155556/starfishX/moc.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/morningstarGetfn.py` & `starfishX-0.155556/starfishX/morningstarGetfn.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/news_api.py` & `starfishX-0.155556/starfishX/news_api.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/npl_fn.py` & `starfishX-0.155556/starfishX/npl_fn.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/nvdr.py` & `starfishX-0.155556/starfishX/nvdr.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/openInterest.py` & `starfishX-0.155556/starfishX/openInterest.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/__init__.py` & `starfishX-0.155556/starfishX/peterlynch/__init__.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/balancesheet.py` & `starfishX-0.155556/starfishX/peterlynch/balancesheet.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/fcf.py` & `starfishX-0.155556/starfishX/peterlynch/fcf.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/iaa.py` & `starfishX-0.155556/starfishX/peterlynch/iaa.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/industrial.py` & `starfishX-0.155556/starfishX/peterlynch/industrial.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/longtermdebt.py` & `starfishX-0.155556/starfishX/peterlynch/longtermdebt.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/pehistory.py` & `starfishX-0.155556/starfishX/peterlynch/pehistory.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/peproxy.py` & `starfishX-0.155556/starfishX/peterlynch/peproxy.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/r59.py` & `starfishX-0.155556/starfishX/peterlynch/r59.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/shareholders.py` & `starfishX-0.155556/starfishX/peterlynch/shareholders.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/sixclass.py` & `starfishX-0.155556/starfishX/peterlynch/sixclass.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/strategy.py` & `starfishX-0.155556/starfishX/peterlynch/strategy.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/peterlynch/sumofthepart.py` & `starfishX-0.155556/starfishX/peterlynch/sumofthepart.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/risk_kit.py` & `starfishX-0.155556/starfishX/risk_kit.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/sentimentAnalysis.py` & `starfishX-0.155556/starfishX/sentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/shortsale.py` & `starfishX-0.155556/starfishX/shortsale.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/squarify.py` & `starfishX-0.155556/starfishX/squarify.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/starfishXfn.py` & `starfishX-0.155556/starfishX/starfishXfn.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/utilHelpers.py` & `starfishX-0.155556/starfishX/utilHelpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     return data[-1][ratio]    
     
 
 def getRatio_info():
   # url จากตลาดหลักทรัพย์
 
   rp = []
-  symbol = 'advanc'
+  symbol = 'ADVANC'
   url = getURL(symbol,'trading-stat')
   headers = {'Accept': 'application/json'}
   r = requests.get(url, headers=headers)
   data = r.json()  
   for i in data[-1]:
     rp.append(i)
```

### Comparing `starfishX-0.155555/starfishX/utility.py` & `starfishX-0.155556/starfishX/utility.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX/volatility/vol.py` & `starfishX-0.155556/starfishX/volatility/vol.py`

 * *Files identical despite different names*

### Comparing `starfishX-0.155555/starfishX.egg-info/PKG-INFO` & `starfishX-0.155556/starfishX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: starfishX
-Version: 0.155555
+Version: 0.155556
 Summary: Get data of stock exchange thailand (SET)
 Home-page: https://github.com/tapattan/starfishX
 Author: nattapat attiratanasunthron
 Author-email: tapattan@gmail.com
-License: UNKNOWN
 Keywords: starfishx,finance,การลงทุน,หุ้น,peterlynch
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Library สำหรับประมวลข้อมูลตลาดหุ้นไทย Stock Exchange of Thailand https://www.set.or.th และการจัดการ Portfolio
 
 พื้นฐานที่ต้องการ
 
     $ conda install -c conda-forge matplotlib
@@ -209,8 +207,7 @@
 - 6.Yang-Zhang (Open-High-Low-Close + จัดการราคาที่ไม่เปลี่ยนแปลงได้ + จัดการราคาที่มีการเปิดกระโดดได้)
 
 ติดต่อฉัน แจ้ง BUG แจ้ง Error ได้ที่
 
  Facebook : https://www.facebook.com/Superstarman-1464755373546185/
 
  Email    : tapattan@จีเมล์ดอทคอม
-
```

### Comparing `starfishX-0.155555/starfishX.egg-info/SOURCES.txt` & `starfishX-0.155556/starfishX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

