# Comparing `tmp/bbot-1.0.5.1598.tar.gz` & `tmp/bbot-1.0.5.1612rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1598.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1612rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1598.tar` & `bbot-1.0.5.1612rc0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-04-10 18:48:15.374275 bbot-1.0.5.1598/LICENSE
--rw-r--r--   0        0        0    51011 2023-04-10 18:48:15.374275 bbot-1.0.5.1598/README.md
--rw-r--r--   0        0        0      209 2023-04-10 18:48:33.990611 bbot-1.0.5.1598/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6478 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13323 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/__init__.py
--rw-r--r--   0        0        0     3137 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8912 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30167 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     7432 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29187 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4261 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    28177 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9514 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3731 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-04-10 18:48:15.378275 bbot-1.0.5.1598/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25265 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     4614 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/github.py
--rw-r--r--   0        0        0    10060 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5491 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      311 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    15650 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4481 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10777 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/masscan.py
--rw-r--r--   0        0        0    13311 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4012 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-04-10 18:48:15.382275 bbot-1.0.5.1598/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0     3844 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/base.py
--rw-r--r--   0        0        0     1737 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1787 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1007 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3609 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1606 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8304 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2080 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26114 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3251 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4057 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/conftest.py
--rw-r--r--   0        0        0     2591 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/helpers.py
--rw-r--r--   0        0        0    71538 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5669 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4012 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-04-10 18:48:15.386275 bbot-1.0.5.1598/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11466 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      479 2023-04-10 18:48:15.390275 bbot-1.0.5.1598/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-04-10 18:48:15.394275 bbot-1.0.5.1598/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-04-10 18:48:15.394275 bbot-1.0.5.1598/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-04-10 18:48:15.394275 bbot-1.0.5.1598/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-04-10 18:48:15.398275 bbot-1.0.5.1598/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1336 2023-04-10 18:48:33.990611 bbot-1.0.5.1598/pyproject.toml
--rw-r--r--   0        0        0    52286 1970-01-01 00:00:00.000000 bbot-1.0.5.1598/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/LICENSE
+-rw-r--r--   0        0        0    51011 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/README.md
+-rw-r--r--   0        0        0      211 2023-04-11 16:01:56.447020 bbot-1.0.5.1612rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6478 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13323 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3137 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8912 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    30113 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-04-11 16:01:31.022834 bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     7432 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29289 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4261 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    28177 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9514 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25113 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     5001 2023-04-11 16:01:31.026834 bbot-1.0.5.1612rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10060 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5491 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    15770 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4481 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10777 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13620 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4012 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0     3844 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     1737 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1787 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1007 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3609 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1606 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8304 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2255 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-04-11 16:01:31.030834 bbot-1.0.5.1612rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3251 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4057 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2591 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/helpers.py
+-rw-r--r--   0        0        0    74367 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5859 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4012 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11616 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      479 2023-04-11 16:01:31.034834 bbot-1.0.5.1612rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-04-11 16:01:31.042834 bbot-1.0.5.1612rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1338 2023-04-11 16:01:56.443020 bbot-1.0.5.1612rc0/pyproject.toml
+-rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1612rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1598/LICENSE` & `bbot-1.0.5.1612rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/README.md` & `bbot-1.0.5.1612rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/agent/agent.py` & `bbot-1.0.5.1612rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/cli.py` & `bbot-1.0.5.1612rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1612rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/configurator/args.py` & `bbot-1.0.5.1612rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/configurator/environ.py` & `bbot-1.0.5.1612rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/configurator/files.py` & `bbot-1.0.5.1612rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/errors.py` & `bbot-1.0.5.1612rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/event/base.py` & `bbot-1.0.5.1612rc0/bbot/core/event/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,14 +677,16 @@
         return set()
 
 
 class URL_UNVERIFIED(BaseEvent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.web_spider_distance = getattr(self.source, "web_spider_distance", 0)
+        if self.type == "URL_UNVERIFIED":
+            self.web_spider_distance += 1
         self.num_redirects = getattr(self.source, "num_redirects", 0)
 
     def sanitize_data(self, data):
         self.parsed = validators.validate_url_parsed(data)
 
         # tag as dir or endpoint
         if str(self.parsed.path).endswith("/"):
@@ -782,20 +784,17 @@
     def _words(self):
         return extract_words(self.host_stem)
 
 
 class HTTP_RESPONSE(URL_UNVERIFIED, DictEvent):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.web_spider_distance = getattr(self.source, "web_spider_distance", 0)
         self.num_redirects = getattr(self.source, "num_redirects", 0)
         if str(self.data.get("status_code", 0)).startswith("3"):
             self.num_redirects += 1
-        else:
-            self.web_spider_distance += 1
 
     def sanitize_data(self, data):
         url = data.get("url", "")
         self.parsed = validators.validate_url_parsed(url)
 
         header_dict = {}
         for i in data.get("raw_header", "").splitlines():
```

### Comparing `bbot-1.0.5.1598/bbot/core/event/helpers.py` & `bbot-1.0.5.1612rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/cache.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/command.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/diff.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/dns.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/dns.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,25 +166,28 @@
                 break
             except (dns.resolver.NoNameservers, dns.exception.Timeout, dns.resolver.LifetimeTimeout) as e:
                 with self._error_lock:
                     try:
                         self._errors[parent_hash] += 1
                     except KeyError:
                         self._errors[parent_hash] = 1
-                log.verbose(
-                    f'DNS error or timeout for {rdtype} query "{query}" ({self._errors[parent_hash]:,} so far): {e}'
-                )
                 errors.append(e)
                 # don't retry if we get a SERVFAIL
                 if isinstance(e, dns.resolver.NoNameservers):
                     break
                 tries_left -= 1
+                err_msg = (
+                    f'DNS error or timeout for {rdtype} query "{query}" ({self._errors[parent_hash]:,} so far): {e}'
+                )
                 if tries_left > 0:
                     retry_num = (retries + 1) - tries_left
+                    self.debug(err_msg)
                     self.debug(f"Retry (#{retry_num}) resolving {query} with kwargs={kwargs}")
+                else:
+                    log.verbose(err_msg)
 
         self.debug(f"Results for {query} with kwargs={kwargs}: {results}")
         return results, errors
 
     def _resolve_ip(self, query, **kwargs):
         self.debug(f"Reverse-resolving {query} with kwargs={kwargs}")
         retries = kwargs.pop("retries", 0)
```

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/helper.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/logger.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/misc.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/modules.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/url.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/validators.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/web.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1612rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/core/logger/logger.py` & `bbot-1.0.5.1612rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/db/neo4j.py` & `bbot-1.0.5.1612rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/defaults.yml` & `bbot-1.0.5.1612rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/anubisdb.py` & `bbot-1.0.5.1612rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1612rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/badsecrets.py` & `bbot-1.0.5.1612rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/base.py` & `bbot-1.0.5.1612rc0/bbot/modules/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,21 +549,14 @@
     def _is_active(status):
         if status["running"]:
             return True
         total = status["tasks"]["total"] + status["events"]["incoming"] + status["events"]["outgoing"]
         return total > 0
 
     @property
-    def active(self):
-        """
-        Indicates whether the module has data yet to be processed
-        """
-        return self._foo
-
-    @property
     def running(self):
         """
         Indicates whether the module is currently processing data.
         """
         return self._running_counter.value > 0
 
     def request_with_fail_count(self, *args, **kwargs):
```

### Comparing `bbot-1.0.5.1598/bbot/modules/bevigil.py` & `bbot-1.0.5.1612rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/binaryedge.py` & `bbot-1.0.5.1612rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1612rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1612rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1612rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1612rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1612rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/builtwith.py` & `bbot-1.0.5.1612rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/bypass403.py` & `bbot-1.0.5.1612rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/c99.py` & `bbot-1.0.5.1612rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/censys.py` & `bbot-1.0.5.1612rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/certspotter.py` & `bbot-1.0.5.1612rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/crobat.py` & `bbot-1.0.5.1612rc0/bbot/modules/crobat.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,22 @@
         """
         This filter_event is used across many modules
         """
         query = self.make_query(event)
         # reject if already processed
         if self.already_processed(query):
             return False, "Event was already processed"
+        eligible, reason = self.eligible_for_enumeration(event)
+        if eligible:
+            self.processed.add(hash(query))
+            return True, reason
+        return False, reason
+
+    def eligible_for_enumeration(self, event):
+        query = self.make_query(event)
         # check if wildcard
         is_wildcard = self._is_wildcard(query)
         # check if cloud
         is_cloud = False
         if any(t.startswith("cloud-") for t in event.tags):
             is_cloud = True
         # reject if it's a cloud resource and not in our target
@@ -57,16 +65,15 @@
                 return False, "Event has a DNS resolution error"
             if self.reject_wildcards == "strict":
                 if is_wildcard:
                     return False, "Event is a wildcard domain"
             elif self.reject_wildcards == "cloud_only":
                 if is_wildcard and is_cloud:
                     return False, "Event is both a cloud resource and a wildcard domain"
-        self.processed.add(hash(query))
-        return True
+        return True, ""
 
     def already_processed(self, hostname):
         for parent in self.helpers.domain_parents(hostname, include_self=True):
             if hash(parent) in self.processed:
                 return True
         return False
 
@@ -80,15 +87,19 @@
 
     def handle_event(self, event):
         query = self.make_query(event)
         results = self.query(query)
         if results:
             for hostname in set(results):
                 if hostname:
-                    hostname = self.helpers.validators.validate_host(hostname)
+                    try:
+                        hostname = self.helpers.validators.validate_host(hostname)
+                    except ValueError as e:
+                        self.verbose(e)
+                        continue
                     if hostname and hostname.endswith(f".{query}") and not hostname == event.data:
                         self.emit_event(hostname, "DNS_NAME", event, abort_if=self.abort_if)
 
     def request_url(self, query):
         url = f"{self.base_url}/subdomains/{self.helpers.quote(query)}"
         return self.request_with_fail_count(url)
```

### Comparing `bbot-1.0.5.1598/bbot/modules/crt.py` & `bbot-1.0.5.1612rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1612rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1612rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1612rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1612rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1612rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1612rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/emailformat.py` & `bbot-1.0.5.1612rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1612rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1612rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/fullhunt.py` & `bbot-1.0.5.1612rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1612rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/github.py` & `bbot-1.0.5.1612rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/gowitness.py` & `bbot-1.0.5.1612rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/hackertarget.py` & `bbot-1.0.5.1612rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/host_header.py` & `bbot-1.0.5.1612rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/httpx.py` & `bbot-1.0.5.1612rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/hunt.py` & `bbot-1.0.5.1612rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/hunterio.py` & `bbot-1.0.5.1612rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1612rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/internal/base.py` & `bbot-1.0.5.1612rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1612rc0/bbot/modules/internal/excavate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import html
 import base64
 import jwt as j
-from urllib.parse import urlparse, urljoin
+from urllib.parse import urljoin
 
 from bbot.core.helpers.regexes import _email_regex
 from bbot.modules.internal.base import BaseInternalModule
 
 
 class BaseExtractor:
     # If using capture groups, be sure to name them beginning with "capture".
@@ -86,34 +86,36 @@
         for name, regex in self.compiled_regexes.items():
             for result in regex.findall(content):
                 if name == "fullurl":
                     protocol, other = result
                     result = f"{protocol}://{other}"
 
                 elif name in ("a-tag", "script-tag") and parsed:
-                    path = html.unescape(result[1]).lstrip("/")
+                    path = html.unescape(result[1])
 
                     for p in self.prefix_blacklist:
                         if path.lower().startswith(p.lower()):
                             self.excavate.debug(
                                 f"omitted result from a-tag parser because of blacklisted prefix [{p}]"
                             )
                             continue
 
                     if not self.compiled_regexes["fullurl"].match(path):
-                        path = f"{'/'.join(event.parsed.path.split('/')[0:-1])}/{path}"
-                        full_url = f"{event.parsed.scheme}://{event.parsed.netloc}{path}"
-                        result = urljoin(full_url, urlparse(full_url).path)
+                        source_url = event.parsed.geturl()
+                        result = urljoin(source_url, path)
+                        # this is necessary to weed out mailto: and such
+                        if not self.compiled_regexes["fullurl"].match(result):
+                            continue
                     else:
                         result = path
 
                 yield result, name
 
     def report(self, result, name, event, **kwargs):
-        spider_danger = kwargs.get("spider_danger", True)
+        consider_spider_danger = kwargs.get("consider_spider_danger", True)
         exceeded_max_links = kwargs.get("exceeded_max_links", False)
 
         tags = []
 
         parsed_uri = self.excavate.helpers.urlparse(result)
         host, port = self.excavate.helpers.split_host_port(parsed_uri.netloc)
         # Handle non-HTTP URIs (ftp, s3, etc.)
@@ -130,15 +132,16 @@
             self.excavate.emit_event(
                 {"protocol": parsed_uri.scheme, "host": str(host)},
                 "PROTOCOL",
                 source=event,
             )
             return
 
-        if exceeded_max_links or (spider_danger and self.excavate.is_spider_danger(event, result)):
+        is_spider_danger = self.excavate.is_spider_danger(event, result)
+        if exceeded_max_links or (consider_spider_danger and is_spider_danger):
             tags.append("spider-danger")
 
         self.excavate.debug(f"Found URL [{result}] from parsing [{event.data.get('url')}] with regex [{name}]")
         self.excavate.emit_event(result, "URL_UNVERIFIED", source=event, tags=tags)
 
 
 class EmailExtractor(BaseExtractor):
@@ -344,23 +347,23 @@
                     self.error_extractor,
                     self.jwt,
                     self.javascript,
                     self.serialization,
                     self.functionality,
                 ],
                 event,
