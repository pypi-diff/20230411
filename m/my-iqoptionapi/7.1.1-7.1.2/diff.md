# Comparing `tmp/my-iqoptionapi-7.1.1.tar.gz` & `tmp/my_iqoptionapi-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-iqoptionapi-7.1.1.tar", last modified: Tue Apr 11 09:21:10 2023, max compression
+gzip compressed data, was "my_iqoptionapi-7.1.2.tar", last modified: Tue Apr 11 20:58:14 2023, max compression
```

## Comparing `my-iqoptionapi-7.1.1.tar` & `my_iqoptionapi-7.1.2.tar`

### file list

```diff
@@ -1,148 +1,146 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:10.100827 my-iqoptionapi-7.1.1/
--rw-rw-rw-   0        0        0     1094 2023-04-11 07:13:14.000000 my-iqoptionapi-7.1.1/LICENCE
--rw-rw-rw-   0        0        0      288 2023-04-11 09:21:10.099828 my-iqoptionapi-7.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-04-11 07:39:03.000000 my-iqoptionapi-7.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.829999 my-iqoptionapi-7.1.1/my-iqoptionapi/
--rw-rw-rw-   0        0        0       26 2023-04-11 08:46:24.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.847951 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/
--rw-rw-rw-   0        0        0      541 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/__init__.py
--rw-rw-rw-   0        0        0    31700 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/api.py
--rw-rw-rw-   0        0        0     6720 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/constants.py
--rw-rw-rw-   0        0        0     3335 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/country_id.py
--rw-rw-rw-   0        0        0     2680 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/expiration.py
--rw-rw-rw-   0        0        0      414 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/global_value.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.891177 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/
--rw-rw-rw-   0        0        0       48 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/__init__.py
--rw-rw-rw-   0        0        0      712 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/appinit.py
--rw-rw-rw-   0        0        0      242 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/auth.py
--rw-rw-rw-   0        0        0      244 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/billing.py
--rw-rw-rw-   0        0        0      902 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/buyback.py
--rw-rw-rw-   0        0        0      935 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/changebalance.py
--rw-rw-rw-   0        0        0      980 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/events.py
--rw-rw-rw-   0        0        0      679 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/getprofile.py
--rw-rw-rw-   0        0        0      753 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/getregdata.py
--rw-rw-rw-   0        0        0     1004 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/login.py
--rw-rw-rw-   0        0        0     1123 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/login2fa.py
--rw-rw-rw-   0        0        0      334 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/loginv2.py
--rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/logout.py
--rw-rw-rw-   0        0        0      244 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/profile.py
--rw-rw-rw-   0        0        0      248 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/register.py
--rw-rw-rw-   0        0        0      923 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/resource.py
--rw-rw-rw-   0        0        0     1410 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/send_sms.py
--rw-rw-rw-   0        0        0      790 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/token.py
--rw-rw-rw-   0        0        0     1445 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/verify.py
--rw-rw-rw-   0        0        0    63900 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/stable_api.py
--rw-rw-rw-   0        0        0       21 2023-04-11 08:49:27.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/version_control.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.895837 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/
--rw-rw-rw-   0        0        0       43 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.966638 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/
--rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/__init__.py
--rw-rw-rw-   0        0        0      631 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/api_game_betinfo.py
--rw-rw-rw-   0        0        0      864 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/api_game_getoptions.py
--rw-rw-rw-   0        0        0      845 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/base.py
--rw-rw-rw-   0        0        0     2068 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buy_place_order_temp.py
--rw-rw-rw-   0        0        0      376 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buyback.py
--rw-rw-rw-   0        0        0     1257 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buyv2.py
--rw-rw-rw-   0        0        0     3282 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buyv3.py
--rw-rw-rw-   0        0        0      397 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/cancel_order.py
--rw-rw-rw-   0        0        0     1310 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/candles.py
--rw-rw-rw-   0        0        0      481 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/change_auto_margin_call.py
--rw-rw-rw-   0        0        0      953 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/change_tpsl.py
--rw-rw-rw-   0        0        0      709 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/changebalance.py
--rw-rw-rw-   0        0        0      410 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/close_position.py
--rw-rw-rw-   0        0        0     1963 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/digital_option.py
--rw-rw-rw-   0        0        0      486 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_available_leverages.py
--rw-rw-rw-   0        0        0      368 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_balances.py
--rw-rw-rw-   0        0        0      603 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_deferred_orders.py
--rw-rw-rw-   0        0        0     1312 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_financial_information.py
--rw-rw-rw-   0        0        0      485 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_order.py
--rw-rw-rw-   0        0        0      514 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_overnight_fee.py
--rw-rw-rw-   0        0        0     2294 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_positions.py
--rw-rw-rw-   0        0        0      457 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/heartbeat.py
--rw-rw-rw-   0        0        0      447 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/instruments.py
--rw-rw-rw-   0        0        0     1339 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/leaderboard.py
--rw-rw-rw-   0        0        0     1069 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/sell_digital_option.py
--rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/sell_option.py
--rw-rw-rw-   0        0        0      534 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/setactives.py
--rw-rw-rw-   0        0        0      460 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/ssid.py
--rw-rw-rw-   0        0        0     1067 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/strike_list.py
--rw-rw-rw-   0        0        0     5010 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/subscribe.py
--rw-rw-rw-   0        0        0      515 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/technical_indicators.py
--rw-rw-rw-   0        0        0     1126 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/traders_mood.py
--rw-rw-rw-   0        0        0     4492 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/unsubscribe.py
--rw-rw-rw-   0        0        0     1558 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/user.py
--rw-rw-rw-   0        0        0     9212 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/client.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:09.979602 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/
--rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/base.py
--rw-rw-rw-   0        0        0      728 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/betinfo.py
--rw-rw-rw-   0        0        0     2931 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/candles.py
--rw-rw-rw-   0        0        0      683 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/listinfodata.py
--rw-rw-rw-   0        0        0     3310 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/profile.py
--rw-rw-rw-   0        0        0     1987 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/timesync.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:10.085866 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/
--rw-rw-rw-   0        0        0       52 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/api_game_betinfo_result.py
--rw-rw-rw-   0        0        0      193 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/api_game_getoptions_result.py
--rw-rw-rw-   0        0        0      200 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/api_option_init_all_result.py
--rw-rw-rw-   0        0        0      195 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/auto_margin_call_changed.py
--rw-rw-rw-   0        0        0      172 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/available_leverages.py
--rw-rw-rw-   0        0        0      555 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/balance_changed.py
--rw-rw-rw-   0        0        0      143 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/balances.py
--rw-rw-rw-   0        0        0      285 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/buy_complete.py
--rw-rw-rw-   0        0        0      771 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/candle_generated.py
--rw-rw-rw-   0        0        0      967 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/candle_generated_v2.py
--rw-rw-rw-   0        0        0      220 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/candles.py
--rw-rw-rw-   0        0        0      381 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/client_price_generated.py
--rw-rw-rw-   0        0        0      593 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/commission_changed.py
--rw-rw-rw-   0        0        0      160 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/deferred_orders.py
--rw-rw-rw-   0        0        0      598 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/digital_option_placed.py
--rw-rw-rw-   0        0        0      182 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/financial_information.py
--rw-rw-rw-   0        0        0      201 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/heartbeat.py
--rw-rw-rw-   0        0        0      168 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/history_positions.py
--rw-rw-rw-   0        0        0      189 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/initialization_data.py
--rw-rw-rw-   0        0        0     1367 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/instrument_quotes_generated.py
--rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/instruments.py
--rw-rw-rw-   0        0        0      194 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/leaderboard_deals_client.py
--rw-rw-rw-   0        0        0      221 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/leaderboard_userinfo_deals_client.py
--rw-rw-rw-   0        0        0      237 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/list_info_data.py
--rw-rw-rw-   0        0        0      952 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal.py
--rw-rw-rw-   0        0        0     1007 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal_binary_option_placed.py
--rw-rw-rw-   0        0        0     1019 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal_digital_option.py
--rw-rw-rw-   0        0        0      178 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/option.py
--rw-rw-rw-   0        0        0      340 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/option_closed.py
--rw-rw-rw-   0        0        0      203 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/option_opened.py
--rw-rw-rw-   0        0        0      147 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/options.py
--rw-rw-rw-   0        0        0      137 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/order.py
--rw-rw-rw-   0        0        0      157 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/order_canceled.py
--rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/order_placed_temp.py
--rw-rw-rw-   0        0        0      154 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/overnight_fee.py
--rw-rw-rw-   0        0        0      141 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/position.py
--rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/position_changed.py
--rw-rw-rw-   0        0        0      216 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/position_closed.py
--rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/position_history.py
--rw-rw-rw-   0        0        0      144 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/positions.py
--rw-rw-rw-   0        0        0     1089 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/profile.py
--rw-rw-rw-   0        0        0      151 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/result.py
--rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/socket_option_closed.py
--rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/socket_option_opened.py
--rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/sold_options.py
--rw-rw-rw-   0        0        0      148 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/strike_list.py
--rw-rw-rw-   0        0        0      557 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/technical_indicators.py
--rw-rw-rw-   0        0        0      164 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/time_sync.py
--rw-rw-rw-   0        0        0      229 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/top_assets_updated.py
--rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/tpsl_changed.py
--rw-rw-rw-   0        0        0      211 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/traders_mood_changed.py
--rw-rw-rw-   0        0        0      212 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/training_balance_reset.py
--rw-rw-rw-   0        0        0      174 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/underlying_list.py
--rw-rw-rw-   0        0        0      179 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/user_profile_client.py
--rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/users_availability.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:21:10.097834 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/
--rw-rw-rw-   0        0        0      288 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7071 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-11 09:21:09.000000 my-iqoptionapi-7.1.1/my_iqoptionapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 09:21:10.100827 my-iqoptionapi-7.1.1/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-04-11 09:20:51.000000 my-iqoptionapi-7.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.989750 my_iqoptionapi-7.1.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-11 07:13:14.000000 my_iqoptionapi-7.1.2/LICENCE
+-rw-rw-rw-   0        0        0      288 2023-04-11 20:58:14.988755 my_iqoptionapi-7.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-11 20:13:18.000000 my_iqoptionapi-7.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.710545 my_iqoptionapi-7.1.2/my_iqoptionapi/
+-rw-rw-rw-   0        0        0      541 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/__init__.py
+-rw-rw-rw-   0        0        0    31931 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/api.py
+-rw-rw-rw-   0        0        0     6720 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/constants.py
+-rw-rw-rw-   0        0        0     3335 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/country_id.py
+-rw-rw-rw-   0        0        0     2680 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/expiration.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/global_value.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.766402 my_iqoptionapi-7.1.2/my_iqoptionapi/http/
+-rw-rw-rw-   0        0        0       48 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/appinit.py
+-rw-rw-rw-   0        0        0      245 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/auth.py
+-rw-rw-rw-   0        0        0      247 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/billing.py
+-rw-rw-rw-   0        0        0      908 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/buyback.py
+-rw-rw-rw-   0        0        0      941 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/changebalance.py
+-rw-rw-rw-   0        0        0      983 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/events.py
+-rw-rw-rw-   0        0        0      682 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/getprofile.py
+-rw-rw-rw-   0        0        0      759 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/getregdata.py
+-rw-rw-rw-   0        0        0     1007 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/login.py
+-rw-rw-rw-   0        0        0     1126 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/login2fa.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/loginv2.py
+-rw-rw-rw-   0        0        0      639 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/logout.py
+-rw-rw-rw-   0        0        0      247 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/profile.py
+-rw-rw-rw-   0        0        0      251 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/register.py
+-rw-rw-rw-   0        0        0      926 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/resource.py
+-rw-rw-rw-   0        0        0     1413 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/send_sms.py
+-rw-rw-rw-   0        0        0      796 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/token.py
+-rw-rw-rw-   0        0        0     1448 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/http/verify.py
+-rw-rw-rw-   0        0        0    63924 2023-04-11 20:00:34.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/stable_api.py
+-rw-rw-rw-   0        0        0       21 2023-04-11 20:58:06.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/version_control.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.770386 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/
+-rw-rw-rw-   0        0        0       43 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.850123 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/
+-rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/__init__.py
+-rw-rw-rw-   0        0        0      634 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/api_game_betinfo.py
+-rw-rw-rw-   0        0        0      870 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/api_game_getoptions.py
+-rw-rw-rw-   0        0        0      848 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/base.py
+-rw-rw-rw-   0        0        0     2074 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buy_place_order_temp.py
+-rw-rw-rw-   0        0        0      379 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buyback.py
+-rw-rw-rw-   0        0        0     1266 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buyv2.py
+-rw-rw-rw-   0        0        0     3300 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buyv3.py
+-rw-rw-rw-   0        0        0      400 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/cancel_order.py
+-rw-rw-rw-   0        0        0     1316 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/candles.py
+-rw-rw-rw-   0        0        0      484 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/change_auto_margin_call.py
+-rw-rw-rw-   0        0        0      956 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/change_tpsl.py
+-rw-rw-rw-   0        0        0      712 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/changebalance.py
+-rw-rw-rw-   0        0        0      413 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/close_position.py
+-rw-rw-rw-   0        0        0     1969 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/digital_option.py
+-rw-rw-rw-   0        0        0      489 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_available_leverages.py
+-rw-rw-rw-   0        0        0      371 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_balances.py
+-rw-rw-rw-   0        0        0      609 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_deferred_orders.py
+-rw-rw-rw-   0        0        0     1315 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_financial_information.py
+-rw-rw-rw-   0        0        0      488 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_order.py
+-rw-rw-rw-   0        0        0      517 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_overnight_fee.py
+-rw-rw-rw-   0        0        0     2300 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_positions.py
+-rw-rw-rw-   0        0        0      460 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/heartbeat.py
+-rw-rw-rw-   0        0        0      450 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/instruments.py
+-rw-rw-rw-   0        0        0     1342 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/leaderboard.py
+-rw-rw-rw-   0        0        0     1072 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/sell_digital_option.py
+-rw-rw-rw-   0        0        0      639 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/sell_option.py
+-rw-rw-rw-   0        0        0      537 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/setactives.py
+-rw-rw-rw-   0        0        0      463 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/ssid.py
+-rw-rw-rw-   0        0        0     1070 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/strike_list.py
+-rw-rw-rw-   0        0        0     5016 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/subscribe.py
+-rw-rw-rw-   0        0        0      518 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/technical_indicators.py
+-rw-rw-rw-   0        0        0     1129 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/traders_mood.py
+-rw-rw-rw-   0        0        0     4498 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/unsubscribe.py
+-rw-rw-rw-   0        0        0     1564 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/user.py
+-rw-rw-rw-   0        0        0     9383 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.865084 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/
+-rw-rw-rw-   0        0        0       51 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/base.py
+-rw-rw-rw-   0        0        0      731 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/betinfo.py
+-rw-rw-rw-   0        0        0     2943 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/candles.py
+-rw-rw-rw-   0        0        0      686 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/listinfodata.py
+-rw-rw-rw-   0        0        0     3313 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/profile.py
+-rw-rw-rw-   0        0        0     1990 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/timesync.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.985760 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/
+-rw-rw-rw-   0        0        0       52 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/api_game_betinfo_result.py
+-rw-rw-rw-   0        0        0      193 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/api_game_getoptions_result.py
+-rw-rw-rw-   0        0        0      200 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/api_option_init_all_result.py
+-rw-rw-rw-   0        0        0      195 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/auto_margin_call_changed.py
+-rw-rw-rw-   0        0        0      172 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/available_leverages.py
+-rw-rw-rw-   0        0        0      555 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/balance_changed.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/balances.py
+-rw-rw-rw-   0        0        0      285 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/buy_complete.py
+-rw-rw-rw-   0        0        0      777 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/candle_generated.py
+-rw-rw-rw-   0        0        0      970 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/candle_generated_v2.py
+-rw-rw-rw-   0        0        0      220 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/candles.py
+-rw-rw-rw-   0        0        0      381 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/client_price_generated.py
+-rw-rw-rw-   0        0        0      596 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/commission_changed.py
+-rw-rw-rw-   0        0        0      160 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/deferred_orders.py
+-rw-rw-rw-   0        0        0      598 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/digital_option_placed.py
+-rw-rw-rw-   0        0        0      182 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/financial_information.py
+-rw-rw-rw-   0        0        0      201 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/heartbeat.py
+-rw-rw-rw-   0        0        0      168 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/history_positions.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/initialization_data.py
+-rw-rw-rw-   0        0        0     1370 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/instrument_quotes_generated.py
+-rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/instruments.py
+-rw-rw-rw-   0        0        0      194 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/leaderboard_deals_client.py
+-rw-rw-rw-   0        0        0      221 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/leaderboard_userinfo_deals_client.py
+-rw-rw-rw-   0        0        0      237 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/list_info_data.py
+-rw-rw-rw-   0        0        0      955 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal.py
+-rw-rw-rw-   0        0        0     1010 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal_binary_option_placed.py
+-rw-rw-rw-   0        0        0     1022 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal_digital_option.py
+-rw-rw-rw-   0        0        0      178 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/option.py
+-rw-rw-rw-   0        0        0      340 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/option_closed.py
+-rw-rw-rw-   0        0        0      203 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/option_opened.py
+-rw-rw-rw-   0        0        0      147 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/options.py
+-rw-rw-rw-   0        0        0      137 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/order.py
+-rw-rw-rw-   0        0        0      157 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/order_canceled.py
+-rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/order_placed_temp.py
+-rw-rw-rw-   0        0        0      154 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/overnight_fee.py
+-rw-rw-rw-   0        0        0      141 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/position.py
+-rw-rw-rw-   0        0        0      636 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/position_changed.py
+-rw-rw-rw-   0        0        0      216 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/position_closed.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/position_history.py
+-rw-rw-rw-   0        0        0      144 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/positions.py
+-rw-rw-rw-   0        0        0     1092 2023-04-11 20:00:35.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/profile.py
+-rw-rw-rw-   0        0        0      151 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/result.py
+-rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/socket_option_closed.py
+-rw-rw-rw-   0        0        0      214 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/socket_option_opened.py
+-rw-rw-rw-   0        0        0      159 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/sold_options.py
+-rw-rw-rw-   0        0        0      148 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/strike_list.py
+-rw-rw-rw-   0        0        0      557 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/technical_indicators.py
+-rw-rw-rw-   0        0        0      164 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/time_sync.py
+-rw-rw-rw-   0        0        0      229 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/top_assets_updated.py
+-rw-rw-rw-   0        0        0      163 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/tpsl_changed.py
+-rw-rw-rw-   0        0        0      211 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/traders_mood_changed.py
+-rw-rw-rw-   0        0        0      212 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/training_balance_reset.py
+-rw-rw-rw-   0        0        0      174 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/underlying_list.py
+-rw-rw-rw-   0        0        0      179 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/user_profile_client.py
+-rw-rw-rw-   0        0        0      176 2023-04-11 06:56:48.000000 my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/users_availability.py
+drwxrwxrwx   0        0        0        0 2023-04-11 20:58:14.725509 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/
+-rw-rw-rw-   0        0        0      288 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5520 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 20:58:14.000000 my_iqoptionapi-7.1.2/my_iqoptionapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 20:58:14.990747 my_iqoptionapi-7.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-04-11 20:07:42.000000 my_iqoptionapi-7.1.2/setup.py
```

### Comparing `my-iqoptionapi-7.1.1/LICENCE` & `my_iqoptionapi-7.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/__init__.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/__init__.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/api.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,73 +4,73 @@
 import json
 import logging
 import threading
 import requests
 import ssl
 import atexit
 from collections import deque
