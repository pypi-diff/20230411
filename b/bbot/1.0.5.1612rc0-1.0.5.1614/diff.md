# Comparing `tmp/bbot-1.0.5.1612rc0.tar.gz` & `tmp/bbot-1.0.5.1614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1612rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1614.tar", max compression
```

## Comparing `bbot-1.0.5.1612rc0.tar` & `bbot-1.0.5.1614.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/README.md
--rw-r--r--   0        0        0      211 2023-04-11 16:01:56.447020 bbot-1.0.5.1612rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6478 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13323 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3137 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8912 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30113 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     7432 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29289 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4261 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    28177 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9514 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3731 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25113 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     5001 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10060 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5491 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      311 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    15770 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4481 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10777 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    13620 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4012 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0     3844 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     1737 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1787 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1007 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3609 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1606 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8304 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2255 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26114 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3251 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4057 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2591 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    74367 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5859 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4012 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11616 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      479 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-04-11 16:01:56.443020 bbot-1.0.5.1612rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1612rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/LICENSE
+-rw-r--r--   0        0        0    51011 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/README.md
+-rw-r--r--   0        0        0      209 2023-04-11 16:33:47.059975 bbot-1.0.5.1614/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6478 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13323 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3137 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8912 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    30113 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     7432 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29289 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4261 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    28177 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9514 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-04-11 16:33:28.427457 bbot-1.0.5.1614/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25113 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     5001 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/github.py
+-rw-r--r--   0        0        0    10060 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5491 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    15770 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4481 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10777 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13620 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4012 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0     3844 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     1737 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1787 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1007 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3609 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-04-11 16:33:28.431457 bbot-1.0.5.1614/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1606 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8304 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2255 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3251 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4057 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2591 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/helpers.py
+-rw-r--r--   0        0        0    74367 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5859 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4012 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11616 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      479 2023-04-11 16:33:28.435457 bbot-1.0.5.1614/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-04-11 16:33:28.443457 bbot-1.0.5.1614/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-04-11 16:33:28.443457 bbot-1.0.5.1614/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-04-11 16:33:28.443457 bbot-1.0.5.1614/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-04-11 16:33:28.443457 bbot-1.0.5.1614/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1336 2023-04-11 16:33:47.055975 bbot-1.0.5.1614/pyproject.toml
+-rw-r--r--   0        0        0    52286 1970-01-01 00:00:00.000000 bbot-1.0.5.1614/PKG-INFO
```

### Comparing `bbot-1.0.5.1612rc0/LICENSE` & `bbot-1.0.5.1614/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/README.md` & `bbot-1.0.5.1614/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/agent/agent.py` & `bbot-1.0.5.1614/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/cli.py` & `bbot-1.0.5.1614/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1614/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1614/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1614/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1614/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/errors.py` & `bbot-1.0.5.1614/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/event/base.py` & `bbot-1.0.5.1614/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1614/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1614/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1614/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1614/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1614/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1614/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1614/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1614/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1614/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1614/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1614/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1614/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1614/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1614/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1614/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1614/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1614/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1614/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1614/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1614/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1614/bbot/core/helpers/threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1614/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1614/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1614/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1614/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1614/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1614/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/defaults.yml` & `bbot-1.0.5.1614/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1614/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1614/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1614/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/base.py` & `bbot-1.0.5.1614/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1614/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1614/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1614/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1614/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1614/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1614/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1614/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1614/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1614/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/c99.py` & `bbot-1.0.5.1614/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/censys.py` & `bbot-1.0.5.1614/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1614/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1614/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/crt.py` & `bbot-1.0.5.1614/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1614/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1614/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1614/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1614/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1614/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1614/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1614/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1614/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1614/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1614/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1614/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/github.py` & `bbot-1.0.5.1614/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1614/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1614/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1614/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1614/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1614/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1614/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1614/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1614/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1614/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1614/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1614/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1614/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1614/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1614/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1614/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1614/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1614/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/otx.py` & `bbot-1.0.5.1614/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1614/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1614/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1614/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1614/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1614/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1614/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1614/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1614/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1614/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1614/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1614/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1614/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1614/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1614/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1614/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1614/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1614/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1614/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/robots.py` & `bbot-1.0.5.1614/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1614/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1614/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1614/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1614/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1614/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/social.py` & `bbot-1.0.5.1614/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1614/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1614/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1614/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1614/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1614/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1614/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1614/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1614/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1614/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1614/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1614/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1614/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1614/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1614/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1614/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/scanner/target.py` & `bbot-1.0.5.1614/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1614/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/conftest.py` & `bbot-1.0.5.1614/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/helpers.py` & `bbot-1.0.5.1614/bbot/test/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1614/bbot/test/modules_test_classes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1614/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test.conf` & `bbot-1.0.5.1614/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1614/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1614/bbot/test/test_step_1/test_modules_full.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1614/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1614/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1614/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1614/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1614/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1612rc0/pyproject.toml` & `bbot-1.0.5.1614/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1612rc"
+version = "v1.0.5.1614"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1612rc0/PKG-INFO` & `bbot-1.0.5.1614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1612rc0
+Version: 1.0.5.1614
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