-                spider_danger=True,
+                consider_spider_danger=True,
             )
 
             headers = self.helpers.recursive_decode(event.data.get("raw_header", ""))
             self.search(
                 headers,
                 [self.hostname, self.url, self.email, self.error_extractor, self.jwt, self.serialization],
                 event,
-                spider_danger=False,
+                consider_spider_danger=False,
             )
 
         else:
             self.search(
                 str(data),
                 [self.hostname, self.url, self.email, self.error_extractor, self.jwt, self.serialization],
                 event,
```

### Comparing `bbot-1.0.5.1598/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1612rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1612rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/ipstack.py` & `bbot-1.0.5.1612rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/leakix.py` & `bbot-1.0.5.1612rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/masscan.py` & `bbot-1.0.5.1612rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/massdns.py` & `bbot-1.0.5.1612rc0/bbot/modules/massdns.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,25 @@
             nameservers_url,
             cache_hrs=24 * 7,
         )
         self.devops_mutations = list(self.helpers.word_cloud.devops_mutations)
         return super().setup()
 
     def filter_event(self, event):
-        self.add_found(event)
-        return super().filter_event(event)
+        query = self.make_query(event)
+        eligible, reason = self.eligible_for_enumeration(event)
+        if eligible:
+            self.add_found(event)
+        # reject if already processed
+        if self.already_processed(query):
+            return False, f'Query "{query}" was already processed'
+        if eligible:
+            self.processed.add(hash(query))
+            return True, reason
+        return False, reason
 
     def handle_event(self, event):
         query = self.make_query(event)
         h = hash(query)
         if not h in self.source_events:
             self.source_events[h] = event
 
