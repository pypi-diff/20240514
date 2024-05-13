# Comparing `tmp/py_alpaca_api-0.2.7.tar.gz` & `tmp/py_alpaca_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.2.7.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.3.0.tar", max compression
```

## Comparing `py_alpaca_api-0.2.7.tar` & `py_alpaca_api-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.2.7/LICENSE
--rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.7/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0    44564 2024-05-12 20:57:16.476460 py_alpaca_api-0.2.7/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0    18290 2024-05-12 20:57:16.456460 py_alpaca_api-0.2.7/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     1225 2024-05-12 20:59:25.106424 py_alpaca_api-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.3.0/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0    45327 2024-05-13 23:08:08.097238 py_alpaca_api-0.3.0/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0    19356 2024-05-13 23:08:08.087238 py_alpaca_api-0.3.0/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     1279 2024-05-13 23:09:15.937219 py_alpaca_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.3.0/PKG-INFO
```

### Comparing `py_alpaca_api-0.2.7/LICENSE` & `py_alpaca_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.2.7/README.md` & `py_alpaca_api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.2.7/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.3.0/py_alpaca_api/alpaca.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,14 +313,15 @@
                 "unrealized_plpc": "profit_pct",
                 "unrealized_intraday_pl": "intraday_profit_dol",
                 "unrealized_intraday_plpc": "intraday_profit_pct",
             },
             inplace=True,
         )
         # Calculate portfolio percentage
