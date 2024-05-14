# Comparing `tmp/unusualwhales_python_client-4.1.1.tar.gz` & `tmp/unusualwhales_python_client-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unusualwhales_python_client-4.1.1.tar", max compression
+gzip compressed data, was "unusualwhales_python_client-4.2.1.tar", max compression
```

## Comparing `unusualwhales_python_client-4.1.1.tar` & `unusualwhales_python_client-4.2.1.tar`

### file list

```diff
@@ -1,206 +1,206 @@
--rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusualwhales_python_client-4.1.1/LICENSE
--rw-r--r--   0        0        0     3123 2024-05-13 00:30:59.158405 unusualwhales_python_client-4.1.1/README.md
--rw-r--r--   0        0        0      598 2024-05-13 00:33:44.467311 unusualwhales_python_client-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-13 00:31:21.811050 unusualwhales_python_client-4.1.1/unusualwhales/.DS_Store
--rw-r--r--   0        0        0      194 2024-05-13 00:28:09.144268 unusualwhales_python_client-4.1.1/unusualwhales/__init__.py
--rw-r--r--   0        0        0     6148 2024-05-13 00:31:26.819597 unusualwhales_python_client-4.1.1/unusualwhales/api/.DS_Store
--rw-r--r--   0        0        0       58 2024-05-13 00:33:10.876060 unusualwhales_python_client-4.1.1/unusualwhales/api/__init__.py
--rw-r--r--   0        0        0     1781 2024-05-05 22:58:01.830486 unusualwhales_python_client-4.1.1/unusualwhales/api/congress/__init__.py
--rw-r--r--   0        0        0     7005 2024-05-05 22:58:01.823131 unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_late_reports.py
--rw-r--r--   0        0        0     7023 2024-05-05 22:58:01.824675 unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_reports.py
--rw-r--r--   0        0        0     7014 2024-05-05 22:58:01.831679 unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_trades.py
--rw-r--r--   0        0        0     8028 2024-05-05 22:58:01.826496 unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_trades_by_member.py
--rw-r--r--   0        0        0      446 2024-05-05 22:58:01.829139 unusualwhales_python_client-4.1.1/unusualwhales/api/contract/__init__.py
--rw-r--r--   0        0        0     6138 2024-05-05 22:58:01.830625 unusualwhales_python_client-4.1.1/unusualwhales/api/contract/get_price_history.py
--rw-r--r--   0        0        0      941 2024-05-05 22:58:01.835779 unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/__init__.py
--rw-r--r--   0        0        0     6452 2024-05-05 22:58:01.835589 unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/get_trades_by_date.py
--rw-r--r--   0        0        0     7516 2024-05-05 22:58:01.835085 unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/get_trades_by_ticker.py
--rw-r--r--   0        0        0     1349 2024-05-05 22:58:01.832866 unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/__init__.py
--rw-r--r--   0        0        0     6038 2024-05-05 22:58:01.831679 unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_afterhours.py
--rw-r--r--   0        0        0     6117 2024-05-05 22:58:01.834848 unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_premarket.py
--rw-r--r--   0        0        0     4696 2024-05-05 22:58:01.833809 unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_ticker_earnings.py
--rw-r--r--   0        0        0     1402 2024-05-13 00:31:49.829150 unusualwhales_python_client-4.1.1/unusualwhales/api/endpoints.py
--rw-r--r--   0        0        0     1348 2024-05-05 22:58:01.830714 unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/__init__.py
--rw-r--r--   0        0        0     4023 2024-05-05 22:58:01.833019 unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_holdings.py
--rw-r--r--   0        0        0     4573 2024-05-05 22:58:01.833952 unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_info.py
--rw-r--r--   0        0        0     4855 2024-05-05 22:58:01.834085 unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_sector_country_weights.py
--rw-r--r--   0        0        0     4159 2024-05-05 22:58:01.831930 unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_ticker_exposure.py
--rw-r--r--   0        0        0     2839 2024-05-05 22:58:01.823337 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/__init__.py
--rw-r--r--   0        0        0     8952 2024-05-05 22:58:01.822353 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_contract_flow.py
--rw-r--r--   0        0        0     4453 2024-05-05 22:58:01.825676 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_flow_by_expiry.py
--rw-r--r--   0        0        0     4936 2024-05-05 22:58:01.817837 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_flow_by_strike.py
--rw-r--r--   0        0        0     3238 2024-05-05 22:58:01.828140 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_full_tape.py
--rw-r--r--   0        0        0     7458 2024-05-05 22:58:01.829248 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_order_flow.py
--rw-r--r--   0        0        0    29182 2024-05-05 22:58:01.820244 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_ticker_order_flow.py
--rw-r--r--   0        0        0     5864 2024-05-05 22:58:01.827332 unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_unusual_flow_alerts.py
--rw-r--r--   0        0        0     6232 2024-05-05 22:58:01.822234 unusualwhales_python_client-4.1.1/unusualwhales/api/market/__init__.py
--rw-r--r--   0        0        0     3842 2024-05-05 22:58:01.828023 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_economic_calendar.py
--rw-r--r--   0        0        0     3816 2024-05-05 22:58:01.829065 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_fda_calendar.py
--rw-r--r--   0        0        0     3791 2024-05-05 22:58:01.825695 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_holidays.py
--rw-r--r--   0        0        0     3863 2024-05-05 22:58:01.834907 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_imbalances.py
--rw-r--r--   0        0        0     5779 2024-05-05 22:58:01.829486 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_insider_trades.py
--rw-r--r--   0        0        0     6286 2024-05-05 22:58:01.827248 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_options_volume.py
--rw-r--r--   0        0        0    12838 2024-05-05 22:58:01.834573 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_tide.py
--rw-r--r--   0        0        0     7082 2024-05-05 22:58:01.823487 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_tide_by_etf.py
--rw-r--r--   0        0        0     7741 2024-05-05 22:58:01.835255 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_open_interest_change.py
--rw-r--r--   0        0        0     4661 2024-05-05 22:58:01.832684 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_sector_stats.py
--rw-r--r--   0        0        0     5862 2024-05-05 22:58:01.833214 unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_spike.py
--rw-r--r--   0        0        0     1567 2024-05-05 22:58:01.834188 unusualwhales_python_client-4.1.1/unusualwhales/api/screener/__init__.py
--rw-r--r--   0        0        0     9212 2024-05-05 22:58:01.832213 unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_analyst_ratings.py
--rw-r--r--   0        0        0    45656 2024-05-05 22:58:01.836166 unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_option_contracts.py
--rw-r--r--   0        0        0    64388 2024-05-05 22:58:01.832860 unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_stocks.py
--rw-r--r--   0        0        0     1911 2024-05-05 22:58:01.823405 unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/__init__.py
--rw-r--r--   0        0        0     4349 2024-05-05 22:58:01.835591 unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py
--rw-r--r--   0        0        0     4894 2024-05-05 22:58:01.822528 unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_monthly_average_returns.py
--rw-r--r--   0        0        0    13866 2024-05-05 22:58:01.836165 unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_monthly_top_performers.py
--rw-r--r--   0        0        0     5020 2024-05-05 22:58:01.835479 unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py
--rw-r--r--   0        0        0    17216 2024-05-05 22:58:01.830003 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/__init__.py
--rw-r--r--   0        0        0     5853 2024-05-05 22:58:01.834185 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py
--rw-r--r--   0        0        0     9262 2024-05-05 22:58:01.829643 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_candles.py
--rw-r--r--   0        0        0     6291 2024-05-05 22:58:01.828752 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py
--rw-r--r--   0        0        0    14315 2024-05-05 22:58:01.822998 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure.py
--rw-r--r--   0        0        0     6429 2024-05-05 22:58:01.828427 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py
--rw-r--r--   0        0        0     6497 2024-05-05 22:58:01.829394 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6999 2024-05-05 22:58:01.828148 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py
--rw-r--r--   0        0        0     6480 2024-05-05 22:58:01.832353 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py
--rw-r--r--   0        0        0     6321 2024-05-05 22:58:01.831374 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_info.py
--rw-r--r--   0        0        0     5033 2024-05-05 22:58:01.829629 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_insider_trades.py
--rw-r--r--   0        0        0     4786 2024-05-05 22:58:01.830922 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_max_pain.py
--rw-r--r--   0        0        0    10631 2024-05-05 22:58:01.827490 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_net_premium_ticks.py
--rw-r--r--   0        0        0     7927 2024-05-05 22:58:01.827804 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_open_interest_change.py
--rw-r--r--   0        0        0     7486 2024-05-05 22:58:01.826158 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_chains.py
--rw-r--r--   0        0        0    11023 2024-05-05 22:58:01.833220 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_contracts.py
--rw-r--r--   0        0        0     6147 2024-05-05 22:58:01.825845 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_volume_by_price_level.py
--rw-r--r--   0        0        0     6050 2024-05-05 22:58:01.826463 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_options_volume.py
--rw-r--r--   0        0        0     9170 2024-05-05 22:58:01.834719 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_risk_reversal_skew.py
--rw-r--r--   0        0        0     5024 2024-05-05 22:58:01.828580 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_sector_tickers.py
--rw-r--r--   0        0        0    14302 2024-05-05 22:58:01.827684 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_spot_exposures.py
--rw-r--r--   0        0        0    14631 2024-05-05 22:58:01.823985 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py
--rw-r--r--   0        0        0     6546 2024-05-05 22:58:01.827244 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_volatility_term_structure.py
--rw-r--r--   0        0        0     7312 2024-05-05 22:58:01.833314 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_volume_by_price_level.py
--rw-r--r--   0        0        0     6195 2024-05-05 22:58:01.824309 unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py
--rw-r--r--   0        0        0     7122 2024-05-13 00:28:35.664213 unusualwhales_python_client-4.1.1/unusualwhales/client.py
--rw-r--r--   0        0        0      546 2024-05-05 22:58:01.816143 unusualwhales_python_client-4.1.1/unusualwhales/errors.py
--rw-r--r--   0        0        0    10021 2024-05-05 22:58:01.822073 unusualwhales_python_client-4.1.1/unusualwhales/models/__init__.py
--rw-r--r--   0        0        0     2227 2024-05-05 22:58:01.823494 unusualwhales_python_client-4.1.1/unusualwhales/models/analalyst_rating_results.py
--rw-r--r--   0        0        0      262 2024-05-05 22:58:01.779003 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_action.py
--rw-r--r--   0        0        0      267 2024-05-05 22:58:01.779493 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_field_action.py
--rw-r--r--   0        0        0      183 2024-05-05 22:58:01.758542 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_field_recommendation.py
--rw-r--r--   0        0        0     6697 2024-05-05 22:58:01.820117 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_rating.py
--rw-r--r--   0        0        0      178 2024-05-05 22:58:01.765008 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_recommendation.py
--rw-r--r--   0        0        0      428 2024-05-05 22:58:01.775125 unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_sector.py
--rw-r--r--   0        0        0     5399 2024-05-05 22:58:01.821958 unusualwhales_python_client-4.1.1/unusualwhales/models/candle_data.py
--rw-r--r--   0        0        0     2098 2024-05-05 22:58:01.833898 unusualwhales_python_client-4.1.1/unusualwhales/models/candle_data_results.py
--rw-r--r--   0        0        0      251 2024-05-05 22:58:01.780257 unusualwhales_python_client-4.1.1/unusualwhales/models/candle_size.py
--rw-r--r--   0        0        0     5755 2024-05-05 22:58:01.816560 unusualwhales_python_client-4.1.1/unusualwhales/models/congressional_trade_report.py
--rw-r--r--   0        0        0     2308 2024-05-05 22:58:01.833569 unusualwhales_python_client-4.1.1/unusualwhales/models/congressional_trade_report_results.py
--rw-r--r--   0        0        0     5235 2024-05-05 22:58:01.830332 unusualwhales_python_client-4.1.1/unusualwhales/models/country_sector_exposure.py
--rw-r--r--   0        0        0     3869 2024-05-05 22:58:01.828297 unusualwhales_python_client-4.1.1/unusualwhales/models/daily_market_tide.py
--rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.833609 unusualwhales_python_client-4.1.1/unusualwhales/models/daily_market_tide_response.py
--rw-r--r--   0        0        0     9770 2024-05-05 22:58:01.832534 unusualwhales_python_client-4.1.1/unusualwhales/models/darkpool_trade.py
--rw-r--r--   0        0        0     3375 2024-05-05 22:58:01.818843 unusualwhales_python_client-4.1.1/unusualwhales/models/darkpool_trade_response.py
--rw-r--r--   0        0        0     8924 2024-05-05 22:58:01.834330 unusualwhales_python_client-4.1.1/unusualwhales/models/earnings.py
--rw-r--r--   0        0        0     2069 2024-05-05 22:58:01.833907 unusualwhales_python_client-4.1.1/unusualwhales/models/earnings_results.py
--rw-r--r--   0        0        0     4185 2024-05-05 22:58:01.823207 unusualwhales_python_client-4.1.1/unusualwhales/models/economic_calendar.py
--rw-r--r--   0        0        0      189 2024-05-05 22:58:01.783710 unusualwhales_python_client-4.1.1/unusualwhales/models/economic_type.py
--rw-r--r--   0        0        0     2673 2024-05-05 22:58:01.820875 unusualwhales_python_client-4.1.1/unusualwhales/models/error_message.py
--rw-r--r--   0        0        0     1779 2024-05-05 22:58:01.822650 unusualwhales_python_client-4.1.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
--rw-r--r--   0        0        0     2063 2024-05-05 22:58:01.825400 unusualwhales_python_client-4.1.1/unusualwhales/models/etf_countries_item.py
--rw-r--r--   0        0        0     3171 2024-05-05 22:58:01.822868 unusualwhales_python_client-4.1.1/unusualwhales/models/etf_info.py
--rw-r--r--   0        0        0     6423 2024-05-05 22:58:01.832037 unusualwhales_python_client-4.1.1/unusualwhales/models/etf_info_data.py
--rw-r--r--   0        0        0     2044 2024-05-05 22:58:01.818548 unusualwhales_python_client-4.1.1/unusualwhales/models/etf_sectors_item.py
--rw-r--r--   0        0        0     2953 2024-05-05 22:58:01.832447 unusualwhales_python_client-4.1.1/unusualwhales/models/expiry_breakdown.py
--rw-r--r--   0        0        0     2248 2024-05-05 22:58:01.825125 unusualwhales_python_client-4.1.1/unusualwhales/models/expiry_breakdown_result.py
--rw-r--r--   0        0        0     5086 2024-05-05 22:58:01.817753 unusualwhales_python_client-4.1.1/unusualwhales/models/fda_calendar.py
--rw-r--r--   0        0        0    10635 2024-05-05 22:58:01.817394 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert.py
--rw-r--r--   0        0        0     2086 2024-05-05 22:58:01.816655 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert_results.py
--rw-r--r--   0        0        0      590 2024-05-05 22:58:01.780015 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert_rule.py
--rw-r--r--   0        0        0    12800 2024-05-05 22:58:01.827106 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_expiry.py
--rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.827194 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_expiry_results.py
--rw-r--r--   0        0        0    12688 2024-05-05 22:58:01.819326 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_strike.py
--rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.830018 unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_strike_results.py
--rw-r--r--   0        0        0     6320 2024-05-05 22:58:01.816924 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure.py
--rw-r--r--   0        0        0     6349 2024-05-05 22:58:01.822486 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6808 2024-05-05 22:58:01.831535 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py
--rw-r--r--   0        0        0     2358 2024-05-05 22:58:01.821530 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py
--rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.827851 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_results.py
--rw-r--r--   0        0        0     2134 2024-05-05 22:58:01.816486 unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_results.py
--rw-r--r--   0        0        0     9046 2024-05-05 22:58:01.826947 unusualwhales_python_client-4.1.1/unusualwhales/models/greeks.py
--rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.829764 unusualwhales_python_client-4.1.1/unusualwhales/models/historical_risk_reversal_skew.py
--rw-r--r--   0        0        0     2300 2024-05-05 22:58:01.822832 unusualwhales_python_client-4.1.1/unusualwhales/models/historical_risk_reversal_skew_results.py
--rw-r--r--   0        0        0     8935 2024-05-05 22:58:01.817484 unusualwhales_python_client-4.1.1/unusualwhales/models/holdings.py
--rw-r--r--   0        0        0     2648 2024-05-05 22:58:01.821969 unusualwhales_python_client-4.1.1/unusualwhales/models/holdings_response.py
--rw-r--r--   0        0        0     4229 2024-05-05 22:58:01.818954 unusualwhales_python_client-4.1.1/unusualwhales/models/imbalances_volume.py
--rw-r--r--   0        0        0     4234 2024-05-05 22:58:01.831021 unusualwhales_python_client-4.1.1/unusualwhales/models/implied_volatility_term_structure.py
--rw-r--r--   0        0        0     2348 2024-05-05 22:58:01.822055 unusualwhales_python_client-4.1.1/unusualwhales/models/implied_volatility_term_structure_results.py
--rw-r--r--   0        0        0     3185 2024-05-05 22:58:01.834435 unusualwhales_python_client-4.1.1/unusualwhales/models/insider_statistic.py
--rw-r--r--   0        0        0     2770 2024-05-05 22:58:01.816314 unusualwhales_python_client-4.1.1/unusualwhales/models/insider_statistics.py
--rw-r--r--   0        0        0      190 2024-05-05 22:58:01.766259 unusualwhales_python_client-4.1.1/unusualwhales/models/insider_trades_member_type.py
--rw-r--r--   0        0        0      345 2024-05-05 22:58:01.775861 unusualwhales_python_client-4.1.1/unusualwhales/models/insider_trades_transaction_type.py
--rw-r--r--   0        0        0      164 2024-05-05 22:58:01.778813 unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_imbalance_event.py
--rw-r--r--   0        0        0      165 2024-05-05 22:58:01.783423 unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_imbalance_side.py
--rw-r--r--   0        0        0      213 2024-05-05 22:58:01.776228 unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_imbalance_type.py
--rw-r--r--   0        0        0      168 2024-05-05 22:58:01.773079 unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_market_time.py
--rw-r--r--   0        0        0      528 2024-05-05 22:58:01.774624 unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_sector.py
--rw-r--r--   0        0        0     4512 2024-05-05 22:58:01.834484 unusualwhales_python_client-4.1.1/unusualwhales/models/market_holidays.py
--rw-r--r--   0        0        0     3378 2024-05-05 22:58:01.831296 unusualwhales_python_client-4.1.1/unusualwhales/models/market_options_volume.py
--rw-r--r--   0        0        0     1710 2024-05-05 22:58:01.827677 unusualwhales_python_client-4.1.1/unusualwhales/models/market_sector_ticker_results.py
--rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.830420 unusualwhales_python_client-4.1.1/unusualwhales/models/max_pain.py
--rw-r--r--   0        0        0     2159 2024-05-05 22:58:01.833744 unusualwhales_python_client-4.1.1/unusualwhales/models/max_pain_results.py
--rw-r--r--   0        0        0     3421 2024-05-05 22:58:01.833406 unusualwhales_python_client-4.1.1/unusualwhales/models/net_prem_tick.py
--rw-r--r--   0        0        0     4303 2024-05-05 22:58:01.828862 unusualwhales_python_client-4.1.1/unusualwhales/models/net_prem_tick_results.py
--rw-r--r--   0        0        0     2494 2024-05-05 22:58:01.821207 unusualwhales_python_client-4.1.1/unusualwhales/models/off_lit_price_level.py
--rw-r--r--   0        0        0     2270 2024-05-05 22:58:01.816343 unusualwhales_python_client-4.1.1/unusualwhales/models/off_lit_price_level_results.py
--rw-r--r--   0        0        0    11261 2024-05-05 22:58:01.823477 unusualwhales_python_client-4.1.1/unusualwhales/models/oi_change.py
--rw-r--r--   0        0        0     2101 2024-05-05 22:58:01.828752 unusualwhales_python_client-4.1.1/unusualwhales/models/oi_change_results.py
--rw-r--r--   0        0        0    10954 2024-05-05 22:58:01.817830 unusualwhales_python_client-4.1.1/unusualwhales/models/option_chain_contract.py
--rw-r--r--   0        0        0     2316 2024-05-05 22:58:01.818322 unusualwhales_python_client-4.1.1/unusualwhales/models/option_chain_contract_results.py
--rw-r--r--   0        0        0     2187 2024-05-05 22:58:01.818071 unusualwhales_python_client-4.1.1/unusualwhales/models/option_chains_results.py
--rw-r--r--   0        0        0    11275 2024-05-05 22:58:01.818618 unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract.py
--rw-r--r--   0        0        0     2251 2024-05-05 22:58:01.829762 unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_results.py
--rw-r--r--   0        0        0    14866 2024-05-05 22:58:01.824112 unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_screener_item.py
--rw-r--r--   0        0        0     2375 2024-05-05 22:58:01.831061 unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_screener_results.py
--rw-r--r--   0        0        0      157 2024-05-05 22:58:01.768374 unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_type.py
--rw-r--r--   0        0        0     2522 2024-05-05 22:58:01.825820 unusualwhales_python_client-4.1.1/unusualwhales/models/option_price_level.py
--rw-r--r--   0        0        0     2283 2024-05-05 22:58:01.827958 unusualwhales_python_client-4.1.1/unusualwhales/models/option_price_level_results.py
--rw-r--r--   0        0        0      149 2024-05-05 22:58:01.770159 unusualwhales_python_client-4.1.1/unusualwhales/models/option_type.py
--rw-r--r--   0        0        0      153 2024-05-05 22:58:01.771290 unusualwhales_python_client-4.1.1/unusualwhales/models/order_direction.py
--rw-r--r--   0        0        0      949 2024-05-05 22:58:01.774812 unusualwhales_python_client-4.1.1/unusualwhales/models/screener_contract_order_by_field.py
--rw-r--r--   0        0        0     1401 2024-05-05 22:58:01.780126 unusualwhales_python_client-4.1.1/unusualwhales/models/screener_order_by_field.py
--rw-r--r--   0        0        0     5330 2024-05-05 22:58:01.832188 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_market.py
--rw-r--r--   0        0        0     2245 2024-05-05 22:58:01.817561 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_market_results.py
--rw-r--r--   0        0        0     4802 2024-05-05 22:58:01.826952 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_monthly.py
--rw-r--r--   0        0        0     2864 2024-05-05 22:58:01.816371 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_monthly_results.py
--rw-r--r--   0        0        0      412 2024-05-05 22:58:01.784552 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_performance_order_by.py
--rw-r--r--   0        0        0     6634 2024-05-05 22:58:01.820876 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_performers.py
--rw-r--r--   0        0        0     2884 2024-05-05 22:58:01.822592 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_performers_results.py
--rw-r--r--   0        0        0     2957 2024-05-05 22:58:01.827974 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_year_month.py
--rw-r--r--   0        0        0     3159 2024-05-05 22:58:01.828370 unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_year_month_results.py
--rw-r--r--   0        0        0      515 2024-05-05 22:58:01.783541 unusualwhales_python_client-4.1.1/unusualwhales/models/sector.py
--rw-r--r--   0        0        0    10830 2024-05-05 22:58:01.830188 unusualwhales_python_client-4.1.1/unusualwhales/models/sector_etf.py
--rw-r--r--   0        0        0     2890 2024-05-05 22:58:01.823726 unusualwhales_python_client-4.1.1/unusualwhales/models/sector_etf_results.py
--rw-r--r--   0        0        0      173 2024-05-05 22:58:01.769865 unusualwhales_python_client-4.1.1/unusualwhales/models/side.py
--rw-r--r--   0        0        0      206 2024-05-05 22:58:01.776708 unusualwhales_python_client-4.1.1/unusualwhales/models/single_issue_type.py
--rw-r--r--   0        0        0      343 2024-05-05 22:58:01.762014 unusualwhales_python_client-4.1.1/unusualwhales/models/single_month_number.py
--rw-r--r--   0        0        0      521 2024-05-05 22:58:01.779594 unusualwhales_python_client-4.1.1/unusualwhales/models/single_sector.py
--rw-r--r--   0        0        0      334 2024-05-05 22:58:01.769228 unusualwhales_python_client-4.1.1/unusualwhales/models/single_trade_external_hour_sold_code.py
--rw-r--r--   0        0        0      312 2024-05-05 22:58:01.761864 unusualwhales_python_client-4.1.1/unusualwhales/models/single_trade_sale_cond_code.py
--rw-r--r--   0        0        0      304 2024-05-05 22:58:01.781307 unusualwhales_python_client-4.1.1/unusualwhales/models/single_trade_settlement.py
--rw-r--r--   0        0        0      275 2024-05-05 22:58:01.752668 unusualwhales_python_client-4.1.1/unusualwhales/models/single_trade_trade_code.py
--rw-r--r--   0        0        0     2304 2024-05-05 22:58:01.832942 unusualwhales_python_client-4.1.1/unusualwhales/models/spike_value.py
--rw-r--r--   0        0        0     7769 2024-05-05 22:58:01.832634 unusualwhales_python_client-4.1.1/unusualwhales/models/spot_gex_exposures_per_1_min.py
--rw-r--r--   0        0        0     2274 2024-05-05 22:58:01.833460 unusualwhales_python_client-4.1.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py
--rw-r--r--   0        0        0     8339 2024-05-05 22:58:01.833587 unusualwhales_python_client-4.1.1/unusualwhales/models/spot_greek_exposures_by_strike.py
--rw-r--r--   0        0        0     2305 2024-05-05 22:58:01.817337 unusualwhales_python_client-4.1.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py
--rw-r--r--   0        0        0      202 2024-05-05 22:58:01.756301 unusualwhales_python_client-4.1.1/unusualwhales/models/stock_earnings_time.py
--rw-r--r--   0        0        0      205 2024-05-05 22:58:01.779639 unusualwhales_python_client-4.1.1/unusualwhales/models/stock_issue_type.py
--rw-r--r--   0        0        0    24207 2024-05-05 22:58:01.822193 unusualwhales_python_client-4.1.1/unusualwhales/models/stock_screener_response.py
--rw-r--r--   0        0        0     2280 2024-05-05 22:58:01.823614 unusualwhales_python_client-4.1.1/unusualwhales/models/stock_screener_response_results.py
--rw-r--r--   0        0        0     8648 2024-05-05 22:58:01.828620 unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_info.py
--rw-r--r--   0        0        0     2636 2024-05-05 22:58:01.831049 unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_info_results.py
--rw-r--r--   0        0        0    11609 2024-05-05 22:58:01.832705 unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_options_volume.py
--rw-r--r--   0        0        0     2436 2024-05-05 22:58:01.828948 unusualwhales_python_client-4.1.1/unusualwhales/models/volume_oi_per_expiry.py
--rw-r--r--   0        0        0     2233 2024-05-05 22:58:01.816470 unusualwhales_python_client-4.1.1/unusualwhales/models/volume_oi_per_expiry_results.py
--rw-r--r--   0        0        0       25 2024-05-05 22:58:01.341037 unusualwhales_python_client-4.1.1/unusualwhales/py.typed
--rw-r--r--   0        0        0      985 2024-05-05 22:58:01.827475 unusualwhales_python_client-4.1.1/unusualwhales/types.py
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 unusualwhales_python_client-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusualwhales_python_client-4.2.1/LICENSE
+-rw-r--r--   0        0        0     3107 2024-05-13 06:22:56.179296 unusualwhales_python_client-4.2.1/README.md
+-rw-r--r--   0        0        0      598 2024-05-14 16:51:33.424139 unusualwhales_python_client-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-13 00:31:21.811050 unusualwhales_python_client-4.2.1/unusualwhales/.DS_Store
+-rw-r--r--   0        0        0      194 2024-05-13 00:28:09.144268 unusualwhales_python_client-4.2.1/unusualwhales/__init__.py
+-rw-r--r--   0        0        0     6148 2024-05-13 00:31:26.819597 unusualwhales_python_client-4.2.1/unusualwhales/api/.DS_Store
+-rw-r--r--   0        0        0       58 2024-05-13 00:33:10.876060 unusualwhales_python_client-4.2.1/unusualwhales/api/__init__.py
+-rw-r--r--   0        0        0     1781 2024-05-05 22:58:01.830486 unusualwhales_python_client-4.2.1/unusualwhales/api/congress/__init__.py
+-rw-r--r--   0        0        0     6907 2024-05-14 16:51:00.220751 unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_late_reports.py
+-rw-r--r--   0        0        0     6925 2024-05-14 16:50:58.400595 unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_reports.py
+-rw-r--r--   0        0        0     6916 2024-05-14 16:50:58.400580 unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_trades.py
+-rw-r--r--   0        0        0     7930 2024-05-14 16:50:58.400812 unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_trades_by_member.py
+-rw-r--r--   0        0        0      446 2024-05-05 22:58:01.829139 unusualwhales_python_client-4.2.1/unusualwhales/api/contract/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-14 16:50:58.436664 unusualwhales_python_client-4.2.1/unusualwhales/api/contract/get_price_history.py
+-rw-r--r--   0        0        0      941 2024-05-05 22:58:01.835779 unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/__init__.py
+-rw-r--r--   0        0        0     6354 2024-05-14 16:50:58.416761 unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/get_trades_by_date.py
+-rw-r--r--   0        0        0     7418 2024-05-14 16:50:58.416770 unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/get_trades_by_ticker.py
+-rw-r--r--   0        0        0     1349 2024-05-05 22:58:01.832866 unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/__init__.py
+-rw-r--r--   0        0        0     5940 2024-05-14 16:50:58.432577 unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_afterhours.py
+-rw-r--r--   0        0        0     6019 2024-05-14 16:50:58.432749 unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_premarket.py
+-rw-r--r--   0        0        0     4598 2024-05-14 16:50:58.432595 unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_ticker_earnings.py
+-rw-r--r--   0        0        0     1402 2024-05-13 00:31:49.829150 unusualwhales_python_client-4.2.1/unusualwhales/api/endpoints.py
+-rw-r--r--   0        0        0     1348 2024-05-05 22:58:01.830714 unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/__init__.py
+-rw-r--r--   0        0        0     3925 2024-05-14 16:50:58.432768 unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_holdings.py
+-rw-r--r--   0        0        0     4475 2024-05-14 16:50:58.432811 unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_info.py
+-rw-r--r--   0        0        0     4757 2024-05-14 16:50:58.432793 unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_sector_country_weights.py
+-rw-r--r--   0        0        0     4061 2024-05-14 16:50:58.432729 unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_ticker_exposure.py
+-rw-r--r--   0        0        0     2839 2024-05-05 22:58:01.823337 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/__init__.py
+-rw-r--r--   0        0        0     8854 2024-05-14 16:50:58.415793 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_contract_flow.py
+-rw-r--r--   0        0        0     4355 2024-05-14 16:50:58.415780 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_flow_by_expiry.py
+-rw-r--r--   0        0        0     4838 2024-05-14 16:50:58.415765 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_flow_by_strike.py
+-rw-r--r--   0        0        0     3170 2024-05-14 16:50:58.409858 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_full_tape.py
+-rw-r--r--   0        0        0     7360 2024-05-14 16:50:58.428050 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_order_flow.py
+-rw-r--r--   0        0        0    29084 2024-05-14 16:50:58.416171 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_ticker_order_flow.py
+-rw-r--r--   0        0        0     5766 2024-05-14 16:50:58.416153 unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_unusual_flow_alerts.py
+-rw-r--r--   0        0        0     6232 2024-05-05 22:58:01.822234 unusualwhales_python_client-4.2.1/unusualwhales/api/market/__init__.py
+-rw-r--r--   0        0        0     3744 2024-05-14 16:50:58.416725 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_economic_calendar.py
+-rw-r--r--   0        0        0     3718 2024-05-14 16:50:58.416691 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_fda_calendar.py
+-rw-r--r--   0        0        0     3693 2024-05-14 16:50:58.416675 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_holidays.py
+-rw-r--r--   0        0        0     3765 2024-05-14 16:50:58.416650 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_imbalances.py
+-rw-r--r--   0        0        0     5681 2024-05-14 16:50:58.416749 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_insider_trades.py
+-rw-r--r--   0        0        0     6188 2024-05-14 16:50:58.416738 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_market_options_volume.py
+-rw-r--r--   0        0        0    12740 2024-05-14 16:50:58.416220 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_market_tide.py
+-rw-r--r--   0        0        0     6984 2024-05-14 16:50:58.416714 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_market_tide_by_etf.py
+-rw-r--r--   0        0        0     7643 2024-05-14 16:50:58.422952 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_open_interest_change.py
+-rw-r--r--   0        0        0     4563 2024-05-14 16:50:58.416198 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_sector_stats.py
+-rw-r--r--   0        0        0     5764 2024-05-14 16:50:58.416245 unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_spike.py
+-rw-r--r--   0        0        0     1567 2024-05-05 22:58:01.834188 unusualwhales_python_client-4.2.1/unusualwhales/api/screener/__init__.py
+-rw-r--r--   0        0        0     9114 2024-05-14 16:50:58.436720 unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_analyst_ratings.py
+-rw-r--r--   0        0        0    45558 2024-05-14 16:50:58.432711 unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_option_contracts.py
+-rw-r--r--   0        0        0    64290 2024-05-14 16:50:58.432678 unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_stocks.py
+-rw-r--r--   0        0        0     1911 2024-05-05 22:58:01.823405 unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/__init__.py
+-rw-r--r--   0        0        0     4251 2024-05-14 16:50:58.422811 unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py
+-rw-r--r--   0        0        0     4796 2024-05-14 16:50:58.436634 unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_monthly_average_returns.py
+-rw-r--r--   0        0        0    13768 2024-05-14 16:50:58.422794 unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_monthly_top_performers.py
+-rw-r--r--   0        0        0     4922 2024-05-14 16:50:58.422779 unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py
+-rw-r--r--   0        0        0    17216 2024-05-05 22:58:01.830003 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/__init__.py
+-rw-r--r--   0        0        0     5755 2024-05-14 16:50:58.422764 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py
+-rw-r--r--   0        0        0     9164 2024-05-14 16:50:58.417097 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_candles.py
+-rw-r--r--   0        0        0     6193 2024-05-14 16:50:58.422567 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py
+-rw-r--r--   0        0        0    14217 2024-05-14 16:50:58.422514 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure.py
+-rw-r--r--   0        0        0     6331 2024-05-14 16:50:58.416902 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py
+-rw-r--r--   0        0        0     6399 2024-05-14 16:50:58.417006 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6901 2024-05-14 16:50:58.416987 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py
+-rw-r--r--   0        0        0     6382 2024-05-14 16:50:58.422640 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py
+-rw-r--r--   0        0        0     6223 2024-05-14 16:50:58.422594 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_info.py
+-rw-r--r--   0        0        0     4935 2024-05-14 16:50:58.422714 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_insider_trades.py
+-rw-r--r--   0        0        0     4688 2024-05-14 16:50:58.417114 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_max_pain.py
+-rw-r--r--   0        0        0    10533 2024-05-14 16:50:58.432551 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_net_premium_ticks.py
+-rw-r--r--   0        0        0     7829 2024-05-14 16:50:58.422624 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_open_interest_change.py
+-rw-r--r--   0        0        0     7388 2024-05-14 16:50:58.417081 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_chains.py
+-rw-r--r--   0        0        0    10925 2024-05-14 16:50:58.422611 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_contracts.py
+-rw-r--r--   0        0        0     6049 2024-05-14 16:50:58.422749 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_volume_by_price_level.py
+-rw-r--r--   0        0        0     5952 2024-05-14 16:50:58.422542 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_options_volume.py
+-rw-r--r--   0        0        0     9072 2024-05-14 16:50:58.436939 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_risk_reversal_skew.py
+-rw-r--r--   0        0        0     4926 2024-05-14 16:50:58.417023 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_sector_tickers.py
+-rw-r--r--   0        0        0    14204 2024-05-14 16:50:58.417056 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_spot_exposures.py
+-rw-r--r--   0        0        0    14533 2024-05-14 16:50:58.417039 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py
+-rw-r--r--   0        0        0     6448 2024-05-14 16:50:58.416964 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volatility_term_structure.py
+-rw-r--r--   0        0        0     7214 2024-05-14 16:50:58.422733 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volume_by_price_level.py
+-rw-r--r--   0        0        0     6097 2024-05-14 16:50:58.423065 unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py
+-rw-r--r--   0        0        0     7122 2024-05-13 00:28:35.664213 unusualwhales_python_client-4.2.1/unusualwhales/client.py
+-rw-r--r--   0        0        0      546 2024-05-05 22:58:01.816143 unusualwhales_python_client-4.2.1/unusualwhales/errors.py
+-rw-r--r--   0        0        0    10021 2024-05-05 22:58:01.822073 unusualwhales_python_client-4.2.1/unusualwhales/models/__init__.py
+-rw-r--r--   0        0        0     2227 2024-05-05 22:58:01.823494 unusualwhales_python_client-4.2.1/unusualwhales/models/analalyst_rating_results.py
+-rw-r--r--   0        0        0      262 2024-05-05 22:58:01.779003 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_action.py
+-rw-r--r--   0        0        0      267 2024-05-05 22:58:01.779493 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_field_action.py
+-rw-r--r--   0        0        0      183 2024-05-05 22:58:01.758542 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_field_recommendation.py
+-rw-r--r--   0        0        0     6697 2024-05-05 22:58:01.820117 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_rating.py
+-rw-r--r--   0        0        0      178 2024-05-05 22:58:01.765008 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_recommendation.py
+-rw-r--r--   0        0        0      428 2024-05-05 22:58:01.775125 unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_sector.py
+-rw-r--r--   0        0        0     5399 2024-05-05 22:58:01.821958 unusualwhales_python_client-4.2.1/unusualwhales/models/candle_data.py
+-rw-r--r--   0        0        0     2098 2024-05-05 22:58:01.833898 unusualwhales_python_client-4.2.1/unusualwhales/models/candle_data_results.py
+-rw-r--r--   0        0        0      251 2024-05-05 22:58:01.780257 unusualwhales_python_client-4.2.1/unusualwhales/models/candle_size.py
+-rw-r--r--   0        0        0     5755 2024-05-05 22:58:01.816560 unusualwhales_python_client-4.2.1/unusualwhales/models/congressional_trade_report.py
+-rw-r--r--   0        0        0     2308 2024-05-05 22:58:01.833569 unusualwhales_python_client-4.2.1/unusualwhales/models/congressional_trade_report_results.py
+-rw-r--r--   0        0        0     5235 2024-05-05 22:58:01.830332 unusualwhales_python_client-4.2.1/unusualwhales/models/country_sector_exposure.py
+-rw-r--r--   0        0        0     3869 2024-05-05 22:58:01.828297 unusualwhales_python_client-4.2.1/unusualwhales/models/daily_market_tide.py
+-rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.833609 unusualwhales_python_client-4.2.1/unusualwhales/models/daily_market_tide_response.py
+-rw-r--r--   0        0        0     9770 2024-05-05 22:58:01.832534 unusualwhales_python_client-4.2.1/unusualwhales/models/darkpool_trade.py
+-rw-r--r--   0        0        0     3375 2024-05-05 22:58:01.818843 unusualwhales_python_client-4.2.1/unusualwhales/models/darkpool_trade_response.py
+-rw-r--r--   0        0        0     8924 2024-05-05 22:58:01.834330 unusualwhales_python_client-4.2.1/unusualwhales/models/earnings.py
+-rw-r--r--   0        0        0     2069 2024-05-05 22:58:01.833907 unusualwhales_python_client-4.2.1/unusualwhales/models/earnings_results.py
+-rw-r--r--   0        0        0     4185 2024-05-05 22:58:01.823207 unusualwhales_python_client-4.2.1/unusualwhales/models/economic_calendar.py
+-rw-r--r--   0        0        0      189 2024-05-05 22:58:01.783710 unusualwhales_python_client-4.2.1/unusualwhales/models/economic_type.py
+-rw-r--r--   0        0        0     2673 2024-05-05 22:58:01.820875 unusualwhales_python_client-4.2.1/unusualwhales/models/error_message.py
+-rw-r--r--   0        0        0     1779 2024-05-05 22:58:01.822650 unusualwhales_python_client-4.2.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
+-rw-r--r--   0        0        0     2063 2024-05-05 22:58:01.825400 unusualwhales_python_client-4.2.1/unusualwhales/models/etf_countries_item.py
+-rw-r--r--   0        0        0     3171 2024-05-05 22:58:01.822868 unusualwhales_python_client-4.2.1/unusualwhales/models/etf_info.py
+-rw-r--r--   0        0        0     6423 2024-05-05 22:58:01.832037 unusualwhales_python_client-4.2.1/unusualwhales/models/etf_info_data.py
+-rw-r--r--   0        0        0     2044 2024-05-05 22:58:01.818548 unusualwhales_python_client-4.2.1/unusualwhales/models/etf_sectors_item.py
+-rw-r--r--   0        0        0     2953 2024-05-05 22:58:01.832447 unusualwhales_python_client-4.2.1/unusualwhales/models/expiry_breakdown.py
+-rw-r--r--   0        0        0     2248 2024-05-05 22:58:01.825125 unusualwhales_python_client-4.2.1/unusualwhales/models/expiry_breakdown_result.py
+-rw-r--r--   0        0        0     5086 2024-05-05 22:58:01.817753 unusualwhales_python_client-4.2.1/unusualwhales/models/fda_calendar.py
+-rw-r--r--   0        0        0    10635 2024-05-05 22:58:01.817394 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert.py
+-rw-r--r--   0        0        0     2086 2024-05-05 22:58:01.816655 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert_results.py
+-rw-r--r--   0        0        0      590 2024-05-05 22:58:01.780015 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert_rule.py
+-rw-r--r--   0        0        0    12800 2024-05-05 22:58:01.827106 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_expiry.py
+-rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.827194 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_expiry_results.py
+-rw-r--r--   0        0        0    12688 2024-05-05 22:58:01.819326 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_strike.py
+-rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.830018 unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_strike_results.py
+-rw-r--r--   0        0        0     6320 2024-05-05 22:58:01.816924 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure.py
+-rw-r--r--   0        0        0     6349 2024-05-05 22:58:01.822486 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6808 2024-05-05 22:58:01.831535 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py
+-rw-r--r--   0        0        0     2358 2024-05-05 22:58:01.821530 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py
+-rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.827851 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_results.py
+-rw-r--r--   0        0        0     2134 2024-05-05 22:58:01.816486 unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_results.py
+-rw-r--r--   0        0        0     9046 2024-05-05 22:58:01.826947 unusualwhales_python_client-4.2.1/unusualwhales/models/greeks.py
+-rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.829764 unusualwhales_python_client-4.2.1/unusualwhales/models/historical_risk_reversal_skew.py
+-rw-r--r--   0        0        0     2300 2024-05-05 22:58:01.822832 unusualwhales_python_client-4.2.1/unusualwhales/models/historical_risk_reversal_skew_results.py
+-rw-r--r--   0        0        0     8935 2024-05-05 22:58:01.817484 unusualwhales_python_client-4.2.1/unusualwhales/models/holdings.py
+-rw-r--r--   0        0        0     2648 2024-05-05 22:58:01.821969 unusualwhales_python_client-4.2.1/unusualwhales/models/holdings_response.py
+-rw-r--r--   0        0        0     4229 2024-05-05 22:58:01.818954 unusualwhales_python_client-4.2.1/unusualwhales/models/imbalances_volume.py
+-rw-r--r--   0        0        0     4234 2024-05-05 22:58:01.831021 unusualwhales_python_client-4.2.1/unusualwhales/models/implied_volatility_term_structure.py
+-rw-r--r--   0        0        0     2348 2024-05-05 22:58:01.822055 unusualwhales_python_client-4.2.1/unusualwhales/models/implied_volatility_term_structure_results.py
+-rw-r--r--   0        0        0     3185 2024-05-05 22:58:01.834435 unusualwhales_python_client-4.2.1/unusualwhales/models/insider_statistic.py
+-rw-r--r--   0        0        0     2770 2024-05-05 22:58:01.816314 unusualwhales_python_client-4.2.1/unusualwhales/models/insider_statistics.py
+-rw-r--r--   0        0        0      190 2024-05-05 22:58:01.766259 unusualwhales_python_client-4.2.1/unusualwhales/models/insider_trades_member_type.py
+-rw-r--r--   0        0        0      345 2024-05-05 22:58:01.775861 unusualwhales_python_client-4.2.1/unusualwhales/models/insider_trades_transaction_type.py
+-rw-r--r--   0        0        0      164 2024-05-05 22:58:01.778813 unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_imbalance_event.py
+-rw-r--r--   0        0        0      165 2024-05-05 22:58:01.783423 unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_imbalance_side.py
+-rw-r--r--   0        0        0      213 2024-05-05 22:58:01.776228 unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_imbalance_type.py
+-rw-r--r--   0        0        0      168 2024-05-05 22:58:01.773079 unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_market_time.py
+-rw-r--r--   0        0        0      528 2024-05-05 22:58:01.774624 unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_sector.py
+-rw-r--r--   0        0        0     4512 2024-05-05 22:58:01.834484 unusualwhales_python_client-4.2.1/unusualwhales/models/market_holidays.py
+-rw-r--r--   0        0        0     3378 2024-05-05 22:58:01.831296 unusualwhales_python_client-4.2.1/unusualwhales/models/market_options_volume.py
+-rw-r--r--   0        0        0     1710 2024-05-05 22:58:01.827677 unusualwhales_python_client-4.2.1/unusualwhales/models/market_sector_ticker_results.py
+-rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.830420 unusualwhales_python_client-4.2.1/unusualwhales/models/max_pain.py
+-rw-r--r--   0        0        0     2159 2024-05-05 22:58:01.833744 unusualwhales_python_client-4.2.1/unusualwhales/models/max_pain_results.py
+-rw-r--r--   0        0        0     3421 2024-05-05 22:58:01.833406 unusualwhales_python_client-4.2.1/unusualwhales/models/net_prem_tick.py
+-rw-r--r--   0        0        0     4303 2024-05-05 22:58:01.828862 unusualwhales_python_client-4.2.1/unusualwhales/models/net_prem_tick_results.py
+-rw-r--r--   0        0        0     2494 2024-05-05 22:58:01.821207 unusualwhales_python_client-4.2.1/unusualwhales/models/off_lit_price_level.py
+-rw-r--r--   0        0        0     2270 2024-05-05 22:58:01.816343 unusualwhales_python_client-4.2.1/unusualwhales/models/off_lit_price_level_results.py
+-rw-r--r--   0        0        0    11261 2024-05-05 22:58:01.823477 unusualwhales_python_client-4.2.1/unusualwhales/models/oi_change.py
+-rw-r--r--   0        0        0     2101 2024-05-05 22:58:01.828752 unusualwhales_python_client-4.2.1/unusualwhales/models/oi_change_results.py
+-rw-r--r--   0        0        0    10954 2024-05-05 22:58:01.817830 unusualwhales_python_client-4.2.1/unusualwhales/models/option_chain_contract.py
+-rw-r--r--   0        0        0     2316 2024-05-05 22:58:01.818322 unusualwhales_python_client-4.2.1/unusualwhales/models/option_chain_contract_results.py
+-rw-r--r--   0        0        0     2187 2024-05-05 22:58:01.818071 unusualwhales_python_client-4.2.1/unusualwhales/models/option_chains_results.py
+-rw-r--r--   0        0        0    11275 2024-05-05 22:58:01.818618 unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract.py
+-rw-r--r--   0        0        0     2251 2024-05-05 22:58:01.829762 unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_results.py
+-rw-r--r--   0        0        0    14866 2024-05-05 22:58:01.824112 unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_screener_item.py
+-rw-r--r--   0        0        0     2375 2024-05-05 22:58:01.831061 unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_screener_results.py
+-rw-r--r--   0        0        0      157 2024-05-05 22:58:01.768374 unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_type.py
+-rw-r--r--   0        0        0     2522 2024-05-05 22:58:01.825820 unusualwhales_python_client-4.2.1/unusualwhales/models/option_price_level.py
+-rw-r--r--   0        0        0     2283 2024-05-05 22:58:01.827958 unusualwhales_python_client-4.2.1/unusualwhales/models/option_price_level_results.py
+-rw-r--r--   0        0        0      149 2024-05-05 22:58:01.770159 unusualwhales_python_client-4.2.1/unusualwhales/models/option_type.py
+-rw-r--r--   0        0        0      153 2024-05-05 22:58:01.771290 unusualwhales_python_client-4.2.1/unusualwhales/models/order_direction.py
+-rw-r--r--   0        0        0      949 2024-05-05 22:58:01.774812 unusualwhales_python_client-4.2.1/unusualwhales/models/screener_contract_order_by_field.py
+-rw-r--r--   0        0        0     1401 2024-05-05 22:58:01.780126 unusualwhales_python_client-4.2.1/unusualwhales/models/screener_order_by_field.py
+-rw-r--r--   0        0        0     5330 2024-05-05 22:58:01.832188 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_market.py
+-rw-r--r--   0        0        0     2245 2024-05-05 22:58:01.817561 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_market_results.py
+-rw-r--r--   0        0        0     4802 2024-05-05 22:58:01.826952 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_monthly.py
+-rw-r--r--   0        0        0     2864 2024-05-05 22:58:01.816371 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_monthly_results.py
+-rw-r--r--   0        0        0      412 2024-05-05 22:58:01.784552 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_performance_order_by.py
+-rw-r--r--   0        0        0     6634 2024-05-05 22:58:01.820876 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_performers.py
+-rw-r--r--   0        0        0     2884 2024-05-05 22:58:01.822592 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_performers_results.py
+-rw-r--r--   0        0        0     2957 2024-05-05 22:58:01.827974 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_year_month.py
+-rw-r--r--   0        0        0     3159 2024-05-05 22:58:01.828370 unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_year_month_results.py
+-rw-r--r--   0        0        0      515 2024-05-05 22:58:01.783541 unusualwhales_python_client-4.2.1/unusualwhales/models/sector.py
+-rw-r--r--   0        0        0    10830 2024-05-05 22:58:01.830188 unusualwhales_python_client-4.2.1/unusualwhales/models/sector_etf.py
+-rw-r--r--   0        0        0     2890 2024-05-05 22:58:01.823726 unusualwhales_python_client-4.2.1/unusualwhales/models/sector_etf_results.py
+-rw-r--r--   0        0        0      173 2024-05-05 22:58:01.769865 unusualwhales_python_client-4.2.1/unusualwhales/models/side.py
+-rw-r--r--   0        0        0      206 2024-05-05 22:58:01.776708 unusualwhales_python_client-4.2.1/unusualwhales/models/single_issue_type.py
+-rw-r--r--   0        0        0      343 2024-05-05 22:58:01.762014 unusualwhales_python_client-4.2.1/unusualwhales/models/single_month_number.py
+-rw-r--r--   0        0        0      521 2024-05-05 22:58:01.779594 unusualwhales_python_client-4.2.1/unusualwhales/models/single_sector.py
+-rw-r--r--   0        0        0      334 2024-05-05 22:58:01.769228 unusualwhales_python_client-4.2.1/unusualwhales/models/single_trade_external_hour_sold_code.py
+-rw-r--r--   0        0        0      312 2024-05-05 22:58:01.761864 unusualwhales_python_client-4.2.1/unusualwhales/models/single_trade_sale_cond_code.py
+-rw-r--r--   0        0        0      304 2024-05-05 22:58:01.781307 unusualwhales_python_client-4.2.1/unusualwhales/models/single_trade_settlement.py
+-rw-r--r--   0        0        0      275 2024-05-05 22:58:01.752668 unusualwhales_python_client-4.2.1/unusualwhales/models/single_trade_trade_code.py
+-rw-r--r--   0        0        0     2304 2024-05-05 22:58:01.832942 unusualwhales_python_client-4.2.1/unusualwhales/models/spike_value.py
+-rw-r--r--   0        0        0     7769 2024-05-05 22:58:01.832634 unusualwhales_python_client-4.2.1/unusualwhales/models/spot_gex_exposures_per_1_min.py
+-rw-r--r--   0        0        0     2274 2024-05-05 22:58:01.833460 unusualwhales_python_client-4.2.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py
+-rw-r--r--   0        0        0     8339 2024-05-05 22:58:01.833587 unusualwhales_python_client-4.2.1/unusualwhales/models/spot_greek_exposures_by_strike.py
+-rw-r--r--   0        0        0     2305 2024-05-05 22:58:01.817337 unusualwhales_python_client-4.2.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py
+-rw-r--r--   0        0        0      202 2024-05-05 22:58:01.756301 unusualwhales_python_client-4.2.1/unusualwhales/models/stock_earnings_time.py
+-rw-r--r--   0        0        0      205 2024-05-05 22:58:01.779639 unusualwhales_python_client-4.2.1/unusualwhales/models/stock_issue_type.py
+-rw-r--r--   0        0        0    24207 2024-05-05 22:58:01.822193 unusualwhales_python_client-4.2.1/unusualwhales/models/stock_screener_response.py
+-rw-r--r--   0        0        0     2280 2024-05-05 22:58:01.823614 unusualwhales_python_client-4.2.1/unusualwhales/models/stock_screener_response_results.py
+-rw-r--r--   0        0        0     8648 2024-05-05 22:58:01.828620 unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_info.py
+-rw-r--r--   0        0        0     2636 2024-05-05 22:58:01.831049 unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_info_results.py
+-rw-r--r--   0        0        0    11609 2024-05-05 22:58:01.832705 unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_options_volume.py
+-rw-r--r--   0        0        0     2436 2024-05-05 22:58:01.828948 unusualwhales_python_client-4.2.1/unusualwhales/models/volume_oi_per_expiry.py
+-rw-r--r--   0        0        0     2233 2024-05-05 22:58:01.816470 unusualwhales_python_client-4.2.1/unusualwhales/models/volume_oi_per_expiry_results.py
+-rw-r--r--   0        0        0       25 2024-05-05 22:58:01.341037 unusualwhales_python_client-4.2.1/unusualwhales/py.typed
+-rw-r--r--   0        0        0      985 2024-05-05 22:58:01.827475 unusualwhales_python_client-4.2.1/unusualwhales/types.py
+-rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 unusualwhales_python_client-4.2.1/PKG-INFO
```

### Comparing `unusualwhales_python_client-4.1.1/LICENSE` & `unusualwhales_python_client-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/README.md` & `unusualwhales_python_client-4.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 ## Example Implementation
 ```python
 import os
 import decimal
 from dotenv import load_dotenv
-from unusualwhales import UnusualWhalesClient, UnusualWhalesApi
+from unusualwhales import UnusualWhalesClient, 
 
 from unusualwhales.models import OffLitPriceLevelResults, OffLitPriceLevel
 from unusualwhales.api.stock import get_volume_by_price_level
 
 load_dotenv('.env')
 UW_API_TOKEN = os.environ.get("UW_API_TOKEN", None)
```

