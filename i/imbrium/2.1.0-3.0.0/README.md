# Comparing `tmp/imbrium-2.1.0.tar.gz` & `tmp/imbrium-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imbrium-2.1.0.tar", last modified: Wed Oct 25 05:35:39 2023, max compression
+gzip compressed data, was "imbrium-3.0.0.tar", last modified: Mon May 13 23:47:49 2024, max compression
```

## Comparing `imbrium-2.1.0.tar` & `imbrium-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.651675 imbrium-2.1.0/
--rw-rw-rw-   0        0        0     2528 2023-10-25 04:15:24.000000 imbrium-2.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-2.1.0/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0   124482 2023-10-25 05:35:39.649130 imbrium-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0   101503 2023-10-25 03:57:48.000000 imbrium-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.537293 imbrium-2.1.0/imbrium/
--rw-rw-rw-   0        0        0      245 2023-10-17 23:51:34.000000 imbrium-2.1.0/imbrium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.574762 imbrium-2.1.0/imbrium/architectures/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:43:43.000000 imbrium-2.1.0/imbrium/architectures/__init__.py
--rw-rw-rw-   0        0        0    54361 2023-10-25 04:56:19.000000 imbrium-2.1.0/imbrium/architectures/models.py
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.591066 imbrium-2.1.0/imbrium/blueprints/
--rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-2.1.0/imbrium/blueprints/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-10-18 00:06:23.000000 imbrium-2.1.0/imbrium/blueprints/abstract_multivariate.py
--rw-rw-rw-   0        0        0     1939 2023-10-18 00:06:23.000000 imbrium-2.1.0/imbrium/blueprints/abstract_univariate.py
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.621961 imbrium-2.1.0/imbrium/predictors/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:43:58.000000 imbrium-2.1.0/imbrium/predictors/__init__.py
--rw-rw-rw-   0        0        0    43272 2023-10-25 04:56:19.000000 imbrium-2.1.0/imbrium/predictors/multivarhybrid.py
--rw-rw-rw-   0        0        0    41475 2023-10-25 04:56:19.000000 imbrium-2.1.0/imbrium/predictors/multivarpure.py
--rw-rw-rw-   0        0        0    42361 2023-10-25 04:56:19.000000 imbrium-2.1.0/imbrium/predictors/univarhybrid.py
--rw-rw-rw-   0        0        0    41227 2023-10-25 04:56:19.000000 imbrium-2.1.0/imbrium/predictors/univarpure.py
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.637926 imbrium-2.1.0/imbrium/utils/
--rw-rw-rw-   0        0        0        0 2023-09-24 18:44:13.000000 imbrium-2.1.0/imbrium/utils/__init__.py
--rw-rw-rw-   0        0        0      784 2023-09-24 00:54:18.000000 imbrium-2.1.0/imbrium/utils/optimizer.py
--rw-rw-rw-   0        0        0    10284 2023-10-15 16:44:37.000000 imbrium-2.1.0/imbrium/utils/transformer.py
-drwxrwxrwx   0        0        0        0 2023-10-25 05:35:39.564645 imbrium-2.1.0/imbrium.egg-info/
--rw-rw-rw-   0        0        0   124482 2023-10-25 05:35:39.000000 imbrium-2.1.0/imbrium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-10-25 05:35:39.000000 imbrium-2.1.0/imbrium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-25 05:35:39.000000 imbrium-2.1.0/imbrium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-10-25 05:35:39.000000 imbrium-2.1.0/imbrium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-25 05:35:39.000000 imbrium-2.1.0/imbrium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-25 05:35:39.651675 imbrium-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-10-25 05:08:48.000000 imbrium-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.841497 imbrium-3.0.0/
+-rw-rw-rw-   0        0        0     2990 2024-05-13 01:00:22.000000 imbrium-3.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0   102154 2024-05-13 23:47:49.825900 imbrium-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0   101412 2024-05-13 23:07:01.000000 imbrium-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.653997 imbrium-3.0.0/imbrium/
+-rw-rw-rw-   0        0        0      245 2023-12-03 16:02:47.000000 imbrium-3.0.0/imbrium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.716493 imbrium-3.0.0/imbrium/architectures/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:43:43.000000 imbrium-3.0.0/imbrium/architectures/__init__.py
+-rw-rw-rw-   0        0        0    54099 2024-05-13 22:58:17.000000 imbrium-3.0.0/imbrium/architectures/models.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.732121 imbrium-3.0.0/imbrium/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-3.0.0/imbrium/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     2375 2024-05-13 22:58:14.000000 imbrium-3.0.0/imbrium/blueprints/abstract_multivariate.py
+-rw-rw-rw-   0        0        0     2247 2024-05-13 22:58:14.000000 imbrium-3.0.0/imbrium/blueprints/abstract_univariate.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.778998 imbrium-3.0.0/imbrium/predictors/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:43:58.000000 imbrium-3.0.0/imbrium/predictors/__init__.py
+-rw-rw-rw-   0        0        0    43757 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/multivarhybrid.py
+-rw-rw-rw-   0        0        0    42043 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/multivarpure.py
+-rw-rw-rw-   0        0        0    42846 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/univarhybrid.py
+-rw-rw-rw-   0        0        0    41739 2024-05-13 22:58:18.000000 imbrium-3.0.0/imbrium/predictors/univarpure.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.810251 imbrium-3.0.0/imbrium/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-24 18:44:13.000000 imbrium-3.0.0/imbrium/utils/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-12-03 12:53:22.000000 imbrium-3.0.0/imbrium/utils/optimizer.py
+-rw-rw-rw-   0        0        0    10924 2024-05-12 19:50:14.000000 imbrium-3.0.0/imbrium/utils/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:47:49.700871 imbrium-3.0.0/imbrium.egg-info/
+-rw-rw-rw-   0        0        0   102154 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 23:47:49.000000 imbrium-3.0.0/imbrium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 23:47:49.841497 imbrium-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2024-05-11 21:54:00.000000 imbrium-3.0.0/setup.py
```

### Comparing `imbrium-2.1.0/CHANGELOG.md` & `imbrium-3.0.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -80,23 +80,31 @@
 
 - added depth parameter to architectures
 - added optimizer configuration support
 - added optimizer configuration to seeker
 
 ### 2.0.0
 
-- adapted `keras_core`
+- adapted `keras`
 - removed internal hyperparameter tuning
 - removed encoder-decoder architectures
 - improved layer configuration via dictionary input
 - split data argument into target and feature numpy arrays
  
 ### 2.0.1
 
 - fix: removed dead pandas imports 
 - chore: added tensorflow as base requirement
  
 ### 2.1.0
 
 - feat!: removed data preparation out of predictor class, sub_seq, steps_past, steps_future need now to be defined in each model method
   - allows for advanced hyper parameter tuning