+        pos_data_df["market_value"] = pos_data_df["market_value"].astype(float)
         asset_sum = pos_data_df["market_value"].sum()
         pos_data_df["portfolio_pct"] = pos_data_df["market_value"] / asset_sum
         # Convert columns to appropriate data types
         pos_data_df = pos_data_df.astype(
             {
                 "asset_id": "str",
                 "symbol": "str",
@@ -416,16 +417,34 @@
         url = f"{self.trade_url}/positions/{symbol}"
         # Get request to Alpaca API for position information
         response = requests.get(url, headers=self.headers)
         # Check if response is successful
         if response.status_code != 200:
             # Raise exception if response is not successful
             raise ValueError(response.text)
+
+        res_dict = json.loads(response.text)
+
+        equity = self.get_account().equity
+        res_dict["portfolio_pct"] = round(float(res_dict["market_value"]) / equity, 4)
+
+        res_dict["profit_dol"] = round(float(res_dict["unrealized_pl"]), 2)
+        del res_dict["unrealized_pl"]
+
+        res_dict["profit_pct"] = round(float(res_dict["unrealized_plpc"]), 4)
+        del res_dict["unrealized_plpc"]
+
+        res_dict["intraday_profit_dol"] = round(float(res_dict["unrealized_intraday_pl"]), 2)
+        del res_dict["unrealized_intraday_pl"]
+
+        res_dict["intraday_profit_pct"] = round(float(res_dict["unrealized_intraday_plpc"]), 4)
+        del res_dict["unrealized_intraday_plpc"]
+
         # Return position information as a PositionClass object
-        return position_class_from_dict(json.loads(response.text))
+        return position_class_from_dict(res_dict)
 
     ########################################################
     # \\\\\\\\\\\\\\\\ Close All Positions ////////////////#
     ########################################################
     def close_all_positions(self, cancel_orders: bool = False):
         """Close all positions
```

### Comparing `py_alpaca_api-0.2.7/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.3.0/py_alpaca_api/src/data_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -305,18 +305,30 @@
 
     Returns:
     --------
     ClockClass
         A ClockClass object.
     """  # noqa
     return ClockClass(
-        market_time=(data_dict["timestamp"].split(".")[0].replace("T", " ") if data_dict["timestamp"] else ""),
+        market_time=(
+            datetime.strptime(data_dict["timestamp"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["timestamp"]
+            else datetime.date(0, 0, 0)
+        ),
         is_open=bool(data_dict["is_open"]),
-        next_open=(data_dict["next_open"].replace("T", " ").replace("-04:00", "") if data_dict["next_open"] else ""),
-        next_close=(data_dict["next_close"].replace("-04:00", "").replace("T", " ") if data_dict["next_close"] else ""),
+        next_open=(
+            datetime.strptime(data_dict["next_open"].replace("T", " ").replace("-04:00", ""), "%Y-%m-%d %H:%M:%S")
+            if data_dict["next_open"]
+            else datetime.date(0, 0, 0)
+        ),
+        next_close=(
+            datetime.strptime(data_dict["next_close"].replace("-04:00", "").replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["next_close"]
+            else datetime.date(0, 0, 0)
+        ),
     )
 
 
 ############################################
 # Data Class Position Conversion Functions
 ############################################
 def position_class_from_dict(data_dict):
@@ -328,33 +340,34 @@
         A dictionary containing the position data.
 
     Returns:
     --------
     PositionClass
         A PositionClass object.
     """  # noqa
+
     return PositionClass(
-        asset_id=str(data_dict["asset_id"]) if data_dict["asset_id"] else "",
-        symbol=str(data_dict["symbol"]) if data_dict["symbol"] else "",
-        exchange=str(data_dict["exchange"]) if data_dict["exchange"] else "",
-        asset_class=(str(data_dict["asset_class"]) if data_dict["asset_class"] else ""),
-        avg_entry_price=(float(data_dict["avg_entry_price"]) if data_dict["avg_entry_price"] else 0),
-        qty=(float(data_dict["qty"]) if data_dict["qty"] else 0),
-        qty_available=(float(data_dict["qty_available"]) if data_dict["qty_available"] else 0),
-        side=str(data_dict["side"]) if data_dict["side"] else "",
-        market_value=(float(data_dict["market_value"]) if data_dict["market_value"] else 0),
-        cost_basis=(float(data_dict["cost_basis"]) if data_dict["cost_basis"] else 0),
-        profit_dol=(float(data_dict["profit_dol"]) if data_dict["profit_dol"] else 0),
-        profit_pct=(float(data_dict["profit_pct"]) if data_dict["profit_pct"] else 0),
-        intraday_profit_dol=(float(data_dict["intraday_profit_dol"]) if data_dict["intraday_profit_dol"] else 0),
-        intraday_profit_pct=(float(data_dict["intraday_profit_pct"]) if data_dict["intraday_profit_pct"] else 0),
-        portfolio_pct=(float(data_dict["portfolio_pct"]) if data_dict["portfolio_pct"] else 0),
-        current_price=(float(data_dict["current_price"]) if data_dict["current_price"] else 0),
-        lastday_price=(float(data_dict["lastday_price"]) if data_dict["lastday_price"] else 0),
-        change_today=(float(data_dict["change_today"]) if data_dict["change_today"] else 0),
+        asset_id=str(data_dict["asset_id"] if data_dict["asset_id"] else ""),
+        symbol=str(data_dict["symbol"] if data_dict["symbol"] else ""),
+        exchange=str(data_dict["exchange"] if data_dict["exchange"] else ""),
+        asset_class=str(data_dict["asset_class"] if data_dict["asset_class"] else ""),
+        avg_entry_price=float(data_dict["avg_entry_price"] if data_dict["avg_entry_price"] else 0),
+        qty=float(data_dict["qty"] if data_dict["qty"] else 0),
+        qty_available=float(data_dict["qty_available"] if data_dict["qty_available"] else 0),
+        side=str(data_dict["side"] if data_dict["side"] else ""),
+        market_value=float(data_dict["market_value"] if data_dict["market_value"] else 0),
+        cost_basis=float(data_dict["cost_basis"] if data_dict["cost_basis"] else 0),
+        profit_dol=float(data_dict["profit_dol"] if data_dict["profit_dol"] else 0),
+        profit_pct=float(data_dict["profit_pct"] if data_dict["profit_pct"] else 0),
+        intraday_profit_dol=float(data_dict["intraday_profit_dol"] if data_dict["intraday_profit_dol"] else 0),
+        intraday_profit_pct=float(data_dict["intraday_profit_pct"] if data_dict["intraday_profit_pct"] else 0),
+        portfolio_pct=float(data_dict["portfolio_pct"] if data_dict["portfolio_pct"] else 0),
+        current_price=float(data_dict["current_price"] if data_dict["current_price"] else 0),
+        lastday_price=float(data_dict["lastday_price"] if data_dict["lastday_price"] else 0),
+        change_today=float(data_dict["change_today"] if data_dict["change_today"] else 0),
         asset_marginable=bool(data_dict["asset_marginable"]),
     )
 
 
 ############################################
 # Data Class Account Conversion Functions
 ############################################
@@ -368,54 +381,58 @@
 
     Returns:
     --------
     AccountClass
         An AccountClass object.
     """  # noqa
     return AccountClass(
-        id=str(data_dict["id"]) if data_dict["id"] else "",
+        id=str(data_dict["id"] if data_dict["id"] else ""),
         account_number=str(data_dict["account_number"]),
-        status=str(data_dict["status"]) if data_dict["status"] else "",
-        crypto_status=(str(data_dict["crypto_status"]) if data_dict["crypto_status"] else ""),
-        options_approved_level=(int(data_dict["options_approved_level"]) if data_dict["options_approved_level"] else None),
-        options_trading_level=(int(data_dict["options_trading_level"]) if data_dict["options_trading_level"] else None),
-        currency=str(data_dict["currency"]) if data_dict["currency"] else "",
-        buying_power=(float(data_dict["buying_power"]) if data_dict["buying_power"] else None),
-        regt_buying_power=(float(data_dict["regt_buying_power"]) if data_dict["regt_buying_power"] else None),
-        daytrading_buying_power=(float(data_dict["daytrading_buying_power"]) if data_dict["daytrading_buying_power"] else None),
-        effective_buying_power=(float(data_dict["effective_buying_power"]) if data_dict["effective_buying_power"] else None),
-        non_marginable_buying_power=(float(data_dict["non_marginable_buying_power"]) if data_dict["non_marginable_buying_power"] else None),
-        options_buying_power=(float(data_dict["options_buying_power"]) if data_dict["options_buying_power"] else None),
-        bod_dtbp=(float(data_dict["bod_dtbp"]) if data_dict["bod_dtbp"] else None),
-        cash=float(data_dict["cash"]) if data_dict["cash"] else None,
-        accrued_fees=(float(data_dict["accrued_fees"]) if data_dict["accrued_fees"] else None),
-        pending_transfer_in=(float(data_dict["pending_transfer_in"]) if data_dict["pending_transfer_in"] else None),
-        portfolio_value=(float(data_dict["portfolio_value"]) if data_dict["portfolio_value"] else None),
+        status=str(data_dict["status"] if data_dict["status"] else ""),
+        crypto_status=str(data_dict["crypto_status"] if data_dict["crypto_status"] else ""),
+        options_approved_level=int(data_dict["options_approved_level"] if data_dict["options_approved_level"] else 0),
+        options_trading_level=int(data_dict["options_trading_level"] if data_dict["options_trading_level"] else 0),
+        currency=str(data_dict["currency"] if data_dict["currency"] else ""),
+        buying_power=float(data_dict["buying_power"] if data_dict["buying_power"] else 0),
+        regt_buying_power=float(data_dict["regt_buying_power"] if data_dict["regt_buying_power"] else 0),
+        daytrading_buying_power=float(data_dict["daytrading_buying_power"] if data_dict["daytrading_buying_power"] else 0),
+        effective_buying_power=float(data_dict["effective_buying_power"] if data_dict["effective_buying_power"] else 0),
+        non_marginable_buying_power=float(data_dict["non_marginable_buying_power"] if data_dict["non_marginable_buying_power"] else 0),
+        options_buying_power=float(data_dict["options_buying_power"] if data_dict["options_buying_power"] else 0),
+        bod_dtbp=float(data_dict["bod_dtbp"] if data_dict["bod_dtbp"] else 0),
+        cash=float(data_dict["cash"] if data_dict["cash"] else 0),
+        accrued_fees=float(data_dict["accrued_fees"] if data_dict["accrued_fees"] else 0),
+        pending_transfer_in=float(data_dict["pending_transfer_in"] if data_dict["pending_transfer_in"] else 0),
+        portfolio_value=float(data_dict["portfolio_value"] if data_dict["portfolio_value"] else 0),
         pattern_day_trader=bool(data_dict["pattern_day_trader"]),
         trading_blocked=bool(data_dict["trading_blocked"]),
         transfers_blocked=bool(data_dict["transfers_blocked"]),
         account_blocked=bool(data_dict["account_blocked"]),
-        created_at=(data_dict["created_at"].split(".")[0].replace("T", " ") if data_dict["created_at"] else None),
+        created_at=(
+            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["created_at"]
+            else datetime.date(0, 0, 0)
+        ),
         trade_suspended_by_user=bool(data_dict["trade_suspended_by_user"]),
-        multiplier=(int(data_dict["multiplier"]) if data_dict["multiplier"] else None),
+        multiplier=int(data_dict["multiplier"] if data_dict["multiplier"] else 0),
         shorting_enabled=bool(data_dict["shorting_enabled"]),
-        equity=float(data_dict["equity"]) if data_dict["equity"] else None,
-        last_equity=(float(data_dict["last_equity"]) if data_dict["last_equity"] else None),
-        long_market_value=(float(data_dict["long_market_value"]) if data_dict["long_market_value"] else None),
-        short_market_value=(float(data_dict["short_market_value"]) if data_dict["short_market_value"] else None),
-        position_market_value=(float(data_dict["position_market_value"]) if data_dict["position_market_value"] else None),
-        initial_margin=(float(data_dict["initial_margin"]) if data_dict["initial_margin"] else None),
-        maintenance_margin=(float(data_dict["maintenance_margin"]) if data_dict["maintenance_margin"] else None),
-        last_maintenance_margin=(float(data_dict["last_maintenance_margin"]) if data_dict["last_maintenance_margin"] else None),
-        sma=float(data_dict["sma"]) if data_dict["sma"] else None,
-        daytrade_count=(int(data_dict["daytrade_count"]) if data_dict["daytrade_count"] else None),
-        balance_asof=(str(data_dict["balance_asof"]) if data_dict["balance_asof"] else ""),
-        crypto_tier=(int(data_dict["crypto_tier"]) if data_dict["crypto_tier"] else None),
-        intraday_adjustments=(int(data_dict["intraday_adjustments"]) if data_dict["intraday_adjustments"] else None),
-        pending_reg_taf_fees=(float(data_dict["pending_reg_taf_fees"]) if data_dict["pending_reg_taf_fees"] else None),
+        equity=float(data_dict["equity"] if data_dict["equity"] else 0),
+        last_equity=float(data_dict["last_equity"] if data_dict["last_equity"] else 0),
+        long_market_value=float(data_dict["long_market_value"] if data_dict["long_market_value"] else 0),
+        short_market_value=float(data_dict["short_market_value"] if data_dict["short_market_value"] else 0),
+        position_market_value=float(data_dict["position_market_value"] if data_dict["position_market_value"] else 0),
+        initial_margin=float(data_dict["initial_margin"] if data_dict["initial_margin"] else 0),
+        maintenance_margin=float(data_dict["maintenance_margin"] if data_dict["maintenance_margin"] else 0),
+        last_maintenance_margin=float(data_dict["last_maintenance_margin"] if data_dict["last_maintenance_margin"] else 0),
+        sma=float(data_dict["sma"] if data_dict["sma"] else 0),
+        daytrade_count=int(data_dict["daytrade_count"] if data_dict["daytrade_count"] else 0),
+        balance_asof=str(data_dict["balance_asof"] if data_dict["balance_asof"] else ""),
+        crypto_tier=int(data_dict["crypto_tier"] if data_dict["crypto_tier"] else 0),
+        intraday_adjustments=int(data_dict["intraday_adjustments"] if data_dict["intraday_adjustments"] else 0),
+        pending_reg_taf_fees=float(data_dict["pending_reg_taf_fees"] if data_dict["pending_reg_taf_fees"] else 0),
     )
 
 
 ############################################
 # Data Class Asset Conversion Functions
 ############################################
 def asset_class_from_dict(data_dict):
@@ -460,42 +477,74 @@
 
     Returns:
     --------
     OrderClass
         An OrderClass object.
     """  # noqa
     return OrderClass(
-        id=str(data_dict["id"]) if data_dict["id"] else "",
-        client_order_id=data_dict["client_order_id"],
-        created_at=(data_dict["created_at"].split(".")[0].replace("T", " ") if data_dict["created_at"] else ""),
-        updated_at=(data_dict["updated_at"].split(".")[0].replace("T", " ") if data_dict["updated_at"] else ""),
-        submitted_at=(data_dict["submitted_at"].split(".")[0].replace("T", " ") if data_dict["submitted_at"] else ""),
-        filled_at=(data_dict["filled_at"].split(".")[0].replace("T", " ") if data_dict["filled_at"] else ""),
-        expired_at=(data_dict["expired_at"].split(".")[0].replace("T", " ") if data_dict["expired_at"] else ""),
-        canceled_at=(data_dict["canceled_at"].split(".")[0].replace("T", " ") if data_dict["canceled_at"] else ""),
-        failed_at=(data_dict["failed_at"].split(".")[0].replace("T", " ") if data_dict["failed_at"] else ""),
-        replaced_at=(data_dict["replaced_at"].split(".")[0].replace("T", " ") if data_dict["replaced_at"] else ""),
-        replaced_by=(data_dict["replaced_by"].split(".")[0].replace("T", " ") if data_dict["replaced_by"] else ""),
-        replaces=str(data_dict["replaces"]) if data_dict["replaces"] else "",
-        asset_id=str(data_dict["asset_id"]) if data_dict["asset_id"] else "",
-        symbol=str(data_dict["symbol"]) if data_dict["symbol"] else "",
-        asset_class=(str(data_dict["asset_class"]) if data_dict["asset_class"] else ""),
-        notional=float(data_dict["notional"]) if data_dict["notional"] else 0,
-        qty=float(data_dict["qty"]) if data_dict["qty"] else 0,
-        filled_qty=(float(data_dict["filled_qty"]) if data_dict["filled_qty"] else 0),
-        filled_avg_price=(float(data_dict["filled_avg_price"]) if data_dict["filled_avg_price"] else 0),
-        order_class=(str(data_dict["order_class"]) if data_dict["order_class"] else ""),
-        order_type=(str(data_dict["order_type"]) if data_dict["order_type"] else ""),
-        type=str(data_dict["type"]) if data_dict["type"] else "",
-        side=str(data_dict["side"]) if data_dict["side"] else "",
-        time_in_force=(str(data_dict["time_in_force"]) if data_dict["time_in_force"] else ""),
-        limit_price=(float(data_dict["limit_price"]) if data_dict["limit_price"] else 0),
-        stop_price=(float(data_dict["stop_price"]) if data_dict["stop_price"] else 0),
-        status=str(data_dict["status"]) if data_dict["status"] else "",
+        id=str(data_dict["id"] if data_dict["id"] else ""),
+        client_order_id=str(data_dict["client_order_id"]),
+        created_at=(
+            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["created_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        updated_at=(
+            datetime.strptime(data_dict["updated_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["updated_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        submitted_at=(
+            datetime.strptime(data_dict["submitted_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["submitted_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        filled_at=(
+            datetime.strptime(data_dict["filled_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["filled_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        expired_at=(
+            datetime.strptime(data_dict["expired_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["expired_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        canceled_at=(
+            datetime.strptime(data_dict["canceled_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["canceled_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        failed_at=(
+            datetime.strptime(data_dict["failed_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["failed_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        replaced_at=(
+            datetime.strptime(data_dict["replaced_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["replaced_at"]
+            else datetime(1, 1, 1, 0, 0)
+        ),
+        replaced_by=str(data_dict["replaced_by"] if data_dict["replaced_by"] else ""),
+        replaces=str(data_dict["replaces"] if data_dict["replaces"] else ""),
+        asset_id=str(data_dict["asset_id"] if data_dict["asset_id"] else ""),
+        symbol=str(data_dict["symbol"] if data_dict["symbol"] else ""),
+        asset_class=str(data_dict["asset_class"] if data_dict["asset_class"] else ""),
+        notional=float(data_dict["notional"] if data_dict["notional"] else 0),
+        qty=float(data_dict["qty"] if data_dict["qty"] else 0),
+        filled_qty=float(data_dict["filled_qty"] if data_dict["filled_qty"] else 0),
+        filled_avg_price=float(data_dict["filled_avg_price"] if data_dict["filled_avg_price"] else 0),
+        order_class=str(data_dict["order_class"] if data_dict["order_class"] else ""),
+        order_type=str(data_dict["order_type"] if data_dict["order_type"] else ""),
+        type=str(data_dict["type"] if data_dict["type"] else ""),
+        side=str(data_dict["side"] if data_dict["side"] else ""),
+        time_in_force=str(data_dict["time_in_force"] if data_dict["time_in_force"] else ""),
+        limit_price=float(data_dict["limit_price"] if data_dict["limit_price"] else 0),
+        stop_price=float(data_dict["stop_price"] if data_dict["stop_price"] else 0),
+        status=str(data_dict["status"] if data_dict["status"] else ""),
         extended_hours=bool(data_dict["extended_hours"]),
-        legs=object(data_dict["legs"]) if data_dict["legs"] else {},
-        trail_percent=(float(data_dict["trail_percent"]) if data_dict["trail_percent"] else 0),
-        trail_price=(float(data_dict["trail_price"]) if data_dict["trail_price"] else 0),
-        hwm=float(data_dict["hwm"]) if data_dict["hwm"] else 0,
-        subtag=str(data_dict["subtag"]) if data_dict["subtag"] else "",
-        source=str(data_dict["source"]) if data_dict["source"] else "",
+        legs=data_dict["legs"] if data_dict["legs"] else {},
+        trail_percent=float(data_dict["trail_percent"] if data_dict["trail_percent"] else 0),
+        trail_price=float(data_dict["trail_price"] if data_dict["trail_price"] else 0),
+        hwm=float(data_dict["hwm"] if data_dict["hwm"] else 0),
+        subtag=str(data_dict["subtag"] if data_dict["subtag"] else ""),
+        source=str(data_dict["source"] if data_dict["source"] else ""),
     )
```

### Comparing `py_alpaca_api-0.2.7/pyproject.toml` & `py_alpaca_api-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.2.7"
+version = "0.3.0"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
@@ -20,14 +20,16 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 requests-mock = "^1.12.1"
 black = "^24.4.2"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ipykernel = "^6.29.4"
+pytest-mock = "^3.14.0"
+pytest-mock-server = "^0.3.0"
 
 
 [tool.poetry.group.test.dependencies]
 flake8 = "^7.0.0"
 
 
 [tool.poetry.group.doc.dependencies]
```

### Comparing `py_alpaca_api-0.2.7/PKG-INFO` & `py_alpaca_api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.2.7
+Version: 0.3.0
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