### Comparing `unusualwhales_python_client-4.1.1/pyproject.toml` & `unusualwhales_python_client-4.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unusualwhales-python-client"
-version = "4.1.1"
+version = "4.2.1"
 description = "A client library for accessing Unusual Whales API"
 authors = ["Mac Anderson <mac@macanderson.com>"]
 readme = "README.md"
 packages = [{ include = "unusualwhales" }]
 include = ["unusualwhales/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/.DS_Store` & `unusualwhales_python_client-4.2.1/unusualwhales/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/.DS_Store` & `unusualwhales_python_client-4.2.1/unusualwhales/api/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/congress/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/congress/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_late_reports.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_trades.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.congressional_trade_report_results import CongressionalTradeReportResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -22,23 +22,23 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/congress/late-reports",
+        "url": "/api/congress/recent-trades",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CongressionalTradeReportResults.from_dict(response.json())
 
@@ -53,35 +53,34 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Late Reports
+    """Recent Congressional Trades
 
-     Returns the recent late reports by congress members.
-    If a date is given, will only return recent late reports, which's report date is <= the given input
-    date.
+     Returns the latest transacted trades by congress members.
+    If a date is given, will only return reports, which's transaction date is <= the given input date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -104,23 +103,22 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Late Reports
+    """Recent Congressional Trades
 
-     Returns the recent late reports by congress members.
-    If a date is given, will only return recent late reports, which's report date is <= the given input
-    date.
+     Returns the latest transacted trades by congress members.
+    If a date is given, will only return reports, which's transaction date is <= the given input date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -138,23 +136,22 @@
         limit=limit,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Late Reports
+    """Recent Congressional Trades
 
-     Returns the recent late reports by congress members.
-    If a date is given, will only return recent late reports, which's report date is <= the given input
-    date.
+     Returns the latest transacted trades by congress members.
+    If a date is given, will only return reports, which's transaction date is <= the given input date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -175,23 +172,22 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Late Reports
+    """Recent Congressional Trades
 
-     Returns the recent late reports by congress members.
-    If a date is given, will only return recent late reports, which's report date is <= the given input
-    date.
+     Returns the latest transacted trades by congress members.
+    If a date is given, will only return reports, which's transaction date is <= the given input date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_reports.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.congressional_trade_report_results import CongressionalTradeReportResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -30,15 +30,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CongressionalTradeReportResults.from_dict(response.json())
 
@@ -53,27 +53,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reported Congress Trades
 
      Returns the latest reported trades by congress members.
     If a date is given, will only return reports, which's transaction date is <= the given input date.
@@ -103,15 +103,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reported Congress Trades
 
      Returns the latest reported trades by congress members.
     If a date is given, will only return reports, which's transaction date is <= the given input date.
@@ -136,15 +136,15 @@
         limit=limit,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reported Congress Trades
 
      Returns the latest reported trades by congress members.
     If a date is given, will only return reports, which's transaction date is <= the given input date.
@@ -172,15 +172,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reported Congress Trades
 
      Returns the latest reported trades by congress members.
     If a date is given, will only return reports, which's transaction date is <= the given input date.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_trades.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_late_reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.congressional_trade_report_results import CongressionalTradeReportResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -22,23 +22,23 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/congress/recent-trades",
+        "url": "/api/congress/late-reports",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CongressionalTradeReportResults.from_dict(response.json())
 
@@ -53,34 +53,35 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Congressional Trades
+    """Recent Late Reports
 
-     Returns the latest transacted trades by congress members.
-    If a date is given, will only return reports, which's transaction date is <= the given input date.
+     Returns the recent late reports by congress members.
+    If a date is given, will only return recent late reports, which's report date is <= the given input
+    date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -103,22 +104,23 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Congressional Trades
+    """Recent Late Reports
 
-     Returns the latest transacted trades by congress members.
-    If a date is given, will only return reports, which's transaction date is <= the given input date.
+     Returns the recent late reports by congress members.
+    If a date is given, will only return recent late reports, which's report date is <= the given input
+    date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -136,22 +138,23 @@
         limit=limit,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Congressional Trades
+    """Recent Late Reports
 
-     Returns the latest transacted trades by congress members.
-    If a date is given, will only return reports, which's transaction date is <= the given input date.
+     Returns the recent late reports by congress members.
+    If a date is given, will only return recent late reports, which's report date is <= the given input
+    date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
@@ -172,22 +175,23 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
-    """Recent Congressional Trades
+    """Recent Late Reports
 
-     Returns the latest transacted trades by congress members.
-    If a date is given, will only return reports, which's transaction date is <= the given input date.
+     Returns the recent late reports by congress members.
+    If a date is given, will only return recent late reports, which's report date is <= the given input
+    date.
 
     Args:
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/congress/get_trades_by_member.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/congress/get_trades_by_member.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.congressional_trade_report_results import CongressionalTradeReportResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -33,15 +33,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CongressionalTradeReportResults.from_dict(response.json())
 
@@ -56,27 +56,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
     name: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reports By Trader
 
      Returns the recent reports by the given congress member.
@@ -112,15 +112,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
     name: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reports By Trader
 
      Returns the recent reports by the given congress member.
@@ -151,15 +151,15 @@
         date=date,
         name=name,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
     name: Union[Unset, str] = UNSET,
 ) -> Response[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reports By Trader
 
      Returns the recent reports by the given congress member.
@@ -193,15 +193,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
     name: Union[Unset, str] = UNSET,
 ) -> Optional[Union[CongressionalTradeReportResults, ErrorMessage, str]]:
     """Recent Reports By Trader
 
      Returns the recent reports by the given congress member.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/contract/get_price_history.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/contract/get_price_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.option_chain_contract_results import OptionChainContractResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     id: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = OptionChainContractResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     """Price history for the given option contract
 
      Historic EOD Stats for the given option contract
 
     Args:
@@ -99,15 +99,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     """Price history for the given option contract
 
      Historic EOD Stats for the given option contract
 
     Args:
@@ -129,15 +129,15 @@
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     """Price history for the given option contract
 
      Historic EOD Stats for the given option contract
 
     Args:
@@ -162,15 +162,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     """Price history for the given option contract
 
      Historic EOD Stats for the given option contract
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/get_trades_by_date.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/get_trades_by_date.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.darkpool_trade_response import DarkpoolTradeResponse
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -30,15 +30,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = DarkpoolTradeResponse.from_dict(response.json())
 
@@ -53,27 +53,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given date. All Symbols.
 
      Returns the latest darkpool trades.
 
@@ -102,15 +102,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given date. All Symbols.
 
      Returns the latest darkpool trades.
 
@@ -134,15 +134,15 @@
         limit=limit,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given date. All Symbols.
 
      Returns the latest darkpool trades.
 
@@ -169,15 +169,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given date. All Symbols.
 
      Returns the latest darkpool trades.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/darkpool/get_trades_by_ticker.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/darkpool/get_trades_by_ticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.darkpool_trade_response import DarkpoolTradeResponse
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -31,15 +31,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = DarkpoolTradeResponse.from_dict(response.json())
 
@@ -54,28 +54,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given ticker and date
 
      Returns the darkpool trades for the given ticker on a given day.
     Date must be the current or a past date. If no date is given, returns data for the current/last
@@ -109,15 +109,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given ticker and date
 
      Returns the darkpool trades for the given ticker on a given day.
     Date must be the current or a past date. If no date is given, returns data for the current/last
@@ -146,15 +146,15 @@
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given ticker and date
 
      Returns the darkpool trades for the given ticker on a given day.
     Date must be the current or a past date. If no date is given, returns data for the current/last
@@ -186,15 +186,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[DarkpoolTradeResponse, ErrorMessage, str]]:
     """Darkpool trades for a given ticker and date
 
      Returns the darkpool trades for the given ticker on a given day.
     Date must be the current or a past date. If no date is given, returns data for the current/last
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_afterhours.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_afterhours.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.earnings_results import EarningsResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -27,15 +27,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = EarningsResults.from_dict(response.json())
 
@@ -50,27 +50,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     """Afterhours
 
      Returns the next upcoming afterhours earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -97,15 +97,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     """Afterhours
 
      Returns the next upcoming afterhours earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -127,15 +127,15 @@
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     """Afterhours
 
      Returns the next upcoming afterhours earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -160,15 +160,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     """Afterhours
 
      Returns the next upcoming afterhours earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_premarket.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_premarket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.earnings_results import EarningsResults
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -27,15 +27,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = EarningsResults.from_dict(response.json())
 
@@ -50,27 +50,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     """Next Premarket Earnings by Date
 
      Returns the next upcoming premarket earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -97,15 +97,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     """Next Premarket Earnings by Date
 
      Returns the next upcoming premarket earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -127,15 +127,15 @@
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     """Next Premarket Earnings by Date
 
      Returns the next upcoming premarket earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -160,15 +160,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     """Next Premarket Earnings by Date
 
      Returns the next upcoming premarket earnings for the given date.
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/earnings/get_ticker_earnings.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_monthly_average_returns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.earnings_results import EarningsResults
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
+from ...models.seasonality_monthly_results import SeasonalityMonthlyResults
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/earnings/{ticker}",
+        "url": f"/api/seasonality/{ticker}/monthly",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = EarningsResults.from_dict(response.json())
+        response_200 = SeasonalityMonthlyResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -41,42 +41,42 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[EarningsResults, ErrorMessage, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[EarningsResults, ErrorMessage, str]]:
-    """Past Ticker Earnings
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    """Average return per month
 
-     Returns the past earnings for the given ticker.
+     Returns the average return by month for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[EarningsResults, ErrorMessage, str]]
+        Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
     )
 
     response = client.get_httpx_client().request(
@@ -85,84 +85,84 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
-    """Past Ticker Earnings
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    """Average return per month
 
-     Returns the past earnings for the given ticker.
+     Returns the average return by month for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[EarningsResults, ErrorMessage, str]
+        Union[ErrorMessage, SeasonalityMonthlyResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[EarningsResults, ErrorMessage, str]]:
-    """Past Ticker Earnings
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    """Average return per month
 
-     Returns the past earnings for the given ticker.
+     Returns the average return by month for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[EarningsResults, ErrorMessage, str]]
+        Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
-    """Past Ticker Earnings
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    """Average return per month
 
-     Returns the past earnings for the given ticker.
+     Returns the average return by month for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[EarningsResults, ErrorMessage, str]
+        Union[ErrorMessage, SeasonalityMonthlyResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
         )
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/endpoints.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_holdings.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_holdings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.holdings_response import HoldingsResponse
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
 ) -> Dict[str, Any]:
@@ -17,15 +17,15 @@
         "url": f"/api/etfs/{ticker}/holdings",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[HoldingsResponse]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = HoldingsResponse.from_dict(response.json())
 
@@ -33,28 +33,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[HoldingsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[HoldingsResponse]:
     """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -77,15 +77,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[HoldingsResponse]:
     """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -103,15 +103,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[HoldingsResponse]:
     """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -132,15 +132,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[HoldingsResponse]:
     """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_info.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.etf_info import EtfInfo
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
@@ -18,15 +18,15 @@
         "url": f"/api/etfs/{ticker}/info",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, EtfInfo, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = EtfInfo.from_dict(response.json())
 
@@ -41,28 +41,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, EtfInfo, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, EtfInfo, str]]:
     """Information
 
      Returns the information about the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -85,15 +85,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, EtfInfo, str]]:
     """Information
 
      Returns the information about the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -111,15 +111,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, EtfInfo, str]]:
     """Information
 
      Returns the information about the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -140,15 +140,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, EtfInfo, str]]:
     """Information
 
      Returns the information about the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_sector_country_weights.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_sector_country_weights.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.country_sector_exposure import CountrySectorExposure
 from ...models.error_message import ErrorMessage
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
@@ -18,15 +18,15 @@
         "url": f"/api/etfs/{ticker}/weights",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CountrySectorExposure, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CountrySectorExposure.from_dict(response.json())
 
@@ -41,28 +41,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CountrySectorExposure, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[CountrySectorExposure, ErrorMessage, str]]:
     """Sector & Country weights
 
      Returns the sector & country weights for the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -85,15 +85,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[CountrySectorExposure, ErrorMessage, str]]:
     """Sector & Country weights
 
      Returns the sector & country weights for the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -111,15 +111,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[CountrySectorExposure, ErrorMessage, str]]:
     """Sector & Country weights
 
      Returns the sector & country weights for the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -140,15 +140,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[CountrySectorExposure, ErrorMessage, str]]:
     """Sector & Country weights
 
      Returns the sector & country weights for the given ETF ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/etfs/get_ticker_exposure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/etfs/get_ticker_exposure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.holdings_response import HoldingsResponse
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
 ) -> Dict[str, Any]:
@@ -17,15 +17,15 @@
         "url": f"/api/etfs/{ticker}/exposure",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[HoldingsResponse]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = HoldingsResponse.from_dict(response.json())
 
@@ -33,28 +33,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[HoldingsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[HoldingsResponse]:
     """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -77,15 +77,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[HoldingsResponse]:
     """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -103,15 +103,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[HoldingsResponse]:
     """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -132,15 +132,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[HoldingsResponse]:
     """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_contract_flow.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_contract_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.flow_per_expiry import FlowPerExpiry
 from ...models.side import Side
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
@@ -42,15 +42,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowPerExpiry.from_dict(response.json())
 
@@ -65,28 +65,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
     """Get Option Order Flow for a Given Contract
 
