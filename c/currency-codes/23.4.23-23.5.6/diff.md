# Comparing `tmp/currency_codes-23.4.23.tar.gz` & `tmp/currency_codes-23.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currency_codes-23.4.23.tar", max compression
+gzip compressed data, was "currency_codes-23.5.6.tar", max compression
```

## Comparing `currency_codes-23.4.23.tar` & `currency_codes-23.5.6.tar`

### file list

```diff
@@ -1,17 +1,12 @@
--rw-r--r--   0        0        0     3753 2023-04-23 12:02:31.250775 currency_codes-23.4.23/README.md
--rw-r--r--   0        0        0      475 2023-04-23 12:02:31.258109 currency_codes-23.4.23/currency_codes/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 09:13:33.109933 currency_codes-23.4.23/currency_codes/assets/__init__.py
--rw-r--r--   0        0        0      176 2023-04-23 09:18:04.594804 currency_codes-23.4.23/currency_codes/assets/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      610 2023-04-23 12:02:37.814748 currency_codes-23.4.23/currency_codes/assets/__pycache__/commodity.cpython-39.pyc
--rw-r--r--   0        0        0     3290 2023-04-23 12:02:37.816470 currency_codes-23.4.23/currency_codes/assets/__pycache__/crypto.cpython-39.pyc
--rw-r--r--   0        0        0     7118 2023-04-23 12:02:37.818082 currency_codes-23.4.23/currency_codes/assets/__pycache__/fiat.cpython-39.pyc
--rw-r--r--   0        0        0     1591 2023-04-23 12:02:37.818798 currency_codes-23.4.23/currency_codes/assets/__pycache__/other.cpython-39.pyc
--rw-r--r--   0        0        0      493 2023-04-23 12:02:31.207620 currency_codes-23.4.23/currency_codes/assets/commodity.py
--rw-r--r--   0        0        0     7117 2023-04-23 12:02:31.255131 currency_codes-23.4.23/currency_codes/assets/crypto.py
--rw-r--r--   0        0        0    12934 2023-04-23 12:02:31.231405 currency_codes-23.4.23/currency_codes/assets/fiat.py
--rw-r--r--   0        0        0     2309 2023-04-23 12:02:31.217671 currency_codes-23.4.23/currency_codes/assets/other.py
--rw-r--r--   0        0        0      443 2023-04-22 11:32:57.255197 currency_codes-23.4.23/currency_codes/exceptions.py
--rw-r--r--   0        0        0     1734 2023-04-23 12:02:31.240990 currency_codes-23.4.23/currency_codes/main.py
--rw-r--r--   0        0        0      527 2023-04-22 11:32:57.266042 currency_codes-23.4.23/currency_codes/models.py
--rw-r--r--   0        0        0      995 2023-04-23 12:02:31.219093 currency_codes-23.4.23/pyproject.toml
--rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 currency_codes-23.4.23/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-06 13:04:34.509440 currency_codes-23.5.6/LICENSE
+-rw-r--r--   0        0        0     3609 2023-05-06 13:04:34.509440 currency_codes-23.5.6/README.md
+-rw-r--r--   0        0        0      406 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 13:05:15.662226 currency_codes-23.5.6/currency_codes/assets/__init__.py
+-rw-r--r--   0        0        0    10607 2023-05-06 21:04:45.707666 currency_codes-23.5.6/currency_codes/assets/crypto.py
+-rw-r--r--   0        0        0    13074 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/assets/fiat.py
+-rw-r--r--   0        0        0     2770 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/assets/other.py
+-rw-r--r--   0        0        0      443 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/exceptions.py
+-rw-r--r--   0        0        0     1748 2023-05-06 13:04:34.513440 currency_codes-23.5.6/currency_codes/main.py
+-rw-r--r--   0        0        0      699 2023-05-06 21:04:45.707666 currency_codes-23.5.6/currency_codes/models.py
+-rw-r--r--   0        0        0     1027 2023-05-06 21:04:45.711666 currency_codes-23.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 currency_codes-23.5.6/PKG-INFO
```

### Comparing `currency_codes-23.4.23/README.md` & `currency_codes-23.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ## Description
 Comprehensive Python package for managing currency codes across different types of assets. Having all the currency codes in one package can simplify the development process for applications that involve multiple currencies and assets. This package could also help to ensure consistency and accuracy in managing currency codes across different parts of an application  
 The package provides currency codes for different types of assets. Such as 
 - fiat (US dollar, UAE Dirham, ...)
 - crypto (Bitcoin, Solana, ...)
