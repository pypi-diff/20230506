# Comparing `tmp/motoo-1.1.89-py3-none-any.whl.zip` & `tmp/motoo-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14498 bytes, number of entries: 6
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-01 05:59 motoo/__init__.py
--rw-rw-r--  2.0 unx    82190 b- defN 23-May-06 02:36 motoo/wit_util.py
--rw-rw-r--  2.0 unx      683 b- defN 23-May-06 02:37 motoo-1.1.89.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-06 02:37 motoo-1.1.89.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-06 02:37 motoo-1.1.89.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      438 b- defN 23-May-06 02:37 motoo-1.1.89.dist-info/RECORD
-6 files, 83409 bytes uncompressed, 13704 bytes compressed:  83.6%
+Zip file size: 12105 bytes, number of entries: 6
+-rw-r--r--  2.0 unx        0 b- defN 21-Aug-19 03:52 motoo/__init__.py
+-rw-r--r--  2.0 unx    68303 b- defN 22-Aug-06 04:00 motoo/wit_util.py
+-rw-r--r--  2.0 unx      682 b- defN 22-Aug-06 04:01 motoo-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Aug-06 04:01 motoo-1.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 22-Aug-06 04:01 motoo-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      434 b- defN 22-Aug-06 04:01 motoo-1.1.9.dist-info/RECORD
+6 files, 69517 bytes uncompressed, 11319 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: motoo/__init__.py
 Comment: 
 
 Filename: motoo/wit_util.py
 Comment: 
 
-Filename: motoo-1.1.89.dist-info/METADATA
+Filename: motoo-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: motoo-1.1.89.dist-info/WHEEL
+Filename: motoo-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: motoo-1.1.89.dist-info/top_level.txt
+Filename: motoo-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: motoo-1.1.89.dist-info/RECORD
+Filename: motoo-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## motoo/wit_util.py