@@ -126,15 +126,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
     """Get Option Order Flow for a Given Contract
 
@@ -169,15 +169,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
     """Get Option Order Flow for a Given Contract
 
@@ -215,15 +215,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
     """Get Option Order Flow for a Given Contract
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_flow_by_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_flow_by_expiry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.flow_per_expiry_results import FlowPerExpiryResults
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
 ) -> Dict[str, Any]:
@@ -17,15 +17,15 @@
         "url": f"/api/stock/{ticker}/flow-per-expiry",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[FlowPerExpiryResults]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowPerExpiryResults.from_dict(response.json())
 
@@ -33,28 +33,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[FlowPerExpiryResults]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[FlowPerExpiryResults]:
     """Option Order Flow for a Ticker Grouped by Expiry
 
      Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -77,15 +77,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[FlowPerExpiryResults]:
     """Option Order Flow for a Ticker Grouped by Expiry
 
      Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -103,15 +103,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[FlowPerExpiryResults]:
     """Option Order Flow for a Ticker Grouped by Expiry
 
      Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -132,15 +132,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[FlowPerExpiryResults]:
     """Option Order Flow for a Ticker Grouped by Expiry
 
      Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_flow_by_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_flow_by_strike.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.flow_per_strike_results import FlowPerStrikeResults
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
@@ -18,15 +18,15 @@
         "url": f"/api/stock/{ticker}/flow-per-strike",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowPerStrikeResults.from_dict(response.json())
 
@@ -41,28 +41,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     """Option Order Flow for a Ticker Grouped By Strike
 
      Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -85,15 +85,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     """Option Order Flow for a Ticker Grouped By Strike
 
      Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -111,15 +111,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     """Option Order Flow for a Ticker Grouped By Strike
 
      Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
