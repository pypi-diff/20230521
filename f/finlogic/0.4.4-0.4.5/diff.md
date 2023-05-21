# Comparing `tmp/finlogic-0.4.4.tar.gz` & `tmp/finlogic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.4.tar", last modified: Wed May 17 10:53:06 2023, max compression
+gzip compressed data, was "finlogic-0.4.5.tar", last modified: Sun May 21 14:28:01 2023, max compression
```

## Comparing `finlogic-0.4.4.tar` & `finlogic-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.4/LICENSE
--rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.4/README.md
--rw-r--r--   0        0        0      423 2023-05-17 10:51:22.833432 finlogic-0.4.4/finlogic/__init__.py
--rw-r--r--   0        0        0    23507 2023-05-17 10:44:23.276617 finlogic-0.4.4/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.4/finlogic/config.py
--rw-r--r--   0        0        0     9775 2023-05-17 10:25:31.301270 finlogic-0.4.4/finlogic/cvm.py
--rw-r--r--   0        0        0     4460 2023-05-17 10:44:29.881677 finlogic-0.4.4/finlogic/database.py
--rw-r--r--   0        0        0     3156 2023-05-17 03:27:27.153327 finlogic-0.4.4/finlogic/fduckdb.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.4/finlogic/fprint.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.4/finlogic/language.py
--rw-r--r--   0        0        0     1005 2023-05-17 10:53:06.688384 finlogic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     3314 2023-05-12 00:21:10.028393 finlogic-0.4.4/tests/test_company.py
--rw-r--r--   0        0        0      900 2023-05-17 10:44:08.373481 finlogic-0.4.4/tests/test_database.py
--rw-r--r--   0        0        0    11655 1970-01-01 00:00:00.000000 finlogic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.5/LICENSE
+-rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.5/README.md
+-rw-r--r--   0        0        0      423 2023-05-19 08:15:00.845332 finlogic-0.4.5/finlogic/__init__.py
+-rw-r--r--   0        0        0    24331 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.5/finlogic/config.py
+-rw-r--r--   0        0        0    10641 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/cvm.py
+-rw-r--r--   0        0        0     4460 2023-05-17 10:44:29.881677 finlogic-0.4.5/finlogic/database.py
+-rw-r--r--   0        0        0     3140 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/fduckdb.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.5/finlogic/fprint.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.5/finlogic/language.py
+-rw-r--r--   0        0        0     1014 2023-05-21 14:28:01.503322 finlogic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.5/tests/test_company.py
+-rw-r--r--   0        0        0      900 2023-05-21 14:25:13.096740 finlogic-0.4.5/tests/test_database.py
+-rw-r--r--   0        0        0    11687 1970-01-01 00:00:00.000000 finlogic-0.4.5/PKG-INFO
```

### Comparing `finlogic-0.4.4/LICENSE` & `finlogic-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.4/README.md` & `finlogic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.4/finlogic/company.py` & `finlogic-0.4.5/finlogic/company.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,45 +26,58 @@
 from .fprint import print_dict
 from .fduckdb import execute
 
 
 class Company:
     """A class to represent a company financial data.
 
-    This class provides methods to create financial reports and to calculate
-    financial indicators based on a company's accounting data. The class also
-    has an AI generated dictionary to translate from Portuguese to English.
-
-    Methods:
-        report: Creates a financial report for the company.
-        custom_report: Creates a custom financial report for the company.
-        indicators: Calculates the financial indicators of the company.
+     This class provides methods to create financial reports and to calculate
+     financial indicators based on a company's accounting data. The class also
+     has an AI generated dictionary to translate from Portuguese to English.
+
+    Attributes:
+         identifier: A unique identifier for the company. Both CVM ID (int) and
+            Fiscal ID (str) can be used.
+         acc_method: The accounting methods can be either 'con' for consolidated or
+            'sep' for separate. Defaults to 'con' (str).
+         acc_unit: The accounting unit for the financial statements where "t"
+            represents thousands, "m" represents millions and "b" represents
+            billions (int, float or str). Defaults to 1.
+         tax_rate: The tax rate for the company. Defaults to 0.34, which is
+            the standard corporate tax rate in Brazil (float).
+         language: The language for the financial reports. Options are "english"
+            or "portuguese". Defaults to "english" (str).
+
+     Methods:
+         report: Creates a financial report for the company.
+         custom_report: Creates a custom financial report for the company.
+         indicators: Calculates the financial indicators of the company.
 
-    Raises:
-        ValueError: If the input arguments are invalid.
+     Raises:
+         ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
-        acc_method: Literal["consolidated", "separate"] = "consolidated",
-        acc_unit: int | float | str = 1,
+        acc_method: Literal["con", "sep"] = "con",
+        acc_unit: int | float | Literal["t", "m", "b"] = 1,
         tax_rate: float = 0.34,
-        language: str = "english",
+        language: Literal["english", "portuguese"] = "english",
     ):
         """Initializes a new instance of the Company class."""
         self._initialized = False
         self.identifier = identifier
         self.acc_method = acc_method
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
         self._initialized = True
         # Only set company dataframe after identifier, acc_method and acc_unit are set
-        self._set_dfc()
+        self._set_df()
 
     @property
     def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
         identifier. The identifier can be either the CVM ID or the Fiscal ID
@@ -100,87 +113,89 @@
             self.tax_id = df.loc[0, "tax_id"]
             self.name_id = df.loc[0, "name_id"]
             self._identifier = identifier
         else:
             raise KeyError(f"Company 'identifier' {identifier} not found.")
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_dfc()
+            self._set_df()
 
     @property
-    def acc_method(self) -> Literal["consolidated", "separate"]:
+    def acc_method(self) -> Literal["con", "sep"]:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
-        The "acc_method" must be "consolidated" or "separate". Consolidated
-        accounting combines the financial statements of a parent company and its
-        subsidiaries, while separate accounting keeps them separate. Defaults to
-        'consolidated'.
+        The "acc_method" must be "con" for consolidated or "sep" for separate.
+        Consolidated accounting combines the financial statements of a parent
+        company and its subsidiaries, while separate accounting keeps them
+        separate. Defaults to 'consolidated'.
 
         Raises:
             ValueError: If the accounting method is invalid.
         """
         return self._acc_unit
 
     @acc_method.setter