-from iqoptionapi.http.login import Login
-from iqoptionapi.http.loginv2 import Loginv2
-from iqoptionapi.http.logout import Logout
-from iqoptionapi.http.login2fa import Login2FA
-from iqoptionapi.http.send_sms import SMS_Sender
-from iqoptionapi.http.verify import Verify
-from iqoptionapi.http.getprofile import Getprofile
-from iqoptionapi.http.auth import Auth
-from iqoptionapi.http.token import Token
-from iqoptionapi.http.appinit import Appinit
-from iqoptionapi.http.billing import Billing
-from iqoptionapi.http.buyback import Buyback
-from iqoptionapi.http.changebalance import Changebalance
-from iqoptionapi.http.events import Events
-from iqoptionapi.ws.client import WebsocketClient
-from iqoptionapi.ws.chanels.get_balances import *
-
-from iqoptionapi.ws.chanels.ssid import Ssid
-from iqoptionapi.ws.chanels.subscribe import *
-from iqoptionapi.ws.chanels.unsubscribe import *
-from iqoptionapi.ws.chanels.setactives import SetActives
-from iqoptionapi.ws.chanels.candles import GetCandles
-from iqoptionapi.ws.chanels.buyv2 import Buyv2
-from iqoptionapi.ws.chanels.buyv3 import *
-from iqoptionapi.ws.chanels.user import *
-from iqoptionapi.ws.chanels.api_game_betinfo import Game_betinfo
-from iqoptionapi.ws.chanels.instruments import Get_instruments
-from iqoptionapi.ws.chanels.get_financial_information import GetFinancialInformation
-from iqoptionapi.ws.chanels.strike_list import Strike_list
-from iqoptionapi.ws.chanels.leaderboard import Leader_Board
-
-from iqoptionapi.ws.chanels.traders_mood import Traders_mood_subscribe
-from iqoptionapi.ws.chanels.traders_mood import Traders_mood_unsubscribe
-from iqoptionapi.ws.chanels.technical_indicators import Technical_indicators
-from iqoptionapi.ws.chanels.buy_place_order_temp import Buy_place_order_temp
-from iqoptionapi.ws.chanels.get_order import Get_order
-from iqoptionapi.ws.chanels.get_deferred_orders import GetDeferredOrders
-from iqoptionapi.ws.chanels.get_positions import *
-
-from iqoptionapi.ws.chanels.get_available_leverages import Get_available_leverages
-from iqoptionapi.ws.chanels.cancel_order import Cancel_order
-from iqoptionapi.ws.chanels.close_position import Close_position
-from iqoptionapi.ws.chanels.get_overnight_fee import Get_overnight_fee
-from iqoptionapi.ws.chanels.heartbeat import Heartbeat
-
-
-from iqoptionapi.ws.chanels.digital_option import *
-from iqoptionapi.ws.chanels.api_game_getoptions import *
-from iqoptionapi.ws.chanels.sell_option import Sell_Option
-from iqoptionapi.ws.chanels.sell_digital_option import Sell_Digital_Option
-from iqoptionapi.ws.chanels.change_tpsl import Change_Tpsl
-from iqoptionapi.ws.chanels.change_auto_margin_call import ChangeAutoMarginCall
-
-from iqoptionapi.ws.objects.timesync import TimeSync
-from iqoptionapi.ws.objects.profile import Profile
-from iqoptionapi.ws.objects.candles import Candles
-from iqoptionapi.ws.objects.listinfodata import ListInfoData
-from iqoptionapi.ws.objects.betinfo import Game_betinfo_data
-import iqoptionapi.global_value as global_value
+from my_iqoptionapi.http.login import Login
+from my_iqoptionapi.http.loginv2 import Loginv2
+from my_iqoptionapi.http.logout import Logout
+from my_iqoptionapi.http.login2fa import Login2FA
+from my_iqoptionapi.http.send_sms import SMS_Sender
+from my_iqoptionapi.http.verify import Verify
+from my_iqoptionapi.http.getprofile import Getprofile
+from my_iqoptionapi.http.auth import Auth
+from my_iqoptionapi.http.token import Token
+from my_iqoptionapi.http.appinit import Appinit
+from my_iqoptionapi.http.billing import Billing
+from my_iqoptionapi.http.buyback import Buyback
+from my_iqoptionapi.http.changebalance import Changebalance
+from my_iqoptionapi.http.events import Events
+from my_iqoptionapi.ws.client import WebsocketClient
+from my_iqoptionapi.ws.chanels.get_balances import *
+
+from my_iqoptionapi.ws.chanels.ssid import Ssid
+from my_iqoptionapi.ws.chanels.subscribe import *
+from my_iqoptionapi.ws.chanels.unsubscribe import *
+from my_iqoptionapi.ws.chanels.setactives import SetActives
+from my_iqoptionapi.ws.chanels.candles import GetCandles
+from my_iqoptionapi.ws.chanels.buyv2 import Buyv2
+from my_iqoptionapi.ws.chanels.buyv3 import *
+from my_iqoptionapi.ws.chanels.user import *
+from my_iqoptionapi.ws.chanels.api_game_betinfo import Game_betinfo
+from my_iqoptionapi.ws.chanels.instruments import Get_instruments
+from my_iqoptionapi.ws.chanels.get_financial_information import GetFinancialInformation
+from my_iqoptionapi.ws.chanels.strike_list import Strike_list
+from my_iqoptionapi.ws.chanels.leaderboard import Leader_Board
+
+from my_iqoptionapi.ws.chanels.traders_mood import Traders_mood_subscribe
+from my_iqoptionapi.ws.chanels.traders_mood import Traders_mood_unsubscribe
+from my_iqoptionapi.ws.chanels.technical_indicators import Technical_indicators
+from my_iqoptionapi.ws.chanels.buy_place_order_temp import Buy_place_order_temp
+from my_iqoptionapi.ws.chanels.get_order import Get_order
+from my_iqoptionapi.ws.chanels.get_deferred_orders import GetDeferredOrders
+from my_iqoptionapi.ws.chanels.get_positions import *
+
+from my_iqoptionapi.ws.chanels.get_available_leverages import Get_available_leverages
+from my_iqoptionapi.ws.chanels.cancel_order import Cancel_order
+from my_iqoptionapi.ws.chanels.close_position import Close_position
+from my_iqoptionapi.ws.chanels.get_overnight_fee import Get_overnight_fee
+from my_iqoptionapi.ws.chanels.heartbeat import Heartbeat
+
+
+from my_iqoptionapi.ws.chanels.digital_option import *
+from my_iqoptionapi.ws.chanels.api_game_getoptions import *
+from my_iqoptionapi.ws.chanels.sell_option import Sell_Option
+from my_iqoptionapi.ws.chanels.sell_digital_option import Sell_Digital_Option
+from my_iqoptionapi.ws.chanels.change_tpsl import Change_Tpsl
+from my_iqoptionapi.ws.chanels.change_auto_margin_call import ChangeAutoMarginCall
+
+from my_iqoptionapi.ws.objects.timesync import TimeSync
+from my_iqoptionapi.ws.objects.profile import Profile
+from my_iqoptionapi.ws.objects.candles import Candles
+from my_iqoptionapi.ws.objects.listinfodata import ListInfoData
+from my_iqoptionapi.ws.objects.betinfo import Game_betinfo_data
+import my_iqoptionapi.global_value as global_value
 from collections import defaultdict
 
 
 def nested_dict(n, type):
     if n == 1:
         return defaultdict(type)
     else:
