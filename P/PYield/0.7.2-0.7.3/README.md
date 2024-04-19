# Comparing `tmp/pyield-0.7.2.tar.gz` & `tmp/pyield-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.2.tar", last modified: Wed Apr 17 08:53:02 2024, max compression
+gzip compressed data, was "pyield-0.7.3.tar", last modified: Fri Apr 19 11:13:54 2024, max compression
```

## Comparing `pyield-0.7.2.tar` & `pyield-0.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.2/LICENSE
--rw-r--r--   0        0        0     5168 2024-04-16 12:01:55.675922 pyield-0.7.2/README.md
--rw-r--r--   0        0        0       22 2024-04-17 08:50:38.480980 pyield-0.7.2/pyield/__about__.py
--rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.2/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.2/pyield/bday.py
--rw-r--r--   0        0        0     3446 2024-04-16 12:01:55.675922 pyield-0.7.2/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.2/pyield/data_analysis.py
--rw-r--r--   0        0        0      223 2024-04-16 12:01:55.675922 pyield-0.7.2/pyield/futures/__init__.py
--rw-r--r--   0        0        0     5615 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/common.py
--rw-r--r--   0        0        0     5816 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/ddi.py
--rw-r--r--   0        0        0     5847 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/di.py
--rw-r--r--   0        0        0    11530 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/futures/di_xml.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.2/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.2/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.2/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.2/pyield/holidays/core.py
--rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.2/pyield/indicators.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.2/pyield/py.typed
--rw-r--r--   0        0        0     6612 2024-04-16 12:01:55.676922 pyield-0.7.2/pyield/treasuries.py
--rw-r--r--   0        0        0     2111 2024-04-14 09:43:03.423065 pyield-0.7.2/pyield/utils.py
--rw-r--r--   0        0        0     1165 2024-04-17 08:53:02.132938 pyield-0.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.2/tests/test_bday.py
--rw-r--r--   0        0        0     2554 2024-04-16 12:01:55.677922 pyield-0.7.2/tests/test_futures.py
--rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 pyield-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5177 2024-04-19 11:12:40.008362 pyield-0.7.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/__about__.py
+-rw-r--r--   0        0        0      380 2024-04-14 09:19:55.868897 pyield-0.7.3/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.3/pyield/bday.py
+-rw-r--r--   0        0        0     3625 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.3/pyield/data_analysis.py
+-rw-r--r--   0        0        0      289 2024-04-19 11:12:40.008362 pyield-0.7.3/pyield/futures/__init__.py
+-rw-r--r--   0        0        0     7483 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/common.py
+-rw-r--r--   0        0        0     5810 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     7272 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/di.py
+-rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.3/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.3/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.3/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.3/pyield/holidays/core.py
+-rw-r--r--   0        0        0     2273 2024-04-14 11:04:04.016185 pyield-0.7.3/pyield/indicators.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.3/pyield/py.typed
+-rw-r--r--   0        0        0     6622 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/treasuries.py
+-rw-r--r--   0        0        0     2142 2024-04-19 11:12:40.009362 pyield-0.7.3/pyield/utils.py
+-rw-r--r--   0        0        0     1165 2024-04-19 11:13:54.665452 pyield-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.3/tests/test_bday.py
+-rw-r--r--   0        0        0     2581 2024-04-19 11:12:40.009362 pyield-0.7.3/tests/test_futures.py
+-rw-r--r--   0        0        0     7194 1970-01-01 00:00:00.000000 pyield-0.7.3/PKG-INFO
```

### Comparing `pyield-0.7.2/LICENSE` & `pyield-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/README.md` & `pyield-0.7.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,22 +55,22 @@
 ```
 
 ### Futures Data
 ```python
 # Fetch a DataFrame with the DI Futures data from B3
 >>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 
-TradeDate  ExpirationCode ExpirationDate BDaysToExpiration ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
-2024-03-08 K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
-2024-03-08 M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
+TradeDate  TickerSymbol ExpirationDate BDaysToExp ... LastRate LastAskRate LastBidRate SettlementRate
+2024-03-08 DI1J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
+2024-03-08 DI1K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
+2024-03-08 DI1M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
 ...        ...            ...            ...               ... ...      ...         ...         ...