-- commodity (Palladium, Gold, ...)
-- others (WIR Franc, CFP Franc, ...) 
+- others (Palladium, Gold, WIR Franc, CFP Franc, ...) 
 
 ## Sources
  - [Coinmarketcap website](https://coinmarketcap.com) for crypto
  - [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
 
 ## Installation
 Install the package with the following command:
 ```shell
 pip install currency_codes
 ```
 
-## How to use the package?
+## How to use the package
 ### Get a currency info by a currency code
 You can get any currency info using the snippet below
 ```python
 from currency_codes import get_currency_by_code, Currency
 
 currency_code: str = "EUR"
 currency: Currency = get_currency_by_code(currency_code)
@@ -82,22 +81,17 @@
 If you want to get information only about crypto currencies, you can use `get_crypto_currencies` function
 ```python
 from currency_codes import get_crypto_currencies, Currency
 
 crypto_currencies: list[Currency] = get_crypto_currencies()
 ```
 
-### Get the list of commodity currencies
-If you want to get information only about commodity currencies, you can use `get_commodity_currencies` function
-```python
-from currency_codes import get_commodity_currencies, Currency
-
-commodity_currencies: list[Currency] = get_commodity_currencies()
-```
-
 ### Get the list of other currencies
 If you want to get information only about other currencies, you can use `get_other_currencies` function
 ```python
 from currency_codes import get_other_currencies, Currency
 
 other_currencies: list[Currency] = get_other_currencies()
 ```
+
+## How to contribute
+Contributions are always welcomed. If you found any mistakes or missing currencies, please raise a PR to make the package more accurate for all of us
```

### Comparing `currency_codes-23.4.23/currency_codes/assets/fiat.py` & `currency_codes-23.5.6/currency_codes/assets/fiat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+from typing import List
+
 from currency_codes.models import Currency
 
 
-def get_fiat_currencies() -> list[Currency]:
+def get_fiat_currencies() -> List[Currency]:
+    """Provides a list of fiat currencies
+
+    Returns:
+        List of Currency: list of fiat currencies
+    """
+
     return _fiat_currencies
 
 
-_fiat_currencies: list[Currency] = [
+_fiat_currencies: List[Currency] = [
     Currency(name="Afghani", code="AFN", numeric_code="971", minor_units=2),
     Currency(name="Euro", code="EUR", numeric_code="978", minor_units=2),
     Currency(name="Lek", code="ALL", numeric_code="008", minor_units=2),
     Currency(name="Algerian Dinar", code="DZD", numeric_code="012", minor_units=2),
     Currency(name="US Dollar", code="USD", numeric_code="840", minor_units=2),
     Currency(name="Kwanza", code="AOA", numeric_code="973", minor_units=2),
     Currency(name="East Caribbean Dollar", code="XCD", numeric_code="951", minor_units=2),
```

### Comparing `currency_codes-23.4.23/currency_codes/assets/other.py` & `currency_codes-23.5.6/currency_codes/assets/other.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+from typing import List
+
 from currency_codes.models import Currency
 
 
-def get_other_currencies() -> list[Currency]:
+def get_other_currencies() -> List[Currency]:
+    """Provides a list of other currencies
+
+    Returns:
+        List of Currency: list of other currencies
+    """
+
     return _other_currencies
 
 
-_other_currencies: list[Currency] = [
+_other_currencies: List[Currency] = [
+    Currency(name="Palladium", code="XPD", numeric_code="964", minor_units=None),
+    Currency(name="Platinum", code="XPT", numeric_code="962", minor_units=None),
+    Currency(name="Gold", code="XAU", numeric_code="959", minor_units=None),
+    Currency(name="Silver", code="XAG", numeric_code="961", minor_units=None),
     Currency(name="Sucre", code="XSU", numeric_code="994", minor_units=None),
     Currency(name="CFP Franc", code="XPF", numeric_code="953", minor_units=0),
     Currency(name="CFA Franc BEAC", code="XAF", numeric_code="950", minor_units=0),
     Currency(name="US Dollar (Next day)", code="USN", numeric_code="997", minor_units=2),
     Currency(name="Unidad Previsional", code="UYW", numeric_code="927", minor_units=4),
     Currency(name="Mvdol", code="BOV", numeric_code="984", minor_units=2),
     Currency(name="Unidad de Fomento", code="CLF", numeric_code="990", minor_units=4),
```

### Comparing `currency_codes-23.4.23/currency_codes/main.py` & `currency_codes-23.5.6/currency_codes/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-from currency_codes.assets.commodity import get_commodity_currencies
+from typing import List
+
 from currency_codes.assets.crypto import get_crypto_currencies
 from currency_codes.assets.fiat import get_fiat_currencies
 from currency_codes.assets.other import get_other_currencies
 from currency_codes.exceptions import CurrencyNotFoundError
 from currency_codes.models import Currency
 
 
-def get_all_currencies() -> list[Currency]:
+def get_all_currencies() -> List[Currency]:
+    """Provides a list of all currencies
+
+    Returns:
+        List of Currency: list of all currencies
+    """
+
     fiat = get_fiat_currencies()
     crypto = get_crypto_currencies()
-    commodity = get_commodity_currencies()
     other = get_other_currencies()
-    return fiat + crypto + commodity + other
+    return fiat + crypto + other
 
 
 def get_currency_by_code(code: str, case_sensitive: bool = False) -> Currency:
     """Provides a currency by a code
 
     Args:
         code (str): country code
@@ -51,8 +57,8 @@
 
     for currency in currencies:
         if currency.numeric_code == numeric_code:
             return currency
     raise CurrencyNotFoundError("numeric code", numeric_code)
 
 
-currencies: list[Currency] = get_all_currencies()
+currencies: List[Currency] = get_all_currencies()
```

### Comparing `currency_codes-23.4.23/pyproject.toml` & `currency_codes-23.5.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "currency_codes"
-version = "23.04.23"
+version = "23.05.06"
 description = "All currency codes in one package"
 authors = ["Artem Kuchumov <duketemon@gmail.com>"]
 keywords = ["ISO 4217", "ISO-4217", "Currency Codes", "Currencies", "fiat", "crypto", "commodity"]
 readme = "README.md"
-homepage = "https://github.com/duketemon/currency-codes"
-repository = "https://github.com/duketemon/currency-codes"
+homepage = "https://github.com/duketemon/currency_codes/blob/main/README.md#description"
+repository = "https://github.com/duketemon/currency_codes"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `currency_codes-23.4.23/PKG-INFO` & `currency_codes-23.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: currency-codes
-Version: 23.4.23
+Version: 23.5.6
 Summary: All currency codes in one package
-Home-page: https://github.com/duketemon/currency-codes
+Home-page: https://github.com/duketemon/currency_codes/blob/main/README.md#description
 Keywords: ISO 4217,ISO-4217,Currency Codes,Currencies,fiat,crypto,commodity
 Author: Artem Kuchumov
 Author-email: duketemon@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/duketemon/currency-codes
+Project-URL: Repository, https://github.com/duketemon/currency_codes
 Description-Content-Type: text/markdown
 
 ## Description
 Comprehensive Python package for managing currency codes across different types of assets. Having all the currency codes in one package can simplify the development process for applications that involve multiple currencies and assets. This package could also help to ensure consistency and accuracy in managing currency codes across different parts of an application  
 The package provides currency codes for different types of assets. Such as 
 - fiat (US dollar, UAE Dirham, ...)
 - crypto (Bitcoin, Solana, ...)
-- commodity (Palladium, Gold, ...)
-- others (WIR Franc, CFP Franc, ...) 
+- others (Palladium, Gold, WIR Franc, CFP Franc, ...) 
 
 ## Sources
  - [Coinmarketcap website](https://coinmarketcap.com) for crypto
  - [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
 
 ## Installation
 Install the package with the following command:
 ```shell
 pip install currency_codes
 ```
 
-## How to use the package?
+## How to use the package
 ### Get a currency info by a currency code
 You can get any currency info using the snippet below
 ```python
 from currency_codes import get_currency_by_code, Currency
 
 currency_code: str = "EUR"
 currency: Currency = get_currency_by_code(currency_code)
@@ -100,23 +99,18 @@
 If you want to get information only about crypto currencies, you can use `get_crypto_currencies` function
 ```python
 from currency_codes import get_crypto_currencies, Currency
 
 crypto_currencies: list[Currency] = get_crypto_currencies()
 ```
 
-### Get the list of commodity currencies
-If you want to get information only about commodity currencies, you can use `get_commodity_currencies` function
-```python
-from currency_codes import get_commodity_currencies, Currency
-
-commodity_currencies: list[Currency] = get_commodity_currencies()
-```
-
 ### Get the list of other currencies
 If you want to get information only about other currencies, you can use `get_other_currencies` function
 ```python
 from currency_codes import get_other_currencies, Currency
 
 other_currencies: list[Currency] = get_other_currencies()
 ```
 
+## How to contribute
+Contributions are always welcomed. If you found any mistakes or missing currencies, please raise a PR to make the package more accurate for all of us
+
```