-- fix: removed tensor board activation logic bug
+- fix: removed tensor board activation logic bug
+
+### 3.0.0
+
+- chore!: changed from temp library keras_core to keras > 3.0.0
+- chore!: removed python 3.8 support to accomodate tensorflow and keras dependiencies
+- chore: increased major to 3.0.0 to align with keras major
+- feat: added evaluate_model method to test model performance on test data
+- refactor!: removed validation split from `fit_model`. Control validation and test split via evaluation_split and validation_split paramters in class variables
```

### Comparing `imbrium-2.1.0/LICENSE` & `imbrium-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imbrium-2.1.0/PKG-INFO` & `imbrium-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,2793 +1,2776 @@
-Metadata-Version: 2.1
-Name: imbrium
-Version: 2.1.0
-Summary: Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.
-Home-page: https://github.com/maxmekiska/imbrium
-Author: Maximilian Mekiska
-Author-email: maxmekiska@gmail.com
-License: UNKNOWN
-Description: # imbrium [![Downloads](https://pepy.tech/badge/imbrium)](https://pepy.tech/project/imbrium) [![PyPi](https://img.shields.io/pypi/v/imbrium.svg?color=blue)](https://pypi.org/project/imbrium/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/Imbrium?color=black)](https://github.com/maxmekiska/Imbrium/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/imbrium.svg)](https://pypi.python.org/project/imbrium/)
-         
-        ## Status
-        
-        | Build | Status|
-        |---|---|
-        | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=main) |
-        |  `DEV BUILD`   |  ![development](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=development) |
-        
-        ## Pip install
-        
-        ```shell
-        pip install imbrium
-        ```
-        
-        Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step
-        Time Series Forecasting.
-        
-        
-                                  ██╗███╗░░░███╗██████╗░██████╗░██╗██╗░░░██╗███╗░░░███╗
-                                    ║████╗░████║██╔══██╗██╔══██╗██║██║░░░██║████╗░████║
-                                  ██║██╔████╔██║██████╦╝██████╔╝██║██║░░░██║██╔████╔██║
-                                  ██║██║╚██╔╝██║██╔══██╗██╔══██╗██║██║░░░██║██║╚██╔╝██║
-                                  ██║██║░╚═╝░██║██████╦╝██║░░██║██║╚██████╔╝██║░╚═╝░██║
-                                  ╚═╝╚═╝░░░░░╚═╝╚═════╝░╚═╝░░╚═╝╚═╝░╚═════╝░╚═╝░░░░░╚═╝
-        
-        
-        ## Introduction to imbrium
-        
-        imbrium is a deep learning library that specializes in time series forecasting. Its primary objective is to provide a user-friendly repository of deep learning architectures for this purpose. The focus is on simplifying the process of creating and applying these architectures, with the goal of allowing users to create complex architectures without having to build them from scratch. Instead, the emphasis shifts to high-level configuration of the architectures.
-        
-        
-        ## imbrium Summary
-        
-        imbrium is designed to simplify the application of deep learning models for time series forecasting. The library offers a variety of pre-built architectures. The user retains full control over the configuration of each layer, including the number of neurons, the type of activation function, loss function, optimizer, and metrics applied. This allows for the flexibility to adapt the architecture to the specific needs of the forecast task at hand. Imbrium also offers a user-friendly interface for training and evaluating these models, making it easy to quickly iterate and test different configurations.
-        
-        imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window (steps_past) through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables (steps_future). This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
-        
-        ## imbrium 2.0.0
-        
-        - adapting `keras_core`
-        - removing internal hyperparameter tuning
-        - removing encoder-decoder architectures
-        - improve layer configuration
-        - split input data into target and feature numpy arrays
-        - overall lighten the library
-        
-        ### Get started with imbrium
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        <details>
-          <summary>Univariate Pure Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import PureUni
-        
-        # create a PureUni object (numpy array expected)
-        predictor = PureUni(target = target_numpy_array) 
-        
-        # the following models are available for a PureUni objects;
-        
-        # create and fit a muti-layer perceptron model
-        predictor.create_fit_mlp( 
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                dense_block_one = 1,
-                dense_block_two = 1,
-                dense_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a recurrent neural network model
-        predictor.create_fit_rnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                rnn_block_three = 1,
-                metrics = "mean_squared_error",
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a long short-term neural network model
-        predictor.create_fit_lstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                lstm_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional neural network
-        predictor = create_fit_cnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                dense_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a gated recurrent unit neural network  
-        predictor.create_fit_gru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                gru_block_one = 1,
-                gru_block_two = 1,
-                gru_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional recurrent neural network
-        predictor.create_fit_birnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional long short-term memory neural network
-        predictor.create_fit_bilstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional gated recurrent neural network
-        predictor.create_fit_bigru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        predictor.predict(data)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        
-        </details>
-        
-        <details>
-          <summary>Multivariate Pure Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import PureMulti
-        
-        # create a PureMulti object (numpy array expected)
-        predictor = PureMulti(target = target_numpy_array, features = features_numpy_array) 
-        
-        # the following models are available for a PureMulti objects;
-        
-        # create and fit a muti-layer perceptron model
-        predictor.create_fit_mlp( 
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                dense_block_one = 1,
-                dense_block_two = 1,
-                dense_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a recurrent neural network model
-        predictor.create_fit_rnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                rnn_block_three = 1,
-                metrics = "mean_squared_error",
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a long short-term neural network model
-        predictor.create_fit_lstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                lstm_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional neural network
-        predictor = create_fit_cnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                dense_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a gated recurrent unit neural network  
-        predictor.create_fit_gru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                gru_block_one = 1,
-                gru_block_two = 1,
-                gru_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional recurrent neural network
-        predictor.create_fit_birnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional long short-term memory neural network
-        predictor.create_fit_bilstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional gated recurrent neural network
-        predictor.create_fit_bigru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        predictor.predict(data)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        </details>
-        
-        <details>
-          <summary>Univariate Hybrid Predictors</summary>
-          <br>
-        
-        ```python
-        from imbrium import HybridUni
-        
-        # create a HybridUni object (numpy array expected)
-        predictor = HybridUni(target = target_numpy_array) 
-        
-        # the following models are available for a HybridUni objects:
-        # create and fit a convolutional recurrent neural network
-        predictor.create_fit_cnnrnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional long short-term memory neural network
-        predictor.create_fit_cnnlstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional gated recurrent unit neural network  
-        predictor.create_fit_cnngru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                gru_block_one = 1,
-                gru_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional recurrent neural network
-        predictor.create_fit_cnnbirnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional long short-term neural network
-        predictor.create_fit_cnnbilstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional gated recurrent neural network
-        predictor.create_fit_cnnbigru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
-        predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        
-        </details>
-        
-        <details>
-          <summary>Multivariate Hybrid Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import HybridMulti
-        
-        # create a HybridMulti object (numpy array expected)
-        predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array) 
-        
-        # the following models are available for a HybridMulti objects:
-        # create and fit a convolutional recurrent neural network
-        predictor.create_fit_cnnrnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional long short-term memory neural network
-        predictor.create_fit_cnnlstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional gated recurrent unit neural network  
-        predictor.create_fit_cnngru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                gru_block_one = 1,
-                gru_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional recurrent neural network
-        predictor.create_fit_cnnbirnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional long short-term neural network
-        predictor.create_fit_cnnbilstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional gated recurrent neural network
-        predictor.create_fit_cnnbigru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
-        predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        </details>
-        
-        </details>
-        
-        ### Use Case: scaling + hyper parameter optimization
-        
-        https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/use-case-1.ipynb
-        
-        ### Integration tests
-        
-        https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/IntegrationTest.ipynb
-        
-        
-        ## LEGACY: imbrium versions <= v.1.3.0
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        The library differentiates between two
-        modes:
-        
-        1. Univariate-Multistep forecasting
-        2. Multivariate-Multistep forecasting
-        
-        These two main modes are further divided based on the complexity of the underlying model architectures:
-        
-        1. Pure
-        2. Hybrid
-        
-        Pure supports the following architectures:
-        
-        - Multilayer perceptron (MLP)
-        - Recurrent neural network (RNN)
-        - Long short-term memory (LSTM)
-        - Gated recurrent unit (GRU)
-        - Convolutional neural network (CNN)
-        - Bidirectional recurrent neural network (BI-RNN)
-        - Bidirectional long-short term memory (BI-LSTM)
-        - Bidirectional gated recurrent unit (BI-GRU)
-        - Encoder-Decoder recurrent neural network
-        - Encoder-Decoder long-short term memory
-        - Encoder-Decoder convolutional neural network (Encoding via CNN, Decoding via GRU)
-        - Encoder-Decoder gated recurrent unit
-        
-        Hybrid supports:
-        
-        - Convolutional neural network + recurrent neural network (CNN-RNN)
-        - Convolutional neural network + Long short-term memory (CNN-LSTM)
-        - Convolutional neural network + Gated recurrent unit (CNN-GRU)
-        - Convolutional neural network + Bidirectional recurrent neural network (CNN-BI-RNN)
-        - Convolutional neural network + Bidirectional long-short term memory (CNN-BI-LSTM)
-        - Convolutional neural network + Bidirectional gated recurrent unit (CNN-BI-GRU)
-        
-        Please note that each model is supported by a prior input data pre-processing procedure which allows to set a look-back period, look-forward period, sub-sequences division (only for hybrid architectures) and data scaling method.
-        
-        The following scikit-learn scaling procedures are supported:
-        
-        - StandardScaler
-        - MinMaxScaler
-        - MaxAbsScaler
-        - Normalizing ([0, 1])
-        - None (raw data input)
-        
-        During training/fitting, callback conditions can be defined to guard against
-        overfitting.
-        
-        Trained models can furthermore be saved or loaded if the user wishes to do so.
-        
-        ## How to use imbrium?
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Attention: Typing has been left in the below examples to ease the configuration readability.
-        
-        #### Version updates:
-        
-        ##### Version >= 1.2.0
-        
-        Version 1.2.0 started supporting tensor board dashboards: https://www.tensorflow.org/tensorboard/get_started
-        
-        ##### Version >= 1.3.0
-        
-        Version 1.3.0 started supporting adjustable layer depth configurations for all architectures. If you wish to adjust the layer depth, please make sure to include a custom layer_config accounting for the correct number of layers. The last layer cannot contain a dropout parameter -> tuple needs to be of length 3: (neurons, activation, regularization).
-        
-        ### `Univariate Models`:
-        
-        1. Univariate-Multistep forecasting - Pure architectures
-        
-        ```python
-        from imbrium.predictors.univarpure import PureUni
-        
-        predictor = PureUni(
-                            steps_past: int,
-                            steps_future: int,
-                            data = pd.DataFrame(),
-                            scale: str = ''
+# imbrium [![Downloads](https://pepy.tech/badge/imbrium)](https://pepy.tech/project/imbrium) [![PyPi](https://img.shields.io/pypi/v/imbrium.svg?color=blue)](https://pypi.org/project/imbrium/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/Imbrium?color=black)](https://github.com/maxmekiska/Imbrium/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/imbrium.svg)](https://pypi.python.org/project/imbrium/)
+ 
+## Status
+
+| Build | Status|
+|---|---|
+| `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=main) |
+|  `DEV BUILD`   |  ![development](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=development) |
+
+## Pip install
+
+```shell
+pip install imbrium
+```
+
+Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step
+Time Series Forecasting.
+
+
+                          ██╗███╗░░░███╗██████╗░██████╗░██╗██╗░░░██╗███╗░░░███╗
+                            ║████╗░████║██╔══██╗██╔══██╗██║██║░░░██║████╗░████║
+                          ██║██╔████╔██║██████╦╝██████╔╝██║██║░░░██║██╔████╔██║
+                          ██║██║╚██╔╝██║██╔══██╗██╔══██╗██║██║░░░██║██║╚██╔╝██║
+                          ██║██║░╚═╝░██║██████╦╝██║░░██║██║╚██████╔╝██║░╚═╝░██║
+                          ╚═╝╚═╝░░░░░╚═╝╚═════╝░╚═╝░░╚═╝╚═╝░╚═════╝░╚═╝░░░░░╚═╝
+
+
+## Introduction to imbrium
+
+imbrium is a deep learning library that specializes in time series forecasting. Its primary objective is to provide a user-friendly repository of deep learning architectures for this purpose. The focus is on simplifying the process of creating and applying these architectures, with the goal of allowing users to create complex architectures without having to build them from scratch. Instead, the emphasis shifts to high-level configuration of the architectures.
+
+
+## imbrium Summary
+
+imbrium is designed to simplify the application of deep learning models for time series forecasting. The library offers a variety of pre-built architectures. The user retains full control over the configuration of each layer, including the number of neurons, the type of activation function, loss function, optimizer, and metrics applied. This allows for the flexibility to adapt the architecture to the specific needs of the forecast task at hand. Imbrium also offers a user-friendly interface for training and evaluating these models, making it easy to quickly iterate and test different configurations.
+
+imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window - `steps_past` through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables - `steps_future`. This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
+
+## imbrium `2.0.0`
+
+- adapting `keras_core`
+- removing internal hyperparameter tuning
+- removing encoder-decoder architectures
+- improve layer configuration
+- split input data into target and feature numpy arrays
+- overall lighten the library
+
+## imbrium `3.0.0`
+
+- switch from `keras_core` to `keras > 3.0.0`
+
+### Get started with imbrium
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+<details>
+  <summary>Univariate Pure Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import PureUni
+
+# create a PureUni object (numpy array expected)
+predictor = PureUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a PureUni objects;
+
+# create and fit a muti-layer perceptron model
+predictor.create_fit_mlp( 
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        dense_block_one = 1,
+        dense_block_two = 1,
+        dense_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a recurrent neural network model
+predictor.create_fit_rnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        rnn_block_three = 1,
+        metrics = "mean_squared_error",
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a long short-term neural network model
+predictor.create_fit_lstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        lstm_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional neural network
+predictor = create_fit_cnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        dense_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a gated recurrent unit neural network  
+predictor.create_fit_gru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        gru_block_one = 1,
+        gru_block_two = 1,
+        gru_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional recurrent neural network
+predictor.create_fit_birnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional long short-term memory neural network
+predictor.create_fit_bilstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional gated recurrent neural network
+predictor.create_fit_bigru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+predictor.predict(data)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+
+</details>
+
+<details>
+  <summary>Multivariate Pure Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import PureMulti
+
+# create a PureMulti object (numpy array expected)
+predictor = PureMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a PureMulti objects;
+
+# create and fit a muti-layer perceptron model
+predictor.create_fit_mlp( 
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        dense_block_one = 1,
+        dense_block_two = 1,
+        dense_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a recurrent neural network model
+predictor.create_fit_rnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        rnn_block_three = 1,
+        metrics = "mean_squared_error",
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a long short-term neural network model
+predictor.create_fit_lstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        lstm_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional neural network
+predictor = create_fit_cnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        dense_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a gated recurrent unit neural network  
+predictor.create_fit_gru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        gru_block_one = 1,
+        gru_block_two = 1,
+        gru_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional recurrent neural network
+predictor.create_fit_birnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional long short-term memory neural network
+predictor.create_fit_bilstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional gated recurrent neural network
+predictor.create_fit_bigru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+predictor.predict(data)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+</details>
+
+<details>
+  <summary>Univariate Hybrid Predictors</summary>
+  <br>
+
+```python
+from imbrium import HybridUni
+
+# create a HybridUni object (numpy array expected)
+predictor = HybridUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a HybridUni objects:
+# create and fit a convolutional recurrent neural network
+predictor.create_fit_cnnrnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional long short-term memory neural network
+predictor.create_fit_cnnlstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional gated recurrent unit neural network  
+predictor.create_fit_cnngru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        gru_block_one = 1,
+        gru_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional recurrent neural network
+predictor.create_fit_cnnbirnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional long short-term neural network
+predictor.create_fit_cnnbilstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional gated recurrent neural network
+predictor.create_fit_cnnbigru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+# - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
+predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+
+</details>
+
+<details>
+  <summary>Multivariate Hybrid Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import HybridMulti
+
+# create a HybridMulti object (numpy array expected)
+predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a HybridMulti objects:
+# create and fit a convolutional recurrent neural network
+predictor.create_fit_cnnrnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional long short-term memory neural network
+predictor.create_fit_cnnlstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional gated recurrent unit neural network  
+predictor.create_fit_cnngru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        gru_block_one = 1,
+        gru_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional recurrent neural network
+predictor.create_fit_cnnbirnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional long short-term neural network
+predictor.create_fit_cnnbilstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional gated recurrent neural network
+predictor.create_fit_cnnbigru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+# - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
+predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+</details>
+
+</details>
+
+### Use Case: scaling + hyper parameter optimization
+
+https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/use-case-1.ipynb
+
+### Integration tests
+
+https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/IntegrationTest.ipynb
+
+
+## legacy: imbrium versions `<= 1.3.0`
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The library differentiates between two
+modes:
+
+1. Univariate-Multistep forecasting
+2. Multivariate-Multistep forecasting
+
+These two main modes are further divided based on the complexity of the underlying model architectures:
+
+1. Pure
+2. Hybrid
+
+Pure supports the following architectures:
+
+- Multilayer perceptron (MLP)
+- Recurrent neural network (RNN)
+- Long short-term memory (LSTM)
+- Gated recurrent unit (GRU)
+- Convolutional neural network (CNN)
+- Bidirectional recurrent neural network (BI-RNN)
+- Bidirectional long-short term memory (BI-LSTM)
+- Bidirectional gated recurrent unit (BI-GRU)
+- Encoder-Decoder recurrent neural network
+- Encoder-Decoder long-short term memory
+- Encoder-Decoder convolutional neural network (Encoding via CNN, Decoding via GRU)
+- Encoder-Decoder gated recurrent unit
+
+Hybrid supports:
+
+- Convolutional neural network + recurrent neural network (CNN-RNN)
+- Convolutional neural network + Long short-term memory (CNN-LSTM)
+- Convolutional neural network + Gated recurrent unit (CNN-GRU)
+- Convolutional neural network + Bidirectional recurrent neural network (CNN-BI-RNN)
+- Convolutional neural network + Bidirectional long-short term memory (CNN-BI-LSTM)
+- Convolutional neural network + Bidirectional gated recurrent unit (CNN-BI-GRU)
+
+Please note that each model is supported by a prior input data pre-processing procedure which allows to set a look-back period, look-forward period, sub-sequences division (only for hybrid architectures) and data scaling method.
+
+The following scikit-learn scaling procedures are supported:
+
+- StandardScaler
+- MinMaxScaler
+- MaxAbsScaler
+- Normalizing ([0, 1])
+- None (raw data input)
+
+During training/fitting, callback conditions can be defined to guard against
+overfitting.
+
+Trained models can furthermore be saved or loaded if the user wishes to do so.
+
+## How to use imbrium?
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Attention: Typing has been left in the below examples to ease the configuration readability.
+
+#### Version updates:
+
+##### Version >= 1.2.0
+
+Version 1.2.0 started supporting tensor board dashboards: https://www.tensorflow.org/tensorboard/get_started
+
+##### Version >= 1.3.0
+
+Version 1.3.0 started supporting adjustable layer depth configurations for all architectures. If you wish to adjust the layer depth, please make sure to include a custom layer_config accounting for the correct number of layers. The last layer cannot contain a dropout parameter -> tuple needs to be of length 3: (neurons, activation, regularization).
+
+### `Univariate Models`:
+
+1. Univariate-Multistep forecasting - Pure architectures
+
+```python
+from imbrium.predictors.univarpure import PureUni
+
+predictor = PureUni(
+                    steps_past: int,
+                    steps_future: int,
+                    data = pd.DataFrame(),
+                    scale: str = ''
+                   )
+
+# Choose between one of the architectures:
+
+predictor.create_mlp(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     dense_block_one: int = 1,
+                     dense_block_two: int = 1,
+                     dense_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                    )
+
+predictor.create_rnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     rnn_block_one: int = 1,
+                     rnn_block_two: int = 1,
+                     rnn_block_three: int = 1,
+                     layer_config: dict = 
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_lstm(
+                      optimizer: str = 'adam',
+                      optimizer_args: dict = None,
+                      loss: str = 'mean_squared_error',
+                      metrics: str = 'mean_squared_error',
+                      lstm_block_one: int = 1,
+                      lstm_block_two: int = 1,
+                      lstm_block_three: int = 1,
+                      layer_config: dict =
+                      {
+                        'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                     )
+
+predictor.create_gru(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     gru_block_one: int = 1,
+                     gru_block_two: int = 1,
+                     gru_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_cnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     conv_block_one: int = 1,
+                     conv_block_two: int = 1,
+                     dense_block_one: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer2': (2), # (pool_size)
+                      'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_birnn(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       birnn_block_one: int = 1,
+                       rnn_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_bilstm(
+                        optimizer: str = 'adam', 
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        bilstm_block_one: int = 1,
+                        lstm_block_one: int = 1,
+                        layer_config: dict = 
+                        {
+                          'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                       )
+
+predictor.create_bigru(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       bigru_block_one: int = 1,
+                       gru_block_one: int = 1,
+                       layer_config: dict = 
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_encdec_rnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_rnn_block_one: int = 1,
+                            enc_rnn_block_two: int = 1,
+                            dec_rnn_block_one: int = 1,
+                            dec_rnn_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                            )
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_mlp(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             dense_block_one: int = 1,
-                             dense_block_two: int = 1,
-                             dense_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                            )
-        
-        predictor.create_rnn(
+
+predictor.create_encdec_lstm(
                              optimizer: str = 'adam',
                              optimizer_args: dict = None,
                              loss: str = 'mean_squared_error',
                              metrics: str = 'mean_squared_error',
-                             rnn_block_one: int = 1,
-                             rnn_block_two: int = 1,
-                             rnn_block_three: int = 1,
+                             enc_lstm_block_one: int = 1,
+                             enc_lstm_block_two: int = 1,
+                             dec_lstm_block_one: int = 1,
+                             dec_lstm_block_two: int = 1,
                              layer_config: dict = 
                              {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
                              }
                             )
-        
-        predictor.create_lstm(
-                              optimizer: str = 'adam',
-                              optimizer_args: dict = None,
-                              loss: str = 'mean_squared_error',
-                              metrics: str = 'mean_squared_error',
-                              lstm_block_one: int = 1,
-                              lstm_block_two: int = 1,
-                              lstm_block_three: int = 1,
-                              layer_config: dict =
-                              {
-                                'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                             )
-        
-        predictor.create_gru(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             gru_block_one: int = 1,
-                             gru_block_two: int = 1,
-                             gru_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_cnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             conv_block_one: int = 1,
-                             conv_block_two: int = 1,
-                             dense_block_one: int = 1,
-                             layer_config: dict =
-                             {
+
+predictor.create_encdec_cnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_conv_block_one: int = 1,
+                            enc_conv_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict = 
+                            {
                               'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer2': (2), # (pool_size)
-                              'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_birnn(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               birnn_block_one: int = 1,
-                               rnn_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_bilstm(
-                                optimizer: str = 'adam', 
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                bilstm_block_one: int = 1,
-                                lstm_block_one: int = 1,
-                                layer_config: dict = 
-                                {
-                                  'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                               )
-        
-        predictor.create_bigru(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               bigru_block_one: int = 1,
-                               gru_block_one: int = 1,
-                               layer_config: dict = 
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_encdec_rnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_rnn_block_one: int = 1,
-                                    enc_rnn_block_two: int = 1,
-                                    dec_rnn_block_one: int = 1,
-                                    dec_rnn_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                   )
-        
-        predictor.create_encdec_lstm(
-                                     optimizer: str = 'adam',
-                                     optimizer_args: dict = None,
-                                     loss: str = 'mean_squared_error',
-                                     metrics: str = 'mean_squared_error',
-                                     enc_lstm_block_one: int = 1,
-                                     enc_lstm_block_two: int = 1,
-                                     dec_lstm_block_one: int = 1,
-                                     dec_lstm_block_two: int = 1,
-                                     layer_config: dict = 
-                                     {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                     }
-                                    )
-        
-        predictor.create_encdec_cnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_conv_block_one: int = 1,
-                                    enc_conv_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict = 
-                                    {
-                                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer2': (2), # (pool_size)
-                                      'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer4': (100, 'relu', 0.0)  # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_gru(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_gru_block_one: int = 1,
-                                    enc_gru_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict = 
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss', 
-                            patience=3
-                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor = PureUni(steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        
-        2. Univariate-Multistep forecasting - Hybrid architectures
-        
-        ```python
-        from imbrium.predictors.univarhybrid import HybridUni
-        
-        predictor = HybridUni(
-                              sub_seq: int,
-                              steps_past: int,
-                              steps_future: int, data = pd.DataFrame(),
-                              scale: str = ''
-                             )
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_cnnrnn(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                rnn_block_one: int = 1,
-                                rnn_block_two: int = 1,
-                                layer_config = 
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0, 0.0) # (neurons, activation, regularization, dropout)
-                                }
-                              )
-        
-        predictor.create_cnnlstm(
-                                 optimizer: str = 'adam', 
-                                 optimizer_args: dict = None,
-                                 loss: str = 'mean_squared_error',
-                                 metrics: str = 'mean_squared_error',
-                                 conv_block_one: int = 1,
-                                 conv_block_two: int = 1,
-                                 lstm_block_one: int = 1,
-                                 lstm_block_two: int = 1,
-                                 layer_config = 
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnngru(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                gru_block_one: int = 1,
-                                gru_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnbirnn(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  birnn_block_one: int = 1,
-                                  rnn_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        predictor.create_cnnbilstm(
-                                   optimizer: str = 'adam',
-                                   optimizer_args: dict = None,
-                                   loss: str = 'mean_squared_error',
-                                   metrics: str = 'mean_squared_error',
-                                   conv_block_one: int = 1,
-                                   conv_block_two: int = 1,
-                                   bilstm_block_one: int = 1,
-                                   lstm_block_one: int = 1,
-                                   layer_config =
-                                   {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_cnnbigru(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  bigru_block_one: int = 1,
-                                  gru_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
-                            )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor =  HybridUni(sub_seq: int, steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        
-        ### `Multivariate Models`:
-        
-        1. Multivariate-Multistep forecasting - Pure architectures
-        
-        ```python
-        from imbrium.predictors.multivarpure import PureMulti
-        
-        # please make sure that the target feature is the first variable in the feature list
-        predictor = PureMulti(steps_past: int, steps_future: int, data = DataFrame(), features = [], scale: str = '')
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_mlp(
+                              'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer4': (100, 'relu', 0.0)  # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_encdec_gru(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_gru_block_one: int = 1,
+                            enc_gru_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict = 
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss', 
+                    patience=3
+                   )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor = PureUni(steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+
+2. Univariate-Multistep forecasting - Hybrid architectures
+
+```python
+from imbrium.predictors.univarhybrid import HybridUni
+
+predictor = HybridUni(
+                      sub_seq: int,
+                      steps_past: int,
+                      steps_future: int, data = pd.DataFrame(),
+                      scale: str = ''
+                     )
+
+# Choose between one of the architectures:
+
+predictor.create_cnnrnn(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        rnn_block_one: int = 1,
+                        rnn_block_two: int = 1,
+                        layer_config = 
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0, 0.0) # (neurons, activation, regularization, dropout)
+                        }
+                      )
+
+predictor.create_cnnlstm(
+                         optimizer: str = 'adam', 
+                         optimizer_args: dict = None,
+                         loss: str = 'mean_squared_error',
+                         metrics: str = 'mean_squared_error',
+                         conv_block_one: int = 1,
+                         conv_block_two: int = 1,
+                         lstm_block_one: int = 1,
+                         lstm_block_two: int = 1,
+                         layer_config = 
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnngru(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        gru_block_one: int = 1,
+                        gru_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnbirnn(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          birnn_block_one: int = 1,
+                          rnn_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
+                        )
+
+predictor.create_cnnbilstm(
+                           optimizer: str = 'adam',
+                           optimizer_args: dict = None,
+                           loss: str = 'mean_squared_error',
+                           metrics: str = 'mean_squared_error',
+                           conv_block_one: int = 1,
+                           conv_block_two: int = 1,
+                           bilstm_block_one: int = 1,
+                           lstm_block_one: int = 1,
+                           layer_config =
+                           {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_cnnbigru(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          bigru_block_one: int = 1,
+                          gru_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
+                        )
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                    )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor =  HybridUni(sub_seq: int, steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+
+### `Multivariate Models`:
+
+1. Multivariate-Multistep forecasting - Pure architectures
+
+```python
+from imbrium.predictors.multivarpure import PureMulti
+
+# please make sure that the target feature is the first variable in the feature list
+predictor = PureMulti(steps_past: int, steps_future: int, data = DataFrame(), features = [], scale: str = '')
+
+# Choose between one of the architectures:
+
+predictor.create_mlp(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     dense_block_one: int = 1,
+                     dense_block_two: int = 1,
+                     dense_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_rnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     rnn_block_one: int = 1,
+                     rnn_block_two: int = 1,
+                     rnn_block_three: int = 1,
+                     layer_config: dict = 
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_lstm(
+                      optimizer: str = 'adam',
+                      optimizer_args: dict = None,
+                      loss: str = 'mean_squared_error',
+                      metrics: str = 'mean_squared_error',
+                      lstm_block_one: int = 1,
+                      lstm_block_two: int = 1,
+                      lstm_block_three: int = 1,
+                      layer_config: dict =
+                      {
+                        'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50,'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
+                        'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                    )
+
+predictor.create_gru(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     gru_block_one: int = 1,
+                     gru_block_two: int = 1,
+                     gru_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     } 
+                    )
+
+predictor.create_cnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     conv_block_one: int = 1,
+                     conv_block_two: int = 1,
+                     dense_block_one: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer2': (2), # (pool_size)
+                      'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_birnn(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       birnn_block_one: int = 1,
+                       rnn_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_bilstm(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        bilstm_block_one: int = 1,
+                        lstm_block_one: int = 1,
+                        layer_config: dict =
+                        {
+                          'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_bigru(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       bigru_block_one: int = 1,
+                       gru_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_encdec_rnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_rnn_block_one: int = 1,
+                            enc_rnn_block_two: int = 1,
+                            dec_rnn_block_one: int = 1,
+                            dec_rnn_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_encdec_lstm(
                              optimizer: str = 'adam',
                              optimizer_args: dict = None,
                              loss: str = 'mean_squared_error',
                              metrics: str = 'mean_squared_error',
-                             dense_block_one: int = 1,
-                             dense_block_two: int = 1,
-                             dense_block_three: int = 1,
+                             enc_lstm_block_one: int = 1,
+                             enc_lstm_block_two: int = 1,
+                             dec_lstm_block_one: int = 1,
+                             dec_lstm_block_two: int = 1,
                              layer_config: dict =
                              {
-                              'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
                              }
                             )
-        
-        predictor.create_rnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             rnn_block_one: int = 1,
-                             rnn_block_two: int = 1,
-                             rnn_block_three: int = 1,
-                             layer_config: dict = 
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_lstm(
-                              optimizer: str = 'adam',
-                              optimizer_args: dict = None,
-                              loss: str = 'mean_squared_error',
-                              metrics: str = 'mean_squared_error',
-                              lstm_block_one: int = 1,
-                              lstm_block_two: int = 1,
-                              lstm_block_three: int = 1,
-                              layer_config: dict =
-                              {
-                                'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50,'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
-                                'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                            )
-        
-        predictor.create_gru(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             gru_block_one: int = 1,
-                             gru_block_two: int = 1,
-                             gru_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             } 
-                            )
-        
-        predictor.create_cnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             conv_block_one: int = 1,
-                             conv_block_two: int = 1,
-                             dense_block_one: int = 1,
-                             layer_config: dict =
-                             {
+
+predictor.create_encdec_cnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_conv_block_one: int = 1,
+                            enc_conv_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict =
+                            {
                               'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer2': (2), # (pool_size)
-                              'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_birnn(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               birnn_block_one: int = 1,
-                               rnn_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_bilstm(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                bilstm_block_one: int = 1,
-                                lstm_block_one: int = 1,
-                                layer_config: dict =
-                                {
-                                  'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_bigru(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               bigru_block_one: int = 1,
-                               gru_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_encdec_rnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_rnn_block_one: int = 1,
-                                    enc_rnn_block_two: int = 1,
-                                    dec_rnn_block_one: int = 1,
-                                    dec_rnn_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_lstm(
-                                     optimizer: str = 'adam',
-                                     optimizer_args: dict = None,
-                                     loss: str = 'mean_squared_error',
-                                     metrics: str = 'mean_squared_error',
-                                     enc_lstm_block_one: int = 1,
-                                     enc_lstm_block_two: int = 1,
-                                     dec_lstm_block_one: int = 1,
-                                     dec_lstm_block_two: int = 1,
-                                     layer_config: dict =
-                                     {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                     }
-                                    )
-        
-        predictor.create_encdec_cnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_conv_block_one: int = 1,
-                                    enc_conv_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer2': (2), # (pool_size)
-                                      'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer4': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_gru(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_gru_block_one: int = 1,
-                                    enc_gru_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
+                              'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer4': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor = PureMulti(steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        2. Multivariate-Multistep forecasting - Hybrid architectures
-        
-        ```python
-        from imbrium.predictors.multivarhybrid import HybridMulti
-        
-        # please make sure that the target feature is the first variable in the feature list
-        predictor = HybridMulti(sub_seq: int, steps_past: int, steps_future: int, data = DataFrame(), features:list = [], scale: str = '')
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_cnnrnn(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                rnn_block_one: int = 1,
-                                rnn_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnlstm(
-                                 optimizer: str = 'adam',
-                                 optimizer_args: dict = None,
-                                 loss: str = 'mean_squared_error',
-                                 metrics: str = 'mean_squared_error',
-                                 conv_block_one: int = 1,
-                                 conv_block_two: int = 1,
-                                 lstm_block_one: int = 1,
-                                 lstm_block_two: int = 1,
-                                 layer_config =
-                                 {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                 }
-                                )
-        
-        predictor.create_cnngru(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                gru_block_one: int = 1,
-                                gru_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnbirnn(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  birnn_block_one: int = 1,
-                                  rnn_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        predictor.create_cnnbilstm(
-                                   optimizer: str = 'adam',
-                                   optimizer_args: dict = None,
-                                   loss: str = 'mean_squared_error',
-                                   metrics: str = 'mean_squared_error',
-                                   conv_block_one: int = 1,
-                                   conv_block_two: int = 1,
-                                   bilstm_block_one: int = 1,
-                                   lstm_block_one: int = 1,
-                                   layer_config =
-                                   {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                   }
-                                  )
-        
-        predictor.create_cnnbigru(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  bigru_block_one: int = 1,
-                                  gru_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
+
+predictor.create_encdec_gru(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_gru_block_one: int = 1,
+                            enc_gru_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor =  HybridMulti(sub_seq: int, steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        </details>
-        
-        ## Hyperparameter Optimization imbrium 1.1.0
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Starting from version 1.1.0, imbrium will support experimental hyperparamerter optimization for the model layer config and optimizer arguments. The optimization process uses the Optuna library (https://optuna.org/).
-        
-        ### Optimization via the seeker decorator
-        
-        To leverage Optimization, use the new classes `OptimizePureUni`, `OptimizeHybridUni`, `OptimizePureMulti` and `OptimizeHybridMulti`. These classes implement optimizable model architecture methods:
-        
-        `OptimizePureUni` & `OptimizePureMulti`:
-        
-          - create_fit_mlp
-          - create_fit_rnn
-          - create_fit_lstm
-          - create_fit_cnn
-          - create_fit_gru
-          - create_fit_birnn
-          - create_fit_bilstm
-          - create_fit_bigru
-          - create_fit_encdec_rnn
-          - create_fit_encdec_lstm
-          - create_fit_encdec_gru
-          - create_fit_encdec_cnn
-        
-        `OptimizeHybridUni` & `OptimizeHybridMulti`:
-        
-          - create_fit_cnnrnn
-          - create_fit_cnnlstm
-          - create_fit_cnngru
-          - create_fit_cnnbirnn
-          - create_fit_cnnbilstm
-          - create_fit_cnnbigru
-        
-        #### Example `OptimizePureUni`
-        
-        ```python
-        from imbrium.predictors.univarpure import OptimizePureUni
-        from imbrium.utils.optimization import seeker
-        
-        # initialize optimizable predictor object
-        predictor = OptimizePureUni(steps_past=5, steps_future=10, data=data, scale='standard')
-        
-        
-        # use seeker decorator on optimization harness
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (5, 'relu'),
-                      'layer1': (10,'relu'),
-                      'layer2': (5, 'relu')
-                    },
-                    {
-                      'layer0': (2, 'relu'),
-                      'layer1': (5, 'relu'),
-                      'layer2': (2, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 2)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            # use optimizable create_fit_xxx method
-            return predictor.create_fit_lstm(*args, **kwargs)
-        
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=0,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
-                        )
-        
-        predictor.show_performance()
-        predictor.predict(data.tail(5))
-        predictor.model_blueprint()
-        ```
-        
-        #### Example `OptimizeHybridUni`
-        
-        ```python
-        from imbrium.predictors.univarhybrid import OptimizeHybridUni
-        from imbrium.utils.optimization import seeker
-        
-        predictor = OptimizeHybridUni(sub_seq = 2, steps_past = 10, steps_future = 5, data = data, scale = 'maxabs')
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (25, 'relu'),
-                      'layer4': (10, 'relu')
-                    },
-                    {
-                      'layer0': (16, 1, 'relu'),
-                      'layer1': (8, 1, 'relu'),
-                      'layer2': (2)
-                      'layer3': (55, 'relu'),
-                      'layer4': (10, 'relu')
-                    },
-                    {
-                      'layer0': (32, 1, 'relu'),
-                      'layer1': (16, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (25, 'relu'),
-                      'layer4': (10, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 2)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_cnnlstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=0,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                  )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor = PureMulti(steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+2. Multivariate-Multistep forecasting - Hybrid architectures
+
+```python
+from imbrium.predictors.multivarhybrid import HybridMulti
+
+# please make sure that the target feature is the first variable in the feature list
+predictor = HybridMulti(sub_seq: int, steps_past: int, steps_future: int, data = DataFrame(), features:list = [], scale: str = '')
+
+# Choose between one of the architectures:
+
+predictor.create_cnnrnn(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        rnn_block_one: int = 1,
+                        rnn_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnlstm(
+                         optimizer: str = 'adam',
+                         optimizer_args: dict = None,
+                         loss: str = 'mean_squared_error',
+                         metrics: str = 'mean_squared_error',
+                         conv_block_one: int = 1,
+                         conv_block_two: int = 1,
+                         lstm_block_one: int = 1,
+                         lstm_block_two: int = 1,
+                         layer_config =
+                         {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                         }
                         )
-        
-        predictor.show_performance()
-        predictor.predict(data.tail(10))
-        predictor.model_blueprint()
-        ```
-        
-        #### Example `OptimizePureMulti`
-        
-        ```python
-        predictor = OptimizePureMulti(
-                                      steps_past =  5,
-                                      steps_future = 10,
-                                      data = data,
-                                      features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
-                                      scale = 'normalize'
-                                    )
-        
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (5, 'relu'),
-                      'layer1': (10,'relu'),
-                      'layer2': (5, 'relu')
-                    },
-                    {
-                      'layer0': (2, 'relu'),
-                      'layer1': (5, 'relu'),
-                      'layer2': (2, 'relu')
-                    },
-                    {
-                      'layer0': (20, 'relu'),
-                      'layer1': (50, 'relu'),
-                      'layer2': (20, 'sigmoid')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 3)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_lstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=1, 
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+predictor.create_cnngru(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        gru_block_one: int = 1,
+                        gru_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnbirnn(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          birnn_block_one: int = 1,
+                          rnn_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
                         )
-        
-        
-        predictor.show_performance()
-        predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(5))
-        predictor.model_blueprint()
-        ```
-        
-        
-        #### Example `OptimizeHybridMulti`
-        
-        ```python
-        predictor = OptimizeHybridMulti(
-                                        sub_seq = 2, 
-                                        steps_past = 10,
-                                        steps_future = 5,
-                                        data = data,
-                                        features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
-                                        scale = 'normalize'
-                                      )
-        
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    },
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    },
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 3)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_cnnlstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=1,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+predictor.create_cnnbilstm(
+                           optimizer: str = 'adam',
+                           optimizer_args: dict = None,
+                           loss: str = 'mean_squared_error',
+                           metrics: str = 'mean_squared_error',
+                           conv_block_one: int = 1,
+                           conv_block_two: int = 1,
+                           bilstm_block_one: int = 1,
+                           lstm_block_one: int = 1,
+                           layer_config =
+                           {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                           }
+                          )
+
+predictor.create_cnnbigru(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          bigru_block_one: int = 1,
+                          gru_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
                         )
-        
-        
-        predictor.show_performance()
-        predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(10))
-        predictor.model_blueprint()
-        ```
-        #### The shell of the seeker harness
-          
-        ```python
-        predictor = OptimizePureMulti(...)
-        
-        @seeker(optimizer_range=[...], 
-                layer_config_range= [
-                    {...},
-                    {...},
-                    {...}
-                ], 
-                optimizer_args_range = [
-                    {...},
-                    {...},
-                ]
-                optimization_target = '...', n_trials = x)
-        def create_fit_model(predictor: object, *args, **kwargs): # seeker harness
-            return predictor.create_fit_xxx(*args, **kwargs)
-        
-        create_fit_model(...) # execute seeker harness
-        
-        
-        predictor.show_performance()
-        predictor.predict(...)
-        predictor.model_blueprint()
-        ```
-        
-        
-        </details>
-        
-        ## References
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Brwonlee, J., 2016. Display deep learning model training history in keras [Online]. Available from:
-        https://machinelearningmastery.com/display-deep-
-        learning-model-training-history-in-keras/.
-        
-        Brwonlee, J., 2018a. How to develop convolutional neural network models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-convolutional-
-        neural-network-models-for-time-series-forecasting/.
-        
-        Brwonlee, J., 2018b. How to develop lstm models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-
-        lstm-models-for-time-series-forecasting/.
-        
-        Brwonlee, J., 2018c. How to develop multilayer perceptron models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-multilayer-
-        perceptron-models-for-time-series-forecasting/.
-        
-        </details>
-        
-        
-        </details>
-Keywords: machinelearning,keras,deeplearning,timeseries,forecasting
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                  )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor =  HybridMulti(sub_seq: int, steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+</details>
+
+## Hyperparameter Optimization imbrium 1.1.0
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Starting from version 1.1.0, imbrium will support experimental hyperparamerter optimization for the model layer config and optimizer arguments. The optimization process uses the Optuna library (https://optuna.org/).
+
+### Optimization via the seeker decorator
+
+To leverage Optimization, use the new classes `OptimizePureUni`, `OptimizeHybridUni`, `OptimizePureMulti` and `OptimizeHybridMulti`. These classes implement optimizable model architecture methods:
+
+`OptimizePureUni` & `OptimizePureMulti`:
+
+  - create_fit_mlp
+  - create_fit_rnn
+  - create_fit_lstm
+  - create_fit_cnn
+  - create_fit_gru
+  - create_fit_birnn
+  - create_fit_bilstm
+  - create_fit_bigru
+  - create_fit_encdec_rnn
+  - create_fit_encdec_lstm
+  - create_fit_encdec_gru
+  - create_fit_encdec_cnn
+
+`OptimizeHybridUni` & `OptimizeHybridMulti`:
+
+  - create_fit_cnnrnn
+  - create_fit_cnnlstm
+  - create_fit_cnngru
+  - create_fit_cnnbirnn
+  - create_fit_cnnbilstm
+  - create_fit_cnnbigru
+
+#### Example `OptimizePureUni`
+
+```python
+from imbrium.predictors.univarpure import OptimizePureUni
+from imbrium.utils.optimization import seeker
+
+# initialize optimizable predictor object
+predictor = OptimizePureUni(steps_past=5, steps_future=10, data=data, scale='standard')
+
+
+# use seeker decorator on optimization harness
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (5, 'relu'),
+              'layer1': (10,'relu'),
+              'layer2': (5, 'relu')
+            },
+            {
+              'layer0': (2, 'relu'),
+              'layer1': (5, 'relu'),
+              'layer2': (2, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 2)
+def create_fit_model(predictor: object, *args, **kwargs):
+    # use optimizable create_fit_xxx method
+    return predictor.create_fit_lstm(*args, **kwargs)
+
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=0,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+predictor.show_performance()
+predictor.predict(data.tail(5))
+predictor.model_blueprint()
+```
+
+#### Example `OptimizeHybridUni`
+
+```python
+from imbrium.predictors.univarhybrid import OptimizeHybridUni
+from imbrium.utils.optimization import seeker
+
+predictor = OptimizeHybridUni(sub_seq = 2, steps_past = 10, steps_future = 5, data = data, scale = 'maxabs')
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (25, 'relu'),
+              'layer4': (10, 'relu')
+            },
+            {
+              'layer0': (16, 1, 'relu'),
+              'layer1': (8, 1, 'relu'),
+              'layer2': (2)
+              'layer3': (55, 'relu'),
+              'layer4': (10, 'relu')
+            },
+            {
+              'layer0': (32, 1, 'relu'),
+              'layer1': (16, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (25, 'relu'),
+              'layer4': (10, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 2)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_cnnlstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=0,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+predictor.show_performance()
+predictor.predict(data.tail(10))
+predictor.model_blueprint()
+```
+
+#### Example `OptimizePureMulti`
+
+```python
+predictor = OptimizePureMulti(
+                              steps_past =  5,
+                              steps_future = 10,
+                              data = data,
+                              features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
+                              scale = 'normalize'
+                            )
+
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (5, 'relu'),
+              'layer1': (10,'relu'),
+              'layer2': (5, 'relu')
+            },
+            {
+              'layer0': (2, 'relu'),
+              'layer1': (5, 'relu'),
+              'layer2': (2, 'relu')
+            },
+            {
+              'layer0': (20, 'relu'),
+              'layer1': (50, 'relu'),
+              'layer2': (20, 'sigmoid')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 3)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_lstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=1, 
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+
+predictor.show_performance()
+predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(5))
+predictor.model_blueprint()
+```
+
+
+#### Example `OptimizeHybridMulti`
+
+```python
+predictor = OptimizeHybridMulti(
+                                sub_seq = 2, 
+                                steps_past = 10,
+                                steps_future = 5,
+                                data = data,
+                                features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
+                                scale = 'normalize'
+                              )
+
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            },
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            },
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 3)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_cnnlstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=1,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+
+predictor.show_performance()
+predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(10))
+predictor.model_blueprint()
+```
+#### The shell of the seeker harness
+  
+```python
+predictor = OptimizePureMulti(...)
+
+@seeker(optimizer_range=[...], 
+        layer_config_range= [
+            {...},
+            {...},
+            {...}
+        ], 
+        optimizer_args_range = [
+            {...},
+            {...},
+        ]
+        optimization_target = '...', n_trials = x)
+def create_fit_model(predictor: object, *args, **kwargs): # seeker harness
+    return predictor.create_fit_xxx(*args, **kwargs)
+
+create_fit_model(...) # execute seeker harness
+
+
+predictor.show_performance()
+predictor.predict(...)
+predictor.model_blueprint()
+```
+
+
+</details>
+
+## References
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Brwonlee, J., 2016. Display deep learning model training history in keras [Online]. Available from:
+https://machinelearningmastery.com/display-deep-
+learning-model-training-history-in-keras/.
+
+Brwonlee, J., 2018a. How to develop convolutional neural network models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-convolutional-
+neural-network-models-for-time-series-forecasting/.
+
+Brwonlee, J., 2018b. How to develop lstm models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-
+lstm-models-for-time-series-forecasting/.
+
+Brwonlee, J., 2018c. How to develop multilayer perceptron models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-multilayer-
+perceptron-models-for-time-series-forecasting/.
+
+</details>
+
+
+</details>
```

### Comparing `imbrium-2.1.0/README.md` & `imbrium-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: imbrium
+Version: 3.0.0
+Summary: Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.
+Home-page: https://github.com/maxmekiska/imbrium
+Author: Maximilian Mekiska
+Author-email: maxmekiska@gmail.com
+License: UNKNOWN
+Keywords: machinelearning,keras,deeplearning,timeseries,forecasting
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # imbrium [![Downloads](https://pepy.tech/badge/imbrium)](https://pepy.tech/project/imbrium) [![PyPi](https://img.shields.io/pypi/v/imbrium.svg?color=blue)](https://pypi.org/project/imbrium/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/Imbrium?color=black)](https://github.com/maxmekiska/Imbrium/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/imbrium.svg)](https://pypi.python.org/project/imbrium/)
  
 ## Status
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -30,25 +48,29 @@
 imbrium is a deep learning library that specializes in time series forecasting. Its primary objective is to provide a user-friendly repository of deep learning architectures for this purpose. The focus is on simplifying the process of creating and applying these architectures, with the goal of allowing users to create complex architectures without having to build them from scratch. Instead, the emphasis shifts to high-level configuration of the architectures.
 
 
 ## imbrium Summary
 
 imbrium is designed to simplify the application of deep learning models for time series forecasting. The library offers a variety of pre-built architectures. The user retains full control over the configuration of each layer, including the number of neurons, the type of activation function, loss function, optimizer, and metrics applied. This allows for the flexibility to adapt the architecture to the specific needs of the forecast task at hand. Imbrium also offers a user-friendly interface for training and evaluating these models, making it easy to quickly iterate and test different configurations.
 
-imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window (steps_past) through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables (steps_future). This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
+imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window - `steps_past` through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables - `steps_future`. This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
 
-## imbrium 2.0.0
+## imbrium `2.0.0`
 
 - adapting `keras_core`
 - removing internal hyperparameter tuning
 - removing encoder-decoder architectures
 - improve layer configuration
 - split input data into target and feature numpy arrays
 - overall lighten the library
 
+## imbrium `3.0.0`
+
+- switch from `keras_core` to `keras > 3.0.0`
+
 ### Get started with imbrium
 
 <details>
   <summary>Expand</summary>
   <br>
 
 <details>
@@ -56,15 +78,15 @@
   <br>
 
 
 ```python
 from imbrium import PureUni
 
 # create a PureUni object (numpy array expected)
-predictor = PureUni(target = target_numpy_array) 
+predictor = PureUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
 
 # the following models are available for a PureUni objects;
 
 # create and fit a muti-layer perceptron model
 predictor.create_fit_mlp( 
         steps_past,
         steps_future,
@@ -94,15 +116,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a recurrent neural network model
 predictor.create_fit_rnn(
         steps_past,
         steps_future,
@@ -132,15 +153,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a long short-term neural network model
 predictor.create_fit_lstm(
         steps_past,
         steps_future,
@@ -170,15 +190,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional neural network
 predictor = create_fit_cnn(
         steps_past,
         steps_future,
@@ -219,15 +238,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a gated recurrent unit neural network  
 predictor.create_fit_gru(
         steps_past,
         steps_future,
@@ -261,15 +279,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional recurrent neural network
 predictor.create_fit_birnn(
         steps_past,
         steps_future,
@@ -294,15 +311,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional long short-term memory neural network
 predictor.create_fit_bilstm(
         steps_past,
         steps_future,
@@ -327,15 +343,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional gated recurrent neural network
 predictor.create_fit_bigru(
         steps_past,
         steps_future,
@@ -360,15 +375,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
 
 # in addition, you can add to all models early stopping arguments:
 
@@ -381,14 +395,20 @@
 restore_best_weights=False,
 start_from_epoch=0
 
 
 # instpect model structure
 predictor.model_blueprint()
 
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
 # insptect keras model performances via (access dictionary via history key):
 predictor.show_performance()
 
 # make predictions via (numpy array expected):
 predictor.predict(data)
 
 # save predictor via:
@@ -405,15 +425,15 @@
   <br>
 
 
 ```python
 from imbrium import PureMulti
 
 # create a PureMulti object (numpy array expected)
-predictor = PureMulti(target = target_numpy_array, features = features_numpy_array) 
+predictor = PureMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
 
 # the following models are available for a PureMulti objects;
 
 # create and fit a muti-layer perceptron model
 predictor.create_fit_mlp( 
         steps_past,
         steps_future,
@@ -443,15 +463,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a recurrent neural network model
 predictor.create_fit_rnn(
         steps_past,
         steps_future,
@@ -481,15 +500,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a long short-term neural network model
 predictor.create_fit_lstm(
         steps_past,
         steps_future,
@@ -519,15 +537,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional neural network
 predictor = create_fit_cnn(
         steps_past,
         steps_future,
@@ -568,15 +585,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a gated recurrent unit neural network  
 predictor.create_fit_gru(
         steps_past,
         steps_future,
@@ -610,15 +626,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional recurrent neural network
 predictor.create_fit_birnn(
         steps_past,
         steps_future,
@@ -643,15 +658,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional long short-term memory neural network
 predictor.create_fit_bilstm(
         steps_past,
         steps_future,
@@ -676,15 +690,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a bidirectional gated recurrent neural network
 predictor.create_fit_bigru(
         steps_past,
         steps_future,
@@ -709,15 +722,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
 
 # in addition, you can add to all models early stopping arguments:
 
@@ -730,14 +742,20 @@
 restore_best_weights=False,
 start_from_epoch=0
 
 
 # instpect model structure
 predictor.model_blueprint()
 
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
 # insptect keras model performances via (access dictionary via history key):
 predictor.show_performance()
 
 # make predictions via (numpy array expected):
 predictor.predict(data)
 
 # save predictor via:
@@ -752,15 +770,15 @@
   <summary>Univariate Hybrid Predictors</summary>
   <br>
 
 ```python
 from imbrium import HybridUni
 
 # create a HybridUni object (numpy array expected)
-predictor = HybridUni(target = target_numpy_array) 
+predictor = HybridUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
 
 # the following models are available for a HybridUni objects:
 # create and fit a convolutional recurrent neural network
 predictor.create_fit_cnnrnn(
         sub_seq,
         steps_past,
         steps_future,
@@ -810,15 +828,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional long short-term memory neural network
 predictor.create_fit_cnnlstm(
         sub_seq,
         steps_past,
@@ -869,15 +886,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional gated recurrent unit neural network  
 predictor.create_fit_cnngru(
         sub_seq,
         steps_past,
@@ -928,15 +944,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional recurrent neural network
 predictor.create_fit_cnnbirnn(
         sub_seq,
         steps_past,
@@ -987,15 +1002,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional long short-term neural network
 predictor.create_fit_cnnbilstm(
         sub_seq,
         steps_past,
@@ -1046,15 +1060,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional gated recurrent neural network
 predictor.create_fit_cnnbigru(
         sub_seq,
         steps_past,
@@ -1105,15 +1118,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
 
 # in addition, you can add to all models early stopping arguments:
 
@@ -1126,14 +1138,20 @@
 restore_best_weights=False,
 start_from_epoch=0
 
 
 # instpect model structure
 predictor.model_blueprint()
 
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
 # insptect keras model performances via (access dictionary via history key):
 predictor.show_performance()
 
 # make predictions via (numpy array expected):
 # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
 predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
 
@@ -1151,15 +1169,15 @@
   <br>
 
 
 ```python
 from imbrium import HybridMulti
 
 # create a HybridMulti object (numpy array expected)
-predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array) 
+predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
 
 # the following models are available for a HybridMulti objects:
 # create and fit a convolutional recurrent neural network
 predictor.create_fit_cnnrnn(
         sub_seq,
         steps_past,
         steps_future,
@@ -1209,15 +1227,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional long short-term memory neural network
 predictor.create_fit_cnnlstm(
         sub_seq,
         steps_past,
@@ -1268,15 +1285,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional gated recurrent unit neural network  
 predictor.create_fit_cnngru(
         sub_seq,
         steps_past,
@@ -1327,15 +1343,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional recurrent neural network
 predictor.create_fit_cnnbirnn(
         sub_seq,
         steps_past,
@@ -1386,15 +1401,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional long short-term neural network
 predictor.create_fit_cnnbilstm(
         sub_seq,
         steps_past,
@@ -1445,15 +1459,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # create and fit a convolutional bidirectional gated recurrent neural network
 predictor.create_fit_cnnbigru(
         sub_seq,
         steps_past,
@@ -1504,15 +1517,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs = 100,
         show_progress = 1,
-        validation_split = 0.20,
         board = False,
 )
 
 # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
 
 # in addition, you can add to all models early stopping arguments:
 
@@ -1525,14 +1537,20 @@
 restore_best_weights=False,
 start_from_epoch=0
 
 
 # instpect model structure
 predictor.model_blueprint()
 
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
 # insptect keras model performances via (access dictionary via history key):
 predictor.show_performance()
 
 # make predictions via (numpy array expected):
 # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
 predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
 
@@ -1551,15 +1569,15 @@
 https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/use-case-1.ipynb
 
 ### Integration tests
 
 https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/IntegrationTest.ipynb
 
 
-## LEGACY: imbrium versions <= v.1.3.0
+## legacy: imbrium versions `<= 1.3.0`
 <details>
   <summary>Expand</summary>
   <br>
 
 The library differentiates between two
 modes:
 
@@ -2769,8 +2787,9 @@
 Brwonlee, J., 2018c. How to develop multilayer perceptron models for time series forecasting [Online]. Available from:
 https://machinelearningmastery.com/how-to-develop-multilayer-
 perceptron-models-for-time-series-forecasting/.
 
 </details>
 
 
-</details>
+</details>
+
```

### Comparing `imbrium-2.1.0/imbrium/architectures/models.py` & `imbrium-3.0.0/imbrium/architectures/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import keras_core
-from keras_core import regularizers
-from keras_core.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
-                               Dropout, Flatten, MaxPooling1D, SimpleRNN,
-                               TimeDistributed)
+import keras
+from keras import regularizers
+from keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense, Dropout,
+                          Flatten, MaxPooling1D, SimpleRNN, TimeDistributed)
 
 
 def mlp(
     optimizer: str,
     loss: str,
     metrics: str,
     dense_block_one: int,
@@ -24,18 +23,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(shape=(input_shape,)))
+    model = keras.Sequential()
+    model.add(keras.Input(shape=(input_shape,)))
     for i in range(dense_block_one):
         model.add(
             Dense(
                 layer_config[f"layer{layer_num}"]["config"]["neurons"],
                 activation=layer_config[f"layer{layer_num}"]["config"]["activation"],
                 kernel_regularizer=regularizers.L2(
                     layer_config[f"layer{layer_num}"]["config"]["regularization"]
@@ -108,18 +107,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(rnn_block_one):
         model.add(
             SimpleRNN(
                 layer_config[f"layer{layer_num}"]["config"]["neurons"],
                 activation=layer_config[f"layer{layer_num}"]["config"]["activation"],
                 return_sequences=True,
                 kernel_regularizer=regularizers.L2(
@@ -195,18 +194,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(lstm_block_one):
         model.add(
             LSTM(
                 layer_config[f"layer{layer_num}"]["config"]["neurons"],
                 activation=layer_config[f"layer{layer_num}"]["config"]["activation"],
                 return_sequences=True,
                 kernel_regularizer=regularizers.L2(
@@ -282,18 +281,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             Conv1D(
                 filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                 kernel_size=layer_config[f"layer{layer_num}"]["config"]["kernel_size"],
                 activation=layer_config[f"layer{layer_num}"]["config"]["activation"],
                 kernel_regularizer=regularizers.L2(
@@ -373,18 +372,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(gru_block_one):
         model.add(
             GRU(
                 layer_config[f"layer{layer_num}"]["config"]["neurons"],
                 activation=layer_config[f"layer{layer_num}"]["config"]["activation"],
                 return_sequences=True,
                 kernel_regularizer=regularizers.L2(
@@ -459,18 +458,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(birnn_block_one):
         model.add(
             Bidirectional(
                 SimpleRNN(
                     layer_config[f"layer{layer_num}"]["config"]["neurons"],
                     activation=layer_config[f"layer{layer_num}"]["config"][
                         "activation"
@@ -536,18 +535,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(bilstm_block_one):
         model.add(
             Bidirectional(
                 LSTM(
                     layer_config[f"layer{layer_num}"]["config"]["neurons"],
                     activation=layer_config[f"layer{layer_num}"]["config"][
                         "activation"
@@ -613,18 +612,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(bigru_block_one):
         model.add(
             Bidirectional(
                 GRU(
                     layer_config[f"layer{layer_num}"]["config"]["neurons"],
                     activation=layer_config[f"layer{layer_num}"]["config"][
                         "activation"
@@ -692,18 +691,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
@@ -814,18 +813,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
@@ -936,18 +935,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
@@ -1058,18 +1057,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
@@ -1184,18 +1183,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
@@ -1310,18 +1309,18 @@
         metrics (str): Performance measurement.
         layer_config (dict): Adjust neurons and activation functions.
         input_shape (tuple): Time series input shape.
         ouput_shape (int): Time series output shape.
     Returns:
         model (object): Returns compiled Keras model.
     """
-    keras_core.backend.clear_session()
+    keras.backend.clear_session()
     layer_num = 0
-    model = keras_core.Sequential()
-    model.add(keras_core.Input(input_shape))
+    model = keras.Sequential()
+    model.add(keras.Input(input_shape))
     for i in range(conv_block_one):
         model.add(
             TimeDistributed(
                 Conv1D(
                     filters=layer_config[f"layer{layer_num}"]["config"]["filters"],
                     kernel_size=layer_config[f"layer{layer_num}"]["config"][
                         "kernel_size"
```

### Comparing `imbrium-2.1.0/imbrium/blueprints/abstract_multivariate.py` & `imbrium-3.0.0/imbrium/blueprints/abstract_univariate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from abc import ABC, abstractmethod
 
 from numpy import array
 
 
-class MultiVariateMultiStep(ABC):
-    """Abstract class that defines the general blueprint of a multivariate
+class UniVariateMultiStep(ABC):
+    """Abstract class that defines the general blueprint of a univariate
     multistep prediction object.
     """
 
     @abstractmethod
-    def __init__(self):
+    def __init__(
+        self,
+        target: array = array([]),
+        features: array = array([]),
+        evaluation_split: float = 0.2,
+        validation_split: float = 0.2,
+    ):
         pass
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         pass
 
     @abstractmethod
     def set_model_id(self, name: str):
@@ -76,29 +82,31 @@
         show_progress: int = 1,
         validation_split: float = 0.20,
         **callback_setting: dict
     ):
         pass
 
     @abstractmethod
+    def evaluate_model(self):
+        pass
+
+    @abstractmethod
     def model_blueprint(self):
         pass
 
     @abstractmethod
     def show_performance(self):
         pass
 
     @abstractmethod
-    def predict(
-        self,
-        data: array,
-        sub_seq: int = None,
-        steps_past: int = None,
-        steps_future: int = None,
-    ) -> array:
+    def show_evaluation(self):
+        pass
+
+    @abstractmethod
+    def predict(self, data: array) -> array:
         pass
 
     @abstractmethod
     def freeze(self, absolute_path: str):
         pass
 
     @abstractmethod
```

### Comparing `imbrium-2.1.0/imbrium/blueprints/abstract_univariate.py` & `imbrium-3.0.0/imbrium/blueprints/abstract_multivariate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from abc import ABC, abstractmethod
 
 from numpy import array
 
 
-class UniVariateMultiStep(ABC):
-    """Abstract class that defines the general blueprint of a univariate
+class MultiVariateMultiStep(ABC):
+    """Abstract class that defines the general blueprint of a multivariate
     multistep prediction object.
     """
 
     @abstractmethod
-    def __init__(self):
+    def __init__(
+        self,
+        target: array = array([]),
+        features: array = array([]),
+        evaluation_split: float = 0.2,
+        validation_split: float = 0.2,
+    ):
         pass
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         pass
 
     @abstractmethod
     def set_model_id(self, name: str):
@@ -76,23 +82,37 @@
         show_progress: int = 1,
         validation_split: float = 0.20,
         **callback_setting: dict
     ):
         pass
 
     @abstractmethod
+    def evaluate_model(self):
+        pass
+
+    @abstractmethod
     def model_blueprint(self):
         pass
 
     @abstractmethod
     def show_performance(self):
         pass
 
     @abstractmethod
-    def predict(self, data: array) -> array:
+    def show_evaluation(self):
+        pass
+
+    @abstractmethod
+    def predict(
+        self,
+        data: array,
+        sub_seq: int = None,
+        steps_past: int = None,
+        steps_future: int = None,
+    ) -> array:
         pass
 
     @abstractmethod
     def freeze(self, absolute_path: str):
         pass
 
     @abstractmethod
```

### Comparing `imbrium-2.1.0/imbrium/predictors/multivarhybrid.py` & `imbrium-3.0.0/imbrium/predictors/multivarhybrid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import datetime
 import os
 
-from keras_core.callbacks import EarlyStopping, TensorBoard
-from keras_core.saving import load_model
+from keras.callbacks import EarlyStopping, TensorBoard
+from keras.saving import load_model
 from numpy import array
 
 from imbrium.architectures.models import (cnnbigru, cnnbilstm, cnnbirnn,
                                           cnngru, cnnlstm, cnnrnn)
 from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
-from imbrium.utils.transformer import data_prep_multi, multistep_prep_hybrid
+from imbrium.utils.transformer import (data_prep_multi, multistep_prep_hybrid,
+                                       train_test_split)
 
 
 class BaseHybridMulti(MultiVariateMultiStep):
     """Implements neural network based multivariate multipstep hybrid predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
         target: array = array([]),
         features: array = array([]),
+        evaluation_split: float = 0.20,
+        validation_split: float = 0.20,
     ) -> object:
         """
         Parameters:
             target (array): Input target array.
             features (array): Input feature array.
+            evaluation_split (float): train test split.
+            validation_split (float): validation size of train set.
         """
         self.target = target
         self.features = features
+        self.evaluation_split = evaluation_split
+        self.validation_split = validation_split
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
         self.model_id = ""
 
     def _model_intake_prep(
@@ -42,14 +49,20 @@
         self.steps_past = steps_past
         self.sub_seq = sub_seq
         if len(self.target) > 0:
             temp_data = data_prep_multi(self.target, self.features)
             self.input_x, self.input_y, self.modified_back = multistep_prep_hybrid(
                 temp_data, sub_seq, steps_past, steps_future
             )
+            self.input_x, self.input_x_test = train_test_split(
+                self.input_x, test_size=self.evaluation_split
+            )
+            self.input_y, self.input_y_test = train_test_split(
+                self.input_y, test_size=self.evaluation_split
+            )
         else:
             pass
 
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
@@ -676,88 +689,101 @@
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
-            validation_split (float): Determines size of Validation data.
             board (bool): Creates TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
+                    shuffle=False,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
+                    shuffle=False,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
+                    shuffle=False,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
+                    shuffle=False,
                 )
         return self.details
 
+    def evaluate_model(self):
+        self.evaluation_details = self.model.evaluate(
+            x=self.input_x_test, y=self.input_y_test
+        )
+
+        return self.evaluation_details
+
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
     def show_performance(self):
         """Returns performance details."""
         return self.details
 
+    def show_evaluation(self):
+        """Returns performance details on test data."""
+        return self.evaluation_details
+
     def predict(
         self,
         data: array,
         sub_seq: int = None,
         steps_past: int = None,
         steps_future: int = None,
     ) -> array:
@@ -850,15 +876,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -872,15 +897,14 @@
             rnn_block_one=rnn_block_one,
             rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
@@ -933,15 +957,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -955,15 +978,14 @@
             lstm_block_one=lstm_block_one,
             lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
@@ -1016,15 +1038,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1038,15 +1059,14 @@
             gru_block_one=gru_block_one,
             gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
@@ -1099,15 +1119,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1121,15 +1140,14 @@
             birnn_block_one=birnn_block_one,
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
@@ -1182,15 +1200,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1204,15 +1221,14 @@
             bilstm_block_one=bilstm_block_one,
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
@@ -1265,15 +1281,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1287,15 +1302,14 @@
             bigru_block_one=bigru_block_one,
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["HybridMulti"]
```

### Comparing `imbrium-2.1.0/imbrium/predictors/multivarpure.py` & `imbrium-3.0.0/imbrium/predictors/multivarpure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,65 @@
 import datetime
 import os
 
-from keras_core.callbacks import EarlyStopping, TensorBoard
-from keras_core.saving import load_model
+from keras.callbacks import EarlyStopping, TensorBoard
+from keras.saving import load_model
 from numpy import array
 
 from imbrium.architectures.models import (bigru, bilstm, birnn, cnn, gru, lstm,
                                           mlp, rnn)
 from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
-from imbrium.utils.transformer import data_prep_multi, multistep_prep_standard
+from imbrium.utils.transformer import (data_prep_multi,
+                                       multistep_prep_standard,
+                                       train_test_split)
 
 
 class BasePureMulti(MultiVariateMultiStep):
     """Implements deep neural networks based on multivariate multipstep
     standard predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
         target: array = array([]),
         features: array = array([]),
+        evaluation_split: float = 0.20,
+        validation_split: float = 0.20,
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
             features (array): Input feature data numpy array.
+            evaluation_split (float): train test split.
+            validation_split (float): validation size of train set.
         """
         self.target = target
         self.features = features
+        self.evaluation_split = evaluation_split
+        self.validation_split = validation_split
         self.model_id = ""
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         """Private method that prepares feature and label data arrays for model intake."""
         if len(self.target) > 0:
             temp_data = data_prep_multi(self.target, self.features)
             self.input_x, self.input_y = multistep_prep_standard(
                 temp_data, steps_past, steps_future
             )
+            self.input_x, self.input_x_test = train_test_split(
+                self.input_x, test_size=self.evaluation_split
+            )
+            self.input_y, self.input_y_test = train_test_split(
+                self.input_y, test_size=self.evaluation_split
+            )
         else:
             pass
 
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
@@ -157,14 +171,20 @@
 
         optimizer_obj = get_optimizer(optimizer, optimizer_args)
 
         self.dimension = self.input_x.shape[1] * self.input_x.shape[2]
 
         self.input_x = self.input_x.reshape((self.input_x.shape[0], self.dimension))
 
+        self.dimension_test = self.input_x_test.shape[1] * self.input_x_test.shape[2]
+
+        self.input_x_test = self.input_x_test.reshape(
+            (self.input_x_test.shape[0], self.dimension_test)
+        )
+
         self.model = mlp(
             optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
             dense_block_one=dense_block_one,
             dense_block_two=dense_block_two,
             dense_block_three=dense_block_three,
@@ -636,88 +656,101 @@
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
-            validation_split (float): Determines size of Validation data.
             board (bool): Create TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
+                    shuffle=False,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
+                    shuffle=False,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
+                    shuffle=False,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
+                    shuffle=False,
                 )
         return self.details
 
+    def evaluate_model(self):
+        self.evaluation_details = self.model.evaluate(
+            x=self.input_x_test, y=self.input_y_test
+        )
+
+        return self.evaluation_details
+
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
     def show_performance(self):
         """Returns performance details."""
         return self.details
 
+    def show_evaluation(self):
+        """Returns performance details on test data."""
+        return self.evaluation_details
+
     def predict(self, data: array) -> array:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
@@ -782,15 +815,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -802,15 +834,14 @@
             dense_block_two=dense_block_two,
             dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
@@ -842,15 +873,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a RNN model."""
         self.create_rnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -862,15 +892,14 @@
             rnn_block_two=rnn_block_two,
             rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
@@ -902,15 +931,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -922,15 +950,14 @@
             lstm_block_two=lstm_block_two,
             lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
@@ -973,15 +1000,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a CNN model."""
         self.create_cnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -993,15 +1019,14 @@
             conv_block_two=conv_block_two,
             dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
@@ -1037,15 +1062,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1057,15 +1081,14 @@
             gru_block_two=gru_block_two,
             gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
@@ -1092,15 +1115,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-RNN model."""
         self.create_birnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1111,15 +1133,14 @@
             birnn_block_one=birnn_block_one,
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
@@ -1146,15 +1167,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-LSTM model."""
         self.create_bilstm(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1165,15 +1185,14 @@
             bilstm_block_one=bilstm_block_one,
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
@@ -1200,15 +1219,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a BI-GRU model."""
         self.create_bigru(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1219,15 +1237,14 @@
             bigru_block_one=bigru_block_one,
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["PureMulti"]
```

### Comparing `imbrium-2.1.0/imbrium/predictors/univarhybrid.py` & `imbrium-3.0.0/imbrium/predictors/univarhybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import datetime
 import os
 
-from keras_core.callbacks import EarlyStopping, TensorBoard
-from keras_core.saving import load_model
+from keras.callbacks import EarlyStopping, TensorBoard
+from keras.saving import load_model
 from numpy import array
 
 from imbrium.architectures.models import (cnnbigru, cnnbilstm, cnnbirnn,
                                           cnngru, cnnlstm, cnnrnn)
 from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
-from imbrium.utils.transformer import data_prep_uni, sequence_prep_hybrid_uni
+from imbrium.utils.transformer import (data_prep_uni, sequence_prep_hybrid_uni,
+                                       train_test_split)
 
 
 class BaseHybridUni(UniVariateMultiStep):
     """Implements neural network based univariate multipstep hybrid predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
         target=array([]),
+        evaluation_split: float = 0.20,
+        validation_split: float = 0.20,
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
+            evaluation_split (float): train test split.
+            validation_split (float): validation size of train set.
         """
         self.target = target
+        self.evaluation_split = evaluation_split
+        self.validation_split = validation_split
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
         self.model_id = ""
 
     def _model_intake_prep(
         self, sub_seq: int, steps_past: int, steps_future: int
@@ -38,14 +45,20 @@
         self.steps_past = steps_past
         self.sub_seq = sub_seq
         if len(self.target) > 0:
             temp_data = data_prep_uni(self.target)
             self.input_x, self.input_y, self.modified_back = sequence_prep_hybrid_uni(
                 temp_data, sub_seq, steps_past, steps_future
             )
+            self.input_x, self.input_x_test = train_test_split(
+                self.input_x, test_size=self.evaluation_split
+            )
+            self.input_y, self.input_y_test = train_test_split(
+                self.input_y, test_size=self.evaluation_split
+            )
         else:
             pass
 
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
@@ -648,88 +661,101 @@
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
-            validation_split (float): Determines size of Validation data.
             board (bool): Create TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
+                    shuffle=False,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
+                    shuffle=False,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
+                    shuffle=False,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
+                    shuffle=False,
                 )
         return self.details
 
+    def evaluate_model(self):
+        self.evaluation_details = self.model.evaluate(
+            x=self.input_x_test, y=self.input_y_test
+        )
+
+        return self.evaluation_details
+
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
     def show_performance(self):
         """Returns performance details."""
         return self.details
 
+    def show_evaluation(self):
+        """Returns performance details on test data."""
+        return self.evaluation_details
+
     def predict(
         self, data: array, sub_seq: int = None, steps_past=None, steps_future=None
     ) -> array:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
@@ -820,15 +846,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -842,15 +867,14 @@
             rnn_block_one=rnn_block_one,
             rnn_block_two=rnn_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
@@ -903,15 +927,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -925,15 +948,14 @@
             lstm_block_one=lstm_block_one,
             lstm_block_two=lstm_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
@@ -986,15 +1008,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1008,15 +1029,14 @@
             gru_block_one=gru_block_one,
             gru_block_two=gru_block_two,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
@@ -1069,15 +1089,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1091,15 +1110,14 @@
             birnn_block_one=birnn_block_one,
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
@@ -1152,15 +1170,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1174,15 +1191,14 @@
             bilstm_block_one=bilstm_block_one,
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
@@ -1235,15 +1251,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             sub_seq=sub_seq,
             steps_past=steps_past,
@@ -1257,15 +1272,14 @@
             bigru_block_one=bigru_block_one,
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["HybridUni"]
```

### Comparing `imbrium-2.1.0/imbrium/predictors/univarpure.py` & `imbrium-3.0.0/imbrium/predictors/univarpure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,62 @@
 import datetime
 import os
+from typing import Tuple
 
-from keras_core.callbacks import EarlyStopping, TensorBoard
-from keras_core.saving import load_model
+from keras.callbacks import EarlyStopping, TensorBoard
+from keras.saving import load_model
 from numpy import array
 
 from imbrium.architectures.models import (bigru, bilstm, birnn, cnn, gru, lstm,
                                           mlp, rnn)
 from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
 from imbrium.utils.optimizer import get_optimizer
-from imbrium.utils.transformer import data_prep_uni, sequence_prep_standard_uni
+from imbrium.utils.transformer import (data_prep_uni,
+                                       sequence_prep_standard_uni,
+                                       train_test_split)
 
 
 class BasePureUni(UniVariateMultiStep):
     """Implements neural network based univariate multipstep predictors."""
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
         target: array = array([]),
+        evaluation_split: float = 0.20,
+        validation_split: float = 0.20,
     ) -> object:
         """
         Parameters:
             target (array): Input target data numpy array.
+            evaluation_split (float): train test split.
+            validation_split (float): validation size of train set.
         """
         self.target = target
+        self.evaluation_split = evaluation_split
+        self.validation_split = validation_split
         self.model_id = ""
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
     def _model_intake_prep(self, steps_past: int, steps_future: int) -> None:
         """Private method that prepares feature and label data arrays for model intake."""
         if len(self.target) > 0:
             temp_data = data_prep_uni(self.target)
             self.input_x, self.input_y = sequence_prep_standard_uni(
                 temp_data, steps_past, steps_future
             )
+            self.input_x, self.input_x_test = train_test_split(
+                self.input_x, test_size=self.evaluation_split
+            )
+            self.input_y, self.input_y_test = train_test_split(
+                self.input_y, test_size=self.evaluation_split
+            )
         else:
             pass
 
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
@@ -151,14 +166,18 @@
 
         self._model_intake_prep(steps_past, steps_future)
 
         self.input_x = self.input_x.reshape(
             (self.input_x.shape[0], self.input_x.shape[1])
         )
 
+        self.input_x_test = self.input_x_test.reshape(
+            (self.input_x_test.shape[0], self.input_x_test.shape[1])
+        )
+
         optimizer_obj = get_optimizer(optimizer, optimizer_args)
 
         self.model = mlp(
             optimizer=optimizer_obj,
             loss=loss,
             metrics=metrics,
             dense_block_one=dense_block_one,
@@ -632,88 +651,101 @@
             output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
-            validation_split (float): Determines size of Validation data.
             board (bool): Creates TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback_board],
+                    shuffle=False,
                 )
             else:
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
+                    shuffle=False,
                 )
 
         else:
             if board == True:
                 callback_board = TensorBoard(
                     log_dir="logs/fit/"
                     + self.model_id
                     + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
                     histogram_freq=1,
                 )
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback, callback_board],
+                    shuffle=False,
                 )
             else:
                 callback = EarlyStopping(**callback_setting)
                 self.details = self.model.fit(
                     self.input_x,
                     self.input_y,
-                    validation_split=validation_split,
+                    validation_split=self.validation_split,
                     epochs=epochs,
                     verbose=show_progress,
                     callbacks=[callback],
+                    shuffle=False,
                 )
         return self.details
 
+    def evaluate_model(self):
+        self.evaluation_details = self.model.evaluate(
+            x=self.input_x_test, y=self.input_y_test
+        )
+
+        return self.evaluation_details
+
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
     def show_performance(self):
         """Returns performance details."""
         return self.details
 
+    def show_evaluation(self):
+        """Returns performance details on test data."""
+        return self.evaluation_details
+
     def predict(self, data: array) -> array:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (array): Forecast for sequence provided.
         """
@@ -779,15 +811,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -799,15 +830,14 @@
             dense_block_two=dense_block_two,
             dense_block_three=dense_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
@@ -839,15 +869,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Recurrent Neural Network model."""
         self.create_rnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -859,15 +888,14 @@
             rnn_block_two=rnn_block_two,
             rnn_block_three=rnn_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
@@ -899,15 +927,14 @@
             },
             "layer2": {
                 "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -919,15 +946,14 @@
             lstm_block_two=lstm_block_two,
             lstm_block_three=lstm_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
@@ -970,15 +996,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Convolutional Neural Network model."""
         self.create_cnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -990,15 +1015,14 @@
             conv_block_two=conv_block_two,
             dense_block_one=dense_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
@@ -1034,15 +1058,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1054,15 +1077,14 @@
             gru_block_two=gru_block_two,
             gru_block_three=gru_block_three,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
@@ -1089,15 +1111,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional RNN model."""
         self.create_birnn(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1108,15 +1129,14 @@
             birnn_block_one=birnn_block_one,
             rnn_block_one=rnn_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
@@ -1143,15 +1163,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional LSTM model."""
         self.create_bilstm(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1162,15 +1181,14 @@
             bilstm_block_one=bilstm_block_one,
             lstm_block_one=lstm_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
@@ -1197,15 +1215,14 @@
                     "activation": "relu",
                     "regularization": 0.0,
                 }
             },
         },
         epochs: int = 100,
         show_progress: int = 1,
-        validation_split: float = 0.20,
         board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional GRU model."""
         self.create_bigru(
             steps_past=steps_past,
             steps_future=steps_future,
@@ -1216,15 +1233,14 @@
             bigru_block_one=bigru_block_one,
             gru_block_one=gru_block_one,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
-            validation_split=validation_split,
             board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
 
 __all__ = ["PureUni"]
```

### Comparing `imbrium-2.1.0/imbrium/utils/optimizer.py` & `imbrium-3.0.0/imbrium/utils/optimizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import keras_core
+import keras
 
 
-def get_optimizer(
-    optimizer: str, optimizer_args: dict
-) -> keras_core.optimizers.Optimizer:
+def get_optimizer(optimizer: str, optimizer_args: dict) -> keras.optimizers.Optimizer:
     """Get optimizer object from string name and arguments."""
     optimizer_dict = {
-        "adadelta": keras_core.optimizers.Adadelta,
-        "adagrad": keras_core.optimizers.Adagrad,
-        "adam": keras_core.optimizers.Adam,
-        "adamax": keras_core.optimizers.Adamax,
-        "ftrl": keras_core.optimizers.Ftrl,
-        "nadam": keras_core.optimizers.Nadam,
-        "rmsprop": keras_core.optimizers.RMSprop,
-        "sgd": keras_core.optimizers.SGD,
+        "adadelta": keras.optimizers.Adadelta,
+        "adagrad": keras.optimizers.Adagrad,
+        "adam": keras.optimizers.Adam,
+        "adamax": keras.optimizers.Adamax,
+        "ftrl": keras.optimizers.Ftrl,
+        "nadam": keras.optimizers.Nadam,
+        "rmsprop": keras.optimizers.RMSprop,
+        "sgd": keras.optimizers.SGD,
     }
 
     if optimizer_args is None:
         optimizer_obj = optimizer
     else:
         optimizer_obj = optimizer_dict.get(optimizer)(**optimizer_args)
```

### Comparing `imbrium-2.1.0/imbrium/utils/transformer.py` & `imbrium-3.0.0/imbrium/utils/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from numpy import array, dstack, empty, reshape, vstack
+from typing import Tuple
+
+from numpy import array, dstack, empty, vstack
 
 
 def data_prep_uni(data: array) -> array:
     """Prepares data for model intake.
     Parameters:
         data (array): Input time series.
     Returns:
@@ -256,7 +258,26 @@
         x, _, mod = sequence_prep_hybrid_multi(
             input_sequence[i], sub_seq, steps_past, steps_future
         )
         X.append(x)
     X = dstack(X)
     Y = Y[0]  # getting array out of list
     return X, Y, mod
+
+
+def train_test_split(data: array, test_size=0.2) -> Tuple[array, array]:
+    """Splits the time series data into training and testing sets.
+    Parameters:
+        data (array): Sequence that contains time series
+        in array format
+        test_size (float): % of original data used as test dataset
+    Returns:
+        train_data (array): Array containing train data
+        test_data  (array): Array containing test data
+    """
+    n_samples = len(data)
+    n_test = int(test_size * n_samples)
+
+    train_data = data[:-n_test]
+    test_data = data[-n_test:]
+
+    return train_data, test_data
```

### Comparing `imbrium-2.1.0/imbrium.egg-info/PKG-INFO` & `imbrium-3.0.0/imbrium.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,2793 +1,2795 @@
 Metadata-Version: 2.1
 Name: imbrium
-Version: 2.1.0
+Version: 3.0.0
 Summary: Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.
 Home-page: https://github.com/maxmekiska/imbrium
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 License: UNKNOWN
-Description: # imbrium [![Downloads](https://pepy.tech/badge/imbrium)](https://pepy.tech/project/imbrium) [![PyPi](https://img.shields.io/pypi/v/imbrium.svg?color=blue)](https://pypi.org/project/imbrium/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/Imbrium?color=black)](https://github.com/maxmekiska/Imbrium/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/imbrium.svg)](https://pypi.python.org/project/imbrium/)
-         
-        ## Status
-        
-        | Build | Status|
-        |---|---|
-        | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=main) |
-        |  `DEV BUILD`   |  ![development](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=development) |
-        
-        ## Pip install
-        
-        ```shell
-        pip install imbrium
-        ```
-        
-        Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step
-        Time Series Forecasting.
-        
-        
-                                  ██╗███╗░░░███╗██████╗░██████╗░██╗██╗░░░██╗███╗░░░███╗
-                                    ║████╗░████║██╔══██╗██╔══██╗██║██║░░░██║████╗░████║
-                                  ██║██╔████╔██║██████╦╝██████╔╝██║██║░░░██║██╔████╔██║
-                                  ██║██║╚██╔╝██║██╔══██╗██╔══██╗██║██║░░░██║██║╚██╔╝██║
-                                  ██║██║░╚═╝░██║██████╦╝██║░░██║██║╚██████╔╝██║░╚═╝░██║
-                                  ╚═╝╚═╝░░░░░╚═╝╚═════╝░╚═╝░░╚═╝╚═╝░╚═════╝░╚═╝░░░░░╚═╝
-        
-        
-        ## Introduction to imbrium
-        
-        imbrium is a deep learning library that specializes in time series forecasting. Its primary objective is to provide a user-friendly repository of deep learning architectures for this purpose. The focus is on simplifying the process of creating and applying these architectures, with the goal of allowing users to create complex architectures without having to build them from scratch. Instead, the emphasis shifts to high-level configuration of the architectures.
-        
-        
-        ## imbrium Summary
-        
-        imbrium is designed to simplify the application of deep learning models for time series forecasting. The library offers a variety of pre-built architectures. The user retains full control over the configuration of each layer, including the number of neurons, the type of activation function, loss function, optimizer, and metrics applied. This allows for the flexibility to adapt the architecture to the specific needs of the forecast task at hand. Imbrium also offers a user-friendly interface for training and evaluating these models, making it easy to quickly iterate and test different configurations.
-        
-        imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window (steps_past) through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables (steps_future). This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
-        
-        ## imbrium 2.0.0
-        
-        - adapting `keras_core`
-        - removing internal hyperparameter tuning
-        - removing encoder-decoder architectures
-        - improve layer configuration
-        - split input data into target and feature numpy arrays
-        - overall lighten the library
-        
-        ### Get started with imbrium
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        <details>
-          <summary>Univariate Pure Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import PureUni
-        
-        # create a PureUni object (numpy array expected)
-        predictor = PureUni(target = target_numpy_array) 
-        
-        # the following models are available for a PureUni objects;
-        
-        # create and fit a muti-layer perceptron model
-        predictor.create_fit_mlp( 
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                dense_block_one = 1,
-                dense_block_two = 1,
-                dense_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a recurrent neural network model
-        predictor.create_fit_rnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                rnn_block_three = 1,
-                metrics = "mean_squared_error",
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a long short-term neural network model
-        predictor.create_fit_lstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                lstm_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional neural network
-        predictor = create_fit_cnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                dense_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a gated recurrent unit neural network  
-        predictor.create_fit_gru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                gru_block_one = 1,
-                gru_block_two = 1,
-                gru_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional recurrent neural network
-        predictor.create_fit_birnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional long short-term memory neural network
-        predictor.create_fit_bilstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional gated recurrent neural network
-        predictor.create_fit_bigru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        predictor.predict(data)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        
-        </details>
-        
-        <details>
-          <summary>Multivariate Pure Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import PureMulti
-        
-        # create a PureMulti object (numpy array expected)
-        predictor = PureMulti(target = target_numpy_array, features = features_numpy_array) 
-        
-        # the following models are available for a PureMulti objects;
-        
-        # create and fit a muti-layer perceptron model
-        predictor.create_fit_mlp( 
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                dense_block_one = 1,
-                dense_block_two = 1,
-                dense_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a recurrent neural network model
-        predictor.create_fit_rnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                rnn_block_three = 1,
-                metrics = "mean_squared_error",
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a long short-term neural network model
-        predictor.create_fit_lstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                lstm_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional neural network
-        predictor = create_fit_cnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                dense_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a gated recurrent unit neural network  
-        predictor.create_fit_gru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                gru_block_one = 1,
-                gru_block_two = 1,
-                gru_block_three = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional recurrent neural network
-        predictor.create_fit_birnn(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional long short-term memory neural network
-        predictor.create_fit_bilstm(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a bidirectional gated recurrent neural network
-        predictor.create_fit_bigru(
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "neurons": 50,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        predictor.predict(data)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        </details>
-        
-        <details>
-          <summary>Univariate Hybrid Predictors</summary>
-          <br>
-        
-        ```python
-        from imbrium import HybridUni
-        
-        # create a HybridUni object (numpy array expected)
-        predictor = HybridUni(target = target_numpy_array) 
-        
-        # the following models are available for a HybridUni objects:
-        # create and fit a convolutional recurrent neural network
-        predictor.create_fit_cnnrnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional long short-term memory neural network
-        predictor.create_fit_cnnlstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional gated recurrent unit neural network  
-        predictor.create_fit_cnngru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                gru_block_one = 1,
-                gru_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional recurrent neural network
-        predictor.create_fit_cnnbirnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional long short-term neural network
-        predictor.create_fit_cnnbilstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional gated recurrent neural network
-        predictor.create_fit_cnnbigru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
-        predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        
-        </details>
-        
-        <details>
-          <summary>Multivariate Hybrid Predictors</summary>
-          <br>
-        
-        
-        ```python
-        from imbrium import HybridMulti
-        
-        # create a HybridMulti object (numpy array expected)
-        predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array) 
-        
-        # the following models are available for a HybridMulti objects:
-        # create and fit a convolutional recurrent neural network
-        predictor.create_fit_cnnrnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                rnn_block_one = 1,
-                rnn_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional long short-term memory neural network
-        predictor.create_fit_cnnlstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                lstm_block_one = 1,
-                lstm_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional gated recurrent unit neural network  
-        predictor.create_fit_cnngru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                gru_block_one = 1,
-                gru_block_two = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional recurrent neural network
-        predictor.create_fit_cnnbirnn(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                birnn_block_one = 1,
-                rnn_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional long short-term neural network
-        predictor.create_fit_cnnbilstm(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bilstm_block_one = 1,
-                lstm_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # create and fit a convolutional bidirectional gated recurrent neural network
-        predictor.create_fit_cnnbigru(
-                sub_seq,
-                steps_past,
-                steps_future,
-                optimizer = "adam",
-                optimizer_args = None,
-                loss = "mean_squared_error",
-                metrics = "mean_squared_error",
-                conv_block_one = 1,
-                conv_block_two = 1,
-                bigru_block_one = 1,
-                gru_block_one = 1,
-                layer_config = {
-                    "layer0": {
-                        "config": {
-                            "filters": 64,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer1": {
-                        "config": {
-                            "filters": 32,
-                            "kernel_size": 1,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer2": {
-                        "config": {
-                            "pool_size": 2,
-                        }
-                    },
-                    "layer3": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                            "dropout": 0.0,
-                        }
-                    },
-                    "layer4": {
-                        "config": {
-                            "neurons": 32,
-                            "activation": "relu",
-                            "regularization": 0.0,
-                        }
-                    },
-                },
-                epochs = 100,
-                show_progress = 1,
-                validation_split = 0.20,
-                board = False,
-        )
-        
-        # you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
-        
-        # in addition, you can add to all models early stopping arguments:
-        
-        monitor='val_loss',
-        min_delta=0,
-        patience=0,
-        verbose=0,
-        mode='auto',
-        baseline=None,
-        restore_best_weights=False,
-        start_from_epoch=0
-        
-        
-        # instpect model structure
-        predictor.model_blueprint()
-        
-        # insptect keras model performances via (access dictionary via history key):
-        predictor.show_performance()
-        
-        # make predictions via (numpy array expected):
-        # - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
-        predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
-        
-        # save predictor via:
-        predictor.freeze(absolute_path)
-        
-        # load saved predictor via:
-        predictor.retrieve(location)
-        ```  
-        </details>
-        
-        </details>
-        
-        ### Use Case: scaling + hyper parameter optimization
-        
-        https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/use-case-1.ipynb
-        
-        ### Integration tests
-        
-        https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/IntegrationTest.ipynb
-        
-        
-        ## LEGACY: imbrium versions <= v.1.3.0
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        The library differentiates between two
-        modes:
-        
-        1. Univariate-Multistep forecasting
-        2. Multivariate-Multistep forecasting
-        
-        These two main modes are further divided based on the complexity of the underlying model architectures:
-        
-        1. Pure
-        2. Hybrid
-        
-        Pure supports the following architectures:
-        
-        - Multilayer perceptron (MLP)
-        - Recurrent neural network (RNN)
-        - Long short-term memory (LSTM)
-        - Gated recurrent unit (GRU)
-        - Convolutional neural network (CNN)
-        - Bidirectional recurrent neural network (BI-RNN)
-        - Bidirectional long-short term memory (BI-LSTM)
-        - Bidirectional gated recurrent unit (BI-GRU)
-        - Encoder-Decoder recurrent neural network
-        - Encoder-Decoder long-short term memory
-        - Encoder-Decoder convolutional neural network (Encoding via CNN, Decoding via GRU)
-        - Encoder-Decoder gated recurrent unit
-        
-        Hybrid supports:
-        
-        - Convolutional neural network + recurrent neural network (CNN-RNN)
-        - Convolutional neural network + Long short-term memory (CNN-LSTM)
-        - Convolutional neural network + Gated recurrent unit (CNN-GRU)
-        - Convolutional neural network + Bidirectional recurrent neural network (CNN-BI-RNN)
-        - Convolutional neural network + Bidirectional long-short term memory (CNN-BI-LSTM)
-        - Convolutional neural network + Bidirectional gated recurrent unit (CNN-BI-GRU)
-        
-        Please note that each model is supported by a prior input data pre-processing procedure which allows to set a look-back period, look-forward period, sub-sequences division (only for hybrid architectures) and data scaling method.
-        
-        The following scikit-learn scaling procedures are supported:
-        
-        - StandardScaler
-        - MinMaxScaler
-        - MaxAbsScaler
-        - Normalizing ([0, 1])
-        - None (raw data input)
-        
-        During training/fitting, callback conditions can be defined to guard against
-        overfitting.
-        
-        Trained models can furthermore be saved or loaded if the user wishes to do so.
-        
-        ## How to use imbrium?
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Attention: Typing has been left in the below examples to ease the configuration readability.
-        
-        #### Version updates:
-        
-        ##### Version >= 1.2.0
-        
-        Version 1.2.0 started supporting tensor board dashboards: https://www.tensorflow.org/tensorboard/get_started
-        
-        ##### Version >= 1.3.0
-        
-        Version 1.3.0 started supporting adjustable layer depth configurations for all architectures. If you wish to adjust the layer depth, please make sure to include a custom layer_config accounting for the correct number of layers. The last layer cannot contain a dropout parameter -> tuple needs to be of length 3: (neurons, activation, regularization).
-        
-        ### `Univariate Models`:
-        
-        1. Univariate-Multistep forecasting - Pure architectures
-        
-        ```python
-        from imbrium.predictors.univarpure import PureUni
-        
-        predictor = PureUni(
-                            steps_past: int,
-                            steps_future: int,
-                            data = pd.DataFrame(),
-                            scale: str = ''
+Keywords: machinelearning,keras,deeplearning,timeseries,forecasting
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# imbrium [![Downloads](https://pepy.tech/badge/imbrium)](https://pepy.tech/project/imbrium) [![PyPi](https://img.shields.io/pypi/v/imbrium.svg?color=blue)](https://pypi.org/project/imbrium/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/Imbrium?color=black)](https://github.com/maxmekiska/Imbrium/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/imbrium.svg)](https://pypi.python.org/project/imbrium/)
+ 
+## Status
+
+| Build | Status|
+|---|---|
+| `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=main) |
+|  `DEV BUILD`   |  ![development](https://github.com/maxmekiska/imbrium/actions/workflows/main.yml/badge.svg?branch=development) |
+
+## Pip install
+
+```shell
+pip install imbrium
+```
+
+Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step
+Time Series Forecasting.
+
+
+                          ██╗███╗░░░███╗██████╗░██████╗░██╗██╗░░░██╗███╗░░░███╗
+                            ║████╗░████║██╔══██╗██╔══██╗██║██║░░░██║████╗░████║
+                          ██║██╔████╔██║██████╦╝██████╔╝██║██║░░░██║██╔████╔██║
+                          ██║██║╚██╔╝██║██╔══██╗██╔══██╗██║██║░░░██║██║╚██╔╝██║
+                          ██║██║░╚═╝░██║██████╦╝██║░░██║██║╚██████╔╝██║░╚═╝░██║
+                          ╚═╝╚═╝░░░░░╚═╝╚═════╝░╚═╝░░╚═╝╚═╝░╚═════╝░╚═╝░░░░░╚═╝
+
+
+## Introduction to imbrium
+
+imbrium is a deep learning library that specializes in time series forecasting. Its primary objective is to provide a user-friendly repository of deep learning architectures for this purpose. The focus is on simplifying the process of creating and applying these architectures, with the goal of allowing users to create complex architectures without having to build them from scratch. Instead, the emphasis shifts to high-level configuration of the architectures.
+
+
+## imbrium Summary
+
+imbrium is designed to simplify the application of deep learning models for time series forecasting. The library offers a variety of pre-built architectures. The user retains full control over the configuration of each layer, including the number of neurons, the type of activation function, loss function, optimizer, and metrics applied. This allows for the flexibility to adapt the architecture to the specific needs of the forecast task at hand. Imbrium also offers a user-friendly interface for training and evaluating these models, making it easy to quickly iterate and test different configurations.
+
+imbrium uses the sliding window approach to generate forecasts. The sliding window approach in time series forecasting involves moving a fixed-size window - `steps_past` through historical data, using the data within the window as input features. The next data points outside the window are used as the target variables - `steps_future`. This method allows the model to learn sequential patterns and trends in the data, enabling accurate predictions for future points in the time series. 
+
+## imbrium `2.0.0`
+
+- adapting `keras_core`
+- removing internal hyperparameter tuning
+- removing encoder-decoder architectures
+- improve layer configuration
+- split input data into target and feature numpy arrays
+- overall lighten the library
+
+## imbrium `3.0.0`
+
+- switch from `keras_core` to `keras > 3.0.0`
+
+### Get started with imbrium
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+<details>
+  <summary>Univariate Pure Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import PureUni
+
+# create a PureUni object (numpy array expected)
+predictor = PureUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a PureUni objects;
+
+# create and fit a muti-layer perceptron model
+predictor.create_fit_mlp( 
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        dense_block_one = 1,
+        dense_block_two = 1,
+        dense_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a recurrent neural network model
+predictor.create_fit_rnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        rnn_block_three = 1,
+        metrics = "mean_squared_error",
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a long short-term neural network model
+predictor.create_fit_lstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        lstm_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional neural network
+predictor = create_fit_cnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        dense_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a gated recurrent unit neural network  
+predictor.create_fit_gru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        gru_block_one = 1,
+        gru_block_two = 1,
+        gru_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional recurrent neural network
+predictor.create_fit_birnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional long short-term memory neural network
+predictor.create_fit_bilstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional gated recurrent neural network
+predictor.create_fit_bigru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+predictor.predict(data)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+
+</details>
+
+<details>
+  <summary>Multivariate Pure Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import PureMulti
+
+# create a PureMulti object (numpy array expected)
+predictor = PureMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a PureMulti objects;
+
+# create and fit a muti-layer perceptron model
+predictor.create_fit_mlp( 
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        dense_block_one = 1,
+        dense_block_two = 1,
+        dense_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a recurrent neural network model
+predictor.create_fit_rnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        rnn_block_three = 1,
+        metrics = "mean_squared_error",
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a long short-term neural network model
+predictor.create_fit_lstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        lstm_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {"neurons": 50, "activation": "relu", "regularization": 0.0}
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional neural network
+predictor = create_fit_cnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        dense_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a gated recurrent unit neural network  
+predictor.create_fit_gru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        gru_block_one = 1,
+        gru_block_two = 1,
+        gru_block_three = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional recurrent neural network
+predictor.create_fit_birnn(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional long short-term memory neural network
+predictor.create_fit_bilstm(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a bidirectional gated recurrent neural network
+predictor.create_fit_bigru(
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "neurons": 50,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+predictor.predict(data)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+</details>
+
+<details>
+  <summary>Univariate Hybrid Predictors</summary>
+  <br>
+
+```python
+from imbrium import HybridUni
+
+# create a HybridUni object (numpy array expected)
+predictor = HybridUni(target = target_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a HybridUni objects:
+# create and fit a convolutional recurrent neural network
+predictor.create_fit_cnnrnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional long short-term memory neural network
+predictor.create_fit_cnnlstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional gated recurrent unit neural network  
+predictor.create_fit_cnngru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        gru_block_one = 1,
+        gru_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional recurrent neural network
+predictor.create_fit_cnnbirnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional long short-term neural network
+predictor.create_fit_cnnbilstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional gated recurrent neural network
+predictor.create_fit_cnnbigru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+# - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
+predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+
+</details>
+
+<details>
+  <summary>Multivariate Hybrid Predictors</summary>
+  <br>
+
+
+```python
+from imbrium import HybridMulti
+
+# create a HybridMulti object (numpy array expected)
+predictor = HybridMulti(target = target_numpy_array, features = features_numpy_array, evaluation_split = 0.2, validation_split = 0.2) 
+
+# the following models are available for a HybridMulti objects:
+# create and fit a convolutional recurrent neural network
+predictor.create_fit_cnnrnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        rnn_block_one = 1,
+        rnn_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional long short-term memory neural network
+predictor.create_fit_cnnlstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        lstm_block_one = 1,
+        lstm_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional gated recurrent unit neural network  
+predictor.create_fit_cnngru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        gru_block_one = 1,
+        gru_block_two = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional recurrent neural network
+predictor.create_fit_cnnbirnn(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        birnn_block_one = 1,
+        rnn_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional long short-term neural network
+predictor.create_fit_cnnbilstm(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bilstm_block_one = 1,
+        lstm_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# create and fit a convolutional bidirectional gated recurrent neural network
+predictor.create_fit_cnnbigru(
+        sub_seq,
+        steps_past,
+        steps_future,
+        optimizer = "adam",
+        optimizer_args = None,
+        loss = "mean_squared_error",
+        metrics = "mean_squared_error",
+        conv_block_one = 1,
+        conv_block_two = 1,
+        bigru_block_one = 1,
+        gru_block_one = 1,
+        layer_config = {
+            "layer0": {
+                "config": {
+                    "filters": 64,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer1": {
+                "config": {
+                    "filters": 32,
+                    "kernel_size": 1,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer2": {
+                "config": {
+                    "pool_size": 2,
+                }
+            },
+            "layer3": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                    "dropout": 0.0,
+                }
+            },
+            "layer4": {
+                "config": {
+                    "neurons": 32,
+                    "activation": "relu",
+                    "regularization": 0.0,
+                }
+            },
+        },
+        epochs = 100,
+        show_progress = 1,
+        board = False,
+)
+
+# you can add additional layer to the defualt layers by increasing the layer block count and adding the configuration for the layer in the layer_config dictionary. Please note that the last layer should not have a dropout key.
+
+# in addition, you can add to all models early stopping arguments:
+
+monitor='val_loss',
+min_delta=0,
+patience=0,
+verbose=0,
+mode='auto',
+baseline=None,
+restore_best_weights=False,
+start_from_epoch=0
+
+
+# instpect model structure
+predictor.model_blueprint()
+
+# evaluate model performance on testing data
+predictor.evaluate_model()
+
+# get model performance on testing data
+predictor.show_evaluation()
+
+# insptect keras model performances via (access dictionary via history key):
+predictor.show_performance()
+
+# make predictions via (numpy array expected):
+# - when loading/retrieving a saved model, provide sub_seq, steps_past, steps_future in the predict method!
+predictor.predict(data, sub_seq=None, steps_past=None, steps_future=None)
+
+# save predictor via:
+predictor.freeze(absolute_path)
+
+# load saved predictor via:
+predictor.retrieve(location)
+```  
+</details>
+
+</details>
+
+### Use Case: scaling + hyper parameter optimization
+
+https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/use-case-1.ipynb
+
+### Integration tests
+
+https://github.com/maxmekiska/ImbriumTesting-Demo/blob/main/IntegrationTest.ipynb
+
+
+## legacy: imbrium versions `<= 1.3.0`
+<details>
+  <summary>Expand</summary>
+  <br>
+
+The library differentiates between two
+modes:
+
+1. Univariate-Multistep forecasting
+2. Multivariate-Multistep forecasting
+
+These two main modes are further divided based on the complexity of the underlying model architectures:
+
+1. Pure
+2. Hybrid
+
+Pure supports the following architectures:
+
+- Multilayer perceptron (MLP)
+- Recurrent neural network (RNN)
+- Long short-term memory (LSTM)
+- Gated recurrent unit (GRU)
+- Convolutional neural network (CNN)
+- Bidirectional recurrent neural network (BI-RNN)
+- Bidirectional long-short term memory (BI-LSTM)
+- Bidirectional gated recurrent unit (BI-GRU)
+- Encoder-Decoder recurrent neural network
+- Encoder-Decoder long-short term memory
+- Encoder-Decoder convolutional neural network (Encoding via CNN, Decoding via GRU)
+- Encoder-Decoder gated recurrent unit
+
+Hybrid supports:
+
+- Convolutional neural network + recurrent neural network (CNN-RNN)
+- Convolutional neural network + Long short-term memory (CNN-LSTM)
+- Convolutional neural network + Gated recurrent unit (CNN-GRU)
+- Convolutional neural network + Bidirectional recurrent neural network (CNN-BI-RNN)
+- Convolutional neural network + Bidirectional long-short term memory (CNN-BI-LSTM)
+- Convolutional neural network + Bidirectional gated recurrent unit (CNN-BI-GRU)
+
+Please note that each model is supported by a prior input data pre-processing procedure which allows to set a look-back period, look-forward period, sub-sequences division (only for hybrid architectures) and data scaling method.
+
+The following scikit-learn scaling procedures are supported:
+
+- StandardScaler
+- MinMaxScaler
+- MaxAbsScaler
+- Normalizing ([0, 1])
+- None (raw data input)
+
+During training/fitting, callback conditions can be defined to guard against
+overfitting.
+
+Trained models can furthermore be saved or loaded if the user wishes to do so.
+
+## How to use imbrium?
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Attention: Typing has been left in the below examples to ease the configuration readability.
+
+#### Version updates:
+
+##### Version >= 1.2.0
+
+Version 1.2.0 started supporting tensor board dashboards: https://www.tensorflow.org/tensorboard/get_started
+
+##### Version >= 1.3.0
+
+Version 1.3.0 started supporting adjustable layer depth configurations for all architectures. If you wish to adjust the layer depth, please make sure to include a custom layer_config accounting for the correct number of layers. The last layer cannot contain a dropout parameter -> tuple needs to be of length 3: (neurons, activation, regularization).
+
+### `Univariate Models`:
+
+1. Univariate-Multistep forecasting - Pure architectures
+
+```python
+from imbrium.predictors.univarpure import PureUni
+
+predictor = PureUni(
+                    steps_past: int,
+                    steps_future: int,
+                    data = pd.DataFrame(),
+                    scale: str = ''
+                   )
+
+# Choose between one of the architectures:
+
+predictor.create_mlp(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     dense_block_one: int = 1,
+                     dense_block_two: int = 1,
+                     dense_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                    )
+
+predictor.create_rnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     rnn_block_one: int = 1,
+                     rnn_block_two: int = 1,
+                     rnn_block_three: int = 1,
+                     layer_config: dict = 
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_lstm(
+                      optimizer: str = 'adam',
+                      optimizer_args: dict = None,
+                      loss: str = 'mean_squared_error',
+                      metrics: str = 'mean_squared_error',
+                      lstm_block_one: int = 1,
+                      lstm_block_two: int = 1,
+                      lstm_block_three: int = 1,
+                      layer_config: dict =
+                      {
+                        'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                     )
+
+predictor.create_gru(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     gru_block_one: int = 1,
+                     gru_block_two: int = 1,
+                     gru_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_cnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     conv_block_one: int = 1,
+                     conv_block_two: int = 1,
+                     dense_block_one: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer2': (2), # (pool_size)
+                      'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_birnn(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       birnn_block_one: int = 1,
+                       rnn_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_bilstm(
+                        optimizer: str = 'adam', 
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        bilstm_block_one: int = 1,
+                        lstm_block_one: int = 1,
+                        layer_config: dict = 
+                        {
+                          'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                       )
+
+predictor.create_bigru(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       bigru_block_one: int = 1,
+                       gru_block_one: int = 1,
+                       layer_config: dict = 
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_encdec_rnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_rnn_block_one: int = 1,
+                            enc_rnn_block_two: int = 1,
+                            dec_rnn_block_one: int = 1,
+                            dec_rnn_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                            )
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_mlp(
+
+predictor.create_encdec_lstm(
                              optimizer: str = 'adam',
                              optimizer_args: dict = None,
                              loss: str = 'mean_squared_error',
                              metrics: str = 'mean_squared_error',
-                             dense_block_one: int = 1,
-                             dense_block_two: int = 1,
-                             dense_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                            )
-        
-        predictor.create_rnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             rnn_block_one: int = 1,
-                             rnn_block_two: int = 1,
-                             rnn_block_three: int = 1,
+                             enc_lstm_block_one: int = 1,
+                             enc_lstm_block_two: int = 1,
+                             dec_lstm_block_one: int = 1,
+                             dec_lstm_block_two: int = 1,
                              layer_config: dict = 
                              {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_lstm(
-                              optimizer: str = 'adam',
-                              optimizer_args: dict = None,
-                              loss: str = 'mean_squared_error',
-                              metrics: str = 'mean_squared_error',
-                              lstm_block_one: int = 1,
-                              lstm_block_two: int = 1,
-                              lstm_block_three: int = 1,
-                              layer_config: dict =
-                              {
-                                'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                             )
-        
-        predictor.create_gru(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             gru_block_one: int = 1,
-                             gru_block_two: int = 1,
-                             gru_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
                              }
                             )
-        
-        predictor.create_cnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             conv_block_one: int = 1,
-                             conv_block_two: int = 1,
-                             dense_block_one: int = 1,
-                             layer_config: dict =
-                             {
+
+predictor.create_encdec_cnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_conv_block_one: int = 1,
+                            enc_conv_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict = 
+                            {
                               'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer2': (2), # (pool_size)
-                              'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_birnn(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               birnn_block_one: int = 1,
-                               rnn_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_bilstm(
-                                optimizer: str = 'adam', 
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                bilstm_block_one: int = 1,
-                                lstm_block_one: int = 1,
-                                layer_config: dict = 
-                                {
-                                  'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                               )
-        
-        predictor.create_bigru(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               bigru_block_one: int = 1,
-                               gru_block_one: int = 1,
-                               layer_config: dict = 
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_encdec_rnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_rnn_block_one: int = 1,
-                                    enc_rnn_block_two: int = 1,
-                                    dec_rnn_block_one: int = 1,
-                                    dec_rnn_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                   )
-        
-        predictor.create_encdec_lstm(
-                                     optimizer: str = 'adam',
-                                     optimizer_args: dict = None,
-                                     loss: str = 'mean_squared_error',
-                                     metrics: str = 'mean_squared_error',
-                                     enc_lstm_block_one: int = 1,
-                                     enc_lstm_block_two: int = 1,
-                                     dec_lstm_block_one: int = 1,
-                                     dec_lstm_block_two: int = 1,
-                                     layer_config: dict = 
-                                     {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                     }
-                                    )
-        
-        predictor.create_encdec_cnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_conv_block_one: int = 1,
-                                    enc_conv_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict = 
-                                    {
-                                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer2': (2), # (pool_size)
-                                      'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer4': (100, 'relu', 0.0)  # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_gru(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_gru_block_one: int = 1,
-                                    enc_gru_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict = 
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss', 
-                            patience=3
-                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor = PureUni(steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        
-        2. Univariate-Multistep forecasting - Hybrid architectures
-        
-        ```python
-        from imbrium.predictors.univarhybrid import HybridUni
-        
-        predictor = HybridUni(
-                              sub_seq: int,
-                              steps_past: int,
-                              steps_future: int, data = pd.DataFrame(),
-                              scale: str = ''
-                             )
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_cnnrnn(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                rnn_block_one: int = 1,
-                                rnn_block_two: int = 1,
-                                layer_config = 
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0, 0.0) # (neurons, activation, regularization, dropout)
-                                }
-                              )
-        
-        predictor.create_cnnlstm(
-                                 optimizer: str = 'adam', 
-                                 optimizer_args: dict = None,
-                                 loss: str = 'mean_squared_error',
-                                 metrics: str = 'mean_squared_error',
-                                 conv_block_one: int = 1,
-                                 conv_block_two: int = 1,
-                                 lstm_block_one: int = 1,
-                                 lstm_block_two: int = 1,
-                                 layer_config = 
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnngru(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                gru_block_one: int = 1,
-                                gru_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnbirnn(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  birnn_block_one: int = 1,
-                                  rnn_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        predictor.create_cnnbilstm(
-                                   optimizer: str = 'adam',
-                                   optimizer_args: dict = None,
-                                   loss: str = 'mean_squared_error',
-                                   metrics: str = 'mean_squared_error',
-                                   conv_block_one: int = 1,
-                                   conv_block_two: int = 1,
-                                   bilstm_block_one: int = 1,
-                                   lstm_block_one: int = 1,
-                                   layer_config =
-                                   {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_cnnbigru(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  bigru_block_one: int = 1,
-                                  gru_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
-                            )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor =  HybridUni(sub_seq: int, steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        
-        ### `Multivariate Models`:
-        
-        1. Multivariate-Multistep forecasting - Pure architectures
-        
-        ```python
-        from imbrium.predictors.multivarpure import PureMulti
-        
-        # please make sure that the target feature is the first variable in the feature list
-        predictor = PureMulti(steps_past: int, steps_future: int, data = DataFrame(), features = [], scale: str = '')
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_mlp(
+                              'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer4': (100, 'relu', 0.0)  # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_encdec_gru(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_gru_block_one: int = 1,
+                            enc_gru_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict = 
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss', 
+                    patience=3
+                   )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor = PureUni(steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+
+2. Univariate-Multistep forecasting - Hybrid architectures
+
+```python
+from imbrium.predictors.univarhybrid import HybridUni
+
+predictor = HybridUni(
+                      sub_seq: int,
+                      steps_past: int,
+                      steps_future: int, data = pd.DataFrame(),
+                      scale: str = ''
+                     )
+
+# Choose between one of the architectures:
+
+predictor.create_cnnrnn(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        rnn_block_one: int = 1,
+                        rnn_block_two: int = 1,
+                        layer_config = 
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0, 0.0) # (neurons, activation, regularization, dropout)
+                        }
+                      )
+
+predictor.create_cnnlstm(
+                         optimizer: str = 'adam', 
+                         optimizer_args: dict = None,
+                         loss: str = 'mean_squared_error',
+                         metrics: str = 'mean_squared_error',
+                         conv_block_one: int = 1,
+                         conv_block_two: int = 1,
+                         lstm_block_one: int = 1,
+                         lstm_block_two: int = 1,
+                         layer_config = 
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0),  # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnngru(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        gru_block_one: int = 1,
+                        gru_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnbirnn(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          birnn_block_one: int = 1,
+                          rnn_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
+                        )
+
+predictor.create_cnnbilstm(
+                           optimizer: str = 'adam',
+                           optimizer_args: dict = None,
+                           loss: str = 'mean_squared_error',
+                           metrics: str = 'mean_squared_error',
+                           conv_block_one: int = 1,
+                           conv_block_two: int = 1,
+                           bilstm_block_one: int = 1,
+                           lstm_block_one: int = 1,
+                           layer_config =
+                           {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_cnnbigru(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          bigru_block_one: int = 1,
+                          gru_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
+                        )
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                    )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor =  HybridUni(sub_seq: int, steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+
+### `Multivariate Models`:
+
+1. Multivariate-Multistep forecasting - Pure architectures
+
+```python
+from imbrium.predictors.multivarpure import PureMulti
+
+# please make sure that the target feature is the first variable in the feature list
+predictor = PureMulti(steps_past: int, steps_future: int, data = DataFrame(), features = [], scale: str = '')
+
+# Choose between one of the architectures:
+
+predictor.create_mlp(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     dense_block_one: int = 1,
+                     dense_block_two: int = 1,
+                     dense_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_rnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     rnn_block_one: int = 1,
+                     rnn_block_two: int = 1,
+                     rnn_block_three: int = 1,
+                     layer_config: dict = 
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_lstm(
+                      optimizer: str = 'adam',
+                      optimizer_args: dict = None,
+                      loss: str = 'mean_squared_error',
+                      metrics: str = 'mean_squared_error',
+                      lstm_block_one: int = 1,
+                      lstm_block_two: int = 1,
+                      lstm_block_three: int = 1,
+                      layer_config: dict =
+                      {
+                        'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50,'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
+                        'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                      }
+                    )
+
+predictor.create_gru(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     gru_block_one: int = 1,
+                     gru_block_two: int = 1,
+                     gru_block_three: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                      'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     } 
+                    )
+
+predictor.create_cnn(
+                     optimizer: str = 'adam',
+                     optimizer_args: dict = None,
+                     loss: str = 'mean_squared_error',
+                     metrics: str = 'mean_squared_error',
+                     conv_block_one: int = 1,
+                     conv_block_two: int = 1,
+                     dense_block_one: int = 1,
+                     layer_config: dict =
+                     {
+                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                      'layer2': (2), # (pool_size)
+                      'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                     }
+                    )
+
+predictor.create_birnn(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       birnn_block_one: int = 1,
+                       rnn_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_bilstm(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        bilstm_block_one: int = 1,
+                        lstm_block_one: int = 1,
+                        layer_config: dict =
+                        {
+                          'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_bigru(
+                       optimizer: str = 'adam',
+                       optimizer_args: dict = None,
+                       loss: str = 'mean_squared_error',
+                       metrics: str = 'mean_squared_error',
+                       bigru_block_one: int = 1,
+                       gru_block_one: int = 1,
+                       layer_config: dict =
+                       {
+                        'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                        'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                       }
+                      )
+
+predictor.create_encdec_rnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_rnn_block_one: int = 1,
+                            enc_rnn_block_two: int = 1,
+                            dec_rnn_block_one: int = 1,
+                            dec_rnn_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
+                          )
+
+predictor.create_encdec_lstm(
                              optimizer: str = 'adam',
                              optimizer_args: dict = None,
                              loss: str = 'mean_squared_error',
                              metrics: str = 'mean_squared_error',
-                             dense_block_one: int = 1,
-                             dense_block_two: int = 1,
-                             dense_block_three: int = 1,
+                             enc_lstm_block_one: int = 1,
+                             enc_lstm_block_two: int = 1,
+                             dec_lstm_block_one: int = 1,
+                             dec_lstm_block_two: int = 1,
                              layer_config: dict =
                              {
-                              'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (25,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_rnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             rnn_block_one: int = 1,
-                             rnn_block_two: int = 1,
-                             rnn_block_three: int = 1,
-                             layer_config: dict = 
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
                              }
                             )
-        
-        predictor.create_lstm(
-                              optimizer: str = 'adam',
-                              optimizer_args: dict = None,
-                              loss: str = 'mean_squared_error',
-                              metrics: str = 'mean_squared_error',
-                              lstm_block_one: int = 1,
-                              lstm_block_two: int = 1,
-                              lstm_block_three: int = 1,
-                              layer_config: dict =
-                              {
-                                'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50,'relu', 0.0, 0.0),  # (neurons, activation, regularization, dropout)
-                                'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                              }
-                            )
-        
-        predictor.create_gru(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             gru_block_one: int = 1,
-                             gru_block_two: int = 1,
-                             gru_block_three: int = 1,
-                             layer_config: dict =
-                             {
-                              'layer0': (40, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer1': (50,'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                              'layer2': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             } 
-                            )
-        
-        predictor.create_cnn(
-                             optimizer: str = 'adam',
-                             optimizer_args: dict = None,
-                             loss: str = 'mean_squared_error',
-                             metrics: str = 'mean_squared_error',
-                             conv_block_one: int = 1,
-                             conv_block_two: int = 1,
-                             dense_block_one: int = 1,
-                             layer_config: dict =
-                             {
+
+predictor.create_encdec_cnn(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_conv_block_one: int = 1,
+                            enc_conv_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict =
+                            {
                               'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
                               'layer2': (2), # (pool_size)
-                              'layer3': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                             }
-                            )
-        
-        predictor.create_birnn(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               birnn_block_one: int = 1,
-                               rnn_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_bilstm(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                bilstm_block_one: int = 1,
-                                lstm_block_one: int = 1,
-                                layer_config: dict =
-                                {
-                                  'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_bigru(
-                               optimizer: str = 'adam',
-                               optimizer_args: dict = None,
-                               loss: str = 'mean_squared_error',
-                               metrics: str = 'mean_squared_error',
-                               bigru_block_one: int = 1,
-                               gru_block_one: int = 1,
-                               layer_config: dict =
-                               {
-                                'layer0': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                'layer1': (50, 'relu', 0.0) # (neurons, activation, regularization)
-                               }
-                              )
-        
-        predictor.create_encdec_rnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_rnn_block_one: int = 1,
-                                    enc_rnn_block_two: int = 1,
-                                    dec_rnn_block_one: int = 1,
-                                    dec_rnn_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_lstm(
-                                     optimizer: str = 'adam',
-                                     optimizer_args: dict = None,
-                                     loss: str = 'mean_squared_error',
-                                     metrics: str = 'mean_squared_error',
-                                     enc_lstm_block_one: int = 1,
-                                     enc_lstm_block_two: int = 1,
-                                     dec_lstm_block_one: int = 1,
-                                     dec_lstm_block_two: int = 1,
-                                     layer_config: dict =
-                                     {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                     }
-                                    )
-        
-        predictor.create_encdec_cnn(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_conv_block_one: int = 1,
-                                    enc_conv_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                      'layer2': (2), # (pool_size)
-                                      'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer4': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        predictor.create_encdec_gru(
-                                    optimizer: str = 'adam',
-                                    optimizer_args: dict = None,
-                                    loss: str = 'mean_squared_error',
-                                    metrics: str = 'mean_squared_error',
-                                    enc_gru_block_one: int = 1,
-                                    enc_gru_block_two: int = 1,
-                                    dec_gru_block_one: int = 1,
-                                    dec_gru_block_two: int = 1,
-                                    layer_config: dict =
-                                    {
-                                      'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                      'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
-                                    }
-                                  )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
+                              'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer4': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor = PureMulti(steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        2. Multivariate-Multistep forecasting - Hybrid architectures
-        
-        ```python
-        from imbrium.predictors.multivarhybrid import HybridMulti
-        
-        # please make sure that the target feature is the first variable in the feature list
-        predictor = HybridMulti(sub_seq: int, steps_past: int, steps_future: int, data = DataFrame(), features:list = [], scale: str = '')
-        
-        # Choose between one of the architectures:
-        
-        predictor.create_cnnrnn(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                rnn_block_one: int = 1,
-                                rnn_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnlstm(
-                                 optimizer: str = 'adam',
-                                 optimizer_args: dict = None,
-                                 loss: str = 'mean_squared_error',
-                                 metrics: str = 'mean_squared_error',
-                                 conv_block_one: int = 1,
-                                 conv_block_two: int = 1,
-                                 lstm_block_one: int = 1,
-                                 lstm_block_two: int = 1,
-                                 layer_config =
-                                 {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                 }
-                                )
-        
-        predictor.create_cnngru(
-                                optimizer: str = 'adam',
-                                optimizer_args: dict = None,
-                                loss: str = 'mean_squared_error',
-                                metrics: str = 'mean_squared_error',
-                                conv_block_one: int = 1,
-                                conv_block_two: int = 1,
-                                gru_block_one: int = 1,
-                                gru_block_two: int = 1,
-                                layer_config =
-                                {
-                                  'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                  'layer2': (2), # (pool_size)
-                                  'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                  'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                }
-                              )
-        
-        predictor.create_cnnbirnn(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  birnn_block_one: int = 1,
-                                  rnn_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        predictor.create_cnnbilstm(
-                                   optimizer: str = 'adam',
-                                   optimizer_args: dict = None,
-                                   loss: str = 'mean_squared_error',
-                                   metrics: str = 'mean_squared_error',
-                                   conv_block_one: int = 1,
-                                   conv_block_two: int = 1,
-                                   bilstm_block_one: int = 1,
-                                   lstm_block_one: int = 1,
-                                   layer_config =
-                                   {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                   }
-                                  )
-        
-        predictor.create_cnnbigru(
-                                  optimizer: str = 'adam',
-                                  optimizer_args: dict = None,
-                                  loss: str = 'mean_squared_error',
-                                  metrics: str = 'mean_squared_error',
-                                  conv_block_one: int = 1,
-                                  conv_block_two: int = 1,
-                                  bigru_block_one: int = 1,
-                                  gru_block_one: int = 1,
-                                  layer_config =
-                                  {
-                                    'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
-                                    'layer2': (2), # (pool_size)
-                                    'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
-                                    'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
-                                  }
-                                )
-        
-        # Fit the predictor object - more callback settings at:
-        
-        # https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
-        
-        predictor.fit_model(
-                            epochs: int,
-                            show_progress: int = 1,
-                            validation_split: float = 0.20,
-                            board: bool = True, # record training progress in tensorboard
-                            monitor='loss',
-                            patience=3
+
+predictor.create_encdec_gru(
+                            optimizer: str = 'adam',
+                            optimizer_args: dict = None,
+                            loss: str = 'mean_squared_error',
+                            metrics: str = 'mean_squared_error',
+                            enc_gru_block_one: int = 1,
+                            enc_gru_block_two: int = 1,
+                            dec_gru_block_one: int = 1,
+                            dec_gru_block_two: int = 1,
+                            layer_config: dict =
+                            {
+                              'layer0': (100, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer1': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer2': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                              'layer3': (100, 'relu', 0.0) # (neurons, activation, regularization)
+                            }
                           )
-        
-        # Have a look at the model performance
-        predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
-        
-        # Make a prediction based on new unseen data
-        predictor.predict(data: array)
-        
-        # Safe your model:
-        predictor.save_model()
-        
-        # Load a model:
-        # Step 1: initialize a new predictor object with same characteristics as model to load
-        # Step 2: Do not pass in any data
-        # Step 3: Invoke the method load_model()
-        # optional Step 4: Use the setter method set_model_id(name: str) to give model a name
-        
-        loading_predictor =  HybridMulti(sub_seq: int, steps_past: int, steps_future: int)
-        loading_predictor.load_model(location: str)
-        loading_predictor.set_model_id(name: str)
-        ```
-        </details>
-        
-        ## Hyperparameter Optimization imbrium 1.1.0
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Starting from version 1.1.0, imbrium will support experimental hyperparamerter optimization for the model layer config and optimizer arguments. The optimization process uses the Optuna library (https://optuna.org/).
-        
-        ### Optimization via the seeker decorator
-        
-        To leverage Optimization, use the new classes `OptimizePureUni`, `OptimizeHybridUni`, `OptimizePureMulti` and `OptimizeHybridMulti`. These classes implement optimizable model architecture methods:
-        
-        `OptimizePureUni` & `OptimizePureMulti`:
-        
-          - create_fit_mlp
-          - create_fit_rnn
-          - create_fit_lstm
-          - create_fit_cnn
-          - create_fit_gru
-          - create_fit_birnn
-          - create_fit_bilstm
-          - create_fit_bigru
-          - create_fit_encdec_rnn
-          - create_fit_encdec_lstm
-          - create_fit_encdec_gru
-          - create_fit_encdec_cnn
-        
-        `OptimizeHybridUni` & `OptimizeHybridMulti`:
-        
-          - create_fit_cnnrnn
-          - create_fit_cnnlstm
-          - create_fit_cnngru
-          - create_fit_cnnbirnn
-          - create_fit_cnnbilstm
-          - create_fit_cnnbigru
-        
-        #### Example `OptimizePureUni`
-        
-        ```python
-        from imbrium.predictors.univarpure import OptimizePureUni
-        from imbrium.utils.optimization import seeker
-        
-        # initialize optimizable predictor object
-        predictor = OptimizePureUni(steps_past=5, steps_future=10, data=data, scale='standard')
-        
-        
-        # use seeker decorator on optimization harness
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (5, 'relu'),
-                      'layer1': (10,'relu'),
-                      'layer2': (5, 'relu')
-                    },
-                    {
-                      'layer0': (2, 'relu'),
-                      'layer1': (5, 'relu'),
-                      'layer2': (2, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 2)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            # use optimizable create_fit_xxx method
-            return predictor.create_fit_lstm(*args, **kwargs)
-        
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=0,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
-                        )
-        
-        predictor.show_performance()
-        predictor.predict(data.tail(5))
-        predictor.model_blueprint()
-        ```
-        
-        #### Example `OptimizeHybridUni`
-        
-        ```python
-        from imbrium.predictors.univarhybrid import OptimizeHybridUni
-        from imbrium.utils.optimization import seeker
-        
-        predictor = OptimizeHybridUni(sub_seq = 2, steps_past = 10, steps_future = 5, data = data, scale = 'maxabs')
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (25, 'relu'),
-                      'layer4': (10, 'relu')
-                    },
-                    {
-                      'layer0': (16, 1, 'relu'),
-                      'layer1': (8, 1, 'relu'),
-                      'layer2': (2)
-                      'layer3': (55, 'relu'),
-                      'layer4': (10, 'relu')
-                    },
-                    {
-                      'layer0': (32, 1, 'relu'),
-                      'layer1': (16, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (25, 'relu'),
-                      'layer4': (10, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 2)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_cnnlstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=0,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                  )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor = PureMulti(steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+2. Multivariate-Multistep forecasting - Hybrid architectures
+
+```python
+from imbrium.predictors.multivarhybrid import HybridMulti
+
+# please make sure that the target feature is the first variable in the feature list
+predictor = HybridMulti(sub_seq: int, steps_past: int, steps_future: int, data = DataFrame(), features:list = [], scale: str = '')
+
+# Choose between one of the architectures:
+
+predictor.create_cnnrnn(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        rnn_block_one: int = 1,
+                        rnn_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnlstm(
+                         optimizer: str = 'adam',
+                         optimizer_args: dict = None,
+                         loss: str = 'mean_squared_error',
+                         metrics: str = 'mean_squared_error',
+                         conv_block_one: int = 1,
+                         conv_block_two: int = 1,
+                         lstm_block_one: int = 1,
+                         lstm_block_two: int = 1,
+                         layer_config =
+                         {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                         }
                         )
-        
-        predictor.show_performance()
-        predictor.predict(data.tail(10))
-        predictor.model_blueprint()
-        ```
-        
-        #### Example `OptimizePureMulti`
-        
-        ```python
-        predictor = OptimizePureMulti(
-                                      steps_past =  5,
-                                      steps_future = 10,
-                                      data = data,
-                                      features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
-                                      scale = 'normalize'
-                                    )
-        
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (5, 'relu'),
-                      'layer1': (10,'relu'),
-                      'layer2': (5, 'relu')
-                    },
-                    {
-                      'layer0': (2, 'relu'),
-                      'layer1': (5, 'relu'),
-                      'layer2': (2, 'relu')
-                    },
-                    {
-                      'layer0': (20, 'relu'),
-                      'layer1': (50, 'relu'),
-                      'layer2': (20, 'sigmoid')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 3)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_lstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=1, 
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+predictor.create_cnngru(
+                        optimizer: str = 'adam',
+                        optimizer_args: dict = None,
+                        loss: str = 'mean_squared_error',
+                        metrics: str = 'mean_squared_error',
+                        conv_block_one: int = 1,
+                        conv_block_two: int = 1,
+                        gru_block_one: int = 1,
+                        gru_block_two: int = 1,
+                        layer_config =
+                        {
+                          'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                          'layer2': (2), # (pool_size)
+                          'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                          'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                        }
+                      )
+
+predictor.create_cnnbirnn(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          birnn_block_one: int = 1,
+                          rnn_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
                         )
-        
-        
-        predictor.show_performance()
-        predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(5))
-        predictor.model_blueprint()
-        ```
-        
-        
-        #### Example `OptimizeHybridMulti`
-        
-        ```python
-        predictor = OptimizeHybridMulti(
-                                        sub_seq = 2, 
-                                        steps_past = 10,
-                                        steps_future = 5,
-                                        data = data,
-                                        features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
-                                        scale = 'normalize'
-                                      )
-        
-        
-        @seeker(optimizer_range=["adam", "sgd"], 
-                layer_config_range= [
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    },
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    },
-                    {
-                      'layer0': (8, 1, 'relu'),
-                      'layer1': (4, 1, 'relu'),
-                      'layer2': (2),
-                      'layer3': (5, 'relu'),
-                      'layer4': (5, 'relu')
-                    }
-                ], 
-                optimizer_args_range = [
-                    {
-                      'learning_rate': 0.02,
-                    },
-                    {
-                      'learning_rate': 0.0001,
-                    }
-                ]
-                optimization_target='minimize', n_trials = 3)
-        def create_fit_model(predictor: object, *args, **kwargs):
-            return predictor.create_fit_cnnlstm(*args, **kwargs)
-        
-        create_fit_model(
-                         predictor,
-                         loss='mean_squared_error',
-                         metrics='mean_squared_error',
-                         epochs=2,
-                         show_progress=1,
-                         validation_split=0.20,
-                         board=True,
-                         monitor='val_loss',
-                         patience=2,
-                         min_delta=0,
-                         verbose=1
+
+predictor.create_cnnbilstm(
+                           optimizer: str = 'adam',
+                           optimizer_args: dict = None,
+                           loss: str = 'mean_squared_error',
+                           metrics: str = 'mean_squared_error',
+                           conv_block_one: int = 1,
+                           conv_block_two: int = 1,
+                           bilstm_block_one: int = 1,
+                           lstm_block_one: int = 1,
+                           layer_config =
+                           {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                           }
+                          )
+
+predictor.create_cnnbigru(
+                          optimizer: str = 'adam',
+                          optimizer_args: dict = None,
+                          loss: str = 'mean_squared_error',
+                          metrics: str = 'mean_squared_error',
+                          conv_block_one: int = 1,
+                          conv_block_two: int = 1,
+                          bigru_block_one: int = 1,
+                          gru_block_one: int = 1,
+                          layer_config =
+                          {
+                            'layer0': (64, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer1': (32, 1, 'relu', 0.0, 0.0), # (filter_size, kernel_size, activation, regularization, dropout)
+                            'layer2': (2), # (pool_size)
+                            'layer3': (50, 'relu', 0.0, 0.0), # (neurons, activation, regularization, dropout)
+                            'layer4': (25, 'relu', 0.0) # (neurons, activation, regularization)
+                          }
                         )
-        
-        
-        predictor.show_performance()
-        predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(10))
-        predictor.model_blueprint()
-        ```
-        #### The shell of the seeker harness
-          
-        ```python
-        predictor = OptimizePureMulti(...)
-        
-        @seeker(optimizer_range=[...], 
-                layer_config_range= [
-                    {...},
-                    {...},
-                    {...}
-                ], 
-                optimizer_args_range = [
-                    {...},
-                    {...},
-                ]
-                optimization_target = '...', n_trials = x)
-        def create_fit_model(predictor: object, *args, **kwargs): # seeker harness
-            return predictor.create_fit_xxx(*args, **kwargs)
-        
-        create_fit_model(...) # execute seeker harness
-        
-        
-        predictor.show_performance()
-        predictor.predict(...)
-        predictor.model_blueprint()
-        ```
-        
-        
-        </details>
-        
-        ## References
-        
-        <details>
-          <summary>Expand</summary>
-          <br>
-        
-        Brwonlee, J., 2016. Display deep learning model training history in keras [Online]. Available from:
-        https://machinelearningmastery.com/display-deep-
-        learning-model-training-history-in-keras/.
-        
-        Brwonlee, J., 2018a. How to develop convolutional neural network models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-convolutional-
-        neural-network-models-for-time-series-forecasting/.
-        
-        Brwonlee, J., 2018b. How to develop lstm models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-
-        lstm-models-for-time-series-forecasting/.
-        
-        Brwonlee, J., 2018c. How to develop multilayer perceptron models for time series forecasting [Online]. Available from:
-        https://machinelearningmastery.com/how-to-develop-multilayer-
-        perceptron-models-for-time-series-forecasting/.
-        
-        </details>
-        
-        
-        </details>
-Keywords: machinelearning,keras,deeplearning,timeseries,forecasting
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
+
+# Fit the predictor object - more callback settings at:
+
+# https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping
+
+predictor.fit_model(
+                    epochs: int,
+                    show_progress: int = 1,
+                    validation_split: float = 0.20,
+                    board: bool = True, # record training progress in tensorboard
+                    monitor='loss',
+                    patience=3
+                  )
+
+# Have a look at the model performance
+predictor.show_performance(metric_name: str = None) # optionally plot metric name against loss
+
+# Make a prediction based on new unseen data
+predictor.predict(data: array)
+
+# Safe your model:
+predictor.save_model()
+
+# Load a model:
+# Step 1: initialize a new predictor object with same characteristics as model to load
+# Step 2: Do not pass in any data
+# Step 3: Invoke the method load_model()
+# optional Step 4: Use the setter method set_model_id(name: str) to give model a name
+
+loading_predictor =  HybridMulti(sub_seq: int, steps_past: int, steps_future: int)
+loading_predictor.load_model(location: str)
+loading_predictor.set_model_id(name: str)
+```
+</details>
+
+## Hyperparameter Optimization imbrium 1.1.0
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Starting from version 1.1.0, imbrium will support experimental hyperparamerter optimization for the model layer config and optimizer arguments. The optimization process uses the Optuna library (https://optuna.org/).
+
+### Optimization via the seeker decorator
+
+To leverage Optimization, use the new classes `OptimizePureUni`, `OptimizeHybridUni`, `OptimizePureMulti` and `OptimizeHybridMulti`. These classes implement optimizable model architecture methods:
+
+`OptimizePureUni` & `OptimizePureMulti`:
+
+  - create_fit_mlp
+  - create_fit_rnn
+  - create_fit_lstm
+  - create_fit_cnn
+  - create_fit_gru
+  - create_fit_birnn
+  - create_fit_bilstm
+  - create_fit_bigru
+  - create_fit_encdec_rnn
+  - create_fit_encdec_lstm
+  - create_fit_encdec_gru
+  - create_fit_encdec_cnn
+
+`OptimizeHybridUni` & `OptimizeHybridMulti`:
+
+  - create_fit_cnnrnn
+  - create_fit_cnnlstm
+  - create_fit_cnngru
+  - create_fit_cnnbirnn
+  - create_fit_cnnbilstm
+  - create_fit_cnnbigru
+
+#### Example `OptimizePureUni`
+
+```python
+from imbrium.predictors.univarpure import OptimizePureUni
+from imbrium.utils.optimization import seeker
+
+# initialize optimizable predictor object
+predictor = OptimizePureUni(steps_past=5, steps_future=10, data=data, scale='standard')
+
+
+# use seeker decorator on optimization harness
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (5, 'relu'),
+              'layer1': (10,'relu'),
+              'layer2': (5, 'relu')
+            },
+            {
+              'layer0': (2, 'relu'),
+              'layer1': (5, 'relu'),
+              'layer2': (2, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 2)
+def create_fit_model(predictor: object, *args, **kwargs):
+    # use optimizable create_fit_xxx method
+    return predictor.create_fit_lstm(*args, **kwargs)
+
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=0,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+predictor.show_performance()
+predictor.predict(data.tail(5))
+predictor.model_blueprint()
+```
+
+#### Example `OptimizeHybridUni`
+
+```python
+from imbrium.predictors.univarhybrid import OptimizeHybridUni
+from imbrium.utils.optimization import seeker
+
+predictor = OptimizeHybridUni(sub_seq = 2, steps_past = 10, steps_future = 5, data = data, scale = 'maxabs')
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (25, 'relu'),
+              'layer4': (10, 'relu')
+            },
+            {
+              'layer0': (16, 1, 'relu'),
+              'layer1': (8, 1, 'relu'),
+              'layer2': (2)
+              'layer3': (55, 'relu'),
+              'layer4': (10, 'relu')
+            },
+            {
+              'layer0': (32, 1, 'relu'),
+              'layer1': (16, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (25, 'relu'),
+              'layer4': (10, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 2)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_cnnlstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=0,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+predictor.show_performance()
+predictor.predict(data.tail(10))
+predictor.model_blueprint()
+```
+
+#### Example `OptimizePureMulti`
+
+```python
+predictor = OptimizePureMulti(
+                              steps_past =  5,
+                              steps_future = 10,
+                              data = data,
+                              features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
+                              scale = 'normalize'
+                            )
+
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (5, 'relu'),
+              'layer1': (10,'relu'),
+              'layer2': (5, 'relu')
+            },
+            {
+              'layer0': (2, 'relu'),
+              'layer1': (5, 'relu'),
+              'layer2': (2, 'relu')
+            },
+            {
+              'layer0': (20, 'relu'),
+              'layer1': (50, 'relu'),
+              'layer2': (20, 'sigmoid')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 3)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_lstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=1, 
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+
+predictor.show_performance()
+predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(5))
+predictor.model_blueprint()
+```
+
+
+#### Example `OptimizeHybridMulti`
+
+```python
+predictor = OptimizeHybridMulti(
+                                sub_seq = 2, 
+                                steps_past = 10,
+                                steps_future = 5,
+                                data = data,
+                                features = ['target', 'target', 'HouseAge', 'AveRooms', 'AveBedrms'],
+                                scale = 'normalize'
+                              )
+
+
+@seeker(optimizer_range=["adam", "sgd"], 
+        layer_config_range= [
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            },
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            },
+            {
+              'layer0': (8, 1, 'relu'),
+              'layer1': (4, 1, 'relu'),
+              'layer2': (2),
+              'layer3': (5, 'relu'),
+              'layer4': (5, 'relu')
+            }
+        ], 
+        optimizer_args_range = [
+            {
+              'learning_rate': 0.02,
+            },
+            {
+              'learning_rate': 0.0001,
+            }
+        ]
+        optimization_target='minimize', n_trials = 3)
+def create_fit_model(predictor: object, *args, **kwargs):
+    return predictor.create_fit_cnnlstm(*args, **kwargs)
+
+create_fit_model(
+                 predictor,
+                 loss='mean_squared_error',
+                 metrics='mean_squared_error',
+                 epochs=2,
+                 show_progress=1,
+                 validation_split=0.20,
+                 board=True,
+                 monitor='val_loss',
+                 patience=2,
+                 min_delta=0,
+                 verbose=1
+                )
+
+
+predictor.show_performance()
+predictor.predict(data[['target', 'HouseAge', 'AveRooms', 'AveBedrms']].tail(10))
+predictor.model_blueprint()
+```
+#### The shell of the seeker harness
+  
+```python
+predictor = OptimizePureMulti(...)
+
+@seeker(optimizer_range=[...], 
+        layer_config_range= [
+            {...},
+            {...},
+            {...}
+        ], 
+        optimizer_args_range = [
+            {...},
+            {...},
+        ]
+        optimization_target = '...', n_trials = x)
+def create_fit_model(predictor: object, *args, **kwargs): # seeker harness
+    return predictor.create_fit_xxx(*args, **kwargs)
+
+create_fit_model(...) # execute seeker harness
+
+
+predictor.show_performance()
+predictor.predict(...)
+predictor.model_blueprint()
+```
+
+
+</details>
+
+## References
+
+<details>
+  <summary>Expand</summary>
+  <br>
+
+Brwonlee, J., 2016. Display deep learning model training history in keras [Online]. Available from:
+https://machinelearningmastery.com/display-deep-
+learning-model-training-history-in-keras/.
+
+Brwonlee, J., 2018a. How to develop convolutional neural network models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-convolutional-
+neural-network-models-for-time-series-forecasting/.
+
+Brwonlee, J., 2018b. How to develop lstm models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-
+lstm-models-for-time-series-forecasting/.
+
+Brwonlee, J., 2018c. How to develop multilayer perceptron models for time series forecasting [Online]. Available from:
+https://machinelearningmastery.com/how-to-develop-multilayer-
+perceptron-models-for-time-series-forecasting/.
+
+</details>
+
+
+</details>
+
```

### Comparing `imbrium-2.1.0/imbrium.egg-info/SOURCES.txt` & `imbrium-3.0.0/imbrium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imbrium-2.1.0/setup.py` & `imbrium-3.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,23 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/imbrium",
     description="Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="imbrium",
-    version="2.1.0",
+    version="3.0.0",
     packages=find_packages(include=["imbrium", "imbrium.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
-        "keras-core >=0.1.5, <0.2.0",
-        "tensorflow >=2.13.0, <2.14.0",
+        "tensorflow>=2.16.0",
     ],
     classifiers=[
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     keywords=["machinelearning", "keras", "deeplearning", "timeseries", "forecasting"],
-    python_rquieres=">= 3.8.0, <= 3.11.0",
+    python_rquieres=">= 3.9.0, <= 3.11.0",
 )
```