@@ -193,16 +202,16 @@
                 j = json.loads(line)
             except json.decoder.JSONDecodeError:
                 self.debug(f"Failed to decode line: {line}")
                 continue
             answers = j.get("data", {}).get("answers", [])
             if type(answers) == list and len(answers) > 0:
                 answer = answers[0]
-                hostname = answer.get("name", "")
-                if hostname:
+                hostname = answer.get("name", "").strip(".").lower()
+                if hostname.endswith(f".{domain}"):
                     data = answer.get("data", "")
                     rdtype = answer.get("type", "").upper()
                     # avoid garbage answers like this:
                     # 8AAAA queries have been locally blocked by dnscrypt-proxy/Set block_ipv6 to false to disable this feature
                     if data and rdtype and not " " in data:
                         # skip wildcards
                         if rdtype in domain_wildcard_rdtypes:
@@ -213,15 +222,14 @@
                                     f"Skipping {hostname}:{rdtype} because it may be a wildcard (reason: performance)"
                                 )
                                 continue
                             wildcard_rdtypes = self.helpers.is_wildcard(hostname, ips=(data,))
                             if rdtype in wildcard_rdtypes:
                                 self.debug(f"Skipping {hostname}:{rdtype} because it's a wildcard")
                                 continue
-                        hostname = hostname.rstrip(".").lower()
                         hostname_hash = hash(hostname)
                         if hostname_hash not in hosts_yielded:
                             hosts_yielded.add(hostname_hash)
                             yield hostname
 
     def finish(self):
         found = sorted(self.found.items(), key=lambda x: len(x[-1]), reverse=True)
