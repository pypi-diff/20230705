# Comparing `tmp/FundamentalAnalysis-0.2.9.tar.gz` & `tmp/fundamentalanalysis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FundamentalAnalysis-0.2.9.tar", last modified: Thu May 13 07:06:03 2021, max compression
+gzip compressed data, was "fundamentalanalysis-0.3.0.tar", last modified: Wed Jul  5 17:55:58 2023, max compression
```

## Comparing `FundamentalAnalysis-0.2.9.tar` & `fundamentalanalysis-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-05-13 07:06:03.437127 FundamentalAnalysis-0.2.9/
-drwxrwxrwx   0        0        0        0 2021-05-13 07:06:03.422029 FundamentalAnalysis-0.2.9/FundamentalAnalysis/
--rw-rw-rw-   0        0        0      666 2021-03-30 09:52:09.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis/__init__.py
--rw-rw-rw-   0        0        0     9978 2021-05-13 07:03:22.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis/details.py
--rw-rw-rw-   0        0        0     5596 2021-05-13 07:03:22.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis/financial_statements.py
--rw-rw-rw-   0        0        0     5442 2021-05-13 06:56:06.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis/ratios.py
--rw-rw-rw-   0        0        0     6585 2021-05-13 07:03:22.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis/stock_data.py
-drwxrwxrwx   0        0        0        0 2021-05-13 07:06:03.432288 FundamentalAnalysis-0.2.9/FundamentalAnalysis.egg-info/
--rw-rw-rw-   0        0        0     9995 2021-05-13 07:06:02.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2021-05-13 07:06:02.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-13 07:06:02.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2021-05-13 07:06:02.000000 FundamentalAnalysis-0.2.9/FundamentalAnalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9995 2021-05-13 07:06:03.436132 FundamentalAnalysis-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     8031 2021-05-13 07:03:22.000000 FundamentalAnalysis-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2021-05-13 07:06:03.438169 FundamentalAnalysis-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1043 2021-05-13 07:05:06.000000 FundamentalAnalysis-0.2.9/setup.py
+drwxr-xr-x   0 jeroenbouma   (501) staff       (20)        0 2023-07-05 17:55:58.620942 fundamentalanalysis-0.3.0/
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     1073 2022-05-09 06:00:26.000000 fundamentalanalysis-0.3.0/LICENSE
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     1158 2023-07-05 17:55:58.621016 fundamentalanalysis-0.3.0/PKG-INFO
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)      364 2023-07-05 17:54:04.000000 fundamentalanalysis-0.3.0/README.md
+drwxr-xr-x   0 jeroenbouma   (501) staff       (20)        0 2023-07-05 17:55:58.620197 fundamentalanalysis-0.3.0/fundamentalanalysis/
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     1034 2023-07-05 17:55:06.000000 fundamentalanalysis-0.3.0/fundamentalanalysis/__init__.py
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)    10914 2023-07-05 17:52:09.000000 fundamentalanalysis-0.3.0/fundamentalanalysis/details.py
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     5892 2023-07-05 17:52:09.000000 fundamentalanalysis-0.3.0/fundamentalanalysis/financial_statements.py
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     5592 2023-07-05 17:52:09.000000 fundamentalanalysis-0.3.0/fundamentalanalysis/ratios.py
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     6741 2023-07-05 17:52:09.000000 fundamentalanalysis-0.3.0/fundamentalanalysis/stock_data.py
+drwxr-xr-x   0 jeroenbouma   (501) staff       (20)        0 2023-07-05 17:55:58.620799 fundamentalanalysis-0.3.0/fundamentalanalysis.egg-info/
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     1158 2023-07-05 17:55:58.000000 fundamentalanalysis-0.3.0/fundamentalanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)      379 2023-07-05 17:55:58.000000 fundamentalanalysis-0.3.0/fundamentalanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)        1 2023-07-05 17:55:58.000000 fundamentalanalysis-0.3.0/fundamentalanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)       20 2023-07-05 17:55:58.000000 fundamentalanalysis-0.3.0/fundamentalanalysis.egg-info/top_level.txt
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)       38 2023-07-05 17:55:58.621269 fundamentalanalysis-0.3.0/setup.cfg
+-rw-r--r--   0 jeroenbouma   (501) staff       (20)     1019 2023-07-05 17:53:24.000000 fundamentalanalysis-0.3.0/setup.py
```

### Comparing `FundamentalAnalysis-0.2.9/FundamentalAnalysis/__init__.py` & `fundamentalanalysis-0.3.0/fundamentalanalysis/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,32 @@
-# Modules
-from .details import available_companies
-from .details import profile
-from .details import quote
-from .details import enterprise
-from .details import rating
-from .details import discounted_cash_flow
-from .details import earnings_calendar
-
-from .financial_statements import balance_sheet_statement
-from .financial_statements import income_statement
-from .financial_statements import cash_flow_statement
-
-from .ratios import key_metrics
-from .ratios import financial_ratios
-from .ratios import financial_statement_growth
-
-from .stock_data import stock_data
-from .stock_data import stock_data_detailed
-from .stock_data import stock_dividend
+# Modules
+from .details import available_companies
+from .details import profile
+from .details import quote
+from .details import enterprise
+from .details import rating
+from .details import discounted_cash_flow
+from .details import earnings_calendar
+
+from .financial_statements import balance_sheet_statement
+from .financial_statements import income_statement
+from .financial_statements import cash_flow_statement
+
+from .ratios import key_metrics
+from .ratios import financial_ratios
+from .ratios import financial_statement_growth
+
+from .stock_data import stock_data
+from .stock_data import stock_data_detailed
+from .stock_data import stock_dividend
+
+import ssl
+from warnings import warn
+
+ssl._create_default_https_context = ssl._create_unverified_context
+
+warn(
+    "\nThis package has been depreciated. Please use the new package: FinanceToolkit. This package can be installed with: pip install financetoolkit"
+    "\nFor more information, see: https://github.com/JerBouma/FinanceToolkit",
+    DeprecationWarning,
+    stacklevel=2,
+)
```

### Comparing `FundamentalAnalysis-0.2.9/FundamentalAnalysis/details.py` & `fundamentalanalysis-0.3.0/fundamentalanalysis/details.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,292 +1,345 @@
-from urllib.request import urlopen
-from urllib.error import HTTPError
-import json
-import pandas as pd
-
-
-def available_companies(api_key):
-    """
-    Description
-    ----
-    Gives all tickers, company names, current price and stock exchange that are available
-    for retrieval for financial statements, ratios and extended stock data. General stock
-    data can be retrieved for any company or financial instrument.
-
-    Input
-    ----
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-
-    Output
-    ----
-    data (dataframe)
-        Data with the ticker as the index and the company name, price and
-        stock exchange in the columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/stock/list?apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    df = pd.DataFrame(data)
-    df.loc[df["name"].isna(), "name"] = df["symbol"]
-    df = df.set_index("symbol")
-
-    return df
-
-
-def profile(ticker, api_key):
-    """
-    Description
-    ----
-    Gives information about the profile of a company which includes
-    i.a. beta, company description, industry and sector.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "AAPL")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/profile/{ticker}?apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    data_formatted = pd.DataFrame(data).T
-
-    return data_formatted
-
-
-def quote(ticker, api_key):
-    """
-    Description
-    ----
-    Gives information about the quote of a company which includes i.a.
-    high/low close prices, price-to-earning ratio and shares outstanding.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "AMD")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/quote/{ticker}?apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    data_formatted = pd.DataFrame(data).T
-
-    return data_formatted
-
-
-def enterprise(ticker, api_key, period="annual"):
-    """
-    Description
-    ----
-    Gives information about the enterprise value of a company which includes
-    i.a. market capitalisation, Cash & Cash Equivalents, total debt and enterprise value.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "TSLA")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    period (string)
-        Data period, this can be "annual" or "quarter".
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/enterprise-values/{ticker}"
-                           f"?period={period}&apikey={api_key}")
-        data = response.read().decode("utf-8")
-        data_json = json.loads(data)
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data_json:
-        raise ValueError(data_json['Error Message'])
-
-    data_formatted = {}
-    for data in data_json:
-        if period == "quarter":
-            date = data['date'][:7]
-        else:
-            date = data['date'][:4]
-        del data['date']
-        data_formatted[date] = data
-
-    return pd.DataFrame(data_formatted)
-
-
-def rating(ticker, api_key):
-    """
-     Description
-     ----
-     Gives information about the rating of a company which includes i.a. the company
-     rating and recommendation as well as ratings based on a variety of ratios.
-
-     Input
-     ----
-     ticker (string)
-        The company ticker (for example: "MSFT")
-     api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-
-     Output
-     ----
-     data (dataframe)
-        Data with variables in rows and the period in columns..
-     """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/historical-rating/{ticker}?apikey={api_key}")
-        data = response.read().decode("utf-8")
-        data_json = json.loads(data)
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data_json:
-        raise ValueError(data_json['Error Message'])
-
-    for value in data_json:
-        del value['symbol']
-
-    data_formatted = pd.DataFrame(data_json).set_index('date')
-
-    return data_formatted
-
-
-def discounted_cash_flow(ticker, api_key, period="annual"):
-    """
-    Description
-    ----
-    Gives information about the discounted cash flow (DCF) of a company which includes
-    i.a. the (current) stock price and DCF and over time.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "UBER")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    period (string)
-        Data period, this can be "annual" or "quarter".
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/discounted-cash-flow/{ticker}"
-                           f"?period={period}&apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    data_json_current = data[0]
-
-    try:
-        del data_json_current['symbol']
-        data_json_current['DCF'] = data_json_current.pop('dcf')
-    except KeyError:
-        pass
-
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/historical-discounted-cash-flow/{ticker}"
-                           f"?period={period}&apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    data_json = data[0]['historicalDCF']
-
-    data_formatted = {}
-
-    if period == "quarter":
-        current_year = data_json_current['date'][:7]
-    else:
-        current_year = data_json_current['date'][:4]
-    data_formatted[current_year] = data_json_current
-
-    for data in data_json:
-        if period == "quarter":
-            date = data['date'][:7]
-        else:
-            date = data['date'][:4]
-        data_formatted[date] = data
-
-    return pd.DataFrame(data_formatted)
-
-
-def earnings_calendar(api_key):
-    """
-    Description
-    ----
-    Gives information about the earnings date over the upcoming months including
-    the expected PE.
-
-    Input
-    ----
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/earning_calendar/?apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    return pd.DataFrame(data).set_index("date")
+from urllib.request import urlopen
+from urllib.error import HTTPError
+import json
+import pandas as pd
+
+
+def available_companies(api_key):
+    """
+    Description
+    ----
+    Gives all tickers, company names, current price and stock exchange that are available
+    for retrieval for financial statements, ratios and extended stock data. General stock
+    data can be retrieved for any company or financial instrument.
+
+    Input
+    ----
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+
+    Output
+    ----
+    data (dataframe)
+        Data with the ticker as the index and the company name, price and
+        stock exchange in the columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/stock/list?apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    df = pd.DataFrame(data)
+    df.loc[df["name"].isna(), "name"] = df["symbol"]
+    df = df.set_index("symbol")
+
+    return df
+
+
+def profile(ticker, api_key):
+    """
+    Description
+    ----
+    Gives information about the profile of a company which includes
+    i.a. beta, company description, industry and sector.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "AAPL")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/profile/{ticker}?apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    data_formatted = pd.DataFrame(data).T
+
+    return data_formatted
+
+
+def quote(ticker, api_key):
+    """
+    Description
+    ----
+    Gives information about the quote of a company which includes i.a.
+    high/low close prices, price-to-earning ratio and shares outstanding.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "AMD")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/quote/{ticker}?apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    data_formatted = pd.DataFrame(data).T
+
+    return data_formatted
+
+
+def enterprise(ticker, api_key, period="annual", limit=0):
+    """
+    Description
+    ----
+    Gives information about the enterprise value of a company which includes
+    i.a. market capitalisation, Cash & Cash Equivalents, total debt and enterprise value.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "TSLA")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    period (string)
+        Data period, this can be "annual" or "quarter".
+    limit (integer)
+        The limit for the years of data
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/enterprise-values/{ticker}"
+            f"?period={period}&limit={limit}&apikey={api_key}"
+        )
+        data = response.read().decode("utf-8")
+        data_json = json.loads(data)
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data_json:
+        raise ValueError(data_json["Error Message"])
+
+    data_formatted = {}
+    for data in data_json:
+        if period == "quarter":
+            date = data["date"][:7]
+        else:
+            date = data["date"][:4]
+        del data["date"]
+        data_formatted[date] = data
+
+    return pd.DataFrame(data_formatted)
+
+
+def rating(ticker, api_key):
+    """
+    Description
+    ----
+    Gives information about the rating of a company which includes i.a. the company
+    rating and recommendation as well as ratings based on a variety of ratios.
+
+    Input
+    ----
+    ticker (string)
+       The company ticker (for example: "MSFT")
+    api_key (string)
+       The API Key obtained from https://financialmodelingprep.com/developer/docs/
+
+    Output
+    ----
+    data (dataframe)
+       Data with variables in rows and the period in columns..
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/historical-rating/{ticker}?apikey={api_key}"
+        )
+        data = response.read().decode("utf-8")
+        data_json = json.loads(data)
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data_json:
+        raise ValueError(data_json["Error Message"])
+
+    for value in data_json:
+        del value["symbol"]
+
+    data_formatted = pd.DataFrame(data_json).set_index("date")
+
+    return data_formatted
+
+
+def discounted_cash_flow(ticker, api_key, period="annual", limit=0):
+    """
+    Description
+    ----
+    Gives information about the discounted cash flow (DCF) of a company which includes
+    i.a. the (current) stock price and DCF and over time.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "UBER")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    period (string)
+        Data period, this can be "annual" or "quarter".
+    limit (integer)
+        The limit for the years of data
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/discounted-cash-flow/{ticker}"
+            f"?period={period}&limit={limit}&apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    data_json_current = data[0]
+
+    try:
+        del data_json_current["symbol"]
+        data_json_current["DCF"] = data_json_current.pop("dcf")
+    except KeyError:
+        pass
+
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/"
+            f"historical-discounted-cash-flow/{ticker}?period={period}&apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+        data_json = data[0]["historicalDCF"]
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+    except KeyError:
+        try:
+            response = urlopen(
+                f"https://financialmodelingprep.com/api/v3/"
+                f"historical-discounted-cash-flow-statement/{ticker}?period={period}&apikey={api_key}"
+            )
+            data = json.loads(response.read().decode("utf-8"))
+            data_json = data[0]
+        except HTTPError:
+            raise ValueError(
+                "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+                "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+            )
+        except IndexError:
+            raise ValueError(
+                f"No information available for the ticker {ticker}. Please check if this ticker is actually a stock "
+                f"with the available_companies function."
+            )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    data_formatted = {}
+
+    if period == "quarter":
+        current_year = data_json_current["date"][:7]
+    else:
+        current_year = data_json_current["date"][:4]
+    data_formatted[current_year] = data_json_current
+
+    for data in data_json:
+        if period == "quarter":
+            date = data["date"][:7]
+        else:
+            date = data["date"][:4]
+        data_formatted[date] = data
+
+    return pd.DataFrame(data_formatted)
+
+
+def earnings_calendar(api_key):
+    """
+    Description
+    ----
+    Gives information about the earnings date over the upcoming months including
+    the expected PE.
+
+    Input
+    ----
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/earning_calendar/?apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    return pd.DataFrame(data).set_index("date")
```

### Comparing `FundamentalAnalysis-0.2.9/FundamentalAnalysis/ratios.py` & `fundamentalanalysis-0.3.0/fundamentalanalysis/ratios.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,177 @@
-from urllib.request import urlopen
-from urllib.error import HTTPError
-import json
-import pandas as pd
-
-
-def key_metrics(ticker, api_key, period="annual", TTM=False):
-    """
-    Description
-    ----
-    Gives information about key metrics of a company overtime which includes
-    i.a. PE ratio, Debt to Equity, Dividend Yield and Average Inventory.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "NFLX")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    period (string)
-        Data period, this can be "annual" or "quarter".
-    TTM (boolean)
-        Obtain the trailing twelve months (TTM) key metrics.
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    if TTM:
-        URL = f"https://financialmodelingprep.com/api/v3/key-metrics-ttm/{ticker}?apikey={api_key}"
-    else:
-        URL = f"https://financialmodelingprep.com/api/v3/key-metrics/{ticker}?period={period}&apikey={api_key}"
-
-    try:
-        response = urlopen(URL)
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    if TTM:
-        data_formatted = pd.Series(data[0])
-    else:
-        data_formatted = {}
-        for value in data:
-            if period == "quarter":
-                date = value['date'][:7]
-            else:
-                date = value['date'][:4]
-            del value['date']
-            del value['symbol']
-
-            data_formatted[date] = value
-        data_formatted = pd.DataFrame(data_formatted)
-
-    return data_formatted
-
-def financial_ratios(ticker, api_key, period="annual", TTM=False):
-    """
-    Description
-    ----
-    Gives information about the financial ratios of a company overtime
-    which includes i.a. investment, liquidity, profitability and debt ratios.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "LYFT")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    period (string)
-        Data period, this can be "annual" or "quarter".
-    TTM (boolean)
-        Obtain the trailing twelve months (TTM) ratios.
-
-    Output
-    ----
-    data (dataframe or series)
-        Data with variables in rows and the period in columns.
-    """
-    if TTM:
-        URL = f"https://financialmodelingprep.com/api/v3/ratios-ttm/{ticker}?apikey={api_key}"
-    else:
-        URL = f"https://financialmodelingprep.com/api/v3/ratios/{ticker}?period={period}&apikey={api_key}"
-
-    try:
-        response = urlopen(URL)
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    if TTM:
-        data_formatted = pd.Series(data[0])
-    else:
-        data_formatted = {}
-        for value in data:
-            if period == "quarter":
-                date = value['date'][:7]
-            else:
-                date = value['date'][:4]
-            del value['date']
-            del value['symbol']
-
-            data_formatted[date] = value
-        data_formatted = pd.DataFrame(data_formatted)
-
-    return data_formatted
-
-
-def financial_statement_growth(ticker, api_key, period="annual"):
-    """
-    Description
-    ----
-    Gives information about the financial statement growth of a company overtime
-    which includes i.a. EBIT growth (%) and shareholder equity growth (% per 3, 5
-    and 10 years)
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "WMT")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    period (string)
-        Data period, this can be "annual" or "quarter".
-
-    Output
-    ----
-    data (dataframe)
-        Data with variables in rows and the period in columns.
-    """
-    try:
-        response = urlopen(f"https://financialmodelingprep.com/api/v3/financial-growth/{ticker}"
-                           f"?period={period}&apikey={api_key}")
-        data = json.loads(response.read().decode("utf-8"))
-    except HTTPError:
-        raise ValueError("This endpoint is only for premium members. Please visit the subscription page to upgrade the "
-                         "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing")
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    data_formatted = {}
-    for value in data:
-        if period == "quarter":
-            date = value['date'][:7]
-        else:
-            date = value['date'][:4]
-        del value['date']
-        del value['symbol']
-
-        data_formatted[date] = value
-
-    return pd.DataFrame(data_formatted)
+from urllib.request import urlopen
+from urllib.error import HTTPError
+import json
+import pandas as pd
+
+
+def key_metrics(ticker, api_key, period="annual", TTM=False, limit=0):
+    """
+    Description
+    ----
+    Gives information about key metrics of a company overtime which includes
+    i.a. PE ratio, Debt to Equity, Dividend Yield and Average Inventory.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "NFLX")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    period (string)
+        Data period, this can be "annual" or "quarter".
+    TTM (boolean)
+        Obtain the trailing twelve months (TTM) key metrics.
+    limit (integer)
+        The limit for the years of data
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    if TTM:
+        URL = f"https://financialmodelingprep.com/api/v3/key-metrics-ttm/{ticker}?limit={limit}&apikey={api_key}"
+    else:
+        URL = f"https://financialmodelingprep.com/api/v3/key-metrics/{ticker}?period={period}&limit={limit}&apikey={api_key}"
+
+    try:
+        response = urlopen(URL)
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    if TTM:
+        data_formatted = pd.Series(data[0])
+    else:
+        data_formatted = {}
+        for value in data:
+            if period == "quarter":
+                date = value["date"][:7]
+            else:
+                date = value["date"][:4]
+            del value["date"]
+            del value["symbol"]
+
+            data_formatted[date] = value
+        data_formatted = pd.DataFrame(data_formatted)
+
+    return data_formatted
+
+
+def financial_ratios(ticker, api_key, period="annual", TTM=False, limit=0):
+    """
+    Description
+    ----
+    Gives information about the financial ratios of a company overtime
+    which includes i.a. investment, liquidity, profitability and debt ratios.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "LYFT")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    period (string)
+        Data period, this can be "annual" or "quarter".
+    TTM (boolean)
+        Obtain the trailing twelve months (TTM) ratios.
+    limit (integer)
+        The limit for the years of data
+
+    Output
+    ----
+    data (dataframe or series)
+        Data with variables in rows and the period in columns.
+    """
+    if TTM:
+        URL = f"https://financialmodelingprep.com/api/v3/ratios-ttm/{ticker}?limit={limit}&apikey={api_key}"
+    else:
+        URL = f"https://financialmodelingprep.com/api/v3/ratios/{ticker}?period={period}&limit={limit}&apikey={api_key}"
+
+    try:
+        response = urlopen(URL)
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    if TTM:
+        data_formatted = pd.Series(data[0])
+    else:
+        data_formatted = {}
+        for value in data:
+            if period == "quarter":
+                date = value["date"][:7]
+            else:
+                date = value["date"][:4]
+            del value["date"]
+            del value["symbol"]
+
+            data_formatted[date] = value
+        data_formatted = pd.DataFrame(data_formatted)
+
+    return data_formatted
+
+
+def financial_statement_growth(ticker, api_key, period="annual", limit=0):
+    """
+    Description
+    ----
+    Gives information about the financial statement growth of a company overtime
+    which includes i.a. EBIT growth (%) and shareholder equity growth (% per 3, 5
+    and 10 years)
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "WMT")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    period (string)
+        Data period, this can be "annual" or "quarter".
+    limit (integer)
+        The limit for the years of data
+
+    Output
+    ----
+    data (dataframe)
+        Data with variables in rows and the period in columns.
+    """
+    try:
+        response = urlopen(
+            f"https://financialmodelingprep.com/api/v3/financial-growth/{ticker}"
+            f"?period={period}&limit={limit}&apikey={api_key}"
+        )
+        data = json.loads(response.read().decode("utf-8"))
+    except HTTPError:
+        raise ValueError(
+            "This endpoint is only for premium members. Please visit the subscription page to upgrade the "
+            "plan (Starter or higher) at https://financialmodelingprep.com/developer/docs/pricing"
+        )
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    data_formatted = {}
+    for value in data:
+        if period == "quarter":
+            date = value["date"][:7]
+        else:
+            date = value["date"][:4]
+        del value["date"]
+        del value["symbol"]
+
+        data_formatted[date] = value
+
+    return pd.DataFrame(data_formatted)
```

### Comparing `FundamentalAnalysis-0.2.9/FundamentalAnalysis/stock_data.py` & `fundamentalanalysis-0.3.0/fundamentalanalysis/stock_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,200 @@
-import pandas as pd
-from datetime import datetime
-import requests
-from urllib.request import urlopen
-import json
-
-
-def stock_data(ticker, period="max", interval="1d", start=None, end=None):
-    """
-    Description
-    ----
-    Gives information about the profile of a company which includes
-    i.a. beta, company description, industry and sector.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "URTH")
-    period (string)
-        The range of the data (default = "max"), this can hold the following
-        periods: "1d","5d","1mo","3mo","6mo","1y","2y","5y","10y","ytd","max"
-    interval (string)
-        The frequency of the data (default = "1d"), this can hold the
-        following intervals: "1m", "2m", "5m", "15m","30m","60m",
-        "90m", "1h", "1d", "5d", "1wk", "1mo", "3mo".
-        Note that an interval less than 1h can only hold a period 1mo or less."
-    start (string)
-        The start date in the format %Y-%m-%d. Choose either start/end
-        or period.
-    end (string)
-        The end date in the format %Y-%m-%d. Choose either start/end
-        or period.
-
-    Output
-    ----
-    data (dataframe)
-        Data with dates in rows and the quotes in columns.
-    """
-    parameters = {"interval": interval}
-
-    if start is None or end is None:
-        parameters['range'] = period
-    else:
-        start_timestamp = int(datetime.strptime(start, '%Y-%m-%d').timestamp())
-        end_timestamp = int(datetime.strptime(end, '%Y-%m-%d').timestamp())
-        parameters["period1"] = start_timestamp
-        parameters["period2"] = end_timestamp
-
-    url = f"https://query1.finance.yahoo.com/v8/finance/chart/{ticker}"
-
-    try:
-        data = requests.get(url=url, params=parameters)
-        data_json = data.json()['chart']['result'][0]
-    except TypeError:
-        raise TypeError("No data available. Please check if you have a valid period and/or interval. \n"
-                        "Note that an interval less than 1h can only hold a period of 1mo or less.")
-
-    timestamp = data_json['timestamp']
-    dates = []
-    for ts in timestamp:
-        if interval in ['1m', '2m', '5m', '15m',
-                        '30m', '60m', '90m', '1h']:
-            dates.append(datetime.fromtimestamp(int(ts)))
-        else:
-            dates.append(datetime.fromtimestamp(int(ts)).date())
-
-    indicators = data_json['indicators']['quote'][0]
-    try:
-        indicators.update(data_json['indicators']['adjclose'][0])
-    except Exception as e:
-        print("Data for " + str(e) + " could not be included.")
-
-    return pd.DataFrame(indicators, index=dates)
-
-
-def stock_data_detailed(ticker, api_key, begin="1792-05-17", end=None):
-    """
-    Description
-    ----
-    Gives complete information about the company's stock which includes open, high,
-    low, close, adjusted close, volume, unadjusted volume, change, change percent,
-    volume weighted average price, label and change over time.
-
-    This function only allows company tickers and is limited to the companies found
-    by calling available_companies() from the details module.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "FIZZ")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    begin (string)
-        Begin date in the format %Y-%m-%d.
-        Default is the beginning of the Stock Market: 1792-05-17.
-    end (string)
-        End date in the format %Y-%m-%d.
-        Default is the current date.
-
-    Output
-    ----
-    data (dataframe)
-        Data with the date in the rows and the variables in the columns.
-    """
-    response = urlopen(f"https://financialmodelingprep.com/api/v3/historical-price-full/{ticker}"
-                       f"?from={str(begin)}&to={str(end)}&apikey={api_key}")
-    data = json.loads(response.read().decode("utf-8"))
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    try:
-        data_json = data['historical']
-    except KeyError:
-        raise ValueError("No data available. Please note this function only takes a specific selection of companies. \n"
-                         "See: FundamentalAnalysis.available_companies()")
-
-    data_formatted = {}
-    for value in data_json:
-        date = value['date']
-        del value['date']
-        data_formatted[date] = value
-    data_formatted = pd.DataFrame(data_formatted).T
-
-    return data_formatted
-
-
-def stock_dividend(ticker, api_key, begin="1792-05-17", end=None):
-    """
-    Description
-    ----
-    Gives complete information about the company's dividend which includes adjusted dividend, dividend,
-    record date, payment date and declaration date over time.
-
-    This function only allows company tickers and is limited to the companies found
-    by calling available_companies() from the details module.
-
-    Input
-    ----
-    ticker (string)
-        The company ticker (for example: "TSLA")
-    api_key (string)
-        The API Key obtained from https://financialmodelingprep.com/developer/docs/
-    begin (string)
-        Begin date in the format %Y-%m-%d.
-        Default is the beginning of the Stock Market: 1792-05-17.
-    end (string)
-        End date in the format %Y-%m-%d.
-        Default is the current date.
-
-    Output
-    ----
-    data (dataframe)
-        Data with the date in the rows and the variables in the columns.
-    """
-    if end is None:
-        end = pd.Timestamp.today().strftime('%Y-%m-%d')
-
-    response = urlopen(f"https://financialmodelingprep.com/api/v3/historical-price-full/stock_dividend/{ticker}"
-                       f"?apikey={api_key}")
-
-    data = json.loads(response.read().decode("utf-8"))
-
-    if 'Error Message' in data:
-        raise ValueError(data['Error Message'])
-
-    try:
-        data_json = data['historical']
-    except KeyError:
-        raise ValueError("No data available. Please note this function only takes a specific selection of companies. \n"
-                         "See: FundamentalAnalysis.available_companies()")
-
-    data_formatted = {}
-    for value in data_json:
-        date = value['date']
-        del value['date']
-        data_formatted[date] = value
-    data_formatted = pd.DataFrame(data_formatted).T
-
-    begin_bool = data_formatted.index > begin
-    end_bool = data_formatted.index < end
-    data_formatted = data_formatted[begin_bool & end_bool]
-
-    return data_formatted
+import pandas as pd
+from datetime import datetime
+import requests
+from urllib.request import urlopen
+import json
+
+
+def stock_data(ticker, period="max", interval="1d", start=None, end=None):
+    """
+    Description
+    ----
+    Gives information about the profile of a company which includes
+    i.a. beta, company description, industry and sector.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "URTH")
+    period (string)
+        The range of the data (default = "max"), this can hold the following
+        periods: "1d","5d","1mo","3mo","6mo","1y","2y","5y","10y","ytd","max"
+    interval (string)
+        The frequency of the data (default = "1d"), this can hold the
+        following intervals: "1m", "2m", "5m", "15m","30m","60m",
+        "90m", "1h", "1d", "5d", "1wk", "1mo", "3mo".
+        Note that an interval less than 1h can only hold a period 1mo or less."
+    start (string)
+        The start date in the format %Y-%m-%d. Choose either start/end
+        or period.
+    end (string)
+        The end date in the format %Y-%m-%d. Choose either start/end
+        or period.
+
+    Output
+    ----
+    data (dataframe)
+        Data with dates in rows and the quotes in columns.
+    """
+    parameters = {"interval": interval}
+
+    if start is None or end is None:
+        parameters["range"] = period
+    else:
+        start_timestamp = int(datetime.strptime(start, "%Y-%m-%d").timestamp())
+        end_timestamp = int(datetime.strptime(end, "%Y-%m-%d").timestamp())
+        parameters["period1"] = start_timestamp
+        parameters["period2"] = end_timestamp
+
+    url = f"https://query1.finance.yahoo.com/v8/finance/chart/{ticker}"
+
+    try:
+        header = {
+            "Connection": "keep-alive",
+            "Expires": "-1",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) \
+                                     AppleWebKit/537.36 (KHTML, like Gecko) Chrome/54.0.2840.99 Safari/537.36",
+        }
+        data = requests.get(url=url, params=parameters, headers=header)
+        data_json = data.json()["chart"]["result"][0]
+    except TypeError:
+        raise TypeError(
+            "No data available. Please check if you have a valid period and/or interval. \n"
+            "Note that an interval less than 1h can only hold a period of 1mo or less."
+        )
+
+    timestamp = data_json["timestamp"]
+    dates = []
+    for ts in timestamp:
+        if interval in ["1m", "2m", "5m", "15m", "30m", "60m", "90m", "1h"]:
+            dates.append(datetime.fromtimestamp(int(ts)))
+        else:
+            dates.append(datetime.fromtimestamp(int(ts)).date())
+
+    indicators = data_json["indicators"]["quote"][0]
+    try:
+        indicators.update(data_json["indicators"]["adjclose"][0])
+    except Exception as e:
+        print("Data for " + str(e) + " could not be included.")
+
+    return pd.DataFrame(indicators, index=dates)
+
+
+def stock_data_detailed(ticker, api_key, begin="1792-05-17", end=None):
+    """
+    Description
+    ----
+    Gives complete information about the company's stock which includes open, high,
+    low, close, adjusted close, volume, unadjusted volume, change, change percent,
+    volume weighted average price, label and change over time.
+
+    This function only allows company tickers and is limited to the companies found
+    by calling available_companies() from the details module.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "FIZZ")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    begin (string)
+        Begin date in the format %Y-%m-%d.
+        Default is the beginning of the Stock Market: 1792-05-17.
+    end (string)
+        End date in the format %Y-%m-%d.
+        Default is the current date.
+
+    Output
+    ----
+    data (dataframe)
+        Data with the date in the rows and the variables in the columns.
+    """
+    response = urlopen(
+        f"https://financialmodelingprep.com/api/v3/historical-price-full/{ticker}"
+        f"?from={str(begin)}&to={str(end)}&apikey={api_key}"
+    )
+    data = json.loads(response.read().decode("utf-8"))
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    try:
+        data_json = data["historical"]
+    except KeyError:
+        raise ValueError(
+            "No data available. Please note this function only takes a specific selection of companies. \n"
+            "See: fundamentalanalysis.available_companies()"
+        )
+
+    data_formatted = {}
+    for value in data_json:
+        date = value["date"]
+        del value["date"]
+        data_formatted[date] = value
+    data_formatted = pd.DataFrame(data_formatted).T
+
+    return data_formatted
+
+
+def stock_dividend(ticker, api_key, begin="1792-05-17", end=None):
+    """
+    Description
+    ----
+    Gives complete information about the company's dividend which includes adjusted dividend, dividend,
+    record date, payment date and declaration date over time.
+
+    This function only allows company tickers and is limited to the companies found
+    by calling available_companies() from the details module.
+
+    Input
+    ----
+    ticker (string)
+        The company ticker (for example: "TSLA")
+    api_key (string)
+        The API Key obtained from https://financialmodelingprep.com/developer/docs/
+    begin (string)
+        Begin date in the format %Y-%m-%d.
+        Default is the beginning of the Stock Market: 1792-05-17.
+    end (string)
+        End date in the format %Y-%m-%d.
+        Default is the current date.
+
+    Output
+    ----
+    data (dataframe)
+        Data with the date in the rows and the variables in the columns.
+    """
+    if end is None:
+        end = pd.Timestamp.today().strftime("%Y-%m-%d")
+
+    response = urlopen(
+        f"https://financialmodelingprep.com/api/v3/historical-price-full/stock_dividend/{ticker}"
+        f"?apikey={api_key}"
+    )
+
+    data = json.loads(response.read().decode("utf-8"))
+
+    if "Error Message" in data:
+        raise ValueError(data["Error Message"])
+
+    try:
+        data_json = data["historical"]
+    except KeyError:
+        raise ValueError(
+            "No data available. Please note this function only takes a specific selection of companies. \n"
+            "See: fundamentalanalysis.available_companies()"
+        )
+
+    data_formatted = {}
+    for value in data_json:
+        date = value["date"]
+        del value["date"]
+        data_formatted[date] = value
+    data_formatted = pd.DataFrame(data_formatted).T
+
+    begin_bool = data_formatted.index > begin
+    end_bool = data_formatted.index < end
+    data_formatted = data_formatted[begin_bool & end_bool]
+
+    return data_formatted
```

### Comparing `FundamentalAnalysis-0.2.9/setup.py` & `fundamentalanalysis-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="FundamentalAnalysis",
-    packages=["FundamentalAnalysis"],
-    version="0.2.9",
-    license="MIT",
-    description="Fully-fledged Fundamental Analysis package capable of collecting 20 years of Company Profiles,\
-    Financial Statements, Ratios and Stock Data of 20.000+ companies.",
-    author="JerBouma",
-    author_email="jer.bouma@gmail.com",
-    url="https://github.com/JerBouma/FundamentalAnalysis",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    keywords=["fundamental", "analysis", "finance"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Financial and Insurance Industry",
-        "Topic :: Office/Business :: Financial :: Investment",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3"
-    ],
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="fundamentalanalysis",
+    packages=["fundamentalanalysis"],
+    version="0.3.0",
+    license="MIT",
+    description="Fully-fledged Fundamental Analysis package capable of collecting 20 years of Company Profiles,\
+    Financial Statements, Ratios and Stock Data of 20.000+ companies.",
+    author="JerBouma",
+    author_email="jer.bouma@gmail.com",
+    url="https://github.com/JerBouma/FundamentalAnalysis",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    keywords=["fundamental", "analysis", "finance"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Financial and Insurance Industry",
+        "Topic :: Office/Business :: Financial :: Investment",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+    ],
+)
```