-2024-03-08 F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
+2024-03-08 DI1F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 DI1F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 DI1F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
```

### Comparing `pyield-0.7.2/pyield/bday.py` & `pyield-0.7.3/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/data_access.py` & `pyield-0.7.3/pyield/data_access.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Supported options:
             - "TRB": Treasury bonds (indicative rates from ANBIMA).
             - "LTN", "LFT", "NTN-F", "NTN-B": Specific types of Brazilian treasury bonds
                   (indicative rates from ANBIMA).
             - "DI1": One-day Interbank Deposit Futures (Futuro de DI) from B3.
             - "DDI": DI x U.S. Dollar Spread Futures (Futuro de Cupom Cambial) from B3.
         reference_date (str | pd.Timestamp | None): The reference date for which data is
-            fetched. Defaults to the previous business day if None.
+            fetched. Defaults to the last business day if None.
         **kwargs: Additional keyword arguments, specifically:
             - return_raw (bool): Whether to return raw data without processing. Defaults
               to False.
 
     Returns:
         pd.DataFrame: A DataFrame containing the fetched data for the specified asset.
 
@@ -44,15 +44,21 @@
     if asset_code.lower() == "trb":
         return tr.fetch_bonds(reference_date=normalized_date, return_raw=return_raw)
     elif asset_code.lower() in ["ltn", "lft", "ntn-f", "ntn-b"]:
         df = tr.fetch_bonds(reference_date=normalized_date)
         return df.query(f"BondType == '{asset_code.upper()}'")
 
     elif asset_code.lower() == "di1":