@@ -179,25 +179,25 @@
         self.buy_successful = None
         self.__active_account_type = None
 
     def prepare_http_url(self, resource):
         """Construct http url from resource url.
 
         :param resource: The instance of
-            :class:`Resource <iqoptionapi.http.resource.Resource>`.
+            :class:`Resource <my_iqoptionapi.http.resource.Resource>`.
 
         :returns: The full url to IQ Option http resource.
         """
         return "/".join((self.https_url, resource.url))
 
     def send_http_request(self, resource, method, data=None, params=None, headers=None):  # pylint: disable=too-many-arguments
         """Send http request to IQ Option server.
 
         :param resource: The instance of
-            :class:`Resource <iqoptionapi.http.resource.Resource>`.
+            :class:`Resource <my_iqoptionapi.http.resource.Resource>`.
         :param str method: The http request method.
         :param dict data: (optional) The http request data.
         :param dict params: (optional) The http request params.
         :param dict headers: (optional) The http request headers.
 
         :returns: The instance of :class:`Response <requests.Response>`.
         """
@@ -220,15 +220,15 @@
         response.raise_for_status()
         return response
 
     def send_http_request_v2(self, url, method, data=None, params=None, headers=None):  # pylint: disable=too-many-arguments
         """Send http request to IQ Option server.
 
         :param resource: The instance of
-            :class:`Resource <iqoptionapi.http.resource.Resource>`.
+            :class:`Resource <my_iqoptionapi.http.resource.Resource>`.
         :param str method: The http request method.
         :param dict data: (optional) The http request data.
         :param dict params: (optional) The http request params.
         :param dict headers: (optional) The http request headers.
 
         :returns: The instance of :class:`Response <requests.Response>`.
         """
