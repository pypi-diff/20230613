# Comparing `tmp/pypara-0.0.8.tar.gz` & `tmp/pypara-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypara-0.0.8.tar", last modified: Fri May 18 06:57:43 2018, max compression
+gzip compressed data, was "dist/pypara-0.0.9.tar", last modified: Tue Jul 17 05:53:52 2018, max compression
```

## Comparing `pypara-0.0.8.tar` & `pypara-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-05-18 06:57:43.000000 pypara-0.0.8/
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara/
--rw-r--r--   0 vst       (1000) vst       (1000)    22717 2018-05-18 06:51:14.000000 pypara-0.0.8/pypara/currencies.py
--rw-r--r--   0 vst       (1000) vst       (1000)       61 2018-05-18 06:56:55.000000 pypara-0.0.8/pypara/__init__.py
--rw-r--r--   0 vst       (1000) vst       (1000)    17917 2018-04-27 06:33:32.000000 pypara-0.0.8/pypara/monetary.py
--rw-r--r--   0 vst       (1000) vst       (1000)     4462 2018-04-27 06:33:32.000000 pypara-0.0.8/pypara/exchange.py
--rw-r--r--   0 vst       (1000) vst       (1000)      635 2018-04-27 06:33:32.000000 pypara-0.0.8/pypara/generic.py
--rw-r--r--   0 vst       (1000) vst       (1000)       39 2018-04-27 06:33:32.000000 pypara-0.0.8/MANIFEST.in
--rw-r--r--   0 vst       (1000) vst       (1000)      110 2018-05-18 06:57:43.000000 pypara-0.0.8/setup.cfg
--rw-r--r--   0 vst       (1000) vst       (1000)      965 2018-04-27 06:33:32.000000 pypara-0.0.8/README.rst
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/
--rw-r--r--   0 vst       (1000) vst       (1000)       37 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/requires.txt
--rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-04-30 04:48:26.000000 pypara-0.0.8/pypara.egg-info/not-zip-safe
--rw-r--r--   0 vst       (1000) vst       (1000)      327 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/SOURCES.txt
--rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/dependency_links.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1762 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/PKG-INFO
--rw-r--r--   0 vst       (1000) vst       (1000)        7 2018-05-18 06:57:43.000000 pypara-0.0.8/pypara.egg-info/top_level.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1469 2018-04-27 06:33:32.000000 pypara-0.0.8/LICENSE.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1767 2018-04-27 06:33:32.000000 pypara-0.0.8/setup.py
--rw-r--r--   0 vst       (1000) vst       (1000)     1762 2018-05-18 06:57:43.000000 pypara-0.0.8/PKG-INFO
+drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/
+drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara/
+-rw-r--r--   0 vst       (1000) vst       (1000)    23927 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/currencies.py
+-rw-r--r--   0 vst       (1000) vst       (1000)    24168 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/dcc.py
+-rw-r--r--   0 vst       (1000) vst       (1000)       61 2018-07-17 03:32:28.000000 pypara-0.0.9/pypara/__init__.py
+-rw-r--r--   0 vst       (1000) vst       (1000)    37963 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/monetary.py
+-rw-r--r--   0 vst       (1000) vst       (1000)     5823 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/exchange.py
+-rw-r--r--   0 vst       (1000) vst       (1000)     1241 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/generic.py
+-rw-r--r--   0 vst       (1000) vst       (1000)       39 2018-04-27 06:33:32.000000 pypara-0.0.9/MANIFEST.in
+-rw-r--r--   0 vst       (1000) vst       (1000)      115 2018-07-17 05:53:52.000000 pypara-0.0.9/setup.cfg
+-rw-r--r--   0 vst       (1000) vst       (1000)      965 2018-04-27 06:33:32.000000 pypara-0.0.9/README.rst
+drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/
+-rw-r--r--   0 vst       (1000) vst       (1000)       37 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/requires.txt
+-rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-04-30 04:48:26.000000 pypara-0.0.9/pypara.egg-info/not-zip-safe
+-rw-r--r--   0 vst       (1000) vst       (1000)      341 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/SOURCES.txt
+-rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/dependency_links.txt
+-rw-r--r--   0 vst       (1000) vst       (1000)     1812 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/PKG-INFO
+-rw-r--r--   0 vst       (1000) vst       (1000)        7 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/top_level.txt
+-rw-r--r--   0 vst       (1000) vst       (1000)     1469 2018-04-27 06:33:32.000000 pypara-0.0.9/LICENSE.txt
+-rw-r--r--   0 vst       (1000) vst       (1000)     1842 2018-07-17 03:33:38.000000 pypara-0.0.9/setup.py
+-rw-r--r--   0 vst       (1000) vst       (1000)     1812 2018-07-17 05:53:52.000000 pypara-0.0.9/PKG-INFO
```

### Comparing `pypara-0.0.8/pypara/currencies.py` & `pypara-0.0.9/pypara/currencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from decimal import Decimal
-from typing import Dict, List, Tuple, Optional, Type, Any, Callable
-
 from collections import OrderedDict
+from decimal import Decimal
 from enum import Enum
+from typing import Dict, List, Tuple, Optional, Type, Any, Callable, NamedTuple
 
 from .generic import MaxPrecisionQuantizer, ProgrammingError, make_quantizer
 
 
 class CurrencyLookupError(LookupError):
     """
     Provides a currency lookup error.
@@ -37,164 +36,163 @@
     #: Defines crypto currency type.
     CRYPTO = "Crypto Currency"
 
     #: Defines alternative currency type.
     ALTERNATIVE = "Alernative"
 
 
-class Currency:
+class Currency(NamedTuple):
     """
     Defines currency value object model which is extending ISO 4217 to embrace other currency types.
 
     Note that you should not call :class:`Currency` constructor directly, but instead use the :method:`Currency.build`.
     :method:`Currency.build` is responsible of performing some checks before creating the currency.
 
-    >>> Currency("XXX", "My Currency", 2)
-    <Currency XXX>
-    >>> USD = Currency("USD", "US Dollars", 2)
+    Try with USD:
+
+    >>> USD = Currency.of("USD", "US Dollars", 2, CurrencyType.MONEY)
     >>> USD.quantize(Decimal("1.005"))
     Decimal('1.00')
     >>> USD.quantize(Decimal("1.015"))
     Decimal('1.02')