-    def acc_method(self, value: Literal["consolidated", "separate"]):
-        if value in {"consolidated", "separate"}:
-            # Set accounting method to upper case as in FinLogic Database
-            self._acc_method = value.upper()
+    def acc_method(self, value: Literal["con", "sep"]):
+        # Set accounting method to upper case as in FinLogic Database
+        if value == "con":
+            self._acc_method = "CONSOLIDATED"
+        elif value == "sep":
+            self._acc_method = "SEPARATE"
         else:
             raise ValueError("acc_method expects 'consolidated' or 'separate'")
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_dfc()
+            self._set_df()
 
     @property
     def acc_unit(self) -> float:
         """Gets or sets the accounting unit for the financial statements.
 
         The "acc_unit" is a constant that will divide all company
         accounting values. The constant must be a number greater than
         zero or one of the following strings:
-            - "thousand" to represent thousands       (1,000)
-            - "million" to represent millions     (1,000,000)
-            - "billion" to represent billions (1,000,000,000)
+            - "t" to represent thousands       (1,000)
+            - "m" to represent millions     (1,000,000)
+            - "b" to represent billions (1,000,000,000)
 
         Returns:
             The current accounting unit.
 
         Raises:
             ValueError: If the accounting unit is invalid.
 
         Examples:
             To set the accounting unit to millions:
-                company.acc_unit = "million"
+                company.acc_unit = "m"
 
             To set the accounting unit to a custom factor, e.g., 10,000:
                 company.acc_unit = 10_000
         """
         return self._acc_unit
 
     @acc_unit.setter
-    def acc_unit(self, value: int | float | str) -> float | int:
+    def acc_unit(self, value: int | float | Literal["t", "m", "b"]):
         match value:
-            case "thousand":
+            case "t":
                 self._acc_unit = 1_000
-            case "million":
+            case "m":
                 self._acc_unit = 1_000_000
-            case "billion":
+            case "b":
                 self._acc_unit = 1_000_000_000
             case str():  # Add this case to catch invalid strings
                 raise ValueError("Invalid string for Accounting Unit")
             case v if v > 0:
-                self._acc_unit = v
+                self._acc_unit = float(v)
             case _:
                 raise ValueError("Accounting Unit is invalid")
 
         # If object was already initialized, reset company dataframe
         if self._initialized:
-            self._set_dfc()
+            self._set_df()
 
     @property
     def tax_rate(self) -> float:
         """Gets or sets company 'tax_rate' property.
 
         The "tax_rate" is used to calculate some of the company
         indicators, such as EBIT and net income. The default value
@@ -223,250 +238,257 @@
         Raises:
             KeyError: If the provided language is not supported.
         """
 
         return self._language
 
     @language.setter