@@ -289,16 +297,16 @@
 
                 if mutations:
                     self.info(f"Trying {len(mutations):,} mutations against {domain} ({i+1}/{len(found)})")
                     results = list(self.massdns(query, mutations))
                     for hostname in results:
                         source_event = self.get_source_event(hostname)
                         if source_event is None:
-                            self.verbose(f"Could not correlate source event from: {hostname}")
-                            source_event = self.scan.root_event
+                            self.warning(f"Could not correlate source event from: {hostname}")
+                            continue
                         self.emit_result(hostname, source_event, query)
                     if results:
                         continue
                 break
 
     def add_found(self, host):
         if not isinstance(host, str):
```

### Comparing `bbot-1.0.5.1598/bbot/modules/naabu.py` & `bbot-1.0.5.1612rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/ntlm.py` & `bbot-1.0.5.1612rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/otx.py` & `bbot-1.0.5.1612rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/base.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/csv.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/http.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/human.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/json.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/web_report.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/output/websocket.py` & `bbot-1.0.5.1612rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1612rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1612rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1612rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/passivetotal.py` & `bbot-1.0.5.1612rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/pgp.py` & `bbot-1.0.5.1612rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/rapiddns.py` & `bbot-1.0.5.1612rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1612rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/report/asn.py` & `bbot-1.0.5.1612rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/riddler.py` & `bbot-1.0.5.1612rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/robots.py` & `bbot-1.0.5.1612rc0/bbot/modules/robots.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,8 +49,11 @@
                             )
 
                         elif split_l[0].lower() == "sitemap" and self.config.get("include_sitemap") == True:
                             unverified_url = split_l[1]
                         else:
                             continue
 