@@ -140,15 +140,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, FlowPerStrikeResults, str]]:
     """Option Order Flow for a Ticker Grouped By Strike
 
      Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_full_tape.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_full_tape.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...types import Response
 
 
 def _get_kwargs(
     date: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
         "url": f"/api/option-trades/full-tape/{date}",
     }
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: UnusualWhalesClient, response: httpx.Response) -> Optional[Any]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         return None
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: UnusualWhalesClient, response: httpx.Response) -> Response[Any]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     date: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Any]:
     """Full Tape all trades and statuses for all option orders by date
 
      Download the full tape of data for a given trading date.
 
     NOTICE:
     This endpoint is not included by default in your access.
@@ -76,15 +76,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     date: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Any]:
     """Full Tape all trades and statuses for all option orders by date
 
      Download the full tape of data for a given trading date.
 
     NOTICE:
     This endpoint is not included by default in your access.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_order_flow.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_order_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.flow_per_expiry_results import FlowPerExpiryResults
 from ...models.side import Side
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
@@ -36,15 +36,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowPerExpiryResults.from_dict(response.json())
 
@@ -59,28 +59,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
@@ -112,15 +112,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
@@ -147,15 +147,15 @@
         min_premium=min_premium,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
@@ -185,15 +185,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiryResults, str]]:
     """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_ticker_order_flow.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_ticker_order_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.flow_alert import FlowAlert
 from ...models.flow_alert_rule import FlowAlertRule
 from ...models.single_issue_type import SingleIssueType
 from ...types import UNSET, Response, Unset
 
 