@@ -279,153 +279,153 @@
         global_value.ssl_Mutual_exclusion_write = False
 
     @property
     def logout(self):
         """Property for get IQ Option http login resource.
 
         :returns: The instance of :class:`Login
-            <iqoptionapi.http.login.Login>`.
+            <my_iqoptionapi.http.login.Login>`.
         """
         return Logout(self)
 
     @property
     def login(self):
         """Property for get IQ Option http login resource.
 
         :returns: The instance of :class:`Login
-            <iqoptionapi.http.login.Login>`.
+            <my_iqoptionapi.http.login.Login>`.
         """
         return Login(self)
 
     @property
     def login_2fa(self):
         """Property for get IQ Option http login 2FA resource.
 
         :returns: The instance of :class:`Login2FA
-            <iqoptionapi.http.login2fa.Login2FA>`.
+            <my_iqoptionapi.http.login2fa.Login2FA>`.
         """
         return Login2FA(self)
 
     @property
     def send_sms_code(self):
         """Property for get IQ Option http send sms code resource.
 
         :returns: The instance of :class:`SMS_Sender
-            <iqoptionapi.http.send_sms.SMS_Sender>`.
+            <my_iqoptionapi.http.send_sms.SMS_Sender>`.
         """
         return SMS_Sender(self)
 
     @property
     def verify_2fa(self):
         """Property for get IQ Option http verify 2fa resource.
 
         :returns: The instance of :class:`Verify
-            <iqoptionapi.http.verify.Verify>`.
+            <my_iqoptionapi.http.verify.Verify>`.
         """
         return Verify(self)
 
     @property
     def loginv2(self):
         """Property for get IQ Option http loginv2 resource.
 
         :returns: The instance of :class:`Loginv2
-            <iqoptionapi.http.loginv2.Loginv2>`.
+            <my_iqoptionapi.http.loginv2.Loginv2>`.
         """
         return Loginv2(self)
 
     @property
     def auth(self):
         """Property for get IQ Option http auth resource.
 
         :returns: The instance of :class:`Auth
-            <iqoptionapi.http.auth.Auth>`.
+            <my_iqoptionapi.http.auth.Auth>`.
         """
         return Auth(self)
 
     @property
     def appinit(self):
         """Property for get IQ Option http appinit resource.
 
         :returns: The instance of :class:`Appinit
-            <iqoptionapi.http.appinit.Appinit>`.
+            <my_iqoptionapi.http.appinit.Appinit>`.
         """
         return Appinit(self)
 
     @property
     def token(self):
         """Property for get IQ Option http token resource.
 
         :returns: The instance of :class:`Token
-            <iqoptionapi.http.auth.Token>`.
+            <my_iqoptionapi.http.auth.Token>`.
         """
         return Token(self)
 
     # @property
     # def profile(self):
     #     """Property for get IQ Option http profile resource.
 
     #     :returns: The instance of :class:`Profile
-    #         <iqoptionapi.http.profile.Profile>`.
+    #         <my_iqoptionapi.http.profile.Profile>`.
     #     """
     #     return Profile(self)
     def reset_training_balance(self):
         # sendResults True/False
         # {"name":"sendMessage","request_id":"142","msg":{"name":"reset-training-balance","version":"2.0"}}
 
         self.send_websocket_request(name="sendMessage", msg={"name": "reset-training-balance",
                                                              "version": "2.0"})
 
     @property
     def changebalance(self):
         """Property for get IQ Option http changebalance resource.
 
         :returns: The instance of :class:`Changebalance
-            <iqoptionapi.http.changebalance.Changebalance>`.
+            <my_iqoptionapi.http.changebalance.Changebalance>`.
         """
         return Changebalance(self)
 
     @property
     def events(self):
         return Events(self)
 
     @property
     def billing(self):
         """Property for get IQ Option http billing resource.
 
         :returns: The instance of :class:`Billing
-            <iqoptionapi.http.billing.Billing>`.
+            <my_iqoptionapi.http.billing.Billing>`.
         """
         return Billing(self)
 
     @property
     def buyback(self):
         """Property for get IQ Option http buyback resource.
 
         :returns: The instance of :class:`Buyback
-            <iqoptionapi.http.buyback.Buyback>`.
+            <my_iqoptionapi.http.buyback.Buyback>`.
         """
         return Buyback(self)
 # ------------------------------------------------------------------------
 
     @property
     def getprofile(self):
         """Property for get IQ Option http getprofile resource.
 
         :returns: The instance of :class:`Login
-            <iqoptionapi.http.getprofile.Getprofile>`.
+            <my_iqoptionapi.http.getprofile.Getprofile>`.
         """
         return Getprofile(self)
 # for active code ...
 
     @property
     def get_balances(self):
         """Property for get IQ Option http getprofile resource.
 
         :returns: The instance of :class:`Login
-            <iqoptionapi.http.getprofile.Getprofile>`.
+            <my_iqoptionapi.http.getprofile.Getprofile>`.
         """
         return Get_Balances(self)
 
     @property
     def get_instruments(self):
         return Get_instruments(self)
 