-                        self.emit_event(unverified_url, "URL_UNVERIFIED", source=event)
+                        tags = []
+                        if self.is_spider_danger(event, unverified_url):
+                            tags.append("spider-danger")
+                        self.emit_event(unverified_url, "URL_UNVERIFIED", source=event, tags=tags)
```

### Comparing `bbot-1.0.5.1598/bbot/modules/secretsdb.py` & `bbot-1.0.5.1612rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/securitytrails.py` & `bbot-1.0.5.1612rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1612rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/skymem.py` & `bbot-1.0.5.1612rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/smuggler.py` & `bbot-1.0.5.1612rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/social.py` & `bbot-1.0.5.1612rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/sslcert.py` & `bbot-1.0.5.1612rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1612rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/telerik.py` & `bbot-1.0.5.1612rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/threatminer.py` & `bbot-1.0.5.1612rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1612rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/urlscan.py` & `bbot-1.0.5.1612rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/viewdns.py` & `bbot-1.0.5.1612rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/virustotal.py` & `bbot-1.0.5.1612rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/wafw00f.py` & `bbot-1.0.5.1612rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1612rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/wayback.py` & `bbot-1.0.5.1612rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/modules/zoomeye.py` & `bbot-1.0.5.1612rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/scanner/manager.py` & `bbot-1.0.5.1612rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/scanner/scanner.py` & `bbot-1.0.5.1612rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/scanner/stats.py` & `bbot-1.0.5.1612rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/scanner/target.py` & `bbot-1.0.5.1612rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1612rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/conftest.py` & `bbot-1.0.5.1612rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/helpers.py` & `bbot-1.0.5.1612rc0/bbot/test/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1612rc0/bbot/test/modules_test_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,19 @@
         expect_args = {"method": "GET", "uri": "/"}
         respond_args = {"response_data": response_data}
         self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
         # verify relatives path a-tag parsing is working correctly
 
         expect_args = {"method": "GET", "uri": "/subdir/links.html"}
