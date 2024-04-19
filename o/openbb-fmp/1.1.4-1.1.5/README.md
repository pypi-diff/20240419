# Comparing `tmp/openbb_fmp-1.1.4.tar.gz` & `tmp/openbb_fmp-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fmp-1.1.4.tar", max compression
+gzip compressed data, was "openbb_fmp-1.1.5.tar", max compression
```

## Comparing `openbb_fmp-1.1.4.tar` & `openbb_fmp-1.1.5.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0      478 2024-02-29 11:03:36.842618 openbb_fmp-1.1.4/README.md
--rw-r--r--   0        0        0     8111 2024-03-21 17:38:35.639684 openbb_fmp-1.1.4/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.842842 openbb_fmp-1.1.4/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-03-22 12:40:11.813669 openbb_fmp-1.1.4/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-03-21 17:38:35.639999 openbb_fmp-1.1.4/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-03-21 17:38:35.640233 openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-03-21 17:38:35.640374 openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-03-21 17:38:35.640519 openbb_fmp-1.1.4/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-03-21 17:38:35.640658 openbb_fmp-1.1.4/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-03-21 17:38:35.640811 openbb_fmp-1.1.4/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-03-21 17:38:35.640987 openbb_fmp-1.1.4/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-03-21 17:38:35.641081 openbb_fmp-1.1.4/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-03-22 12:40:11.813778 openbb_fmp-1.1.4/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-03-22 23:30:27.583357 openbb_fmp-1.1.4/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-03-21 17:38:35.641324 openbb_fmp-1.1.4/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-03-21 17:38:35.641450 openbb_fmp-1.1.4/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-03-21 17:38:35.641570 openbb_fmp-1.1.4/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-03-21 17:38:35.641674 openbb_fmp-1.1.4/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-03-21 17:38:35.641803 openbb_fmp-1.1.4/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6022 2024-03-13 16:36:51.716717 openbb_fmp-1.1.4/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-03-13 16:36:51.716848 openbb_fmp-1.1.4/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-03-21 17:38:35.641919 openbb_fmp-1.1.4/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-03-13 16:36:51.717093 openbb_fmp-1.1.4/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-03-21 17:38:35.642025 openbb_fmp-1.1.4/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-03-21 17:38:35.642174 openbb_fmp-1.1.4/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-03-21 17:38:35.642277 openbb_fmp-1.1.4/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-03-22 12:40:11.813889 openbb_fmp-1.1.4/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5202 2024-03-22 12:40:11.813998 openbb_fmp-1.1.4/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-03-21 17:38:35.642537 openbb_fmp-1.1.4/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-03-22 12:40:11.814104 openbb_fmp-1.1.4/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-03-22 12:40:11.814211 openbb_fmp-1.1.4/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-03-22 12:40:11.814334 openbb_fmp-1.1.4/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6763 2024-03-22 12:40:11.814453 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-03-21 17:38:35.643273 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2774 2024-03-21 17:38:35.643512 openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-03-22 12:40:11.814603 openbb_fmp-1.1.4/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-03-21 17:38:35.643652 openbb_fmp-1.1.4/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-03-21 17:38:35.643772 openbb_fmp-1.1.4/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-03-22 12:40:11.814715 openbb_fmp-1.1.4/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-03-22 12:40:11.814800 openbb_fmp-1.1.4/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     3771 2024-03-21 17:38:35.644149 openbb_fmp-1.1.4/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-03-21 17:38:35.644284 openbb_fmp-1.1.4/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-03-21 17:38:35.644395 openbb_fmp-1.1.4/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-03-21 17:38:35.644504 openbb_fmp-1.1.4/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-03-21 17:38:35.644732 openbb_fmp-1.1.4/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-03-21 17:38:35.644866 openbb_fmp-1.1.4/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-03-21 17:38:35.644977 openbb_fmp-1.1.4/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-03-21 17:38:35.645125 openbb_fmp-1.1.4/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-03-21 17:38:35.645341 openbb_fmp-1.1.4/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-03-21 17:38:35.645507 openbb_fmp-1.1.4/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2064 2024-03-21 17:38:35.645627 openbb_fmp-1.1.4/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-03-22 12:40:11.814898 openbb_fmp-1.1.4/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3903 2024-03-21 17:38:35.645747 openbb_fmp-1.1.4/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     5922 2024-03-21 17:38:35.645934 openbb_fmp-1.1.4/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3131 2024-03-22 12:40:11.815005 openbb_fmp-1.1.4/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-03-22 12:40:11.815106 openbb_fmp-1.1.4/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     2900 2024-03-22 12:40:11.815214 openbb_fmp-1.1.4/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847376 openbb_fmp-1.1.4/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-03-21 17:38:35.646414 openbb_fmp-1.1.4/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-03-21 17:38:35.646526 openbb_fmp-1.1.4/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-03-21 17:38:35.646630 openbb_fmp-1.1.4/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-03-21 17:38:35.646749 openbb_fmp-1.1.4/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-03-13 16:36:51.721845 openbb_fmp-1.1.4/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-03-13 16:36:51.721964 openbb_fmp-1.1.4/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847941 openbb_fmp-1.1.4/openbb_fmp/py.typed
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847991 openbb_fmp-1.1.4/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-03-13 16:36:51.722083 openbb_fmp-1.1.4/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4243 2024-03-22 12:40:11.815337 openbb_fmp-1.1.4/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.848164 openbb_fmp-1.1.4/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0      433 2024-04-01 14:20:54.437530 openbb_fmp-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_fmp-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      478 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/README.md
+-rw-r--r--   0        0        0     8255 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6076 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5308 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-04-17 12:33:20.649645 openbb_fmp-1.1.5/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6768 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-04-19 13:10:31.744034 openbb_fmp-1.1.5/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-04-19 13:10:31.744034 openbb_fmp-1.1.5/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-04-19 16:31:25.550563 openbb_fmp-1.1.5/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3521 2024-04-19 13:09:31.739184 openbb_fmp-1.1.5/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:33:20.653645 openbb_fmp-1.1.5/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0      433 2024-04-19 16:41:18.207237 openbb_fmp-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_fmp-1.1.5/PKG-INFO
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/__init__.py` & `openbb_fmp-1.1.5/openbb_fmp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from openbb_fmp.models.etf_holdings_date import FMPEtfHoldingsDateFetcher
 from openbb_fmp.models.etf_holdings_performance import FMPEtfHoldingsPerformanceFetcher
 from openbb_fmp.models.etf_info import FMPEtfInfoFetcher
 from openbb_fmp.models.etf_search import FMPEtfSearchFetcher
 from openbb_fmp.models.etf_sectors import FMPEtfSectorsFetcher
 from openbb_fmp.models.executive_compensation import FMPExecutiveCompensationFetcher
 from openbb_fmp.models.financial_ratios import FMPFinancialRatiosFetcher
