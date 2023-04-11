# Comparing `tmp/mqttwarn-0.32.0.tar.gz` & `tmp/mqttwarn-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttwarn-0.32.0.tar", last modified: Mon Feb 13 16:56:39 2023, max compression
+gzip compressed data, was "mqttwarn-0.33.0.tar", last modified: Tue Apr 11 21:59:27 2023, max compression
```

## Comparing `mqttwarn-0.32.0.tar` & `mqttwarn-0.33.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.929784 mqttwarn-0.32.0/
--rw-r--r--   0 amo        (501) staff       (20)    13355 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)     5773 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/DOCKER.md
--rw-r--r--   0 amo        (501) staff       (20)   132469 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/HANDBOOK.md
--rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      154 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    14144 2023-02-13 16:56:39.929422 mqttwarn-0.32.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)    11158 2023-02-13 16:55:35.000000 mqttwarn-0.32.0/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.884373 mqttwarn-0.32.0/mqttwarn/
--rw-r--r--   0 amo        (501) staff       (20)      462 2023-02-13 16:22:51.000000 mqttwarn-0.32.0/mqttwarn/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)       50 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/__main__.py
--rw-r--r--   0 amo        (501) staff       (20)     5539 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/commands.py
--rw-r--r--   0 amo        (501) staff       (20)     6023 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/configuration.py
--rw-r--r--   0 amo        (501) staff       (20)     7063 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/context.py
--rw-r--r--   0 amo        (501) staff       (20)    28702 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2306 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/cron.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.888613 mqttwarn-0.32.0/mqttwarn/examples/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/examples/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.889331 mqttwarn-0.32.0/mqttwarn/examples/basic/
--rwxr-xr-x   0 amo        (501) staff       (20)     3839 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/examples/basic/mqttwarn.ini
--rwxr-xr-x   0 amo        (501) staff       (20)     3034 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/examples/basic/samplefuncs.py
--rw-r--r--   0 amo        (501) staff       (20)     3067 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/model.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.927326 mqttwarn-0.32.0/mqttwarn/services/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/alexa-notify-me.py
--rw-r--r--   0 amo        (501) staff       (20)     1322 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/amqp.py
--rw-r--r--   0 amo        (501) staff       (20)     1284 2022-11-20 23:28:10.000000 mqttwarn-0.32.0/mqttwarn/services/apns.py
--rw-r--r--   0 amo        (501) staff       (20)      316 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/mqttwarn/services/apprise.py
--rw-r--r--   0 amo        (501) staff       (20)     2636 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/mqttwarn/services/apprise_multi.py
--rw-r--r--   0 amo        (501) staff       (20)     2445 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/mqttwarn/services/apprise_single.py
--rw-r--r--   0 amo        (501) staff       (20)     1468 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/mqttwarn/services/apprise_util.py
--rw-r--r--   0 amo        (501) staff       (20)     1916 2021-06-18 19:07:25.000000 mqttwarn-0.32.0/mqttwarn/services/asterisk.py
--rw-r--r--   0 amo        (501) staff       (20)     1463 2021-06-18 19:07:25.000000 mqttwarn-0.32.0/mqttwarn/services/autoremote.py
--rw-r--r--   0 amo        (501) staff       (20)     2331 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/azure_iot.py
--rw-r--r--   0 amo        (501) staff       (20)     2114 2021-06-18 19:07:25.000000 mqttwarn-0.32.0/mqttwarn/services/carbon.py
--rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/celery.py
--rw-r--r--   0 amo        (501) staff       (20)     2160 2021-06-18 19:07:25.000000 mqttwarn-0.32.0/mqttwarn/services/chromecast.py
--rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/dbus.py
--rw-r--r--   0 amo        (501) staff       (20)     1467 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/desktopnotify.py
--rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/dnsupdate.py
--rw-r--r--   0 amo        (501) staff       (20)     1345 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/emoncms.py
--rw-r--r--   0 amo        (501) staff       (20)      886 2021-06-18 19:07:25.000000 mqttwarn-0.32.0/mqttwarn/services/execute.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/fbchat.py
--rw-r--r--   0 amo        (501) staff       (20)     2124 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/file.py
--rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/freeswitch.py
--rw-r--r--   0 amo        (501) staff       (20)     1451 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/gss.py
--rw-r--r--   0 amo        (501) staff       (20)     4560 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/gss2.py
--rw-r--r--   0 amo        (501) staff       (20)     1414 2021-06-16 17:13:34.000000 mqttwarn-0.32.0/mqttwarn/services/hangbot.py
--rw-r--r--   0 amo        (501) staff       (20)     1588 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/hipchat.py
--rw-r--r--   0 amo        (501) staff       (20)     4203 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/http_urllib.py
--rw-r--r--   0 amo        (501) staff       (20)     2237 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/icinga2.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/ifttt.py
--rw-r--r--   0 amo        (501) staff       (20)     3671 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/influxdb.py
--rw-r--r--   0 amo        (501) staff       (20)     2589 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/ionic.py
--rw-r--r--   0 amo        (501) staff       (20)     1311 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/irccat.py
--rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/linuxnotify.py
--rw-r--r--   0 amo        (501) staff       (20)      881 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/log.py
--rw-r--r--   0 amo        (501) staff       (20)     2465 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/mattermost.py
--rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/mqtt.py
--rw-r--r--   0 amo        (501) staff       (20)     2337 2021-06-02 20:10:23.000000 mqttwarn-0.32.0/mqttwarn/services/mqtt_filter.py
--rw-r--r--   0 amo        (501) staff       (20)     1340 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/mqttpub.py
--rw-r--r--   0 amo        (501) staff       (20)     3064 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/mysql.py
--rw-r--r--   0 amo        (501) staff       (20)     4557 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/mysql_dynamic.py
--rw-r--r--   0 amo        (501) staff       (20)     3075 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/mysql_remap.py
--rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/mythtv.py
--rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/nntp.py
--rw-r--r--   0 amo        (501) staff       (20)     1135 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/nsca.py
--rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/osxsay.py
--rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/pastebinpub.py
--rw-r--r--   0 amo        (501) staff       (20)     1092 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/pipe.py
--rw-r--r--   0 amo        (501) staff       (20)     3360 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/postgres.py
--rw-r--r--   0 amo        (501) staff       (20)     1164 2021-06-10 17:55:48.000000 mqttwarn-0.32.0/mqttwarn/services/prowl.py
--rw-r--r--   0 amo        (501) staff       (20)     1318 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/pushalot.py
--rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/pushbullet.py
--rw-r--r--   0 amo        (501) staff       (20)     5676 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/pushover.py
--rw-r--r--   0 amo        (501) staff       (20)     3553 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/pushsafer.py
--rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/redispub.py
--rw-r--r--   0 amo        (501) staff       (20)     1189 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/rrdtool.py
--rw-r--r--   0 amo        (501) staff       (20)     2202 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/serial.py
--rw-r--r--   0 amo        (501) staff       (20)     3480 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/slack.py
--rw-r--r--   0 amo        (501) staff       (20)     1910 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/slixmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     2156 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/services/smtp.py
--rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/sqlite.py
--rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/sqlite_json2cols.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/sqlite_timestamp.py
--rw-r--r--   0 amo        (501) staff       (20)     2116 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/ssh.py
--rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/syslog.py
--rw-r--r--   0 amo        (501) staff       (20)     4445 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/telegram.py
--rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/thingspeak.py
--rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.32.0/mqttwarn/services/tootpaste.py
--rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/twilio.py
--rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/twitter.py
--rw-r--r--   0 amo        (501) staff       (20)     1210 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/websocket.py
--rw-r--r--   0 amo        (501) staff       (20)     2142 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/services/xbmc.py
--rw-r--r--   0 amo        (501) staff       (20)     1209 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/xively.py
--rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/services/xmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     3239 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/services/zabbix.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.928128 mqttwarn-0.32.0/mqttwarn/testing/
--rw-r--r--   0 amo        (501) staff       (20)        0 2022-08-21 22:46:44.000000 mqttwarn-0.32.0/mqttwarn/testing/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      375 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/testing/fixtures.py
--rw-r--r--   0 amo        (501) staff       (20)     5474 2023-02-13 12:58:46.000000 mqttwarn-0.32.0/mqttwarn/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.929062 mqttwarn-0.32.0/mqttwarn/vendor/
--rw-r--r--   0 amo        (501) staff       (20)     2294 2021-06-19 14:00:07.000000 mqttwarn-0.32.0/mqttwarn/vendor/ZabbixSender.py
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.32.0/mqttwarn/vendor/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-02-13 16:56:39.888283 mqttwarn-0.32.0/mqttwarn.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    14144 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2928 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       51 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.32.0/mqttwarn.egg-info/not-zip-safe
--rw-r--r--   0 amo        (501) staff       (20)     2254 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       24 2023-02-13 16:56:39.000000 mqttwarn-0.32.0/mqttwarn.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     2008 2023-02-13 16:22:51.000000 mqttwarn-0.32.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       14 2023-02-13 16:52:27.000000 mqttwarn-0.32.0/requirements-release.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-02-13 16:56:39.929898 mqttwarn-0.32.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     6197 2023-02-13 16:22:51.000000 mqttwarn-0.32.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.371558 mqttwarn-0.33.0/
+-rw-r--r--   0 amo        (501) staff       (20)    13649 2023-04-11 21:57:30.000000 mqttwarn-0.33.0/CHANGES.rst
+-rw-r--r--   0 amo        (501) staff       (20)     5908 2023-04-11 21:55:55.000000 mqttwarn-0.33.0/DOCKER.md
+-rw-r--r--   0 amo        (501) staff       (20)   133352 2023-04-11 20:10:09.000000 mqttwarn-0.33.0/HANDBOOK.md
+-rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      154 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    13848 2023-04-11 21:59:27.371212 mqttwarn-0.33.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)    10862 2023-03-12 11:46:29.000000 mqttwarn-0.33.0/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.332146 mqttwarn-0.33.0/mqttwarn/
+-rw-r--r--   0 amo        (501) staff       (20)      462 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)       50 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/__main__.py
+-rw-r--r--   0 amo        (501) staff       (20)     5539 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/commands.py
+-rw-r--r--   0 amo        (501) staff       (20)     6023 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/configuration.py
+-rw-r--r--   0 amo        (501) staff       (20)     7063 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/context.py
+-rw-r--r--   0 amo        (501) staff       (20)    28702 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     2306 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/cron.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.334729 mqttwarn-0.33.0/mqttwarn/examples/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/examples/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.335372 mqttwarn-0.33.0/mqttwarn/examples/basic/
+-rwxr-xr-x   0 amo        (501) staff       (20)     3839 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/examples/basic/mqttwarn.ini
+-rwxr-xr-x   0 amo        (501) staff       (20)     3034 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/examples/basic/samplefuncs.py
+-rw-r--r--   0 amo        (501) staff       (20)     3342 2023-03-13 00:29:11.000000 mqttwarn-0.33.0/mqttwarn/model.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.369527 mqttwarn-0.33.0/mqttwarn/services/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1317 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/alexa-notify-me.py
+-rw-r--r--   0 amo        (501) staff       (20)     1322 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/amqp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1284 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apns.py
+-rw-r--r--   0 amo        (501) staff       (20)      316 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise.py
+-rw-r--r--   0 amo        (501) staff       (20)     2636 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_multi.py
+-rw-r--r--   0 amo        (501) staff       (20)     2445 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_single.py
+-rw-r--r--   0 amo        (501) staff       (20)     1468 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_util.py
+-rw-r--r--   0 amo        (501) staff       (20)     1916 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/asterisk.py
+-rw-r--r--   0 amo        (501) staff       (20)     1463 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/autoremote.py
+-rw-r--r--   0 amo        (501) staff       (20)     2331 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/azure_iot.py
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/carbon.py
+-rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/celery.py
+-rw-r--r--   0 amo        (501) staff       (20)     2160 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/chromecast.py
+-rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/dbus.py
+-rw-r--r--   0 amo        (501) staff       (20)     1467 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/desktopnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/dnsupdate.py
+-rw-r--r--   0 amo        (501) staff       (20)     1345 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/emoncms.py
+-rw-r--r--   0 amo        (501) staff       (20)      886 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/execute.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/fbchat.py
+-rw-r--r--   0 amo        (501) staff       (20)     2124 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/file.py
+-rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/freeswitch.py
+-rw-r--r--   0 amo        (501) staff       (20)     1451 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/gss.py
+-rw-r--r--   0 amo        (501) staff       (20)     4560 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/gss2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1414 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/hangbot.py
+-rw-r--r--   0 amo        (501) staff       (20)     1588 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/hipchat.py
+-rw-r--r--   0 amo        (501) staff       (20)     4203 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/http_urllib.py
+-rw-r--r--   0 amo        (501) staff       (20)     2237 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/icinga2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/ifttt.py
+-rw-r--r--   0 amo        (501) staff       (20)     3671 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/influxdb.py
+-rw-r--r--   0 amo        (501) staff       (20)     2589 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/ionic.py
+-rw-r--r--   0 amo        (501) staff       (20)     1311 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/irccat.py
+-rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/linuxnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)      881 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/log.py
+-rw-r--r--   0 amo        (501) staff       (20)     2465 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/mattermost.py
+-rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/mqtt.py
+-rw-r--r--   0 amo        (501) staff       (20)     2337 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mqtt_filter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1340 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mqttpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     3064 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql.py
+-rw-r--r--   0 amo        (501) staff       (20)     4557 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql_dynamic.py
+-rw-r--r--   0 amo        (501) staff       (20)     3075 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql_remap.py
+-rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/mythtv.py
+-rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/nntp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1135 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/nsca.py
+-rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/osxsay.py
+-rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/pastebinpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1092 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/pipe.py
+-rw-r--r--   0 amo        (501) staff       (20)     3360 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/postgres.py
+-rw-r--r--   0 amo        (501) staff       (20)     1164 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/prowl.py
+-rw-r--r--   0 amo        (501) staff       (20)     1318 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/pushalot.py
+-rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/pushbullet.py
+-rw-r--r--   0 amo        (501) staff       (20)     5676 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/pushover.py
+-rw-r--r--   0 amo        (501) staff       (20)     8091 2023-04-11 20:10:09.000000 mqttwarn-0.33.0/mqttwarn/services/pushsafer.py
+-rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/redispub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1189 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/rrdtool.py
+-rw-r--r--   0 amo        (501) staff       (20)     2202 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/serial.py
+-rw-r--r--   0 amo        (501) staff       (20)     3480 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/slack.py
+-rw-r--r--   0 amo        (501) staff       (20)     1910 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/slixmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2156 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/smtp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite.py
+-rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite_json2cols.py
+-rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite_timestamp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2116 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/ssh.py
+-rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/syslog.py
+-rw-r--r--   0 amo        (501) staff       (20)     4445 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/telegram.py
+-rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/thingspeak.py
+-rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.33.0/mqttwarn/services/tootpaste.py
+-rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/twilio.py
+-rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/twitter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1210 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/websocket.py
+-rw-r--r--   0 amo        (501) staff       (20)     2142 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/xbmc.py
+-rw-r--r--   0 amo        (501) staff       (20)     1209 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/xively.py
+-rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/xmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     3239 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/zabbix.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.370127 mqttwarn-0.33.0/mqttwarn/testing/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/testing/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      375 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/testing/fixtures.py
+-rw-r--r--   0 amo        (501) staff       (20)     5474 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.370885 mqttwarn-0.33.0/mqttwarn/vendor/
+-rw-r--r--   0 amo        (501) staff       (20)     2294 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/vendor/ZabbixSender.py
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/vendor/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.334460 mqttwarn-0.33.0/mqttwarn.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    13848 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     2928 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       51 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.33.0/mqttwarn.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (501) staff       (20)     2255 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       24 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     2008 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       14 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/requirements-release.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-11 21:59:27.371632 mqttwarn-0.33.0/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     6198 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/setup.py
```

### Comparing `mqttwarn-0.32.0/CHANGES.rst` & `mqttwarn-0.33.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,34 @@
 ##################
 
 
 in progress
 ===========
 
 
+2023-04-11 0.33.0
+=================
+
+- Pushsafer: Fix to prevent submitting empty parameters to upstream API.
+- Pushsafer: Modernize configuration layout for target addresses.
+- Pushsafer: Add parameters for "Confirm", "Answer Options", and "Force Answer".
+
+Thanks, @appzer.
+
+
 2023-02-13 0.32.0
 =================
 
 - Modernize Docker configuration, now using Debian bullseye and Python 3.11.
 - Improve nightly and on-PR Docker builds.
 - Add versioning based on Git tags, using ``versioningit``. This will aid in
   telling PR- and nightly releases apart from GA releases when running
   ``mqttwarn --version``.
 - Improve Apprise integration by propagating the mqttwarn data dictionary into
-  the Apprise plugin template arguments.
+  the Apprise plugin template arguments. Thanks, @zoic21.
 
 
 2022-11-21 0.31.0
 =================
 
 - Make the PushOver API ``retry`` and ``expire`` options configurable. Thanks, @jlrgraham.
 - Add new configuration setting ``filteredmessagesloglevel``, to optionally set the log
```

### Comparing `mqttwarn-0.32.0/DOCKER.md` & `mqttwarn-0.33.0/DOCKER.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# Running mqttwarn with Docker
+# Running mqttwarn with Podman or Docker
 
-If you would rather use `mqttwarn` without installing Python and the
-required libraries, you can run it as a [Docker container](https://www.docker.com/).
-You need to install only the Docker executable.
+If you would rather use `mqttwarn` without installing Python and the required
+libraries, you can run the OCI image on [Podman] or [Docker].
 
-You can run the image as a service, i.e. in the background, or you can 
-run it interactively, perhaps to help diagnose a problem.
+You can run mqttwarn as a service, i.e. in the background, or you can run it
+interactively, perhaps to help diagnose a problem.
 
 Docker images are automatically published to:
 
 - https://github.com/orgs/jpmens/packages/container/package/mqttwarn-standard
 - https://github.com/orgs/jpmens/packages/container/package/mqttwarn-full
-- ~~https://hub.docker.com/r/jpmens/mqttwarn~~ (not automatically updated)
 
 ## Choosing the Docker image
 
 Choose one of those Docker images.
 ```shell
 # The standard image on GHCR.
 export IMAGE=ghcr.io/jpmens/mqttwarn-standard:latest
@@ -158,25 +156,33 @@
 ```
 
 
 ## Build the image
 
 If you are making any changes to the `mqttwarn` application or to the
 `Dockerfile`, you can build a local image from the files on your drive (not
-from the files on Github).
+from the files on GitHub).
 
 Execute the following from the root of the project :
 ```
-docker build -t mqttwarn-local .
+export DOCKER_BUILDKIT=1
+export COMPOSE_DOCKER_CLI_BUILD=1
+export BUILDKIT_PROGRESS=plain
+
+docker build --tag=local/mqttwarn-standard --file=Dockerfile .
+```
+
+```
+docker build --tag=local/mqttwarn-full --file=Dockerfile.full .
 ```
 
 You can then edit any files and rebuild the image as many times as you need. 
 You don't need to commit any changes.
 
-The name `mqttwarn-local` is not meaningful, other than making it obvious when
+The name `local/mqttwarn-standard` is not meaningful, other than making it obvious when
 you run it that you are using your own personal image. You can use any name you
 like, but avoid `mqttwarn` otherwise it's easily confused with the official
 images.
 
 
 ## Installing additional Python packages into Docker image
 
@@ -195,7 +201,11 @@
 ## The "full" image, including all dependencies
 
 If you prefer not to fiddle with those details, but instead want to run a full
 image including dependencies for all modules, we have you covered. Alongside
 the standard image, there is also `ghcr.io/jpmens/mqttwarn-full:latest`.
 
 The `standard` image weighs in with about 130 MB, the `full` image has 230 MB.
+
+
+[Docker]: https://docker.com/
+[Podman]: https://podman.io/
```

### Comparing `mqttwarn-0.32.0/HANDBOOK.md` & `mqttwarn-0.33.0/HANDBOOK.md`

 * *Files 1% similar despite different names*

```diff
@@ -5282,2999 +5282,3054 @@
 00014a10: 7665 7220 6f6e 2069 4f53 5d28 6173 7365  ver on iOS](asse
 00014a20: 7473 2f70 7573 686f 7665 722e 706e 6729  ts/pushover.png)
 00014a30: 0a0a 5265 7175 6972 6573 3a0a 2a20 416e  ..Requires:.* An
 00014a40: 2061 6363 6f75 6e74 2061 7420 5b70 7573   account at [pus
 00014a50: 686f 7665 722e 6e65 745d 2868 7474 7073  hover.net](https
 00014a60: 3a2f 2f70 7573 686f 7665 722e 6e65 742f  ://pushover.net/
 00014a70: 292e 0a0a 2323 2320 6070 7573 6873 6166  )...### `pushsaf
-00014a80: 6572 600a 0a54 6869 7320 7365 7276 6963  er`..This servic
-00014a90: 6520 6973 2066 6f72 205b 5075 7368 7361  e is for [Pushsa
-00014aa0: 6665 725d 2868 7474 7073 3a2f 2f77 7777  fer](https://www
-00014ab0: 2e70 7573 6873 6166 6572 2e63 6f6d 292c  .pushsafer.com),
-00014ac0: 2061 6e20 6170 7020 666f 7220 694f 532c   an app for iOS,
-00014ad0: 2041 6e64 726f 6964 2061 6e64 2057 696e   Android and Win
-00014ae0: 646f 7773 2031 302e 0a49 6e20 6f72 6465  dows 10..In orde
-00014af0: 7220 746f 2072 6563 6569 7665 2070 7573  r to receive pus
-00014b00: 6873 6166 6572 206e 6f74 6966 6963 6174  hsafer notificat
-00014b10: 696f 6e73 2079 6f75 206e 6565 6420 7768  ions you need wh
-00014b20: 6174 2069 7320 6361 6c6c 6564 2061 205f  at is called a _
-00014b30: 7072 6976 6174 6520 6f72 2061 6c69 6173  private or alias
-00014b40: 206b 6579 5f3a 0a0a 6060 6069 6e69 0a5b   key_:..```ini.[
-00014b50: 636f 6e66 6967 3a70 7573 6873 6166 6572  config:pushsafer
-00014b60: 5d0a 7461 7267 6574 7320 3d20 7b0a 2020  ].targets = {.  
-00014b70: 2020 276e 6167 696f 7327 2020 2020 203a    'nagios'     :
-00014b80: 205b 2770 7269 7661 7465 6b65 7927 2c20   ['privatekey', 
-00014b90: 2744 6576 6963 6520 4944 272c 2027 4963  'Device ID', 'Ic
-00014ba0: 6f6e 272c 2027 536f 756e 6427 2c20 2756  on', 'Sound', 'V
-00014bb0: 6962 7261 7469 6f6e 272c 2027 5552 4c27  ibration', 'URL'
-00014bc0: 2c20 2755 726c 2054 6974 6c65 272c 2027  , 'Url Title', '
-00014bd0: 5469 6d65 324c 6976 6527 2c20 2750 7269  Time2Live', 'Pri
-00014be0: 6f72 6974 7927 2c20 2752 6574 7279 272c  ority', 'Retry',
-00014bf0: 2027 4578 7069 7265 272c 2027 416e 7377   'Expire', 'Answ
-00014c00: 6572 275d 2c0a 2020 2020 2774 7261 636b  er'],.    'track
-00014c10: 696e 6727 2020 203a 205b 2761 6c69 6173  ing'   : ['alias
-00014c20: 6b65 7931 275d 2c0a 2020 2020 2765 7874  key1'],.    'ext
-00014c30: 7261 7068 6f6e 6527 203a 205b 2761 6c69  raphone' : ['ali
-00014c40: 6173 6b65 7932 272c 2027 272c 2027 272c  askey2', '', '',
-00014c50: 2027 272c 2027 272c 2027 272c 2027 272c   '', '', '', '',
-00014c60: 2027 3630 272c 2027 3227 2c20 2736 3027   '60', '2', '60'
-00014c70: 2c20 2736 3030 272c 2027 3027 5d2c 0a09  , '600', '0'],..
-00014c80: 2777 6172 6e6d 6527 2020 2020 203a 205b  'warnme'     : [
-00014c90: 2761 6c69 6173 6b65 7933 272c 2027 272c  'aliaskey3', '',
-00014ca0: 2027 272c 2027 272c 2027 272c 2027 272c   '', '', '', '',
-00014cb0: 2027 272c 2027 3630 272c 2027 3127 2c20   '', '60', '1', 
-00014cc0: 2727 2c20 2727 2c20 2731 275d 0a20 2020  '', '', '1'].   
-00014cd0: 207d 0a60 6060 0a0a 5468 6973 2064 6566   }.```..This def
-00014ce0: 696e 6573 2074 6172 6765 7473 2028 606e  ines targets (`n
-00014cf0: 6167 696f 7360 2c20 6061 6c65 7274 7360  agios`, `alerts`
-00014d00: 2c20 6574 632e 2920 7768 6963 6820 6172  , etc.) which ar
-00014d10: 6520 6469 7265 6374 6564 2074 6f20 7468  e directed to th
-00014d20: 650a 636f 6e66 6967 7572 6564 205f 7072  e.configured _pr
-00014d30: 6976 6174 6520 6f72 2061 6c69 6173 206b  ivate or alias k
-00014d40: 6579 5f20 636f 6d62 696e 6174 696f 6e73  ey_ combinations
-00014d50: 2e20 5468 6973 2069 6e20 7475 726e 2065  . This in turn e
-00014d60: 6e61 626c 6573 2079 6f75 2074 6f0a 6e6f  nables you to.no
-00014d70: 7469 6679 2c20 7361 792c 206f 6e65 206f  tify, say, one o
-00014d80: 7220 6d6f 7265 206f 6620 796f 7572 2064  r more of your d
-00014d90: 6576 6963 6573 2061 7320 7765 6c6c 2061  evices as well a
-00014da0: 7320 6f6e 6520 666f 7220 796f 7572 2073  s one for your s
-00014db0: 706f 7573 652e 0a46 6f72 2061 206c 6973  pouse..For a lis
-00014dc0: 7420 6f66 2061 7661 696c 6162 6c65 2069  t of available i
-00014dd0: 636f 6e73 2c20 736f 756e 6473 2061 6e64  cons, sounds and
-00014de0: 206f 7468 6572 2070 6172 616d 7320 7365   other params se
-00014df0: 6520 7468 650a 5b50 7573 6873 6166 6572  e the.[Pushsafer
-00014e00: 2041 5049 5d28 6874 7470 733a 2f2f 7777   API](https://ww
-00014e10: 772e 7075 7368 7361 6665 722e 636f 6d2f  w.pushsafer.com/
-00014e20: 656e 2f70 7573 6861 7069 292e 0a0a 7c20  en/pushapi)...| 
-00014e30: 546f 7069 6320 6f70 7469 6f6e 2020 7c20  Topic option  | 
-00014e40: 204d 2f4f 2020 207c 2044 6573 6372 6970   M/O   | Descrip
-00014e50: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00014e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e70: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
-00014e80: 2d20 7c20 3a2d 2d2d 2d3a 207c 202d 2d2d  - | :----: | ---
-00014e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014eb0: 2d2d 2d20 7c0a 7c20 6074 6974 6c65 6020  --- |.| `title` 
-00014ec0: 2020 2020 2020 7c20 2020 4f20 2020 207c        |   O    |
-00014ed0: 2061 7070 6c69 6361 7469 6f6e 2074 6974   application tit
-00014ee0: 6c65 2028 6466 6c74 3a20 7075 7368 7361  le (dflt: pushsa
-00014ef0: 6665 7220 6466 6c74 2920 7c0a 0a21 5b70  fer dflt) |..![p
-00014f00: 7573 6873 6166 6572 206f 6e20 694f 535d  ushsafer on iOS]
-00014f10: 2861 7373 6574 732f 7075 7368 7361 6665  (assets/pushsafe
-00014f20: 722e 6a70 6729 0a0a 5265 7175 6972 6573  r.jpg)..Requires
-00014f30: 3a0a 2a20 416e 2061 6363 6f75 6e74 2061  :.* An account a
-00014f40: 7420 5b70 7573 6873 6166 6572 2e63 6f6d  t [pushsafer.com
-00014f50: 5d28 6874 7470 733a 2f2f 7777 772e 7075  ](https://www.pu
-00014f60: 7368 7361 6665 722e 636f 6d2f 292e 0a0a  shsafer.com/)...
-00014f70: 2323 2320 6072 6564 6973 7075 6260 0a0a  ### `redispub`..
-00014f80: 5468 6520 6072 6564 6973 7075 6260 2070  The `redispub` p
-00014f90: 6c75 6769 6e20 7075 626c 6973 6865 7320  lugin publishes 
-00014fa0: 746f 2061 2052 6564 6973 2063 6861 6e6e  to a Redis chann
-00014fb0: 656c 2e0a 0a60 6060 696e 690a 5b63 6f6e  el...```ini.[con
-00014fc0: 6669 673a 7265 6469 7370 7562 5d0a 686f  fig:redispub].ho
-00014fd0: 7374 2020 3d20 2027 6c6f 6361 6c68 6f73  st  =  'localhos
-00014fe0: 7427 0a70 6f72 7420 203d 2020 3633 3739  t'.port  =  6379
-00014ff0: 0a74 6172 6765 7473 203d 207b 0a20 2020  .targets = {.   
-00015000: 2027 7231 2720 2020 2020 203a 205b 2027   'r1'      : [ '
-00015010: 6368 616e 6e65 6c2d 3127 205d 0a20 2020  channel-1' ].   
-00015020: 207d 0a60 6060 0a0a 5265 7175 6972 6573   }.```..Requires
-00015030: 3a0a 2a20 5b72 6564 6973 2d70 795d 2868  :.* [redis-py](h
-00015040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00015050: 6d2f 616e 6479 6d63 6375 7264 792f 7265  m/andymccurdy/re
-00015060: 6469 732d 7079 290a 0a23 2323 2060 7272  dis-py)..### `rr
-00015070: 6474 6f6f 6c60 0a0a 5468 6520 6072 7264  dtool`..The `rrd
-00015080: 746f 6f6c 6020 706c 7567 696e 2075 7064  tool` plugin upd
-00015090: 6174 6573 2061 2072 6f75 6e64 2d72 6f62  ates a round-rob
-000150a0: 696e 2064 6174 6162 6173 6520 6372 6561  in database crea
-000150b0: 7465 6420 6279 205b 7272 6474 6f6f 6c5d  ted by [rrdtool]
-000150c0: 2077 6974 680a 7468 6520 6d65 7373 6167   with.the messag
-000150d0: 6520 7061 796c 6f61 642e 0a0a 6060 6069  e payload...```i
-000150e0: 6e69 0a5b 636f 6e66 6967 3a72 7264 746f  ni.[config:rrdto
-000150f0: 6f6c 5d0a 7461 7267 6574 7320 3d20 7b0a  ol].targets = {.
-00015100: 2020 2020 276c 6976 696e 672d 7465 6d70      'living-temp
-00015110: 2720 203a 205b 272f 746d 702f 6c69 7669  '  : ['/tmp/livi
-00015120: 6e67 2d74 656d 702e 7272 6427 2c20 2027  ng-temp.rrd',  '
-00015130: 2d2d 7465 6d70 6c61 7465 272c 2027 7465  --template', 'te
-00015140: 6d70 275d 2c0a 2020 2020 276b 6974 6368  mp'],.    'kitch
-00015150: 656e 2d74 656d 7027 203a 205b 272f 746d  en-temp' : ['/tm
-00015160: 702f 6b69 7463 6865 6e2d 7465 6d70 2e72  p/kitchen-temp.r
-00015170: 7264 272c 2027 2d2d 7465 6d70 6c61 7465  rd', '--template
-00015180: 272c 2027 7465 6d70 275d 0a20 2020 207d  ', 'temp'].    }
-00015190: 0a60 6060 0a0a 5b72 7264 7079 7468 6f6e  .```..[rrdpython
-000151a0: 2773 2041 5049 5d20 6578 7065 6374 7320  's API] expects 
-000151b0: 7374 7269 6e67 7320 616e 642f 6f72 2061  strings and/or a
-000151c0: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-000151d0: 2061 7320 7061 7261 6d65 7465 7273 2074   as parameters t
-000151e0: 6f20 7468 6520 6675 6e63 7469 6f6e 732e  o the functions.
-000151f0: 0a54 6875 732c 2061 206c 6973 7420 666f  .Thus, a list fo
-00015200: 7220 6120 7461 7267 6574 2073 696d 706c  r a target simpl
-00015210: 7920 636f 6e74 6169 6e73 2074 6865 2063  y contains the c
-00015220: 6f6d 6d61 6e64 206c 696e 6520 6172 6775  ommand line argu
-00015230: 6d65 6e74 7320 666f 7220 6072 7264 746f  ments for `rrdto
-00015240: 6f6c 2075 7064 6174 6560 2e0a 0a54 6865  ol update`...The
-00015250: 2070 6c75 6769 6e20 7769 6c6c 2065 6d62   plugin will emb
-00015260: 6564 2074 6865 206d 6573 7361 6765 2061  ed the message a
-00015270: 7320 6669 6e61 6c20 6172 6775 6d65 6e74  s final argument
-00015280: 2060 4e3a 3c6d 6573 7361 6765 3e60 2c20   `N:<message>`, 
-00015290: 6966 2074 6865 206d 6573 7361 6765 2069  if the message i
-000152a0: 7320 616e 0a69 6e74 6567 6572 206e 756d  s an.integer num
-000152b0: 6265 722e 204f 7468 6572 7769 7365 2c20  ber. Otherwise, 
-000152c0: 6974 2077 696c 6c20 6272 6561 6b20 7570  it will break up
-000152d0: 2074 6865 206d 6573 7361 6765 2069 6e74   the message int
-000152e0: 6f20 7369 6e67 6c65 2077 6f72 6473 2061  o single words a
-000152f0: 6e64 2061 7070 656e 6420 7468 6973 200a  nd append this .
-00015300: 6c69 7374 2074 6f20 7468 6520 6c69 7374  list to the list
-00015310: 2073 7570 706c 6965 6420 6279 2074 6865   supplied by the
-00015320: 2074 6172 6765 742e 2054 6869 7320 6c65   target. This le
-00015330: 6176 6573 2069 7420 746f 2079 6f75 7220  aves it to your 
-00015340: 6469 7363 7265 7469 6f6e 205f 7768 6572  discretion _wher
-00015350: 655f 2074 6f20 7075 740a 6172 6775 6d65  e_ to put.argume
-00015360: 6e74 7320 616e 6420 6576 656e 202d 2077  nts and even - w
-00015370: 6974 6820 7468 6520 7269 6768 7420 6461  ith the right da
-00015380: 7461 206d 6170 7069 6e67 2061 6e64 2065  ta mapping and e
-00015390: 7874 7261 6374 696f 6e20 696e 2070 6c61  xtraction in pla
-000153a0: 6365 202d 2061 6c6c 6f77 7320 666f 7220  ce - allows for 
-000153b0: 0a61 2063 6f6e 6669 6775 7261 7469 6f6e  .a configuration
-000153c0: 206c 696b 653a 0a0a 6060 6069 6e69 0a5b   like:..```ini.[
-000153d0: 636f 6e66 6967 3a72 7264 746f 6f6c 5d0a  config:rrdtool].
-000153e0: 7461 7267 6574 7320 3d20 7b0a 2020 2020  targets = {.    
-000153f0: 2020 2020 2762 6174 7473 656e 736f 7227      'battsensor'
-00015400: 3a20 5b20 5d2c 0a20 2020 2020 2020 207d  : [ ],.        }
-00015410: 0a2e 2e2e 0a5b 6461 7461 6c6f 672d 6261  .....[datalog-ba
-00015420: 7474 6572 792d 6c6f 675d 0a74 6f70 6963  ttery-log].topic
-00015430: 203d 2064 6174 616c 6f67 2f73 656e 736f   = datalog/senso
-00015440: 7273 2f62 6174 742f 2b0a 7461 7267 6574  rs/batt/+.target
-00015450: 7320 3d20 6c6f 673a 696e 666f 2c72 7264  s = log:info,rrd
-00015460: 746f 6f6c 3a62 6174 7473 656e 736f 720a  tool:battsensor.
-00015470: 6461 7461 6d61 7020 3d20 2e2e 2e0a 666f  datamap = ....fo
-00015480: 726d 6174 203d 202f 7372 762f 7272 642f  rmat = /srv/rrd/
-00015490: 7365 6e73 6f72 732f 7b73 656e 736f 725f  sensors/{sensor_
-000154a0: 6964 7d2e 7272 6420 2d74 2062 6174 7420  id}.rrd -t batt 
-000154b0: 7b74 737d 3a7b 6261 7474 7d0a 6060 600a  {ts}:{batt}.```.
-000154c0: 0a52 6571 7569 7265 7320 7468 6520 7272  .Requires the rr
-000154d0: 6474 6f6f 6c20 6269 6e64 696e 6773 2061  dtool bindings a
-000154e0: 7661 696c 6162 6c65 2077 6974 6820 6070  vailable with `p
-000154f0: 6970 2069 6e73 7461 6c6c 2072 7264 746f  ip install rrdto
-00015500: 6f6c 602e 0a0a 5b72 7264 746f 6f6c 5d3a  ol`...[rrdtool]:
-00015510: 2068 7474 703a 2f2f 6f73 732e 6f65 7469   http://oss.oeti
-00015520: 6b65 722e 6368 2f72 7264 746f 6f6c 2f0a  ker.ch/rrdtool/.
-00015530: 5b72 7264 7079 7468 6f6e 2773 2041 5049  [rrdpython's API
-00015540: 5d3a 2068 7474 703a 2f2f 6f73 732e 6f65  ]: http://oss.oe
-00015550: 7469 6b65 722e 6368 2f72 7264 746f 6f6c  tiker.ch/rrdtool
-00015560: 2f70 726f 672f 7272 6470 7974 686f 6e2e  /prog/rrdpython.
-00015570: 656e 2e68 746d 6c0a 0a23 2323 2060 7365  en.html..### `se
-00015580: 7269 616c 600a 0a54 6865 2060 7365 7269  rial`..The `seri
-00015590: 616c 6020 706c 7567 696e 2073 656e 6473  al` plugin sends
-000155a0: 206f 7574 2072 6563 6569 7665 6420 6d65   out received me
-000155b0: 7373 6167 6573 2074 6f20 7468 6520 7365  ssages to the se
-000155c0: 7269 616c 2070 6f72 742e 204d 6573 7361  rial port. Messa
-000155d0: 6765 2070 6179 6c6f 6164 2063 616e 2062  ge payload can b
-000155e0: 6520 6269 6e61 7279 2064 6174 612c 2073  e binary data, s
-000155f0: 7472 696e 6720 6f72 206a 736f 6e2e 0a0a  tring or json...
-00015600: 6060 6069 6e69 0a5b 636f 6e66 6967 3a73  ```ini.[config:s
-00015610: 6572 6961 6c5d 0a61 7070 656e 645f 6e65  erial].append_ne
-00015620: 776c 696e 6520 3d20 4661 6c73 650a 7461  wline = False.ta
-00015630: 7267 6574 7320 3d20 7b0a 2020 2020 2773  rgets = {.    's
-00015640: 6572 6961 6c70 6f72 7431 2720 203a 205b  erialport1'  : [
-00015650: 272f 6465 762f 7474 7955 5342 3027 2c20  '/dev/ttyUSB0', 
-00015660: 2027 3131 3532 3030 275d 2c0a 2020 2020   '115200'],.    
-00015670: 2773 6f6d 652d 6465 7669 6365 2720 3a20  'some-device' : 
-00015680: 5b27 736f 636b 6574 3a2f 2f31 3932 2e31  ['socket://192.1
-00015690: 3638 2e31 2e31 3030 3a32 3332 3327 2c20  68.1.100:2323', 
-000156a0: 2739 3630 3027 5d0a 2020 2020 7d0a 6060  '9600'].    }.``
-000156b0: 600a 4669 7273 7420 7061 7261 6d65 7465  `.First paramete
-000156c0: 7220 696e 2074 6172 6765 7420 636f 6e66  r in target conf
-000156d0: 6967 2063 616e 2062 6520 6120 706f 7274  ig can be a port
-000156e0: 6e61 6d65 206f 7220 616e 205b 7572 6c20  name or an [url 
-000156f0: 6861 6e64 6c65 725d 2868 7474 7073 3a2f  handler](https:/
-00015700: 2f70 7974 686f 6e68 6f73 7465 642e 6f72  /pythonhosted.or
-00015710: 672f 7079 7365 7269 616c 2f75 726c 5f68  g/pyserial/url_h
-00015720: 616e 646c 6572 732e 6874 6d6c 292e 0a53  andlers.html)..S
-00015730: 6563 6f6e 6420 7061 7261 6d65 7465 7220  econd parameter 
-00015740: 6973 2074 6865 2062 6175 6472 6174 6520  is the baudrate 
-00015750: 666f 7220 7468 6520 706f 7274 2e0a 4966  for the port..If
-00015760: 2060 6170 7065 6e64 5f6e 6577 6c69 6e65   `append_newline
-00015770: 6020 6973 2054 7275 652c 2061 206e 6577  ` is True, a new
-00015780: 6c69 6e65 2063 6861 7261 6374 6572 2069  line character i
-00015790: 7320 756e 636f 6e64 6974 696f 6e61 6c6c  s unconditionall
-000157a0: 7920 6170 7065 6e64 6564 2074 6f20 7468  y appended to th
-000157b0: 6520 7374 7269 6e67 2077 7269 7474 656e  e string written
-000157c0: 2074 6f20 7468 6520 7365 7269 616c 706f   to the serialpo
-000157d0: 7274 2e0a 0a52 6571 7569 7265 7320 7468  rt...Requires th
-000157e0: 6520 7079 7365 7269 616c 2062 696e 6469  e pyserial bindi
-000157f0: 6e67 7320 6176 6169 6c61 626c 6520 7769  ngs available wi
-00015800: 7468 2060 7069 7020 696e 7374 616c 6c20  th `pip install 
-00015810: 7079 7365 7269 616c 602e 0a0a 2323 2320  pyserial`...### 
-00015820: 6073 6c61 636b 600a 0a54 6865 2060 736c  `slack`..The `sl
-00015830: 6163 6b60 2070 6c75 6769 6e20 706f 7374  ack` plugin post
-00015840: 7320 6d65 7373 6167 6573 2074 6f20 6368  s messages to ch
-00015850: 616e 6e65 6c73 2069 6e20 6f72 2075 7365  annels in or use
-00015860: 7273 206f 6620 7468 6520 5b73 6c61 636b  rs of the [slack
-00015870: 2e63 6f6d 5d28 6874 7470 3a2f 2f73 6c61  .com](http://sla
-00015880: 636b 2e63 6f6d 2920 7365 7276 6963 652e  ck.com) service.
-00015890: 2054 6865 2063 6f6e 6669 6775 7261 7469   The configurati
-000158a0: 6f6e 206f 6620 7468 6973 2073 6572 7669  on of this servi
-000158b0: 6365 2072 6571 7569 7265 7320 616e 2041  ce requires an A
-000158c0: 5049 2074 6f6b 656e 206f 6274 6169 6e69  PI token obtaini
-000158d0: 6e61 626c 6520 7468 6572 652e 0a0a 6060  nable there...``
-000158e0: 6069 6e69 0a5b 636f 6e66 6967 3a73 6c61  `ini.[config:sla
-000158f0: 636b 5d0a 746f 6b65 6e20 3d20 2778 7878  ck].token = 'xxx
-00015900: 782d 3132 3334 3536 3738 3930 2d31 3233  x-1234567890-123
-00015910: 3435 3637 3839 302d 3132 3334 3536 3738  4567890-12345678
-00015920: 3930 2d31 3233 3461 3127 0a74 6172 6765  90-1234a1'.targe
-00015930: 7473 203d 207b 0a20 2020 2020 2020 2020  ts = {.         
-00015940: 2020 2020 2020 2023 2020 205b 746f 6b65         #   [toke
-00015950: 6e2c 5d20 2363 6861 6e6e 656c 2f40 7573  n,] #channel/@us
-00015960: 6572 2c20 7573 6572 6e61 6d65 2c20 6963  er, username, ic
-00015970: 6f6e 2c20 5b61 735f 7573 6572 5d0a 2020  on, [as_user].  
-00015980: 2027 6a70 6d65 6e73 2720 2020 2020 3a20   'jpmens'     : 
-00015990: 5b20 2740 6a70 6d65 6e73 272c 2020 2022  [ '@jpmens',   "
-000159a0: 416c 6572 7465 7222 2c20 2020 273a 646f  Alerter",   ':do
-000159b0: 6f72 3a27 2020 2020 2020 2020 2020 5d2c  or:'          ],
-000159c0: 0a20 2020 2767 656e 6572 616c 2720 2020  .   'general'   
-000159d0: 203a 205b 2027 2367 656e 6572 616c 272c   : [ '#general',
-000159e0: 2020 226d 7174 7477 6172 6e22 2c20 2027    "mqttwarn",  '
-000159f0: 3a73 7972 696e 6765 3a27 2020 2020 2020  :syringe:'      
-00015a00: 205d 2c0a 2020 2027 7465 7374 2720 2020   ],.   'test'   
-00015a10: 2020 2020 3a20 5b20 2723 7465 7374 272c      : [ '#test',
-00015a20: 2020 2020 2022 426f 7455 7365 7222 2c20       "BotUser", 
-00015a30: 2020 273a 756e 7573 6564 3a27 2c20 2054    ':unused:',  T
-00015a40: 7275 6520 5d2c 0a20 2020 2773 6563 6f6e  rue ],.   'secon
-00015a50: 642d 6163 6327 203a 205b 2027 7878 7878  d-acc' : [ 'xxxx
-00015a60: 2d39 3939 3939 3939 2d39 3939 3939 3939  -9999999-9999999
-00015a70: 2d39 3939 3939 3939 3927 2c20 2723 6765  -99999999', '#ge
-00015a80: 6e65 7261 6c27 2c20 2274 6573 7422 2c20  neral', "test", 
-00015a90: 273a 686f 7573 653a 2720 5d2c 0a20 207d  ':house:' ],.  }
-00015aa0: 0a60 6060 0a0a 5468 6520 7365 7276 6963  .```..The servic
-00015ab0: 6520 6c65 7665 6c20 6074 6f6b 656e 6020  e level `token` 
-00015ac0: 6973 206f 7074 696f 6e61 6c2c 2062 7574  is optional, but
-00015ad0: 2069 6620 6d69 7373 696e 6720 6561 6368   if missing each
-00015ae0: 2074 6172 6765 7420 6d75 7374 2068 6176   target must hav
-00015af0: 6520 6120 6074 6f6b 656e 6020 6465 6669  e a `token` defi
-00015b00: 6e65 642e 0a0a 4561 6368 2074 6172 6765  ned...Each targe
-00015b10: 7420 6465 6669 6e65 7320 7468 6520 6e61  t defines the na
-00015b20: 6d65 206f 6620 616e 2065 7869 7374 696e  me of an existin
-00015b30: 6720 6368 616e 6e65 6c20 2860 2363 6861  g channel (`#cha
-00015b40: 6e6e 656c 6e61 6d65 6029 206f 7220 6120  nnelname`) or a 
-00015b50: 7573 6572 2028 6040 7573 6572 6e61 6d65  user (`@username
-00015b60: 6029 2074 6f20 6265 0a61 6464 7265 7373  `) to be.address
-00015b70: 6564 2c20 7468 6520 6e61 6d65 206f 6620  ed, the name of 
-00015b80: 7468 6520 7365 6e64 696e 6720 7573 6572  the sending user
-00015b90: 2061 7320 7765 6c6c 2061 7320 616e 205b   as well as an [
-00015ba0: 656d 6f6a 6920 6963 6f6e 5d28 6874 7470  emoji icon](http
-00015bb0: 3a2f 2f77 7777 2e65 6d6f 6a69 2d63 6865  ://www.emoji-che
-00015bc0: 6174 2d73 6865 6574 2e63 6f6d 2920 746f  at-sheet.com) to
-00015bd0: 2075 7365 2e0a 0a4f 7074 696f 6e61 6c6c   use...Optionall
-00015be0: 792c 2061 2074 6172 6765 7420 6361 6e20  y, a target can 
-00015bf0: 6465 6669 6e65 2074 6865 206d 6573 7361  define the messa
-00015c00: 6765 2074 6f20 6765 7420 706f 7374 6564  ge to get posted
-00015c10: 2061 7320 6120 7573 6572 2c20 7065 720a   as a user, per.
-00015c20: 5b53 6c61 636b 2041 7574 686f 7273 6869  [Slack Authorshi
-00015c30: 7020 646f 6375 6d65 6e74 6174 696f 6e5d  p documentation]
-00015c40: 2868 7474 7073 3a2f 2f61 7069 2e73 6c61  (https://api.sla
-00015c50: 636b 2e63 6f6d 2f6d 6574 686f 6473 2f63  ck.com/methods/c
-00015c60: 6861 742e 706f 7374 4d65 7373 6167 6523  hat.postMessage#
-00015c70: 6175 7468 6f72 7368 6970 292e 0a4e 6f74  authorship)..Not
-00015c80: 6520 7468 6174 2070 6f73 7469 6e67 2061  e that posting a
-00015c90: 7320 6120 7573 6572 2069 6e20 6120 6368  s a user in a ch
-00015ca0: 616e 6e65 6c20 6973 206f 6e6c 7920 706f  annel is only po
-00015cb0: 7373 6962 6c65 2c20 6966 2074 6865 2075  ssible, if the u
-00015cc0: 7365 7220 6861 730a 6a6f 696e 6564 2074  ser has.joined t
-00015cd0: 6865 2063 6861 6e6e 656c 2e0a 0a21 5b53  he channel...![S
-00015ce0: 6c61 636b 5d28 6173 7365 7473 2f73 6c61  lack](assets/sla
-00015cf0: 636b 2e70 6e67 290a 0a54 6869 7320 706c  ck.png)..This pl
-00015d00: 7567 696e 2072 6571 7569 7265 7320 5b50  ugin requires [P
-00015d10: 7974 686f 6e20 736c 6163 6b2d 7364 6b5d  ython slack-sdk]
-00015d20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00015d30: 636f 6d2f 736c 6163 6b61 7069 2f70 7974  com/slackapi/pyt
-00015d40: 686f 6e2d 736c 6163 6b2d 7364 6b29 2e0a  hon-slack-sdk)..
-00015d50: 0a54 6865 2073 6c61 636b 2073 6572 7669  .The slack servi
-00015d60: 6365 2077 696c 6c20 6163 6365 7074 2061  ce will accept a
-00015d70: 2070 6179 6c6f 6164 2077 6974 6820 6569   payload with ei
-00015d80: 7468 6572 2061 2073 696d 706c 6520 7465  ther a simple te
-00015d90: 7874 206d 6573 7361 6765 2c20 6f72 2061  xt message, or a
-00015da0: 206a 736f 6e20 7061 796c 6f61 6420 7768   json payload wh
-00015db0: 6963 6820 636f 6e74 6169 6e73 0a61 2060  ich contains.a `
-00015dc0: 6d65 7373 6167 6560 2061 6e64 2065 6974  message` and eit
-00015dd0: 6865 7220 616e 2060 696d 6167 6575 726c  her an `imageurl
-00015de0: 6020 6f72 2060 696d 6167 6562 6173 6536  ` or `imagebase6
-00015df0: 3460 2065 6e63 6f64 6564 2069 6d61 6765  4` encoded image
-00015e00: 2e0a 0a46 7572 7468 6572 2c20 7468 6520  ...Further, the 
-00015e10: 696d 6167 6575 726c 2070 6179 6c6f 6164  imageurl payload
-00015e20: 2c20 6361 6e20 6861 7665 2074 6865 2061  , can have the a
-00015e30: 6464 6974 696f 6e61 6c20 7061 7261 6d65  dditional parame
-00015e40: 7465 7273 206f 6620 616e 2061 7574 6820  ters of an auth 
-00015e50: 7479 7065 2028 6261 7369 632c 2064 6967  type (basic, dig
-00015e60: 6573 7429 2061 6e64 2061 2075 7365 7220  est) and a user 
-00015e70: 616e 6420 7061 7373 776f 7264 2e20 2054  and password.  T
-00015e80: 6869 7320 6973 2075 7365 6675 6c20 6966  his is useful if
-00015e90: 2079 6f75 7220 696d 6167 696e 6720 6465   your imaging de
-00015ea0: 7669 6365 2075 7365 7320 6175 7468 656e  vice uses authen
-00015eb0: 7469 6361 7469 6f6e 2e20 2053 6f6d 6520  tication.  Some 
-00015ec0: 6578 616d 706c 6573 2061 7265 2073 6f6d  examples are som
-00015ed0: 6520 4950 2063 616d 6572 6173 2c20 6f72  e IP cameras, or
-00015ee0: 2073 6f6d 6520 6f74 6865 7220 7369 6d70   some other simp
-00015ef0: 6c65 2069 6e74 6572 6e65 7420 6261 7365  le internet base
-00015f00: 6420 696d 6167 6520 7365 7276 6963 6573  d image services
-00015f10: 2e0a 0a54 6865 2066 6f6c 6c6f 7769 6e67  ...The following
-00015f20: 2070 6179 6c6f 6164 7320 6172 6520 7661   payloads are va
-00015f30: 6c69 643b 0a0a 6060 600a 5369 6d70 6c65  lid;..```.Simple
-00015f40: 2074 6578 7420 6d65 7373 6167 650a 6060   text message.``
-00015f50: 600a 0a60 6060 6a73 6f6e 0a7b 0a20 2020  `..```json.{.   
-00015f60: 2022 6d65 7373 6167 6522 3a20 224d 6573   "message": "Mes
-00015f70: 7361 6765 206f 6e6c 792c 2077 6974 6820  sage only, with 
-00015f80: 6e6f 2069 6d61 6765 220a 7d0a 6060 600a  no image".}.```.
-00015f90: 0a60 6060 6a73 6f6e 0a20 7b0a 2020 2020  .```json. {.    
-00015fa0: 226d 6573 7361 6765 223a 2022 4d65 7373  "message": "Mess
-00015fb0: 6167 6520 7769 7468 2062 6173 6536 3420  age with base64 
-00015fc0: 656e 636f 6465 6420 696d 6167 6522 2c0a  encoded image",.
-00015fd0: 2020 2020 2269 6d61 6765 6261 7365 3634      "imagebase64
-00015fe0: 223a 2022 3c62 6173 6536 3420 656e 636f  ": "<base64 enco
-00015ff0: 6465 6420 696d 6167 653e 220a 207d 0a60  ded image>". }.`
-00016000: 6060 0a0a 6060 606a 736f 6e0a 207b 0a20  ``..```json. {. 
-00016010: 2020 2022 6d65 7373 6167 6522 3a20 224d     "message": "M
-00016020: 6573 7361 6765 2077 6974 6820 696d 6167  essage with imag
-00016030: 6520 646f 776e 6c6f 6164 6564 2066 726f  e downloaded fro
-00016040: 6d20 5552 4c22 2c0a 2020 2020 2269 6d61  m URL",.    "ima
-00016050: 6765 7572 6c22 3a20 223c 696d 6167 6520  geurl": "<image 
-00016060: 7572 6c3e 220a 207d 0a60 6060 0a0a 6060  url>". }.```..``
-00016070: 606a 736f 6e0a 207b 0a20 2020 2022 6d65  `json. {.    "me
-00016080: 7373 6167 6522 3a20 224d 6573 7361 6765  ssage": "Message
-00016090: 2077 6974 6820 696d 6167 6520 646f 776e   with image down
-000160a0: 6c6f 6164 6564 2066 726f 6d20 5552 4c3a  loaded from URL:
-000160b0: 2064 6967 6573 7420 6175 7468 656e 7469   digest authenti
-000160c0: 6361 7469 6f6e 222c 0a20 2020 2022 696d  cation",.    "im
-000160d0: 6167 6575 726c 223a 2022 3c69 6d61 6765  ageurl": "<image
-000160e0: 2075 726c 3e22 2c0a 2020 2020 2261 7574   url>",.    "aut
-000160f0: 6822 3a20 2264 6967 6573 7422 2c0a 2020  h": "digest",.  
-00016100: 2020 2275 7365 7222 3a20 226d 7973 7065    "user": "myspe
-00016110: 6369 616c 7573 6572 222c 0a20 2020 2022  cialuser",.    "
-00016120: 7061 7373 776f 7264 223a 2022 6d79 7370  password": "mysp
-00016130: 6563 6961 6c70 6173 7377 6f72 6422 0a20  ecialpassword". 
-00016140: 7d0a 6060 600a 466f 7220 7468 6520 6162  }.```.For the ab
-00016150: 6f76 6520 6578 616d 706c 652c 2049 2077  ove example, I w
-00016160: 6f75 6c64 206f 6e6c 7920 7265 636f 6d6d  ould only recomm
-00016170: 656e 6420 7468 6973 2062 6520 7573 6564  end this be used
-00016180: 2069 6e20 6120 6c6f 6361 6c20 4d51 5454   in a local MQTT
-00016190: 2073 6572 7665 7220 696e 7374 616e 6365   server instance
-000161a0: 2c20 6173 2074 6865 2070 6173 7377 6f72  , as the passwor
-000161b0: 6420 666f 7220 796f 7572 2069 6d61 6769  d for your imagi
-000161c0: 6e67 2064 6576 6963 6520 6973 2062 6569  ng device is bei
-000161d0: 6e67 2074 7261 6e73 6d69 7474 6564 2069  ng transmitted i
-000161e0: 6e20 7468 6520 636c 6561 7220 746f 206d  n the clear to m
-000161f0: 7174 7477 6172 6e2e 0a0a 2323 2320 6073  qttwarn...### `s
-00016200: 716c 6974 6560 0a0a 5468 6520 6073 716c  qlite`..The `sql
-00016210: 6974 6560 2070 6c75 6769 6e20 6372 6561  ite` plugin crea
-00016220: 7465 7320 6120 7461 626c 6520 696e 2074  tes a table in t
-00016230: 6865 2064 6174 6162 6173 6520 6669 6c65  he database file
-00016240: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
-00016250: 6520 7461 7267 6574 732c 0a61 6e64 2063  e targets,.and c
-00016260: 7265 6174 6573 2061 2073 6368 656d 6120  reates a schema 
-00016270: 7769 7468 2061 2073 696e 676c 6520 636f  with a single co
-00016280: 6c75 6d6e 2063 616c 6c65 6420 6070 6179  lumn called `pay
-00016290: 6c6f 6164 6020 6f66 2074 7970 6520 6054  load` of type `T
-000162a0: 4558 5460 2e20 5f6d 7174 7477 6172 6e5f  EXT`. _mqttwarn_
-000162b0: 0a63 6f6d 6d69 7473 206d 6573 7361 6765  .commits message
-000162c0: 7320 726f 7574 6564 2074 6f20 7375 6368  s routed to such
-000162d0: 2061 2074 6172 6765 7420 696d 6d65 6469   a target immedi
-000162e0: 6174 656c 792e 0a0a 6060 6069 6e69 0a5b  ately...```ini.[
-000162f0: 636f 6e66 6967 3a73 716c 6974 655d 0a74  config:sqlite].t
-00016300: 6172 6765 7473 203d 207b 0a20 2020 2020  argets = {.     
-00016310: 2020 2020 2020 2020 2020 2020 2020 2370                #p
-00016320: 6174 6820 2020 2020 2020 2023 7461 626c  ath        #tabl
-00016330: 656e 616d 650a 2020 2764 656d 6f74 6162  ename.  'demotab
-00016340: 6c65 2720 3a20 5b20 272f 746d 702f 6d2e  le' : [ '/tmp/m.
-00016350: 6462 272c 2020 276d 7174 7477 6172 6e27  db',  'mqttwarn'
-00016360: 2020 5d0a 2020 7d0a 6060 600a 0a23 2323    ].  }.```..###
-00016370: 2060 7371 6c69 7465 5f6a 736f 6e32 636f   `sqlite_json2co
-00016380: 6c73 600a 0a54 6865 2060 7371 6c69 7465  ls`..The `sqlite
-00016390: 5f6a 736f 6e32 636f 6c73 6020 706c 7567  _json2cols` plug
-000163a0: 696e 2063 7265 6174 6573 2061 2074 6162  in creates a tab
-000163b0: 6c65 2069 6e20 7468 6520 6461 7461 6261  le in the databa
-000163c0: 7365 2066 696c 6520 7370 6563 6966 6965  se file specifie
-000163d0: 6420 696e 2074 6865 2074 6172 6765 7473  d in the targets
-000163e0: 0a61 6e64 2063 7265 6174 6573 2061 2073  .and creates a s
-000163f0: 6368 656d 6120 6261 7365 6420 6f6e 2074  chema based on t
-00016400: 6865 204a 534f 4e20 7061 796c 6f61 642e  he JSON payload.
-00016410: 0a49 7420 7769 6c6c 2063 7265 6174 6520  .It will create 
-00016420: 6120 636f 6c75 6d6e 2066 6f72 2065 6163  a column for eac
-00016430: 6820 4a53 4f4e 2065 6e74 7279 2061 6e64  h JSON entry and
-00016440: 2072 7564 696d 656e 7461 7279 2074 7279   rudimentary try
-00016450: 2074 6f20 6465 7465 726d 696e 6520 6974   to determine it
-00016460: 7320 6461 7461 7479 7065 206f 6e20 6372  s datatype on cr
-00016470: 6561 7469 6f6e 2028 466c 6f61 7420 6f72  eation (Float or
-00016480: 2043 6861 7229 2e0a 0a41 7320 616e 2065   Char)...As an e
-00016490: 7861 6d70 6c65 2c20 7075 626c 6973 6869  xample, publishi
-000164a0: 6e67 2074 6869 7320 4a53 4f4e 2070 6179  ng this JSON pay
-000164b0: 6c6f 6164 3a0a 0a60 6060 0a6d 6f73 7175  load:..```.mosqu
-000164c0: 6974 746f 5f70 7562 202d 7420 7465 7374  itto_pub -t test
-000164d0: 2f68 656c 6c6f 202d 6d20 277b 2022 6e61  /hello -m '{ "na
-000164e0: 6d65 2220 3a20 2254 686f 7222 2c20 2246  me" : "Thor", "F
-000164f0: 6174 6865 7222 203a 2027 4f64 696e 272c  ather" : 'Odin',
-00016500: 2022 4167 6522 203a 2033 3020 7d27 0a60   "Age" : 30 }'.`
-00016510: 6060 0a0a 4120 7461 626c 6520 6173 2073  ``..A table as s
-00016520: 7461 7465 6420 696e 2074 6865 2063 6f6e  tated in the con
-00016530: 6669 6775 7261 7469 6f6e 2077 696c 6c20  figuration will 
-00016540: 6265 2063 7265 6174 6564 206f 6e20 7468  be created on th
-00016550: 6520 666c 7920 7769 7468 2074 6865 2066  e fly with the f
-00016560: 6f6c 6c6f 7769 6e67 2073 7472 7563 7475  ollowing structu
-00016570: 7265 2061 6e64 2063 6f6e 7465 6e74 3a0a  re and content:.
-00016580: 0a60 6060 0a2b 2d2d 2d2d 2d2d 2b2d 2d2d  .```.+------+---
-00016590: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2b0a 7c20  -----+------+.| 
-000165a0: 6e61 6d65 207c 2046 6174 6865 7220 7c20  name | Father | 
-000165b0: 4167 6520 207c 0a2b 2d2d 2d2d 2d2d 2b2d  Age  |.+------+-
-000165c0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2b0a  -------+------+.
-000165d0: 7c20 5468 6f72 207c 204f 6469 6e20 2020  | Thor | Odin   
-000165e0: 7c20 3330 2e30 207c 0a2b 2d2d 2d2d 2d2d  | 30.0 |.+------
-000165f0: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
-00016600: 2b0a 6060 600a 4e6f 2074 6162 6c65 2069  +.```.No table i
-00016610: 7320 6372 6561 7465 6420 6966 2074 6865  s created if the
-00016620: 2074 6162 6c65 206e 616d 6520 616c 7265   table name alre
-00016630: 6164 7920 6578 6973 7473 2e0a 0a20 5f6d  ady exists... _m
-00016640: 7174 7477 6172 6e5f 0a63 6f6d 6d69 7473  qttwarn_.commits
-00016650: 206d 6573 7361 6765 7320 726f 7574 6564   messages routed
-00016660: 2074 6f20 7375 6368 2061 2074 6172 6765   to such a targe
-00016670: 7420 696d 6d65 6469 6174 656c 792e 0a0a  t immediately...
-00016680: 6060 6069 6e69 0a5b 636f 6e66 6967 3a73  ```ini.[config:s
-00016690: 716c 6974 655f 6a73 6f6e 3263 6f6c 735d  qlite_json2cols]
-000166a0: 0a74 6172 6765 7473 203d 207b 0a20 2020  .targets = {.   
-000166b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166c0: 2370 6174 6820 2020 2020 2020 2023 7461  #path        #ta
-000166d0: 626c 656e 616d 650a 2020 2764 656d 6f74  blename.  'demot
-000166e0: 6162 6c65 2720 3a20 5b20 272f 746d 702f  able' : [ '/tmp/
-000166f0: 6d2e 6462 272c 2020 276d 7174 7477 6172  m.db',  'mqttwar
-00016700: 6e27 2020 5d0a 2020 7d0a 6060 600a 0a23  n'  ].  }.```..#
-00016710: 2323 2060 7371 6c69 7465 5f74 696d 6573  ## `sqlite_times
-00016720: 7461 6d70 600a 0a54 6865 2060 7371 6c69  tamp`..The `sqli
-00016730: 7465 5f74 696d 6573 7461 6d70 6020 706c  te_timestamp` pl
-00016740: 7567 696e 2077 6f72 6b73 206a 7573 7420  ugin works just 
-00016750: 6c69 6b65 2074 6865 2027 7371 6c69 7465  like the 'sqlite
-00016760: 2720 706c 7567 696e 2c20 6275 7420 6974  ' plugin, but it
-00016770: 2063 7265 6174 6573 2033 2063 6f6c 756d   creates 3 colum
-00016780: 6e73 3a20 6964 2c20 7061 796c 6f61 6420  ns: id, payload 
-00016790: 616e 6420 7469 6d65 7374 616d 702e 0a54  and timestamp..T
-000167a0: 6865 2069 6420 6973 2074 6865 2074 6162  he id is the tab
-000167b0: 6c65 2069 6e64 6578 2061 6e64 2074 6865  le index and the
-000167c0: 2074 696d 6573 7461 6d70 2069 7320 7468   timestamp is th
-000167d0: 6520 696e 7365 7274 696f 6e20 6461 7465  e insertion date
-000167e0: 2061 6e64 2074 696d 6520 696e 2073 6563   and time in sec
-000167f0: 6f6e 6473 2e0a 0a60 6060 696e 690a 5b63  onds...```ini.[c
-00016800: 6f6e 6669 673a 7371 6c69 7465 5f74 696d  onfig:sqlite_tim
-00016810: 6573 7461 6d70 5d0a 7461 7267 6574 7320  estamp].targets 
-00016820: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00016830: 2020 2020 2020 2023 7061 7468 2020 2020         #path    
-00016840: 2020 2020 2374 6162 6c65 6e61 6d65 0a20      #tablename. 
-00016850: 2027 6465 6d6f 7461 626c 6527 203a 205b   'demotable' : [
-00016860: 2027 2f74 6d70 2f6d 2e64 6227 2c20 2027   '/tmp/m.db',  '
-00016870: 6d71 7474 7761 726e 2720 205d 0a20 207d  mqttwarn'  ].  }
-00016880: 0a60 6060 0a0a 2323 2320 6073 6d74 7060  .```..### `smtp`
-00016890: 0a0a 5468 6520 6073 6d74 7060 2073 6572  ..The `smtp` ser
-000168a0: 7669 6365 2062 6173 6963 616c 6c79 2069  vice basically i
-000168b0: 6d70 6c65 6d65 6e74 7320 616e 204d 5154  mplements an MQT
-000168c0: 5420 746f 2053 4d54 5020 6761 7465 7761  T to SMTP gatewa
-000168d0: 7920 7768 6963 6820 6e65 6564 730a 636f  y which needs.co
-000168e0: 6e66 6967 7572 6174 696f 6e2e 0a0a 6060  nfiguration...``
-000168f0: 6069 6e69 0a5b 636f 6e66 6967 3a73 6d74  `ini.[config:smt
-00016900: 705d 0a73 6572 7665 7220 203d 2020 276c  p].server  =  'l
-00016910: 6f63 616c 686f 7374 3a32 3527 0a73 656e  ocalhost:25'.sen
-00016920: 6465 7220 203d 2020 224d 5154 5477 6172  der  =  "MQTTwar
-00016930: 6e20 3c6a 706d 406c 6f63 616c 686f 7374  n <jpm@localhost
-00016940: 3e22 0a75 7365 726e 616d 6520 203d 2020  >".username  =  
-00016950: 4e6f 6e65 0a70 6173 7377 6f72 6420 203d  None.password  =
-00016960: 2020 4e6f 6e65 0a73 7461 7274 746c 7320    None.starttls 
-00016970: 203d 2020 4661 6c73 650a 2320 4f70 7469   =  False.# Opti
-00016980: 6f6e 616c 2073 656e 6420 6d73 6720 6173  onal send msg as
-00016990: 2068 746d 6c20 6f72 206f 6e6c 7920 706c   html or only pl
-000169a0: 6169 6e20 7465 7874 0a68 746d 6c6d 7367  ain text.htmlmsg
-000169b0: 2020 203d 2020 4661 6c73 650a 7461 7267     =  False.targ
-000169c0: 6574 7320 3d20 7b0a 2020 2020 276c 6f63  ets = {.    'loc
-000169d0: 616c 6a27 2020 2020 203a 205b 2027 6a70  alj'     : [ 'jp
-000169e0: 6d40 6c6f 6361 6c68 6f73 7427 205d 2c0a  m@localhost' ],.
-000169f0: 2020 2020 2773 7065 6369 616c 2720 2020      'special'   
-00016a00: 203a 205b 2027 6265 6e40 676d 6169 6c27   : [ 'ben@gmail'
-00016a10: 2c20 2773 757a 6965 4065 7861 6d70 6c65  , 'suzie@example
-00016a20: 2e6e 6574 2720 5d0a 2020 2020 7d0a 6060  .net' ].    }.``
-00016a30: 600a 0a54 6172 6765 7473 206d 6179 2063  `..Targets may c
-00016a40: 6f6e 7461 696e 206d 6f72 6520 7468 616e  ontain more than
-00016a50: 206f 6e65 2072 6563 6970 6965 6e74 2c20   one recipient, 
-00016a60: 696e 2077 6869 6368 2063 6173 6520 616c  in which case al
-00016a70: 6c20 7370 6563 6966 6965 640a 7265 6369  l specified.reci
-00016a80: 7069 656e 7473 2067 6574 2074 6865 206d  pients get the m
-00016a90: 6573 7361 6765 2e0a 0a7c 2054 6f70 6963  essage...| Topic
-00016aa0: 206f 7074 696f 6e20 207c 2020 4d2f 4f20   option  |  M/O 
-00016ab0: 2020 7c20 4465 7363 7269 7074 696f 6e20    | Description 
-00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ad0: 2020 2020 2020 2020 2020 207c 0a7c 202d             |.| -
-00016ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c 203a  ------------ | :
-00016af0: 2d2d 2d2d 3a20 7c20 2d2d 2d2d 2d2d 2d2d  ----: | --------
-00016b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c  -------------- |
-00016b20: 0a7c 2060 7469 746c 6560 2020 2020 2020  .| `title`      
-00016b30: 207c 2020 204f 2020 2020 7c20 652d 6d61   |   O    | e-ma
-00016b40: 696c 2073 7562 6a65 6374 2e20 2864 666c  il subject. (dfl
-00016b50: 743a 2060 6d71 7474 7761 726e 206e 6f74  t: `mqttwarn not
-00016b60: 6966 6963 6174 696f 6e60 2920 7c0a 0a23  ification`) |..#
-00016b70: 2323 2060 7373 6860 0a0a 5468 6520 6073  ## `ssh`..The `s
-00016b80: 7368 6020 7365 7276 6963 6520 6361 6e20  sh` service can 
-00016b90: 7275 6e20 636f 6d6d 616e 6473 206f 7665  run commands ove
-00016ba0: 7220 7373 682e 0a49 6620 626f 7468 2075  r ssh..If both u
-00016bb0: 7365 7220 616e 6420 7061 7373 776f 7264  ser and password
-00016bc0: 2061 7265 2064 6566 696e 6564 2069 6e20   are defined in 
-00016bd0: 7468 6520 636f 6e66 6967 2c20 7468 6579  the config, they
-00016be0: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
-00016bf0: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
-00016c00: 686f 7374 2e0a 4966 2062 6f74 6820 7573  host..If both us
-00016c10: 6572 2061 6e64 2070 6173 7377 6f72 6420  er and password 
-00016c20: 6172 6520 2a6e 6f74 2a20 6465 6669 6e65  are *not* define
-00016c30: 6420 696e 2074 6865 2063 6f6e 6669 672c  d in the config,
-00016c40: 2074 6865 2073 6572 7669 6365 2077 696c   the service wil
-00016c50: 6c20 7061 7273 6520 7468 6520 7573 6572  l parse the user
-00016c60: 2773 0a73 7368 2063 6f6e 6669 6720 6669  's.ssh config fi
-00016c70: 6c65 2074 6f20 7365 6520 7768 6963 6820  le to see which 
-00016c80: 6b65 7920 2849 6465 6e74 6974 7946 696c  key (IdentityFil
-00016c90: 6529 2074 6f20 7573 653b 2069 7420 7769  e) to use; it wi
-00016ca0: 6c6c 2061 6c73 6f20 6c6f 6f6b 2066 6f72  ll also look for
-00016cb0: 2055 7365 7220 616e 6420 506f 7274 0a69   User and Port.i
-00016cc0: 6e20 7468 6973 2066 696c 652e 0a0a 4966  n this file...If
-00016cd0: 2075 7369 6e67 2061 206b 6579 2c20 6f6e   using a key, on
-00016ce0: 6c79 2074 6865 2068 6f73 7420 6973 202a  ly the host is *
-00016cf0: 7265 7175 6972 6564 2a2e 0a0a 5468 6520  required*...The 
-00016d00: 6f75 7470 7574 2069 7320 6967 6e6f 7265  output is ignore
-00016d10: 6420 666f 7220 6e6f 772e 0a0a 4e6f 7465  d for now...Note
-00016d20: 3a20 7573 696e 6720 7468 6973 206d 6f64  : using this mod
-00016d30: 756c 6520 6c65 7473 2079 6f75 2073 7065  ule lets you spe
-00016d40: 6369 6679 2061 2075 7365 726e 616d 6520  cify a username 
-00016d50: 616e 6420 6120 7061 7373 776f 7264 2077  and a password w
-00016d60: 6869 6368 2063 616e 2062 6520 7573 6564  hich can be used
-00016d70: 2074 6f20 6c6f 6769 6e20 746f 2074 6865   to login to the
-00016d80: 2074 6172 6765 7420 7379 7374 656d 2e20   target system. 
-00016d90: 4173 2073 7563 682c 2079 6f75 7220 606d  As such, your `m
-00016da0: 7174 7477 6172 6e2e 696e 6960 2063 6f6e  qttwarn.ini` con
-00016db0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00016dc0: 7368 6f75 6c64 2062 6520 7765 6c6c 2070  should be well p
-00016dd0: 726f 7465 6374 6564 2066 726f 6d20 7072  rotected from pr
-00016de0: 7969 6e67 2065 7965 7321 2028 5468 6973  ying eyes! (This
-00016df0: 2061 7070 6c69 6573 2067 656e 6572 616c   applies general
-00016e00: 6c79 2c20 666f 7220 6f74 6865 7220 7461  ly, for other ta
-00016e10: 7267 6574 2073 7065 6369 6669 6361 7469  rget specificati
-00016e20: 6f6e 7320 7769 7468 2063 7265 6465 6e74  ons with credent
-00016e30: 6961 6c73 2061 7320 7765 6c6c 2e29 0a0a  ials as well.)..
-00016e40: 6060 6069 6e69 0a5b 636f 6e66 6967 3a73  ```ini.[config:s
-00016e50: 7368 5d0a 686f 7374 2020 3d20 2731 3932  sh].host  = '192
-00016e60: 2e31 3638 2e31 2e31 270a 706f 7274 2020  .168.1.1'.port  
-00016e70: 3d20 3232 0a75 7365 7220 203d 2027 7573  = 22.user  = 'us
-00016e80: 6572 6e61 6d65 270a 7061 7373 2020 3d20  ername'.pass  = 
-00016e90: 2770 6173 7377 6f72 6427 0a74 6172 6765  'password'.targe
-00016ea0: 7473 203d 207b 0a09 0927 7330 3127 2020  ts = {...'s01'  
-00016eb0: 2020 3a20 5b20 2763 6f6d 6d61 6e64 2077    : [ 'command w
-00016ec0: 6974 6820 6f6e 6520 7375 6273 7469 7475  ith one substitu
-00016ed0: 7469 6f6e 2025 7327 205d 2c0a 0909 2773  tion %s' ],...'s
-00016ee0: 3032 2720 2020 203a 205b 2027 636f 6d6d  02'    : [ 'comm
-00016ef0: 616e 6420 7769 7468 2074 776f 2073 7562  and with two sub
-00016f00: 7374 6974 7574 696f 6e73 2025 735f 5f25  stitutions %s__%
-00016f10: 7327 205d 0a20 2020 207d 0a0a 5b73 7368  s' ].    }..[ssh
-00016f20: 2f2b 5d0a 666f 726d 6174 203d 207b 6172  /+].format = {ar
-00016f30: 6773 7d0a 7461 7267 6574 7320 3d20 7373  gs}.targets = ss
-00016f40: 683a 7330 310a 0a5b 6475 616c 7373 682f  h:s01..[dualssh/
-00016f50: 2b5d 0a66 6f72 6d61 7420 3d20 7b61 7267  +].format = {arg
-00016f60: 737d 0a74 6172 6765 7473 203d 2073 7368  s}.targets = ssh
-00016f70: 3a73 3032 0a60 6060 0a0a 5461 7267 6574  :s02.```..Target
-00016f80: 7320 6d61 7920 636f 6e74 6169 6e20 4f4e  s may contain ON
-00016f90: 4520 636f 6d6d 616e 642e 0a0a 606d 6f73  E command...`mos
-00016fa0: 7175 6974 746f 5f70 7562 202d 7420 6475  quitto_pub -t du
-00016fb0: 616c 7373 682f 7465 7374 202d 6d20 277b  alssh/test -m '{
-00016fc0: 2022 6172 6773 2220 3a20 5b22 7465 7374   "args" : ["test
-00016fd0: 222c 2274 6573 7432 225d 207d 2760 0a0a  ","test2"] }'`..
-00016fe0: 0a23 2323 2060 7379 736c 6f67 600a 0a54  .### `syslog`..T
-00016ff0: 6865 2060 7379 736c 6f67 6020 7365 7276  he `syslog` serv
-00017000: 6963 6520 7472 616e 7366 6572 7320 4d51  ice transfers MQ
-00017010: 5454 206d 6573 7361 6765 7320 746f 2061  TT messages to a
-00017020: 206c 6f63 616c 2073 7973 6c6f 6720 7365   local syslog se
-00017030: 7276 6572 2e0a 0a60 6060 696e 690a 5b63  rver...```ini.[c
-00017040: 6f6e 6669 673a 7379 736c 6f67 5d0a 7461  onfig:syslog].ta
-00017050: 7267 6574 7320 3d20 7b0a 2020 2020 2020  rgets = {.      
-00017060: 2020 2020 2020 2020 2320 6661 6369 6c69          # facili
-00017070: 7479 2020 2020 6f70 7469 6f6e 0a20 2020  ty    option.   
-00017080: 2027 7573 6572 2720 2020 3a20 5b27 7573   'user'   : ['us
-00017090: 6572 272c 2020 2020 2027 7069 6427 5d2c  er',     'pid'],
-000170a0: 0a20 2020 2027 6b65 726e 656c 2720 3a20  .    'kernel' : 
-000170b0: 5b27 6b65 726e 656c 272c 2020 2027 7069  ['kernel',   'pi
-000170c0: 6427 5d0a 2020 2020 7d0a 6060 600a 0a7c  d'].    }.```..|
-000170d0: 2054 6f70 6963 206f 7074 696f 6e20 207c   Topic option  |
-000170e0: 2020 4d2f 4f20 2020 7c20 4465 7363 7269    M/O   | Descri
-000170f0: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
-00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017110: 207c 0a7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d   |.| -----------
-00017120: 2d2d 207c 203a 2d2d 2d2d 3a20 7c20 2d2d  -- | :----: | --
-00017130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017150: 2d2d 2d2d 207c 0a7c 2060 7469 746c 6560  ---- |.| `title`
-00017160: 2020 2020 2020 207c 2020 204f 2020 2020         |   O    
-00017170: 7c20 6170 706c 6963 6174 696f 6e20 7469  | application ti
-00017180: 746c 6520 2864 666c 743a 2060 6d71 7474  tle (dflt: `mqtt
-00017190: 7761 726e 6029 2020 207c 0a7c 2060 7072  warn`)   |.| `pr
-000171a0: 696f 7269 7479 6020 2020 207c 2020 204f  iority`    |   O
-000171b0: 2020 2020 7c20 6c6f 6720 6c65 7665 6c20      | log level 
-000171c0: 2864 666c 743a 202d 3129 2020 2020 2020  (dflt: -1)      
-000171d0: 2020 2020 2020 2020 2020 2020 207c 0a0a               |..
-000171e0: 5768 6572 6520 6070 7269 6f72 6974 7960  Where `priority`
-000171f0: 2063 616e 2062 6520 6265 7477 6565 6e20   can be between 
-00017200: 2d32 2061 6e64 2035 2061 6e64 206d 6170  -2 and 5 and map
-00017210: 7320 746f 2060 7379 736c 6f67 6020 6c65  s to `syslog` le
-00017220: 7665 6c73 2062 793b 0a0a 7c20 5072 696f  vels by;..| Prio
-00017230: 7269 7479 207c 2053 7973 6c6f 6720 4c6f  rity | Syslog Lo
-00017240: 6720 4c65 7665 6c20 7c0a 7c20 2d2d 2d2d  g Level |.| ----
-00017250: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
-00017260: 2d2d 2d2d 2d2d 2d20 7c0a 7c20 2d32 2020  ------- |.| -2  
-00017270: 2020 2020 207c 204c 4f47 5f44 4542 5547       | LOG_DEBUG
-00017280: 2020 2020 2020 2020 7c0a 7c20 2d31 2020          |.| -1  
-00017290: 2020 2020 207c 204c 4f47 5f49 4e46 4f20       | LOG_INFO 
-000172a0: 2020 2020 2020 2020 7c0a 7c20 3020 2020          |.| 0   
-000172b0: 2020 2020 207c 204c 4f47 5f4e 4f54 4943       | LOG_NOTIC
-000172c0: 4520 2020 2020 2020 7c0a 7c20 3120 2020  E       |.| 1   
-000172d0: 2020 2020 207c 204c 4f47 5f57 4152 4e49       | LOG_WARNI
-000172e0: 4e47 2020 2020 2020 7c0a 7c20 3220 2020  NG      |.| 2   
-000172f0: 2020 2020 207c 204c 4f47 5f45 5252 2020       | LOG_ERR  
-00017300: 2020 2020 2020 2020 7c0a 7c20 3320 2020          |.| 3   
-00017310: 2020 2020 207c 204c 4f47 5f43 5249 5420       | LOG_CRIT 
-00017320: 2020 2020 2020 2020 7c0a 7c20 3420 2020          |.| 4   
-00017330: 2020 2020 207c 204c 4f47 5f41 4c45 5254       | LOG_ALERT
-00017340: 2020 2020 2020 2020 7c0a 7c20 3520 2020          |.| 5   
-00017350: 2020 2020 207c 204c 4f47 5f45 4d45 5247       | LOG_EMERG
-00017360: 2020 2020 2020 2020 7c0a 0a60 6060 0a41          |..```.A
-00017370: 7072 2032 3220 3132 3a34 323a 3432 206d  pr 22 12:42:42 m
-00017380: 7174 7465 7374 3031 3920 6d71 7474 7761  qttest019 mqttwa
-00017390: 726e 5b39 3438 345d 3a20 4469 736b 2075  rn[9484]: Disk u
-000173a0: 7469 6c69 7a61 7469 6f6e 3a20 3934 250a  tilization: 94%.
-000173b0: 6060 600a 0a23 2323 2060 7465 6c65 6772  ```..### `telegr
-000173c0: 616d 600a 0a54 6869 7320 6973 2074 6f20  am`..This is to 
-000173d0: 7365 6e64 206d 6573 7361 6765 7320 6173  send messages as
-000173e0: 2061 2042 6f74 2074 6f20 6120 5b54 656c   a Bot to a [Tel
-000173f0: 6567 7261 6d5d 2868 7474 7073 3a2f 2f74  egram](https://t
-00017400: 656c 6567 7261 6d2e 6f72 6729 2063 6861  elegram.org) cha
-00017410: 742e 2046 6972 7374 2073 6574 2075 7020  t. First set up 
-00017420: 6120 426f 7420 616e 6420 6f62 7461 696e  a Bot and obtain
-00017430: 2069 7473 2061 7574 6865 6e74 6963 6174   its authenticat
-00017440: 696f 6e20 746f 6b65 6e20 7768 6963 6820  ion token which 
-00017450: 796f 7520 6164 6420 746f 205f 6d71 7474  you add to _mqtt
-00017460: 7761 726e 5f27 7320 636f 6e66 6967 7572  warn_'s configur
-00017470: 6174 696f 6e2e 2059 6f75 276c 6c20 616c  ation. You'll al
-00017480: 736f 206e 6565 6420 746f 2073 7461 7274  so need to start
-00017490: 2061 2063 6861 7420 7769 7468 2074 6869   a chat with thi
-000174a0: 7320 626f 7420 736f 2069 7427 7320 6162  s bot so it's ab
-000174b0: 6c65 2074 6f20 636f 6d6d 756e 6963 6174  le to communicat
-000174c0: 6520 7769 7468 2070 6172 7469 6375 6c61  e with particula
-000174d0: 7220 7573 6572 2e0a 0a4f 7074 696f 6e61  r user...Optiona
-000174e0: 6c6c 7920 796f 7520 6361 6e20 7370 6563  lly you can spec
-000174f0: 6966 7920 6070 6172 7365 5f6d 6f64 6560  ify `parse_mode`
-00017500: 2077 6869 6368 2077 696c 6c20 6265 2075   which will be u
-00017510: 7365 6420 6475 7269 6e67 206d 6573 7361  sed during messa
-00017520: 6765 2073 656e 6469 6e67 2e20 506c 6561  ge sending. Plea
-00017530: 7365 2c20 6368 6563 6b20 5b64 6f63 735d  se, check [docs]
-00017540: 2868 7474 7073 3a2f 2f63 6f72 652e 7465  (https://core.te
-00017550: 6c65 6772 616d 2e6f 7267 2f62 6f74 732f  legram.org/bots/
-00017560: 6170 6923 666f 726d 6174 7469 6e67 2d6f  api#formatting-o
-00017570: 7074 696f 6e73 2920 666f 7220 6164 6469  ptions) for addi
-00017580: 7469 6f6e 616c 2069 6e66 6f72 6d61 7469  tional informati
-00017590: 6f6e 2e0a 0a49 6620 796f 7520 6861 7665  on...If you have
-000175a0: 2074 6865 2060 6368 6174 4964 6020 796f   the `chatId` yo
-000175b0: 7520 6361 6e20 7370 6563 6966 7920 7468  u can specify th
-000175c0: 6520 7465 6c65 6772 616d 2073 6572 7669  e telegram servi
-000175d0: 6365 2074 6f20 7573 6520 7468 6520 6368  ce to use the ch
-000175e0: 6174 4964 2064 6972 6563 746c 792e 2057  atId directly. W
-000175f0: 6172 6e69 6e67 2c20 7468 6973 2077 696c  arning, this wil
-00017600: 6c20 6e65 6564 2074 6f20 6265 2074 6865  l need to be the
-00017610: 2063 6173 6520 666f 7220 616c 6c20 7468   case for all th
-00017620: 6520 7461 7267 6574 7320 696e 2074 6869  e targets in thi
-00017630: 7320 6e6f 7469 6669 6572 210a 0a51 7569  s notifier!..Qui
-00017640: 636b 6573 7420 7761 7920 746f 2067 6574  ckest way to get
-00017650: 2074 6865 2060 6368 6174 6964 6020 6973   the `chatid` is
-00017660: 2062 7920 7669 7369 7469 6e67 2074 6869   by visiting thi
-00017670: 7320 5552 4c20 2869 6e73 6572 7420 796f  s URL (insert yo
-00017680: 7572 2061 7069 206b 6579 293a 2068 7474  ur api key): htt
-00017690: 7073 3a2f 2f61 7069 2e74 656c 6567 7261  ps://api.telegra
-000176a0: 6d2e 6f72 672f 626f 7459 4f55 525f 4150  m.org/botYOUR_AP
-000176b0: 495f 544f 4b45 4e2f 6765 7455 7064 6174  I_TOKEN/getUpdat
-000176c0: 6573 2061 6e64 2067 6574 7469 6e67 2074  es and getting t
-000176d0: 6865 2069 6420 6672 6f6d 2074 6865 2022  he id from the "
-000176e0: 6672 6f6d 2220 7365 6374 696f 6e2e 0a0a  from" section...
-000176f0: 436f 6e66 6967 7572 6520 7468 6520 6074  Configure the `t
-00017700: 656c 6567 7261 6d60 2073 6572 7669 6365  elegram` service
-00017710: 2057 4954 484f 5554 2063 6861 7449 643a   WITHOUT chatId:
-00017720: 0a0a 6060 6069 6e69 0a5b 636f 6e66 6967  ..```ini.[config
-00017730: 3a74 656c 6567 7261 6d5d 0a74 696d 656f  :telegram].timeo
-00017740: 7574 203d 2036 300a 7061 7273 655f 6d6f  ut = 60.parse_mo
-00017750: 6465 203d 2027 4d61 726b 646f 776e 270a  de = 'Markdown'.
-00017760: 746f 6b65 6e20 3d20 276d 6d6d 6d6d 6d6d  token = 'mmmmmmm
-00017770: 6d6d 3a41 4141 4141 4141 4141 4141 4141  mm:AAAAAAAAAAAAA
-00017780: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
-00017790: 4141 4141 4141 270a 7461 7267 6574 7320  AAAAAA'.targets 
-000177a0: 3d20 7b0a 2020 2023 2020 2020 2020 2020  = {.   #        
-000177b0: 4669 7273 7420 4e61 6d65 206f 7220 4075  First Name or @u
-000177c0: 7365 726e 616d 6520 6f72 2023 6368 6174  sername or #chat
-000177d0: 5f69 640a 2020 2027 6a30 3127 203a 205b  _id.   'j01' : [
-000177e0: 2027 4669 7273 7420 4e61 6d65 2720 5d2c   'First Name' ],
-000177f0: 0a20 2020 276a 3032 2720 3a20 5b20 2740  .   'j02' : [ '@
-00017800: 7573 6572 6e61 6d65 2720 5d2c 0a20 2020  username' ],.   
-00017810: 276a 3033 2720 3a20 5b20 2723 6368 6174  'j03' : [ '#chat
-00017820: 5f69 6427 205d 0a20 2020 207d 0a60 6060  _id' ].    }.```
-00017830: 0a43 6f6e 6669 6775 7265 2074 6865 2060  .Configure the `
-00017840: 7465 6c65 6772 616d 6020 7365 7276 6963  telegram` servic
-00017850: 6520 5749 5448 2063 6861 7469 643a 0a60  e WITH chatid:.`
-00017860: 6060 696e 690a 5b63 6f6e 6669 673a 7465  ``ini.[config:te
-00017870: 6c65 6772 616d 5d0a 7469 6d65 6f75 7420  legram].timeout 
-00017880: 3d20 3630 0a70 6172 7365 5f6d 6f64 6520  = 60.parse_mode 
-00017890: 3d20 274d 6172 6b64 6f77 6e27 0a74 6f6b  = 'Markdown'.tok
-000178a0: 656e 203d 2027 6d6d 6d6d 6d6d 6d6d 6d3a  en = 'mmmmmmmmm:
-000178b0: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
-000178c0: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
-000178d0: 4141 4127 0a75 7365 5f63 6861 745f 6964  AAA'.use_chat_id
-000178e0: 203d 2054 7275 650a 7461 7267 6574 7320   = True.targets 
-000178f0: 3d20 7b0a 2020 2020 2320 2020 2020 2020  = {.    #       
-00017900: 6368 6174 4964 2028 696e 2071 756f 7465  chatId (in quote
-00017910: 7329 0a20 2020 2027 6a30 3127 203a 205b  s).    'j01' : [
-00017920: 2731 3233 3435 3637 3839 275d 0a20 2020  '123456789'].   
-00017930: 207d 0a60 6060 0a0a 506f 7373 6962 6c65   }.```..Possible
-00017940: 2069 7373 7565 3a0a 0a2a 2049 6620 4669   issue:..* If Fi
-00017950: 7273 7420 6e61 6d65 206f 7220 4075 7365  rst name or @use
-00017960: 726e 616d 6520 7761 7320 7370 6563 6966  rname was specif
-00017970: 6965 6420 6173 2074 6172 6765 742c 2070  ied as target, p
-00017980: 6c75 6769 6e20 7769 6c6c 2063 616c 6c20  lugin will call 
-00017990: 5b67 6574 5570 6461 7465 735d 2868 7474  [getUpdates](htt
-000179a0: 7073 3a2f 2f63 6f72 652e 7465 6c65 6772  ps://core.telegr
-000179b0: 616d 2e6f 7267 2f62 6f74 732f 6170 6923  am.org/bots/api#
-000179c0: 6765 7475 7064 6174 6573 2920 746f 2067  getupdates) to g
-000179d0: 6574 2060 6368 6174 5f69 6460 2062 7574  et `chat_id` but
-000179e0: 2074 6869 7320 6361 6c6c 2072 6574 7572   this call retur
-000179f0: 6e73 206f 6e6c 7920 6c61 7374 2031 3030  ns only last 100
-00017a00: 206d 6573 7361 6765 733b 2069 6620 5f79   messages; if _y
-00017a10: 6f75 5f20 6861 7665 6e27 7420 7370 6f6b  ou_ haven't spok
-00017a20: 656e 2074 6f20 796f 7572 2042 6f74 2072  en to your Bot r
-00017a30: 6563 656e 746c 7920 6974 206d 6179 2077  ecently it may w
-00017a40: 656c 6c20 6265 2070 6f73 7369 626c 6520  ell be possible 
-00017a50: 7765 2063 616e 2774 2066 696e 6420 7468  we can't find th
-00017a60: 6520 5f63 6861 742d 6964 5f20 6173 736f  e _chat-id_ asso
-00017a70: 6369 6174 6564 2077 6974 6820 5f79 6f75  ciated with _you
-00017a80: 5f2e 2049 6620 6368 6174 5f69 6420 6973  _. If chat_id is
-00017a90: 206b 6e6f 776e 2c20 6974 2063 616e 2062   known, it can b
-00017aa0: 6520 7365 7420 6173 2074 6172 6765 7420  e set as target 
-00017ab0: 7573 696e 6720 6023 6020 7369 676e 2e0a  using `#` sign..
-00017ac0: 0a21 5b54 656c 6567 7261 6d5d 2861 7373  .![Telegram](ass
-00017ad0: 6574 732f 7465 6c65 6772 616d 2e70 6e67  ets/telegram.png
-00017ae0: 290a 0a23 2323 2060 7468 696e 6773 7065  )..### `thingspe
-00017af0: 616b 600a 0a54 6865 2060 7468 696e 6773  ak`..The `things
-00017b00: 7065 616b 6020 7365 7276 6963 6520 7075  peak` service pu
-00017b10: 626c 6973 6865 7320 6461 7461 2074 6f20  blishes data to 
-00017b20: 7468 696e 6773 7065 616b 2e63 6f6d 2075  thingspeak.com u
-00017b30: 7369 6e67 2074 6865 2074 6869 6e67 7370  sing the thingsp
-00017b40: 6561 6b20 4150 492e 0a0a 6060 6069 6e69  eak API...```ini
-00017b50: 0a5b 636f 6e66 6967 3a74 6869 6e67 7370  .[config:thingsp
-00017b60: 6561 6b5d 0a74 6172 6765 7473 203d 207b  eak].targets = {
-00017b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b80: 2020 2020 2341 5049 2057 5249 5445 204b      #API WRITE K
-00017b90: 4559 2020 2020 2020 2066 6965 6c64 2020  EY       field  
-00017ba0: 2020 2020 6f70 7469 6f6e 616c 2062 7569      optional bui
-00017bb0: 6c64 6461 7461 3d74 7275 652f 6661 6c73  lddata=true/fals
-00017bc0: 650a 2020 2020 2766 6965 6c64 3127 2020  e.    'field1'  
-00017bd0: 203a 205b 2027 5858 5959 5a5a 5858 5959   : [ 'XXYYZZXXYY
-00017be0: 5a5a 5858 5959 272c 2027 6669 656c 6431  ZZXXYY', 'field1
-00017bf0: 2720 2c20 2774 7275 6527 205d 2c0a 2020  ' , 'true' ],.  
-00017c00: 2020 2766 6965 6c64 3227 2020 203a 205b    'field2'   : [
-00017c10: 2027 5858 5959 5a5a 5858 5959 5a5a 5858   'XXYYZZXXYYZZXX
-00017c20: 5959 272c 2027 6669 656c 6432 2720 5d2c  YY', 'field2' ],
-00017c30: 0a20 2020 2027 636f 6d70 6f73 6974 6527  .    'composite'
-00017c40: 3a20 5b20 2758 5859 595a 5a58 5859 595a  : [ 'XXYYZZXXYYZ
-00017c50: 5a58 5859 5927 2c20 5b20 2774 656d 7027  ZXXYY', [ 'temp'
-00017c60: 2c20 2768 756d 2720 5d20 5d0a 2020 7d0a  , 'hum' ] ].  }.
-00017c70: 6060 600a 5573 696e 6720 6062 7569 6c64  ```.Using `build
-00017c80: 6461 7461 3d74 7275 6560 2079 6f75 2063  data=true` you c
-00017c90: 616e 2062 7569 6c64 2061 6e20 7570 6461  an build an upda
-00017ca0: 7465 2077 6974 6820 6d75 6c74 6970 6c65  te with multiple
-00017cb0: 2066 6965 6c64 7320 696e 206f 6e65 2075   fields in one u
-00017cc0: 7064 6174 652e 2055 7369 6e67 2074 6869  pdate. Using thi
-00017cd0: 7320 6675 6e63 7469 6f6e 206e 6f20 6469  s function no di
-00017ce0: 7265 6374 2075 7064 6174 6520 6973 2070  rect update is p
-00017cf0: 6572 666f 726d 6564 2e20 4f6e 6c79 2077  erformed. Only w
-00017d00: 6974 6820 7468 6520 6e65 7874 2075 7064  ith the next upd
-00017d10: 6174 6520 7769 7468 6f75 7420 6275 696c  ate without buil
-00017d20: 6464 6174 613d 7472 7565 2061 6c6c 2065  ddata=true all e
-00017d30: 6e74 7269 6573 2061 7265 2073 656e 7420  ntries are sent 
-00017d40: 2865 2e67 2e20 7768 656e 206d 756c 7469  (e.g. when multi
-00017d50: 706c 6520 7365 6e73 6f72 7320 6172 6520  ple sensors are 
-00017d60: 7570 6461 7469 6e67 2064 6966 6665 7265  updating differe
-00017d70: 6e74 2074 6f70 6963 732c 2074 6865 6e20  nt topics, then 
-00017d80: 796f 7520 6361 6e20 646f 2074 6865 2062  you can do the b
-00017d90: 7569 6c64 2074 6865 2064 6174 6120 616e  uild the data an
-00017da0: 6420 7375 626d 6974 2077 6865 6e20 7468  d submit when th
-00017db0: 6520 6c61 7374 2073 656e 736f 7220 6973  e last sensor is
-00017dc0: 2073 656e 6469 6e67 2074 6865 2064 6174   sending the dat
-00017dd0: 6129 2e0a 0a53 7570 706c 7920 616e 206f  a)...Supply an o
-00017de0: 7264 6572 6564 206c 6973 7420 6f66 206d  rdered list of m
-00017df0: 6573 7361 6765 2064 6174 6120 6669 656c  essage data fiel
-00017e00: 6420 6e61 6d65 7320 746f 2065 7874 7261  d names to extra
-00017e10: 6374 2073 6576 6572 616c 2076 616c 7565  ct several value
-00017e20: 7320 6672 6f6d 2061 2073 696e 676c 6520  s from a single 
-00017e30: 6d65 7373 6167 6520 2865 2e67 2e20 607b  message (e.g. `{
-00017e40: 2022 7465 6d70 223a 2031 302c 2022 6875   "temp": 10, "hu
-00017e50: 6d22 3a20 3737 207d 6029 2e20 5661 6c75  m": 77 }`). Valu
-00017e60: 6573 2077 696c 6c20 6265 2061 7373 6967  es will be assig
-00017e70: 6e65 6420 746f 2066 6965 6c64 312c 2066  ned to field1, f
-00017e80: 6965 6c64 322c 2065 7463 2069 6e20 6f72  ield2, etc in or
-00017e90: 6465 722e 0a0a 4e6f 7465 3a20 5573 6520  der...Note: Use 
-00017ea0: 7468 6520 6669 656c 6420 6173 2070 6572  the field as per
-00017eb0: 2074 6865 2065 7861 6d70 6c65 2028 6c6f   the example (lo
-00017ec0: 7765 7220 6361 7365 2c20 6027 6669 656c  wer case, `'fiel
-00017ed0: 6431 2760 2077 6974 6820 7468 6520 6c61  d1'` with the la
-00017ee0: 7374 2064 6967 6974 2062 6569 6e67 2074  st digit being t
-00017ef0: 6865 2066 6965 6c64 206e 756d 6265 7229  he field number)
-00017f00: 2e0a 0a23 2323 2060 746f 6f74 7061 7374  ...### `tootpast
-00017f10: 6560 0a0a 5468 6520 6074 6f6f 7470 6173  e`..The `tootpas
-00017f20: 7465 6020 7365 7276 6963 6520 6973 2066  te` service is f
-00017f30: 6f72 2070 6f73 7469 6e67 2074 6f20 7468  or posting to th
-00017f40: 6520 5b4d 6173 746f 646f 6e20 736f 6369  e [Mastodon soci
-00017f50: 616c 206e 6574 776f 726b 5d28 6874 7470  al network](http
-00017f60: 733a 2f2f 6d61 7374 6f64 6f6e 2e73 6f63  s://mastodon.soc
-00017f70: 6961 6c2f 6162 6f75 7429 2e0a 0a60 6060  ial/about)...```
-00017f80: 696e 690a 5b63 6f6e 6669 673a 746f 6f74  ini.[config:toot
-00017f90: 7061 7374 655d 0a74 6172 6765 7473 203d  paste].targets =
-00017fa0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00017fb0: 2320 636c 6965 6e74 6372 6564 732c 2075  # clientcreds, u
-00017fc0: 7365 7263 7265 6473 2c20 6261 7365 5f75  sercreds, base_u
-00017fd0: 726c 0a20 2020 2027 756e 6f27 2020 3a20  rl.    'uno'  : 
-00017fe0: 5b20 2761 2e63 6c69 656e 7427 2c20 2027  [ 'a.client',  '
-00017ff0: 612e 7573 6572 272c 2027 6874 7470 733a  a.user', 'https:
-00018000: 2f2f 6d61 7374 6f2e 696f 2720 5d2c 0a20  //masto.io' ],. 
-00018010: 207d 0a60 6060 0a0a 5468 6520 7370 6563   }.```..The spec
-00018020: 6966 6965 6420 6063 6c69 656e 7463 7265  ified `clientcre
-00018030: 6473 6020 616e 6420 6075 7365 7263 7265  ds` and `usercre
-00018040: 6473 6020 6172 6520 7061 7468 7320 746f  ds` are paths to
-00018050: 2066 696c 6573 2063 7265 6174 6564 2077   files created w
-00018060: 6974 6820 7468 6520 7365 7276 6963 652c  ith the service,
-00018070: 2061 7320 666f 6c6c 6f77 733a 0a0a 6060   as follows:..``
-00018080: 600a 7079 7468 6f6e 2073 6572 7669 6365  `.python service
-00018090: 732f 746f 6f74 7061 7374 652e 7079 2027  s/tootpaste.py '
-000180a0: 6874 7470 733a 2f2f 6d61 7374 6f2e 696f  https://masto.io
-000180b0: 2720 276a 616e 6540 6578 616d 706c 652e  ' 'jane@example.
-000180c0: 6f72 6727 2027 7861 6661 3532 3830 3839  org' 'xafa528089
-000180d0: 3027 2077 6172 6e6d 6520 7375 3033 2d61  0' warnme su03-a
-000180e0: 2e63 6c69 656e 7420 7375 3033 2d61 2e75  .client su03-a.u
-000180f0: 7365 720a 6060 600a 0a54 6865 2061 7267  ser.```..The arg
-00018100: 756d 656e 7473 2c20 696e 206f 7264 6572  uments, in order
-00018110: 3a0a 0a31 2e20 6261 7365 2055 524c 2028  :..1. base URL (
-00018120: 652e 672e 2060 6874 7470 733a 2f2f 6d61  e.g. `https://ma
-00018130: 7374 6f64 6f6e 2e73 6f63 6961 6c60 290a  stodon.social`).
-00018140: 322e 2079 6f75 7220 652d 6d61 696c 2061  2. your e-mail a
-00018150: 6464 7265 7373 0a33 2e20 7468 6520 7061  ddress.3. the pa
-00018160: 7373 776f 7264 2063 6f72 7265 7370 6f6e  ssword correspon
-00018170: 6469 6e67 2074 6f20 7468 6520 652d 6d61  ding to the e-ma
-00018180: 696c 2061 6464 7265 7373 0a34 2e20 7468  il address.4. th
-00018190: 6520 636c 6965 6e74 206e 616d 6520 286e  e client name (n
-000181a0: 616d 6520 6f66 2074 6865 2070 6f73 7469  ame of the posti
-000181b0: 6e67 2070 726f 6772 616d 290a 352e 2074  ng program).5. t
-000181c0: 6865 2063 6c69 656e 7463 7265 6473 2066  he clientcreds f
-000181d0: 696c 650a 362e 2074 6865 2075 7365 7263  ile.6. the userc
-000181e0: 7265 6473 2066 696c 652e 0a0a 5468 6520  reds file...The 
-000181f0: 7477 6f20 6c61 7374 2066 696c 6573 2061  two last files a
-00018200: 7265 2063 7265 6174 6564 2061 6e64 2073  re created and s
-00018210: 686f 756c 6420 6265 2070 726f 7465 6374  hould be protect
-00018220: 6564 2066 726f 6d20 7072 7969 6e67 2065  ed from prying e
-00018230: 7965 732e 0a0a 215b 746f 6f74 7061 7374  yes...![tootpast
-00018240: 6520 284d 6173 746f 646f 6e29 5d28 6173  e (Mastodon)](as
-00018250: 7365 7473 2f74 6f6f 7470 6173 7465 2e70  sets/tootpaste.p
-00018260: 6e67 290a 0a60 746f 6f74 7061 7374 6560  ng)..`tootpaste`
-00018270: 2072 6571 7569 7265 7320 6120 6070 6970   requires a `pip
-00018280: 2069 6e73 7461 6c6c 204d 6173 746f 646f   install Mastodo
-00018290: 6e2e 7079 6020 285b 4d61 7374 6f64 6f6e  n.py` ([Mastodon
-000182a0: 2e70 795d 2868 7474 7073 3a2f 2f67 6974  .py](https://git
-000182b0: 6875 622e 636f 6d2f 6861 6c63 792f 4d61  hub.com/halcy/Ma
-000182c0: 7374 6f64 6f6e 2e70 7929 292e 0a0a 2323  stodon.py))...##
-000182d0: 2320 6074 7769 6c69 6f60 0a0a 6060 6069  # `twilio`..```i
-000182e0: 6e69 0a5b 636f 6e66 6967 3a74 7769 6c69  ni.[config:twili
-000182f0: 6f5d 0a74 6172 6765 7473 203d 207b 0a20  o].targets = {. 
-00018300: 2020 2020 2020 2020 2020 2020 2320 4163              # Ac
-00018310: 636f 756e 7420 5349 4420 2020 2020 2020  count SID       
-00018320: 2020 2020 2041 7574 6820 546f 6b65 6e20       Auth Token 
-00018330: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-00018340: 2020 2020 2020 2020 2020 2020 2074 6f0a               to.
-00018350: 2020 2027 686f 6c61 2720 203a 205b 2027     'hola'  : [ '
-00018360: 4143 5858 5858 5858 5858 5858 5858 5858  ACXXXXXXXXXXXXXX
-00018370: 5858 5827 2c20 2759 5959 5959 5959 5959  XXX', 'YYYYYYYYY
-00018380: 5959 5959 5959 5959 5927 2c20 222b 3135  YYYYYYYYY', "+15
-00018390: 3130 3535 3531 3233 3422 2c20 2022 2b31  105551234",  "+1
-000183a0: 3231 3235 3535 3132 3334 2220 5d0a 2020  2125551234" ].  
-000183b0: 207d 0a60 6060 0a0a 215b 5477 696c 696f   }.```..![Twilio
-000183c0: 2074 6573 745d 2861 7373 6574 732f 7477   test](assets/tw
-000183d0: 696c 6c69 6f2e 6a70 6729 0a0a 5265 7175  illio.jpg)..Requ
-000183e0: 6972 6573 3a0a 202a 2061 2054 7769 6c69  ires:. * a Twili
-000183f0: 6f20 6163 636f 756e 740a 202a 205b 7477  o account. * [tw
-00018400: 696c 696f 2d70 7974 686f 6e5d 2868 7474  ilio-python](htt
-00018410: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00018420: 7477 696c 696f 2f74 7769 6c69 6f2d 7079  twilio/twilio-py
-00018430: 7468 6f6e 290a 0a23 2323 2060 7477 6974  thon)..### `twit
-00018440: 7465 7260 0a0a 4e6f 7469 6669 6361 7469  ter`..Notificati
-00018450: 6f6e 206f 6620 6f6e 6520 6f72 206d 6f72  on of one or mor
-00018460: 6520 5b54 7769 7474 6572 5d28 6874 7470  e [Twitter](http
-00018470: 3a2f 2f74 7769 7474 6572 2e63 6f6d 2920  ://twitter.com) 
-00018480: 6163 636f 756e 7473 2072 6571 7569 7265  accounts require
-00018490: 7320 7365 7474 696e 670a 7570 2061 6e20  s setting.up an 
-000184a0: 6170 706c 6963 6174 696f 6e20 6174 205b  application at [
-000184b0: 6170 7073 2e74 7769 7474 6572 2e63 6f6d  apps.twitter.com
-000184c0: 5d28 6874 7470 733a 2f2f 6170 7073 2e74  ](https://apps.t
-000184d0: 7769 7474 6572 2e63 6f6d 292e 2046 6f72  witter.com). For
-000184e0: 2065 6163 6820 5477 6974 7465 720a 6163   each Twitter.ac
-000184f0: 636f 756e 742c 2079 6f75 206e 6565 6420  count, you need 
-00018500: 666f 7572 2028 3429 2062 6974 7320 7768  four (4) bits wh
-00018510: 6963 6820 6172 6520 6e61 6d65 6420 6173  ich are named as
-00018520: 2073 686f 776e 2062 656c 6f77 2e0a 0a55   shown below...U
-00018530: 706f 6e20 636f 6e66 6967 7572 696e 6720  pon configuring 
-00018540: 7468 6973 2073 6572 7669 6365 2773 2074  this service's t
-00018550: 6172 6765 7473 2c20 6d61 6b65 2073 7572  argets, make sur
-00018560: 6520 7468 6520 666f 7572 2028 3429 2065  e the four (4) e
-00018570: 6c65 6d65 6e74 7320 6f66 2074 6865 0a6c  lements of the.l
-00018580: 6973 7420 6172 6520 696e 2074 6865 206f  ist are in the o
-00018590: 7264 6572 2073 7065 6369 6669 6564 210a  rder specified!.
-000185a0: 0a60 6060 696e 690a 5b63 6f6e 6669 673a  .```ini.[config:
-000185b0: 7477 6974 7465 725d 0a74 6172 6765 7473  twitter].targets
-000185c0: 203d 207b 0a20 2027 6a61 6e65 6a6f 6c27   = {.  'janejol'
-000185d0: 2020 203a 2020 5b20 2776 7676 7676 7676     :  [ 'vvvvvvv
-000185e0: 7676 7676 7676 7676 7676 7676 7676 7627  vvvvvvvvvvvvvvv'
-000185f0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00018600: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00018610: 2063 6f6e 7375 6d65 725f 6b65 790a 2020   consumer_key.  
-00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018630: 2027 7777 7777 7777 7777 7777 7777 7777   'wwwwwwwwwwwwww
-00018640: 7777 7777 7777 7777 7777 7777 7777 7777  wwwwwwwwwwwwwwww
-00018650: 7777 7777 7777 7777 7777 7777 272c 2020  wwwwwwwwwwww',  
-00018660: 2020 2020 2020 2020 2320 636f 6e73 756d          # consum
-00018670: 6572 5f73 6563 7265 740a 2020 2020 2020  er_secret.      
-00018680: 2020 2020 2020 2020 2020 2020 2027 7878               'xx
-00018690: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
-000186a0: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
-000186b0: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
-000186c0: 272c 2020 2320 6163 6365 7373 5f74 6f6b  ',  # access_tok
-000186d0: 656e 5f6b 6579 0a20 2020 2020 2020 2020  en_key.         
-000186e0: 2020 2020 2020 2020 2020 277a 7a7a 7a7a            'zzzzz
-000186f0: 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a  zzzzzzzzzzzzzzzz
-00018700: 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a  zzzzzzzzzzzzzzzz
-00018710: 7a7a 7a7a 7a27 2020 2020 2020 2020 2020  zzzzz'          
-00018720: 2023 2061 6363 6573 735f 746f 6b65 6e5f   # access_token_
-00018730: 7365 6372 6574 0a20 2020 2020 2020 2020  secret.         
-00018740: 2020 2020 2020 2020 205d 0a20 2020 7d0a           ].   }.
-00018750: 6060 600a 0a21 5b61 2074 7765 6574 5d28  ```..![a tweet](
-00018760: 6173 7365 7473 2f74 7769 7474 6572 2e6a  assets/twitter.j
-00018770: 7067 290a 0a52 6571 7569 7265 733a 0a2a  pg)..Requires:.*
-00018780: 2041 2054 7769 7474 6572 2061 6363 6f75   A Twitter accou
-00018790: 6e74 0a2a 2061 7070 206b 6579 7320 666f  nt.* app keys fo
-000187a0: 7220 5477 6974 7465 722c 2066 726f 6d20  r Twitter, from 
-000187b0: 5b61 7070 732e 7477 6974 7465 722e 636f  [apps.twitter.co
-000187c0: 6d5d 2868 7474 7073 3a2f 2f61 7070 732e  m](https://apps.
-000187d0: 7477 6974 7465 722e 636f 6d29 0a2a 205b  twitter.com).* [
-000187e0: 7079 7468 6f6e 2d74 7769 7474 6572 5d28  python-twitter](
-000187f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00018800: 6f6d 2f62 6561 722f 7079 7468 6f6e 2d74  om/bear/python-t
-00018810: 7769 7474 6572 290a 0a23 2323 2060 7765  witter)..### `we
-00018820: 6273 6f63 6b65 7460 0a0a 5468 6520 7765  bsocket`..The we
-00018830: 6273 6f63 6b65 7420 7365 7276 6963 6520  bsocket service 
-00018840: 6361 6e20 6265 2075 7365 6420 746f 2073  can be used to s
-00018850: 656e 6420 6461 7461 2074 6f20 6120 7765  end data to a we
-00018860: 6273 6f63 6b65 7420 7365 7276 6572 2064  bsocket server d
-00018870: 6566 696e 6564 2062 7920 6974 7320 7572  efined by its ur
-00018880: 692e 2060 7773 3a2f 2f60 206f 7220 6077  i. `ws://` or `w
-00018890: 7373 3a2f 2f60 2073 6368 656d 6173 0a61  ss://` schemas.a
-000188a0: 7265 2073 7570 706f 7274 6564 2e0a 0a60  re supported...`
-000188b0: 6060 696e 690a 5b63 6f6e 6669 673a 7765  ``ini.[config:we
-000188c0: 6273 6f63 6b65 745d 0a74 6172 6765 7473  bsocket].targets
-000188d0: 203d 207b 0a20 2020 2020 2020 2023 2074   = {.        # t
-000188e0: 6172 6765 7469 6420 2020 2020 2020 203a  argetid        :
-000188f0: 205b 2027 7773 7572 6927 5d0a 2020 2020   [ 'wsuri'].    
-00018900: 2020 2020 2777 7373 7365 7276 6572 2720      'wssserver' 
-00018910: 3a20 5b20 2777 733a 2f2f 6c6f 6361 6c68  : [ 'ws://localh
-00018920: 6f73 742f 7773 2720 5d2c 0a7d 200a 6060  ost/ws' ],.} .``
-00018930: 600a 0a52 6571 7569 7265 733a 0a2a 205b  `..Requires:.* [
-00018940: 7765 6273 6f63 6b65 742d 636c 6965 6e74  websocket-client
-00018950: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00018960: 7974 686f 6e2e 6f72 672f 7079 7069 2f77  ython.org/pypi/w
-00018970: 6562 736f 636b 6574 2d63 6c69 656e 742f  ebsocket-client/
-00018980: 2920 2d20 7069 7020 696e 7374 616c 6c20  ) - pip install 
-00018990: 7765 6273 6f63 6b65 742d 636c 6965 6e74  websocket-client
-000189a0: 0a0a 2323 2320 6078 626d 6360 0a0a 5468  ..### `xbmc`..Th
-000189b0: 6973 2073 6572 7669 6365 2061 6c6c 6f77  is service allow
-000189c0: 7320 666f 7220 6f6e 2d73 6372 6565 6e20  s for on-screen 
-000189d0: 6e6f 7469 6669 6361 7469 6f6e 2070 6f70  notification pop
-000189e0: 2d75 7073 206f 6e20 5b58 424d 435d 2868  -ups on [XBMC](h
-000189f0: 7474 703a 2f2f 7862 6d63 2e6f 7267 2f29  ttp://xbmc.org/)
-00018a00: 2069 6e73 7461 6e63 6573 2e20 4561 6368   instances. Each
-00018a10: 2074 6172 6765 7420 7265 7175 6972 6573   target requires
-00018a20: 0a74 6865 2061 6464 7265 7373 2061 6e64  .the address and
-00018a30: 2070 6f72 7420 6f66 2074 6865 2058 424d   port of the XBM
-00018a40: 4320 696e 7374 616e 6365 2028 3c68 6f73  C instance (<hos
-00018a50: 746e 616d 653e 3a3c 706f 7274 3e29 2c20  tname>:<port>), 
-00018a60: 616e 6420 616e 206f 7074 696f 6e61 6c20  and an optional 
-00018a70: 7573 6572 6e61 6d65 2061 6e64 2070 6173  username and pas
-00018a80: 7377 6f72 6420 6966 2061 7574 6865 6e74  sword if authent
-00018a90: 6963 6174 696f 6e20 6973 2072 6571 7569  ication is requi
-00018aa0: 7265 642e 0a0a 6060 6069 6e69 0a5b 636f  red...```ini.[co
-00018ab0: 6e66 6967 3a78 626d 635d 0a74 6172 6765  nfig:xbmc].targe
-00018ac0: 7473 203d 207b 0a20 2020 2020 2020 2020  ts = {.         
-00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ae0: 2023 2068 6f73 743a 706f 7274 2c20 2020   # host:port,   
-00018af0: 2020 2020 2020 2020 5b75 7365 725d 2c20          [user], 
-00018b00: 5b70 6173 7377 6f72 645d 0a20 2020 2027  [password].    '
-00018b10: 6c69 7669 6e67 5f77 6974 685f 6175 7468  living_with_auth
-00018b20: 2720 3a20 205b 2027 3139 322e 3136 382e  ' :  [ '192.168.
-00018b30: 312e 3430 3a38 3038 3027 2c20 2778 626d  1.40:8080', 'xbm
-00018b40: 6327 2c20 2778 626d 6327 205d 2c0a 2020  c', 'xbmc' ],.  
-00018b50: 2020 2762 6564 726f 6f6d 5f6e 6f5f 6175    'bedroom_no_au
-00018b60: 7468 2720 203a 2020 5b20 2731 3932 2e31  th'  :  [ '192.1
-00018b70: 3638 2e31 2e34 313a 3830 3830 2720 5d0a  68.1.41:8080' ].
-00018b80: 2020 2020 7d0a 6060 600a 0a7c 2054 6f70      }.```..| Top
-00018b90: 6963 206f 7074 696f 6e20 207c 2020 4d2f  ic option  |  M/
-00018ba0: 4f20 2020 7c20 4465 7363 7269 7074 696f  O   | Descriptio
-00018bb0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00018bc0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00018bd0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 207c   ------------- |
-00018be0: 203a 2d2d 2d2d 3a20 7c20 2d2d 2d2d 2d2d   :----: | ------
-00018bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018c10: 207c 0a7c 2060 7469 746c 6560 2020 2020   |.| `title`    
-00018c20: 2020 207c 2020 204f 2020 2020 7c20 6e6f     |   O    | no
-00018c30: 7469 6669 6361 7469 6f6e 2074 6974 6c65  tification title
-00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c50: 2020 2020 207c 0a7c 2060 696d 6167 6560       |.| `image`
-00018c60: 2020 2020 2020 207c 2020 204f 2020 2020         |   O    
-00018c70: 7c20 6e6f 7469 6669 6361 7469 6f6e 2069  | notification i
-00018c80: 6d61 6765 2055 524c 2020 285b 6578 616d  mage URL  ([exam
-00018c90: 706c 655d 2868 7474 7073 3a2f 2f67 6974  ple](https://git
-00018ca0: 6875 622e 636f 6d2f 6a70 6d65 6e73 2f6d  hub.com/jpmens/m
-00018cb0: 7174 7477 6172 6e2f 6973 7375 6573 2f35  qttwarn/issues/5
-00018cc0: 3323 6973 7375 6563 6f6d 6d65 6e74 2d33  3#issuecomment-3
-00018cd0: 3936 3931 3432 3929 297c 0a0a 2323 2320  9691429))|..### 
-00018ce0: 6078 6d70 7060 0a0a 5468 6520 6078 6d70  `xmpp`..The `xmp
-00018cf0: 7060 2073 6572 7669 6365 2073 656e 6473  p` service sends
-00018d00: 206e 6f74 6966 6963 6174 696f 6e20 746f   notification to
-00018d10: 206f 6e65 206f 7220 6d6f 7265 205b 584d   one or more [XM
-00018d20: 5050 5d28 6874 7470 3a2f 2f65 6e2e 7769  PP](http://en.wi
-00018d30: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00018d40: 2f58 4d50 5029 0a28 4a61 6262 6572 2920  /XMPP).(Jabber) 
-00018d50: 7265 6369 7069 656e 7473 2e0a 0a60 6060  recipients...```
-00018d60: 696e 690a 5b63 6f6e 6669 673a 786d 7070  ini.[config:xmpp
-00018d70: 5d0a 7365 6e64 6572 203d 2027 6d71 7474  ].sender = 'mqtt
-00018d80: 7761 726e 406a 6162 6265 722e 7365 7276  warn@jabber.serv
-00018d90: 6572 270a 7061 7373 776f 7264 203d 2027  er'.password = '
-00018da0: 5061 7373 776f 7264 2066 6f72 2073 656e  Password for sen
-00018db0: 6465 7227 0a74 6172 6765 7473 203d 207b  der'.targets = {
-00018dc0: 0a20 2020 2027 6164 6d69 6e27 203a 205b  .    'admin' : [
-00018dd0: 2027 6164 6d69 6e31 406a 6162 6265 722e   'admin1@jabber.
-00018de0: 7365 7276 6572 272c 2027 6164 6d69 6e32  server', 'admin2
-00018df0: 406a 6162 6265 722e 7365 7276 6572 2720  @jabber.server' 
-00018e00: 5d0a 2020 2020 7d0a 6060 600a 0a54 6172  ].    }.```..Tar
-00018e10: 6765 7473 206d 6179 2063 6f6e 7461 696e  gets may contain
-00018e20: 206d 6f72 6520 7468 616e 206f 6e65 2072   more than one r
-00018e30: 6563 6970 6965 6e74 2c20 696e 2077 6869  ecipient, in whi
-00018e40: 6368 2063 6173 6520 616c 6c20 7370 6563  ch case all spec
-00018e50: 6966 6965 640a 7265 6369 7069 656e 7473  ified.recipients
-00018e60: 2067 6574 2074 6865 206d 6573 7361 6765   get the message
-00018e70: 2e0a 0a52 6571 7569 7265 733a 0a2a 2058  ...Requires:.* X
-00018e80: 4d50 5020 284a 6162 6265 7229 2061 6363  MPP (Jabber) acc
-00018e90: 6f75 6e74 7320 2861 7420 6c65 6173 7420  ounts (at least 
-00018ea0: 6f6e 6520 666f 7220 7468 6520 7365 6e64  one for the send
-00018eb0: 6572 2061 6e64 206f 6e65 2066 6f72 2074  er and one for t
-00018ec0: 6865 2072 6563 6970 6965 6e74 290a 2a20  he recipient).* 
-00018ed0: 5b78 6d70 7070 795d 2868 7474 703a 2f2f  [xmpppy](http://
-00018ee0: 786d 7070 7079 2e73 6f75 7263 6566 6f72  xmpppy.sourcefor
-00018ef0: 6765 2e6e 6574 290a 0a23 2323 2060 736c  ge.net)..### `sl
-00018f00: 6978 6d70 7060 0a0a 5468 6520 6073 6c69  ixmpp`..The `sli
-00018f10: 786d 7070 6020 7365 7276 6963 6520 7365  xmpp` service se
-00018f20: 6e64 7320 6e6f 7469 6669 6361 7469 6f6e  nds notification
-00018f30: 2074 6f20 6f6e 6520 6f72 206d 6f72 6520   to one or more 
-00018f40: 5b58 4d50 505d 2868 7474 703a 2f2f 656e  [XMPP](http://en
-00018f50: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00018f60: 696b 692f 584d 5050 290a 284a 6162 6265  iki/XMPP).(Jabbe
-00018f70: 7229 2072 6563 6970 6965 6e74 732e 0a0a  r) recipients...
-00018f80: 6060 6069 6e69 0a5b 636f 6e66 6967 3a73  ```ini.[config:s
-00018f90: 6c69 786d 7070 5d0a 7365 6e64 6572 203d  lixmpp].sender =
-00018fa0: 2027 6d71 7474 7761 726e 406a 6162 6265   'mqttwarn@jabbe
-00018fb0: 722e 7365 7276 6572 270a 7061 7373 776f  r.server'.passwo
-00018fc0: 7264 203d 2027 5061 7373 776f 7264 2066  rd = 'Password f
-00018fd0: 6f72 2073 656e 6465 7227 0a74 6172 6765  or sender'.targe
-00018fe0: 7473 203d 207b 0a20 2020 2027 6164 6d69  ts = {.    'admi
-00018ff0: 6e27 203a 205b 2027 6164 6d69 6e31 406a  n' : [ 'admin1@j
-00019000: 6162 6265 722e 7365 7276 6572 272c 2027  abber.server', '
-00019010: 6164 6d69 6e32 406a 6162 6265 722e 7365  admin2@jabber.se
-00019020: 7276 6572 2720 5d0a 2020 2020 7d0a 6060  rver' ].    }.``
-00019030: 600a 0a54 6172 6765 7473 206d 6179 2063  `..Targets may c
-00019040: 6f6e 7461 696e 206d 6f72 6520 7468 616e  ontain more than
-00019050: 206f 6e65 2072 6563 6970 6965 6e74 2c20   one recipient, 
-00019060: 696e 2077 6869 6368 2063 6173 6520 616c  in which case al
-00019070: 6c20 7370 6563 6966 6965 640a 7265 6369  l specified.reci
-00019080: 7069 656e 7473 2067 6574 2074 6865 206d  pients get the m
-00019090: 6573 7361 6765 2e0a 0a52 6571 7569 7265  essage...Require
-000190a0: 733a 0a2a 2058 4d50 5020 284a 6162 6265  s:.* XMPP (Jabbe
-000190b0: 7229 2061 6363 6f75 6e74 7320 2861 7420  r) accounts (at 
-000190c0: 6c65 6173 7420 6f6e 6520 666f 7220 7468  least one for th
-000190d0: 6520 7365 6e64 6572 2061 6e64 206f 6e65  e sender and one
-000190e0: 2066 6f72 2074 6865 2072 6563 6970 6965   for the recipie
-000190f0: 6e74 290a 2a20 5b73 6c69 786d 7070 5d28  nt).* [slixmpp](
-00019100: 6874 7470 733a 2f2f 6c61 622e 6c6f 7569  https://lab.loui
-00019110: 7a2e 6f72 672f 706f 657a 696f 2f73 6c69  z.org/poezio/sli
-00019120: 786d 7070 290a 0a23 2323 2060 7869 7665  xmpp)..### `xive
-00019130: 6c79 600a 0a54 6865 2060 7869 7665 6c79  ly`..The `xively
-00019140: 6020 7365 7276 6963 6520 6361 6e20 7365  ` service can se
-00019150: 6e64 2061 2073 7562 7365 7420 6f66 2079  nd a subset of y
-00019160: 6f75 7220 6461 7461 2074 6f20 5b58 6976  our data to [Xiv
-00019170: 656c 795d 2868 7474 703a 2f2f 7869 7665  ely](http://xive
-00019180: 6c79 2e63 6f6d 2920 7065 7220 6465 6669  ly.com) per defi
-00019190: 6e65 6420 6665 6564 6964 2e0a 0a60 6060  ned feedid...```
-000191a0: 696e 690a 5b63 6f6e 6669 673a 7869 7665  ini.[config:xive
-000191b0: 6c79 5d0a 6170 696b 6579 203d 2027 3132  ly].apikey = '12
-000191c0: 3334 3536 3738 3930 6162 6364 6566 6768  34567890abcdefgh
-000191d0: 696b 6c6d 6e6f 7071 7273 7475 7677 7879  iklmnopqrstuvwxy
-000191e0: 7a27 0a74 6172 6765 7473 203d 207b 0a20  z'.targets = {. 
-000191f0: 2020 2020 2020 2023 2066 6565 6469 6420         # feedid 
-00019200: 2020 2020 2020 203a 205b 2027 6461 7461         : [ 'data
-00019210: 7374 7265 616d 3127 2c20 2764 6174 6173  stream1', 'datas
-00019220: 7472 6561 6d32 275d 0a20 2020 2020 2020  tream2'].       
-00019230: 2027 3132 3334 3536 3727 203a 205b 2027   '1234567' : [ '
-00019240: 7465 6d70 6572 6174 7572 6527 2c20 2777  temperature', 'w
-00019250: 6174 6572 6c65 7665 6c27 205d 2c0a 2020  aterlevel' ],.  
-00019260: 2020 2020 2020 2737 3635 3433 3231 2720        '7654321' 
-00019270: 3a20 5b20 2764 6174 6149 7465 6d41 2720  : [ 'dataItemA' 
-00019280: 5d0a 2020 7d0a 6060 600a 0a50 7562 6c69  ].  }.```..Publi
-00019290: 7368 696e 6720 7468 6520 666f 6c6c 6f77  shing the follow
-000192a0: 696e 6720 4a53 4f4e 206d 6573 7361 6765  ing JSON message
-000192b0: 2077 696c 6c20 6164 6420 6120 6461 7461   will add a data
-000192c0: 706f 696e 7420 746f 2074 6865 2060 7465  point to the `te
-000192d0: 6d70 6572 6174 7572 6560 2061 6e64 0a60  mperature` and.`
-000192e0: 7761 7465 726c 6576 656c 6020 6368 616e  waterlevel` chan
-000192f0: 6e65 6c20 6f66 2079 6f75 7220 7869 7665  nel of your xive
-00019300: 6c79 2066 6565 6420 3132 3334 3536 3720  ly feed 1234567 
-00019310: 2860 6875 6d69 6469 7479 6020 7769 6c6c  (`humidity` will
-00019320: 2062 6520 6967 6e6f 7265 642c 0a61 7320   be ignored,.as 
-00019330: 6974 2773 206e 6f74 2064 6566 696e 6564  it's not defined
-00019340: 2069 6e20 7468 6520 7869 7665 6c79 0a63   in the xively.c
-00019350: 6f6e 6669 6775 7261 7469 6f6e 2061 626f  onfiguration abo
-00019360: 7665 293a 0a0a 6060 600a 6d6f 7371 7569  ve):..```.mosqui
-00019370: 7474 6f5f 7075 6220 2d74 2022 6f73 782f  tto_pub -t "osx/
-00019380: 6a73 6f6e 2220 2d6d 2027 7b22 7465 6d70  json" -m '{"temp
-00019390: 6572 6174 7572 6522 3a31 352c 2277 6174  erature":15,"wat
-000193a0: 6572 6c65 7665 6c22 3a31 3030 2c22 6875  erlevel":100,"hu
-000193b0: 6d69 6469 7479 223a 3335 7d27 0a60 6060  midity":35}'.```
-000193c0: 0a0a 0a52 6571 7569 7265 733a 0a2a 205b  ...Requires:.* [
-000193d0: 5869 7665 6c79 5d28 6874 7470 3a2f 2f78  Xively](http://x
-000193e0: 6976 656c 792e 636f 6d29 2061 6363 6f75  ively.com) accou
-000193f0: 6e74 2077 6974 6820 616e 2061 6c72 6561  nt with an alrea
-00019400: 6479 2065 7869 7374 696e 6720 4665 6564  dy existing Feed
-00019410: 0a2a 205b 7869 7665 6c79 2d70 7974 686f  .* [xively-pytho
-00019420: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00019430: 622e 636f 6d2f 7869 7665 6c79 2f78 6976  b.com/xively/xiv
-00019440: 656c 792d 7079 7468 6f6e 2920 2d20 7069  ely-python) - pi
-00019450: 7020 696e 7374 616c 6c20 7869 7665 6c79  p install xively
-00019460: 2d70 7974 686f 6e0a 0a23 2323 2060 7a61  -python..### `za
-00019470: 6262 6978 600a 0a54 6865 2060 7a61 6262  bbix`..The `zabb
-00019480: 6978 6020 7365 7276 6963 6520 7365 7276  ix` service serv
-00019490: 6573 2074 776f 2070 7572 706f 7365 733a  es two purposes:
-000194a0: 0a0a 312e 2069 7420 6361 6e20 6372 6561  ..1. it can crea
-000194b0: 7465 2061 205b 5a61 6262 6978 5d20 686f  te a [Zabbix] ho
-000194c0: 7374 206f 6e2d 7468 652d 666c 7920 7669  st on-the-fly vi
-000194d0: 6120 4c6f 772d 6c65 7665 6c20 4469 7363  a Low-level Disc
-000194e0: 6f76 6572 7920 284c 4c44 290a 322e 2069  overy (LLD).2. i
-000194f0: 7420 6361 6e20 7365 6e64 2061 6e20 6974  t can send an it
-00019500: 656d 2f76 616c 7565 2070 6169 7220 746f  em/value pair to
-00019510: 2061 205b 5a61 6262 6978 5d20 7472 6170   a [Zabbix] trap
-00019520: 7065 720a 0a21 5b5a 6162 6269 785d 2861  per..![Zabbix](a
-00019530: 7373 6574 732f 7a61 6262 6978 2e70 6e67  ssets/zabbix.png
-00019540: 290a 0a54 6f20 6372 6561 7465 2061 6e20  )..To create an 
-00019550: 6170 7072 6f70 7269 6174 6520 6469 7363  appropriate disc
-00019560: 6f76 6572 7920 686f 7374 2c20 696e 205a  overy host, in Z
-00019570: 6162 6269 783a 0a2d 2043 6f6e 6669 6775  abbix:.- Configu
-00019580: 7261 7469 6f6e 2d3e 486f 7374 732d 3e43  ration->Hosts->C
-00019590: 7265 6174 6520 686f 7374 2028 606d 7174  reate host (`mqt
-000195a0: 7477 6172 6e30 3160 290a 2d20 436f 6e66  twarn01`).- Conf
-000195b0: 6967 7572 6174 696f 6e2d 3e44 6973 636f  iguration->Disco
-000195c0: 7665 7279 2d3e 4372 6561 7465 2064 6973  very->Create dis
-000195d0: 636f 7665 7279 2072 756c 650a 2020 2d20  covery rule.  - 
-000195e0: 4e61 6d65 3a20 604d 5154 5477 6172 6e60  Name: `MQTTwarn`
-000195f0: 2028 616e 7920 7375 6974 6162 6c65 206e   (any suitable n
-00019600: 616d 6529 0a20 202d 2054 7970 653a 2060  ame).  - Type: `
-00019610: 5a61 6262 6978 2074 7261 7070 6572 600a  Zabbix trapper`.
-00019620: 2020 2d20 4b65 793a 2060 6d71 7474 2e64    - Key: `mqtt.d
-00019630: 6973 636f 7665 7279 6020 2874 6869 7320  iscovery` (this 
-00019640: 6d75 7374 206d 6174 6368 2074 6865 2063  must match the c
-00019650: 6f6e 6669 6775 7265 6420 6064 6973 636f  onfigured `disco
-00019660: 7665 7279 5f6b 6579 602c 2077 6869 6368  very_key`, which
-00019670: 2064 6566 6175 6c74 7320 746f 2060 6d71   defaults to `mq
-00019680: 7474 2e64 6973 636f 7665 7279 6029 0a20  tt.discovery`). 
-00019690: 202d 2041 6c6c 6f77 6564 2068 6f73 7473   - Allowed hosts
-000196a0: 3a20 6031 3932 2e31 3638 2e31 2e31 3330  : `192.168.1.130
-000196b0: 2c31 3237 2e30 2e30 2e31 6020 2865 7861  ,127.0.0.1` (exa
-000196c0: 6d70 6c65 290a 0a54 6865 2074 6172 6765  mple)..The targe
-000196d0: 7420 616e 6420 746f 7069 6320 636f 6e66  t and topic conf
-000196e0: 6967 7572 6174 696f 6e20 6c6f 6f6b 206c  iguration look l
-000196f0: 696b 6520 7468 6973 3a0a 0a60 6060 696e  ike this:..```in
-00019700: 690a 5b63 6f6e 6669 673a 7a61 6262 6978  i.[config:zabbix
-00019710: 5d0a 686f 7374 203d 2022 6d71 7474 7761  ].host = "mqttwa
-00019720: 726e 3031 2220 2023 2061 6e20 6578 6973  rn01"  # an exis
-00019730: 7469 6e67 2068 6f73 7420 636f 6e66 6967  ting host config
-00019740: 7572 6564 2069 6e20 5a61 6262 6978 0a64  ured in Zabbix.d
-00019750: 6973 636f 7665 7279 5f6b 6579 203d 2022  iscovery_key = "
-00019760: 6d71 7474 2e64 6973 636f 7665 7279 220a  mqtt.discovery".
-00019770: 7461 7267 6574 7320 3d20 7b0a 2020 2020  targets = {.    
-00019780: 2020 2020 2020 2020 2320 5472 6170 7065          # Trappe
-00019790: 7220 6164 6472 6573 7320 2020 706f 7274  r address   port
-000197a0: 0a20 2020 2027 7431 2720 203a 205b 2027  .    't1'  : [ '
-000197b0: 3137 322e 3136 2e31 3533 2e31 3130 272c  172.16.153.110',
-000197c0: 2031 3030 3531 205d 2c0a 2020 7d0a 0a5b   10051 ],.  }..[
-000197d0: 7a61 6262 6978 2f63 6c69 656e 7473 2f2b  zabbix/clients/+
-000197e0: 5d0a 616c 6c64 6174 6120 3d20 5a61 6262  ].alldata = Zabb
-000197f0: 6978 4461 7461 2829 0a74 6172 6765 7473  ixData().targets
-00019800: 203d 207a 6162 6269 783a 7431 0a0a 5b7a   = zabbix:t1..[z
-00019810: 6162 6269 782f 6974 656d 2f23 5d0a 616c  abbix/item/#].al
-00019820: 6c64 6174 6120 3d20 5a61 6262 6978 4461  ldata = ZabbixDa
-00019830: 7461 2829 0a74 6172 6765 7473 203d 207a  ta().targets = z
-00019840: 6162 6269 783a 7431 0a60 6060 0a0a 4120  abbix:t1.```..A 
-00019850: 7472 616e 7366 6f72 6d61 7469 6f6e 2066  transformation f
-00019860: 756e 6374 696f 6e20 696e 2060 616c 6c64  unction in `alld
-00019870: 6174 6160 2069 7320 7265 7175 6972 6564  ata` is required
-00019880: 2074 6f20 6578 7472 6163 7420 7468 6520   to extract the 
-00019890: 636c 6965 6e74 2773 206e 616d 650a 6672  client's name.fr
-000198a0: 6f6d 2074 6865 2074 6f70 6963 2c20 616e  om the topic, an
-000198b0: 6420 666f 7220 2331 2c20 746f 2064 6566  d for #1, to def
-000198c0: 696e 6520 6120 2268 6f73 7420 616c 6976  ine a "host aliv
-000198d0: 6522 2069 7465 6d20 6b65 7920 696e 205b  e" item key in [
-000198e0: 5a61 6262 6978 5d2e 0a0a 6060 6070 7974  Zabbix]...```pyt
-000198f0: 686f 6e0a 2320 4966 2074 6865 2074 6f70  hon.# If the top
-00019900: 6963 2062 6567 696e 7320 7769 7468 207a  ic begins with z
-00019910: 6162 6269 782f 636c 6965 6e74 7320 7765  abbix/clients we
-00019920: 2068 6176 6520 6120 686f 7374 2067 6f69   have a host goi
-00019930: 6e67 2075 7020 6f72 2064 6f77 6e0a 2320  ng up or down.# 
-00019940: 652e 672e 2022 7a61 6262 6978 2f63 6c69  e.g. "zabbix/cli
-00019950: 656e 7473 2f6a 6f67 3033 2220 2d3e 2022  ents/jog03" -> "
-00019960: 6a6f 6730 3322 0a23 2020 2065 7874 7261  jog03".#   extra
-00019970: 6374 2063 6c69 656e 7420 6e61 6d65 2028  ct client name (
-00019980: 3372 6420 7061 7274 206f 6620 746f 7069  3rd part of topi
-00019990: 6329 0a23 2020 2073 6574 2073 7461 7475  c).#   set statu
-000199a0: 7320 6b65 7920 2865 2e67 2e20 2768 6f73  s key (e.g. 'hos
-000199b0: 742e 7570 2729 2074 6f20 7075 626c 6973  t.up') to publis
-000199c0: 6820 312f 3020 6f6e 2069 7420 2865 2e67  h 1/0 on it (e.g
-000199d0: 2064 7572 696e 6720 4c57 5429 0a23 0a23   during LWT).#.#
-000199e0: 2069 6620 7468 6520 746f 7069 6320 7374   if the topic st
-000199f0: 6172 7473 2077 6974 6820 7a61 6262 6978  arts with zabbix
-00019a00: 2f69 7465 6d20 7765 2068 6176 6520 616e  /item we have an
-00019a10: 2069 7465 6d2f 7661 6c75 6520 666f 7220   item/value for 
-00019a20: 7468 6520 686f 7374 0a23 2065 2e67 2e20  the host.# e.g. 
-00019a30: 227a 6162 6269 782f 6974 656d 2f6a 6f67  "zabbix/item/jog
-00019a40: 3033 2f74 696d 652e 7374 616d 7022 202d  03/time.stamp" -
-00019a50: 3e20 226a 6f67 3033 220a 2320 2020 6578  > "jog03".#   ex
-00019a60: 7472 6163 7420 636c 6965 6e74 206e 616d  tract client nam
-00019a70: 6520 2833 7264 2070 6172 7420 6f66 2074  e (3rd part of t
-00019a80: 6f70 6963 290a 230a 0a64 6566 205a 6162  opic).#..def Zab
-00019a90: 6269 7844 6174 6128 746f 7069 632c 2064  bixData(topic, d
-00019aa0: 6174 612c 2073 7276 3d4e 6f6e 6529 3a0a  ata, srv=None):.
-00019ab0: 2020 2020 636c 6965 6e74 203d 2027 756e      client = 'un
-00019ac0: 6b6e 6f77 6e27 0a20 2020 206b 6579 203d  known'.    key =
-00019ad0: 204e 6f6e 650a 2020 2020 7374 6174 7573   None.    status
-00019ae0: 5f6b 6579 203d 204e 6f6e 650a 0a20 2020  _key = None..   
-00019af0: 2070 6172 7473 203d 2074 6f70 6963 2e73   parts = topic.s
-00019b00: 706c 6974 2827 2f27 290a 0a20 2020 2027  plit('/')..    '
-00019b10: 2727 2057 6861 7420 7765 2063 616c 6c20  '' What we call 
-00019b20: 2763 6c69 656e 7427 2069 7320 696e 2066  'client' is in f
-00019b30: 6163 7420 6120 225a 6162 6269 7820 486f  act a "Zabbix Ho
-00019b40: 7374 222c 2069 2e65 2e20 7468 6520 6e61  st", i.e. the na
-00019b50: 6d65 206f 6620 610a 2020 2020 2020 2020  me of a.        
-00019b60: 686f 7374 2063 6f6e 6669 6775 7265 6420  host configured 
-00019b70: 7769 7468 2069 7465 6d73 3b20 6974 2069  with items; it i
-00019b80: 7420 6e6f 7420 7468 6520 6e61 6d65 2f61  t not the name/a
-00019b90: 6464 7265 7373 206f 6620 7468 6520 6d61  ddress of the ma
-00019ba0: 6368 696e 6520 6f6e 0a20 2020 2020 2020  chine on.       
-00019bb0: 2077 6869 6368 205a 6162 6269 7820 7365   which Zabbix se
-00019bc0: 7276 6572 2072 756e 732e 2053 6f2c 2069  rver runs. So, i
-00019bd0: 6e20 7468 6520 5549 3a20 436f 6e66 6967  n the UI: Config
-00019be0: 7572 6174 696f 6e20 2d3e 2043 7265 6174  uration -> Creat
-00019bf0: 6520 686f 7374 2027 2727 0a0a 2020 2020  e host '''..    
-00019c00: 636c 6965 6e74 203d 2070 6172 7473 5b32  client = parts[2
-00019c10: 5d0a 0a20 2020 2069 6620 746f 7069 632e  ]..    if topic.
-00019c20: 7374 6172 7473 7769 7468 2827 7a61 6262  startswith('zabb
-00019c30: 6978 2f63 6c69 656e 7473 2f27 293a 0a20  ix/clients/'):. 
-00019c40: 2020 2020 2020 2073 7461 7475 735f 6b65         status_ke
-00019c50: 7920 3d20 2768 6f73 742e 7570 270a 0a20  y = 'host.up'.. 
-00019c60: 2020 2027 2727 2054 6869 7320 226b 6579     ''' This "key
-00019c70: 2220 6973 2061 6374 7561 6c6c 7920 616e  " is actually an
-00019c80: 204c 4c44 2069 7465 6d20 7768 6963 6820   LLD item which 
-00019c90: 7765 2776 6520 7072 652d 6372 6561 7465  we've pre-create
-00019ca0: 6420 696e 2074 6865 205a 6162 6269 780a  d in the Zabbix.
-00019cb0: 2020 2020 2020 2020 5549 2e20 436f 6e66          UI. Conf
-00019cc0: 6967 7572 6174 696f 6e2d 3e48 6f73 7473  iguration->Hosts
-00019cd0: 2d3e 4469 7363 6f76 6572 792d 3e49 7465  ->Discovery->Ite
-00019ce0: 6d20 7072 6f74 6f74 7970 6573 2d3e 4372  m prototypes->Cr
-00019cf0: 6561 7465 2069 7465 6d20 7072 6f74 6f74  eate item protot
-00019d00: 7970 650a 0920 2020 4e61 6d65 3a20 4d57  ype..   Name: MW
-00019d10: 2063 6c69 656e 7420 2431 0a09 2020 2054   client $1..   T
-00019d20: 7970 653a 205a 6162 6269 7820 7472 6170  ype: Zabbix trap
-00019d30: 7065 720a 0920 2020 4b65 793a 206d 7174  per..   Key: mqt
-00019d40: 7477 6172 6e2e 6964 5b7b 234d 5154 5448  twarn.id[{#MQTTH
-00019d50: 4f53 547d 5d0a 0920 2020 5479 7065 3a20  OST}]..   Type: 
-00019d60: 7465 7874 2028 6361 6e20 6265 2061 6e79  text (can be any
-00019d70: 2073 7569 7461 626c 6520 7479 7065 290a   suitable type).
-00019d80: 0a09 5075 626c 6973 6869 6e67 2061 2076  ..Publishing a v
-00019d90: 616c 7565 2077 6974 680a 0924 206d 6f73  alue with..$ mos
-00019da0: 7175 6974 746f 5f70 7562 202d 7420 7a61  quitto_pub -t za
-00019db0: 6262 6978 2f69 7465 6d2f 6d71 7474 7761  bbix/item/mqttwa
-00019dc0: 726e 3031 2f6d 7174 7477 6172 6e2e 6964  rn01/mqttwarn.id
-00019dd0: 5b6d 3032 5d20 2d6d 2027 7374 6f72 6d79  [m02] -m 'stormy
-00019de0: 270a 0977 696c 6c20 6d65 616e 2074 6861  '..will mean tha
-00019df0: 7420 7765 276c 6c20 7573 6520 7468 6520  t we'll use the 
-00019e00: 636c 6965 6e74 2022 6d71 7474 7761 726e  client "mqttwarn
-00019e10: 3031 2220 2873 6565 2070 7265 7669 6f75  01" (see previou
-00019e20: 736c 7929 2061 6e64 0a09 7468 6520 6974  sly) and..the it
-00019e30: 656d 206e 616d 6564 2022 6d71 7474 7761  em named "mqttwa
-00019e40: 726e 2e69 645b 6d30 325d 2220 7768 6963  rn.id[m02]" whic
-00019e50: 6820 6973 2074 6865 206e 616d 6520 6f66  h is the name of
-00019e60: 2061 2070 7265 7669 6f75 736c 790a 0964   a previously..d
-00019e70: 6973 636f 7665 7265 6420 6974 656d 2e0a  iscovered item..
-00019e80: 2020 2020 2727 270a 0a20 2020 2069 6620      '''..    if 
-00019e90: 746f 7069 632e 7374 6172 7473 7769 7468  topic.startswith
-00019ea0: 2827 7a61 6262 6978 2f69 7465 6d2f 2729  ('zabbix/item/')
-00019eb0: 3a0a 2020 2020 2020 2020 6b65 7920 3d20  :.        key = 
-00019ec0: 7061 7274 735b 335d 0a0a 2020 2020 7265  parts[3]..    re
-00019ed0: 7475 726e 2064 6963 7428 636c 6965 6e74  turn dict(client
-00019ee0: 3d63 6c69 656e 742c 206b 6579 3d6b 6579  =client, key=key
-00019ef0: 2c20 7374 6174 7573 5f6b 6579 3d73 7461  , status_key=sta
-00019f00: 7475 735f 6b65 7929 0a60 6060 0a0a 2323  tus_key).```..##
-00019f10: 2320 4372 6561 7469 6e67 2043 7573 746f  # Creating Custo
-00019f20: 6d20 5365 7276 6963 6520 506c 7567 696e  m Service Plugin
-00019f30: 730a 0a43 7265 6174 696e 6720 6e65 7720  s..Creating new 
-00019f40: 706c 7567 696e 7320 6973 2072 6174 6865  plugins is rathe
-00019f50: 7220 6561 7379 2c20 616e 6420 4920 7265  r easy, and I re
-00019f60: 636f 6d6d 656e 6420 796f 7520 7461 6b65  commend you take
-00019f70: 2074 6865 2060 6669 6c65 6020 706c 7567   the `file` plug
-00019f80: 696e 0a61 6e64 2073 7461 7274 2066 726f  in.and start fro
-00019f90: 6d20 7468 6174 2e0a 0a50 6c75 6769 6e73  m that...Plugins
-00019fa0: 2061 7265 2069 6e76 6f6b 6564 2077 6974   are invoked wit
-00019fb0: 6820 7477 6f20 6172 6775 6d65 6e74 7320  h two arguments 
-00019fc0: 2860 7372 7660 2061 6e64 2060 6974 656d  (`srv` and `item
-00019fd0: 6029 2e20 6073 7276 6020 6973 2061 6e20  `). `srv` is an 
-00019fe0: 6f62 6a65 6374 0a77 6974 6820 736f 6d65  object.with some
-00019ff0: 2068 656c 7065 7220 6675 6e63 7469 6f6e   helper function
-0001a000: 732c 2061 6e64 2060 6974 656d 6020 6120  s, and `item` a 
-0001a010: 6469 6374 2077 6869 6368 2063 6f6e 7461  dict which conta
-0001a020: 696e 7320 696e 666f 726d 6174 696f 6e20  ins information 
-0001a030: 6f6e 2074 6865 206d 6573 7361 6765 0a77  on the message.w
-0001a040: 6869 6368 2069 7320 746f 2062 6520 6861  hich is to be ha
-0001a050: 6e64 6c65 6420 6279 2074 6865 2070 6c75  ndled by the plu
-0001a060: 6769 6e2e 2060 6974 656d 6020 636f 6e74  gin. `item` cont
-0001a070: 6169 6e73 2074 6865 2066 6f6c 6c6f 7769  ains the followi
-0001a080: 6e67 2065 6c65 6d65 6e74 733a 0a0a 6060  ng elements:..``
-0001a090: 6070 7974 686f 6e0a 6974 656d 203d 207b  `python.item = {
-0001a0a0: 0a20 2020 2027 7365 7276 6963 6527 2020  .    'service'  
-0001a0b0: 2020 2020 203a 2027 7374 7269 6e67 272c       : 'string',
-0001a0c0: 2020 2020 2020 2023 206e 616d 6520 6f66         # name of
-0001a0d0: 2068 616e 646c 696e 6720 7365 7276 6963   handling servic
-0001a0e0: 6520 2860 7477 6974 7465 7260 2c20 6066  e (`twitter`, `f
-0001a0f0: 696c 6560 2c20 2e2e 290a 2020 2020 2774  ile`, ..).    't
-0001a100: 6172 6765 7427 2020 2020 2020 2020 3a20  arget'        : 
-0001a110: 2773 7472 696e 6727 2c20 2020 2020 2020  'string',       
-0001a120: 2320 6e61 6d65 206f 6620 7461 7267 6574  # name of target
-0001a130: 2028 606f 3160 2c20 606a 616e 656a 6f6c   (`o1`, `janejol
-0001a140: 6029 2069 6e20 7365 7276 6963 650a 2020  `) in service.  
-0001a150: 2020 2761 6464 7273 2720 2020 2020 2020    'addrs'       
-0001a160: 2020 3a20 6c69 7374 2c20 2020 2020 2020    : list,       
-0001a170: 2020 2020 2320 6c69 7374 206f 6620 6164      # list of ad
-0001a180: 6472 6573 7365 7320 6672 6f6d 2053 4552  dresses from SER
-0001a190: 5649 4345 5f74 6172 6765 7473 0a20 2020  VICE_targets.   
-0001a1a0: 2027 636f 6e66 6967 2720 2020 2020 2020   'config'       
-0001a1b0: 203a 2064 6963 742c 2020 2020 2020 2020   : dict,        
-0001a1c0: 2020 2023 204e 6f6e 6520 6f72 2064 6963     # None or dic
-0001a1d0: 7420 6672 6f6d 2053 4552 5649 4345 5f63  t from SERVICE_c
-0001a1e0: 6f6e 6669 6720 7b7d 0a20 2020 2027 746f  onfig {}.    'to
-0001a1f0: 7069 6327 2020 2020 2020 2020 203a 2027  pic'         : '
-0001a200: 7374 7269 6e67 272c 2020 2020 2020 2023  string',       #
-0001a210: 2069 6e63 6f6d 696e 6720 746f 7069 6320   incoming topic 
-0001a220: 6272 616e 6368 206e 616d 650a 2020 2020  branch name.    
-0001a230: 2770 6179 6c6f 6164 2720 2020 2020 2020  'payload'       
-0001a240: 3a20 2773 7472 696e 6727 2c20 2020 2020  : 'string',     
-0001a250: 2020 2320 7261 7720 6d65 7373 6167 6520    # raw message 
-0001a260: 7061 796c 6f61 640a 2020 2020 276d 6573  payload.    'mes
-0001a270: 7361 6765 2720 2020 2020 2020 3a20 2773  sage'       : 's
-0001a280: 7472 696e 6727 2c20 2020 2020 2020 2320  tring',       # 
-0001a290: 666f 726d 6174 7465 6420 6d65 7373 6167  formatted messag
-0001a2a0: 6520 2869 6620 6e6f 2066 6f72 6d61 7420  e (if no format 
-0001a2b0: 7374 7269 6e67 2074 6865 6e20 3d20 7061  string then = pa
-0001a2c0: 796c 6f61 6429 0a20 2020 2027 6461 7461  yload).    'data
-0001a2d0: 2720 2020 2020 2020 2020 203a 204e 6f6e  '          : Non
-0001a2e0: 652c 2020 2020 2020 2020 2020 2023 2064  e,           # d
-0001a2f0: 6963 7420 7769 7468 2074 7261 6e73 666f  ict with transfo
-0001a300: 726d 6174 696f 6e20 6461 7461 0a20 2020  rmation data.   
-0001a310: 2027 7469 746c 6527 2020 2020 2020 2020   'title'        
-0001a320: 203a 2027 6d71 7474 7761 726e 272c 2020   : 'mqttwarn',  
-0001a330: 2020 2023 2070 6f73 7369 626c 6520 7469     # possible ti
-0001a340: 746c 6520 6672 6f6d 2074 6974 6c65 7b7d  tle from title{}
-0001a350: 0a20 2020 2027 7072 696f 7269 7479 2720  .    'priority' 
-0001a360: 2020 2020 203a 2030 2c20 2020 2020 2020       : 0,       
-0001a370: 2020 2020 2020 2023 2070 6f73 7369 626c         # possibl
-0001a380: 6520 7072 696f 7269 7479 2066 726f 6d20  e priority from 
-0001a390: 7072 696f 7269 7479 7b7d 0a7d 0a60 6060  priority{}.}.```
-0001a3a0: 0a0a 2323 204f 7574 626f 756e 6420 6d65  ..## Outbound me
-0001a3b0: 7373 6167 6573 0a0a 2323 2320 4d65 7373  ssages..### Mess
-0001a3c0: 6167 6520 666f 7277 6172 6469 6e67 0a0a  age forwarding..
-0001a3d0: 546f 2073 696d 706c 7920 666f 7277 6172  To simply forwar
-0001a3e0: 6420 616e 2069 6e63 6f6d 696e 6720 4d51  d an incoming MQ
-0001a3f0: 5454 206d 6573 7361 6765 2c20 796f 7520  TT message, you 
-0001a400: 646f 6e27 7420 6e65 6564 2074 6f20 646f  don't need to do
-0001a410: 2061 6e79 7468 696e 6720 6f74 6865 7220   anything other 
-0001a420: 7468 616e 2063 6f6e 6669 6775 7265 2074  than configure t
-0001a430: 6865 2074 6172 6765 742e 2041 6464 2061  he target. Add a
-0001a440: 2074 6f70 6963 2073 6563 7469 6f6e 2074   topic section t
-0001a450: 6f20 796f 7572 2060 6d71 7474 7761 726e  o your `mqttwarn
-0001a460: 2e69 6e69 602c 2062 7920 7369 6d70 6c79  .ini`, by simply
-0001a470: 206e 616d 696e 6720 6974 2061 6674 6572   naming it after
-0001a480: 2074 6865 2074 6f70 6963 2079 6f75 2077   the topic you w
-0001a490: 6973 6820 746f 2068 6176 6520 666f 7277  ish to have forw
-0001a4a0: 6172 6465 642c 2061 6e64 2077 6974 6869  arded, and withi
-0001a4b0: 6e20 6465 6669 6e65 2074 6865 2060 7461  n define the `ta
-0001a4c0: 7267 6574 7360 2e20 5468 6520 7061 796c  rgets`. The payl
-0001a4d0: 6f61 6420 6f66 2074 6865 2069 6e62 6f75  oad of the inbou
-0001a4e0: 6e64 206d 6573 7361 6765 2077 696c 6c20  nd message will 
-0001a4f0: 7468 656e 2062 6520 666f 7277 6172 6465  then be forwarde
-0001a500: 6420 746f 2074 6865 2064 6566 696e 6564  d to the defined
-0001a510: 2073 6572 7669 6365 2070 6c75 6769 6e2c   service plugin,
-0001a520: 2077 6574 6865 7220 6974 2073 696d 706c   wether it simpl
-0001a530: 7920 7361 7973 2022 4f4e 222c 206f 7220  y says "ON", or 
-0001a540: 636f 6e74 6169 6e73 2061 206c 6172 6765  contains a large
-0001a550: 204a 534f 4e20 6469 6374 696f 6e61 7279   JSON dictionary
-0001a560: 2e0a 0a5b 6f66 6669 6365 2f75 7073 5d0a  ...[office/ups].
-0001a570: 7461 7267 6574 7320 3d20 6c6f 673a 6465  targets = log:de
-0001a580: 6275 670a 0a54 6869 7320 6578 616d 706c  bug..This exampl
-0001a590: 6520 7368 6f77 7320 686f 7720 746f 2068  e shows how to h
-0001a5a0: 6176 6520 6d65 7373 6167 6573 2072 6563  ave messages rec
-0001a5b0: 6569 7665 6420 6f6e 2074 6865 204d 5154  eived on the MQT
-0001a5c0: 5420 746f 7069 6320 606f 6666 6963 652f  T topic `office/
-0001a5d0: 7570 7360 2c20 7361 7665 6420 696e 746f  ups`, saved into
-0001a5e0: 2074 6865 2060 6d71 7474 7761 726e 2e6c   the `mqttwarn.l
-0001a5f0: 6f67 6020 6669 6c65 2077 6974 6820 6120  og` file with a 
-0001a600: 6064 6562 7567 6020 6c61 6265 6c2e 2054  `debug` label. T
-0001a610: 6869 7320 6f66 2063 6f75 7273 6520 6173  his of course as
-0001a620: 7375 6d65 7320 7468 6174 2079 6f75 2068  sumes that you h
-0001a630: 6176 6520 636f 6e66 6967 7572 6564 2074  ave configured t
-0001a640: 6865 206c 6f67 2073 6563 7469 6f6e 2074  he log section t
-0001a650: 6865 2077 6179 2064 6573 6372 6962 6564  he way described
-0001a660: 205b 6162 6f76 655d 2823 7468 652d 636f   [above](#the-co
-0001a670: 6e66 6967 7878 782d 7365 6374 696f 6e73  nfigxxx-sections
-0001a680: 292e 200a 0a42 7574 206d 7174 7477 6172  ). ..But mqttwar
-0001a690: 6e20 7072 6f76 6964 6573 2073 6576 6572  n provides sever
-0001a6a0: 616c 206f 7074 696f 6e73 2074 6f20 6372  al options to cr
-0001a6b0: 6561 7465 2061 2064 6966 6665 7265 6e74  eate a different
-0001a6c0: 206f 7574 626f 756e 6420 6d65 7373 6167   outbound messag
-0001a6d0: 652c 2061 6c6c 6f77 696e 6720 796f 7520  e, allowing you 
-0001a6e0: 666f 7220 6578 616d 706c 6520 746f 206d  for example to m
-0001a6f0: 616b 6520 796f 7572 206f 7574 626f 756e  ake your outboun
-0001a700: 6420 6d65 7373 6167 6520 6d6f 7265 2068  d message more h
-0001a710: 756d 616e 2d72 6561 6461 626c 652e 200a  uman-readable. .
-0001a720: 0a54 6865 2074 6974 6c65 2061 6e64 2066  .The title and f
-0001a730: 6f72 6d61 7420 6469 7265 6374 6976 6573  ormat directives
-0001a740: 2064 6566 696e 6520 7468 6520 7469 746c   define the titl
-0001a750: 6520 616e 6420 7468 6520 626f 6479 206f  e and the body o
-0001a760: 6620 7468 6520 6f75 7462 6f75 6e64 206d  f the outbound m
-0001a770: 6573 7361 6765 2e20 4865 7265 2c20 796f  essage. Here, yo
-0001a780: 7520 6361 6e20 7475 726e 2061 6e20 4d51  u can turn an MQ
-0001a790: 5454 2070 6179 6c6f 6164 2074 6861 7420  TT payload that 
-0001a7a0: 7369 6d70 6c79 2073 7461 7465 7320 224f  simply states "O
-0001a7b0: 4e22 2c20 696e 746f 2061 2066 7269 656e  N", into a frien
-0001a7c0: 646c 6965 7220 7665 7273 696f 6e2e 200a  dlier version. .
-0001a7d0: 0a60 6060 0a5b 6f66 6669 6365 2f75 7073  .```.[office/ups
-0001a7e0: 5d0a 7469 746c 6520 3d20 4f66 6669 6365  ].title = Office
-0001a7f0: 2055 5053 0a66 6f72 6d61 7420 3d20 5468   UPS.format = Th
-0001a800: 6520 6f66 6669 6365 2055 5053 2069 7320  e office UPS is 
-0001a810: 7b70 6179 6c6f 6164 7d0a 6060 600a 0a4e  {payload}.```..N
-0001a820: 6f74 6963 6520 7468 6174 2074 6865 206f  otice that the o
-0001a830: 7269 6769 6e61 6c20 4d51 5454 2070 6179  riginal MQTT pay
-0001a840: 6c6f 6164 2069 7320 7265 6665 7265 6e63  load is referenc
-0001a850: 6564 2c20 736f 2074 6861 7420 6966 2074  ed, so that if t
-0001a860: 6865 2055 5053 2069 7320 7377 6974 6368  he UPS is switch
-0001a870: 6564 206f 6666 2061 6e64 2073 656e 6473  ed off and sends
-0001a880: 206f 7574 2061 2063 6f72 7265 7370 6f6e   out a correspon
-0001a890: 6469 6e67 204d 5154 5420 6d65 7373 6167  ding MQTT messag
-0001a8a0: 652c 2074 6865 206f 7574 626f 756e 6420  e, the outbound 
-0001a8b0: 6d65 7373 6167 6520 7769 6c6c 2073 7461  message will sta
-0001a8c0: 7465 2074 6865 2073 616d 652e 2054 6865  te the same. The
-0001a8d0: 2069 6e66 6f72 6d61 7469 6f6e 2074 6861   information tha
-0001a8e0: 7420 6973 2061 7661 696c 6162 6c65 2074  t is available t
-0001a8f0: 6f20 796f 7520 696e 2063 7265 6174 696e  o you in creatin
-0001a900: 6720 7468 6520 6f75 7462 6f75 6e64 206d  g the outbound m
-0001a910: 6573 7361 6765 2c20 6973 2063 616c 6c65  essage, is calle
-0001a920: 6420 7468 6520 7472 616e 7366 6f72 6d61  d the transforma
-0001a930: 7469 6f6e 2064 6174 612e 2054 6865 2076  tion data. The v
-0001a940: 6572 7920 6261 7369 6320 7365 7420 6f66  ery basic set of
-0001a950: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-0001a960: 6461 7461 2069 7320 7468 6520 666f 6c6c  data is the foll
-0001a970: 6f77 696e 6720 3a20 0a0a 6060 6070 7974  owing : ..```pyt
-0001a980: 686f 6e0a 7b0a 2020 2774 6f70 6963 2720  hon.{.  'topic' 
-0001a990: 2020 2020 2020 2020 3a20 746f 7069 6320          : topic 
-0001a9a0: 6e61 6d65 0a20 2027 7061 796c 6f61 6427  name.  'payload'
-0001a9b0: 2020 2020 2020 203a 2074 6f70 6963 2070         : topic p
-0001a9c0: 6179 6c6f 6164 0a20 2027 5f64 7465 706f  ayload.  '_dtepo
-0001a9d0: 6368 2720 2020 2020 203a 2065 706f 6368  ch'      : epoch
-0001a9e0: 2074 696d 6520 2020 2020 2020 2020 2020   time           
-0001a9f0: 2020 2020 2020 2023 2031 3339 3236 3238         # 1392628
-0001aa00: 3538 310a 2020 275f 6474 6973 6f27 2020  581.  '_dtiso'  
-0001aa10: 2020 2020 2020 3a20 4953 4f20 6461 7465        : ISO date
-0001aa20: 2028 5554 4329 2020 2020 2020 2020 2020   (UTC)          
-0001aa30: 2020 2020 2320 3230 3134 2d30 322d 3137      # 2014-02-17
-0001aa40: 5431 303a 3338 3a34 332e 3931 3036 3931  T10:38:43.910691
-0001aa50: 5a0a 2020 275f 6474 6868 6d6d 2720 2020  Z.  '_dthhmm'   
-0001aa60: 2020 2020 3a20 7469 6d65 7374 616d 7020      : timestamp 
-0001aa70: 4848 3a4d 4d20 286c 6f63 616c 2920 2020  HH:MM (local)   
-0001aa80: 2020 2320 3130 3a31 360a 2020 275f 6474    # 10:16.  '_dt
-0001aa90: 6868 6d6d 7373 2720 2020 2020 3a20 7469  hhmmss'     : ti
-0001aaa0: 6d65 7374 616d 7020 4848 3a4d 4d3a 5353  mestamp HH:MM:SS
-0001aab0: 2028 6c6f 6361 6c29 2020 2320 3130 3a31   (local)  # 10:1
-0001aac0: 363a 3231 0a7d 0a60 6060 0a0a 2323 2320  6:21.}.```..### 
-0001aad0: 5472 616e 7366 6f72 6d69 6e67 2069 6e62  Transforming inb
-0001aae0: 6f75 6e64 204a 534f 4e0a 0a49 6e20 6164  ound JSON..In ad
-0001aaf0: 6469 7469 6f6e 2074 6f20 7061 7373 696e  dition to passin
-0001ab00: 6720 7468 6520 7061 796c 6f61 6420 7265  g the payload re
-0001ab10: 6365 6976 6564 2076 6961 204d 5154 5420  ceived via MQTT 
-0001ab20: 746f 2061 2073 6572 7669 6365 2c20 5f6d  to a service, _m
-0001ab30: 7174 7477 6172 6e5f 2061 6c6c 6f77 7320  qttwarn_ allows 
-0001ab40: 796f 7520 646f 2064 6f20 7468 6520 666f  you do do the fo
-0001ab50: 6c6c 6f77 696e 673a 0a0a 2a20 5472 616e  llowing:..* Tran
-0001ab60: 7366 6f72 6d20 7061 796c 6f61 6473 206f  sform payloads o
-0001ab70: 6e20 6120 7065 722f 746f 7069 6320 6261  n a per/topic ba
-0001ab80: 7369 732e 2046 6f72 2065 7861 6d70 6c65  sis. For example
-0001ab90: 2c20 796f 7520 6b6e 6f77 2079 6f75 276c  , you know you'l
-0001aba0: 6c20 6265 2072 6563 6569 7669 6e67 204a  l be receiving J
-0001abb0: 534f 4e2c 2062 7574 2079 6f75 2077 616e  SON, but you wan
-0001abc0: 7420 746f 2077 6172 6e20 7769 7468 2061  t to warn with a
-0001abd0: 206e 6963 656c 7920 666f 726d 6174 7465   nicely formatte
-0001abe0: 6420 6d65 7373 6167 652e 0a2a 2046 6f72  d message..* For
-0001abf0: 2063 6572 7461 696e 2073 6572 7669 6365   certain service
-0001ac00: 732c 2079 6f75 2063 616e 2063 6861 6e67  s, you can chang
-0001ac10: 6520 7468 6520 5f74 6974 6c65 5f20 286f  e the _title_ (o
-0001ac20: 7220 5f73 7562 6a65 6374 5f29 206f 6620  r _subject_) of 
-0001ac30: 7468 6520 6f75 7467 6f69 6e67 206d 6573  the outgoing mes
-0001ac40: 7361 6765 2e0a 2a20 466f 7220 6365 7274  sage..* For cert
-0001ac50: 6169 6e20 7365 7276 6963 6573 2c20 796f  ain services, yo
-0001ac60: 7520 6361 6e20 6368 616e 6765 2074 6865  u can change the
-0001ac70: 205f 7072 696f 7269 7479 5f20 6f66 2074   _priority_ of t
-0001ac80: 6865 206f 7574 676f 696e 6720 6d65 7373  he outgoing mess
-0001ac90: 6167 652e 0a0a 436f 6e73 6964 6572 2074  age...Consider t
-0001aca0: 6865 2066 6f6c 6c6f 7769 6e67 204a 534f  he following JSO
-0001acb0: 4e20 7061 796c 6f61 6420 7075 626c 6973  N payload publis
-0001acc0: 6865 6420 746f 2074 6865 204d 5154 5420  hed to the MQTT 
-0001acd0: 6272 6f6b 6572 3a0a 0a60 6060 7368 656c  broker:..```shel
-0001ace0: 6c0a 6d6f 7371 7569 7474 6f5f 7075 6220  l.mosquitto_pub 
-0001acf0: 2d74 2027 6f73 782f 6a73 6f6e 2720 2d6d  -t 'osx/json' -m
-0001ad00: 2027 7b22 6672 7569 7422 3a22 6261 6e61   '{"fruit":"bana
-0001ad10: 6e61 222c 2022 7072 6963 6522 3a20 3633  na", "price": 63
-0001ad20: 2c20 2274 7374 2220 3a20 2231 3339 3137  , "tst" : "13917
-0001ad30: 3739 3333 3622 7d27 0a60 6060 0a0a 5573  79336"}'.```..Us
-0001ad40: 696e 6720 6066 6f72 6d61 7460 2077 6520  ing `format` we 
-0001ad50: 6361 6e20 636f 6e66 6967 7572 6520 5f6d  can configure _m
-0001ad60: 7174 7477 6172 6e5f 2074 6f20 7472 616e  qttwarn_ to tran
-0001ad70: 7366 6f72 6d20 7468 6174 204a 534f 4e20  sform that JSON 
-0001ad80: 696e 746f 2061 2064 6966 6665 7265 6e74  into a different
-0001ad90: 206f 7574 676f 696e 6720 6d65 7373 6167   outgoing messag
-0001ada0: 6520 7768 6963 6820 6973 2074 6865 2074  e which is the t
-0001adb0: 6578 7420 7468 6174 2069 7320 6163 7475  ext that is actu
-0001adc0: 616c 6c79 206e 6f74 6966 6965 642e 2050  ally notified. P
-0001add0: 6172 7420 6f66 2073 6169 6420 6066 6f72  art of said `for
-0001ade0: 6d61 7460 206c 6f6f 6b73 206c 696b 6520  mat` looks like 
-0001adf0: 7468 6973 2069 6e20 7468 6520 636f 6e66  this in the conf
-0001ae00: 6967 7572 6174 696f 6e20 6669 6c65 2c20  iguration file, 
-0001ae10: 616e 6420 6261 7369 6361 6c6c 7920 7370  and basically sp
-0001ae20: 6563 6966 6965 7320 7468 6174 206d 6573  ecifies that mes
-0001ae30: 7361 6765 7320 7075 626c 6973 6865 6420  sages published 
-0001ae40: 746f 2060 6f73 782f 6a73 6f6e 6020 7368  to `osx/json` sh
-0001ae50: 6f75 6c64 2062 6520 7472 616e 7366 6f72  ould be transfor
-0001ae60: 6d65 6420 6173 206f 6e20 7468 6520 7269  med as on the ri
-0001ae70: 6768 742d 6861 6e64 2073 6964 652e 0a0a  ght-hand side...
-0001ae80: 6060 6069 6e69 0a66 6f72 6d61 7420 3d20  ```ini.format = 
-0001ae90: 2249 276c 6c20 6861 7665 2061 207b 6672  "I'll have a {fr
-0001aea0: 7569 747d 2069 6620 6974 2063 6f73 7473  uit} if it costs
-0001aeb0: 207b 7072 6963 657d 220a 6060 600a 0a28   {price}".```..(
-0001aec0: 456d 6265 6464 6564 2060 225c 6e22 6020  Embedded `"\n"` 
-0001aed0: 6172 6520 636f 6e76 6572 7465 6420 746f  are converted to
-0001aee0: 206e 6577 6c69 6e65 7320 6f6e 206f 7574   newlines on out
-0001aef0: 7075 742e 290a 0a54 6865 2072 6573 756c  put.)..The resul
-0001af00: 7420 6973 3a0a 0a21 5b4f 5358 206e 6f74  t is:..![OSX not
-0001af10: 6966 6965 725d 2861 7373 6574 732f 6465  ifier](assets/de
-0001af20: 736b 746f 706e 6f74 6966 792e 6a70 6729  sktopnotify.jpg)
-0001af30: 0a0a 596f 7520 6173 736f 6369 6174 6520  ..You associate 
-0001af40: 4d51 5454 2074 6f70 6963 2062 7261 6e63  MQTT topic branc
-0001af50: 6865 7320 746f 2061 7070 6c69 6361 7469  hes to applicati
-0001af60: 6f6e 7320 696e 2074 6865 2063 6f6e 6669  ons in the confi
-0001af70: 6775 7261 7469 6f6e 2066 696c 6520 2863  guration file (c
-0001af80: 6f70 7920 606d 7174 7477 6172 6e2e 696e  opy `mqttwarn.in
-0001af90: 692e 7361 6d70 6c65 6020 746f 2060 6d71  i.sample` to `mq
-0001afa0: 7474 7761 726e 2e69 6e69 6020 666f 7220  ttwarn.ini` for 
-0001afb0: 7573 6529 2e20 496e 206f 7468 6572 2077  use). In other w
-0001afc0: 6f72 6473 2c20 796f 7520 6361 6e20 6163  ords, you can ac
-0001afd0: 636f 6d70 6c69 7368 2c20 7361 792c 2066  complish, say, f
-0001afe0: 6f6c 6c6f 7769 6e67 206d 6170 7069 6e67  ollowing mapping
-0001aff0: 733a 0a0a 2a20 5055 4273 2074 6f20 606f  s:..* PUBs to `o
-0001b000: 776e 7472 6163 6b73 2f6a 616e 652f 6970  wntracks/jane/ip
-0001b010: 686f 6e65 6020 7368 6f75 6c64 2062 6520  hone` should be 
-0001b020: 6e6f 7469 6669 6564 2076 6961 2050 7573  notified via Pus
-0001b030: 686f 7665 7220 746f 204a 6f68 6e27 7320  hover to John's 
-0001b040: 7068 6f6e 650a 2a20 5055 4273 2074 6f20  phone.* PUBs to 
-0001b050: 606f 7065 6e68 6162 2f74 656d 7065 7261  `openhab/tempera
-0001b060: 7475 7265 6020 7368 6f75 6c64 2062 6520  ture` should be 
-0001b070: 5477 6565 7465 640a 2a20 5055 4273 2074  Tweeted.* PUBs t
-0001b080: 6f20 6068 6f6d 652f 6d6f 6e69 746f 7269  o `home/monitori
-0001b090: 6e67 2f61 6c65 7274 2f2b 6020 7368 6f75  ng/alert/+` shou
-0001b0a0: 6c64 206e 6f74 6966 7920 5477 6974 7465  ld notify Twitte
-0001b0b0: 722c 204d 6169 6c2c 2061 6e64 2050 726f  r, Mail, and Pro
-0001b0c0: 776c 0a0a 5365 6520 6465 7461 696c 7320  wl..See details 
-0001b0d0: 696e 2074 6865 2063 6f6e 6669 6720 7361  in the config sa
-0001b0e0: 6d70 6c65 2066 6f72 2068 6f77 2074 6f20  mple for how to 
-0001b0f0: 636f 6e66 6967 7572 6520 7468 6973 2073  configure this s
-0001b100: 6372 6970 742e 0a54 6865 2070 6174 6820  cript..The path 
-0001b110: 746f 2074 6865 2063 6f6e 6669 6775 7261  to the configura
-0001b120: 7469 6f6e 2066 696c 6520 2877 6869 6368  tion file (which
-0001b130: 206d 7573 7420 6265 2076 616c 6964 2050   must be valid P
-0001b140: 7974 686f 6e29 2069 7320 6f62 7461 696e  ython) is obtain
-0001b150: 6564 2066 726f 6d20 7468 6520 604d 5154  ed from the `MQT
-0001b160: 5457 4152 4e49 4e49 6020 656e 7669 726f  TWARNINI` enviro
-0001b170: 6e6d 656e 7420 7661 7269 6162 6c65 2077  nment variable w
-0001b180: 6869 6368 2064 6566 6175 6c74 7320 746f  hich defaults to
-0001b190: 2060 6d71 7474 7761 726e 2e69 6e69 6020   `mqttwarn.ini` 
-0001b1a0: 696e 2074 6865 2063 7572 7265 6e74 2064  in the current d
-0001b1b0: 6972 6563 746f 7279 2e0a 0a45 7665 6e20  irectory...Even 
-0001b1c0: 6d6f 7265 2061 6476 616e 6365 642c 2077  more advanced, w
-0001b1d0: 6865 6e20 7265 6365 6976 696e 6720 4a53  hen receiving JS
-0001b1e0: 4f4e 2064 6174 6120 6c69 6b65 2060 7b22  ON data like `{"
-0001b1f0: 6461 7461 223a 207b 2268 756d 6964 6974  data": {"humidit
-0001b200: 7922 3a20 3632 2e31 387d 7d60 2c20 796f  y": 62.18}}`, yo
-0001b210: 7520 6d69 6768 740a 7761 6e74 2074 6f20  u might.want to 
-0001b220: 6578 7472 6163 7420 7661 6c75 6573 2075  extract values u
-0001b230: 7369 6e67 2074 6865 2060 666f 726d 6174  sing the `format
-0001b240: 6020 6d65 6368 616e 6973 6d20 6265 666f  ` mechanism befo
-0001b250: 7265 2066 6f72 7761 7264 696e 670a 6974  re forwarding.it
-0001b260: 2074 6f20 6f74 6865 7220 6461 7461 2073   to other data s
-0001b270: 696e 6b73 2c20 6c69 6b65 0a0a 6060 6069  inks, like..```i
-0001b280: 6e69 0a66 6f72 6d61 7420 3d20 227b 6461  ni.format = "{da
-0001b290: 7461 7d22 0a60 6060 0a0a 486f 7765 7665  ta}".```..Howeve
-0001b2a0: 722c 2074 6865 206f 7574 636f 6d65 2077  r, the outcome w
-0001b2b0: 696c 6c20 6265 2074 6865 2073 7472 696e  ill be the strin
-0001b2c0: 672d 7365 7269 616c 697a 6564 2066 6f72  g-serialized for
-0001b2d0: 6d20 6f66 2074 6865 2050 7974 686f 6e0a  m of the Python.
-0001b2e0: 7265 7072 6573 656e 7461 7469 6f6e 3a20  representation: 
-0001b2f0: 607b 7527 6875 6d69 6469 7479 273a 2036  `{u'humidity': 6
-0001b300: 322e 3138 7d60 2c20 7768 6963 6820 636f  2.18}`, which co
-0001b310: 756c 6420 6e6f 7420 6265 2077 6861 7420  uld not be what 
-0001b320: 796f 750a 7761 6e74 2069 6620 796f 7572  you.want if your
-0001b330: 2064 6174 6120 7369 6e6b 2069 7320 6578   data sink is ex
-0001b340: 7065 6374 696e 6720 4a53 4f4e 2066 6f72  pecting JSON for
-0001b350: 6d61 7420 6167 6169 6e2e 0a0a 546f 2061  mat again...To a
-0001b360: 6368 6965 7665 2074 6869 732c 2079 6f75  chieve this, you
-0001b370: 2073 686f 756c 6420 7573 6520 6170 7072   should use appr
-0001b380: 6f70 7269 6174 6520 7479 7065 2063 6f65  opriate type coe
-0001b390: 7263 696f 6e20 6265 666f 7265 0a66 6f72  rcion before.for
-0001b3a0: 6d61 7474 696e 672c 206c 696b 650a 0a60  matting, like..`
-0001b3b0: 6060 696e 690a 666f 726d 6174 203d 2022  ``ini.format = "
-0001b3c0: 7b64 6174 6121 6a7d 220a 6060 600a 0a54  {data!j}".```..T
-0001b3d0: 6869 7320 7769 6c6c 2073 6572 6961 6c69  his will seriali
-0001b3e0: 7a65 2074 6865 2066 6f72 6d61 7474 6564  ze the formatted
-0001b3f0: 2064 6174 6120 746f 204a 534f 4e20 666f   data to JSON fo
-0001b400: 726d 6174 2061 7070 726f 7072 6961 7465  rmat appropriate
-0001b410: 6c79 2c0a 736f 2074 6865 206f 7574 636f  ly,.so the outco
-0001b420: 6d65 2077 696c 6c20 6265 2060 7b22 6875  me will be `{"hu
-0001b430: 6d69 6469 7479 223a 2036 322e 3138 7d60  midity": 62.18}`
-0001b440: 2e0a 0a23 2323 2320 4e65 7374 6564 204a  ...#### Nested J
-0001b450: 534f 4e0a 0a57 6974 6869 6e20 7465 6d70  SON..Within temp
-0001b460: 6c61 7465 7320 616e 6420 666f 726d 6174  lates and format
-0001b470: 732c 2079 6f75 2063 616e 2072 6566 6572  s, you can refer
-0001b480: 206f 6e6c 7920 746f 2074 6865 2074 6f70   only to the top
-0001b490: 2d6c 6576 656c 206e 616d 6573 206f 6620  -level names of 
-0001b4a0: 616e 2069 6e63 6f6d 696e 6720 4a53 4f4e  an incoming JSON
-0001b4b0: 206d 6573 7361 6765 2c0a 7768 6963 6820   message,.which 
-0001b4c0: 7369 676e 6966 6963 616e 746c 7920 6c69  significantly li
-0001b4d0: 6d69 7473 2074 6865 206b 696e 6473 206f  mits the kinds o
-0001b4e0: 6620 6d65 7373 6167 6573 2060 6d71 7474  f messages `mqtt
-0001b4f0: 7761 726e 6020 6361 6e20 7072 6f63 6573  warn` can proces
-0001b500: 732e 2041 205b 736f 6c75 7469 6f6e 2069  s. A [solution i
-0001b510: 7320 696e 2074 6865 2077 6f72 6b73 5d28  s in the works](
-0001b520: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0001b530: 6f6d 2f6a 706d 656e 732f 6d71 7474 7761  om/jpmens/mqttwa
-0001b540: 726e 2f69 7373 7565 732f 3330 3329 0a66  rn/issues/303).f
-0001b550: 6f72 2074 6869 732c 2062 7574 2069 6e20  or this, but in 
-0001b560: 7468 6520 6d65 616e 7469 6d65 2079 6f75  the meantime you
-0001b570: 2063 616e 2075 7365 2061 6e20 6061 6c6c   can use an `all
-0001b580: 6461 7461 6020 6675 6e63 7469 6f6e 2074  data` function t
-0001b590: 6f20 7472 616e 7366 6f72 6d20 7468 6520  o transform the 
-0001b5a0: 4a53 4f4e 2069 6e74 6f20 736f 6d65 7468  JSON into someth
-0001b5b0: 696e 6720 0a60 6d71 7474 7761 726e 6020  ing .`mqttwarn` 
-0001b5c0: 5f63 616e 5f20 7072 6f63 6573 732e 0a0a  _can_ process...
-0001b5d0: 5468 6520 7472 6963 6b20 6973 2074 6f20  The trick is to 
-0001b5e0: 6275 696c 6420 6120 6e65 7720 4a53 4f4e  build a new JSON
-0001b5f0: 206d 6573 7361 6765 2077 6974 6820 5f6f   message with _o
-0001b600: 6e6c 795f 2074 6f70 2d6c 6576 656c 2076  nly_ top-level v
-0001b610: 616c 7565 732c 2073 7065 6369 6669 6361  alues, specifica
-0001b620: 6c6c 7920 7468 6520 7661 6c75 6573 2079  lly the values y
-0001b630: 6f75 206e 6565 642e 0a0a 2323 2320 4375  ou need...### Cu
-0001b640: 7374 6f6d 2066 756e 6374 696f 6e73 0a0a  stom functions..
-0001b650: 4120 746f 7069 6320 7365 6374 696f 6e20  A topic section 
-0001b660: 696e 2074 6865 2049 4e49 2066 696c 6520  in the INI file 
-0001b670: 6361 6e20 6861 7665 2070 726f 7065 7274  can have propert
-0001b680: 6965 7320 7365 7420 6173 2070 6572 2074  ies set as per t
-0001b690: 6865 2074 6162 6c65 2061 7420 7468 6520  he table at the 
-0001b6a0: 626f 7474 6f6d 206f 6620 5b74 6869 7320  bottom of [this 
-0001b6b0: 7365 6374 696f 6e5d 2868 7474 7073 3a2f  section](https:/
-0001b6c0: 2f67 6974 6875 622e 636f 6d2f 6a70 6d65  /github.com/jpme
-0001b6d0: 6e73 2f6d 7174 7477 6172 6e23 7468 652d  ns/mqttwarn#the-
-0001b6e0: 5f5f 746f 7069 635f 5f2d 7365 6374 696f  __topic__-sectio
-0001b6f0: 6e73 292e 2054 6865 2060 7461 7267 6574  ns). The `target
-0001b700: 7360 2c20 6074 6f70 6963 6020 616e 6420  s`, `topic` and 
-0001b710: 6071 6f73 6020 7072 6f70 6572 7469 6573  `qos` properties
-0001b720: 2063 616e 206e 6f74 2062 6520 6465 6669   can not be defi
-0001b730: 6e65 6420 7769 7468 2061 2066 756e 6374  ned with a funct
-0001b740: 696f 6e2e 200a 0a23 2323 2320 546f 7069  ion. ..#### Topi
-0001b750: 632d 7365 6374 696f 6e20 7072 6f70 6572  c-section proper
-0001b760: 7469 6573 2074 6861 7420 6361 6e20 6361  ties that can ca
-0001b770: 6c6c 2061 2063 7573 746f 6d20 6675 6e63  ll a custom func
-0001b780: 7469 6f6e 0a0a 2d20 6064 6174 616d 6170  tion..- `datamap
-0001b790: 6020 3a20 6469 6374 696f 6e61 7279 2c20  ` : dictionary, 
-0001b7a0: 6f72 2061 2066 756e 6374 696f 6e20 7468  or a function th
-0001b7b0: 6174 2072 6574 7572 6e73 2061 2064 6963  at returns a dic
-0001b7c0: 7469 6f6e 6172 790a 2d20 6061 6c6c 6461  tionary.- `allda
-0001b7d0: 7461 6020 3a20 6469 6374 696f 6e61 7279  ta` : dictionary
-0001b7e0: 2c20 6f72 2061 2066 756e 6374 696f 6e20  , or a function 
-0001b7f0: 7468 6174 2072 6574 7572 6e73 2061 2064  that returns a d
-0001b800: 6963 7469 6f6e 6172 790a 2d20 6066 696c  ictionary.- `fil
-0001b810: 7465 7260 203a 2062 6f6f 6c65 616e 2c20  ter` : boolean, 
-0001b820: 6f72 2061 2066 756e 6374 696f 6e20 7468  or a function th
-0001b830: 6174 2072 6574 7572 6e73 2061 2062 6f6f  at returns a boo
-0001b840: 6c65 616e 0a2d 2060 7469 746c 6560 203a  lean.- `title` :
-0001b850: 2073 7472 696e 672c 206f 7220 6120 6675   string, or a fu
-0001b860: 6e63 7469 6f6e 2074 6861 7420 7265 7475  nction that retu
-0001b870: 726e 7320 6120 7374 7269 6e67 0a2d 2060  rns a string.- `
-0001b880: 666f 726d 6174 6020 3a20 7374 7269 6e67  format` : string
-0001b890: 2c20 6f72 2061 2066 756e 6374 696f 6e20  , or a function 
-0001b8a0: 7468 6174 2072 6574 7572 6e73 2061 2073  that returns a s
-0001b8b0: 7472 696e 670a 2d20 6070 7269 6f72 6974  tring.- `priorit
-0001b8c0: 7960 203a 2073 6565 2062 656c 6f77 0a2d  y` : see below.-
-0001b8d0: 2060 696d 6167 6560 203a 2073 6565 2062   `image` : see b
-0001b8e0: 656c 6f77 0a0a 2323 2323 2044 6174 6120  elow..#### Data 
-0001b8f0: 6d61 7070 696e 6720 6675 6e63 7469 6f6e  mapping function
-0001b900: 730a 0a42 6f74 6820 7468 6520 6064 6174  s..Both the `dat
-0001b910: 616d 6170 6020 616e 6420 7468 6520 6061  amap` and the `a
-0001b920: 6c6c 6461 7461 6020 7072 6f70 6572 7469  lldata` properti
-0001b930: 6573 2069 6e20 6120 746f 7069 6320 7365  es in a topic se
-0001b940: 6374 696f 6e20 6361 6e20 6361 6c6c 2061  ction can call a
-0001b950: 2066 756e 6374 696f 6e20 7768 6963 6820   function which 
-0001b960: 7265 7475 726e 7320 6120 5b64 6963 7469  returns a [dicti
-0001b970: 6f6e 6172 795d 2868 7474 7073 3a2f 2f64  onary](https://d
-0001b980: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f32  ocs.python.org/2
-0001b990: 2f74 7574 6f72 6961 6c2f 6461 7461 7374  /tutorial/datast
-0001b9a0: 7275 6374 7572 6573 2e68 746d 6c23 6469  ructures.html#di
-0001b9b0: 6374 696f 6e61 7269 6573 292e 2054 6865  ctionaries). The
-0001b9c0: 206b 6579 7320 696e 2074 6869 7320 6469   keys in this di
-0001b9d0: 6374 696f 6e61 7279 2063 616e 2062 6520  ctionary can be 
-0001b9e0: 7573 6564 2077 6865 6e20 6465 7363 7269  used when descri
-0001b9f0: 6269 6e67 2074 6865 206f 7574 626f 756e  bing the outboun
-0001ba00: 6420 6074 6974 6c65 6020 616e 6420 6066  d `title` and `f
-0001ba10: 6f72 6d61 7460 2070 726f 7065 7274 6965  ormat` propertie
-0001ba20: 7320 6f66 2074 6865 2073 616d 6520 746f  s of the same to
-0001ba30: 7069 6320 7365 6374 696f 6e2e 0a0a 2d20  pic section...- 
-0001ba40: 6074 6f70 6963 603a 2063 6f6e 7461 696e  `topic`: contain
-0001ba50: 7320 7468 6520 7661 6c75 6520 696e 2060  s the value in `
-0001ba60: 6461 7461 5b27 746f 7069 6327 5d60 0a2d  data['topic']`.-
-0001ba70: 2060 6461 7461 603a 2070 726f 7669 6465   `data`: provide
-0001ba80: 7320 6163 6365 7373 2074 6f20 736f 6d65  s access to some
-0001ba90: 2069 6e66 6f72 6d61 7469 6f6e 206f 6620   information of 
-0001baa0: 7468 6520 696e 626f 756e 6420 4d51 5454  the inbound MQTT
-0001bab0: 2074 7261 6e73 6d69 7373 696f 6e2c 205b   transmission, [
-0001bac0: 6d6f 7265 2064 6574 6169 6c20 6865 7265  more detail here
-0001bad0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0001bae0: 2e63 6f6d 2f6a 706d 656e 732f 6d71 7474  .com/jpmens/mqtt
-0001baf0: 7761 726e 2374 7261 6e73 666f 726d 6174  warn#transformat
-0001bb00: 696f 6e2d 6461 7461 290a 2d20 6073 6572  ion-data).- `ser
-0001bb10: 7669 6365 603a 2070 726f 7669 6465 7320  vice`: provides 
-0001bb20: 6163 6365 7373 2074 6f20 7468 6520 696e  access to the in
-0001bb30: 7374 616e 6365 206f 6620 7468 6520 6070  stance of the `p
-0001bb40: 6168 6f2e 6d71 7474 2e63 6c69 656e 742e  aho.mqtt.client.
-0001bb50: 436c 6965 6e74 6020 6f62 6a65 6374 2028  Client` object (
-0001bb60: 7768 6963 6820 7072 6f76 6964 6573 2061  which provides a
-0001bb70: 2070 6c65 7468 6f72 6120 6f66 2070 726f   plethora of pro
-0001bb80: 7065 7274 6965 7320 616e 6420 6d65 7468  perties and meth
-0001bb90: 6f64 7329 2c20 746f 2074 6865 2060 6d71  ods), to the `mq
-0001bba0: 7474 7761 726e 6020 6c6f 6767 696e 6720  ttwarn` logging 
-0001bbb0: 7365 7475 702c 2074 6f20 7468 6520 5079  setup, to the Py
-0001bbc0: 7468 6f6e 2060 676c 6f62 616c 7328 2960  thon `globals()`
-0001bbd0: 206d 6574 686f 6420 616e 6420 616c 6c20   method and all 
-0001bbe0: 7468 6174 2065 6e74 6169 6c73 2c20 616e  that entails, an
-0001bbf0: 6420 746f 2074 6865 206e 616d 6520 6f66  d to the name of
-0001bc00: 2074 6865 2073 6372 6970 742e 200a 0a23   the script. ..#
-0001bc10: 2323 2320 4669 6c74 6572 2066 756e 6374  ### Filter funct
-0001bc20: 696f 6e73 0a0a 4120 6675 6e63 7469 6f6e  ions..A function
-0001bc30: 2063 616c 6c65 6420 6672 6f6d 2074 6865   called from the
-0001bc40: 2060 6669 6c74 6572 6020 7072 6f70 6572   `filter` proper
-0001bc50: 7479 2069 6e20 6120 746f 7069 6320 7365  ty in a topic se
-0001bc60: 6374 696f 6e20 6e65 6564 7320 746f 2072  ction needs to r
-0001bc70: 6574 7572 6e20 6046 616c 7365 6020 746f  eturn `False` to
-0001bc80: 2073 746f 7020 7468 6520 6f75 7462 6f75   stop the outbou
-0001bc90: 6e64 206e 6f74 6966 6963 6174 696f 6e2e  nd notification.
-0001bca0: 2049 7420 6861 7320 6163 6365 7373 2074   It has access t
-0001bcb0: 6f20 7468 6520 6074 6f70 6963 6020 616e  o the `topic` an
-0001bcc0: 6420 7468 6520 606d 6573 7361 6765 6020  d the `message` 
-0001bcd0: 7374 7269 6e67 7320 6f66 2074 6865 2069  strings of the i
-0001bce0: 6e62 6f75 6e64 204d 5154 5420 7472 616e  nbound MQTT tran
-0001bcf0: 736d 6973 7369 6f6e 2e20 0a0a 2323 2323  smission. ..####
-0001bd00: 204f 7574 7075 7420 6675 6e63 7469 6f6e   Output function
-0001bd10: 730a 0a42 6f74 6820 7468 6520 6074 6974  s..Both the `tit
-0001bd20: 6c65 6020 616e 6420 7468 6520 6066 6f72  le` and the `for
-0001bd30: 6d61 7460 2070 726f 7065 7274 6965 7320  mat` properties 
-0001bd40: 696e 2074 6865 2074 6f70 6963 2073 6563  in the topic sec
-0001bd50: 7469 6f6e 2063 616e 2063 6f6e 7461 696e  tion can contain
-0001bd60: 2061 2073 7472 696e 6720 7768 6572 6520   a string where 
-0001bd70: 607b 6272 6163 6b65 7465 647d 6020 7265  `{bracketed}` re
-0001bd80: 6665 7265 6e63 6573 2067 6574 2072 6573  ferences get res
-0001bd90: 6f6c 7665 6420 7573 696e 6720 7468 6520  olved using the 
-0001bda0: 6469 6374 696f 6e61 7279 2072 6574 7572  dictionary retur
-0001bdb0: 6e65 6420 6672 6f6d 2061 2064 6174 6120  ned from a data 
-0001bdc0: 6d61 7070 696e 6720 6675 6e63 7469 6f6e  mapping function
-0001bdd0: 2e20 4f72 2074 6865 7920 6361 6e20 6361  . Or they can ca
-0001bde0: 6c6c 2061 2066 756e 6374 696f 6e20 7468  ll a function th
-0001bdf0: 6174 2072 6574 7572 6e73 2061 2073 7472  at returns a str
-0001be00: 696e 6720 7468 6174 206d 6179 206f 7220  ing that may or 
-0001be10: 6d61 7920 6e6f 7420 636f 6e74 6169 6e20  may not contain 
-0001be20: 7375 6368 2072 6566 6572 656e 6365 732e  such references.
-0001be30: 2054 6865 2066 756e 6374 696f 6e73 2063   The functions c
-0001be40: 616c 6c65 6420 6865 7265 2064 6f20 6e6f  alled here do no
-0001be50: 7420 6861 7665 2061 6363 6573 7320 746f  t have access to
-0001be60: 2074 6865 2061 6374 7561 6c20 6469 6374   the actual dict
-0001be70: 696f 6e61 7279 2072 6574 7572 6e65 6420  ionary returned 
-0001be80: 6672 6f6d 2064 6174 6120 6d61 7070 696e  from data mappin
-0001be90: 6720 6675 6e63 7469 6f6e 7320 7468 6f75  g functions thou
-0001bea0: 6768 2e0a 0a23 2323 2320 4e6f 7465 730a  gh...#### Notes.
-0001beb0: 0a57 6865 6e20 7772 6974 696e 6720 6375  .When writing cu
-0001bec0: 7374 6f6d 2066 756e 6374 696f 6e73 2c20  stom functions, 
-0001bed0: 6974 2063 616e 2062 6520 6469 6666 6963  it can be diffic
-0001bee0: 756c 7420 746f 2064 6574 6572 6d69 6e65  ult to determine
-0001bef0: 2077 6861 7420 7468 6520 6973 7375 6520   what the issue 
-0001bf00: 6973 2077 6865 6e20 6765 7474 696e 6720  is when getting 
-0001bf10: 616e 2065 7272 6f72 206d 6573 7361 6765  an error message
-0001bf20: 2073 7563 6820 6173 0a0a 6060 600a 5741   such as..```.WA
-0001bf30: 524e 494e 4720 5b6d 7174 7477 6172 6e5d  RNING [mqttwarn]
-0001bf40: 2043 616e 6e6f 7420 696e 766f 6b65 2066   Cannot invoke f
-0001bf50: 696c 7465 7220 6675 6e63 7469 6f6e 2078  ilter function x
-0001bf60: 7878 7820 6465 6669 6e65 6420 696e 2079  xxx defined in y
-0001bf70: 7979 7979 3a20 2e2e 2e0a 6060 600a 0a54  yyyy: ....```..T
-0001bf80: 6869 7320 6973 2074 7970 6963 616c 6c79  his is typically
-0001bf90: 2069 6e64 6963 6174 6573 2076 6172 6961   indicates varia
-0001bfa0: 626c 6573 206f 7220 6675 6e63 7469 6f6e  bles or function
-0001bfb0: 2063 616c 6c73 2077 6869 6368 2068 6176   calls which hav
-0001bfc0: 656e 2774 2062 6565 6e20 6465 6669 6e65  en't been define
-0001bfd0: 6420 6f72 2073 696d 696c 6172 2e0a 0a23  d or similar...#
-0001bfe0: 2323 2320 4578 616d 706c 6573 0a0a 4265  ### Examples..Be
-0001bff0: 6c6f 7720 6172 6520 6120 6e75 6d62 6572  low are a number
-0001c000: 206f 6620 6578 616d 706c 6520 7363 656e   of example scen
-0001c010: 6172 696f 7320 7768 6572 6520 6375 7374  arios where cust
-0001c020: 6f6d 2066 756e 6374 696f 6e73 2061 7265  om functions are
-0001c030: 2062 6569 6e67 2075 7365 642e 0a0a 2323   being used...##
-0001c040: 2323 2320 5573 696e 6720 6675 6e63 7469  ### Using functi
-0001c050: 6f6e 7320 746f 2072 6570 6c61 6365 2069  ons to replace i
-0001c060: 6e63 6f6d 696e 6720 7061 796c 6f61 6473  ncoming payloads
-0001c070: 0a0a 436f 6e73 6964 6572 2074 6865 2066  ..Consider the f
-0001c080: 6f6c 6c6f 7769 6e67 2063 6f6e 6669 6775  ollowing configu
-0001c090: 7261 7469 6f6e 2073 6e69 7070 6574 2069  ration snippet i
-0001c0a0: 6e20 6164 6469 7469 6f6e 2074 6f20 7468  n addition to th
-0001c0b0: 6520 636f 6e66 6967 7572 6174 696f 6e0a  e configuration.
-0001c0c0: 6f66 2074 6865 2060 6d71 7474 6020 7365  of the `mqtt` se
-0001c0d0: 7276 6963 6520 7368 6f77 6e20 6162 6f76  rvice shown abov
-0001c0e0: 653a 0a0a 4164 6420 7468 6973 2074 6f20  e:..Add this to 
-0001c0f0: 6120 6375 7374 6f6d 2050 7974 686f 6e20  a custom Python 
-0001c100: 6669 6c65 2c20 6c69 6b65 2c20 652e 672e  file, like, e.g.
-0001c110: 2060 2f65 7463 2f6d 7174 7477 6172 6e2f   `/etc/mqttwarn/
-0001c120: 6d79 6675 6e63 7469 6f6e 732e 7079 602e  myfunctions.py`.
-0001c130: 0a60 6060 7079 7468 6f6e 0a64 6566 206c  .```python.def l
-0001c140: 6f6f 6b75 705f 6461 7461 2864 6174 612c  ookup_data(data,
-0001c150: 2073 7276 3d4e 6f6e 6529 3a0a 2020 2020   srv=None):.    
-0001c160: 6966 2074 7970 6528 6461 7461 2920 3d3d  if type(data) ==
-0001c170: 2064 6963 7420 616e 6420 2766 7275 6974   dict and 'fruit
-0001c180: 2720 696e 2064 6174 613a 0a20 2020 2020  ' in data:.     
-0001c190: 2020 2020 2020 2072 6574 7572 6e20 2241         return "A
-0001c1a0: 6e61 6e61 7322 0a20 2020 2072 6574 7572  nanas".    retur
-0001c1b0: 6e20 4e6f 6e65 0a60 6060 0a0a 5265 6769  n None.```..Regi
-0001c1c0: 7374 6572 2074 6861 7420 6669 6c65 2062  ster that file b
-0001c1d0: 7920 7361 7969 6e67 3a0a 0a60 6060 696e  y saying:..```in
-0001c1e0: 690a 5b64 6566 6175 6c74 735d 0a3b 2070  i.[defaults].; p
-0001c1f0: 6174 6820 746f 2066 696c 6520 636f 6e74  ath to file cont
-0001c200: 6169 6e69 6e67 2073 656c 662d 6465 6669  aining self-defi
-0001c210: 6e65 6420 6675 6e63 7469 6f6e 7320 666f  ned functions fo
-0001c220: 7220 666f 726d 6174 6d61 7020 616e 6420  r formatmap and 
-0001c230: 6461 7461 6d61 700a 6675 6e63 7469 6f6e  datamap.function
-0001c240: 7320 3d20 276d 7966 756e 6374 696f 6e73  s = 'myfunctions
-0001c250: 2e70 7927 0a60 6060 0a0a 5468 656e 2c20  .py'.```..Then, 
-0001c260: 696e 2074 6865 2073 6563 7469 6f6e 2064  in the section d
-0001c270: 6566 696e 696e 6720 7468 6520 746f 7069  efining the topi
-0001c280: 6320 7765 206c 6973 7465 6e20 6f6e 3a0a  c we listen on:.
-0001c290: 0a60 6060 696e 690a 2e2e 2e0a 5b74 6573  .```ini.....[tes
-0001c2a0: 742f 746f 7069 635d 0a23 666f 726d 6174  t/topic].#format
-0001c2b0: 203d 2020 5369 6e63 6520 7768 656e 2064   =  Since when d
-0001c2c0: 6f65 7320 6120 7b66 7275 6974 7d20 636f  oes a {fruit} co
-0001c2d0: 7374 207b 7072 6963 657d 3f0a 666f 726d  st {price}?.form
-0001c2e0: 6174 203d 2020 6c6f 6f6b 7570 5f64 6174  at =  lookup_dat
-0001c2f0: 6128 290a 6060 600a 0a48 6572 652c 2077  a().```..Here, w
-0001c300: 6520 7265 706c 6163 6564 2074 6865 2060  e replaced the `
-0001c310: 666f 726d 6174 6d61 7060 2065 6e74 7279  formatmap` entry
-0001c320: 2066 6f72 2074 6865 2074 6f70 6963 2062   for the topic b
-0001c330: 7920 6120 6375 7374 6f6d 2066 756e 6374  y a custom funct
-0001c340: 696f 6e2e 0a0a 5468 6573 6520 6675 6e63  ion...These func
-0001c350: 7469 6f6e 7320 6172 6520 696e 766f 6b65  tions are invoke
-0001c360: 6420 7769 7468 2064 6563 6f64 6564 204a  d with decoded J
-0001c370: 534f 4e20 6064 6174 6160 2070 6173 7365  SON `data` passe
-0001c380: 6420 746f 2074 6865 6d20 6173 2061 0a5f  d to them as a._
-0001c390: 6469 6374 5f2e 2054 6865 2073 7472 696e  dict_. The strin
-0001c3a0: 6720 7265 7475 726e 6564 2020 6279 2074  g returned  by t
-0001c3b0: 6865 2066 756e 6374 696f 6e20 7265 7475  he function retu
-0001c3c0: 726e 6564 2073 7472 696e 6720 7265 706c  rned string repl
-0001c3d0: 6163 6573 2074 6865 0a6f 7574 676f 696e  aces the.outgoin
-0001c3e0: 6720 606d 6573 7361 6765 603a 0a0a 6060  g `message`:..``
-0001c3f0: 600a 696e 2f61 3120 7b22 6672 7569 7422  `.in/a1 {"fruit"
-0001c400: 3a22 7069 6e65 6170 706c 6522 2c20 2270  :"pineapple", "p
-0001c410: 7269 6365 223a 2031 3331 2c20 2274 7374  rice": 131, "tst
-0001c420: 2220 3a20 2231 3339 3137 3739 3333 3622  " : "1391779336"
-0001c430: 7d0a 6f75 742f 666f 6f64 2041 6e61 6e61  }.out/food Anana
-0001c440: 730a 6f75 742f 6672 7569 742f 7069 6e65  s.out/fruit/pine
-0001c450: 6170 706c 6520 416e 616e 6173 0a60 6060  apple Ananas.```
-0001c460: 0a0a 596f 7520 6361 6e20 6465 6669 6e65  ..You can define
-0001c470: 2063 7573 746f 6d20 6675 6e63 7469 6f6e   custom function
-0001c480: 7320 696e 2061 2050 7974 686f 6e20 6669  s in a Python fi
-0001c490: 6c65 2077 6869 6368 2079 6f75 2063 6f6e  le which you con
-0001c4a0: 6669 6775 7265 2061 730a 6066 756e 6374  figure as.`funct
-0001c4b0: 696f 6e73 6020 696e 2074 6865 2060 5b64  ions` in the `[d
-0001c4c0: 6566 6175 6c74 5d60 2073 6563 7469 6f6e  efault]` section
-0001c4d0: 206f 6620 7468 6520 606d 7174 7477 6172   of the `mqttwar
-0001c4e0: 6e2e 696e 6960 2063 6f6e 6669 6775 7261  n.ini` configura
-0001c4f0: 7469 6f6e 0a66 696c 652c 2061 7320 6f75  tion.file, as ou
-0001c500: 746c 696e 6564 2061 626f 7665 2e20 5768  tlined above. Wh
-0001c510: 656e 2072 656c 6174 6976 6520 6669 6c65  en relative file
-0001c520: 206e 616d 6573 2061 7265 2067 6976 656e   names are given
-0001c530: 2c20 7468 6579 2077 696c 6c20 6265 0a72  , they will be.r
-0001c540: 6573 6f6c 7665 6420 6672 6f6d 2074 6865  esolved from the
-0001c550: 2064 6972 6563 746f 7279 206f 6620 7468   directory of th
-0001c560: 6520 606d 7174 7477 6172 6e2e 696e 6960  e `mqttwarn.ini`
-0001c570: 2066 696c 652c 2077 6869 6368 2069 732c   file, which is,
-0001c580: 2062 7920 6465 6661 756c 742c 0a74 6865   by default,.the
-0001c590: 2060 2f65 7463 2f6d 7174 7477 6172 6e60   `/etc/mqttwarn`
-0001c5a0: 2066 6f6c 6465 722e 0a0a 4966 2061 2066   folder...If a f
-0001c5b0: 756e 6374 696f 6e20 6f70 6572 6174 696e  unction operatin
-0001c5c0: 6720 6f6e 2061 206d 6573 7361 6765 2028  g on a message (
-0001c5d0: 692e 652e 2077 6974 6869 6e20 6066 6f72  i.e. within `for
-0001c5e0: 6d61 7420 3d60 2920 7265 7475 726e 7320  mat =`) returns 
-0001c5f0: 604e 6f6e 6560 206f 7220 616e 2065 6d70  `None` or an emp
-0001c600: 7479 2073 7472 696e 672c 2074 6865 2074  ty string, the t
-0001c610: 6172 6765 7420 6e6f 7469 6669 6361 7469  arget notificati
-0001c620: 6f6e 2069 7320 7375 7070 7265 7373 6564  on is suppressed
-0001c630: 2e0a 0a54 6865 206f 7074 696f 6e61 6c20  ...The optional 
-0001c640: 6073 7276 6020 6973 2061 6e20 6f62 6a65  `srv` is an obje
-0001c650: 6374 2077 6974 6820 736f 6d65 2068 656c  ct with some hel
-0001c660: 7065 7220 6675 6e63 7469 6f6e 732e 2049  per functions. I
-0001c670: 6e20 7061 7274 6963 756c 6172 2c20 7468  n particular, th
-0001c680: 6573 6520 616c 6c6f 7720 7573 2074 6f20  ese allow us to 
-0001c690: 7573 6520 5f6d 7174 7477 6172 6e5f 2773  use _mqttwarn_'s
-0001c6a0: 206c 6f67 6769 6e67 2061 6e64 204d 5154   logging and MQT
-0001c6b0: 5420 7075 626c 6973 6820 6675 6e63 7469  T publish functi
-0001c6c0: 6f6e 732c 2061 7320 696e 2074 6869 7320  ons, as in this 
-0001c6d0: 6578 616d 706c 653a 0a0a 6060 6070 7974  example:..```pyt
-0001c6e0: 686f 6e0a 6465 6620 7030 3146 6f72 6d61  hon.def p01Forma
-0001c6f0: 7428 6461 7461 2c20 7372 7629 3a0a 2020  t(data, srv):.  
-0001c700: 2020 7320 3d20 2270 3031 2d48 4f4c 4122    s = "p01-HOLA"
-0001c710: 0a0a 2020 2020 7372 762e 6c6f 6767 696e  ..    srv.loggin
-0001c720: 672e 696e 666f 2822 2b2b 2b2b 2b2b 2b2b  g.info("++++++++
-0001c730: 2b2b 2b20 4855 4855 2229 0a0a 2020 2020  +++ HUHU")..    
-0001c740: 7372 762e 6d71 7474 632e 7075 626c 6973  srv.mqttc.publis
-0001c750: 6828 2270 3031 2f52 4553 506f 6e73 6522  h("p01/RESPonse"
-0001c760: 2c20 732c 2071 6f73 3d30 2c20 7265 7461  , s, qos=0, reta
-0001c770: 696e 3d46 616c 7365 290a 0a20 2020 2072  in=False)..    r
-0001c780: 6574 7572 6e20 730a 6060 600a 0a42 6520  eturn s.```..Be 
-0001c790: 6164 7669 7365 6420 7468 6174 2069 6620  advised that if 
-0001c7a0: 796f 7520 4d51 5454 2070 7562 6c69 7368  you MQTT publish
-0001c7b0: 2062 6163 6b20 746f 2074 6865 2073 616d   back to the sam
-0001c7c0: 6520 746f 7069 6320 7768 6963 6820 7472  e topic which tr
-0001c7d0: 6967 6765 7265 6420 7468 6520 696e 766f  iggered the invo
-0001c7e0: 6361 7469 6f6e 0a6f 6620 796f 7572 2066  cation.of your f
-0001c7f0: 756e 6374 696f 6e2c 2079 6f75 276c 6c20  unction, you'll 
-0001c800: 6372 6561 7465 2061 6e20 656e 646c 6573  create an endles
-0001c810: 7320 6c6f 6f70 2e0a 0a23 2323 2323 2049  s loop...##### I
-0001c820: 6e63 6f72 706f 7261 7469 6e67 2074 6f70  ncorporating top
-0001c830: 6963 206e 616d 6573 2069 6e74 6f20 7472  ic names into tr
-0001c840: 616e 7366 6f72 6d61 7469 6f6e 2064 6174  ansformation dat
-0001c850: 610a 0a41 6e20 4d51 5454 2074 6f70 6963  a..An MQTT topic
-0001c860: 2062 7261 6e63 6820 6e61 6d65 2063 6f6e   branch name con
-0001c870: 7461 696e 7320 696e 666f 726d 6174 696f  tains informatio
-0001c880: 6e20 796f 7520 6d61 7920 7761 6e74 2074  n you may want t
-0001c890: 6f20 7573 6520 696e 2074 7261 6e73 666f  o use in transfo
-0001c8a0: 726d 6174 696f 6e73 2e0a 4173 2061 2072  rmations..As a r
-0001c8b0: 6174 6865 7220 6578 7472 656d 6520 6578  ather extreme ex
-0001c8c0: 616d 706c 652c 2063 6f6e 7369 6465 7220  ample, consider 
-0001c8d0: 7468 6520 5b4f 776e 5472 6163 6b73 5d20  the [OwnTracks] 
-0001c8e0: 7072 6f67 7261 6d20 2874 6865 0a61 7274  program (the.art
-0001c8f0: 6973 7420 666f 726d 6572 6c79 206b 6e6f  ist formerly kno
-0001c900: 776e 2061 7320 5f4d 5154 5469 7475 6465  wn as _MQTTitude
-0001c910: 5f29 2e0a 0a57 6865 6e20 616e 205b 4f77  _)...When an [Ow
-0001c920: 6e54 7261 636b 735d 2064 6576 6963 6520  nTracks] device 
-0001c930: 6465 7465 6374 7320 6120 6368 616e 6765  detects a change
-0001c940: 206f 6620 6120 636f 6e66 6967 7572 6564   of a configured
-0001c950: 2077 6179 706f 696e 7420 6f72 2067 656f   waypoint or geo
-0001c960: 2d66 656e 6365 2028 6120 7265 6769 6f6e  -fence (a region
-0001c970: 206d 6f6e 6974 6f72 696e 6720 6120 7573   monitoring a us
-0001c980: 6572 2063 616e 2073 6574 2075 7020 6f6e  er can set up on
-0001c990: 2074 6865 2064 6576 6963 6529 2c20 6974   the device), it
-0001c9a0: 2065 6d69 7473 2061 204a 534f 4e20 7061   emits a JSON pa
-0001c9b0: 796c 6f61 6420 7768 6963 6820 6c6f 6f6b  yload which look
-0001c9c0: 7320 6c69 6b65 2074 6869 732c 206f 6e20  s like this, on 
-0001c9d0: 6120 746f 7069 6320 6e61 6d65 2063 6f6e  a topic name con
-0001c9e0: 7369 7374 696e 6720 6f66 2060 6f77 6e74  sisting of `ownt
-0001c9f0: 7261 636b 732f 5f75 7365 726e 616d 655f  racks/_username_
-0001ca00: 2f5f 6465 7669 6365 6964 5f60 3a0a 0a60  /_deviceid_`:..`
-0001ca10: 6060 0a6f 776e 7472 6163 6b73 2f6a 616e  ``.owntracks/jan
-0001ca20: 652f 7068 6f6e 6520 2d6d 2027 7b22 5f74  e/phone -m '{"_t
-0001ca30: 7970 6522 3a20 226c 6f63 6174 696f 6e22  ype": "location"
-0001ca40: 2c20 226c 6174 223a 2022 3532 2e34 3737  , "lat": "52.477
-0001ca50: 3033 3532 2220 2e2e 2020 2264 6573 6322  0352" ..  "desc"
-0001ca60: 3a20 2248 6f6d 6522 2c20 2265 7665 6e74  : "Home", "event
-0001ca70: 223a 2022 6c65 6176 6522 7d27 0a60 6060  ": "leave"}'.```
-0001ca80: 0a0a 496e 206f 7264 6572 2074 6f20 6265  ..In order to be
-0001ca90: 2061 626c 6520 746f 206f 6274 6169 6e20   able to obtain 
-0001caa0: 7468 6520 7573 6572 6e61 6d65 2028 606a  the username (`j
-0001cab0: 616e 6560 2920 616e 6420 6865 7220 6465  ane`) and her de
-0001cac0: 7669 6365 206e 616d 6520 2860 7068 6f6e  vice name (`phon
-0001cad0: 6560 2920 666f 7220 7573 650a 696e 2074  e`) for use.in t
-0001cae0: 7261 6e73 666f 726d 6174 696f 6e73 2028  ransformations (
-0001caf0: 7365 6520 7072 6576 696f 7573 2073 6563  see previous sec
-0001cb00: 7469 6f6e 292c 2077 6520 776f 756c 6420  tion), we would 
-0001cb10: 6964 6561 6c6c 7920 7761 6e74 2074 6f20  ideally want to 
-0001cb20: 7061 7273 6520 7468 6520 4d51 5454 2074  parse the MQTT t
-0001cb30: 6f70 6963 206e 616d 6520 616e 6420 6164  opic name and ad
-0001cb40: 6420 7468 6174 2074 6f20 7468 6520 6974  d that to the it
-0001cb50: 656d 2064 6174 6120 6f75 7220 706c 7567  em data our plug
-0001cb60: 696e 7320 6f62 7461 696e 2e20 5965 732c  ins obtain. Yes,
-0001cb70: 2077 6520 6361 6e2e 0a0a 416e 206f 7074   we can...An opt
-0001cb80: 696f 6e61 6c20 6064 6174 616d 6170 6020  ional `datamap` 
-0001cb90: 696e 206f 7572 2063 6f6e 6669 6775 7261  in our configura
-0001cba0: 7469 6f6e 2066 696c 6520 6465 6669 6e65  tion file define
-0001cbb0: 7320 7468 6520 6e61 6d65 206f 6620 6120  s the name of a 
-0001cbc0: 6675 6e63 7469 6f6e 2077 6520 7072 6f76  function we prov
-0001cbd0: 6964 652c 2061 6c73 6f20 696e 2074 6865  ide, also in the
-0001cbe0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-0001cbf0: 696c 652c 2077 6869 6368 2061 6363 6f6d  ile, which accom
-0001cc00: 706c 6973 6865 7320 7468 6174 2e0a 0a60  plishes that...`
-0001cc10: 6060 696e 690a 5b6f 776e 7472 6163 6b73  ``ini.[owntracks
-0001cc20: 2f6a 616e 652f 7068 6f6e 655d 0a64 6174  /jane/phone].dat
-0001cc30: 616d 6170 203d 204f 776e 5472 6163 6b73  amap = OwnTracks
-0001cc40: 546f 7069 6344 6174 614d 6170 2829 0a60  TopicDataMap().`
-0001cc50: 6060 0a0a 5468 6973 2073 7065 6369 6669  ``..This specifi
-0001cc60: 6573 2074 6861 7420 7768 656e 2061 206d  es that when a m
-0001cc70: 6573 7361 6765 2066 6f72 2074 6865 2064  essage for the d
-0001cc80: 6566 696e 6564 2074 6f70 6963 2060 6f77  efined topic `ow
-0001cc90: 6e74 7261 636b 732f 6a61 6e65 2f70 686f  ntracks/jane/pho
-0001cca0: 6e65 6020 6973 2070 726f 6365 7373 6564  ne` is processed
-0001ccb0: 2c20 6f75 7220 6675 6e63 7469 6f6e 2060  , our function `
-0001ccc0: 4f77 6e54 7261 636b 7354 6f70 6963 4461  OwnTracksTopicDa
-0001ccd0: 7461 4d61 7028 2960 2073 686f 756c 6420  taMap()` should 
-0001cce0: 6265 2069 6e76 6f6b 6564 2074 6f20 7061  be invoked to pa
-0001ccf0: 7273 6520 7468 6174 2e20 2841 7320 7573  rse that. (As us
-0001cd00: 7561 6c2c 2074 6f70 6963 206e 616d 6573  ual, topic names
-0001cd10: 206d 6179 2063 6f6e 7461 696e 204d 5154   may contain MQT
-0001cd20: 5420 7769 6c64 6361 7264 732e 290a 0a54  T wildcards.)..T
-0001cd30: 6865 2066 756e 6374 696f 6e20 7765 2064  he function we d
-0001cd40: 6566 696e 6520 746f 2064 6f20 7468 6174  efine to do that
-0001cd50: 2069 733a 0a0a 6060 6070 7974 686f 6e0a   is:..```python.
-0001cd60: 6465 6620 4f77 6e54 7261 636b 7354 6f70  def OwnTracksTop
-0001cd70: 6963 4461 7461 4d61 7028 746f 7069 6329  icDataMap(topic)
-0001cd80: 3a0a 2020 2020 6966 2074 7970 6528 746f  :.    if type(to
-0001cd90: 7069 6329 203d 3d20 7374 723a 0a20 2020  pic) == str:.   
-0001cda0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001cdb0: 2020 2020 2020 2320 6f77 6e74 7261 636b        # owntrack
-0001cdc0: 732f 7573 6572 6e61 6d65 2f64 6576 6963  s/username/devic
-0001cdd0: 650a 2020 2020 2020 2020 2020 2020 7061  e.            pa
-0001cde0: 7274 7320 3d20 746f 7069 632e 7370 6c69  rts = topic.spli
-0001cdf0: 7428 272f 2729 0a20 2020 2020 2020 2020  t('/').         
-0001ce00: 2020 2075 7365 726e 616d 6520 3d20 7061     username = pa
-0001ce10: 7274 735b 315d 0a20 2020 2020 2020 2020  rts[1].         
-0001ce20: 2020 2064 6576 6963 6569 6420 3d20 7061     deviceid = pa
-0001ce30: 7274 735b 325d 0a20 2020 2020 2020 2065  rts[2].        e
-0001ce40: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-0001ce50: 2020 2064 6576 6963 6569 6420 3d20 2775     deviceid = 'u
-0001ce60: 6e6b 6e6f 776e 270a 2020 2020 2020 2020  nknown'.        
-0001ce70: 2020 2020 7573 6572 6e61 6d65 203d 2027      username = '
-0001ce80: 756e 6b6e 6f77 6e27 0a20 2020 2020 2020  unknown'.       
-0001ce90: 2072 6574 7572 6e20 6469 6374 2875 7365   return dict(use
-0001cea0: 726e 616d 653d 7573 6572 6e61 6d65 2c20  rname=username, 
-0001ceb0: 6465 7669 6365 3d64 6576 6963 6569 6429  device=deviceid)
-0001cec0: 0a20 2020 2072 6574 7572 6e20 4e6f 6e65  .    return None
-0001ced0: 0a60 6060 0a0a 5468 6520 7265 7475 726e  .```..The return
-0001cee0: 6564 205f 6469 6374 5f20 6973 206d 6572  ed _dict_ is mer
-0001cef0: 6765 6420 696e 746f 2074 6865 2074 7261  ged into the tra
-0001cf00: 6e73 666f 726d 6174 696f 6e20 6461 7461  nsformation data
-0001cf10: 2c20 692e 652e 2069 7420 6973 206d 6164  , i.e. it is mad
-0001cf20: 6520 6176 6169 6c61 626c 6520 746f 2070  e available to p
-0001cf30: 6c75 6769 6e73 2061 6e64 2074 6f20 7472  lugins and to tr
-0001cf40: 616e 7366 6f72 6d61 7469 6f6e 2072 756c  ansformation rul
-0001cf50: 6573 2028 6066 6f72 6d61 7460 292e 2049  es (`format`). I
-0001cf60: 6620 7765 2074 6865 6e20 6372 6561 7465  f we then create
-0001cf70: 2074 6865 2066 6f6c 6c6f 7769 6e67 2072   the following r
-0001cf80: 756c 650a 0a60 6060 696e 690a 666f 726d  ule..```ini.form
-0001cf90: 6174 203d 207b 7573 6572 6e61 6d65 7d3a  at = {username}:
-0001cfa0: 207b 6576 656e 747d 203d 3e20 7b64 6573   {event} => {des
-0001cfb0: 637d 0a60 6060 0a0a 7468 6520 6162 6f76  c}.```..the abov
-0001cfc0: 6520 5055 426c 6973 6820 7769 6c6c 2062  e PUBlish will b
-0001cfd0: 6520 7472 616e 7366 6f72 6d65 6420 696e  e transformed in
-0001cfe0: 746f 0a0a 6060 600a 6a61 6e65 3a20 6c65  to..```.jane: le
-0001cff0: 6176 6520 3d3e 2048 6f6d 650a 6060 600a  ave => Home.```.
-0001d000: 0a23 2323 2323 204d 6572 6769 6e67 206d  .##### Merging m
-0001d010: 6f72 6520 6461 7461 2023 2323 0a0a 5468  ore data ###..Th
-0001d020: 6520 6f70 7469 6f6e 616c 2060 616c 6c64  e optional `alld
-0001d030: 6174 6160 2066 756e 6374 696f 6e20 796f  ata` function yo
-0001d040: 7520 7772 6974 6520 616e 6420 636f 6e66  u write and conf
-0001d050: 6967 7572 6520 6f6e 2061 2070 6572 2f74  igure on a per/t
-0001d060: 6f70 6963 2062 6173 6973 2c20 6973 0a70  opic basis, is.p
-0001d070: 6173 7365 6420 7468 6520 6d65 7373 6167  assed the messag
-0001d080: 6520 5f74 6f70 6963 5f2c 2069 7473 205f  e _topic_, its _
-0001d090: 6461 7461 5f20 616e 6420 616e 206f 7074  data_ and an opt
-0001d0a0: 696f 6e61 6c20 5f73 7276 5f20 6f62 6a65  ional _srv_ obje
-0001d0b0: 6374 2e20 5468 6973 2066 756e 6374 696f  ct. This functio
-0001d0c0: 6e0a 7368 6f75 6c64 2072 6574 7572 6e20  n.should return 
-0001d0d0: 6120 5f64 6963 745f 2028 6f72 205f 4e6f  a _dict_ (or _No
-0001d0e0: 6e65 5f29 206f 6620 6461 7461 2077 6869  ne_) of data whi
-0001d0f0: 6368 2069 7320 6d65 7267 6564 2069 6e74  ch is merged int
-0001d100: 6f20 7468 6520 7768 6f6c 650a 6c69 7374  o the whole.list
-0001d110: 206f 6620 7472 616e 7366 6f72 6d61 7469   of transformati
-0001d120: 6f6e 2064 6174 612e 2054 6869 7320 6578  on data. This ex
-0001d130: 7061 6e64 7320 6f6e 2074 6865 2074 776f  pands on the two
-0001d140: 206f 7468 6572 2074 7261 6e73 666f 726d   other transform
-0001d150: 6174 696f 6e20 6675 6e63 7469 6f6e 730a  ation functions.
-0001d160: 746f 206d 616b 6520 746f 7069 6320 616e  to make topic an
-0001d170: 6420 7468 6520 6d65 7373 6167 6527 7320  d the message's 
-0001d180: 7061 796c 6f61 6420 6176 6169 6c61 626c  payload availabl
-0001d190: 6520 7369 6d75 6c74 616e 656f 7573 6c79  e simultaneously
-0001d1a0: 2e0a 0a0a 2323 2323 2320 4120 6375 7374  ....##### A cust
-0001d1b0: 6f6d 2066 756e 6374 696f 6e20 746f 2063  om function to c
-0001d1c0: 6f6e 7665 7274 206e 6573 7465 6420 4a53  onvert nested JS
-0001d1d0: 4f4e 0a0a 466f 7220 6578 616d 706c 652c  ON..For example,
-0001d1e0: 2073 6179 2077 6520 6172 6520 7265 6365   say we are rece
-0001d1f0: 6976 696e 6720 6d65 7373 6167 6573 2066  iving messages f
-0001d200: 726f 6d20 6120 7465 6d70 6572 6174 7572  rom a temperatur
-0001d210: 6520 7365 6e73 6f72 200a 7275 6e6e 696e  e sensor .runnin
-0001d220: 6720 5b54 6173 6d6f 7461 5d28 6874 7470  g [Tasmota](http
-0001d230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-0001d240: 7265 6e64 7374 2f53 6f6e 6f66 662d 5461  rendst/Sonoff-Ta
-0001d250: 736d 6f74 612f 292c 0a61 6e64 2077 6520  smota/),.and we 
-0001d260: 7769 7368 2074 6f20 636f 6e76 6572 7420  wish to convert 
-0001d270: 7468 656d 2069 6e74 6f20 5b49 6e66 6c75  them into [Influ
-0001d280: 7844 4220 6c69 6e65 2066 6f72 6d61 745d  xDB line format]
-0001d290: 2868 7474 7073 3a2f 2f64 6f63 732e 696e  (https://docs.in
-0001d2a0: 666c 7578 6461 7461 2e63 6f6d 2f69 6e66  fluxdata.com/inf
-0001d2b0: 6c75 7864 622f 7631 2e36 2f77 7269 7465  luxdb/v1.6/write
-0001d2c0: 5f70 726f 746f 636f 6c73 2f6c 696e 655f  _protocols/line_
-0001d2d0: 7072 6f74 6f63 6f6c 5f74 7574 6f72 6961  protocol_tutoria
-0001d2e0: 6c2f 292e 0a0a 5468 6520 696e 636f 6d69  l/)...The incomi
-0001d2f0: 6e67 205b 4a53 4f4e 5d28 6874 7470 733a  ng [JSON](https:
-0001d300: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7265  //github.com/are
-0001d310: 6e64 7374 2f53 6f6e 6f66 662d 5461 736d  ndst/Sonoff-Tasm
-0001d320: 6f74 612f 7769 6b69 2f4a 534f 4e2d 5374  ota/wiki/JSON-St
-0001d330: 6174 7573 2d52 6573 706f 6e73 6573 2364  atus-Responses#d
-0001d340: 7331 3862 3230 2920 7769 6c6c 206c 6f6f  s18b20) will loo
-0001d350: 6b20 6c69 6b65 2074 6869 733a 0a60 6060  k like this:.```
-0001d360: 0a7b 0a20 2020 2022 5469 6d65 223a 2022  .{.    "Time": "
-0001d370: 3230 3138 2e30 322e 3031 2032 313a 3239  2018.02.01 21:29
-0001d380: 3a34 3022 2c0a 2020 2020 2244 5331 3842  :40",.    "DS18B
-0001d390: 3230 223a 207b 0a20 2020 2020 2022 5465  20": {.      "Te
-0001d3a0: 6d70 6572 6174 7572 6522 3a20 3139 2e37  mperature": 19.7
-0001d3b0: 0a20 2020 207d 2c0a 2020 2020 2254 656d  .    },.    "Tem
-0001d3c0: 7055 6e69 7422 3a20 2243 220a 7d2c 0a60  pUnit": "C".},.`
-0001d3d0: 6060 0a0a 5369 6e63 6520 6054 656d 7065  ``..Since `Tempe
-0001d3e0: 7261 7475 7265 6020 6361 6e6e 6f74 2062  rature` cannot b
-0001d3f0: 6520 7265 6665 7265 6e63 6564 2064 6972  e referenced dir
-0001d400: 6563 746c 7920 7769 7468 696e 2061 2060  ectly within a `
-0001d410: 666f 726d 6174 602c 2077 6520 6e65 6564  format`, we need
-0001d420: 2074 6f20 6d61 6b65 2069 7420 6120 746f   to make it a to
-0001d430: 702d 6c65 7665 6c20 7661 6c75 652e 200a  p-level value. .
-0001d440: 5768 696c 6520 7765 2772 6520 6174 2069  While we're at i
-0001d450: 742c 2077 6520 6361 6e20 6368 616e 6765  t, we can change
-0001d460: 2074 6865 2064 6174 6520 746f 206d 696c   the date to mil
-0001d470: 6c69 7365 636f 6e64 7320 7369 6e63 6520  liseconds since 
-0001d480: 7468 6520 6570 6f63 682c 2061 6e64 2069  the epoch, and i
-0001d490: 6e63 6c75 6465 2074 6865 2074 6f70 6963  nclude the topic
-0001d4a0: 3a0a 6060 600a 7b0a 2020 2020 2254 6f70  :.```.{.    "Top
-0001d4b0: 6963 223a 2022 7461 736d 6f74 612f 7465  ic": "tasmota/te
-0001d4c0: 6d70 2f64 732f 3122 2c20 0a20 2020 2022  mp/ds/1", .    "
-0001d4d0: 5469 6d65 7374 616d 7022 3a20 3135 3137  Timestamp": 1517
-0001d4e0: 3532 3533 3139 3030 302c 200a 2020 2020  525319000, .    
-0001d4f0: 2254 656d 7065 7261 7475 7265 223a 2031  "Temperature": 1
-0001d500: 392e 370a 7d0a 6060 600a 0a54 6869 7320  9.7.}.```..This 
-0001d510: 6361 6e20 6265 2061 6363 6f6d 706c 6973  can be accomplis
-0001d520: 6865 6420 7769 7468 2074 6865 2066 6f6c  hed with the fol
-0001d530: 6c6f 7769 6e67 2066 756e 6374 696f 6e3a  lowing function:
-0001d540: 200a 6060 600a 696d 706f 7274 2061 7374   .```.import ast
-0001d550: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
-0001d560: 696d 706f 7274 2074 696d 650a 6672 6f6d  import time.from
-0001d570: 2064 6174 6574 696d 6520 696d 706f 7274   datetime import
-0001d580: 2064 6174 6574 696d 650a 0a64 6566 2064   datetime..def d
-0001d590: 7331 3862 3230 5f76 616c 7565 7328 746f  s18b20_values(to
-0001d5a0: 7069 632c 2064 6174 612c 2073 7276 3d4e  pic, data, srv=N
-0001d5b0: 6f6e 6529 3a0a 2020 2020 7061 796c 6f61  one):.    payloa
-0001d5c0: 6420 3d20 6173 742e 6c69 7465 7261 6c5f  d = ast.literal_
-0001d5d0: 6576 616c 2864 6174 615b 2270 6179 6c6f  eval(data["paylo
-0001d5e0: 6164 225d 290a 2020 2020 7473 203d 2064  ad"]).    ts = d
-0001d5f0: 6174 6574 696d 652e 7374 7270 7469 6d65  atetime.strptime
-0001d600: 2870 6179 6c6f 6164 5b22 5469 6d65 225d  (payload["Time"]
-0001d610: 2c20 2225 592e 256d 2e25 6420 2548 3a25  , "%Y.%m.%d %H:%
-0001d620: 4d3a 2553 2229 0a20 2020 206d 696c 6c69  M:%S").    milli
-0001d630: 7320 3d20 6c6f 6e67 2874 696d 652e 6d6b  s = long(time.mk
-0001d640: 7469 6d65 2874 732e 7469 6d65 7475 706c  time(ts.timetupl
-0001d650: 6528 2929 202a 2031 3030 3029 0a20 2020  e()) * 1000).   
-0001d660: 2074 656d 7020 3d20 7061 796c 6f61 645b   temp = payload[
-0001d670: 2244 5331 3842 3230 225d 5b22 5465 6d70  "DS18B20"]["Temp
-0001d680: 6572 6174 7572 6522 5d0a 2020 2020 6420  erature"].    d 
-0001d690: 3d20 6469 6374 2820 546f 7069 6320 3d20  = dict( Topic = 
-0001d6a0: 746f 7069 632c 2054 696d 6573 7461 6d70  topic, Timestamp
-0001d6b0: 203d 206d 696c 6c69 732c 2054 656d 7065   = millis, Tempe
-0001d6c0: 7261 7475 7265 203d 2074 656d 7020 290a  rature = temp ).
-0001d6d0: 2020 2020 6c6f 6767 696e 672e 6465 6275      logging.debu
-0001d6e0: 6728 6429 0a20 2020 2072 6574 7572 6e20  g(d).    return 
-0001d6f0: 640a 6060 600a 0a41 7070 6c79 2069 7420  d.```..Apply it 
-0001d700: 746f 2061 2074 6f70 6963 2069 6e20 606d  to a topic in `m
-0001d710: 7174 7477 6172 6e2e 696e 6960 3a0a 6060  qttwarn.ini`:.``
-0001d720: 600a 5b74 6173 6d6f 7461 2f74 656d 702f  `.[tasmota/temp/
-0001d730: 6473 2f2b 5d0a 7461 7267 6574 7320 3d20  ds/+].targets = 
-0001d740: 6c6f 673a 696e 666f 0a61 6c6c 6461 7461  log:info.alldata
-0001d750: 203d 2064 7331 3862 3230 5f76 616c 7565   = ds18b20_value
-0001d760: 7328 290a 666f 726d 6174 2020 3d20 7765  s().format  = we
-0001d770: 6174 6865 722c 546f 7069 633d 7b54 6f70  ather,Topic={Top
-0001d780: 6963 7d20 5465 6d70 6572 6174 7572 653d  ic} Temperature=
-0001d790: 7b54 656d 7065 7261 7475 7265 7d20 7b54  {Temperature} {T
-0001d7a0: 696d 6573 7461 6d70 7d0a 6060 600a 0a57  imestamp}.```..W
-0001d7b0: 6869 6368 2072 6573 756c 7473 2069 6e3a  hich results in:
-0001d7c0: 0a60 6060 0a32 3031 382d 3037 2d31 3920  .```.2018-07-19 
-0001d7d0: 3232 3a30 303a 3234 2c34 3532 2044 4542  22:00:24,452 DEB
-0001d7e0: 5547 205b 6d71 7474 7761 726e 5d20 4d65  UG [mqttwarn] Me
-0001d7f0: 7373 6167 6520 7265 6365 6976 6564 206f  ssage received o
-0001d800: 6e20 7461 736d 6f74 612f 7465 6d70 2f64  n tasmota/temp/d
-0001d810: 732f 313a 207b 2022 5469 6d65 223a 2022  s/1: { "Time": "
-0001d820: 3230 3138 2e30 322e 3031 2032 323a 3438  2018.02.01 22:48
-0001d830: 3a33 3922 2c20 2244 5331 3842 3230 223a  :39", "DS18B20":
-0001d840: 207b 2022 5465 6d70 6572 6174 7572 6522   { "Temperature"
-0001d850: 3a20 3139 2e37 207d 2c20 2254 656d 7055  : 19.7 }, "TempU
-0001d860: 6e69 7422 3a20 2243 2220 7d0a 3230 3138  nit": "C" }.2018
-0001d870: 2d30 372d 3139 2032 323a 3030 3a32 342c  -07-19 22:00:24,
-0001d880: 3435 3320 4445 4255 4720 5b6d 7174 7477  453 DEBUG [mqttw
-0001d890: 6172 6e5d 2053 6563 7469 6f6e 205b 7461  arn] Section [ta
-0001d8a0: 736d 6f74 612f 7465 6d70 2f64 732f 2b5d  smota/temp/ds/+]
-0001d8b0: 206d 6174 6368 6573 206d 6573 7361 6765   matches message
-0001d8c0: 206f 6e20 7461 736d 6f74 612f 7465 6d70   on tasmota/temp
-0001d8d0: 2f64 732f 312e 2050 726f 6365 7373 696e  /ds/1. Processin
-0001d8e0: 672e 2e2e 0a32 3031 382d 3037 2d31 3920  g....2018-07-19 
-0001d8f0: 3232 3a30 303a 3234 2c34 3537 2044 4542  22:00:24,457 DEB
-0001d900: 5547 205b 6675 6e63 735d 207b 2754 6f70  UG [funcs] {'Top
-0001d910: 6963 273a 2075 2774 6173 6d6f 7461 2f74  ic': u'tasmota/t
-0001d920: 656d 702f 6473 2f31 272c 2027 5469 6d65  emp/ds/1', 'Time
-0001d930: 7374 616d 7027 3a20 3135 3137 3532 3533  stamp': 15175253
-0001d940: 3139 3030 304c 2c20 2754 656d 7065 7261  19000L, 'Tempera
-0001d950: 7475 7265 273a 2031 392e 377d 0a32 3031  ture': 19.7}.201
-0001d960: 382d 3037 2d31 3920 3232 3a30 303a 3234  8-07-19 22:00:24
-0001d970: 2c34 3539 2044 4542 5547 205b 6d71 7474  ,459 DEBUG [mqtt
-0001d980: 7761 726e 5d20 4d65 7373 6167 6520 6f6e  warn] Message on
-0001d990: 2074 6173 6d6f 7461 2f74 656d 702f 6473   tasmota/temp/ds
-0001d9a0: 2f31 2067 6f69 6e67 2074 6f20 6c6f 673a  /1 going to log:
-0001d9b0: 696e 666f 0a32 3031 382d 3037 2d31 3920  info.2018-07-19 
-0001d9c0: 3232 3a30 303a 3234 2c34 3539 2044 4542  22:00:24,459 DEB
-0001d9d0: 5547 205b 6d71 7474 7761 726e 5d20 4e65  UG [mqttwarn] Ne
-0001d9e0: 7720 606c 6f67 3a69 6e66 6f27 206a 6f62  w `log:info' job
-0001d9f0: 3a20 7461 736d 6f74 612f 7465 6d70 2f64  : tasmota/temp/d
-0001da00: 732f 310a 3230 3138 2d30 372d 3139 2032  s/1.2018-07-19 2
-0001da10: 323a 3030 3a32 342c 3435 3920 4445 4255  2:00:24,459 DEBU
-0001da20: 4720 5b6d 7174 7477 6172 6e5d 2050 726f  G [mqttwarn] Pro
-0001da30: 6365 7373 6f72 2023 3020 6973 2068 616e  cessor #0 is han
-0001da40: 646c 696e 673a 2060 6c6f 6727 2066 6f72  dling: `log' for
-0001da50: 2069 6e66 6f0a 3230 3138 2d30 372d 3139   info.2018-07-19
-0001da60: 2032 323a 3030 3a32 342c 3436 3020 4445   22:00:24,460 DE
-0001da70: 4255 4720 5b6c 6f67 5d20 2a2a 2a20 4d4f  BUG [log] *** MO
-0001da80: 4455 4c45 3d73 6572 7669 6365 732f 6c6f  DULE=services/lo
-0001da90: 672e 7079 633a 2073 6572 7669 6365 3d6c  g.pyc: service=l
-0001daa0: 6f67 2c20 7461 7267 6574 3d69 6e66 6f0a  og, target=info.
-0001dab0: 3230 3138 2d30 372d 3139 2032 323a 3030  2018-07-19 22:00
-0001dac0: 3a32 342c 3436 3020 494e 464f 2020 5b6c  :24,460 INFO  [l
-0001dad0: 6f67 5d20 7765 6174 6865 722c 546f 7069  og] weather,Topi
-0001dae0: 633d 7461 736d 6f74 612f 7465 6d70 2f64  c=tasmota/temp/d
-0001daf0: 732f 3120 5465 6d70 6572 6174 7572 653d  s/1 Temperature=
-0001db00: 3139 2e37 2031 3531 3735 3235 3331 3930  19.7 15175253190
-0001db10: 3030 0a60 6060 0a0a 2323 2323 2320 546f  00.```..##### To
-0001db20: 7069 6320 7461 7267 6574 730a 0a42 7920  pic targets..By 
-0001db30: 696e 636f 7270 6f72 6174 696e 6720 7472  incorporating tr
-0001db40: 616e 7366 6f72 6d61 7469 6f6e 2064 6174  ansformation dat
-0001db50: 6120 696e 746f 2074 6f70 6963 2074 6172  a into topic tar
-0001db60: 6765 7473 2c20 7765 2063 616e 206d 616b  gets, we can mak
-0001db70: 6520 5f6d 7174 7477 6172 6e5f 2064 6973  e _mqttwarn_ dis
-0001db80: 7061 7463 680a 6d65 7373 6167 6573 2064  patch.messages d
-0001db90: 796e 616d 6963 616c 6c79 2062 6173 6564  ynamically based
-0001dba0: 206f 6e20 7468 6520 7661 6c75 6573 206f   on the values o
-0001dbb0: 6620 7468 6520 7472 616e 7366 6f72 6d61  f the transforma
-0001dbc0: 7469 6f6e 2064 6174 6120 6469 6374 696f  tion data dictio
-0001dbd0: 6e61 7279 2e0a 0a54 6f20 6765 7420 616e  nary...To get an
-0001dbe0: 2069 6465 6120 6162 6f75 7420 686f 7720   idea about how 
-0001dbf0: 7468 6973 2077 6f72 6b73 2c20 6c65 7427  this works, let'
-0001dc00: 7320 6465 6669 6e65 2061 2070 6c61 6365  s define a place
-0001dc10: 686f 6c64 6572 2076 6172 6961 626c 6520  holder variable 
-0001dc20: 696e 7369 6465 2074 6865 0a60 7461 7267  inside the.`targ
-0001dc30: 6574 7360 2064 6972 6563 7469 7665 206f  ets` directive o
-0001dc40: 6620 6120 746f 7069 6320 7365 6374 696f  f a topic sectio
-0001dc50: 6e20 696e 2074 6865 2060 6d71 7474 7761  n in the `mqttwa
-0001dc60: 726e 2e69 6e69 6020 636f 6e66 6967 7572  rn.ini` configur
-0001dc70: 6174 696f 6e20 6669 6c65 3a0a 0a20 2020  ation file:..   
-0001dc80: 205b 746f 7069 632d 7461 7267 6574 732d   [topic-targets-
-0001dc90: 6479 6e61 6d69 635d 0a20 2020 2074 6f70  dynamic].    top
-0001dca0: 6963 2020 203d 2074 6573 742f 746f 7069  ic   = test/topi
-0001dcb0: 632d 7461 7267 6574 732d 6479 6e61 6d69  c-targets-dynami
-0001dcc0: 630a 2020 2020 666f 726d 6174 2020 3d20  c.    format  = 
-0001dcd0: 536f 6d65 7468 696e 6720 7b6c 6f67 6c65  Something {logle
-0001dce0: 7665 6c7d 2068 6170 7065 6e65 6421 207b  vel} happened! {
-0001dcf0: 6d65 7373 6167 657d 0a20 2020 2074 6172  message}.    tar
-0001dd00: 6765 7473 203d 206c 6f67 3a7b 6c6f 676c  gets = log:{logl
-0001dd10: 6576 656c 7d0a 0a57 6865 6e20 7365 6e64  evel}..When send
-0001dd20: 696e 6720 7468 6973 2076 616c 7565 2074  ing this value t
-0001dd30: 6872 6f75 6768 2061 204a 534f 4e20 656e  hrough a JSON en
-0001dd40: 636f 6465 6420 6d65 7373 6167 6520 6f72  coded message or
-0001dd50: 2062 7920 636f 6d70 7574 696e 6720 6974   by computing it
-0001dd60: 0a74 6872 6f75 6768 2074 6865 2060 6461  .through the `da
-0001dd70: 7461 6d61 7060 206f 7220 6061 6c6c 6461  tamap` or `allda
-0001dd80: 7461 6020 7472 616e 7366 6f72 6d61 7469  ta` transformati
-0001dd90: 6f6e 206d 6163 6869 6e65 7279 2c20 6974  on machinery, it
-0001dda0: 2077 696c 6c20 6765 740a 696e 7465 7270   will get.interp
-0001ddb0: 6f6c 6174 6564 2069 6e74 6f20 7468 6520  olated into the 
-0001ddc0: 6465 7369 676e 6174 6564 2074 6f70 6963  designated topic
-0001ddd0: 2074 6172 6765 742e 2045 7861 6d70 6c65   target. Example
-0001dde0: 3a0a 0a20 2020 206d 6f73 7175 6974 746f  :..    mosquitto
-0001ddf0: 5f70 7562 202d 7420 7465 7374 2f74 6f70  _pub -t test/top
-0001de00: 6963 2d74 6172 6765 7473 2d64 796e 616d  ic-targets-dynam
-0001de10: 6963 202d 6d20 277b 226c 6f67 6c65 7665  ic -m '{"logleve
-0001de20: 6c22 3a20 2263 7269 7422 2c20 226d 6573  l": "crit", "mes
-0001de30: 7361 6765 223a 2022 4e75 7220 44c3 b66e  sage": "Nur D..n
-0001de40: 6572 206d 6163 6874 2073 6368 c3b6 6e65  er macht sch..ne
-0001de50: 7221 227d 270a 0a54 6869 7320 7769 6c6c  r!"}'..This will
-0001de60: 2069 7373 7565 2074 6865 2066 6f6c 6c6f   issue the follo
-0001de70: 7769 6e67 206d 6573 7361 6765 2069 6e74  wing message int
-0001de80: 6f20 7468 6520 6c6f 6720 6669 6c65 3a0a  o the log file:.
-0001de90: 0a20 2020 2032 3031 362d 3032 2d31 3420  .    2016-02-14 
-0001dea0: 3138 3a30 393a 3334 2c38 3232 2043 5249  18:09:34,822 CRI
-0001deb0: 5449 4341 4c20 5b6c 6f67 5d20 536f 6d65  TICAL [log] Some
-0001dec0: 7468 696e 6720 6372 6974 2068 6170 7065  thing crit happe
-0001ded0: 6e65 6421 204e 7572 2044 c3b6 6e65 7220  ned! Nur D..ner 
-0001dee0: 6d61 6368 7420 7363 68c3 b66e 6572 210a  macht sch..ner!.
-0001def0: 0a57 6869 6c65 2074 6869 7320 6c69 7474  .While this litt
-0001df00: 6c65 2065 7861 6d70 6c65 206d 6967 6874  le example might
-0001df10: 2066 6565 6c20 6172 7469 6669 6369 616c   feel artificial
-0001df20: 2c20 7468 6572 6520 6172 6520 6d6f 7265  , there are more
-0001df30: 206d 6561 6e69 6e67 6675 6c0a 7573 6520   meaningful.use 
-0001df40: 6361 7365 7320 6c69 6b65 2064 6574 6572  cases like deter
-0001df50: 6d69 6e69 6e67 2074 6865 2072 6563 6970  mining the recip
-0001df60: 6965 6e74 2061 6464 7265 7373 206f 6620  ient address of 
-0001df70: 6073 6d74 7060 206f 7220 6078 6d70 7060  `smtp` or `xmpp`
-0001df80: 2072 6563 6569 7665 7273 0a74 6872 6f75   receivers.throu
-0001df90: 6768 2069 6e66 6f72 6d61 7469 6f6e 2066  gh information f
-0001dfa0: 726f 6d20 746f 7069 6320 6e61 6d65 7320  rom topic names 
-0001dfb0: 6f72 206d 6573 7361 6765 2070 6179 6c6f  or message paylo
-0001dfc0: 6164 732e 0a50 6c65 6173 6520 6861 7665  ads..Please have
-0001dfd0: 2061 206c 6f6f 6b20 6174 205b 496e 636f   a look at [Inco
-0001dfe0: 7270 6f72 6174 6520 746f 7069 6320 6e61  rporate topic na
-0001dff0: 6d65 7320 696e 746f 2074 6f70 6963 2074  mes into topic t
-0001e000: 6172 6765 7473 5d28 6874 7470 733a 2f2f  argets](https://
-0001e010: 6769 7468 7562 2e63 6f6d 2f6a 706d 656e  github.com/jpmen
-0001e020: 732f 6d71 7474 7761 726e 2f77 696b 692f  s/mqttwarn/wiki/
-0001e030: 496e 636f 7270 6f72 6174 696e 672d 746f  Incorporating-to
-0001e040: 7069 632d 6e61 6d65 7323 696e 636f 7270  pic-names#incorp
-0001e050: 6f72 6174 652d 746f 7069 632d 6e61 6d65  orate-topic-name
-0001e060: 732d 696e 746f 2d74 6f70 6963 2d74 6172  s-into-topic-tar
-0001e070: 6765 7473 290a 666f 7220 6120 6d6f 7265  gets).for a more
-0001e080: 2073 656e 7369 626c 6520 6578 616d 706c   sensible exampl
-0001e090: 652e 0a0a 0a23 2323 2323 2046 696c 7465  e....##### Filte
-0001e0a0: 7269 6e67 206e 6f74 6966 6963 6174 696f  ring notificatio
-0001e0b0: 6e73 0a0a 4120 6e6f 7469 6669 6361 7469  ns..A notificati
-0001e0c0: 6f6e 2063 616e 2062 6520 6669 6c74 6572  on can be filter
-0001e0d0: 6564 2028 6f72 2073 7570 7072 6573 7365  ed (or suppresse
-0001e0e0: 642c 206f 7220 6967 6e6f 7265 6429 2075  d, or ignored) u
-0001e0f0: 7369 6e67 2061 2063 7573 746f 6d20 6675  sing a custom fu
-0001e100: 6e63 7469 6f6e 2e0a 0a41 6e20 6f70 7469  nction...An opti
-0001e110: 6f6e 616c 2060 6669 6c74 6572 6020 7365  onal `filter` se
-0001e120: 7474 696e 6720 696e 2061 2073 6563 7469  tting in a secti
-0001e130: 6f6e 2062 6c6f 636b 2064 6566 696e 6573  on block defines
-0001e140: 2074 6865 206e 616d 6520 6f66 2061 2050   the name of a P
-0001e150: 7974 686f 6e20 6675 6e63 7469 6f6e 2070  ython function p
-0001e160: 726f 7669 6465 6420 696e 2066 696c 6520  rovided in file 
-0001e170: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
-0001e180: 2060 6675 6e63 7469 6f6e 7360 2064 6972   `functions` dir
-0001e190: 6563 7469 7665 2e0a 0a60 6060 696e 690a  ective...```ini.
-0001e1a0: 5b6f 776e 7472 6163 6b73 2f23 2f70 686f  [owntracks/#/pho
-0001e1b0: 6e65 5d0a 6669 6c74 6572 203d 206f 776e  ne].filter = own
-0001e1c0: 7472 6163 6b73 5f66 696c 7465 7228 290a  tracks_filter().
-0001e1d0: 6060 600a 0a54 6869 7320 6578 616d 706c  ```..This exampl
-0001e1e0: 6520 7370 6563 6966 6965 7320 7468 6174  e specifies that
-0001e1f0: 2077 6865 6e20 6120 6d65 7373 6167 6520   when a message 
-0001e200: 666f 7220 7468 6520 6465 6669 6e65 6420  for the defined 
-0001e210: 746f 7069 6320 606f 776e 7472 6163 6b73  topic `owntracks
-0001e220: 2f6a 616e 652f 7068 6f6e 6560 2069 7320  /jane/phone` is 
-0001e230: 7265 6365 6976 6564 2c20 7468 6520 6675  received, the fu
-0001e240: 6e63 7469 6f6e 2060 6f77 6e74 7261 636b  nction `owntrack
-0001e250: 735f 6669 6c74 6572 2829 6020 7368 6f75  s_filter()` shou
-0001e260: 6c64 2062 6520 696e 766f 6b65 6420 746f  ld be invoked to
-0001e270: 2064 6574 6572 6d69 6e65 2077 6865 7468   determine wheth
-0001e280: 6572 0a6f 7220 6e6f 7420 746f 2070 726f  er.or not to pro
-0001e290: 6365 7373 2074 6865 206d 6573 7361 6765  cess the message
-0001e2a0: 2e0a 0a54 6865 2066 696c 7465 7220 6675  ...The filter fu
-0001e2b0: 6e63 7469 6f6e 2073 686f 756c 6420 7265  nction should re
-0001e2c0: 7475 726e 2060 5472 7565 6020 6966 2074  turn `True` if t
-0001e2d0: 6865 206d 6573 7361 6765 2073 686f 756c  he message shoul
-0001e2e0: 6420 6265 2073 7570 7072 6573 7365 642c  d be suppressed,
-0001e2f0: 206f 7220 6046 616c 7365 6020 6966 2074   or `False` if t
-0001e300: 6865 206d 6573 7361 6765 2073 686f 756c  he message shoul
-0001e310: 6420 6265 2070 726f 6365 7373 6564 2e0a  d be processed..
-0001e320: 4974 2073 686f 756c 6420 6861 7665 2074  It should have t
-0001e330: 6865 2066 6f6c 6c6f 7769 6e67 2073 6967  he following sig
-0001e340: 6e61 7475 7265 3a0a 0a60 6060 7079 7468  nature:..```pyth
-0001e350: 6f6e 0a64 6566 206f 776e 7472 6163 6b73  on.def owntracks
-0001e360: 5f66 696c 7465 7228 746f 7069 632c 206d  _filter(topic, m
-0001e370: 6573 7361 6765 2c20 7365 6374 696f 6e2c  essage, section,
-0001e380: 2073 7276 293a 0a20 2020 2072 6574 7572   srv):.    retur
-0001e390: 6e20 6d65 7373 6167 652e 6669 6e64 2827  n message.find('
-0001e3a0: 6576 656e 7427 2920 3d3d 202d 310a 6060  event') == -1.``
-0001e3b0: 600a 0a54 6865 2066 6f6c 6c6f 7769 6e67  `..The following
-0001e3c0: 2c20 7769 7468 2066 6577 6572 2061 7267  , with fewer arg
-0001e3d0: 756d 656e 7473 2c20 6973 2061 6c73 6f20  uments, is also 
-0001e3e0: 6163 6365 7074 6162 6c65 2c20 6275 7420  acceptable, but 
-0001e3f0: 7468 6520 6162 6f76 6520 6973 2070 7265  the above is pre
-0001e400: 6665 7272 6564 2e0a 6060 6070 7974 686f  ferred..```pytho
-0001e410: 6e0a 6465 6620 6f77 6e74 7261 636b 735f  n.def owntracks_
-0001e420: 6669 6c74 6572 2874 6f70 6963 2c20 6d65  filter(topic, me
-0001e430: 7373 6167 6529 3a0a 2020 2020 7265 7475  ssage):.    retu
-0001e440: 726e 206d 6573 7361 6765 2e66 696e 6428  rn message.find(
-0001e450: 2765 7665 6e74 2729 203d 3d20 2d31 0a60  'event') == -1.`
-0001e460: 6060 0a0a 5468 6573 6520 6675 6e63 7469  ``..These functi
-0001e470: 6f6e 7320 7769 6c6c 2072 6574 7572 6e20  ons will return 
-0001e480: 6054 7275 6560 2066 6f72 206d 6573 7361  `True` for messa
-0001e490: 6765 7320 7468 6174 2064 6f20 6e6f 7420  ges that do not 
-0001e4a0: 636f 6e74 6169 6e20 7468 6520 6065 7665  contain the `eve
-0001e4b0: 6e74 6020 746f 6b65 6e2c 2061 6e64 2074  nt` token, and t
-0001e4c0: 6875 7320 7375 7070 7265 7373 2074 686f  hus suppress tho
-0001e4d0: 7365 206d 6573 7361 6765 732e 0a0a 4e6f  se messages...No
-0001e4e0: 7465 2074 6861 7420 7468 6520 6074 6f70  te that the `top
-0001e4f0: 6963 6020 7061 7261 6d65 7465 7220 7769  ic` parameter wi
-0001e500: 6c6c 2062 6520 7468 6520 6e61 6d65 206f  ll be the name o
-0001e510: 6620 7468 6520 7370 6563 6966 6963 2074  f the specific t
-0001e520: 6f70 6963 2028 652e 672e 2060 6f77 6e74  opic (e.g. `ownt
-0001e530: 7261 636b 732f 6a61 6e65 2f70 686f 6e65  racks/jane/phone
-0001e540: 6029 2074 6861 7420 7468 6520 6d65 7373  `) that the mess
-0001e550: 6167 650a 7761 7320 7265 6365 6976 6564  age.was received
-0001e560: 206f 6e2e 2020 5468 6520 6e61 6d65 206f   on.  The name o
-0001e570: 6620 7468 6520 7365 6374 696f 6e20 2865  f the section (e
-0001e580: 2e67 2e20 606f 776e 7472 6163 6b73 2f23  .g. `owntracks/#
-0001e590: 2f70 686f 6e65 6029 2077 696c 6c20 6265  /phone`) will be
-0001e5a0: 2074 6865 2060 7365 6374 696f 6e60 2061   the `section` a
-0001e5b0: 7267 756d 656e 742e 0a0a 0a23 2323 2054  rgument....### T
-0001e5c0: 656d 706c 6174 6573 2023 2323 0a0a 496e  emplates ###..In
-0001e5d0: 7374 6561 6420 6f66 2066 6f72 6d61 7474  stead of formatt
-0001e5e0: 696e 6720 6f75 7470 7574 2077 6974 6820  ing output with 
-0001e5f0: 7468 6520 6066 6f72 6d61 7460 2073 7065  the `format` spe
-0001e600: 6369 6669 6361 7469 6f6e 2061 7320 6465  cification as de
-0001e610: 7363 7269 6265 6420 6162 6f76 652c 0a5f  scribed above,._
-0001e620: 6d71 7474 7761 726e 5f20 6861 7320 7072  mqttwarn_ has pr
-0001e630: 6f76 6973 696f 6e20 666f 7220 7265 6e64  ovision for rend
-0001e640: 6572 696e 6720 7468 6520 6f75 7470 7574  ering the output
-0001e650: 206d 6573 7361 6765 2066 726f 6d20 5b4a   message from [J
-0001e660: 696e 6a61 325d 2074 656d 706c 6174 6573  inja2] templates
-0001e670: 2c0a 7072 6f62 6162 6c79 2070 6172 7469  ,.probably parti
-0001e680: 6375 6c61 726c 7920 696e 7465 7265 7374  cularly interest
-0001e690: 696e 6720 666f 7220 7468 6520 6073 6d74  ing for the `smt
-0001e6a0: 7060 206f 7220 606e 6e74 7060 2061 6e64  p` or `nntp` and
-0001e6b0: 2060 6669 6c65 6020 7461 7267 6574 732e   `file` targets.
-0001e6c0: 0a0a 436f 6e73 6964 6572 2074 6865 2066  ..Consider the f
-0001e6d0: 6f6c 6c6f 7769 6e67 2065 7861 6d70 6c65  ollowing example
-0001e6e0: 2074 6f70 6963 2063 6f6e 6669 6775 7261   topic configura
-0001e6f0: 7469 6f6e 2c20 7768 6572 6520 7765 2069  tion, where we i
-0001e700: 6c6c 7573 7472 6174 6520 7573 696e 670a  llustrate using.
-0001e710: 6120 7465 6d70 6c61 7465 2069 6e73 7465  a template inste
-0001e720: 6164 206f 6620 6066 6f72 6d61 7460 2028  ad of `format` (
-0001e730: 7768 6963 6820 6973 2063 6f6d 6d65 6e74  which is comment
-0001e740: 6564 206f 7574 292e 0a0a 6060 6069 6e69  ed out)...```ini
-0001e750: 0a5b 6e6e 2f2b 5d0a 7461 7267 6574 7320  .[nn/+].targets 
-0001e760: 3d20 6e6e 7470 3a6a 7061 610a 3b20 666f  = nntp:jpaa.; fo
-0001e770: 726d 6174 203d 207b 6e61 6d65 7d3a 207b  rmat = {name}: {
-0001e780: 6e75 6d62 6572 7d20 3d3e 207b 5f64 7468  number} => {_dth
-0001e790: 686d 6d7d 0a74 656d 706c 6174 6520 3d20  hmm}.template = 
-0001e7a0: 6465 6d6f 2e6a 320a 6060 600a 0a5f 6d71  demo.j2.```.._mq
-0001e7b0: 7474 7761 726e 5f20 6c6f 6164 7320 4a69  ttwarn_ loads Ji
-0001e7c0: 6e6a 6132 2074 656d 706c 6174 6573 2066  nja2 templates f
-0001e7d0: 726f 6d20 7468 6520 6074 656d 706c 6174  rom the `templat
-0001e7e0: 6573 2f60 2064 6972 6563 746f 7279 2072  es/` directory r
-0001e7f0: 656c 6174 6976 6520 746f 2074 6865 0a63  elative to the.c
-0001e800: 6f6e 6669 6775 7265 6420 6064 6972 6563  onfigured `direc
-0001e810: 746f 7279 602e 2041 7373 756d 696e 6720  tory`. Assuming 
-0001e820: 7765 2068 6176 6520 7468 6520 666f 6c6c  we have the foll
-0001e830: 6f77 696e 6720 636f 6e74 656e 7420 696e  owing content in
-0001e840: 2074 6865 2066 696c 650a 6074 656d 706c   the file.`templ
-0001e850: 6174 6573 2f64 656d 6f2e 6a32 600a 0a60  ates/demo.j2`..`
-0001e860: 6060 6a69 6e6a 6132 0a7b 230a 2020 2020  ``jinja2.{#.    
-0001e870: 7468 6973 2069 7320 6120 636f 6d6d 656e  this is a commen
-0001e880: 740a 2020 2020 696e 204a 696e 6a61 320a  t.    in Jinja2.
-0001e890: 2020 2020 5365 6520 6874 7470 3a2f 2f6a      See http://j
-0001e8a0: 696e 6a61 2e70 6f63 6f6f 2e6f 7267 2f64  inja.pocoo.org/d
-0001e8b0: 6f63 732f 7465 6d70 6c61 7465 732f 2066  ocs/templates/ f
-0001e8c0: 6f72 2069 6e66 6f72 6d61 7469 6f6e 0a20  or information. 
-0001e8d0: 2020 206f 6e20 4a69 6e6a 6132 2074 656d     on Jinja2 tem
-0001e8e0: 706c 6174 6573 2e0a 237d 0a7b 2520 7365  plates..#}.{% se
-0001e8f0: 7420 7570 6e61 6d65 203d 206e 616d 6520  t upname = name 
-0001e900: 7c20 7570 7065 7220 257d 0a7b 2520 7365  | upper %}.{% se
-0001e910: 7420 7769 6474 6820 3d20 3630 2025 7d0a  t width = 60 %}.
-0001e920: 7b25 2066 6f72 206e 2069 6e20 7261 6e67  {% for n in rang
-0001e930: 6528 302c 2077 6964 7468 2920 257d 2d7b  e(0, width) %}-{
-0001e940: 2520 656e 6466 6f72 2025 7d0a 0a4e 616d  % endfor %}..Nam
-0001e950: 652e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  e...............
-0001e960: 2e2e 3a20 7b7b 2075 706e 616d 6520 7d7d  ..: {{ upname }}
-0001e970: 0a4e 756d 6265 722e 2e2e 2e2e 2e2e 2e2e  .Number.........
-0001e980: 2e2e 2e2e 2e2e 3a20 7b7b 206e 756d 6265  ......: {{ numbe
-0001e990: 7220 7d7d 0a54 696d 6573 7461 6d70 2e2e  r }}.Timestamp..
-0001e9a0: 2e2e 2e2e 2e2e 2e2e 2e2e 3a20 7b7b 205f  ..........: {{ _
-0001e9b0: 6474 6868 6d6d 207d 7d0a 4f72 6967 696e  dthhmm }}.Origin
-0001e9c0: 616c 2070 6179 6c6f 6164 2e2e 2e2e 2e3a  al payload.....:
-0001e9d0: 207b 7b20 7061 796c 6f61 6420 7d7d 0a60   {{ payload }}.`
-0001e9e0: 6060 0a0a 636f 756c 6420 7072 6f64 7563  ``..could produc
-0001e9f0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-0001ea00: 6d65 7373 6167 652c 206f 6e20 616e 7920  message, on any 
-0001ea10: 7461 7267 6574 2077 6869 6368 2075 7365  target which use
-0001ea20: 7320 7468 6973 2063 6f6e 6669 6775 7261  s this configura
-0001ea30: 7469 6f6e 2e0a 0a60 6060 0a2d 2d2d 2d2d  tion...```.-----
-0001ea40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ea50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ea60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ea70: 2d2d 2d2d 2d2d 2d0a 4e61 6d65 2e2e 2e2e  -------.Name....
-0001ea80: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e3a 204a  .............: J
-0001ea90: 414e 4520 4a4f 4c49 450a 4e75 6d62 6572  ANE JOLIE.Number
-0001eaa0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e3a  ...............:
-0001eab0: 2034 370a 5469 6d65 7374 616d 702e 2e2e   47.Timestamp...
-0001eac0: 2e2e 2e2e 2e2e 2e2e 2e3a 2031 393a 3135  .........: 19:15
-0001ead0: 0a4f 7269 6769 6e61 6c20 7061 796c 6f61  .Original payloa
-0001eae0: 642e 2e2e 2e2e 3a20 7b22 6e61 6d65 223a  d.....: {"name":
-0001eaf0: 224a 616e 6520 4a6f 6c69 6522 2c22 6e75  "Jane Jolie","nu
-0001eb00: 6d62 6572 223a 3437 2c20 2269 6422 3a39  mber":47, "id":9
-0001eb10: 317d 0a60 6060 0a0a 4f6e 6520 6f66 2074  1}.```..One of t
-0001eb20: 6865 2074 656d 706c 6174 6520 7661 7269  he template vari
-0001eb30: 6162 6c65 7320 796f 7520 6d61 7920 6265  ables you may be
-0001eb40: 2069 6e74 6572 6573 7465 6420 696e 2069   interested in i
-0001eb50: 7320 6361 6c6c 6564 2060 7b7b 2070 6179  s called `{{ pay
-0001eb60: 6c6f 6164 207d 7d60 3b20 7468 6973 0a63  load }}`; this.c
-0001eb70: 6172 7269 6573 2074 6865 206f 7269 6769  arries the origi
-0001eb80: 6e61 6c20 4d51 5454 206d 6573 7361 6765  nal MQTT message
-0001eb90: 2069 6e20 6974 2e20 416c 736f 2c20 6966   in it. Also, if
-0001eba0: 2074 6865 2070 6179 6c6f 6164 2077 6173   the payload was
-0001ebb0: 204a 534f 4e2c 2074 686f 7365 2061 7265   JSON, those are
-0001ebc0: 0a61 7661 696c 6162 6c65 2061 6c73 6f20  .available also 
-0001ebd0: 2861 7320 7368 6f77 6e20 696e 2074 6865  (as shown in the
-0001ebe0: 2061 626f 7665 2065 7861 6d70 6c65 292c   above example),
-0001ebf0: 2074 6f67 6574 6865 7220 7769 7468 2061   together with a
-0001ec00: 6c6c 2074 6865 206f 7468 6572 0a74 7261  ll the other.tra
-0001ec10: 6e73 666f 726d 6174 696f 6e20 6461 7461  nsformation data
-0001ec20: 2e0a 0a49 6620 7468 6520 7465 6d70 6c61  ...If the templa
-0001ec30: 7465 2063 616e 6e6f 7420 6265 2072 656e  te cannot be ren
-0001ec40: 6465 7265 642c 2073 6179 2c20 6974 2063  dered, say, it c
-0001ec50: 6f6e 7461 696e 7320 6120 4a69 6e6a 6132  ontains a Jinja2
-0001ec60: 2065 7272 6f72 206f 7220 7468 6520 7465   error or the te
-0001ec70: 6d70 6c61 7465 0a66 696c 6520 6361 6e6e  mplate.file cann
-0001ec80: 6f74 2062 6520 666f 756e 642c 2065 7463  ot be found, etc
-0001ec90: 2e2c 2074 6865 206f 7269 6769 6e61 6c20  ., the original 
-0001eca0: 7261 7720 6d65 7373 6167 6520 6973 2075  raw message is u
-0001ecb0: 7365 6420 696e 206c 6965 7520 6f6e 206f  sed in lieu on o
-0001ecc0: 7574 7075 742e 0a0a 4173 206d 656e 7469  utput...As menti
-0001ecd0: 6f6e 6564 2061 6c72 6561 6479 2c20 7765  oned already, we
-0001ece0: 2074 6869 6e6b 2074 6869 7320 6973 2075   think this is u
-0001ecf0: 7365 6675 6c20 666f 7220 7461 7267 6574  seful for target
-0001ed00: 7320 7768 6963 6820 6578 7065 6374 2061  s which expect a
-0001ed10: 2063 6572 7461 696e 0a61 6d6f 756e 7420   certain.amount 
-0001ed20: 6f66 2074 6578 7420 2860 6669 6c65 602c  of text (`file`,
-0001ed30: 2060 736d 7470 602c 2061 6e64 2060 6e6e   `smtp`, and `nn
-0001ed40: 7470 6020 636f 6d65 2074 6f20 6d69 6e64  tp` come to mind
-0001ed50: 292e 0a0a 5573 6520 6f66 2074 6869 7320  )...Use of this 
-0001ed60: 6665 6174 7572 6520 7265 7175 6972 6573  feature requires
-0001ed70: 205b 4a69 6e6a 6132 5d2c 2062 7574 2079   [Jinja2], but y
-0001ed80: 6f75 2064 6f6e 2774 2068 6176 6520 746f  ou don't have to
-0001ed90: 2069 6e73 7461 6c6c 2069 7420 6966 2079   install it if y
-0001eda0: 6f75 2064 6f6e 2774 206e 6565 640a 7465  ou don't need.te
-0001edb0: 6d70 6c61 7469 6e67 2e0a 0a23 2320 5065  mplating...## Pe
-0001edc0: 7269 6f64 6963 2074 6173 6b73 0a0a 5f6d  riodic tasks.._m
-0001edd0: 7174 7477 6172 6e5f 2063 616e 2075 7365  qttwarn_ can use
-0001ede0: 2066 756e 6374 696f 6e73 2079 6f75 2064   functions you d
-0001edf0: 6566 696e 6520 696e 2074 6865 2066 696c  efine in the fil
-0001ee00: 6520 7370 6563 6966 6965 6420 605b 6465  e specified `[de
-0001ee10: 6661 756c 7473 5d60 2073 6563 7469 6f6e  faults]` section
-0001ee20: 0a74 6f20 7065 7269 6f64 6963 616c 6c79  .to periodically
-0001ee30: 2064 6f20 7768 6174 6576 6572 2079 6f75   do whatever you
-0001ee40: 2077 616e 742c 2066 6f72 2065 7861 6d70   want, for examp
-0001ee50: 6c65 2c20 7075 626c 6973 6820 616e 204d  le, publish an M
-0001ee60: 5154 5420 6d65 7373 6167 652e 2054 6865  QTT message. The
-0001ee70: 7265 0a61 7265 2074 776f 2074 6869 6e67  re.are two thing
-0001ee80: 7320 796f 7520 6861 7665 2074 6f20 646f  s you have to do
-0001ee90: 3a0a 0a31 2e20 4372 6561 7465 2074 6865  :..1. Create the
-0001eea0: 2066 756e 6374 696f 6e0a 322e 2043 6f6e   function.2. Con
-0001eeb0: 6669 6775 7265 205f 6d71 7474 7761 726e  figure _mqttwarn
-0001eec0: 5f20 746f 2075 7365 2074 6861 7420 6675  _ to use that fu
-0001eed0: 6e63 7469 6f6e 2061 6e64 2073 7065 6369  nction and speci
-0001eee0: 6679 2074 6865 2069 6e74 6572 7661 6c20  fy the interval 
-0001eef0: 696e 2073 6563 6f6e 6473 0a0a 4173 7375  in seconds..Assu
-0001ef00: 6d65 2077 6520 6861 7665 2074 6865 2066  me we have the f
-0001ef10: 6f6c 6c6f 7769 6e67 2063 7573 746f 6d20  ollowing custom 
-0001ef20: 6675 6e63 7469 6f6e 2064 6566 696e 6564  function defined
-0001ef30: 3a0a 0a60 6060 7079 7468 6f6e 0a64 6566  :..```python.def
-0001ef40: 2070 696e 6765 7228 7372 763d 4e6f 6e65   pinger(srv=None
-0001ef50: 293a 0a20 2020 2073 7276 2e6d 7174 7463  ):.    srv.mqttc
-0001ef60: 2e70 7562 6c69 7368 2822 7074 2f50 494e  .publish("pt/PIN
-0001ef70: 4745 5222 2c20 2248 656c 6c6f 2066 726f  GER", "Hello fro
-0001ef80: 6d20 6d71 7474 7761 726e 2122 2c20 716f  m mqttwarn!", qo
-0001ef90: 733d 3029 0a60 6060 0a0a 5765 2063 6f6e  s=0).```..We con
-0001efa0: 6669 6775 7265 2074 6869 7320 6675 6e63  figure this func
-0001efb0: 7469 6f6e 2074 6f20 7275 6e20 6576 6572  tion to run ever
-0001efc0: 792c 2073 6179 2c20 3130 2073 6563 6f6e  y, say, 10 secon
-0001efd0: 6473 2c20 696e 2074 6865 2060 6d71 7474  ds, in the `mqtt
-0001efe0: 7761 726e 2e69 6e69 602c 0a69 6e20 7468  warn.ini`,.in th
-0001eff0: 6520 605b 6372 6f6e 5d60 2073 6563 7469  e `[cron]` secti
-0001f000: 6f6e 3a0a 0a60 6060 696e 690a 5b63 726f  on:..```ini.[cro
-0001f010: 6e5d 0a70 696e 6765 7220 3d20 3130 2e35  n].pinger = 10.5
-0001f020: 0a60 6060 0a0a 4561 6368 206b 6579 776f  .```..Each keywo
-0001f030: 7264 2069 6e20 7468 6520 605b 6372 6f6e  rd in the `[cron
-0001f040: 5d60 2073 6563 7469 6f6e 2073 7065 6369  ]` section speci
-0001f050: 6669 6573 2074 6865 206e 616d 6520 6f66  fies the name of
-0001f060: 206f 6e65 206f 6620 796f 7572 2063 7573   one of your cus
-0001f070: 746f 6d0a 6675 6e63 7469 6f6e 732c 2061  tom.functions, a
-0001f080: 6e64 2069 7473 2066 6c6f 6174 2076 616c  nd its float val
-0001f090: 7565 2069 7320 616e 2069 6e74 6572 7661  ue is an interva
-0001f0a0: 6c20 696e 205f 7365 636f 6e64 735f 2061  l in _seconds_ a
-0001f0b0: 6674 6572 2077 6869 6368 2079 6f75 720a  fter which your.
-0001f0c0: 6375 7374 6f6d 2066 756e 6374 696f 6e20  custom function 
-0001f0d0: 285f 7069 6e67 6572 2829 5f20 696e 2074  (_pinger()_ in t
-0001f0e0: 6869 7320 6361 7365 2920 6973 2069 6e76  his case) is inv
-0001f0f0: 6f6b 6564 2e20 596f 7572 2066 756e 6374  oked. Your funct
-0001f100: 696f 6e20 6861 7320 6163 6365 7373 0a74  ion has access.t
-0001f110: 6f20 7468 6520 6073 7276 6020 6f62 6a65  o the `srv` obje
-0001f120: 6374 2028 7768 6963 6820 7761 7320 6465  ct (which was de
-0001f130: 7363 7269 6265 6420 6561 726c 6965 7229  scribed earlier)
-0001f140: 2e0a 0a46 756e 6374 696f 6e20 6e61 6d65  ...Function name
-0001f150: 7320 6172 6520 746f 2062 6520 7370 6563  s are to be spec
-0001f160: 6966 6965 6420 696e 206c 6f77 6572 2d63  ified in lower-c
-0001f170: 6173 6520 6368 6172 6163 7465 7273 2e0a  ase characters..
-0001f180: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
-0001f190: 7275 6e20 7468 6520 6375 7374 6f6d 2066  run the custom f
-0001f1a0: 756e 6374 696f 6e20 696d 6d65 6469 6174  unction immediat
-0001f1b0: 656c 7920 6166 7465 7220 7374 6172 7469  ely after starti
-0001f1c0: 6e67 206d 7174 7477 6172 6e0a 696e 7374  ng mqttwarn.inst
-0001f1d0: 6561 6420 6f66 2077 6169 7469 6e67 2066  ead of waiting f
-0001f1e0: 6f72 2074 6865 2069 6e74 6572 7661 6c20  or the interval 
-0001f1f0: 746f 2065 6c61 7073 652c 2079 6f75 206d  to elapse, you m
-0001f200: 6967 6874 2077 616e 7420 746f 2063 6f6e  ight want to con
-0001f210: 6669 6775 7265 3a0a 0a60 6060 696e 690a  figure:..```ini.
-0001f220: 5b63 726f 6e5d 0a70 696e 6765 7220 3d20  [cron].pinger = 
-0001f230: 3130 2e35 3b20 6e6f 773d 7472 7565 0a60  10.5; now=true.`
-0001f240: 6060 0a0a 2323 2044 6f63 6b65 720a 0a49  ``..## Docker..I
-0001f250: 6e20 6f72 6465 7220 746f 2072 756e 2060  n order to run `
-0001f260: 6d71 7474 7761 726e 6020 6f6e 2044 6f63  mqttwarn` on Doc
-0001f270: 6b65 722c 2070 6c65 6173 6520 666f 6c6c  ker, please foll
-0001f280: 6f77 2075 7020 6174 205b 444f 434b 4552  ow up at [DOCKER
-0001f290: 2e6d 645d 2844 4f43 4b45 522e 6d64 292e  .md](DOCKER.md).
-0001f2a0: 0a0a 0a23 2320 4c6f 6164 696e 6720 6578  ...## Loading ex
-0001f2b0: 7465 726e 616c 2073 6572 7669 6365 730a  ternal services.
-0001f2c0: 0a49 6e20 6f72 6465 7220 746f 2062 7269  .In order to bri
-0001f2d0: 6e67 2069 6e20 6375 7374 6f6d 2065 6d69  ng in custom emi
-0001f2e0: 7474 6572 206d 6163 6869 6e65 7279 2074  tter machinery t
-0001f2f0: 6f20 606d 7174 7477 6172 6e60 2069 6e20  o `mqttwarn` in 
-0001f300: 666f 726d 206f 6620 7365 7276 6963 650a  form of service.
-0001f310: 706c 7567 696e 732c 2074 6865 7265 2061  plugins, there a
-0001f320: 7265 2074 776f 206f 7074 696f 6e73 2e0a  re two options..
-0001f330: 0a0a 2323 2320 5365 7276 6963 6520 706c  ..### Service pl
-0001f340: 7567 696e 2066 726f 6d20 7061 636b 6167  ugin from packag
-0001f350: 650a 0a54 6869 7320 636f 6e66 6967 7572  e..This configur
-0001f360: 6174 696f 6e20 736e 6970 7065 7420 6f75  ation snippet ou
-0001f370: 746c 696e 6573 2068 6f77 2074 6f20 6c6f  tlines how to lo
-0001f380: 6164 2061 2063 7573 746f 6d20 706c 7567  ad a custom plug
-0001f390: 696e 2066 726f 6d20 6120 5079 7468 6f6e  in from a Python
-0001f3a0: 0a6d 6f64 756c 6520 7265 6665 7265 6e63  .module referenc
-0001f3b0: 6564 2069 6e20 2264 6f74 7465 6422 206e  ed in "dotted" n
-0001f3c0: 6f74 6174 696f 6e2e 204d 6f64 756c 6573  otation. Modules
-0001f3d0: 2077 696c 6c20 6265 2073 6561 7263 6865   will be searche
-0001f3e0: 6420 666f 7220 696e 2061 6c6c 0a64 6972  d for in all.dir
-0001f3f0: 6563 746f 7269 6573 206c 6973 7465 6420  ectories listed 
-0001f400: 696e 205b 6073 7973 2e70 6174 6860 5d2e  in [`sys.path`].
-0001f410: 2043 7573 746f 6d20 6469 7265 6374 6f72   Custom director
-0001f420: 6965 7320 6361 6e20 6265 2061 6464 6564  ies can be added
-0001f430: 2062 7920 7573 696e 6720 7468 650a 5b60   by using the.[`
-0001f440: 5059 5448 4f4e 5041 5448 605d 2065 6e76  PYTHONPATH`] env
-0001f450: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-0001f460: 652e 0a0a 5b60 7379 732e 7061 7468 605d  e...[`sys.path`]
-0001f470: 3a20 6874 7470 733a 2f2f 646f 6373 2e70  : https://docs.p
-0001f480: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
-0001f490: 6172 792f 7379 732e 6874 6d6c 2373 7973  ary/sys.html#sys
-0001f4a0: 2e70 6174 680a 5b60 5059 5448 4f4e 5041  .path.[`PYTHONPA
-0001f4b0: 5448 605d 3a20 6874 7470 733a 2f2f 646f  TH`]: https://do
-0001f4c0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-0001f4d0: 7573 696e 672f 636d 646c 696e 652e 6874  using/cmdline.ht
-0001f4e0: 6d6c 2365 6e76 7661 722d 5059 5448 4f4e  ml#envvar-PYTHON
-0001f4f0: 5041 5448 0a0a 6060 6069 6e69 0a5b 6465  PATH..```ini.[de
-0001f500: 6661 756c 7473 5d0a 3b20 6e61 6d65 2074  faults].; name t
-0001f510: 6865 2073 6572 7669 6365 2070 726f 7669  he service provi
-0001f520: 6465 7273 2079 6f75 2077 696c 6c20 6265  ders you will be
-0001f530: 2075 7369 6e67 2e0a 6c61 756e 6368 2020   using..launch  
-0001f540: 2020 3d20 6c6f 672c 2066 696c 652c 2074    = log, file, t
-0001f550: 6573 7473 2e61 636d 652e 666f 6f62 6172  ests.acme.foobar
-0001f560: 0a0a 5b74 6573 742f 706c 7567 696e 2d6d  ..[test/plugin-m
-0001f570: 6f64 756c 655d 0a3b 2065 6368 6f20 277b  odule].; echo '{
-0001f580: 226e 616d 6522 3a20 2274 656d 7065 7261  "name": "tempera
-0001f590: 7475 7265 222c 2022 7661 6c75 6522 3a20  ture", "value": 
-0001f5a0: 3432 2e34 327d 2720 7c20 6d6f 7371 7569  42.42}' | mosqui
-0001f5b0: 7474 6f5f 7075 6220 2d68 206c 6f63 616c  tto_pub -h local
-0001f5c0: 686f 7374 202d 7420 7465 7374 2f70 6c75  host -t test/plu
-0001f5d0: 6769 6e2d 6d6f 6475 6c65 202d 6c0a 7461  gin-module -l.ta
-0001f5e0: 7267 6574 7320 3d20 7465 7374 732e 6163  rgets = tests.ac
-0001f5f0: 6d65 2e66 6f6f 6261 723a 6465 6661 756c  me.foobar:defaul
-0001f600: 740a 666f 726d 6174 203d 207b 6e61 6d65  t.format = {name
-0001f610: 7d3a 207b 7661 6c75 657d 0a0a 5b63 6f6e  }: {value}..[con
-0001f620: 6669 673a 7465 7374 732e 6163 6d65 2e66  fig:tests.acme.f
-0001f630: 6f6f 6261 725d 0a74 6172 6765 7473 203d  oobar].targets =
-0001f640: 207b 0a20 2020 2027 6465 6661 756c 7427   {.    'default'
-0001f650: 2020 3a20 5b20 2764 6566 6175 6c74 2720    : [ 'default' 
-0001f660: 5d2c 0a20 207d 0a60 6060 0a0a 2323 2320  ],.  }.```..### 
-0001f670: 5365 7276 6963 6520 706c 7567 696e 2066  Service plugin f
-0001f680: 726f 6d20 6669 6c65 0a0a 5468 6973 2063  rom file..This c
-0001f690: 6f6e 6669 6775 7261 7469 6f6e 2073 6e69  onfiguration sni
-0001f6a0: 7070 6574 206f 7574 6c69 6e65 7320 686f  ppet outlines ho
-0001f6b0: 7720 746f 206c 6f61 6420 6120 6375 7374  w to load a cust
-0001f6c0: 6f6d 2070 6c75 6769 6e20 6672 6f6d 2061  om plugin from a
-0001f6d0: 2050 7974 686f 6e0a 6669 6c65 2072 6566   Python.file ref
-0001f6e0: 6572 656e 6365 6420 6279 2066 696c 6520  erenced by file 
-0001f6f0: 6e61 6d65 2e20 5768 656e 2072 656c 6174  name. When relat
-0001f700: 6976 6520 6669 6c65 206e 616d 6573 2061  ive file names a
-0001f710: 7265 2067 6976 656e 2c20 7468 6579 2077  re given, they w
-0001f720: 696c 6c20 6265 0a72 6573 6f6c 7665 6420  ill be.resolved 
-0001f730: 6672 6f6d 2074 6865 2064 6972 6563 746f  from the directo
-0001f740: 7279 206f 6620 7468 6520 606d 7174 7477  ry of the `mqttw
-0001f750: 6172 6e2e 696e 6960 2066 696c 652c 2077  arn.ini` file, w
-0001f760: 6869 6368 2069 732c 2062 7920 6465 6661  hich is, by defa
-0001f770: 756c 742c 0a74 6865 2060 2f65 7463 2f6d  ult,.the `/etc/m
-0001f780: 7174 7477 6172 6e60 2066 6f6c 6465 722e  qttwarn` folder.
-0001f790: 0a0a 6060 6069 6e69 0a5b 6465 6661 756c  ..```ini.[defaul
-0001f7a0: 7473 5d0a 3b20 6e61 6d65 2074 6865 2073  ts].; name the s
-0001f7b0: 6572 7669 6365 2070 726f 7669 6465 7273  ervice providers
-0001f7c0: 2079 6f75 2077 696c 6c20 6265 2075 7369   you will be usi
-0001f7d0: 6e67 2e0a 6c61 756e 6368 2020 2020 3d20  ng..launch    = 
-0001f7e0: 6c6f 672c 2066 696c 652c 2074 6573 7473  log, file, tests
-0001f7f0: 2f61 636d 652f 666f 6f62 6172 2e70 790a  /acme/foobar.py.
-0001f800: 0a5b 7465 7374 2f70 6c75 6769 6e2d 6669  .[test/plugin-fi
-0001f810: 6c65 5d0a 3b20 6563 686f 2027 7b22 6e61  le].; echo '{"na
-0001f820: 6d65 223a 2022 7465 6d70 6572 6174 7572  me": "temperatur
-0001f830: 6522 2c20 2276 616c 7565 223a 2034 322e  e", "value": 42.
-0001f840: 3432 7d27 207c 206d 6f73 7175 6974 746f  42}' | mosquitto
-0001f850: 5f70 7562 202d 6820 6c6f 6361 6c68 6f73  _pub -h localhos
-0001f860: 7420 2d74 2074 6573 742f 706c 7567 696e  t -t test/plugin
-0001f870: 2d66 696c 6520 2d6c 0a74 6172 6765 7473  -file -l.targets
-0001f880: 203d 2074 6573 7473 2f61 636d 652f 666f   = tests/acme/fo
-0001f890: 6f62 6172 2e70 793a 6465 6661 756c 740a  obar.py:default.
-0001f8a0: 666f 726d 6174 203d 207b 6e61 6d65 7d3a  format = {name}:
-0001f8b0: 207b 7661 6c75 657d 0a0a 5b63 6f6e 6669   {value}..[confi
-0001f8c0: 673a 7465 7374 732f 6163 6d65 2f66 6f6f  g:tests/acme/foo
-0001f8d0: 6261 722e 7079 5d0a 7461 7267 6574 7320  bar.py].targets 
-0001f8e0: 3d20 7b0a 2020 2020 2764 6566 6175 6c74  = {.    'default
-0001f8f0: 2720 203a 205b 2027 6465 6661 756c 7427  '  : [ 'default'
-0001f900: 205d 2c0a 2020 7d0a 6060 600a 0a0a 2323   ],.  }.```...##
-0001f910: 2045 7861 6d70 6c65 7320 2323 0a0a 5468   Examples ##..Th
-0001f920: 6973 2073 6563 7469 6f6e 2063 6f6e 7461  is section conta
-0001f930: 696e 7320 736f 6d65 2065 7861 6d70 6c65  ins some example
-0001f940: 7320 6f66 2068 6f77 2060 6d71 7474 7761  s of how `mqttwa
-0001f950: 726e 6020 6361 6e20 6265 2075 7365 6420  rn` can be used 
-0001f960: 7769 7468 2073 6f6d 6520 6d6f 7265 2063  with some more c
-0001f970: 6f6d 706c 6578 2063 6f6e 6669 6775 7261  omplex configura
-0001f980: 7469 6f6e 732e 0a0a 2323 2320 4c6f 7720  tions...### Low 
-0001f990: 6261 7474 6572 7920 6e6f 7469 6669 6361  battery notifica
-0001f9a0: 7469 6f6e 7320 2323 230a 0a42 7920 7375  tions ###..By su
-0001f9b0: 6273 6372 6962 696e 6720 746f 2079 6f75  bscribing to you
-0001f9c0: 7220 5b4f 776e 5472 6163 6b73 5d20 746f  r [OwnTracks] to
-0001f9d0: 7069 6320 616e 6420 6164 6469 6e67 2074  pic and adding t
-0001f9e0: 6865 2066 6f6c 6c6f 7769 6e67 2063 7573  he following cus
-0001f9f0: 746f 6d20 6669 6c74 6572 2079 6f75 2063  tom filter you c
-0001fa00: 616e 2067 6574 2060 6d71 7474 7761 726e  an get `mqttwarn
-0001fa10: 6020 746f 2073 656e 6420 6e6f 7469 6669  ` to send notifi
-0001fa20: 6361 7469 6f6e 7320 7768 656e 2079 6f75  cations when you
-0001fa30: 7220 7068 6f6e 6520 6261 7474 6572 7920  r phone battery 
-0001fa40: 6765 7473 2062 656c 6f77 2061 2063 6572  gets below a cer
-0001fa50: 7461 696e 206c 6576 656c 3b0a 0a60 6060  tain level;..```
-0001fa60: 7079 7468 6f6e 0a69 6d70 6f72 7420 6a73  python.import js
-0001fa70: 6f6e 0a0a 6465 6620 6f77 6e74 7261 636b  on..def owntrack
-0001fa80: 735f 6261 7474 6669 6c74 6572 2874 6f70  s_battfilter(top
-0001fa90: 6963 2c20 6d65 7373 6167 6529 3a0a 2020  ic, message):.  
-0001faa0: 2020 6461 7461 203d 2064 6963 7428 6a73    data = dict(js
-0001fab0: 6f6e 2e6c 6f61 6473 286d 6573 7361 6765  on.loads(message
-0001fac0: 292e 6974 656d 7328 2929 0a20 2020 2069  ).items()).    i
-0001fad0: 6620 6461 7461 5b27 6261 7474 275d 2069  f data['batt'] i
-0001fae0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001faf0: 2020 2020 7265 7475 726e 2069 6e74 2864      return int(d
-0001fb00: 6174 615b 2762 6174 7427 5d29 203e 2032  ata['batt']) > 2
-0001fb10: 300a 2020 2020 7265 7475 726e 2054 7275  0.    return Tru
-0001fb20: 650a 6060 600a 0a4e 6f77 2073 696d 706c  e.```..Now simpl
-0001fb30: 7920 6164 6420 796f 7572 2063 686f 6963  y add your choic
-0001fb40: 6520 6f66 2074 6172 6765 7428 7329 2074  e of target(s) t
-0001fb50: 6f20 7468 6520 746f 7069 6327 7320 7365  o the topic's se
-0001fb60: 6374 696f 6e20 616e 6420 6120 6e69 6365  ction and a nice
-0001fb70: 2066 6f72 6d61 7420 7374 7269 6e67 2061   format string a
-0001fb80: 6e64 2079 6f75 2061 7265 2064 6f6e 653b  nd you are done;
-0001fb90: 0a0a 6060 6069 6e69 0a5b 6f77 6e74 7261  ..```ini.[owntra
-0001fba0: 636b 732f 235d 0a74 6172 6765 7473 203d  cks/#].targets =
-0001fbb0: 2070 7573 686f 7665 722c 2078 626d 630a   pushover, xbmc.
-0001fbc0: 6669 6c74 6572 203d 206f 776e 7472 6163  filter = owntrac
-0001fbd0: 6b73 5f62 6174 7466 696c 7465 7228 290a  ks_battfilter().
-0001fbe0: 666f 726d 6174 203d 204d 7920 7068 6f6e  format = My phon
-0001fbf0: 6520 6261 7474 6572 7920 6973 2067 6574  e battery is get
-0001fc00: 7469 6e67 206c 6f77 2028 7b62 6174 747d  ting low ({batt}
-0001fc10: 2529 210a 6060 600a 0a23 2323 2050 726f  %)!.```..### Pro
-0001fc20: 6475 6369 6e67 204a 534f 4e0a 0a41 7373  ducing JSON..Ass
-0001fc30: 756d 696e 6720 7765 2067 6574 2c20 6672  uming we get, fr
-0001fc40: 6f6d 2061 6e20 4172 6475 696e 6f2c 2073  om an Arduino, s
-0001fc50: 6179 2c20 6120 7369 6e67 6c65 206e 756d  ay, a single num
-0001fc60: 6572 6963 616c 2076 616c 7565 2069 6e20  erical value in 
-0001fc70: 7468 6520 7061 796c 6f61 6420 6f66 2061  the payload of a
-0001fc80: 6e20 4d51 5454 0a6d 6573 7361 6765 2c20  n MQTT.message, 
-0001fc90: 7765 2077 616e 7420 746f 2067 656e 6572  we want to gener
-0001fca0: 6174 6520 4a53 4f4e 2077 6974 6820 736f  ate JSON with so
-0001fcb0: 6d65 2061 6464 6974 696f 6e61 6c20 6669  me additional fi
-0001fcc0: 656c 6473 2e20 5573 696e 6720 6120 4a69  elds. Using a Ji
-0001fcd0: 6e6a 6132 2074 656d 706c 6174 650a 666f  nja2 template.fo
-0001fce0: 7220 7468 6520 7461 736b 2c20 646f 6573  r the task, does
-0001fcf0: 2065 7861 6374 6c79 2077 6861 7420 7765   exactly what we
-0001fd00: 206e 6565 643a 0a0a 5468 6520 666f 6c6c   need:..The foll
-0001fd10: 6f77 696e 6720 7461 7267 6574 2063 6f6e  owing target con
-0001fd20: 6669 6775 7261 7469 6f6e 2069 6e76 6f6b  figuration invok
-0001fd30: 6573 2074 6865 2074 656d 706c 6174 653a  es the template:
-0001fd40: 0a0a 6060 6069 6e69 0a5b 6172 6475 696e  ..```ini.[arduin
-0001fd50: 6f2f 7465 6d70 5d0a 7461 7267 6574 7320  o/temp].targets 
-0001fd60: 3d20 6c6f 673a 696e 666f 2c20 6874 7470  = log:info, http
-0001fd70: 3a67 7261 796c 6f67 320a 7465 6d70 6c61  :graylog2.templa
-0001fd80: 7465 203d 2074 656d 7032 6a73 6f6e 2e6a  te = temp2json.j
-0001fd90: 736f 6e0a 6060 600a 0a54 6865 204a 696e  son.```..The Jin
-0001fda0: 6a61 3220 7465 6d70 6c61 7465 206c 6f6f  ja2 template loo
-0001fdb0: 6b73 206c 696b 6520 7468 6973 3a0a 0a60  ks like this:..`
-0001fdc0: 6060 6a69 6e6a 6132 0a7b 230a 2020 2020  ``jinja2.{#.    
-0001fdd0: 5765 2065 7870 6563 7420 6120 7369 6e67  We expect a sing
-0001fde0: 6c65 206e 756d 6572 6963 2074 656d 7065  le numeric tempe
-0001fdf0: 7261 7475 7265 2076 616c 7565 2069 6e20  rature value in 
-0001fe00: 6070 6179 6c6f 6164 270a 2020 2020 5265  `payload'.    Re
-0001fe10: 7475 726e 204a 534f 4e20 7375 6974 6162  turn JSON suitab
-0001fe20: 6c65 2066 6f72 2047 7261 796c 6f67 3220  le for Graylog2 
-0001fe30: 2872 6571 7569 7265 7320 686f 7374 2061  (requires host a
-0001fe40: 6e64 2073 686f 7274 5f6d 6573 7361 6765  nd short_message
-0001fe50: 290a 0a20 2020 2044 6566 696e 6520 6120  )..    Define a 
-0001fe60: 6461 7461 2073 7472 7563 7475 7265 2069  data structure i
-0001fe70: 6e20 4a69 6e6a 6132 2061 6e64 2072 6574  n Jinja2 and ret
-0001fe80: 7572 6e20 6974 2061 7320 6120 4a53 4f4e  urn it as a JSON
-0001fe90: 2073 7472 696e 672e 0a20 2020 204e 6f74   string..    Not
-0001fea0: 6520 686f 7720 7472 616e 7366 6f72 6d61  e how transforma
-0001feb0: 7469 6f6e 2064 6174 6120 2870 726f 6475  tion data (produ
-0001fec0: 6365 6420 7769 7468 696e 206d 7174 7477  ced within mqttw
-0001fed0: 6172 6e29 2069 7320 7573 6564 3a0a 2020  arn) is used:.  
-0001fee0: 2020 7468 6520 7661 7269 6162 6c65 7320    the variables 
-0001fef0: 605f 6474 6973 6f27 2061 6e64 2060 7061  `_dtiso' and `pa
-0001ff00: 796c 6f61 6427 2063 6f6e 7461 696e 2061  yload' contain a
-0001ff10: 2074 696d 6573 7461 6d70 2061 6e64 206f   timestamp and o
-0001ff20: 7572 0a20 2020 2070 6179 6c6f 6164 2072  ur.    payload r
-0001ff30: 6573 7065 6374 6976 656c 792e 0a23 7d0a  espectively..#}.
-0001ff40: 7b25 2073 6574 2064 6174 6120 3d20 7b0a  {% set data = {.
-0001ff50: 0927 686f 7374 2709 093a 2074 6f70 6963  .'host'..: topic
-0001ff60: 2c0a 0927 7368 6f72 745f 6d65 7373 6167  ,..'short_messag
-0001ff70: 6527 093a 2022 4865 6174 2022 202b 2070  e'.: "Heat " + p
-0001ff80: 6179 6c6f 6164 2c0a 0927 7473 7427 0909  ayload,..'tst'..
-0001ff90: 3a20 5f64 7469 736f 2c0a 0927 7465 6d70  : _dtiso,..'temp
-0001ffa0: 6572 6174 7572 6527 093a 2070 6179 6c6f  erature'.: paylo
-0001ffb0: 6164 2c0a 0927 776f 6f68 6f6f 6f27 093a  ad,..'woohooo'.:
-0001ffc0: 2031 372c 0a09 7d0a 0925 7d0a 7b7b 2064   17,..}..%}.{{ d
-0001ffd0: 6174 6120 7c20 6a73 6f6e 6966 7920 7d7d  ata | jsonify }}
-0001ffe0: 0a60 6060 0a0a 616e 6420 616e 2065 7861  .```..and an exa
-0001fff0: 6d70 6c65 204a 534f 4e20 7374 7269 6e67  mple JSON string
-00020000: 2072 6574 7572 6e65 6420 6279 2074 6861   returned by tha
-00020010: 7420 7465 6d70 6c61 7465 2069 7320 7468  t template is th
-00020020: 656e 2070 6173 7365 6420 746f 206f 7572  en passed to our
-00020030: 2063 6f6e 6669 6775 7265 640a 7461 7267   configured.targ
-00020040: 6574 733a 0a0a 6060 606a 736f 6e0a 7b22  ets:..```json.{"
-00020050: 686f 7374 223a 2022 6172 6475 696e 6f2f  host": "arduino/
-00020060: 7465 6d70 222c 2022 776f 6f68 6f6f 6f22  temp", "woohooo"
-00020070: 3a20 3137 2c20 2274 7374 223a 2022 3230  : 17, "tst": "20
-00020080: 3134 2d30 342d 3133 5430 393a 3235 3a34  14-04-13T09:25:4
-00020090: 362e 3234 3731 3530 5a22 2c20 2274 656d  6.247150Z", "tem
-000200a0: 7065 7261 7475 7265 223a 2022 3232 222c  perature": "22",
-000200b0: 2022 7368 6f72 745f 6d65 7373 6167 6522   "short_message"
-000200c0: 3a20 2248 6561 7420 3232 227d 0a60 6060  : "Heat 22"}.```
-000200d0: 0a0a 0a23 2323 2041 6d61 7a6f 6e20 416c  ...### Amazon Al
-000200e0: 6578 610a 0a41 6e20 616c 7465 726e 6174  exa..An alternat
-000200f0: 6976 6520 746f 2061 6c65 7861 2d6e 6f74  ive to alexa-not
-00020100: 6966 792d 6d65 206e 6f74 6966 6963 6174  ify-me notificat
-00020110: 696f 6e20 2873 7065 616b 6572 2067 6c6f  ion (speaker glo
-00020120: 7773 2079 656c 6c6f 7720 616e 6420 6177  ws yellow and aw
-00020130: 6169 7473 2069 6e73 7472 7563 7469 6f6e  aits instruction
-00020140: 2074 6f20 706c 6179 2074 6865 206e 6f74   to play the not
-00020150: 6966 6963 6174 696f 6e29 2069 7320 746f  ification) is to
-00020160: 2066 6f72 2054 5453 2074 6f20 7370 6563   for TTS to spec
-00020170: 6966 6963 2064 6576 6963 6573 206f 7220  ific devices or 
-00020180: 616e 6e6f 756e 6365 2074 6f20 6120 7370  announce to a sp
-00020190: 6561 6b65 7220 6772 6f75 702e 0a0a 5365  eaker group...Se
-000201a0: 6520 7468 6520 6578 616d 706c 6573 2064  e the examples d
-000201b0: 6972 6563 746f 7279 2066 6f72 2069 6e74  irectory for int
-000201c0: 6567 7261 7469 6f6e 2077 6974 6820 7069  egration with pi
-000201d0: 7065 2061 6e64 2068 7474 7073 3a2f 2f67  pe and https://g
-000201e0: 6974 6875 622e 636f 6d2f 7468 6f72 7374  ithub.com/thorst
-000201f0: 656e 2d67 6568 7269 672f 616c 6578 612d  en-gehrig/alexa-
-00020200: 7265 6d6f 7465 2d63 6f6e 7472 6f6c 2073  remote-control s
-00020210: 6865 6c6c 2073 6372 6970 7473 2e0a 0a49  hell scripts...I
-00020220: 6e73 7472 7563 7469 6f6e 733a 0a0a 2a20  nstructions:..* 
-00020230: 446f 776e 6c6f 6164 2f63 6865 636b 6f75  Download/checkou
-00020240: 7420 6874 7470 733a 2f2f 6769 7468 7562  t https://github
-00020250: 2e63 6f6d 2f74 686f 7273 7465 6e2d 6765  .com/thorsten-ge
-00020260: 6872 6967 2f61 6c65 7861 2d72 656d 6f74  hrig/alexa-remot
-00020270: 652d 636f 6e74 726f 6c0a 2a20 4564 6974  e-control.* Edit
-00020280: 2073 6563 7265 7473 2e73 680a 2a20 456e   secrets.sh.* En
-00020290: 7375 7265 2070 6174 6873 2061 7265 2063  sure paths are c
-000202a0: 6f72 7265 6374 2028 7363 7269 7074 7320  orrect (scripts 
-000202b0: 616e 6420 696e 6920 6669 6c65 2061 7373  and ini file ass
-000202c0: 756d 6520 7061 7468 202f 686f 6d65 2f70  ume path /home/p
-000202d0: 692f 7368 656c 6c2f 616c 6578 612d 7265  i/shell/alexa-re
-000202e0: 6d6f 7465 2d63 6f6e 7472 6f6c 290a 2a20  mote-control).* 
-000202f0: 4564 6974 2069 6e69 2066 696c 6520 7461  Edit ini file ta
-00020300: 7267 6574 7320 7769 7468 2064 6576 6963  rgets with devic
-00020310: 6520 6e61 6d65 7320 616e 642f 6f72 2067  e names and/or g
-00020320: 726f 7570 206e 616d 6520 2873 6179 7374  roup name (sayst
-00020330: 6469 6e20 666f 7220 7369 6e67 6c65 2064  din for single d
-00020340: 6576 6963 6573 2c20 616e 6e6f 756e 6365  evices, announce
-00020350: 5f73 7464 696e 2066 6f72 2067 726f 7570  _stdin for group
-00020360: 7329 0a2a 2053 616e 6974 7920 6368 6563  s).* Sanity chec
-00020370: 6b2c 2063 686d 6f64 2061 2b78 206f 6e20  k, chmod a+x on 
-00020380: 616c 6c20 7368 656c 6c20 7363 7269 7074  all shell script
-00020390: 730a 0a0a 0a23 2320 4e6f 7465 730a 0a22  s....## Notes.."
-000203a0: 4d51 5454 2220 6973 2061 2074 7261 6465  MQTT" is a trade
-000203b0: 6d61 726b 206f 6620 7468 6520 4f41 5349  mark of the OASI
-000203c0: 5320 6f70 656e 2073 7461 6e64 6172 6473  S open standards
-000203d0: 2063 6f6e 736f 7274 6975 6d2c 2077 6869   consortium, whi
-000203e0: 6368 2070 7562 6c69 7368 6573 2074 6865  ch publishes the
-000203f0: 204d 5154 5420 7370 6563 6966 6963 6174   MQTT specificat
-00020400: 696f 6e73 2e0a 0a0a 0a23 2320 5072 6573  ions.....## Pres
-00020410: 730a 0a2a 205b 4d51 5454 7761 726e 3a20  s..* [MQTTwarn: 
-00020420: 4569 6e20 5275 6e64 756d 2d53 6f72 676c  Ein Rundum-Sorgl
-00020430: 6f73 2d4e 6f74 6966 6965 725d 2868 7474  os-Notifier](htt
-00020440: 703a 2f2f 6a61 7865 6e74 6572 2e64 652f  p://jaxenter.de/
-00020450: 6e65 7773 2f4d 5154 5477 6172 6e2d 4569  news/MQTTwarn-Ei
-00020460: 6e2d 5275 6e64 756d 2d53 6f72 676c 6f73  n-Rundum-Sorglos
-00020470: 2d4e 6f74 6966 6965 722d 3137 3133 3132  -Notifier-171312
-00020480: 292c 2061 7274 6963 6c65 2069 6e20 4765  ), article in Ge
-00020490: 726d 616e 2061 7420 4a41 5865 6e74 6572  rman at JAXenter
-000204a0: 2e0a 2a20 5b53 6368 7761 726d 616c 6172  ..* [Schwarmalar
-000204b0: 6d20 7573 696e 6720 6d71 7474 7761 726e  m using mqttwarn
-000204c0: 5d28 6874 7470 733a 2f2f 6869 7665 6579  ](https://hiveey
-000204d0: 6573 2e6f 7267 2f64 6f63 732f 7379 7374  es.org/docs/syst
-000204e0: 656d 2f73 6368 7761 726d 616c 6172 6d2d  em/schwarmalarm-
-000204f0: 6d71 7474 7761 726e 2e68 746d 6c29 0a0a  mqttwarn.html)..
-00020500: 2020 5b4f 776e 5472 6163 6b73 5d3a 2068    [OwnTracks]: h
-00020510: 7474 703a 2f2f 6f77 6e74 7261 636b 732e  ttp://owntracks.
-00020520: 6f72 670a 2020 5b4a 696e 6a61 325d 3a20  org.  [Jinja2]: 
-00020530: 6874 7470 3a2f 2f6a 696e 6a61 2e70 6f63  http://jinja.poc
-00020540: 6f6f 2e6f 7267 2f64 6f63 732f 7465 6d70  oo.org/docs/temp
-00020550: 6c61 7465 732f 0a20 205b 5a61 6262 6978  lates/.  [Zabbix
-00020560: 5d3a 2068 7474 703a 2f2f 7a61 6262 6978  ]: http://zabbix
-00020570: 2e63 6f6d 0a                             .com.
+00014a80: 6572 600a 0a5b 5075 7368 7361 6665 725d  er`..[Pushsafer]
+00014a90: 2868 7474 7073 3a2f 2f77 7777 2e70 7573  (https://www.pus
+00014aa0: 6873 6166 6572 2e63 6f6d 2920 6973 2061  hsafer.com) is a
+00014ab0: 6e20 6170 7020 666f 7220 694f 532c 2041  n app for iOS, A
+00014ac0: 6e64 726f 6964 2061 6e64 2057 696e 646f  ndroid and Windo
+00014ad0: 7773 2031 302e 0a59 6f75 2063 616e 2064  ws 10..You can d
+00014ae0: 6566 696e 6520 6469 6666 6572 656e 7420  efine different 
+00014af0: 6e6f 7469 6669 6361 7469 6f6e 2074 6172  notification tar
+00014b00: 6765 7473 2c20 696e 2074 7572 6e20 6469  gets, in turn di
+00014b10: 7370 6174 6368 696e 6720 746f 206f 6e65  spatching to one
+00014b20: 206f 7220 0a6d 756c 7469 706c 6520 5075   or .multiple Pu
+00014b30: 7368 7361 6665 7220 6465 7669 6365 7320  shsafer devices 
+00014b40: 6f72 2067 726f 7570 732e 0a46 6f72 2061  or groups..For a
+00014b50: 206c 6973 7420 6f66 2061 7661 696c 6162   list of availab
+00014b60: 6c65 2069 636f 6e73 2c20 736f 756e 6473  le icons, sounds
+00014b70: 2061 6e64 206f 7468 6572 2070 6172 616d   and other param
+00014b80: 6574 6572 732c 2073 6565 2074 6865 0a5b  eters, see the.[
+00014b90: 5075 7368 7361 6665 7220 4150 495d 2868  Pushsafer API](h
+00014ba0: 7474 7073 3a2f 2f77 7777 2e70 7573 6873  ttps://www.pushs
+00014bb0: 6166 6572 2e63 6f6d 2f65 6e2f 7075 7368  afer.com/en/push
+00014bc0: 6170 6929 2064 6f63 756d 656e 7461 7469  api) documentati
+00014bd0: 6f6e 2e0a 0a23 2323 2320 5265 7175 6972  on...#### Requir
+00014be0: 656d 656e 7473 0a49 6e20 6f72 6465 7220  ements.In order 
+00014bf0: 746f 2072 6563 6569 7665 2050 7573 6873  to receive Pushs
+00014c00: 6166 6572 206e 6f74 6966 6963 6174 696f  afer notificatio
+00014c10: 6e73 2c20 796f 7520 6e65 6564 2077 6861  ns, you need wha
+00014c20: 7420 6973 2063 616c 6c65 6420 6120 5f70  t is called a _p
+00014c30: 7269 7661 7465 200a 6f72 2061 6c69 6173  rivate .or alias
+00014c40: 206b 6579 5f2e 2054 6f20 7265 6365 6976   key_. To receiv
+00014c50: 6520 7375 6368 2061 206b 6579 2c20 796f  e such a key, yo
+00014c60: 7520 7769 6c6c 206e 6565 6420 746f 2073  u will need to s
+00014c70: 6967 6e20 7570 2066 6f72 2061 6e20 6163  ign up for an ac
+00014c80: 636f 756e 742e 0a0a 2323 2323 2043 6f6e  count...#### Con
+00014c90: 6669 6775 7261 7469 6f6e 2065 7861 6d70  figuration examp
+00014ca0: 6c65 0a0a 6060 6069 6e69 0a5b 636f 6e66  le..```ini.[conf
+00014cb0: 6967 3a70 7573 6873 6166 6572 5d0a 3b20  ig:pushsafer].; 
+00014cc0: 6874 7470 733a 2f2f 7777 772e 7075 7368  https://www.push
+00014cd0: 7361 6665 722e 636f 6d2f 656e 2f70 7573  safer.com/en/pus
+00014ce0: 6861 7069 0a3b 2068 7474 7073 3a2f 2f77  hapi.; https://w
+00014cf0: 7777 2e70 7573 6873 6166 6572 2e63 6f6d  ww.pushsafer.com
+00014d00: 2f65 6e2f 7075 7368 6170 695f 6578 740a  /en/pushapi_ext.
+00014d10: 7461 7267 6574 7320 3d20 7b0a 2020 2020  targets = {.    
+00014d20: 2762 6173 6963 273a 207b 2027 7072 6976  'basic': { 'priv
+00014d30: 6174 655f 6b65 7927 3a20 2733 5341 7a31  ate_key': '3SAz1
+00014d40: 6132 6954 5973 6831 3965 5849 4d69 4f27  a2iTYsh19eXIMiO'
+00014d50: 207d 2c0a 2020 2020 276e 6167 696f 7327   },.    'nagios'
+00014d60: 3a20 7b0a 2020 2020 2020 2020 2770 7269  : {.        'pri
+00014d70: 7661 7465 5f6b 6579 273a 2027 3353 417a  vate_key': '3SAz
+00014d80: 3161 3269 5459 7368 3139 6558 494d 694f  1a2iTYsh19eXIMiO
+00014d90: 272c 0a20 2020 2020 2020 2027 6465 7669  ',.        'devi
+00014da0: 6365 273a 2027 3532 7c36 357c 3738 272c  ce': '52|65|78',
+00014db0: 0a20 2020 2020 2020 2027 6963 6f6e 273a  .        'icon':
+00014dc0: 2036 342c 0a20 2020 2020 2020 2027 736f   64,.        'so
+00014dd0: 756e 6427 3a20 322c 0a20 2020 2020 2020  und': 2,.       
+00014de0: 2027 7669 6272 6174 696f 6e27 3a20 312c   'vibration': 1,
+00014df0: 0a20 2020 2020 2020 2027 7572 6c27 3a20  .        'url': 
+00014e00: 2768 7474 703a 2f2f 6578 616d 706c 652e  'http://example.
+00014e10: 6f72 6727 2c0a 2020 2020 2020 2020 2775  org',.        'u
+00014e20: 726c 5f74 6974 6c65 273a 2027 4578 616d  rl_title': 'Exam
+00014e30: 706c 6520 4f72 6727 2c0a 2020 2020 2020  ple Org',.      
+00014e40: 2020 2774 696d 655f 746f 5f6c 6976 6527    'time_to_live'
+00014e50: 3a20 3630 2c0a 2020 2020 2020 2020 2770  : 60,.        'p
+00014e60: 7269 6f72 6974 7927 3a20 322c 0a20 2020  riority': 2,.   
+00014e70: 2020 2020 2027 7265 7472 7927 3a20 3630       'retry': 60
+00014e80: 2c0a 2020 2020 2020 2020 2765 7870 6972  ,.        'expir
+00014e90: 6527 3a20 3630 302c 0a20 2020 2020 2020  e': 600,.       
+00014ea0: 2027 616e 7377 6572 273a 2031 2c0a 2020   'answer': 1,.  
+00014eb0: 2020 2020 2020 2761 6e73 7765 726f 7074        'answeropt
+00014ec0: 696f 6e73 273a 2027 7965 737c 6e6f 7c6d  ions': 'yes|no|m
+00014ed0: 6179 6265 272c 0a20 2020 2020 2020 2027  aybe',.        '
+00014ee0: 616e 7377 6572 666f 7263 6527 3a20 312c  answerforce': 1,
+00014ef0: 0a20 2020 2020 2020 2027 636f 6e66 6972  .        'confir
+00014f00: 6d27 3a20 3130 2c0a 2020 2020 2020 2020  m': 10,.        
+00014f10: 7d2c 0a20 2020 2027 7472 6163 6b69 6e67  },.    'tracking
+00014f20: 273a 207b 0a20 2020 2020 2020 2027 7072  ': {.        'pr
+00014f30: 6976 6174 655f 6b65 7927 3a20 2733 5341  ivate_key': '3SA
+00014f40: 7a31 6132 6954 5973 6831 3965 5849 4d69  z1a2iTYsh19eXIMi
+00014f50: 4f27 2c0a 2020 2020 2020 2020 2764 6576  O',.        'dev
+00014f60: 6963 6527 3a20 2767 7332 3327 2c0a 2020  ice': 'gs23',.  
+00014f70: 2020 2020 2020 2769 636f 6e27 3a20 3138        'icon': 18
+00014f80: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
+00014f90: 2027 6578 7472 6170 686f 6e65 273a 207b   'extraphone': {
+00014fa0: 2027 7072 6976 6174 655f 6b65 7927 3a20   'private_key': 
+00014fb0: 2761 6c69 6173 6b65 7932 272c 2027 7469  'aliaskey2', 'ti
+00014fc0: 6d65 5f74 6f5f 6c69 7665 273a 2036 302c  me_to_live': 60,
+00014fd0: 2027 7072 696f 7269 7479 273a 2032 2c20   'priority': 2, 
+00014fe0: 2772 6574 7279 273a 2036 302c 2027 6578  'retry': 60, 'ex
+00014ff0: 7069 7265 273a 2036 3030 2c20 2761 6e73  pire': 600, 'ans
+00015000: 7765 7227 3a20 3020 7d2c 0a20 2020 2027  wer': 0 },.    '
+00015010: 7761 726e 6d65 273a 207b 2027 7072 6976  warnme': { 'priv
+00015020: 6174 655f 6b65 7927 3a20 2761 6c69 6173  ate_key': 'alias
+00015030: 6b65 7933 272c 2027 7469 6d65 5f74 6f5f  key3', 'time_to_
+00015040: 6c69 7665 273a 2036 302c 2027 7072 696f  live': 60, 'prio
+00015050: 7269 7479 273a 2031 2c20 2761 6e73 7765  rity': 1, 'answe
+00015060: 7227 3a20 312c 2027 616e 7377 6572 666f  r': 1, 'answerfo
+00015070: 7263 6527 3a20 312c 2027 636f 6e66 6972  rce': 1, 'confir
+00015080: 6d27 3a20 3130 207d 2c0a 2020 2020 7d0a  m': 10 },.    }.
+00015090: 6060 600a 0a23 2323 2320 4d51 5454 2074  ```..#### MQTT t
+000150a0: 6f70 6963 206f 7074 696f 6e73 0a0a 7c20  opic options..| 
+000150b0: 546f 7069 6320 6f70 7469 6f6e 2020 7c20  Topic option  | 
+000150c0: 204d 2f4f 2020 207c 2044 6573 6372 6970   M/O   | Descrip
+000150d0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
+000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150f0: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
+00015100: 2d20 7c20 3a2d 2d2d 2d3a 207c 202d 2d2d  - | :----: | ---
+00015110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00015120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00015130: 2d2d 2d20 7c0a 7c20 6074 6974 6c65 6020  --- |.| `title` 
+00015140: 2020 2020 2020 7c20 2020 4f20 2020 207c        |   O    |
+00015150: 2061 7070 6c69 6361 7469 6f6e 2074 6974   application tit
+00015160: 6c65 2028 6466 6c74 3a20 7075 7368 7361  le (dflt: pushsa
+00015170: 6665 7220 6466 6c74 2920 7c0a 0a23 2323  fer dflt) |..###
+00015180: 2320 4e6f 7465 730a 2d20 5b52 6574 7279  # Notes.- [Retry
+00015190: 5d28 6874 7470 733a 2f2f 7777 772e 7075  ](https://www.pu
+000151a0: 7368 7361 6665 722e 636f 6d2f 656e 2f70  shsafer.com/en/p
+000151b0: 7573 6861 7069 5f65 7874 2341 5049 2d52  ushapi_ext#API-R
+000151c0: 4529 0a20 2077 6974 6820 5b45 7870 6972  E).  with [Expir
+000151d0: 655d 2868 7474 7073 3a2f 2f77 7777 2e70  e](https://www.p
+000151e0: 7573 6873 6166 6572 2e63 6f6d 2f65 6e2f  ushsafer.com/en/
+000151f0: 7075 7368 6170 695f 6578 7423 4150 492d  pushapi_ext#API-
+00015200: 4558 293a 0a20 2046 6f72 2063 6f6e 6669  EX):.  For confi
+00015210: 6775 7269 6e67 2064 656c 6976 6572 7920  guring delivery 
+00015220: 7265 7472 6965 732c 2079 6f75 206d 7573  retries, you mus
+00015230: 7420 7365 7420 626f 7468 2070 6172 616d  t set both param
+00015240: 6574 6572 732e 0a2d 2054 6865 206c 6567  eters..- The leg
+00015250: 6163 7920 636f 6e66 6967 7572 6174 696f  acy configuratio
+00015260: 6e20 6c61 796f 7574 2c20 6261 7365 6420  n layout, based 
+00015270: 6f6e 2061 206c 6973 7420 666f 7220 7468  on a list for th
+00015280: 6520 6061 6464 7273 6020 736c 6f74 2c0a  e `addrs` slot,.
+00015290: 2020 6973 2073 7469 6c6c 2073 7570 706f    is still suppo
+000152a0: 7274 6564 2e0a 0a23 2323 2320 5363 7265  rted...#### Scre
+000152b0: 656e 7368 6f74 0a21 5b70 7573 6873 6166  enshot.![pushsaf
+000152c0: 6572 206f 6e20 694f 535d 2861 7373 6574  er on iOS](asset
+000152d0: 732f 7075 7368 7361 6665 722e 6a70 6729  s/pushsafer.jpg)
+000152e0: 0a0a 0a23 2323 2060 7265 6469 7370 7562  ...### `redispub
+000152f0: 600a 0a54 6865 2060 7265 6469 7370 7562  `..The `redispub
+00015300: 6020 706c 7567 696e 2070 7562 6c69 7368  ` plugin publish
+00015310: 6573 2074 6f20 6120 5265 6469 7320 6368  es to a Redis ch
+00015320: 616e 6e65 6c2e 0a0a 6060 6069 6e69 0a5b  annel...```ini.[
+00015330: 636f 6e66 6967 3a72 6564 6973 7075 625d  config:redispub]
+00015340: 0a68 6f73 7420 203d 2020 276c 6f63 616c  .host  =  'local
+00015350: 686f 7374 270a 706f 7274 2020 3d20 2036  host'.port  =  6
+00015360: 3337 390a 7461 7267 6574 7320 3d20 7b0a  379.targets = {.
+00015370: 2020 2020 2772 3127 2020 2020 2020 3a20      'r1'      : 
+00015380: 5b20 2763 6861 6e6e 656c 2d31 2720 5d0a  [ 'channel-1' ].
+00015390: 2020 2020 7d0a 6060 600a 0a52 6571 7569      }.```..Requi
+000153a0: 7265 733a 0a2a 205b 7265 6469 732d 7079  res:.* [redis-py
+000153b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000153c0: 2e63 6f6d 2f61 6e64 796d 6363 7572 6479  .com/andymccurdy
+000153d0: 2f72 6564 6973 2d70 7929 0a0a 2323 2320  /redis-py)..### 
+000153e0: 6072 7264 746f 6f6c 600a 0a54 6865 2060  `rrdtool`..The `
+000153f0: 7272 6474 6f6f 6c60 2070 6c75 6769 6e20  rrdtool` plugin 
+00015400: 7570 6461 7465 7320 6120 726f 756e 642d  updates a round-
+00015410: 726f 6269 6e20 6461 7461 6261 7365 2063  robin database c
+00015420: 7265 6174 6564 2062 7920 5b72 7264 746f  reated by [rrdto
+00015430: 6f6c 5d20 7769 7468 0a74 6865 206d 6573  ol] with.the mes
+00015440: 7361 6765 2070 6179 6c6f 6164 2e0a 0a60  sage payload...`
+00015450: 6060 696e 690a 5b63 6f6e 6669 673a 7272  ``ini.[config:rr
+00015460: 6474 6f6f 6c5d 0a74 6172 6765 7473 203d  dtool].targets =
+00015470: 207b 0a20 2020 2027 6c69 7669 6e67 2d74   {.    'living-t
+00015480: 656d 7027 2020 3a20 5b27 2f74 6d70 2f6c  emp'  : ['/tmp/l
+00015490: 6976 696e 672d 7465 6d70 2e72 7264 272c  iving-temp.rrd',
+000154a0: 2020 272d 2d74 656d 706c 6174 6527 2c20    '--template', 
+000154b0: 2774 656d 7027 5d2c 0a20 2020 2027 6b69  'temp'],.    'ki
+000154c0: 7463 6865 6e2d 7465 6d70 2720 3a20 5b27  tchen-temp' : ['
+000154d0: 2f74 6d70 2f6b 6974 6368 656e 2d74 656d  /tmp/kitchen-tem
+000154e0: 702e 7272 6427 2c20 272d 2d74 656d 706c  p.rrd', '--templ
+000154f0: 6174 6527 2c20 2774 656d 7027 5d0a 2020  ate', 'temp'].  
+00015500: 2020 7d0a 6060 600a 0a5b 7272 6470 7974    }.```..[rrdpyt
+00015510: 686f 6e27 7320 4150 495d 2065 7870 6563  hon's API] expec
+00015520: 7473 2073 7472 696e 6773 2061 6e64 2f6f  ts strings and/o
+00015530: 7220 6120 6c69 7374 206f 6620 7374 7269  r a list of stri
+00015540: 6e67 7320 6173 2070 6172 616d 6574 6572  ngs as parameter
+00015550: 7320 746f 2074 6865 2066 756e 6374 696f  s to the functio
+00015560: 6e73 2e0a 5468 7573 2c20 6120 6c69 7374  ns..Thus, a list
+00015570: 2066 6f72 2061 2074 6172 6765 7420 7369   for a target si
+00015580: 6d70 6c79 2063 6f6e 7461 696e 7320 7468  mply contains th
+00015590: 6520 636f 6d6d 616e 6420 6c69 6e65 2061  e command line a
+000155a0: 7267 756d 656e 7473 2066 6f72 2060 7272  rguments for `rr
+000155b0: 6474 6f6f 6c20 7570 6461 7465 602e 0a0a  dtool update`...
+000155c0: 5468 6520 706c 7567 696e 2077 696c 6c20  The plugin will 
+000155d0: 656d 6265 6420 7468 6520 6d65 7373 6167  embed the messag
+000155e0: 6520 6173 2066 696e 616c 2061 7267 756d  e as final argum
+000155f0: 656e 7420 604e 3a3c 6d65 7373 6167 653e  ent `N:<message>
+00015600: 602c 2069 6620 7468 6520 6d65 7373 6167  `, if the messag
+00015610: 6520 6973 2061 6e0a 696e 7465 6765 7220  e is an.integer 
+00015620: 6e75 6d62 6572 2e20 4f74 6865 7277 6973  number. Otherwis
+00015630: 652c 2069 7420 7769 6c6c 2062 7265 616b  e, it will break
+00015640: 2075 7020 7468 6520 6d65 7373 6167 6520   up the message 
+00015650: 696e 746f 2073 696e 676c 6520 776f 7264  into single word
+00015660: 7320 616e 6420 6170 7065 6e64 2074 6869  s and append thi
+00015670: 7320 0a6c 6973 7420 746f 2074 6865 206c  s .list to the l
+00015680: 6973 7420 7375 7070 6c69 6564 2062 7920  ist supplied by 
+00015690: 7468 6520 7461 7267 6574 2e20 5468 6973  the target. This
+000156a0: 206c 6561 7665 7320 6974 2074 6f20 796f   leaves it to yo
+000156b0: 7572 2064 6973 6372 6574 696f 6e20 5f77  ur discretion _w
+000156c0: 6865 7265 5f20 746f 2070 7574 0a61 7267  here_ to put.arg
+000156d0: 756d 656e 7473 2061 6e64 2065 7665 6e20  uments and even 
+000156e0: 2d20 7769 7468 2074 6865 2072 6967 6874  - with the right
+000156f0: 2064 6174 6120 6d61 7070 696e 6720 616e   data mapping an
+00015700: 6420 6578 7472 6163 7469 6f6e 2069 6e20  d extraction in 
+00015710: 706c 6163 6520 2d20 616c 6c6f 7773 2066  place - allows f
+00015720: 6f72 200a 6120 636f 6e66 6967 7572 6174  or .a configurat
+00015730: 696f 6e20 6c69 6b65 3a0a 0a60 6060 696e  ion like:..```in
+00015740: 690a 5b63 6f6e 6669 673a 7272 6474 6f6f  i.[config:rrdtoo
+00015750: 6c5d 0a74 6172 6765 7473 203d 207b 0a20  l].targets = {. 
+00015760: 2020 2020 2020 2027 6261 7474 7365 6e73         'battsens
+00015770: 6f72 273a 205b 205d 2c0a 2020 2020 2020  or': [ ],.      
+00015780: 2020 7d0a 2e2e 2e0a 5b64 6174 616c 6f67    }.....[datalog
+00015790: 2d62 6174 7465 7279 2d6c 6f67 5d0a 746f  -battery-log].to
+000157a0: 7069 6320 3d20 6461 7461 6c6f 672f 7365  pic = datalog/se
+000157b0: 6e73 6f72 732f 6261 7474 2f2b 0a74 6172  nsors/batt/+.tar
+000157c0: 6765 7473 203d 206c 6f67 3a69 6e66 6f2c  gets = log:info,
+000157d0: 7272 6474 6f6f 6c3a 6261 7474 7365 6e73  rrdtool:battsens
+000157e0: 6f72 0a64 6174 616d 6170 203d 202e 2e2e  or.datamap = ...
+000157f0: 0a66 6f72 6d61 7420 3d20 2f73 7276 2f72  .format = /srv/r
+00015800: 7264 2f73 656e 736f 7273 2f7b 7365 6e73  rd/sensors/{sens
+00015810: 6f72 5f69 647d 2e72 7264 202d 7420 6261  or_id}.rrd -t ba
+00015820: 7474 207b 7473 7d3a 7b62 6174 747d 0a60  tt {ts}:{batt}.`
+00015830: 6060 0a0a 5265 7175 6972 6573 2074 6865  ``..Requires the
+00015840: 2072 7264 746f 6f6c 2062 696e 6469 6e67   rrdtool binding
+00015850: 7320 6176 6169 6c61 626c 6520 7769 7468  s available with
+00015860: 2060 7069 7020 696e 7374 616c 6c20 7272   `pip install rr
+00015870: 6474 6f6f 6c60 2e0a 0a5b 7272 6474 6f6f  dtool`...[rrdtoo
+00015880: 6c5d 3a20 6874 7470 3a2f 2f6f 7373 2e6f  l]: http://oss.o
+00015890: 6574 696b 6572 2e63 682f 7272 6474 6f6f  etiker.ch/rrdtoo
+000158a0: 6c2f 0a5b 7272 6470 7974 686f 6e27 7320  l/.[rrdpython's 
+000158b0: 4150 495d 3a20 6874 7470 3a2f 2f6f 7373  API]: http://oss
+000158c0: 2e6f 6574 696b 6572 2e63 682f 7272 6474  .oetiker.ch/rrdt
+000158d0: 6f6f 6c2f 7072 6f67 2f72 7264 7079 7468  ool/prog/rrdpyth
+000158e0: 6f6e 2e65 6e2e 6874 6d6c 0a0a 2323 2320  on.en.html..### 
+000158f0: 6073 6572 6961 6c60 0a0a 5468 6520 6073  `serial`..The `s
+00015900: 6572 6961 6c60 2070 6c75 6769 6e20 7365  erial` plugin se
+00015910: 6e64 7320 6f75 7420 7265 6365 6976 6564  nds out received
+00015920: 206d 6573 7361 6765 7320 746f 2074 6865   messages to the
+00015930: 2073 6572 6961 6c20 706f 7274 2e20 4d65   serial port. Me
+00015940: 7373 6167 6520 7061 796c 6f61 6420 6361  ssage payload ca
+00015950: 6e20 6265 2062 696e 6172 7920 6461 7461  n be binary data
+00015960: 2c20 7374 7269 6e67 206f 7220 6a73 6f6e  , string or json
+00015970: 2e0a 0a60 6060 696e 690a 5b63 6f6e 6669  ...```ini.[confi
+00015980: 673a 7365 7269 616c 5d0a 6170 7065 6e64  g:serial].append
+00015990: 5f6e 6577 6c69 6e65 203d 2046 616c 7365  _newline = False
+000159a0: 0a74 6172 6765 7473 203d 207b 0a20 2020  .targets = {.   
+000159b0: 2027 7365 7269 616c 706f 7274 3127 2020   'serialport1'  
+000159c0: 3a20 5b27 2f64 6576 2f74 7479 5553 4230  : ['/dev/ttyUSB0
+000159d0: 272c 2020 2731 3135 3230 3027 5d2c 0a20  ',  '115200'],. 
+000159e0: 2020 2027 736f 6d65 2d64 6576 6963 6527     'some-device'
+000159f0: 203a 205b 2773 6f63 6b65 743a 2f2f 3139   : ['socket://19
+00015a00: 322e 3136 382e 312e 3130 303a 3233 3233  2.168.1.100:2323
+00015a10: 272c 2027 3936 3030 275d 0a20 2020 207d  ', '9600'].    }
+00015a20: 0a60 6060 0a46 6972 7374 2070 6172 616d  .```.First param
+00015a30: 6574 6572 2069 6e20 7461 7267 6574 2063  eter in target c
+00015a40: 6f6e 6669 6720 6361 6e20 6265 2061 2070  onfig can be a p
+00015a50: 6f72 746e 616d 6520 6f72 2061 6e20 5b75  ortname or an [u
+00015a60: 726c 2068 616e 646c 6572 5d28 6874 7470  rl handler](http
+00015a70: 733a 2f2f 7079 7468 6f6e 686f 7374 6564  s://pythonhosted
+00015a80: 2e6f 7267 2f70 7973 6572 6961 6c2f 7572  .org/pyserial/ur
+00015a90: 6c5f 6861 6e64 6c65 7273 2e68 746d 6c29  l_handlers.html)
+00015aa0: 2e0a 5365 636f 6e64 2070 6172 616d 6574  ..Second paramet
+00015ab0: 6572 2069 7320 7468 6520 6261 7564 7261  er is the baudra
+00015ac0: 7465 2066 6f72 2074 6865 2070 6f72 742e  te for the port.
+00015ad0: 0a49 6620 6061 7070 656e 645f 6e65 776c  .If `append_newl
+00015ae0: 696e 6560 2069 7320 5472 7565 2c20 6120  ine` is True, a 
+00015af0: 6e65 776c 696e 6520 6368 6172 6163 7465  newline characte
+00015b00: 7220 6973 2075 6e63 6f6e 6469 7469 6f6e  r is uncondition
+00015b10: 616c 6c79 2061 7070 656e 6465 6420 746f  ally appended to
+00015b20: 2074 6865 2073 7472 696e 6720 7772 6974   the string writ
+00015b30: 7465 6e20 746f 2074 6865 2073 6572 6961  ten to the seria
+00015b40: 6c70 6f72 742e 0a0a 5265 7175 6972 6573  lport...Requires
+00015b50: 2074 6865 2070 7973 6572 6961 6c20 6269   the pyserial bi
+00015b60: 6e64 696e 6773 2061 7661 696c 6162 6c65  ndings available
+00015b70: 2077 6974 6820 6070 6970 2069 6e73 7461   with `pip insta
+00015b80: 6c6c 2070 7973 6572 6961 6c60 2e0a 0a23  ll pyserial`...#
+00015b90: 2323 2060 736c 6163 6b60 0a0a 5468 6520  ## `slack`..The 
+00015ba0: 6073 6c61 636b 6020 706c 7567 696e 2070  `slack` plugin p
+00015bb0: 6f73 7473 206d 6573 7361 6765 7320 746f  osts messages to
+00015bc0: 2063 6861 6e6e 656c 7320 696e 206f 7220   channels in or 
+00015bd0: 7573 6572 7320 6f66 2074 6865 205b 736c  users of the [sl
+00015be0: 6163 6b2e 636f 6d5d 2868 7474 703a 2f2f  ack.com](http://
+00015bf0: 736c 6163 6b2e 636f 6d29 2073 6572 7669  slack.com) servi
+00015c00: 6365 2e20 5468 6520 636f 6e66 6967 7572  ce. The configur
+00015c10: 6174 696f 6e20 6f66 2074 6869 7320 7365  ation of this se
+00015c20: 7276 6963 6520 7265 7175 6972 6573 2061  rvice requires a
+00015c30: 6e20 4150 4920 746f 6b65 6e20 6f62 7461  n API token obta
+00015c40: 696e 696e 6162 6c65 2074 6865 7265 2e0a  ininable there..
+00015c50: 0a60 6060 696e 690a 5b63 6f6e 6669 673a  .```ini.[config:
+00015c60: 736c 6163 6b5d 0a74 6f6b 656e 203d 2027  slack].token = '
+00015c70: 7878 7878 2d31 3233 3435 3637 3839 302d  xxxx-1234567890-
+00015c80: 3132 3334 3536 3738 3930 2d31 3233 3435  1234567890-12345
+00015c90: 3637 3839 302d 3132 3334 6131 270a 7461  67890-1234a1'.ta
+00015ca0: 7267 6574 7320 3d20 7b0a 2020 2020 2020  rgets = {.      
+00015cb0: 2020 2020 2020 2020 2020 2320 2020 5b74            #   [t
+00015cc0: 6f6b 656e 2c5d 2023 6368 616e 6e65 6c2f  oken,] #channel/
+00015cd0: 4075 7365 722c 2075 7365 726e 616d 652c  @user, username,
+00015ce0: 2069 636f 6e2c 205b 6173 5f75 7365 725d   icon, [as_user]
+00015cf0: 0a20 2020 276a 706d 656e 7327 2020 2020  .   'jpmens'    
+00015d00: 203a 205b 2027 406a 706d 656e 7327 2c20   : [ '@jpmens', 
+00015d10: 2020 2241 6c65 7274 6572 222c 2020 2027    "Alerter",   '
+00015d20: 3a64 6f6f 723a 2720 2020 2020 2020 2020  :door:'         
+00015d30: 205d 2c0a 2020 2027 6765 6e65 7261 6c27   ],.   'general'
+00015d40: 2020 2020 3a20 5b20 2723 6765 6e65 7261      : [ '#genera
+00015d50: 6c27 2c20 2022 6d71 7474 7761 726e 222c  l',  "mqttwarn",
+00015d60: 2020 273a 7379 7269 6e67 653a 2720 2020    ':syringe:'   
+00015d70: 2020 2020 5d2c 0a20 2020 2774 6573 7427      ],.   'test'
+00015d80: 2020 2020 2020 203a 205b 2027 2374 6573         : [ '#tes
+00015d90: 7427 2c20 2020 2020 2242 6f74 5573 6572  t',     "BotUser
+00015da0: 222c 2020 2027 3a75 6e75 7365 643a 272c  ",   ':unused:',
+00015db0: 2020 5472 7565 205d 2c0a 2020 2027 7365    True ],.   'se
+00015dc0: 636f 6e64 2d61 6363 2720 3a20 5b20 2778  cond-acc' : [ 'x
+00015dd0: 7878 782d 3939 3939 3939 392d 3939 3939  xxx-9999999-9999
+00015de0: 3939 392d 3939 3939 3939 3939 272c 2027  999-99999999', '
+00015df0: 2367 656e 6572 616c 272c 2022 7465 7374  #general', "test
+00015e00: 222c 2027 3a68 6f75 7365 3a27 205d 2c0a  ", ':house:' ],.
+00015e10: 2020 7d0a 6060 600a 0a54 6865 2073 6572    }.```..The ser
+00015e20: 7669 6365 206c 6576 656c 2060 746f 6b65  vice level `toke
+00015e30: 6e60 2069 7320 6f70 7469 6f6e 616c 2c20  n` is optional, 
+00015e40: 6275 7420 6966 206d 6973 7369 6e67 2065  but if missing e
+00015e50: 6163 6820 7461 7267 6574 206d 7573 7420  ach target must 
+00015e60: 6861 7665 2061 2060 746f 6b65 6e60 2064  have a `token` d
+00015e70: 6566 696e 6564 2e0a 0a45 6163 6820 7461  efined...Each ta
+00015e80: 7267 6574 2064 6566 696e 6573 2074 6865  rget defines the
+00015e90: 206e 616d 6520 6f66 2061 6e20 6578 6973   name of an exis
+00015ea0: 7469 6e67 2063 6861 6e6e 656c 2028 6023  ting channel (`#
+00015eb0: 6368 616e 6e65 6c6e 616d 6560 2920 6f72  channelname`) or
+00015ec0: 2061 2075 7365 7220 2860 4075 7365 726e   a user (`@usern
+00015ed0: 616d 6560 2920 746f 2062 650a 6164 6472  ame`) to be.addr
+00015ee0: 6573 7365 642c 2074 6865 206e 616d 6520  essed, the name 
+00015ef0: 6f66 2074 6865 2073 656e 6469 6e67 2075  of the sending u
+00015f00: 7365 7220 6173 2077 656c 6c20 6173 2061  ser as well as a
+00015f10: 6e20 5b65 6d6f 6a69 2069 636f 6e5d 2868  n [emoji icon](h
+00015f20: 7474 703a 2f2f 7777 772e 656d 6f6a 692d  ttp://www.emoji-
+00015f30: 6368 6561 742d 7368 6565 742e 636f 6d29  cheat-sheet.com)
+00015f40: 2074 6f20 7573 652e 0a0a 4f70 7469 6f6e   to use...Option
+00015f50: 616c 6c79 2c20 6120 7461 7267 6574 2063  ally, a target c
+00015f60: 616e 2064 6566 696e 6520 7468 6520 6d65  an define the me
+00015f70: 7373 6167 6520 746f 2067 6574 2070 6f73  ssage to get pos
+00015f80: 7465 6420 6173 2061 2075 7365 722c 2070  ted as a user, p
+00015f90: 6572 0a5b 536c 6163 6b20 4175 7468 6f72  er.[Slack Author
+00015fa0: 7368 6970 2064 6f63 756d 656e 7461 7469  ship documentati
+00015fb0: 6f6e 5d28 6874 7470 733a 2f2f 6170 692e  on](https://api.
+00015fc0: 736c 6163 6b2e 636f 6d2f 6d65 7468 6f64  slack.com/method
+00015fd0: 732f 6368 6174 2e70 6f73 744d 6573 7361  s/chat.postMessa
+00015fe0: 6765 2361 7574 686f 7273 6869 7029 2e0a  ge#authorship)..
+00015ff0: 4e6f 7465 2074 6861 7420 706f 7374 696e  Note that postin
+00016000: 6720 6173 2061 2075 7365 7220 696e 2061  g as a user in a
+00016010: 2063 6861 6e6e 656c 2069 7320 6f6e 6c79   channel is only
+00016020: 2070 6f73 7369 626c 652c 2069 6620 7468   possible, if th
+00016030: 6520 7573 6572 2068 6173 0a6a 6f69 6e65  e user has.joine
+00016040: 6420 7468 6520 6368 616e 6e65 6c2e 0a0a  d the channel...
+00016050: 215b 536c 6163 6b5d 2861 7373 6574 732f  ![Slack](assets/
+00016060: 736c 6163 6b2e 706e 6729 0a0a 5468 6973  slack.png)..This
+00016070: 2070 6c75 6769 6e20 7265 7175 6972 6573   plugin requires
+00016080: 205b 5079 7468 6f6e 2073 6c61 636b 2d73   [Python slack-s
+00016090: 646b 5d28 6874 7470 733a 2f2f 6769 7468  dk](https://gith
+000160a0: 7562 2e63 6f6d 2f73 6c61 636b 6170 692f  ub.com/slackapi/
+000160b0: 7079 7468 6f6e 2d73 6c61 636b 2d73 646b  python-slack-sdk
+000160c0: 292e 0a0a 5468 6520 736c 6163 6b20 7365  )...The slack se
+000160d0: 7276 6963 6520 7769 6c6c 2061 6363 6570  rvice will accep
+000160e0: 7420 6120 7061 796c 6f61 6420 7769 7468  t a payload with
+000160f0: 2065 6974 6865 7220 6120 7369 6d70 6c65   either a simple
+00016100: 2074 6578 7420 6d65 7373 6167 652c 206f   text message, o
+00016110: 7220 6120 6a73 6f6e 2070 6179 6c6f 6164  r a json payload
+00016120: 2077 6869 6368 2063 6f6e 7461 696e 730a   which contains.
+00016130: 6120 606d 6573 7361 6765 6020 616e 6420  a `message` and 
+00016140: 6569 7468 6572 2061 6e20 6069 6d61 6765  either an `image
+00016150: 7572 6c60 206f 7220 6069 6d61 6765 6261  url` or `imageba
+00016160: 7365 3634 6020 656e 636f 6465 6420 696d  se64` encoded im
+00016170: 6167 652e 0a0a 4675 7274 6865 722c 2074  age...Further, t
+00016180: 6865 2069 6d61 6765 7572 6c20 7061 796c  he imageurl payl
+00016190: 6f61 642c 2063 616e 2068 6176 6520 7468  oad, can have th
+000161a0: 6520 6164 6469 7469 6f6e 616c 2070 6172  e additional par
+000161b0: 616d 6574 6572 7320 6f66 2061 6e20 6175  ameters of an au
+000161c0: 7468 2074 7970 6520 2862 6173 6963 2c20  th type (basic, 
+000161d0: 6469 6765 7374 2920 616e 6420 6120 7573  digest) and a us
+000161e0: 6572 2061 6e64 2070 6173 7377 6f72 642e  er and password.
+000161f0: 2020 5468 6973 2069 7320 7573 6566 756c    This is useful
+00016200: 2069 6620 796f 7572 2069 6d61 6769 6e67   if your imaging
+00016210: 2064 6576 6963 6520 7573 6573 2061 7574   device uses aut
+00016220: 6865 6e74 6963 6174 696f 6e2e 2020 536f  hentication.  So
+00016230: 6d65 2065 7861 6d70 6c65 7320 6172 6520  me examples are 
+00016240: 736f 6d65 2049 5020 6361 6d65 7261 732c  some IP cameras,
+00016250: 206f 7220 736f 6d65 206f 7468 6572 2073   or some other s
+00016260: 696d 706c 6520 696e 7465 726e 6574 2062  imple internet b
+00016270: 6173 6564 2069 6d61 6765 2073 6572 7669  ased image servi
+00016280: 6365 732e 0a0a 5468 6520 666f 6c6c 6f77  ces...The follow
+00016290: 696e 6720 7061 796c 6f61 6473 2061 7265  ing payloads are
+000162a0: 2076 616c 6964 3b0a 0a60 6060 0a53 696d   valid;..```.Sim
+000162b0: 706c 6520 7465 7874 206d 6573 7361 6765  ple text message
+000162c0: 0a60 6060 0a0a 6060 606a 736f 6e0a 7b0a  .```..```json.{.
+000162d0: 2020 2020 226d 6573 7361 6765 223a 2022      "message": "
+000162e0: 4d65 7373 6167 6520 6f6e 6c79 2c20 7769  Message only, wi
+000162f0: 7468 206e 6f20 696d 6167 6522 0a7d 0a60  th no image".}.`
+00016300: 6060 0a0a 6060 606a 736f 6e0a 207b 0a20  ``..```json. {. 
+00016310: 2020 2022 6d65 7373 6167 6522 3a20 224d     "message": "M
+00016320: 6573 7361 6765 2077 6974 6820 6261 7365  essage with base
+00016330: 3634 2065 6e63 6f64 6564 2069 6d61 6765  64 encoded image
+00016340: 222c 0a20 2020 2022 696d 6167 6562 6173  ",.    "imagebas
+00016350: 6536 3422 3a20 223c 6261 7365 3634 2065  e64": "<base64 e
+00016360: 6e63 6f64 6564 2069 6d61 6765 3e22 0a20  ncoded image>". 
+00016370: 7d0a 6060 600a 0a60 6060 6a73 6f6e 0a20  }.```..```json. 
+00016380: 7b0a 2020 2020 226d 6573 7361 6765 223a  {.    "message":
+00016390: 2022 4d65 7373 6167 6520 7769 7468 2069   "Message with i
+000163a0: 6d61 6765 2064 6f77 6e6c 6f61 6465 6420  mage downloaded 
+000163b0: 6672 6f6d 2055 524c 222c 0a20 2020 2022  from URL",.    "
+000163c0: 696d 6167 6575 726c 223a 2022 3c69 6d61  imageurl": "<ima
+000163d0: 6765 2075 726c 3e22 0a20 7d0a 6060 600a  ge url>". }.```.
+000163e0: 0a60 6060 6a73 6f6e 0a20 7b0a 2020 2020  .```json. {.    
+000163f0: 226d 6573 7361 6765 223a 2022 4d65 7373  "message": "Mess
+00016400: 6167 6520 7769 7468 2069 6d61 6765 2064  age with image d
+00016410: 6f77 6e6c 6f61 6465 6420 6672 6f6d 2055  ownloaded from U
+00016420: 524c 3a20 6469 6765 7374 2061 7574 6865  RL: digest authe
+00016430: 6e74 6963 6174 696f 6e22 2c0a 2020 2020  ntication",.    
+00016440: 2269 6d61 6765 7572 6c22 3a20 223c 696d  "imageurl": "<im
+00016450: 6167 6520 7572 6c3e 222c 0a20 2020 2022  age url>",.    "
+00016460: 6175 7468 223a 2022 6469 6765 7374 222c  auth": "digest",
+00016470: 0a20 2020 2022 7573 6572 223a 2022 6d79  .    "user": "my
+00016480: 7370 6563 6961 6c75 7365 7222 2c0a 2020  specialuser",.  
+00016490: 2020 2270 6173 7377 6f72 6422 3a20 226d    "password": "m
+000164a0: 7973 7065 6369 616c 7061 7373 776f 7264  yspecialpassword
+000164b0: 220a 207d 0a60 6060 0a46 6f72 2074 6865  ". }.```.For the
+000164c0: 2061 626f 7665 2065 7861 6d70 6c65 2c20   above example, 
+000164d0: 4920 776f 756c 6420 6f6e 6c79 2072 6563  I would only rec
+000164e0: 6f6d 6d65 6e64 2074 6869 7320 6265 2075  ommend this be u
+000164f0: 7365 6420 696e 2061 206c 6f63 616c 204d  sed in a local M
+00016500: 5154 5420 7365 7276 6572 2069 6e73 7461  QTT server insta
+00016510: 6e63 652c 2061 7320 7468 6520 7061 7373  nce, as the pass
+00016520: 776f 7264 2066 6f72 2079 6f75 7220 696d  word for your im
+00016530: 6167 696e 6720 6465 7669 6365 2069 7320  aging device is 
+00016540: 6265 696e 6720 7472 616e 736d 6974 7465  being transmitte
+00016550: 6420 696e 2074 6865 2063 6c65 6172 2074  d in the clear t
+00016560: 6f20 6d71 7474 7761 726e 2e0a 0a23 2323  o mqttwarn...###
+00016570: 2060 7371 6c69 7465 600a 0a54 6865 2060   `sqlite`..The `
+00016580: 7371 6c69 7465 6020 706c 7567 696e 2063  sqlite` plugin c
+00016590: 7265 6174 6573 2061 2074 6162 6c65 2069  reates a table i
+000165a0: 6e20 7468 6520 6461 7461 6261 7365 2066  n the database f
+000165b0: 696c 6520 7370 6563 6966 6965 6420 696e  ile specified in
+000165c0: 2074 6865 2074 6172 6765 7473 2c0a 616e   the targets,.an
+000165d0: 6420 6372 6561 7465 7320 6120 7363 6865  d creates a sche
+000165e0: 6d61 2077 6974 6820 6120 7369 6e67 6c65  ma with a single
+000165f0: 2063 6f6c 756d 6e20 6361 6c6c 6564 2060   column called `
+00016600: 7061 796c 6f61 6460 206f 6620 7479 7065  payload` of type
+00016610: 2060 5445 5854 602e 205f 6d71 7474 7761   `TEXT`. _mqttwa
+00016620: 726e 5f0a 636f 6d6d 6974 7320 6d65 7373  rn_.commits mess
+00016630: 6167 6573 2072 6f75 7465 6420 746f 2073  ages routed to s
+00016640: 7563 6820 6120 7461 7267 6574 2069 6d6d  uch a target imm
+00016650: 6564 6961 7465 6c79 2e0a 0a60 6060 696e  ediately...```in
+00016660: 690a 5b63 6f6e 6669 673a 7371 6c69 7465  i.[config:sqlite
+00016670: 5d0a 7461 7267 6574 7320 3d20 7b0a 2020  ].targets = {.  
+00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016690: 2023 7061 7468 2020 2020 2020 2020 2374   #path        #t
+000166a0: 6162 6c65 6e61 6d65 0a20 2027 6465 6d6f  ablename.  'demo
+000166b0: 7461 626c 6527 203a 205b 2027 2f74 6d70  table' : [ '/tmp
+000166c0: 2f6d 2e64 6227 2c20 2027 6d71 7474 7761  /m.db',  'mqttwa
+000166d0: 726e 2720 205d 0a20 207d 0a60 6060 0a0a  rn'  ].  }.```..
+000166e0: 2323 2320 6073 716c 6974 655f 6a73 6f6e  ### `sqlite_json
+000166f0: 3263 6f6c 7360 0a0a 5468 6520 6073 716c  2cols`..The `sql
+00016700: 6974 655f 6a73 6f6e 3263 6f6c 7360 2070  ite_json2cols` p
+00016710: 6c75 6769 6e20 6372 6561 7465 7320 6120  lugin creates a 
+00016720: 7461 626c 6520 696e 2074 6865 2064 6174  table in the dat
+00016730: 6162 6173 6520 6669 6c65 2073 7065 6369  abase file speci
+00016740: 6669 6564 2069 6e20 7468 6520 7461 7267  fied in the targ
+00016750: 6574 730a 616e 6420 6372 6561 7465 7320  ets.and creates 
+00016760: 6120 7363 6865 6d61 2062 6173 6564 206f  a schema based o
+00016770: 6e20 7468 6520 4a53 4f4e 2070 6179 6c6f  n the JSON paylo
+00016780: 6164 2e0a 4974 2077 696c 6c20 6372 6561  ad..It will crea
+00016790: 7465 2061 2063 6f6c 756d 6e20 666f 7220  te a column for 
+000167a0: 6561 6368 204a 534f 4e20 656e 7472 7920  each JSON entry 
+000167b0: 616e 6420 7275 6469 6d65 6e74 6172 7920  and rudimentary 
+000167c0: 7472 7920 746f 2064 6574 6572 6d69 6e65  try to determine
+000167d0: 2069 7473 2064 6174 6174 7970 6520 6f6e   its datatype on
+000167e0: 2063 7265 6174 696f 6e20 2846 6c6f 6174   creation (Float
+000167f0: 206f 7220 4368 6172 292e 0a0a 4173 2061   or Char)...As a
+00016800: 6e20 6578 616d 706c 652c 2070 7562 6c69  n example, publi
+00016810: 7368 696e 6720 7468 6973 204a 534f 4e20  shing this JSON 
+00016820: 7061 796c 6f61 643a 0a0a 6060 600a 6d6f  payload:..```.mo
+00016830: 7371 7569 7474 6f5f 7075 6220 2d74 2074  squitto_pub -t t
+00016840: 6573 742f 6865 6c6c 6f20 2d6d 2027 7b20  est/hello -m '{ 
+00016850: 226e 616d 6522 203a 2022 5468 6f72 222c  "name" : "Thor",
+00016860: 2022 4661 7468 6572 2220 3a20 274f 6469   "Father" : 'Odi
+00016870: 6e27 2c20 2241 6765 2220 3a20 3330 207d  n', "Age" : 30 }
+00016880: 270a 6060 600a 0a41 2074 6162 6c65 2061  '.```..A table a
+00016890: 7320 7374 6174 6564 2069 6e20 7468 6520  s stated in the 
+000168a0: 636f 6e66 6967 7572 6174 696f 6e20 7769  configuration wi
+000168b0: 6c6c 2062 6520 6372 6561 7465 6420 6f6e  ll be created on
+000168c0: 2074 6865 2066 6c79 2077 6974 6820 7468   the fly with th
+000168d0: 6520 666f 6c6c 6f77 696e 6720 7374 7275  e following stru
+000168e0: 6374 7572 6520 616e 6420 636f 6e74 656e  cture and conten
+000168f0: 743a 0a0a 6060 600a 2b2d 2d2d 2d2d 2d2b  t:..```.+------+
+00016900: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2b  --------+------+
+00016910: 0a7c 206e 616d 6520 7c20 4661 7468 6572  .| name | Father
+00016920: 207c 2041 6765 2020 7c0a 2b2d 2d2d 2d2d   | Age  |.+-----
+00016930: 2d2b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  -+--------+-----
+00016940: 2d2b 0a7c 2054 686f 7220 7c20 4f64 696e  -+.| Thor | Odin
+00016950: 2020 207c 2033 302e 3020 7c0a 2b2d 2d2d     | 30.0 |.+---
+00016960: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ---+--------+---
+00016970: 2d2d 2d2b 0a60 6060 0a4e 6f20 7461 626c  ---+.```.No tabl
+00016980: 6520 6973 2063 7265 6174 6564 2069 6620  e is created if 
+00016990: 7468 6520 7461 626c 6520 6e61 6d65 2061  the table name a
+000169a0: 6c72 6561 6479 2065 7869 7374 732e 0a0a  lready exists...
+000169b0: 205f 6d71 7474 7761 726e 5f0a 636f 6d6d   _mqttwarn_.comm
+000169c0: 6974 7320 6d65 7373 6167 6573 2072 6f75  its messages rou
+000169d0: 7465 6420 746f 2073 7563 6820 6120 7461  ted to such a ta
+000169e0: 7267 6574 2069 6d6d 6564 6961 7465 6c79  rget immediately
+000169f0: 2e0a 0a60 6060 696e 690a 5b63 6f6e 6669  ...```ini.[confi
+00016a00: 673a 7371 6c69 7465 5f6a 736f 6e32 636f  g:sqlite_json2co
+00016a10: 6c73 5d0a 7461 7267 6574 7320 3d20 7b0a  ls].targets = {.
+00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a30: 2020 2023 7061 7468 2020 2020 2020 2020     #path        
+00016a40: 2374 6162 6c65 6e61 6d65 0a20 2027 6465  #tablename.  'de
+00016a50: 6d6f 7461 626c 6527 203a 205b 2027 2f74  motable' : [ '/t
+00016a60: 6d70 2f6d 2e64 6227 2c20 2027 6d71 7474  mp/m.db',  'mqtt
+00016a70: 7761 726e 2720 205d 0a20 207d 0a60 6060  warn'  ].  }.```
+00016a80: 0a0a 2323 2320 6073 716c 6974 655f 7469  ..### `sqlite_ti
+00016a90: 6d65 7374 616d 7060 0a0a 5468 6520 6073  mestamp`..The `s
+00016aa0: 716c 6974 655f 7469 6d65 7374 616d 7060  qlite_timestamp`
+00016ab0: 2070 6c75 6769 6e20 776f 726b 7320 6a75   plugin works ju
+00016ac0: 7374 206c 696b 6520 7468 6520 2773 716c  st like the 'sql
+00016ad0: 6974 6527 2070 6c75 6769 6e2c 2062 7574  ite' plugin, but
+00016ae0: 2069 7420 6372 6561 7465 7320 3320 636f   it creates 3 co
+00016af0: 6c75 6d6e 733a 2069 642c 2070 6179 6c6f  lumns: id, paylo
+00016b00: 6164 2061 6e64 2074 696d 6573 7461 6d70  ad and timestamp
+00016b10: 2e0a 5468 6520 6964 2069 7320 7468 6520  ..The id is the 
+00016b20: 7461 626c 6520 696e 6465 7820 616e 6420  table index and 
+00016b30: 7468 6520 7469 6d65 7374 616d 7020 6973  the timestamp is
+00016b40: 2074 6865 2069 6e73 6572 7469 6f6e 2064   the insertion d
+00016b50: 6174 6520 616e 6420 7469 6d65 2069 6e20  ate and time in 
+00016b60: 7365 636f 6e64 732e 0a0a 6060 6069 6e69  seconds...```ini
+00016b70: 0a5b 636f 6e66 6967 3a73 716c 6974 655f  .[config:sqlite_
+00016b80: 7469 6d65 7374 616d 705d 0a74 6172 6765  timestamp].targe
+00016b90: 7473 203d 207b 0a20 2020 2020 2020 2020  ts = {.         
+00016ba0: 2020 2020 2020 2020 2020 2370 6174 6820            #path 
+00016bb0: 2020 2020 2020 2023 7461 626c 656e 616d         #tablenam
+00016bc0: 650a 2020 2764 656d 6f74 6162 6c65 2720  e.  'demotable' 
+00016bd0: 3a20 5b20 272f 746d 702f 6d2e 6462 272c  : [ '/tmp/m.db',
+00016be0: 2020 276d 7174 7477 6172 6e27 2020 5d0a    'mqttwarn'  ].
+00016bf0: 2020 7d0a 6060 600a 0a23 2323 2060 736d    }.```..### `sm
+00016c00: 7470 600a 0a54 6865 2060 736d 7470 6020  tp`..The `smtp` 
+00016c10: 7365 7276 6963 6520 6261 7369 6361 6c6c  service basicall
+00016c20: 7920 696d 706c 656d 656e 7473 2061 6e20  y implements an 
+00016c30: 4d51 5454 2074 6f20 534d 5450 2067 6174  MQTT to SMTP gat
+00016c40: 6577 6179 2077 6869 6368 206e 6565 6473  eway which needs
+00016c50: 0a63 6f6e 6669 6775 7261 7469 6f6e 2e0a  .configuration..
+00016c60: 0a60 6060 696e 690a 5b63 6f6e 6669 673a  .```ini.[config:
+00016c70: 736d 7470 5d0a 7365 7276 6572 2020 3d20  smtp].server  = 
+00016c80: 2027 6c6f 6361 6c68 6f73 743a 3235 270a   'localhost:25'.
+00016c90: 7365 6e64 6572 2020 3d20 2022 4d51 5454  sender  =  "MQTT
+00016ca0: 7761 726e 203c 6a70 6d40 6c6f 6361 6c68  warn <jpm@localh
+00016cb0: 6f73 743e 220a 7573 6572 6e61 6d65 2020  ost>".username  
+00016cc0: 3d20 204e 6f6e 650a 7061 7373 776f 7264  =  None.password
+00016cd0: 2020 3d20 204e 6f6e 650a 7374 6172 7474    =  None.startt
+00016ce0: 6c73 2020 3d20 2046 616c 7365 0a23 204f  ls  =  False.# O
+00016cf0: 7074 696f 6e61 6c20 7365 6e64 206d 7367  ptional send msg
+00016d00: 2061 7320 6874 6d6c 206f 7220 6f6e 6c79   as html or only
+00016d10: 2070 6c61 696e 2074 6578 740a 6874 6d6c   plain text.html
+00016d20: 6d73 6720 2020 3d20 2046 616c 7365 0a74  msg   =  False.t
+00016d30: 6172 6765 7473 203d 207b 0a20 2020 2027  argets = {.    '
+00016d40: 6c6f 6361 6c6a 2720 2020 2020 3a20 5b20  localj'     : [ 
+00016d50: 276a 706d 406c 6f63 616c 686f 7374 2720  'jpm@localhost' 
+00016d60: 5d2c 0a20 2020 2027 7370 6563 6961 6c27  ],.    'special'
+00016d70: 2020 2020 3a20 5b20 2762 656e 4067 6d61      : [ 'ben@gma
+00016d80: 696c 272c 2027 7375 7a69 6540 6578 616d  il', 'suzie@exam
+00016d90: 706c 652e 6e65 7427 205d 0a20 2020 207d  ple.net' ].    }
+00016da0: 0a60 6060 0a0a 5461 7267 6574 7320 6d61  .```..Targets ma
+00016db0: 7920 636f 6e74 6169 6e20 6d6f 7265 2074  y contain more t
+00016dc0: 6861 6e20 6f6e 6520 7265 6369 7069 656e  han one recipien
+00016dd0: 742c 2069 6e20 7768 6963 6820 6361 7365  t, in which case
+00016de0: 2061 6c6c 2073 7065 6369 6669 6564 0a72   all specified.r
+00016df0: 6563 6970 6965 6e74 7320 6765 7420 7468  ecipients get th
+00016e00: 6520 6d65 7373 6167 652e 0a0a 7c20 546f  e message...| To
+00016e10: 7069 6320 6f70 7469 6f6e 2020 7c20 204d  pic option  |  M
+00016e20: 2f4f 2020 207c 2044 6573 6372 6970 7469  /O   | Descripti
+00016e30: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00016e40: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00016e50: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  | ------------- 
+00016e60: 7c20 3a2d 2d2d 2d3a 207c 202d 2d2d 2d2d  | :----: | -----
+00016e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016e90: 2d20 7c0a 7c20 6074 6974 6c65 6020 2020  - |.| `title`   
+00016ea0: 2020 2020 7c20 2020 4f20 2020 207c 2065      |   O    | e
+00016eb0: 2d6d 6169 6c20 7375 626a 6563 742e 2028  -mail subject. (
+00016ec0: 6466 6c74 3a20 606d 7174 7477 6172 6e20  dflt: `mqttwarn 
+00016ed0: 6e6f 7469 6669 6361 7469 6f6e 6029 207c  notification`) |
+00016ee0: 0a0a 2323 2320 6073 7368 600a 0a54 6865  ..### `ssh`..The
+00016ef0: 2060 7373 6860 2073 6572 7669 6365 2063   `ssh` service c
+00016f00: 616e 2072 756e 2063 6f6d 6d61 6e64 7320  an run commands 
+00016f10: 6f76 6572 2073 7368 2e0a 4966 2062 6f74  over ssh..If bot
+00016f20: 6820 7573 6572 2061 6e64 2070 6173 7377  h user and passw
+00016f30: 6f72 6420 6172 6520 6465 6669 6e65 6420  ord are defined 
+00016f40: 696e 2074 6865 2063 6f6e 6669 672c 2074  in the config, t
+00016f50: 6865 7920 7769 6c6c 2062 6520 7573 6564  hey will be used
+00016f60: 2074 6f20 636f 6e6e 6563 7420 746f 2074   to connect to t
+00016f70: 6865 2068 6f73 742e 0a49 6620 626f 7468  he host..If both
+00016f80: 2075 7365 7220 616e 6420 7061 7373 776f   user and passwo
+00016f90: 7264 2061 7265 202a 6e6f 742a 2064 6566  rd are *not* def
+00016fa0: 696e 6564 2069 6e20 7468 6520 636f 6e66  ined in the conf
+00016fb0: 6967 2c20 7468 6520 7365 7276 6963 6520  ig, the service 
+00016fc0: 7769 6c6c 2070 6172 7365 2074 6865 2075  will parse the u
+00016fd0: 7365 7227 730a 7373 6820 636f 6e66 6967  ser's.ssh config
+00016fe0: 2066 696c 6520 746f 2073 6565 2077 6869   file to see whi
+00016ff0: 6368 206b 6579 2028 4964 656e 7469 7479  ch key (Identity
+00017000: 4669 6c65 2920 746f 2075 7365 3b20 6974  File) to use; it
+00017010: 2077 696c 6c20 616c 736f 206c 6f6f 6b20   will also look 
+00017020: 666f 7220 5573 6572 2061 6e64 2050 6f72  for User and Por
+00017030: 740a 696e 2074 6869 7320 6669 6c65 2e0a  t.in this file..
+00017040: 0a49 6620 7573 696e 6720 6120 6b65 792c  .If using a key,
+00017050: 206f 6e6c 7920 7468 6520 686f 7374 2069   only the host i
+00017060: 7320 2a72 6571 7569 7265 642a 2e0a 0a54  s *required*...T
+00017070: 6865 206f 7574 7075 7420 6973 2069 676e  he output is ign
+00017080: 6f72 6564 2066 6f72 206e 6f77 2e0a 0a4e  ored for now...N
+00017090: 6f74 653a 2075 7369 6e67 2074 6869 7320  ote: using this 
+000170a0: 6d6f 6475 6c65 206c 6574 7320 796f 7520  module lets you 
+000170b0: 7370 6563 6966 7920 6120 7573 6572 6e61  specify a userna
+000170c0: 6d65 2061 6e64 2061 2070 6173 7377 6f72  me and a passwor
+000170d0: 6420 7768 6963 6820 6361 6e20 6265 2075  d which can be u
+000170e0: 7365 6420 746f 206c 6f67 696e 2074 6f20  sed to login to 
+000170f0: 7468 6520 7461 7267 6574 2073 7973 7465  the target syste
+00017100: 6d2e 2041 7320 7375 6368 2c20 796f 7572  m. As such, your
+00017110: 2060 6d71 7474 7761 726e 2e69 6e69 6020   `mqttwarn.ini` 
+00017120: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00017130: 6c65 2073 686f 756c 6420 6265 2077 656c  le should be wel
+00017140: 6c20 7072 6f74 6563 7465 6420 6672 6f6d  l protected from
+00017150: 2070 7279 696e 6720 6579 6573 2120 2854   prying eyes! (T
+00017160: 6869 7320 6170 706c 6965 7320 6765 6e65  his applies gene
+00017170: 7261 6c6c 792c 2066 6f72 206f 7468 6572  rally, for other
+00017180: 2074 6172 6765 7420 7370 6563 6966 6963   target specific
+00017190: 6174 696f 6e73 2077 6974 6820 6372 6564  ations with cred
+000171a0: 656e 7469 616c 7320 6173 2077 656c 6c2e  entials as well.
+000171b0: 290a 0a60 6060 696e 690a 5b63 6f6e 6669  )..```ini.[confi
+000171c0: 673a 7373 685d 0a68 6f73 7420 203d 2027  g:ssh].host  = '
+000171d0: 3139 322e 3136 382e 312e 3127 0a70 6f72  192.168.1.1'.por
+000171e0: 7420 203d 2032 320a 7573 6572 2020 3d20  t  = 22.user  = 
+000171f0: 2775 7365 726e 616d 6527 0a70 6173 7320  'username'.pass 
+00017200: 203d 2027 7061 7373 776f 7264 270a 7461   = 'password'.ta
+00017210: 7267 6574 7320 3d20 7b0a 0909 2773 3031  rgets = {...'s01
+00017220: 2720 2020 203a 205b 2027 636f 6d6d 616e  '    : [ 'comman
+00017230: 6420 7769 7468 206f 6e65 2073 7562 7374  d with one subst
+00017240: 6974 7574 696f 6e20 2573 2720 5d2c 0a09  itution %s' ],..
+00017250: 0927 7330 3227 2020 2020 3a20 5b20 2763  .'s02'    : [ 'c
+00017260: 6f6d 6d61 6e64 2077 6974 6820 7477 6f20  ommand with two 
+00017270: 7375 6273 7469 7475 7469 6f6e 7320 2573  substitutions %s
+00017280: 5f5f 2573 2720 5d0a 2020 2020 7d0a 0a5b  __%s' ].    }..[
+00017290: 7373 682f 2b5d 0a66 6f72 6d61 7420 3d20  ssh/+].format = 
+000172a0: 7b61 7267 737d 0a74 6172 6765 7473 203d  {args}.targets =
+000172b0: 2073 7368 3a73 3031 0a0a 5b64 7561 6c73   ssh:s01..[duals
+000172c0: 7368 2f2b 5d0a 666f 726d 6174 203d 207b  sh/+].format = {
+000172d0: 6172 6773 7d0a 7461 7267 6574 7320 3d20  args}.targets = 
+000172e0: 7373 683a 7330 320a 6060 600a 0a54 6172  ssh:s02.```..Tar
+000172f0: 6765 7473 206d 6179 2063 6f6e 7461 696e  gets may contain
+00017300: 204f 4e45 2063 6f6d 6d61 6e64 2e0a 0a60   ONE command...`
+00017310: 6d6f 7371 7569 7474 6f5f 7075 6220 2d74  mosquitto_pub -t
+00017320: 2064 7561 6c73 7368 2f74 6573 7420 2d6d   dualssh/test -m
+00017330: 2027 7b20 2261 7267 7322 203a 205b 2274   '{ "args" : ["t
+00017340: 6573 7422 2c22 7465 7374 3222 5d20 7d27  est","test2"] }'
+00017350: 600a 0a0a 2323 2320 6073 7973 6c6f 6760  `...### `syslog`
+00017360: 0a0a 5468 6520 6073 7973 6c6f 6760 2073  ..The `syslog` s
+00017370: 6572 7669 6365 2074 7261 6e73 6665 7273  ervice transfers
+00017380: 204d 5154 5420 6d65 7373 6167 6573 2074   MQTT messages t
+00017390: 6f20 6120 6c6f 6361 6c20 7379 736c 6f67  o a local syslog
+000173a0: 2073 6572 7665 722e 0a0a 6060 6069 6e69   server...```ini
+000173b0: 0a5b 636f 6e66 6967 3a73 7973 6c6f 675d  .[config:syslog]
+000173c0: 0a74 6172 6765 7473 203d 207b 0a20 2020  .targets = {.   
+000173d0: 2020 2020 2020 2020 2020 2023 2066 6163             # fac
+000173e0: 696c 6974 7920 2020 206f 7074 696f 6e0a  ility    option.
+000173f0: 2020 2020 2775 7365 7227 2020 203a 205b      'user'   : [
+00017400: 2775 7365 7227 2c20 2020 2020 2770 6964  'user',     'pid
+00017410: 275d 2c0a 2020 2020 276b 6572 6e65 6c27  '],.    'kernel'
+00017420: 203a 205b 276b 6572 6e65 6c27 2c20 2020   : ['kernel',   
+00017430: 2770 6964 275d 0a20 2020 207d 0a60 6060  'pid'].    }.```
+00017440: 0a0a 7c20 546f 7069 6320 6f70 7469 6f6e  ..| Topic option
+00017450: 2020 7c20 204d 2f4f 2020 207c 2044 6573    |  M/O   | Des
+00017460: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017480: 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d 2d2d      |.| --------
+00017490: 2d2d 2d2d 2d20 7c20 3a2d 2d2d 2d3a 207c  ----- | :----: |
+000174a0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000174b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000174c0: 2d2d 2d2d 2d2d 2d20 7c0a 7c20 6074 6974  ------- |.| `tit
+000174d0: 6c65 6020 2020 2020 2020 7c20 2020 4f20  le`       |   O 
+000174e0: 2020 207c 2061 7070 6c69 6361 7469 6f6e     | application
+000174f0: 2074 6974 6c65 2028 6466 6c74 3a20 606d   title (dflt: `m
+00017500: 7174 7477 6172 6e60 2920 2020 7c0a 7c20  qttwarn`)   |.| 
+00017510: 6070 7269 6f72 6974 7960 2020 2020 7c20  `priority`    | 
+00017520: 2020 4f20 2020 207c 206c 6f67 206c 6576    O    | log lev
+00017530: 656c 2028 6466 6c74 3a20 2d31 2920 2020  el (dflt: -1)   
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 7c0a 0a57 6865 7265 2060 7072 696f 7269  |..Where `priori
+00017560: 7479 6020 6361 6e20 6265 2062 6574 7765  ty` can be betwe
+00017570: 656e 202d 3220 616e 6420 3520 616e 6420  en -2 and 5 and 
+00017580: 6d61 7073 2074 6f20 6073 7973 6c6f 6760  maps to `syslog`
+00017590: 206c 6576 656c 7320 6279 3b0a 0a7c 2050   levels by;..| P
+000175a0: 7269 6f72 6974 7920 7c20 5379 736c 6f67  riority | Syslog
+000175b0: 204c 6f67 204c 6576 656c 207c 0a7c 202d   Log Level |.| -
+000175c0: 2d2d 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d  ------- | ------
+000175d0: 2d2d 2d2d 2d2d 2d2d 2d2d 207c 0a7c 202d  ---------- |.| -
+000175e0: 3220 2020 2020 2020 7c20 4c4f 475f 4445  2       | LOG_DE
+000175f0: 4255 4720 2020 2020 2020 207c 0a7c 202d  BUG        |.| -
+00017600: 3120 2020 2020 2020 7c20 4c4f 475f 494e  1       | LOG_IN
+00017610: 464f 2020 2020 2020 2020 207c 0a7c 2030  FO         |.| 0
+00017620: 2020 2020 2020 2020 7c20 4c4f 475f 4e4f          | LOG_NO
+00017630: 5449 4345 2020 2020 2020 207c 0a7c 2031  TICE       |.| 1
+00017640: 2020 2020 2020 2020 7c20 4c4f 475f 5741          | LOG_WA
+00017650: 524e 494e 4720 2020 2020 207c 0a7c 2032  RNING      |.| 2
+00017660: 2020 2020 2020 2020 7c20 4c4f 475f 4552          | LOG_ER
+00017670: 5220 2020 2020 2020 2020 207c 0a7c 2033  R          |.| 3
+00017680: 2020 2020 2020 2020 7c20 4c4f 475f 4352          | LOG_CR
+00017690: 4954 2020 2020 2020 2020 207c 0a7c 2034  IT         |.| 4
+000176a0: 2020 2020 2020 2020 7c20 4c4f 475f 414c          | LOG_AL
+000176b0: 4552 5420 2020 2020 2020 207c 0a7c 2035  ERT        |.| 5
+000176c0: 2020 2020 2020 2020 7c20 4c4f 475f 454d          | LOG_EM
+000176d0: 4552 4720 2020 2020 2020 207c 0a0a 6060  ERG        |..``
+000176e0: 600a 4170 7220 3232 2031 323a 3432 3a34  `.Apr 22 12:42:4
+000176f0: 3220 6d71 7474 6573 7430 3139 206d 7174  2 mqttest019 mqt
+00017700: 7477 6172 6e5b 3934 3834 5d3a 2044 6973  twarn[9484]: Dis
+00017710: 6b20 7574 696c 697a 6174 696f 6e3a 2039  k utilization: 9
+00017720: 3425 0a60 6060 0a0a 2323 2320 6074 656c  4%.```..### `tel
+00017730: 6567 7261 6d60 0a0a 5468 6973 2069 7320  egram`..This is 
+00017740: 746f 2073 656e 6420 6d65 7373 6167 6573  to send messages
+00017750: 2061 7320 6120 426f 7420 746f 2061 205b   as a Bot to a [
+00017760: 5465 6c65 6772 616d 5d28 6874 7470 733a  Telegram](https:
+00017770: 2f2f 7465 6c65 6772 616d 2e6f 7267 2920  //telegram.org) 
+00017780: 6368 6174 2e20 4669 7273 7420 7365 7420  chat. First set 
+00017790: 7570 2061 2042 6f74 2061 6e64 206f 6274  up a Bot and obt
+000177a0: 6169 6e20 6974 7320 6175 7468 656e 7469  ain its authenti
+000177b0: 6361 7469 6f6e 2074 6f6b 656e 2077 6869  cation token whi
+000177c0: 6368 2079 6f75 2061 6464 2074 6f20 5f6d  ch you add to _m
+000177d0: 7174 7477 6172 6e5f 2773 2063 6f6e 6669  qttwarn_'s confi
+000177e0: 6775 7261 7469 6f6e 2e20 596f 7527 6c6c  guration. You'll
+000177f0: 2061 6c73 6f20 6e65 6564 2074 6f20 7374   also need to st
+00017800: 6172 7420 6120 6368 6174 2077 6974 6820  art a chat with 
+00017810: 7468 6973 2062 6f74 2073 6f20 6974 2773  this bot so it's
+00017820: 2061 626c 6520 746f 2063 6f6d 6d75 6e69   able to communi
+00017830: 6361 7465 2077 6974 6820 7061 7274 6963  cate with partic
+00017840: 756c 6172 2075 7365 722e 0a0a 4f70 7469  ular user...Opti
+00017850: 6f6e 616c 6c79 2079 6f75 2063 616e 2073  onally you can s
+00017860: 7065 6369 6679 2060 7061 7273 655f 6d6f  pecify `parse_mo
+00017870: 6465 6020 7768 6963 6820 7769 6c6c 2062  de` which will b
+00017880: 6520 7573 6564 2064 7572 696e 6720 6d65  e used during me
+00017890: 7373 6167 6520 7365 6e64 696e 672e 2050  ssage sending. P
+000178a0: 6c65 6173 652c 2063 6865 636b 205b 646f  lease, check [do
+000178b0: 6373 5d28 6874 7470 733a 2f2f 636f 7265  cs](https://core
+000178c0: 2e74 656c 6567 7261 6d2e 6f72 672f 626f  .telegram.org/bo
+000178d0: 7473 2f61 7069 2366 6f72 6d61 7474 696e  ts/api#formattin
+000178e0: 672d 6f70 7469 6f6e 7329 2066 6f72 2061  g-options) for a
+000178f0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
+00017900: 6174 696f 6e2e 0a0a 4966 2079 6f75 2068  ation...If you h
+00017910: 6176 6520 7468 6520 6063 6861 7449 6460  ave the `chatId`
+00017920: 2079 6f75 2063 616e 2073 7065 6369 6679   you can specify
+00017930: 2074 6865 2074 656c 6567 7261 6d20 7365   the telegram se
+00017940: 7276 6963 6520 746f 2075 7365 2074 6865  rvice to use the
+00017950: 2063 6861 7449 6420 6469 7265 6374 6c79   chatId directly
+00017960: 2e20 5761 726e 696e 672c 2074 6869 7320  . Warning, this 
+00017970: 7769 6c6c 206e 6565 6420 746f 2062 6520  will need to be 
+00017980: 7468 6520 6361 7365 2066 6f72 2061 6c6c  the case for all
+00017990: 2074 6865 2074 6172 6765 7473 2069 6e20   the targets in 
+000179a0: 7468 6973 206e 6f74 6966 6965 7221 0a0a  this notifier!..
+000179b0: 5175 6963 6b65 7374 2077 6179 2074 6f20  Quickest way to 
+000179c0: 6765 7420 7468 6520 6063 6861 7469 6460  get the `chatid`
+000179d0: 2069 7320 6279 2076 6973 6974 696e 6720   is by visiting 
+000179e0: 7468 6973 2055 524c 2028 696e 7365 7274  this URL (insert
+000179f0: 2079 6f75 7220 6170 6920 6b65 7929 3a20   your api key): 
+00017a00: 6874 7470 733a 2f2f 6170 692e 7465 6c65  https://api.tele
+00017a10: 6772 616d 2e6f 7267 2f62 6f74 594f 5552  gram.org/botYOUR
+00017a20: 5f41 5049 5f54 4f4b 454e 2f67 6574 5570  _API_TOKEN/getUp
+00017a30: 6461 7465 7320 616e 6420 6765 7474 696e  dates and gettin
+00017a40: 6720 7468 6520 6964 2066 726f 6d20 7468  g the id from th
+00017a50: 6520 2266 726f 6d22 2073 6563 7469 6f6e  e "from" section
+00017a60: 2e0a 0a43 6f6e 6669 6775 7265 2074 6865  ...Configure the
+00017a70: 2060 7465 6c65 6772 616d 6020 7365 7276   `telegram` serv
+00017a80: 6963 6520 5749 5448 4f55 5420 6368 6174  ice WITHOUT chat
+00017a90: 4964 3a0a 0a60 6060 696e 690a 5b63 6f6e  Id:..```ini.[con
+00017aa0: 6669 673a 7465 6c65 6772 616d 5d0a 7469  fig:telegram].ti
+00017ab0: 6d65 6f75 7420 3d20 3630 0a70 6172 7365  meout = 60.parse
+00017ac0: 5f6d 6f64 6520 3d20 274d 6172 6b64 6f77  _mode = 'Markdow
+00017ad0: 6e27 0a74 6f6b 656e 203d 2027 6d6d 6d6d  n'.token = 'mmmm
+00017ae0: 6d6d 6d6d 6d3a 4141 4141 4141 4141 4141  mmmmm:AAAAAAAAAA
+00017af0: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
+00017b00: 4141 4141 4141 4141 4127 0a74 6172 6765  AAAAAAAAA'.targe
+00017b10: 7473 203d 207b 0a20 2020 2320 2020 2020  ts = {.   #     
+00017b20: 2020 2046 6972 7374 204e 616d 6520 6f72     First Name or
+00017b30: 2040 7573 6572 6e61 6d65 206f 7220 2363   @username or #c
+00017b40: 6861 745f 6964 0a20 2020 276a 3031 2720  hat_id.   'j01' 
+00017b50: 3a20 5b20 2746 6972 7374 204e 616d 6527  : [ 'First Name'
+00017b60: 205d 2c0a 2020 2027 6a30 3227 203a 205b   ],.   'j02' : [
+00017b70: 2027 4075 7365 726e 616d 6527 205d 2c0a   '@username' ],.
+00017b80: 2020 2027 6a30 3327 203a 205b 2027 2363     'j03' : [ '#c
+00017b90: 6861 745f 6964 2720 5d0a 2020 2020 7d0a  hat_id' ].    }.
+00017ba0: 6060 600a 436f 6e66 6967 7572 6520 7468  ```.Configure th
+00017bb0: 6520 6074 656c 6567 7261 6d60 2073 6572  e `telegram` ser
+00017bc0: 7669 6365 2057 4954 4820 6368 6174 6964  vice WITH chatid
+00017bd0: 3a0a 6060 6069 6e69 0a5b 636f 6e66 6967  :.```ini.[config
+00017be0: 3a74 656c 6567 7261 6d5d 0a74 696d 656f  :telegram].timeo
+00017bf0: 7574 203d 2036 300a 7061 7273 655f 6d6f  ut = 60.parse_mo
+00017c00: 6465 203d 2027 4d61 726b 646f 776e 270a  de = 'Markdown'.
+00017c10: 746f 6b65 6e20 3d20 276d 6d6d 6d6d 6d6d  token = 'mmmmmmm
+00017c20: 6d6d 3a41 4141 4141 4141 4141 4141 4141  mm:AAAAAAAAAAAAA
+00017c30: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
+00017c40: 4141 4141 4141 270a 7573 655f 6368 6174  AAAAAA'.use_chat
+00017c50: 5f69 6420 3d20 5472 7565 0a74 6172 6765  _id = True.targe
+00017c60: 7473 203d 207b 0a20 2020 2023 2020 2020  ts = {.    #    
+00017c70: 2020 2063 6861 7449 6420 2869 6e20 7175     chatId (in qu
+00017c80: 6f74 6573 290a 2020 2020 276a 3031 2720  otes).    'j01' 
+00017c90: 3a20 5b27 3132 3334 3536 3738 3927 5d0a  : ['123456789'].
+00017ca0: 2020 2020 7d0a 6060 600a 0a50 6f73 7369      }.```..Possi
+00017cb0: 626c 6520 6973 7375 653a 0a0a 2a20 4966  ble issue:..* If
+00017cc0: 2046 6972 7374 206e 616d 6520 6f72 2040   First name or @
+00017cd0: 7573 6572 6e61 6d65 2077 6173 2073 7065  username was spe
+00017ce0: 6369 6669 6564 2061 7320 7461 7267 6574  cified as target
+00017cf0: 2c20 706c 7567 696e 2077 696c 6c20 6361  , plugin will ca
+00017d00: 6c6c 205b 6765 7455 7064 6174 6573 5d28  ll [getUpdates](
+00017d10: 6874 7470 733a 2f2f 636f 7265 2e74 656c  https://core.tel
+00017d20: 6567 7261 6d2e 6f72 672f 626f 7473 2f61  egram.org/bots/a
+00017d30: 7069 2367 6574 7570 6461 7465 7329 2074  pi#getupdates) t
+00017d40: 6f20 6765 7420 6063 6861 745f 6964 6020  o get `chat_id` 
+00017d50: 6275 7420 7468 6973 2063 616c 6c20 7265  but this call re
+00017d60: 7475 726e 7320 6f6e 6c79 206c 6173 7420  turns only last 
+00017d70: 3130 3020 6d65 7373 6167 6573 3b20 6966  100 messages; if
+00017d80: 205f 796f 755f 2068 6176 656e 2774 2073   _you_ haven't s
+00017d90: 706f 6b65 6e20 746f 2079 6f75 7220 426f  poken to your Bo
+00017da0: 7420 7265 6365 6e74 6c79 2069 7420 6d61  t recently it ma
+00017db0: 7920 7765 6c6c 2062 6520 706f 7373 6962  y well be possib
+00017dc0: 6c65 2077 6520 6361 6e27 7420 6669 6e64  le we can't find
+00017dd0: 2074 6865 205f 6368 6174 2d69 645f 2061   the _chat-id_ a
+00017de0: 7373 6f63 6961 7465 6420 7769 7468 205f  ssociated with _
+00017df0: 796f 755f 2e20 4966 2063 6861 745f 6964  you_. If chat_id
+00017e00: 2069 7320 6b6e 6f77 6e2c 2069 7420 6361   is known, it ca
+00017e10: 6e20 6265 2073 6574 2061 7320 7461 7267  n be set as targ
+00017e20: 6574 2075 7369 6e67 2060 2360 2073 6967  et using `#` sig
+00017e30: 6e2e 0a0a 215b 5465 6c65 6772 616d 5d28  n...![Telegram](
+00017e40: 6173 7365 7473 2f74 656c 6567 7261 6d2e  assets/telegram.
+00017e50: 706e 6729 0a0a 2323 2320 6074 6869 6e67  png)..### `thing
+00017e60: 7370 6561 6b60 0a0a 5468 6520 6074 6869  speak`..The `thi
+00017e70: 6e67 7370 6561 6b60 2073 6572 7669 6365  ngspeak` service
+00017e80: 2070 7562 6c69 7368 6573 2064 6174 6120   publishes data 
+00017e90: 746f 2074 6869 6e67 7370 6561 6b2e 636f  to thingspeak.co
+00017ea0: 6d20 7573 696e 6720 7468 6520 7468 696e  m using the thin
+00017eb0: 6773 7065 616b 2041 5049 2e0a 0a60 6060  gspeak API...```
+00017ec0: 696e 690a 5b63 6f6e 6669 673a 7468 696e  ini.[config:thin
+00017ed0: 6773 7065 616b 5d0a 7461 7267 6574 7320  gspeak].targets 
+00017ee0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00017ef0: 2020 2020 2020 2023 4150 4920 5752 4954         #API WRIT
+00017f00: 4520 4b45 5920 2020 2020 2020 6669 656c  E KEY       fiel
+00017f10: 6420 2020 2020 206f 7074 696f 6e61 6c20  d      optional 
+00017f20: 6275 696c 6464 6174 613d 7472 7565 2f66  builddata=true/f
+00017f30: 616c 7365 0a20 2020 2027 6669 656c 6431  alse.    'field1
+00017f40: 2720 2020 3a20 5b20 2758 5859 595a 5a58  '   : [ 'XXYYZZX
+00017f50: 5859 595a 5a58 5859 5927 2c20 2766 6965  XYYZZXXYY', 'fie
+00017f60: 6c64 3127 202c 2027 7472 7565 2720 5d2c  ld1' , 'true' ],
+00017f70: 0a20 2020 2027 6669 656c 6432 2720 2020  .    'field2'   
+00017f80: 3a20 5b20 2758 5859 595a 5a58 5859 595a  : [ 'XXYYZZXXYYZ
+00017f90: 5a58 5859 5927 2c20 2766 6965 6c64 3227  ZXXYY', 'field2'
+00017fa0: 205d 2c0a 2020 2020 2763 6f6d 706f 7369   ],.    'composi
+00017fb0: 7465 273a 205b 2027 5858 5959 5a5a 5858  te': [ 'XXYYZZXX
+00017fc0: 5959 5a5a 5858 5959 272c 205b 2027 7465  YYZZXXYY', [ 'te
+00017fd0: 6d70 272c 2027 6875 6d27 205d 205d 0a20  mp', 'hum' ] ]. 
+00017fe0: 207d 0a60 6060 0a55 7369 6e67 2060 6275   }.```.Using `bu
+00017ff0: 696c 6464 6174 613d 7472 7565 6020 796f  ilddata=true` yo
+00018000: 7520 6361 6e20 6275 696c 6420 616e 2075  u can build an u
+00018010: 7064 6174 6520 7769 7468 206d 756c 7469  pdate with multi
+00018020: 706c 6520 6669 656c 6473 2069 6e20 6f6e  ple fields in on
+00018030: 6520 7570 6461 7465 2e20 5573 696e 6720  e update. Using 
+00018040: 7468 6973 2066 756e 6374 696f 6e20 6e6f  this function no
+00018050: 2064 6972 6563 7420 7570 6461 7465 2069   direct update i
+00018060: 7320 7065 7266 6f72 6d65 642e 204f 6e6c  s performed. Onl
+00018070: 7920 7769 7468 2074 6865 206e 6578 7420  y with the next 
+00018080: 7570 6461 7465 2077 6974 686f 7574 2062  update without b
+00018090: 7569 6c64 6461 7461 3d74 7275 6520 616c  uilddata=true al
+000180a0: 6c20 656e 7472 6965 7320 6172 6520 7365  l entries are se
+000180b0: 6e74 2028 652e 672e 2077 6865 6e20 6d75  nt (e.g. when mu
+000180c0: 6c74 6970 6c65 2073 656e 736f 7273 2061  ltiple sensors a
+000180d0: 7265 2075 7064 6174 696e 6720 6469 6666  re updating diff
+000180e0: 6572 656e 7420 746f 7069 6373 2c20 7468  erent topics, th
+000180f0: 656e 2079 6f75 2063 616e 2064 6f20 7468  en you can do th
+00018100: 6520 6275 696c 6420 7468 6520 6461 7461  e build the data
+00018110: 2061 6e64 2073 7562 6d69 7420 7768 656e   and submit when
+00018120: 2074 6865 206c 6173 7420 7365 6e73 6f72   the last sensor
+00018130: 2069 7320 7365 6e64 696e 6720 7468 6520   is sending the 
+00018140: 6461 7461 292e 0a0a 5375 7070 6c79 2061  data)...Supply a
+00018150: 6e20 6f72 6465 7265 6420 6c69 7374 206f  n ordered list o
+00018160: 6620 6d65 7373 6167 6520 6461 7461 2066  f message data f
+00018170: 6965 6c64 206e 616d 6573 2074 6f20 6578  ield names to ex
+00018180: 7472 6163 7420 7365 7665 7261 6c20 7661  tract several va
+00018190: 6c75 6573 2066 726f 6d20 6120 7369 6e67  lues from a sing
+000181a0: 6c65 206d 6573 7361 6765 2028 652e 672e  le message (e.g.
+000181b0: 2060 7b20 2274 656d 7022 3a20 3130 2c20   `{ "temp": 10, 
+000181c0: 2268 756d 223a 2037 3720 7d60 292e 2056  "hum": 77 }`). V
+000181d0: 616c 7565 7320 7769 6c6c 2062 6520 6173  alues will be as
+000181e0: 7369 676e 6564 2074 6f20 6669 656c 6431  signed to field1
+000181f0: 2c20 6669 656c 6432 2c20 6574 6320 696e  , field2, etc in
+00018200: 206f 7264 6572 2e0a 0a4e 6f74 653a 2055   order...Note: U
+00018210: 7365 2074 6865 2066 6965 6c64 2061 7320  se the field as 
+00018220: 7065 7220 7468 6520 6578 616d 706c 6520  per the example 
+00018230: 286c 6f77 6572 2063 6173 652c 2060 2766  (lower case, `'f
+00018240: 6965 6c64 3127 6020 7769 7468 2074 6865  ield1'` with the
+00018250: 206c 6173 7420 6469 6769 7420 6265 696e   last digit bein
+00018260: 6720 7468 6520 6669 656c 6420 6e75 6d62  g the field numb
+00018270: 6572 292e 0a0a 2323 2320 6074 6f6f 7470  er)...### `tootp
+00018280: 6173 7465 600a 0a54 6865 2060 746f 6f74  aste`..The `toot
+00018290: 7061 7374 6560 2073 6572 7669 6365 2069  paste` service i
+000182a0: 7320 666f 7220 706f 7374 696e 6720 746f  s for posting to
+000182b0: 2074 6865 205b 4d61 7374 6f64 6f6e 2073   the [Mastodon s
+000182c0: 6f63 6961 6c20 6e65 7477 6f72 6b5d 2868  ocial network](h
+000182d0: 7474 7073 3a2f 2f6d 6173 746f 646f 6e2e  ttps://mastodon.
+000182e0: 736f 6369 616c 2f61 626f 7574 292e 0a0a  social/about)...
+000182f0: 6060 6069 6e69 0a5b 636f 6e66 6967 3a74  ```ini.[config:t
+00018300: 6f6f 7470 6173 7465 5d0a 7461 7267 6574  ootpaste].target
+00018310: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00018320: 2020 2023 2063 6c69 656e 7463 7265 6473     # clientcreds
+00018330: 2c20 7573 6572 6372 6564 732c 2062 6173  , usercreds, bas
+00018340: 655f 7572 6c0a 2020 2020 2775 6e6f 2720  e_url.    'uno' 
+00018350: 203a 205b 2027 612e 636c 6965 6e74 272c   : [ 'a.client',
+00018360: 2020 2761 2e75 7365 7227 2c20 2768 7474    'a.user', 'htt
+00018370: 7073 3a2f 2f6d 6173 746f 2e69 6f27 205d  ps://masto.io' ]
+00018380: 2c0a 2020 7d0a 6060 600a 0a54 6865 2073  ,.  }.```..The s
+00018390: 7065 6369 6669 6564 2060 636c 6965 6e74  pecified `client
+000183a0: 6372 6564 7360 2061 6e64 2060 7573 6572  creds` and `user
+000183b0: 6372 6564 7360 2061 7265 2070 6174 6873  creds` are paths
+000183c0: 2074 6f20 6669 6c65 7320 6372 6561 7465   to files create
+000183d0: 6420 7769 7468 2074 6865 2073 6572 7669  d with the servi
+000183e0: 6365 2c20 6173 2066 6f6c 6c6f 7773 3a0a  ce, as follows:.
+000183f0: 0a60 6060 0a70 7974 686f 6e20 7365 7276  .```.python serv
+00018400: 6963 6573 2f74 6f6f 7470 6173 7465 2e70  ices/tootpaste.p
+00018410: 7920 2768 7474 7073 3a2f 2f6d 6173 746f  y 'https://masto
+00018420: 2e69 6f27 2027 6a61 6e65 4065 7861 6d70  .io' 'jane@examp
+00018430: 6c65 2e6f 7267 2720 2778 6166 6135 3238  le.org' 'xafa528
+00018440: 3038 3930 2720 7761 726e 6d65 2073 7530  0890' warnme su0
+00018450: 332d 612e 636c 6965 6e74 2073 7530 332d  3-a.client su03-
+00018460: 612e 7573 6572 0a60 6060 0a0a 5468 6520  a.user.```..The 
+00018470: 6172 6775 6d65 6e74 732c 2069 6e20 6f72  arguments, in or
+00018480: 6465 723a 0a0a 312e 2062 6173 6520 5552  der:..1. base UR
+00018490: 4c20 2865 2e67 2e20 6068 7474 7073 3a2f  L (e.g. `https:/
+000184a0: 2f6d 6173 746f 646f 6e2e 736f 6369 616c  /mastodon.social
+000184b0: 6029 0a32 2e20 796f 7572 2065 2d6d 6169  `).2. your e-mai
+000184c0: 6c20 6164 6472 6573 730a 332e 2074 6865  l address.3. the
+000184d0: 2070 6173 7377 6f72 6420 636f 7272 6573   password corres
+000184e0: 706f 6e64 696e 6720 746f 2074 6865 2065  ponding to the e
+000184f0: 2d6d 6169 6c20 6164 6472 6573 730a 342e  -mail address.4.
+00018500: 2074 6865 2063 6c69 656e 7420 6e61 6d65   the client name
+00018510: 2028 6e61 6d65 206f 6620 7468 6520 706f   (name of the po
+00018520: 7374 696e 6720 7072 6f67 7261 6d29 0a35  sting program).5
+00018530: 2e20 7468 6520 636c 6965 6e74 6372 6564  . the clientcred
+00018540: 7320 6669 6c65 0a36 2e20 7468 6520 7573  s file.6. the us
+00018550: 6572 6372 6564 7320 6669 6c65 2e0a 0a54  ercreds file...T
+00018560: 6865 2074 776f 206c 6173 7420 6669 6c65  he two last file
+00018570: 7320 6172 6520 6372 6561 7465 6420 616e  s are created an
+00018580: 6420 7368 6f75 6c64 2062 6520 7072 6f74  d should be prot
+00018590: 6563 7465 6420 6672 6f6d 2070 7279 696e  ected from pryin
+000185a0: 6720 6579 6573 2e0a 0a21 5b74 6f6f 7470  g eyes...![tootp
+000185b0: 6173 7465 2028 4d61 7374 6f64 6f6e 295d  aste (Mastodon)]
+000185c0: 2861 7373 6574 732f 746f 6f74 7061 7374  (assets/tootpast
+000185d0: 652e 706e 6729 0a0a 6074 6f6f 7470 6173  e.png)..`tootpas
+000185e0: 7465 6020 7265 7175 6972 6573 2061 2060  te` requires a `
+000185f0: 7069 7020 696e 7374 616c 6c20 4d61 7374  pip install Mast
+00018600: 6f64 6f6e 2e70 7960 2028 5b4d 6173 746f  odon.py` ([Masto
+00018610: 646f 6e2e 7079 5d28 6874 7470 733a 2f2f  don.py](https://
+00018620: 6769 7468 7562 2e63 6f6d 2f68 616c 6379  github.com/halcy
+00018630: 2f4d 6173 746f 646f 6e2e 7079 2929 2e0a  /Mastodon.py))..
+00018640: 0a23 2323 2060 7477 696c 696f 600a 0a60  .### `twilio`..`
+00018650: 6060 696e 690a 5b63 6f6e 6669 673a 7477  ``ini.[config:tw
+00018660: 696c 696f 5d0a 7461 7267 6574 7320 3d20  ilio].targets = 
+00018670: 7b0a 2020 2020 2020 2020 2020 2020 2023  {.             #
+00018680: 2041 6363 6f75 6e74 2053 4944 2020 2020   Account SID    
+00018690: 2020 2020 2020 2020 4175 7468 2054 6f6b          Auth Tok
+000186a0: 656e 2020 2020 2020 2020 2020 2020 6672  en            fr
+000186b0: 6f6d 2020 2020 2020 2020 2020 2020 2020  om              
+000186c0: 746f 0a20 2020 2768 6f6c 6127 2020 3a20  to.   'hola'  : 
+000186d0: 5b20 2741 4358 5858 5858 5858 5858 5858  [ 'ACXXXXXXXXXXX
+000186e0: 5858 5858 5858 272c 2027 5959 5959 5959  XXXXXX', 'YYYYYY
+000186f0: 5959 5959 5959 5959 5959 5959 272c 2022  YYYYYYYYYYYY', "
+00018700: 2b31 3531 3035 3535 3132 3334 222c 2020  +15105551234",  
+00018710: 222b 3132 3132 3535 3531 3233 3422 205d  "+12125551234" ]
+00018720: 0a20 2020 7d0a 6060 600a 0a21 5b54 7769  .   }.```..![Twi
+00018730: 6c69 6f20 7465 7374 5d28 6173 7365 7473  lio test](assets
+00018740: 2f74 7769 6c6c 696f 2e6a 7067 290a 0a52  /twillio.jpg)..R
+00018750: 6571 7569 7265 733a 0a20 2a20 6120 5477  equires:. * a Tw
+00018760: 696c 696f 2061 6363 6f75 6e74 0a20 2a20  ilio account. * 
+00018770: 5b74 7769 6c69 6f2d 7079 7468 6f6e 5d28  [twilio-python](
+00018780: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00018790: 6f6d 2f74 7769 6c69 6f2f 7477 696c 696f  om/twilio/twilio
+000187a0: 2d70 7974 686f 6e29 0a0a 2323 2320 6074  -python)..### `t
+000187b0: 7769 7474 6572 600a 0a4e 6f74 6966 6963  witter`..Notific
+000187c0: 6174 696f 6e20 6f66 206f 6e65 206f 7220  ation of one or 
+000187d0: 6d6f 7265 205b 5477 6974 7465 725d 2868  more [Twitter](h
+000187e0: 7474 703a 2f2f 7477 6974 7465 722e 636f  ttp://twitter.co
+000187f0: 6d29 2061 6363 6f75 6e74 7320 7265 7175  m) accounts requ
+00018800: 6972 6573 2073 6574 7469 6e67 0a75 7020  ires setting.up 
+00018810: 616e 2061 7070 6c69 6361 7469 6f6e 2061  an application a
+00018820: 7420 5b61 7070 732e 7477 6974 7465 722e  t [apps.twitter.
+00018830: 636f 6d5d 2868 7474 7073 3a2f 2f61 7070  com](https://app
+00018840: 732e 7477 6974 7465 722e 636f 6d29 2e20  s.twitter.com). 
+00018850: 466f 7220 6561 6368 2054 7769 7474 6572  For each Twitter
+00018860: 0a61 6363 6f75 6e74 2c20 796f 7520 6e65  .account, you ne
+00018870: 6564 2066 6f75 7220 2834 2920 6269 7473  ed four (4) bits
+00018880: 2077 6869 6368 2061 7265 206e 616d 6564   which are named
+00018890: 2061 7320 7368 6f77 6e20 6265 6c6f 772e   as shown below.
+000188a0: 0a0a 5570 6f6e 2063 6f6e 6669 6775 7269  ..Upon configuri
+000188b0: 6e67 2074 6869 7320 7365 7276 6963 6527  ng this service'
+000188c0: 7320 7461 7267 6574 732c 206d 616b 6520  s targets, make 
+000188d0: 7375 7265 2074 6865 2066 6f75 7220 2834  sure the four (4
+000188e0: 2920 656c 656d 656e 7473 206f 6620 7468  ) elements of th
+000188f0: 650a 6c69 7374 2061 7265 2069 6e20 7468  e.list are in th
+00018900: 6520 6f72 6465 7220 7370 6563 6966 6965  e order specifie
+00018910: 6421 0a0a 6060 6069 6e69 0a5b 636f 6e66  d!..```ini.[conf
+00018920: 6967 3a74 7769 7474 6572 5d0a 7461 7267  ig:twitter].targ
+00018930: 6574 7320 3d20 7b0a 2020 276a 616e 656a  ets = {.  'janej
+00018940: 6f6c 2720 2020 3a20 205b 2027 7676 7676  ol'   :  [ 'vvvv
+00018950: 7676 7676 7676 7676 7676 7676 7676 7676  vvvvvvvvvvvvvvvv
+00018960: 7676 272c 2020 2020 2020 2020 2020 2020  vv',            
+00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018980: 2020 2320 636f 6e73 756d 6572 5f6b 6579    # consumer_key
+00018990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000189a0: 2020 2020 2777 7777 7777 7777 7777 7777      'wwwwwwwwwww
+000189b0: 7777 7777 7777 7777 7777 7777 7777 7777  wwwwwwwwwwwwwwww
+000189c0: 7777 7777 7777 7777 7777 7777 7777 7727  wwwwwwwwwwwwwww'
+000189d0: 2c20 2020 2020 2020 2020 2023 2063 6f6e  ,          # con
+000189e0: 7375 6d65 725f 7365 6372 6574 0a20 2020  sumer_secret.   
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 2778 7878 7878 7878 7878 7878 7878 7878  'xxxxxxxxxxxxxxx
+00018a10: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
+00018a20: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
+00018a30: 7878 7827 2c20 2023 2061 6363 6573 735f  xxx',  # access_
+00018a40: 746f 6b65 6e5f 6b65 790a 2020 2020 2020  token_key.      
+00018a50: 2020 2020 2020 2020 2020 2020 2027 7a7a               'zz
+00018a60: 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a  zzzzzzzzzzzzzzzz
+00018a70: 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a 7a7a  zzzzzzzzzzzzzzzz
+00018a80: 7a7a 7a7a 7a7a 7a7a 2720 2020 2020 2020  zzzzzzzz'       
+00018a90: 2020 2020 2320 6163 6365 7373 5f74 6f6b      # access_tok
+00018aa0: 656e 5f73 6563 7265 740a 2020 2020 2020  en_secret.      
+00018ab0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00018ac0: 207d 0a60 6060 0a0a 215b 6120 7477 6565   }.```..![a twee
+00018ad0: 745d 2861 7373 6574 732f 7477 6974 7465  t](assets/twitte
+00018ae0: 722e 6a70 6729 0a0a 5265 7175 6972 6573  r.jpg)..Requires
+00018af0: 3a0a 2a20 4120 5477 6974 7465 7220 6163  :.* A Twitter ac
+00018b00: 636f 756e 740a 2a20 6170 7020 6b65 7973  count.* app keys
+00018b10: 2066 6f72 2054 7769 7474 6572 2c20 6672   for Twitter, fr
+00018b20: 6f6d 205b 6170 7073 2e74 7769 7474 6572  om [apps.twitter
+00018b30: 2e63 6f6d 5d28 6874 7470 733a 2f2f 6170  .com](https://ap
+00018b40: 7073 2e74 7769 7474 6572 2e63 6f6d 290a  ps.twitter.com).
+00018b50: 2a20 5b70 7974 686f 6e2d 7477 6974 7465  * [python-twitte
+00018b60: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00018b70: 622e 636f 6d2f 6265 6172 2f70 7974 686f  b.com/bear/pytho
+00018b80: 6e2d 7477 6974 7465 7229 0a0a 2323 2320  n-twitter)..### 
+00018b90: 6077 6562 736f 636b 6574 600a 0a54 6865  `websocket`..The
+00018ba0: 2077 6562 736f 636b 6574 2073 6572 7669   websocket servi
+00018bb0: 6365 2063 616e 2062 6520 7573 6564 2074  ce can be used t
+00018bc0: 6f20 7365 6e64 2064 6174 6120 746f 2061  o send data to a
+00018bd0: 2077 6562 736f 636b 6574 2073 6572 7665   websocket serve
+00018be0: 7220 6465 6669 6e65 6420 6279 2069 7473  r defined by its
+00018bf0: 2075 7269 2e20 6077 733a 2f2f 6020 6f72   uri. `ws://` or
+00018c00: 2060 7773 733a 2f2f 6020 7363 6865 6d61   `wss://` schema
+00018c10: 730a 6172 6520 7375 7070 6f72 7465 642e  s.are supported.
+00018c20: 0a0a 6060 6069 6e69 0a5b 636f 6e66 6967  ..```ini.[config
+00018c30: 3a77 6562 736f 636b 6574 5d0a 7461 7267  :websocket].targ
+00018c40: 6574 7320 3d20 7b0a 2020 2020 2020 2020  ets = {.        
+00018c50: 2320 7461 7267 6574 6964 2020 2020 2020  # targetid      
+00018c60: 2020 3a20 5b20 2777 7375 7269 275d 0a20    : [ 'wsuri']. 
+00018c70: 2020 2020 2020 2027 7773 7373 6572 7665         'wssserve
+00018c80: 7227 203a 205b 2027 7773 3a2f 2f6c 6f63  r' : [ 'ws://loc
+00018c90: 616c 686f 7374 2f77 7327 205d 2c0a 7d20  alhost/ws' ],.} 
+00018ca0: 0a60 6060 0a0a 5265 7175 6972 6573 3a0a  .```..Requires:.
+00018cb0: 2a20 5b77 6562 736f 636b 6574 2d63 6c69  * [websocket-cli
+00018cc0: 656e 745d 2868 7474 7073 3a2f 2f70 7970  ent](https://pyp
+00018cd0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+00018ce0: 692f 7765 6273 6f63 6b65 742d 636c 6965  i/websocket-clie
+00018cf0: 6e74 2f29 202d 2070 6970 2069 6e73 7461  nt/) - pip insta
+00018d00: 6c6c 2077 6562 736f 636b 6574 2d63 6c69  ll websocket-cli
+00018d10: 656e 740a 0a23 2323 2060 7862 6d63 600a  ent..### `xbmc`.
+00018d20: 0a54 6869 7320 7365 7276 6963 6520 616c  .This service al
+00018d30: 6c6f 7773 2066 6f72 206f 6e2d 7363 7265  lows for on-scre
+00018d40: 656e 206e 6f74 6966 6963 6174 696f 6e20  en notification 
+00018d50: 706f 702d 7570 7320 6f6e 205b 5842 4d43  pop-ups on [XBMC
+00018d60: 5d28 6874 7470 3a2f 2f78 626d 632e 6f72  ](http://xbmc.or
+00018d70: 672f 2920 696e 7374 616e 6365 732e 2045  g/) instances. E
+00018d80: 6163 6820 7461 7267 6574 2072 6571 7569  ach target requi
+00018d90: 7265 730a 7468 6520 6164 6472 6573 7320  res.the address 
+00018da0: 616e 6420 706f 7274 206f 6620 7468 6520  and port of the 
+00018db0: 5842 4d43 2069 6e73 7461 6e63 6520 283c  XBMC instance (<
+00018dc0: 686f 7374 6e61 6d65 3e3a 3c70 6f72 743e  hostname>:<port>
+00018dd0: 292c 2061 6e64 2061 6e20 6f70 7469 6f6e  ), and an option
+00018de0: 616c 2075 7365 726e 616d 6520 616e 6420  al username and 
+00018df0: 7061 7373 776f 7264 2069 6620 6175 7468  password if auth
+00018e00: 656e 7469 6361 7469 6f6e 2069 7320 7265  entication is re
+00018e10: 7175 6972 6564 2e0a 0a60 6060 696e 690a  quired...```ini.
+00018e20: 5b63 6f6e 6669 673a 7862 6d63 5d0a 7461  [config:xbmc].ta
+00018e30: 7267 6574 7320 3d20 7b0a 2020 2020 2020  rgets = {.      
+00018e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e50: 2020 2020 2320 686f 7374 3a70 6f72 742c      # host:port,
+00018e60: 2020 2020 2020 2020 2020 205b 7573 6572             [user
+00018e70: 5d2c 205b 7061 7373 776f 7264 5d0a 2020  ], [password].  
+00018e80: 2020 276c 6976 696e 675f 7769 7468 5f61    'living_with_a
+00018e90: 7574 6827 203a 2020 5b20 2731 3932 2e31  uth' :  [ '192.1
+00018ea0: 3638 2e31 2e34 303a 3830 3830 272c 2027  68.1.40:8080', '
+00018eb0: 7862 6d63 272c 2027 7862 6d63 2720 5d2c  xbmc', 'xbmc' ],
+00018ec0: 0a20 2020 2027 6265 6472 6f6f 6d5f 6e6f  .    'bedroom_no
+00018ed0: 5f61 7574 6827 2020 3a20 205b 2027 3139  _auth'  :  [ '19
+00018ee0: 322e 3136 382e 312e 3431 3a38 3038 3027  2.168.1.41:8080'
+00018ef0: 205d 0a20 2020 207d 0a60 6060 0a0a 7c20   ].    }.```..| 
+00018f00: 546f 7069 6320 6f70 7469 6f6e 2020 7c20  Topic option  | 
+00018f10: 204d 2f4f 2020 207c 2044 6573 6372 6970   M/O   | Descrip
+00018f20: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
+00018f50: 2d20 7c20 3a2d 2d2d 2d3a 207c 202d 2d2d  - | :----: | ---
+00018f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018f80: 2d2d 2d20 7c0a 7c20 6074 6974 6c65 6020  --- |.| `title` 
+00018f90: 2020 2020 2020 7c20 2020 4f20 2020 207c        |   O    |
+00018fa0: 206e 6f74 6966 6963 6174 696f 6e20 7469   notification ti
+00018fb0: 746c 6520 2020 2020 2020 2020 2020 2020  tle             
+00018fc0: 2020 2020 2020 2020 7c0a 7c20 6069 6d61          |.| `ima
+00018fd0: 6765 6020 2020 2020 2020 7c20 2020 4f20  ge`       |   O 
+00018fe0: 2020 207c 206e 6f74 6966 6963 6174 696f     | notificatio
+00018ff0: 6e20 696d 6167 6520 5552 4c20 2028 5b65  n image URL  ([e
+00019000: 7861 6d70 6c65 5d28 6874 7470 733a 2f2f  xample](https://
+00019010: 6769 7468 7562 2e63 6f6d 2f6a 706d 656e  github.com/jpmen
+00019020: 732f 6d71 7474 7761 726e 2f69 7373 7565  s/mqttwarn/issue
+00019030: 732f 3533 2369 7373 7565 636f 6d6d 656e  s/53#issuecommen
+00019040: 742d 3339 3639 3134 3239 2929 7c0a 0a23  t-39691429))|..#
+00019050: 2323 2060 786d 7070 600a 0a54 6865 2060  ## `xmpp`..The `
+00019060: 786d 7070 6020 7365 7276 6963 6520 7365  xmpp` service se
+00019070: 6e64 7320 6e6f 7469 6669 6361 7469 6f6e  nds notification
+00019080: 2074 6f20 6f6e 6520 6f72 206d 6f72 6520   to one or more 
+00019090: 5b58 4d50 505d 2868 7474 703a 2f2f 656e  [XMPP](http://en
+000190a0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+000190b0: 696b 692f 584d 5050 290a 284a 6162 6265  iki/XMPP).(Jabbe
+000190c0: 7229 2072 6563 6970 6965 6e74 732e 0a0a  r) recipients...
+000190d0: 6060 6069 6e69 0a5b 636f 6e66 6967 3a78  ```ini.[config:x
+000190e0: 6d70 705d 0a73 656e 6465 7220 3d20 276d  mpp].sender = 'm
+000190f0: 7174 7477 6172 6e40 6a61 6262 6572 2e73  qttwarn@jabber.s
+00019100: 6572 7665 7227 0a70 6173 7377 6f72 6420  erver'.password 
+00019110: 3d20 2750 6173 7377 6f72 6420 666f 7220  = 'Password for 
+00019120: 7365 6e64 6572 270a 7461 7267 6574 7320  sender'.targets 
+00019130: 3d20 7b0a 2020 2020 2761 646d 696e 2720  = {.    'admin' 
+00019140: 3a20 5b20 2761 646d 696e 3140 6a61 6262  : [ 'admin1@jabb
+00019150: 6572 2e73 6572 7665 7227 2c20 2761 646d  er.server', 'adm
+00019160: 696e 3240 6a61 6262 6572 2e73 6572 7665  in2@jabber.serve
+00019170: 7227 205d 0a20 2020 207d 0a60 6060 0a0a  r' ].    }.```..
+00019180: 5461 7267 6574 7320 6d61 7920 636f 6e74  Targets may cont
+00019190: 6169 6e20 6d6f 7265 2074 6861 6e20 6f6e  ain more than on
+000191a0: 6520 7265 6369 7069 656e 742c 2069 6e20  e recipient, in 
+000191b0: 7768 6963 6820 6361 7365 2061 6c6c 2073  which case all s
+000191c0: 7065 6369 6669 6564 0a72 6563 6970 6965  pecified.recipie
+000191d0: 6e74 7320 6765 7420 7468 6520 6d65 7373  nts get the mess
+000191e0: 6167 652e 0a0a 5265 7175 6972 6573 3a0a  age...Requires:.
+000191f0: 2a20 584d 5050 2028 4a61 6262 6572 2920  * XMPP (Jabber) 
+00019200: 6163 636f 756e 7473 2028 6174 206c 6561  accounts (at lea
+00019210: 7374 206f 6e65 2066 6f72 2074 6865 2073  st one for the s
+00019220: 656e 6465 7220 616e 6420 6f6e 6520 666f  ender and one fo
+00019230: 7220 7468 6520 7265 6369 7069 656e 7429  r the recipient)
+00019240: 0a2a 205b 786d 7070 7079 5d28 6874 7470  .* [xmpppy](http
+00019250: 3a2f 2f78 6d70 7070 792e 736f 7572 6365  ://xmpppy.source
+00019260: 666f 7267 652e 6e65 7429 0a0a 2323 2320  forge.net)..### 
+00019270: 6073 6c69 786d 7070 600a 0a54 6865 2060  `slixmpp`..The `
+00019280: 736c 6978 6d70 7060 2073 6572 7669 6365  slixmpp` service
+00019290: 2073 656e 6473 206e 6f74 6966 6963 6174   sends notificat
+000192a0: 696f 6e20 746f 206f 6e65 206f 7220 6d6f  ion to one or mo
+000192b0: 7265 205b 584d 5050 5d28 6874 7470 3a2f  re [XMPP](http:/
+000192c0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+000192d0: 672f 7769 6b69 2f58 4d50 5029 0a28 4a61  g/wiki/XMPP).(Ja
+000192e0: 6262 6572 2920 7265 6369 7069 656e 7473  bber) recipients
+000192f0: 2e0a 0a60 6060 696e 690a 5b63 6f6e 6669  ...```ini.[confi
+00019300: 673a 736c 6978 6d70 705d 0a73 656e 6465  g:slixmpp].sende
+00019310: 7220 3d20 276d 7174 7477 6172 6e40 6a61  r = 'mqttwarn@ja
+00019320: 6262 6572 2e73 6572 7665 7227 0a70 6173  bber.server'.pas
+00019330: 7377 6f72 6420 3d20 2750 6173 7377 6f72  sword = 'Passwor
+00019340: 6420 666f 7220 7365 6e64 6572 270a 7461  d for sender'.ta
+00019350: 7267 6574 7320 3d20 7b0a 2020 2020 2761  rgets = {.    'a
+00019360: 646d 696e 2720 3a20 5b20 2761 646d 696e  dmin' : [ 'admin
+00019370: 3140 6a61 6262 6572 2e73 6572 7665 7227  1@jabber.server'
+00019380: 2c20 2761 646d 696e 3240 6a61 6262 6572  , 'admin2@jabber
+00019390: 2e73 6572 7665 7227 205d 0a20 2020 207d  .server' ].    }
+000193a0: 0a60 6060 0a0a 5461 7267 6574 7320 6d61  .```..Targets ma
+000193b0: 7920 636f 6e74 6169 6e20 6d6f 7265 2074  y contain more t
+000193c0: 6861 6e20 6f6e 6520 7265 6369 7069 656e  han one recipien
+000193d0: 742c 2069 6e20 7768 6963 6820 6361 7365  t, in which case
+000193e0: 2061 6c6c 2073 7065 6369 6669 6564 0a72   all specified.r
+000193f0: 6563 6970 6965 6e74 7320 6765 7420 7468  ecipients get th
+00019400: 6520 6d65 7373 6167 652e 0a0a 5265 7175  e message...Requ
+00019410: 6972 6573 3a0a 2a20 584d 5050 2028 4a61  ires:.* XMPP (Ja
+00019420: 6262 6572 2920 6163 636f 756e 7473 2028  bber) accounts (
+00019430: 6174 206c 6561 7374 206f 6e65 2066 6f72  at least one for
+00019440: 2074 6865 2073 656e 6465 7220 616e 6420   the sender and 
+00019450: 6f6e 6520 666f 7220 7468 6520 7265 6369  one for the reci
+00019460: 7069 656e 7429 0a2a 205b 736c 6978 6d70  pient).* [slixmp
+00019470: 705d 2868 7474 7073 3a2f 2f6c 6162 2e6c  p](https://lab.l
+00019480: 6f75 697a 2e6f 7267 2f70 6f65 7a69 6f2f  ouiz.org/poezio/
+00019490: 736c 6978 6d70 7029 0a0a 2323 2320 6078  slixmpp)..### `x
+000194a0: 6976 656c 7960 0a0a 5468 6520 6078 6976  ively`..The `xiv
+000194b0: 656c 7960 2073 6572 7669 6365 2063 616e  ely` service can
+000194c0: 2073 656e 6420 6120 7375 6273 6574 206f   send a subset o
+000194d0: 6620 796f 7572 2064 6174 6120 746f 205b  f your data to [
+000194e0: 5869 7665 6c79 5d28 6874 7470 3a2f 2f78  Xively](http://x
+000194f0: 6976 656c 792e 636f 6d29 2070 6572 2064  ively.com) per d
+00019500: 6566 696e 6564 2066 6565 6469 642e 0a0a  efined feedid...
+00019510: 6060 6069 6e69 0a5b 636f 6e66 6967 3a78  ```ini.[config:x
+00019520: 6976 656c 795d 0a61 7069 6b65 7920 3d20  ively].apikey = 
+00019530: 2731 3233 3435 3637 3839 3061 6263 6465  '1234567890abcde
+00019540: 6667 6869 6b6c 6d6e 6f70 7172 7374 7576  fghiklmnopqrstuv
+00019550: 7778 797a 270a 7461 7267 6574 7320 3d20  wxyz'.targets = 
+00019560: 7b0a 2020 2020 2020 2020 2320 6665 6564  {.        # feed
+00019570: 6964 2020 2020 2020 2020 3a20 5b20 2764  id        : [ 'd
+00019580: 6174 6173 7472 6561 6d31 272c 2027 6461  atastream1', 'da
+00019590: 7461 7374 7265 616d 3227 5d0a 2020 2020  tastream2'].    
+000195a0: 2020 2020 2731 3233 3435 3637 2720 3a20      '1234567' : 
+000195b0: 5b20 2774 656d 7065 7261 7475 7265 272c  [ 'temperature',
+000195c0: 2027 7761 7465 726c 6576 656c 2720 5d2c   'waterlevel' ],
+000195d0: 0a20 2020 2020 2020 2027 3736 3534 3332  .        '765432
+000195e0: 3127 203a 205b 2027 6461 7461 4974 656d  1' : [ 'dataItem
+000195f0: 4127 205d 0a20 207d 0a60 6060 0a0a 5075  A' ].  }.```..Pu
+00019600: 626c 6973 6869 6e67 2074 6865 2066 6f6c  blishing the fol
+00019610: 6c6f 7769 6e67 204a 534f 4e20 6d65 7373  lowing JSON mess
+00019620: 6167 6520 7769 6c6c 2061 6464 2061 2064  age will add a d
+00019630: 6174 6170 6f69 6e74 2074 6f20 7468 6520  atapoint to the 
+00019640: 6074 656d 7065 7261 7475 7265 6020 616e  `temperature` an
+00019650: 640a 6077 6174 6572 6c65 7665 6c60 2063  d.`waterlevel` c
+00019660: 6861 6e6e 656c 206f 6620 796f 7572 2078  hannel of your x
+00019670: 6976 656c 7920 6665 6564 2031 3233 3435  ively feed 12345
+00019680: 3637 2028 6068 756d 6964 6974 7960 2077  67 (`humidity` w
+00019690: 696c 6c20 6265 2069 676e 6f72 6564 2c0a  ill be ignored,.
+000196a0: 6173 2069 7427 7320 6e6f 7420 6465 6669  as it's not defi
+000196b0: 6e65 6420 696e 2074 6865 2078 6976 656c  ned in the xivel
+000196c0: 790a 636f 6e66 6967 7572 6174 696f 6e20  y.configuration 
+000196d0: 6162 6f76 6529 3a0a 0a60 6060 0a6d 6f73  above):..```.mos
+000196e0: 7175 6974 746f 5f70 7562 202d 7420 226f  quitto_pub -t "o
+000196f0: 7378 2f6a 736f 6e22 202d 6d20 277b 2274  sx/json" -m '{"t
+00019700: 656d 7065 7261 7475 7265 223a 3135 2c22  emperature":15,"
+00019710: 7761 7465 726c 6576 656c 223a 3130 302c  waterlevel":100,
+00019720: 2268 756d 6964 6974 7922 3a33 357d 270a  "humidity":35}'.
+00019730: 6060 600a 0a0a 5265 7175 6972 6573 3a0a  ```...Requires:.
+00019740: 2a20 5b58 6976 656c 795d 2868 7474 703a  * [Xively](http:
+00019750: 2f2f 7869 7665 6c79 2e63 6f6d 2920 6163  //xively.com) ac
+00019760: 636f 756e 7420 7769 7468 2061 6e20 616c  count with an al
+00019770: 7265 6164 7920 6578 6973 7469 6e67 2046  ready existing F
+00019780: 6565 640a 2a20 5b78 6976 656c 792d 7079  eed.* [xively-py
+00019790: 7468 6f6e 5d28 6874 7470 733a 2f2f 6769  thon](https://gi
+000197a0: 7468 7562 2e63 6f6d 2f78 6976 656c 792f  thub.com/xively/
+000197b0: 7869 7665 6c79 2d70 7974 686f 6e29 202d  xively-python) -
+000197c0: 2070 6970 2069 6e73 7461 6c6c 2078 6976   pip install xiv
+000197d0: 656c 792d 7079 7468 6f6e 0a0a 2323 2320  ely-python..### 
+000197e0: 607a 6162 6269 7860 0a0a 5468 6520 607a  `zabbix`..The `z
+000197f0: 6162 6269 7860 2073 6572 7669 6365 2073  abbix` service s
+00019800: 6572 7665 7320 7477 6f20 7075 7270 6f73  erves two purpos
+00019810: 6573 3a0a 0a31 2e20 6974 2063 616e 2063  es:..1. it can c
+00019820: 7265 6174 6520 6120 5b5a 6162 6269 785d  reate a [Zabbix]
+00019830: 2068 6f73 7420 6f6e 2d74 6865 2d66 6c79   host on-the-fly
+00019840: 2076 6961 204c 6f77 2d6c 6576 656c 2044   via Low-level D
+00019850: 6973 636f 7665 7279 2028 4c4c 4429 0a32  iscovery (LLD).2
+00019860: 2e20 6974 2063 616e 2073 656e 6420 616e  . it can send an
+00019870: 2069 7465 6d2f 7661 6c75 6520 7061 6972   item/value pair
+00019880: 2074 6f20 6120 5b5a 6162 6269 785d 2074   to a [Zabbix] t
+00019890: 7261 7070 6572 0a0a 215b 5a61 6262 6978  rapper..![Zabbix
+000198a0: 5d28 6173 7365 7473 2f7a 6162 6269 782e  ](assets/zabbix.
+000198b0: 706e 6729 0a0a 546f 2063 7265 6174 6520  png)..To create 
+000198c0: 616e 2061 7070 726f 7072 6961 7465 2064  an appropriate d
+000198d0: 6973 636f 7665 7279 2068 6f73 742c 2069  iscovery host, i
+000198e0: 6e20 5a61 6262 6978 3a0a 2d20 436f 6e66  n Zabbix:.- Conf
+000198f0: 6967 7572 6174 696f 6e2d 3e48 6f73 7473  iguration->Hosts
+00019900: 2d3e 4372 6561 7465 2068 6f73 7420 2860  ->Create host (`
+00019910: 6d71 7474 7761 726e 3031 6029 0a2d 2043  mqttwarn01`).- C
+00019920: 6f6e 6669 6775 7261 7469 6f6e 2d3e 4469  onfiguration->Di
+00019930: 7363 6f76 6572 792d 3e43 7265 6174 6520  scovery->Create 
+00019940: 6469 7363 6f76 6572 7920 7275 6c65 0a20  discovery rule. 
+00019950: 202d 204e 616d 653a 2060 4d51 5454 7761   - Name: `MQTTwa
+00019960: 726e 6020 2861 6e79 2073 7569 7461 626c  rn` (any suitabl
+00019970: 6520 6e61 6d65 290a 2020 2d20 5479 7065  e name).  - Type
+00019980: 3a20 605a 6162 6269 7820 7472 6170 7065  : `Zabbix trappe
+00019990: 7260 0a20 202d 204b 6579 3a20 606d 7174  r`.  - Key: `mqt
+000199a0: 742e 6469 7363 6f76 6572 7960 2028 7468  t.discovery` (th
+000199b0: 6973 206d 7573 7420 6d61 7463 6820 7468  is must match th
+000199c0: 6520 636f 6e66 6967 7572 6564 2060 6469  e configured `di
+000199d0: 7363 6f76 6572 795f 6b65 7960 2c20 7768  scovery_key`, wh
+000199e0: 6963 6820 6465 6661 756c 7473 2074 6f20  ich defaults to 
+000199f0: 606d 7174 742e 6469 7363 6f76 6572 7960  `mqtt.discovery`
+00019a00: 290a 2020 2d20 416c 6c6f 7765 6420 686f  ).  - Allowed ho
+00019a10: 7374 733a 2060 3139 322e 3136 382e 312e  sts: `192.168.1.
+00019a20: 3133 302c 3132 372e 302e 302e 3160 2028  130,127.0.0.1` (
+00019a30: 6578 616d 706c 6529 0a0a 5468 6520 7461  example)..The ta
+00019a40: 7267 6574 2061 6e64 2074 6f70 6963 2063  rget and topic c
+00019a50: 6f6e 6669 6775 7261 7469 6f6e 206c 6f6f  onfiguration loo
+00019a60: 6b20 6c69 6b65 2074 6869 733a 0a0a 6060  k like this:..``
+00019a70: 6069 6e69 0a5b 636f 6e66 6967 3a7a 6162  `ini.[config:zab
+00019a80: 6269 785d 0a68 6f73 7420 3d20 226d 7174  bix].host = "mqt
+00019a90: 7477 6172 6e30 3122 2020 2320 616e 2065  twarn01"  # an e
+00019aa0: 7869 7374 696e 6720 686f 7374 2063 6f6e  xisting host con
+00019ab0: 6669 6775 7265 6420 696e 205a 6162 6269  figured in Zabbi
+00019ac0: 780a 6469 7363 6f76 6572 795f 6b65 7920  x.discovery_key 
+00019ad0: 3d20 226d 7174 742e 6469 7363 6f76 6572  = "mqtt.discover
+00019ae0: 7922 0a74 6172 6765 7473 203d 207b 0a20  y".targets = {. 
+00019af0: 2020 2020 2020 2020 2020 2023 2054 7261             # Tra
+00019b00: 7070 6572 2061 6464 7265 7373 2020 2070  pper address   p
+00019b10: 6f72 740a 2020 2020 2774 3127 2020 3a20  ort.    't1'  : 
+00019b20: 5b20 2731 3732 2e31 362e 3135 332e 3131  [ '172.16.153.11
+00019b30: 3027 2c20 3130 3035 3120 5d2c 0a20 207d  0', 10051 ],.  }
+00019b40: 0a0a 5b7a 6162 6269 782f 636c 6965 6e74  ..[zabbix/client
+00019b50: 732f 2b5d 0a61 6c6c 6461 7461 203d 205a  s/+].alldata = Z
+00019b60: 6162 6269 7844 6174 6128 290a 7461 7267  abbixData().targ
+00019b70: 6574 7320 3d20 7a61 6262 6978 3a74 310a  ets = zabbix:t1.
+00019b80: 0a5b 7a61 6262 6978 2f69 7465 6d2f 235d  .[zabbix/item/#]
+00019b90: 0a61 6c6c 6461 7461 203d 205a 6162 6269  .alldata = Zabbi
+00019ba0: 7844 6174 6128 290a 7461 7267 6574 7320  xData().targets 
+00019bb0: 3d20 7a61 6262 6978 3a74 310a 6060 600a  = zabbix:t1.```.
+00019bc0: 0a41 2074 7261 6e73 666f 726d 6174 696f  .A transformatio
+00019bd0: 6e20 6675 6e63 7469 6f6e 2069 6e20 6061  n function in `a
+00019be0: 6c6c 6461 7461 6020 6973 2072 6571 7569  lldata` is requi
+00019bf0: 7265 6420 746f 2065 7874 7261 6374 2074  red to extract t
+00019c00: 6865 2063 6c69 656e 7427 7320 6e61 6d65  he client's name
+00019c10: 0a66 726f 6d20 7468 6520 746f 7069 632c  .from the topic,
+00019c20: 2061 6e64 2066 6f72 2023 312c 2074 6f20   and for #1, to 
+00019c30: 6465 6669 6e65 2061 2022 686f 7374 2061  define a "host a
+00019c40: 6c69 7665 2220 6974 656d 206b 6579 2069  live" item key i
+00019c50: 6e20 5b5a 6162 6269 785d 2e0a 0a60 6060  n [Zabbix]...```
+00019c60: 7079 7468 6f6e 0a23 2049 6620 7468 6520  python.# If the 
+00019c70: 746f 7069 6320 6265 6769 6e73 2077 6974  topic begins wit
+00019c80: 6820 7a61 6262 6978 2f63 6c69 656e 7473  h zabbix/clients
+00019c90: 2077 6520 6861 7665 2061 2068 6f73 7420   we have a host 
+00019ca0: 676f 696e 6720 7570 206f 7220 646f 776e  going up or down
+00019cb0: 0a23 2065 2e67 2e20 227a 6162 6269 782f  .# e.g. "zabbix/
+00019cc0: 636c 6965 6e74 732f 6a6f 6730 3322 202d  clients/jog03" -
+00019cd0: 3e20 226a 6f67 3033 220a 2320 2020 6578  > "jog03".#   ex
+00019ce0: 7472 6163 7420 636c 6965 6e74 206e 616d  tract client nam
+00019cf0: 6520 2833 7264 2070 6172 7420 6f66 2074  e (3rd part of t
+00019d00: 6f70 6963 290a 2320 2020 7365 7420 7374  opic).#   set st
+00019d10: 6174 7573 206b 6579 2028 652e 672e 2027  atus key (e.g. '
+00019d20: 686f 7374 2e75 7027 2920 746f 2070 7562  host.up') to pub
+00019d30: 6c69 7368 2031 2f30 206f 6e20 6974 2028  lish 1/0 on it (
+00019d40: 652e 6720 6475 7269 6e67 204c 5754 290a  e.g during LWT).
+00019d50: 230a 2320 6966 2074 6865 2074 6f70 6963  #.# if the topic
+00019d60: 2073 7461 7274 7320 7769 7468 207a 6162   starts with zab
+00019d70: 6269 782f 6974 656d 2077 6520 6861 7665  bix/item we have
+00019d80: 2061 6e20 6974 656d 2f76 616c 7565 2066   an item/value f
+00019d90: 6f72 2074 6865 2068 6f73 740a 2320 652e  or the host.# e.
+00019da0: 672e 2022 7a61 6262 6978 2f69 7465 6d2f  g. "zabbix/item/
+00019db0: 6a6f 6730 332f 7469 6d65 2e73 7461 6d70  jog03/time.stamp
+00019dc0: 2220 2d3e 2022 6a6f 6730 3322 0a23 2020  " -> "jog03".#  
+00019dd0: 2065 7874 7261 6374 2063 6c69 656e 7420   extract client 
+00019de0: 6e61 6d65 2028 3372 6420 7061 7274 206f  name (3rd part o
+00019df0: 6620 746f 7069 6329 0a23 0a0a 6465 6620  f topic).#..def 
+00019e00: 5a61 6262 6978 4461 7461 2874 6f70 6963  ZabbixData(topic
+00019e10: 2c20 6461 7461 2c20 7372 763d 4e6f 6e65  , data, srv=None
+00019e20: 293a 0a20 2020 2063 6c69 656e 7420 3d20  ):.    client = 
+00019e30: 2775 6e6b 6e6f 776e 270a 2020 2020 6b65  'unknown'.    ke
+00019e40: 7920 3d20 4e6f 6e65 0a20 2020 2073 7461  y = None.    sta
+00019e50: 7475 735f 6b65 7920 3d20 4e6f 6e65 0a0a  tus_key = None..
+00019e60: 2020 2020 7061 7274 7320 3d20 746f 7069      parts = topi
+00019e70: 632e 7370 6c69 7428 272f 2729 0a0a 2020  c.split('/')..  
+00019e80: 2020 2727 2720 5768 6174 2077 6520 6361    ''' What we ca
+00019e90: 6c6c 2027 636c 6965 6e74 2720 6973 2069  ll 'client' is i
+00019ea0: 6e20 6661 6374 2061 2022 5a61 6262 6978  n fact a "Zabbix
+00019eb0: 2048 6f73 7422 2c20 692e 652e 2074 6865   Host", i.e. the
+00019ec0: 206e 616d 6520 6f66 2061 0a20 2020 2020   name of a.     
+00019ed0: 2020 2068 6f73 7420 636f 6e66 6967 7572     host configur
+00019ee0: 6564 2077 6974 6820 6974 656d 733b 2069  ed with items; i
+00019ef0: 7420 6974 206e 6f74 2074 6865 206e 616d  t it not the nam
+00019f00: 652f 6164 6472 6573 7320 6f66 2074 6865  e/address of the
+00019f10: 206d 6163 6869 6e65 206f 6e0a 2020 2020   machine on.    
+00019f20: 2020 2020 7768 6963 6820 5a61 6262 6978      which Zabbix
+00019f30: 2073 6572 7665 7220 7275 6e73 2e20 536f   server runs. So
+00019f40: 2c20 696e 2074 6865 2055 493a 2043 6f6e  , in the UI: Con
+00019f50: 6669 6775 7261 7469 6f6e 202d 3e20 4372  figuration -> Cr
+00019f60: 6561 7465 2068 6f73 7420 2727 270a 0a20  eate host '''.. 
+00019f70: 2020 2063 6c69 656e 7420 3d20 7061 7274     client = part
+00019f80: 735b 325d 0a0a 2020 2020 6966 2074 6f70  s[2]..    if top
+00019f90: 6963 2e73 7461 7274 7377 6974 6828 277a  ic.startswith('z
+00019fa0: 6162 6269 782f 636c 6965 6e74 732f 2729  abbix/clients/')
+00019fb0: 3a0a 2020 2020 2020 2020 7374 6174 7573  :.        status
+00019fc0: 5f6b 6579 203d 2027 686f 7374 2e75 7027  _key = 'host.up'
+00019fd0: 0a0a 2020 2020 2727 2720 5468 6973 2022  ..    ''' This "
+00019fe0: 6b65 7922 2069 7320 6163 7475 616c 6c79  key" is actually
+00019ff0: 2061 6e20 4c4c 4420 6974 656d 2077 6869   an LLD item whi
+0001a000: 6368 2077 6527 7665 2070 7265 2d63 7265  ch we've pre-cre
+0001a010: 6174 6564 2069 6e20 7468 6520 5a61 6262  ated in the Zabb
+0001a020: 6978 0a20 2020 2020 2020 2055 492e 2043  ix.        UI. C
+0001a030: 6f6e 6669 6775 7261 7469 6f6e 2d3e 486f  onfiguration->Ho
+0001a040: 7374 732d 3e44 6973 636f 7665 7279 2d3e  sts->Discovery->
+0001a050: 4974 656d 2070 726f 746f 7479 7065 732d  Item prototypes-
+0001a060: 3e43 7265 6174 6520 6974 656d 2070 726f  >Create item pro
+0001a070: 746f 7479 7065 0a09 2020 204e 616d 653a  totype..   Name:
+0001a080: 204d 5720 636c 6965 6e74 2024 310a 0920   MW client $1.. 
+0001a090: 2020 5479 7065 3a20 5a61 6262 6978 2074    Type: Zabbix t
+0001a0a0: 7261 7070 6572 0a09 2020 204b 6579 3a20  rapper..   Key: 
+0001a0b0: 6d71 7474 7761 726e 2e69 645b 7b23 4d51  mqttwarn.id[{#MQ
+0001a0c0: 5454 484f 5354 7d5d 0a09 2020 2054 7970  TTHOST}]..   Typ
+0001a0d0: 653a 2074 6578 7420 2863 616e 2062 6520  e: text (can be 
+0001a0e0: 616e 7920 7375 6974 6162 6c65 2074 7970  any suitable typ
+0001a0f0: 6529 0a0a 0950 7562 6c69 7368 696e 6720  e)...Publishing 
+0001a100: 6120 7661 6c75 6520 7769 7468 0a09 2420  a value with..$ 
+0001a110: 6d6f 7371 7569 7474 6f5f 7075 6220 2d74  mosquitto_pub -t
+0001a120: 207a 6162 6269 782f 6974 656d 2f6d 7174   zabbix/item/mqt
+0001a130: 7477 6172 6e30 312f 6d71 7474 7761 726e  twarn01/mqttwarn
+0001a140: 2e69 645b 6d30 325d 202d 6d20 2773 746f  .id[m02] -m 'sto
+0001a150: 726d 7927 0a09 7769 6c6c 206d 6561 6e20  rmy'..will mean 
+0001a160: 7468 6174 2077 6527 6c6c 2075 7365 2074  that we'll use t
+0001a170: 6865 2063 6c69 656e 7420 226d 7174 7477  he client "mqttw
+0001a180: 6172 6e30 3122 2028 7365 6520 7072 6576  arn01" (see prev
+0001a190: 696f 7573 6c79 2920 616e 640a 0974 6865  iously) and..the
+0001a1a0: 2069 7465 6d20 6e61 6d65 6420 226d 7174   item named "mqt
+0001a1b0: 7477 6172 6e2e 6964 5b6d 3032 5d22 2077  twarn.id[m02]" w
+0001a1c0: 6869 6368 2069 7320 7468 6520 6e61 6d65  hich is the name
+0001a1d0: 206f 6620 6120 7072 6576 696f 7573 6c79   of a previously
+0001a1e0: 0a09 6469 7363 6f76 6572 6564 2069 7465  ..discovered ite
+0001a1f0: 6d2e 0a20 2020 2027 2727 0a0a 2020 2020  m..    '''..    
+0001a200: 6966 2074 6f70 6963 2e73 7461 7274 7377  if topic.startsw
+0001a210: 6974 6828 277a 6162 6269 782f 6974 656d  ith('zabbix/item
+0001a220: 2f27 293a 0a20 2020 2020 2020 206b 6579  /'):.        key
+0001a230: 203d 2070 6172 7473 5b33 5d0a 0a20 2020   = parts[3]..   
+0001a240: 2072 6574 7572 6e20 6469 6374 2863 6c69   return dict(cli
+0001a250: 656e 743d 636c 6965 6e74 2c20 6b65 793d  ent=client, key=
+0001a260: 6b65 792c 2073 7461 7475 735f 6b65 793d  key, status_key=
+0001a270: 7374 6174 7573 5f6b 6579 290a 6060 600a  status_key).```.
+0001a280: 0a23 2323 2043 7265 6174 696e 6720 4375  .### Creating Cu
+0001a290: 7374 6f6d 2053 6572 7669 6365 2050 6c75  stom Service Plu
+0001a2a0: 6769 6e73 0a0a 4372 6561 7469 6e67 206e  gins..Creating n
+0001a2b0: 6577 2070 6c75 6769 6e73 2069 7320 7261  ew plugins is ra
+0001a2c0: 7468 6572 2065 6173 792c 2061 6e64 2049  ther easy, and I
+0001a2d0: 2072 6563 6f6d 6d65 6e64 2079 6f75 2074   recommend you t
+0001a2e0: 616b 6520 7468 6520 6066 696c 6560 2070  ake the `file` p
+0001a2f0: 6c75 6769 6e0a 616e 6420 7374 6172 7420  lugin.and start 
+0001a300: 6672 6f6d 2074 6861 742e 0a0a 506c 7567  from that...Plug
+0001a310: 696e 7320 6172 6520 696e 766f 6b65 6420  ins are invoked 
+0001a320: 7769 7468 2074 776f 2061 7267 756d 656e  with two argumen
+0001a330: 7473 2028 6073 7276 6020 616e 6420 6069  ts (`srv` and `i
+0001a340: 7465 6d60 292e 2060 7372 7660 2069 7320  tem`). `srv` is 
+0001a350: 616e 206f 626a 6563 740a 7769 7468 2073  an object.with s
+0001a360: 6f6d 6520 6865 6c70 6572 2066 756e 6374  ome helper funct
+0001a370: 696f 6e73 2c20 616e 6420 6069 7465 6d60  ions, and `item`
+0001a380: 2061 2064 6963 7420 7768 6963 6820 636f   a dict which co
+0001a390: 6e74 6169 6e73 2069 6e66 6f72 6d61 7469  ntains informati
+0001a3a0: 6f6e 206f 6e20 7468 6520 6d65 7373 6167  on on the messag
+0001a3b0: 650a 7768 6963 6820 6973 2074 6f20 6265  e.which is to be
+0001a3c0: 2068 616e 646c 6564 2062 7920 7468 6520   handled by the 
+0001a3d0: 706c 7567 696e 2e20 6069 7465 6d60 2063  plugin. `item` c
+0001a3e0: 6f6e 7461 696e 7320 7468 6520 666f 6c6c  ontains the foll
+0001a3f0: 6f77 696e 6720 656c 656d 656e 7473 3a0a  owing elements:.
+0001a400: 0a60 6060 7079 7468 6f6e 0a69 7465 6d20  .```python.item 
+0001a410: 3d20 7b0a 2020 2020 2773 6572 7669 6365  = {.    'service
+0001a420: 2720 2020 2020 2020 3a20 2773 7472 696e  '       : 'strin
+0001a430: 6727 2c20 2020 2020 2020 2320 6e61 6d65  g',       # name
+0001a440: 206f 6620 6861 6e64 6c69 6e67 2073 6572   of handling ser
+0001a450: 7669 6365 2028 6074 7769 7474 6572 602c  vice (`twitter`,
+0001a460: 2060 6669 6c65 602c 202e 2e29 0a20 2020   `file`, ..).   
+0001a470: 2027 7461 7267 6574 2720 2020 2020 2020   'target'       
+0001a480: 203a 2027 7374 7269 6e67 272c 2020 2020   : 'string',    
+0001a490: 2020 2023 206e 616d 6520 6f66 2074 6172     # name of tar
+0001a4a0: 6765 7420 2860 6f31 602c 2060 6a61 6e65  get (`o1`, `jane
+0001a4b0: 6a6f 6c60 2920 696e 2073 6572 7669 6365  jol`) in service
+0001a4c0: 0a20 2020 2027 6164 6472 7327 2020 2020  .    'addrs'    
+0001a4d0: 2020 2020 203a 206c 6973 742c 2020 2020       : list,    
+0001a4e0: 2020 2020 2020 2023 206c 6973 7420 6f66         # list of
+0001a4f0: 2061 6464 7265 7373 6573 2066 726f 6d20   addresses from 
+0001a500: 5345 5256 4943 455f 7461 7267 6574 730a  SERVICE_targets.
+0001a510: 2020 2020 2763 6f6e 6669 6727 2020 2020      'config'    
+0001a520: 2020 2020 3a20 6469 6374 2c20 2020 2020      : dict,     
+0001a530: 2020 2020 2020 2320 4e6f 6e65 206f 7220        # None or 
+0001a540: 6469 6374 2066 726f 6d20 5345 5256 4943  dict from SERVIC
+0001a550: 455f 636f 6e66 6967 207b 7d0a 2020 2020  E_config {}.    
+0001a560: 2774 6f70 6963 2720 2020 2020 2020 2020  'topic'         
+0001a570: 3a20 2773 7472 696e 6727 2c20 2020 2020  : 'string',     
+0001a580: 2020 2320 696e 636f 6d69 6e67 2074 6f70    # incoming top
+0001a590: 6963 2062 7261 6e63 6820 6e61 6d65 0a20  ic branch name. 
+0001a5a0: 2020 2027 7061 796c 6f61 6427 2020 2020     'payload'    
+0001a5b0: 2020 203a 2027 7374 7269 6e67 272c 2020     : 'string',  
+0001a5c0: 2020 2020 2023 2072 6177 206d 6573 7361       # raw messa
+0001a5d0: 6765 2070 6179 6c6f 6164 0a20 2020 2027  ge payload.    '
+0001a5e0: 6d65 7373 6167 6527 2020 2020 2020 203a  message'       :
+0001a5f0: 2027 7374 7269 6e67 272c 2020 2020 2020   'string',      
+0001a600: 2023 2066 6f72 6d61 7474 6564 206d 6573   # formatted mes
+0001a610: 7361 6765 2028 6966 206e 6f20 666f 726d  sage (if no form
+0001a620: 6174 2073 7472 696e 6720 7468 656e 203d  at string then =
+0001a630: 2070 6179 6c6f 6164 290a 2020 2020 2764   payload).    'd
+0001a640: 6174 6127 2020 2020 2020 2020 2020 3a20  ata'          : 
+0001a650: 4e6f 6e65 2c20 2020 2020 2020 2020 2020  None,           
+0001a660: 2320 6469 6374 2077 6974 6820 7472 616e  # dict with tran
+0001a670: 7366 6f72 6d61 7469 6f6e 2064 6174 610a  sformation data.
+0001a680: 2020 2020 2774 6974 6c65 2720 2020 2020      'title'     
+0001a690: 2020 2020 3a20 276d 7174 7477 6172 6e27      : 'mqttwarn'
+0001a6a0: 2c20 2020 2020 2320 706f 7373 6962 6c65  ,     # possible
+0001a6b0: 2074 6974 6c65 2066 726f 6d20 7469 746c   title from titl
+0001a6c0: 657b 7d0a 2020 2020 2770 7269 6f72 6974  e{}.    'priorit
+0001a6d0: 7927 2020 2020 2020 3a20 302c 2020 2020  y'      : 0,    
+0001a6e0: 2020 2020 2020 2020 2020 2320 706f 7373            # poss
+0001a6f0: 6962 6c65 2070 7269 6f72 6974 7920 6672  ible priority fr
+0001a700: 6f6d 2070 7269 6f72 6974 797b 7d0a 7d0a  om priority{}.}.
+0001a710: 6060 600a 0a23 2320 4f75 7462 6f75 6e64  ```..## Outbound
+0001a720: 206d 6573 7361 6765 730a 0a23 2323 204d   messages..### M
+0001a730: 6573 7361 6765 2066 6f72 7761 7264 696e  essage forwardin
+0001a740: 670a 0a54 6f20 7369 6d70 6c79 2066 6f72  g..To simply for
+0001a750: 7761 7264 2061 6e20 696e 636f 6d69 6e67  ward an incoming
+0001a760: 204d 5154 5420 6d65 7373 6167 652c 2079   MQTT message, y
+0001a770: 6f75 2064 6f6e 2774 206e 6565 6420 746f  ou don't need to
+0001a780: 2064 6f20 616e 7974 6869 6e67 206f 7468   do anything oth
+0001a790: 6572 2074 6861 6e20 636f 6e66 6967 7572  er than configur
+0001a7a0: 6520 7468 6520 7461 7267 6574 2e20 4164  e the target. Ad
+0001a7b0: 6420 6120 746f 7069 6320 7365 6374 696f  d a topic sectio
+0001a7c0: 6e20 746f 2079 6f75 7220 606d 7174 7477  n to your `mqttw
+0001a7d0: 6172 6e2e 696e 6960 2c20 6279 2073 696d  arn.ini`, by sim
+0001a7e0: 706c 7920 6e61 6d69 6e67 2069 7420 6166  ply naming it af
+0001a7f0: 7465 7220 7468 6520 746f 7069 6320 796f  ter the topic yo
+0001a800: 7520 7769 7368 2074 6f20 6861 7665 2066  u wish to have f
+0001a810: 6f72 7761 7264 6564 2c20 616e 6420 7769  orwarded, and wi
+0001a820: 7468 696e 2064 6566 696e 6520 7468 6520  thin define the 
+0001a830: 6074 6172 6765 7473 602e 2054 6865 2070  `targets`. The p
+0001a840: 6179 6c6f 6164 206f 6620 7468 6520 696e  ayload of the in
+0001a850: 626f 756e 6420 6d65 7373 6167 6520 7769  bound message wi
+0001a860: 6c6c 2074 6865 6e20 6265 2066 6f72 7761  ll then be forwa
+0001a870: 7264 6564 2074 6f20 7468 6520 6465 6669  rded to the defi
+0001a880: 6e65 6420 7365 7276 6963 6520 706c 7567  ned service plug
+0001a890: 696e 2c20 7765 7468 6572 2069 7420 7369  in, wether it si
+0001a8a0: 6d70 6c79 2073 6179 7320 224f 4e22 2c20  mply says "ON", 
+0001a8b0: 6f72 2063 6f6e 7461 696e 7320 6120 6c61  or contains a la
+0001a8c0: 7267 6520 4a53 4f4e 2064 6963 7469 6f6e  rge JSON diction
+0001a8d0: 6172 792e 0a0a 5b6f 6666 6963 652f 7570  ary...[office/up
+0001a8e0: 735d 0a74 6172 6765 7473 203d 206c 6f67  s].targets = log
+0001a8f0: 3a64 6562 7567 0a0a 5468 6973 2065 7861  :debug..This exa
+0001a900: 6d70 6c65 2073 686f 7773 2068 6f77 2074  mple shows how t
+0001a910: 6f20 6861 7665 206d 6573 7361 6765 7320  o have messages 
+0001a920: 7265 6365 6976 6564 206f 6e20 7468 6520  received on the 
+0001a930: 4d51 5454 2074 6f70 6963 2060 6f66 6669  MQTT topic `offi
+0001a940: 6365 2f75 7073 602c 2073 6176 6564 2069  ce/ups`, saved i
+0001a950: 6e74 6f20 7468 6520 606d 7174 7477 6172  nto the `mqttwar
+0001a960: 6e2e 6c6f 6760 2066 696c 6520 7769 7468  n.log` file with
+0001a970: 2061 2060 6465 6275 6760 206c 6162 656c   a `debug` label
+0001a980: 2e20 5468 6973 206f 6620 636f 7572 7365  . This of course
+0001a990: 2061 7373 756d 6573 2074 6861 7420 796f   assumes that yo
+0001a9a0: 7520 6861 7665 2063 6f6e 6669 6775 7265  u have configure
+0001a9b0: 6420 7468 6520 6c6f 6720 7365 6374 696f  d the log sectio
+0001a9c0: 6e20 7468 6520 7761 7920 6465 7363 7269  n the way descri
+0001a9d0: 6265 6420 5b61 626f 7665 5d28 2374 6865  bed [above](#the
+0001a9e0: 2d63 6f6e 6669 6778 7878 2d73 6563 7469  -configxxx-secti
+0001a9f0: 6f6e 7329 2e20 0a0a 4275 7420 6d71 7474  ons). ..But mqtt
+0001aa00: 7761 726e 2070 726f 7669 6465 7320 7365  warn provides se
+0001aa10: 7665 7261 6c20 6f70 7469 6f6e 7320 746f  veral options to
+0001aa20: 2063 7265 6174 6520 6120 6469 6666 6572   create a differ
+0001aa30: 656e 7420 6f75 7462 6f75 6e64 206d 6573  ent outbound mes
+0001aa40: 7361 6765 2c20 616c 6c6f 7769 6e67 2079  sage, allowing y
+0001aa50: 6f75 2066 6f72 2065 7861 6d70 6c65 2074  ou for example t
+0001aa60: 6f20 6d61 6b65 2079 6f75 7220 6f75 7462  o make your outb
+0001aa70: 6f75 6e64 206d 6573 7361 6765 206d 6f72  ound message mor
+0001aa80: 6520 6875 6d61 6e2d 7265 6164 6162 6c65  e human-readable
+0001aa90: 2e20 0a0a 5468 6520 7469 746c 6520 616e  . ..The title an
+0001aaa0: 6420 666f 726d 6174 2064 6972 6563 7469  d format directi
+0001aab0: 7665 7320 6465 6669 6e65 2074 6865 2074  ves define the t
+0001aac0: 6974 6c65 2061 6e64 2074 6865 2062 6f64  itle and the bod
+0001aad0: 7920 6f66 2074 6865 206f 7574 626f 756e  y of the outboun
+0001aae0: 6420 6d65 7373 6167 652e 2048 6572 652c  d message. Here,
+0001aaf0: 2079 6f75 2063 616e 2074 7572 6e20 616e   you can turn an
+0001ab00: 204d 5154 5420 7061 796c 6f61 6420 7468   MQTT payload th
+0001ab10: 6174 2073 696d 706c 7920 7374 6174 6573  at simply states
+0001ab20: 2022 4f4e 222c 2069 6e74 6f20 6120 6672   "ON", into a fr
+0001ab30: 6965 6e64 6c69 6572 2076 6572 7369 6f6e  iendlier version
+0001ab40: 2e20 0a0a 6060 600a 5b6f 6666 6963 652f  . ..```.[office/
+0001ab50: 7570 735d 0a74 6974 6c65 203d 204f 6666  ups].title = Off
+0001ab60: 6963 6520 5550 530a 666f 726d 6174 203d  ice UPS.format =
+0001ab70: 2054 6865 206f 6666 6963 6520 5550 5320   The office UPS 
+0001ab80: 6973 207b 7061 796c 6f61 647d 0a60 6060  is {payload}.```
+0001ab90: 0a0a 4e6f 7469 6365 2074 6861 7420 7468  ..Notice that th
+0001aba0: 6520 6f72 6967 696e 616c 204d 5154 5420  e original MQTT 
+0001abb0: 7061 796c 6f61 6420 6973 2072 6566 6572  payload is refer
+0001abc0: 656e 6365 642c 2073 6f20 7468 6174 2069  enced, so that i
+0001abd0: 6620 7468 6520 5550 5320 6973 2073 7769  f the UPS is swi
+0001abe0: 7463 6865 6420 6f66 6620 616e 6420 7365  tched off and se
+0001abf0: 6e64 7320 6f75 7420 6120 636f 7272 6573  nds out a corres
+0001ac00: 706f 6e64 696e 6720 4d51 5454 206d 6573  ponding MQTT mes
+0001ac10: 7361 6765 2c20 7468 6520 6f75 7462 6f75  sage, the outbou
+0001ac20: 6e64 206d 6573 7361 6765 2077 696c 6c20  nd message will 
+0001ac30: 7374 6174 6520 7468 6520 7361 6d65 2e20  state the same. 
+0001ac40: 5468 6520 696e 666f 726d 6174 696f 6e20  The information 
+0001ac50: 7468 6174 2069 7320 6176 6169 6c61 626c  that is availabl
+0001ac60: 6520 746f 2079 6f75 2069 6e20 6372 6561  e to you in crea
+0001ac70: 7469 6e67 2074 6865 206f 7574 626f 756e  ting the outboun
+0001ac80: 6420 6d65 7373 6167 652c 2069 7320 6361  d message, is ca
+0001ac90: 6c6c 6564 2074 6865 2074 7261 6e73 666f  lled the transfo
+0001aca0: 726d 6174 696f 6e20 6461 7461 2e20 5468  rmation data. Th
+0001acb0: 6520 7665 7279 2062 6173 6963 2073 6574  e very basic set
+0001acc0: 206f 6620 7472 616e 7366 6f72 6d61 7469   of transformati
+0001acd0: 6f6e 2064 6174 6120 6973 2074 6865 2066  on data is the f
+0001ace0: 6f6c 6c6f 7769 6e67 203a 200a 0a60 6060  ollowing : ..```
+0001acf0: 7079 7468 6f6e 0a7b 0a20 2027 746f 7069  python.{.  'topi
+0001ad00: 6327 2020 2020 2020 2020 203a 2074 6f70  c'         : top
+0001ad10: 6963 206e 616d 650a 2020 2770 6179 6c6f  ic name.  'paylo
+0001ad20: 6164 2720 2020 2020 2020 3a20 746f 7069  ad'       : topi
+0001ad30: 6320 7061 796c 6f61 640a 2020 275f 6474  c payload.  '_dt
+0001ad40: 6570 6f63 6827 2020 2020 2020 3a20 6570  epoch'      : ep
+0001ad50: 6f63 6820 7469 6d65 2020 2020 2020 2020  och time        
+0001ad60: 2020 2020 2020 2020 2020 2320 3133 3932            # 1392
+0001ad70: 3632 3835 3831 0a20 2027 5f64 7469 736f  628581.  '_dtiso
+0001ad80: 2720 2020 2020 2020 203a 2049 534f 2064  '        : ISO d
+0001ad90: 6174 6520 2855 5443 2920 2020 2020 2020  ate (UTC)       
+0001ada0: 2020 2020 2020 2023 2032 3031 342d 3032         # 2014-02
+0001adb0: 2d31 3754 3130 3a33 383a 3433 2e39 3130  -17T10:38:43.910
+0001adc0: 3639 315a 0a20 2027 5f64 7468 686d 6d27  691Z.  '_dthhmm'
+0001add0: 2020 2020 2020 203a 2074 696d 6573 7461         : timesta
+0001ade0: 6d70 2048 483a 4d4d 2028 6c6f 6361 6c29  mp HH:MM (local)
+0001adf0: 2020 2020 2023 2031 303a 3136 0a20 2027       # 10:16.  '
+0001ae00: 5f64 7468 686d 6d73 7327 2020 2020 203a  _dthhmmss'     :
+0001ae10: 2074 696d 6573 7461 6d70 2048 483a 4d4d   timestamp HH:MM
+0001ae20: 3a53 5320 286c 6f63 616c 2920 2023 2031  :SS (local)  # 1
+0001ae30: 303a 3136 3a32 310a 7d0a 6060 600a 0a23  0:16:21.}.```..#
+0001ae40: 2323 2054 7261 6e73 666f 726d 696e 6720  ## Transforming 
+0001ae50: 696e 626f 756e 6420 4a53 4f4e 0a0a 496e  inbound JSON..In
+0001ae60: 2061 6464 6974 696f 6e20 746f 2070 6173   addition to pas
+0001ae70: 7369 6e67 2074 6865 2070 6179 6c6f 6164  sing the payload
+0001ae80: 2072 6563 6569 7665 6420 7669 6120 4d51   received via MQ
+0001ae90: 5454 2074 6f20 6120 7365 7276 6963 652c  TT to a service,
+0001aea0: 205f 6d71 7474 7761 726e 5f20 616c 6c6f   _mqttwarn_ allo
+0001aeb0: 7773 2079 6f75 2064 6f20 646f 2074 6865  ws you do do the
+0001aec0: 2066 6f6c 6c6f 7769 6e67 3a0a 0a2a 2054   following:..* T
+0001aed0: 7261 6e73 666f 726d 2070 6179 6c6f 6164  ransform payload
+0001aee0: 7320 6f6e 2061 2070 6572 2f74 6f70 6963  s on a per/topic
+0001aef0: 2062 6173 6973 2e20 466f 7220 6578 616d   basis. For exam
+0001af00: 706c 652c 2079 6f75 206b 6e6f 7720 796f  ple, you know yo
+0001af10: 7527 6c6c 2062 6520 7265 6365 6976 696e  u'll be receivin
+0001af20: 6720 4a53 4f4e 2c20 6275 7420 796f 7520  g JSON, but you 
+0001af30: 7761 6e74 2074 6f20 7761 726e 2077 6974  want to warn wit
+0001af40: 6820 6120 6e69 6365 6c79 2066 6f72 6d61  h a nicely forma
+0001af50: 7474 6564 206d 6573 7361 6765 2e0a 2a20  tted message..* 
+0001af60: 466f 7220 6365 7274 6169 6e20 7365 7276  For certain serv
+0001af70: 6963 6573 2c20 796f 7520 6361 6e20 6368  ices, you can ch
+0001af80: 616e 6765 2074 6865 205f 7469 746c 655f  ange the _title_
+0001af90: 2028 6f72 205f 7375 626a 6563 745f 2920   (or _subject_) 
+0001afa0: 6f66 2074 6865 206f 7574 676f 696e 6720  of the outgoing 
+0001afb0: 6d65 7373 6167 652e 0a2a 2046 6f72 2063  message..* For c
+0001afc0: 6572 7461 696e 2073 6572 7669 6365 732c  ertain services,
+0001afd0: 2079 6f75 2063 616e 2063 6861 6e67 6520   you can change 
+0001afe0: 7468 6520 5f70 7269 6f72 6974 795f 206f  the _priority_ o
+0001aff0: 6620 7468 6520 6f75 7467 6f69 6e67 206d  f the outgoing m
+0001b000: 6573 7361 6765 2e0a 0a43 6f6e 7369 6465  essage...Conside
+0001b010: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+0001b020: 4a53 4f4e 2070 6179 6c6f 6164 2070 7562  JSON payload pub
+0001b030: 6c69 7368 6564 2074 6f20 7468 6520 4d51  lished to the MQ
+0001b040: 5454 2062 726f 6b65 723a 0a0a 6060 6073  TT broker:..```s
+0001b050: 6865 6c6c 0a6d 6f73 7175 6974 746f 5f70  hell.mosquitto_p
+0001b060: 7562 202d 7420 276f 7378 2f6a 736f 6e27  ub -t 'osx/json'
+0001b070: 202d 6d20 277b 2266 7275 6974 223a 2262   -m '{"fruit":"b
+0001b080: 616e 616e 6122 2c20 2270 7269 6365 223a  anana", "price":
+0001b090: 2036 332c 2022 7473 7422 203a 2022 3133   63, "tst" : "13
+0001b0a0: 3931 3737 3933 3336 227d 270a 6060 600a  91779336"}'.```.
+0001b0b0: 0a55 7369 6e67 2060 666f 726d 6174 6020  .Using `format` 
+0001b0c0: 7765 2063 616e 2063 6f6e 6669 6775 7265  we can configure
+0001b0d0: 205f 6d71 7474 7761 726e 5f20 746f 2074   _mqttwarn_ to t
+0001b0e0: 7261 6e73 666f 726d 2074 6861 7420 4a53  ransform that JS
+0001b0f0: 4f4e 2069 6e74 6f20 6120 6469 6666 6572  ON into a differ
+0001b100: 656e 7420 6f75 7467 6f69 6e67 206d 6573  ent outgoing mes
+0001b110: 7361 6765 2077 6869 6368 2069 7320 7468  sage which is th
+0001b120: 6520 7465 7874 2074 6861 7420 6973 2061  e text that is a
+0001b130: 6374 7561 6c6c 7920 6e6f 7469 6669 6564  ctually notified
+0001b140: 2e20 5061 7274 206f 6620 7361 6964 2060  . Part of said `
+0001b150: 666f 726d 6174 6020 6c6f 6f6b 7320 6c69  format` looks li
+0001b160: 6b65 2074 6869 7320 696e 2074 6865 2063  ke this in the c
+0001b170: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+0001b180: 652c 2061 6e64 2062 6173 6963 616c 6c79  e, and basically
+0001b190: 2073 7065 6369 6669 6573 2074 6861 7420   specifies that 
+0001b1a0: 6d65 7373 6167 6573 2070 7562 6c69 7368  messages publish
+0001b1b0: 6564 2074 6f20 606f 7378 2f6a 736f 6e60  ed to `osx/json`
+0001b1c0: 2073 686f 756c 6420 6265 2074 7261 6e73   should be trans
+0001b1d0: 666f 726d 6564 2061 7320 6f6e 2074 6865  formed as on the
+0001b1e0: 2072 6967 6874 2d68 616e 6420 7369 6465   right-hand side
+0001b1f0: 2e0a 0a60 6060 696e 690a 666f 726d 6174  ...```ini.format
+0001b200: 203d 2022 4927 6c6c 2068 6176 6520 6120   = "I'll have a 
+0001b210: 7b66 7275 6974 7d20 6966 2069 7420 636f  {fruit} if it co
+0001b220: 7374 7320 7b70 7269 6365 7d22 0a60 6060  sts {price}".```
+0001b230: 0a0a 2845 6d62 6564 6465 6420 6022 5c6e  ..(Embedded `"\n
+0001b240: 2260 2061 7265 2063 6f6e 7665 7274 6564  "` are converted
+0001b250: 2074 6f20 6e65 776c 696e 6573 206f 6e20   to newlines on 
+0001b260: 6f75 7470 7574 2e29 0a0a 5468 6520 7265  output.)..The re
+0001b270: 7375 6c74 2069 733a 0a0a 215b 4f53 5820  sult is:..![OSX 
+0001b280: 6e6f 7469 6669 6572 5d28 6173 7365 7473  notifier](assets
+0001b290: 2f64 6573 6b74 6f70 6e6f 7469 6679 2e6a  /desktopnotify.j
+0001b2a0: 7067 290a 0a59 6f75 2061 7373 6f63 6961  pg)..You associa
+0001b2b0: 7465 204d 5154 5420 746f 7069 6320 6272  te MQTT topic br
+0001b2c0: 616e 6368 6573 2074 6f20 6170 706c 6963  anches to applic
+0001b2d0: 6174 696f 6e73 2069 6e20 7468 6520 636f  ations in the co
+0001b2e0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+0001b2f0: 2028 636f 7079 2060 6d71 7474 7761 726e   (copy `mqttwarn
+0001b300: 2e69 6e69 2e73 616d 706c 6560 2074 6f20  .ini.sample` to 
+0001b310: 606d 7174 7477 6172 6e2e 696e 6960 2066  `mqttwarn.ini` f
+0001b320: 6f72 2075 7365 292e 2049 6e20 6f74 6865  or use). In othe
+0001b330: 7220 776f 7264 732c 2079 6f75 2063 616e  r words, you can
+0001b340: 2061 6363 6f6d 706c 6973 682c 2073 6179   accomplish, say
+0001b350: 2c20 666f 6c6c 6f77 696e 6720 6d61 7070  , following mapp
+0001b360: 696e 6773 3a0a 0a2a 2050 5542 7320 746f  ings:..* PUBs to
+0001b370: 2060 6f77 6e74 7261 636b 732f 6a61 6e65   `owntracks/jane
+0001b380: 2f69 7068 6f6e 6560 2073 686f 756c 6420  /iphone` should 
+0001b390: 6265 206e 6f74 6966 6965 6420 7669 6120  be notified via 
+0001b3a0: 5075 7368 6f76 6572 2074 6f20 4a6f 686e  Pushover to John
+0001b3b0: 2773 2070 686f 6e65 0a2a 2050 5542 7320  's phone.* PUBs 
+0001b3c0: 746f 2060 6f70 656e 6861 622f 7465 6d70  to `openhab/temp
+0001b3d0: 6572 6174 7572 6560 2073 686f 756c 6420  erature` should 
+0001b3e0: 6265 2054 7765 6574 6564 0a2a 2050 5542  be Tweeted.* PUB
+0001b3f0: 7320 746f 2060 686f 6d65 2f6d 6f6e 6974  s to `home/monit
+0001b400: 6f72 696e 672f 616c 6572 742f 2b60 2073  oring/alert/+` s
+0001b410: 686f 756c 6420 6e6f 7469 6679 2054 7769  hould notify Twi
+0001b420: 7474 6572 2c20 4d61 696c 2c20 616e 6420  tter, Mail, and 
+0001b430: 5072 6f77 6c0a 0a53 6565 2064 6574 6169  Prowl..See detai
+0001b440: 6c73 2069 6e20 7468 6520 636f 6e66 6967  ls in the config
+0001b450: 2073 616d 706c 6520 666f 7220 686f 7720   sample for how 
+0001b460: 746f 2063 6f6e 6669 6775 7265 2074 6869  to configure thi
+0001b470: 7320 7363 7269 7074 2e0a 5468 6520 7061  s script..The pa
+0001b480: 7468 2074 6f20 7468 6520 636f 6e66 6967  th to the config
+0001b490: 7572 6174 696f 6e20 6669 6c65 2028 7768  uration file (wh
+0001b4a0: 6963 6820 6d75 7374 2062 6520 7661 6c69  ich must be vali
+0001b4b0: 6420 5079 7468 6f6e 2920 6973 206f 6274  d Python) is obt
+0001b4c0: 6169 6e65 6420 6672 6f6d 2074 6865 2060  ained from the `
+0001b4d0: 4d51 5454 5741 524e 494e 4960 2065 6e76  MQTTWARNINI` env
+0001b4e0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+0001b4f0: 6520 7768 6963 6820 6465 6661 756c 7473  e which defaults
+0001b500: 2074 6f20 606d 7174 7477 6172 6e2e 696e   to `mqttwarn.in
+0001b510: 6960 2069 6e20 7468 6520 6375 7272 656e  i` in the curren
+0001b520: 7420 6469 7265 6374 6f72 792e 0a0a 4576  t directory...Ev
+0001b530: 656e 206d 6f72 6520 6164 7661 6e63 6564  en more advanced
+0001b540: 2c20 7768 656e 2072 6563 6569 7669 6e67  , when receiving
+0001b550: 204a 534f 4e20 6461 7461 206c 696b 6520   JSON data like 
+0001b560: 607b 2264 6174 6122 3a20 7b22 6875 6d69  `{"data": {"humi
+0001b570: 6469 7479 223a 2036 322e 3138 7d7d 602c  dity": 62.18}}`,
+0001b580: 2079 6f75 206d 6967 6874 0a77 616e 7420   you might.want 
+0001b590: 746f 2065 7874 7261 6374 2076 616c 7565  to extract value
+0001b5a0: 7320 7573 696e 6720 7468 6520 6066 6f72  s using the `for
+0001b5b0: 6d61 7460 206d 6563 6861 6e69 736d 2062  mat` mechanism b
+0001b5c0: 6566 6f72 6520 666f 7277 6172 6469 6e67  efore forwarding
+0001b5d0: 0a69 7420 746f 206f 7468 6572 2064 6174  .it to other dat
+0001b5e0: 6120 7369 6e6b 732c 206c 696b 650a 0a60  a sinks, like..`
+0001b5f0: 6060 696e 690a 666f 726d 6174 203d 2022  ``ini.format = "
+0001b600: 7b64 6174 617d 220a 6060 600a 0a48 6f77  {data}".```..How
+0001b610: 6576 6572 2c20 7468 6520 6f75 7463 6f6d  ever, the outcom
+0001b620: 6520 7769 6c6c 2062 6520 7468 6520 7374  e will be the st
+0001b630: 7269 6e67 2d73 6572 6961 6c69 7a65 6420  ring-serialized 
+0001b640: 666f 726d 206f 6620 7468 6520 5079 7468  form of the Pyth
+0001b650: 6f6e 0a72 6570 7265 7365 6e74 6174 696f  on.representatio
+0001b660: 6e3a 2060 7b75 2768 756d 6964 6974 7927  n: `{u'humidity'
+0001b670: 3a20 3632 2e31 387d 602c 2077 6869 6368  : 62.18}`, which
+0001b680: 2063 6f75 6c64 206e 6f74 2062 6520 7768   could not be wh
+0001b690: 6174 2079 6f75 0a77 616e 7420 6966 2079  at you.want if y
+0001b6a0: 6f75 7220 6461 7461 2073 696e 6b20 6973  our data sink is
+0001b6b0: 2065 7870 6563 7469 6e67 204a 534f 4e20   expecting JSON 
+0001b6c0: 666f 726d 6174 2061 6761 696e 2e0a 0a54  format again...T
+0001b6d0: 6f20 6163 6869 6576 6520 7468 6973 2c20  o achieve this, 
+0001b6e0: 796f 7520 7368 6f75 6c64 2075 7365 2061  you should use a
+0001b6f0: 7070 726f 7072 6961 7465 2074 7970 6520  ppropriate type 
+0001b700: 636f 6572 6369 6f6e 2062 6566 6f72 650a  coercion before.
+0001b710: 666f 726d 6174 7469 6e67 2c20 6c69 6b65  formatting, like
+0001b720: 0a0a 6060 6069 6e69 0a66 6f72 6d61 7420  ..```ini.format 
+0001b730: 3d20 227b 6461 7461 216a 7d22 0a60 6060  = "{data!j}".```
+0001b740: 0a0a 5468 6973 2077 696c 6c20 7365 7269  ..This will seri
+0001b750: 616c 697a 6520 7468 6520 666f 726d 6174  alize the format
+0001b760: 7465 6420 6461 7461 2074 6f20 4a53 4f4e  ted data to JSON
+0001b770: 2066 6f72 6d61 7420 6170 7072 6f70 7269   format appropri
+0001b780: 6174 656c 792c 0a73 6f20 7468 6520 6f75  ately,.so the ou
+0001b790: 7463 6f6d 6520 7769 6c6c 2062 6520 607b  tcome will be `{
+0001b7a0: 2268 756d 6964 6974 7922 3a20 3632 2e31  "humidity": 62.1
+0001b7b0: 387d 602e 0a0a 2323 2323 204e 6573 7465  8}`...#### Neste
+0001b7c0: 6420 4a53 4f4e 0a0a 5769 7468 696e 2074  d JSON..Within t
+0001b7d0: 656d 706c 6174 6573 2061 6e64 2066 6f72  emplates and for
+0001b7e0: 6d61 7473 2c20 796f 7520 6361 6e20 7265  mats, you can re
+0001b7f0: 6665 7220 6f6e 6c79 2074 6f20 7468 6520  fer only to the 
+0001b800: 746f 702d 6c65 7665 6c20 6e61 6d65 7320  top-level names 
+0001b810: 6f66 2061 6e20 696e 636f 6d69 6e67 204a  of an incoming J
+0001b820: 534f 4e20 6d65 7373 6167 652c 0a77 6869  SON message,.whi
+0001b830: 6368 2073 6967 6e69 6669 6361 6e74 6c79  ch significantly
+0001b840: 206c 696d 6974 7320 7468 6520 6b69 6e64   limits the kind
+0001b850: 7320 6f66 206d 6573 7361 6765 7320 606d  s of messages `m
+0001b860: 7174 7477 6172 6e60 2063 616e 2070 726f  qttwarn` can pro
+0001b870: 6365 7373 2e20 4120 5b73 6f6c 7574 696f  cess. A [solutio
+0001b880: 6e20 6973 2069 6e20 7468 6520 776f 726b  n is in the work
+0001b890: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+0001b8a0: 622e 636f 6d2f 6a70 6d65 6e73 2f6d 7174  b.com/jpmens/mqt
+0001b8b0: 7477 6172 6e2f 6973 7375 6573 2f33 3033  twarn/issues/303
+0001b8c0: 290a 666f 7220 7468 6973 2c20 6275 7420  ).for this, but 
+0001b8d0: 696e 2074 6865 206d 6561 6e74 696d 6520  in the meantime 
+0001b8e0: 796f 7520 6361 6e20 7573 6520 616e 2060  you can use an `
+0001b8f0: 616c 6c64 6174 6160 2066 756e 6374 696f  alldata` functio
+0001b900: 6e20 746f 2074 7261 6e73 666f 726d 2074  n to transform t
+0001b910: 6865 204a 534f 4e20 696e 746f 2073 6f6d  he JSON into som
+0001b920: 6574 6869 6e67 200a 606d 7174 7477 6172  ething .`mqttwar
+0001b930: 6e60 205f 6361 6e5f 2070 726f 6365 7373  n` _can_ process
+0001b940: 2e0a 0a54 6865 2074 7269 636b 2069 7320  ...The trick is 
+0001b950: 746f 2062 7569 6c64 2061 206e 6577 204a  to build a new J
+0001b960: 534f 4e20 6d65 7373 6167 6520 7769 7468  SON message with
+0001b970: 205f 6f6e 6c79 5f20 746f 702d 6c65 7665   _only_ top-leve
+0001b980: 6c20 7661 6c75 6573 2c20 7370 6563 6966  l values, specif
+0001b990: 6963 616c 6c79 2074 6865 2076 616c 7565  ically the value
+0001b9a0: 7320 796f 7520 6e65 6564 2e0a 0a23 2323  s you need...###
+0001b9b0: 2043 7573 746f 6d20 6675 6e63 7469 6f6e   Custom function
+0001b9c0: 730a 0a41 2074 6f70 6963 2073 6563 7469  s..A topic secti
+0001b9d0: 6f6e 2069 6e20 7468 6520 494e 4920 6669  on in the INI fi
+0001b9e0: 6c65 2063 616e 2068 6176 6520 7072 6f70  le can have prop
+0001b9f0: 6572 7469 6573 2073 6574 2061 7320 7065  erties set as pe
+0001ba00: 7220 7468 6520 7461 626c 6520 6174 2074  r the table at t
+0001ba10: 6865 2062 6f74 746f 6d20 6f66 205b 7468  he bottom of [th
+0001ba20: 6973 2073 6563 7469 6f6e 5d28 6874 7470  is section](http
+0001ba30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+0001ba40: 706d 656e 732f 6d71 7474 7761 726e 2374  pmens/mqttwarn#t
+0001ba50: 6865 2d5f 5f74 6f70 6963 5f5f 2d73 6563  he-__topic__-sec
+0001ba60: 7469 6f6e 7329 2e20 5468 6520 6074 6172  tions). The `tar
+0001ba70: 6765 7473 602c 2060 746f 7069 6360 2061  gets`, `topic` a
+0001ba80: 6e64 2060 716f 7360 2070 726f 7065 7274  nd `qos` propert
+0001ba90: 6965 7320 6361 6e20 6e6f 7420 6265 2064  ies can not be d
+0001baa0: 6566 696e 6564 2077 6974 6820 6120 6675  efined with a fu
+0001bab0: 6e63 7469 6f6e 2e20 0a0a 2323 2323 2054  nction. ..#### T
+0001bac0: 6f70 6963 2d73 6563 7469 6f6e 2070 726f  opic-section pro
+0001bad0: 7065 7274 6965 7320 7468 6174 2063 616e  perties that can
+0001bae0: 2063 616c 6c20 6120 6375 7374 6f6d 2066   call a custom f
+0001baf0: 756e 6374 696f 6e0a 0a2d 2060 6461 7461  unction..- `data
+0001bb00: 6d61 7060 203a 2064 6963 7469 6f6e 6172  map` : dictionar
+0001bb10: 792c 206f 7220 6120 6675 6e63 7469 6f6e  y, or a function
+0001bb20: 2074 6861 7420 7265 7475 726e 7320 6120   that returns a 
+0001bb30: 6469 6374 696f 6e61 7279 0a2d 2060 616c  dictionary.- `al
+0001bb40: 6c64 6174 6160 203a 2064 6963 7469 6f6e  ldata` : diction
+0001bb50: 6172 792c 206f 7220 6120 6675 6e63 7469  ary, or a functi
+0001bb60: 6f6e 2074 6861 7420 7265 7475 726e 7320  on that returns 
+0001bb70: 6120 6469 6374 696f 6e61 7279 0a2d 2060  a dictionary.- `
+0001bb80: 6669 6c74 6572 6020 3a20 626f 6f6c 6561  filter` : boolea
+0001bb90: 6e2c 206f 7220 6120 6675 6e63 7469 6f6e  n, or a function
+0001bba0: 2074 6861 7420 7265 7475 726e 7320 6120   that returns a 
+0001bbb0: 626f 6f6c 6561 6e0a 2d20 6074 6974 6c65  boolean.- `title
+0001bbc0: 6020 3a20 7374 7269 6e67 2c20 6f72 2061  ` : string, or a
+0001bbd0: 2066 756e 6374 696f 6e20 7468 6174 2072   function that r
+0001bbe0: 6574 7572 6e73 2061 2073 7472 696e 670a  eturns a string.
+0001bbf0: 2d20 6066 6f72 6d61 7460 203a 2073 7472  - `format` : str
+0001bc00: 696e 672c 206f 7220 6120 6675 6e63 7469  ing, or a functi
+0001bc10: 6f6e 2074 6861 7420 7265 7475 726e 7320  on that returns 
+0001bc20: 6120 7374 7269 6e67 0a2d 2060 7072 696f  a string.- `prio
+0001bc30: 7269 7479 6020 3a20 7365 6520 6265 6c6f  rity` : see belo
+0001bc40: 770a 2d20 6069 6d61 6765 6020 3a20 7365  w.- `image` : se
+0001bc50: 6520 6265 6c6f 770a 0a23 2323 2320 4461  e below..#### Da
+0001bc60: 7461 206d 6170 7069 6e67 2066 756e 6374  ta mapping funct
+0001bc70: 696f 6e73 0a0a 426f 7468 2074 6865 2060  ions..Both the `
+0001bc80: 6461 7461 6d61 7060 2061 6e64 2074 6865  datamap` and the
+0001bc90: 2060 616c 6c64 6174 6160 2070 726f 7065   `alldata` prope
+0001bca0: 7274 6965 7320 696e 2061 2074 6f70 6963  rties in a topic
+0001bcb0: 2073 6563 7469 6f6e 2063 616e 2063 616c   section can cal
+0001bcc0: 6c20 6120 6675 6e63 7469 6f6e 2077 6869  l a function whi
+0001bcd0: 6368 2072 6574 7572 6e73 2061 205b 6469  ch returns a [di
+0001bce0: 6374 696f 6e61 7279 5d28 6874 7470 733a  ctionary](https:
+0001bcf0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+0001bd00: 672f 322f 7475 746f 7269 616c 2f64 6174  g/2/tutorial/dat
+0001bd10: 6173 7472 7563 7475 7265 732e 6874 6d6c  astructures.html
+0001bd20: 2364 6963 7469 6f6e 6172 6965 7329 2e20  #dictionaries). 
+0001bd30: 5468 6520 6b65 7973 2069 6e20 7468 6973  The keys in this
+0001bd40: 2064 6963 7469 6f6e 6172 7920 6361 6e20   dictionary can 
+0001bd50: 6265 2075 7365 6420 7768 656e 2064 6573  be used when des
+0001bd60: 6372 6962 696e 6720 7468 6520 6f75 7462  cribing the outb
+0001bd70: 6f75 6e64 2060 7469 746c 6560 2061 6e64  ound `title` and
+0001bd80: 2060 666f 726d 6174 6020 7072 6f70 6572   `format` proper
+0001bd90: 7469 6573 206f 6620 7468 6520 7361 6d65  ties of the same
+0001bda0: 2074 6f70 6963 2073 6563 7469 6f6e 2e0a   topic section..
+0001bdb0: 0a2d 2060 746f 7069 6360 3a20 636f 6e74  .- `topic`: cont
+0001bdc0: 6169 6e73 2074 6865 2076 616c 7565 2069  ains the value i
+0001bdd0: 6e20 6064 6174 615b 2774 6f70 6963 275d  n `data['topic']
+0001bde0: 600a 2d20 6064 6174 6160 3a20 7072 6f76  `.- `data`: prov
+0001bdf0: 6964 6573 2061 6363 6573 7320 746f 2073  ides access to s
+0001be00: 6f6d 6520 696e 666f 726d 6174 696f 6e20  ome information 
+0001be10: 6f66 2074 6865 2069 6e62 6f75 6e64 204d  of the inbound M
+0001be20: 5154 5420 7472 616e 736d 6973 7369 6f6e  QTT transmission
+0001be30: 2c20 5b6d 6f72 6520 6465 7461 696c 2068  , [more detail h
+0001be40: 6572 655d 2868 7474 7073 3a2f 2f67 6974  ere](https://git
+0001be50: 6875 622e 636f 6d2f 6a70 6d65 6e73 2f6d  hub.com/jpmens/m
+0001be60: 7174 7477 6172 6e23 7472 616e 7366 6f72  qttwarn#transfor
+0001be70: 6d61 7469 6f6e 2d64 6174 6129 0a2d 2060  mation-data).- `
+0001be80: 7365 7276 6963 6560 3a20 7072 6f76 6964  service`: provid
+0001be90: 6573 2061 6363 6573 7320 746f 2074 6865  es access to the
+0001bea0: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+0001beb0: 2060 7061 686f 2e6d 7174 742e 636c 6965   `paho.mqtt.clie
+0001bec0: 6e74 2e43 6c69 656e 7460 206f 626a 6563  nt.Client` objec
+0001bed0: 7420 2877 6869 6368 2070 726f 7669 6465  t (which provide
+0001bee0: 7320 6120 706c 6574 686f 7261 206f 6620  s a plethora of 
+0001bef0: 7072 6f70 6572 7469 6573 2061 6e64 206d  properties and m
+0001bf00: 6574 686f 6473 292c 2074 6f20 7468 6520  ethods), to the 
+0001bf10: 606d 7174 7477 6172 6e60 206c 6f67 6769  `mqttwarn` loggi
+0001bf20: 6e67 2073 6574 7570 2c20 746f 2074 6865  ng setup, to the
+0001bf30: 2050 7974 686f 6e20 6067 6c6f 6261 6c73   Python `globals
+0001bf40: 2829 6020 6d65 7468 6f64 2061 6e64 2061  ()` method and a
+0001bf50: 6c6c 2074 6861 7420 656e 7461 696c 732c  ll that entails,
+0001bf60: 2061 6e64 2074 6f20 7468 6520 6e61 6d65   and to the name
+0001bf70: 206f 6620 7468 6520 7363 7269 7074 2e20   of the script. 
+0001bf80: 0a0a 2323 2323 2046 696c 7465 7220 6675  ..#### Filter fu
+0001bf90: 6e63 7469 6f6e 730a 0a41 2066 756e 6374  nctions..A funct
+0001bfa0: 696f 6e20 6361 6c6c 6564 2066 726f 6d20  ion called from 
+0001bfb0: 7468 6520 6066 696c 7465 7260 2070 726f  the `filter` pro
+0001bfc0: 7065 7274 7920 696e 2061 2074 6f70 6963  perty in a topic
+0001bfd0: 2073 6563 7469 6f6e 206e 6565 6473 2074   section needs t
+0001bfe0: 6f20 7265 7475 726e 2060 4661 6c73 6560  o return `False`
+0001bff0: 2074 6f20 7374 6f70 2074 6865 206f 7574   to stop the out
+0001c000: 626f 756e 6420 6e6f 7469 6669 6361 7469  bound notificati
+0001c010: 6f6e 2e20 4974 2068 6173 2061 6363 6573  on. It has acces
+0001c020: 7320 746f 2074 6865 2060 746f 7069 6360  s to the `topic`
+0001c030: 2061 6e64 2074 6865 2060 6d65 7373 6167   and the `messag
+0001c040: 6560 2073 7472 696e 6773 206f 6620 7468  e` strings of th
+0001c050: 6520 696e 626f 756e 6420 4d51 5454 2074  e inbound MQTT t
+0001c060: 7261 6e73 6d69 7373 696f 6e2e 200a 0a23  ransmission. ..#
+0001c070: 2323 2320 4f75 7470 7574 2066 756e 6374  ### Output funct
+0001c080: 696f 6e73 0a0a 426f 7468 2074 6865 2060  ions..Both the `
+0001c090: 7469 746c 6560 2061 6e64 2074 6865 2060  title` and the `
+0001c0a0: 666f 726d 6174 6020 7072 6f70 6572 7469  format` properti
+0001c0b0: 6573 2069 6e20 7468 6520 746f 7069 6320  es in the topic 
+0001c0c0: 7365 6374 696f 6e20 6361 6e20 636f 6e74  section can cont
+0001c0d0: 6169 6e20 6120 7374 7269 6e67 2077 6865  ain a string whe
+0001c0e0: 7265 2060 7b62 7261 636b 6574 6564 7d60  re `{bracketed}`
+0001c0f0: 2072 6566 6572 656e 6365 7320 6765 7420   references get 
+0001c100: 7265 736f 6c76 6564 2075 7369 6e67 2074  resolved using t
+0001c110: 6865 2064 6963 7469 6f6e 6172 7920 7265  he dictionary re
+0001c120: 7475 726e 6564 2066 726f 6d20 6120 6461  turned from a da
+0001c130: 7461 206d 6170 7069 6e67 2066 756e 6374  ta mapping funct
+0001c140: 696f 6e2e 204f 7220 7468 6579 2063 616e  ion. Or they can
+0001c150: 2063 616c 6c20 6120 6675 6e63 7469 6f6e   call a function
+0001c160: 2074 6861 7420 7265 7475 726e 7320 6120   that returns a 
+0001c170: 7374 7269 6e67 2074 6861 7420 6d61 7920  string that may 
+0001c180: 6f72 206d 6179 206e 6f74 2063 6f6e 7461  or may not conta
+0001c190: 696e 2073 7563 6820 7265 6665 7265 6e63  in such referenc
+0001c1a0: 6573 2e20 5468 6520 6675 6e63 7469 6f6e  es. The function
+0001c1b0: 7320 6361 6c6c 6564 2068 6572 6520 646f  s called here do
+0001c1c0: 206e 6f74 2068 6176 6520 6163 6365 7373   not have access
+0001c1d0: 2074 6f20 7468 6520 6163 7475 616c 2064   to the actual d
+0001c1e0: 6963 7469 6f6e 6172 7920 7265 7475 726e  ictionary return
+0001c1f0: 6564 2066 726f 6d20 6461 7461 206d 6170  ed from data map
+0001c200: 7069 6e67 2066 756e 6374 696f 6e73 2074  ping functions t
+0001c210: 686f 7567 682e 0a0a 2323 2323 204e 6f74  hough...#### Not
+0001c220: 6573 0a0a 5768 656e 2077 7269 7469 6e67  es..When writing
+0001c230: 2063 7573 746f 6d20 6675 6e63 7469 6f6e   custom function
+0001c240: 732c 2069 7420 6361 6e20 6265 2064 6966  s, it can be dif
+0001c250: 6669 6375 6c74 2074 6f20 6465 7465 726d  ficult to determ
+0001c260: 696e 6520 7768 6174 2074 6865 2069 7373  ine what the iss
+0001c270: 7565 2069 7320 7768 656e 2067 6574 7469  ue is when getti
+0001c280: 6e67 2061 6e20 6572 726f 7220 6d65 7373  ng an error mess
+0001c290: 6167 6520 7375 6368 2061 730a 0a60 6060  age such as..```
+0001c2a0: 0a57 4152 4e49 4e47 205b 6d71 7474 7761  .WARNING [mqttwa
+0001c2b0: 726e 5d20 4361 6e6e 6f74 2069 6e76 6f6b  rn] Cannot invok
+0001c2c0: 6520 6669 6c74 6572 2066 756e 6374 696f  e filter functio
+0001c2d0: 6e20 7878 7878 2064 6566 696e 6564 2069  n xxxx defined i
+0001c2e0: 6e20 7979 7979 793a 202e 2e2e 0a60 6060  n yyyyy: ....```
+0001c2f0: 0a0a 5468 6973 2069 7320 7479 7069 6361  ..This is typica
+0001c300: 6c6c 7920 696e 6469 6361 7465 7320 7661  lly indicates va
+0001c310: 7269 6162 6c65 7320 6f72 2066 756e 6374  riables or funct
+0001c320: 696f 6e20 6361 6c6c 7320 7768 6963 6820  ion calls which 
+0001c330: 6861 7665 6e27 7420 6265 656e 2064 6566  haven't been def
+0001c340: 696e 6564 206f 7220 7369 6d69 6c61 722e  ined or similar.
+0001c350: 0a0a 2323 2323 2045 7861 6d70 6c65 730a  ..#### Examples.
+0001c360: 0a42 656c 6f77 2061 7265 2061 206e 756d  .Below are a num
+0001c370: 6265 7220 6f66 2065 7861 6d70 6c65 2073  ber of example s
+0001c380: 6365 6e61 7269 6f73 2077 6865 7265 2063  cenarios where c
+0001c390: 7573 746f 6d20 6675 6e63 7469 6f6e 7320  ustom functions 
+0001c3a0: 6172 6520 6265 696e 6720 7573 6564 2e0a  are being used..
+0001c3b0: 0a23 2323 2323 2055 7369 6e67 2066 756e  .##### Using fun
+0001c3c0: 6374 696f 6e73 2074 6f20 7265 706c 6163  ctions to replac
+0001c3d0: 6520 696e 636f 6d69 6e67 2070 6179 6c6f  e incoming paylo
+0001c3e0: 6164 730a 0a43 6f6e 7369 6465 7220 7468  ads..Consider th
+0001c3f0: 6520 666f 6c6c 6f77 696e 6720 636f 6e66  e following conf
+0001c400: 6967 7572 6174 696f 6e20 736e 6970 7065  iguration snippe
+0001c410: 7420 696e 2061 6464 6974 696f 6e20 746f  t in addition to
+0001c420: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+0001c430: 6f6e 0a6f 6620 7468 6520 606d 7174 7460  on.of the `mqtt`
+0001c440: 2073 6572 7669 6365 2073 686f 776e 2061   service shown a
+0001c450: 626f 7665 3a0a 0a41 6464 2074 6869 7320  bove:..Add this 
+0001c460: 746f 2061 2063 7573 746f 6d20 5079 7468  to a custom Pyth
+0001c470: 6f6e 2066 696c 652c 206c 696b 652c 2065  on file, like, e
+0001c480: 2e67 2e20 602f 6574 632f 6d71 7474 7761  .g. `/etc/mqttwa
+0001c490: 726e 2f6d 7966 756e 6374 696f 6e73 2e70  rn/myfunctions.p
+0001c4a0: 7960 2e0a 6060 6070 7974 686f 6e0a 6465  y`..```python.de
+0001c4b0: 6620 6c6f 6f6b 7570 5f64 6174 6128 6461  f lookup_data(da
+0001c4c0: 7461 2c20 7372 763d 4e6f 6e65 293a 0a20  ta, srv=None):. 
+0001c4d0: 2020 2069 6620 7479 7065 2864 6174 6129     if type(data)
+0001c4e0: 203d 3d20 6469 6374 2061 6e64 2027 6672   == dict and 'fr
+0001c4f0: 7569 7427 2069 6e20 6461 7461 3a0a 2020  uit' in data:.  
+0001c500: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001c510: 2022 416e 616e 6173 220a 2020 2020 7265   "Ananas".    re
+0001c520: 7475 726e 204e 6f6e 650a 6060 600a 0a52  turn None.```..R
+0001c530: 6567 6973 7465 7220 7468 6174 2066 696c  egister that fil
+0001c540: 6520 6279 2073 6179 696e 673a 0a0a 6060  e by saying:..``
+0001c550: 6069 6e69 0a5b 6465 6661 756c 7473 5d0a  `ini.[defaults].
+0001c560: 3b20 7061 7468 2074 6f20 6669 6c65 2063  ; path to file c
+0001c570: 6f6e 7461 696e 696e 6720 7365 6c66 2d64  ontaining self-d
+0001c580: 6566 696e 6564 2066 756e 6374 696f 6e73  efined functions
+0001c590: 2066 6f72 2066 6f72 6d61 746d 6170 2061   for formatmap a
+0001c5a0: 6e64 2064 6174 616d 6170 0a66 756e 6374  nd datamap.funct
+0001c5b0: 696f 6e73 203d 2027 6d79 6675 6e63 7469  ions = 'myfuncti
+0001c5c0: 6f6e 732e 7079 270a 6060 600a 0a54 6865  ons.py'.```..The
+0001c5d0: 6e2c 2069 6e20 7468 6520 7365 6374 696f  n, in the sectio
+0001c5e0: 6e20 6465 6669 6e69 6e67 2074 6865 2074  n defining the t
+0001c5f0: 6f70 6963 2077 6520 6c69 7374 656e 206f  opic we listen o
+0001c600: 6e3a 0a0a 6060 6069 6e69 0a2e 2e2e 0a5b  n:..```ini.....[
+0001c610: 7465 7374 2f74 6f70 6963 5d0a 2366 6f72  test/topic].#for
+0001c620: 6d61 7420 3d20 2053 696e 6365 2077 6865  mat =  Since whe
+0001c630: 6e20 646f 6573 2061 207b 6672 7569 747d  n does a {fruit}
+0001c640: 2063 6f73 7420 7b70 7269 6365 7d3f 0a66   cost {price}?.f
+0001c650: 6f72 6d61 7420 3d20 206c 6f6f 6b75 705f  ormat =  lookup_
+0001c660: 6461 7461 2829 0a60 6060 0a0a 4865 7265  data().```..Here
+0001c670: 2c20 7765 2072 6570 6c61 6365 6420 7468  , we replaced th
+0001c680: 6520 6066 6f72 6d61 746d 6170 6020 656e  e `formatmap` en
+0001c690: 7472 7920 666f 7220 7468 6520 746f 7069  try for the topi
+0001c6a0: 6320 6279 2061 2063 7573 746f 6d20 6675  c by a custom fu
+0001c6b0: 6e63 7469 6f6e 2e0a 0a54 6865 7365 2066  nction...These f
+0001c6c0: 756e 6374 696f 6e73 2061 7265 2069 6e76  unctions are inv
+0001c6d0: 6f6b 6564 2077 6974 6820 6465 636f 6465  oked with decode
+0001c6e0: 6420 4a53 4f4e 2060 6461 7461 6020 7061  d JSON `data` pa
+0001c6f0: 7373 6564 2074 6f20 7468 656d 2061 7320  ssed to them as 
+0001c700: 610a 5f64 6963 745f 2e20 5468 6520 7374  a._dict_. The st
+0001c710: 7269 6e67 2072 6574 7572 6e65 6420 2062  ring returned  b
+0001c720: 7920 7468 6520 6675 6e63 7469 6f6e 2072  y the function r
+0001c730: 6574 7572 6e65 6420 7374 7269 6e67 2072  eturned string r
+0001c740: 6570 6c61 6365 7320 7468 650a 6f75 7467  eplaces the.outg
+0001c750: 6f69 6e67 2060 6d65 7373 6167 6560 3a0a  oing `message`:.
+0001c760: 0a60 6060 0a69 6e2f 6131 207b 2266 7275  .```.in/a1 {"fru
+0001c770: 6974 223a 2270 696e 6561 7070 6c65 222c  it":"pineapple",
+0001c780: 2022 7072 6963 6522 3a20 3133 312c 2022   "price": 131, "
+0001c790: 7473 7422 203a 2022 3133 3931 3737 3933  tst" : "13917793
+0001c7a0: 3336 227d 0a6f 7574 2f66 6f6f 6420 416e  36"}.out/food An
+0001c7b0: 616e 6173 0a6f 7574 2f66 7275 6974 2f70  anas.out/fruit/p
+0001c7c0: 696e 6561 7070 6c65 2041 6e61 6e61 730a  ineapple Ananas.
+0001c7d0: 6060 600a 0a59 6f75 2063 616e 2064 6566  ```..You can def
+0001c7e0: 696e 6520 6375 7374 6f6d 2066 756e 6374  ine custom funct
+0001c7f0: 696f 6e73 2069 6e20 6120 5079 7468 6f6e  ions in a Python
+0001c800: 2066 696c 6520 7768 6963 6820 796f 7520   file which you 
+0001c810: 636f 6e66 6967 7572 6520 6173 0a60 6675  configure as.`fu
+0001c820: 6e63 7469 6f6e 7360 2069 6e20 7468 6520  nctions` in the 
+0001c830: 605b 6465 6661 756c 745d 6020 7365 6374  `[default]` sect
+0001c840: 696f 6e20 6f66 2074 6865 2060 6d71 7474  ion of the `mqtt
+0001c850: 7761 726e 2e69 6e69 6020 636f 6e66 6967  warn.ini` config
+0001c860: 7572 6174 696f 6e0a 6669 6c65 2c20 6173  uration.file, as
+0001c870: 206f 7574 6c69 6e65 6420 6162 6f76 652e   outlined above.
+0001c880: 2057 6865 6e20 7265 6c61 7469 7665 2066   When relative f
+0001c890: 696c 6520 6e61 6d65 7320 6172 6520 6769  ile names are gi
+0001c8a0: 7665 6e2c 2074 6865 7920 7769 6c6c 2062  ven, they will b
+0001c8b0: 650a 7265 736f 6c76 6564 2066 726f 6d20  e.resolved from 
+0001c8c0: 7468 6520 6469 7265 6374 6f72 7920 6f66  the directory of
+0001c8d0: 2074 6865 2060 6d71 7474 7761 726e 2e69   the `mqttwarn.i
+0001c8e0: 6e69 6020 6669 6c65 2c20 7768 6963 6820  ni` file, which 
+0001c8f0: 6973 2c20 6279 2064 6566 6175 6c74 2c0a  is, by default,.
+0001c900: 7468 6520 602f 6574 632f 6d71 7474 7761  the `/etc/mqttwa
+0001c910: 726e 6020 666f 6c64 6572 2e0a 0a49 6620  rn` folder...If 
+0001c920: 6120 6675 6e63 7469 6f6e 206f 7065 7261  a function opera
+0001c930: 7469 6e67 206f 6e20 6120 6d65 7373 6167  ting on a messag
+0001c940: 6520 2869 2e65 2e20 7769 7468 696e 2060  e (i.e. within `
+0001c950: 666f 726d 6174 203d 6029 2072 6574 7572  format =`) retur
+0001c960: 6e73 2060 4e6f 6e65 6020 6f72 2061 6e20  ns `None` or an 
+0001c970: 656d 7074 7920 7374 7269 6e67 2c20 7468  empty string, th
+0001c980: 6520 7461 7267 6574 206e 6f74 6966 6963  e target notific
+0001c990: 6174 696f 6e20 6973 2073 7570 7072 6573  ation is suppres
+0001c9a0: 7365 642e 0a0a 5468 6520 6f70 7469 6f6e  sed...The option
+0001c9b0: 616c 2060 7372 7660 2069 7320 616e 206f  al `srv` is an o
+0001c9c0: 626a 6563 7420 7769 7468 2073 6f6d 6520  bject with some 
+0001c9d0: 6865 6c70 6572 2066 756e 6374 696f 6e73  helper functions
+0001c9e0: 2e20 496e 2070 6172 7469 6375 6c61 722c  . In particular,
+0001c9f0: 2074 6865 7365 2061 6c6c 6f77 2075 7320   these allow us 
+0001ca00: 746f 2075 7365 205f 6d71 7474 7761 726e  to use _mqttwarn
+0001ca10: 5f27 7320 6c6f 6767 696e 6720 616e 6420  _'s logging and 
+0001ca20: 4d51 5454 2070 7562 6c69 7368 2066 756e  MQTT publish fun
+0001ca30: 6374 696f 6e73 2c20 6173 2069 6e20 7468  ctions, as in th
+0001ca40: 6973 2065 7861 6d70 6c65 3a0a 0a60 6060  is example:..```
+0001ca50: 7079 7468 6f6e 0a64 6566 2070 3031 466f  python.def p01Fo
+0001ca60: 726d 6174 2864 6174 612c 2073 7276 293a  rmat(data, srv):
+0001ca70: 0a20 2020 2073 203d 2022 7030 312d 484f  .    s = "p01-HO
+0001ca80: 4c41 220a 0a20 2020 2073 7276 2e6c 6f67  LA"..    srv.log
+0001ca90: 6769 6e67 2e69 6e66 6f28 222b 2b2b 2b2b  ging.info("+++++
+0001caa0: 2b2b 2b2b 2b2b 2048 5548 5522 290a 0a20  ++++++ HUHU").. 
+0001cab0: 2020 2073 7276 2e6d 7174 7463 2e70 7562     srv.mqttc.pub
+0001cac0: 6c69 7368 2822 7030 312f 5245 5350 6f6e  lish("p01/RESPon
+0001cad0: 7365 222c 2073 2c20 716f 733d 302c 2072  se", s, qos=0, r
+0001cae0: 6574 6169 6e3d 4661 6c73 6529 0a0a 2020  etain=False)..  
+0001caf0: 2020 7265 7475 726e 2073 0a60 6060 0a0a    return s.```..
+0001cb00: 4265 2061 6476 6973 6564 2074 6861 7420  Be advised that 
+0001cb10: 6966 2079 6f75 204d 5154 5420 7075 626c  if you MQTT publ
+0001cb20: 6973 6820 6261 636b 2074 6f20 7468 6520  ish back to the 
+0001cb30: 7361 6d65 2074 6f70 6963 2077 6869 6368  same topic which
+0001cb40: 2074 7269 6767 6572 6564 2074 6865 2069   triggered the i
+0001cb50: 6e76 6f63 6174 696f 6e0a 6f66 2079 6f75  nvocation.of you
+0001cb60: 7220 6675 6e63 7469 6f6e 2c20 796f 7527  r function, you'
+0001cb70: 6c6c 2063 7265 6174 6520 616e 2065 6e64  ll create an end
+0001cb80: 6c65 7373 206c 6f6f 702e 0a0a 2323 2323  less loop...####
+0001cb90: 2320 496e 636f 7270 6f72 6174 696e 6720  # Incorporating 
+0001cba0: 746f 7069 6320 6e61 6d65 7320 696e 746f  topic names into
+0001cbb0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+0001cbc0: 6461 7461 0a0a 416e 204d 5154 5420 746f  data..An MQTT to
+0001cbd0: 7069 6320 6272 616e 6368 206e 616d 6520  pic branch name 
+0001cbe0: 636f 6e74 6169 6e73 2069 6e66 6f72 6d61  contains informa
+0001cbf0: 7469 6f6e 2079 6f75 206d 6179 2077 616e  tion you may wan
+0001cc00: 7420 746f 2075 7365 2069 6e20 7472 616e  t to use in tran
+0001cc10: 7366 6f72 6d61 7469 6f6e 732e 0a41 7320  sformations..As 
+0001cc20: 6120 7261 7468 6572 2065 7874 7265 6d65  a rather extreme
+0001cc30: 2065 7861 6d70 6c65 2c20 636f 6e73 6964   example, consid
+0001cc40: 6572 2074 6865 205b 4f77 6e54 7261 636b  er the [OwnTrack
+0001cc50: 735d 2070 726f 6772 616d 2028 7468 650a  s] program (the.
+0001cc60: 6172 7469 7374 2066 6f72 6d65 726c 7920  artist formerly 
+0001cc70: 6b6e 6f77 6e20 6173 205f 4d51 5454 6974  known as _MQTTit
+0001cc80: 7564 655f 292e 0a0a 5768 656e 2061 6e20  ude_)...When an 
+0001cc90: 5b4f 776e 5472 6163 6b73 5d20 6465 7669  [OwnTracks] devi
+0001cca0: 6365 2064 6574 6563 7473 2061 2063 6861  ce detects a cha
+0001ccb0: 6e67 6520 6f66 2061 2063 6f6e 6669 6775  nge of a configu
+0001ccc0: 7265 6420 7761 7970 6f69 6e74 206f 7220  red waypoint or 
+0001ccd0: 6765 6f2d 6665 6e63 6520 2861 2072 6567  geo-fence (a reg
+0001cce0: 696f 6e20 6d6f 6e69 746f 7269 6e67 2061  ion monitoring a
+0001ccf0: 2075 7365 7220 6361 6e20 7365 7420 7570   user can set up
+0001cd00: 206f 6e20 7468 6520 6465 7669 6365 292c   on the device),
+0001cd10: 2069 7420 656d 6974 7320 6120 4a53 4f4e   it emits a JSON
+0001cd20: 2070 6179 6c6f 6164 2077 6869 6368 206c   payload which l
+0001cd30: 6f6f 6b73 206c 696b 6520 7468 6973 2c20  ooks like this, 
+0001cd40: 6f6e 2061 2074 6f70 6963 206e 616d 6520  on a topic name 
+0001cd50: 636f 6e73 6973 7469 6e67 206f 6620 606f  consisting of `o
+0001cd60: 776e 7472 6163 6b73 2f5f 7573 6572 6e61  wntracks/_userna
+0001cd70: 6d65 5f2f 5f64 6576 6963 6569 645f 603a  me_/_deviceid_`:
+0001cd80: 0a0a 6060 600a 6f77 6e74 7261 636b 732f  ..```.owntracks/
+0001cd90: 6a61 6e65 2f70 686f 6e65 202d 6d20 277b  jane/phone -m '{
+0001cda0: 225f 7479 7065 223a 2022 6c6f 6361 7469  "_type": "locati
+0001cdb0: 6f6e 222c 2022 6c61 7422 3a20 2235 322e  on", "lat": "52.
+0001cdc0: 3437 3730 3335 3222 202e 2e20 2022 6465  4770352" ..  "de
+0001cdd0: 7363 223a 2022 486f 6d65 222c 2022 6576  sc": "Home", "ev
+0001cde0: 656e 7422 3a20 226c 6561 7665 227d 270a  ent": "leave"}'.
+0001cdf0: 6060 600a 0a49 6e20 6f72 6465 7220 746f  ```..In order to
+0001ce00: 2062 6520 6162 6c65 2074 6f20 6f62 7461   be able to obta
+0001ce10: 696e 2074 6865 2075 7365 726e 616d 6520  in the username 
+0001ce20: 2860 6a61 6e65 6029 2061 6e64 2068 6572  (`jane`) and her
+0001ce30: 2064 6576 6963 6520 6e61 6d65 2028 6070   device name (`p
+0001ce40: 686f 6e65 6029 2066 6f72 2075 7365 0a69  hone`) for use.i
+0001ce50: 6e20 7472 616e 7366 6f72 6d61 7469 6f6e  n transformation
+0001ce60: 7320 2873 6565 2070 7265 7669 6f75 7320  s (see previous 
+0001ce70: 7365 6374 696f 6e29 2c20 7765 2077 6f75  section), we wou
+0001ce80: 6c64 2069 6465 616c 6c79 2077 616e 7420  ld ideally want 
+0001ce90: 746f 2070 6172 7365 2074 6865 204d 5154  to parse the MQT
+0001cea0: 5420 746f 7069 6320 6e61 6d65 2061 6e64  T topic name and
+0001ceb0: 2061 6464 2074 6861 7420 746f 2074 6865   add that to the
+0001cec0: 2069 7465 6d20 6461 7461 206f 7572 2070   item data our p
+0001ced0: 6c75 6769 6e73 206f 6274 6169 6e2e 2059  lugins obtain. Y
+0001cee0: 6573 2c20 7765 2063 616e 2e0a 0a41 6e20  es, we can...An 
+0001cef0: 6f70 7469 6f6e 616c 2060 6461 7461 6d61  optional `datama
+0001cf00: 7060 2069 6e20 6f75 7220 636f 6e66 6967  p` in our config
+0001cf10: 7572 6174 696f 6e20 6669 6c65 2064 6566  uration file def
+0001cf20: 696e 6573 2074 6865 206e 616d 6520 6f66  ines the name of
+0001cf30: 2061 2066 756e 6374 696f 6e20 7765 2070   a function we p
+0001cf40: 726f 7669 6465 2c20 616c 736f 2069 6e20  rovide, also in 
+0001cf50: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+0001cf60: 6e20 6669 6c65 2c20 7768 6963 6820 6163  n file, which ac
+0001cf70: 636f 6d70 6c69 7368 6573 2074 6861 742e  complishes that.
+0001cf80: 0a0a 6060 6069 6e69 0a5b 6f77 6e74 7261  ..```ini.[owntra
+0001cf90: 636b 732f 6a61 6e65 2f70 686f 6e65 5d0a  cks/jane/phone].
+0001cfa0: 6461 7461 6d61 7020 3d20 4f77 6e54 7261  datamap = OwnTra
+0001cfb0: 636b 7354 6f70 6963 4461 7461 4d61 7028  cksTopicDataMap(
+0001cfc0: 290a 6060 600a 0a54 6869 7320 7370 6563  ).```..This spec
+0001cfd0: 6966 6965 7320 7468 6174 2077 6865 6e20  ifies that when 
+0001cfe0: 6120 6d65 7373 6167 6520 666f 7220 7468  a message for th
+0001cff0: 6520 6465 6669 6e65 6420 746f 7069 6320  e defined topic 
+0001d000: 606f 776e 7472 6163 6b73 2f6a 616e 652f  `owntracks/jane/
+0001d010: 7068 6f6e 6560 2069 7320 7072 6f63 6573  phone` is proces
+0001d020: 7365 642c 206f 7572 2066 756e 6374 696f  sed, our functio
+0001d030: 6e20 604f 776e 5472 6163 6b73 546f 7069  n `OwnTracksTopi
+0001d040: 6344 6174 614d 6170 2829 6020 7368 6f75  cDataMap()` shou
+0001d050: 6c64 2062 6520 696e 766f 6b65 6420 746f  ld be invoked to
+0001d060: 2070 6172 7365 2074 6861 742e 2028 4173   parse that. (As
+0001d070: 2075 7375 616c 2c20 746f 7069 6320 6e61   usual, topic na
+0001d080: 6d65 7320 6d61 7920 636f 6e74 6169 6e20  mes may contain 
+0001d090: 4d51 5454 2077 696c 6463 6172 6473 2e29  MQTT wildcards.)
+0001d0a0: 0a0a 5468 6520 6675 6e63 7469 6f6e 2077  ..The function w
+0001d0b0: 6520 6465 6669 6e65 2074 6f20 646f 2074  e define to do t
+0001d0c0: 6861 7420 6973 3a0a 0a60 6060 7079 7468  hat is:..```pyth
+0001d0d0: 6f6e 0a64 6566 204f 776e 5472 6163 6b73  on.def OwnTracks
+0001d0e0: 546f 7069 6344 6174 614d 6170 2874 6f70  TopicDataMap(top
+0001d0f0: 6963 293a 0a20 2020 2069 6620 7479 7065  ic):.    if type
+0001d100: 2874 6f70 6963 2920 3d3d 2073 7472 3a0a  (topic) == str:.
+0001d110: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001d120: 2020 2020 2020 2020 2023 206f 776e 7472           # owntr
+0001d130: 6163 6b73 2f75 7365 726e 616d 652f 6465  acks/username/de
+0001d140: 7669 6365 0a20 2020 2020 2020 2020 2020  vice.           
+0001d150: 2070 6172 7473 203d 2074 6f70 6963 2e73   parts = topic.s
+0001d160: 706c 6974 2827 2f27 290a 2020 2020 2020  plit('/').      
+0001d170: 2020 2020 2020 7573 6572 6e61 6d65 203d        username =
+0001d180: 2070 6172 7473 5b31 5d0a 2020 2020 2020   parts[1].      
+0001d190: 2020 2020 2020 6465 7669 6365 6964 203d        deviceid =
+0001d1a0: 2070 6172 7473 5b32 5d0a 2020 2020 2020   parts[2].      
+0001d1b0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+0001d1c0: 2020 2020 2020 6465 7669 6365 6964 203d        deviceid =
+0001d1d0: 2027 756e 6b6e 6f77 6e27 0a20 2020 2020   'unknown'.     
+0001d1e0: 2020 2020 2020 2075 7365 726e 616d 6520         username 
+0001d1f0: 3d20 2775 6e6b 6e6f 776e 270a 2020 2020  = 'unknown'.    
+0001d200: 2020 2020 7265 7475 726e 2064 6963 7428      return dict(
+0001d210: 7573 6572 6e61 6d65 3d75 7365 726e 616d  username=usernam
+0001d220: 652c 2064 6576 6963 653d 6465 7669 6365  e, device=device
+0001d230: 6964 290a 2020 2020 7265 7475 726e 204e  id).    return N
+0001d240: 6f6e 650a 6060 600a 0a54 6865 2072 6574  one.```..The ret
+0001d250: 7572 6e65 6420 5f64 6963 745f 2069 7320  urned _dict_ is 
+0001d260: 6d65 7267 6564 2069 6e74 6f20 7468 6520  merged into the 
+0001d270: 7472 616e 7366 6f72 6d61 7469 6f6e 2064  transformation d
+0001d280: 6174 612c 2069 2e65 2e20 6974 2069 7320  ata, i.e. it is 
+0001d290: 6d61 6465 2061 7661 696c 6162 6c65 2074  made available t
+0001d2a0: 6f20 706c 7567 696e 7320 616e 6420 746f  o plugins and to
+0001d2b0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+0001d2c0: 7275 6c65 7320 2860 666f 726d 6174 6029  rules (`format`)
+0001d2d0: 2e20 4966 2077 6520 7468 656e 2063 7265  . If we then cre
+0001d2e0: 6174 6520 7468 6520 666f 6c6c 6f77 696e  ate the followin
+0001d2f0: 6720 7275 6c65 0a0a 6060 6069 6e69 0a66  g rule..```ini.f
+0001d300: 6f72 6d61 7420 3d20 7b75 7365 726e 616d  ormat = {usernam
+0001d310: 657d 3a20 7b65 7665 6e74 7d20 3d3e 207b  e}: {event} => {
+0001d320: 6465 7363 7d0a 6060 600a 0a74 6865 2061  desc}.```..the a
+0001d330: 626f 7665 2050 5542 6c69 7368 2077 696c  bove PUBlish wil
+0001d340: 6c20 6265 2074 7261 6e73 666f 726d 6564  l be transformed
+0001d350: 2069 6e74 6f0a 0a60 6060 0a6a 616e 653a   into..```.jane:
+0001d360: 206c 6561 7665 203d 3e20 486f 6d65 0a60   leave => Home.`
+0001d370: 6060 0a0a 2323 2323 2320 4d65 7267 696e  ``..##### Mergin
+0001d380: 6720 6d6f 7265 2064 6174 6120 2323 230a  g more data ###.
+0001d390: 0a54 6865 206f 7074 696f 6e61 6c20 6061  .The optional `a
+0001d3a0: 6c6c 6461 7461 6020 6675 6e63 7469 6f6e  lldata` function
+0001d3b0: 2079 6f75 2077 7269 7465 2061 6e64 2063   you write and c
+0001d3c0: 6f6e 6669 6775 7265 206f 6e20 6120 7065  onfigure on a pe
+0001d3d0: 722f 746f 7069 6320 6261 7369 732c 2069  r/topic basis, i
+0001d3e0: 730a 7061 7373 6564 2074 6865 206d 6573  s.passed the mes
+0001d3f0: 7361 6765 205f 746f 7069 635f 2c20 6974  sage _topic_, it
+0001d400: 7320 5f64 6174 615f 2061 6e64 2061 6e20  s _data_ and an 
+0001d410: 6f70 7469 6f6e 616c 205f 7372 765f 206f  optional _srv_ o
+0001d420: 626a 6563 742e 2054 6869 7320 6675 6e63  bject. This func
+0001d430: 7469 6f6e 0a73 686f 756c 6420 7265 7475  tion.should retu
+0001d440: 726e 2061 205f 6469 6374 5f20 286f 7220  rn a _dict_ (or 
+0001d450: 5f4e 6f6e 655f 2920 6f66 2064 6174 6120  _None_) of data 
+0001d460: 7768 6963 6820 6973 206d 6572 6765 6420  which is merged 
+0001d470: 696e 746f 2074 6865 2077 686f 6c65 0a6c  into the whole.l
+0001d480: 6973 7420 6f66 2074 7261 6e73 666f 726d  ist of transform
+0001d490: 6174 696f 6e20 6461 7461 2e20 5468 6973  ation data. This
+0001d4a0: 2065 7870 616e 6473 206f 6e20 7468 6520   expands on the 
+0001d4b0: 7477 6f20 6f74 6865 7220 7472 616e 7366  two other transf
+0001d4c0: 6f72 6d61 7469 6f6e 2066 756e 6374 696f  ormation functio
+0001d4d0: 6e73 0a74 6f20 6d61 6b65 2074 6f70 6963  ns.to make topic
+0001d4e0: 2061 6e64 2074 6865 206d 6573 7361 6765   and the message
+0001d4f0: 2773 2070 6179 6c6f 6164 2061 7661 696c  's payload avail
+0001d500: 6162 6c65 2073 696d 756c 7461 6e65 6f75  able simultaneou
+0001d510: 736c 792e 0a0a 0a23 2323 2323 2041 2063  sly....##### A c
+0001d520: 7573 746f 6d20 6675 6e63 7469 6f6e 2074  ustom function t
+0001d530: 6f20 636f 6e76 6572 7420 6e65 7374 6564  o convert nested
+0001d540: 204a 534f 4e0a 0a46 6f72 2065 7861 6d70   JSON..For examp
+0001d550: 6c65 2c20 7361 7920 7765 2061 7265 2072  le, say we are r
+0001d560: 6563 6569 7669 6e67 206d 6573 7361 6765  eceiving message
+0001d570: 7320 6672 6f6d 2061 2074 656d 7065 7261  s from a tempera
+0001d580: 7475 7265 2073 656e 736f 7220 0a72 756e  ture sensor .run
+0001d590: 6e69 6e67 205b 5461 736d 6f74 615d 2868  ning [Tasmota](h
+0001d5a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0001d5b0: 6d2f 6172 656e 6473 742f 536f 6e6f 6666  m/arendst/Sonoff
+0001d5c0: 2d54 6173 6d6f 7461 2f29 2c0a 616e 6420  -Tasmota/),.and 
+0001d5d0: 7765 2077 6973 6820 746f 2063 6f6e 7665  we wish to conve
+0001d5e0: 7274 2074 6865 6d20 696e 746f 205b 496e  rt them into [In
+0001d5f0: 666c 7578 4442 206c 696e 6520 666f 726d  fluxDB line form
+0001d600: 6174 5d28 6874 7470 733a 2f2f 646f 6373  at](https://docs
+0001d610: 2e69 6e66 6c75 7864 6174 612e 636f 6d2f  .influxdata.com/
+0001d620: 696e 666c 7578 6462 2f76 312e 362f 7772  influxdb/v1.6/wr
+0001d630: 6974 655f 7072 6f74 6f63 6f6c 732f 6c69  ite_protocols/li
+0001d640: 6e65 5f70 726f 746f 636f 6c5f 7475 746f  ne_protocol_tuto
+0001d650: 7269 616c 2f29 2e0a 0a54 6865 2069 6e63  rial/)...The inc
+0001d660: 6f6d 696e 6720 5b4a 534f 4e5d 2868 7474  oming [JSON](htt
+0001d670: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0001d680: 6172 656e 6473 742f 536f 6e6f 6666 2d54  arendst/Sonoff-T
+0001d690: 6173 6d6f 7461 2f77 696b 692f 4a53 4f4e  asmota/wiki/JSON
+0001d6a0: 2d53 7461 7475 732d 5265 7370 6f6e 7365  -Status-Response
+0001d6b0: 7323 6473 3138 6232 3029 2077 696c 6c20  s#ds18b20) will 
+0001d6c0: 6c6f 6f6b 206c 696b 6520 7468 6973 3a0a  look like this:.
+0001d6d0: 6060 600a 7b0a 2020 2020 2254 696d 6522  ```.{.    "Time"
+0001d6e0: 3a20 2232 3031 382e 3032 2e30 3120 3231  : "2018.02.01 21
+0001d6f0: 3a32 393a 3430 222c 0a20 2020 2022 4453  :29:40",.    "DS
+0001d700: 3138 4232 3022 3a20 7b0a 2020 2020 2020  18B20": {.      
+0001d710: 2254 656d 7065 7261 7475 7265 223a 2031  "Temperature": 1
+0001d720: 392e 370a 2020 2020 7d2c 0a20 2020 2022  9.7.    },.    "
+0001d730: 5465 6d70 556e 6974 223a 2022 4322 0a7d  TempUnit": "C".}
+0001d740: 2c0a 6060 600a 0a53 696e 6365 2060 5465  ,.```..Since `Te
+0001d750: 6d70 6572 6174 7572 6560 2063 616e 6e6f  mperature` canno
+0001d760: 7420 6265 2072 6566 6572 656e 6365 6420  t be referenced 
+0001d770: 6469 7265 6374 6c79 2077 6974 6869 6e20  directly within 
+0001d780: 6120 6066 6f72 6d61 7460 2c20 7765 206e  a `format`, we n
+0001d790: 6565 6420 746f 206d 616b 6520 6974 2061  eed to make it a
+0001d7a0: 2074 6f70 2d6c 6576 656c 2076 616c 7565   top-level value
+0001d7b0: 2e20 0a57 6869 6c65 2077 6527 7265 2061  . .While we're a
+0001d7c0: 7420 6974 2c20 7765 2063 616e 2063 6861  t it, we can cha
+0001d7d0: 6e67 6520 7468 6520 6461 7465 2074 6f20  nge the date to 
+0001d7e0: 6d69 6c6c 6973 6563 6f6e 6473 2073 696e  milliseconds sin
+0001d7f0: 6365 2074 6865 2065 706f 6368 2c20 616e  ce the epoch, an
+0001d800: 6420 696e 636c 7564 6520 7468 6520 746f  d include the to
+0001d810: 7069 633a 0a60 6060 0a7b 0a20 2020 2022  pic:.```.{.    "
+0001d820: 546f 7069 6322 3a20 2274 6173 6d6f 7461  Topic": "tasmota
+0001d830: 2f74 656d 702f 6473 2f31 222c 200a 2020  /temp/ds/1", .  
+0001d840: 2020 2254 696d 6573 7461 6d70 223a 2031    "Timestamp": 1
+0001d850: 3531 3735 3235 3331 3930 3030 2c20 0a20  517525319000, . 
+0001d860: 2020 2022 5465 6d70 6572 6174 7572 6522     "Temperature"
+0001d870: 3a20 3139 2e37 0a7d 0a60 6060 0a0a 5468  : 19.7.}.```..Th
+0001d880: 6973 2063 616e 2062 6520 6163 636f 6d70  is can be accomp
+0001d890: 6c69 7368 6564 2077 6974 6820 7468 6520  lished with the 
+0001d8a0: 666f 6c6c 6f77 696e 6720 6675 6e63 7469  following functi
+0001d8b0: 6f6e 3a20 0a60 6060 0a69 6d70 6f72 7420  on: .```.import 
+0001d8c0: 6173 740a 696d 706f 7274 206c 6f67 6769  ast.import loggi
+0001d8d0: 6e67 0a69 6d70 6f72 7420 7469 6d65 0a66  ng.import time.f
+0001d8e0: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
+0001d8f0: 6f72 7420 6461 7465 7469 6d65 0a0a 6465  ort datetime..de
+0001d900: 6620 6473 3138 6232 305f 7661 6c75 6573  f ds18b20_values
+0001d910: 2874 6f70 6963 2c20 6461 7461 2c20 7372  (topic, data, sr
+0001d920: 763d 4e6f 6e65 293a 0a20 2020 2070 6179  v=None):.    pay
+0001d930: 6c6f 6164 203d 2061 7374 2e6c 6974 6572  load = ast.liter
+0001d940: 616c 5f65 7661 6c28 6461 7461 5b22 7061  al_eval(data["pa
+0001d950: 796c 6f61 6422 5d29 0a20 2020 2074 7320  yload"]).    ts 
+0001d960: 3d20 6461 7465 7469 6d65 2e73 7472 7074  = datetime.strpt
+0001d970: 696d 6528 7061 796c 6f61 645b 2254 696d  ime(payload["Tim
+0001d980: 6522 5d2c 2022 2559 2e25 6d2e 2564 2025  e"], "%Y.%m.%d %
+0001d990: 483a 254d 3a25 5322 290a 2020 2020 6d69  H:%M:%S").    mi
+0001d9a0: 6c6c 6973 203d 206c 6f6e 6728 7469 6d65  llis = long(time
+0001d9b0: 2e6d 6b74 696d 6528 7473 2e74 696d 6574  .mktime(ts.timet
+0001d9c0: 7570 6c65 2829 2920 2a20 3130 3030 290a  uple()) * 1000).
+0001d9d0: 2020 2020 7465 6d70 203d 2070 6179 6c6f      temp = paylo
+0001d9e0: 6164 5b22 4453 3138 4232 3022 5d5b 2254  ad["DS18B20"]["T
+0001d9f0: 656d 7065 7261 7475 7265 225d 0a20 2020  emperature"].   
+0001da00: 2064 203d 2064 6963 7428 2054 6f70 6963   d = dict( Topic
+0001da10: 203d 2074 6f70 6963 2c20 5469 6d65 7374   = topic, Timest
+0001da20: 616d 7020 3d20 6d69 6c6c 6973 2c20 5465  amp = millis, Te
+0001da30: 6d70 6572 6174 7572 6520 3d20 7465 6d70  mperature = temp
+0001da40: 2029 0a20 2020 206c 6f67 6769 6e67 2e64   ).    logging.d
+0001da50: 6562 7567 2864 290a 2020 2020 7265 7475  ebug(d).    retu
+0001da60: 726e 2064 0a60 6060 0a0a 4170 706c 7920  rn d.```..Apply 
+0001da70: 6974 2074 6f20 6120 746f 7069 6320 696e  it to a topic in
+0001da80: 2060 6d71 7474 7761 726e 2e69 6e69 603a   `mqttwarn.ini`:
+0001da90: 0a60 6060 0a5b 7461 736d 6f74 612f 7465  .```.[tasmota/te
+0001daa0: 6d70 2f64 732f 2b5d 0a74 6172 6765 7473  mp/ds/+].targets
+0001dab0: 203d 206c 6f67 3a69 6e66 6f0a 616c 6c64   = log:info.alld
+0001dac0: 6174 6120 3d20 6473 3138 6232 305f 7661  ata = ds18b20_va
+0001dad0: 6c75 6573 2829 0a66 6f72 6d61 7420 203d  lues().format  =
+0001dae0: 2077 6561 7468 6572 2c54 6f70 6963 3d7b   weather,Topic={
+0001daf0: 546f 7069 637d 2054 656d 7065 7261 7475  Topic} Temperatu
+0001db00: 7265 3d7b 5465 6d70 6572 6174 7572 657d  re={Temperature}
+0001db10: 207b 5469 6d65 7374 616d 707d 0a60 6060   {Timestamp}.```
+0001db20: 0a0a 5768 6963 6820 7265 7375 6c74 7320  ..Which results 
+0001db30: 696e 3a0a 6060 600a 3230 3138 2d30 372d  in:.```.2018-07-
+0001db40: 3139 2032 323a 3030 3a32 342c 3435 3220  19 22:00:24,452 
+0001db50: 4445 4255 4720 5b6d 7174 7477 6172 6e5d  DEBUG [mqttwarn]
+0001db60: 204d 6573 7361 6765 2072 6563 6569 7665   Message receive
+0001db70: 6420 6f6e 2074 6173 6d6f 7461 2f74 656d  d on tasmota/tem
+0001db80: 702f 6473 2f31 3a20 7b20 2254 696d 6522  p/ds/1: { "Time"
+0001db90: 3a20 2232 3031 382e 3032 2e30 3120 3232  : "2018.02.01 22
+0001dba0: 3a34 383a 3339 222c 2022 4453 3138 4232  :48:39", "DS18B2
+0001dbb0: 3022 3a20 7b20 2254 656d 7065 7261 7475  0": { "Temperatu
+0001dbc0: 7265 223a 2031 392e 3720 7d2c 2022 5465  re": 19.7 }, "Te
+0001dbd0: 6d70 556e 6974 223a 2022 4322 207d 0a32  mpUnit": "C" }.2
+0001dbe0: 3031 382d 3037 2d31 3920 3232 3a30 303a  018-07-19 22:00:
+0001dbf0: 3234 2c34 3533 2044 4542 5547 205b 6d71  24,453 DEBUG [mq
+0001dc00: 7474 7761 726e 5d20 5365 6374 696f 6e20  ttwarn] Section 
+0001dc10: 5b74 6173 6d6f 7461 2f74 656d 702f 6473  [tasmota/temp/ds
+0001dc20: 2f2b 5d20 6d61 7463 6865 7320 6d65 7373  /+] matches mess
+0001dc30: 6167 6520 6f6e 2074 6173 6d6f 7461 2f74  age on tasmota/t
+0001dc40: 656d 702f 6473 2f31 2e20 5072 6f63 6573  emp/ds/1. Proces
+0001dc50: 7369 6e67 2e2e 2e0a 3230 3138 2d30 372d  sing....2018-07-
+0001dc60: 3139 2032 323a 3030 3a32 342c 3435 3720  19 22:00:24,457 
+0001dc70: 4445 4255 4720 5b66 756e 6373 5d20 7b27  DEBUG [funcs] {'
+0001dc80: 546f 7069 6327 3a20 7527 7461 736d 6f74  Topic': u'tasmot
+0001dc90: 612f 7465 6d70 2f64 732f 3127 2c20 2754  a/temp/ds/1', 'T
+0001dca0: 696d 6573 7461 6d70 273a 2031 3531 3735  imestamp': 15175
+0001dcb0: 3235 3331 3930 3030 4c2c 2027 5465 6d70  25319000L, 'Temp
+0001dcc0: 6572 6174 7572 6527 3a20 3139 2e37 7d0a  erature': 19.7}.
+0001dcd0: 3230 3138 2d30 372d 3139 2032 323a 3030  2018-07-19 22:00
+0001dce0: 3a32 342c 3435 3920 4445 4255 4720 5b6d  :24,459 DEBUG [m
+0001dcf0: 7174 7477 6172 6e5d 204d 6573 7361 6765  qttwarn] Message
+0001dd00: 206f 6e20 7461 736d 6f74 612f 7465 6d70   on tasmota/temp
+0001dd10: 2f64 732f 3120 676f 696e 6720 746f 206c  /ds/1 going to l
+0001dd20: 6f67 3a69 6e66 6f0a 3230 3138 2d30 372d  og:info.2018-07-
+0001dd30: 3139 2032 323a 3030 3a32 342c 3435 3920  19 22:00:24,459 
+0001dd40: 4445 4255 4720 5b6d 7174 7477 6172 6e5d  DEBUG [mqttwarn]
+0001dd50: 204e 6577 2060 6c6f 673a 696e 666f 2720   New `log:info' 
+0001dd60: 6a6f 623a 2074 6173 6d6f 7461 2f74 656d  job: tasmota/tem
+0001dd70: 702f 6473 2f31 0a32 3031 382d 3037 2d31  p/ds/1.2018-07-1
+0001dd80: 3920 3232 3a30 303a 3234 2c34 3539 2044  9 22:00:24,459 D
+0001dd90: 4542 5547 205b 6d71 7474 7761 726e 5d20  EBUG [mqttwarn] 
+0001dda0: 5072 6f63 6573 736f 7220 2330 2069 7320  Processor #0 is 
+0001ddb0: 6861 6e64 6c69 6e67 3a20 606c 6f67 2720  handling: `log' 
+0001ddc0: 666f 7220 696e 666f 0a32 3031 382d 3037  for info.2018-07
+0001ddd0: 2d31 3920 3232 3a30 303a 3234 2c34 3630  -19 22:00:24,460
+0001dde0: 2044 4542 5547 205b 6c6f 675d 202a 2a2a   DEBUG [log] ***
+0001ddf0: 204d 4f44 554c 453d 7365 7276 6963 6573   MODULE=services
+0001de00: 2f6c 6f67 2e70 7963 3a20 7365 7276 6963  /log.pyc: servic
+0001de10: 653d 6c6f 672c 2074 6172 6765 743d 696e  e=log, target=in
+0001de20: 666f 0a32 3031 382d 3037 2d31 3920 3232  fo.2018-07-19 22
+0001de30: 3a30 303a 3234 2c34 3630 2049 4e46 4f20  :00:24,460 INFO 
+0001de40: 205b 6c6f 675d 2077 6561 7468 6572 2c54   [log] weather,T
+0001de50: 6f70 6963 3d74 6173 6d6f 7461 2f74 656d  opic=tasmota/tem
+0001de60: 702f 6473 2f31 2054 656d 7065 7261 7475  p/ds/1 Temperatu
+0001de70: 7265 3d31 392e 3720 3135 3137 3532 3533  re=19.7 15175253
+0001de80: 3139 3030 300a 6060 600a 0a23 2323 2323  19000.```..#####
+0001de90: 2054 6f70 6963 2074 6172 6765 7473 0a0a   Topic targets..
+0001dea0: 4279 2069 6e63 6f72 706f 7261 7469 6e67  By incorporating
+0001deb0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+0001dec0: 6461 7461 2069 6e74 6f20 746f 7069 6320  data into topic 
+0001ded0: 7461 7267 6574 732c 2077 6520 6361 6e20  targets, we can 
+0001dee0: 6d61 6b65 205f 6d71 7474 7761 726e 5f20  make _mqttwarn_ 
+0001def0: 6469 7370 6174 6368 0a6d 6573 7361 6765  dispatch.message
+0001df00: 7320 6479 6e61 6d69 6361 6c6c 7920 6261  s dynamically ba
+0001df10: 7365 6420 6f6e 2074 6865 2076 616c 7565  sed on the value
+0001df20: 7320 6f66 2074 6865 2074 7261 6e73 666f  s of the transfo
+0001df30: 726d 6174 696f 6e20 6461 7461 2064 6963  rmation data dic
+0001df40: 7469 6f6e 6172 792e 0a0a 546f 2067 6574  tionary...To get
+0001df50: 2061 6e20 6964 6561 2061 626f 7574 2068   an idea about h
+0001df60: 6f77 2074 6869 7320 776f 726b 732c 206c  ow this works, l
+0001df70: 6574 2773 2064 6566 696e 6520 6120 706c  et's define a pl
+0001df80: 6163 6568 6f6c 6465 7220 7661 7269 6162  aceholder variab
+0001df90: 6c65 2069 6e73 6964 6520 7468 650a 6074  le inside the.`t
+0001dfa0: 6172 6765 7473 6020 6469 7265 6374 6976  argets` directiv
+0001dfb0: 6520 6f66 2061 2074 6f70 6963 2073 6563  e of a topic sec
+0001dfc0: 7469 6f6e 2069 6e20 7468 6520 606d 7174  tion in the `mqt
+0001dfd0: 7477 6172 6e2e 696e 6960 2063 6f6e 6669  twarn.ini` confi
+0001dfe0: 6775 7261 7469 6f6e 2066 696c 653a 0a0a  guration file:..
+0001dff0: 2020 2020 5b74 6f70 6963 2d74 6172 6765      [topic-targe
+0001e000: 7473 2d64 796e 616d 6963 5d0a 2020 2020  ts-dynamic].    
+0001e010: 746f 7069 6320 2020 3d20 7465 7374 2f74  topic   = test/t
+0001e020: 6f70 6963 2d74 6172 6765 7473 2d64 796e  opic-targets-dyn
+0001e030: 616d 6963 0a20 2020 2066 6f72 6d61 7420  amic.    format 
+0001e040: 203d 2053 6f6d 6574 6869 6e67 207b 6c6f   = Something {lo
+0001e050: 676c 6576 656c 7d20 6861 7070 656e 6564  glevel} happened
+0001e060: 2120 7b6d 6573 7361 6765 7d0a 2020 2020  ! {message}.    
+0001e070: 7461 7267 6574 7320 3d20 6c6f 673a 7b6c  targets = log:{l
+0001e080: 6f67 6c65 7665 6c7d 0a0a 5768 656e 2073  oglevel}..When s
+0001e090: 656e 6469 6e67 2074 6869 7320 7661 6c75  ending this valu
+0001e0a0: 6520 7468 726f 7567 6820 6120 4a53 4f4e  e through a JSON
+0001e0b0: 2065 6e63 6f64 6564 206d 6573 7361 6765   encoded message
+0001e0c0: 206f 7220 6279 2063 6f6d 7075 7469 6e67   or by computing
+0001e0d0: 2069 740a 7468 726f 7567 6820 7468 6520   it.through the 
+0001e0e0: 6064 6174 616d 6170 6020 6f72 2060 616c  `datamap` or `al
+0001e0f0: 6c64 6174 6160 2074 7261 6e73 666f 726d  ldata` transform
+0001e100: 6174 696f 6e20 6d61 6368 696e 6572 792c  ation machinery,
+0001e110: 2069 7420 7769 6c6c 2067 6574 0a69 6e74   it will get.int
+0001e120: 6572 706f 6c61 7465 6420 696e 746f 2074  erpolated into t
+0001e130: 6865 2064 6573 6967 6e61 7465 6420 746f  he designated to
+0001e140: 7069 6320 7461 7267 6574 2e20 4578 616d  pic target. Exam
+0001e150: 706c 653a 0a0a 2020 2020 6d6f 7371 7569  ple:..    mosqui
+0001e160: 7474 6f5f 7075 6220 2d74 2074 6573 742f  tto_pub -t test/
+0001e170: 746f 7069 632d 7461 7267 6574 732d 6479  topic-targets-dy
+0001e180: 6e61 6d69 6320 2d6d 2027 7b22 6c6f 676c  namic -m '{"logl
+0001e190: 6576 656c 223a 2022 6372 6974 222c 2022  evel": "crit", "
+0001e1a0: 6d65 7373 6167 6522 3a20 224e 7572 2044  message": "Nur D
+0001e1b0: c3b6 6e65 7220 6d61 6368 7420 7363 68c3  ..ner macht sch.
+0001e1c0: b66e 6572 2122 7d27 0a0a 5468 6973 2077  .ner!"}'..This w
+0001e1d0: 696c 6c20 6973 7375 6520 7468 6520 666f  ill issue the fo
+0001e1e0: 6c6c 6f77 696e 6720 6d65 7373 6167 6520  llowing message 
+0001e1f0: 696e 746f 2074 6865 206c 6f67 2066 696c  into the log fil
+0001e200: 653a 0a0a 2020 2020 3230 3136 2d30 322d  e:..    2016-02-
+0001e210: 3134 2031 383a 3039 3a33 342c 3832 3220  14 18:09:34,822 
+0001e220: 4352 4954 4943 414c 205b 6c6f 675d 2053  CRITICAL [log] S
+0001e230: 6f6d 6574 6869 6e67 2063 7269 7420 6861  omething crit ha
+0001e240: 7070 656e 6564 2120 4e75 7220 44c3 b66e  ppened! Nur D..n
+0001e250: 6572 206d 6163 6874 2073 6368 c3b6 6e65  er macht sch..ne
+0001e260: 7221 0a0a 5768 696c 6520 7468 6973 206c  r!..While this l
+0001e270: 6974 746c 6520 6578 616d 706c 6520 6d69  ittle example mi
+0001e280: 6768 7420 6665 656c 2061 7274 6966 6963  ght feel artific
+0001e290: 6961 6c2c 2074 6865 7265 2061 7265 206d  ial, there are m
+0001e2a0: 6f72 6520 6d65 616e 696e 6766 756c 0a75  ore meaningful.u
+0001e2b0: 7365 2063 6173 6573 206c 696b 6520 6465  se cases like de
+0001e2c0: 7465 726d 696e 696e 6720 7468 6520 7265  termining the re
+0001e2d0: 6369 7069 656e 7420 6164 6472 6573 7320  cipient address 
+0001e2e0: 6f66 2060 736d 7470 6020 6f72 2060 786d  of `smtp` or `xm
+0001e2f0: 7070 6020 7265 6365 6976 6572 730a 7468  pp` receivers.th
+0001e300: 726f 7567 6820 696e 666f 726d 6174 696f  rough informatio
+0001e310: 6e20 6672 6f6d 2074 6f70 6963 206e 616d  n from topic nam
+0001e320: 6573 206f 7220 6d65 7373 6167 6520 7061  es or message pa
+0001e330: 796c 6f61 6473 2e0a 506c 6561 7365 2068  yloads..Please h
+0001e340: 6176 6520 6120 6c6f 6f6b 2061 7420 5b49  ave a look at [I
+0001e350: 6e63 6f72 706f 7261 7465 2074 6f70 6963  ncorporate topic
+0001e360: 206e 616d 6573 2069 6e74 6f20 746f 7069   names into topi
+0001e370: 6320 7461 7267 6574 735d 2868 7474 7073  c targets](https
+0001e380: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a70  ://github.com/jp
+0001e390: 6d65 6e73 2f6d 7174 7477 6172 6e2f 7769  mens/mqttwarn/wi
+0001e3a0: 6b69 2f49 6e63 6f72 706f 7261 7469 6e67  ki/Incorporating
+0001e3b0: 2d74 6f70 6963 2d6e 616d 6573 2369 6e63  -topic-names#inc
+0001e3c0: 6f72 706f 7261 7465 2d74 6f70 6963 2d6e  orporate-topic-n
+0001e3d0: 616d 6573 2d69 6e74 6f2d 746f 7069 632d  ames-into-topic-
+0001e3e0: 7461 7267 6574 7329 0a66 6f72 2061 206d  targets).for a m
+0001e3f0: 6f72 6520 7365 6e73 6962 6c65 2065 7861  ore sensible exa
+0001e400: 6d70 6c65 2e0a 0a0a 2323 2323 2320 4669  mple....##### Fi
+0001e410: 6c74 6572 696e 6720 6e6f 7469 6669 6361  ltering notifica
+0001e420: 7469 6f6e 730a 0a41 206e 6f74 6966 6963  tions..A notific
+0001e430: 6174 696f 6e20 6361 6e20 6265 2066 696c  ation can be fil
+0001e440: 7465 7265 6420 286f 7220 7375 7070 7265  tered (or suppre
+0001e450: 7373 6564 2c20 6f72 2069 676e 6f72 6564  ssed, or ignored
+0001e460: 2920 7573 696e 6720 6120 6375 7374 6f6d  ) using a custom
+0001e470: 2066 756e 6374 696f 6e2e 0a0a 416e 206f   function...An o
+0001e480: 7074 696f 6e61 6c20 6066 696c 7465 7260  ptional `filter`
+0001e490: 2073 6574 7469 6e67 2069 6e20 6120 7365   setting in a se
+0001e4a0: 6374 696f 6e20 626c 6f63 6b20 6465 6669  ction block defi
+0001e4b0: 6e65 7320 7468 6520 6e61 6d65 206f 6620  nes the name of 
+0001e4c0: 6120 5079 7468 6f6e 2066 756e 6374 696f  a Python functio
+0001e4d0: 6e20 7072 6f76 6964 6564 2069 6e20 6669  n provided in fi
+0001e4e0: 6c65 2073 7065 6369 6669 6564 2062 7920  le specified by 
+0001e4f0: 7468 6520 6066 756e 6374 696f 6e73 6020  the `functions` 
+0001e500: 6469 7265 6374 6976 652e 0a0a 6060 6069  directive...```i
+0001e510: 6e69 0a5b 6f77 6e74 7261 636b 732f 232f  ni.[owntracks/#/
+0001e520: 7068 6f6e 655d 0a66 696c 7465 7220 3d20  phone].filter = 
+0001e530: 6f77 6e74 7261 636b 735f 6669 6c74 6572  owntracks_filter
+0001e540: 2829 0a60 6060 0a0a 5468 6973 2065 7861  ().```..This exa
+0001e550: 6d70 6c65 2073 7065 6369 6669 6573 2074  mple specifies t
+0001e560: 6861 7420 7768 656e 2061 206d 6573 7361  hat when a messa
+0001e570: 6765 2066 6f72 2074 6865 2064 6566 696e  ge for the defin
+0001e580: 6564 2074 6f70 6963 2060 6f77 6e74 7261  ed topic `owntra
+0001e590: 636b 732f 6a61 6e65 2f70 686f 6e65 6020  cks/jane/phone` 
+0001e5a0: 6973 2072 6563 6569 7665 642c 2074 6865  is received, the
+0001e5b0: 2066 756e 6374 696f 6e20 606f 776e 7472   function `owntr
+0001e5c0: 6163 6b73 5f66 696c 7465 7228 2960 2073  acks_filter()` s
+0001e5d0: 686f 756c 6420 6265 2069 6e76 6f6b 6564  hould be invoked
+0001e5e0: 2074 6f20 6465 7465 726d 696e 6520 7768   to determine wh
+0001e5f0: 6574 6865 720a 6f72 206e 6f74 2074 6f20  ether.or not to 
+0001e600: 7072 6f63 6573 7320 7468 6520 6d65 7373  process the mess
+0001e610: 6167 652e 0a0a 5468 6520 6669 6c74 6572  age...The filter
+0001e620: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
+0001e630: 2072 6574 7572 6e20 6054 7275 6560 2069   return `True` i
+0001e640: 6620 7468 6520 6d65 7373 6167 6520 7368  f the message sh
+0001e650: 6f75 6c64 2062 6520 7375 7070 7265 7373  ould be suppress
+0001e660: 6564 2c20 6f72 2060 4661 6c73 6560 2069  ed, or `False` i
+0001e670: 6620 7468 6520 6d65 7373 6167 6520 7368  f the message sh
+0001e680: 6f75 6c64 2062 6520 7072 6f63 6573 7365  ould be processe
+0001e690: 642e 0a49 7420 7368 6f75 6c64 2068 6176  d..It should hav
+0001e6a0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+0001e6b0: 7369 676e 6174 7572 653a 0a0a 6060 6070  signature:..```p
+0001e6c0: 7974 686f 6e0a 6465 6620 6f77 6e74 7261  ython.def owntra
+0001e6d0: 636b 735f 6669 6c74 6572 2874 6f70 6963  cks_filter(topic
+0001e6e0: 2c20 6d65 7373 6167 652c 2073 6563 7469  , message, secti
+0001e6f0: 6f6e 2c20 7372 7629 3a0a 2020 2020 7265  on, srv):.    re
+0001e700: 7475 726e 206d 6573 7361 6765 2e66 696e  turn message.fin
+0001e710: 6428 2765 7665 6e74 2729 203d 3d20 2d31  d('event') == -1
+0001e720: 0a60 6060 0a0a 5468 6520 666f 6c6c 6f77  .```..The follow
+0001e730: 696e 672c 2077 6974 6820 6665 7765 7220  ing, with fewer 
+0001e740: 6172 6775 6d65 6e74 732c 2069 7320 616c  arguments, is al
+0001e750: 736f 2061 6363 6570 7461 626c 652c 2062  so acceptable, b
+0001e760: 7574 2074 6865 2061 626f 7665 2069 7320  ut the above is 
+0001e770: 7072 6566 6572 7265 642e 0a60 6060 7079  preferred..```py
+0001e780: 7468 6f6e 0a64 6566 206f 776e 7472 6163  thon.def owntrac
+0001e790: 6b73 5f66 696c 7465 7228 746f 7069 632c  ks_filter(topic,
+0001e7a0: 206d 6573 7361 6765 293a 0a20 2020 2072   message):.    r
+0001e7b0: 6574 7572 6e20 6d65 7373 6167 652e 6669  eturn message.fi
+0001e7c0: 6e64 2827 6576 656e 7427 2920 3d3d 202d  nd('event') == -
+0001e7d0: 310a 6060 600a 0a54 6865 7365 2066 756e  1.```..These fun
+0001e7e0: 6374 696f 6e73 2077 696c 6c20 7265 7475  ctions will retu
+0001e7f0: 726e 2060 5472 7565 6020 666f 7220 6d65  rn `True` for me
+0001e800: 7373 6167 6573 2074 6861 7420 646f 206e  ssages that do n
+0001e810: 6f74 2063 6f6e 7461 696e 2074 6865 2060  ot contain the `
+0001e820: 6576 656e 7460 2074 6f6b 656e 2c20 616e  event` token, an
+0001e830: 6420 7468 7573 2073 7570 7072 6573 7320  d thus suppress 
+0001e840: 7468 6f73 6520 6d65 7373 6167 6573 2e0a  those messages..
+0001e850: 0a4e 6f74 6520 7468 6174 2074 6865 2060  .Note that the `
+0001e860: 746f 7069 6360 2070 6172 616d 6574 6572  topic` parameter
+0001e870: 2077 696c 6c20 6265 2074 6865 206e 616d   will be the nam
+0001e880: 6520 6f66 2074 6865 2073 7065 6369 6669  e of the specifi
+0001e890: 6320 746f 7069 6320 2865 2e67 2e20 606f  c topic (e.g. `o
+0001e8a0: 776e 7472 6163 6b73 2f6a 616e 652f 7068  wntracks/jane/ph
+0001e8b0: 6f6e 6560 2920 7468 6174 2074 6865 206d  one`) that the m
+0001e8c0: 6573 7361 6765 0a77 6173 2072 6563 6569  essage.was recei
+0001e8d0: 7665 6420 6f6e 2e20 2054 6865 206e 616d  ved on.  The nam
+0001e8e0: 6520 6f66 2074 6865 2073 6563 7469 6f6e  e of the section
+0001e8f0: 2028 652e 672e 2060 6f77 6e74 7261 636b   (e.g. `owntrack
+0001e900: 732f 232f 7068 6f6e 6560 2920 7769 6c6c  s/#/phone`) will
+0001e910: 2062 6520 7468 6520 6073 6563 7469 6f6e   be the `section
+0001e920: 6020 6172 6775 6d65 6e74 2e0a 0a0a 2323  ` argument....##
+0001e930: 2320 5465 6d70 6c61 7465 7320 2323 230a  # Templates ###.
+0001e940: 0a49 6e73 7465 6164 206f 6620 666f 726d  .Instead of form
+0001e950: 6174 7469 6e67 206f 7574 7075 7420 7769  atting output wi
+0001e960: 7468 2074 6865 2060 666f 726d 6174 6020  th the `format` 
+0001e970: 7370 6563 6966 6963 6174 696f 6e20 6173  specification as
+0001e980: 2064 6573 6372 6962 6564 2061 626f 7665   described above
+0001e990: 2c0a 5f6d 7174 7477 6172 6e5f 2068 6173  ,._mqttwarn_ has
+0001e9a0: 2070 726f 7669 7369 6f6e 2066 6f72 2072   provision for r
+0001e9b0: 656e 6465 7269 6e67 2074 6865 206f 7574  endering the out
+0001e9c0: 7075 7420 6d65 7373 6167 6520 6672 6f6d  put message from
+0001e9d0: 205b 4a69 6e6a 6132 5d20 7465 6d70 6c61   [Jinja2] templa
+0001e9e0: 7465 732c 0a70 726f 6261 626c 7920 7061  tes,.probably pa
+0001e9f0: 7274 6963 756c 6172 6c79 2069 6e74 6572  rticularly inter
+0001ea00: 6573 7469 6e67 2066 6f72 2074 6865 2060  esting for the `
+0001ea10: 736d 7470 6020 6f72 2060 6e6e 7470 6020  smtp` or `nntp` 
+0001ea20: 616e 6420 6066 696c 6560 2074 6172 6765  and `file` targe
+0001ea30: 7473 2e0a 0a43 6f6e 7369 6465 7220 7468  ts...Consider th
+0001ea40: 6520 666f 6c6c 6f77 696e 6720 6578 616d  e following exam
+0001ea50: 706c 6520 746f 7069 6320 636f 6e66 6967  ple topic config
+0001ea60: 7572 6174 696f 6e2c 2077 6865 7265 2077  uration, where w
+0001ea70: 6520 696c 6c75 7374 7261 7465 2075 7369  e illustrate usi
+0001ea80: 6e67 0a61 2074 656d 706c 6174 6520 696e  ng.a template in
+0001ea90: 7374 6561 6420 6f66 2060 666f 726d 6174  stead of `format
+0001eaa0: 6020 2877 6869 6368 2069 7320 636f 6d6d  ` (which is comm
+0001eab0: 656e 7465 6420 6f75 7429 2e0a 0a60 6060  ented out)...```
+0001eac0: 696e 690a 5b6e 6e2f 2b5d 0a74 6172 6765  ini.[nn/+].targe
+0001ead0: 7473 203d 206e 6e74 703a 6a70 6161 0a3b  ts = nntp:jpaa.;
+0001eae0: 2066 6f72 6d61 7420 3d20 7b6e 616d 657d   format = {name}
+0001eaf0: 3a20 7b6e 756d 6265 727d 203d 3e20 7b5f  : {number} => {_
+0001eb00: 6474 6868 6d6d 7d0a 7465 6d70 6c61 7465  dthhmm}.template
+0001eb10: 203d 2064 656d 6f2e 6a32 0a60 6060 0a0a   = demo.j2.```..
+0001eb20: 5f6d 7174 7477 6172 6e5f 206c 6f61 6473  _mqttwarn_ loads
+0001eb30: 204a 696e 6a61 3220 7465 6d70 6c61 7465   Jinja2 template
+0001eb40: 7320 6672 6f6d 2074 6865 2060 7465 6d70  s from the `temp
+0001eb50: 6c61 7465 732f 6020 6469 7265 6374 6f72  lates/` director
+0001eb60: 7920 7265 6c61 7469 7665 2074 6f20 7468  y relative to th
+0001eb70: 650a 636f 6e66 6967 7572 6564 2060 6469  e.configured `di
+0001eb80: 7265 6374 6f72 7960 2e20 4173 7375 6d69  rectory`. Assumi
+0001eb90: 6e67 2077 6520 6861 7665 2074 6865 2066  ng we have the f
+0001eba0: 6f6c 6c6f 7769 6e67 2063 6f6e 7465 6e74  ollowing content
+0001ebb0: 2069 6e20 7468 6520 6669 6c65 0a60 7465   in the file.`te
+0001ebc0: 6d70 6c61 7465 732f 6465 6d6f 2e6a 3260  mplates/demo.j2`
+0001ebd0: 0a0a 6060 606a 696e 6a61 320a 7b23 0a20  ..```jinja2.{#. 
+0001ebe0: 2020 2074 6869 7320 6973 2061 2063 6f6d     this is a com
+0001ebf0: 6d65 6e74 0a20 2020 2069 6e20 4a69 6e6a  ment.    in Jinj
+0001ec00: 6132 0a20 2020 2053 6565 2068 7474 703a  a2.    See http:
+0001ec10: 2f2f 6a69 6e6a 612e 706f 636f 6f2e 6f72  //jinja.pocoo.or
+0001ec20: 672f 646f 6373 2f74 656d 706c 6174 6573  g/docs/templates
+0001ec30: 2f20 666f 7220 696e 666f 726d 6174 696f  / for informatio
+0001ec40: 6e0a 2020 2020 6f6e 204a 696e 6a61 3220  n.    on Jinja2 
+0001ec50: 7465 6d70 6c61 7465 732e 0a23 7d0a 7b25  templates..#}.{%
+0001ec60: 2073 6574 2075 706e 616d 6520 3d20 6e61   set upname = na
+0001ec70: 6d65 207c 2075 7070 6572 2025 7d0a 7b25  me | upper %}.{%
+0001ec80: 2073 6574 2077 6964 7468 203d 2036 3020   set width = 60 
+0001ec90: 257d 0a7b 2520 666f 7220 6e20 696e 2072  %}.{% for n in r
+0001eca0: 616e 6765 2830 2c20 7769 6474 6829 2025  ange(0, width) %
+0001ecb0: 7d2d 7b25 2065 6e64 666f 7220 257d 0a0a  }-{% endfor %}..
+0001ecc0: 4e61 6d65 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  Name............
+0001ecd0: 2e2e 2e2e 2e3a 207b 7b20 7570 6e61 6d65  .....: {{ upname
+0001ece0: 207d 7d0a 4e75 6d62 6572 2e2e 2e2e 2e2e   }}.Number......
+0001ecf0: 2e2e 2e2e 2e2e 2e2e 2e3a 207b 7b20 6e75  .........: {{ nu
+0001ed00: 6d62 6572 207d 7d0a 5469 6d65 7374 616d  mber }}.Timestam
+0001ed10: 702e 2e2e 2e2e 2e2e 2e2e 2e2e 2e3a 207b  p............: {
+0001ed20: 7b20 5f64 7468 686d 6d20 7d7d 0a4f 7269  { _dthhmm }}.Ori
+0001ed30: 6769 6e61 6c20 7061 796c 6f61 642e 2e2e  ginal payload...
+0001ed40: 2e2e 3a20 7b7b 2070 6179 6c6f 6164 207d  ..: {{ payload }
+0001ed50: 7d0a 6060 600a 0a63 6f75 6c64 2070 726f  }.```..could pro
+0001ed60: 6475 6365 2074 6865 2066 6f6c 6c6f 7769  duce the followi
+0001ed70: 6e67 206d 6573 7361 6765 2c20 6f6e 2061  ng message, on a
+0001ed80: 6e79 2074 6172 6765 7420 7768 6963 6820  ny target which 
+0001ed90: 7573 6573 2074 6869 7320 636f 6e66 6967  uses this config
+0001eda0: 7572 6174 696f 6e2e 0a0a 6060 600a 2d2d  uration...```.--
+0001edb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001edc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001edd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001ede0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a4e 616d 652e  ----------.Name.
+0001edf0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+0001ee00: 3a20 4a41 4e45 204a 4f4c 4945 0a4e 756d  : JANE JOLIE.Num
+0001ee10: 6265 722e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ber.............
+0001ee20: 2e2e 3a20 3437 0a54 696d 6573 7461 6d70  ..: 47.Timestamp
+0001ee30: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 3a20 3139  ............: 19
+0001ee40: 3a31 350a 4f72 6967 696e 616c 2070 6179  :15.Original pay
+0001ee50: 6c6f 6164 2e2e 2e2e 2e3a 207b 226e 616d  load.....: {"nam
+0001ee60: 6522 3a22 4a61 6e65 204a 6f6c 6965 222c  e":"Jane Jolie",
+0001ee70: 226e 756d 6265 7222 3a34 372c 2022 6964  "number":47, "id
+0001ee80: 223a 3931 7d0a 6060 600a 0a4f 6e65 206f  ":91}.```..One o
+0001ee90: 6620 7468 6520 7465 6d70 6c61 7465 2076  f the template v
+0001eea0: 6172 6961 626c 6573 2079 6f75 206d 6179  ariables you may
+0001eeb0: 2062 6520 696e 7465 7265 7374 6564 2069   be interested i
+0001eec0: 6e20 6973 2063 616c 6c65 6420 607b 7b20  n is called `{{ 
+0001eed0: 7061 796c 6f61 6420 7d7d 603b 2074 6869  payload }}`; thi
+0001eee0: 730a 6361 7272 6965 7320 7468 6520 6f72  s.carries the or
+0001eef0: 6967 696e 616c 204d 5154 5420 6d65 7373  iginal MQTT mess
+0001ef00: 6167 6520 696e 2069 742e 2041 6c73 6f2c  age in it. Also,
+0001ef10: 2069 6620 7468 6520 7061 796c 6f61 6420   if the payload 
+0001ef20: 7761 7320 4a53 4f4e 2c20 7468 6f73 6520  was JSON, those 
+0001ef30: 6172 650a 6176 6169 6c61 626c 6520 616c  are.available al
+0001ef40: 736f 2028 6173 2073 686f 776e 2069 6e20  so (as shown in 
+0001ef50: 7468 6520 6162 6f76 6520 6578 616d 706c  the above exampl
+0001ef60: 6529 2c20 746f 6765 7468 6572 2077 6974  e), together wit
+0001ef70: 6820 616c 6c20 7468 6520 6f74 6865 720a  h all the other.
+0001ef80: 7472 616e 7366 6f72 6d61 7469 6f6e 2064  transformation d
+0001ef90: 6174 612e 0a0a 4966 2074 6865 2074 656d  ata...If the tem
+0001efa0: 706c 6174 6520 6361 6e6e 6f74 2062 6520  plate cannot be 
+0001efb0: 7265 6e64 6572 6564 2c20 7361 792c 2069  rendered, say, i
+0001efc0: 7420 636f 6e74 6169 6e73 2061 204a 696e  t contains a Jin
+0001efd0: 6a61 3220 6572 726f 7220 6f72 2074 6865  ja2 error or the
+0001efe0: 2074 656d 706c 6174 650a 6669 6c65 2063   template.file c
+0001eff0: 616e 6e6f 7420 6265 2066 6f75 6e64 2c20  annot be found, 
+0001f000: 6574 632e 2c20 7468 6520 6f72 6967 696e  etc., the origin
+0001f010: 616c 2072 6177 206d 6573 7361 6765 2069  al raw message i
+0001f020: 7320 7573 6564 2069 6e20 6c69 6575 206f  s used in lieu o
+0001f030: 6e20 6f75 7470 7574 2e0a 0a41 7320 6d65  n output...As me
+0001f040: 6e74 696f 6e65 6420 616c 7265 6164 792c  ntioned already,
+0001f050: 2077 6520 7468 696e 6b20 7468 6973 2069   we think this i
+0001f060: 7320 7573 6566 756c 2066 6f72 2074 6172  s useful for tar
+0001f070: 6765 7473 2077 6869 6368 2065 7870 6563  gets which expec
+0001f080: 7420 6120 6365 7274 6169 6e0a 616d 6f75  t a certain.amou
+0001f090: 6e74 206f 6620 7465 7874 2028 6066 696c  nt of text (`fil
+0001f0a0: 6560 2c20 6073 6d74 7060 2c20 616e 6420  e`, `smtp`, and 
+0001f0b0: 606e 6e74 7060 2063 6f6d 6520 746f 206d  `nntp` come to m
+0001f0c0: 696e 6429 2e0a 0a55 7365 206f 6620 7468  ind)...Use of th
+0001f0d0: 6973 2066 6561 7475 7265 2072 6571 7569  is feature requi
+0001f0e0: 7265 7320 5b4a 696e 6a61 325d 2c20 6275  res [Jinja2], bu
+0001f0f0: 7420 796f 7520 646f 6e27 7420 6861 7665  t you don't have
+0001f100: 2074 6f20 696e 7374 616c 6c20 6974 2069   to install it i
+0001f110: 6620 796f 7520 646f 6e27 7420 6e65 6564  f you don't need
+0001f120: 0a74 656d 706c 6174 696e 672e 0a0a 2323  .templating...##
+0001f130: 2050 6572 696f 6469 6320 7461 736b 730a   Periodic tasks.
+0001f140: 0a5f 6d71 7474 7761 726e 5f20 6361 6e20  ._mqttwarn_ can 
+0001f150: 7573 6520 6675 6e63 7469 6f6e 7320 796f  use functions yo
+0001f160: 7520 6465 6669 6e65 2069 6e20 7468 6520  u define in the 
+0001f170: 6669 6c65 2073 7065 6369 6669 6564 2060  file specified `
+0001f180: 5b64 6566 6175 6c74 735d 6020 7365 6374  [defaults]` sect
+0001f190: 696f 6e0a 746f 2070 6572 696f 6469 6361  ion.to periodica
+0001f1a0: 6c6c 7920 646f 2077 6861 7465 7665 7220  lly do whatever 
+0001f1b0: 796f 7520 7761 6e74 2c20 666f 7220 6578  you want, for ex
+0001f1c0: 616d 706c 652c 2070 7562 6c69 7368 2061  ample, publish a
+0001f1d0: 6e20 4d51 5454 206d 6573 7361 6765 2e20  n MQTT message. 
+0001f1e0: 5468 6572 650a 6172 6520 7477 6f20 7468  There.are two th
+0001f1f0: 696e 6773 2079 6f75 2068 6176 6520 746f  ings you have to
+0001f200: 2064 6f3a 0a0a 312e 2043 7265 6174 6520   do:..1. Create 
+0001f210: 7468 6520 6675 6e63 7469 6f6e 0a32 2e20  the function.2. 
+0001f220: 436f 6e66 6967 7572 6520 5f6d 7174 7477  Configure _mqttw
+0001f230: 6172 6e5f 2074 6f20 7573 6520 7468 6174  arn_ to use that
+0001f240: 2066 756e 6374 696f 6e20 616e 6420 7370   function and sp
+0001f250: 6563 6966 7920 7468 6520 696e 7465 7276  ecify the interv
+0001f260: 616c 2069 6e20 7365 636f 6e64 730a 0a41  al in seconds..A
+0001f270: 7373 756d 6520 7765 2068 6176 6520 7468  ssume we have th
+0001f280: 6520 666f 6c6c 6f77 696e 6720 6375 7374  e following cust
+0001f290: 6f6d 2066 756e 6374 696f 6e20 6465 6669  om function defi
+0001f2a0: 6e65 643a 0a0a 6060 6070 7974 686f 6e0a  ned:..```python.
+0001f2b0: 6465 6620 7069 6e67 6572 2873 7276 3d4e  def pinger(srv=N
+0001f2c0: 6f6e 6529 3a0a 2020 2020 7372 762e 6d71  one):.    srv.mq
+0001f2d0: 7474 632e 7075 626c 6973 6828 2270 742f  ttc.publish("pt/
+0001f2e0: 5049 4e47 4552 222c 2022 4865 6c6c 6f20  PINGER", "Hello 
+0001f2f0: 6672 6f6d 206d 7174 7477 6172 6e21 222c  from mqttwarn!",
+0001f300: 2071 6f73 3d30 290a 6060 600a 0a57 6520   qos=0).```..We 
+0001f310: 636f 6e66 6967 7572 6520 7468 6973 2066  configure this f
+0001f320: 756e 6374 696f 6e20 746f 2072 756e 2065  unction to run e
+0001f330: 7665 7279 2c20 7361 792c 2031 3020 7365  very, say, 10 se
+0001f340: 636f 6e64 732c 2069 6e20 7468 6520 606d  conds, in the `m
+0001f350: 7174 7477 6172 6e2e 696e 6960 2c0a 696e  qttwarn.ini`,.in
+0001f360: 2074 6865 2060 5b63 726f 6e5d 6020 7365   the `[cron]` se
+0001f370: 6374 696f 6e3a 0a0a 6060 6069 6e69 0a5b  ction:..```ini.[
+0001f380: 6372 6f6e 5d0a 7069 6e67 6572 203d 2031  cron].pinger = 1
+0001f390: 302e 350a 6060 600a 0a45 6163 6820 6b65  0.5.```..Each ke
+0001f3a0: 7977 6f72 6420 696e 2074 6865 2060 5b63  yword in the `[c
+0001f3b0: 726f 6e5d 6020 7365 6374 696f 6e20 7370  ron]` section sp
+0001f3c0: 6563 6966 6965 7320 7468 6520 6e61 6d65  ecifies the name
+0001f3d0: 206f 6620 6f6e 6520 6f66 2079 6f75 7220   of one of your 
+0001f3e0: 6375 7374 6f6d 0a66 756e 6374 696f 6e73  custom.functions
+0001f3f0: 2c20 616e 6420 6974 7320 666c 6f61 7420  , and its float 
+0001f400: 7661 6c75 6520 6973 2061 6e20 696e 7465  value is an inte
+0001f410: 7276 616c 2069 6e20 5f73 6563 6f6e 6473  rval in _seconds
+0001f420: 5f20 6166 7465 7220 7768 6963 6820 796f  _ after which yo
+0001f430: 7572 0a63 7573 746f 6d20 6675 6e63 7469  ur.custom functi
+0001f440: 6f6e 2028 5f70 696e 6765 7228 295f 2069  on (_pinger()_ i
+0001f450: 6e20 7468 6973 2063 6173 6529 2069 7320  n this case) is 
+0001f460: 696e 766f 6b65 642e 2059 6f75 7220 6675  invoked. Your fu
+0001f470: 6e63 7469 6f6e 2068 6173 2061 6363 6573  nction has acces
+0001f480: 730a 746f 2074 6865 2060 7372 7660 206f  s.to the `srv` o
+0001f490: 626a 6563 7420 2877 6869 6368 2077 6173  bject (which was
+0001f4a0: 2064 6573 6372 6962 6564 2065 6172 6c69   described earli
+0001f4b0: 6572 292e 0a0a 4675 6e63 7469 6f6e 206e  er)...Function n
+0001f4c0: 616d 6573 2061 7265 2074 6f20 6265 2073  ames are to be s
+0001f4d0: 7065 6369 6669 6564 2069 6e20 6c6f 7765  pecified in lowe
+0001f4e0: 722d 6361 7365 2063 6861 7261 6374 6572  r-case character
+0001f4f0: 732e 0a0a 4966 2079 6f75 2077 616e 7420  s...If you want 
+0001f500: 746f 2072 756e 2074 6865 2063 7573 746f  to run the custo
+0001f510: 6d20 6675 6e63 7469 6f6e 2069 6d6d 6564  m function immed
+0001f520: 6961 7465 6c79 2061 6674 6572 2073 7461  iately after sta
+0001f530: 7274 696e 6720 6d71 7474 7761 726e 0a69  rting mqttwarn.i
+0001f540: 6e73 7465 6164 206f 6620 7761 6974 696e  nstead of waitin
+0001f550: 6720 666f 7220 7468 6520 696e 7465 7276  g for the interv
+0001f560: 616c 2074 6f20 656c 6170 7365 2c20 796f  al to elapse, yo
+0001f570: 7520 6d69 6768 7420 7761 6e74 2074 6f20  u might want to 
+0001f580: 636f 6e66 6967 7572 653a 0a0a 6060 6069  configure:..```i
+0001f590: 6e69 0a5b 6372 6f6e 5d0a 7069 6e67 6572  ni.[cron].pinger
+0001f5a0: 203d 2031 302e 353b 206e 6f77 3d74 7275   = 10.5; now=tru
+0001f5b0: 650a 6060 600a 0a23 2320 446f 636b 6572  e.```..## Docker
+0001f5c0: 0a0a 496e 206f 7264 6572 2074 6f20 7275  ..In order to ru
+0001f5d0: 6e20 606d 7174 7477 6172 6e60 206f 6e20  n `mqttwarn` on 
+0001f5e0: 446f 636b 6572 2c20 706c 6561 7365 2066  Docker, please f
+0001f5f0: 6f6c 6c6f 7720 7570 2061 7420 5b44 4f43  ollow up at [DOC
+0001f600: 4b45 522e 6d64 5d28 444f 434b 4552 2e6d  KER.md](DOCKER.m
+0001f610: 6429 2e0a 0a0a 2323 204c 6f61 6469 6e67  d)....## Loading
+0001f620: 2065 7874 6572 6e61 6c20 7365 7276 6963   external servic
+0001f630: 6573 0a0a 496e 206f 7264 6572 2074 6f20  es..In order to 
+0001f640: 6272 696e 6720 696e 2063 7573 746f 6d20  bring in custom 
+0001f650: 656d 6974 7465 7220 6d61 6368 696e 6572  emitter machiner
+0001f660: 7920 746f 2060 6d71 7474 7761 726e 6020  y to `mqttwarn` 
+0001f670: 696e 2066 6f72 6d20 6f66 2073 6572 7669  in form of servi
+0001f680: 6365 0a70 6c75 6769 6e73 2c20 7468 6572  ce.plugins, ther
+0001f690: 6520 6172 6520 7477 6f20 6f70 7469 6f6e  e are two option
+0001f6a0: 732e 0a0a 0a23 2323 2053 6572 7669 6365  s....### Service
+0001f6b0: 2070 6c75 6769 6e20 6672 6f6d 2070 6163   plugin from pac
+0001f6c0: 6b61 6765 0a0a 5468 6973 2063 6f6e 6669  kage..This confi
+0001f6d0: 6775 7261 7469 6f6e 2073 6e69 7070 6574  guration snippet
+0001f6e0: 206f 7574 6c69 6e65 7320 686f 7720 746f   outlines how to
+0001f6f0: 206c 6f61 6420 6120 6375 7374 6f6d 2070   load a custom p
+0001f700: 6c75 6769 6e20 6672 6f6d 2061 2050 7974  lugin from a Pyt
+0001f710: 686f 6e0a 6d6f 6475 6c65 2072 6566 6572  hon.module refer
+0001f720: 656e 6365 6420 696e 2022 646f 7474 6564  enced in "dotted
+0001f730: 2220 6e6f 7461 7469 6f6e 2e20 4d6f 6475  " notation. Modu
+0001f740: 6c65 7320 7769 6c6c 2062 6520 7365 6172  les will be sear
+0001f750: 6368 6564 2066 6f72 2069 6e20 616c 6c0a  ched for in all.
+0001f760: 6469 7265 6374 6f72 6965 7320 6c69 7374  directories list
+0001f770: 6564 2069 6e20 5b60 7379 732e 7061 7468  ed in [`sys.path
+0001f780: 605d 2e20 4375 7374 6f6d 2064 6972 6563  `]. Custom direc
+0001f790: 746f 7269 6573 2063 616e 2062 6520 6164  tories can be ad
+0001f7a0: 6465 6420 6279 2075 7369 6e67 2074 6865  ded by using the
+0001f7b0: 0a5b 6050 5954 484f 4e50 4154 4860 5d20  .[`PYTHONPATH`] 
+0001f7c0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+0001f7d0: 6162 6c65 2e0a 0a5b 6073 7973 2e70 6174  able...[`sys.pat
+0001f7e0: 6860 5d3a 2068 7474 7073 3a2f 2f64 6f63  h`]: https://doc
+0001f7f0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+0001f800: 6962 7261 7279 2f73 7973 2e68 746d 6c23  ibrary/sys.html#
+0001f810: 7379 732e 7061 7468 0a5b 6050 5954 484f  sys.path.[`PYTHO
+0001f820: 4e50 4154 4860 5d3a 2068 7474 7073 3a2f  NPATH`]: https:/
+0001f830: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
+0001f840: 2f33 2f75 7369 6e67 2f63 6d64 6c69 6e65  /3/using/cmdline
+0001f850: 2e68 746d 6c23 656e 7676 6172 2d50 5954  .html#envvar-PYT
+0001f860: 484f 4e50 4154 480a 0a60 6060 696e 690a  HONPATH..```ini.
+0001f870: 5b64 6566 6175 6c74 735d 0a3b 206e 616d  [defaults].; nam
+0001f880: 6520 7468 6520 7365 7276 6963 6520 7072  e the service pr
+0001f890: 6f76 6964 6572 7320 796f 7520 7769 6c6c  oviders you will
+0001f8a0: 2062 6520 7573 696e 672e 0a6c 6175 6e63   be using..launc
+0001f8b0: 6820 2020 203d 206c 6f67 2c20 6669 6c65  h    = log, file
+0001f8c0: 2c20 7465 7374 732e 6163 6d65 2e66 6f6f  , tests.acme.foo
+0001f8d0: 6261 720a 0a5b 7465 7374 2f70 6c75 6769  bar..[test/plugi
+0001f8e0: 6e2d 6d6f 6475 6c65 5d0a 3b20 6563 686f  n-module].; echo
+0001f8f0: 2027 7b22 6e61 6d65 223a 2022 7465 6d70   '{"name": "temp
+0001f900: 6572 6174 7572 6522 2c20 2276 616c 7565  erature", "value
+0001f910: 223a 2034 322e 3432 7d27 207c 206d 6f73  ": 42.42}' | mos
+0001f920: 7175 6974 746f 5f70 7562 202d 6820 6c6f  quitto_pub -h lo
+0001f930: 6361 6c68 6f73 7420 2d74 2074 6573 742f  calhost -t test/
+0001f940: 706c 7567 696e 2d6d 6f64 756c 6520 2d6c  plugin-module -l
+0001f950: 0a74 6172 6765 7473 203d 2074 6573 7473  .targets = tests
+0001f960: 2e61 636d 652e 666f 6f62 6172 3a64 6566  .acme.foobar:def
+0001f970: 6175 6c74 0a66 6f72 6d61 7420 3d20 7b6e  ault.format = {n
+0001f980: 616d 657d 3a20 7b76 616c 7565 7d0a 0a5b  ame}: {value}..[
+0001f990: 636f 6e66 6967 3a74 6573 7473 2e61 636d  config:tests.acm
+0001f9a0: 652e 666f 6f62 6172 5d0a 7461 7267 6574  e.foobar].target
+0001f9b0: 7320 3d20 7b0a 2020 2020 2764 6566 6175  s = {.    'defau
+0001f9c0: 6c74 2720 203a 205b 2027 6465 6661 756c  lt'  : [ 'defaul
+0001f9d0: 7427 205d 2c0a 2020 7d0a 6060 600a 0a23  t' ],.  }.```..#
+0001f9e0: 2323 2053 6572 7669 6365 2070 6c75 6769  ## Service plugi
+0001f9f0: 6e20 6672 6f6d 2066 696c 650a 0a54 6869  n from file..Thi
+0001fa00: 7320 636f 6e66 6967 7572 6174 696f 6e20  s configuration 
+0001fa10: 736e 6970 7065 7420 6f75 746c 696e 6573  snippet outlines
+0001fa20: 2068 6f77 2074 6f20 6c6f 6164 2061 2063   how to load a c
+0001fa30: 7573 746f 6d20 706c 7567 696e 2066 726f  ustom plugin fro
+0001fa40: 6d20 6120 5079 7468 6f6e 0a66 696c 6520  m a Python.file 
+0001fa50: 7265 6665 7265 6e63 6564 2062 7920 6669  referenced by fi
+0001fa60: 6c65 206e 616d 652e 2057 6865 6e20 7265  le name. When re
+0001fa70: 6c61 7469 7665 2066 696c 6520 6e61 6d65  lative file name
+0001fa80: 7320 6172 6520 6769 7665 6e2c 2074 6865  s are given, the
+0001fa90: 7920 7769 6c6c 2062 650a 7265 736f 6c76  y will be.resolv
+0001faa0: 6564 2066 726f 6d20 7468 6520 6469 7265  ed from the dire
+0001fab0: 6374 6f72 7920 6f66 2074 6865 2060 6d71  ctory of the `mq
+0001fac0: 7474 7761 726e 2e69 6e69 6020 6669 6c65  ttwarn.ini` file
+0001fad0: 2c20 7768 6963 6820 6973 2c20 6279 2064  , which is, by d
+0001fae0: 6566 6175 6c74 2c0a 7468 6520 602f 6574  efault,.the `/et
+0001faf0: 632f 6d71 7474 7761 726e 6020 666f 6c64  c/mqttwarn` fold
+0001fb00: 6572 2e0a 0a60 6060 696e 690a 5b64 6566  er...```ini.[def
+0001fb10: 6175 6c74 735d 0a3b 206e 616d 6520 7468  aults].; name th
+0001fb20: 6520 7365 7276 6963 6520 7072 6f76 6964  e service provid
+0001fb30: 6572 7320 796f 7520 7769 6c6c 2062 6520  ers you will be 
+0001fb40: 7573 696e 672e 0a6c 6175 6e63 6820 2020  using..launch   
+0001fb50: 203d 206c 6f67 2c20 6669 6c65 2c20 7465   = log, file, te
+0001fb60: 7374 732f 6163 6d65 2f66 6f6f 6261 722e  sts/acme/foobar.
+0001fb70: 7079 0a0a 5b74 6573 742f 706c 7567 696e  py..[test/plugin
+0001fb80: 2d66 696c 655d 0a3b 2065 6368 6f20 277b  -file].; echo '{
+0001fb90: 226e 616d 6522 3a20 2274 656d 7065 7261  "name": "tempera
+0001fba0: 7475 7265 222c 2022 7661 6c75 6522 3a20  ture", "value": 
+0001fbb0: 3432 2e34 327d 2720 7c20 6d6f 7371 7569  42.42}' | mosqui
+0001fbc0: 7474 6f5f 7075 6220 2d68 206c 6f63 616c  tto_pub -h local
+0001fbd0: 686f 7374 202d 7420 7465 7374 2f70 6c75  host -t test/plu
+0001fbe0: 6769 6e2d 6669 6c65 202d 6c0a 7461 7267  gin-file -l.targ
+0001fbf0: 6574 7320 3d20 7465 7374 732f 6163 6d65  ets = tests/acme
+0001fc00: 2f66 6f6f 6261 722e 7079 3a64 6566 6175  /foobar.py:defau
+0001fc10: 6c74 0a66 6f72 6d61 7420 3d20 7b6e 616d  lt.format = {nam
+0001fc20: 657d 3a20 7b76 616c 7565 7d0a 0a5b 636f  e}: {value}..[co
+0001fc30: 6e66 6967 3a74 6573 7473 2f61 636d 652f  nfig:tests/acme/
+0001fc40: 666f 6f62 6172 2e70 795d 0a74 6172 6765  foobar.py].targe
+0001fc50: 7473 203d 207b 0a20 2020 2027 6465 6661  ts = {.    'defa
+0001fc60: 756c 7427 2020 3a20 5b20 2764 6566 6175  ult'  : [ 'defau
+0001fc70: 6c74 2720 5d2c 0a20 207d 0a60 6060 0a0a  lt' ],.  }.```..
+0001fc80: 0a23 2320 4578 616d 706c 6573 2023 230a  .## Examples ##.
+0001fc90: 0a54 6869 7320 7365 6374 696f 6e20 636f  .This section co
+0001fca0: 6e74 6169 6e73 2073 6f6d 6520 6578 616d  ntains some exam
+0001fcb0: 706c 6573 206f 6620 686f 7720 606d 7174  ples of how `mqt
+0001fcc0: 7477 6172 6e60 2063 616e 2062 6520 7573  twarn` can be us
+0001fcd0: 6564 2077 6974 6820 736f 6d65 206d 6f72  ed with some mor
+0001fce0: 6520 636f 6d70 6c65 7820 636f 6e66 6967  e complex config
+0001fcf0: 7572 6174 696f 6e73 2e0a 0a23 2323 204c  urations...### L
+0001fd00: 6f77 2062 6174 7465 7279 206e 6f74 6966  ow battery notif
+0001fd10: 6963 6174 696f 6e73 2023 2323 0a0a 4279  ications ###..By
+0001fd20: 2073 7562 7363 7269 6269 6e67 2074 6f20   subscribing to 
+0001fd30: 796f 7572 205b 4f77 6e54 7261 636b 735d  your [OwnTracks]
+0001fd40: 2074 6f70 6963 2061 6e64 2061 6464 696e   topic and addin
+0001fd50: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
+0001fd60: 6375 7374 6f6d 2066 696c 7465 7220 796f  custom filter yo
+0001fd70: 7520 6361 6e20 6765 7420 606d 7174 7477  u can get `mqttw
+0001fd80: 6172 6e60 2074 6f20 7365 6e64 206e 6f74  arn` to send not
+0001fd90: 6966 6963 6174 696f 6e73 2077 6865 6e20  ifications when 
+0001fda0: 796f 7572 2070 686f 6e65 2062 6174 7465  your phone batte
+0001fdb0: 7279 2067 6574 7320 6265 6c6f 7720 6120  ry gets below a 
+0001fdc0: 6365 7274 6169 6e20 6c65 7665 6c3b 0a0a  certain level;..
+0001fdd0: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+0001fde0: 206a 736f 6e0a 0a64 6566 206f 776e 7472   json..def owntr
+0001fdf0: 6163 6b73 5f62 6174 7466 696c 7465 7228  acks_battfilter(
+0001fe00: 746f 7069 632c 206d 6573 7361 6765 293a  topic, message):
+0001fe10: 0a20 2020 2064 6174 6120 3d20 6469 6374  .    data = dict
+0001fe20: 286a 736f 6e2e 6c6f 6164 7328 6d65 7373  (json.loads(mess
+0001fe30: 6167 6529 2e69 7465 6d73 2829 290a 2020  age).items()).  
+0001fe40: 2020 6966 2064 6174 615b 2762 6174 7427    if data['batt'
+0001fe50: 5d20 6973 206e 6f74 204e 6f6e 653a 0a20  ] is not None:. 
+0001fe60: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+0001fe70: 7428 6461 7461 5b27 6261 7474 275d 2920  t(data['batt']) 
+0001fe80: 3e20 3230 0a20 2020 2072 6574 7572 6e20  > 20.    return 
+0001fe90: 5472 7565 0a60 6060 0a0a 4e6f 7720 7369  True.```..Now si
+0001fea0: 6d70 6c79 2061 6464 2079 6f75 7220 6368  mply add your ch
+0001feb0: 6f69 6365 206f 6620 7461 7267 6574 2873  oice of target(s
+0001fec0: 2920 746f 2074 6865 2074 6f70 6963 2773  ) to the topic's
+0001fed0: 2073 6563 7469 6f6e 2061 6e64 2061 206e   section and a n
+0001fee0: 6963 6520 666f 726d 6174 2073 7472 696e  ice format strin
+0001fef0: 6720 616e 6420 796f 7520 6172 6520 646f  g and you are do
+0001ff00: 6e65 3b0a 0a60 6060 696e 690a 5b6f 776e  ne;..```ini.[own
+0001ff10: 7472 6163 6b73 2f23 5d0a 7461 7267 6574  tracks/#].target
+0001ff20: 7320 3d20 7075 7368 6f76 6572 2c20 7862  s = pushover, xb
+0001ff30: 6d63 0a66 696c 7465 7220 3d20 6f77 6e74  mc.filter = ownt
+0001ff40: 7261 636b 735f 6261 7474 6669 6c74 6572  racks_battfilter
+0001ff50: 2829 0a66 6f72 6d61 7420 3d20 4d79 2070  ().format = My p
+0001ff60: 686f 6e65 2062 6174 7465 7279 2069 7320  hone battery is 
+0001ff70: 6765 7474 696e 6720 6c6f 7720 287b 6261  getting low ({ba
+0001ff80: 7474 7d25 2921 0a60 6060 0a0a 2323 2320  tt}%)!.```..### 
+0001ff90: 5072 6f64 7563 696e 6720 4a53 4f4e 0a0a  Producing JSON..
+0001ffa0: 4173 7375 6d69 6e67 2077 6520 6765 742c  Assuming we get,
+0001ffb0: 2066 726f 6d20 616e 2041 7264 7569 6e6f   from an Arduino
+0001ffc0: 2c20 7361 792c 2061 2073 696e 676c 6520  , say, a single 
+0001ffd0: 6e75 6d65 7269 6361 6c20 7661 6c75 6520  numerical value 
+0001ffe0: 696e 2074 6865 2070 6179 6c6f 6164 206f  in the payload o
+0001fff0: 6620 616e 204d 5154 540a 6d65 7373 6167  f an MQTT.messag
+00020000: 652c 2077 6520 7761 6e74 2074 6f20 6765  e, we want to ge
+00020010: 6e65 7261 7465 204a 534f 4e20 7769 7468  nerate JSON with
+00020020: 2073 6f6d 6520 6164 6469 7469 6f6e 616c   some additional
+00020030: 2066 6965 6c64 732e 2055 7369 6e67 2061   fields. Using a
+00020040: 204a 696e 6a61 3220 7465 6d70 6c61 7465   Jinja2 template
+00020050: 0a66 6f72 2074 6865 2074 6173 6b2c 2064  .for the task, d
+00020060: 6f65 7320 6578 6163 746c 7920 7768 6174  oes exactly what
+00020070: 2077 6520 6e65 6564 3a0a 0a54 6865 2066   we need:..The f
+00020080: 6f6c 6c6f 7769 6e67 2074 6172 6765 7420  ollowing target 
+00020090: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
+000200a0: 766f 6b65 7320 7468 6520 7465 6d70 6c61  vokes the templa
+000200b0: 7465 3a0a 0a60 6060 696e 690a 5b61 7264  te:..```ini.[ard
+000200c0: 7569 6e6f 2f74 656d 705d 0a74 6172 6765  uino/temp].targe
+000200d0: 7473 203d 206c 6f67 3a69 6e66 6f2c 2068  ts = log:info, h
+000200e0: 7474 703a 6772 6179 6c6f 6732 0a74 656d  ttp:graylog2.tem
+000200f0: 706c 6174 6520 3d20 7465 6d70 326a 736f  plate = temp2jso
+00020100: 6e2e 6a73 6f6e 0a60 6060 0a0a 5468 6520  n.json.```..The 
+00020110: 4a69 6e6a 6132 2074 656d 706c 6174 6520  Jinja2 template 
+00020120: 6c6f 6f6b 7320 6c69 6b65 2074 6869 733a  looks like this:
+00020130: 0a0a 6060 606a 696e 6a61 320a 7b23 0a20  ..```jinja2.{#. 
+00020140: 2020 2057 6520 6578 7065 6374 2061 2073     We expect a s
+00020150: 696e 676c 6520 6e75 6d65 7269 6320 7465  ingle numeric te
+00020160: 6d70 6572 6174 7572 6520 7661 6c75 6520  mperature value 
+00020170: 696e 2060 7061 796c 6f61 6427 0a20 2020  in `payload'.   
+00020180: 2052 6574 7572 6e20 4a53 4f4e 2073 7569   Return JSON sui
+00020190: 7461 626c 6520 666f 7220 4772 6179 6c6f  table for Graylo
+000201a0: 6732 2028 7265 7175 6972 6573 2068 6f73  g2 (requires hos
+000201b0: 7420 616e 6420 7368 6f72 745f 6d65 7373  t and short_mess
+000201c0: 6167 6529 0a0a 2020 2020 4465 6669 6e65  age)..    Define
+000201d0: 2061 2064 6174 6120 7374 7275 6374 7572   a data structur
+000201e0: 6520 696e 204a 696e 6a61 3220 616e 6420  e in Jinja2 and 
+000201f0: 7265 7475 726e 2069 7420 6173 2061 204a  return it as a J
+00020200: 534f 4e20 7374 7269 6e67 2e0a 2020 2020  SON string..    
+00020210: 4e6f 7465 2068 6f77 2074 7261 6e73 666f  Note how transfo
+00020220: 726d 6174 696f 6e20 6461 7461 2028 7072  rmation data (pr
+00020230: 6f64 7563 6564 2077 6974 6869 6e20 6d71  oduced within mq
+00020240: 7474 7761 726e 2920 6973 2075 7365 643a  ttwarn) is used:
+00020250: 0a20 2020 2074 6865 2076 6172 6961 626c  .    the variabl
+00020260: 6573 2060 5f64 7469 736f 2720 616e 6420  es `_dtiso' and 
+00020270: 6070 6179 6c6f 6164 2720 636f 6e74 6169  `payload' contai
+00020280: 6e20 6120 7469 6d65 7374 616d 7020 616e  n a timestamp an
+00020290: 6420 6f75 720a 2020 2020 7061 796c 6f61  d our.    payloa
+000202a0: 6420 7265 7370 6563 7469 7665 6c79 2e0a  d respectively..
+000202b0: 237d 0a7b 2520 7365 7420 6461 7461 203d  #}.{% set data =
+000202c0: 207b 0a09 2768 6f73 7427 0909 3a20 746f   {..'host'..: to
+000202d0: 7069 632c 0a09 2773 686f 7274 5f6d 6573  pic,..'short_mes
+000202e0: 7361 6765 2709 3a20 2248 6561 7420 2220  sage'.: "Heat " 
+000202f0: 2b20 7061 796c 6f61 642c 0a09 2774 7374  + payload,..'tst
+00020300: 2709 093a 205f 6474 6973 6f2c 0a09 2774  '..: _dtiso,..'t
+00020310: 656d 7065 7261 7475 7265 2709 3a20 7061  emperature'.: pa
+00020320: 796c 6f61 642c 0a09 2777 6f6f 686f 6f6f  yload,..'woohooo
+00020330: 2709 3a20 3137 2c0a 097d 0a09 257d 0a7b  '.: 17,..}..%}.{
+00020340: 7b20 6461 7461 207c 206a 736f 6e69 6679  { data | jsonify
+00020350: 207d 7d0a 6060 600a 0a61 6e64 2061 6e20   }}.```..and an 
+00020360: 6578 616d 706c 6520 4a53 4f4e 2073 7472  example JSON str
+00020370: 696e 6720 7265 7475 726e 6564 2062 7920  ing returned by 
+00020380: 7468 6174 2074 656d 706c 6174 6520 6973  that template is
+00020390: 2074 6865 6e20 7061 7373 6564 2074 6f20   then passed to 
+000203a0: 6f75 7220 636f 6e66 6967 7572 6564 0a74  our configured.t
+000203b0: 6172 6765 7473 3a0a 0a60 6060 6a73 6f6e  argets:..```json
+000203c0: 0a7b 2268 6f73 7422 3a20 2261 7264 7569  .{"host": "ardui
+000203d0: 6e6f 2f74 656d 7022 2c20 2277 6f6f 686f  no/temp", "wooho
+000203e0: 6f6f 223a 2031 372c 2022 7473 7422 3a20  oo": 17, "tst": 
+000203f0: 2232 3031 342d 3034 2d31 3354 3039 3a32  "2014-04-13T09:2
+00020400: 353a 3436 2e32 3437 3135 305a 222c 2022  5:46.247150Z", "
+00020410: 7465 6d70 6572 6174 7572 6522 3a20 2232  temperature": "2
+00020420: 3222 2c20 2273 686f 7274 5f6d 6573 7361  2", "short_messa
+00020430: 6765 223a 2022 4865 6174 2032 3222 7d0a  ge": "Heat 22"}.
+00020440: 6060 600a 0a0a 2323 2320 416d 617a 6f6e  ```...### Amazon
+00020450: 2041 6c65 7861 0a0a 416e 2061 6c74 6572   Alexa..An alter
+00020460: 6e61 7469 7665 2074 6f20 616c 6578 612d  native to alexa-
+00020470: 6e6f 7469 6679 2d6d 6520 6e6f 7469 6669  notify-me notifi
+00020480: 6361 7469 6f6e 2028 7370 6561 6b65 7220  cation (speaker 
+00020490: 676c 6f77 7320 7965 6c6c 6f77 2061 6e64  glows yellow and
+000204a0: 2061 7761 6974 7320 696e 7374 7275 6374   awaits instruct
+000204b0: 696f 6e20 746f 2070 6c61 7920 7468 6520  ion to play the 
+000204c0: 6e6f 7469 6669 6361 7469 6f6e 2920 6973  notification) is
+000204d0: 2074 6f20 666f 7220 5454 5320 746f 2073   to for TTS to s
+000204e0: 7065 6369 6669 6320 6465 7669 6365 7320  pecific devices 
+000204f0: 6f72 2061 6e6e 6f75 6e63 6520 746f 2061  or announce to a
+00020500: 2073 7065 616b 6572 2067 726f 7570 2e0a   speaker group..
+00020510: 0a53 6565 2074 6865 2065 7861 6d70 6c65  .See the example
+00020520: 7320 6469 7265 6374 6f72 7920 666f 7220  s directory for 
+00020530: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
+00020540: 2070 6970 6520 616e 6420 6874 7470 733a   pipe and https:
+00020550: 2f2f 6769 7468 7562 2e63 6f6d 2f74 686f  //github.com/tho
+00020560: 7273 7465 6e2d 6765 6872 6967 2f61 6c65  rsten-gehrig/ale
+00020570: 7861 2d72 656d 6f74 652d 636f 6e74 726f  xa-remote-contro
+00020580: 6c20 7368 656c 6c20 7363 7269 7074 732e  l shell scripts.
+00020590: 0a0a 496e 7374 7275 6374 696f 6e73 3a0a  ..Instructions:.
+000205a0: 0a2a 2044 6f77 6e6c 6f61 642f 6368 6563  .* Download/chec
+000205b0: 6b6f 7574 2068 7474 7073 3a2f 2f67 6974  kout https://git
+000205c0: 6875 622e 636f 6d2f 7468 6f72 7374 656e  hub.com/thorsten
+000205d0: 2d67 6568 7269 672f 616c 6578 612d 7265  -gehrig/alexa-re
+000205e0: 6d6f 7465 2d63 6f6e 7472 6f6c 0a2a 2045  mote-control.* E
+000205f0: 6469 7420 7365 6372 6574 732e 7368 0a2a  dit secrets.sh.*
+00020600: 2045 6e73 7572 6520 7061 7468 7320 6172   Ensure paths ar
+00020610: 6520 636f 7272 6563 7420 2873 6372 6970  e correct (scrip
+00020620: 7473 2061 6e64 2069 6e69 2066 696c 6520  ts and ini file 
+00020630: 6173 7375 6d65 2070 6174 6820 2f68 6f6d  assume path /hom
+00020640: 652f 7069 2f73 6865 6c6c 2f61 6c65 7861  e/pi/shell/alexa
+00020650: 2d72 656d 6f74 652d 636f 6e74 726f 6c29  -remote-control)
+00020660: 0a2a 2045 6469 7420 696e 6920 6669 6c65  .* Edit ini file
+00020670: 2074 6172 6765 7473 2077 6974 6820 6465   targets with de
+00020680: 7669 6365 206e 616d 6573 2061 6e64 2f6f  vice names and/o
+00020690: 7220 6772 6f75 7020 6e61 6d65 2028 7361  r group name (sa
+000206a0: 7973 7464 696e 2066 6f72 2073 696e 676c  ystdin for singl
+000206b0: 6520 6465 7669 6365 732c 2061 6e6e 6f75  e devices, annou
+000206c0: 6e63 655f 7374 6469 6e20 666f 7220 6772  nce_stdin for gr
+000206d0: 6f75 7073 290a 2a20 5361 6e69 7479 2063  oups).* Sanity c
+000206e0: 6865 636b 2c20 6368 6d6f 6420 612b 7820  heck, chmod a+x 
+000206f0: 6f6e 2061 6c6c 2073 6865 6c6c 2073 6372  on all shell scr
+00020700: 6970 7473 0a0a 0a0a 2323 204e 6f74 6573  ipts....## Notes
+00020710: 0a0a 224d 5154 5422 2069 7320 6120 7472  .."MQTT" is a tr
+00020720: 6164 656d 6172 6b20 6f66 2074 6865 204f  ademark of the O
+00020730: 4153 4953 206f 7065 6e20 7374 616e 6461  ASIS open standa
+00020740: 7264 7320 636f 6e73 6f72 7469 756d 2c20  rds consortium, 
+00020750: 7768 6963 6820 7075 626c 6973 6865 7320  which publishes 
+00020760: 7468 6520 4d51 5454 2073 7065 6369 6669  the MQTT specifi
+00020770: 6361 7469 6f6e 732e 0a0a 0a0a 2323 2050  cations.....## P
+00020780: 7265 7373 0a0a 2a20 5b4d 5154 5477 6172  ress..* [MQTTwar
+00020790: 6e3a 2045 696e 2052 756e 6475 6d2d 536f  n: Ein Rundum-So
+000207a0: 7267 6c6f 732d 4e6f 7469 6669 6572 5d28  rglos-Notifier](
+000207b0: 6874 7470 3a2f 2f6a 6178 656e 7465 722e  http://jaxenter.
+000207c0: 6465 2f6e 6577 732f 4d51 5454 7761 726e  de/news/MQTTwarn
+000207d0: 2d45 696e 2d52 756e 6475 6d2d 536f 7267  -Ein-Rundum-Sorg
+000207e0: 6c6f 732d 4e6f 7469 6669 6572 2d31 3731  los-Notifier-171
+000207f0: 3331 3229 2c20 6172 7469 636c 6520 696e  312), article in
+00020800: 2047 6572 6d61 6e20 6174 204a 4158 656e   German at JAXen
+00020810: 7465 722e 0a2a 205b 5363 6877 6172 6d61  ter..* [Schwarma
+00020820: 6c61 726d 2075 7369 6e67 206d 7174 7477  larm using mqttw
+00020830: 6172 6e5d 2868 7474 7073 3a2f 2f68 6976  arn](https://hiv
+00020840: 6565 7965 732e 6f72 672f 646f 6373 2f73  eeyes.org/docs/s
+00020850: 7973 7465 6d2f 7363 6877 6172 6d61 6c61  ystem/schwarmala
+00020860: 726d 2d6d 7174 7477 6172 6e2e 6874 6d6c  rm-mqttwarn.html
+00020870: 290a 0a20 205b 4f77 6e54 7261 636b 735d  )..  [OwnTracks]
+00020880: 3a20 6874 7470 3a2f 2f6f 776e 7472 6163  : http://owntrac
+00020890: 6b73 2e6f 7267 0a20 205b 4a69 6e6a 6132  ks.org.  [Jinja2
+000208a0: 5d3a 2068 7474 703a 2f2f 6a69 6e6a 612e  ]: http://jinja.
+000208b0: 706f 636f 6f2e 6f72 672f 646f 6373 2f74  pocoo.org/docs/t
+000208c0: 656d 706c 6174 6573 2f0a 2020 5b5a 6162  emplates/.  [Zab
+000208d0: 6269 785d 3a20 6874 7470 3a2f 2f7a 6162  bix]: http://zab
+000208e0: 6269 782e 636f 6d0a                      bix.com.
```

### Comparing `mqttwarn-0.32.0/LICENSE` & `mqttwarn-0.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/PKG-INFO` & `mqttwarn-0.33.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttwarn
-Version: 0.32.0
+Version: 0.33.0
 Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
 Home-page: https://github.com/jpmens/mqttwarn
 Author: Jan-Piet Mens, Ben Jones, Andreas Motl
 Author-email: jpmens@gmail.com
 License: EPL 2.0
 Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
 Classifier: Development Status :: 4 - Beta
@@ -343,15 +343,15 @@
 There are also some extensions to mqttwarn not included in the core package.
 Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
 `community contributions to mqttwarn`_.
 
 
 Licenses
 ========
-This software is copyright © 2014-2022 Jan-Piet Mens and contributors. All
+This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
@@ -373,23 +373,14 @@
 Press
 =====
 * The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
 * The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
   as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
 
 
-Notes
-=====
-*mqttwarn* is currently undergoing some refurbishment and will also be
-ported to Python 3 during that phase. You are welcome to participate!
-
-We outlined the tasks for the next releases within the backlog_.
-They might be transferred into GitHub issues progressively, if applicable.
-
-
 Legal stuff
 ===========
 "MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
 
 
 ----
```

### Comparing `mqttwarn-0.32.0/README.rst` & `mqttwarn-0.33.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 There are also some extensions to mqttwarn not included in the core package.
 Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
 `community contributions to mqttwarn`_.
 
 
 Licenses
 ========
-This software is copyright © 2014-2022 Jan-Piet Mens and contributors. All
+This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
@@ -290,23 +290,14 @@
 Press
 =====
 * The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
 * The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
   as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
 
 
-Notes
-=====
-*mqttwarn* is currently undergoing some refurbishment and will also be
-ported to Python 3 during that phase. You are welcome to participate!
-
-We outlined the tasks for the next releases within the backlog_.
-They might be transferred into GitHub issues progressively, if applicable.
-
-
 Legal stuff
 ===========
 "MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
 
 
 ----
```

### Comparing `mqttwarn-0.32.0/mqttwarn/commands.py` & `mqttwarn-0.33.0/mqttwarn/commands.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/configuration.py` & `mqttwarn-0.33.0/mqttwarn/configuration.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/context.py` & `mqttwarn-0.33.0/mqttwarn/context.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/core.py` & `mqttwarn-0.33.0/mqttwarn/core.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/cron.py` & `mqttwarn-0.33.0/mqttwarn/cron.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/examples/basic/mqttwarn.ini` & `mqttwarn-0.33.0/mqttwarn/examples/basic/mqttwarn.ini`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/examples/basic/samplefuncs.py` & `mqttwarn-0.33.0/mqttwarn/examples/basic/samplefuncs.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/model.py` & `mqttwarn-0.33.0/mqttwarn/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,24 +33,30 @@
     def enum(self):
         item = {}
         for (k, v) in list(self.__dict__.items()):
             item[k] = v
         return item
 
 
+# Covering old- and new-style configuration layouts. `addrs` has
+# originally been a list of strings, has been expanded to be a
+# list of dictionaries (Apprise), and to be a dictionary (Pushsafer).
+addrs_type = Union[List[Union[str, Dict[str, str]]], Dict[str, str]]
+
+
 @dataclass
 class ProcessorItem:
     """
     Data container for feeding information into service plugins - V2.
     """
 
     service: Optional[str] = None
     target: Optional[str] = None
     config: Dict = field(default_factory=dict)
-    addrs: List[Union[str, Dict[str, str]]] = field(default_factory=list)
+    addrs: addrs_type = field(default_factory=list)  # type: ignore[assignment]
     priority: Optional[int] = None
     topic: Optional[str] = None
     title: Optional[str] = None
     message: Optional[Union[str, bytes]] = None
     data: Optional[Dict] = None
 
     def asdict(self):
```

### Comparing `mqttwarn-0.32.0/mqttwarn/services/alexa-notify-me.py` & `mqttwarn-0.33.0/mqttwarn/services/alexa-notify-me.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/amqp.py` & `mqttwarn-0.33.0/mqttwarn/services/amqp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/apns.py` & `mqttwarn-0.33.0/mqttwarn/services/apns.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/apprise_multi.py` & `mqttwarn-0.33.0/mqttwarn/services/apprise_multi.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/apprise_single.py` & `mqttwarn-0.33.0/mqttwarn/services/apprise_single.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/apprise_util.py` & `mqttwarn-0.33.0/mqttwarn/services/apprise_util.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/asterisk.py` & `mqttwarn-0.33.0/mqttwarn/services/asterisk.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/autoremote.py` & `mqttwarn-0.33.0/mqttwarn/services/autoremote.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/azure_iot.py` & `mqttwarn-0.33.0/mqttwarn/services/azure_iot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/carbon.py` & `mqttwarn-0.33.0/mqttwarn/services/carbon.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/celery.py` & `mqttwarn-0.33.0/mqttwarn/services/celery.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/chromecast.py` & `mqttwarn-0.33.0/mqttwarn/services/chromecast.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/dbus.py` & `mqttwarn-0.33.0/mqttwarn/services/dbus.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/desktopnotify.py` & `mqttwarn-0.33.0/mqttwarn/services/desktopnotify.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/dnsupdate.py` & `mqttwarn-0.33.0/mqttwarn/services/dnsupdate.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/emoncms.py` & `mqttwarn-0.33.0/mqttwarn/services/emoncms.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/execute.py` & `mqttwarn-0.33.0/mqttwarn/services/execute.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/fbchat.py` & `mqttwarn-0.33.0/mqttwarn/services/fbchat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/file.py` & `mqttwarn-0.33.0/mqttwarn/services/file.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/freeswitch.py` & `mqttwarn-0.33.0/mqttwarn/services/freeswitch.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/gss.py` & `mqttwarn-0.33.0/mqttwarn/services/gss.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/gss2.py` & `mqttwarn-0.33.0/mqttwarn/services/gss2.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/hangbot.py` & `mqttwarn-0.33.0/mqttwarn/services/hangbot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/hipchat.py` & `mqttwarn-0.33.0/mqttwarn/services/hipchat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/http_urllib.py` & `mqttwarn-0.33.0/mqttwarn/services/http_urllib.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/icinga2.py` & `mqttwarn-0.33.0/mqttwarn/services/icinga2.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/ifttt.py` & `mqttwarn-0.33.0/mqttwarn/services/ifttt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/influxdb.py` & `mqttwarn-0.33.0/mqttwarn/services/influxdb.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/ionic.py` & `mqttwarn-0.33.0/mqttwarn/services/ionic.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/irccat.py` & `mqttwarn-0.33.0/mqttwarn/services/irccat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/linuxnotify.py` & `mqttwarn-0.33.0/mqttwarn/services/linuxnotify.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/log.py` & `mqttwarn-0.33.0/mqttwarn/services/log.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mattermost.py` & `mqttwarn-0.33.0/mqttwarn/services/mattermost.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mqtt.py` & `mqttwarn-0.33.0/mqttwarn/services/mqtt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mqtt_filter.py` & `mqttwarn-0.33.0/mqttwarn/services/mqtt_filter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mqttpub.py` & `mqttwarn-0.33.0/mqttwarn/services/mqttpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mysql.py` & `mqttwarn-0.33.0/mqttwarn/services/mysql.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mysql_dynamic.py` & `mqttwarn-0.33.0/mqttwarn/services/mysql_dynamic.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mysql_remap.py` & `mqttwarn-0.33.0/mqttwarn/services/mysql_remap.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/mythtv.py` & `mqttwarn-0.33.0/mqttwarn/services/mythtv.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/nntp.py` & `mqttwarn-0.33.0/mqttwarn/services/nntp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/nsca.py` & `mqttwarn-0.33.0/mqttwarn/services/nsca.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/osxsay.py` & `mqttwarn-0.33.0/mqttwarn/services/osxsay.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/pastebinpub.py` & `mqttwarn-0.33.0/mqttwarn/services/pastebinpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/pipe.py` & `mqttwarn-0.33.0/mqttwarn/services/pipe.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/postgres.py` & `mqttwarn-0.33.0/mqttwarn/services/postgres.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/prowl.py` & `mqttwarn-0.33.0/mqttwarn/services/prowl.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/pushalot.py` & `mqttwarn-0.33.0/mqttwarn/services/pushalot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/pushbullet.py` & `mqttwarn-0.33.0/mqttwarn/services/pushbullet.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/pushover.py` & `mqttwarn-0.33.0/mqttwarn/services/pushover.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/redispub.py` & `mqttwarn-0.33.0/mqttwarn/services/redispub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/rrdtool.py` & `mqttwarn-0.33.0/mqttwarn/services/rrdtool.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/serial.py` & `mqttwarn-0.33.0/mqttwarn/services/serial.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/slack.py` & `mqttwarn-0.33.0/mqttwarn/services/slack.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/slixmpp.py` & `mqttwarn-0.33.0/mqttwarn/services/slixmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/smtp.py` & `mqttwarn-0.33.0/mqttwarn/services/smtp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/sqlite.py` & `mqttwarn-0.33.0/mqttwarn/services/sqlite.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/sqlite_json2cols.py` & `mqttwarn-0.33.0/mqttwarn/services/sqlite_json2cols.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/sqlite_timestamp.py` & `mqttwarn-0.33.0/mqttwarn/services/sqlite_timestamp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/ssh.py` & `mqttwarn-0.33.0/mqttwarn/services/ssh.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/syslog.py` & `mqttwarn-0.33.0/mqttwarn/services/syslog.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/telegram.py` & `mqttwarn-0.33.0/mqttwarn/services/telegram.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/thingspeak.py` & `mqttwarn-0.33.0/mqttwarn/services/thingspeak.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/tootpaste.py` & `mqttwarn-0.33.0/mqttwarn/services/tootpaste.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/twilio.py` & `mqttwarn-0.33.0/mqttwarn/services/twilio.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/twitter.py` & `mqttwarn-0.33.0/mqttwarn/services/twitter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/websocket.py` & `mqttwarn-0.33.0/mqttwarn/services/websocket.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/xbmc.py` & `mqttwarn-0.33.0/mqttwarn/services/xbmc.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/xively.py` & `mqttwarn-0.33.0/mqttwarn/services/xively.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/xmpp.py` & `mqttwarn-0.33.0/mqttwarn/services/xmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/services/zabbix.py` & `mqttwarn-0.33.0/mqttwarn/services/zabbix.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/util.py` & `mqttwarn-0.33.0/mqttwarn/util.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn/vendor/ZabbixSender.py` & `mqttwarn-0.33.0/mqttwarn/vendor/ZabbixSender.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn.egg-info/PKG-INFO` & `mqttwarn-0.33.0/mqttwarn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttwarn
-Version: 0.32.0
+Version: 0.33.0
 Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
 Home-page: https://github.com/jpmens/mqttwarn
 Author: Jan-Piet Mens, Ben Jones, Andreas Motl
 Author-email: jpmens@gmail.com
 License: EPL 2.0
 Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
 Classifier: Development Status :: 4 - Beta
@@ -343,15 +343,15 @@
 There are also some extensions to mqttwarn not included in the core package.
 Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
 `community contributions to mqttwarn`_.
 
 
 Licenses
 ========
-This software is copyright © 2014-2022 Jan-Piet Mens and contributors. All
+This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
@@ -373,23 +373,14 @@
 Press
 =====
 * The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
 * The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
   as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
 
 
-Notes
-=====
-*mqttwarn* is currently undergoing some refurbishment and will also be
-ported to Python 3 during that phase. You are welcome to participate!
-
-We outlined the tasks for the next releases within the backlog_.
-They might be transferred into GitHub issues progressively, if applicable.
-
-
 Legal stuff
 ===========
 "MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
 
 
 ----
```

### Comparing `mqttwarn-0.32.0/mqttwarn.egg-info/SOURCES.txt` & `mqttwarn-0.33.0/mqttwarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/mqttwarn.egg-info/requires.txt` & `mqttwarn-0.33.0/mqttwarn.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 isort<6
 black<23
 build<1
 mypy<1
 poethepoet<1
 
 [develop:python_version >= "3.7"]
-ruff==0.0.52
+ruff==0.0.254
 
 [dnsupdate]
 dnspython>=1.15.0
 
 [fbchat]
 fbchat>=1.3.6
```

### Comparing `mqttwarn-0.32.0/pyproject.toml` & `mqttwarn-0.33.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.32.0/setup.py` & `mqttwarn-0.33.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 # Packages needed for development and running CI.
 extras["develop"] = [
     "isort<6",
     "black<23",
     "build<1",
     "mypy<1",
     "poethepoet<1",
-    'ruff==0.0.52; python_version>="3.7"',
+    'ruff==0.0.254; python_version>="3.7"',
 ]
 
 
 setup(
     cmdclass=get_cmdclasses(),
     name="mqttwarn",
     description="mqttwarn - subscribe to MQTT topics and notify pluggable services",
```