@@ -112,15 +112,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, FlowAlert, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowAlert.from_dict(response.json())
 
@@ -135,27 +135,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, FlowAlert, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     max_premium: Union[Unset, int] = UNSET,
     min_size: Union[Unset, int] = UNSET,
     max_size: Union[Unset, int] = UNSET,
     min_volume: Union[Unset, int] = UNSET,
     max_volume: Union[Unset, int] = UNSET,
@@ -278,15 +278,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     max_premium: Union[Unset, int] = UNSET,
     min_size: Union[Unset, int] = UNSET,
     max_size: Union[Unset, int] = UNSET,
     min_volume: Union[Unset, int] = UNSET,
     max_volume: Union[Unset, int] = UNSET,
@@ -404,15 +404,15 @@
         max_dte=max_dte,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     max_premium: Union[Unset, int] = UNSET,
     min_size: Union[Unset, int] = UNSET,
     max_size: Union[Unset, int] = UNSET,
     min_volume: Union[Unset, int] = UNSET,
     max_volume: Union[Unset, int] = UNSET,
@@ -533,15 +533,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     max_premium: Union[Unset, int] = UNSET,
     min_size: Union[Unset, int] = UNSET,
     max_size: Union[Unset, int] = UNSET,
     min_volume: Union[Unset, int] = UNSET,
     max_volume: Union[Unset, int] = UNSET,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/flow/get_unusual_flow_alerts.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/flow/get_unusual_flow_alerts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.flow_alert_results import FlowAlertResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, FlowAlertResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FlowAlertResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, FlowAlertResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlertResults, str]]:
     """Unusual Whales Alerts for a Ticker
 
      Returns the latest unusual whales flow alerts for the given ticker.
 
     Args:
@@ -99,15 +99,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlertResults, str]]:
     """Unusual Whales Alerts for a Ticker
 
      Returns the latest unusual whales flow alerts for the given ticker.
 
     Args:
@@ -129,15 +129,15 @@
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlertResults, str]]:
     """Unusual Whales Alerts for a Ticker
 
      Returns the latest unusual whales flow alerts for the given ticker.
 
     Args:
@@ -162,15 +162,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlertResults, str]]:
     """Unusual Whales Alerts for a Ticker
 
      Returns the latest unusual whales flow alerts for the given ticker.
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_economic_calendar.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_economic_calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.economic_calendar import EconomicCalendar
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
         "url": "/api/market/economic-calendar",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[EconomicCalendar, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = EconomicCalendar.from_dict(response.json())
 
@@ -34,27 +34,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[EconomicCalendar, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[EconomicCalendar, str]]:
     """Economic calendar
 
      Returns the economic calendar.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -71,15 +71,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[EconomicCalendar, str]]:
     """Economic calendar
 
      Returns the economic calendar.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -92,15 +92,15 @@
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[EconomicCalendar, str]]:
     """Economic calendar
 
      Returns the economic calendar.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -115,15 +115,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[EconomicCalendar, str]]:
     """Economic calendar
 
      Returns the economic calendar.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_fda_calendar.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_fda_calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.fda_calendar import FdaCalendar
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
         "url": "/api/market/fda-calendar",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[FdaCalendar, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = FdaCalendar.from_dict(response.json())
 
@@ -34,27 +34,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[FdaCalendar, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[FdaCalendar, str]]:
     """Fda calendar
 
      Returns the fda calendar for the current week.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -71,15 +71,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[FdaCalendar, str]]:
     """Fda calendar
 
      Returns the fda calendar for the current week.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -92,15 +92,15 @@
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[FdaCalendar, str]]:
     """Fda calendar
 
      Returns the fda calendar for the current week.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -115,15 +115,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[FdaCalendar, str]]:
     """Fda calendar
 
      Returns the fda calendar for the current week.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_holidays.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_holidays.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.market_holidays import MarketHolidays
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
         "url": "/api/market/holidays",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[MarketHolidays, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = MarketHolidays.from_dict(response.json())
 
@@ -34,27 +34,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[MarketHolidays, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[MarketHolidays, str]]:
     """Market Holidays
 
      Returns the market holidays.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -71,15 +71,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[MarketHolidays, str]]:
     """Market Holidays
 
      Returns the market holidays.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -92,15 +92,15 @@
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[MarketHolidays, str]]:
     """Market Holidays
 
      Returns the market holidays.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -115,15 +115,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[MarketHolidays, str]]:
     """Market Holidays
 
      Returns the market holidays.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_imbalances.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_sector_stats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,160 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.imbalances_volume import ImbalancesVolume
+from ...client import UnusualWhalesClient
+from ...models.sector_etf_results import SectorETFResults
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/imbalances",
+        "url": "/api/market/sector-etfs",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ImbalancesVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[SectorETFResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = ImbalancesVolume.from_dict(response.json())
+        response_200 = SectorETFResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = response.text
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ImbalancesVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[SectorETFResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ImbalancesVolume, str]]:
-    """MOC/MOO Imbalances Data
+    client: UnusualWhalesClient,
+) -> Response[Union[SectorETFResults, str]]:
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the MOC/MOO imbalances.
+     Returns the current Trading Days statistics for the SPDR sector etfs
+
+    ----
+    This can be used to build a market overview such as:
+
+    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ImbalancesVolume, str]]
+        Response[Union[SectorETFResults, str]]
     """
 
     kwargs = _get_kwargs()
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ImbalancesVolume, str]]:
-    """MOC/MOO Imbalances Data
+    client: UnusualWhalesClient,
+) -> Optional[Union[SectorETFResults, str]]:
+    """Returns the stats for sector etfs for the most recent trading day
+
+     Returns the current Trading Days statistics for the SPDR sector etfs
+
+    ----
+    This can be used to build a market overview such as:
 
-     Returns the MOC/MOO imbalances.
+    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ImbalancesVolume, str]
+        Union[SectorETFResults, str]
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ImbalancesVolume, str]]:
-    """MOC/MOO Imbalances Data
+    client: UnusualWhalesClient,
+) -> Response[Union[SectorETFResults, str]]:
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the MOC/MOO imbalances.
+     Returns the current Trading Days statistics for the SPDR sector etfs
+
+    ----
+    This can be used to build a market overview such as:
+
+    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ImbalancesVolume, str]]
+        Response[Union[SectorETFResults, str]]
     """
 
     kwargs = _get_kwargs()
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ImbalancesVolume, str]]:
-    """MOC/MOO Imbalances Data
+    client: UnusualWhalesClient,
+) -> Optional[Union[SectorETFResults, str]]:
+    """Returns the stats for sector etfs for the most recent trading day
+
+     Returns the current Trading Days statistics for the SPDR sector etfs
+
+    ----
+    This can be used to build a market overview such as:
 
-     Returns the MOC/MOO imbalances.
+    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ImbalancesVolume, str]
+        Union[SectorETFResults, str]
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_insider_trades.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_insider_trades.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.market_options_volume import MarketOptionsVolume
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -27,15 +27,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = MarketOptionsVolume.from_dict(response.json())
 
@@ -50,27 +50,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
     """Total Insider Buy & Sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     across the market
 
@@ -95,15 +95,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
     """Total Insider Buy & Sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     across the market
 
@@ -123,15 +123,15 @@
         client=client,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
     """Total Insider Buy & Sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     across the market
 
@@ -154,15 +154,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
     """Total Insider Buy & Sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     across the market
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_options_volume.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_spike.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.market_options_volume import MarketOptionsVolume
+from ...models.spike_value import SPIKEValue
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    limit: Union[Unset, int] = UNSET,
+    date: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
 