-        respond_args = {"response_data": "<a href='../relative.html'>relative</a>"}
+        respond_args = {"response_data": "<a href='../relative.html'/><a href='/2/depth2.html'/>"}
         self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
         expect_args = {"method": "GET", "uri": "/relative.html"}
-        respond_args = {"response_data": "alive"}
+        respond_args = {"response_data": "<a href='/distance2.html'/>"}
         self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
     def check_events(self, events):
         event_data = [e.data for e in events]
         assert "https://www1.test.notreal/" in event_data
         assert "https://www2.test.notreal/" in event_data
         assert "https://www3.test.notreal/" in event_data
@@ -136,17 +136,86 @@
 
         assert any(
             e.type == "URL_UNVERIFIED"
             and e.data == "http://127.0.0.1:8888/relative.html"
             and "spider-danger" not in e.tags
             for e in events
         )
+
+        assert any(
+            e.type == "URL_UNVERIFIED"
+            and e.data == "http://127.0.0.1:8888/2/depth2.html"
+            and "spider-danger" in e.tags
+            for e in events
+        )
+
+        assert any(
+            e.type == "URL_UNVERIFIED"
+            and e.data == "http://127.0.0.1:8888/distance2.html"
+            and "spider-danger" in e.tags
+            for e in events
+        )
         return True
 
 
+class Excavate_relativelinks(HttpxMockHelper):
+    additional_modules = ["httpx"]
+    targets = ["http://127.0.0.1:8888/", "test.notreal", "http://127.0.0.1:8888/subdir/"]
+    config_overrides = {"web_spider_distance": 1, "web_spider_depth": 1}
+
+    def setup(self):
+        self.bbot_httpserver.no_handler_status_code = 404
+
+    def mock_args(self):
+        # root relative
+        expect_args = {"method": "GET", "uri": "/rootrelative.html"}
+        respond_args = {"response_data": "alive"}
+        self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+        # page relative
+        expect_args = {"method": "GET", "uri": "/subdir/pagerelative.html"}
+        respond_args = {"response_data": "alive"}
+        self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+        expect_args = {"method": "GET", "uri": "/subdir/"}
+        respond_args = {
+            "response_data": "<a href='/rootrelative.html'>root relative</a><a href='pagerelative.html'>page relative</a>"
+        }
+        self.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+    def check_events(self, events):
+        root_relative_detection = False
+        page_relative_detection = False
+        root_page_confusion_1 = False
+        root_page_confusion_2 = False
+
+        for e in events:
+            if e.type == "URL_UNVERIFIED":
+                # these cases represent the desired behavior for parsing relative links
+                if e.data == "http://127.0.0.1:8888/rootrelative.html":
+                    root_relative_detection = True
+                if e.data == "http://127.0.0.1:8888/subdir/pagerelative.html":
+                    page_relative_detection = True
+
+                # these cases indicates that excavate parsed the relative links incorrectly
+                if e.data == "http://127.0.0.1:8888/pagerelative.html":
+                    root_page_confusion_1 = True
+                if e.data == "http://127.0.0.1:8888/subdir/rootrelative.html":
+                    root_page_confusion_2 = True
+
+        if (
+            root_relative_detection
+            and page_relative_detection
+            and not root_page_confusion_1
+            and not root_page_confusion_2
+        ):
+            return True
+        return False
+
+
 class Subdomain_Hijack(HttpxMockHelper):
     additional_modules = ["httpx", "excavate"]
 
     def mock_args(self):
         fingerprints = self.module.fingerprints
         assert fingerprints, "No subdomain hijacking fingerprints available"
         fingerprint = next(iter(fingerprints))
