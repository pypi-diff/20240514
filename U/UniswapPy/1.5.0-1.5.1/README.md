# Comparing `tmp/uniswappy-1.5.0.tar.gz` & `tmp/uniswappy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswappy-1.5.0.tar", last modified: Wed May  8 21:49:24 2024, max compression
+gzip compressed data, was "uniswappy-1.5.1.tar", last modified: Mon May 13 22:58:31 2024, max compression
```

## Comparing `uniswappy-1.5.0.tar` & `uniswappy-1.5.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.811194 uniswappy-1.5.0/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 uniswappy-1.5.0/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-08 21:49:24.811128 uniswappy-1.5.0/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     4341 2024-05-01 19:05:23.000000 uniswappy-1.5.0/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.810878 uniswappy-1.5.0/UniswapPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     3752 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 uniswappy-1.5.0/UniswapPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       30 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/top_level.txt
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.770417 uniswappy-1.5.0/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.773645 uniswappy-1.5.0/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      953 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.770841 uniswappy-1.5.0/python/prod/cpt/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.774871 uniswappy-1.5.0/python/prod/cpt/exchg/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/exchg/ChildUniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    21851 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/exchg/UniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    42402 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/exchg/UniswapV3Exchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 uniswappy-1.5.0/python/prod/cpt/exchg/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.775546 uniswappy-1.5.0/python/prod/cpt/factory/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4208 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/factory/UniswapFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 uniswappy-1.5.0/python/prod/cpt/factory/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.776015 uniswappy-1.5.0/python/prod/cpt/index/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3366 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/index/RebaseIndexToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3462 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/index/SettlementLPToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-05-07 01:41:36.000000 uniswappy-1.5.0/python/prod/cpt/index/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.777189 uniswappy-1.5.0/python/prod/cpt/quote/
--rw-r--r--   0 ian_moore   (501) staff       (20)     6933 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/quote/IndexTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7081 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/quote/LPQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/quote/LPTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/quote/TreeAmountQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/cpt/quote/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.777726 uniswappy-1.5.0/python/prod/cpt/vault/
--rw-r--r--   0 ian_moore   (501) staff       (20)    15304 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/vault/IndexVault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/vault/Vault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/cpt/vault/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.778077 uniswappy-1.5.0/python/prod/cpt/wallet/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/wallet/Wallets.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-05-07 02:47:23.000000 uniswappy-1.5.0/python/prod/cpt/wallet/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.779011 uniswappy-1.5.0/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1664 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/DOAERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1441 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/ERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1088 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/IndexERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1700 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/LPERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.771321 uniswappy-1.5.0/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.779878 uniswappy-1.5.0/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)      494 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/math/basic/IDGenerator.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/basic/RoundFloat.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.780571 uniswappy-1.5.0/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/interest/CompoundReturn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/interest/Yield.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.781689 uniswappy-1.5.0/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/ConstantIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/IPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.800009 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801153 uniswappy-1.5.0/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/BrownianModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/EventSelectionModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/ModelQueue.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/TimeDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/TokenDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801674 uniswappy-1.5.0/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5551 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/math/risk/MaxDrop.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801972 uniswappy-1.5.0/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)      301 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/Process.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.802361 uniswappy-1.5.0/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2465 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/burn/IndexTokenBurn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.802879 uniswappy-1.5.0/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7051 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/deposit/SwapDeposit.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.803280 uniswappy-1.5.0/python/prod/process/join/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1870 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/join/Join.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/join/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.803751 uniswappy-1.5.0/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3611 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/liquidity/AddLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3200 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/liquidity/RemoveLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.804052 uniswappy-1.5.0/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2737 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/mint/SwapIndexMint.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.804659 uniswappy-1.5.0/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2319 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/swap/RandomSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2566 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/swap/Swap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     5338 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/swap/WithdrawSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.806022 uniswappy-1.5.0/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/Arbitrage.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4973 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/simulate/CorrectReserves.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/MarkovState.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/simulate/QuantTerminal.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/SimpleLPSimulation.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2229 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/simulate/SolveDeltas.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/simulate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.772086 uniswappy-1.5.0/python/prod/utils/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.806343 uniswappy-1.5.0/python/prod/utils/client/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/client/API0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/client/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.807287 uniswappy-1.5.0/python/prod/utils/data/
--rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 uniswappy-1.5.0/python/prod/utils/data/Chain0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/data/ExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/data/FactoryData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 uniswappy-1.5.0/python/prod/utils/data/UniswapExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/data/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.807819 uniswappy-1.5.0/python/prod/utils/interfaces/
--rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/interfaces/IExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/interfaces/IExchangeFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 uniswappy-1.5.0/python/prod/utils/interfaces/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.808254 uniswappy-1.5.0/python/prod/utils/tools/
--rw-r--r--   0 ian_moore   (501) staff       (20)      725 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/MockAddress.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.810674 uniswappy-1.5.0/python/prod/utils/tools/v3/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/FullMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/LiquidityMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Position.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SafeMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Shared.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    10496 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SqrtPriceMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SwapMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Tick.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/TickMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3208 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Helper.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Utils.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      303 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-05-08 21:49:24.811432 uniswappy-1.5.0/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1572 2024-05-08 21:48:13.000000 uniswappy-1.5.0/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.168704 uniswappy-1.5.1/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 uniswappy-1.5.1/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-13 22:58:31.168644 uniswappy-1.5.1/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4341 2024-05-01 19:05:23.000000 uniswappy-1.5.1/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.168419 uniswappy-1.5.1/UniswapPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-13 22:58:31.000000 uniswappy-1.5.1/UniswapPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3752 2024-05-13 22:58:31.000000 uniswappy-1.5.1/UniswapPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-05-13 22:58:31.000000 uniswappy-1.5.1/UniswapPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 uniswappy-1.5.1/UniswapPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       30 2024-05-13 22:58:31.000000 uniswappy-1.5.1/UniswapPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-05-13 22:58:31.000000 uniswappy-1.5.1/UniswapPy.egg-info/top_level.txt
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.141540 uniswappy-1.5.1/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.145032 uniswappy-1.5.1/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      953 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.141960 uniswappy-1.5.1/python/prod/cpt/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.146032 uniswappy-1.5.1/python/prod/cpt/exchg/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/cpt/exchg/ChildUniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    21851 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/cpt/exchg/UniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    42402 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/cpt/exchg/UniswapV3Exchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 uniswappy-1.5.1/python/prod/cpt/exchg/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.146466 uniswappy-1.5.1/python/prod/cpt/factory/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4208 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/cpt/factory/UniswapFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 uniswappy-1.5.1/python/prod/cpt/factory/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.147061 uniswappy-1.5.1/python/prod/cpt/index/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3518 2024-05-13 22:29:19.000000 uniswappy-1.5.1/python/prod/cpt/index/RebaseIndexToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3462 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/cpt/index/SettlementLPToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-05-07 01:41:36.000000 uniswappy-1.5.1/python/prod/cpt/index/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.148251 uniswappy-1.5.1/python/prod/cpt/quote/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6933 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/cpt/quote/IndexTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7081 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/cpt/quote/LPQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/cpt/quote/LPTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/cpt/quote/TreeAmountQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/cpt/quote/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.149066 uniswappy-1.5.1/python/prod/cpt/vault/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15304 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/cpt/vault/IndexVault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/cpt/vault/Vault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/cpt/vault/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.149547 uniswappy-1.5.1/python/prod/cpt/wallet/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/cpt/wallet/Wallets.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-05-07 02:47:23.000000 uniswappy-1.5.1/python/prod/cpt/wallet/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.150423 uniswappy-1.5.1/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1664 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/erc/DOAERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1441 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/erc/ERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1088 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/erc/IndexERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1700 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/erc/LPERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.142435 uniswappy-1.5.1/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.150962 uniswappy-1.5.1/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      494 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/math/basic/IDGenerator.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/basic/RoundFloat.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.151418 uniswappy-1.5.1/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/interest/CompoundReturn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/interest/Yield.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.151919 uniswappy-1.5.1/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/ips/ConstantIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/ips/IPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.152207 uniswappy-1.5.1/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/ips/aggregate/AggregateIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.153105 uniswappy-1.5.1/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/model/BrownianModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/model/EventSelectionModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/model/ModelQueue.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/model/TimeDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/model/TokenDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.153402 uniswappy-1.5.1/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5551 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/math/risk/MaxDrop.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.153667 uniswappy-1.5.1/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      301 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/Process.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.154028 uniswappy-1.5.1/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2465 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/burn/IndexTokenBurn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.157785 uniswappy-1.5.1/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7051 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/process/deposit/SwapDeposit.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.161796 uniswappy-1.5.1/python/prod/process/join/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1870 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/process/join/Join.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/join/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.162236 uniswappy-1.5.1/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3611 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/process/liquidity/AddLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3200 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/liquidity/RemoveLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.162501 uniswappy-1.5.1/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2737 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/mint/SwapIndexMint.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.163109 uniswappy-1.5.1/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2319 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/swap/RandomSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2566 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/process/swap/Swap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5338 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/process/swap/WithdrawSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.5.1/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.164257 uniswappy-1.5.1/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/simulate/Arbitrage.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4973 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/simulate/CorrectReserves.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/simulate/MarkovState.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 uniswappy-1.5.1/python/prod/simulate/QuantTerminal.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/simulate/SimpleLPSimulation.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2229 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/simulate/SolveDeltas.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 uniswappy-1.5.1/python/prod/simulate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.143335 uniswappy-1.5.1/python/prod/utils/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.164560 uniswappy-1.5.1/python/prod/utils/client/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 uniswappy-1.5.1/python/prod/utils/client/API0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 uniswappy-1.5.1/python/prod/utils/client/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.165399 uniswappy-1.5.1/python/prod/utils/data/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 uniswappy-1.5.1/python/prod/utils/data/Chain0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/utils/data/ExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/utils/data/FactoryData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 uniswappy-1.5.1/python/prod/utils/data/UniswapExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 uniswappy-1.5.1/python/prod/utils/data/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.165806 uniswappy-1.5.1/python/prod/utils/interfaces/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/utils/interfaces/IExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 uniswappy-1.5.1/python/prod/utils/interfaces/IExchangeFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 uniswappy-1.5.1/python/prod/utils/interfaces/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.166199 uniswappy-1.5.1/python/prod/utils/tools/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      725 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/utils/tools/MockAddress.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/utils/tools/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-13 22:58:31.168233 uniswappy-1.5.1/python/prod/utils/tools/v3/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/FullMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/LiquidityMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/Position.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/SafeMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/Shared.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10496 2024-05-01 19:05:23.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/SqrtPriceMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/SwapMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/Tick.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/TickMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3275 2024-05-09 00:09:10.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/UniV3Helper.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/UniV3Utils.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      303 2024-05-08 21:48:13.000000 uniswappy-1.5.1/python/prod/utils/tools/v3/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-05-13 22:58:31.168922 uniswappy-1.5.1/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1572 2024-05-13 22:55:34.000000 uniswappy-1.5.1/setup.py
```

### Comparing `uniswappy-1.5.0/LICENSE.txt` & `uniswappy-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/PKG-INFO` & `uniswappy-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `uniswappy-1.5.0/README.md` & `uniswappy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/UniswapPy.egg-info/PKG-INFO` & `uniswappy-1.5.1/UniswapPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `uniswappy-1.5.0/UniswapPy.egg-info/SOURCES.txt` & `uniswappy-1.5.1/UniswapPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/__init__.py` & `uniswappy-1.5.1/python/prod/__init__.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/exchg/ChildUniswapExchange.py` & `uniswappy-1.5.1/python/prod/cpt/exchg/ChildUniswapExchange.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/exchg/UniswapExchange.py` & `uniswappy-1.5.1/python/prod/cpt/exchg/UniswapExchange.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/exchg/UniswapV3Exchange.py` & `uniswappy-1.5.1/python/prod/cpt/exchg/UniswapV3Exchange.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/factory/UniswapFactory.py` & `uniswappy-1.5.1/python/prod/cpt/factory/UniswapFactory.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/index/RebaseIndexToken.py` & `uniswappy-1.5.1/python/prod/cpt/index/RebaseIndexToken.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,34 +57,35 @@
         itkn_amt = dy1 + dy2
 
         return itkn_amt if itkn_amt > 0 else 0  
 
     def calc_univ3_tkn_settlement(self, lp, token_in, dL, lwr_tick, upr_tick):
                 
         L = lp.get_liquidity()