-    >>> JPY = Currency("JPY", "Japanese Yen", 0)
+
+    Now, with JPY which has a different precision than USD:
+
+    >>> JPY = Currency.of("JPY", "Japanese Yen", 0, CurrencyType.MONEY)
     >>> JPY.quantize(Decimal("0.5"))
     Decimal('0')
     >>> JPY.quantize(Decimal("1.5"))
     Decimal('2')
-    >>> ZZZ = Currency("ZZZ", "Some weird currency", -1)
+
+    And with a weird currency which has no fixed precision.
+
+    >>> ZZZ = Currency.of("ZZZ", "Some weird currency", -1, CurrencyType.CRYPTO)
     >>> ZZZ.quantize(Decimal("1.0000000000005"))
     Decimal('1.000000000000')
     >>> ZZZ.quantize(Decimal("1.0000000000015"))
     Decimal('1.000000000002')
-    >>> Currency("USD", "US Dollars", 2) == Currency("USD", "United States Dollars", 3)
+
+    Equalities:
+
+    >>> usd1 = Currency.of("USD", "US Dollars", 2, CurrencyType.MONEY)
+    >>> usd2 = Currency.of("USD", "US Dollars", 2, CurrencyType.MONEY)
+    >>> usdx = Currency.of("USD", "UX Dollars", 2, CurrencyType.MONEY)
+    >>> usd1 == usd2
     True
-    >>> Currency("USD", "US Dollars", 2) == Currency("EUR", "US Dollars", 2)
+    >>> usd1 == usdx
     False
-    >>> hash(Currency("USD", "US Dollars", 2)) == hash(Currency("USD", "United States Dollars", 3))
-    True
-    >>> hash(Currency("USD", "US Dollars", 2)) == hash("USD")
+    >>> hash(usd1) == hash(usd2)
     True
+    >>> hash(usd1) == hash(usdx)
+    False
     """
 
-    #: Limit instance attributes.
-    __slots__ = ["__code", "__name", "__decimals", "__quantizer", "__ctype"]
-
-    def __init__(self, code: str, name: str, decimals: int, ctype: CurrencyType = CurrencyType.MONEY) -> None:
-        """
-        Creates a currency value object model instance.
-        """
-        ## Check the code:
-        assert isinstance(code, str)
-        assert code.isalpha()
-        assert code.isupper()
-        assert " " not in code
+    #: Defines the code of the currency.
+    code: str
 
-        ## Check the name:
-        assert isinstance(name, str)
-        assert name
-        assert not name.startswith(" ")
-        assert not name.endswith(" ")
+    #: Defines the name of the currency.
+    name: str
 
-        ## Check the decimals:
-        assert isinstance(decimals, int)
-        assert decimals >= -1
+    #: Defines the number of decimals of the currency.
+    decimals: int
 
-        ## Check the ctype:
-        assert isinstance(ctype, CurrencyType)
+    #: Defines the type of the currency.
+    type: CurrencyType
 
-        ## Define the quantizer:
-        if decimals < 0:
-            quantizer = MaxPrecisionQuantizer
-        elif decimals == 0:
-            quantizer = Decimal("0")
-        else:
-            quantizer = make_quantizer(decimals)
+    #: Defines the quantiser of the currency.
+    quantizer: Decimal
 
-        ## Setup slots:
-        self.__code = code
-        self.__name = name
-        self.__decimals = decimals
-        self.__quantizer = quantizer
-        self.__ctype = ctype
+    #: Defines the pre-computed, cached hash.
+    hashcache: int
 
-    @property
-    def code(self) -> str:
+    def __eq__(self, other: Any) -> bool:
         """
-        Returns the code of the currency.
+        Checks if the `self` and `other` are same currencies.
         """
-        return self.__code
+        ## TODO: Can we optimise this without any changes in the semantics?
+        return other.__class__ == Currency and self[5] == other[5]  # type: ignore
 
-    @property
-    def name(self) -> str:
+    def __hash__(self) -> int:
         """
-        Returns the name of the currency.
+        Returns the pre-computed and cached hash.
         """
-        return self.__name
+        return self[5]
 
-    @property
-    def decimals(self) -> int:
-        """
-        Returns the number of decimal points as per the fractional units of the currency.
+    def quantize(self, qty: Decimal) -> Decimal:
         """
-        return self.__decimals
+        Quantizes the decimal ``qty`` wrt to ccy's minor units fraction. Note that
+        the [ROUND HALF TO EVEN](https://en.wikipedia.org/wiki/Rounding) method
+        is used for rounding purposes.
 
-    @property
-    def type(self) -> CurrencyType:
+        **Note** that the HALF-TO-EVEN method is inherited from the default decimal context instead of
+        explicitly passing it. Therefore, if call-site application is making changes to the default
+        context, the rounding method may not be HALF-TO-EVEN anymore.
         """
-        Returns the type of the currency.
-        """
-        return self.__ctype
+        return qty.quantize(self[4])
 
-    def __repr__(self) -> str:
+    @classmethod
+    def of(cls, code: str, name: str, decimals: int, type: CurrencyType) -> "Currency":
         """
-        Provides an internal string representation of the :class:`Currency` instance.
+        Attempts to create a currency instance and returns it.
         """
-        return f"<Currency {self.__code}>"
+        ## Check the code:
+        ProgrammingError.passert(isinstance(code, str), "Currency code must be a string")
+        ProgrammingError.passert(code.isalpha(), "Currency code must contain only alphabetic characters")
+        ProgrammingError.passert(code.isupper(), "Currency code must be all uppercase")
 
-    def __eq__(self, other: Any) -> bool:
-        """
-        Indicates if two currencies are same.
-        """
-        return isinstance(other, Currency) and self.code == other.code
+        ## Check the name:
+        ProgrammingError.passert(isinstance(name, str), "Currency name must be a string")
+        ProgrammingError.passert(name != "", "Currency name can not be empty")
+        ProgrammingError.passert(not (name.startswith(" ") or name.endswith(" ")), "Trim the currency name")
 
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the instance.
-        """
-        return hash(self.code)
+        ## Check the decimals:
+        ProgrammingError.passert(isinstance(decimals, int), "Number of decimals must be an integer")
+        ProgrammingError.passert(decimals >= -1, "Number of decimals can not be less than -1")
 
