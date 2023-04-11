# Comparing `tmp/thetagang-1.4.0.tar.gz` & `tmp/thetagang-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.4.0.tar", max compression
+gzip compressed data, was "thetagang-1.5.0.tar", max compression
```

## Comparing `thetagang-1.4.0.tar` & `thetagang-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    34523 2023-02-17 16:36:52.844223 thetagang-1.4.0/LICENSE
--rw-r--r--   0        0        0    14673 2023-02-17 16:36:52.844223 thetagang-1.4.0/README.md
--rw-r--r--   0        0        0     1628 2023-02-17 16:36:52.844223 thetagang-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/__init__.py
--rw-r--r--   0        0        0     7474 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/config.py
--rw-r--r--   0        0        0      642 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/entry.py
--rw-r--r--   0        0        0     1022 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/main.py
--rw-r--r--   0        0        0      376 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/options.py
--rw-r--r--   0        0        0    45852 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/test_util.py
--rwxr-xr-x   0        0        0     7287 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/thetagang.py
--rw-r--r--   0        0        0     4834 2023-02-17 16:36:52.848223 thetagang-1.4.0/thetagang/util.py
--rw-r--r--   0        0        0    15942 1970-01-01 00:00:00.000000 thetagang-1.4.0/setup.py
--rw-r--r--   0        0        0    15937 1970-01-01 00:00:00.000000 thetagang-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-11 11:55:13.557196 thetagang-1.5.0/LICENSE
+-rw-r--r--   0        0        0    14673 2023-04-11 11:55:13.557196 thetagang-1.5.0/README.md
+-rw-r--r--   0        0        0     1618 2023-04-11 11:55:13.557196 thetagang-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/__init__.py
+-rw-r--r--   0        0        0     7734 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/config.py
+-rw-r--r--   0        0        0      642 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/entry.py
+-rw-r--r--   0        0        0     1022 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/main.py
+-rw-r--r--   0        0        0      376 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/options.py
+-rw-r--r--   0        0        0    47953 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     7753 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5323 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/util.py
+-rw-r--r--   0        0        0    15937 1970-01-01 00:00:00.000000 thetagang-1.5.0/PKG-INFO
```

### Comparing `thetagang-1.4.0/LICENSE` & `thetagang-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/README.md` & `thetagang-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/pyproject.toml` & `thetagang-1.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.4.0"
+version = "1.5.0"
 
 [tool.poetry.dependencies]
-click = ">=7.1.2,<9.0.0"
-click-log = ">=0.3.2,<0.5.0"
-colorama = "^0.4.4"
-ib_insync = "^0.9.66"
+click = "^8.1.3"
+click-log = "^0.4.0"
+colorama = "^0.4.6"
+ib_insync = "^0.9.81"
 python = ">=3.8,<4.0"
 python-dateutil = "^2.8.1"
 pytimeparse = "^1.1.8"
 schema = "^0.7.3"
 toml = "^0.10.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 autoflake = "^2.0"
 autohooks = "^23.1.0"
 autohooks-plugin-black = "^22.11.0"
 autohooks-plugin-isort = "^22.8.0"
 autohooks-plugin-pylint = "^22.8.1"
 black = "^23.1.0"
 isort = "^5.12.0"
-pylint = "^2.16.1"
+pylint = "^2.16.2"
 pytest = "^7.2.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/brndnmtthws/thetagang/issues"
 "GitHub" = "https://github.com/brndnmtthws/thetagang"
 
 [tool.poetry.scripts]
```

### Comparing `thetagang-1.4.0/thetagang/config.py` & `thetagang-1.5.0/thetagang/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,20 +132,23 @@
                 object: {
                     Or("weight", "parts", only_one=True): And(
                         Or(float, int),
                         lambda n: 0 <= n <= 1 if isinstance(n, float) else n > 0,
                     ),
                     Optional("primary_exchange"): And(str, len),
                     Optional("delta"): And(float, lambda n: 0 <= n <= 1),
+                    Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                     Optional("calls"): {
                         Optional("delta"): And(float, lambda n: 0 <= n <= 1),
+                        Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                     },
                     Optional("puts"): {
                         Optional("delta"): And(float, lambda n: 0 <= n <= 1),
+                        Optional("write_threshold"): And(float, lambda n: 0 <= n <= 1),
                         Optional("strike_limit"): And(float, lambda n: n > 0),
                     },
                 }
             },
             Optional("ib_insync"): {Optional("logfile"): And(str, len)},
             "ibc": {
                 Optional("password"): And(str, len),
```

### Comparing `thetagang-1.4.0/thetagang/config_defaults.py` & `thetagang-1.5.0/thetagang/config_defaults.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/thetagang/dict_merge.py` & `thetagang-1.5.0/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/thetagang/main.py` & `thetagang-1.5.0/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/thetagang/portfolio_manager.py` & `thetagang-1.5.0/thetagang/portfolio_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     account_summary_to_dict,
     count_short_option_positions,
     get_call_cap,
     get_highest_price,
     get_lowest_price,
     get_strike_limit,
     get_target_delta,
+    get_write_threshold,
     midpoint_or_market_price,
     portfolio_positions_to_dict,
     position_pnl,
     wait_n_seconds,
 )
 
 from .options import option_dte