+        L_diff = (L - dL) 
         if(token_in.token_name == lp.token0):
-            sqrtp_cur = lp.slot0.sqrtPriceX96/2**96
             sqrtp_pa = TickMath.getSqrtRatioAtTick(lwr_tick)/2**96
             sqrtp_pb = TickMath.getSqrtRatioAtTick(upr_tick)/2**96 
+            sqrtp_cur = lp.slot0.sqrtPriceX96/2**96 
             dPy = (sqrtp_cur - sqrtp_pa)
-            dPx = (1/sqrtp_cur - 1/sqrtp_pb)          
+            dPx = (1/sqrtp_cur - 1/sqrtp_pb)  
+            dx = dL*dPx
+            dy = dL*dPy    
+            sqrtp_next = sqrtp_cur + (997*dy)/(L_diff*1000) 
+            itkn_amt = dx + L_diff * (1/sqrtp_cur - 1/sqrtp_next)
         elif(token_in.token_name == lp.token1):
             sqrtp_cur = 2**96/lp.slot0.sqrtPriceX96
             sqrtp_pa = 2**96/TickMath.getSqrtRatioAtTick(lwr_tick)
             sqrtp_pb = 2**96/TickMath.getSqrtRatioAtTick(upr_tick)
-            dPx = (1/sqrtp_cur - 1/sqrtp_pa)
-            dPy = (sqrtp_cur - sqrtp_pb)
-    
-        dAmt = dL*dPx
-        
-        L_diff = (L - dL) 
-        sqrtp_next = sqrtp_cur + (997*dAmt)/(L_diff*1000) 
-        dy1 = dAmt
-        dy2 = L_diff * (1/sqrtp_cur - 1/sqrtp_next)
-        itkn_amt = dy1 + dy2
+            dPy = (1/sqrtp_cur - 1/sqrtp_pa)
+            dPx = (sqrtp_cur - sqrtp_pb)
+            dx = dL*dPx
+            dy = dL*dPy
+            sqrtp_next = sqrtp_cur + (997*dx)/(L_diff*1000) 
+            itkn_amt = dy + L_diff * (1/sqrtp_cur - 1/sqrtp_next)
 
         return itkn_amt if itkn_amt > 0 else 0 
     
 
     def get_reserves(self, lp, token_in):
         tokens = lp.factory.token_from_exchange[lp.name]
         if(token_in.token_name == lp.token1):