-    def quantize(self, qty: Decimal) -> Decimal:
-        """
-        Quantizes the decimal ``qty`` wrt to ccy's minor units fraction. Note that
-        the [ROUND HALF TO EVEN](https://en.wikipedia.org/wiki/Rounding) method
-        is used for rounding purposes.
-        """
-        return qty.quantize(self.__quantizer)
+        ## Check the type:
+        ProgrammingError.passert(isinstance(type, CurrencyType), "Currency Type must be of type `CurrencyType`")
+
+        ## Define the quantizer:
+        if decimals > 0:
+            quantizer = make_quantizer(decimals)
+        elif decimals < 0:
+            quantizer = MaxPrecisionQuantizer
+        else:
+            quantizer = Decimal("0")
+
+        ## By now, we should have all required instance attributes. However, we want to compute and cache the hash.
+        hashcode = hash((code, name, decimals, type, quantizer))
+
+        ## Done, create the currency object and return:
+        return Currency(code, name, decimals, type, quantizer, hashcode)
 
 
 class CurrencyRegistry:
     """
     Defines a currency registry model.
 
     >>> "USD" in Currencies
     True
     >>> Currencies.has("USD")
     True
     >>> "XXX" in Currencies
     False
     >>> Currencies.has("XXX")
     False
-    >>> Currencies["USD"]
-    <Currency USD>
-    >>> Currencies.get("USD")
-    <Currency USD>
-    >>> assert Currencies["USD"] == Currencies.get("USD")
+    >>> Currencies["USD"].code
+    'USD'
+    >>> Currencies["USD"].name
+    'US Dollar'
+    >>> Currencies["USD"].type.name
+    'MONEY'
+    >>> Currencies.get("USD") == Currencies["USD"]
+    True
     >>> Currencies.get("XXX")
-    >>> Currencies.get("XXX", default=Currencies["USD"])
-    <Currency USD>
+    >>> Currencies.get("XXX", default=Currencies["USD"]) == Currencies["USD"]
+    True
     >>> assert len(Currencies) == len(Currencies.all)
     >>> assert Currencies.codes == [currency.code for currency in Currencies.all]
     >>> assert Currencies.codenames == [(currency.code, currency.name) for currency in Currencies.all]
     """
 
     #: Defines the singleton instance.
     __instance = None  # type: CurrencyRegistry
@@ -304,18 +302,15 @@
 
     def get(self, code: str, default: Optional[Currency]=None) -> Optional[Currency]:
         """
         Returns the currency for the given code.
 
         Note that if the code is not a valid currency code, a currency lookup error is raised.
         """
-        try:
-            return self.__registry[code]
-        except KeyError:
-            return default
+        return self.__registry.get(code, default)
 
     @property
     def all(self) -> List["Currency"]:
         """
         Returns the list of currencies.
         """
         return self.__currencies
@@ -337,190 +332,190 @@
 
 #: Defines the global currencies registry.
 Currencies = CurrencyRegistry()
 
 
 ## Create and register currencies in one go:
 with Currencies as register:
-    register(Currency("AED", "UAE Dirham", 2, CurrencyType.MONEY))
-    register(Currency("AFN", "Afghani", 2, CurrencyType.MONEY))
-    register(Currency("ALL", "Lek", 2, CurrencyType.MONEY))
-    register(Currency("AMD", "Armenian Dram", 2, CurrencyType.MONEY))
-    register(Currency("ANG", "Netherlands Antillean Guilder", 2, CurrencyType.MONEY))
-    register(Currency("AOA", "Kwanza", 2, CurrencyType.MONEY))
-    register(Currency("ARS", "Argentine Peso", 2, CurrencyType.MONEY))
-    register(Currency("AUD", "Australian Dollar", 2, CurrencyType.MONEY))
-    register(Currency("AWG", "Aruban Florin", 2, CurrencyType.MONEY))
-    register(Currency("AZN", "Azerbaijanian Manat", 2, CurrencyType.MONEY))
-    register(Currency("BAM", "Convertible Mark", 2, CurrencyType.MONEY))
-    register(Currency("BBD", "Barbados Dollar", 2, CurrencyType.MONEY))
-    register(Currency("BCH", "Bitcoin Cash", -1, CurrencyType.CRYPTO))
-    register(Currency("BDT", "Taka", 2, CurrencyType.MONEY))
-    register(Currency("BGN", "Bulgarian Lev", 2, CurrencyType.MONEY))
-    register(Currency("BHD", "Bahraini Dinar", 3, CurrencyType.MONEY))
-    register(Currency("BIF", "Burundi Franc", 0, CurrencyType.MONEY))
-    register(Currency("BMD", "Bermudian Dollar", 2, CurrencyType.MONEY))
-    register(Currency("BND", "Brunei Dollar", 2, CurrencyType.MONEY))
-    register(Currency("BOB", "Boliviano", 2, CurrencyType.MONEY))
-    register(Currency("BOV", "Mvdol", 2, CurrencyType.MONEY))
-    register(Currency("BRL", "Brazilian Real", 2, CurrencyType.MONEY))
-    register(Currency("BSD", "Bahamian Dollar", 2, CurrencyType.MONEY))
-    register(Currency("BTC", "Bitcoin", -1, CurrencyType.CRYPTO))
-    register(Currency("BTN", "Ngultrum", 2, CurrencyType.MONEY))
-    register(Currency("BWP", "Pula", 2, CurrencyType.MONEY))
-    register(Currency("BYR", "Belarussian Ruble", 0, CurrencyType.MONEY))
-    register(Currency("BZD", "Belize Dollar", 2, CurrencyType.MONEY))
-    register(Currency("CAD", "Canadian Dollar", 2, CurrencyType.MONEY))
-    register(Currency("CDF", "Congolese Franc", 2, CurrencyType.MONEY))
-    register(Currency("CHE", "WIR Euro", 2, CurrencyType.MONEY))
-    register(Currency("CHF", "Swiss Franc", 2, CurrencyType.MONEY))
-    register(Currency("CHW", "WIR Franc", 2, CurrencyType.MONEY))
-    register(Currency("CLF", "Unidad de Fomento", 4, CurrencyType.MONEY))
-    register(Currency("CLP", "Chilean Peso", 0, CurrencyType.MONEY))
-    register(Currency("CNH", "Yuan Renminbi (Off-shore)", 2, CurrencyType.MONEY))
-    register(Currency("CNY", "Yuan Renminbi", 2, CurrencyType.MONEY))
-    register(Currency("COP", "Colombian Peso", 2, CurrencyType.MONEY))
-    register(Currency("COU", "Unidad de Valor Real", 2, CurrencyType.MONEY))
-    register(Currency("CRC", "Costa Rican Colon", 2, CurrencyType.MONEY))
-    register(Currency("CUC", "Peso Convertible", 2, CurrencyType.MONEY))
-    register(Currency("CUP", "Cuban Peso", 2, CurrencyType.MONEY))
-    register(Currency("CVE", "Cabo Verde Escudo", 2, CurrencyType.MONEY))
-    register(Currency("CZK", "Czech Koruna", 2, CurrencyType.MONEY))
-    register(Currency("DASH", "Dash", -1, CurrencyType.CRYPTO))
-    register(Currency("DJF", "Djibouti Franc", 0, CurrencyType.MONEY))
-    register(Currency("DKK", "Danish Krone", 2, CurrencyType.MONEY))
-    register(Currency("DOP", "Dominican Peso", 2, CurrencyType.MONEY))
-    register(Currency("DZD", "Algerian Dinar", 2, CurrencyType.MONEY))
-    register(Currency("EGP", "Egyptian Pound", 2, CurrencyType.MONEY))
-    register(Currency("EOS", "EOSIO", -1, CurrencyType.CRYPTO))
-    register(Currency("ERN", "Nakfa", 2, CurrencyType.MONEY))
-    register(Currency("ETB", "Ethiopian Birr", 2, CurrencyType.MONEY))
-    register(Currency("ETC", "Ethereum Classic", -1, CurrencyType.CRYPTO))
-    register(Currency("ETH", "Ethereum", -1, CurrencyType.CRYPTO))
-    register(Currency("EUR", "Euro", 2, CurrencyType.MONEY))
-    register(Currency("FJD", "Fiji Dollar", 2, CurrencyType.MONEY))
-    register(Currency("FKP", "Falkland Islands Pound", 2, CurrencyType.MONEY))
-    register(Currency("GBP", "Pound Sterling", 2, CurrencyType.MONEY))
-    register(Currency("GEL", "Lari", 2, CurrencyType.MONEY))
-    register(Currency("GHS", "Ghana Cedi", 2, CurrencyType.MONEY))
-    register(Currency("GIP", "Gibraltar Pound", 2, CurrencyType.MONEY))
-    register(Currency("GMD", "Dalasi", 2, CurrencyType.MONEY))
-    register(Currency("GNF", "Guinea Franc", 0, CurrencyType.MONEY))
-    register(Currency("GTQ", "Quetzal", 2, CurrencyType.MONEY))
-    register(Currency("GYD", "Guyana Dollar", 2, CurrencyType.MONEY))
-    register(Currency("HKD", "Hong Kong Dollar", 2, CurrencyType.MONEY))
-    register(Currency("HNL", "Lempira", 2, CurrencyType.MONEY))
-    register(Currency("HRK", "Kuna", 2, CurrencyType.MONEY))
-    register(Currency("HTG", "Gourde", 2, CurrencyType.MONEY))
-    register(Currency("HUF", "Forint", 2, CurrencyType.MONEY))
-    register(Currency("IDR", "Rupiah", 2, CurrencyType.MONEY))
-    register(Currency("ILS", "New Israeli Sheqel", 2, CurrencyType.MONEY))
-    register(Currency("INR", "Indian Rupee", 2, CurrencyType.MONEY))
-    register(Currency("IOT", "IOTA", -1, CurrencyType.CRYPTO))
-    register(Currency("IQD", "Iraqi Dinar", 3, CurrencyType.MONEY))
-    register(Currency("IRR", "Iranian Rial", 2, CurrencyType.MONEY))
-    register(Currency("ISK", "Iceland Krona", 0, CurrencyType.MONEY))
-    register(Currency("JMD", "Jamaican Dollar", 2, CurrencyType.MONEY))
-    register(Currency("JOD", "Jordanian Dinar", 3, CurrencyType.MONEY))
-    register(Currency("JPY", "Yen", 0, CurrencyType.MONEY))
-    register(Currency("KES", "Kenyan Shilling", 2, CurrencyType.MONEY))
-    register(Currency("KGS", "Som", 2, CurrencyType.MONEY))
-    register(Currency("KHR", "Riel", 2, CurrencyType.MONEY))
-    register(Currency("KMF", "Comoro Franc", 0, CurrencyType.MONEY))
-    register(Currency("KPW", "North Korean Won", 2, CurrencyType.MONEY))
-    register(Currency("KRW", "Won", 0, CurrencyType.MONEY))
-    register(Currency("KWD", "Kuwaiti Dinar", 3, CurrencyType.MONEY))
-    register(Currency("KYD", "Cayman Islands Dollar", 2, CurrencyType.MONEY))
-    register(Currency("KZT", "Tenge", 2, CurrencyType.MONEY))
-    register(Currency("LAK", "Kip", 2, CurrencyType.MONEY))
-    register(Currency("LBP", "Lebanese Pound", 2, CurrencyType.MONEY))
-    register(Currency("LKR", "Sri Lanka Rupee", 2, CurrencyType.MONEY))
-    register(Currency("LRD", "Liberian Dollar", 2, CurrencyType.MONEY))
-    register(Currency("LSL", "Loti", 2, CurrencyType.MONEY))
-    register(Currency("LTC", "Litecoin", -1, CurrencyType.CRYPTO))
-    register(Currency("LYD", "Libyan Dinar", 3, CurrencyType.MONEY))
-    register(Currency("MAD", "Moroccan Dirham", 2, CurrencyType.MONEY))
-    register(Currency("MDL", "Moldovan Leu", 2, CurrencyType.MONEY))
-    register(Currency("MGA", "Malagasy Ariary", 2, CurrencyType.MONEY))
-    register(Currency("MKD", "Denar", 2, CurrencyType.MONEY))
-    register(Currency("MMK", "Kyat", 2, CurrencyType.MONEY))
-    register(Currency("MNT", "Tugrik", 2, CurrencyType.MONEY))
-    register(Currency("MOP", "Pataca", 2, CurrencyType.MONEY))
-    register(Currency("MRO", "Ouguiya", 2, CurrencyType.MONEY))
-    register(Currency("MUR", "Mauritius Rupee", 2, CurrencyType.MONEY))
-    register(Currency("MVR", "Rufiyaa", 2, CurrencyType.MONEY))
-    register(Currency("MWK", "Kwacha", 2, CurrencyType.MONEY))
-    register(Currency("MXN", "Mexican Peso", 2, CurrencyType.MONEY))
-    register(Currency("MXV", "Mexican Unidad de Inversion (UDI)", 2, CurrencyType.MONEY))
-    register(Currency("MYR", "Malaysian Ringgit", 2, CurrencyType.MONEY))
-    register(Currency("MZN", "Mozambique Metical", 2, CurrencyType.MONEY))
-    register(Currency("NAD", "Namibia Dollar", 2, CurrencyType.MONEY))
-    register(Currency("NEO", "NEO", -1, CurrencyType.CRYPTO))
-    register(Currency("NGN", "Naira", 2, CurrencyType.MONEY))
-    register(Currency("NIO", "Cordoba Oro", 2, CurrencyType.MONEY))
-    register(Currency("NOK", "Norwegian Krone", 2, CurrencyType.MONEY))
-    register(Currency("NPR", "Nepalese Rupee", 2, CurrencyType.MONEY))
-    register(Currency("NZD", "New Zealand Dollar", 2, CurrencyType.MONEY))
-    register(Currency("OMG", "OmiseGO", -1, CurrencyType.CRYPTO))
-    register(Currency("OMR", "Rial Omani", 3, CurrencyType.MONEY))
-    register(Currency("PAB", "Balboa", 2, CurrencyType.MONEY))
-    register(Currency("PEN", "Nuevo Sol", 2, CurrencyType.MONEY))
-    register(Currency("PGK", "Kina", 2, CurrencyType.MONEY))
-    register(Currency("PHP", "Philippine Peso", 2, CurrencyType.MONEY))
-    register(Currency("PKR", "Pakistan Rupee", 2, CurrencyType.MONEY))
-    register(Currency("PLN", "Zloty", 2, CurrencyType.MONEY))
-    register(Currency("PYG", "Guarani", 0, CurrencyType.MONEY))
-    register(Currency("QAR", "Qatari Rial", 2, CurrencyType.MONEY))
-    register(Currency("RON", "Romanian Leu", 2, CurrencyType.MONEY))
-    register(Currency("RSD", "Serbian Dinar", 2, CurrencyType.MONEY))
-    register(Currency("RUB", "Russian Ruble", 2, CurrencyType.MONEY))
-    register(Currency("RWF", "Rwanda Franc", 0, CurrencyType.MONEY))
-    register(Currency("SAR", "Saudi Riyal", 2, CurrencyType.MONEY))
-    register(Currency("SBD", "Solomon Islands Dollar", 2, CurrencyType.MONEY))
-    register(Currency("SCR", "Seychelles Rupee", 2, CurrencyType.MONEY))
-    register(Currency("SDG", "Sudanese Pound", 2, CurrencyType.MONEY))
-    register(Currency("SEK", "Swedish Krona", 2, CurrencyType.MONEY))
-    register(Currency("SGD", "Singapore Dollar", 2, CurrencyType.MONEY))
-    register(Currency("SHP", "Saint Helena Pound", 2, CurrencyType.MONEY))
-    register(Currency("SLL", "Leone", 2, CurrencyType.MONEY))
-    register(Currency("SOS", "Somali Shilling", 2, CurrencyType.MONEY))
-    register(Currency("SRD", "Surinam Dollar", 2, CurrencyType.MONEY))
-    register(Currency("SSP", "South Sudanese Pound", 2, CurrencyType.MONEY))
-    register(Currency("STD", "Dobra", 2, CurrencyType.MONEY))
-    register(Currency("SVC", "El Salvador Colon", 2, CurrencyType.MONEY))
-    register(Currency("SYP", "Syrian Pound", 2, CurrencyType.MONEY))
-    register(Currency("SZL", "Lilangeni", 2, CurrencyType.MONEY))
-    register(Currency("THB", "Baht", 2, CurrencyType.MONEY))
-    register(Currency("TJS", "Somoni", 2, CurrencyType.MONEY))
-    register(Currency("TMT", "Turkmenistan New Manat", 2, CurrencyType.MONEY))
-    register(Currency("TND", "Tunisian Dinar", 3, CurrencyType.MONEY))
-    register(Currency("TOP", "Pa'anga", 2, CurrencyType.MONEY))
-    register(Currency("TRY", "Turkish Lira", 2, CurrencyType.MONEY))
-    register(Currency("TTD", "Trinidad and Tobago Dollar", 2, CurrencyType.MONEY))
-    register(Currency("TWD", "New Taiwan Dollar", 2, CurrencyType.MONEY))
-    register(Currency("TZS", "Tanzanian Shilling", 2, CurrencyType.MONEY))
-    register(Currency("UAH", "Hryvnia", 2, CurrencyType.MONEY))
-    register(Currency("UGX", "Uganda Shilling", 0, CurrencyType.MONEY))
-    register(Currency("USD", "US Dollar", 2, CurrencyType.MONEY))
-    register(Currency("USN", "US Dollar (Next day)", 2, CurrencyType.MONEY))
-    register(Currency("UYI", "Uruguay Peso en Unidades Indexadas", 0, CurrencyType.MONEY))
-    register(Currency("UYU", "Peso Uruguayo", 2, CurrencyType.MONEY))
-    register(Currency("UZS", "Uzbekistan Sum", 2, CurrencyType.MONEY))
-    register(Currency("VEF", "Bolivar", 2, CurrencyType.MONEY))
-    register(Currency("VND", "Dong", 0, CurrencyType.MONEY))
-    register(Currency("VUV", "Vatu", 0, CurrencyType.MONEY))
-    register(Currency("WST", "Tala", 2, CurrencyType.MONEY))
-    register(Currency("XAG", "Silver", -1, CurrencyType.METAL))
-    register(Currency("XAU", "Gold", -1, CurrencyType.METAL))
-    register(Currency("XCD", "East Caribbean Dollar", 2, CurrencyType.MONEY))
-    register(Currency("XLM", "Stellar", -1, CurrencyType.CRYPTO))
-    register(Currency("XMR", "Monero", -1, CurrencyType.CRYPTO))
-    register(Currency("XPD", "Palladium", -1, CurrencyType.METAL))
-    register(Currency("XPT", "Platinum", -1, CurrencyType.METAL))
-    register(Currency("XRP", "Ripple", -1, CurrencyType.CRYPTO))
-    register(Currency("XSU", "Sucre", -1, CurrencyType.MONEY))
-    register(Currency("XUA", "ADB Unit of Account", -1, CurrencyType.MONEY))
-    register(Currency("YER", "Yemeni Rial", 2, CurrencyType.MONEY))
-    register(Currency("ZAR", "Rand", 2, CurrencyType.MONEY))
-    register(Currency("ZEC", "Zcash", -1, CurrencyType.CRYPTO))
-    register(Currency("ZMW", "Zambian Kwacha", 2, CurrencyType.MONEY))
-    register(Currency("ZWL", "Zimbabwe Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("AED", "UAE Dirham", 2, CurrencyType.MONEY))
+    register(Currency.of("AFN", "Afghani", 2, CurrencyType.MONEY))
+    register(Currency.of("ALL", "Lek", 2, CurrencyType.MONEY))
+    register(Currency.of("AMD", "Armenian Dram", 2, CurrencyType.MONEY))
+    register(Currency.of("ANG", "Netherlands Antillean Guilder", 2, CurrencyType.MONEY))
+    register(Currency.of("AOA", "Kwanza", 2, CurrencyType.MONEY))
+    register(Currency.of("ARS", "Argentine Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("AUD", "Australian Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("AWG", "Aruban Florin", 2, CurrencyType.MONEY))
+    register(Currency.of("AZN", "Azerbaijanian Manat", 2, CurrencyType.MONEY))
+    register(Currency.of("BAM", "Convertible Mark", 2, CurrencyType.MONEY))
+    register(Currency.of("BBD", "Barbados Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("BCH", "Bitcoin Cash", -1, CurrencyType.CRYPTO))
+    register(Currency.of("BDT", "Taka", 2, CurrencyType.MONEY))
+    register(Currency.of("BGN", "Bulgarian Lev", 2, CurrencyType.MONEY))
+    register(Currency.of("BHD", "Bahraini Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("BIF", "Burundi Franc", 0, CurrencyType.MONEY))
+    register(Currency.of("BMD", "Bermudian Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("BND", "Brunei Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("BOB", "Boliviano", 2, CurrencyType.MONEY))
+    register(Currency.of("BOV", "Mvdol", 2, CurrencyType.MONEY))
+    register(Currency.of("BRL", "Brazilian Real", 2, CurrencyType.MONEY))
+    register(Currency.of("BSD", "Bahamian Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("BTC", "Bitcoin", -1, CurrencyType.CRYPTO))
+    register(Currency.of("BTN", "Ngultrum", 2, CurrencyType.MONEY))
+    register(Currency.of("BWP", "Pula", 2, CurrencyType.MONEY))
+    register(Currency.of("BYR", "Belarussian Ruble", 0, CurrencyType.MONEY))
+    register(Currency.of("BZD", "Belize Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("CAD", "Canadian Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("CDF", "Congolese Franc", 2, CurrencyType.MONEY))
+    register(Currency.of("CHE", "WIR Euro", 2, CurrencyType.MONEY))
+    register(Currency.of("CHF", "Swiss Franc", 2, CurrencyType.MONEY))
+    register(Currency.of("CHW", "WIR Franc", 2, CurrencyType.MONEY))
+    register(Currency.of("CLF", "Unidad de Fomento", 4, CurrencyType.MONEY))
+    register(Currency.of("CLP", "Chilean Peso", 0, CurrencyType.MONEY))
+    register(Currency.of("CNH", "Yuan Renminbi (Off-shore)", 2, CurrencyType.MONEY))
+    register(Currency.of("CNY", "Yuan Renminbi", 2, CurrencyType.MONEY))
+    register(Currency.of("COP", "Colombian Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("COU", "Unidad de Valor Real", 2, CurrencyType.MONEY))
+    register(Currency.of("CRC", "Costa Rican Colon", 2, CurrencyType.MONEY))
+    register(Currency.of("CUC", "Peso Convertible", 2, CurrencyType.MONEY))
+    register(Currency.of("CUP", "Cuban Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("CVE", "Cabo Verde Escudo", 2, CurrencyType.MONEY))
+    register(Currency.of("CZK", "Czech Koruna", 2, CurrencyType.MONEY))
+    register(Currency.of("DASH", "Dash", -1, CurrencyType.CRYPTO))
+    register(Currency.of("DJF", "Djibouti Franc", 0, CurrencyType.MONEY))
+    register(Currency.of("DKK", "Danish Krone", 2, CurrencyType.MONEY))
+    register(Currency.of("DOP", "Dominican Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("DZD", "Algerian Dinar", 2, CurrencyType.MONEY))
+    register(Currency.of("EGP", "Egyptian Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("EOS", "EOSIO", -1, CurrencyType.CRYPTO))
+    register(Currency.of("ERN", "Nakfa", 2, CurrencyType.MONEY))
+    register(Currency.of("ETB", "Ethiopian Birr", 2, CurrencyType.MONEY))
+    register(Currency.of("ETC", "Ethereum Classic", -1, CurrencyType.CRYPTO))
+    register(Currency.of("ETH", "Ethereum", -1, CurrencyType.CRYPTO))
+    register(Currency.of("EUR", "Euro", 2, CurrencyType.MONEY))
+    register(Currency.of("FJD", "Fiji Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("FKP", "Falkland Islands Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("GBP", "Pound Sterling", 2, CurrencyType.MONEY))
+    register(Currency.of("GEL", "Lari", 2, CurrencyType.MONEY))
+    register(Currency.of("GHS", "Ghana Cedi", 2, CurrencyType.MONEY))
+    register(Currency.of("GIP", "Gibraltar Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("GMD", "Dalasi", 2, CurrencyType.MONEY))
+    register(Currency.of("GNF", "Guinea Franc", 0, CurrencyType.MONEY))
+    register(Currency.of("GTQ", "Quetzal", 2, CurrencyType.MONEY))
+    register(Currency.of("GYD", "Guyana Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("HKD", "Hong Kong Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("HNL", "Lempira", 2, CurrencyType.MONEY))
+    register(Currency.of("HRK", "Kuna", 2, CurrencyType.MONEY))
+    register(Currency.of("HTG", "Gourde", 2, CurrencyType.MONEY))
+    register(Currency.of("HUF", "Forint", 2, CurrencyType.MONEY))
+    register(Currency.of("IDR", "Rupiah", 2, CurrencyType.MONEY))
+    register(Currency.of("ILS", "New Israeli Sheqel", 2, CurrencyType.MONEY))
+    register(Currency.of("INR", "Indian Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("IOT", "IOTA", -1, CurrencyType.CRYPTO))
+    register(Currency.of("IQD", "Iraqi Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("IRR", "Iranian Rial", 2, CurrencyType.MONEY))
+    register(Currency.of("ISK", "Iceland Krona", 0, CurrencyType.MONEY))
+    register(Currency.of("JMD", "Jamaican Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("JOD", "Jordanian Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("JPY", "Yen", 0, CurrencyType.MONEY))
+    register(Currency.of("KES", "Kenyan Shilling", 2, CurrencyType.MONEY))
+    register(Currency.of("KGS", "Som", 2, CurrencyType.MONEY))
+    register(Currency.of("KHR", "Riel", 2, CurrencyType.MONEY))
+    register(Currency.of("KMF", "Comoro Franc", 0, CurrencyType.MONEY))
+    register(Currency.of("KPW", "North Korean Won", 2, CurrencyType.MONEY))
+    register(Currency.of("KRW", "Won", 0, CurrencyType.MONEY))
+    register(Currency.of("KWD", "Kuwaiti Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("KYD", "Cayman Islands Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("KZT", "Tenge", 2, CurrencyType.MONEY))
+    register(Currency.of("LAK", "Kip", 2, CurrencyType.MONEY))
+    register(Currency.of("LBP", "Lebanese Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("LKR", "Sri Lanka Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("LRD", "Liberian Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("LSL", "Loti", 2, CurrencyType.MONEY))
+    register(Currency.of("LTC", "Litecoin", -1, CurrencyType.CRYPTO))
+    register(Currency.of("LYD", "Libyan Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("MAD", "Moroccan Dirham", 2, CurrencyType.MONEY))
+    register(Currency.of("MDL", "Moldovan Leu", 2, CurrencyType.MONEY))
+    register(Currency.of("MGA", "Malagasy Ariary", 2, CurrencyType.MONEY))
+    register(Currency.of("MKD", "Denar", 2, CurrencyType.MONEY))
+    register(Currency.of("MMK", "Kyat", 2, CurrencyType.MONEY))
+    register(Currency.of("MNT", "Tugrik", 2, CurrencyType.MONEY))
+    register(Currency.of("MOP", "Pataca", 2, CurrencyType.MONEY))
+    register(Currency.of("MRO", "Ouguiya", 2, CurrencyType.MONEY))
+    register(Currency.of("MUR", "Mauritius Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("MVR", "Rufiyaa", 2, CurrencyType.MONEY))
+    register(Currency.of("MWK", "Kwacha", 2, CurrencyType.MONEY))
+    register(Currency.of("MXN", "Mexican Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("MXV", "Mexican Unidad de Inversion (UDI)", 2, CurrencyType.MONEY))
+    register(Currency.of("MYR", "Malaysian Ringgit", 2, CurrencyType.MONEY))
+    register(Currency.of("MZN", "Mozambique Metical", 2, CurrencyType.MONEY))
+    register(Currency.of("NAD", "Namibia Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("NEO", "NEO", -1, CurrencyType.CRYPTO))
+    register(Currency.of("NGN", "Naira", 2, CurrencyType.MONEY))
+    register(Currency.of("NIO", "Cordoba Oro", 2, CurrencyType.MONEY))
+    register(Currency.of("NOK", "Norwegian Krone", 2, CurrencyType.MONEY))
+    register(Currency.of("NPR", "Nepalese Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("NZD", "New Zealand Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("OMG", "OmiseGO", -1, CurrencyType.CRYPTO))
+    register(Currency.of("OMR", "Rial Omani", 3, CurrencyType.MONEY))
+    register(Currency.of("PAB", "Balboa", 2, CurrencyType.MONEY))
+    register(Currency.of("PEN", "Nuevo Sol", 2, CurrencyType.MONEY))
+    register(Currency.of("PGK", "Kina", 2, CurrencyType.MONEY))
+    register(Currency.of("PHP", "Philippine Peso", 2, CurrencyType.MONEY))
+    register(Currency.of("PKR", "Pakistan Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("PLN", "Zloty", 2, CurrencyType.MONEY))
+    register(Currency.of("PYG", "Guarani", 0, CurrencyType.MONEY))
+    register(Currency.of("QAR", "Qatari Rial", 2, CurrencyType.MONEY))
+    register(Currency.of("RON", "Romanian Leu", 2, CurrencyType.MONEY))
+    register(Currency.of("RSD", "Serbian Dinar", 2, CurrencyType.MONEY))
+    register(Currency.of("RUB", "Russian Ruble", 2, CurrencyType.MONEY))
+    register(Currency.of("RWF", "Rwanda Franc", 0, CurrencyType.MONEY))
+    register(Currency.of("SAR", "Saudi Riyal", 2, CurrencyType.MONEY))
+    register(Currency.of("SBD", "Solomon Islands Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("SCR", "Seychelles Rupee", 2, CurrencyType.MONEY))
+    register(Currency.of("SDG", "Sudanese Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("SEK", "Swedish Krona", 2, CurrencyType.MONEY))
+    register(Currency.of("SGD", "Singapore Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("SHP", "Saint Helena Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("SLL", "Leone", 2, CurrencyType.MONEY))
+    register(Currency.of("SOS", "Somali Shilling", 2, CurrencyType.MONEY))
+    register(Currency.of("SRD", "Surinam Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("SSP", "South Sudanese Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("STD", "Dobra", 2, CurrencyType.MONEY))
+    register(Currency.of("SVC", "El Salvador Colon", 2, CurrencyType.MONEY))
+    register(Currency.of("SYP", "Syrian Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("SZL", "Lilangeni", 2, CurrencyType.MONEY))
+    register(Currency.of("THB", "Baht", 2, CurrencyType.MONEY))
+    register(Currency.of("TJS", "Somoni", 2, CurrencyType.MONEY))
+    register(Currency.of("TMT", "Turkmenistan New Manat", 2, CurrencyType.MONEY))
+    register(Currency.of("TND", "Tunisian Dinar", 3, CurrencyType.MONEY))
+    register(Currency.of("TOP", "Pa'anga", 2, CurrencyType.MONEY))
+    register(Currency.of("TRY", "Turkish Lira", 2, CurrencyType.MONEY))
+    register(Currency.of("TTD", "Trinidad and Tobago Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("TWD", "New Taiwan Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("TZS", "Tanzanian Shilling", 2, CurrencyType.MONEY))
+    register(Currency.of("UAH", "Hryvnia", 2, CurrencyType.MONEY))
+    register(Currency.of("UGX", "Uganda Shilling", 0, CurrencyType.MONEY))
+    register(Currency.of("USD", "US Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("USN", "US Dollar (Next day)", 2, CurrencyType.MONEY))
+    register(Currency.of("UYI", "Uruguay Peso en Unidades Indexadas", 0, CurrencyType.MONEY))
+    register(Currency.of("UYU", "Peso Uruguayo", 2, CurrencyType.MONEY))
+    register(Currency.of("UZS", "Uzbekistan Sum", 2, CurrencyType.MONEY))
+    register(Currency.of("VEF", "Bolivar", 2, CurrencyType.MONEY))
+    register(Currency.of("VND", "Dong", 0, CurrencyType.MONEY))
+    register(Currency.of("VUV", "Vatu", 0, CurrencyType.MONEY))
+    register(Currency.of("WST", "Tala", 2, CurrencyType.MONEY))
+    register(Currency.of("XAG", "Silver", -1, CurrencyType.METAL))
+    register(Currency.of("XAU", "Gold", -1, CurrencyType.METAL))
+    register(Currency.of("XCD", "East Caribbean Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("XLM", "Stellar", -1, CurrencyType.CRYPTO))
+    register(Currency.of("XMR", "Monero", -1, CurrencyType.CRYPTO))
+    register(Currency.of("XPD", "Palladium", -1, CurrencyType.METAL))
+    register(Currency.of("XPT", "Platinum", -1, CurrencyType.METAL))
+    register(Currency.of("XRP", "Ripple", -1, CurrencyType.CRYPTO))
+    register(Currency.of("XSU", "Sucre", -1, CurrencyType.MONEY))
+    register(Currency.of("XUA", "ADB Unit of Account", -1, CurrencyType.MONEY))
+    register(Currency.of("YER", "Yemeni Rial", 2, CurrencyType.MONEY))
+    register(Currency.of("ZAR", "Rand", 2, CurrencyType.MONEY))
+    register(Currency.of("ZEC", "Zcash", -1, CurrencyType.CRYPTO))
+    register(Currency.of("ZMW", "Zambian Kwacha", 2, CurrencyType.MONEY))
+    register(Currency.of("ZWL", "Zimbabwe Dollar", 2, CurrencyType.MONEY))
```

### Comparing `pypara-0.0.8/README.rst` & `pypara-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pypara-0.0.8/pypara.egg-info/PKG-INFO` & `pypara-0.0.9/pypara.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypara
-Version: 0.0.8
+Version: 0.0.9
 Summary: Currencies, Monetary Value Objects, Arithmetic and Conversion
 Home-page: https://github.com/vst/pypara
 Author: Vehbi Sinan Tunalioglu
 Author-email: vst@vsthost.com
 License: BSD
 Description: Currencies, Monetary Value Objects, Arithmetic and Conversion
         =============================================================
@@ -43,8 +43,9 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: dev
```

### Comparing `pypara-0.0.8/LICENSE.txt` & `pypara-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypara-0.0.8/setup.py` & `pypara-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #: Defines the package root directory.
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 #: Defines the README file contents.
 with open(os.path.join(BASEDIR, "README.rst")) as cfile:
     README = cfile.read()
 
-#: Defines a list of required libraries.
+#: Defines a list of required libraries (proudly no dependencies).
 REQUIREMENTS = []
 
 #: Defines extra requirements for various other purposes.
 REQUIREMENTS_EXTRAS = {
     "dev": [
         "ipython",
         "mypy",
@@ -49,14 +49,15 @@
     long_description=README,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
     ],
     author="Vehbi Sinan Tunalioglu",
     author_email="vst@vsthost.com",
     url="https://github.com/vst/pypara",
     license="BSD",
     packages=find_packages(exclude=["pypara.tests"]),
     include_package_data=True,
```

### Comparing `pypara-0.0.8/PKG-INFO` & `pypara-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypara
-Version: 0.0.8
+Version: 0.0.9
 Summary: Currencies, Monetary Value Objects, Arithmetic and Conversion
 Home-page: https://github.com/vst/pypara
 Author: Vehbi Sinan Tunalioglu
 Author-email: vst@vsthost.com
 License: BSD
 Description: Currencies, Monetary Value Objects, Arithmetic and Conversion
         =============================================================
@@ -43,8 +43,9 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: dev
```