+from openbb_fmp.models.forward_eps_estimates import FMPForwardEpsEstimatesFetcher
 from openbb_fmp.models.historical_dividends import FMPHistoricalDividendsFetcher
 from openbb_fmp.models.historical_employees import FMPHistoricalEmployeesFetcher
 from openbb_fmp.models.historical_eps import FMPHistoricalEpsFetcher
 from openbb_fmp.models.historical_splits import FMPHistoricalSplitsFetcher
 from openbb_fmp.models.income_statement import FMPIncomeStatementFetcher
 from openbb_fmp.models.income_statement_growth import FMPIncomeStatementGrowthFetcher
 from openbb_fmp.models.index_constituents import FMPIndexConstituentsFetcher
@@ -104,14 +105,15 @@
         "EtfHoldingsPerformance": FMPEtfHoldingsPerformanceFetcher,
         "EtfInfo": FMPEtfInfoFetcher,
         "EtfPricePerformance": FMPPricePerformanceFetcher,
         "EtfSearch": FMPEtfSearchFetcher,
         "EtfSectors": FMPEtfSectorsFetcher,
         "ExecutiveCompensation": FMPExecutiveCompensationFetcher,
         "FinancialRatios": FMPFinancialRatiosFetcher,
+        "ForwardEpsEstimates": FMPForwardEpsEstimatesFetcher,
         "HistoricalDividends": FMPHistoricalDividendsFetcher,
         "HistoricalEmployees": FMPHistoricalEmployeesFetcher,
         "HistoricalEps": FMPHistoricalEpsFetcher,
         "HistoricalSplits": FMPHistoricalSplitsFetcher,
         "IncomeStatement": FMPIncomeStatementFetcher,
         "IncomeStatementGrowth": FMPIncomeStatementGrowthFetcher,
         "IndexConstituents": FMPIndexConstituentsFetcher,
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/analyst_estimates.py` & `openbb_fmp-1.1.5/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/available_indices.py` & `openbb_fmp-1.1.5/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet.py` & `openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/balance_sheet_growth.py` & `openbb_fmp-1.1.5/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/calendar_dividend.py` & `openbb_fmp-1.1.5/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/calendar_earnings.py` & `openbb_fmp-1.1.5/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/calendar_splits.py` & `openbb_fmp-1.1.5/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/cash_flow.py` & `openbb_fmp-1.1.5/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/cash_flow_growth.py` & `openbb_fmp-1.1.5/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/company_filings.py` & `openbb_fmp-1.1.5/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/company_news.py` & `openbb_fmp-1.1.5/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/company_overview.py` & `openbb_fmp-1.1.5/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/crypto_historical.py` & `openbb_fmp-1.1.5/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/crypto_search.py` & `openbb_fmp-1.1.5/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/currency_historical.py` & `openbb_fmp-1.1.5/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/currency_pairs.py` & `openbb_fmp-1.1.5/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/currency_snapshots.py` & `openbb_fmp-1.1.5/openbb_fmp/models/currency_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """FMP Currency Snapshots Model."""
 
 # pylint: disable=unused-argument
 
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_snapshots import (
     CurrencySnapshotsData,
     CurrencySnapshotsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from pandas import DataFrame, concat
 from pydantic import Field, field_validator
 
 
 class FMPCurrencySnapshotsQueryParams(CurrencySnapshotsQueryParams):
     """FMP Currency Snapshots Query.
 
@@ -81,29 +84,27 @@
     @staticmethod
     async def aextract_data(
         query: FMPCurrencySnapshotsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the data from the FMP endpoint."""
-
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         url = f"https://financialmodelingprep.com/api/v3/quotes/forex?apikey={api_key}"
 
         return await amake_request(url, **kwargs)  # type: ignore
 
     @staticmethod
     def transform_data(
         query: FMPCurrencySnapshotsQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPCurrencySnapshotsData]:
         """Filter by the query parameters and validate the model."""
-
         if not data:
             raise EmptyDataError("No data was returned from the FMP endpoint.")
 
         # Drop all the zombie columns FMP returns.
         df = (
             DataFrame(data)
             .dropna(how="all", axis=1)
@@ -139,15 +140,15 @@
                     .filter(items=counter_currencies, axis=0)
                     .reset_index()
                 )
             # If there are no records, don't concatenate.
             if len(temp) > 0:
                 # Convert the Unix timestamp to a datetime.
                 temp.timestamp = temp.timestamp.apply(
-                    lambda x: datetime.fromtimestamp(x)
+                    lambda x: safe_fromtimestamp(x, tz=timezone.utc)
                 )
                 new_df = concat([new_df, temp])
             if len(new_df) == 0:
                 raise EmptyDataError(
                     "No data was found using the applied filters. Check the parameters."
                 )
             # Fill and replace any NaN values with NoneType.
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/discovery_filings.py` & `openbb_fmp-1.1.5/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/earnings_call_transcript.py` & `openbb_fmp-1.1.5/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/economic_calendar.py` & `openbb_fmp-1.1.5/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_historical.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_ownership.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_peers.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_profile.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_quote.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_quote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """FMP Equity Quote Model."""
 
+# pylint: disable=unused-argument
+
 import asyncio
-from datetime import datetime, timezone
-from typing import Any, Dict, List, Optional
+from datetime import (
+    date as dateType,
+    datetime,
+    timezone,
+)
+from typing import Any, Dict, List, Optional, Union
 from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_quote import (
     EquityQuoteData,
     EquityQuoteQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
-from openbb_core.provider.utils.helpers import amake_request
+from openbb_core.provider.utils.helpers import amake_request, safe_fromtimestamp
 from openbb_fmp.utils.helpers import get_querystring, response_callback
 from pydantic import Field, field_validator
 
 
 class FMPEquityQuoteQueryParams(EquityQuoteQueryParams):
     """FMP Equity Quote Query.
 
@@ -59,30 +65,30 @@
     pe: Optional[float] = Field(default=None, description="Price earnings ratio.")
     earnings_announcement: Optional[datetime] = Field(
         default=None, description="Upcoming earnings announcement date."
     )
 
     @field_validator("last_timestamp", mode="before", check_fields=False)
     @classmethod
-    def validate_last_timestamp(cls, v):  # pylint: disable=E0213
+    def validate_last_timestamp(cls, v: Union[str, int]) -> Optional[dateType]:
         """Return the date as a datetime object."""
         if v:
             v = int(v) if isinstance(v, str) else v
-            return datetime.fromtimestamp(int(v), tz=timezone.utc)
+            return safe_fromtimestamp(v, tz=timezone.utc)
         return None
 
     @field_validator("earnings_announcement", mode="before", check_fields=False)
     @classmethod
-    def timestamp_validate(cls, v):  # pylint: disable=E0213
+    def timestamp_validate(cls, v: str) -> Optional[dateType]:
         """Return the datetime string as a datetime object."""
         if v:
             dt = datetime.strptime(v, "%Y-%m-%dT%H:%M:%S.%f%z")
             dt = dt.replace(microsecond=0)
             timestamp = dt.timestamp()
-            return datetime.fromtimestamp(timestamp, tz=timezone.utc)
+            return safe_fromtimestamp(timestamp, tz=timezone.utc)
         return None
 
     @field_validator("change_percent", mode="after", check_fields=False)
     @classmethod
     def normalize_percent(cls, v):  # pylint: disable=E0213
         """Return the percent value as a normalized value."""
         return float(v) / 100 if v else None
@@ -111,15 +117,15 @@
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         symbols = query.symbol.split(",")
 
-        results = []
+        results: list = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = f"{base_url}/quote/{symbol}?{query_str}&apikey={api_key}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
             )
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_screener.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_fmp-1.1.5/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_countries.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_equity_exposure.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         return float(v) / 100 if v else None
 
     @field_validator("cusip", "isin", "balance", "name", "symbol", "value")
     @classmethod
     def replace_empty(cls, v):
         """Replace empty strings and 0s with None."""
         if isinstance(v, str):
-            return v if v not in ("", "0") else None
+            return v if v not in ("", "0", "-") else None
         if isinstance(v, (float, int)):
             return v if v and v not in (0.0, 0) else None
         return v if v else None
 
 
 class FMPEtfHoldingsFetcher(
     Fetcher[
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_date.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_holdings_performance.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_holdings_performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         )
         if holdings is None:
             raise RuntimeError(f"No holdings data found for {query.symbol}.")
         holdings_list = DataFrame(holdings).asset.unique().tolist()
         # Split into chunks of 500
         chunks = [holdings_list[i : i + 500] for i in range(0, len(holdings_list), 500)]
         # Get price performance for the holdings
-        holdings_performance: list = []
+        holdings_performance: List[Dict] = []
         for holding_chunk in chunks:
             holdings_str = (
                 ",".join(holding_chunk) if len(holding_chunk) > 1 else holding_chunk[0]
             )
             _performance = await FMPPricePerformanceFetcher().aextract_data(
                 FMPPricePerformanceFetcher.transform_query({"symbol": holdings_str}),
                 credentials,
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_info.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_search.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/etf_sectors.py` & `openbb_fmp-1.1.5/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/executive_compensation.py` & `openbb_fmp-1.1.5/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/financial_ratios.py` & `openbb_fmp-1.1.5/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/historical_dividends.py` & `openbb_fmp-1.1.5/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/historical_employees.py` & `openbb_fmp-1.1.5/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/historical_eps.py` & `openbb_fmp-1.1.5/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/historical_splits.py` & `openbb_fmp-1.1.5/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/income_statement.py` & `openbb_fmp-1.1.5/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/income_statement_growth.py` & `openbb_fmp-1.1.5/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/index_constituents.py` & `openbb_fmp-1.1.5/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/index_historical.py` & `openbb_fmp-1.1.5/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/insider_trading.py` & `openbb_fmp-1.1.5/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/institutional_ownership.py` & `openbb_fmp-1.1.5/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/key_executives.py` & `openbb_fmp-1.1.5/openbb_fmp/models/key_executives.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """FMP Key Executives Model."""
 
-from datetime import datetime
-from typing import Any, Dict, List, Optional
+# pylint: disable=unused-argument
+
+from datetime import (
+    date as dateType,
+)
+from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.key_executives import (
     KeyExecutivesData,
     KeyExecutivesQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_fmp.utils.helpers import get_data_many
 from pydantic import field_validator
 
 
 class FMPKeyExecutivesQueryParams(KeyExecutivesQueryParams):
     """FMP Key Executives Query.
 
@@ -20,17 +25,20 @@
 
 
 class FMPKeyExecutivesData(KeyExecutivesData):
     """FMP Key Executives Data."""
 
     @field_validator("titleSince", mode="before", check_fields=False)
     @classmethod
-    def time_validate(cls, v):  # pylint: disable=E0213
+    def time_validate(cls, v: Union[float, int]) -> Optional[dateType]:
         """Return the date as a datetime object."""
-        return datetime.fromtimestamp(v / 1000)
+        if v:
+            v = v / 1000
+            return safe_fromtimestamp(v)
+        return v  # type: ignore
 
 
 class FMPKeyExecutivesFetcher(
     Fetcher[
         FMPKeyExecutivesQueryParams,
         List[FMPKeyExecutivesData],
     ]
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/key_metrics.py` & `openbb_fmp-1.1.5/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/market_indices.py` & `openbb_fmp-1.1.5/openbb_fmp/models/market_indices.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """FMP Market Indices Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
 
 from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_indices import (
     MarketIndicesData,
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/market_snapshots.py` & `openbb_fmp-1.1.5/openbb_fmp/models/market_snapshots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """FMP Market Snapshots Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import (
     date as dateType,
     datetime,
+    timezone,
 )
 from typing import Any, Dict, List, Optional, Union
 
 from dateutil import parser
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.market_snapshots import (
     MarketSnapshotsData,
     MarketSnapshotsQueryParams,
 )
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
 from openbb_fmp.utils.definitions import EXCHANGES
 from openbb_fmp.utils.helpers import get_data
 from pydantic import Field, field_validator
 
 
 class FMPMarketSnapshotsQueryParams(MarketSnapshotsQueryParams):
     """FMP Market Snapshots Query.
@@ -83,22 +87,28 @@
         description="The upcoming earnings announcement date.",
         alias="earningsAnnouncement",
         default=None,
     )
 
     @field_validator("last_price_timestamp", mode="before", check_fields=False)
     @classmethod
-    def validate_timestamp(cls, v):
+    def validate_timestamp(cls, v: Union[str, int, float]) -> Optional[dateType]:
         """Validate the timestamp."""
+        if isinstance(v, str):
+            try:
+                v = float(v)
+            except ValueError:
+                return None
+
         if isinstance(v, (int, float)) and v != 0:
             try:
-                v = datetime.fromtimestamp(v)
-                if v.hour == 0 and v.minute == 0 and v.second == 0:
-                    v = v.date()
-                return v
+                v = safe_fromtimestamp(v, tz=timezone.utc)  # type: ignore
+                if v.hour == 0 and v.minute == 0 and v.second == 0:  # type: ignore
+                    v = v.date()  # type: ignore
+                return v  # type: ignore
             except ValueError:
                 return None
         return None
 
     @field_validator("earnings_date", mode="before", check_fields=False)
     @classmethod
     def date_validate(cls, v):  # pylint: disable=E0213
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/price_performance.py` & `openbb_fmp-1.1.5/openbb_fmp/models/price_performance.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.recent_performance import (
     RecentPerformanceData,
     RecentPerformanceQueryParams,
 )
-from openbb_fmp.utils.helpers import create_url, get_data_many
+from openbb_fmp.utils.helpers import create_url, get_data_urls
 from pydantic import Field, model_validator
 
 
 class FMPPricePerformanceQueryParams(RecentPerformanceQueryParams):
     """FMP Price Performance Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/stock-split-calendar-api/
@@ -67,32 +67,42 @@
     async def aextract_data(
         query: FMPPricePerformanceQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
-
-        url = create_url(
-            version=3,
-            endpoint=f"stock-price-change/{query.symbol}",
-            api_key=api_key,
-            exclude=["symbol"],
-        )
-        return await get_data_many(url, **kwargs)
+        symbols = query.symbol.upper().split(",")
+        symbols = list(dict.fromkeys(symbols))
+        chunk_size = 200
+        chunks = [
+            symbols[i : i + chunk_size] for i in range(0, len(symbols), chunk_size)
+        ]
+        urls = [
+            create_url(
+                version=3,
+                endpoint=f"stock-price-change/{','.join(chunk)}",
+                api_key=api_key,
+                exclude=["symbol"],
+            )
+            for chunk in chunks
+        ]
+        data = await get_data_urls(urls, **kwargs)
+        return data
 
     @staticmethod
     def transform_data(
         query: FMPPricePerformanceQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FMPPricePerformanceData]:
         """Return the transformed data."""
 
-        symbols = query.symbol.split(",")
+        symbols = query.symbol.upper().split(",")
+        symbols = list(dict.fromkeys(symbols))
         if len(data) != len(symbols):
             data_symbols = [d["symbol"] for d in data]
             missing_symbols = [
                 symbol for symbol in symbols if symbol not in data_symbols
             ]
             warn(f"Missing data for symbols: {missing_symbols}")
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/price_target.py` & `openbb_fmp-1.1.5/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/price_target_consensus.py` & `openbb_fmp-1.1.5/openbb_fmp/models/price_target_consensus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 """FMP Price Target Consensus Model."""
 
+# pylint: disable=unused-argument
+
 import asyncio
 from typing import Any, Dict, List, Optional
 from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.price_target_consensus import (
     PriceTargetConsensusData,
     PriceTargetConsensusQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_fmp.utils.helpers import create_url, response_callback
+from pydantic import field_validator
 
 
 class FMPPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """FMP Price Target Consensus Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/price-target-consensus-api/
     """
 
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def check_symbol(cls, value):
+        """Check the symbol."""
+        if not value:
+            raise RuntimeError("Error: Symbol is a required field for FMP.")
+        return value
+
 
 class FMPPriceTargetConsensusData(PriceTargetConsensusData):
     """FMP Price Target Consensus Data."""
 
 
 class FMPPriceTargetConsensusFetcher(
     Fetcher[
@@ -45,16 +56,16 @@
         query: FMPPriceTargetConsensusQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
-        symbols = query.symbol.split(",")
-        results = []
+        symbols = query.symbol.split(",")  # type: ignore
+        results: List[Dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = create_url(
                 4, "price-target-consensus", api_key, query, exclude=["symbol"]
             )
             url = f"{url}&symbol={symbol}"
```

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/revenue_business_line.py` & `openbb_fmp-1.1.5/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/revenue_geographic.py` & `openbb_fmp-1.1.5/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/risk_premium.py` & `openbb_fmp-1.1.5/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/share_statistics.py` & `openbb_fmp-1.1.5/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/treasury_rates.py` & `openbb_fmp-1.1.5/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/models/world_news.py` & `openbb_fmp-1.1.5/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/utils/definitions.py` & `openbb_fmp-1.1.5/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.1.4/openbb_fmp/utils/helpers.py` & `openbb_fmp-1.1.5/openbb_fmp/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 )
 from pydantic import BaseModel
 
 
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[Dict, List[Dict]]:
-    """Callback for make_request."""
-
+    """Use callback for make_request."""
     data = await response.json()
     if isinstance(data, dict) and "Error Message" in data:
         raise RuntimeError(f"FMP Error Message -> {data['Error Message']}")
 
     if isinstance(data, dict) and "error" in data:
         raise RuntimeError(
             f"FMP Error Message -> {data['error']}. Status code: {response.status}"
```

### Comparing `openbb_fmp-1.1.4/PKG-INFO` & `openbb_fmp-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-fmp
-Version: 1.1.4
+Version: 1.1.5
 Summary: FMP extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Financial Modeling Prep Provider
 
 This extension integrates the [Financial Modeling Prep](https://site.financialmodelingprep.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