-    params["limit"] = limit
+    params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/total-options-volume",
+        "url": "/api/market/spike",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = MarketOptionsVolume.from_dict(response.json())
+        response_200 = SPIKEValue.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -50,157 +50,145 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Get Options Activity for the Entire Market (Market Tide)
-
-     Returns the total options volume and premium for all trade executions
-    that happened on a given trading date.
-
-    ----
-    This can be used to build a market options overview such as:
-
-    ![Market State](https://i.imgur.com/IioJyq9.png)
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
+    """SPIKE
+
+     Returns the SPIKE values for the given date.
+    Date must be the current or a past date. If no date is given, returns data for the current/last
+    market day.
 
     Args:
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, MarketOptionsVolume, str]]
+        Response[Union[ErrorMessage, SPIKEValue, str]]
     """
 
     kwargs = _get_kwargs(
-        limit=limit,
+        date=date,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Get Options Activity for the Entire Market (Market Tide)
-
-     Returns the total options volume and premium for all trade executions
-    that happened on a given trading date.
-
-    ----
-    This can be used to build a market options overview such as:
-
-    ![Market State](https://i.imgur.com/IioJyq9.png)
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
+    """SPIKE
+
+     Returns the SPIKE values for the given date.
+    Date must be the current or a past date. If no date is given, returns data for the current/last
+    market day.
 
     Args:
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, MarketOptionsVolume, str]
+        Union[ErrorMessage, SPIKEValue, str]
     """
 
     return sync_detailed(
         client=client,
-        limit=limit,
+        date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Get Options Activity for the Entire Market (Market Tide)
-
-     Returns the total options volume and premium for all trade executions
-    that happened on a given trading date.
-
-    ----
-    This can be used to build a market options overview such as:
-
-    ![Market State](https://i.imgur.com/IioJyq9.png)
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
+    """SPIKE
+
+     Returns the SPIKE values for the given date.
+    Date must be the current or a past date. If no date is given, returns data for the current/last
+    market day.
 
     Args:
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, MarketOptionsVolume, str]]
+        Response[Union[ErrorMessage, SPIKEValue, str]]
     """
 
     kwargs = _get_kwargs(
-        limit=limit,
+        date=date,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Get Options Activity for the Entire Market (Market Tide)
-
-     Returns the total options volume and premium for all trade executions
-    that happened on a given trading date.
-
-    ----
-    This can be used to build a market options overview such as:
-
-    ![Market State](https://i.imgur.com/IioJyq9.png)
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
+    """SPIKE
+
+     Returns the SPIKE values for the given date.
+    Date must be the current or a past date. If no date is given, returns data for the current/last
+    market day.
 
     Args:
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, MarketOptionsVolume, str]
+        Union[ErrorMessage, SPIKEValue, str]
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            limit=limit,
+            date=date,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_tide.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_market_tide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.daily_market_tide_response import DailyMarketTideResponse
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
@@ -33,15 +33,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = DailyMarketTideResponse.from_dict(response.json())
 
@@ -56,27 +56,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Response[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
@@ -141,15 +141,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Optional[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
@@ -209,15 +209,15 @@
         otm_only=otm_only,
         interval_5m=interval_5m,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Response[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
@@ -280,15 +280,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Optional[Union[DailyMarketTideResponse, ErrorMessage, str]]:
     """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_market_tide_by_etf.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/market/get_market_tide_by_etf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.daily_market_tide import DailyMarketTide
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = DailyMarketTide.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
     """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
@@ -103,15 +103,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
     """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
@@ -137,15 +137,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
     """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
@@ -174,15 +174,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
     """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_open_interest_change.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_open_interest_change.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.oi_change_results import OIChangeResults
 from ...models.order_direction import OrderDirection
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
+    ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
@@ -29,23 +30,23 @@
 
     params["order"] = json_order
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/oi-change",
+        "url": f"/api/stock/{ticker}/oi-change",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[OIChangeResults]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = OIChangeResults.from_dict(response.json())
 
@@ -53,181 +54,189 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[OIChangeResults]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChangeResults]:
-    """Returns the Option Contracts With The Highest Open Interest Change by Date
+    """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChangeResults]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChangeResults]:
-    """Returns the Option Contracts With The Highest Open Interest Change by Date
+    """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChangeResults
     """
 
     return sync_detailed(
+        ticker=ticker,
         client=client,
         date=date,
         limit=limit,
         order=order,
     ).parsed
 
 
 async def asyncio_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChangeResults]:
-    """Returns the Option Contracts With The Highest Open Interest Change by Date
+    """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChangeResults]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChangeResults]:
-    """Returns the Option Contracts With The Highest Open Interest Change by Date
+    """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChangeResults
     """
 
     return (
         await asyncio_detailed(
+            ticker=ticker,
             client=client,
             date=date,
             limit=limit,
             order=order,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_sector_stats.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,160 +1,144 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.sector_etf_results import SectorETFResults
+from ...client import UnusualWhalesClient
+from ...models.seasonality_market_results import SeasonalityMarketResults
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/sector-etfs",
+        "url": "/api/seasonality/market",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[SectorETFResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[SeasonalityMarketResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = SectorETFResults.from_dict(response.json())
+        response_200 = SeasonalityMarketResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = response.text
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[SectorETFResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[SeasonalityMarketResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[SectorETFResults, str]]:
-    """Returns the stats for sector etfs for the most recent trading day
+    client: UnusualWhalesClient,
+) -> Response[Union[SeasonalityMarketResults, str]]:
+    """Market Seasonality for ETFs
 
-     Returns the current Trading Days statistics for the SPDR sector etfs
-
-    ----
-    This can be used to build a market overview such as:
-
-    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
+     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
+    XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[SectorETFResults, str]]
+        Response[Union[SeasonalityMarketResults, str]]
     """
 
     kwargs = _get_kwargs()
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[SectorETFResults, str]]:
-    """Returns the stats for sector etfs for the most recent trading day
-
-     Returns the current Trading Days statistics for the SPDR sector etfs
-
-    ----
-    This can be used to build a market overview such as:
+    client: UnusualWhalesClient,
+) -> Optional[Union[SeasonalityMarketResults, str]]:
+    """Market Seasonality for ETFs
 
-    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
+     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
+    XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[SectorETFResults, str]
+        Union[SeasonalityMarketResults, str]
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[SectorETFResults, str]]:
-    """Returns the stats for sector etfs for the most recent trading day
+    client: UnusualWhalesClient,
+) -> Response[Union[SeasonalityMarketResults, str]]:
+    """Market Seasonality for ETFs
 
-     Returns the current Trading Days statistics for the SPDR sector etfs
-
-    ----
-    This can be used to build a market overview such as:
-
-    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
+     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
+    XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[SectorETFResults, str]]
+        Response[Union[SeasonalityMarketResults, str]]
     """
 
     kwargs = _get_kwargs()
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[SectorETFResults, str]]:
-    """Returns the stats for sector etfs for the most recent trading day
-
-     Returns the current Trading Days statistics for the SPDR sector etfs
-
-    ----
-    This can be used to build a market overview such as:
+    client: UnusualWhalesClient,
+) -> Optional[Union[SeasonalityMarketResults, str]]:
+    """Market Seasonality for ETFs
 
-    ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
+     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
+    XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[SectorETFResults, str]
+        Union[SeasonalityMarketResults, str]
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/market/get_spike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.spike_value import SPIKEValue
+from ...models.volume_oi_per_expiry_results import VolumeOIPerExpiryResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
+    ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/spike",
+        "url": f"/api/stock/{ticker}/option/volume-oi-expiry",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = SPIKEValue.from_dict(response.json())
+        response_200 = VolumeOIPerExpiryResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -50,145 +51,149 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
-    """SPIKE
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
+    """Volume & OI per Expiry
 
-     Returns the SPIKE values for the given date.
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SPIKEValue, str]]
+        Response[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
-    """SPIKE
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
+    """Volume & OI per Expiry
 
-     Returns the SPIKE values for the given date.
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SPIKEValue, str]
+        Union[ErrorMessage, VolumeOIPerExpiryResults, str]
     """
 
     return sync_detailed(
+        ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, SPIKEValue, str]]:
-    """SPIKE
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
+    """Volume & OI per Expiry
 
-     Returns the SPIKE values for the given date.
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SPIKEValue, str]]
+        Response[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, SPIKEValue, str]]:
-    """SPIKE
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiryResults, str]]:
+    """Volume & OI per Expiry
 
-     Returns the SPIKE values for the given date.
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SPIKEValue, str]
+        Union[ErrorMessage, VolumeOIPerExpiryResults, str]
     """
 
     return (
         await asyncio_detailed(
+            ticker=ticker,
             client=client,
             date=date,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/screener/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/screener/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_analyst_ratings.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_analyst_ratings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.analalyst_rating_results import AnalalystRatingResults
 from ...models.analyst_action import AnalystAction
 from ...models.analyst_recommendation import AnalystRecommendation
 from ...models.analyst_sector import AnalystSector
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
@@ -54,15 +54,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[AnalalystRatingResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = AnalalystRatingResults.from_dict(response.json())
 
@@ -77,27 +77,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[AnalalystRatingResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Response[Union[AnalalystRatingResults, ErrorMessage, str]]:
     """Analyst Ratings for a Ticker
@@ -135,15 +135,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Optional[Union[AnalalystRatingResults, ErrorMessage, str]]:
     """Analyst Ratings for a Ticker
@@ -176,15 +176,15 @@
         recommendation=recommendation,
         sector=sector,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Response[Union[AnalalystRatingResults, ErrorMessage, str]]:
     """Analyst Ratings for a Ticker
@@ -220,15 +220,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Optional[Union[AnalalystRatingResults, ErrorMessage, str]]:
     """Analyst Ratings for a Ticker
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_option_contracts.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_option_contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.option_contract_screener_results import OptionContractScreenerResults
 from ...models.option_type import OptionType
 from ...models.order_direction import OrderDirection
 from ...models.screener_contract_order_by_field import ScreenerContractOrderByField
 from ...models.single_issue_type import SingleIssueType
 from ...models.single_sector import SingleSector
@@ -166,15 +166,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, OptionContractScreenerResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = OptionContractScreenerResults.from_dict(response.json())
 
@@ -189,27 +189,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, OptionContractScreenerResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     sectors: Union[Unset, List[SingleSector]] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
@@ -394,15 +394,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     sectors: Union[Unset, List[SingleSector]] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
@@ -582,15 +582,15 @@
         order=order,
         order_direction=order_direction,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     sectors: Union[Unset, List[SingleSector]] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
@@ -773,15 +773,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker_symbol: Union[Unset, str] = UNSET,
     sectors: Union[Unset, List[SingleSector]] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/screener/get_stocks.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/screener/get_stocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.order_direction import OrderDirection
 from ...models.screener_order_by_field import ScreenerOrderByField
 from ...models.single_issue_type import SingleIssueType
 from ...models.single_sector import SingleSector
 from ...models.stock_screener_response import StockScreenerResponse
 from ...types import UNSET, Response, Unset
@@ -227,15 +227,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, StockScreenerResponse, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = StockScreenerResponse.from_dict(response.json())
 
@@ -250,27 +250,27 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, StockScreenerResponse, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_change: Union[Unset, int] = UNSET,
     max_change: Union[Unset, int] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_s_p_500: Union[Unset, bool] = UNSET,
@@ -513,15 +513,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_change: Union[Unset, int] = UNSET,
     max_change: Union[Unset, int] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_s_p_500: Union[Unset, bool] = UNSET,
@@ -759,15 +759,15 @@
         order=order,
         order_direction=order_direction,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_change: Union[Unset, int] = UNSET,
     max_change: Union[Unset, int] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_s_p_500: Union[Unset, bool] = UNSET,
@@ -1008,15 +1008,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     ticker: Union[Unset, str] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_change: Union[Unset, int] = UNSET,
     max_change: Union[Unset, int] = UNSET,
     min_underlying_price: Union[Unset, int] = UNSET,
     max_underlying_price: Union[Unset, int] = UNSET,
     is_s_p_500: Union[Unset, bool] = UNSET,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,169 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.seasonality_market_results import SeasonalityMarketResults
+from ...client import UnusualWhalesClient
+from ...models.error_message import ErrorMessage
+from ...models.seasonality_year_month_results import SeasonalityYearMonthResults
 from ...types import Response
 
 
-def _get_kwargs() -> Dict[str, Any]:
+def _get_kwargs(
+    ticker: str,
+) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/seasonality/market",
+        "url": f"/api/seasonality/{ticker}/year-month",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[SeasonalityMarketResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = SeasonalityMarketResults.from_dict(response.json())
+        response_200 = SeasonalityYearMonthResults.from_dict(response.json())
 
         return response_200
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = ErrorMessage.from_dict(response.json())
+
+        return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = response.text
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[SeasonalityMarketResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[SeasonalityMarketResults, str]]:
-    """Market Seasonality for ETFs
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    """Price change per month per year
+
+     Returns the relative price change for all past months over multiple years.
 
-     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
-    XLRE, XLF, XLI, XLB .
+    Args:
+        ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[SeasonalityMarketResults, str]]
+        Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]
     """
 
-    kwargs = _get_kwargs()
+    kwargs = _get_kwargs(
+        ticker=ticker,
+    )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[SeasonalityMarketResults, str]]:
-    """Market Seasonality for ETFs
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    """Price change per month per year
+
+     Returns the relative price change for all past months over multiple years.
 
-     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
-    XLRE, XLF, XLI, XLB .
+    Args:
+        ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[SeasonalityMarketResults, str]
+        Union[ErrorMessage, SeasonalityYearMonthResults, str]
     """
 
     return sync_detailed(
+        ticker=ticker,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[SeasonalityMarketResults, str]]:
-    """Market Seasonality for ETFs
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    """Price change per month per year
 
-     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
-    XLRE, XLF, XLI, XLB .
+     Returns the relative price change for all past months over multiple years.
+
+    Args:
+        ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[SeasonalityMarketResults, str]]
+        Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]
     """
 
-    kwargs = _get_kwargs()
+    kwargs = _get_kwargs(
+        ticker=ticker,
+    )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[SeasonalityMarketResults, str]]:
-    """Market Seasonality for ETFs
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    """Price change per month per year
+
+     Returns the relative price change for all past months over multiple years.
 
-     Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
-    XLRE, XLF, XLI, XLB .
+    Args:
+        ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[SeasonalityMarketResults, str]
+        Union[ErrorMessage, SeasonalityYearMonthResults, str]
     """
 
     return (
         await asyncio_detailed(
+            ticker=ticker,
             client=client,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_monthly_average_returns.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.seasonality_monthly_results import SeasonalityMonthlyResults
-from ...types import Response
+from ...models.greeks import Greeks
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
+    *,
+    date: Union[Unset, str] = UNSET,
+    expiry: str,
 ) -> Dict[str, Any]:
+    # Dictionary of query parameters to be sent with the request.
+    params: Dict[str, Any] = {}
+
+    params["date"] = date
+
+    params["expiry"] = expiry
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/seasonality/{ticker}/monthly",
+        "url": f"/api/stock/{ticker}/greeks",
+        "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, Greeks, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = SeasonalityMonthlyResults.from_dict(response.json())
+        response_200 = Greeks.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -41,129 +54,161 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, Greeks, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
-    """Average return per month
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+    expiry: str,
+) -> Response[Union[ErrorMessage, Greeks, str]]:
+    """Option Greeks by Expiry All Strikes
 
-     Returns the average return by month for the given ticker.
+     Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]
+        Response[Union[ErrorMessage, Greeks, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
+        date=date,
+        expiry=expiry,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
-    """Average return per month
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+    expiry: str,
+) -> Optional[Union[ErrorMessage, Greeks, str]]:
+    """Option Greeks by Expiry All Strikes
 
-     Returns the average return by month for the given ticker.
+     Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SeasonalityMonthlyResults, str]
+        Union[ErrorMessage, Greeks, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
+        date=date,
+        expiry=expiry,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
-    """Average return per month
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+    expiry: str,
+) -> Response[Union[ErrorMessage, Greeks, str]]:
+    """Option Greeks by Expiry All Strikes
 
-     Returns the average return by month for the given ticker.
+     Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SeasonalityMonthlyResults, str]]
+        Response[Union[ErrorMessage, Greeks, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
+        date=date,
+        expiry=expiry,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ErrorMessage, SeasonalityMonthlyResults, str]]:
-    """Average return per month
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+    expiry: str,
+) -> Optional[Union[ErrorMessage, Greeks, str]]:
+    """Option Greeks by Expiry All Strikes
 
-     Returns the average return by month for the given ticker.
+     Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SeasonalityMonthlyResults, str]
+        Union[ErrorMessage, Greeks, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
+            date=date,
+            expiry=expiry,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_monthly_top_performers.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/seasonality/get_monthly_top_performers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.order_direction import OrderDirection
 from ...models.seasonality_performance_order_by import SeasonalityPerformanceOrderBy
 from ...models.seasonality_performers_results import SeasonalityPerformersResults
 from ...models.single_month_number import SingleMonthNumber
 from ...types import UNSET, Response, Unset
 
@@ -57,15 +57,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, SeasonalityPerformersResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = SeasonalityPerformersResults.from_dict(response.json())
 
@@ -80,28 +80,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, SeasonalityPerformersResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     month: SingleMonthNumber,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     min_years: Union[Unset, int] = UNSET,
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
@@ -155,15 +155,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     month: SingleMonthNumber,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     min_years: Union[Unset, int] = UNSET,
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
@@ -212,15 +212,15 @@
         order_direction=order_direction,
     ).parsed
 
 
 async def asyncio_detailed(
     month: SingleMonthNumber,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     min_years: Union[Unset, int] = UNSET,
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
@@ -272,15 +272,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     month: SingleMonthNumber,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     min_years: Union[Unset, int] = UNSET,
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/earnings/get_ticker_earnings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
+from ...models.earnings_results import EarningsResults
 from ...models.error_message import ErrorMessage
-from ...models.seasonality_year_month_results import SeasonalityYearMonthResults
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/seasonality/{ticker}/year-month",
+        "url": f"/api/earnings/{ticker}",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = SeasonalityYearMonthResults.from_dict(response.json())
+        response_200 = EarningsResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -41,42 +41,42 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[EarningsResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
-    """Price change per month per year
+    client: UnusualWhalesClient,
+) -> Response[Union[EarningsResults, ErrorMessage, str]]:
+    """Past Ticker Earnings
 
-     Returns the relative price change for all past months over multiple years.
+     Returns the past earnings for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]
+        Response[Union[EarningsResults, ErrorMessage, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
     )
 
     response = client.get_httpx_client().request(
@@ -85,84 +85,84 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
-    """Price change per month per year
+    client: UnusualWhalesClient,
+) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
+    """Past Ticker Earnings
 
-     Returns the relative price change for all past months over multiple years.
+     Returns the past earnings for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SeasonalityYearMonthResults, str]
+        Union[EarningsResults, ErrorMessage, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
-    """Price change per month per year
+    client: UnusualWhalesClient,
+) -> Response[Union[EarningsResults, ErrorMessage, str]]:
+    """Past Ticker Earnings
 
-     Returns the relative price change for all past months over multiple years.
+     Returns the past earnings for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, SeasonalityYearMonthResults, str]]
+        Response[Union[EarningsResults, ErrorMessage, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[Union[ErrorMessage, SeasonalityYearMonthResults, str]]:
-    """Price change per month per year
+    client: UnusualWhalesClient,
+) -> Optional[Union[EarningsResults, ErrorMessage, str]]:
+    """Past Ticker Earnings
 
-     Returns the relative price change for all past months over multiple years.
+     Returns the past earnings for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, SeasonalityYearMonthResults, str]
+        Union[EarningsResults, ErrorMessage, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
         )
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.option_chain_contract_results import OptionChainContractResults
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = OptionChainContractResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expirations: str,
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     """ATM option contracts for the given expiries
 
      Returns the ATM option contracts for the given expirations
 
     Args:
@@ -98,15 +98,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expirations: str,
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     """ATM option contracts for the given expiries
 
      Returns the ATM option contracts for the given expirations
 
     Args:
@@ -127,15 +127,15 @@
         expirations=expirations,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expirations: str,
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     """ATM option contracts for the given expiries
 
      Returns the ATM option contracts for the given expirations
 
     Args:
@@ -159,15 +159,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expirations: str,
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     """ATM option contracts for the given expiries
 
      Returns the ATM option contracts for the given expirations
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_candles.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_candles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.candle_data_results import CandleDataResults
 from ...models.candle_size import CandleSize
 from ...models.error_message import ErrorMessage
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
@@ -36,15 +36,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[CandleDataResults, ErrorMessage, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = CandleDataResults.from_dict(response.json())
 
@@ -59,29 +59,29 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[CandleDataResults, ErrorMessage, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     candle_size: CandleSize,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     timeframe: Union[Unset, str] = UNSET,
     trading_day: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[CandleDataResults, ErrorMessage, str]]:
     """OHLC
 
      Returns the Open High Low Close (OHLC) candle data for a given ticker.
@@ -127,15 +127,15 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     candle_size: CandleSize,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     timeframe: Union[Unset, str] = UNSET,
     trading_day: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[CandleDataResults, ErrorMessage, str]]:
     """OHLC
 
      Returns the Open High Low Close (OHLC) candle data for a given ticker.
@@ -176,15 +176,15 @@
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     candle_size: CandleSize,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     timeframe: Union[Unset, str] = UNSET,
     trading_day: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[CandleDataResults, ErrorMessage, str]]:
     """OHLC
 
      Returns the Open High Low Close (OHLC) candle data for a given ticker.
@@ -228,15 +228,15 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     candle_size: CandleSize,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     timeframe: Union[Unset, str] = UNSET,
     trading_day: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[CandleDataResults, ErrorMessage, str]]:
     """OHLC
 
      Returns the Open High Low Close (OHLC) candle data for a given ticker.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.expiry_breakdown_result import ExpiryBreakdownResult
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = ExpiryBreakdownResult.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
      Returns all expirations for the given Trading Day for a ticker.
 
     Args:
@@ -100,15 +100,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
      Returns all expirations for the given Trading Day for a ticker.
 
     Args:
@@ -131,15 +131,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
      Returns all expirations for the given Trading Day for a ticker.
 
     Args:
@@ -165,15 +165,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, ExpiryBreakdownResult, str]]:
     """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
      Returns all expirations for the given Trading Day for a ticker.
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.greek_exposure_results import GreekExposureResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -31,15 +31,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, GreekExposureResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = GreekExposureResults.from_dict(response.json())
 
@@ -54,28 +54,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, GreekExposureResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     timeframe: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureResults, str]]:
     """Greek Exposure
 
      Greek Exposure is the assumed greek exposure that market makers are exposed to. The most popular
     greek exposure is gamma exposure (GEX).
@@ -136,15 +136,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     timeframe: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureResults, str]]:
     """Greek Exposure
 
      Greek Exposure is the assumed greek exposure that market makers are exposed to. The most popular
     greek exposure is gamma exposure (GEX).
@@ -200,15 +200,15 @@
         timeframe=timeframe,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     timeframe: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureResults, str]]:
     """Greek Exposure
 
      Greek Exposure is the assumed greek exposure that market makers are exposed to. The most popular
     greek exposure is gamma exposure (GEX).