-    def language(self, language: str):
+    def language(self, language: Literal["english", "portuguese"]):
         # Supported languages
         list_languages = ["english", "portuguese"]
         if language.lower() in list_languages:
             self._language = language.capitalize()
         else:
             sup_lang = f"Supported languages: {', '.join(list_languages)}"
             raise KeyError(f"'{language}' not supported. {sup_lang}")
 
-    def _set_dfc(self) -> pd.DataFrame:
+    def _set_df(self) -> pd.DataFrame:
         """Sets the company data frame.
 
-        This method creates a data frame with the company's financial
+        This method creates a dataframe with the company's financial
         statements.
         """
-        # Create the company data frame
         query = f"""
             SELECT *
               FROM reports
              WHERE cvm_id = {self._cvm_id}
                AND acc_method = '{self._acc_method}'
-             ORDER BY acc_code, period_reference, period_end
+             ORDER BY 
+                acc_code,
+                period_reference,
+                acc_fixed,
+                report_type,
+                period_begin,
+                period_end
         """
-        dfc = execute(query, "df")
+        df = execute(query, "df")
 
         # Change acc_unit only for accounts different from 3.99
-        dfc["acc_value"] = np.where(
-            dfc["acc_code"].str.startswith("3.99"),
-            dfc["acc_value"],
-            dfc["acc_value"] / self._acc_unit,
+        df["acc_value"] = np.where(
+            df["acc_code"].str.startswith("3.99"),
+            df["acc_value"],
+            df["acc_value"] / self._acc_unit,
+        )
+        annual_df = df.query('report_type == "ANNUAL"')
+        self._first_annual = annual_df["period_end"].min()
+        self._last_annual = annual_df["period_end"].max()
+        quarterly_df = df.query('report_type == "QUARTERLY"')
+        self._last_quarterly = quarterly_df["period_end"].max()
+        self._last_period = df["period_end"].max()
+
+        # Keep last quarterly report only if it is after the last annual report
+        # for calculating TTM values
+        df.query(
+            'report_type == "ANNUAL" or \
+             period_reference == @self._last_period',
+            inplace=True,
         )
-        annual_reports = dfc.query('report_type == "ANNUAL"')
-        self._first_annual = annual_reports["period_end"].min()
-        self._last_annual = annual_reports["period_end"].max()
-        quarterly_reports = dfc.query('report_type == "QUARTERLY"')
-        self._last_quarterly = quarterly_reports["period_end"].max()
 
-        # Drop columns that are already company atributes
-        dfc.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
+        # Drop columns that are already company attributes or will not be used
+        df.drop(
+            columns=[
+                "name_id",
+                "cvm_id",
+                "tax_id",
+                "acc_method",
+                "file_source",
+                "file_mtime",
+            ],
+            inplace=True,
+        )
 
-        # Keep only the newest 'report_version' in df
+        # Keep only the last value for the same account code and period (begin and end)
+        # The dataframe was already sorted by the SQL query.
         cols = [
-            "report_type",
-            "report_version",
-            "period_reference",
-            "period_order",
             "acc_code",
+            "period_begin",
+            "period_end",
         ]
-        dfc.sort_values(by=cols, ignore_index=True, inplace=True)
-        cols = dfc.columns.tolist()
-        cols_remove = ["report_version", "acc_value", "acc_fixed"]
-        [cols.remove(col) for col in cols_remove]
-        # Ascending order --> last is the newest report_version
-        dfc.drop_duplicates(cols, keep="last", inplace=True, ignore_index=True)
+        df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
 
         # Set company data frame
-        self._dfc = dfc
+        self._df = df
 
     def info(self) -> dict:
         """Print a concise summary of a company."""
         # Some companies have no quarterly reports (see cvm_id 9784)
         if self._last_quarterly is pd.NaT:
             last_quarterly = "No quarterly reports"
         else:
             last_quarterly = self._last_quarterly.strftime("%Y-%m-%d")
 
         company_info = {
             "Name": self.name_id,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self.tax_id,
-            "Total Accounting Rows": len(self._dfc.index),
+            "Total Accounting Rows": len(self._df.index),
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
             "Selected Tax Rate": self._tax_rate,
             "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
             "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
             "Last Quarterly Report": last_quarterly,
         }
         print_dict(info_dict=company_info, table_name="Company Info")
 
-    def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        # keep only last quarterly fs
-        if self._last_annual > self._last_quarterly:
-            df = dfi.query('report_type == "ANNUAL"').copy()
-            df.query(
-                "period_order == 'PREVIOUS' or \
-                 period_end == @self._last_annual",
-                inplace=True,
-            )
-        else:
-            df = dfi.query(
-                'report_type == "ANNUAL" or \
-                 period_end == @self._last_quarterly'
-            ).copy()
-            df.query(
-                "period_order == 'PREVIOUS' or \
-                 period_end == @self._last_quarterly or \
-                 period_end == @self._last_annual",
-                inplace=True,
-            )
-
-        # Create output dataframe with only the index
-        dfo = df.sort_values(by="period_end", ascending=True)[
-            ["acc_name", "acc_code", "acc_fixed"]
-        ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
+    def _build_report_index(self, dfi: pd.DataFrame) -> pd.DataFrame:
+        """Build the index for the report."""
+        # "acc_code" works as a primary key. Other columns set the preference order
+        df = (
+            dfi[["acc_code", "acc_fixed", "acc_name", "period_reference"]]
+            .sort_values(by=["acc_code", "acc_fixed", "period_reference"])
+            .drop_duplicates(subset=["acc_code"], keep="last", ignore_index=True)[
+                ["acc_code", "acc_name"]
+            ]
+        )
+        return df
 
-        periods = sorted(df["period_end"].drop_duplicates())
+    def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
+        # Start "dfo" with the index
+        dfo = self._build_report_index(dfi)
+        year_cols = ["acc_code", "acc_value"]
+        periods = sorted(dfi["period_end"].drop_duplicates())
         for period in periods:
-            year_cols = ["acc_value", "acc_code"]
-            df_year = df.query("period_end == @period")[year_cols].copy()
+            df_year = dfi.query("period_end == @period")[year_cols].copy()
             period_str = period.strftime("%Y-%m-%d")
             if period == self._last_quarterly:
                 period_str += " (ttm)"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
-
+        dfo.fillna(0, inplace=True)
         return dfo.sort_values("acc_code", ignore_index=True)
 
     def report(
         self,
         report_type: str,
-        acc_level: int | None = None,
+        acc_level: int = 0,
         num_years: int = 0,
     ) -> pd.DataFrame:
         """Generate an accounting report for the company.
 
         This function generates a report representing one of the financial
         statements for the company adjusted by the attributes passed.
 
         Args:
-            report_type: Type of financial report to be generated. Options
-                include: "assets", "cash", "current_assets",
-                "non_current_assets", "liabilities", "debt",
-                "current_liabilities", "non_current_liabilities",
-                "liabilities_and_equity", "equity", "income",
-                "earnings_per_share", "comprehensive_income",
-                "changes_in_equity", "cash_flow" and "added_value".
-            acc_level: Detail level to show for account codes. Options are 2,
-                3, 4 or None. Defaults to None. How the values works:
+            report_type: Type of financial report to be generated. Options are:
+                - balance_sheet
+                    - assets
+                        - cash
+                        - current_assets,
+                        - non_current_assets
+                    - liabilities
+                        - debt
+                        - current_liabilities
+                        - non_current_liabilities,
+                    - liabilities_and_equity
+                        - equity
+                - income_statement
+                - cash_flow
+                - earnings_per_share
+                - comprehensive_income,
+                - added_value
+            acc_level: Detail level to show for account codes. Options are 0, 1,
+                2, 3 or 4. Defaults to 0. How the values works:
+                    0    -> X...       (show all accounts)
+                    1    -> X          (show 1 level)
                     2    -> X.YY       (show 2 levels)
                     3    -> X.YY.ZZ    (show 3 levels)
                     4    -> X.YY.ZZ.WW (show 4 levels)
-                    None -> X...       (default: show all accounts)
             num_years: Number of years to include in the report. Defaults to 0
                 (all years).
 
         Returns:
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
             ValueError: If some argument is invalid.
         """
+        # Copy company dataframe to avoid changing it
+        df = self._df.copy()
+        periods = sorted(df["period_end"].drop_duplicates())
+        if num_years > len(periods):
+            num_years = len(periods)
+        periods = periods[-num_years:]
+        df.query("period_end in @periods", inplace=True)
         # Check input arguments.
-        if acc_level not in {None, 2, 3, 4}:
-            raise ValueError("acc_level expects None, 2, 3 or 4")
+        if acc_level not in {0, 1, 2, 3, 4}:
+            raise ValueError("acc_level expects 0, 1, 2, 3 or 4")
 
-        df = self._dfc.copy()
+        # Filter dataframe for selected acc_level
+        # Example of an acc_code: "7.08.04.04" -> 4 levels and 3 dots
+        if acc_level:
+            df.query(rf"acc_code.str.count('\.') <= {acc_level - 1}", inplace=True)
 
         # Set language
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
 
         if self._language == "English":
             _pten_dict = dict(language_df.values)
             _pten_dict = MyDict(_pten_dict)
             df["acc_name"] = df["acc_name"].map(_pten_dict)
 
-        # Filter dataframe for selected acc_level
-        if acc_level:
-            acc_code_limit = acc_level * 3 - 2  # noqa
-            df.query("acc_code.str.len() <= @acc_code_limit", inplace=True)
         """
         Filter dataframe for selected report_type (report type)
         df['acc_code'].str[0].unique() -> [1, 2, 3, 4, 5, 6, 7]
         The first part of 'acc_code' is the report type
         Table of reports correspondence:
             1 -> Balance Sheet - Assets
             2 -> Balance Sheet - Liabilities and Shareholders’ Equity
             3 -> Income
             4 -> Comprehensive Income
             5 -> Changes in Equity
             6 -> Cash Flow (Indirect Method)
             7 -> Added Value
         """
         report_types = {
-            "assets": ["1"],
-            "cash": ["1.01.01", "1.01.02"],
-            "current_assets": ["1.01"],
-            "non_current_assets": ["1.02"],
-            "liabilities": ["2.01", "2.02"],
-            "debt": ["2.01.04", "2.02.01"],
-            "current_liabilities": ["2.01"],
-            "non_current_liabilities": ["2.02"],
-            "liabilities_and_equity": ["2"],
-            "equity": ["2.03"],
-            "income": ["3"],
-            "earnings_per_share": ["3.99"],
-            "comprehensive_income": ["4"],
-            "changes_in_equity": ["5"],
-            "cash_flow": ["6"],
-            "added_value": ["7"],
+            "balance_sheet": ("1", "2"),
+            "income_statement": ("3"),
+            "cash_flow": ("6"),
+            "earnings_per_share": ("3.99"),
+            "comprehensive_income": ("4"),
+            "added_value": ("7"),
+            "assets": ("1"),
+            "cash": ("1.01.01", "1.01.02"),
+            "current_assets": ("1.01"),
+            "non_current_assets": ("1.02"),
+            "liabilities": ("2.01", "2.02"),
+            "debt": ("2.01.04", "2.02.01"),
+            "current_liabilities": ("2.01"),
+            "non_current_liabilities": ("2.02"),
+            "liabilities_and_equity": ("2"),
+            "equity": ("2.03"),
         }
-        acc_codes = report_types[report_type]
-        expr = ""
-        for count, acc_code in enumerate(acc_codes):
-            if count > 0:
-                expr += " or "
-            expr += f'acc_code.str.startswith("{acc_code}")'
-        df.query(expr, inplace=True)
+        acc_codes = report_types[report_type]  # noqa
+        df.query("acc_code.str.startswith(@acc_codes)", inplace=True)
+        df.reset_index(drop=True, inplace=True)
 
-        # remove earnings per share from income statment
-        if report_type == "income":
+        if report_type in {"income_statement", "cash_flow"}:
+            # remove earnings per share from income statment
             df = df[~df["acc_code"].str.startswith("3.99")]
-
-        if report_type in {"income", "cash_flow"}:
             df = self._calculate_ttm(df)
 
-        df.reset_index(drop=True, inplace=True)
-
-        report_df = self._build_report(df)
-        report_df.set_index(keys="acc_code", drop=True, inplace=True)
-        # Show only selected years
-        if num_years > 0:
-            cols = report_df.columns.to_list()
-            cols = cols[0:2] + cols[-num_years:]
-            report_df = report_df[cols]
-        # Fill NaN values with 0
-        report_df.fillna(0, inplace=True)
-        return report_df
+        return self._build_report(df)
 
     def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
         if self._last_annual > self._last_quarterly:
-            return dfi.query('report_type == "ANNUAL"').copy()
+            return dfi.query('report_type == "ANNUAL"')
 
         df1 = dfi.query("period_end == @self._last_quarterly").copy()
         df1.query("period_begin == period_begin.min()", inplace=True)
 
         df2 = dfi.query("period_reference == @self._last_quarterly").copy()
         df2.query("period_begin == period_begin.min()", inplace=True)
         df2["acc_value"] = -df2["acc_value"]
@@ -503,19 +525,18 @@
 
         Returns:
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
             ValueError: If some argument is invalid.
         """
-        df_as = self.report("assets")
-        df_le = self.report("liabilities_and_equity")
-        df_is = self.report("income")
+        df_bs = self.report("balance_sheet")
+        df_is = self.report("income_statement")
         df_cf = self.report("cash_flow")
-        dfo = pd.concat([df_as, df_le, df_is, df_cf]).query("acc_code == @acc_list")
+        dfo = pd.concat([df_bs, df_is, df_cf]).query(f"acc_code == {acc_list}")
         # Show only selected years
         if num_years > 0:
             cols = dfo.columns.to_list()
             cols = cols[0:2] + cols[-num_years:]
             dfo = dfo[cols]
         return dfo
 
@@ -543,21 +564,23 @@
         References:
             [1] Aswath Damodaran, "Return on Capital (ROC), Return on Invested
                 Capital (ROIC) and Return on Equity (ROE): Measurement and
                 Implications.", 2007,
                 https://people.stern.nyu.edu/adamodar/pdfoles/papers/returnmeasures.pdf
                 https://people.stern.nyu.edu/adamodar/New_Home_Page/datafile/variable.htm
         """
-        df_as = self.report("assets")
-        df_le = self.report("liabilities_and_equity")
-        df_in = self.report("income")
+        df_bs = self.report("balance_sheet")
+        df_is = self.report("income_statement")
         df_cf = self.report("cash_flow")
-        df = pd.concat([df_as, df_le, df_in, df_cf]).drop(
-            columns=["acc_fixed", "acc_name"]
+        df = (
+            pd.concat([df_bs, df_is, df_cf])
+            .drop(columns=["acc_name"])
+            .set_index("acc_code", drop=True)
         )
+
         # Calculate indicators series
         revenues = df.loc["3.01"]
         gross_profit = df.loc["3.03"]
         ebit = df.loc["3.05"]
         ebt = df.loc["3.07"]
         effective_tax = df.loc["3.08"]
         depreciation_amortization = df.loc["6.01.01.04"]
```

### Comparing `finlogic-0.4.4/finlogic/cvm.py` & `finlogic-0.4.5/finlogic/cvm.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,73 +111,100 @@
         "VERSAO": "report_version",
         "DT_REFER": "period_reference",
         "DT_INI_EXERC": "period_begin",
         "DT_FIM_EXERC": "period_end",
         "ORDEM_EXERC": "period_order",
         "CD_CONTA": "acc_code",
         "DS_CONTA": "acc_name",
+        "COLUNA_DF": "es_name",  # equity_statement_name
         "ST_CONTA_FIXA": "acc_fixed",
         "VL_CONTA": "acc_value",
-        "COLUNA_DF": "equity_statement",
-        # Columns below will be dropped after processing.
         "GRUPO_DFP": "report_group",
         "MOEDA": "Currency",
         "ESCALA_MOEDA": "currency_unit",
     }
     df = df.rename(columns=columns_translation)[columns_translation.values()]
 
     # Currency column has only one value (BRL) so it is not necessary.
     df = df.drop(columns=["Currency"])
 
+    # The CVM file stores only the last report_version -> drop it.
+    df = df.drop(columns=["report_version"])
+    # report_version max. value is aprox. 9, so it can be uint8 (0 to 255)
+    # df["report_version"] = df["report_version"].astype("uint8")
+
+    # acc_fixed values are ['S', 'N']
+    map_dic = {"S": True, "N": False}
+    df["acc_fixed"] = df["acc_fixed"].map(map_dic).astype(bool)
+
     # Remove rows with acc_value == 0 and acc_fixed == False
-    df.query("acc_value != 0 or acc_fixed == True", inplace=True)
+    # df.query("acc_value != 0 or acc_fixed == True", inplace=True)
+    df.query("acc_value != 0", inplace=True)
 
-    # report_version max. value is aprox. 9, so it can be uint8 (0 to 255)
-    df["report_version"] = df["report_version"].astype("uint8")
-    # cvm_id from max. value is 600_000, so it can be uint32 (0 to 4_294_967_295)
+    # acc_fixed is being used used only non fixed accounts with acc_value == 0
+    # So it can be dropped after the query above.
+    # df = df.drop(columns=["acc_fixed"])
+
+    # cvm_id max. value is 600_000, so it can be uint32 (0 to 4_294_967_295)
     df["cvm_id"] = df["cvm_id"].astype("uint32")
+
     # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
     # In database, "report_type" is positioned after "tax_id" -> position = 3
     if filepath.name.startswith("dfp"):
         df.insert(loc=3, column="report_type", value="ANNUAL")
     else:
         df.insert(loc=3, column="report_type", value="QUARTERLY")
 
+    # For the moment, es_name will not be used since it adds to much complexity to
+    # the database. It will be dropped.
+    df = df.drop(columns=["es_name"])
     # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
-    columns = ["name_id", "acc_name", "equity_statement"]
-    df[columns] = df[columns].apply(remove_empty_spaces)
+    # columns = ["name_id", "acc_name", "es_name"]
+    # df[columns] = df[columns].apply(remove_empty_spaces)
 
     # Replace "BCO " with "BANCO " in "name_id" column.
     df["name_id"] = df["name_id"].str.replace("BCO ", "BANCO ")
 
     # Convert string columns to categorical before mapping.
     columns = df.select_dtypes(include="object").columns
     df[columns] = df[columns].astype("category")
 
-    # "acc_fixed" values are: 'S', 'N'
-    map_dic = {"S": True, "N": False}
-    df["acc_fixed"] = df["acc_fixed"].map(map_dic).astype(bool)
     # currency_unit values are ['MIL', 'UNIDADE']
     map_dic = {"UNIDADE": 1, "MIL": 1000}
     df["currency_unit"] = df["currency_unit"].map(map_dic).astype(int)
 
     # Do not ajust acc_value for 3.99 codes.
     df["acc_value"] = df["acc_value"].where(
         df["acc_code"].str.startswith("3.99"),
         df["acc_value"] * df["currency_unit"],
     )
+    # After the adjustment, currency_unit column is not necessary.
     df.drop(columns=["currency_unit"], inplace=True)
 
-    # "period_order" values are: 'ÚLTIMO', 'PENÚLTIMO'
-    map_dic = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
-    df["period_order"] = df["period_order"].map(map_dic)
+    """The "period_order" column is a redundant information, since it is possible to
+    infer it from the "period_reference", "period_begin" and "period_end" columns.
+    For example:
+        if "period_reference" is 2020-12-31
+           "period_begin" is 2020-01-01
+           "period_end" is 2020-12-31
+        then "period_order" is "LAST".
+
+        If "period_reference" is 2020-12-31
+           "period_begin" is 2019-01-01
+           "period_end" is 2019-12-31
+        then "period_order" is "PREVIOUS".
+    Old code:
+        "period_order" values are: 'ÚLTIMO', 'PENÚLTIMO'
+        map_dic = {"ÚLTIMO": "LAST", "PENÚLTIMO": "PREVIOUS"}
+        df["period_order"] = df["period_order"].map(map_dic)
     """
-    acc_method -> Financial Statemen Type
-    Consolidated and Separate Financial Statements (IAS 27/2003)
-    df['GRUPO_DFP'].unique() result:
+    df = df.drop(columns=["period_order"])
+
+    """
+    df['report_group'].unique() result:
         'DF Consolidado - Balanço Patrimonial Ativo',
         'DF Consolidado - Balanço Patrimonial Passivo',
         'DF Consolidado - Demonstração das Mutações do Patrimônio Líquido',
         'DF Consolidado - Demonstração de Resultado Abrangente',
         'DF Consolidado - Demonstração de Valor Adicionado',
         'DF Consolidado - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Consolidado - Demonstração do Resultado',
@@ -188,22 +215,19 @@
         'DF Individual - Demonstração de Valor Adicionado',
         'DF Individual - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
-    map_dic = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
-    df.insert(9, "acc_method", df["report_group"].str[3:6].map(map_dic))
-    # 'GRUPO_DFP' data can be inferred from 'acc_code'
+    map_dic = {"DF C": "CONSOLIDATED", "DF I": "SEPARATE"}
+    df.insert(9, "acc_method", df["report_group"].str[:4].map(map_dic))
+    # 'report_group' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
 
-    # Correct/harmonize some account texts.
-    # df["acc_name"].replace(to_replace=["\xa0ON\xa0", "On"], value="ON", inplace=True)
-
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
     cols.remove("acc_value")
     df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
```

### Comparing `finlogic-0.4.4/finlogic/database.py` & `finlogic-0.4.5/finlogic/database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.4/finlogic/fduckdb.py` & `finlogic-0.4.5/finlogic/fduckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def get_info() -> dict:
     """Return a dictionary with information about the database."""
     info_dict = {}
     if is_empty():
         return info_dict
 
     query = """--sql
-        SELECT DISTINCT cvm_id, report_version, report_type, period_reference
+        SELECT DISTINCT cvm_id, report_type, period_reference
           FROM reports;
     """
     num_of_reports = execute(query, "df").shape[0]
     db_last_modified = datetime.fromtimestamp(FINLOGIC_DB_PATH.stat().st_mtime)
     query = "SELECT COUNT(*) FROM reports"
     number_of_rows = execute(query, "fetchone")[0]
     query = "SELECT MIN(period_end) FROM reports"
```

### Comparing `finlogic-0.4.4/finlogic/fprint.py` & `finlogic-0.4.5/finlogic/fprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.4/finlogic/language.py` & `finlogic-0.4.5/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.4/pyproject.toml` & `finlogic-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,23 @@
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "duckdb>=0.7.0",
     "rich>=13.0.0",
 ]
-version = "0.4.4"
+version = "0.4.5"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
-test = [
-    "pytest>=7.0.0",
+dev = [
+    "pytest",
+    "ipykernel",
 ]
 
 [project.urls]
 repository = "https://github.com/crdcj/FinLogic"
 
 [tool.pdm.version]
 source = "file"
```

### Comparing `finlogic-0.4.4/tests/test_company.py` & `finlogic-0.4.5/tests/test_company.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest
 import finlogic as fl
 
 
 class TestCompany(unittest.TestCase):
     def setUp(self):
-        self.petro_sep = fl.Company(9512, acc_method="separate", acc_unit="billion")
-        self.petro_con = fl.Company(9512, acc_method="consolidated", acc_unit="billion")
+        self.petro_sep = fl.Company(9512, acc_method="sep", acc_unit="b")
+        self.petro_con = fl.Company(9512, acc_method="con", acc_unit="b")
 
     def test_identifier(self):
-        """Test the identifier method of the Company class.""" ""
+        """Test the identifier method of the Company class."""
         test_cvm_id = 4170
         test_tax_id = "33.592.510/0001-54"
         self.petro_sep.identifier = test_cvm_id
         self.assertEqual(self.petro_sep._cvm_id, test_cvm_id)
         self.assertEqual(self.petro_sep.tax_id, test_tax_id)
 
         self.petro_sep.identifier = test_tax_id
@@ -34,17 +34,17 @@
         self.assertEqual(self.petro_sep.tax_id, "33.000.167/0001-01")
 
     def test_report(self):
         """Test if the report method of the Company class returns the correct
         values."""
         petro_report = self.petro_con.report(report_type="assets")
         # Get Total Assets
-        assets_2009 = round(petro_report.at["1", "2009-12-31"], 3)
-        assets_2015 = round(petro_report.at["1", "2015-12-31"], 3)
-        assets_2020 = round(petro_report.at["1", "2020-12-31"], 3)
+        assets_2009 = round(petro_report.query("acc_code == '1'")["2009-12-31"][0], 3)
+        assets_2015 = round(petro_report.query("acc_code == '1'")["2015-12-31"][0], 3)
+        assets_2020 = round(petro_report.query("acc_code == '1'")["2020-12-31"][0], 3)
         # Check the reports
         self.assertEqual(assets_2009, 350.419)
         self.assertEqual(assets_2015, 900.135)
         self.assertEqual(assets_2020, 987.419)
 
     def test_indicators(self):
         # Petro indicators (separate)
```

### Comparing `finlogic-0.4.4/tests/test_database.py` & `finlogic-0.4.5/tests/test_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TestDatabase(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
         db_info = fdb.get_info()
         self.assertEqual(db_info["first_report"], "2009-01-31")
-        self.assertTrue(db_info["number_of_rows"] > 8_000_000)
+        self.assertTrue(db_info["number_of_rows"] > 7_000_000)
 
     def test_search_company(self):
         """Test the search_company method of the Database module."""
         search_result = fl.search_company("petrobras")
         """
             name_id                            cvm_id  tax_id
         0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
```

### Comparing `finlogic-0.4.4/PKG-INFO` & `finlogic-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.4
+Version: 0.4.5
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -32,16 +32,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: duckdb>=0.7.0
 Requires-Dist: rich>=13.0.0
-Requires-Dist: pytest>=7.0.0; extra == "test"
-Provides-Extra: test
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ipykernel; extra == "dev"
+Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-blue.svg)](https://github.com/psf/black)
```

