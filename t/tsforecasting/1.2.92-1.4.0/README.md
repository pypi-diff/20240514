# Comparing `tmp/tsforecasting-1.2.92-py3-none-any.whl.zip` & `tmp/tsforecasting-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 24420 bytes, number of entries: 17
+Zip file size: 24389 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 tsforecasting/__init__.py
 -rw-rw-rw-  2.0 fat     9670 b- defN 24-May-06 21:34 tsforecasting/forecasting.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 tsforecasting/configs/__init__.py
 -rw-rw-rw-  2.0 fat     2776 b- defN 24-May-06 20:48 tsforecasting/configs/parameters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 tsforecasting/models/__init__.py
 -rw-rw-rw-  2.0 fat    27183 b- defN 24-May-06 20:48 tsforecasting/models/forecasting_models.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 tsforecasting/performance/__init__.py
 -rw-rw-rw-  2.0 fat     5852 b- defN 24-May-06 20:48 tsforecasting/performance/evaluation.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 tsforecasting/processing/__init__.py
--rw-rw-rw-  2.0 fat    12477 b- defN 24-May-06 22:36 tsforecasting/processing/processor.py
+-rw-rw-rw-  2.0 fat    12338 b- defN 24-May-14 19:58 tsforecasting/processing/processor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 tsforecasting/training/__init__.py
 -rw-rw-rw-  2.0 fat    11206 b- defN 24-May-06 21:34 tsforecasting/training/validation.py
--rw-rw-rw-  2.0 fat     1078 b- defN 24-May-07 21:28 tsforecasting-1.2.92.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9791 b- defN 24-May-07 21:28 tsforecasting-1.2.92.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 21:28 tsforecasting-1.2.92.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-May-07 21:28 tsforecasting-1.2.92.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1504 b- defN 24-May-07 21:28 tsforecasting-1.2.92.dist-info/RECORD
-17 files, 81645 bytes uncompressed, 21890 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-May-14 19:59 tsforecasting-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9788 b- defN 24-May-14 19:59 tsforecasting-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 19:59 tsforecasting-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-May-14 19:59 tsforecasting-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1499 b- defN 24-May-14 19:59 tsforecasting-1.4.0.dist-info/RECORD
+17 files, 81498 bytes uncompressed, 21869 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tsforecasting/training/__init__.py
 Comment: 
 
 Filename: tsforecasting/training/validation.py
 Comment: 
 
-Filename: tsforecasting-1.2.92.dist-info/LICENSE
+Filename: tsforecasting-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting-1.2.92.dist-info/METADATA
+Filename: tsforecasting-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting-1.2.92.dist-info/WHEEL
+Filename: tsforecasting-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting-1.2.92.dist-info/top_level.txt
+Filename: tsforecasting-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting-1.2.92.dist-info/RECORD
+Filename: tsforecasting-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsforecasting/processing/processor.py