@@ -435,15 +435,15 @@
 # ----------------------------------------------------------------------------
 
     @property
     def ssid(self):
         """Property for get IQ Option websocket ssid chanel.
 
         :returns: The instance of :class:`Ssid
-            <iqoptionapi.ws.chanels.ssid.Ssid>`.
+            <my_iqoptionapi.ws.chanels.ssid.Ssid>`.
         """
         return Ssid(self)
 # --------------------------------------------------------------------------------
 
     @property
     def Subscribe_Live_Deal(self):
         return Subscribe_live_deal(self)
@@ -474,28 +474,28 @@
 # --------------------------------------------------------------------------------
     @property
     def subscribe(self):
         "candle-generated"
         """Property for get IQ Option websocket subscribe chanel.
 
         :returns: The instance of :class:`Subscribe
-            <iqoptionapi.ws.chanels.subscribe.Subscribe>`.
+            <my_iqoptionapi.ws.chanels.subscribe.Subscribe>`.
         """
         return Subscribe(self)
 
     @property
     def subscribe_all_size(self):
         return Subscribe_candles(self)
 
     @property
     def unsubscribe(self):
         """Property for get IQ Option websocket unsubscribe chanel.
 
         :returns: The instance of :class:`Unsubscribe
-            <iqoptionapi.ws.chanels.unsubscribe.Unsubscribe>`.
+            <my_iqoptionapi.ws.chanels.unsubscribe.Unsubscribe>`.
         """
         return Unsubscribe(self)
 
     @property
     def unsubscribe_all_size(self):
         return Unsubscribe_candles(self)
 
@@ -599,28 +599,28 @@
 # -----------------------------------------------------------------------------------
 
     @property
     def setactives(self):
         """Property for get IQ Option websocket setactives chanel.
 
         :returns: The instance of :class:`SetActives
-            <iqoptionapi.ws.chanels.setactives.SetActives>`.
+            <my_iqoptionapi.ws.chanels.setactives.SetActives>`.
         """
         return SetActives(self)
 
     @property
     def Get_Leader_Board(self):
         return Leader_Board(self)
 
     @property
     def getcandles(self):
         """Property for get IQ Option websocket candles chanel.
 
         :returns: The instance of :class:`GetCandles
-            <iqoptionapi.ws.chanels.candles.GetCandles>`.
+            <my_iqoptionapi.ws.chanels.candles.GetCandles>`.
         """
         return GetCandles(self)
 
     def get_api_option_init_all(self):
         self.send_websocket_request(name="api_option_init_all", msg="")
 
     def get_api_option_init_all_v2(self):
@@ -655,15 +655,15 @@
         return Buyv3_by_raw_expired(self)
 
     @property
     def buy(self):
         """Property for get IQ Option websocket buyv2 request.
 
         :returns: The instance of :class:`Buyv2
-            <iqoptionapi.ws.chanels.buyv2.Buyv2>`.
+            <my_iqoptionapi.ws.chanels.buyv2.Buyv2>`.
         """
         self.buy_successful = None
         return Buyv2(self)
 
     @property
     def sell_option(self):
         return Sell_Option(self)
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/constants.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/constants.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/country_id.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/country_id.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/expiration.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/expiration.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/appinit.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/appinit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ option appinit http resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 
 
 class Appinit(Resource):
     """Class for IQ option login resource."""
     # pylint: disable=too-few-public-methods
 
     url = "appinit"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/buyback.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/buyback.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for IQ option buyback resource."""
 
-from iqoptionapi.http.resource import Resource
-from iqoptionapi.http.billing import Billing
+from my_iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.billing import Billing
 
 
 class Buyback(Resource):
     """Class for IQ option buyback resource."""
     # pylint: disable=too-few-public-methods
 
     url = "/".join((Billing.url, "buyback"))
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/changebalance.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/changebalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for IQ option changebalance resource."""
 
-from iqoptionapi.http.resource import Resource
-from iqoptionapi.http.profile import Profile
+from my_iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.profile import Profile
 
 
 class Changebalance(Resource):
     """Class for IQ option changebalance resource."""
     # pylint: disable=too-few-public-methods
 
     url = "/".join((Profile.url, "changebalance"))
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/events.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http login resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 
 
 class Events(Resource):
     """Class for IQ option login resource."""
     # pylint: disable=too-few-public-methods
 
     url = ""
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/getprofile.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/getprofile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http getprofile resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 
 
 class Getprofile(Resource):
     """Class for IQ option getprofile resource."""
     # pylint: disable=too-few-public-methods
 
     url = "getprofile"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/getregdata.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/getregdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for IQ Option http getregdata resource."""
 
-from iqoptionapi.http.resource import Resource
-from iqoptionapi.http.register import Register
+from my_iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.register import Register
 
 
 class Getprofile(Resource):
     """Class for IQ option getregdata resource."""
     # pylint: disable=too-few-public-methods
 
     url = "/".join((Register.url, "getregdata"))
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/login.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http login resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 
 
 class Login(Resource):
     """Class for IQ option login resource."""
     # pylint: disable=too-few-public-methods
 
     url = ""
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/login2fa.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/login2fa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http login resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 
 
 class Login2FA(Resource):
     """Class for IQ option login resource."""
     # pylint: disable=too-few-public-methods
 
     url = ""
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/logout.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/token.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-"""Module for IQ Option http login resource."""
+"""Module for IQ Option http token resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.auth import Auth
 
 
-class Logout(Resource):
-    """Class for IQ option login resource."""
+class Token(Resource):
+    """Class for IQ Option http token resource."""
     # pylint: disable=too-few-public-methods
 
-    url = ""
+    url = "/".join((Auth.url, "token"))
 
-    def _post(self, data=None, headers=None):
-        """Send get request for IQ Option API login http resource.
+    def __init__(self, api):
+        super(Token, self).__init__(api)
+
+    def _get(self):
+        """Send get request for IQ Option API token http resource.
 
         :returns: The instance of :class:`requests.Response`.
         """
-        return self.api.send_http_request_v2(method="POST", url="https://auth.iqoption.com/api/v1.0/logout",data=data, headers=headers)
+        return self.send_http_request("GET")
 
     def __call__(self):
-       
-        return self._post()
+        """Method to get IQ Option API token http request.
 
+        :returns: The instance of :class:`requests.Response`.
+        """
+        return self._get()
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/resource.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Resource(object):
     """Class for base IQ Option API http resource."""
     # pylint: disable=too-few-public-methods
 
     def __init__(self, api):
         """
         :param api: The instance of :class:`IQOptionAPI
-            <iqoptionapi.api.IQOptionAPI>`.
+            <my_iqoptionapi.api.IQOptionAPI>`.
         """
         self.api = api
 
     def send_http_request(self, method, data=None, params=None, headers=None):
         """Send http request to IQ Option API.
 
         :param str method: The http request method.
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/send_sms.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/send_sms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http sms resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 import json
 
 
 class SMS_Sender(Resource):
     """Class for IQ option sms resource."""
     # pylint: disable=too-few-public-methods
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/http/verify.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/http/verify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option http verify resource."""
 
-from iqoptionapi.http.resource import Resource
+from my_iqoptionapi.http.resource import Resource
 import json
 
 
 class Verify(Resource):
     """Class for IQ option verify resource."""
     # pylint: disable=too-few-public-methods
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/stable_api.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/stable_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # python
-from iqoptionapi.api import IQOptionAPI
-import iqoptionapi.constants as OP_code
-import iqoptionapi.country_id as Country
+from my_iqoptionapi.api import IQOptionAPI
+import my_iqoptionapi.constants as OP_code
+import my_iqoptionapi.country_id as Country
 import threading
 import time
 import json
 import logging
 import operator
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.global_value as global_value
 from collections import defaultdict
 from collections import deque
-from iqoptionapi.expiration import get_expiration_time, get_remaning_time
-from iqoptionapi.version_control import api_version
+from my_iqoptionapi.expiration import get_expiration_time, get_remaning_time
+from my_iqoptionapi.version_control import api_version
 from datetime import datetime, timedelta
 from random import randint
 
 
 def nested_dict(n, type):
     if n == 1:
         return defaultdict(type)
@@ -768,15 +768,15 @@
 
                     return data["result"]["data"][str(id_number)]["profit"] - data["result"]["data"][str(id_number)][
                         "deposit"]
                 except:
                     pass
             time.sleep(polling_time)
 
-        # Function by kkagill ( https://github.com/Lu-Yi-Hsun/iqoptionapi/issues/196 | https://github.com/kkagill )
+        # Function by kkagill ( https://github.com/Lu-Yi-Hsun/my_iqoptionapi/issues/196 | https://github.com/kkagill )
         # Function only work with Options!
 
     def check_win_v4(self, id_number):
         while True:
             try:
                 if self.api.socket_option_closed[id_number] != None:
                     break
@@ -1027,15 +1027,15 @@
         profit = self.api.instrument_quites_generated_data[ACTIVE][duration * 60]
         for key in profit:
             if key.find("SPT") != -1:
                 return profit[key]
         return False
 
     # thank thiagottjv
-    # https://github.com/Lu-Yi-Hsun/iqoptionapi/issues/65#issuecomment-513998357
+    # https://github.com/Lu-Yi-Hsun/my_iqoptionapi/issues/65#issuecomment-513998357
 
     def buy_digital_spot(self, active, amount, action, duration):
         # Expiration time need to be formatted like this: YYYYMMDDHHII
         # And need to be on GMT time
 
         # Type - P or C
         action = action.lower()
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/api_game_betinfo.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/api_game_betinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import logging
 class Game_betinfo(Base):
     name = "api_game_betinfo"
     def __call__(self, id_number_list):
         data = {"currency": "USD"}
         if type(id_number_list) is list:
             for idx, val in enumerate(id_number_list):
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/api_game_getoptions.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/api_game_getoptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #python
 """Module for IQ option candles websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.global_value as global_value
 class Get_options(Base):
 
     name = "api_game_getoptions"
 
     def __call__(self,limit):
     
         data = {"limit":int(limit),
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/base.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Base(object):
     """Class for base IQ Option websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     def __init__(self, api):
         """
         :param api: The instance of :class:`IQOptionAPI
