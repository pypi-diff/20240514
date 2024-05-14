# Comparing `tmp/optrabot-0.9.2a1.tar.gz` & `tmp/optrabot-0.9.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.9.2a1.tar", max compression
+gzip compressed data, was "optrabot-0.9.3a0.tar", max compression
```

## Comparing `optrabot-0.9.2a1.tar` & `optrabot-0.9.3a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.2a1/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.2a1/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.2a1/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.2a1/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.2a1/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.2a1/optrabot/alembic.ini
--rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.2a1/optrabot/config.py
--rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.2a1/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.2a1/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-05-07 18:46:58.969402 optrabot-0.9.2a1/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.2a1/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.2a1/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.2a1/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10733 2024-05-08 11:10:23.701664 optrabot-0.9.2a1/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.2a1/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.2a1/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.2a1/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.2a1/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-05-08 06:34:31.950408 optrabot-0.9.2a1/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.2a1/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.2a1/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.2a1/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.2a1/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    49985 2024-05-08 11:10:23.702123 optrabot-0.9.2a1/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      845 2024-05-08 11:21:42.865668 optrabot-0.9.2a1/pyproject.toml
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 optrabot-0.9.2a1/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.3a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.3a0/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.3a0/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.3a0/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.3a0/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.3a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.3a0/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.3a0/optrabot/config.py
+-rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.3a0/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.3a0/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-05-07 18:46:58.969402 optrabot-0.9.3a0/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.3a0/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.3a0/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.3a0/optrabot/optionhelper.py
+-rw-r--r--   0        0        0    10909 2024-05-14 15:03:40.795427 optrabot-0.9.3a0/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.3a0/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.3a0/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.3a0/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.3a0/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-08 06:34:31.950408 optrabot-0.9.3a0/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.3a0/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.3a0/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.3a0/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.3a0/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    50485 2024-05-14 15:03:40.796044 optrabot-0.9.3a0/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      845 2024-05-14 18:48:59.093747 optrabot-0.9.3a0/pyproject.toml
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 optrabot-0.9.3a0/PKG-INFO
```

### Comparing `optrabot-0.9.2a1/README.md` & `optrabot-0.9.3a0/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/alembic/env.py` & `optrabot-0.9.3a0/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/alembic/script.py.mako` & `optrabot-0.9.3a0/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.9.3a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/alembic.ini` & `optrabot-0.9.3a0/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/config.py` & `optrabot-0.9.3a0/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/crud.py` & `optrabot-0.9.3a0/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/database.py` & `optrabot-0.9.3a0/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/main.py` & `optrabot-0.9.3a0/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/marketdatatype.py` & `optrabot-0.9.3a0/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/models.py` & `optrabot-0.9.3a0/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/optionhelper.py` & `optrabot-0.9.3a0/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/optrabot.py` & `optrabot-0.9.3a0/optrabot/optrabot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import array
 from collections import OrderedDict
 import asyncio
 import datetime as dt
 import json
 from fastapi import FastAPI
 from ib_insync import *
+import logging
 from loguru import logger
 from sqlalchemy.orm import Session
 from optrabot import schemas
 from optrabot.marketdatatype import MarketDataType
 from optrabot.optionhelper import OptionHelper
 from optrabot.config import Config
 from .tradinghubclient import TradinghubClient
@@ -23,16 +24,17 @@
 		self._apiKey = None
 		self.thc : TradinghubClient = None
 		self._tradingEnabled = False
 		self._marketDataType : MarketDataType = None
 		self.Version = pkg_resources.get_distribution('optrabot').version
 		self._backgroundScheduler = AsyncIOScheduler()
 		self._backgroundScheduler.start()
+		logging.getLogger('apscheduler').setLevel(logging.ERROR) # Prevents unnecessary logging from apscheduler
 		if self.Version == '0.1.0':