```

### Comparing `uniswappy-1.5.0/python/prod/cpt/index/SettlementLPToken.py` & `uniswappy-1.5.1/python/prod/cpt/index/SettlementLPToken.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/quote/IndexTokenQuote.py` & `uniswappy-1.5.1/python/prod/cpt/quote/IndexTokenQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/quote/LPQuote.py` & `uniswappy-1.5.1/python/prod/cpt/quote/LPQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/quote/LPTokenQuote.py` & `uniswappy-1.5.1/python/prod/cpt/quote/LPTokenQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/quote/TreeAmountQuote.py` & `uniswappy-1.5.1/python/prod/cpt/quote/TreeAmountQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/vault/IndexVault.py` & `uniswappy-1.5.1/python/prod/cpt/vault/IndexVault.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/vault/Vault.py` & `uniswappy-1.5.1/python/prod/cpt/vault/Vault.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/cpt/wallet/Wallets.py` & `uniswappy-1.5.1/python/prod/cpt/wallet/Wallets.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/erc/DOAERC20.py` & `uniswappy-1.5.1/python/prod/erc/DOAERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/erc/ERC20.py` & `uniswappy-1.5.1/python/prod/erc/ERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/erc/IndexERC20.py` & `uniswappy-1.5.1/python/prod/erc/IndexERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/erc/LPERC20.py` & `uniswappy-1.5.1/python/prod/erc/LPERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/interest/Yield.py` & `uniswappy-1.5.1/python/prod/math/interest/Yield.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/interest/ips/ConstantIPS.py` & `uniswappy-1.5.1/python/prod/math/interest/ips/ConstantIPS.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/model/BrownianModel.py` & `uniswappy-1.5.1/python/prod/math/model/BrownianModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/model/ModelQueue.py` & `uniswappy-1.5.1/python/prod/math/model/ModelQueue.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/model/TimeDeltaModel.py` & `uniswappy-1.5.1/python/prod/math/model/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/model/TokenDeltaModel.py` & `uniswappy-1.5.1/python/prod/math/model/TokenDeltaModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/math/risk/MaxDrop.py` & `uniswappy-1.5.1/python/prod/math/risk/MaxDrop.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/burn/IndexTokenBurn.py` & `uniswappy-1.5.1/python/prod/process/burn/IndexTokenBurn.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/deposit/SwapDeposit.py` & `uniswappy-1.5.1/python/prod/process/deposit/SwapDeposit.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/join/Join.py` & `uniswappy-1.5.1/python/prod/process/join/Join.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/liquidity/AddLiquidity.py` & `uniswappy-1.5.1/python/prod/process/liquidity/AddLiquidity.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/liquidity/RemoveLiquidity.py` & `uniswappy-1.5.1/python/prod/process/liquidity/RemoveLiquidity.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/mint/SwapIndexMint.py` & `uniswappy-1.5.1/python/prod/process/mint/SwapIndexMint.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/swap/RandomSwap.py` & `uniswappy-1.5.1/python/prod/process/swap/RandomSwap.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/swap/Swap.py` & `uniswappy-1.5.1/python/prod/process/swap/Swap.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/process/swap/WithdrawSwap.py` & `uniswappy-1.5.1/python/prod/process/swap/WithdrawSwap.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/Arbitrage.py` & `uniswappy-1.5.1/python/prod/simulate/Arbitrage.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/CorrectReserves.py` & `uniswappy-1.5.1/python/prod/simulate/CorrectReserves.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/MarkovState.py` & `uniswappy-1.5.1/python/prod/simulate/MarkovState.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/QuantTerminal.py` & `uniswappy-1.5.1/python/prod/simulate/QuantTerminal.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/SimpleLPSimulation.py` & `uniswappy-1.5.1/python/prod/simulate/SimpleLPSimulation.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/simulate/SolveDeltas.py` & `uniswappy-1.5.1/python/prod/simulate/SolveDeltas.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/client/API0x.py` & `uniswappy-1.5.1/python/prod/utils/client/API0x.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/data/Chain0x.py` & `uniswappy-1.5.1/python/prod/utils/data/Chain0x.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/data/UniswapExchangeData.py` & `uniswappy-1.5.1/python/prod/utils/data/UniswapExchangeData.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/MockAddress.py` & `uniswappy-1.5.1/python/prod/utils/tools/MockAddress.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/FullMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/FullMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/LiquidityMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/LiquidityMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/Position.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/Position.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/SafeMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/SafeMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/Shared.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/Shared.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/SqrtPriceMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/SqrtPriceMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/SwapMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/SwapMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/Tick.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/Tick.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/TickMath.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/TickMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Helper.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/UniV3Helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             tick_p -= R        
  
         return tick_p   
     
     def price_to_tick(self, p):
         return math.floor(math.log(p, 1.0001))    
 
+    def tick_to_price(self, tick):
+        return 1.0001**tick   
+
     def price_to_sqrtp(self, p):
         return int(math.sqrt(p) * Q96)    
 
     def sqrtp_to_price(self, sqrtp):
         return sqrtp/2**99  
 
     def dec2gwei(self, tkn_amt, precision=None):
```

### Comparing `uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Utils.py` & `uniswappy-1.5.1/python/prod/utils/tools/v3/UniV3Utils.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.5.0/setup.py` & `uniswappy-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='UniswapPy',
-      version='1.5.0',
+      version='1.5.1',
       description='Uniswap Analytics with Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/defipy-devs/uniswappy',
       author = "icmoore",
       author_email = "defipy.devs@gmail.com",
       license='MIT',
```