@@ -623,14 +692,15 @@
         allow_bool = False
         disallow_bool = False
         sitemap_bool = False
         wildcard_bool = False
 
         for e in events:
             if e.type == "URL_UNVERIFIED":
+                assert "spider-danger" in e.tags, f"{e} doesn't have spider-danger tag"
                 if e.data == "http://127.0.0.1:8888/allow/":
                     allow_bool = True
 
                 if e.data == "http://127.0.0.1:8888/disallow/":
                     disallow_bool = True
 
                 if e.data == "http://127.0.0.1:8888/sitemap.txt":
```

### Comparing `bbot-1.0.5.1598/bbot/test/run_tests.sh` & `bbot-1.0.5.1612rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test.conf` & `bbot-1.0.5.1612rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_1/test_modules_full.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 
 def test_excavate(bbot_config, bbot_scanner, bbot_httpserver):
     x = Excavate(bbot_config, bbot_scanner, bbot_httpserver)
     x.run()
 
 
+def test_excavate_relativelinks(bbot_config, bbot_scanner, bbot_httpserver):
+    x = Excavate_relativelinks(bbot_config, bbot_scanner, bbot_httpserver, module_name="excavate")
+    x.run()
+
+
 def test_subdomain_hijack(bbot_config, bbot_scanner, bbot_httpserver):
     x = Subdomain_Hijack(bbot_config, bbot_scanner, bbot_httpserver)
     x.run()
 
 
 def test_fingerprintx(bbot_config, bbot_scanner, bbot_httpserver):
     x = Fingerprintx(bbot_config, bbot_scanner, bbot_httpserver)
```

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_modules_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import requests_mock
+from contextlib import suppress
 
 from ..bbot_fixtures import *
 
 
 def test_modules_basic(patch_commands, patch_ansible, scan, helpers, events, bbot_config, bbot_scanner):
     fallback_nameservers = scan.helpers.temp_dir / "nameservers.txt"
     with open(fallback_nameservers, "w") as f:
@@ -228,11 +229,14 @@
         for future in helpers.as_completed(futures):
             assert future.result() == None
         futures.clear()
 
         # event filters
         for module_name, module in scan2.modules.items():
             log.info(f"Testing {module_name}.filter_event()")
-            assert module.filter_event(events.emoji) in (
+            result = module.filter_event(events.emoji)
+            with suppress(ValueError, TypeError):
+                result, reason = result
+            assert result in (
                 True,
                 False,
             ), f"{module_name}.filter_event() must return either True or False"
```

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1612rc0/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1612rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1612rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1612rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1612rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1598/pyproject.toml` & `bbot-1.0.5.1612rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1598"
+version = "v1.0.5.1612rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1598/PKG-INFO` & `bbot-1.0.5.1612rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1598
+Version: 1.0.5.1612rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