-            <iqoptionapi.api.IQOptionAPI>`.
+            <my_iqoptionapi.api.IQOptionAPI>`.
         """
         self.api = api
 
     def send_websocket_request(self, name, msg,request_id=""):
         """Send request to IQ Option server websocket.
 
         :param str name: The websocket chanel name.
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buy_place_order_temp.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buy_place_order_temp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
-import iqoptionapi.global_value as global_value
+from my_iqoptionapi.ws.chanels.base import Base
+import my_iqoptionapi.global_value as global_value
 #work for forex digit cfd(stock)
 
 class Buy_place_order_temp(Base):
     name = "sendMessage"
     def __call__(self,
                 instrument_type,instrument_id,
                 side,amount,leverage,
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buyv2.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buyv2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for IQ Option buyV2 websocket chanel."""
 from datetime import datetime, timedelta
-import iqoptionapi.global_value as global_value
-from iqoptionapi.ws.chanels.base import Base
-from iqoptionapi.expiration import get_expiration_time
+import my_iqoptionapi.global_value as global_value
+from my_iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.expiration import get_expiration_time
 
 
 class Buyv2(Base):
     """Class for IQ option buy websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "sendMessage"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/buyv3.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/buyv3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import logging
-import iqoptionapi.global_value as global_value
-from iqoptionapi.expiration import get_expiration_time
+import my_iqoptionapi.global_value as global_value
+from my_iqoptionapi.expiration import get_expiration_time
 
 
 class Buyv3(Base):
 
     name = "sendMessage"
 
     def __call__(self, price, active, direction, duration, request_id):
 
         # thank Darth-Carrotpie's code
-        # https://github.com/Lu-Yi-Hsun/iqoptionapi/issues/6
+        # https://github.com/Lu-Yi-Hsun/my_iqoptionapi/issues/6
         exp, idx = get_expiration_time(
             int(self.api.timesync.server_timestamp), duration)
         if idx < 5:
             option = 3  # "turbo"
         else:
             option = 1  # "binary"
         data = {
@@ -37,15 +37,15 @@
 class Buyv3_by_raw_expired(Base):
 
     name = "sendMessage"
 
     def __call__(self, price, active, direction, option, expired, request_id):
 
         # thank Darth-Carrotpie's code
-        # https://github.com/Lu-Yi-Hsun/iqoptionapi/issues/6
+        # https://github.com/Lu-Yi-Hsun/my_iqoptionapi/issues/6
 
         if option == "turbo":
             option_id = 3  # "turbo"
         elif option == "binary":
             option_id = 1  # "binary"
         data = {
             "body": {"price": price,
@@ -59,15 +59,15 @@
             "version": "1.0"
         }
         self.send_websocket_request(self.name, data, str(request_id))
 
 
 """
     # thank Darth-Carrotpie's code
-    # https://github.com/Lu-Yi-Hsun/iqoptionapi/issues/6
+    # https://github.com/Lu-Yi-Hsun/my_iqoptionapi/issues/6
     def get_expiration_time(self, duration):
         exp = time.time()
         if duration >= 1 and duration <= 5:
             option = 3#"turbo"
             # Round to next full minute
             # datetime.datetime.now().second>30
             if (exp % 60) > 30:
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/candles.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/candles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ option candles websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
 
 class GetCandles(Base):
     """Class for IQ option candles websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "sendMessage"
@@ -13,15 +13,15 @@
         """Method to send message to candles websocket chanel.
 
         :param active_id: The active/asset identifier.
         :param duration: The candle duration (timeframe for the candles).
         :param amount: The number of candles you want to have
         """
         #thank SeanStayn share new request
-        #https://github.com/n1nj4z33/iqoptionapi/issues/88
+        #https://github.com/n1nj4z33/my_iqoptionapi/issues/88
         data = {"name":"get-candles",
                 "version":"2.0",
                 "body":{
                         "active_id":int(active_id),
                         "split_normalization": True,
                         "size":interval,#time size sample:if interval set 1 mean get time 0~1 candle 
                         "to":int(endtime),   #int(self.api.timesync.server_timestamp),
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/change_tpsl.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/change_tpsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #python
 
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 class Change_Tpsl(Base):
     name = "sendMessage"
     def __call__(self,ID_Name,ID,
                 stop_lose_kind,stop_lose_value,
                 take_profit_kind,take_profit_value,
                 use_trail_stop):
         data = {
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/changebalance.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/changebalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for IQ Option buyV2 websocket chanel."""
 import datetime
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 class Changebalance(Base):
     """Class for IQ option buy websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "api_profile_changebalance"
 
     def __call__(self, balance_id):
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/digital_option.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/digital_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # python
 
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
-import iqoptionapi.global_value as global_value
+from my_iqoptionapi.ws.chanels.base import Base
+import my_iqoptionapi.global_value as global_value
 from random import randint
 # work for forex digit cfd(stock)
 
 
 class Digital_options_place_digital_option(Base):
     name = "sendMessage"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_deferred_orders.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_deferred_orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.global_value as global_value
 class GetDeferredOrders(Base):
     
     name = "sendMessage"
 
     def __call__(self,instrument_type):
      
         data = {"name":"get-deferred-orders",
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_financial_information.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_financial_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 class GetFinancialInformation(Base):
     name = "sendMessage"
     def __call__(self,activeId):
         data = {
             "name":"get-financial-information",
             "version":"1.0",
             "body":{
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_overnight_fee.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_overnight_fee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 
 
 class Get_overnight_fee(Base):
     name = "sendMessage"
     def __call__(self,instrument_type,active_id):
         data = {
             "name":"get-overnight-fee",
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/get_positions.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/get_positions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
-import iqoptionapi.global_value as global_value
+from my_iqoptionapi.ws.chanels.base import Base
+import my_iqoptionapi.global_value as global_value
 
 class Get_positions(Base):
     name = "sendMessage"
     def __call__(self,instrument_type):
         if instrument_type=="digital-option":
             name="digital-options.get-positions"
         elif instrument_type=="fx-option":
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/leaderboard.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/leaderboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
  
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
 """
 {"name":"sendMessage","request_id":"356","msg":{"name":"request-leaderboard-deals-client","version":"1.0","body":{"country_id":0,"user_country_id":191,"from_position":1,"to_position":64,"near_traders_country_count":64,"near_traders_count":64,"top_country_count":64,"top_count":64,"top_type":2}}}
 """
 class Leader_Board(Base):
     name = "sendMessage"
     def __call__(self, country_id,user_country_id,from_position,to_position,near_traders_country_count,near_traders_count,top_country_count,top_count,top_type):
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/sell_digital_option.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/sell_digital_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
  
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
 
 class Sell_Digital_Option(Base):
     name = "sendMessage"
     def __call__(self, position_ids):
         """ 
         :param options_ids: list or int
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/sell_option.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/sell_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
  
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import time
 
 class Sell_Option(Base):
     name = "sendMessage"
     def __call__(self, options_ids):
         """ 
         :param options_ids: list or int
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/setactives.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/setactives.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ option setactives websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 
 
 class SetActives(Base):
     """Class for IQ option setactives websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "setActives"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/strike_list.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/strike_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import logging
 class Strike_list(Base):
     name = "sendMessage"
     
     def __call__(self,name,duration):  
         """
         duration:minute
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/subscribe.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/subscribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for IQ option subscribe websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import datetime
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 
 class Subscribe(Base):
     """Class for IQ option candles websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "subscribeMessage"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/technical_indicators.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/technical_indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 
 
 class Technical_indicators(Base):
     name = "sendMessage"
 
     def __call__(self, active):
         data = {
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/traders_mood.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/traders_mood.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import time
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 
 
 class Traders_mood_subscribe(Base):
     name = "subscribeMessage"
 
     def __call__(self, active, instrument="turbo-option"):
         data = {
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/unsubscribe.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/unsubscribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for IQ option unsubscribe websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import datetime
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 
 class Unsubscribe(Base):
     """Class for IQ option candles websocket chanel."""
     # pylint: disable=too-few-public-methods
 
     name = "unsubscribeMessage"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/chanels/user.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/chanels/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for IQ option unsubscribe websocket chanel."""
 
-from iqoptionapi.ws.chanels.base import Base
+from my_iqoptionapi.ws.chanels.base import Base
 import datetime
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 
 class Get_user_profile_client(Base):
    
     name = "sendMessage"
 
     def __call__(self, user_id):
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/client.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 """Module for IQ option websocket."""
 
 import json
 import logging
 import websocket
-import iqoptionapi.constants as OP_code
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.constants as OP_code
+import my_iqoptionapi.global_value as global_value
 from threading import Thread
-from iqoptionapi.ws.received.technical_indicators import technical_indicators
-from iqoptionapi.ws.received.time_sync import time_sync
-from iqoptionapi.ws.received.heartbeat import heartbeat
-from iqoptionapi.ws.received.balances import balances
-from iqoptionapi.ws.received.profile import profile
-from iqoptionapi.ws.received.balance_changed import balance_changed
-from iqoptionapi.ws.received.candles import candles
-from iqoptionapi.ws.received.buy_complete import buy_complete
-from iqoptionapi.ws.received.option import option
-from iqoptionapi.ws.received.position_history import position_history
-from iqoptionapi.ws.received.list_info_data import list_info_data
-from iqoptionapi.ws.received.candle_generated import candle_generated_realtime
-from iqoptionapi.ws.received.candle_generated_v2 import candle_generated_v2
-from iqoptionapi.ws.received.commission_changed import commission_changed
-from iqoptionapi.ws.received.socket_option_opened import socket_option_opened
-from iqoptionapi.ws.received.api_option_init_all_result import api_option_init_all_result
-from iqoptionapi.ws.received.initialization_data import initialization_data
-from iqoptionapi.ws.received.underlying_list import underlying_list
-from iqoptionapi.ws.received.instruments import instruments
-from iqoptionapi.ws.received.financial_information import financial_information
-from iqoptionapi.ws.received.position_changed import position_changed
-from iqoptionapi.ws.received.option_opened import option_opened
-from iqoptionapi.ws.received.option_closed import option_closed
-from iqoptionapi.ws.received.top_assets_updated import top_assets_updated
-from iqoptionapi.ws.received.strike_list import strike_list
-from iqoptionapi.ws.received.api_game_betinfo_result import api_game_betinfo_result
-from iqoptionapi.ws.received.traders_mood_changed import traders_mood_changed
-from iqoptionapi.ws.received.order import order
-from iqoptionapi.ws.received.position import position
-from iqoptionapi.ws.received.positions import positions
-from iqoptionapi.ws.received.order_placed_temp import order_placed_temp
-from iqoptionapi.ws.received.deferred_orders import deferred_orders
-from iqoptionapi.ws.received.history_positions import history_positions
-from iqoptionapi.ws.received.available_leverages import available_leverages
-from iqoptionapi.ws.received.order_canceled import order_canceled
-from iqoptionapi.ws.received.position_closed import position_closed
-from iqoptionapi.ws.received.overnight_fee import overnight_fee
-from iqoptionapi.ws.received.api_game_getoptions_result import api_game_getoptions_result
-from iqoptionapi.ws.received.sold_options import sold_options
-from iqoptionapi.ws.received.tpsl_changed import tpsl_changed
-from iqoptionapi.ws.received.auto_margin_call_changed import auto_margin_call_changed
-from iqoptionapi.ws.received.digital_option_placed import digital_option_placed
-from iqoptionapi.ws.received.result import result
-from iqoptionapi.ws.received.instrument_quotes_generated import instrument_quotes_generated
-from iqoptionapi.ws.received.training_balance_reset import training_balance_reset
-from iqoptionapi.ws.received.socket_option_closed import socket_option_closed
-from iqoptionapi.ws.received.live_deal_binary_option_placed import live_deal_binary_option_placed
-from iqoptionapi.ws.received.live_deal_digital_option import live_deal_digital_option
-from iqoptionapi.ws.received.leaderboard_deals_client import leaderboard_deals_client
-from iqoptionapi.ws.received.live_deal import live_deal
-from iqoptionapi.ws.received.user_profile_client import user_profile_client
-from iqoptionapi.ws.received.leaderboard_userinfo_deals_client import leaderboard_userinfo_deals_client
-from iqoptionapi.ws.received.client_price_generated import client_price_generated
-from iqoptionapi.ws.received.users_availability import users_availability
+from my_iqoptionapi.ws.received.technical_indicators import technical_indicators
+from my_iqoptionapi.ws.received.time_sync import time_sync
+from my_iqoptionapi.ws.received.heartbeat import heartbeat
+from my_iqoptionapi.ws.received.balances import balances
+from my_iqoptionapi.ws.received.profile import profile
+from my_iqoptionapi.ws.received.balance_changed import balance_changed
+from my_iqoptionapi.ws.received.candles import candles
+from my_iqoptionapi.ws.received.buy_complete import buy_complete
+from my_iqoptionapi.ws.received.option import option
+from my_iqoptionapi.ws.received.position_history import position_history
+from my_iqoptionapi.ws.received.list_info_data import list_info_data
+from my_iqoptionapi.ws.received.candle_generated import candle_generated_realtime
+from my_iqoptionapi.ws.received.candle_generated_v2 import candle_generated_v2
+from my_iqoptionapi.ws.received.commission_changed import commission_changed
+from my_iqoptionapi.ws.received.socket_option_opened import socket_option_opened
+from my_iqoptionapi.ws.received.api_option_init_all_result import api_option_init_all_result
+from my_iqoptionapi.ws.received.initialization_data import initialization_data
+from my_iqoptionapi.ws.received.underlying_list import underlying_list
+from my_iqoptionapi.ws.received.instruments import instruments
+from my_iqoptionapi.ws.received.financial_information import financial_information
+from my_iqoptionapi.ws.received.position_changed import position_changed
+from my_iqoptionapi.ws.received.option_opened import option_opened
+from my_iqoptionapi.ws.received.option_closed import option_closed
+from my_iqoptionapi.ws.received.top_assets_updated import top_assets_updated
+from my_iqoptionapi.ws.received.strike_list import strike_list
+from my_iqoptionapi.ws.received.api_game_betinfo_result import api_game_betinfo_result
+from my_iqoptionapi.ws.received.traders_mood_changed import traders_mood_changed
+from my_iqoptionapi.ws.received.order import order
+from my_iqoptionapi.ws.received.position import position
+from my_iqoptionapi.ws.received.positions import positions
+from my_iqoptionapi.ws.received.order_placed_temp import order_placed_temp
+from my_iqoptionapi.ws.received.deferred_orders import deferred_orders
+from my_iqoptionapi.ws.received.history_positions import history_positions
+from my_iqoptionapi.ws.received.available_leverages import available_leverages
+from my_iqoptionapi.ws.received.order_canceled import order_canceled
+from my_iqoptionapi.ws.received.position_closed import position_closed
+from my_iqoptionapi.ws.received.overnight_fee import overnight_fee
+from my_iqoptionapi.ws.received.api_game_getoptions_result import api_game_getoptions_result
+from my_iqoptionapi.ws.received.sold_options import sold_options
+from my_iqoptionapi.ws.received.tpsl_changed import tpsl_changed
+from my_iqoptionapi.ws.received.auto_margin_call_changed import auto_margin_call_changed
+from my_iqoptionapi.ws.received.digital_option_placed import digital_option_placed
+from my_iqoptionapi.ws.received.result import result
+from my_iqoptionapi.ws.received.instrument_quotes_generated import instrument_quotes_generated
+from my_iqoptionapi.ws.received.training_balance_reset import training_balance_reset
+from my_iqoptionapi.ws.received.socket_option_closed import socket_option_closed
+from my_iqoptionapi.ws.received.live_deal_binary_option_placed import live_deal_binary_option_placed
+from my_iqoptionapi.ws.received.live_deal_digital_option import live_deal_digital_option
+from my_iqoptionapi.ws.received.leaderboard_deals_client import leaderboard_deals_client
+from my_iqoptionapi.ws.received.live_deal import live_deal
+from my_iqoptionapi.ws.received.user_profile_client import user_profile_client
+from my_iqoptionapi.ws.received.leaderboard_userinfo_deals_client import leaderboard_userinfo_deals_client
+from my_iqoptionapi.ws.received.client_price_generated import client_price_generated
+from my_iqoptionapi.ws.received.users_availability import users_availability
 
 
 class WebsocketClient(object):
     """Class for work with IQ option websocket."""
 
     def __init__(self, api):
         """
         :param api: The instance of :class:`IQOptionAPI
-            <iqoptionapi.api.IQOptionAPI>`.
+            <my_iqoptionapi.api.IQOptionAPI>`.
         """
         self.api = api
         self.wss = websocket.WebSocketApp(
             self.api.wss_url, on_message=self.on_message,
             on_error=self.on_error, on_close=self.on_close,
             on_open=self.on_open)
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/betinfo.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/betinfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #python
 """Module for IQ Option Profile websocket object."""
-from iqoptionapi.ws.objects.base import Base
+from my_iqoptionapi.ws.objects.base import Base
 
 
 class Game_betinfo_data(Base):
     """Class for IQ Option Profile websocket object."""
 
     def __init__(self):
         super(Game_betinfo_data, self).__init__()
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/candles.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/candles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ Option Candles websocket object."""
 
-from iqoptionapi.ws.objects.base import Base
+from my_iqoptionapi.ws.objects.base import Base
 
 
 class Candle(object):
     """Class for IQ Option candle."""
 
     def __init__(self, candle_data):
         """
@@ -86,28 +86,28 @@
         self.__candles_data = candles_data
 
     @property
     def first_candle(self):
         """Method to get first candle.
 
         :returns: The instance of :class:`Candle
-            <iqoptionapi.ws.objects.candles.Candle>`.
+            <my_iqoptionapi.ws.objects.candles.Candle>`.
         """
         return Candle(self.candles_data[0])
 
     @property
     def second_candle(self):
         """Method to get second candle.
 
         :returns: The instance of :class:`Candle
-            <iqoptionapi.ws.objects.candles.Candle>`.
+            <my_iqoptionapi.ws.objects.candles.Candle>`.
         """
         return Candle(self.candles_data[1])
 
     @property
     def current_candle(self):
         """Method to get current candle.
 
         :returns: The instance of :class:`Candle
-            <iqoptionapi.ws.objects.candles.Candle>`.
+            <my_iqoptionapi.ws.objects.candles.Candle>`.
         """
         return Candle(self.candles_data[-1])
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/listinfodata.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/listinfodata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module for IQ Option Candles websocket object."""
 from collections import OrderedDict
 
-from iqoptionapi.ws.objects.base import Base
+from my_iqoptionapi.ws.objects.base import Base
 
 class ListInfoData(Base):
     """Class for IQ Option Candles websocket object."""
 
     def __init__(self):
         super(ListInfoData, self).__init__()
         self.__name = "listInfoData"
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/profile.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ Option Profile websocket object."""
-from iqoptionapi.ws.objects.base import Base
+from my_iqoptionapi.ws.objects.base import Base
 
 
 class Profile(Base):
     """Class for IQ Option Profile websocket object."""
 
     def __init__(self):
         super(Profile, self).__init__()
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/objects/timesync.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/objects/timesync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for IQ Option TimeSync websocket object."""
 
 import time
 import datetime
 
-from iqoptionapi.ws.objects.base import Base
+from my_iqoptionapi.ws.objects.base import Base
 
 
 class TimeSync(Base):
     """Class for IQ Option TimeSync websocket object."""
 
     def __init__(self):
         super(TimeSync, self).__init__()
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/balance_changed.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/balance_changed.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/candle_generated.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/candle_generated.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.constants as OP_code
+import my_iqoptionapi.global_value as global_value
 
 def candle_generated_realtime(api, message, dict_queue_add):
     if message["name"] == "candle-generated":
         Active_name = list(OP_code.ACTIVES.keys())[list(
             OP_code.ACTIVES.values()).index(message["msg"]["active_id"])]
 
         active = str(Active_name)
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/candle_generated_v2.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/candle_generated_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 def candle_generated_v2(api, message, dict_queue_add):
     if message["name"] == "candles-generated":
         Active_name = list(OP_code.ACTIVES.keys())[list(
                 OP_code.ACTIVES.values()).index(message["msg"]["active_id"])]
         active = str(Active_name)
         for k, v in message["msg"]["candles"].items():
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/commission_changed.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/commission_changed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 def commission_changed(api, message):
     if message["name"] == "commission-changed":
         instrument_type = message["msg"]["instrument_type"]
         active_id = message["msg"]["active_id"]
         Active_name = list(OP_code.ACTIVES.keys())[list(
             OP_code.ACTIVES.values()).index(active_id)]
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/digital_option_placed.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/digital_option_placed.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/instrument_quotes_generated.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/instrument_quotes_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 
 def instrument_quotes_generated(api, message):
     if message["name"] == "instrument-quotes-generated":
 
         Active_name = list(OP_code.ACTIVES.keys())[list(OP_code.ACTIVES.values()).index(message["msg"]["active"])]
         period = message["msg"]["expiration"]["period"]
         ans = {}
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 from threading import Thread
 
 def live_deal(api, message): 
     if message["name"] == "live-deal":
         # name = message["name"]
         active_id = message["msg"]["instrument_active_id"]
         active = list(OP_code.ACTIVES.keys())[
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal_binary_option_placed.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal_binary_option_placed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 from threading import Thread
 
 def live_deal_binary_option_placed(api, message):
     if message["name"] == "live-deal-binary-option-placed":
         # name = message["name"]
         active_id = message["msg"]["active_id"]
         active = list(OP_code.ACTIVES.keys())[
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/live_deal_digital_option.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/live_deal_digital_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.constants as OP_code
+import my_iqoptionapi.constants as OP_code
 from threading import Thread
 
 def live_deal_digital_option(api, message):
     if message["name"] == "live-deal-digital-option":
         # name = message["name"]
         active_id = message["msg"]["instrument_active_id"]
         active = list(OP_code.ACTIVES.keys())[
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/position_changed.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/position_changed.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/profile.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module for IQ option websocket."""
-import iqoptionapi.global_value as global_value
+import my_iqoptionapi.global_value as global_value
 
 def profile(api, message):
     if message["name"] == "profile":
         api.profile.msg = message["msg"]
         if api.profile.msg != False:
             # ---------------------------
             try:
```

### Comparing `my-iqoptionapi-7.1.1/my-iqoptionapi/iqoptionapi/ws/received/technical_indicators.py` & `my_iqoptionapi-7.1.2/my_iqoptionapi/ws/received/technical_indicators.py`

 * *Files identical despite different names*

### Comparing `my-iqoptionapi-7.1.1/setup.py` & `my_iqoptionapi-7.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The python wrapper for IQ Option API package setup."""
 from setuptools import setup, find_packages
-#from myiqoptionapi.iqoptionapi.version_control import api_version
+from my_iqoptionapi.version_control import api_version
 
 setup(
-    name="my-iqoptionapi",
-    version="7.1.1",
+    name="my_iqoptionapi",
+    version=api_version,
     packages=find_packages(),
     install_requires=["pylint", "requests", "websocket-client==0.56"],
     include_package_data=True,
     description="Best IQ Option API for python",
     long_description="Best IQ Option API for python",
     url="https://github.com/zskull-py/iqoptionapi",
     author="zSkull.py",
```