-			self.Version = '0.8.1' # Set Version to 0.8.1 for the loca development environment
+			self.Version = '0.9.3' # Set Version to 0.8.1 for the loca development environment
 
 	def __setitem__(self, key, value):
 		setattr(self, key, value)
 
 	def __getitem__(self, key):
 		return getattr(self, key)
 	
@@ -116,14 +118,15 @@
 		try:
 			ib: IB = self['ib']
 			ib.errorEvent += self.onErrorEvent
 			await ib.connectAsync(twshost, twsport, clientId=twsclient)
 			logger.debug("Connected to IB")
 			ib.disconnectedEvent += self.onDisconnected
 			ib.execDetailsEvent += self.thc.onExecDetailsEvent
+			ib.orderStatusEvent += self.thc.onOrderStatusEvent
 			ib.commissionReportEvent += self.thc.onCommissionReportEvent
 			with Session(get_db_engine()) as session:
 				for managedAccount in ib.managedAccounts():
 					logger.debug('Managed Account: {}', managedAccount)
 					known_account = crud.get_account(session, managedAccount)
 					if known_account == None:
 						logger.debug('Account is new. Adding it to the Database')
```

### Comparing `optrabot-0.9.2a1/optrabot/schemas.py` & `optrabot-0.9.3a0/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/stoplossadjuster.py` & `optrabot-0.9.3a0/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/tradehelper.py` & `optrabot-0.9.3a0/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/tradetemplate/template.py` & `optrabot-0.9.3a0/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.9.3a0/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.9.3a0/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.2a1/optrabot/tradinghubclient.py` & `optrabot-0.9.3a0/optrabot/tradinghubclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 		self._ironFlyAskPrice = 0.0
 		self._ironFlyComboContract = None
 		self._ironFlyContracts = None
 		self._ironFlyLongLegContracts = None
 		self._ironFlyShortComboContract = None
 		self._longLegFillsPrice = 0.0
 		self._longLegFillsReceived = 0
+		self._previousIronFlyPrice = 0.0
+		self._unchangedIronFlyPriceCounter = 0
 		self._shuttingdown = False
 		#self._positionMonitorTask = None
 		self._position = False
 		self._closingLongLegs = False
 		self._fillTransactionMap = {}
 		self._entryOrderFilled = 0   # Number of fills for the entry order
 		
@@ -243,15 +245,14 @@
 			if longCallContract.strike != longCallStrike:
 				logger.warning('Using different Long Call strike {}, because of existing open orders on desired strike {}.', longCallContract.strike, longCallStrike)
 
 			self._ironFlyLongLegContracts = [longCallContract, longPutContract]
 			self._ironFlyContracts = [shortPutContract, shortCallContract, longPutContract, longCallContract]
 			self._ironFlyComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
 			self._ironFlyShortComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
