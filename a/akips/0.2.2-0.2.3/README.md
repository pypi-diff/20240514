# Comparing `tmp/akips-0.2.2.tar.gz` & `tmp/akips-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akips-0.2.2.tar", max compression
+gzip compressed data, was "akips-0.2.3.tar", max compression
```

## Comparing `akips-0.2.2.tar` & `akips-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.2.2/LICENSE
--rw-r--r--   0        0        0     1458 2023-09-25 15:32:31.817902 akips-0.2.2/README.md
--rw-r--r--   0        0        0    13027 2024-05-02 18:18:47.198493 akips-0.2.2/akips/__init__.py
--rw-r--r--   0        0        0      254 2023-09-22 19:01:52.560879 akips-0.2.2/akips/exceptions.py
--rw-r--r--   0        0        0      515 2024-05-13 16:08:05.304440 akips-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 akips-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1557 2024-05-13 16:49:22.855266 akips-0.2.3/README.md
+-rw-r--r--   0        0        0    13767 2024-05-14 11:26:53.820084 akips-0.2.3/akips/__init__.py
+-rw-r--r--   0        0        0      256 2024-05-14 09:34:33.270139 akips-0.2.3/akips/exceptions.py
+-rw-r--r--   0        0        0      560 2024-05-14 11:26:15.042024 akips-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 akips-0.2.3/PKG-INFO
```

### Comparing `akips-0.2.2/LICENSE` & `akips-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akips-0.2.2/README.md` & `akips-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,11 +35,14 @@
 
 devices = api.get_devices()
 for name, fields in devices.items():
     print("Device: {} {}".format(name,fields))
 
 ```
 
+## API Documentation
+[API Documentation](https://wwhitaker.github.io/akips/docs/akips/index.html)
+
 ## Bugs/Requests
 
 Please use the [GitHub issue tracker](https://github.com/wwhitaker/akips/issues) 
 to submit bugs or request features.
```

### Comparing `akips-0.2.2/akips/__init__.py` & `akips-0.2.3/akips/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-''' Base module '''
-__version__ = '0.2.2'
+""" This akips python module provides a simple way for python scripts to interact with
+the AKiPS Network Monitoring Software Web API interface. """
+__version__ = '0.2.3'
 
 import io
 import re
 import logging
 from datetime import datetime
 import requests
 import pytz
@@ -12,42 +13,42 @@
 from akips.exceptions import AkipsError
 
 # Logging configuration
 logger = logging.getLogger(__name__)
 
 
 class AKIPS:
-    ''' Class to handle interactions with AKiPS API '''
-    server_timezone = 'America/New_York'
+    """ Class to handle interactions with AKiPS API """
 
-    def __init__(self, server, username='api-ro', password=None, verify=True):
-        ''' Connect to the AKiPS instance '''
+    def __init__(self, server, username='api-ro', password=None,
+                 verify=True, timezone='America/New_York'):
         self.server = server
         self.username = username
         self.password = password
         self.verify = verify
+        self.server_timezone = timezone
         self.session = requests.Session()
 
         if not verify:
             requests.packages.urllib3.disable_warnings()    # pylint: disable=no-member
 
     def get_devices(self, group_filter='any', groups=[]):
-        ''' Pull a list of key attributes for all devices in akips '''
+        """ Pull a list of key attributes for all devices in akips """
         attributes = [
             'ip4addr',
             'SNMPv2-MIB.sysName',
             'SNMPv2-MIB.sysDescr',
             'SNMPv2-MIB.sysLocation'
         ]
         cmd_attributes = "|".join(attributes)
         params = {
             'cmds': f'mget text * sys /{cmd_attributes}/',
         }
         if groups:
-            ''' [any|all|not group {group name} ...] '''
+            """ [any|all|not group {group name} ...] """
             group_list = " ".join(groups)
             params['cmds'] += f" {group_filter} group {group_list}"
         text = self._get(params=params)
         if text:
             data = {}
             # Data comes back as 'plain/text' type so we have to parse it
             lines = text.split('\n')
@@ -60,15 +61,15 @@
                     # Save this attribute value to data
                     data[match.group(1)][match.group(3)] = match.group(4)
             logger.debug("Found {} devices in akips".format(len(data.keys())))
             return data
         return None
 
     def get_device(self, name):
-        ''' Pull the entire configuration for a single device '''
+        """ Pull the entire configuration for a single device """
         params = {
             'cmds': f'mget * {name} * *'
         }
         text = self._get(params=params)
         if text:
             data = {}
             # Data comes back as 'plain/text' type so we have to parse it.  Example:
@@ -89,81 +90,75 @@
             if name:
                 data['name'] = name
             logger.debug("Found device {} in akips".format(data))
             return data
         return None
 
     def get_device_by_ip(self, ipaddr, use_cache=True):