```diff
@@ -1,10 +1,11 @@
 import math, os
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
 from functools import reduce
 from scipy.stats import rankdata
 from scipy.stats.mstats import rankdata as mrankdata
 from tempfile import TemporaryFile
 import boto3
 import uuid
 import requests
@@ -17,71 +18,57 @@
 lib_max = max
 lib_min = min
 STOCK_ZERO_CODE = '000000'
 PRESENT_DATE = '00000000'
 
 def value_to_wit_data(value, d=datetime.today().strftime('%Y%m%d'), default_value=np.nan):
     wit_data = WitData(default_value)
-    wit_data.init_with_np(np.array([d]), np.array([STOCK_ZERO_CODE]), np.array([[value]]))
+    wit_data.init_with_np([d], [STOCK_ZERO_CODE], [[value]])
     return wit_data
 
 def value_to_present_wit_data(value, default_value=np.nan):
     return value_to_wit_data(value, d=PRESENT_DATE, default_value=default_value)
 
 def dict_to_wit_data(dict_data, default_value=np.nan):
     wit_data = WitData(default_value)
     wit_data.init_with_dict(dict_data)
     return wit_data
 
-def np_to_wit_data(dates, stock_codes, data, default_value=np.nan, strs=np.array([]), rstring_flag=False):
+def np_to_wit_data(dates, stock_codes, data, default_value=np.nan):
     wit_data = WitData(default_value)
-    dates = dates if isinstance(dates, np.ndarray) else np.array(dates)
-    stock_codes = stock_codes if isinstance(stock_codes, np.ndarray) else np.array(stock_codes)
-    data = data if isinstance(data, np.ndarray) else np.array(data)
-    strs = strs if isinstance(strs, np.ndarray) else np.array(strs)
-    wit_data.init_with_np(dates, stock_codes, data, strs=strs)
-    if rstring_flag:
-        WitData.make_strs(wit_data)
+    wit_data.init_with_np(np.array(dates), np.array(stock_codes), np.array(data))
     return wit_data
 
 def bytes_to_wit_data(text):
     wit_data = WitData()
     wit_data.init_with_bytes(text)
     return wit_data
 
 def file_to_wit_data(filename):
     text = b''
     with open(filename, "rb") as f:
         text = f.read()
     
     return bytes_to_wit_data(text)
 
-def db_rows_to_wit_data(rows, trade_date_column='tradeDate', stock_code_column='stockCode', value_column='itemValue', default_value=np.nan, dtype=float):
+def db_rows_to_wit_data(rows, trade_date_column='tradeDate', stock_code_column='stockCode', value_column='itemValue', default_value=np.nan):
     wit_data = None
     if len(rows) > 0:
         wit_data = WitData(default_value)
         wit_data.init_with_db_rows(rows, trade_date_column, stock_code_column, value_column)
-        if wit_data.get_data_type() != 'RSTRING':
-            wit_data = wit_data.astype(dtype)
     return wit_data
 
-def db_pivot_to_wit_data(rows, trade_date_column='tradeDate', delete_columns=[], default_value=np.nan, dtype=float):
+def db_pivot_to_wit_data(rows, trade_date_column='tradeDate', delete_columns=[], default_value=np.nan):
     wit_data = None
     if len(rows) > 0:
         wit_data = WitData(default_value)
         wit_data.init_with_db_pivot(rows, trade_date_column, delete_columns)
-        if wit_data.get_data_type() != 'RSTRING':
-            wit_data = wit_data.astype(dtype)
     return wit_data
 
 def dataframe_to_wit_data(df, default_value=np.nan):
-    wit_data = _dataframe_to_wit_data(df, default_value=default_value)
-    return wit_data
-
-def _dataframe_to_wit_data(df, default_value=np.nan):
     wit_data = WitData(default_value)
     wit_data.init_with_dataframe(df)
     return wit_data
 
 def reshape_wit_data_list(original_wit_data_list, default_value=np.nan):
     wit_data_list = []
     present_wit_indexes = []
@@ -90,116 +77,103 @@
             wit_data_list.append(data.copy())
         else:
             wit_data_list.append(data)
 
         if isinstance(data, WitData) and data.get_type() == WitDataType.PRESENT_TYPE:
             present_wit_indexes.append(index)
 
-    same_flag = True
-    for i in range(1, len(wit_data_list)):
-        prev_wit = wit_data_list[i-1]
-        next_wit = wit_data_list[i]
-        if isinstance(prev_wit, WitData) and isinstance(next_wit, WitData):
-            if len(prev_wit.dates) != len(next_wit.dates) or len(prev_wit.stock_codes) != len(next_wit.stock_codes) \
-                or np.any(prev_wit.dates != next_wit.dates) or np.any(prev_wit.stock_codes != next_wit.stock_codes):
-                same_flag = False
-        else:
-            same_flag = False
-        if not same_flag:
-            break
-
-    if same_flag:
-        return wit_data_list
-
     original_default_value = default_value
     if len(wit_data_list) < 2: return wit_data_list
     std_wit = get_std_wit(wit_data_list)
     std_type = get_std_type(wit_data_list)
     for i, a_wit in enumerate(wit_data_list):
         if isinstance(a_wit, WitData):
             aa_wit = a_wit.spread(std_type)
             wit_data_list[i].dates = aa_wit.dates
             wit_data_list[i].stock_codes = aa_wit.stock_codes
             wit_data_list[i].data = aa_wit.data
-            wit_data_list[i].strs = aa_wit.strs
-            WitData.relieve_strs(wit_data_list[i])
 
     all_dates = reduce(np.union1d, (wit.dates for wit in wit_data_list if isinstance(wit, WitData)))
     all_stock_codes = reduce(np.union1d, (wit.stock_codes for wit in wit_data_list if isinstance(wit, WitData)))
 
     if len(all_stock_codes) > 1 or all_stock_codes[0] != STOCK_ZERO_CODE:
         all_stock_codes = np.delete(all_stock_codes, np.where(all_stock_codes==STOCK_ZERO_CODE))
 
     for i, a_wit in enumerate(wit_data_list):
         if not isinstance(a_wit, WitData) or a_wit.data is None or len(a_wit.data) == 0:
-            if a_wit is None or (isinstance(a_wit, WitData) and (a_wit.data is None or len(a_wit.data) == 0)): a_wit = std_wit.default_value
-            wit_data_list[i] = np_to_wit_data(all_dates, all_stock_codes, np.full((len(all_dates), len(all_stock_codes)), a_wit), default_value=std_wit.default_value, rstring_flag=False)
+            if a_wit is None: a_wit = std_wit.default_value
+            wit_data_list[i] = np_to_wit_data(all_dates, all_stock_codes, np.repeat(np.array([a_wit]), len(all_dates) * len(all_stock_codes)).reshape(len(all_dates), len(all_stock_codes)), default_value=std_wit.default_value)
         else:
             a_wit._arrange()
 
     for i, a_wit in enumerate(wit_data_list):
-        if a_wit.get_data_type() == 'NUMBER':
+        dtype = a_wit.data.dtype
+        if np.issubdtype(dtype, np.number):
             a_wit.data = a_wit.data.astype(float)
             default_value = original_default_value
-        elif a_wit.get_data_type() == 'BOOL':
-            a_wit.data = a_wit.data.astype(bool)
+        elif np.issubdtype(dtype, np.bool_):
             if not isinstance(default_value, np.bool_): default_value = False
-        elif a_wit.get_data_type().endswith('STRING'):
-            a_wit.data = a_wit.data.astype(object)
+        elif np.issubdtype(dtype, object):
             default_value = a_wit.default_value if isinstance(a_wit.default_value, str) else ''
         else:
             default_value = original_default_value
 
+        
         a_wit_df = wit_data_list[i].to_dataframe()
-        addable_dates = np.array(list(set(all_dates) - set(wit_data_list[i].dates)))
-        if len(addable_dates) > 0:
-            if i in present_wit_indexes:
-                addable_wit_df = pd.concat([a_wit_df]*len(addable_dates), axis=0)
-                addable_wit_df.index = addable_dates
-            else:
-                addable_wit_df = pd.DataFrame(data=np.full([len(addable_dates), len(a_wit_df.columns)], default_value, dtype=a_wit.get_dtype()), index=addable_dates, columns=a_wit_df.columns)
-            a_wit_df = pd.concat([a_wit_df, addable_wit_df], axis=0)
+        addable_dates = np.setdiff1d(all_dates, wit_data_list[i].dates)
+        if i in present_wit_indexes:
+            addable_wit = np_to_wit_data(addable_dates, wit_data_list[i].stock_codes, np.full([len(addable_dates), len(wit_data_list[i].stock_codes)], wit_data_list[i].data[0], dtype=dtype))
+        else:
+            addable_wit = np_to_wit_data(addable_dates, wit_data_list[i].stock_codes, np.full([len(addable_dates), len(wit_data_list[i].stock_codes)], default_value, dtype=dtype))
+        addable_wit_df = addable_wit.to_dataframe()
+        a_wit_df = pd.concat([a_wit_df, addable_wit_df], axis=0)
+        wit_data_list[i] = dataframe_to_wit_data(a_wit_df)
 
         if wit_data_list[i].is_zero_code():
-            a_wit_df = pd.concat([a_wit_df]*len(all_stock_codes), axis=1)
-            a_wit_df.columns = all_stock_codes
+            wit_data_list[i].stock_codes = all_stock_codes
+            wit_data_list[i].data = np.repeat(wit_data_list[i].data, len(all_stock_codes)).reshape((len(wit_data_list[i].dates), len(all_stock_codes)))
         else:
-            addable_stocks = np.array(list(set(all_stock_codes) - set(wit_data_list[i].stock_codes)))
-            if len(addable_stocks) > 0:
-                addable_wit_df = pd.DataFrame(data=np.full([len(a_wit_df.index), len(addable_stocks)], default_value, dtype=a_wit.get_dtype()), index=a_wit_df.index, columns=addable_stocks)
-                a_wit_df = pd.concat([a_wit_df, addable_wit_df], axis=1)
-        a_wit_df = WitData._arrange_df(a_wit_df)
-        wit_data_list[i] = _dataframe_to_wit_data(a_wit_df)
+            a_wit_df = wit_data_list[i].to_dataframe()
+            addable_stocks = np.setdiff1d(all_stock_codes, wit_data_list[i].stock_codes)
+            addable_wit = np_to_wit_data(wit_data_list[i].dates, addable_stocks, np.full([len(wit_data_list[i].dates), len(addable_stocks)], default_value, dtype=dtype))
+            addable_wit_df = addable_wit.to_dataframe()
+            a_wit_df = pd.concat([a_wit_df, addable_wit_df], axis=1)
+            wit_data_list[i] = dataframe_to_wit_data(a_wit_df)
+            wit_data_list[i]._arrange()
+
+    # present wit 뻥튀기
+    # for index in present_wit_indexes:
+    #     non_nan_indexes = []
+    #     for column_index in range(len(wit_data_list[index].stock_codes)):
+    #         non_nan_indexes = np.where(np.logical_not(np.isnan(wit_data_list[index].data[:, column_index])))[0]
+    #         if len(non_nan_indexes) > 0: break
+
+    #     if len(non_nan_indexes) > 0:
+    #         non_nan_index = int(non_nan_indexes[0])
+    #     else:
+    #         continue
+
+    #     wit_data_list[index].dates = np.array(all_dates)
+    #     wit_data_list[index].data = np.full((len(all_dates), len(wit_data_list[index].stock_codes)), wit_data_list[index].data[non_nan_index])
 
     return wit_data_list
 
 def _init_wit_data_for_calculation(operands):
     wit_data_list = []
     for operand in operands:
         a_wit = operand.copy() if isinstance(operand, WitData) else operand
         wit_data_list.append(a_wit)
     wit_data_list = reshape_wit_data_list(wit_data_list)
 
-    for a_wit in wit_data_list:
-        WitData.relieve_strs(a_wit)
-
     return wit_data_list
 
 def get_std_type(wit_data_list):
     std_types = [None, None]
-
-    all_present = True
-    for a_wit in wit_data_list:
-        if isinstance(a_wit, WitData) and a_wit.get_type() != WitDataType.PRESENT_TYPE:
-            all_present = False
-            break
-    if all_present: return WitDataType.PRESENT_TYPE
-
     for a_wit in wit_data_list:
-        if isinstance(a_wit, WitData) and a_wit.get_type() != WitDataType.PRESENT_TYPE:
+        if isinstance(a_wit, WitData):
             for i in range(2):
                 std_index = -1
                 try:
                     std_index = WIT_DATA_TYPE_LINK[i].index(std_types[i])
                 except: pass
 
                 a_wit_index = -2
@@ -207,20 +181,16 @@
                     a_wit_index = WIT_DATA_TYPE_LINK[i].index(a_wit.get_type())
                 except: pass
                 std_types[i] = std_types[i] if std_index > a_wit_index else a_wit.get_type()
 
     if std_types[0] and std_types[1]:
         if std_types[0] == std_types[1]:
             return std_types[0]
-        elif std_types[0] in WIT_DATA_TYPE_LINK[0] and std_types[1] in WIT_DATA_TYPE_LINK[0]:
-            return WIT_DATA_TYPE_LINK[0][lib_max(WIT_DATA_TYPE_LINK[0].index(std_types[0]), WIT_DATA_TYPE_LINK[0].index(std_types[1]))]
-        elif std_types[0] in WIT_DATA_TYPE_LINK[1] and std_types[1] in WIT_DATA_TYPE_LINK[1]:
-            return WIT_DATA_TYPE_LINK[1][lib_max(WIT_DATA_TYPE_LINK[1].index(std_types[0]), WIT_DATA_TYPE_LINK[1].index(std_types[1]))]
-        elif std_types[0] in WIT_DATA_TYPE_LINK[0]: return std_types[0]
-        elif std_types[1] in WIT_DATA_TYPE_LINK[1]: return std_types[1]
+        elif WIT_DATA_TYPE_LINK[0].index(std_types[0]) == 0: return std_types[1]
+        elif WIT_DATA_TYPE_LINK[1].index(std_types[1]) == 0: return std_types[0]
         else: return WitDataType.DAY_TYPE
     elif not std_types[0]:
         return std_types[1]
     elif not std_types[1]:
         return std_types[0]
     else: return WitDataType.DAY_TYPE
 
@@ -237,15 +207,14 @@
     return std_wit
 
 def vectorize(func, operand):
     v_func = np.vectorize(func)
     return v_func(operand)
 
 def single_calculation(func, operand):
-    WitData.relieve_strs(operand)
     return np_to_wit_data(operand.dates, operand.stock_codes, func(operand.data), operand.default_value)
 
 def sequantial_calculation(func, operands):
     if len(operands) < 2: return operands[0]
 
     new_operands = [operand.copy() if isinstance(operand, WitData) else operand for operand in operands]
 
@@ -327,76 +296,63 @@
 def ors(operands):
     return sequantial_compare_calculation(lambda data1, data2 : (data1.astype(bool) | data2.astype(bool)), operands)
 
 def nots(operand):
     return single_calculation(np.logical_not, operand) if isinstance(operand, WitData) else not operand
 
 def greater_than_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 > data2, 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 > data2, 1.0, 0.0)), operands)
 
 def greater_than_or_equal_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 >= data2, 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 >= data2, 1.0, 0.0)), operands)
 
 def less_than_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 < data2, 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 < data2, 1.0, 0.0)), operands)
 
 def less_than_or_equal_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 <= data2, 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 <= data2, 1.0, 0.0)), operands)
 
 def equals_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 == data2, 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 == data2, 1.0, 0.0)), operands)
 
 def not_equals_float(operand1, operand2):
-    return two_elements_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1 != data2, 1.0, 0.0)), operand1, operand2)
+    return two_elements_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1 != data2, 1.0, 0.0)), operand1, operand2)
 
 def ands_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1.astype(bool) & data2.astype(bool), 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1.astype(bool) & data2.astype(bool), 1.0, 0.0)), operands)
 
 def ors_float(operands):
-    return sequantial_compare_calculation(lambda data1, data2 : np.where(pd.isna(data1) | pd.isna(data2), np.nan, np.where(data1.astype(bool) | data2.astype(bool), 1.0, 0.0)), operands)
+    return sequantial_compare_calculation(lambda data1, data2 : np.where(np.isnan(data1) | np.isnan(data2), np.nan, np.where(data1.astype(bool) | data2.astype(bool), 1.0, 0.0)), operands)
 
 def nots_float(operand):
     if isinstance(operand, WitData):
         return operand.isnan().where(np.nan, operand.where(0.0, 1.0))
     else:
         return not operand
 
 def top_rank(operands):
     rank_wit_data = rank(operands[1:], method='ordinal')
     data = rank_wit_data.data <= int(operands[0])
     return np_to_wit_data(rank_wit_data.dates, rank_wit_data.stock_codes, data)
 
 def top_percent(operands):
     rank_wit_data = rank(operands[1:], method='ordinal')
-    data = rank_wit_data.data <= np.count_nonzero(np.logical_not(pd.isna(rank_wit_data.data)), axis=1)[:,np.newaxis] * (float(operands[0]) / 100)
+    data = rank_wit_data.data <= np.count_nonzero(np.logical_not(np.isnan(rank_wit_data.data)), axis=1)[:,np.newaxis] * (float(operands[0]) / 100)
     return np_to_wit_data(rank_wit_data.dates, rank_wit_data.stock_codes, data)
 
 def rank(operands, method='min'):
-    new_operands = []
-    stock_codes = []
-    for operand in operands:
-        if isinstance(operand, WitData):
-            new_operand = operand.copy()
-            new_operands.append(new_operand)
-            stock_codes = np.intersect1d(stock_codes, new_operand.stock_codes) if len(stock_codes) > 0 else new_operand.stock_codes
-        else:
-            new_operands.append(operand)
-
-    for i, operand in enumerate(new_operands):
-        if isinstance(operand, WitData):
-            new_operands[i] = operand.get_stocks_data(stock_codes)
-
+    new_operands = [operand.copy() if isinstance(operand, WitData) else operand for operand in operands]
     inited_operands = _init_wit_data_for_calculation([new_operands[1], new_operands[2]])
     scope = inited_operands[0]
     target = inited_operands[1]
 
     masked_operand = np.ma.masked_invalid(target.data)
     masked_operand.mask = masked_operand.mask | np.logical_not(scope.data)
     for i, line in enumerate(masked_operand.mask):
-        if len(WitData.unique(line)) == 1 and line[0] == True:
+        if len(np.unique(line)) == 1 and line[0] == True:
             masked_operand.data[i] = np.zeros(len(masked_operand.data[i]))
             masked_operand.mask[i] = np.zeros(len(masked_operand.mask[i]), dtype=bool)
     result = mrankdata(masked_operand, axis=1)
     if operands[0]: #상위
         result = 0 - result
     else: #하위
         result[np.where(result==0.0)] = len(scope.stock_codes)
@@ -433,93 +389,38 @@
     elif week_regex.match(date_str): return WitDataType.WEEK_TYPE
     elif month_regex.match(date_str): return WitDataType.MONTH_TYPE
     elif quarter_regex.match(date_str): return WitDataType.QUARTER_TYPE
     elif year_regex.match(date_str): return WitDataType.YEAR_TYPE
     else: return None
 
 def get_date_format_with_day_format(date_str, target_type):
-    if target_type == WitDataType.PRESENT_TYPE:
-        if date_str == '00000000':
-            return datetime.today().strftime('%Y%m%d')
-        else:
-            return date_str
-    elif target_type == WitDataType.DAY_TYPE:
+    if target_type == WitDataType.DAY_TYPE:
         return date_str
     elif target_type == WitDataType.WEEK_TYPE:
-        d = datetime.strptime(date_str, '%Y%m%d')
-        monday = d + timedelta(days=-d.weekday(), weeks=0)
-        year_str = str(monday.year)
-        monday_str = monday.strftime('%Y%m%d')
-        weeks = np.where(np.array(pd.date_range(start=year_str+'0101', end=year_str+'1231', freq='W-MON').strftime("%Y%m%d"))==monday_str)[0][0] + 1
-        return year_str + str(weeks).zfill(2) + 'W'
+        iso_date = (datetime.strptime(date_str, '%Y%m%d')).isocalendar()
+        return str(iso_date[0]) + str(iso_date[1]).zfill(2) + 'W'
     elif target_type == WitDataType.MONTH_TYPE:
         return date_str[:6]
     elif target_type == WitDataType.QUARTER_TYPE:
         return date_str[:4] + str((int(date_str[4:6])+2)//3) + 'Q'
     elif target_type == WitDataType.YEAR_TYPE:
         return date_str[:4]
 
 def get_start_end_date(date_str, target_type):
-    if target_type == WitDataType.PRESENT_TYPE:
-        return (datetime.today().strftime('%Y%m%d'), datetime.today().strftime('%Y%m%d'))
-    elif target_type == WitDataType.DAY_TYPE:
+    if target_type == WitDataType.DAY_TYPE:
         return (date_str, date_str)
     elif target_type == WitDataType.WEEK_TYPE:
         return (datetime.strptime(date_str[:6]+'1', '%Y%W%w').strftime('%Y%m%d'), datetime.strptime(date_str[:6]+'0', '%Y%W%w').strftime('%Y%m%d'))
     elif target_type == WitDataType.MONTH_TYPE:
         return (pd.Period(year=int(date_str[:4]), month=int(date_str[4:6]), freq='D').strftime('%Y%m%d'), pd.Period(year=int(date_str[:4]), month=int(date_str[4:6]), freq='M').strftime('%Y%m%d'))
     elif target_type == WitDataType.QUARTER_TYPE:
         return (pd.Period(year=int(date_str[:4]), quarter=int(date_str[4:5]), freq='D').strftime('%Y%m%d'), pd.Period(year=int(date_str[:4]), quarter=int(date_str[4:5]), freq='Q').strftime('%Y%m%d'))
     elif target_type == WitDataType.YEAR_TYPE:
         return (date_str+'0101', date_str+'1231')
 
-def vertical_merge(wit_list, default_value=np.nan):
-    std_type = wit_list[0].get_type()
-    original_dtypes = np.array([w.data.dtype for w in wit_list])
-    all_same_type = np.all(original_dtypes == original_dtypes[0])
-    dates = []
-    for i, wit_data in enumerate(wit_list):
-        diff_dates = np.array(list(set(wit_data.dates) - set(dates)))
-        if not isinstance(wit_data, WitData):
-            if isinstance(wit_data, float) or isinstance(wit_data, bool):
-                wit_list[i] = value_to_wit_data(wit_data).to_dataframe().loc[diff_dates].astype(original_dtypes[i])
-            else:
-                raise Exception('Value is not proper type.')
-        else:
-            wit_list[i] = wit_data.spread(std_type).to_dataframe().loc[diff_dates]
-        
-        dates.extend(diff_dates.tolist())
-
-    return_value = dataframe_to_wit_data(pd.concat(wit_list, axis=0).fillna(default_value)).astype(original_dtypes[0] if all_same_type else object)
-    return_value._arrange()
-
-    return return_value
-
-def horizontal_merge(wit_list, default_value=np.nan):
-    std_type = wit_list[0].get_type()
-    original_dtypes = np.array([w.data.dtype for w in wit_list])
-    all_same_type = np.all(original_dtypes == original_dtypes[0])
-    stock_codes = []
-    for i, wit_data in enumerate(wit_list):
-        diff_stock_codes = np.array(list(set(wit_data.stock_codes) - set(stock_codes)))
-        if not isinstance(wit_data, WitData):
-            if isinstance(wit_data, float) or isinstance(wit_data, bool):
-                wit_list[i] = value_to_wit_data(wit_data).to_dataframe().loc[:, diff_stock_codes].astype(original_dtypes[i])
-            else:
-                raise Exception('Value is not proper type.')
-        else:
-            wit_list[i] = wit_data.spread(std_type).to_dataframe().loc[:, diff_stock_codes]
-        
-        stock_codes.extend(diff_stock_codes.tolist())
-
-    return_value = dataframe_to_wit_data(pd.concat(wit_list, axis=1).fillna(default_value)).astype(original_dtypes[0] if all_same_type else object)
-    return_value._arrange()
-
-    return return_value
-
 class TimeChecker:
     def __init__(self):
         self.acc_time = 0.0
         self.times = dict()
         self.count = 0
     def go(self):
         uid = uuid.uuid1()
@@ -533,15 +434,15 @@
         print(self.times)
         for uid in list(self.times.keys()):
             self.stop(uid)
         print(self.acc_time, self.count, (self.acc_time / self.count) if self.count > 0 else 0)
 
 class WitUtilIndexer(pd.api.indexers.BaseIndexer):
     def __init__(self, df, days, window_size, nan_day_nan=True):
-        self.non_nan_np = ~pd.isna(df.values)
+        self.non_nan_np = ~np.isnan(df.values)
         self.end_days = days
         self.window_size = window_size
         self.start_days = days - window_size + 1
         self.column_index = 0
         self.non_nan_list = []
         self.start_end_list = []
         self.nan_day_nan = nan_day_nan
@@ -662,34 +563,31 @@
     DAY_TYPE = 1
     WEEK_TYPE = 2
     MONTH_TYPE = 3
     QUARTER_TYPE = 4
     YEAR_TYPE = 5
     PRESENT_TYPE = 6
 
-WIT_DATA_TYPE_LINK = [[WitDataType.PRESENT_TYPE, WitDataType.YEAR_TYPE, WitDataType.QUARTER_TYPE, WitDataType.MONTH_TYPE, WitDataType.DAY_TYPE], [WitDataType.PRESENT_TYPE, WitDataType.YEAR_TYPE, WitDataType.WEEK_TYPE, WitDataType.DAY_TYPE]]
+WIT_DATA_TYPE_LINK = [[WitDataType.YEAR_TYPE, WitDataType.QUARTER_TYPE, WitDataType.MONTH_TYPE, WitDataType.DAY_TYPE], [WitDataType.YEAR_TYPE, WitDataType.WEEK_TYPE, WitDataType.DAY_TYPE]]
 
 class WitData:
-    split_size = 8
     def __init__(self, default_value=np.nan):
+        self.split_size = 8
         self.default_value = default_value
-        self.strs = np.array([])
 
     def __str__(self):
         return str(self.to_dataframe())
         #return f"""dates :\n{self.dates}\n\nstock_codes :\n{self.stock_codes}\n\ndata :\n{self.data}"""
 
     def __repr__(self):
         return str(self.to_dataframe())
 
     def get_type(self):
         if len(self.dates) == 0 or not isinstance(self.dates[0], str):
             return 0
-        elif len(self.dates) == 1 and self.dates[0] in [*map(get_date_format_with_day_format, [datetime.today().strftime('%Y%m%d')]*len(WitDataType), list(WitDataType)), '00000000']:
-            return WitDataType.PRESENT_TYPE
         return get_type_with_date_str(self.dates[0])
 
     def __get_spreading_types(self, data_type):
         return_list = []
         for type_arr in WIT_DATA_TYPE_LINK:
             a_list = []
             return_list.append(a_list)
@@ -714,36 +612,31 @@
             if len(self_types[i]) > len(target_types[i]): return_type = target_types[i][0]
             else: return_type = self_types[i][0]
         
         return return_type
 
     def _arrange(self):
         origin_self = self.copy()
-        origin_dtype = self.get_dtype()
+        origin_dtype = self.data.dtype
         new_df = origin_self.to_dataframe()
-        new_df = WitData._arrange_df(new_df)
-        new_self = _dataframe_to_wit_data(new_df)
-        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data, new_self.strs)
-        if self.get_data_type() != 'RSTRING':
-            self.data = self.data.astype(origin_dtype)
-
-    def _arrange_df(df):
-        df = df.reindex(sorted(df.columns), axis=1)
-        df.sort_index(inplace=True)
-        return df
+        new_df = new_df.reindex(sorted(new_df.columns), axis=1)
+        new_df = new_df.sort_index()
+        new_self = dataframe_to_wit_data(new_df)
+        self.dates = new_self.dates
+        self.stock_codes = new_self.stock_codes
+        self.data = new_self.data.astype(origin_dtype)
 
     def base_calc(self, type_node, begin_days, end_days=0, nan_day_nan=True):
         window_size = end_days - begin_days + 1
 
         self_type = self.get_type()
         if self_type == WitDataType.DAY_TYPE:
-            WitData.relieve_strs(self)
 
             # self.data에 속해있는 np.nan을 vertically 아래쪽으로 몰기
-            nan_shifted = np.apply_along_axis((lambda x: np.concatenate((x[~pd.isna(x)], np.full(np.count_nonzero(pd.isna(x)), np.nan)))), axis=0, arr=self.data)
+            nan_shifted = np.apply_along_axis((lambda x: np.concatenate((x[~np.isnan(x)], np.full(np.count_nonzero(np.isnan(x)), np.nan)))), axis=0, arr=self.data)
 
             # 몰려있는 상태로 rolling 및 계산
             if type_node.endswith('POINT'):
                 df = pd.DataFrame(nan_shifted).shift(-begin_days)
             elif type_node.endswith('MOMENTUM'):
                 first = pd.DataFrame(nan_shifted).shift(-begin_days)
                 last = pd.DataFrame(nan_shifted).shift(-end_days)
@@ -766,24 +659,24 @@
             data = df.values
 
             # rolling 계산값에 column index 붙이기
             indexed = np.concatenate((np.arange(len(data[0])).reshape(1, -1), data))
             
             # 컬럼별로 self.data에 속한 np.nan 기준으로 계산된 indexed_data 사이사이에 넣기
             def insert_nan(x):
-                indexes = np.where(pd.isna(self.data[:,int(x[0])]))[0]
+                indexes = np.where(np.isnan(self.data[:,int(x[0])]))[0]
                 indexes = indexes - np.arange(len(indexes))
                 return np.insert(x[1:], indexes, np.nan)[:len(x)-1]
 
             nan_inserted = np.apply_along_axis(insert_nan, axis=0, arr=indexed)
 
             if not nan_day_nan:
                 nan_inserted = pd.DataFrame(nan_inserted).ffill(axis=0).values
 
-            return np_to_wit_data(self.dates, self.stock_codes, np.round_(nan_inserted, 10) if self.get_data_type() == 'NUMBER' else nan_inserted)
+            return np_to_wit_data(self.dates, self.stock_codes, np.round_(nan_inserted, 10))
             # df = self.to_dataframe()
             # window_size = end_days - begin_days + 1
             # if type_node.endswith('POINT'):
             #     df = df.rolling(SpotIndexer(df=df, days=begin_days, nan_day_nan=nan_day_nan), min_periods=1).sum()
             # elif type_node.endswith('MOMENTUM'):
             #     first = df.rolling(SpotIndexer(df=df, days=begin_days, nan_day_nan=nan_day_nan), min_periods=1).sum()
             #     last = df.rolling(SpotIndexer(df=df, days=end_days, nan_day_nan=nan_day_nan), min_periods=1).sum()
@@ -819,88 +712,110 @@
             elif type_node.endswith('CHANGE'):
                 df = df.shift(-end_days).rolling(window_size).std(ddof=0)
             elif type_node.endswith('MAX'):
                 df = df.shift(-end_days).rolling(window_size).max()
             elif type_node.endswith('MIN'):
                 df = df.shift(-end_days).rolling(window_size).min()
 
-            return dataframe_to_wit_data(df.ffill() if not nan_day_nan else df)
+            return dataframe_to_wit_data(df.ffill())
 
     def shift(self, days, nan_day_nan=True):
-        return self.base_calc('POINT', -days, nan_day_nan=nan_day_nan)
+        return self.base_calc('POINT', -days, nan_day_nan)
 
     def isnan(self):
-        return np_to_wit_data(self.dates, self.stock_codes, pd.isna(self.data))
+        return np_to_wit_data(self.dates, self.stock_codes, np.isnan(self.data))
 
     def where(self, true_data, false_data):
         wit_data_list = reshape_wit_data_list([self, true_data, false_data])
         new_self, new_true_data, new_false_data = wit_data_list[0], wit_data_list[1], wit_data_list[2]
-        WitData.relieve_strs(new_true_data)
-        WitData.relieve_strs(new_false_data)
         return np_to_wit_data(new_true_data.dates, new_true_data.stock_codes, np.where(new_self.data, new_true_data.data, new_false_data.data))
 
     def spread(self, target_type):
-        self._arrange()
         self_type = self.get_type()
-        target_type = self_type if target_type == WitDataType.PRESENT_TYPE else self._get_spreading_type(target_type) if self_type == WitDataType.PRESENT_TYPE else target_type
+        target_type = self._get_spreading_type(target_type) if self_type == WitDataType.PRESENT_TYPE else target_type
         if self_type == target_type: return self.copy()
 
-        new_stock_codes = np.array(self.stock_codes.copy(), dtype=self.stock_codes.dtype)
-
-        start_date, end_date0 = get_start_end_date(lib_min(self.dates), self_type)
-        start_date0, end_date = get_start_end_date(lib_max(self.dates), self_type)
-
-        if target_type == WitDataType.YEAR_TYPE:
-            freq='YS'
-            string_func = lambda d, i: d[:4]
-        elif target_type == WitDataType.QUARTER_TYPE:
-            freq='QS'
-            string_func = lambda d, i: d[:4] + f'{i}Q'
-        elif target_type == WitDataType.MONTH_TYPE:
-            freq='MS'
-            string_func = lambda d, i: d[:6]
-        elif target_type == WitDataType.WEEK_TYPE:
-            freq='W-MON'
-            string_func = lambda d, i: d[:4] + str(i).zfill(2) + 'W'
-        elif target_type == WitDataType.DAY_TYPE:
-            freq='D'
-            string_func = lambda d, i: d
-
-        new_dates = np.array(pd.date_range(start=start_date, end=end_date, freq=freq).strftime("%Y%m%d"))
-        if len(new_dates) == 0: new_dates = np.array([get_date_format_with_day_format(end_date, target_type)])
-        years = np.vectorize(get_date_format_with_day_format)(new_dates, WitDataType.YEAR_TYPE)
-        first_year_element_index = np.where(np.array(pd.date_range(start=new_dates[0][:4]+'0101', end=new_dates[0][:4]+'1231', freq=freq).strftime("%Y%m%d"))==get_start_end_date(new_dates[0], target_type)[0])[0][0] + 1
-        years_indices = years.copy()
-        for i, y in enumerate(years):
-            years_indices[np.where(years_indices==y)] = np.arange(np.count_nonzero(np.where(years_indices==y, True, False))) + (first_year_element_index if i==0 else 1)
-        years_indices = years_indices.astype(int)
-
-        spreaded_self_dates = np.vectorize(get_date_format_with_day_format)(new_dates, self_type)
-
-        new_dates = np.vectorize(string_func)(new_dates, years_indices)
-        def get_index(d):
-            indexes = np.where(self.dates==d)[0]
-            if len(indexes) > 0:
-                return indexes[0]
+        new_dates = np.array([], dtype=str)
+        new_data = np.array([], dtype=self.data.dtype)
+        new_stock_codes = np.array(self.stock_codes.copy(), dtype=str)
+
+        if self_type == WitDataType.YEAR_TYPE:
+            for index, a_date in enumerate(self.dates):
+                start_date, end_date = get_start_end_date(a_date, self_type)
+                if target_type == WitDataType.QUARTER_TYPE:
+                    for num, yyyymmdd in enumerate(pd.date_range(start=start_date, end=end_date, freq='BQ').strftime("%Y%m%d").tolist()):
+                        new_dates = np.append(new_dates, a_date + f'{num+1}Q')
+                        new_data = np.append(new_data, self.data[index])
+
+                elif target_type == WitDataType.MONTH_TYPE:
+                    for num, yyyymmdd in enumerate(pd.date_range(start=start_date, end=end_date, freq='MS').strftime("%Y%m%d").tolist()):
+                        new_dates = np.append(new_dates, yyyymmdd[:6])
+                        new_data = np.append(new_data, self.data[index])
+
+                elif target_type == WitDataType.WEEK_TYPE:
+                    for num, yyyymmdd in enumerate(pd.date_range(start=start_date, end=end_date, freq='W-MON').strftime("%Y%m%d").tolist()):
+                        new_dates = np.append(new_dates, a_date + str(num+1).zfill(2) + 'W')
+                        new_data = np.append(new_data, self.data[index])
+
+                elif target_type == WitDataType.DAY_TYPE:
+                    for yyyymmdd in pd.date_range(start=start_date, end=end_date).strftime("%Y%m%d").tolist():
+                        new_dates = np.append(new_dates, yyyymmdd)
+                        new_data = np.append(new_data, self.data[index])
+
+        elif self_type == WitDataType.QUARTER_TYPE:
+            for index, a_date in enumerate(self.dates):
+                start_date, end_date = get_start_end_date(a_date, self_type)
+                if target_type == WitDataType.MONTH_TYPE:
+                    for num, yyyymmdd in enumerate(pd.date_range(start=start_date, end=end_date, freq='MS').strftime("%Y%m%d").tolist()):
+                        new_dates = np.append(new_dates, yyyymmdd[:6])
+                        new_data = np.append(new_data, self.data[index])
+
+                elif target_type == WitDataType.DAY_TYPE:
+                    for yyyymmdd in pd.date_range(start=start_date, end=end_date).strftime("%Y%m%d").tolist():
+                        new_dates = np.append(new_dates, yyyymmdd)
+                        new_data = np.append(new_data, self.data[index])
+
+        elif self_type == WitDataType.MONTH_TYPE:
+            for index, a_date in enumerate(self.dates):
+                start_date, end_date = get_start_end_date(a_date, self_type)
+                if target_type == WitDataType.DAY_TYPE:
+                    for yyyymmdd in pd.date_range(start=start_date, end=end_date).strftime("%Y%m%d").tolist():
+                        new_dates = np.append(new_dates, yyyymmdd)
+                        new_data = np.append(new_data, self.data[index])
+
+        elif self_type == WitDataType.WEEK_TYPE:
+            for index, a_date in enumerate(self.dates):
+                start_date, end_date = get_start_end_date(a_date, self_type)
+                if target_type == WitDataType.DAY_TYPE:
+                    for yyyymmdd in pd.date_range(start=start_date, end=end_date).strftime("%Y%m%d").tolist():
+                        new_dates = np.append(new_dates, yyyymmdd)
+                        new_data = np.append(new_data, self.data[index])
+
+        elif self_type == WitDataType.PRESENT_TYPE:
+            today = datetime.today().strftime('%Y%m%d')
+            if target_type == WitDataType.DAY_TYPE:
+                d = today
             else:
-                return -1
-        new_dates_indexes = np.vectorize(get_index)(spreaded_self_dates)
-        new_data = self.data[new_dates_indexes]
+                d = get_date_format_with_day_format(today, target_type)
+                
+            new_dates = np.append(new_dates, d)
+            new_data = np.append(new_data, self.data[0])
 
-        return np_to_wit_data(new_dates, new_stock_codes, new_data, strs=self.strs)
+        new_data = new_data.reshape((len(new_dates), len(new_stock_codes)))
+        return np_to_wit_data(new_dates, new_stock_codes, new_data)
 
     def init_with_dict(self, dict_data):
         self.dates = np.sort(np.array(list(dict_data.keys())))
         self.stock_codes = np.array(['X'])
         for one_date in self.dates:
             if one_date != 'returnType':
                 self.stock_codes = np.union1d(np.array(self.stock_codes, dtype=str), np.array(list(dict_data[one_date].keys()), dtype=str))
         self.stock_codes = np.delete(self.stock_codes, np.where(self.stock_codes == 'X'))
 
-        self.data = np.empty((len(self.dates), len(self.stock_codes)), dtype=type(self.default_value))
+        self.data = np.empty((len(self.dates), len(self.stock_codes)))
         self.data[:, :] = self.default_value
 
         if isinstance(list(list(dict_data.values())[0].values())[0], dict):
             for i, one_date in enumerate(self.dates):
                 for j, stock_code in enumerate(self.stock_codes):
                     try:
                         self.data[i, j] = list(dict_data[one_date][stock_code].values())[0]
@@ -910,51 +825,33 @@
             for i, one_date in enumerate(self.dates):
                 for j, stock_code in enumerate(self.stock_codes):
                     try:
                         self.data[i, j] = dict_data[one_date][stock_code]
                     except:
                         self.data[i, j] = self.default_value
 
-    def init_with_np(self, dates, stock_codes, data, strs=np.array([])):
-        self.dates = dates if isinstance(dates, np.ndarray) else np.array(dates)
-        self.stock_codes = stock_codes if isinstance(stock_codes, np.ndarray) else np.array(stock_codes, dtype=stock_codes.dtype)
-        self.data = data if isinstance(data, np.ndarray) else np.array(data)
-        self.strs = strs if isinstance(strs, np.ndarray) else np.array(strs)
+    def init_with_np(self, dates, stock_codes, data):
+        self.dates = np.array(dates)
+        self.stock_codes = np.array(stock_codes, dtype=str)
+        self.data = np.array(data)
 
     def init_with_bytes(self, b):
-        try:
-            default_value_size = int.from_bytes(b[:WitData.split_size], byteorder='big')
-            dates_size = int.from_bytes(b[WitData.split_size:WitData.split_size*2], byteorder='big')
-            stocks_codes_size = int.from_bytes(b[WitData.split_size*2:WitData.split_size*3], byteorder='big')
-            start_index = WitData.split_size * 3
-            default_value_end_index = start_index + default_value_size
-            dates_end_index = default_value_end_index + dates_size
-            stock_codes_end_index = dates_end_index + stocks_codes_size
-            bs = [b[start_index : default_value_end_index], b[default_value_end_index : dates_end_index], b[dates_end_index : stock_codes_end_index], b[stock_codes_end_index:]]
-            nps = []
-            for a_b in bs:
-                nps.append(np_from_byte(a_b))
-            self.default_value = nps[0].item()
-            self.init_with_np(nps[1], np.array(nps[2], dtype=str if isinstance(nps[2][0], str) else object), nps[3])
-        except:
-            default_value_size = int.from_bytes(b[:WitData.split_size], byteorder='big')
-            dates_size = int.from_bytes(b[WitData.split_size:WitData.split_size*2], byteorder='big')
-            stocks_codes_size = int.from_bytes(b[WitData.split_size*2:WitData.split_size*3], byteorder='big')
-            strs_size = int.from_bytes(b[WitData.split_size*3:WitData.split_size*4], byteorder='big')
-            start_index = WitData.split_size * 4
-            default_value_end_index = start_index + default_value_size
-            dates_end_index = default_value_end_index + dates_size
-            stock_codes_end_index = dates_end_index + stocks_codes_size
-            strs_end_index = stock_codes_end_index + strs_size
-            bs = [b[start_index : default_value_end_index], b[default_value_end_index : dates_end_index], b[dates_end_index : stock_codes_end_index], b[stock_codes_end_index : strs_end_index], b[strs_end_index:]]
-            nps = []
-            for a_b in bs:
-                nps.append(np_from_byte(a_b))
-            self.default_value = nps[0].item()
-            self.init_with_np(nps[1], np.array(nps[2], dtype=str if isinstance(nps[2][0], str) else object), nps[4], strs=nps[3])
+        default_value_size = int.from_bytes(b[:self.split_size], byteorder='big')
+        dates_size = int.from_bytes(b[self.split_size:self.split_size*2], byteorder='big')
+        stocks_codes_size = int.from_bytes(b[self.split_size*2:self.split_size*3], byteorder='big')
+        start_index = self.split_size * 3
+        default_value_end_index = start_index + default_value_size
+        dates_end_index = default_value_end_index + dates_size
+        stock_codes_end_index = dates_end_index + stocks_codes_size
+        bs = [b[start_index : default_value_end_index], b[default_value_end_index : dates_end_index], b[dates_end_index : stock_codes_end_index], b[stock_codes_end_index:]]
+        nps = []
+        for a_b in bs:
+            nps.append(np_from_byte(a_b))
+        self.default_value = nps[0].item()
+        self.init_with_np(nps[1], np.array(nps[2], dtype=str), nps[3])
 
     def init_with_db_rows(self, rows, trade_date_column='tradeDate', stock_code_column='stockCode', value_column='itemValue'):
         df = pd.DataFrame.from_records(rows)
         if stock_code_column is None:
             df = df.set_index(trade_date_column)
             df = df.sort_index()
             df.columns = [STOCK_ZERO_CODE]
@@ -965,75 +862,65 @@
     def init_with_db_pivot(self, rows, trade_date_column, delete_columns):
         df = pd.DataFrame.from_records(rows).set_index(trade_date_column).drop(delete_columns, axis='columns')
         df.columns = [column_name.replace('\'', '').upper() for column_name in df.columns]
         self.init_with_dataframe(df)
 
     def init_with_dataframe(self, df):
         df = df[df.notnull()]
+        dtype = df.to_numpy().dtype
         self.dates = df.index.to_numpy()
         self.stock_codes = df.columns.to_numpy()
-        self.stock_codes = np.array(self.stock_codes, dtype=self.stock_codes.dtype)
-        self.data = df.to_numpy()
-        del df
-        if self.get_data_type() == 'NUMBER':
-            self.data = self.data.astype(float)
+        self.stock_codes = np.array(self.stock_codes, dtype=str)
+        if is_numeric_dtype(df.iloc[0]):
+            df = df.astype(float)
+            self.data = df.to_numpy(na_value=np.nan).astype(dtype)
+        else:
+            self.data = df.to_numpy().astype(dtype)
 
     def to_dataframe(self):
         #data = np.nan_to_num(self.data, posinf=np.nan, neginf=np.nan)
-        new_wit = self
-        WitData.relieve_strs(new_wit)
-        df = pd.DataFrame(data=new_wit.data, index=new_wit.dates, columns=new_wit.stock_codes)
+        df = pd.DataFrame(data=self.data, index=self.dates, columns=self.stock_codes)
         return df#.where(pd.notnull(df), None)
 
     def to_dict(self):
         return self.to_dataframe().to_dict('index')
 
     def to_factor_dict(self):
-        new_wit = self.copy()
-        WitData.relieve_strs(new_wit)
         v_func = np.vectorize(lambda x : {'itemValue':x if not math.isnan(x) else None})
+        new_wit = self.copy()
         new_wit.data = v_func(new_wit.data)
         return new_wit.to_dict()
 
     def to_bytes(self):
-        new_wit = self
-        WitData.make_strs(new_wit)
-        arr = [new_wit.default_value, new_wit.dates, new_wit.stock_codes, new_wit.strs, new_wit.data]
-        del new_wit
+        arr = [self.default_value, self.dates, self.stock_codes, self.data]
         bs = []
         for ele in arr:
             bs.append(np_to_byte(ele))
-        return b''.join([len(bs[0]).to_bytes(WitData.split_size, byteorder='big'), len(bs[1]).to_bytes(WitData.split_size, byteorder='big'), len(bs[2]).to_bytes(WitData.split_size, byteorder='big'), len(bs[3]).to_bytes(WitData.split_size, byteorder='big'), \
-            bs[0], bs[1], bs[2], bs[3], bs[4]])
+        return b''.join([len(bs[0]).to_bytes(self.split_size, byteorder='big'), len(bs[1]).to_bytes(self.split_size, byteorder='big'), len(bs[2]).to_bytes(self.split_size, byteorder='big'), \
+            bs[0], bs[1], bs[2], bs[3]])
     
     def save(self, filename):
-        dirs = filename.split('/')
-        for i, dir_name in enumerate(dirs):
-            full_dir_name = '/'.join(dirs[0:i])
-            if full_dir_name and full_dir_name != '' and not os.path.isdir(full_dir_name) and not os.path.isfile(full_dir_name):
-                os.mkdir(full_dir_name)
-
         data = self.to_bytes()
         with open(filename, "wb") as f:
             f.write(data)
     
     def to_tempfile(self):
         data = self.to_bytes()
         file = TemporaryFile()
         file.write(data)
         file.seek(0)
         return file
 
     def copy(self):
-        wit_data = np_to_wit_data(self.dates, self.stock_codes, self.data, default_value=self.default_value, strs=self.strs, rstring_flag=False)
+        wit_data = np_to_wit_data(self.dates, self.stock_codes, self.data, default_value=self.default_value)
         return wit_data
 
     def update(self, wit_data, copy=False):
         if not isinstance(wit_data, WitData):
-            if isinstance(wit_data, float) or isinstance(wit_data, bool) or isinstance(wit_data, str):
+            if isinstance(wit_data, float) or isinstance(wit_data, bool):
                 wit_data = value_to_wit_data(wit_data)
             else:
                 raise Exception('Value is not proper type.')
 
         wit_data = wit_data.spread(self.get_type())
         start_date = lib_min(wit_data.dates)
         end_date = lib_max(wit_data.dates)
@@ -1047,149 +934,162 @@
         df = new_self.to_dataframe()
         df.update(wit_data.to_dataframe())
         new_self = dataframe_to_wit_data(df)
 
         if copy:
             return new_self
         else:
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data, new_self.strs)
+            self.dates = new_self.dates
+            self.stock_codes = new_self.stock_codes
+            self.data = new_self.data
 
-    def vertical_update(self, wit_data, copy=False, default_value=np.nan):
+    def vertical_update(self, wit_data, copy=False):
         #self_start_date = lib_min(self.dates)
         #self_end_date = lib_max(self.dates)
 
         if not isinstance(wit_data, WitData):
-            if isinstance(wit_data, float) or isinstance(wit_data, bool) or isinstance(wit_data, str):
+            if isinstance(wit_data, float) or isinstance(wit_data, bool):
                 wit_data = value_to_wit_data(wit_data)
             else:
                 raise Exception('Value is not proper type.')
 
         wit_data = wit_data.spread(self.get_type())
         #wit_start_date = lib_min(wit_data.dates)
         #wit_end_date = lib_max(wit_data.dates)
         #wit_dates = wit_data.dates
 
-        new_self = self.get_date_data(np.array(list(set(self.dates) - set(wit_data.dates))))
-        new_self = dataframe_to_wit_data(pd.concat([new_self.to_dataframe(), wit_data.to_dataframe()], axis=0).fillna(default_value))
+        new_self = self.get_date_data(np.setdiff1d(self.dates, wit_data.dates))
+        new_self = dataframe_to_wit_data(pd.concat([new_self.to_dataframe(), wit_data.to_dataframe()], axis=0))
         new_self._arrange()
 
+        """reshape_wit_list = reshape_wit_data_list([self, wit_data])
+        new_self, wit_data = reshape_wit_list[0], reshape_wit_list[1]
+
+        wit_data = wit_data.get_date_data(wit_dates)
+
+        if wit_start_date < self_start_date:
+            if wit_end_date < self_start_date:
+                new_self = new_self.get_date_slicing(self_start_date, self_end_date)
+                new_self = np_to_wit_data(np.concatenate((wit_data.dates, new_self.dates)), new_self.stock_codes, np.vstack((wit_data.data, new_self.data)))
+            elif wit_end_date > self_end_date:
+                new_self = wit_data
+            else:
+                new_self = new_self.get_slicing(new_self.get_date_index(wit_end_date) + 1, None)
+                new_self = np_to_wit_data(np.concatenate((wit_data.dates, new_self.dates)), new_self.stock_codes, np.vstack((wit_data.data, new_self.data)))
+        elif wit_start_date > self_end_date:
+            new_self = new_self.get_date_slicing(self_start_date, self_end_date)
+            new_self = np_to_wit_data(np.concatenate((new_self.dates, wit_data.dates)), new_self.stock_codes, np.vstack((new_self.data, wit_data.data)))
+        else:
+            if wit_end_date > self_end_date:
+                new_self = new_self.get_slicing(None, new_self.get_date_index(wit_start_date))
+                new_self = np_to_wit_data(np.concatenate((new_self.dates, wit_data.dates)), new_self.stock_codes, np.vstack((new_self.data, wit_data.data)))
+            else:
+                front_self = new_self.get_slicing(None, new_self.get_date_index(wit_start_date))
+                rear_self = new_self.get_slicing(new_self.get_date_index(wit_end_date) + 1, None)
+                new_self = np_to_wit_data(np.concatenate((front_self.dates, wit_data.dates, rear_self.dates)), new_self.stock_codes, np.vstack((front_self.data, wit_data.data, rear_self.data)))
+        """
+
         if copy:
             return new_self
         else:
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data, new_self.strs)
+            self.dates = new_self.dates
+            self.stock_codes = new_self.stock_codes
+            self.data = new_self.data
 
-    def horizontal_update(self, wit_data, copy=False, default_value=np.nan):
+    def horizontal_update(self, wit_data, copy=False):
         if wit_data is None:
             new_self = self.copy()
         else:
             #self_stock_codes = self.stock_codes.copy()
             if not isinstance(wit_data, WitData):
-                if isinstance(wit_data, float) or isinstance(wit_data, bool) or isinstance(wit_data, str):
+                if isinstance(wit_data, float) or isinstance(wit_data, bool):
                     wit_data = value_to_wit_data(wit_data)
                 else:
                     raise Exception('Value is not proper type.')
 
             if not self.is_zero_code() and wit_data.is_zero_code():
                 wit_data.data = np.repeat(wit_data.data, len(self.stock_codes)).reshape((len(wit_data.dates), len(self.stock_codes)))
             elif self.is_zero_code() and not wit_data.is_zero_code():
                 self.data = np.repeat(self.data, len(wit_data.stock_codes)).reshape((len(self.dates), len(wit_data.stock_codes)))
 
             wit_data = wit_data.spread(self.get_type())
             #wit_stock_codes = wit_data.stock_codes.copy()
 
-            new_self = self.get_stocks_data(np.array(list(set(self.stock_codes) - set(wit_data.stock_codes))))
-            new_self = dataframe_to_wit_data(pd.concat([new_self.to_dataframe(), wit_data.to_dataframe()], axis=1).fillna(default_value))
+            new_self = self.get_stocks_data(np.setdiff1d(self.stock_codes, wit_data.stock_codes))
+            new_self = dataframe_to_wit_data(pd.concat([new_self.to_dataframe(), wit_data.to_dataframe()], axis=1))
             new_self._arrange()
+            
+            # reshape_wit_list = reshape_wit_data_list([self, wit_data])
+            # new_self, wit_data = reshape_wit_list[0], reshape_wit_list[1]
+
+            # new_self = new_self.get_stocks_data(np.setdiff1d(self_stock_codes, wit_stock_codes))
+            # wit_data = wit_data.get_stocks_data(wit_stock_codes)
+
+            # new_self = np_to_wit_data(new_self.dates, np.concatenate((new_self.stock_codes, wit_data.stock_codes)), np.hstack((new_self.data, wit_data.data)))
 
         if copy:
             return new_self
         else:
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data, new_self.strs)
+            self.dates = new_self.dates
+            self.stock_codes = new_self.stock_codes
+            self.data = new_self.data
 
     def get_date_index(self, date):
         date_key = -1
         if date in self.dates:
             date_key = np.where(self.dates==date)[0][0]
         else:
             print(f"DateKeyError(WitData) : {(date, self.dates)}")
         return date_key
 
     def get_stock_code_index(self, stock_code):
         stock_code_key = -1
-        keys = np.where((self.stock_codes==stock_code) if isinstance(stock_code, str) else (self.stock_codes==stock_code).all(axis=1))
-        if len(keys[0]) > 0:
-            stock_code_key = keys[0][0]
+        if len(np.where(self.stock_codes==stock_code)[0]) > 0:
+            stock_code_key = np.where(self.stock_codes==stock_code)[0][0]
         else:
             print(f"StockCodeKeyError(WitData) : {stock_code}")
         return stock_code_key
 
     def get(self, date, stock_code):
         date_key = self.get_date_index(date)
         stock_code_key = self.get_stock_code_index(stock_code)
 
         try:
-            if self.get_data_type() == 'RSTRING':
-                return_value = self.strs[self.data[date_key, stock_code_key]]
-            else:
-                return_value = self.data[date_key, stock_code_key]
+            return_value = self.data[date_key, stock_code_key]
         except:
             print(f"KeyError(WitData) : {date}, {stock_code}")
             return None
 
         return return_value
 
     def get_stock_data(self, stock_code):
         stock_code_key = self.get_stock_code_index(stock_code)
-        WitData.relieve_strs(self)
 
         try:
-            data = self.data[:, [stock_code_key]]
-            return_value = np_to_wit_data(self.dates.copy(), np.array([stock_code], dtype=str if isinstance(stock_code, str) else object), data, default_value=self.default_value, rstring_flag=False)
+            return_value = np_to_wit_data(self.dates.copy(), np.array([stock_code]), self.data[:, [stock_code_key]], default_value=self.default_value)
         except:
             print(f"KeyError(WitData) : {stock_code}")
             return None
 
         return return_value
 
     def get_stocks_data(self, stock_codes):
-        if set(self.stock_codes) == set(stock_codes):
-            return self.copy()
-
-        df = self.to_dataframe()
-        df = df.loc[:, list(set(self.stock_codes) & set(stock_codes))]
-        result = dataframe_to_wit_data(df)
-        # if len(self.stock_codes.shape) > 1:
-        #     stock_code_flags = [self.get_stock_code_index(stock_code) for stock_code in stock_codes]
-        # else:
-        #     stock_code_flags = np.where(np.isin(self.stock_codes, stock_codes))[0]
-        # result = np_to_wit_data(self.dates, np.array(self.stock_codes[stock_code_flags], dtype=self.stock_codes.dtype), self.data[:, stock_code_flags], default_value=self.default_value)
-        result._arrange()
-        return result
+        stock_code_flags = np.where(np.isin(self.stock_codes, stock_codes))[0]
+        return np_to_wit_data(self.dates, np.array(self.stock_codes[stock_code_flags], dtype=str), self.data[:, stock_code_flags], default_value=self.default_value)
 
     def get_date_data(self, dates):
-        WitData.relieve_strs(self)
-        data = self.data[np.isin(self.dates, dates)]
-        wit_data = np_to_wit_data(self.dates[np.isin(self.dates, dates)], self.stock_codes, data, default_value=self.default_value)
+        wit_data = np_to_wit_data(self.dates[np.isin(self.dates, dates)], self.stock_codes, self.data[np.isin(self.dates, dates)], default_value=self.default_value)
         return wit_data
 
     def switch_data(self, original_dates, data):
-        WitData.relieve_strs(self)
         data = np.array(data, dtype=self.data.dtype)
         for i, original_date in enumerate(original_dates):
             self.data[self.get_date_index(original_date)] = data[i]
 
     def get_date_slicing(self, start_date=None, end_date=None):
-        data_type = get_type_with_date_str(self.dates[0])
-        if WitDataType.DAY_TYPE == get_type_with_date_str(start_date) == get_type_with_date_str(end_date) != data_type:
-            start_date = get_date_format_with_day_format(start_date, data_type)
-            end_date = get_date_format_with_day_format(end_date, data_type)
-
-        if self.get_type() == WitDataType.PRESENT_TYPE:
-            return self
-
         start_index = None
         end_index = None
 
         if start_date is None or start_date < self.dates[0]:
             start_index = 0
         elif start_date > self.dates[-1]:
             return None
@@ -1202,428 +1102,218 @@
             return None
         else:
             end_index = np.max(np.where(self.dates <= end_date)) + 1
 
         return self.get_slicing(start_index, end_index)
 
     def get_slicing(self, start_index=None, end_index=None):
-        WitData.relieve_strs(self)
-        data = self.data[start_index:end_index]
-        wit_data = np_to_wit_data(self.dates[start_index:end_index], self.stock_codes, data, default_value=self.default_value)
+        wit_data = np_to_wit_data(self.dates[start_index:end_index], self.stock_codes, self.data[start_index:end_index], default_value=self.default_value)
         return wit_data
 
     def get_shift_days(self, days):
         if len(self.dates) > abs(days):
-            wit_data = self
-            WitData.relieve_strs(wit_data)
+            wit_data = self 
             if days > 0:
-                data = self.data[days:]
-                wit_data = np_to_wit_data(self.dates[:-days], self.stock_codes, data, default_value=self.default_value)
+                wit_data = np_to_wit_data(self.dates[:-days], self.stock_codes, self.data[days:], default_value=self.default_value)
             elif days < 0:
-                data = self.data[:days]
-                wit_data = np_to_wit_data(self.dates[-days:], self.stock_codes, data, default_value=self.default_value)
+                wit_data = np_to_wit_data(self.dates[-days:], self.stock_codes, self.data[:days], default_value=self.default_value)
             return wit_data
         else:
             return None
             #raise ValueError(f"dates : {self.dates}\ndays : {days}")
 
     def is_zero_code(self):
         return len(self.stock_codes) == 1 and self.stock_codes[0] == STOCK_ZERO_CODE
 
     def get_sliding_window(self, window):
-        WitData.relieve_strs(self)
         shape = tuple(np.array(self.data.shape) - np.array(window) + 1) + window
         strides = self.data.strides + self.data.strides
         return np.lib.stride_tricks.as_strided(self.data, shape=shape, strides=strides)
 
     def astype(self, a_type):
-        new_wit = WitData(self.default_value)
-        new_wit.dates = np.array(self.dates)
-        new_wit.stock_codes = np.array(self.stock_codes, dtype=self.stock_codes.dtype)
-        origin_dtype = self.data.dtype
-        if (np.issubdtype(origin_dtype, np.float_) and np.issubdtype(a_type, np.float_)) or \
-           (np.issubdtype(origin_dtype, np.int_) and np.issubdtype(a_type, np.int_)) or \
-           (np.issubdtype(origin_dtype, np.bool_) and np.issubdtype(a_type, np.bool_)) or \
-           (self.get_data_type() == 'RSTRING' and np.issubdtype(a_type, np.character)): # 그대로
-            new_wit.data = self.data
-        elif np.issubdtype(a_type, np.character): # 문자열로 바꿀때
-            new_wit.data = self.data.astype(a_type)
-        elif self.get_data_type() != 'RSTRING': # 기존로직
-            new_wit.data = self.data.astype(a_type)
-            new_wit.strs = np.array([])
-        else: # rstring -> 기타포맷
-            new_wit.data = self.data
-            new_wit.strs = self.strs
-            WitData.relieve_strs(new_wit)
-            new_wit.data = new_wit.data.astype(a_type)
-        return new_wit
-    
-    def unique(data):
-        if not isinstance(data, np.ndarray):
-            d = np.array(data)
-        else:
-            d = data
-
-        if len(d.shape) > 1:
-            d = d.flatten()
-
-        return np.sort(pd.unique(d))
-    
-    def unique_data(self):
-        return WitData.unique(self.data)
-    
-    def make_strs(wit):
-        if wit.get_data_type() == 'STRING':
-            wit.strs = wit.unique_data()
-            wit.data = np.searchsorted(wit.strs, wit.data)
-
-    def relieve_strs(wit):
-        if wit.get_data_type() == 'RSTRING':
-            data = np.full(wit.data.shape, '').astype(object)
-            for i in range(len(wit.data)):
-                data[i] = np.take(wit.strs, wit.data[i])
-            wit.data = data
-            wit.strs = np.array([])
-
-    def get_data_type(self):
-        dtype = self.data.dtype
-        if np.issubdtype(dtype, np.integer) and len(self.strs) > 0:
-            return 'RSTRING'
-        elif np.issubdtype(dtype, np.number):
-            return 'NUMBER'
-        elif np.issubdtype(dtype, np.bool_):
-            return 'BOOL'
-        elif np.issubdtype(dtype, object):
-            return 'STRING'
-        elif np.issubdtype(dtype, np.character):
-            return 'STRING'
-        else:
-            return None
-        
-    def get_dtype(self):
-        dtype = self.data.dtype
-        if np.issubdtype(dtype, np.integer) and len(self.strs) > 0:
-            return str
-        elif np.issubdtype(dtype, np.number):
-            return float
-        elif np.issubdtype(dtype, np.bool_):
-            return np.bool_
-        elif np.issubdtype(dtype, object):
-            return str
-        elif np.issubdtype(dtype, np.character):
-            return str
-        else:
-            return None
-
-    def groupby(self, calc_type, *wits, universe=None):
-        self_copy = self.copy()
-        if universe is not None:
-            universe = universe.get_stocks_data(self_copy.stock_codes)
-            wit_list = [self_copy, *wits, universe]
-            wit_list = reshape_wit_data_list(wit_list)
-            self_copy, *wits_copy, universe = wit_list[0], *wit_list[1:-1], wit_list[-1]
-        else:
-            wit_list = [self_copy, *wits]
-            wit_list = reshape_wit_data_list(wit_list)
-            self_copy, *wits_copy = wit_list[0], *wit_list[1:]
-
-        WitData.relieve_strs(self_copy)
-        for a_wit in wits_copy:
-            WitData.relieve_strs(a_wit)
-
-        distinct_elements = [a_wit.unique_data() for a_wit in wits_copy]
-        combination_elements = np.array(np.meshgrid(*distinct_elements), dtype=object).T.reshape(-1, len(distinct_elements))
-        
-        new_wit = np_to_wit_data(self_copy.dates, combination_elements if len(distinct_elements) > 1 else combination_elements.reshape(-1), np.zeros((len(self_copy.dates), len(combination_elements)), dtype=self.data.dtype))
-        new_wit.stock_codes = np.where(pd.isna(new_wit.stock_codes), '', new_wit.stock_codes).astype(str)
-
-        calc_func = None
-        if calc_type == 'SUM':
-            if self.get_data_type() == 'NUMBER':
-                calc_func = np.nansum
-            else:
-                calc_func = np.nanmax
-        elif calc_type == 'AVG':
-            if self.get_data_type() == 'NUMBER':
-                calc_func = np.nanmean
-            else:
-                calc_func = np.nanmax
-        elif calc_type == 'MIN':
-            calc_func = np.nanmin
-        elif calc_type == 'MAX':
-            calc_func = np.nanmax
-        elif calc_type == 'STD':
-            if self.get_data_type() == 'NUMBER':
-                calc_func = np.nanstd
-            else:
-                calc_func = np.nanmax
-        elif calc_type == 'POR':
-            if self.get_data_type() == 'NUMBER':
-                calc_func = np.nansum
-            else:
-                calc_func = np.nanmax
-        else:
-            calc_func = np.nanmax
-
-        for i, element in enumerate(combination_elements):
-            if universe is not None:
-                new_wit.data[:, i] = calc_func(np.where(reduce(np.ndarray.__and__, [universe.data, *[pd.isna(wit.data) if pd.isna(element[j]) else (wit.data == element[j]) for j, wit in enumerate(wits_copy)]]), self_copy.data, np.nan), axis=1)
-            else:
-                new_wit.data[:, i] = calc_func(np.where(reduce(np.ndarray.__and__, [pd.isna(wit.data) if pd.isna(element[j]) else (wit.data == element[j]) for j, wit in enumerate(wits_copy)]), self_copy.data, np.nan), axis=1)
-
-        if calc_type == 'POR':
-            all_sum = np.repeat(np.nansum(new_wit.data, axis=1).reshape(-1, 1), len(new_wit.stock_codes), axis=1)
-            new_wit.data = new_wit.data / all_sum * 100
-        
-        return new_wit
+        return np_to_wit_data(np.array(self.dates), np.array(self.stock_codes), np.array(self.data).astype(a_type))
 
     def __add__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        both_nan = pd.isna(new_self.data) & pd.isna(new_other.data)
-        if self.get_data_type() == 'NUMBER' and new_other.get_data_type() == 'NUMBER':
-            return np_to_wit_data(new_self.dates, new_self.stock_codes, np.where(both_nan, np.nan, np.nan_to_num(new_self.data) + np.nan_to_num(new_other.data)), default_value=new_self.default_value)
-        else:
-            self_df = new_self.to_dataframe()
-            self_df = self_df.where(~pd.isna(self_df), '').astype(str)
-            other_df = new_other.to_dataframe()
-            other_df = other_df.where(~pd.isna(other_df), '').astype(str)
-            return dataframe_to_wit_data(self_df + other_df)
+        both_nan = np.isnan(new_self.data) & np.isnan(new_other.data)
+        return np_to_wit_data(new_self.dates, new_self.stock_codes, np.where(both_nan, np.nan, np.nan_to_num(new_self.data) + np.nan_to_num(new_other.data)), default_value=new_self.default_value)
 
     def __sub__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        both_nan = pd.isna(new_self.data) & pd.isna(new_other.data)
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
+        both_nan = np.isnan(new_self.data) & np.isnan(new_other.data)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, np.where(both_nan, np.nan, np.nan_to_num(new_self.data) - np.nan_to_num(new_other.data)), default_value=new_self.default_value)
 
     def __mul__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data * (new_other.data if isinstance(new_other, WitData) else new_other), default_value=new_self.default_value)
 
     def __truediv__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data / (new_other.data if isinstance(new_other, WitData) else new_other), default_value=new_self.default_value)
 
     def __mod__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data % (new_other.data if isinstance(new_other, WitData) else new_other), default_value=new_self.default_value)
 
     def __pow__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data ** (new_other.data if isinstance(new_other, WitData) else new_other), default_value=new_self.default_value)
 
     def __and__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data & (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __or__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data | (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __iadd__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
-        if self.get_data_type() == 'NUMBER':
-            self.init_with_np(new_self.dates, new_self.stock_codes, np.nan_to_num(new_self.data) + (np.nan_to_num(new_other.data) if isinstance(new_other, WitData) else new_other))
-        else:
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data + (new_other.data if isinstance(new_other, WitData) else new_other))
+        self.init_with_np(new_self.dates, new_self.stock_codes, np.nan_to_num(new_self.data) + (np.nan_to_num(new_other.data) if isinstance(new_other, WitData) else new_other))
         return self
 
     def __isub__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         self.init_with_np(new_self.dates, new_self.stock_codes, np.nan_to_num(new_self.data) - (np.nan_to_num(new_other.data) if isinstance(new_other, WitData) else new_other))
         return self
 
     def __imul__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other])
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data * (new_other.data if isinstance(new_other, WitData) else new_other))
         return self
 
     def __idiv__(self, other):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            new_self = self.copy()
-            new_other = other.copy() if isinstance(other, WitData) else other
-            reshape_wits = reshape_wit_data_list([new_self, new_other])
-            new_self, new_other = reshape_wits[0], reshape_wits[1]
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data / (new_other.data if isinstance(new_other, WitData) else new_other))
-            return self
+        new_self = self.copy()
+        new_other = other.copy() if isinstance(other, WitData) else other
+        reshape_wits = reshape_wit_data_list([new_self, new_other])
+        new_self, new_other = reshape_wits[0], reshape_wits[1]
+        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data / (new_other.data if isinstance(new_other, WitData) else new_other))
+        return self
 
     def __imod__(self, other):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            new_self = self.copy()
-            new_other = other.copy() if isinstance(other, WitData) else other
-            reshape_wits = reshape_wit_data_list([new_self, new_other])
-            new_self, new_other = reshape_wits[0], reshape_wits[1]
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data % (new_other.data if isinstance(new_other, WitData) else new_other))
-            return self
+        new_self = self.copy()
+        new_other = other.copy() if isinstance(other, WitData) else other
+        reshape_wits = reshape_wit_data_list([new_self, new_other])
+        new_self, new_other = reshape_wits[0], reshape_wits[1]
+        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data % (new_other.data if isinstance(new_other, WitData) else new_other))
+        return self
 
     def __ipow__(self, other):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            new_self = self.copy()
-            new_other = other.copy() if isinstance(other, WitData) else other
-            reshape_wits = reshape_wit_data_list([new_self, new_other])
-            new_self, new_other = reshape_wits[0], reshape_wits[1]
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data ** (new_other.data if isinstance(new_other, WitData) else new_other))
-            return self
+        new_self = self.copy()
+        new_other = other.copy() if isinstance(other, WitData) else other
+        reshape_wits = reshape_wit_data_list([new_self, new_other])
+        new_self, new_other = reshape_wits[0], reshape_wits[1]
+        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data ** (new_other.data if isinstance(new_other, WitData) else new_other))
+        return self
 
     def __iand__(self, other):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            new_self = self.copy()
-            new_other = other.copy() if isinstance(other, WitData) else other
-            reshape_wits = reshape_wit_data_list([new_self, new_other])
-            new_self, new_other = reshape_wits[0], reshape_wits[1]
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data & (new_other.data if isinstance(new_other, WitData) else new_other))
-            return self
+        new_self = self.copy()
+        new_other = other.copy() if isinstance(other, WitData) else other
+        reshape_wits = reshape_wit_data_list([new_self, new_other])
+        new_self, new_other = reshape_wits[0], reshape_wits[1]
+        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data & (new_other.data if isinstance(new_other, WitData) else new_other))
+        return self
 
     def __ior__(self, other):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            new_self = self.copy()
-            new_other = other.copy() if isinstance(other, WitData) else other
-            reshape_wits = reshape_wit_data_list([new_self, new_other])
-            new_self, new_other = reshape_wits[0], reshape_wits[1]
-            self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data | (new_other.data if isinstance(new_other, WitData) else new_other))
-            return self
+        new_self = self.copy()
+        new_other = other.copy() if isinstance(other, WitData) else other
+        reshape_wits = reshape_wit_data_list([new_self, new_other])
+        new_self, new_other = reshape_wits[0], reshape_wits[1]
+        self.init_with_np(new_self.dates, new_self.stock_codes, new_self.data | (new_other.data if isinstance(new_other, WitData) else new_other))
+        return self
 
     def __neg__(self):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), -self.data, default_value=self.default_value)
+        return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), -self.data, default_value=self.default_value)
 
     def __pos__(self):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), +self.data, default_value=self.default_value)
+        return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), +self.data, default_value=self.default_value)
 
     def __abs__(self):
-        if self.get_data_type().endswith('RSTRING'):
-            return self
-        else:
-            return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), abs(self.data), default_value=self.default_value)
+        return np_to_wit_data(self.dates.copy(), self.stock_codes.copy(), abs(self.data), default_value=self.default_value)
 
     def __lt__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data < (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __le__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data <= (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __eq__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data == (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __ne__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data != (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __ge__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data >= (new_other.data if isinstance(new_other, WitData) else new_other))
 
     def __gt__(self, other):
         new_self = self.copy()
         new_other = other.copy() if isinstance(other, WitData) else other
         reshape_wits = reshape_wit_data_list([new_self, new_other], 0)
         new_self, new_other = reshape_wits[0], reshape_wits[1]
-        WitData.relieve_strs(new_self)
-        WitData.relieve_strs(new_other)
         return np_to_wit_data(new_self.dates, new_self.stock_codes, new_self.data > (new_other.data if isinstance(new_other, WitData) else new_other))
 
 class Connector:
     temp_bucket = "ffolio.motoo.temp"
     temp_access = 'AKIAVWWT2XJMYRDE24M4' # account only for s3 upload
     temp_secret = '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'
-    api_server = os.environ['MODOOWITS_API_SERVER'] if 'MODOOWITS_API_SERVER' in os.environ and os.environ['MODOOWITS_API_SERVER'] else 'https://api.quantbox.net'
+    api_server = os.environ['MODOOWITS_API_SERVER'] if 'MODOOWITS_API_SERVER' in os.environ and os.environ['MODOOWITS_API_SERVER'] else 'https://api.modoowits.com'
 
     def __init__(self, api_key):
         self.api_key = api_key
 
     def get_factor_list(self):
         api_url = Connector.api_server + '/saved_wits.wit.get_factor_list'
 
@@ -1638,50 +1328,48 @@
 
         data = dict()
         data['api_key'] = self.api_key
         response = Connector._request(api_url, data)
 
         return response['result'] if 'result' in response else None
 
-    def register_my_wit(self, wit, title, description, meta=None):
+    def register_my_wit(self, wit, title, description):
         api_url = Connector.api_server + '/saved_wits.wit.register_my_wit'
 
         tempfile = wit.to_tempfile()
         s3Client = boto3.client('s3',
             aws_access_key_id=Connector.temp_access, 
             aws_secret_access_key=Connector.temp_secret)
         temp_wit_id = str(uuid.uuid1()).replace('-','')
         s3Client.upload_fileobj(tempfile, Connector.temp_bucket, temp_wit_id)
 
         data = dict()
         data['api_key'] = self.api_key
         data['title'] = title
         data['description'] = description
-        if meta: data['meta'] = meta
         data['temp_wit_id'] = temp_wit_id
         data['work_type'] = 'REGISTER'
         response = Connector._request(api_url, data)
         
         return response['result'] if 'result' in response else None
 
-    def update_my_wit(self, wit_id, wit, title, description, meta=None):
+    def update_my_wit(self, wit_id, wit, title, description):
         api_url = Connector.api_server + '/saved_wits.wit.register_my_wit'
 
         tempfile = wit.to_tempfile()
         s3Client = boto3.client('s3',
             aws_access_key_id=Connector.temp_access, 
             aws_secret_access_key=Connector.temp_secret)
         temp_wit_id = str(uuid.uuid1()).replace('-','')
         s3Client.upload_fileobj(tempfile, Connector.temp_bucket, temp_wit_id)
 
         data = dict()
         data['api_key'] = self.api_key
         data['title'] = title
         data['description'] = description
-        if meta: data['meta'] = meta
         data['temp_wit_id'] = temp_wit_id
         data['work_type'] = 'UPDATE'
         data['wit_id'] = wit_id
         response = Connector._request(api_url, data)
         
         return response['result'] if 'result' in response else None
 
@@ -1756,25 +1444,14 @@
     def get_last_wit_with_title(self, title):
         response = self.get_last_wit_descriptor_with_title(title)
         if 'wit' in response:
             return response['wit']
         else:
             return response
 
-    def get_last_wit_meta_with_title(self, title):
-        api_url = Connector.api_server + '/saved_wits.wit.get_last_wit_meta_with_title'
-
-        data = dict()
-        data['api_key'] = self.api_key
-        data['title'] = title
-        response = Connector._request(api_url, data)
-        if 'result' not in response: return None
-        response = response['result']
-        return response
-
     def get_last_wit_descriptor_with_title(self, title):
         api_url = Connector.api_server + '/saved_wits.wit.get_last_wit_with_title'
 
         data = dict()
         data['api_key'] = self.api_key
         data['title'] = title
         response = Connector._request(api_url, data)
```

## Comparing `motoo-1.1.89.dist-info/METADATA` & `motoo-1.1.9.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motoo
-Version: 1.1.89
+Version: 1.1.9
 Summary: motoo utils
 Home-page: UNKNOWN
 Author: ffolio
 Author-email: david@ffolio.co.kr
 License: UNKNOWN
 Keywords: pypi deploy
 Platform: UNKNOWN
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
-Requires-Dist: boto3
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: requests
 Requires-Dist: scipy
+Requires-Dist: boto3
+Requires-Dist: requests
 
 UNKNOWN
```

