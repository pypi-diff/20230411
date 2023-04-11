# Comparing `tmp/myiqoptionapi-7.1.2.tar.gz` & `tmp/myiqoptionapi-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myiqoptionapi-7.1.2.tar", last modified: Tue Apr 11 08:22:00 2023, max compression
+gzip compressed data, was "myiqoptionapi-7.1.3.tar", last modified: Tue Apr 11 08:49:42 2023, max compression
```

## Comparing `myiqoptionapi-7.1.2.tar` & `myiqoptionapi-7.1.3.tar`

### file list

```diff
@@ -1,13 +1,148 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:22:00.308403 myiqoptionapi-7.1.2/
--rw-rw-rw-   0        0        0     1094 2023-04-11 07:13:14.000000 myiqoptionapi-7.1.2/LICENCE
--rw-rw-rw-   0        0        0      287 2023-04-11 08:22:00.309399 myiqoptionapi-7.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-11 07:39:03.000000 myiqoptionapi-7.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:22:00.306403 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/
--rw-rw-rw-   0        0        0      287 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:22:00.000000 myiqoptionapi-7.1.2/myiqoptionapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      380 2023-04-11 08:22:00.311394 myiqoptionapi-7.1.2/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-11 07:55:04.000000 myiqoptionapi-7.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.751990 myiqoptionapi-7.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-11 07:13:14.000000 myiqoptionapi-7.1.3/LICENCE
+-rw-rw-rw-   0        0        0      287 2023-04-11 08:49:42.751990 myiqoptionapi-7.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-04-11 07:39:03.000000 myiqoptionapi-7.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.468470 myiqoptionapi-7.1.3/myiqoptionapi/
+-rw-rw-rw-   0        0        0       26 2023-04-11 08:46:24.000000 myiqoptionapi-7.1.3/myiqoptionapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.499673 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/
+-rw-rw-rw-   0        0        0      541 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/__init__.py
+-rw-rw-rw-   0        0        0    31700 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/api.py
+-rw-rw-rw-   0        0        0     6720 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/constants.py
+-rw-rw-rw-   0        0        0     3335 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/country_id.py
+-rw-rw-rw-   0        0        0     2680 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/expiration.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/global_value.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.539566 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/
+-rw-rw-rw-   0        0        0       48 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/appinit.py
+-rw-rw-rw-   0        0        0      242 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/auth.py
+-rw-rw-rw-   0        0        0      244 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/billing.py
+-rw-rw-rw-   0        0        0      902 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/buyback.py
+-rw-rw-rw-   0        0        0      935 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/changebalance.py
+-rw-rw-rw-   0        0        0      980 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/events.py
+-rw-rw-rw-   0        0        0      679 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/getprofile.py
+-rw-rw-rw-   0        0        0      753 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/getregdata.py
+-rw-rw-rw-   0        0        0     1004 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/login.py
+-rw-rw-rw-   0        0        0     1123 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/login2fa.py
+-rw-rw-rw-   0        0        0      334 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/loginv2.py
+-rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/logout.py
+-rw-rw-rw-   0        0        0      244 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/profile.py
+-rw-rw-rw-   0        0        0      248 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/register.py
+-rw-rw-rw-   0        0        0      923 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/resource.py
+-rw-rw-rw-   0        0        0     1410 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/send_sms.py
+-rw-rw-rw-   0        0        0      790 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/token.py
+-rw-rw-rw-   0        0        0     1445 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/http/verify.py
+-rw-rw-rw-   0        0        0    63900 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/stable_api.py
+-rw-rw-rw-   0        0        0       21 2023-04-11 08:49:27.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.543547 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/
+-rw-rw-rw-   0        0        0       43 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.618349 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/
+-rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/api_game_betinfo.py
+-rw-rw-rw-   0        0        0      864 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/api_game_getoptions.py
+-rw-rw-rw-   0        0        0      845 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/base.py
+-rw-rw-rw-   0        0        0     2068 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/buy_place_order_temp.py
+-rw-rw-rw-   0        0        0      376 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/buyback.py
+-rw-rw-rw-   0        0        0     1257 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/buyv2.py
+-rw-rw-rw-   0        0        0     3282 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/buyv3.py
+-rw-rw-rw-   0        0        0      397 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/cancel_order.py
+-rw-rw-rw-   0        0        0     1310 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/candles.py
+-rw-rw-rw-   0        0        0      481 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/change_auto_margin_call.py
+-rw-rw-rw-   0        0        0      953 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/change_tpsl.py
+-rw-rw-rw-   0        0        0      709 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/changebalance.py
+-rw-rw-rw-   0        0        0      410 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/close_position.py
+-rw-rw-rw-   0        0        0     1963 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/digital_option.py
+-rw-rw-rw-   0        0        0      486 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_available_leverages.py
+-rw-rw-rw-   0        0        0      368 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_balances.py
+-rw-rw-rw-   0        0        0      603 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_deferred_orders.py
+-rw-rw-rw-   0        0        0     1312 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_financial_information.py
+-rw-rw-rw-   0        0        0      485 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_order.py
+-rw-rw-rw-   0        0        0      514 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_overnight_fee.py
+-rw-rw-rw-   0        0        0     2294 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/get_positions.py
+-rw-rw-rw-   0        0        0      457 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/heartbeat.py
+-rw-rw-rw-   0        0        0      447 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/instruments.py
+-rw-rw-rw-   0        0        0     1339 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/leaderboard.py
+-rw-rw-rw-   0        0        0     1069 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/sell_digital_option.py
+-rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/sell_option.py
+-rw-rw-rw-   0        0        0      534 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/setactives.py
+-rw-rw-rw-   0        0        0      460 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/ssid.py
+-rw-rw-rw-   0        0        0     1067 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/strike_list.py
+-rw-rw-rw-   0        0        0     5010 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/subscribe.py
+-rw-rw-rw-   0        0        0      515 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/technical_indicators.py
+-rw-rw-rw-   0        0        0     1126 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/traders_mood.py
+-rw-rw-rw-   0        0        0     4492 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/unsubscribe.py
+-rw-rw-rw-   0        0        0     1558 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/chanels/user.py
+-rw-rw-rw-   0        0        0     9212 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.633308 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/
+-rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/base.py
+-rw-rw-rw-   0        0        0      728 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/betinfo.py
+-rw-rw-rw-   0        0        0     2931 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/candles.py
+-rw-rw-rw-   0        0        0      683 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/listinfodata.py
+-rw-rw-rw-   0        0        0     3310 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/profile.py
+-rw-rw-rw-   0        0        0     1987 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/objects/timesync.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.749996 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/
+-rw-rw-rw-   0        0        0       52 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/api_game_betinfo_result.py
+-rw-rw-rw-   0        0        0      193 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/api_game_getoptions_result.py
+-rw-rw-rw-   0        0        0      200 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/api_option_init_all_result.py
+-rw-rw-rw-   0        0        0      195 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/auto_margin_call_changed.py
+-rw-rw-rw-   0        0        0      172 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/available_leverages.py
+-rw-rw-rw-   0        0        0      555 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/balance_changed.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/balances.py
+-rw-rw-rw-   0        0        0      285 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/buy_complete.py
+-rw-rw-rw-   0        0        0      771 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/candle_generated.py
+-rw-rw-rw-   0        0        0      967 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/candle_generated_v2.py
+-rw-rw-rw-   0        0        0      220 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/candles.py
+-rw-rw-rw-   0        0        0      381 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/client_price_generated.py
+-rw-rw-rw-   0        0        0      593 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/commission_changed.py
+-rw-rw-rw-   0        0        0      160 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/deferred_orders.py
+-rw-rw-rw-   0        0        0      598 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/digital_option_placed.py
+-rw-rw-rw-   0        0        0      182 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/financial_information.py
+-rw-rw-rw-   0        0        0      201 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/heartbeat.py
+-rw-rw-rw-   0        0        0      168 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/history_positions.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/initialization_data.py
+-rw-rw-rw-   0        0        0     1367 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/instrument_quotes_generated.py
+-rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/instruments.py
+-rw-rw-rw-   0        0        0      194 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/leaderboard_deals_client.py
+-rw-rw-rw-   0        0        0      221 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/leaderboard_userinfo_deals_client.py
+-rw-rw-rw-   0        0        0      237 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/list_info_data.py
+-rw-rw-rw-   0        0        0      952 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/live_deal.py
+-rw-rw-rw-   0        0        0     1007 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/live_deal_binary_option_placed.py
+-rw-rw-rw-   0        0        0     1019 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/live_deal_digital_option.py
+-rw-rw-rw-   0        0        0      178 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/option.py
+-rw-rw-rw-   0        0        0      340 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/option_closed.py
+-rw-rw-rw-   0        0        0      203 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/option_opened.py
+-rw-rw-rw-   0        0        0      147 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/options.py
+-rw-rw-rw-   0        0        0      137 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/order.py
+-rw-rw-rw-   0        0        0      157 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/order_canceled.py
+-rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/order_placed_temp.py
+-rw-rw-rw-   0        0        0      154 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/overnight_fee.py
+-rw-rw-rw-   0        0        0      141 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/position.py
+-rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/position_changed.py
+-rw-rw-rw-   0        0        0      216 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/position_closed.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/position_history.py
+-rw-rw-rw-   0        0        0      144 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/positions.py
+-rw-rw-rw-   0        0        0     1089 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/profile.py
+-rw-rw-rw-   0        0        0      151 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/result.py
+-rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/socket_option_closed.py
+-rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/socket_option_opened.py
+-rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/sold_options.py
+-rw-rw-rw-   0        0        0      148 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/strike_list.py
+-rw-rw-rw-   0        0        0      557 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/technical_indicators.py
+-rw-rw-rw-   0        0        0      164 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/time_sync.py
+-rw-rw-rw-   0        0        0      229 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/top_assets_updated.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/tpsl_changed.py
+-rw-rw-rw-   0        0        0      211 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/traders_mood_changed.py
+-rw-rw-rw-   0        0        0      212 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/training_balance_reset.py
+-rw-rw-rw-   0        0        0      174 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/underlying_list.py
+-rw-rw-rw-   0        0        0      179 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/user_profile_client.py
+-rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 myiqoptionapi-7.1.3/myiqoptionapi/iqoptionapi/ws/received/users_availability.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:49:42.482713 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6947 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:49:42.000000 myiqoptionapi-7.1.3/myiqoptionapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      380 2023-04-11 08:49:42.755981 myiqoptionapi-7.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-11 08:48:42.000000 myiqoptionapi-7.1.3/setup.py
```

### Comparing `myiqoptionapi-7.1.2/LICENCE` & `myiqoptionapi-7.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `myiqoptionapi-7.1.2/setup.py` & `myiqoptionapi-7.1.3/setup.py`

 * *Files identical despite different names*