-        ''' Search for a device by an alternate IP address
-        This makes use of a special site script and not the normal api '''
+        """ Search for a device by an alternate IP address
+        This makes use of a special site script and not the normal api """
         # params = {
         #     'function': 'web_find_device_by_ip',
         #     'ipaddr': ipaddr
         # }
         # section = '/api-script/'
         pass
 
     def get_unreachable(self):
-        ''' Pull a list of unreachable IPv4 ping devices '''
+        """ Pull a list of unreachable IPv4 ping devices """
         params = {
             'cmds': 'mget * * * /PING.icmpState|SNMP.snmpState/ value /down/',
         }
         text = self._get(params=params)
         data = {}
         if text:
             lines = text.split('\n')
             for line in lines:
                 match = re.match(r'^(\S+)\s(\S+)\s(\S+)\s=\s(\S+),(\S+),(\S+),(\S+),(\S+)?$', line)
                 if match:
                     # epoch fields are in the server's timezone
                     name = match.group(1)
                     attribute = match.group(3)
-                    event_start = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
+                    event_start = datetime.fromtimestamp(
+                        int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                     if name not in data:
                         # populate a starting point for this device
                         data[name] = {
                             'name': name,
                             'ping_state': 'n/a',
                             'snmp_state': 'n/a',
                             'event_start': event_start  # epoch in local timezone
                         }
                     if attribute == 'PING.icmpState':
                         data[name]['child'] = match.group(2),
                         data[name]['ping_state'] = match.group(5)
                         data[name]['index'] = match.group(4)
-                        data[name]['device_added'] = datetime.fromtimestamp(int(match.group(6)), tz=pytz.timezone(self.server_timezone))
-                        data[name]['event_start'] = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['device_added'] = datetime.fromtimestamp(
+                            int(match.group(6)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['event_start'] = datetime.fromtimestamp(
+                            int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                         data[name]['ip4addr'] = match.group(8)
                     elif attribute == 'SNMP.snmpState':
                         data[name]['child'] = match.group(2),
                         data[name]['snmp_state'] = match.group(5)
                         data[name]['index'] = match.group(4)
-                        data[name]['device_added'] = datetime.fromtimestamp(int(match.group(6)), tz=pytz.timezone(self.server_timezone))
-                        data[name]['event_start'] = datetime.fromtimestamp(int(match.group(7)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['device_added'] = datetime.fromtimestamp(
+                            int(match.group(6)), tz=pytz.timezone(self.server_timezone))
+                        data[name]['event_start'] = datetime.fromtimestamp(
+                            int(match.group(7)), tz=pytz.timezone(self.server_timezone))
                         data[name]['ip4addr'] = None
                     if event_start < data[name]['event_start']:
                         data[name]['event_start'] = event_start
             logger.debug("Found {} devices in akips".format(len(data)))
             logger.debug("data: {}".format(data))
 
-        # for name in data:
-        #     # Fill in the unreported gaps so we have ping4 and snmp up/down data
-        #     if data[name]['ping_state'] == 'n/a':
-        #         ping_status = self.get_status(device=name, child='ping4', attribute='PING.icmpState')
-
-        #     if data[name]['snmp_state'] == 'n/a':
-        #         snmp_status = self.get_status(device=name, child='sys', attribute='SNMP.snmpState')
-
-        # ideal data return based on unreachable device report
-        # Device, Ping4 (state,IPv4), SNMP (state,IP), Last Change (... ago), Location, Description
-
         return data
 
     def get_group_membership(self):
-        ''' Pull a list of device to group memberships '''
+        """ Pull a list of device to group memberships """
         params = {
             'cmds': 'mgroup device *',
         }
         text = self._get(params=params)
         if text:
             data = {}
             # Data comes back as 'plain/text' type so we have to parse it
@@ -175,40 +170,40 @@
                         # Populate a default entry for all desired fields
                         data[match.group(1)] = match.group(2).split(',')
             logger.debug("Found {} device and group mappings in akips".format(len(data.keys())))
             return data
         return None
 
     def get_maintenance_mode(self):
-        ''' Pull a list of devices in maintenance mode '''
+        """ Pull a list of devices in maintenance mode """
         # params = {
         #     'cmds': 'mget * * any group maintenance_mode',
         # }
         pass
 
     def set_maintenance_mode(self, device_name, mode='True'):
-        ''' Set maintenance mode on or off for a device '''
+        """ Set maintenance mode on or off for a device """
         # params = {
         #     'function': 'web_manual_grouping',
         #     'type': 'device',
         #     'group': 'maintenance_mode',
         #     'device': device_name
         # }
         pass
 
     def get_status(self, device='*', child='*', attribute='*'):
-        ''' Pull the status values we are most interested in '''
+        """ Pull the status values we are most interested in """
         pass
 
     def get_events(self, event_type='all', period='last1h'):
-        ''' Pull a list of events.  Command syntax:
+        """ Pull a list of events.  Command syntax:
             mget event {all,critical,enum,threshold,uptime}
             time {time filter} [{parent regex} {child regex}
             {attribute regex}] [profile {profile name}]
-            [any|all|not group {group name} ...] '''
+            [any|all|not group {group name} ...] """
 
         params = {
             'cmds': f'mget event {event_type} time {period}'
         }
         text = self._get(params=params)
         if text:
             data = []
@@ -228,19 +223,20 @@
                     data.append(entry)
             logger.debug("Found {} events of type {} in akips".format(len(data), type))
             return data
         return None
 
     # Time-series commands
 
-    def get_series(self, period='last1h', device='*', attribute='*', group_filter='any', groups=[], get_dict=True):
-        ''' Pull a series of values.  Command syntax:
+    def get_series(self, period='last1h', device='*', attribute='*', get_dict=True,
+                   group_filter='any', groups=[]):
+        """ Pull a series of values.  Command syntax:
             cseries avg
             time {time filter} type parent child attribute
-            [any|all|not group {group name} ...] '''
+            [any|all|not group {group name} ...] """
         params = {
             'cmds': f'cseries avg time {period} * {device} * {attribute}'
         }
         if groups:
             group_list = " ".join(groups)
             params['cmds'] += f" {group_filter} group {group_list}"
         text = self._get(params=params)
@@ -254,19 +250,20 @@
                 # parse each row as a list, will have a column header row
                 reader = csv.reader(buff)
             csv_to_list = [row for row in reader]
             logger.debug("Found {} series entries".format(len(csv_to_list)))
             return csv_to_list
         return None
 
-    def get_aggregate(self, operator='avg', interval='300', period='last1h', device='*', attribute='*', group_filter='any', groups=[]):
-        ''' Aggregate stats in intervals over a period of time. Command syntax:
+    def get_aggregate(self, period='last1h', device='*', attribute='*',
+                      operator='avg', interval='300', group_filter='any', groups=[]):
+        """ Aggregate stats in intervals over a period of time. Command syntax:
             aggregate interval {avg|total seconds}
             time {time filter} type parent child attribute
-            [any|all|not group {group name} ...] '''
+            [any|all|not group {group name} ...] """
         params = {
             'cmds': f'aggregate interval {operator} {interval} time {period} * {device} * {attribute}'
         }
         if groups:
             group_list = " ".join(groups)
             params['cmds'] += f" {group_filter} group {group_list}"
         text = self._get(params=params)
@@ -276,16 +273,35 @@
             values = lines[0].split(',')
             logger.debug("Found {} aggregate values".format(len(values)))
             return values
         return None
 
     # Base operations
 
+    def _parse_enum(self, enum_string):
+        """ Attributes with a type of enum return five values separated by commas. """
+        match = re.match(r'^(\S*),(\S*),(\S*),(\S*),(\S*)$', enum_string)
+        if match:
+            entry = {
+                'number': match.group(1),       # list number (from MIB)
+                'value': match.group(2),        # text value (from MIB)
+                # 'created': match.group(3),      # time created (epoch timestamp)
+                # 'modified': match.group(4),     # time modified (epoch timestamp)
+                'description': match.group(5)   # child description
+            }
+            entry['created'] = datetime.fromtimestamp(
+                int(match.group(3)), tz=pytz.timezone(self.server_timezone))
+            entry['modified'] = datetime.fromtimestamp(
+                int(match.group(4)), tz=pytz.timezone(self.server_timezone))
+            return entry
+        else:
+            raise AkipsError(message=f'Not a ENUM type value: {enum_string}')
+
     def _get(self, section='/api-db/', params=None, timeout=30):
-        ''' Call HTTP GET against the AKiPS server '''
+        """ Call HTTP GET against the AKiPS server """
         server_url = 'https://' + self.server + section
         params['username'] = self.username
         params['password'] = self.password
 
         if 'cmds' in params:
             logger.debug("akips command: {}".format(params['cmds']))
         try:
```

### Comparing `akips-0.2.2/PKG-INFO` & `akips-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: akips
-Version: 0.2.2
+Version: 0.2.3
 Summary: Module to interact with the AKiPS Network Monitoring Software API interface
 Home-page: https://github.com/wwhitaker/akips
 License: MIT
 Author: William E Whitaker
 Author-email: will.whitaker@unc.edu
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytz
 Requires-Dist: requests (>=2.31)
 Project-URL: Repository, https://github.com/wwhitaker/akips
 Description-Content-Type: text/markdown
@@ -54,12 +55,15 @@
 
 devices = api.get_devices()
 for name, fields in devices.items():
     print("Device: {} {}".format(name,fields))
 
 ```
 
+## API Documentation
+[API Documentation](https://wwhitaker.github.io/akips/docs/akips/index.html)
+
 ## Bugs/Requests
 
 Please use the [GitHub issue tracker](https://github.com/wwhitaker/akips/issues) 
 to submit bugs or request features.
```