@@ -267,15 +267,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     timeframe: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureResults, str]]:
     """Greek Exposure
 
      Greek Exposure is the assumed greek exposure that market makers are exposed to. The most popular
     greek exposure is gamma exposure (GEX).
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.greek_exposure_by_strike_results import GreekExposureByStrikeResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = GreekExposureByStrikeResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
@@ -100,15 +100,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
@@ -131,15 +131,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
@@ -165,15 +165,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.greek_exposure_by_strike_results import GreekExposureByStrikeResults
+from ...models.greek_exposure_by_strike_and_expiry_results import GreekExposureByStrikeAndExpiryResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
+    expiry: str,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
 
     params["date"] = date
 
+    params["expiry"] = expiry
+
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/greek-exposure/strike",
+        "url": f"/api/stock/{ticker}/greek-exposure/strike-expiry",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = GreekExposureByStrikeResults.from_dict(response.json())
+        response_200 = GreekExposureByStrikeAndExpiryResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -51,149 +54,161 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
-    """Greek Exposure Grouped By Strike All Expiries On A Given Date
+    expiry: str,
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    """Greek Exposure By Strike And Expiry
 
-     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
+     The greek exposure of a ticker grouped by strike price for a specific expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]
+        Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
+        expiry=expiry,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
-    """Greek Exposure Grouped By Strike All Expiries On A Given Date
+    expiry: str,
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    """Greek Exposure By Strike And Expiry
 
-     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
+     The greek exposure of a ticker grouped by strike price for a specific expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, GreekExposureByStrikeResults, str]
+        Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
+        expiry=expiry,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
-    """Greek Exposure Grouped By Strike All Expiries On A Given Date
+    expiry: str,
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    """Greek Exposure By Strike And Expiry
 
-     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
+     The greek exposure of a ticker grouped by strike price for a specific expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]
+        Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
+        expiry=expiry,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
-    """Greek Exposure Grouped By Strike All Expiries On A Given Date
+    expiry: str,
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    """Greek Exposure By Strike And Expiry
 
-     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
+     The greek exposure of a ticker grouped by strike price for a specific expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
+        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, GreekExposureByStrikeResults, str]
+        Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
+            expiry=expiry,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,214 +1,220 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.greek_exposure_by_strike_and_expiry_results import GreekExposureByStrikeAndExpiryResults
-from ...types import UNSET, Response, Unset
+from ...models.error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated import (
+    ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+)
+from ...models.ticker_info_results import TickerInfoResults
+from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
-    *,
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
 ) -> Dict[str, Any]:
-    # Dictionary of query parameters to be sent with the request.
-    params: Dict[str, Any] = {}
-
-    params["date"] = date
-
-    params["expiry"] = expiry
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/greek-exposure/strike-expiry",
-        "params": params,
+        "url": f"/api/stock/{ticker}/info",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = GreekExposureByStrikeAndExpiryResults.from_dict(response.json())
+        response_200 = TickerInfoResults.from_dict(response.json())
 
         return response_200
+    if response.status_code == HTTPStatus.NOT_FOUND:
+        response_404 = ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated.from_dict(
+            response.json()
+        )
+
+        return response_404
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = response.text
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
-    """Greek Exposure By Strike And Expiry
+    client: UnusualWhalesClient,
+) -> Response[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
+    """Ticker Information
 
-     The greek exposure of a ticker grouped by strike price for a specific expiry date.
+     Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]
+        Response[Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
-        expiry=expiry,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
-    """Greek Exposure By Strike And Expiry
+    client: UnusualWhalesClient,
+) -> Optional[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
+    """Ticker Information
 
-     The greek exposure of a ticker grouped by strike price for a specific expiry date.
+     Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]
+        Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
-        date=date,
-        expiry=expiry,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
-    """Greek Exposure By Strike And Expiry
+    client: UnusualWhalesClient,
+) -> Response[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
+    """Ticker Information
 
-     The greek exposure of a ticker grouped by strike price for a specific expiry date.
+     Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]
+        Response[Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
-        expiry=expiry,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Optional[Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]]:
-    """Greek Exposure By Strike And Expiry
+    client: UnusualWhalesClient,
+) -> Optional[
+    Union[
+        ErrorMessage,
+        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
+        TickerInfoResults,
+        str,
+    ]
+]:
+    """Ticker Information
 
-     The greek exposure of a ticker grouped by strike price for a specific expiry date.
+     Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, GreekExposureByStrikeAndExpiryResults, str]
+        Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
-            date=date,
-            expiry=expiry,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_max_pain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.greeks import Greeks
-from ...types import UNSET, Response, Unset
+from ...models.max_pain_results import MaxPainResults
+from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
-    *,
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
 ) -> Dict[str, Any]:
-    # Dictionary of query parameters to be sent with the request.
-    params: Dict[str, Any] = {}
-
-    params["date"] = date
-
-    params["expiry"] = expiry
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/greeks",
-        "params": params,
+        "url": f"/api/stock/{ticker}/max-pain",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, Greeks, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, MaxPainResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = Greeks.from_dict(response.json())
+        response_200 = MaxPainResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -54,161 +41,129 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, Greeks, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, MaxPainResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Response[Union[ErrorMessage, Greeks, str]]:
-    """Option Greeks by Expiry All Strikes
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, MaxPainResults, str]]:
+    """Max Pain
 
-     Returns the greeks for each strike for a single expiry date.
+     Returns the max pain for all expirations for the given ticker for the last 120 days
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, Greeks, str]]
+        Response[Union[ErrorMessage, MaxPainResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
-        expiry=expiry,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Optional[Union[ErrorMessage, Greeks, str]]:
-    """Option Greeks by Expiry All Strikes
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, MaxPainResults, str]]:
+    """Max Pain
 
-     Returns the greeks for each strike for a single expiry date.
+     Returns the max pain for all expirations for the given ticker for the last 120 days
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, Greeks, str]
+        Union[ErrorMessage, MaxPainResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
-        date=date,
-        expiry=expiry,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Response[Union[ErrorMessage, Greeks, str]]:
-    """Option Greeks by Expiry All Strikes
+    client: UnusualWhalesClient,
+) -> Response[Union[ErrorMessage, MaxPainResults, str]]:
+    """Max Pain
 
-     Returns the greeks for each strike for a single expiry date.
+     Returns the max pain for all expirations for the given ticker for the last 120 days
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, Greeks, str]]
+        Response[Union[ErrorMessage, MaxPainResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
-        expiry=expiry,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-    expiry: str,
-) -> Optional[Union[ErrorMessage, Greeks, str]]:
-    """Option Greeks by Expiry All Strikes
+    client: UnusualWhalesClient,
+) -> Optional[Union[ErrorMessage, MaxPainResults, str]]:
+    """Max Pain
 
-     Returns the greeks for each strike for a single expiry date.
+     Returns the max pain for all expirations for the given ticker for the last 120 days
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
-        expiry (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, Greeks, str]
+        Union[ErrorMessage, MaxPainResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
-            date=date,
-            expiry=expiry,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_info.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_options_volume.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,220 +1,199 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated import (
-    ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-)
-from ...models.ticker_info_results import TickerInfoResults
-from ...types import Response
+from ...models.ticker_options_volume import TickerOptionsVolume
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
+    *,
+    limit: Union[Unset, int] = UNSET,
 ) -> Dict[str, Any]:
+    # Dictionary of query parameters to be sent with the request.
+    params: Dict[str, Any] = {}
+
+    params["limit"] = limit
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/info",
+        "url": f"/api/stock/{ticker}/options-volume",
+        "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = TickerInfoResults.from_dict(response.json())
+        response_200 = TickerOptionsVolume.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated.from_dict(
-            response.json()
-        )
-
-        return response_404
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = response.text
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
-    """Ticker Information
+    client: UnusualWhalesClient,
+    limit: Union[Unset, int] = UNSET,
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns a information about the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]]
+        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
+        limit=limit,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
-    """Ticker Information
+    client: UnusualWhalesClient,
+    limit: Union[Unset, int] = UNSET,
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns a information about the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]
+        Union[ErrorMessage, TickerOptionsVolume, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
+        limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
-    """Ticker Information
+    client: UnusualWhalesClient,
+    limit: Union[Unset, int] = UNSET,
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns a information about the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]]
+        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
+        limit=limit,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Optional[
-    Union[
-        ErrorMessage,
-        ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
-        TickerInfoResults,
-        str,
-    ]
-]:
-    """Ticker Information
+    client: UnusualWhalesClient,
+    limit: Union[Unset, int] = UNSET,
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns a information about the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated, TickerInfoResults, str]
+        Union[ErrorMessage, TickerOptionsVolume, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
+            limit=limit,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_insider_trades.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_insider_trades.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.insider_statistics import InsiderStatistics
 from ...types import Response
 
 
 def _get_kwargs(
     ticker: str,
@@ -18,15 +18,15 @@
         "url": f"/api/stock/{ticker}/insider-buy-sells",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, InsiderStatistics, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = InsiderStatistics.from_dict(response.json())
 
@@ -41,28 +41,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, InsiderStatistics, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, InsiderStatistics, str]]:
     """Insider buy & sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     for the given ticker
 
     Args:
@@ -86,15 +86,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, InsiderStatistics, str]]:
     """Insider buy & sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     for the given ticker
 
     Args:
@@ -113,15 +113,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, InsiderStatistics, str]]:
     """Insider buy & sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     for the given ticker
 
     Args:
@@ -143,15 +143,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, InsiderStatistics, str]]:
     """Insider buy & sells
 
      Returns the total amount of purchases & sells as well as notional values for insider transactions
     for the given ticker
 
     Args:
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_net_premium_ticks.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_net_premium_ticks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.net_prem_tick_results import NetPremTickResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, NetPremTickResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = NetPremTickResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, NetPremTickResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, NetPremTickResults, str]]:
     r"""Net Prem Ticks
 
      Returns the net premium ticks for a given ticker which can be used to build the following chart:
     ![Net Prem chart](https://i.imgur.com/Rom1kcB.png)
 
@@ -143,15 +143,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, NetPremTickResults, str]]:
     r"""Net Prem Ticks
 
      Returns the net premium ticks for a given ticker which can be used to build the following chart:
     ![Net Prem chart](https://i.imgur.com/Rom1kcB.png)
 
@@ -217,15 +217,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, NetPremTickResults, str]]:
     r"""Net Prem Ticks
 
      Returns the net premium ticks for a given ticker which can be used to build the following chart:
     ![Net Prem chart](https://i.imgur.com/Rom1kcB.png)
 
@@ -294,15 +294,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, NetPremTickResults, str]]:
     r"""Net Prem Ticks
 
      Returns the net premium ticks for a given ticker which can be used to build the following chart:
     ![Net Prem chart](https://i.imgur.com/Rom1kcB.png)
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_open_interest_change.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_chains.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,242 +1,227 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.oi_change_results import OIChangeResults
-from ...models.order_direction import OrderDirection
+from ...client import UnusualWhalesClient
+from ...models.error_message import ErrorMessage
+from ...models.option_chains_results import OptionChainsResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-    order: Union[Unset, OrderDirection] = UNSET,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
 
     params["date"] = date
 
-    params["limit"] = limit
-
-    json_order: Union[Unset, str] = UNSET
-    if not isinstance(order, Unset):
-        json_order = order.value
-
-    params["order"] = json_order
-
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/oi-change",
+        "url": f"/api/stock/{ticker}/option-chains",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[OIChangeResults]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = OIChangeResults.from_dict(response.json())
+        response_200 = OptionChainsResults.from_dict(response.json())
 
         return response_200
+    if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+        response_422 = ErrorMessage.from_dict(response.json())
+
+        return response_422
+    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+        response_500 = response.text
+        return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[OIChangeResults]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-    order: Union[Unset, OrderDirection] = UNSET,
-) -> Response[OIChangeResults]:
-    """OI Change
-
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
+    r"""Tradeable Option Contracts By Ticker
+
+     Returns all option symbols for the given ticker that were present at the given day.
+
+    If no date is given, returns data for the current/last market day.
+
+    You can use the following regex to extract underlying ticker, option type, expiry & strike:
+    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+
+    Keep in mind that the strike needs to be divided by 1,000.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
-        order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
-            by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[OIChangeResults]
+        Response[Union[ErrorMessage, OptionChainsResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
-        limit=limit,
-        order=order,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-    order: Union[Unset, OrderDirection] = UNSET,
-) -> Optional[OIChangeResults]:
-    """OI Change
-
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
+    r"""Tradeable Option Contracts By Ticker
+
+     Returns all option symbols for the given ticker that were present at the given day.
+
+    If no date is given, returns data for the current/last market day.
+
+    You can use the following regex to extract underlying ticker, option type, expiry & strike:
+    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+
+    Keep in mind that the strike needs to be divided by 1,000.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
-        order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
-            by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        OIChangeResults
+        Union[ErrorMessage, OptionChainsResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
-        limit=limit,
-        order=order,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-    order: Union[Unset, OrderDirection] = UNSET,
-) -> Response[OIChangeResults]:
-    """OI Change
-
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
+    r"""Tradeable Option Contracts By Ticker
+
+     Returns all option symbols for the given ticker that were present at the given day.
+
+    If no date is given, returns data for the current/last market day.
+
+    You can use the following regex to extract underlying ticker, option type, expiry & strike:
+    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+
+    Keep in mind that the strike needs to be divided by 1,000.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
-        order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
-            by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[OIChangeResults]
+        Response[Union[ErrorMessage, OptionChainsResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
-        limit=limit,
-        order=order,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-    order: Union[Unset, OrderDirection] = UNSET,
-) -> Optional[OIChangeResults]:
-    """OI Change
-
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
-    Date must be the current or a past date. If no date is given, returns data for the current/last
-    market day.
+) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
+    r"""Tradeable Option Contracts By Ticker
+
+     Returns all option symbols for the given ticker that were present at the given day.
+
+    If no date is given, returns data for the current/last market day.
+
+    You can use the following regex to extract underlying ticker, option type, expiry & strike:
+    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+
+    Keep in mind that the strike needs to be divided by 1,000.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
-        order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
-            by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        OIChangeResults
+        Union[ErrorMessage, OptionChainsResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
-            limit=limit,
-            order=order,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_chains.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_volume_by_price_level.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.option_chains_results import OptionChainsResults
+from ...models.option_price_level_results import OptionPriceLevelResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
@@ -20,29 +20,29 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/option-chains",
+        "url": f"/api/stock/{ticker}/option/stock-price-levels",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = OptionChainsResults.from_dict(response.json())
+        response_200 = OptionPriceLevelResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -51,53 +51,46 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
-    r"""Tradeable Option Contracts By Ticker
+) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    """Option Price Levels
 
-     Returns all option symbols for the given ticker that were present at the given day.
-
-    If no date is given, returns data for the current/last market day.
-
-    You can use the following regex to extract underlying ticker, option type, expiry & strike:
-    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
-
-    Keep in mind that the strike needs to be divided by 1,000.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionChainsResults, str]]
+        Response[Union[ErrorMessage, OptionPriceLevelResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -107,78 +100,64 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
-    r"""Tradeable Option Contracts By Ticker
-
-     Returns all option symbols for the given ticker that were present at the given day.
-
-    If no date is given, returns data for the current/last market day.
-
-    You can use the following regex to extract underlying ticker, option type, expiry & strike:
-    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    """Option Price Levels
 
-    Keep in mind that the strike needs to be divided by 1,000.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionChainsResults, str]
+        Union[ErrorMessage, OptionPriceLevelResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionChainsResults, str]]:
-    r"""Tradeable Option Contracts By Ticker
+) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    """Option Price Levels
 
-     Returns all option symbols for the given ticker that were present at the given day.
-
-    If no date is given, returns data for the current/last market day.
-
-    You can use the following regex to extract underlying ticker, option type, expiry & strike:
-    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
-
-    Keep in mind that the strike needs to be divided by 1,000.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionChainsResults, str]]
+        Response[Union[ErrorMessage, OptionPriceLevelResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -186,40 +165,33 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionChainsResults, str]]:
-    r"""Tradeable Option Contracts By Ticker
-
-     Returns all option symbols for the given ticker that were present at the given day.
-
-    If no date is given, returns data for the current/last market day.
-
-    You can use the following regex to extract underlying ticker, option type, expiry & strike:
-    `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
+) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    """Option Price Levels
 
-    Keep in mind that the strike needs to be divided by 1,000.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionChainsResults, str]
+        Union[ErrorMessage, OptionPriceLevelResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_contracts.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_option_contracts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.option_chain_contract_results import OptionChainContractResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -49,15 +49,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, OptionChainContractResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = OptionChainContractResults.from_dict(response.json())
 
@@ -72,28 +72,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, OptionChainContractResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expiry: Union[Unset, str] = UNSET,
     option_type: Union[Unset, str] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     exclude_zero_vol_chains: Union[Unset, bool] = UNSET,
     exclude_zero_dte: Union[Unset, bool] = UNSET,
     exclude_zero_oi_chains: Union[Unset, bool] = UNSET,
     maybe_otm_only: Union[Unset, bool] = UNSET,
@@ -142,15 +142,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expiry: Union[Unset, str] = UNSET,
     option_type: Union[Unset, str] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     exclude_zero_vol_chains: Union[Unset, bool] = UNSET,
     exclude_zero_dte: Union[Unset, bool] = UNSET,
     exclude_zero_oi_chains: Union[Unset, bool] = UNSET,
     maybe_otm_only: Union[Unset, bool] = UNSET,
@@ -194,15 +194,15 @@
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expiry: Union[Unset, str] = UNSET,
     option_type: Union[Unset, str] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     exclude_zero_vol_chains: Union[Unset, bool] = UNSET,
     exclude_zero_dte: Union[Unset, bool] = UNSET,
     exclude_zero_oi_chains: Union[Unset, bool] = UNSET,
     maybe_otm_only: Union[Unset, bool] = UNSET,
@@ -249,15 +249,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     expiry: Union[Unset, str] = UNSET,
     option_type: Union[Unset, str] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     exclude_zero_vol_chains: Union[Unset, bool] = UNSET,
     exclude_zero_dte: Union[Unset, bool] = UNSET,
     exclude_zero_oi_chains: Union[Unset, bool] = UNSET,
     maybe_otm_only: Union[Unset, bool] = UNSET,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_option_volume_by_price_level.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volume_by_price_level.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.option_price_level_results import OptionPriceLevelResults
+from ...models.off_lit_price_level_results import OffLitPriceLevelResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
@@ -20,29 +20,29 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/option/stock-price-levels",
+        "url": f"/api/stock/{ticker}/stock-volume-price-levels",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = OptionPriceLevelResults.from_dict(response.json())
+        response_200 = OffLitPriceLevelResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -51,46 +51,52 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
-    """Option Price Levels
+) -> Response[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
+    """Off/Lit Price Levels
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
+
+    The price level is calculated by dividing the stock volume by the total
+    ----
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionPriceLevelResults, str]]
+        Response[Union[ErrorMessage, OffLitPriceLevelResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -100,64 +106,76 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
-    """Option Price Levels
+) -> Optional[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
+    """Off/Lit Price Levels
+
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
-     Returns the call and put volume per price level for the given ticker.
+    The price level is calculated by dividing the stock volume by the total
+    ----
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionPriceLevelResults, str]
+        Union[ErrorMessage, OffLitPriceLevelResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionPriceLevelResults, str]]:
-    """Option Price Levels
+) -> Response[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
+    """Off/Lit Price Levels
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
+
+    The price level is calculated by dividing the stock volume by the total
+    ----
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionPriceLevelResults, str]]
+        Response[Union[ErrorMessage, OffLitPriceLevelResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -165,33 +183,39 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionPriceLevelResults, str]]:
-    """Option Price Levels
+) -> Optional[Union[ErrorMessage, OffLitPriceLevelResults, str]]:
+    """Off/Lit Price Levels
+
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
-     Returns the call and put volume per price level for the given ticker.
+    The price level is calculated by dividing the stock volume by the total
+    ----
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionPriceLevelResults, str]
+        Union[ErrorMessage, OffLitPriceLevelResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_options_volume.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
-from ...models.ticker_options_volume import TickerOptionsVolume
+from ...models.greek_exposure_by_strike_results import GreekExposureByStrikeResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
-    limit: Union[Unset, int] = UNSET,
+    date: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     # Dictionary of query parameters to be sent with the request.
     params: Dict[str, Any] = {}
 
-    params["limit"] = limit
+    params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/options-volume",
+        "url": f"/api/stock/{ticker}/greek-exposure/strike",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
-        response_200 = TickerOptionsVolume.from_dict(response.json())
+        response_200 = GreekExposureByStrikeResults.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -51,149 +51,149 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    *, client: UnusualWhalesClient, response: httpx.Response
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
+        Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        limit=limit,
+        date=date,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, TickerOptionsVolume, str]
+        Union[ErrorMessage, GreekExposureByStrikeResults, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
-        limit=limit,
+        date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
+        Response[Union[ErrorMessage, GreekExposureByStrikeResults, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        limit=limit,
+        date=date,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    client: UnusualWhalesClient,
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, GreekExposureByStrikeResults, str]]:
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, TickerOptionsVolume, str]
+        Union[ErrorMessage, GreekExposureByStrikeResults, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
-            limit=limit,
+            date=date,
         )
     ).parsed
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_risk_reversal_skew.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_risk_reversal_skew.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.historical_risk_reversal_skew_results import HistoricalRiskReversalSkewResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -37,15 +37,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = HistoricalRiskReversalSkewResults.from_dict(response.json())
 
@@ -60,28 +60,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Response[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     """Historical Risk Reversal Skew by Expiry and Ticker
 
@@ -126,15 +126,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Optional[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     """Historical Risk Reversal Skew by Expiry and Ticker
 
@@ -174,15 +174,15 @@
         delta=delta,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Response[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     """Historical Risk Reversal Skew by Expiry and Ticker
 
@@ -225,15 +225,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Optional[Union[ErrorMessage, HistoricalRiskReversalSkewResults, str]]:
     """Historical Risk Reversal Skew by Expiry and Ticker
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_sector_tickers.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_sector_tickers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.market_sector_ticker_results import MarketSectorTickerResults
 from ...models.sector import Sector
 from ...types import Response
 
 
 def _get_kwargs(
@@ -19,15 +19,15 @@
         "url": f"/api/stock/{sector}/tickers",
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = MarketSectorTickerResults.from_dict(response.json())
 
@@ -42,28 +42,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     sector: Sector,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
@@ -86,15 +86,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     sector: Sector,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
@@ -112,15 +112,15 @@
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     sector: Sector,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Response[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
@@ -141,15 +141,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     sector: Sector,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
 ) -> Optional[Union[ErrorMessage, MarketSectorTickerResults, str]]:
     """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_spot_exposures.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_spot_exposures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.spot_gex_exposures_per_1_min_results import SpotGEXExposuresPer1MinResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = SpotGEXExposuresPer1MinResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     """Spot GEX exposures per 1min
 
      Returns the spot GEX exposures for the given ticker per minute.
 
     Spot GEX is the assumed $ value of the given greek (ie. gamma) exposure that market makers need to
@@ -132,15 +132,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     """Spot GEX exposures per 1min
 
      Returns the spot GEX exposures for the given ticker per minute.
 
     Spot GEX is the assumed $ value of the given greek (ie. gamma) exposure that market makers need to
@@ -195,15 +195,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     """Spot GEX exposures per 1min
 
      Returns the spot GEX exposures for the given ticker per minute.
 
     Spot GEX is the assumed $ value of the given greek (ie. gamma) exposure that market makers need to
@@ -261,15 +261,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, SpotGEXExposuresPer1MinResults, str]]:
     """Spot GEX exposures per 1min
 
      Returns the spot GEX exposures for the given ticker per minute.
 
     Spot GEX is the assumed $ value of the given greek (ie. gamma) exposure that market makers need to
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.spot_greek_exposures_by_strike import SpotGreekExposuresByStrike
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = SpotGreekExposuresByStrike.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     """Spot GEX exposures by strike
 
      Returns the most recent spot GEX exposures across all strikes for the given ticker on a given date.
     Calculated either with open interest or with volume.
 
@@ -133,15 +133,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     """Spot GEX exposures by strike
 
      Returns the most recent spot GEX exposures across all strikes for the given ticker on a given date.
     Calculated either with open interest or with volume.
 
@@ -197,15 +197,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     """Spot GEX exposures by strike
 
      Returns the most recent spot GEX exposures across all strikes for the given ticker on a given date.
     Calculated either with open interest or with volume.
 
@@ -264,15 +264,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, SpotGreekExposuresByStrike, str]]:
     """Spot GEX exposures by strike
 
      Returns the most recent spot GEX exposures across all strikes for the given ticker on a given date.
     Calculated either with open interest or with volume.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/api/stock/get_volatility_term_structure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/api/stock/get_volatility_term_structure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
-from ...client import AuthenticatedClient, Client
+from ...client import UnusualWhalesClient
 from ...models.error_message import ErrorMessage
 from ...models.implied_volatility_term_structure_results import ImpliedVolatilityTermStructureResults
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
@@ -28,15 +28,15 @@
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Optional[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     response_json = response.json()
     if response_json.get("data") is not None:
         response_json = response_json["data"]
     if response.status_code == HTTPStatus.OK:
         response_200 = ImpliedVolatilityTermStructureResults.from_dict(response.json())
 
@@ -51,28 +51,28 @@
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+    *, client: UnusualWhalesClient, response: httpx.Response
 ) -> Response[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     """Implied Volatility Term Structure
 
      The average of the latest volatilities for the at the money call and put contracts for every expiry
     date.
 
@@ -101,15 +101,15 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     """Implied Volatility Term Structure
 
      The average of the latest volatilities for the at the money call and put contracts for every expiry
     date.
 
@@ -133,15 +133,15 @@
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     """Implied Volatility Term Structure
 
      The average of the latest volatilities for the at the money call and put contracts for every expiry
     date.
 
@@ -168,15 +168,15 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: UnusualWhalesClient,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, ImpliedVolatilityTermStructureResults, str]]:
     """Implied Volatility Term Structure
 
      The average of the latest volatilities for the at the money call and put contracts for every expiry
     date.
```

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/client.py` & `unusualwhales_python_client-4.2.1/unusualwhales/client.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/errors.py` & `unusualwhales_python_client-4.2.1/unusualwhales/errors.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/__init__.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/analalyst_rating_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/analalyst_rating_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/analyst_rating.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/analyst_rating.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/candle_data.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/candle_data.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/candle_data_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/candle_data_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/congressional_trade_report.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/congressional_trade_report.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/congressional_trade_report_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/congressional_trade_report_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/country_sector_exposure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/country_sector_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/daily_market_tide.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/daily_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/daily_market_tide_response.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/daily_market_tide_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/darkpool_trade.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/darkpool_trade.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/darkpool_trade_response.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/darkpool_trade_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/earnings.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/earnings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/earnings_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/earnings_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/economic_calendar.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/error_message.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/error_message.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/etf_countries_item.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/etf_countries_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/etf_info.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/etf_info_data.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/etf_info_data.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/etf_sectors_item.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/etf_sectors_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/expiry_breakdown.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/expiry_breakdown_result.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/expiry_breakdown_result.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/fda_calendar.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_alert_rule.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_alert_rule.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_expiry_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/flow_per_strike_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/flow_per_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_by_strike_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_by_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greek_exposure_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greek_exposure_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/greeks.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/greeks.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/historical_risk_reversal_skew.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/historical_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/historical_risk_reversal_skew_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/historical_risk_reversal_skew_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/holdings.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/holdings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/holdings_response.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/holdings_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/imbalances_volume.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/imbalances_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/implied_volatility_term_structure.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/implied_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/implied_volatility_term_structure_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/implied_volatility_term_structure_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/insider_statistic.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/insider_statistic.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/insider_statistics.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/insider_statistics.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/market_general_sector.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/market_general_sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/market_holidays.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/market_holidays.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/market_options_volume.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/market_sector_ticker_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/market_sector_ticker_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/max_pain.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/max_pain.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/max_pain_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/max_pain_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/net_prem_tick.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/net_prem_tick.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/net_prem_tick_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/net_prem_tick_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/off_lit_price_level.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/off_lit_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/off_lit_price_level_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/off_lit_price_level_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/oi_change.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/oi_change.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/oi_change_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/oi_change_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_chain_contract.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_chain_contract.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_chain_contract_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_chain_contract_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_chains_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_chains_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_screener_item.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_screener_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_contract_screener_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_contract_screener_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_price_level.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/option_price_level_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/option_price_level_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/screener_contract_order_by_field.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/screener_contract_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/screener_order_by_field.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/screener_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_market.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_market.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_market_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_market_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_monthly.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_monthly.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_monthly_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_monthly_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_performers.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_performers.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_performers_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_performers_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_year_month.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_year_month.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/seasonality_year_month_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/seasonality_year_month_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/sector.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/sector_etf.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/sector_etf.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/sector_etf_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/sector_etf_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/single_sector.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/single_sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/spike_value.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/spike_value.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/spot_gex_exposures_per_1_min.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/spot_gex_exposures_per_1_min.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/spot_greek_exposures_by_strike.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/spot_greek_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/stock_screener_response.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/stock_screener_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/stock_screener_response_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/stock_screener_response_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_info.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_info_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_info_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/ticker_options_volume.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/ticker_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/volume_oi_per_expiry.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/volume_oi_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/models/volume_oi_per_expiry_results.py` & `unusualwhales_python_client-4.2.1/unusualwhales/models/volume_oi_per_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/unusualwhales/types.py` & `unusualwhales_python_client-4.2.1/unusualwhales/types.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.1.1/PKG-INFO` & `unusualwhales_python_client-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unusualwhales-python-client
-Version: 4.1.1
+Version: 4.2.1
 Summary: A client library for accessing Unusual Whales API
 Author: Mac Anderson
 Author-email: mac@macanderson.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -22,15 +22,15 @@
 
 
 ## Example Implementation
 ```python
 import os
 import decimal
 from dotenv import load_dotenv
-from unusualwhales import UnusualWhalesClient, UnusualWhalesApi
+from unusualwhales import UnusualWhalesClient, 
 
 from unusualwhales.models import OffLitPriceLevelResults, OffLitPriceLevel
 from unusualwhales.api.stock import get_volume_by_price_level
 
 load_dotenv('.env')
 UW_API_TOKEN = os.environ.get("UW_API_TOKEN", None)
```