-        return ft.fetch_di(trade_date=normalized_date, return_raw=return_raw)
+        today = pd.Timestamp.today().normalize()
+        if normalized_date == today:
+            return ft.fetch_last_di_data()
+        else:
+            return ft.fetch_past_di_data(
+                trade_date=normalized_date, return_raw=return_raw
+            )
     elif asset_code.lower() == "ddi":
         return ft.fetch_ddi(trade_date=normalized_date, return_raw=return_raw)
     else:
         raise ValueError("Asset type not supported.")
 
 
 def fetch_indicator(
@@ -63,15 +69,15 @@
     Fetches data for a specified economic indicator and reference date.
 
     Args:
         indicator_code (str): The code for the economic indicator. Supported options:
             - "SELIC": SELIC target rate from the Central Bank of Brazil.
             - "IPCA": IPCA monthly inflation rate from IBGE.
         reference_date (str | pd.Timestamp | None): The reference date for which data is
-            fetched. Defaults to the previous business day if None.
+            fetched. Defaults to the last business day if None.
 
     Returns:
         pd.Series: A Series containing the fetched data for the specified indicator.
 
     Raises:
         ValueError: If the indicator code is not recognized or supported.
```

### Comparing `pyield-0.7.2/pyield/data_analysis.py` & `pyield-0.7.3/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/futures/common.py` & `pyield-0.7.3/pyield/futures/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -127,20 +127,20 @@
         # Must use old holiday list, since this contract code was used until 2006.
         return bday.offset_bdays(expiration_date, offset=0, holiday_list="old")
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
-def _fetch_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
+def fetch_past_data(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
-    Internal function to fetch raw DI futures data from B3 for a specific trade date.
+    Fetch the historical futures data from B3 for a specific trade date.
 
     Args:
-        trade_date: a datetime-like object representing the trade date.
+        trade_date (pd.Timestamp): The trade date for which the data should be fetched.
 
     Returns:
         pd.DataFrame: Raw DI data as a Pandas pd.DataFrame.
     """
     url_date = trade_date.strftime("%d/%m/%Y")
     # url example: https://www2.bmf.com.br/pages/portal/bmfbovespa/boletim1/SistemaPregao_excel1.asp?Data=05/10/2023&Mercadoria=DI1
     url = f"https://www2.bmf.com.br/pages/portal/bmfbovespa/boletim1/SistemaPregao_excel1.asp?Data={url_date}&Mercadoria={asset_code}&XLS=false"
@@ -169,7 +169,60 @@
     # Force "VAR. PTOS." to be string, since it can also be read as float
     df["VAR. PTOS."] = df["VAR. PTOS."].astype(pd.StringDtype())
 
     # Force "AJUSTE CORRIG. (4)" to be float, since it can be also read as int
     df["AJUSTE CORRIG. (4)"] = df["AJUSTE CORRIG. (4)"].astype(pd.Float64Dtype())
 
     return df
+
+
+def fetch_last_data(future_code: str) -> pd.DataFrame:
+    """
+    Fetch the latest data for a given future code from B3 derivatives quotation API.
+
+    Args:
+    future_code (str): The future code to fetch data for.
+
+    Returns:
+    pd.DataFrame: A DataFrame containing the normalized and cleaned data from the API.
+
+    Raises:
+    Exception: An exception is raised if the data fetch operation fails.
+    """
+
+    url = f"https://cotacao.b3.com.br/mds/api/v1/DerivativeQuotation/{future_code}"
+
+    try:
+        r = requests.get(url)
+        r.raise_for_status()  # Check for HTTP request errors
+    except requests.exceptions.RequestException:
+        raise Exception(f"Failed to fetch data for {future_code}.") from None
+
+    r.encoding = "utf-8"  # Explicitly set response encoding to utf-8 for consistency
+
+    # Normalize JSON response into a flat table
+    df = pd.json_normalize(r.json()["Scty"])
+
+    # Clean and reformat the DataFrame columns
+    df.columns = (df.columns
+        .str.replace("SctyQtn.", "")
+        .str.replace("asset.AsstSummry.", "")
+    )  # fmt: skip
+    df.drop(columns=["desc", "asset.code", "mkt.cd"], inplace=True)
+
+    # Convert maturity codes to datetime and drop rows with missing values
+    df["mtrtyCode"] = pd.to_datetime(df["mtrtyCode"], errors="coerce")
+    df.dropna(subset=["mtrtyCode"], inplace=True)
+
+    # Sort the DataFrame by maturity code and reset the index
+    df.sort_values("mtrtyCode", inplace=True, ignore_index=True)
+
+    # Get current date and time
+    now = pd.Timestamp.now().round("s")
+    # Subtract 15 minutes from the current time to account for API delay
+    trade_ts = now - pd.Timedelta(minutes=15)
+    df["TradeTimestamp"] = trade_ts
+
+    # Convert DataFrame to use nullable data types for better type consistency
+    df = df.convert_dtypes(dtype_backend="numpy_nullable")
+
+    return df
```

### Comparing `pyield-0.7.2/pyield/futures/ddi.py` & `pyield-0.7.3/pyield/futures/ddi.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     if df.empty:
         return df
 
     rename_dict = {
         "VENCTO": "ExpirationCode",
         "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
         "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
-        "NÚM. NEGOC.": "NumOfTrades",
-        "CONTR. NEGOC.": "TradedQuantity",
+        "NÚM. NEGOC.": "TradeCount",
+        "CONTR. NEGOC.": "TradeVolume",
         "VOL.": "FinancialVolume",
         "AJUSTE": "SettlementPrice",
         "AJUSTE ANTER. (3)": "PrevSettlementRate",
         "AJUSTE CORRIG. (4)": "AdjSettlementRate",
         "PREÇO MÍN.": "MinRate",
         "PREÇO MÉD.": "AvgRate",
         "PREÇO MÁX.": "MaxRate",
@@ -129,16 +129,16 @@
         "TradeDate",
         "ExpirationCode",
         "ExpirationDate",
         "DaysToExpiration",
         "OpenContracts",
         # "OpenContractsEndSession" since there is no OpenContracts at the end of the
         # day in XML data, it will be removed to avoid confusion with XML data
-        "NumOfTrades",
-        "TradedQuantity",
+        "TradeCount",
+        "TradeVolume",
         "FinancialVolume",
         "SettlementPrice",
         "MinRate",
         "AvgRate",
         "MaxRate",
         "FirstRate",
         "LastRate",
@@ -168,11 +168,11 @@
         >>> from pyield.futures import di
         >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
 
     Notes:
         - DaysToExpiration: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common._fetch_raw_df(asset_code="DDI", trade_date=trade_date)
+    df_raw = common.fetch_past_data(asset_code="DDI", trade_date=trade_date)
     if return_raw:
         return df_raw
     return _process_raw_df(df_raw, trade_date)
```

### Comparing `pyield-0.7.2/pyield/futures/di.py` & `pyield-0.7.3/pyield/futures/di.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 def _convert_prices_in_older_contracts(df: pd.DataFrame) -> pd.DataFrame:
     # Prior to 01/01/2002, prices were not converted to rates
     convert_cols = [
         "FirstRate",
         "MinRate",
         "MaxRate",
         "AvgRate",
-        "LastRate",
-        "LastBidRate",
-        "LastAskRate",
+        "CloseRate",
+        "CloseBidRate",
+        "CloseAskRate",
     ]
     for col in convert_cols:
-        df[col] = _convert_prices_to_rates(df[col], df["BDaysToExpiration"])
+        df[col] = _convert_prices_to_rates(df[col], df["BDaysToExp"])
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _process_past_data(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
@@ -56,29 +56,29 @@
     if df.empty:
         return df
 
     rename_dict = {
         "VENCTO": "ExpirationCode",
         "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
         "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
-        "NÚM. NEGOC.": "NumOfTrades",
-        "CONTR. NEGOC.": "TradedQuantity",
+        "NÚM. NEGOC.": "TradeCount",
+        "CONTR. NEGOC.": "TradeVolume",
         "VOL.": "FinancialVolume",
         "AJUSTE": "SettlementPrice",
         "AJUSTE ANTER. (3)": "PrevSettlementRate",
         "AJUSTE CORRIG. (4)": "AdjSettlementRate",
         "PREÇO MÍN.": "MinRate",
         "PREÇO MÉD.": "AvgRate",
         "PREÇO MÁX.": "MaxRate",
         "PREÇO ABERTU.": "FirstRate",
-        "ÚLT. PREÇO": "LastRate",
+        "ÚLT. PREÇO": "CloseRate",
         "VAR. PTOS.": "PointsVariation",
         # Attention: bid/ask rates are inverted
-        "ÚLT.OF. COMPRA": "LastAskRate",
-        "ÚLT.OF. VENDA": "LastBidRate",
+        "ÚLT.OF. COMPRA": "CloseAskRate",
+        "ÚLT.OF. VENDA": "CloseBidRate",
     }
 
     df = df.rename(columns=rename_dict)
 
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
@@ -87,74 +87,125 @@
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
             common.get_old_expiration_date, args=(trade_date,)
         )
     else:
         df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
 
-    df["BDaysToExpiration"] = bday.count_bdays(trade_date, df["ExpirationDate"])
-    # Convert to nullable integer, since other columns use this data type
-    df["BDaysToExpiration"] = df["BDaysToExpiration"].astype(pd.Int64Dtype())
+    df["BDaysToExp"] = bday.count_bdays(trade_date, df["ExpirationDate"])
     # Remove expired contracts
-    df.query("BDaysToExpiration > 0", inplace=True)
+    df.query("BDaysToExp > 0", inplace=True)
 
     # Columns where 0 means NaN
     cols_with_nan = [
         "SettlementPrice",
         "FirstRate",
         "MinRate",
         "MaxRate",
         "AvgRate",
-        "LastRate",
-        "LastBidRate",
-        "LastAskRate",
+        "CloseRate",
+        "CloseBidRate",
+        "CloseAskRate",
     ]
     for col in cols_with_nan:
         df[col] = df[col].replace(0, pd.NA)
 
     # Prior to 17/01/2002 (incluive), prices were not converted to rates
     if trade_date <= pd.Timestamp("2002-01-17"):
         df = _convert_prices_in_older_contracts(df)
 
     df["SettlementRate"] = _convert_prices_to_rates(
-        df["SettlementPrice"], df["BDaysToExpiration"]
+        df["SettlementPrice"], df["BDaysToExp"]
     )
 
     # Remove percentage in all rate columns and round to 5 decimal places since it's the
     # precision used by B3. Obs: 5 decimal places = 3 decimal places in percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
     for col in rate_cols:
         df[col] = (df[col] / 100).round(5)
 
+    df["TickerSymbol"] = "DI1" + df["ExpirationCode"]
+
     # Filter and order columns
     ordered_cols = [
         "TradeDate",
-        "ExpirationCode",
+        "TickerSymbol",
+        # "ExpirationCode",
         "ExpirationDate",
-        "BDaysToExpiration",
+        "BDaysToExp",
         "OpenContracts",
         # "OpenContractsEndSession" since there is no OpenContracts at the end of the
         # day in XML data, it will be removed to avoid confusion with XML data
-        "NumOfTrades",
-        "TradedQuantity",
+        "TradeCount",
+        "TradeVolume",
         "FinancialVolume",
         "SettlementPrice",
+        "SettlementRate",
+        "FirstRate",
         "MinRate",
         "AvgRate",
         "MaxRate",
-        "FirstRate",
-        "LastRate",
-        "LastAskRate",
-        "LastBidRate",
-        "SettlementRate",
+        "CloseAskRate",
+        "CloseBidRate",
+        "CloseRate",
     ]
     return df[ordered_cols]
 
 
-def fetch_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def _process_last_di_data(raw_df: pd.DataFrame) -> pd.DataFrame:
+    df = raw_df.copy()
+
+    # Columns to be renamed
+    rename_columns = {
+        "TradeTimestamp": "TradeTimestamp",
+        "symb": "TickerSymbol",
+        "mtrtyCode": "ExpirationDate",
+        "BDaysToExp": "BDaysToExp",
+        "opnCtrcts": "OpenContracts",
+        "tradQty": "TradeCount",
+        "traddCtrctsQty": "TradeVolume",
+        "grssAmt": "FinancialVolume",
+        "prvsDayAdjstmntPric": "PrevSettlementRate",
+        "bottomLmtPric": "MinLimitRate",
+        "topLmtPric": "MaxLimitRate",
+        "opngPric": "OpenRate",
+        "minPric": "MinRate",
+        "avrgPric": "AvgRate",
+        "maxPric": "MaxRate",
+        "buyOffer.price": "LastAskRate",
+        "sellOffer.price": "LastBidRate",
+        "curPrc": "LastRate",
+    }
+    # Rename columns
+    df = df.rename(columns=rename_columns)
+
+    df["BDaysToExp"] = bday.count_bdays(df["TradeTimestamp"], df["ExpirationDate"])
+
+    # Remove percentage in all rate columns
+    rate_cols = [col for col in df.columns if "Rate" in col]
+    df[rate_cols] = df[rate_cols] / 100
+
+    # Reorder columns based on the order of the dictionary
+    return df[rename_columns.values()]
+
+
+def fetch_last_di_data() -> pd.DataFrame:
+    """
+    Fetch the latest DI futures data from B3.
+
+    Returns:
+        pd.DataFrame: A Pandas pd.DataFrame containing the latest DI futures data.
+    """
+    raw_df = common.fetch_last_data(future_code="DI1")
+    return _process_last_di_data(raw_df)
+
+
+def fetch_past_di_data(
+    trade_date: pd.Timestamp, return_raw: bool = False
+) -> pd.DataFrame:
     """
     Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
     trade date. It's the primary external interface for accessing DI data.
 
     Args:
@@ -166,14 +217,14 @@
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
 
     Examples:
         >>> from pyield.futures import di
         >>> di.fetch_di(pd.Timestamp("2021-01-04"))
 
     Notes:
-        - BDaysToExpiration: number of business days to ExpirationDate.
+        - BDaysToExp: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common._fetch_raw_df(asset_code="DI1", trade_date=trade_date)
+    df_raw = common.fetch_past_data(asset_code="DI1", trade_date=trade_date)
     if return_raw:
         return df_raw
-    return _process_raw_df(df_raw, trade_date)
+    return _process_past_data(df_raw, trade_date)
```

### Comparing `pyield-0.7.2/pyield/futures/di_xml.py` & `pyield-0.7.3/pyield/futures/di_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 def _standardize_column_names(df: DataFrame) -> DataFrame:
     rename_dict = {
         "TradDt": "TradeDate",
         "TckrSymb": "Ticker",
         # "MktDataStrmId"
         # "IntlFinVol",
         "OpnIntrst": "OpenContracts",
-        "FinInstrmQty": "TradedQuantity",
+        "FinInstrmQty": "TradeVolume",
         "NtlFinVol": "FinancialVolume",
         "AdjstdQt": "SettlementPrice",
         "MinTradLmt": "MinTradeLimitRate",
         "MaxTradLmt": "MaxTradeLimitRate",
         # Must invert bid/ask for rates
         "BestAskPric": "BestBidRate",
         "BestBidPric": "BestAskRate",
@@ -229,21 +229,21 @@
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradDt"] = df["TradDt"].astype("datetime64[ns]")
 
     expiration = df["TckrSymb"].str[3:].apply(cm.get_expiration_date)
     df.insert(2, "ExpirationDate", expiration)
 
     business_days = bday.count_bdays(df["TradDt"], df["ExpirationDate"])
-    df.insert(3, "BDaysToExpiration", business_days)
+    df.insert(3, "BDaysToExp", business_days)
 
     # Convert to nullable integer, since other columns use this data type
-    df["BDaysToExpiration"] = df["BDaysToExpiration"].astype(pd.Int64Dtype())
+    df["BDaysToExp"] = df["BDaysToExp"].astype(pd.Int64Dtype())
 
     # Remove expired contracts
-    df.query("BDaysToExpiration > 0", inplace=True)
+    df.query("BDaysToExp > 0", inplace=True)
 
     return df.sort_values(by=["ExpirationDate"], ignore_index=True)
 
 
 def read_xml(trade_date: Timestamp, source_type: str, return_raw: bool) -> DataFrame:
     zip_file = _get_file_from_url(trade_date, source_type)
```

### Comparing `pyield-0.7.2/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.3/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.3/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/holidays/core.py` & `pyield-0.7.3/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/indicators.py` & `pyield-0.7.3/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/pyield/treasuries.py` & `pyield-0.7.3/pyield/treasuries.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     Returns:
         pd.DataFrame: A DataFrame containing the bond type, reference date, maturity
             date, and the calculated DI spread in basis points. The data is sorted by
             bond type and maturity date.
     """
     # Fetch DI rates and adjust the maturity date format for compatibility
-    df_di = ft.fetch_di(reference_date)[["ExpirationDate", "SettlementRate"]]
+    df_di = ft.fetch_past_di_data(reference_date)[["ExpirationDate", "SettlementRate"]]
 
     # Renaming the columns to match the ANBIMA structure
     df_di.rename(columns={"ExpirationDate": "MaturityDate"}, inplace=True)
 
     # Adjusting maturity date to match bond data format
     df_di["MaturityDate"] = df_di["MaturityDate"].dt.to_period("M").dt.to_timestamp()
```

### Comparing `pyield-0.7.2/pyield/utils.py` & `pyield-0.7.3/pyield/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from . import bday
 
 
 def _normalize_date(reference_date: str | pd.Timestamp | None = None) -> pd.Timestamp:
     """
     Normalizes the given date to ensure it is a past business day at midnight. If no
-    date is provided, it defaults to the previous business day.
+    date is provided, it defaults to the last business day.
 
     Args:
         reference_date (str | pd.Timestamp | None): The date to normalize. Can be a
         string, pandas Timestamp or None. If None, it defaults to the last business day.
 
     Returns:
         pd.Timestamp: A normalized pandas Timestamp representing a past business day at
@@ -34,17 +34,17 @@
     if isinstance(reference_date, str):
         # Convert string date to Timestamp and normalize to midnight
         normalized_date = pd.Timestamp(reference_date).normalize()
     elif isinstance(reference_date, pd.Timestamp):
         # Normalize Timestamp to midnight
         normalized_date = reference_date.normalize()
     elif reference_date is None:
-        # If no date is provided, use the previous business day
+        # If no date is provided, use the last available business day
         today = pd.Timestamp.today().normalize()
-        normalized_date = bday.offset_bdays(today, -1)
+        normalized_date = bday.offset_bdays(dates=today, offset=0, roll="backward")
     else:
         raise ValueError("Invalid date format.")
 
     # Validate that the date is not in the future
     if normalized_date > pd.Timestamp.today().normalize():
         raise ValueError("Reference date cannot be in the future.")
```

### Comparing `pyield-0.7.2/pyproject.toml` & `pyield-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas>=2.0.0",
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
 ]
 dynamic = []
-version = "0.7.2"
+version = "0.7.3"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.2/tests/test_bday.py` & `pyield-0.7.3/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.2/tests/test_futures.py` & `pyield-0.7.3/tests/test_futures.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,50 +33,48 @@
     result = ft.get_expiration_date(expiration_code)
     contract_expiration = pd.Timestamp("2023-01-02")
     assert result == contract_expiration
 
 
 def test_settlement_rate_with_old_holiday_list():
     settlement_rates = {
-        "N27": 0.09809,
-        "F33": 0.10368,
+        "DI1N27": 0.09809,
+        "DI1F33": 0.10368,
     }
 
     # 22-12-2023 is before the new holiday calendar
     test_date = pd.Timestamp("2023-12-22")
-    df = ft.fetch_di(trade_date=test_date)
-    expiration_codes = list(settlement_rates.keys())  # noqa: F841
-    result = df.query("ExpirationCode in @expiration_codes")["SettlementRate"].to_list()
+    df = ft.fetch_past_di_data(trade_date=test_date)
+    tickers = list(settlement_rates.keys())  # noqa: F841
+    result = df.query("TickerSymbol in @tickers")["SettlementRate"].to_list()
     assert result == list(settlement_rates.values())
 
 
 def test_settlement_rates_with_current_holiday_list():
     settlement_rates = {
-        "F24": 0.11644,
-        "J24": 0.11300,
-        "N24": 0.10786,
-        "V24": 0.10321,
-        "F25": 0.10031,
-        "J25": 0.09852,
-        "N25": 0.09715,
-        "V25": 0.09651,
-        "F26": 0.09583,
-        "N26": 0.09631,
-        "F27": 0.09683,
-        "N27": 0.09794,
-        "F29": 0.10042,
-        "F31": 0.10240,
-        "F33": 0.10331,
+        "DI1F24": 0.11644,
+        "DI1J24": 0.11300,
+        "DI1N24": 0.10786,
+        "DI1V24": 0.10321,
+        "DI1F25": 0.10031,
+        "DI1J25": 0.09852,
+        "DI1N25": 0.09715,
+        "DI1V25": 0.09651,
+        "DI1F26": 0.09583,
+        "DI1N26": 0.09631,
+        "DI1F27": 0.09683,
+        "DI1N27": 0.09794,
+        "DI1F29": 0.10042,
+        "DI1F31": 0.10240,
+        "DI1F33": 0.10331,
     }
     test_date = pd.Timestamp("2023-12-26")
-    df = ft.fetch_di(trade_date=test_date)
-    expiration_codes = list(settlement_rates.keys())  # noqa: F841
-    results = df.query("ExpirationCode in @expiration_codes")[
-        "SettlementRate"
-    ].to_list()
+    df = ft.fetch_past_di_data(trade_date=test_date)
+    tickers = list(settlement_rates.keys())  # noqa: F841
+    results = df.query("TickerSymbol in @tickers")["SettlementRate"].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
     non_business_day = pd.Timestamp("2023-12-24")
     with pytest.raises(ValueError):
-        ft.fetch_di(trade_date=non_business_day)
+        ft.fetch_past_di_data(trade_date=non_business_day)
```

### Comparing `pyield-0.7.2/PKG-INFO` & `pyield-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -97,22 +97,22 @@
 ```
 
 ### Futures Data
 ```python
 # Fetch a DataFrame with the DI Futures data from B3
 >>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 
-TradeDate  ExpirationCode ExpirationDate BDaysToExpiration ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
-2024-03-08 K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
-2024-03-08 M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
+TradeDate  TickerSymbol ExpirationDate BDaysToExp ... LastRate LastAskRate LastBidRate SettlementRate
+2024-03-08 DI1J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
+2024-03-08 DI1K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
+2024-03-08 DI1M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
 ...        ...            ...            ...               ... ...      ...         ...         ...
-2024-03-08 F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
+2024-03-08 DI1F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 DI1F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
+2024-03-08 DI1F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
```