```diff
@@ -79,83 +79,83 @@
                 
         # Concatenate the new features at the beginning of the DataFrame
         X = pd.concat([X_, X], axis=1)
     
         return X
     
     def make_timeseries(self, 
-                        dataset: pd.DataFrame,
-                        window_size: int, 
-                        horizon: int, 
-                        granularity : str = '1d',
-                        datetime_engineering : bool = True):
+                    dataset: pd.DataFrame,
+                    window_size: int, 
+                    horizon: int, 
+                    granularity: str = '1d',
+                    datetime_engineering: bool = True):
         """
         Transforms a DataFrame into a single DataFrame containing sequential windows and horizon predictions,
         including NaNs where full horizon data isn't available. This allows using all available data for training up to the last point.
-
+    
         Args:
             dataset (pd.DataFrame): A DataFrame with at least a 'y' column for time series data and a 'Date' column.
             window_size (int): The number of time steps in each window, indicating how many past observations each input sample includes.
             horizon (int): The number of time steps to predict into the future, which sets how far ahead the labels are relative to the end of each window.
             granularity (str): granularity of datetime column: 1m,30m,1h,1d,1wk,1mo (default='1d')
         Returns:
             pd.DataFrame: A DataFrame where each row represents a window of observations and horizon predictions,
                           starting with the date of the window, followed by lag features, and then horizon predictions.
-
+    
         Raises:
             ValueError: If the `window_size` is larger than the input array length, which would make windowing impossible.
         """
         
         if window_size > len(dataset):
             raise ValueError("The lags length (window_size) cannot exceed the length of the time_series.")
-
-        if granularity=='1wk': granularity="1W"
+    
         time_series = dataset[self.target].values
         date_series = dataset['Date'].values  
-
+    
         # Calculate the maximum index for creating windows
         max_window_index = len(time_series) - window_size
-
+    
         # Create windows and corresponding dates
         windows = np.array([time_series[i:i + window_size] for i in range(max_window_index + 1)])
-            
-        if granularity=='1mo':
-            granularity = '1M'
-            extended_dates = np.array([
-                                        date_series[window_size:][-1] + (
-                                            pd.DateOffset(months=(int(granularity[:-1]) * (i + 1))) if granularity.endswith('M') else
-                                            pd.DateOffset(years=(int(granularity[:-1]) * (i + 1))) if granularity.endswith('Y') else
-                                            pd.Timedelta(granularity, n=(i + 1))
-                                        ) for i in range(1)
-                                    ])
-        else:
-            extended_dates = np.array([date_series[window_size:][-1] + pd.Timedelta(granularity, n=i + 1) for i in range(1)])
-        date_col = np.concatenate([date_series[window_size:], extended_dates])
-        date_col = pd.to_datetime(date_col, unit='ns')
-        
+        window_dates = date_series[window_size - 1:]  # Date corresponding to the end of each window
+    
         # Create horizons, allowing NaNs for the future windows
         horizons = np.array([time_series[i + window_size:i + window_size + horizon] if i + window_size + horizon <= len(time_series)
-                             else np.concatenate([time_series[i + window_size:len(time_series)], np.full((i + window_size + horizon - len(time_series)), np.nan)])
+                             else np.concatenate([time_series[i + window_size:], np.full((i + window_size + horizon - len(time_series)), np.nan)])
                              for i in range(max_window_index + 1)])
-
+    
+        # Add future NaN horizons
+        future_dates = [pd.to_datetime(date_series[-1])] #+ pd.Timedelta(granularity) * (i + 1) for i in range(horizon)]
+        future_windows = [time_series[-window_size:] for _ in range(horizon)]
+        future_horizons = np.array([np.full((horizon,), np.nan) for _ in range(horizon)])
+    
+        # Combine past and future windows and horizons
+        windows = np.concatenate([windows, future_windows[:1]])
+        horizons = np.concatenate([horizons, future_horizons[:1]])
+        window_dates = np.concatenate([window_dates, future_dates[:1]])
+    
+        # Ensure window_dates are datetime
+        window_dates = pd.to_datetime(window_dates)
+    
         # Column names for windows and horizons
         self.lag_cols = [f'y_lag_{i+1}' for i in range(window_size)]
         self.horizon_cols = [f'y_horizon_{i+1}' for i in range(horizon)]
-
+    
         # Create DataFrame for lags and horizons
         lag_df = pd.DataFrame(windows, columns=self.lag_cols)
         horizon_df = pd.DataFrame(horizons, columns=self.horizon_cols)
-
+    
         # Combine into one DataFrame
         X = pd.concat([lag_df, horizon_df], axis=1).reset_index(drop=True)
-        X.insert(0, 'Date', date_col)
+        X.insert(0, 'Date', window_dates)
         
         if datetime_engineering:
             X = self.engin_date(dataset = X,
                                 drop = True)
+        X = X.head(X.shape[0]-1)
         
         self.target_cols = [col for col in X.columns if 'horizon' in col]
         self.input_cols = [col for col in X.columns if col not in self.target_cols]
         
         return X
     
     def future_timestamps(self, dataset: pd.DataFrame, horizon: int, granularity: str = '1d'):
```