-
 			ironFlyMidPrice = None
 			for i in range(5):
 				tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
 				logger.debug("Tickers {}", tickers)
 				ironFlyMidPrice = self._calculateIronFlyMidPrice(tickers, ironFlyComboContract=self._ironFlyComboContract, 
 											   ironFlyShortComboContract=self._ironFlyShortComboContract, 
 											   shortPutContract=shortPutContract,
@@ -280,25 +281,26 @@
 				newTrade = schemas.TradeCreate(account=accountNo, symbol='SPX', strategy=self._currentTemplate.strategy)
 				self._currentTrade = crud.create_trade(session, newTrade)
 				order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + template.name + ' - Open'
 			order.account = accountNo
 			order.outsideRth = True
 			self._fillTransactionMap.clear()
 			self._entryTrade = ib.placeOrder(self._ironFlyComboContract, order)
-			self._entryTrade.statusEvent += self.onOrderStatusEvent
 			self._entryTradeContract = self._ironFlyComboContract
 			self._ironFlyAskPrice = 0.0
 			self._longLegFillsPrice = 0.0
+			self._previousIronFlyPrice = 0.0
+			self._unchangedIronFlyPriceCounter = 0
 			self._longLegFillsReceived = 0
 			self._slShortTrade = None
 			self._tpTrade = None
 			self._entryOrderFilled = 0
 			self._closingLongLegs = False
 			logger.debug("Account: {} Trade placed: {} Number of contracts: {}", order.account, self._entryTrade, amount)
-			asyncio.create_task(self._trackEntryOrder()).add_done_callback(self.optraBot.handleTaskDone)
+			self.optraBot._backgroundScheduler.add_job(self._trackEntryOrder, 'interval', seconds=5, id='TrackEntryOrder')
 
 		except Exception as excp:
 						logger.error("Exception: {}", excp)
 
 	async def _poll_old(self):
 		try:
 			fetch_url = self.hub_host + '/fetch_signal'
@@ -475,25 +477,23 @@
 							newTrade = schemas.TradeCreate(account=accountNo, symbol='SPX', strategy=self._currentTemplate.strategy)
 							self._currentTrade = crud.create_trade(session, newTrade)
 							order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + triggeredTemplate.name + ' - Open'
 						order.account = accountNo
 						order.outsideRth = True
 						self._fillTransactionMap.clear()
 						self._entryTrade = ib.placeOrder(self._ironFlyComboContract, order)
-						self._entryTrade.statusEvent += self.onOrderStatusEvent
 						self._entryTradeContract = self._ironFlyComboContract
 						self._ironFlyAskPrice = 0.0
 						self._longLegFillsPrice = 0.0
 						self._longLegFillsReceived = 0
 						self._slShortTrade = None
 						self._tpTrade = None
 						self._entryOrderFilled = 0
 						self._closingLongLegs = False
 						logger.debug("Account: {} Trade placed: {} Number of contracts: {}", order.account, self._entryTrade, amount)
-						asyncio.create_task(self._trackEntryOrder()).add_done_callback(self.optraBot.handleTaskDone)
 
 				except Exception as excp:
 						logger.error("Exception: {}", excp)
 
 		except Exception as anyEcxp:
 			logger.error("Exception occured during poll: {}", anyEcxp)
 
@@ -544,37 +544,39 @@
 				if not util.isNan(ticker.ask):
 					self._ironFlyAskPrice += ticker.ask
 					ironFlyComboContract.comboLegs.append(ComboLeg(conId=longCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
 		self._ironFlyAskPrice = OptionHelper.roundToTickSize(self._ironFlyAskPrice)
 		return OptionHelper.roundToTickSize(ironFlyMidPrice)
 
 	async def _trackEntryOrder(self):
-		await asyncio.sleep(5) # Wait 5 seconds for order Execution
 		ib: IB = self.optraBot['ib']
 		if self._entryTrade == None:
+			logger.debug("Stopping Entry Order Tracking")
+			self.optraBot._backgroundScheduler.remove_job('TrackEntryOrder')
 			return
 		
 		if self._entryTrade.orderStatus.status == OrderStatus.Cancelled or self._entryTrade.orderStatus.status == OrderStatus.Inactive:
 			self._onEntryOrderCanceled()
 		elif self._entryTrade.orderStatus.status == OrderStatus.Filled:
 			logger.info("Entry Order has been filled already. No adjustment required")
+			logger.debug("Stopping Entry Order Tracking")
+			self.optraBot._backgroundScheduler.remove_job('TrackEntryOrder')
 		elif self._entryTrade.orderStatus.status == OrderStatus.PreSubmitted or self._entryTrade.orderStatus.status == OrderStatus.PendingSubmit:
 			logger.info("Entry Order is still in PreSubmitted state. Waiting for it to be submitted...")
 		elif self._entryTrade.orderStatus.status == OrderStatus.Submitted:
 			currentLimitPrice = self._entryTrade.order.lmtPrice
 			adjustedLimitPrice = currentLimitPrice + self._currentTemplate.adjustmentStep
 			logger.info("Entry Order status ({}). Entry price will be adjusted. Current Limit Price: ${}", self._entryTrade.orderStatus.status, currentLimitPrice)
 			if self._meetsMinimumPremium(adjustedLimitPrice) and adjustedLimitPrice <= self._ironFlyAskPrice:
-				#self.entryOrderAdjustments += 1	
 				self._entryTrade.order.lmtPrice = adjustedLimitPrice
 				try:
 					ib.placeOrder(self._entryTradeContract, self._entryTrade.order)
-					asyncio.create_task(self._trackEntryOrder()).add_done_callback(self.optraBot.handleTaskDone)
 				except Exception as excp:
 					logger('Exception beim Anpassen der Order')
+				return
 			else:
 				if adjustedLimitPrice > -15:
 					logger.info("Entry order limit price reached minimum premium. No entry.")
 				if adjustedLimitPrice > self._ironFlyAskPrice:
 					logger.info("Entry order limit price exceeded initial ask price. No entry.")
 				ib.cancelOrder(self._entryTrade.order)
 		else:
@@ -600,39 +602,39 @@
 					logger.info('Entry Order has been filled at ${} (Qty: {}) and trade is running now.', trade.orderStatus.avgFillPrice, trade.orderStatus.filled)
 					self._position = True
 					if self._currentTemplate.stopLossAdjuster:
 						self._currentTemplate.stopLossAdjuster.setBasePrice(round(self._entryTrade.orderStatus.avgFillPrice * -1, 2))
 					asyncio.create_task(self._placeTakeProfitAndStop(trade)).add_done_callback(self.optraBot.handleTaskDone)
 					#Run 1. Position Monitoring with delay
 					#asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
-					self.optraBot._backgroundScheduler.add_job(self._monitorPosition, 'interval', seconds=10, id='MonitorPosition')
+					self.optraBot._backgroundScheduler.add_job(self._monitorPosition, 'interval', seconds=5, id='MonitorPosition')
 				elif self._position == True:
 					logger.debug('Additionally fill quantity (Qty: {}) for the entry order...depending orders need to be adjusted.', trade.orderStatus.filled)
 					asyncio.create_task(self._adjustTakeProfitAndStop(trade)).add_done_callback(self.optraBot.handleTaskDone)
 
 				if trade.orderStatus.remaining > 0:
 					logger.warning('Partial fill for entry order. Remaining: {}', trade.orderStatus.remaining)
 				executedAmount = trade.orderStatus.filled - self._entryOrderFilled
 				logger.debug('Executed amount for entry trade: {}', executedAmount)
 				if executedAmount > 0:
 					asyncio.create_task(self._reportExecutedTrade(trade, executedAmount)).add_done_callback(self.optraBot.handleTaskDone)
 				self._entryOrderFilled = self._entryTrade.order.totalQuantity - trade.orderStatus.remaining
 
-		elif trade == self._tpTrade:
+		elif self._tpTrade and trade.order.orderId == self._tpTrade.order.orderId:
 			logger.debug('TP Order Status has been raised. Status: {}', trade.orderStatus.status)
 			if trade.orderStatus.status == OrderStatus.Cancelled:
 				logger.info('TP Order has been cancelled!')
 
 			elif trade.orderStatus.status == OrderStatus.Filled:
 				logger.success('TP Order has been filled. Trade finished')
 				self._tpTrade = None
 				self._slShortTrade = None
 				self._onPositionClose()
 
-		elif trade == self._slShortTrade:
+		elif self._slShortTrade and trade.order.orderId == self._slShortTrade.order.orderId:
 			logger.debug('SL order for Short Legs status has been changed. Status: {}', trade.orderStatus.status)
 			if trade.orderStatus.status == OrderStatus.Cancelled:
 				logEntry: TradeLogEntry = None
 				for logEntry in trade.log:
 					if logEntry.status != 'Cancelled':
 						continue
 				if logEntry == None:
@@ -659,15 +661,14 @@
 		logger.info('Entry Order has been cancelled!')
 		self._entryTrade = None
 		logger.debug('Deleting trade {} from database...', self._currentTrade.id )
 		with Session(get_db_engine()) as session:
 			crud.delete_trade(session, self._currentTrade)
 		self._currentTrade = None
 
-
 	async def _getAllOpenOrderContracts(self, account, symbol) -> List:
 		"""
 		Determine the ContractIds of all open Orders for the given account and symbol
 		"""
 		ib: IB = self.optraBot['ib']
 		openTrades: List[Trade] = await ib.reqAllOpenOrdersAsync()
 		openOrderContracts = list()
@@ -807,28 +808,26 @@
 		order = LimitOrder('SELL', fillAmount, limitPrice)
 		order.account = self._currentTemplate.account
 		order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - Take Profit'
 		order.ocaGroup = ocaGroup
 		order.outsideRth = True
 		self._tpTrade = ib.placeOrder(self._ironFlyComboContract, order)
 		logger.debug('Created TP order with id: {}', self._tpTrade.order.orderId)
-		self._tpTrade.statusEvent += self.onOrderStatusEvent
 
 		# Calculation of Stop Price
 		stopFactor = ((self._currentTemplate.stopLoss / 100) + 1) * -1
 		self._ironFlyStopPrice = OptionHelper.roundToTickSize(fillPrice * stopFactor)
 		logger.info('Stop LossPrice ({}%): {}', self._currentTemplate.stopLoss, self._ironFlyStopPrice)
 
 		stopShortsOrder = StopOrder('BUY', self._entryTrade.orderStatus.filled, self._ironFlyStopPrice)
 		stopShortsOrder.account = self._currentTemplate.account
 		stopShortsOrder.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - SL Short Legs'
 		stopShortsOrder.ocaGroup = ocaGroup
 		try:
 			self._slShortTrade = ib.placeOrder(self._ironFlyShortComboContract, stopShortsOrder)
-			self._slShortTrade.statusEvent += self.onOrderStatusEvent
 		except Exception as excp:
 			logger('Exception beim Erstellen der Short Leg Stoploss order')
 
 	async def _adjustTakeProfitAndStop(self, trade: Trade):
 		""" Adjust Take Profit and Stop Order after another partial fill of the entry Order.
 		"""
 		ib: IB = self.optraBot['ib']
@@ -895,81 +894,92 @@
 			#self._positionMonitorTask = None
 			self._stopPositionMonitoring()
 			return
 
 		#asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
 
 		ib: IB = self.optraBot['ib']
-		if not ib.isConnected():
+		if not ib.isConnected() or self.optraBot.isTradingEnabled() == False:
 			logger.error('Interactive Brokers is not connected. Unable to monitor position!')
 			return
 		
-		if self._position == False:
-			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
-			return
+		try:
+			if self._position == False:
+				logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+				return
 
-		tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
-		longLegsValue = 0
-		currentIronFlyAskPrice = 0
-		currentIronFlyBidPrice = 0
-		adjustedStopLossPrice = None
-		for ticker in tickers:
-			if ticker.contract in self._ironFlyLongLegContracts:
-				if ticker.bid >= 0:
-					longLegsValue += ticker.bid
-					currentIronFlyBidPrice -= ticker.bid
-					currentIronFlyAskPrice += ticker.ask
-			else:
-				# Für Short Legs müssen die Ask Preise addiert werden
-				currentIronFlyBidPrice += ticker.ask
-				currentIronFlyAskPrice -= ticker.bid
-	
-		if self._position == False:
-			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
-			return
+			tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
+			longLegsValue = 0
+			currentIronFlyAskPrice = 0
+			currentIronFlyBidPrice = 0
+			adjustedStopLossPrice = None
+			for ticker in tickers:
+				if ticker.contract in self._ironFlyLongLegContracts:
+					if ticker.bid >= 0:
+						longLegsValue += ticker.bid
+						currentIronFlyBidPrice -= ticker.bid
+						currentIronFlyAskPrice += ticker.ask
+				else:
+					# Für Short Legs müssen die Ask Preise addiert werden
+					currentIronFlyBidPrice += ticker.ask
+					currentIronFlyAskPrice -= ticker.bid
+		
+			if self._position == False:
+				logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+				return
 
-		if self._currentTemplate.stopLossAdjuster:
-			if not self._currentTemplate.stopLossAdjuster.isTriggered():
-				# Ask Preis muss positiv gemacht werden
-				currentIronFlyAskPrice = abs(currentIronFlyAskPrice)
-				currentIronFlyPrice = OptionHelper.calculateMidPrice(currentIronFlyBidPrice, currentIronFlyAskPrice)
-				#currentIronFlyPrice = round(currentIronFlyPrice, 2)
-				adjustedStopLossPrice = self._currentTemplate.stopLossAdjuster.execute(currentIronFlyPrice)
-				if adjustedStopLossPrice == None:
-					logger.debug('No need to adjust stop loss now.')
+			currentIronFlyAskPrice = abs(currentIronFlyAskPrice)
+			currentIronFlyPrice = OptionHelper.calculateMidPrice(currentIronFlyBidPrice, currentIronFlyAskPrice)
+			if currentIronFlyPrice == self._previousIronFlyPrice:
+				self._unchangedIronFlyPriceCounter += 1
+			else:
+				self._unchangedIronFlyPriceCounter = 0
+			self._previousIronFlyPrice = currentIronFlyPrice
+			if self._unchangedIronFlyPriceCounter > 10:
+				logger.warning('Price of Iron Fly has not changed for 10 times. There is a problem with price data from TWS probably.')
+				self._unchangedIronFlyPriceCounter = 0
+
+			if self._currentTemplate.stopLossAdjuster:
+				if not self._currentTemplate.stopLossAdjuster.isTriggered():
+					adjustedStopLossPrice = self._currentTemplate.stopLossAdjuster.execute(currentIronFlyPrice)
+					if adjustedStopLossPrice == None:
+						logger.debug('No need to adjust stop loss now.')
+					else:
+						self._ironFlyStopPrice = adjustedStopLossPrice
+						logger.info('Performing stop loss adjustment. New Stop Loss price: {}', self._ironFlyStopPrice)
 				else:
-					self._ironFlyStopPrice = adjustedStopLossPrice
-					logger.info('Performing stop loss adjustment. New Stop Loss price: {}', self._ironFlyStopPrice)
+					logger.debug('Stoploss adjustment has been performed already.')
 			else:
-				logger.debug('Stoploss adjustment has been performed already.')
-		else:
-			logger.debug('No StopLoss adjustment configured.')
-		desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice + longLegsValue)
-		currentStopPrice = OptionHelper.roundToTickSize(self._slShortTrade.order.auxPrice)
-		logger.debug('Long Legs value {} Current Short SL Price: {} Desired Short SL Pice: {}', round(longLegsValue,2), currentStopPrice, desiredStopPrice)
-		openTrades = await ib.reqOpenOrdersAsync()
-
-		if self._position == False:
-			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
-			return
-
-		if self._slShortTrade in openTrades:
-			if self._slShortTrade.isActive():
-				if currentStopPrice != desiredStopPrice:
-					self._slShortTrade.order.auxPrice = desiredStopPrice
-					logger.info('Adjusting Stop Loss price to ${}', desiredStopPrice)
-					ib.placeOrder(self._slShortTrade.contract, self._slShortTrade.order)
-					logger.debug('Updated SL order with id: {}', self._slShortTrade.order.orderId)
+				logger.debug('No StopLoss adjustment configured.')
+			desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice + longLegsValue)
+			currentStopPrice = OptionHelper.roundToTickSize(self._slShortTrade.order.auxPrice)
+			logger.debug('Long Legs value {} Current Short SL Price: {} Desired Short SL Pice: {}', round(longLegsValue,2), currentStopPrice, desiredStopPrice)
+			openOrders = ib.openOrders()
+
+			if self._position == False:
+				logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+				return
+			if any(order.orderId == self._slShortTrade.order.orderId for order in openOrders):
+			#if self._slShortTrade.order in openOrders:
+				if self._slShortTrade.isActive():
+					if currentStopPrice != desiredStopPrice:
+						self._slShortTrade.order.auxPrice = desiredStopPrice
+						logger.info('Adjusting Stop Loss price to ${}', desiredStopPrice)
+						ib.placeOrder(self._slShortTrade.contract, self._slShortTrade.order)
+						logger.debug('Updated SL order with id: {}', self._slShortTrade.order.orderId)
+					else:
+						logger.debug('No adjustment of Stop Loss price required.')
 				else:
-					logger.debug('No adjustment of Stop Loss price required.')
+					logger.debug('SL Order is not active anymore.')
 			else:
-				logger.debug('SL Order is not active anymore.')
-		else:
-			logger.warning('Caution: Stop Loss order for Short Strikes is missing. Trying to reestablish the Stop Loss order now!')
-			await self._reestablishStopLossOrder(desiredStopPrice)
+				logger.warning('Caution: Stop Loss order for Short Strikes is missing. Trying to reestablish the Stop Loss order now!')
+				await self._reestablishStopLossOrder(desiredStopPrice)
+		except ConnectionError as connError:
+			logger.error('Connection to TWS lost during Position Monitoring. Unable to monitor position!')
+
 		logger.debug('Leave Monitor position()')
 
 	async def _monitorPositionDelayed(self):
 		logger.debug('Waiting 10 seconds for next position monitoring.')
 		await asyncio.sleep(10)
 		if self._position == True:
 			asyncio.create_task(self._monitorPosition(), name='MonitorPosition').add_done_callback(self.optraBot.handleTaskDone)
@@ -988,15 +998,14 @@
 		ocaGroup = self._currentTemplate.account + '_' + now.strftime('%H%M%S')
 		stopShortsOrder = StopOrder('BUY', self._entryTrade.orderStatus.filled, desiredStopPrice)
 		stopShortsOrder.account = self._currentTemplate.account
 		stopShortsOrder.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - SL Short Legs'
 		stopShortsOrder.ocaGroup = ocaGroup
 		try:
 			self._slShortTrade = ib.placeOrder(self._ironFlyShortComboContract, stopShortsOrder)
-			self._slShortTrade.statusEvent += self.onOrderStatusEvent
 		except Exception as excp:
 			logger('Exception beim Erstellen der Short Leg Stoploss order')
 		logger.info('Stop Loss order for Short Legs has been reestablished.')
 
 		# Check if Take Profit Order is still in place and recreate it, if it's missing
 		openTrades = await ib.reqOpenOrdersAsync()
 		if self._tpTrade in openTrades:
@@ -1006,15 +1015,14 @@
 			order = LimitOrder('SELL', self._tpTrade.order.totalQuantity, self._tpTrade.order.lmtPrice)
 			order.account = self._currentTemplate.account
 			order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - Take Profit'
 			order.ocaGroup = ocaGroup
 			order.outsideRth = True
 			self._tpTrade = ib.placeOrder(self._ironFlyComboContract, order)
 			logger.debug('Created TP order with id: {}', self._tpTrade.order.orderId)
-			self._tpTrade.statusEvent += self.onOrderStatusEvent
 
 	def _meetsMinimumPremium(self, premium: float) -> bool:
 		""" Checks if given premium meets minimum premium
 
 		Parameters
 		----------
 		premium : float
```

### Comparing `optrabot-0.9.2a1/pyproject.toml` & `optrabot-0.9.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.9.2a1"
+version = "0.9.3a0"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.9.2a1/PKG-INFO` & `optrabot-0.9.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.9.2a1
+Version: 0.9.3a0
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