@@ -622,18 +623,42 @@
             write_only_when_green = self.config["write_when"]["calls"]["green"]
             ticker = (
                 self.get_ticker_for_stock(symbol, self.get_primary_exchange(symbol))
                 if write_only_when_green
                 else None
             )
 
-            ok_to_write = (
-                not write_only_when_green
-                or ticker
-                and ticker.marketPrice() > ticker.close
+            def is_ok_to_write_calls(
+                config, symbol, ticker, write_only_when_green, calls_to_write
+            ):
+                if not write_only_when_green:
+                    return True
+                if not ticker or calls_to_write <= 0:
+                    return False
+                write_threshold = get_write_threshold(config, symbol, "C")
+                absolute_daily_change = math.fabs(
+                    (ticker.marketPrice() - ticker.close) / ticker.close
+                )
+                green = ticker.marketPrice() > ticker.close
+                if not green:
+                    click.secho(
+                        f"Need to write {calls_to_write} calls for {symbol}, but skipping because underlying is not green",
+                        fg="green",
+                    )
+                    return False
+                if absolute_daily_change < write_threshold:
+                    click.secho(
+                        f"Need to write {calls_to_write} calls for {symbol}, but skipping because daily_change={absolute_daily_change:.3f} less than write_threshold={write_threshold:.3f}",
+                        fg="green",
+                    )
+                    return False
+                return True
+
+            ok_to_write = is_ok_to_write_calls(
+                self.config, symbol, ticker, write_only_when_green, calls_to_write
             )
 
             if calls_to_write > 0 and ok_to_write:
                 click.secho(
                     f"Will write {calls_to_write} calls, {new_contracts_needed} needed for {symbol}, capped at {maximum_new_contracts}, at or above strike ${strike_limit} (target_calls={target_calls}, call_count={call_count})",
                     fg="green",
                 )
@@ -647,19 +672,14 @@
                 except RuntimeError as error:
                     click.echo()
                     click.secho(str(error), fg="red")
                     click.secho(
                         f"Failed to write calls for {symbol}. Continuing anyway...",
                         fg="yellow",
                     )
-            elif calls_to_write > 0:
-                click.secho(
-                    f"Need to write {calls_to_write} calls for {symbol}, but skipping because underlying is red",
-                    fg="green",
-                )
 
     def write_calls(self, symbol, primary_exchange, quantity, strike_limit):
         sell_ticker = self.find_eligible_contracts(
             symbol, primary_exchange, "C", strike_limit
         )
 
         if not self.wait_for_midpoint_price(sell_ticker):
@@ -791,35 +811,66 @@
             click.secho(f"    Target share quantity: {target_quantity:,d}", fg="cyan")
 
             # Current number of short puts
             put_count = count_short_option_positions(symbol, portfolio_positions, "P")
 
             write_only_when_red = self.config["write_when"]["puts"]["red"]
 
-            ok_to_write = not write_only_when_red or ticker.marketPrice() < ticker.close
-
-            target_additional_quantity[symbol] = {
-                "qty": math.floor(target_quantity - current_position - 100 * put_count),
-                "ok_to_write": ok_to_write,
-            }
-
-            net_target_shares = target_additional_quantity[symbol]["qty"]
+            qty_to_write = math.floor(
+                target_quantity - current_position - 100 * put_count
+            )
+            net_target_shares = qty_to_write
             net_target_puts = net_target_shares // 100
 
             click.secho(
                 f"    Net quantity: {net_target_shares:,d} shares, {net_target_puts} contracts",
                 fg="cyan",
             )
 
+            def is_ok_to_write_puts(
+                config, symbol, ticker, write_only_when_red, puts_to_write
+            ):
+                if not write_only_when_red:
+                    return True
+                if puts_to_write <= 0:
+                    return False
+                write_threshold = get_write_threshold(config, symbol, "P")
+                absolute_daily_change = math.fabs(
+                    (ticker.marketPrice() - ticker.close) / ticker.close
+                )
+                red = ticker.marketPrice() < ticker.close
+                if not red:
+                    click.secho(
+                        f"Need to write {puts_to_write} puts for {symbol}, but skipping because underlying is not red",
+                        fg="green",
+                    )
+                    return False
+                if absolute_daily_change < write_threshold:
+                    click.secho(
+                        f"Need to write {puts_to_write} puts for {symbol}, but skipping because daily_change={absolute_daily_change:.3f} less than write_threshold={write_threshold:.3f}",
+                        fg="green",
+                    )
+                    return False
+                return True
+
+            ok_to_write = is_ok_to_write_puts(
+                self.config, symbol, ticker, write_only_when_red, net_target_puts
+            )
+
+            target_additional_quantity[symbol] = {
+                "qty": net_target_puts,
+                "ok_to_write": ok_to_write,
+            }
+
         click.echo()
 
         # Figure out how many additional puts are needed, if they're needed
         for symbol, target in target_additional_quantity.items():
             ok_to_write = target["ok_to_write"]
-            additional_quantity = target["qty"] // 100
+            additional_quantity = target["qty"]
             # NOTE: it's possible there are non-standard option contract sizes,
             # like with futures, but we don't bother handling those cases.
             # Please don't use this code with futures.
             if additional_quantity >= 1 and ok_to_write:
                 maximum_new_contracts = self.get_maximum_new_contracts_for(
                     symbol,
                     self.get_primary_exchange(symbol),
@@ -840,19 +891,14 @@
                         )
                     self.write_puts(
                         symbol,
                         self.get_primary_exchange(symbol),
                         puts_to_write,
                         strike_limit,
                     )
-            elif additional_quantity >= 1:
-                click.secho(
-                    f"Need {additional_quantity} additional for {symbol}, but won't write because {symbol} is green",
-                    fg="cyan",
-                )
             elif additional_quantity < 0:
                 excess_puts = -additional_quantity
                 self.has_excess_puts.add(symbol)
                 click.secho(
                     f"Warning: {symbol} has excess_puts={excess_puts} based on net liquidation and target margin usage",
                     fg="yellow",
                 )
```

### Comparing `thetagang-1.4.0/thetagang/test_util.py` & `thetagang-1.5.0/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.4.0/thetagang/thetagang.py` & `thetagang-1.5.0/thetagang/thetagang.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 
 import click
 from ib_insync import IB, IBC, Watchdog, util
 from ib_insync.contract import Contract
 
 from thetagang.config import normalize_config, validate_config
-from thetagang.util import get_strike_limit, get_target_delta
+from thetagang.util import get_strike_limit, get_target_delta, get_write_threshold
 
 from .portfolio_manager import PortfolioManager
 
 util.patchAsyncio()
 
 
 def start(config, without_ibc=False):
@@ -82,15 +82,15 @@
         )
 
     click.secho(
         f"    Puts: credit only        = {config['roll_when']['puts']['credit_only']}",
         fg="cyan",
     )
     click.secho(
-        f"    Puts: roll excess       = {config['roll_when']['puts']['has_excess']}",
+        f"    Puts: roll excess        = {config['roll_when']['puts']['has_excess']}",
         fg="cyan",
     )
     click.secho(
         f"    Calls: credit only       = {config['roll_when']['calls']['credit_only']}",
         fg="cyan",
     )
     click.secho(
@@ -151,24 +151,33 @@
 
     click.echo()
     click.secho("  Symbols:", fg="green")
     for s in config["symbols"].keys():
         c = config["symbols"][s]
         c_delta = f"{get_target_delta(config, s, 'C'):.2f}".rjust(4)
         p_delta = f"{get_target_delta(config, s, 'P'):.2f}".rjust(4)
-        weight_p = f"{(c['weight'] * 100):.2f}".rjust(4)
+        weight_p = f"{(c['weight'] * 100):.2f}".rjust(5)
         strike_limits = ""
         c_limit = get_strike_limit(config, s, "C")
         p_limit = get_strike_limit(config, s, "P")
         if c_limit:
-            strike_limits += f", call strike >= ${c_limit:.2f}"
+            strike_limits += f", calls>=${c_limit:.2f}"
         if p_limit:
-            strike_limits += f", put strike <= ${p_limit:.2f}"
+            strike_limits += f", puts<=${p_limit:.2f}"
+        thresholds = ""
+        only_red = config["write_when"]["puts"]["red"]
+        only_green = config["write_when"]["puts"]["red"]
+        c_thresh = get_write_threshold(config, s, "C")
+        p_thresh = get_write_threshold(config, s, "P")
+        if only_green and c_thresh:
+            thresholds += f", threshold(green)>={100*c_thresh:.2f}%"
+        if only_red and p_thresh:
+            thresholds += f", threshold(red)<={100*p_thresh:.2f}%"
         click.secho(
-            f"    {s.rjust(5)} weight = {weight_p}%, delta = {p_delta}p, {c_delta}c{strike_limits}",
+            f"    {s.rjust(5)} weight={weight_p}%, delta={p_delta}p, {c_delta}c{strike_limits}{thresholds}",
             fg="cyan",
         )
     assert (
         round(
             sum([config["symbols"][s]["weight"] for s in config["symbols"].keys()]), 5
         )
         == 1.00000
```

### Comparing `thetagang-1.4.0/thetagang/util.py` & `thetagang-1.5.0/thetagang/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     if symbol in portfolio_positions:
         return math.floor(
             -sum(
                 [
                     p.position
                     for p in portfolio_positions[symbol]
                     if isinstance(p.contract, Option)
-                    and p.contract.right.startswith(right)
+                    and p.contract.right.upper().startswith(right.upper())
                     and p.position < 0
                 ]
             )
         )
 
     return 0
 
@@ -54,15 +54,15 @@
     if symbol in portfolio_positions:
         return math.floor(
             sum(
                 [
                     p.position
                     for p in portfolio_positions[symbol]
                     if isinstance(p.contract, Option)
-                    and p.contract.right.startswith(right)
+                    and p.contract.right.upper().startswith(right.upper())
                     and p.position > 0
                 ]
             )
         )
 
     return 0
 
@@ -111,29 +111,29 @@
         else:
             return ticker.marketPrice()
 
     return ticker.midpoint()
 
 
 def get_target_delta(config, symbol, right):
-    p_or_c = "calls" if right.startswith("C") else "puts"
+    p_or_c = "calls" if right.upper().startswith("C") else "puts"
     if (
         p_or_c in config["symbols"][symbol]
         and "delta" in config["symbols"][symbol][p_or_c]
     ):
         return config["symbols"][symbol][p_or_c]["delta"]
     if "delta" in config["symbols"][symbol]:
         return config["symbols"][symbol]["delta"]
     if p_or_c in config["target"]:
         return config["target"][p_or_c]["delta"]
     return config["target"]["delta"]
 
 
 def get_strike_limit(config, symbol, right):
-    p_or_c = "calls" if right.startswith("C") else "puts"
+    p_or_c = "calls" if right.upper().startswith("C") else "puts"
     if (
         p_or_c in config["symbols"][symbol]
         and "strike_limit" in config["symbols"][symbol][p_or_c]
     ):
         return config["symbols"][symbol][p_or_c]["strike_limit"]
     return None
 
@@ -142,7 +142,19 @@
     if (
         "write_when" in config
         and "calls" in config["write_when"]
         and "cap_factor" in config["write_when"]["calls"]
     ):
         return max([0, min([1.0, config["write_when"]["calls"]["cap_factor"]])])
     return 1.0
+
+
+def get_write_threshold(config, symbol, right):
+    p_or_c = "calls" if right.upper().startswith("C") else "puts"
+    if (
+        p_or_c in config["symbols"][symbol]
+        and "write_threshold" in config["symbols"][symbol][p_or_c]
+    ):
+        return config["symbols"][symbol][p_or_c]["write_threshold"]
+    if "write_threshold" in config["symbols"][symbol]:
+        return config["symbols"][symbol]["write_threshold"]
+    return 0.0
```

### Comparing `thetagang-1.4.0/setup.py` & `thetagang-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,289 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: thetagang
+Version: 1.5.0
+Summary: ThetaGang is an IBKR bot for getting money
+Home-page: https://github.com/brndnmtthws/thetagang
+License: AGPL-3.0-only
+Author: Brenden Matthews
+Author-email: brenden@brndn.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click-log (>=0.4.0,<0.5.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: ib_insync (>=0.9.81,<0.10.0)
+Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
+Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
+Requires-Dist: schema (>=0.7.3,<0.8.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Bug Tracker, https://github.com/brndnmtthws/thetagang/issues
+Project-URL: Documentation, https://github.com/brndnmtthws/thetagang/blob/master/README.md
+Project-URL: GitHub, https://github.com/brndnmtthws/thetagang
+Project-URL: Repository, https://github.com/brndnmtthws/thetagang.git
+Description-Content-Type: text/markdown
 
-packages = \
-['thetagang']
+[![Docker publish](https://github.com/brndnmtthws/thetagang/workflows/Docker%20publish/badge.svg)](https://hub.docker.com/r/brndnmtthws/thetagang) [![Python Publish](https://github.com/brndnmtthws/thetagang/workflows/Python%20Publish/badge.svg)](https://pypi.org/project/thetagang/) [![Docker Pulls](https://img.shields.io/docker/pulls/brndnmtthws/thetagang)](https://hub.docker.com/r/brndnmtthws/thetagang) [![PyPI download month](https://img.shields.io/pypi/dm/thetagang?label=PyPI%20downloads)](https://pypi.python.org/pypi/thetagang/)
 
-package_data = \
-{'': ['*']}
+[💬 Join the Matrix chat, we can get money together](https://matrix.to/#/#thetagang:frens.io).
 
-install_requires = \
-['click-log>=0.3.2,<0.5.0',
- 'click>=7.1.2,<9.0.0',
- 'colorama>=0.4.4,<0.5.0',
- 'ib_insync>=0.9.66,<0.10.0',
- 'python-dateutil>=2.8.1,<3.0.0',
- 'pytimeparse>=1.1.8,<2.0.0',
- 'schema>=0.7.3,<0.8.0',
- 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['thetagang = thetagang.entry:cli']}
-
-setup_kwargs = {
-    'name': 'thetagang',
-    'version': '1.4.0',
-    'description': 'ThetaGang is an IBKR bot for getting money',
-    'long_description': '[![Docker publish](https://github.com/brndnmtthws/thetagang/workflows/Docker%20publish/badge.svg)](https://hub.docker.com/r/brndnmtthws/thetagang) [![Python Publish](https://github.com/brndnmtthws/thetagang/workflows/Python%20Publish/badge.svg)](https://pypi.org/project/thetagang/) [![Docker Pulls](https://img.shields.io/docker/pulls/brndnmtthws/thetagang)](https://hub.docker.com/r/brndnmtthws/thetagang) [![PyPI download month](https://img.shields.io/pypi/dm/thetagang?label=PyPI%20downloads)](https://pypi.python.org/pypi/thetagang/)\n\n[💬 Join the Matrix chat, we can get money together](https://matrix.to/#/#thetagang:frens.io).\n\n# Θ ThetaGang Θ\n\n*Beat the capitalists at their own game with ThetaGang 📈*\n\n![Decay my sweet babies](thetagang.jpg)\n\nThetaGang is an [IBKR](https://www.interactivebrokers.com/) trading bot for\ncollecting premium by selling options using "The Wheel" strategy. The Wheel\nis a strategy that [surfaced on\nReddit](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/),\nbut has been used by many in the past. This bot implements a slightly\nmodified version of The Wheel, with my own personal tweaks.\n\nI\'ve been streaming most of the work on this project [on Twitch, so follow me\nover there](https://www.twitch.tv/letsmakestuff).\n\n## How it works\n\nStart by reading [the Reddit\npost](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/)\nto get some background.\n\nThe strategy, as implemented here, does a few things differently from the one\ndescribed in the post above. For one, it\'s intended to be used to augment a\ntypical index-fund based portfolio with specific asset allocations. For\nexample, you might want to use a 60/40 portfolio with SPY (S&P500 fund) and\nTLT (20 year treasury fund). This strategy reduces risk, but may also limit\ngains from big market swings. By reducing risk, one can increase leverage.\n\nThe main difference between ThetaGang and simply buying and holding index\nfunds is that this script will attempt to harvest volatility by selling\noptions, rather than buying shares directly. This works because implied\nvolatility is typically higher than realized volatility on average. Instead\nof buying shares, you write puts. This has pros and cons, which are outside\nthe scope of this README.\n\nYou could use this tool on individual stocks, but I personally don\'t\nrecommend it because I am not smart enough to understand which stocks to buy.\nThat\'s why I just buy index funds.\n\nThetaGang will try to acquire your desired allocation of each stock or ETF\naccording to the weights you specify in the config. To acquire the positions,\nthe script will write puts when conditions are met (config parameters, adequate\nbuying power, acceptable contracts are available, enough shares needed, etc).\n\nThetaGang will continue to roll any open option positions indefinitely, with the\nonly exception being ITM puts (although this is configurable). Once puts are in\nthe money, they will be ignored until they expire and are exercised (after which\nyou will own the underlying). When rolling puts, the strike of the new contracts\nare capped at the old strike plus the premium received (to prevent your account\nfrom blowing due to over-ratcheting up the buying power usage).\n\nIf puts are exercised due to being ITM at expiration, you will own the\nstock, and ThetaGang switches from writing puts to writing calls at a strike\nat least as high as the average cost of the stock held.\n\nPlease note: this strategy is based on the assumption that implied volatility\nis, on average, always higher than realized volatility. In cases where this\nis not true, this strategy will cause you to lose money.\n\nIn the case of deep ITM calls, the bot will prefer to roll the calls to next\nstrike or expiration rather than allowing the underlying to get called away. If you\ndon\'t have adequate buying power available in your account, it\'s possible\nthat the options may get exercised instead of rolling forward and the process\nstarts back at the beginning. Please keep in mind this may have tax\nimplications, but that is outside the scope of this README.\n\nIn normal usage, you would run the script as a cronjob on a daily, weekly, or\nmonthly basis according to your preferences. Running more frequently than\ndaily is not recommended, but the choice is yours.\n\n![Paper account sample output](sample.gif)\n\n## Project status\n\nThis project is, in its current state, considered to be complete. I\'m open\nto contributions, but I am unlikely to accept PRs or feature requests that\ninvolve significant changes to the underlying algorithm.\n\nIf you find something that you think is a bug, or some other issue, please\n[create a new issue](https://github.com/brndnmtthws/thetagang/issues/new).\n\n## "Show me your gains bro" – i.e., what are the returns?\n\nAs discussed elsewhere in this README, you must conduct your own research,\nand I suggest starting with resources such as CBOE\'s BXM and BXDM indices,\nand comparing those to SPX. I\'ve had a lot of people complain because "that\nstrategy isn\'t better than buy and hold BRUH"–let me assure you, that is not\nmy goal with this.\n\nThere are conflicting opinions about whether selling options is good or bad,\nmore or less risky, yadda yadda, but generally the risk profile for covered\ncalls and naked puts is no worse than the worst case for simply holding an\nETF or stock. In fact, I\'d argue that selling a naked put is better than\nbuying SPY with a limit order, because at least if SPY goes to zero you keep\nthe premium from selling the option. The main downside is that returns are\ncapped on the upside. Depending on your goals, this may not matter. If you\'re\nlike me, then you\'d rather have consistent returns and give up a little bit\nof potential upside.\n\nGenerally speaking, the point of selling options is not to exceed the returns\nof the underlying, but rather to reduce risk. Reducing risk is an important\nfeature because it, in turn, allows one to increase risk in other ways\n(i.e., allocate higher percentage to stocks or buy riskier assets).\n\nWhether you use this or not is up to you. I have not one single fuck to give,\nwhether you use it or not. I am not here to convince you to use it, I merely\nwant to share knowledge and perhaps help create a little bit of wealth\nredistribution.\n\n💫\n\n## Requirements\n\nThe bot is based on the [ib_insync](https://github.com/erdewit/ib_insync)\nlibrary, and uses [IBC](https://github.com/IbcAlpha/IBC) for managing the API\ngateway.\n\nTo use the bot, you\'ll need an Interactive Brokers account with a working\ninstallation of IBC. If you want to modify the bot, you\'ll need an\ninstallation of Python 3.8 or newer with the\n[`poetry`](https://python-poetry.org/) package manager.\n\nOne more thing: to run this on a live account, you\'ll require enough capital\nto purchase at least 100 shares of the stocks or ETFs you choose. For\nexample, if SPY is trading at $300/share you\'d need $30,000 available. You\ncan search for lower priced alternatives, but these tend to have low volume\non options which may not be appropriate for this strategy. You should\ngenerally avoid low volume ETFs/stocks. If you don\'t have that kind of\ncapital, you\'ll need to keep renting out your time to the capitalists until\nyou can become a capitalist yourself. That\'s the way the pyramid scheme we\ncall capitalism works.\n\n## Installation\n\n*Before running ThetaGang, you should set up an IBKR paper account to test the\ncode.*\n\n```console\n$ pip install thetagang\n```\n\nIt\'s recommended you familiarize yourself with\n[IBC](https://github.com/IbcAlpha/IBC) so you know how it works. You\'ll need\nto know how to configure the various knows and settings, and make sure things\nlike API ports are configured correctly. If you don\'t want to mess around too\nmuch, consider [running ThetaGang with Docker](#running-with-docker).\n\n## Usage\n\n```console\n$ thetagang -h\n```\n\n## Up and running with Docker\n\nMy preferred way for running ThetaGang is to use a cronjob to execute Docker\ncommands. I\'ve built a Docker image as part of this project, which you can\nuse with your installation. There\'s a [prebuilt Docker image\nhere](https://hub.docker.com/repository/docker/brndnmtthws/thetagang).\n\nTo run ThetaGang within Docker, you\'ll need to pass `config.ini` for [IBC\nconfiguration](https://github.com/IbcAlpha/IBC/blob/master/userguide.md) and\n[`thetagang.toml`](/thetagang.toml) for ThetaGang. There\'s a sample\n[`ibc-config.ini`](/ibc-config.ini) included in this repo for your convenience.\n\nThe easiest way to get the config files into the container is by mounting a\nvolume.\n\nTo get started, grab a copy of `thetagang.toml` and `config.ini`:\n\n```console\n$ mkdir ~/thetagang\n$ cd ~/thetagang\n$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml\n$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini\n```\n\nEdit `~/thetagang/thetagang.toml` to suit your needs. Pay particular\nattention to the symbols and weights. At a minimum, you must change the\nusername, password, and account number. You may also want to change the\ntrading move from paper to live when needed.\n\nNow, to run ThetaGang with Docker:\n\n```console\n$ docker run --rm -i --net host \\\n    -v ~/thetagang:/etc/thetagang \\\n    brndnmtthws/thetagang:main \\\n    --config /etc/thetagang/thetagang.toml\n```\n\nLastly, to run ThetaGang as a daily cronjob Monday to Friday at 9am, add\nsomething like this to your crontab (on systems with a cron installation, use\n`crontab -e` to edit your crontab):\n\n```crontab\n0 9 * * 1-5 docker run --rm -i -v ~/thetagang:/etc/thetagang brndnmtthws/thetagang:main --config /etc/thetagang/thetagang.toml\n```\n\n## Determining which ETFs or stocks to run ThetaGang with\n\nI leave this as an exercise to the reader, however I will provide a few\nrecommendations and resources:\n\n### Recommendations\n\n* Stick with high volume ETFs or stocks\n* Careful with margin usage, you\'ll want to calculate the worst case scenario\n  and provide plenty of cushion for yourself based on your portfolio\n\n\n### Resources\n\n* For discussions about selling options, check out\n  [r/thetagang](https://www.reddit.com/r/thetagang/)\n* For backtesting portfolios, you can use [this\n  tool](https://www.portfoliovisualizer.com/backtest-portfolio) and [this\n  tool](https://www.portfoliovisualizer.com/optimize-portfolio) to get an idea\n  of drawdown and typical volatility\n\n## Development\n\nCheck out the code to your local machine and install the Python dependencies:\n\n```shell\n$ poetry install\n$ poetry run autohooks activate\n$ poetry run thetagang -h\n...\n```\n\nYou are now ready to make a splash! 🐳\n\n## FAQ\n\n| Error                                                                                                      | Cause                                                                                                                            | Resolution                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| Requested market data is not subscribed.                                                                   | Requisite market data subscriptions have not been set up on IBKR.                                                                | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |\n| No market data during competing live session                                                               | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script.                                                                                                                                                                                                                                                                                                                                                                                                |\n| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol.                                                    | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn\'t required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`.                                                                                                                                                                                                                   |\n\n## Support and sponsorship\n\nIf you get some value out of this, please consider [sponsoring me](https://github.com/sponsors/brndnmtthws)\nto continue maintaining this project well into the future. Like\neveryone else in the world, I\'m just trying to survive.\n\nIf you like what you see but want something different, I am willing\nto work on bespoke or custom trading bots for a fee. Reach out\nto me directly through my GitHub profile.\n\n## Stargazers over time\n\n[![Stargazers over time](https://starchart.cc/brndnmtthws/thetagang.svg)](https://starchart.cc/brndnmtthws/thetagang)\n',
-    'author': 'Brenden Matthews',
-    'author_email': 'brenden@brndn.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/brndnmtthws/thetagang',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# Θ ThetaGang Θ
 
+*Beat the capitalists at their own game with ThetaGang 📈*
+
+![Decay my sweet babies](thetagang.jpg)
+
+ThetaGang is an [IBKR](https://www.interactivebrokers.com/) trading bot for
+collecting premium by selling options using "The Wheel" strategy. The Wheel
+is a strategy that [surfaced on
+Reddit](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/),
+but has been used by many in the past. This bot implements a slightly
+modified version of The Wheel, with my own personal tweaks.
+
+I've been streaming most of the work on this project [on Twitch, so follow me
+over there](https://www.twitch.tv/letsmakestuff).
+
+## How it works
+
+Start by reading [the Reddit
+post](https://www.reddit.com/r/options/comments/a36k4j/the_wheel_aka_triple_income_strategy_explained/)
+to get some background.
+
+The strategy, as implemented here, does a few things differently from the one
+described in the post above. For one, it's intended to be used to augment a
+typical index-fund based portfolio with specific asset allocations. For
+example, you might want to use a 60/40 portfolio with SPY (S&P500 fund) and
+TLT (20 year treasury fund). This strategy reduces risk, but may also limit
+gains from big market swings. By reducing risk, one can increase leverage.
+
+The main difference between ThetaGang and simply buying and holding index
+funds is that this script will attempt to harvest volatility by selling
+options, rather than buying shares directly. This works because implied
+volatility is typically higher than realized volatility on average. Instead
+of buying shares, you write puts. This has pros and cons, which are outside
+the scope of this README.
+
+You could use this tool on individual stocks, but I personally don't
+recommend it because I am not smart enough to understand which stocks to buy.
+That's why I just buy index funds.
+
+ThetaGang will try to acquire your desired allocation of each stock or ETF
+according to the weights you specify in the config. To acquire the positions,
+the script will write puts when conditions are met (config parameters, adequate
+buying power, acceptable contracts are available, enough shares needed, etc).
+
+ThetaGang will continue to roll any open option positions indefinitely, with the
+only exception being ITM puts (although this is configurable). Once puts are in
+the money, they will be ignored until they expire and are exercised (after which
+you will own the underlying). When rolling puts, the strike of the new contracts
+are capped at the old strike plus the premium received (to prevent your account
+from blowing due to over-ratcheting up the buying power usage).
+
+If puts are exercised due to being ITM at expiration, you will own the
+stock, and ThetaGang switches from writing puts to writing calls at a strike
+at least as high as the average cost of the stock held.
+
+Please note: this strategy is based on the assumption that implied volatility
+is, on average, always higher than realized volatility. In cases where this
+is not true, this strategy will cause you to lose money.
+
+In the case of deep ITM calls, the bot will prefer to roll the calls to next
+strike or expiration rather than allowing the underlying to get called away. If you
+don't have adequate buying power available in your account, it's possible
+that the options may get exercised instead of rolling forward and the process
+starts back at the beginning. Please keep in mind this may have tax
+implications, but that is outside the scope of this README.
+
+In normal usage, you would run the script as a cronjob on a daily, weekly, or
+monthly basis according to your preferences. Running more frequently than
+daily is not recommended, but the choice is yours.
+
+![Paper account sample output](sample.gif)
+
+## Project status
+
+This project is, in its current state, considered to be complete. I'm open
+to contributions, but I am unlikely to accept PRs or feature requests that
+involve significant changes to the underlying algorithm.
+
+If you find something that you think is a bug, or some other issue, please
+[create a new issue](https://github.com/brndnmtthws/thetagang/issues/new).
+
+## "Show me your gains bro" – i.e., what are the returns?
+
+As discussed elsewhere in this README, you must conduct your own research,
+and I suggest starting with resources such as CBOE's BXM and BXDM indices,
+and comparing those to SPX. I've had a lot of people complain because "that
+strategy isn't better than buy and hold BRUH"–let me assure you, that is not
+my goal with this.
+
+There are conflicting opinions about whether selling options is good or bad,
+more or less risky, yadda yadda, but generally the risk profile for covered
+calls and naked puts is no worse than the worst case for simply holding an
+ETF or stock. In fact, I'd argue that selling a naked put is better than
+buying SPY with a limit order, because at least if SPY goes to zero you keep
+the premium from selling the option. The main downside is that returns are
+capped on the upside. Depending on your goals, this may not matter. If you're
+like me, then you'd rather have consistent returns and give up a little bit
+of potential upside.
+
+Generally speaking, the point of selling options is not to exceed the returns
+of the underlying, but rather to reduce risk. Reducing risk is an important
+feature because it, in turn, allows one to increase risk in other ways
+(i.e., allocate higher percentage to stocks or buy riskier assets).
+
+Whether you use this or not is up to you. I have not one single fuck to give,
+whether you use it or not. I am not here to convince you to use it, I merely
+want to share knowledge and perhaps help create a little bit of wealth
+redistribution.
+
+💫
+
+## Requirements
+
+The bot is based on the [ib_insync](https://github.com/erdewit/ib_insync)
+library, and uses [IBC](https://github.com/IbcAlpha/IBC) for managing the API
+gateway.
+
+To use the bot, you'll need an Interactive Brokers account with a working
+installation of IBC. If you want to modify the bot, you'll need an
+installation of Python 3.8 or newer with the
+[`poetry`](https://python-poetry.org/) package manager.
+
+One more thing: to run this on a live account, you'll require enough capital
+to purchase at least 100 shares of the stocks or ETFs you choose. For
+example, if SPY is trading at $300/share you'd need $30,000 available. You
+can search for lower priced alternatives, but these tend to have low volume
+on options which may not be appropriate for this strategy. You should
+generally avoid low volume ETFs/stocks. If you don't have that kind of
+capital, you'll need to keep renting out your time to the capitalists until
+you can become a capitalist yourself. That's the way the pyramid scheme we
+call capitalism works.
+
+## Installation
+
+*Before running ThetaGang, you should set up an IBKR paper account to test the
+code.*
+
+```console
+$ pip install thetagang
+```
+
+It's recommended you familiarize yourself with
+[IBC](https://github.com/IbcAlpha/IBC) so you know how it works. You'll need
+to know how to configure the various knows and settings, and make sure things
+like API ports are configured correctly. If you don't want to mess around too
+much, consider [running ThetaGang with Docker](#running-with-docker).
+
+## Usage
+
+```console
+$ thetagang -h
+```
+
+## Up and running with Docker
+
+My preferred way for running ThetaGang is to use a cronjob to execute Docker
+commands. I've built a Docker image as part of this project, which you can
+use with your installation. There's a [prebuilt Docker image
+here](https://hub.docker.com/repository/docker/brndnmtthws/thetagang).
+
+To run ThetaGang within Docker, you'll need to pass `config.ini` for [IBC
+configuration](https://github.com/IbcAlpha/IBC/blob/master/userguide.md) and
+[`thetagang.toml`](/thetagang.toml) for ThetaGang. There's a sample
+[`ibc-config.ini`](/ibc-config.ini) included in this repo for your convenience.
+
+The easiest way to get the config files into the container is by mounting a
+volume.
+
+To get started, grab a copy of `thetagang.toml` and `config.ini`:
+
+```console
+$ mkdir ~/thetagang
+$ cd ~/thetagang
+$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/thetagang.toml -o ./thetagang.toml
+$ curl -Lq https://raw.githubusercontent.com/brndnmtthws/thetagang/main/ibc-config.ini -o ./config.ini
+```
+
+Edit `~/thetagang/thetagang.toml` to suit your needs. Pay particular
+attention to the symbols and weights. At a minimum, you must change the
+username, password, and account number. You may also want to change the
+trading move from paper to live when needed.
+
+Now, to run ThetaGang with Docker:
+
+```console
+$ docker run --rm -i --net host \
+    -v ~/thetagang:/etc/thetagang \
+    brndnmtthws/thetagang:main \
+    --config /etc/thetagang/thetagang.toml
+```
+
+Lastly, to run ThetaGang as a daily cronjob Monday to Friday at 9am, add
+something like this to your crontab (on systems with a cron installation, use
+`crontab -e` to edit your crontab):
+
+```crontab
+0 9 * * 1-5 docker run --rm -i -v ~/thetagang:/etc/thetagang brndnmtthws/thetagang:main --config /etc/thetagang/thetagang.toml
+```
+
+## Determining which ETFs or stocks to run ThetaGang with
+
+I leave this as an exercise to the reader, however I will provide a few
+recommendations and resources:
+
+### Recommendations
+
+* Stick with high volume ETFs or stocks
+* Careful with margin usage, you'll want to calculate the worst case scenario
+  and provide plenty of cushion for yourself based on your portfolio
+
+
+### Resources
+
+* For discussions about selling options, check out
+  [r/thetagang](https://www.reddit.com/r/thetagang/)
+* For backtesting portfolios, you can use [this
+  tool](https://www.portfoliovisualizer.com/backtest-portfolio) and [this
+  tool](https://www.portfoliovisualizer.com/optimize-portfolio) to get an idea
+  of drawdown and typical volatility
+
+## Development
+
+Check out the code to your local machine and install the Python dependencies:
+
+```shell
+$ poetry install
+$ poetry run autohooks activate
+$ poetry run thetagang -h
+...
+```
+
+You are now ready to make a splash! 🐳
+
+## FAQ
+
+| Error                                                                                                      | Cause                                                                                                                            | Resolution                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Requested market data is not subscribed.                                                                   | Requisite market data subscriptions have not been set up on IBKR.                                                                | [Configure](https://www.interactivebrokers.com/en/software/am3/am/settings/marketdatasubscriptions.htm) your market data subscriptions. The default config that ships with this script uses the `Cboe One Add-On Bundle` and the `US Equity and Options Add-On Streaming Bundle`. **Note**: You _must_ fund your account before IBKR will send data for subscriptions. Without funding you can still subscribe but you will get an error from ibc. |
+| No market data during competing live session                                                               | Your account is logged in somewhere else, such as the IBKR web portal, the desktop app, or even another instance of this script. | Log out of all sessions and then re-run the script.                                                                                                                                                                                                                                                                                                                                                                                                |
+| `ib_insync.wrapper ERROR Error 200, reqId 10: The contract description specified for SYMBOL is ambiguous.` | IBKR needs to know which exchange is the primary exchange for a given symbol.                                                    | You need to specify the primary exchange for the stock. This is normal for companies, typically. For ETFs it usually isn't required. Specify the `primary_exchange` parameter for the symbol, i.e., `primary_exchange = "NYSE"`.                                                                                                                                                                                                                   |
+
+## Support and sponsorship
+
+If you get some value out of this, please consider [sponsoring me](https://github.com/sponsors/brndnmtthws)
+to continue maintaining this project well into the future. Like
+everyone else in the world, I'm just trying to survive.
+
+If you like what you see but want something different, I am willing
+to work on bespoke or custom trading bots for a fee. Reach out
+to me directly through my GitHub profile.
+
+## Stargazers over time
+
+[![Stargazers over time](https://starchart.cc/brndnmtthws/thetagang.svg)](https://starchart.cc/brndnmtthws/thetagang)
 
-setup(**setup_kwargs)
```