## Comparing `tsforecasting-1.2.92.dist-info/LICENSE` & `tsforecasting-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.92.dist-info/METADATA` & `tsforecasting-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.92
+Version: 1.4.0
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -36,15 +36,15 @@
 <br>
 <p align="center">
   <h2 align="center"> TSForecasting - Automated Time Series Forecasting Framework
   <br>
   
 ## Framework Contextualization <a name = "ta"></a>
 
-The `TSForecasting` project offers a comprehensive and integrated pipeline designed to Automate Time Series Forecasting applications. By implementing multivariate approaches that incorporate multiple regression models, it combines multiple relevant modules such as `SKLearn`, `AutoGluon`, `CatBoost` and `XGBoost`, following an `Expanding Window` structured approach for performance evaluation ensuring a robust, scalable and optimized forecasting solution.
+The `TSForecasting` project offers a comprehensive and integrated pipeline designed to Automate Time Series Forecasting applications. By implementing multivariate approaches that incorporate multiple regression models, it combines varied relevant modules such as `SKLearn`, `AutoGluon`, `CatBoost` and `XGBoost`, following an `Expanding Window` structured approach for performance evaluation ensuring a robust, scalable and optimized forecasting solution.
 
 The architecture design includes five main sections, these being: data preprocessing, feature engineering, hyperparameter optimization, forecast ensembling and forecasting method selection which are organized and customizable in a pipeline structure.
 
 This project aims at providing the following application capabilities:
 
 * General applicability on tabular datasets: The developed forecasting procedures are applicable on any data table associated with any Time Series Forecasting scopes.
```

## Comparing `tsforecasting-1.2.92.dist-info/RECORD` & `tsforecasting-1.4.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 tsforecasting/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tsforecasting/configs/parameters.py,sha256=_E3qc3dUcIQgT8_q_0fU9TyXEy4qgLIp37shYe6FJck,2776
 tsforecasting/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tsforecasting/models/forecasting_models.py,sha256=zyxxrjI-b5_io4b9kplfihekf2TBbIIaNf3yH_fRCT4,27183
 tsforecasting/performance/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tsforecasting/performance/evaluation.py,sha256=_HS6FWMp9JaKP5zyl6SP19r4eNfy6GAz5-gyiGdnFqI,5852
 tsforecasting/processing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tsforecasting/processing/processor.py,sha256=GCfylfG2kM7EOdQFzvdIyTlKMIyLjiwBov43P22YrBI,12477
+tsforecasting/processing/processor.py,sha256=LeDFhGF8tWr5hnNfKFPIAAesNbNfvH-btD9PKQvlITA,12338
 tsforecasting/training/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tsforecasting/training/validation.py,sha256=xifCz95kcC_Bdaz1K6MDnYFFLGuhje5hLulk-fJD26k,11206
-tsforecasting-1.2.92.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
-tsforecasting-1.2.92.dist-info/METADATA,sha256=tOfL9vXUW9KNYjtRnsWyaoVfcMiXLma0cY_aZ8dlRHU,9791
-tsforecasting-1.2.92.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tsforecasting-1.2.92.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
-tsforecasting-1.2.92.dist-info/RECORD,,
+tsforecasting-1.4.0.dist-info/LICENSE,sha256=KDcNU0R4Ruo5yPyqmRZJGMYbASNPn58LJSr359FVFfA,1078
+tsforecasting-1.4.0.dist-info/METADATA,sha256=qtPGi6m4bxzkExMBf4Xy6Cus4S-LA0vXuuSqnFH_75Q,9788
+tsforecasting-1.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+tsforecasting-1.4.0.dist-info/top_level.txt,sha256=oKWWwpca0QkvqhgDcYBoVWqcFDLNSkSOuCvuEcZFABY,14
+tsforecasting-1.4.0.dist-info/RECORD,,
```

