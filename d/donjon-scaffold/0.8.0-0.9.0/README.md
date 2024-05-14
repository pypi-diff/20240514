# Comparing `tmp/donjon-scaffold-0.8.0.tar.gz` & `tmp/donjon-scaffold-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donjon-scaffold-0.8.0.tar", last modified: Tue Dec  5 14:10:22 2023, max compression
+gzip compressed data, was "donjon-scaffold-0.9.0.tar", last modified: Tue May 14 13:22:06 2024, max compression
```

## Comparing `donjon-scaffold-0.8.0.tar` & `donjon-scaffold-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2023-12-05 14:10:22.031597 donjon-scaffold-0.8.0/
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      688 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/LICENSE
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      468 2023-12-05 14:10:22.031597 donjon-scaffold-0.8.0/PKG-INFO
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      163 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/README.md
-drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2023-12-05 14:10:22.031597 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      468 2023-12-05 14:10:22.000000 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/PKG-INFO
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      279 2023-12-05 14:10:22.000000 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/SOURCES.txt
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)        1 2023-12-05 14:10:22.000000 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/dependency_links.txt
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)       25 2023-12-05 14:10:22.000000 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/requires.txt
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)        9 2023-12-05 14:10:22.000000 donjon-scaffold-0.8.0/donjon_scaffold.egg-info/top_level.txt
-drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2023-12-05 14:10:22.031597 donjon-scaffold-0.8.0/scaffold/
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)   101232 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/scaffold/__init__.py
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    26768 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/scaffold/iso7816.py
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    14863 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/scaffold/stm32.py
--rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)       38 2023-12-05 14:10:22.031597 donjon-scaffold-0.8.0/setup.cfg
--rwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)     1285 2023-12-05 14:10:21.000000 donjon-scaffold-0.8.0/setup.py
+drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2024-05-14 13:22:06.093261 donjon-scaffold-0.9.0/
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      688 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/LICENSE
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      468 2024-05-14 13:22:06.093261 donjon-scaffold-0.9.0/PKG-INFO
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      163 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/README.md
+drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2024-05-14 13:22:06.089261 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      468 2024-05-14 13:22:06.000000 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/PKG-INFO
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)      295 2024-05-14 13:22:06.000000 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/SOURCES.txt
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)        1 2024-05-14 13:22:06.000000 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/dependency_links.txt
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)       25 2024-05-14 13:22:06.000000 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/requires.txt
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)        9 2024-05-14 13:22:06.000000 donjon-scaffold-0.9.0/donjon_scaffold.egg-info/top_level.txt
+drwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)        0 2024-05-14 13:22:06.093261 donjon-scaffold-0.9.0/scaffold/
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    79565 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/scaffold/__init__.py
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    26039 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/scaffold/bus.py
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    26761 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/scaffold/iso7816.py
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)    14889 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/scaffold/stm32.py
+-rw-rw-r--   0 oheriveaux  (1000) oheriveaux  (1000)       38 2024-05-14 13:22:06.093261 donjon-scaffold-0.9.0/setup.cfg
+-rwxrwxr-x   0 oheriveaux  (1000) oheriveaux  (1000)     1287 2024-05-14 13:22:05.000000 donjon-scaffold-0.9.0/setup.py
```

### Comparing `donjon-scaffold-0.8.0/LICENSE` & `donjon-scaffold-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `donjon-scaffold-0.8.0/scaffold/__init__.py` & `donjon-scaffold-0.9.0/scaffold/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,87 +14,61 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 #
 # Copyright 2019 Ledger SAS, written by Olivier Hériveaux
 
 
 from enum import Enum
-import serial
 from time import sleep
 import serial.tools.list_ports
 from typing import Optional, Union
+from .bus import ScaffoldBus, Register, TimeoutError
 
 
-class TimeoutError(Exception):
-    """ Thrown when a polling read or write command timed out. """
-    def __init__(self, data=None, size=None, expected=None):
-        """
-        :param data: The received data until timeout. None if timeout occured
-        during a write operation.
-        :param size: The number of successfully proceeded bytes.
-        :param expected: The expected number of bytes to be proceeded.
-        """
-        self.data = data
-        self.expected = expected
-        if self.data is not None:
-            assert size is None
-            self.size = len(data)
-        else:
-            self.size = size
-
-    def __str__(self):
-        if self.data is not None:
-            if len(self.data):
-                h = self.data.hex()
-                return (
-                    f'Read timeout: partially received {len(self.data)} '
-                    f'bytes {h}.')
-            else:
-                return 'Read timeout: no data received.'
-        else:
-            return (
-                f'Write timeout. Only {self.size}/{self.expected} bytes '
-                'written.')
+# Prevent flake8 from complaining about unused import. This class is actually
+# re-exported. This should be improved in the future.
+TimeoutError = TimeoutError
 
 
 class Signal:
     """
     Base class for all connectable signals in Scaffold. Every :class:`Signal`
     instance has a Scaffold board parent instance which is used to electrically
     configure the hardware board when two :class:`Signal` are connected
     together.
     """
+
     def __init__(self, parent, path):
         """
         :param parent: Scaffold instance which the signal belongs to.
         :param path: Signal path string. Uniquely identifies a Scaffold board
             internal signal. For instance '/dev/uart0/tx'.
         """
         self.__parent = parent
         self.__path = path
 
     @property
     def parent(self):
-        """ Parent :class:`Scaffold` board instance. Read-only. """
+        """Parent :class:`Scaffold` board instance. Read-only."""
         return self.__parent
 
     @property
     def path(self):
-        """ Signal path. For instance '/dev/uart0/tx'. Read-only. """
+        """Signal path. For instance '/dev/uart0/tx'. Read-only."""
         return self.__path
 
     @property
     def name(self):
         """
         Signal name (last element of the path). For instance 'tx'. Read-only.
         """
-        return self.__path.split('/')[-1]
+        return self.__path.split("/")[-1]
 
     def __str__(self):
-        """ :return: Signal path. For instance '/dev/uart0/tx'. """
+        """:return: Signal path. For instance '/dev/uart0/tx'."""
         return self.__path
 
     def __lshift__(self, other):
         """
         Feed the current signal with another signal.
 
         :param other: Another :class:`Signal` instance. The other signal must
@@ -112,14 +86,15 @@
         self.__parent.sig_connect(other, self)
 
 
 class Module:
     """
     Class to facilitate signals and registers declaration.
     """
+
     def __init__(self, parent, path=None):
         """
         :param parent: The Scaffold instance owning the object.
         :param path: Base path for the signals. For instance '/uart'.
         """
         self.__parent = parent
         self.__path = path
@@ -133,17 +108,17 @@
         :name: Signal name.
         :type name: str
         :return: Created signal object
         :rtype: Signal
         """
         assert not hasattr(self, name)
         if self.__path is None:
-            path = '/' + name
+            path = "/" + name
         else:
-            path = self.__path + '/' + name
+            path = self.__path + "/" + name
         sig = Signal(self.__parent, path)
         self.__dict__[name] = sig
         return sig
 
     def add_signals(self, *names):
         """
         Add many signals to the object and set them as new attributes of the
@@ -159,15 +134,15 @@
     def add_register(self, name, *args, **kwargs):
         """
         Create a new register.
         :param name: Register name.
         :param args: Arguments passed to Register.__init__.
         :param kwargs: Keyword arguments passed to Register.__init__.
         """
-        attr_name = 'reg_' + name
+        attr_name = "reg_" + name
         reg = Register(self.__parent, *args, **kwargs)
         self.__dict__[attr_name] = reg
         # Keep track of the register for reset_registers method
         self.__registers.append(reg)
 
     def __setattr__(self, key, value):
         if key in self.__dict__:
@@ -185,242 +160,24 @@
         Call :meth:`Register.reset` on each defined register.
         """
         for reg in self.__registers:
             reg.reset()
 
     @property
     def parent(self):
-        """ Scaffold instance the module belongs to. Read-only. """
+        """Scaffold instance the module belongs to. Read-only."""
         return self.__parent
 
 
-class Register:
-    """
-    Manages accesses to a register of a module. Implements value cache
-    mechanism whenever possible.
-    """
-    def __init__(
-            self, parent, mode, address, wideness=1, min_value=None,
-            max_value=None, reset=None):
-        """
-        :param parent: The Scaffold instance owning the register.
-        :param address: 16-bits address of the register.
-        :param mode: Access mode string. Can have the following characters: 'r'
-            for read, 'w' for write, 'v' to indicate the register is volatile.
-            When the register is not volatile, a cache is used for read
-            accesses.
-        :param wideness: Number of bytes stored by the register. When this
-            value is not 1, the register cannot be read.
-        :parma min_value: Minimum allowed value. If None, minimum value will be
-            0 by default.
-        :param max_value: Maximum allowed value. If None, maximum value will be
-            2^(wideness*8)-1 by default.
-        :param reset: Value to be set to the register when :meth:`reset` is
-            called. If None, :meth:`reset` has no effect.
-        """
-        self.__parent = parent
-
-        if address not in range(0x10000):
-            raise ValueError('Invalid register address')
-        self.__address = address
-
-        self.__w = 'w' in mode
-        self.__r = 'r' in mode
-        self.__volatile = 'v' in mode
-
-        if wideness < 1:
-            raise ValueError('Invalid wideness')
-        if (wideness > 1) and self.__r:
-            raise ValueError('Wideness must be 1 if register can be read.')
-        self.__wideness = wideness
-
-        if min_value is None:
-            # Set default minimum value to 0.
-            self.__min_value = 0
-        else:
-            # Check maximum value.
-            if min_value not in range(2**(wideness*8)):
-                raise ValueError('Invalid register minimum value')
-            self.__min_value = min_value
-
-        if max_value is None:
-            # Set default maximum value based on register size.
-            self.__max_value = 2**(wideness*8) - 1
-        else:
-            # Check maximum value.
-            if max_value not in range(2**(wideness*8)):
-                raise ValueError('Invalid register maximum value')
-            self.__max_value = max_value
-
-        if self.__min_value > self.__max_value:
-            raise ValueError(
-                'Register minimum value must be lower or equal to maximum '
-                'value')
-
-        self.__reset = reset
-        self.__cache = None
-
-    def set(self, value, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Set a new value to the register. This method will check bounds against
-        the minimum and maximum allowed values of the register. If polling is
-        enabled and the register is wide, polling is applied for each byte of
-        the register.
-
-        :param value: New value.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        """
-        if value < self.__min_value:
-            raise ValueError('Value too low')
-        if value > self.__max_value:
-            raise ValueError('Value too high')
-        if not self.__w:
-            raise RuntimeError('Register cannot be written')
-        # Handle wideness
-        value_bytes = value.to_bytes(self.__wideness, 'big', signed=False)
-        self.__parent.bus.write(
-            self.__address, value_bytes, poll, poll_mask, poll_value)
-        # Save as int
-        self.__cache = value
-
-    def get(self):
-        """
-        :return: Current register value.
-        If the register is not volatile and the value has been cached, no
-        access to the board is performed and the cache is returned. If the
-        register is not volatile but can't be read, the cached value is
-        returned or an exception is raised if cache is not set.
-        """
-        if self.__volatile:
-            if not self.__r:
-                raise RuntimeError('Register cannot be read')
-            return self.__parent.bus.read(self.__address)[0]
-        else:
-            # Register is not volatile, so its data can be cached.
-            if self.__cache is None:
-                if self.__r:
-                    value = self.__parent.bus.read(self.__address)[0]
-                    self.__cache = value
-                else:
-                    raise RuntimeError('Register cannot be read')
-            return self.__cache
-
-    def or_set(self, value):
-        """
-        Sets some bits to 1 in the register.
-        :param value: An int.
-        """
-        self.set(self.get() | value)
-
-    def set_bit(
-            self, index, value, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Sets the value of a single bit of the register.
-        :param index: Bit index, in [0, 7].
-        :param value: True, False, 0 or 1.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        """
-        self.set(
-            (self.get() & ~(1 << index)) | (int(bool(value)) << index),
-            poll, poll_mask, poll_value)
-
-    def get_bit(self, index):
-        """
-        :return: Value of a given bit, 0 or 1.
-        :param index: Bit index, in [0, 7].
-        """
-        return (self.get() >> index) & 1
-
-    def set_mask(
-            self, value, mask, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Set selected bits value.
-        :param value: Bits value.
-        :param mask: A mask indicating which bits must be sets.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        """
-        # TODO: raise an exception is the register is declared as volatile ?
-        current = self.get()
-        self.set(
-            (current & (~mask)) | (value & mask), poll, poll_mask, poll_value)
-
-    def write(self, data, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Raw write in the register. This method raises a RuntimeError if the
-        register cannot be written.
-        :param data: Data to be written. Can be a byte, bytes or bytearray.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        """
-        if not self.__w:
-            raise RuntimeError('Register cannot be written')
-        self.__parent.bus.write(
-            self.__address, data, poll, poll_mask, poll_value)
-
-    def read(self, size=1, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Raw read the register. This method raises a RuntimeError if the
-        register cannot be read.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        :return: bytearray
-        """
-        if not self.__r:
-            raise RuntimeError('Register cannot be read')
-        return self.__parent.bus.read(
-            self.__address, size, poll, poll_mask, poll_value)
-
-    def reset(self):
-        """
-        Set the register value to its default value. If no default value has
-        been defined, this method has no effect.
-        """
-        if self.__reset is not None:
-            self.set(self.__reset)
-
-    @property
-    def address(self):
-        """ :return: Register address. """
-        return self.__address
-
-    @property
-    def max(self):
-        """
-        Maximum possible value for the register.
-        :type: int
-        """
-        return self.__max_value
-
-    @property
-    def min(self):
-        """
-        Minimum possible value for the register.
-        :type: int
-        """
-        return self.__min_value
-
-
 class FreqRegisterHelper:
     """
     Helper to provide frequency attributes which compute clock divisor
     registers value based on asked target frequencies.
     """
+
     def __init__(self, sys_freq, reg):
         """
         :param sys_freq: System base frequency used to compute clock divisors.
         :type sys_freq: int
         :param reg: Register to be configured.
         :type reg: :class:`scaffold.Register`
         """
@@ -435,54 +192,56 @@
 
         :param value: Target frequency, in Hertz.
         :type value: float
         """
         d = round((0.5 * self.__sys_freq / value) - 1)
         # Check that the divisor fits in the register
         if d > self.__reg.max:
-            raise ValueError('Target clock frequency is too low.')
+            raise ValueError("Target clock frequency is too low.")
         if d < self.__reg.min:
-            raise ValueError('Target clock frequency is too high.')
+            raise ValueError("Target clock frequency is too high.")
         # Calculate error between target and effective clock frequency
         real = self.__sys_freq / ((d + 1) * 2)
         err = abs(real - value) / value
         if err > self.__max_err:
             raise RuntimeError(
-                f'Cannot reach target clock frequency within '
-                f'{self.__max_err*100}% accuracy.')
+                f"Cannot reach target clock frequency within "
+                f"{self.__max_err*100}% accuracy."
+            )
         self.__reg.set(d)
         self.__cache = real
 
     def get(self):
         """
         :return: Actual clock frequency. None if frequency has not been set.
         """
         return self.__cache
 
 
 class Version(Module):
-    """ Version module of Scaffold. """
+    """Version module of Scaffold."""
+
     def __init__(self, parent):
         """
         :param parent: The Scaffold instance owning the version module.
         """
         super().__init__(parent)
-        self.add_register('data', 'r', 0x0100)
+        self.add_register("data", "r", 0x0100)
 
     def get_string(self):
         """
         Read the data register multiple times until the full version string has
         been retrieved.
         :return: Hardware version string.
         """
         # We consider the version string is not longer than 32 bytes. This
         # allows us reading the string with only one command to be faster.
         buf = self.reg_data.read(32 + 1 + 32 + 1)
         offset = 0
-        result = ''
+        result = ""
         # Find the first \0 character.
         while buf[offset] != 0:
             offset += 1
         offset += 1
         # Read characters until second \0 character.
         while buf[offset] != 0:
             result += chr(buf[offset])
@@ -496,14 +255,15 @@
 
 
 class LED:
     """
     Represents a LED of the board.
     Each instance of this class is an attribute of a :class:`LEDs` instance.
     """
+
     def __init__(self, parent, index):
         """
         :param parent: Parent LEDs module instance.
         :param index: Bit index of the LED.
         """
         self.__parent = parent
         self.__index = index
@@ -519,46 +279,58 @@
         :type: LEDMode.
         """
         return LEDMode((self.__parent.reg_mode.get() >> self.__index) & 1)
 
     @mode.setter
     def mode(self, value):
         self.__parent.reg_mode.set_mask(
-            LEDMode(value).value << self.__index, 1 << self.__index)
+            LEDMode(value).value << self.__index, 1 << self.__index
+        )
 
 
 class LEDs(Module):
-    """ LEDs module of Scaffold. """
+    """LEDs module of Scaffold."""
+
     def __init__(self, parent):
         """
         :param parent: The Scaffold instance owning the version module.
         """
         super().__init__(parent)
-        self.add_register('control', 'w', 0x0200)
-        self.add_register('brightness', 'w', 0x0201)
-        self.add_register('leds_0', 'w', 0x0202)
-        self.add_register('leds_1', 'w', 0x0203)
-        self.add_register('leds_2', 'w', 0x0204)
-        self.add_register('mode', 'w', 0x0205, wideness=3)
-        if self.parent.version <= '0.3':
+        self.add_register("control", "w", 0x0200)
+        self.add_register("brightness", "w", 0x0201)
+        self.add_register("leds_0", "w", 0x0202)
+        self.add_register("leds_1", "w", 0x0203)
+        self.add_register("leds_2", "w", 0x0204)
+        self.add_register("mode", "w", 0x0205, wideness=3)
+        if self.parent.version <= "0.3":
             # Scaffold hardware v1 only
             leds = [
-                'a0', 'a1', 'b0', 'b1', 'c0', 'c1', 'd0', 'd1', 'd2', 'd3',
-                'd4', 'd5']
+                "a0",
+                "a1",
+                "b0",
+                "b1",
+                "c0",
+                "c1",
+                "d0",
+                "d1",
+                "d2",
+                "d3",
+                "d4",
+                "d5",
+            ]
             offset = 6
         else:
             # Scaffold hardware v1.1
-            leds = [
-                'a0', 'a1', 'a2', 'a3', 'd0', 'd1', 'd2', 'd3', 'd4', 'd5']
+            leds = ["a0", "a1", "a2", "a3", "d0", "d1", "d2", "d3", "d4", "d5"]
             offset = 8
         for i, name in enumerate(leds):
             self.__setattr__(name, LED(self, i + offset))
 
     def reset(self):
-        """ Set module registers to default values. """
+        """Set module registers to default values."""
         self.reg_control = 0
         self.reg_brightness.set(20)
         self.reg_mode.set(0)
 
     @property
     def brightness(self):
         """
@@ -567,20 +339,20 @@
         :type: float
         """
         return self.reg_brightness.get() / 127.0
 
     @brightness.setter
     def brightness(self, value):
         if (value < 0) or (value > 1):
-            raise ValueError('Invalid brightness value')
+            raise ValueError("Invalid brightness value")
         self.reg_brightness.set(int(value * 127))
 
     @property
     def disabled(self):
-        """ If set to True, LEDs driver outputs are all disabled. """
+        """If set to True, LEDs driver outputs are all disabled."""
         return bool(self.reg_control.get() & 1)
 
     @disabled.setter
     def disabled(self, value):
         value = int(bool(value))
         self.reg_control.set_mask(value, 1)
 
@@ -594,44 +366,46 @@
     @override.setter
     def override(self, value):
         value = int(bool(value))
         self.reg_control.set_mask(value << 1, 2)
 
 
 class UARTParity(Enum):
-    """ Possible parity modes for UART peripherals. """
+    """Possible parity modes for UART peripherals."""
+
     NONE = 0
     ODD = 1
     EVEN = 2
 
 
 class UART(Module):
     """
     UART module of Scaffold.
     """
+
     __REG_CONTROL_BIT_FLUSH = 0
     __REG_CONFIG_BIT_TRIGGER = 3
     __REG_CONFIG_BIT_PARITY = 0
 
     def __init__(self, parent, index):
         """
         :param parent: The Scaffold instance owning the UART module.
         :param index: UART module index.
         """
-        super().__init__(parent, f'/uart{index}')
+        super().__init__(parent, f"/uart{index}")
         self.__index = index
         # Declare the signals
-        self.add_signals('rx', 'tx', 'trigger')
+        self.add_signals("rx", "tx", "trigger")
         # Declare the registers
         self.__addr_base = base = 0x0400 + 0x0010 * index
-        self.add_register('status', 'rv', base)
-        self.add_register('control', 'w', base + 1)
-        self.add_register('config', 'w', base + 2)
-        self.add_register('divisor', 'w', base + 3, wideness=2, min_value=1)
-        self.add_register('data', 'rwv', base + 4)
+        self.add_register("status", "rv", base)
+        self.add_register("control", "w", base + 1)
+        self.add_register("config", "w", base + 2)
+        self.add_register("divisor", "w", base + 3, wideness=2, min_value=1)
+        self.add_register("data", "rwv", base + 4)
         # Current board target baudrate (this is not the effective baudrate)
         self.__cache_baudrate = None
         # Accuracy parameter
         self.max_err = 0.01
 
     def reset(self):
         """
@@ -661,26 +435,26 @@
         Set target baudrate. If baudrate is too low or too high, a ValueError
         is thrown. If baudrate cannot be reached within 1% accuracy, a
         RuntimeError is thrown.
         :param value: New target baudrate.
         """
         d = round((self.parent.sys_freq / value) - 1)
         # Check that the divisor can be stored on 16 bits.
-        if d > 0xffff:
-            raise ValueError('Target baudrate is too low.')
+        if d > 0xFFFF:
+            raise ValueError("Target baudrate is too low.")
         if d < 1:
-            raise ValueError('Target baudrate is too high.')
+            raise ValueError("Target baudrate is too high.")
         # Calculate error between target and effective baudrates
         real = self.parent.sys_freq / (d + 1)
         err = abs(real - value) / value
         max_err = self.max_err
         if err > max_err:
             raise RuntimeError(
-                f'Cannot reach target baudrate within {max_err*100}% '
-                'accuracy.')
+                f"Cannot reach target baudrate within {max_err*100}% accuracy."
+            )
         self.reg_divisor.set(d)
         self.__cache_baudrate = real
 
     def transmit(self, data: bytes, trigger: bool = False):
         """
         Transmit data using the UART.
 
@@ -689,110 +463,108 @@
             disable trigger.
         """
         if trigger:
             buf = data[:-1]
         else:
             buf = data
         # Polling on status.ready bit before sending each character.
-        with self.parent.lazy_section():
-            self.reg_data.write(
-                buf, poll=self.reg_status, poll_mask=0x01, poll_value=0x01)
-            if trigger:
-                config = self.reg_config.get()
-                # Enable trigger as soon as previous transmission ends
-                self.reg_config.write(
-                    config | (1 << self.__REG_CONFIG_BIT_TRIGGER),
-                    poll=self.reg_status, poll_mask=0x01, poll_value=0x01)
-                # Send the last byte. No need for polling here, because it has
-                # already been done when enabling trigger.
-                self.reg_data.write(data[-1])
-                # Disable trigger
-                self.reg_config.write(
-                    config, poll=self.reg_status, poll_mask=0x01,
-                    poll_value=0x01)
+        self.reg_data.write(buf, self.reg_status.poll(mask=0x01, value=0x01))
+        if trigger:
+            config = self.reg_config.get()
+            # Enable trigger as soon as previous transmission ends
+            self.reg_config.write(
+                config | (1 << self.__REG_CONFIG_BIT_TRIGGER),
+                self.reg_status.poll(mask=0x01, value=0x01),
+            )
+            # Send the last byte. No need for polling here, because it has
+            # already been done when enabling trigger.
+            self.reg_data.write(data[-1])
+            # Disable trigger
+            self.reg_config.write(config, self.reg_status.poll(mask=0x01, value=0x01))
 
     def receive(self, n=1):
         """
         Receive n bytes from the UART. This function blocks until all bytes
         have been received or the timeout expires and a TimeoutError is thrown.
         """
-        return self.reg_data.read(
-            n, poll=self.reg_status, poll_mask=0x04, poll_value=0x00)
+        return self.reg_data.read(n, self.reg_status.poll(mask=0x04, value=0x00))
 
     def flush(self):
-        """ Discard all the received bytes in the FIFO. """
+        """Discard all the received bytes in the FIFO."""
         self.reg_control.set_bit(self.__REG_CONTROL_BIT_FLUSH, 1)
 
     @property
     def parity(self):
         """
         Parity mode. Disabled by default.
 
         :type: UARTParity
         """
         return UARTParity(
-            (self.reg_config.get() >> self.__REG_CONFIG_BIT_PARITY) & 0b11)
+            (self.reg_config.get() >> self.__REG_CONFIG_BIT_PARITY) & 0b11
+        )
 
     @parity.setter
     def parity(self, value):
         self.reg_config.set_mask(
             (value.value & 0b11) << self.__REG_CONFIG_BIT_PARITY,
-            0b11 << self.__REG_CONFIG_BIT_PARITY)
+            0b11 << self.__REG_CONFIG_BIT_PARITY,
+        )
 
 
 class PulseGenerator(Module):
     """
     Pulse generator module of Scaffold.
     Usually abreviated as pgen.
     """
+
     def __init__(self, parent, path, base):
         """
         :param parent: The :class:`Scaffold` instance owning the UART module.
         :param path: Module path.
         :type path: str
         :param base: Base address for all registers.
         :type base: int
         """
         super().__init__(parent, path)
         # Create the signals
-        self.add_signals('start', 'out')
+        self.add_signals("start", "out")
         # Create the registers
-        self.add_register('status', 'rv', base)
-        self.add_register('control', 'wv', base + 1)
-        self.add_register('config', 'w', base + 2, reset=0)
-        self.add_register('delay', 'w', base + 3, wideness=3, reset=0)
-        self.add_register('interval', 'w', base + 4, wideness=3, reset=0)
-        self.add_register('width', 'w', base + 5, wideness=3, reset=0)
-        self.add_register('count', 'w', base + 6, wideness=2, reset=0)
+        self.add_register("status", "rv", base)
+        self.add_register("control", "wv", base + 1)
+        self.add_register("config", "w", base + 2, reset=0)
+        self.add_register("delay", "w", base + 3, wideness=3, reset=0)
+        self.add_register("interval", "w", base + 4, wideness=3, reset=0)
+        self.add_register("width", "w", base + 5, wideness=3, reset=0)
+        self.add_register("count", "w", base + 6, wideness=2, reset=0)
 
     def fire(self):
-        """ Manually trigger the pulse generation. """
+        """Manually trigger the pulse generation."""
         self.reg_control.set(1)
 
     def wait_ready(self):
         """
         Wait while the pulse generator is busy.
 
         This uses the polling mechanism on the ready bit in the status
         register. It can be used to block next commands and synchronize their
         execution to the end of the pulse.
         """
         # Dummy write to the address 0 which is not mapped.
-        self.parent.bus.write(
-            0, 0, poll=self.reg_status, poll_mask=1, poll_value=1)
+        self.parent.bus.write(0, 0, self.reg_status.poll(mask=1, value=1))
 
     def __duration_to_clock_cycles(self, t):
         """
         Calculate the number of clock cycles corresponding to a given time.
 
         :param t: Time in seconds.
         :type t: float.
         """
         if t < 0:
-            raise ValueError('Duration cannot be negative')
+            raise ValueError("Duration cannot be negative")
         cc = round(t * self.parent.sys_freq)
         return cc
 
     def __clock_cycles_to_duration(self, cc):
         """
         Calculate the time elapsed during a given number of clock cycles.
 
@@ -808,99 +580,99 @@
 
         :type: float
         """
         return self.__clock_cycles_to_duration(self.reg_delay.get() + 1)
 
     @delay.setter
     def delay(self, value):
-        n = self.__duration_to_clock_cycles(value)-1
+        n = self.__duration_to_clock_cycles(value) - 1
         self.reg_delay.set(n)
 
     @property
     def delay_min(self):
-        """ :return: Minimum possible delay. """
+        """:return: Minimum possible delay."""
         return self.__clock_cycles_to_duration(1)
 
     @property
     def delay_max(self):
-        """ :return: Maximum possible delay. """
+        """:return: Maximum possible delay."""
         return self.__clock_cycles_to_duration(self.reg_delay.max + 1)
 
     @property
     def interval(self):
         """
         Delay between pulses, in seconds.
 
         :type: float
         """
         return self.__clock_cycles_to_duration(self.reg_interval.get() + 1)
 
     @interval.setter
     def interval(self, value):
-        n = self.__duration_to_clock_cycles(value)-1
+        n = self.__duration_to_clock_cycles(value) - 1
         self.reg_interval.set(n)
 
     @property
     def interval_min(self):
-        """ :return: Minimum possible interval. """
+        """:return: Minimum possible interval."""
         return self.__clock_cycles_to_duration(1)
 
     @property
     def interval_max(self):
-        """ :return: Maximum possible interval. """
+        """:return: Maximum possible interval."""
         return self.__clock_cycles_to_duration(self.reg_interval.max + 1)
 
     @property
     def width(self):
         """
         Pulse width, in seconds.
 
         :type: float
         """
         return self.__clock_cycles_to_duration(self.reg_width.get() + 1)
 
     @width.setter
     def width(self, value):
-        n = self.__duration_to_clock_cycles(value)-1
+        n = self.__duration_to_clock_cycles(value) - 1
         self.reg_width.set(n)
 
     @property
     def width_min(self):
-        """ :return: Minimum possible pulse width. """
+        """:return: Minimum possible pulse width."""
         return self.__clock_cycles_to_duration(1)
 
     @property
     def width_max(self):
-        """ :return: Maximum possible pulse width. """
+        """:return: Maximum possible pulse width."""
         return self.__clock_cycles_to_duration(self.reg_width.max + 1)
 
     @property
     def count(self):
         """
         Number of pulses to be generated. Minimum value is 1. Maximum value is
         2^16.
 
         :type: int
         """
         return self.reg_count.get() + 1
 
     @count.setter
     def count(self, value):
-        if value not in range(1, 2**16+1):
-            raise ValueError('Invalid pulse count')
-        self.reg_count.set(value-1)
+        if value not in range(1, 2**16 + 1):
+            raise ValueError("Invalid pulse count")
+        self.reg_count.set(value - 1)
 
     @property
     def count_min(self):
-        """ :return: Minimum possible pulse count. """
+        """:return: Minimum possible pulse count."""
         return 1
 
     @property
     def count_max(self):
-        """ :return: Maximum possible pulse count. """
+        """:return: Maximum possible pulse count."""
         return self.reg_count.max + 1
 
     @property
     def polarity(self):
         """
         Pulse polarity. If 0, output is low when idle, and high during pulses.
         When 1, output is high when idle, and low during pulses.
@@ -908,27 +680,28 @@
         :type: int
         """
         return self.reg_config.get() & 1
 
     @polarity.setter
     def polarity(self, value):
         if value not in range(2):
-            raise ValueError('Invalid polarity value: must be 0 or 1')
+            raise ValueError("Invalid polarity value: must be 0 or 1")
         self.reg_config.set_bit(0, value)
 
 
 class Power(Module):
-    """ Controls the platform and DUT sockets power supplies. """
+    """Controls the platform and DUT sockets power supplies."""
+
     __ADDR_CONTROL = 0x0600
 
     def __init__(self, parent):
-        """ :param parent: The Scaffold instance owning the power module. """
-        super().__init__(parent, '/power')
-        self.add_register('control', 'rwv', self.__ADDR_CONTROL)
-        self.add_signals('dut_trigger', 'platform_trigger')
+        """:param parent: The Scaffold instance owning the power module."""
+        super().__init__(parent, "/power")
+        self.add_register("control", "rwv", self.__ADDR_CONTROL)
+        self.add_signals("dut_trigger", "platform_trigger")
 
     @property
     def all(self):
         """
         All power-supplies state. int. Bit 0 corresponds to the DUT power
         supply. Bit 1 corresponds to the platform power-supply. When a bit is
         set to 1, the corresponding power supply is enabled. This attribute can
@@ -939,24 +712,24 @@
     @all.setter
     def all(self, value):
         assert (value & ~0b11) == 0
         self.reg_control.set(value)
 
     @property
     def platform(self):
-        """ Platform power-supply state. int. """
+        """Platform power-supply state. int."""
         return self.reg_control.get_bit(1)
 
     @platform.setter
     def platform(self, value):
         self.reg_control.set_bit(1, value)
 
     @property
     def dut(self):
-        """ DUT power-supply state. int. """
+        """DUT power-supply state. int."""
         return self.reg_control.get_bit(0)
 
     @dut.setter
     def dut(self, value):
         self.reg_control.set_bit(0, value)
 
     def restart_dut(self, toff=0.05, ton=0):
@@ -1016,36 +789,37 @@
 
 
 class ISO7816(Module):
     """
     ISO7816 peripheral of Scaffold. Does not provide convention or protocol
     management. See :class:`scaffold.iso7816.Smartcard` for more features.
     """
+
     __REG_STATUS_BIT_READY = 0
     __REG_STATUS_BIT_PARITY_ERROR = 1
     __REG_STATUS_BIT_EMPTY = 2
     __REG_CONTROL_BIT_FLUSH = 0
     __REG_CONFIG_TRIGGER_TX = 0
     __REG_CONFIG_TRIGGER_RX = 1
     __REG_CONFIG_TRIGGER_LONG = 2
     __REG_CONFIG_PARITY_MODE = 3
 
     def __init__(self, parent):
         """
         :param parent: The Scaffold instance owning the UART module.
         """
-        super().__init__(parent, '/iso7816')
-        self.add_signals('io_in', 'io_out', 'clk', 'trigger')
+        super().__init__(parent, "/iso7816")
+        self.add_signals("io_in", "io_out", "clk", "trigger")
         self.__addr_base = base = 0x0500
-        self.add_register('status', 'rv', base)
-        self.add_register('control', 'w', base + 1)
-        self.add_register('config', 'w', base + 2)
-        self.add_register('divisor', 'w', base + 3)
-        self.add_register('etu', 'w', base + 4, wideness=2)
-        self.add_register('data', 'rwv', base + 5)
+        self.add_register("status", "rv", base)
+        self.add_register("control", "w", base + 1)
+        self.add_register("config", "w", base + 2)
+        self.add_register("divisor", "w", base + 3)
+        self.add_register("etu", "w", base + 4, wideness=2)
+        self.add_register("data", "rwv", base + 5)
         # Accuracy parameter
         self.max_err = 0.01
 
     def reset_config(self):
         """
         Reset ISO7816 peripheral to its default configuration.
         """
@@ -1070,113 +844,136 @@
         """
         return self.__cache_clock_frequency
 
     @clock_frequency.setter
     def clock_frequency(self, value):
         d = round((0.5 * self.parent.sys_freq / value) - 1)
         # Check that the divisor fits one unsigned byte.
-        if d > 0xff:
-            raise ValueError('Target clock frequency is too low.')
+        if d > 0xFF:
+            raise ValueError("Target clock frequency is too low.")
         if d < 0:
-            raise ValueError('Target clock frequency is too high.')
+            raise ValueError("Target clock frequency is too high.")
         # Calculate error between target and effective clock frequency
         real = self.parent.sys_freq / ((d + 1) * 2)
         err = abs(real - value) / value
         max_err = self.max_err = 0.01
         if err > max_err:
             raise RuntimeError(
-                f'Cannot reach target clock frequency within {max_err*100}% '
-                'accuracy.')
+                f"Cannot reach target clock frequency within {max_err*100}% "
+                "accuracy."
+            )
         self.reg_divisor.set(d)
         self.__cache_clock_frequency = real
 
     @property
     def etu(self):
         """
         ISO7816 ETU parameter. Value must be in range [1, 2^11-1]. Default ETU
         is 372.
         """
         return self.reg_etu.get() + 1
 
     @etu.setter
     def etu(self, value):
         if value not in range(1, 2**11):
-            raise ValueError('Invalid ETU parameter')
+            raise ValueError("Invalid ETU parameter")
         self.reg_etu.set(value - 1)
 
     def flush(self):
-        """ Discard all the received bytes in the FIFO. """
+        """Discard all the received bytes in the FIFO."""
         self.reg_control.write(1 << self.__REG_CONTROL_BIT_FLUSH)
 
     def receive(self, n=1, timeout=None):
         """
         Receive bytes. This function blocks until all bytes have been
         received or the timeout expires and a TimeoutError is thrown.
 
         :param n: Number of bytes to be read.
         """
         with self.parent.timeout_section(timeout):
             return self.reg_data.read(
-                n, poll=self.reg_status,
-                poll_mask=(1 << self.__REG_STATUS_BIT_EMPTY), poll_value=0x00)
+                n,
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_EMPTY), value=0x00
+                ),
+            )
 
     def transmit(self, data: bytes, trigger: bool = False):
         """
         Transmit data.
 
         :param data: Data to be transmitted.
         :param trigger: Enable trigger on the last transmitted byte.
         """
         # Polling on status.ready bit before sending each character
         if not trigger:
             self.reg_data.write(
-                data, poll=self.reg_status,
-                poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-                poll_value=(1 << self.__REG_STATUS_BIT_READY))
+                data,
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_READY),
+                    value=(1 << self.__REG_STATUS_BIT_READY),
+                ),
+            )
         else:
             # We want to trig on the last sent character
-            with self.parent.lazy_section():
-                self.reg_config.set_bit(
-                    self.__REG_CONFIG_TRIGGER_TX, 0, poll=self.reg_status,
-                    poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-                    poll_value=(1 << self.__REG_STATUS_BIT_READY))
-                self.reg_data.write(
-                    data[:-1], poll=self.reg_status,
-                    poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-                    poll_value=(1 << self.__REG_STATUS_BIT_READY))
-                self.reg_config.set_bit(
-                    self.__REG_CONFIG_TRIGGER_TX, 1, poll=self.reg_status,
-                    poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-                    poll_value=(1 << self.__REG_STATUS_BIT_READY))
-                self.reg_data.write(data[-1])
-                self.reg_config.set_bit(
-                    self.__REG_CONFIG_TRIGGER_TX, 0, poll=self.reg_status,
-                    poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-                    poll_value=(1 << self.__REG_STATUS_BIT_READY))
+            self.reg_config.set_bit(
+                self.__REG_CONFIG_TRIGGER_TX,
+                0,
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_READY),
+                    value=(1 << self.__REG_STATUS_BIT_READY),
+                ),
+            )
+            self.reg_data.write(
+                data[:-1],
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_READY),
+                    value=(1 << self.__REG_STATUS_BIT_READY),
+                ),
+            )
+            self.reg_config.set_bit(
+                self.__REG_CONFIG_TRIGGER_TX,
+                1,
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_READY),
+                    value=(1 << self.__REG_STATUS_BIT_READY),
+                ),
+            )
+            self.reg_data.write(data[-1])
+            self.reg_config.set_bit(
+                self.__REG_CONFIG_TRIGGER_TX,
+                0,
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_READY),
+                    value=(1 << self.__REG_STATUS_BIT_READY),
+                ),
+            )
 
     @property
     def empty(self):
-        """ True if reception FIFO is empty. """
+        """True if reception FIFO is empty."""
         return bool(self.reg_status.get() & (1 << self.__REG_STATUS_BIT_EMPTY))
 
     @property
     def parity_mode(self):
         """
         Parity mode. Standard is Even parity, but it can be changed to odd or
         forced to a fixed value for testing purposes.
         :type: ISO7816ParityMode
         """
         return ISO7816ParityMode(
-            (self.reg_config.get() >> self.__REG_CONFIG_PARITY_MODE) & 0b11)
+            (self.reg_config.get() >> self.__REG_CONFIG_PARITY_MODE) & 0b11
+        )
 
     @parity_mode.setter
     def parity_mode(self, value):
         self.reg_config.set_mask(
             (value.value & 0b11) << self.__REG_CONFIG_PARITY_MODE,
-            0b11 << self.__REG_CONFIG_PARITY_MODE)
+            0b11 << self.__REG_CONFIG_PARITY_MODE,
+        )
 
     @property
     def trigger_tx(self):
         """
         Enable or disable trigger upon transmission.
         :type: bool
         """
@@ -1212,86 +1009,90 @@
     @trigger_long.setter
     def trigger_long(self, value):
         # We want until transmission is ready to avoid triggering on a pending
         # one.
         self.reg_config.set_bit(
             self.__REG_CONFIG_TRIGGER_LONG,
             value,
-            poll=self.reg_status,
-            poll_mask=1 << self.__REG_STATUS_BIT_READY,
-            poll_value=1 << self.__REG_STATUS_BIT_READY)
+            self.reg_status.poll(
+                mask=1 << self.__REG_STATUS_BIT_READY,
+                value=1 << self.__REG_STATUS_BIT_READY,
+            ),
+        )
 
 
 class I2CNackError(Exception):
     """
     This exception is thrown by I2C peripheral when a transaction received a
     NACK from the I2C slave.
     """
+
     def __init__(self, index):
         """
         :param index: NACKed byte index. If N, then the N-th byte has not been
             acked.
         :type index: int
         """
         super().__init__()
         self.index = index
 
     def __str__(self):
-        """ :return: Error details on the NACKed I2C transaction. """
+        """:return: Error details on the NACKed I2C transaction."""
         return f"Byte of index {self.index} NACKed during I2C transaction."
 
 
 class I2C(Module):
     """
     I2C module of Scaffold.
     """
+
     __REG_STATUS_BIT_READY = 0
     __REG_STATUS_BIT_NACK = 1
     __REG_STATUS_BIT_DATA_AVAIL = 2
     __REG_CONTROL_BIT_START = 0
     __REG_CONTROL_BIT_FLUSH = 1
     __REG_CONFIG_BIT_TRIGGER_START = 0
     __REG_CONFIG_BIT_TRIGGER_END = 1
     __REG_CONFIG_BIT_CLOCK_STRETCHING = 2
 
     def __init__(self, parent, index):
         """
         :param parent: The Scaffold instance owning the I2C module.
         :param index: I2C module index.
         """
-        super().__init__(parent, f'/i2c{index}')
+        super().__init__(parent, f"/i2c{index}")
         self.__index = index
         # Declare the signals
-        self.add_signals('sda_in', 'sda_out', 'scl_in', 'scl_out', 'trigger')
+        self.add_signals("sda_in", "sda_out", "scl_in", "scl_out", "trigger")
         # Declare the registers
         self.__addr_base = base = 0x0700 + 0x0010 * index
-        self.add_register('status', 'rv', base)
-        self.add_register('control', 'w', base + 1)
-        self.add_register('config', 'w', base + 2)
-        self.add_register('divisor', 'w', base + 3, wideness=2, min_value=1)
-        self.add_register('data', 'rwv', base + 4)
-        self.add_register('size_h', 'rwv', base + 5)
-        self.add_register('size_l', 'rwv', base + 6)
+        self.add_register("status", "rv", base)
+        self.add_register("control", "w", base + 1)
+        self.add_register("config", "w", base + 2)
+        self.add_register("divisor", "w", base + 3, wideness=2, min_value=1)
+        self.add_register("data", "rwv", base + 4)
+        self.add_register("size_h", "rwv", base + 5)
+        self.add_register("size_l", "rwv", base + 6)
         self.address = None
         # Current I2C clock frequency
         self.__cache_frequency = None
 
     def reset_config(self):
         """
         Reset the I2C peripheral to a default configuration.
         """
         self.reg_divisor = 1
         self.reg_size_h = 0
         self.reg_size_l = 0
-        self.reg_config = (
-            (1 << self.__REG_CONFIG_BIT_CLOCK_STRETCHING) |
-            (1 << self.__REG_CONFIG_BIT_TRIGGER_START))
+        self.reg_config = (1 << self.__REG_CONFIG_BIT_CLOCK_STRETCHING) | (
+            1 << self.__REG_CONFIG_BIT_TRIGGER_START
+        )
 
     def flush(self):
-        """ Discards all bytes in the transmission/reception FIFO. """
+        """Discards all bytes in the transmission/reception FIFO."""
         self.reg_control.write(1 << self.__REG_CONTROL_BIT_FLUSH)
 
     def raw_transaction(self, data, read_size, trigger=None):
         """
         Executes an I2C transaction. This is a low-level function which does
         not manage I2C addressing nor read/write mode (those shall already be
         defined in data parameter).
@@ -1310,67 +1111,65 @@
             start and 'b' on transaction end.
         :type trigger: int or str.
         :raises I2CNackError: If a NACK is received during the transaction.
         """
         # Verify trigger parameter before doing anything
         t_start = False
         t_end = False
-        if type(trigger) is int:
+        if isinstance(type(trigger), int):
             if trigger not in range(2):
-                raise ValueError('Invalid trigger parameter')
-            t_start = (trigger == 1)
-        elif type(trigger) is str:
-            t_start = ('a' in trigger)
-            t_end = ('b' in trigger)
+                raise ValueError("Invalid trigger parameter")
+            t_start = trigger == 1
+        elif isinstance(type(trigger), str):
+            t_start = "a" in trigger
+            t_end = "b" in trigger
         else:
             if trigger is not None:
-                raise ValueError('Invalid trigger parameter')
-        # We are going to update many registers. We start a lazy section to
-        # make the update faster: all the acknoledgements of bus write
-        # operations are checked at the end.
-        with self.parent.lazy_section():
-            self.flush()
-            self.reg_size_h = read_size >> 8
-            self.reg_size_l = read_size & 0xff
-            # Preload the FIFO
-            self.reg_data.write(data)
-            # Configure trigger for this transaction
-            config_value = 0
-            if t_start:
-                config_value |= (1 << self.__REG_CONFIG_BIT_TRIGGER_START)
-            if t_end:
-                config_value |= (1 << self.__REG_CONFIG_BIT_TRIGGER_END)
-            # Write config with mask to avoid overwritting clock_stretching
-            # option bit
-            self.reg_config.set_mask(
-                config_value,
-                (1 << self.__REG_CONFIG_BIT_TRIGGER_START) |
-                (1 << self.__REG_CONFIG_BIT_TRIGGER_END))
-            # Start the transaction
-            self.reg_control.write(1 << self.__REG_CONTROL_BIT_START)
-            # End of lazy section. Leaving the scope will automatically check
-            # the responses of the Scaffold write operations.
+                raise ValueError("Invalid trigger parameter")
+        self.flush()
+        self.reg_size_h = read_size >> 8
+        self.reg_size_l = read_size & 0xFF
+        # Preload the FIFO
+        self.reg_data.write(data)
+        # Configure trigger for this transaction
+        config_value = 0
+        if t_start:
+            config_value |= 1 << self.__REG_CONFIG_BIT_TRIGGER_START
+        if t_end:
+            config_value |= 1 << self.__REG_CONFIG_BIT_TRIGGER_END
+        # Write config with mask to avoid overwritting clock_stretching
+        # option bit
+        self.reg_config.set_mask(
+            config_value,
+            (1 << self.__REG_CONFIG_BIT_TRIGGER_START)
+            | (1 << self.__REG_CONFIG_BIT_TRIGGER_END),
+        )
+        # Start the transaction
+        self.reg_control.write(1 << self.__REG_CONTROL_BIT_START)
         # Wait until end of transaction and read NACK flag
         st = self.reg_status.read(
-            poll=self.reg_status,
-            poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-            poll_value=(1 << self.__REG_STATUS_BIT_READY))[0]
+            poll=self.reg_status.poll(
+                mask=(1 << self.__REG_STATUS_BIT_READY),
+                value=(1 << self.__REG_STATUS_BIT_READY),
+            )
+        )[0]
         nacked = (st & (1 << self.__REG_STATUS_BIT_NACK)) != 0
         # Fetch all the bytes which are stored in the FIFO.
         if nacked:
             # Get the number of bytes remaining.
-            remaining = (
-                (self.reg_size_h.get() << 8) + self.reg_size_l.get())
+            remaining = (self.reg_size_h.get() << 8) + self.reg_size_l.get()
             raise I2CNackError(len(data) - remaining - 1)
         else:
             fifo = self.reg_data.read(
                 read_size,
-                poll=self.reg_status,
-                poll_mask=(1 << self.__REG_STATUS_BIT_DATA_AVAIL),
-                poll_value=(1 << self.__REG_STATUS_BIT_DATA_AVAIL))
+                self.reg_status.poll(
+                    mask=(1 << self.__REG_STATUS_BIT_DATA_AVAIL),
+                    value=(1 << self.__REG_STATUS_BIT_DATA_AVAIL),
+                ),
+            )
             # FIFO emptyness verification can be enabled below for debug
             # purpose. This shall always be the case, unless there is an
             # implementation bug. This check is not enabled by default because
             # it will slow down I2C communication.
             # if self.reg_status.get_bit(self.__REG_STATUS_BIT_DATA_AVAIL) \
             #     == 1:
             #     raise RuntimeError('FIFO should be empty')
@@ -1389,32 +1188,32 @@
         """
         result = bytearray()
         assert rw in (0, 1)
         # Check that the address is defined in parameters or in self.address.
         if address is None:
             address = self.address
         if address is None:
-            raise ValueError('I2C transaction address is not defined')
+            raise ValueError("I2C transaction address is not defined")
         # Check address
         if address < 0:
-            raise ValueError('I2C address cannot be negative')
+            raise ValueError("I2C address cannot be negative")
         if address >= 2**11:  # R/W bit counted in address, so 11 bits max
-            raise ValueError('I2C address is too big')
+            raise ValueError("I2C address is too big")
         if address > 2**8:
             # 10 bits addressing mode
             # R/W bit is bit 8.
             if address & 0x10:
-                raise ValueError('I2C address bit 8 (R/W) must be 0')
-            result.append(0xf0 + (address >> 8) + rw)
-            result.append(address & 0x0f)
+                raise ValueError("I2C address bit 8 (R/W) must be 0")
+            result.append(0xF0 + (address >> 8) + rw)
+            result.append(address & 0x0F)
         else:
             # 7 bits addressing mode
             # R/W bit is bit 0.
             if address & 1:
-                raise ValueError('I2C address LSB (R/W) must be 0')
+                raise ValueError("I2C address LSB (R/W) must be 0")
             result.append(address + rw)
         return result
 
     def read(self, size, address=None, trigger=None):
         """
         Perform an I2C read transaction.
 
@@ -1471,56 +1270,58 @@
         """
         return self.__cache_frequency
 
     @frequency.setter
     def frequency(self, value):
         d = round((self.parent.sys_freq / (4 * value)) - 1)
         # Check that the divisor can be stored on 16 bits.
-        if d > 0xffff:
-            raise ValueError('Target frequency is too low.')
+        if d > 0xFFFF:
+            raise ValueError("Target frequency is too low.")
         if d < 1:
-            raise ValueError('Target frequency is too high.')
+            raise ValueError("Target frequency is too high.")
         real = self.parent.sys_freq / (d + 1)
         self.reg_divisor.set(d)
         self.__cache_frequency = real
 
 
 class SPIMode(Enum):
     MASTER = 0
     SLAVE = 1
 
 
 class SPI(Module):
     """
     SPI peripheral of Scaffold.
     """
+
     __REG_STATUS_BIT_READY = 0
     __REG_CONTROL_BIT_CLEAR = 6
     __REG_CONTROL_BIT_TRIGGER = 7
     __REG_CONFIG_BIT_POLARITY = 0
     __REG_CONFIG_BIT_PHASE = 1
     __REG_CONFIG_BIT_MODE = 2
 
     def __init__(self, parent, index):
         """
         :param parent: The Scaffold instance owning the SPI module.
         :param index: SPI module index.
         """
-        super().__init__(parent, f'/spi{index}')
+        super().__init__(parent, f"/spi{index}")
         self.__index = index
         # Declare the signals
-        self.add_signals('miso', 'sck', 'mosi', 'ss', 'trigger')
+        self.add_signals("miso", "sck", "mosi", "ss", "trigger")
         # Declare the registers
         self.__addr_base = base = 0x0800 + 0x0010 * index
-        self.add_register('status', 'rv', base)
-        self.add_register('control', 'w', base + 1)
-        self.add_register('config', 'w', base + 2, reset=0x00)
+        self.add_register("status", "rv", base)
+        self.add_register("control", "w", base + 1)
+        self.add_register("config", "w", base + 2, reset=0x00)
         self.add_register(
-            'divisor', 'w', base + 3, wideness=2, min_value=1, reset=0x1000)
-        self.add_register('data', 'rwv', base + 4)
+            "divisor", "w", base + 3, wideness=2, min_value=1, reset=0x1000
+        )
+        self.add_register("data", "rwv", base + 4)
         # Current SPI clock frequency
         self.__cache_frequency = None
 
     @property
     def polarity(self):
         """
         Clock polarity. 0 or 1.
@@ -1540,27 +1341,28 @@
 
     @phase.setter
     def phase(self, value):
         self.reg_config.set_bit(self.__REG_CONFIG_BIT_PHASE, value)
 
     @property
     def mode(self) -> SPIMode:
-        """ SPI mode """
-        if self.parent.version < '0.8':
+        """SPI mode"""
+        if self.parent.version < "0.8":
             return SPIMode.MASTER
         else:
             return SPIMode(self.reg_config.get_bit(self.__REG_CONFIG_BIT_MODE))
 
     @mode.setter
     def mode(self, value: SPIMode):
-        if self.parent.version < '0.8':
+        if self.parent.version < "0.8":
             if value != SPIMode.MASTER:
                 raise RuntimeError(
-                    'Current FPGA confware only supports master mode. '
-                    'Slave mode requires confware >= 0.8.')
+                    "Current FPGA confware only supports master mode. "
+                    "Slave mode requires confware >= 0.8."
+                )
         else:
             self.reg_config.set_bit(self.__REG_CONFIG_BIT_MODE, value.value)
 
     @property
     def frequency(self):
         """
         Target SPI clock frequency.
@@ -1572,18 +1374,18 @@
         """
         return self.__cache_frequency
 
     @frequency.setter
     def frequency(self, value):
         d = round((self.parent.sys_freq / (4 * value)) - 1)
         # Check that the divisor can be stored on 16 bits.
-        if d > 0xffff:
-            raise ValueError('Target frequency is too low.')
+        if d > 0xFFFF:
+            raise ValueError("Target frequency is too low.")
         if d < 1:
-            raise ValueError('Target frequency is too high.')
+            raise ValueError("Target frequency is too high.")
         real = self.parent.sys_freq / (d + 1)
         self.reg_divisor.set(d)
         self.__cache_frequency = real
 
     def transmit(self, value: int, size: int = 8, trigger=False, read=True):
         """
         Performs a SPI transaction to transmit a value and receive data. If a
@@ -1599,41 +1401,43 @@
         :param read: Set 0 or False to disable received value readout (the
             method will return None). Default is True, but disabling it will
             make this command faster if the returned value can be discarded.
         :return: Received value.
         :rtype: int
         """
         if size not in range(1, 33):
-            raise ValueError('Invalid size for SPI transaction')
+            raise ValueError("Invalid size for SPI transaction")
         if value < 0:
-            raise ValueError('value cannot be negative')
+            raise ValueError("value cannot be negative")
         if value >= (2**size):
-            raise ValueError('value is too high')
+            raise ValueError("value is too high")
         # The value to be transmitted must be loaded in the transmission
         # shift-register, less significant bit first. The buffer will transmit
         # its size most significant bits.
         pad = size
         while pad % 8 != 0:
             value <<= 1
             pad += 1
         remaining = size
         while remaining > 0:
-            self.reg_data.write(value & 0xff)
+            self.reg_data.write(value & 0xFF)
             value >>= 8
             remaining -= 8
         # Start transmission
         if trigger:
             trigger = 1
         self.reg_control.write(
             (trigger << self.__REG_CONTROL_BIT_TRIGGER) + (size - 1),
-            poll=self.reg_status,
-            poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-            poll_value=(1 << self.__REG_STATUS_BIT_READY))
+            self.reg_status.poll(
+                mask=(1 << self.__REG_STATUS_BIT_READY),
+                value=(1 << self.__REG_STATUS_BIT_READY),
+            ),
+        )
         if read:
-            res = self.read_data_buffer((size-1)//8 + 1)
+            res = self.read_data_buffer((size - 1) // 8 + 1)
             # Mask to discard garbage bits from previous operations
             res &= 2**size - 1
             return res
 
     def read_data_buffer(self, n):
         """
         Read n bytes from the internal data buffer.
@@ -1643,105 +1447,106 @@
         :return: int
         """
         # The result bits are pushed from the right into the reception
         # buffer. The reception buffer is read by bytes starting at the
         # less significant byte.
         res = self.reg_data.read(
             n,
-            poll=self.reg_status,
-            poll_mask=(1 << self.__REG_STATUS_BIT_READY),
-            poll_value=(1 << self.__REG_STATUS_BIT_READY))
-        return int.from_bytes(res, 'little')
+            self.reg_status.poll(
+                mask=(1 << self.__REG_STATUS_BIT_READY),
+                value=(1 << self.__REG_STATUS_BIT_READY),
+            ),
+        )
+        return int.from_bytes(res, "little")
 
     def append(self, data: Union[int, bytes]):
         """
         Append data to be returned by the peripheral when configured as a
         slave.
 
         .. warning:: Appended data is stored in an internal FIFO memory of the
             SPI peripheral. Size is limited to 512 bytes, any write beyond that
             limit is discarded without any warning.
 
         :param data: Byte or bytes to be appended.
         """
-        if self.parent.version < '0.8':
-            raise RuntimeError(
-                'SPI slave support requires FPGA confware >= 0.8')
+        if self.parent.version < "0.8":
+            raise RuntimeError("SPI slave support requires FPGA confware >= 0.8")
         if self.mode != SPIMode.SLAVE:
-            raise RuntimeError(
-                'Select slave mode first to append response data.')
+            raise RuntimeError("Select slave mode first to append response data.")
         self.reg_data.write(data)
 
     def clear(self):
         """
         Clear the FIFO memory of the data to be returned by the peripheral when
         configured as a slave.
         """
-        if self.parent.version < '0.8':
-            raise RuntimeError(
-                'SPI slave support requires FPGA confware >= 0.8')
+        if self.parent.version < "0.8":
+            raise RuntimeError("SPI slave support requires FPGA confware >= 0.8")
         self.reg_control.write(1 << self.__REG_CONTROL_BIT_CLEAR)
 
 
 class Chain(Module):
-    """ Chain trigger module. """
+    """Chain trigger module."""
+
     __ADDR_CONTROL = 0x0900
 
     def __init__(self, parent, index, size):
         """
         :param parent: Scaffold instance owning the chain module.
         :type parent: Scaffold
         :param index: Module index.
         :type index: int
         :param size: Number of events in the chain.
         :type size: int
         """
-        super().__init__(parent, f'/chain{index}')
-        self.add_register('control', 'wv', self.__ADDR_CONTROL + index * 0x10)
+        super().__init__(parent, f"/chain{index}")
+        self.add_register("control", "wv", self.__ADDR_CONTROL + index * 0x10)
         for i in range(size):
-            self.add_signal(f'event{i}')
-        self.add_signal('trigger')
+            self.add_signal(f"event{i}")
+        self.add_signal("trigger")
 
     def rearm(self):
-        """ Reset the chain trigger to initial state. """
+        """Reset the chain trigger to initial state."""
         self.reg_control.set(1)
 
 
 class Clock(Module):
     """
     Clock generator module. This peripheral allows generating a clock derived
     from the FPGA system clock using a clock divisor. A second clock can be
     generated and enabled during a short period of time to override the first
     clock, generating clock glitches.
     """
-    __ADDR_CONFIG = 0x0a00
-    __ADDR_DIVISOR_A = 0x0a01
-    __ADDR_DIVISOR_B = 0x0a02
-    __ADDR_COUNT = 0x0a03
+
+    __ADDR_CONFIG = 0x0A00
+    __ADDR_DIVISOR_A = 0x0A01
+    __ADDR_DIVISOR_B = 0x0A02
+    __ADDR_COUNT = 0x0A03
 
     def __init__(self, parent, index):
         """
         :param parent: Scaffold instance owning the clock module.
         :type parent: Scaffold
         :param index: Module index.
         :type index: int
         """
-        super().__init__(parent, f'/clock{index}')
-        self.add_register('config', 'w', self.__ADDR_CONFIG + index * 0x10)
-        self.add_register(
-            'divisor_a', 'w', self.__ADDR_DIVISOR_A + index * 0x10)
-        self.add_register(
-            'divisor_b', 'w', self.__ADDR_DIVISOR_B + index * 0x10)
-        self.add_register('count', 'w', self.__ADDR_COUNT + index * 0x10)
-        self.add_signals('glitch', 'out')
+        super().__init__(parent, f"/clock{index}")
+        self.add_register("config", "w", self.__ADDR_CONFIG + index * 0x10)
+        self.add_register("divisor_a", "w", self.__ADDR_DIVISOR_A + index * 0x10)
+        self.add_register("divisor_b", "w", self.__ADDR_DIVISOR_B + index * 0x10)
+        self.add_register("count", "w", self.__ADDR_COUNT + index * 0x10)
+        self.add_signals("glitch", "out")
 
         self.__freq_helper_a = FreqRegisterHelper(
-            self.parent.sys_freq, self.reg_divisor_a)
+            self.parent.sys_freq, self.reg_divisor_a
+        )
         self.__freq_helper_b = FreqRegisterHelper(
-            self.parent.sys_freq, self.reg_divisor_b)
+            self.parent.sys_freq, self.reg_divisor_b
+        )
 
     @property
     def frequency(self):
         """
         Base clock frequency, in Hertz. Only divisors of the system frequency
         can be set: 50 MHz, 25 MHz, 16.66 MHz, 12.5 MHz...
 
@@ -1810,483 +1615,150 @@
     DOWN = 0b01
 
 
 class IO(Signal, Module):
     """
     Board I/O.
     """
+
     def __init__(self, parent, path, index, pullable=False):
         """
         :param parent: Scaffold instance which the signal belongs to.
         :param path: Signal path string.
         :param index: I/O index.
         :param pullable: True if this I/O supports pull resistor.
         """
         Signal.__init__(self, parent, path)
         Module.__init__(self, parent)
         self.index = index
         self.__pullable = pullable
-        if parent.version == '0.2':
+        if parent.version == "0.2":
             # 0.2 only
             # Since I/O will have more options, it is not very convenient to
             # group them anymore.
             self.__group = index // 8
             self.__group_index = index % 8
-            base = 0xe000 + 0x10 * self.__group
-            self.add_register('value', 'rv', base + 0x00)
-            self.add_register('event', 'rwv', base + 0x01, reset=0)
+            base = 0xE000 + 0x10 * self.__group
+            self.add_register("value", "rv", base + 0x00)
+            self.add_register("event", "rwv", base + 0x01, reset=0)
         else:
             # 0.3
-            base = 0xe000 + 0x10 * self.index
-            self.add_register('value', 'rwv', base + 0x00, reset=0)
-            self.add_register('config', 'rw', base + 0x01, reset=0)
+            base = 0xE000 + 0x10 * self.index
+            self.add_register("value", "rwv", base + 0x00, reset=0)
+            self.add_register("config", "rw", base + 0x01, reset=0)
             # No more event register in 0.3. Events are in the value register
 
     @property
     def value(self):
         """
         Current IO logical state.
 
         :getter: Senses the input pin of the board and return either 0 or 1.
         :setter: Sets the output to 0, 1 or high-impedance state (None). This
             will disconnect the I/O from any already connected internal
             peripheral. Same effect can be achieved using << operator.
         """
-        if self.parent.version == '0.2':
+        if self.parent.version == "0.2":
             return (self.reg_value.get() >> self.__group_index) & 1
         else:
             # 0.3
             return self.reg_value.get_bit(0)
 
     @property
     def event(self):
         """
         I/O event register.
 
         :getter: Returns 1 if an event has been detected on this input, 0
             otherwise.
         :setter: Writing 0 to clears the event flag. Writing 1 has no effect.
         """
-        if self.parent.version == '0.2':
+        if self.parent.version == "0.2":
             return (self.reg_event.get() >> self.__group_index) & 1
         else:
             # 0.3
             return self.reg_value.get_bit(1)
 
     def clear_event(self):
         """
         Clear event register.
 
         :warning: If an event is received during this call, it may be cleared
             without being took into account.
         """
-        if self.parent.version == '0.2':
-            self.reg_event.set(0xff ^ (1 << self.__group_index))
+        if self.parent.version == "0.2":
+            self.reg_event.set(0xFF ^ (1 << self.__group_index))
         else:
             # 0.3
             self.reg_value.set(0)
 
     @property
     def mode(self):
         """
         I/O mode. Default is AUTO, but this can be overriden for special
         applications.
 
         :type: IOMode
         """
-        assert self.parent.version >= '0.3'
+        assert self.parent.version >= "0.3"
         return IOMode(self.reg_config.get() & 0b11)
 
     @mode.setter
     def mode(self, value):
-        assert self.parent.version >= '0.3'
+        assert self.parent.version >= "0.3"
         if not isinstance(value, IOMode):
-            raise ValueError('mode must be an instance of IOMode enumeration')
+            raise ValueError("mode must be an instance of IOMode enumeration")
         self.reg_config.set_mask(value.value, 0b11)
 
     @property
     def pull(self):
         """
         Pull resistor mode. Can only be written if the I/O supports this
         feature.
 
         :type: Pull
         """
-        assert self.parent.version >= '0.3'
+        assert self.parent.version >= "0.3"
         if not self.__pullable:
             return Pull.NONE
         return Pull((self.reg_config.get() >> 2) & 0b11)
 
     @pull.setter
     def pull(self, value):
-        assert self.parent.version >= '0.3'
+        assert self.parent.version >= "0.3"
         # Accept None as value
         if value is None:
             value = Pull.NONE
         if (not self.__pullable) and (value != Pull.NONE):
-            raise RuntimeError('This I/O does not support pull resistor')
+            raise RuntimeError("This I/O does not support pull resistor")
         self.reg_config.set_mask(value.value << 2, 0b1100)
 
 
-class ScaffoldBusLazySection:
-    """
-    Helper class to be sure the opened lazy sections are closed at some time.
-    """
-    def __init__(self, bus):
-        self.bus = bus
-
-    def __enter__(self):
-        self.bus.lazy_start()
-
-    def __exit__(self, type, value, traceback):
-        self.bus.lazy_end()
-
-
-class ScaffoldBusTimeoutSection:
-    """
-    Helper class to be sure a pushed timeout configuration is poped at some
-    time. This is to be used with the python 'with' statement.
-    """
-    def __init__(self, bus, timeout):
-        """
-        :param bus: Scaffold bus manager.
-        :type bus: ScaffoldBus
-        :param timeout: Section timeout value, in seconds.
-        :type timeout: int, float
-        """
-        self.bus = bus
-        self.timeout = timeout
-
-    def __enter__(self):
-        self.bus.push_timeout(self.timeout)
-
-    def __exit__(self, type, value, traceback):
-        self.bus.pop_timeout()
-
-
-class ScaffoldBus:
-    """
-    Low level methods to drive the Scaffold device.
-    """
-    MAX_CHUNK = 255
-    FIFO_SIZE = 512
-
-    def __init__(self, sys_freq, baudrate):
-        """
-        :param baudrate: UART baudrate
-        :type baudrate: int
-        """
-        self.__baudrate = baudrate
-        self.sys_freq = sys_freq
-        # How long in seconds one timeout unit is.
-        self.timeout_unit = (3.0/self.sys_freq)
-        self.ser = None
-        self.__lazy_writes = []
-        self.__lazy_fifo_total_size = 0
-        self.__lazy_fifo_sizes = []
-        self.__lazy_stack = 0
-        # Timeout value. This value can't be read from the board, so we cache
-        # it there once set.
-        self.__cache_timeout = None
-        # Timeout stack for push_timeout and pop_timeout methods.
-        self.__timeout_stack = []
-
-    def connect(self, dev):
-        """
-        Connect to Scaffold board using the given serial port.
-        :param dev: Serial port device path. For instance '/dev/ttyUSB0' on
-            linux, 'COM0' on Windows.
-        """
-        self.ser = serial.Serial(dev, self.__baudrate)
-
-    def prepare_datagram(
-            self, rw, addr, size, poll, poll_mask, poll_value):
-        """
-        Helper function to build the datagrams to be sent to the Scaffold
-        device. Also performs basic check on arguments.
-        :rw: 1 for a write command, 0 for a read command.
-        :addr: Register address.
-        :size: Size of the data to be sent or received. Maximum size is 255.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :poll_mask: Register polling mask.
-        :poll_value: Register polling value.
-        :return: A bytearray.
-        """
-        if rw not in range(2):
-            raise ValueError('Invalid rw argument')
-        if size not in range(1, self.MAX_CHUNK+1):
-            raise ValueError('Invalid size')
-        if addr not in range(0x10000):
-            raise ValueError('Invalid address')
-        if isinstance(poll, Register):
-            poll = poll.address
-        if (poll is not None) and (poll not in range(0x10000)):
-            raise ValueError('Invalid polling address')
-        command = rw
-        if size > 1:
-            command |= 2
-        if poll is not None:
-            command |= 4
-        datagram = bytearray()
-        datagram.append(command)
-        datagram.append(addr >> 8)
-        datagram.append(addr & 0xff)
-        if poll is not None:
-            datagram.append(poll >> 8)
-            datagram.append(poll & 0xff)
-            datagram.append(poll_mask)
-            datagram.append(poll_value)
-        if size > 1:
-            datagram.append(size)
-        return datagram
-
-    def write(
-            self, addr, data, poll=None, poll_mask=0xff, poll_value=0x00):
-        """
-        Write data to a register.
-        :param addr: Register address.
-        :param data: Data to be written. Can be a byte, bytes or bytearray.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        """
-        if self.ser is None:
-            raise RuntimeError('Not connected to board')
-
-        # If data is an int, convert it to bytes.
-        if type(data) is int:
-            data = bytes([data])
-
-        offset = 0
-        remaining = len(data)
-        while remaining:
-            chunk_size = min(self.MAX_CHUNK, remaining)
-            datagram = self.prepare_datagram(
-                1, addr, chunk_size, poll, poll_mask, poll_value)
-            datagram += data[offset:offset + chunk_size]
-            assert len(datagram) < self.FIFO_SIZE
-            if self.__lazy_stack == 0:
-                self.ser.write(datagram)
-                # Check immediately the result of the write operation.
-                ack = self.ser.read(1)[0]
-                if ack != chunk_size:
-                    assert poll is not None
-                    # Timeout error !
-                    raise TimeoutError(
-                        size=offset+ack, expected=offset+chunk_size)
-            else:
-                # Lazy-update section. The write result will be checked later,
-                # when all lazy-sections are closed.
-                dg_len = len(datagram)
-                # We don't know how many write datagram have been processed
-                # until we don't fetch the responses. It is possible to
-                # overflow the hardware FIFO if a polling operation is
-                # blocking. We have to check for those potential troubles.
-                while self.__lazy_fifo_total_size + dg_len > self.FIFO_SIZE:
-                    # FIFO might be full. We must process some responses to get
-                    # some guaranteed FIFO space
-                    expected_size = self.__lazy_writes[0]
-                    # Following read will block if first operation in the FIFO
-                    # is still pending.
-                    ack = self.ser.read(1)[0]
-                    del self.__lazy_writes[0]
-                    self.__lazy_fifo_total_size -= self.__lazy_fifo_sizes[0]
-                    del self.__lazy_fifo_sizes[0]
-                    if ack != expected_size:
-                        # Timeout error !
-                        raise TimeoutError(size=ack, expected=expected_size)
-                self.__lazy_fifo_total_size += dg_len
-                self.__lazy_fifo_sizes.append(dg_len)
-                self.ser.write(datagram)
-                self.__lazy_writes.append(chunk_size)
-            remaining -= chunk_size
-            offset += chunk_size
-
-    def read(
-            self, addr, size=1, poll=None, poll_mask=0xff,
-            poll_value=0x00):
-        """
-        Read data from a register.
-        :param addr: Register address.
-        :param poll: Register instance or address. None if polling is not
-            required.
-        :param poll_mask: Register polling mask.
-        :param poll_value: Register polling value.
-        :return: bytearray
-        """
-        if self.ser is None:
-            raise RuntimeError('Not connected to board')
-        # Read operation not permitted during lazy-update sections
-        if self.__lazy_stack > 0:
-            raise RuntimeError(
-                'Read operations not allowed during lazy-update section.')
-        result = bytearray()
-        remaining = size
-        offset = 0
-        while remaining:
-            chunk_size = min(self.MAX_CHUNK, remaining)
-            datagram = self.prepare_datagram(
-                0, addr, chunk_size, poll, poll_mask, poll_value)
-            self.ser.write(datagram)
-            res = self.ser.read(chunk_size+1)
-            ack = res[-1]
-            if ack != chunk_size:
-                assert poll is not None
-                result += res[:ack]
-                raise TimeoutError(data=result, expected=chunk_size+offset)
-            result += res[:-1]
-            remaining -= chunk_size
-            offset += chunk_size
-        return result
-
-    def __set_timeout_raw(self, value):
-        """
-        Configure the polling timeout register.
-
-        :param value: Timeout register value. If 0 the timeout is disabled. One
-            unit corresponds to three FPGA system clock cycles.
-        """
-        if (value < 0) or (value > 0xffffffff):
-            raise ValueError('Timeout value out of range')
-        datagram = bytearray()
-        datagram.append(0x08)
-        datagram += value.to_bytes(4, 'big', signed=False)
-        self.ser.write(datagram)
-        # No response expected from the board
-
-    @property
-    def is_connected(self):
-        return self.set is not None
-
-    def lazy_start(self):
-        """
-        Enters lazy-check update block, or add a block level if already in
-        lazy-check mode. When lazy-check is enabled, the result of write
-        operations on Scaffold bus are not checked immediately, but only when
-        leaving all blocks. This allows updating many different registers
-        without the serial latency because all the responses will be checked at
-        once.
-        """
-        self.__lazy_stack += 1
-
-    def lazy_end(self):
-        """
-        Close current lazy-update block. If this was the last lazy section,
-        fetch all responses from Scaffold and check that all write operations
-        went good. If any write-operation timed-out, the last TimeoutError is
-        thrown.
-        """
-        if self.__lazy_stack == 0:
-            raise RuntimeError('No lazy section started')
-        self.__lazy_stack -= 1
-        last_error = None
-        if self.__lazy_stack == 0:
-            # We closes all update blocks, we must now check all responses of
-            # write requests.
-            for expected_size in self.__lazy_writes:
-                ack = self.ser.read(1)[0]
-                if ack != expected_size:
-                    # Timeout error !
-                    last_error = TimeoutError(size=ack, expected=expected_size)
-            self.__lazy_writes.clear()
-            # All writes have been processed, we know the FIFO buffer is empty.
-            self.__lazy_fifo_total_size = 0
-            self.__lazy_fifo_sizes.clear()
-            if last_error is not None:
-                raise last_error
-
-    @property
-    def timeout(self) -> Optional[float]:
-        """
-        Timeout in seconds for read and write commands. If set to None, timeout
-        is disabled.
-        """
-        if self.__cache_timeout is None:
-            return RuntimeError('Timeout not set yet')
-        if self.__cache_timeout == 0:
-            return None
-        else:
-            return self.__cache_timeout * self.timeout_unit
-
-    @timeout.setter
-    def timeout(self, value: Optional[float]):
-        if value is None:
-            n = 0
-        else:
-            n = max(1, int(value / self.timeout_unit))
-        if n != self.__cache_timeout:
-            self.__set_timeout_raw(n)  # May throw is n out of range.
-            self.__cache_timeout = n  # Must be after set_timeout
-
-    def push_timeout(self, value):
-        """
-        Save previous timeout setting in a stack, and set a new timeout value.
-        Call to `pop_timeout` will restore previous timeout value.
-        The new effective timeout will be lower or equal to the current
-        timeout. That is, the timeout cannot be increased, previous defined
-        timeout have higher priority.
-
-        :param value: New timeout value, in seconds.
-        """
-        if value is None:
-            value = self.timeout
-        else:
-            if self.timeout is not None:
-                value = min(self.timeout, value)
-        self.__timeout_stack.append(self.timeout)
-        self.timeout = value
-
-    def pop_timeout(self):
-        """
-        Restore timeout setting from stack.
-
-        :raises RuntimeError: if timeout stack is already empty.
-        """
-        if len(self.__timeout_stack) == 0:
-            raise RuntimeError('Timeout setting stack is empty')
-        self.timeout = self.__timeout_stack.pop()
-
-    def lazy_section(self):
-        """
-        :return: ScaffoldBusLazySection to be used with the python 'with'
-            tatement to start and close a lazy update section.
-        """
-        return ScaffoldBusLazySection(self)
-
-    def timeout_section(self, timeout):
-        """
-        :return: :class:`ScaffoldBusTimeoutSection` to be used with the python
-            'with' statement to start and close a timeout section.
-        """
-        return ScaffoldBusTimeoutSection(self, timeout)
-
-
 class IODir(Enum):
     """
     I/O direction mode.
     """
+
     INPUT = 0
     OUTPUT = 1
 
 
 class ArchBase:
     """
     Base class for Scaffold API.
     The :class:`Scaffold` class inherits from this class and defines which
     modules and signals are defined on the board. This class can be inherited
     to create other boards than Scaffold sharing the same architecture
     principle.
     """
-    __ADDR_MTXR_BASE = 0xf100
-    __ADDR_MTXL_BASE = 0xf000
 
-    def __init__(self, sys_freq, board_name, supported_versions,
-                 baudrate=2000000):
+    __ADDR_MTXR_BASE = 0xF100
+    __ADDR_MTXL_BASE = 0xF000
+
+    def __init__(self, sys_freq, board_name, supported_versions, baudrate=2000000):
         """
         Defines basic parameters of the board.
 
         :param sys_freq: Architecture system frequency, in Hertz.
         :type sys_freq: int
         :param board_name: Expected board name during version string readout.
         :type board_name: str
@@ -2380,70 +1852,74 @@
             Must be `None` when `dev` is set.
         """
         if dev is None:
             # Try to find automatically the device
             possible_ports = []
             for port in serial.tools.list_ports.comports():
                 # USB description string can be 'Scaffold', with uppercase 'S'.
-                if ((port.product is not None)
-                        and (port.product.lower() ==
-                             self.__expected_board_name)
-                        and ((sn is None) or (port.serial_number == sn))):
+                if (
+                    (port.product is not None)
+                    and (port.product.lower() == self.__expected_board_name)
+                    and ((sn is None) or (port.serial_number == sn))
+                ):
                     possible_ports.append(port)
             if len(possible_ports) > 1:
                 raise RuntimeError(
-                    'Multiple ' + self.__expected_board_name +
-                    ' devices found! I don\'t know which one to use.')
+                    "Multiple "
+                    + self.__expected_board_name
+                    + " devices found! I don't know which one to use."
+                )
             elif len(possible_ports) == 1:
                 dev = possible_ports[0].device
             else:
-                raise RuntimeError(
-                    'No ' + self.__expected_board_name + ' device found')
+                raise RuntimeError("No " + self.__expected_board_name + " device found")
         else:
             if sn is not None:
                 raise ValueError("dev and sn cannot be set together")
 
         self.bus.connect(dev)
         # Check hardware responds and has the correct version.
         self.__version_string = self.__version_module.get_string()
         # Split board name and version string
-        tokens = self.__version_string.split('-')
+        tokens = self.__version_string.split("-")
         if len(tokens) != 2:
             raise RuntimeError(
-                'Failed to parse board version string \''
-                + self.__version_string + '\'')
+                "Failed to parse board version string '" + self.__version_string + "'"
+            )
         self.__board_name = tokens[0]
         self.__version = tokens[1]
         if self.__board_name != self.__expected_board_name:
-            raise RuntimeError('Invalid board name during version check')
+            raise RuntimeError("Invalid board name during version check")
         if self.__version not in self.__supported_versions:
-            raise RuntimeError(
-                'Hardware version ' + self.__version + ' not supported')
+            raise RuntimeError("Hardware version " + self.__version + " not supported")
+        # Tell ScaffoldBus the current version. If version is >= 0.9, delays and buffer
+        # wait operations will be enabled.
+        self.bus.version = self.__version
 
     def __signal_to_path(self, signal):
         """
         Convert a signal, 0, 1 or None to a path. Verify the signal belongs to
         the current Scaffold instance.
         :param signal: Signal, 0, 1 or None.
         :return: Path string.
         """
         if isinstance(signal, Signal):
             if signal.parent != self:
-                raise ValueError('Signal belongs to another Scaffold instance')
+                raise ValueError("Signal belongs to another Scaffold instance")
             return signal.path
         elif type(signal) is int:
             if signal not in (0, 1):
-                raise ValueError('Invalid signal value')
+                raise ValueError("Invalid signal value")
             return str(signal)
         elif type(signal) is int:
             return str(signal)
         elif signal is None:
-            return 'z'  # High impedance
+            return "z"  # High impedance
         else:
-            raise ValueError('Invalid signal type')
+            raise ValueError("Invalid signal type")
 
     def sig_connect(self, a, b):
         """
         Configure interconnect matrices to feed the signal a with the signal b.
 
         :param a: Destination signal.
         :type a: Signal
@@ -2451,54 +1927,54 @@
         :type b: Signal
         """
         # Check both signals belongs to the current board instance
         # Convert signals to path names
         dest_path = self.__signal_to_path(a)
         src_path = self.__signal_to_path(b)
 
-        dest_in_mtxr_out = (dest_path in self.mtxr_out)
-        dest_in_mtxl_out = (dest_path in self.mtxl_out)
+        dest_in_mtxr_out = dest_path in self.mtxr_out
+        dest_in_mtxl_out = dest_path in self.mtxl_out
         if not (dest_in_mtxr_out or dest_in_mtxl_out):
             # Shall never happen unless there is a bug
-            raise RuntimeError(f'Invalid destination path \'{dest_path}\'')
-        src_in_mtxl_in = (src_path in self.mtxl_in)
-        src_in_mtxr_in = (src_path in self.mtxr_in)
+            raise RuntimeError(f"Invalid destination path '{dest_path}'")
+        src_in_mtxl_in = src_path in self.mtxl_in
+        src_in_mtxr_in = src_path in self.mtxr_in
         # Beware: we can have a dest signal with the same name in mtxr and
         # mtxl.
         if dest_in_mtxr_out and src_in_mtxr_in:
             if dest_in_mtxl_out and src_in_mtxl_in:
                 # Shall never happen unless a module output has the same name
                 # as one of its input.
                 raise RuntimeError(
-                    f'Connection ambiguity \'{dest_path}\' << '
-                    + f'\'{src_path}\'.')
+                    f"Connection ambiguity '{dest_path}' << " + f"'{src_path}'."
+                )
             # Connect a module output to an IO output
             src_index = self.mtxr_in.index(src_path)
             dst_index = self.mtxr_out.index(dest_path)
             self.bus.write(self.__ADDR_MTXR_BASE + dst_index, src_index)
         elif dest_in_mtxl_out and src_in_mtxl_in:
             # Connect a module input to an IO input (or 0 or 1).
             src_index = self.mtxl_in.index(src_path)
             dst_index = self.mtxl_out.index(dest_path)
             self.bus.write(self.__ADDR_MTXL_BASE + dst_index, src_index)
         else:
             # Shall never happen unless there is a bug
             raise RuntimeError(
-                f'Failed to connect \'{dest_path}\' << ' + f'\'{src_path}\'.')
+                f"Failed to connect '{dest_path}' << " + f"'{src_path}'."
+            )
 
     def sig_disconnect_all(self):
         """
         Disconnects all input and output signals. This is called during
         initialization to reset the board in a known state.
         """
-        with self.lazy_section():
-            for i in range(len(self.mtxl_out)):
-                self.bus.write(self.__ADDR_MTXL_BASE + i, 0)
-            for i in range(len(self.mtxr_out)):
-                self.bus.write(self.__ADDR_MTXR_BASE + i, 0)
+        for i in range(len(self.mtxl_out)):
+            self.bus.write(self.__ADDR_MTXL_BASE + i, 0)
+        for i in range(len(self.mtxr_out)):
+            self.bus.write(self.__ADDR_MTXR_BASE + i, 0)
 
     @property
     def timeout(self):
         """
         Timeout in seconds for read and write commands. If set to 0, timeout is
         disabled.
         """
@@ -2521,28 +1997,37 @@
         """
         Restore timeout setting from stack.
 
         :raises RuntimeError: if timeout stack is already empty.
         """
         self.bus.pop_timeout()
 
-    def lazy_section(self):
-        """
-        :return: ScaffoldBusLazySection to be used with the python 'with'
-            statement to start and close a lazy update section.
-        """
-        return self.bus.lazy_section()
-
     def timeout_section(self, timeout):
         """
         :return: :class:`ScaffoldBusTimeoutSection` instance to be used with
             the python 'with' statement to push and pop timeout configuration.
         """
         return self.bus.timeout_section(timeout)
 
+    def buffer_wait_section(self):
+        return self.bus.buffer_wait_section()
+
+    def delay(self, duration: float):
+        """
+        Performs a delay operation.
+
+        :param cycles: Delay duration in seconds.
+        """
+        cycles = round(duration * self.sys_freq)
+        self.bus.delay(cycles)
+
+    def wait(self):
+        """Wait for all pending operations to be completed."""
+        self.bus.wait()
+
 
 class Scaffold(ArchBase):
     """
     This class connects to a Scaffold board and provides access to all the
     device parameters and peripherals.
 
     :ivar uarts: list of :class:`scaffold.UART` instance managing UART
@@ -2557,26 +2042,31 @@
         power supplies of DUT and platform sockets.
     :ivar leds: :class:`scaffold.LEDs` instance, managing LEDs brightness and
         lighting mode.
     :ivar [a0,a1,a2,a3,b0,b1,c0,c1,d0,d1,d2,d3,d4,d5]: :class:`scaffold.Signal`
         instances for connecting and controlling the corresponding I/Os of the
         board.
     """
+
     # Number of I/Os
     __IO_D_COUNT = 16
     __IO_P_COUNT = 16
     # Number of UART peripherals
     __UART_COUNT = 2
     # Number of pulse generator peripherals
     __PULSE_GENERATOR_COUNT = 4
     # Number of I2C modules
     __I2C_COUNT = 1
 
-    def __init__(self, dev: Optional[str] = None, init_ios: bool = False,
-                 sn: Optional[str] = None):
+    def __init__(
+        self,
+        dev: Optional[str] = None,
+        init_ios: bool = False,
+        sn: Optional[str] = None,
+    ):
         """
         Create Scaffold API instance.
 
         :param dev: If specified, connect to the hardware Scaffold board using
             the given serial device. If None, tries to find automatically the
             device by scanning USB description strings.
         :param init_ios: True to enable I/Os peripherals initialization. Doing
@@ -2586,22 +2076,26 @@
             sessions.
         :param sn: If `dev` is not specified, automatic detection must find a
             board with the given serial number. This is an interesting feature
             when multiple Scaffold boards are connected to the same computer.
         """
         super().__init__(
             100e6,  # System frequency: 100 MHz
-            'scaffold',  # board name
+            "scaffold",  # board name
             # Supported FPGA bitstream versions
-            ('0.2', '0.3', '0.4', '0.5', '0.6', '0.7', '0.7.1', '0.7.2', '0.8')
+            ("0.2", "0.3", "0.4", "0.5", "0.6", "0.7", "0.7.1", "0.7.2", "0.8", "0.9"),
         )
         self.connect(dev, init_ios, sn)
 
-    def connect(self, dev: Optional[str] = None, init_ios: bool = False,
-                sn: Optional[str] = None):
+    def connect(
+        self,
+        dev: Optional[str] = None,
+        init_ios: bool = False,
+        sn: Optional[str] = None,
+    ):
         """
         Connect to Scaffold board using the given serial port.
 
         :param dev: Serial port device path. For instance '/dev/ttyUSB0' on
             linux, 'COM0' on Windows.
         :param init_ios: True to enable I/Os peripherals initialization. Doing
             so will set all I/Os to a default state, but it may generate pulses
@@ -2619,230 +2113,228 @@
         # Leds module
         self.leds = LEDs(self)
 
         # Create the IO signals
         # Scaffold hardware v1 has FPGA arch version <= 0.3
         # Scaffold hardware v1.1 has FPGA arch version >= 0.4
         # The I/Os have changed between both versions.
-        self.a0 = IO(self, '/io/a0', 0)
-        self.a1 = IO(self, '/io/a1', 1)
-        if self.version <= '0.3':
-            self.b0 = IO(self, '/io/b0', 2)
-            self.b1 = IO(self, '/io/b1', 3)
-            self.c0 = IO(self, '/io/c0', 4)
-            self.c1 = IO(self, '/io/c1', 5)
+        self.a0 = IO(self, "/io/a0", 0)
+        self.a1 = IO(self, "/io/a1", 1)
+        if self.version <= "0.3":
+            self.b0 = IO(self, "/io/b0", 2)
+            self.b1 = IO(self, "/io/b1", 3)
+            self.c0 = IO(self, "/io/c0", 4)
+            self.c1 = IO(self, "/io/c1", 5)
             for i in range(self.__IO_D_COUNT):
-                self.__setattr__(f'd{i}', IO(self, f'/io/d{i}', i+6))
+                self.__setattr__(f"d{i}", IO(self, f"/io/d{i}", i + 6))
         else:
-            self.a2 = IO(self, '/io/a2', 1)
-            self.a3 = IO(self, '/io/a3', 1)
+            self.a2 = IO(self, "/io/a2", 1)
+            self.a3 = IO(self, "/io/a3", 1)
             for i in range(self.__IO_D_COUNT):
                 # Only D0, D1 and D2 can be pulled in Scaffold hardware v1.1.
                 self.__setattr__(
-                    f'd{i}', IO(self, f'/io/d{i}', i + 4, pullable=(i < 3)))
-            if self.version >= '0.6':
+                    f"d{i}", IO(self, f"/io/d{i}", i + 4, pullable=(i < 3))
+                )
+            if self.version >= "0.6":
                 for i in range(self.__IO_P_COUNT):
                     self.__setattr__(
-                        f'p{i}',
-                        IO(self, f'/io/p{i}', i + 4 + self.__IO_D_COUNT))
+                        f"p{i}", IO(self, f"/io/p{i}", i + 4 + self.__IO_D_COUNT)
+                    )
 
         # Create the UART modules
         self.uarts = []
         for i in range(self.__UART_COUNT):
             uart = UART(self, i)
             self.uarts.append(uart)
-            self.__setattr__(f'uart{i}', uart)
+            self.__setattr__(f"uart{i}", uart)
 
         # Create the pulse generator modules
         self.pgens = []
         for i in range(self.__PULSE_GENERATOR_COUNT):
-            pgen = PulseGenerator(self, f'/pgen{i}', 0x0300 + 0x10*i)
+            pgen = PulseGenerator(self, f"/pgen{i}", 0x0300 + 0x10 * i)
             self.pgens.append(pgen)
-            self.__setattr__(f'pgen{i}', pgen)
+            self.__setattr__(f"pgen{i}", pgen)
 
         # Declare the I2C peripherals
         self.i2cs = []
         for i in range(self.__I2C_COUNT):
             i2c = I2C(self, i)
             self.i2cs.append(i2c)
-            self.__setattr__(f'i2c{i}', i2c)
+            self.__setattr__(f"i2c{i}", i2c)
 
         # Declare the SPI peripherals
         self.spis = []
-        if self.version >= '0.7':
+        if self.version >= "0.7":
             for i in range(1):
                 spi = SPI(self, i)
                 self.spis.append(spi)
-                self.__setattr__(f'spi{i}', spi)
+                self.__setattr__(f"spi{i}", spi)
 
         # Declare the trigger chain modules
         self.chains = []
-        if self.version >= '0.7':
+        if self.version >= "0.7":
             for i in range(2):
                 chain = Chain(self, i, 3)
                 self.chains.append(chain)
-                self.__setattr__(f'chain{i}', chain)
+                self.__setattr__(f"chain{i}", chain)
 
         # Declare clock generation module
         self.clocks = []
-        if self.version >= '0.7':
+        if self.version >= "0.7":
             for i in range(1):
                 clock = Clock(self, i)
                 self.clocks.append(clock)
-                self.__setattr__(f'clock{i}', clock)
+                self.__setattr__(f"clock{i}", clock)
 
         # Create the ISO7816 module
         self.iso7816 = ISO7816(self)
 
         # FPGA left matrix input signals
-        self.add_mtxl_in('0')
-        self.add_mtxl_in('1')
-        self.add_mtxl_in('/io/a0')
-        self.add_mtxl_in('/io/a1')
-        if self.version <= '0.3':
+        self.add_mtxl_in("0")
+        self.add_mtxl_in("1")
+        self.add_mtxl_in("/io/a0")
+        self.add_mtxl_in("/io/a1")
+        if self.version <= "0.3":
             # Scaffold hardware v1 only
-            self.add_mtxl_in('/io/b0')
-            self.add_mtxl_in('/io/b1')
-            self.add_mtxl_in('/io/c0')
-            self.add_mtxl_in('/io/c1')
+            self.add_mtxl_in("/io/b0")
+            self.add_mtxl_in("/io/b1")
+            self.add_mtxl_in("/io/c0")
+            self.add_mtxl_in("/io/c1")
         else:
             # Scaffold hardware v1.1
-            self.add_mtxl_in('/io/a2')
-            self.add_mtxl_in('/io/a3')
+            self.add_mtxl_in("/io/a2")
+            self.add_mtxl_in("/io/a3")
         for i in range(self.__IO_D_COUNT):
-            self.add_mtxl_in(f'/io/d{i}')
-        if self.version >= '0.6':
+            self.add_mtxl_in(f"/io/d{i}")
+        if self.version >= "0.6":
             for i in range(self.__IO_P_COUNT):
-                self.add_mtxl_in(f'/io/p{i}')
-        if self.version >= '0.7':
+                self.add_mtxl_in(f"/io/p{i}")
+        if self.version >= "0.7":
             # Feeback signals from module outputs (mostly triggers)
             for i in range(len(self.uarts)):
-                self.add_mtxl_in(f'/uart{i}/trigger')
-            self.add_mtxl_in('/iso7816/trigger')
+                self.add_mtxl_in(f"/uart{i}/trigger")
+            self.add_mtxl_in("/iso7816/trigger")
             for i in range(len(self.i2cs)):
-                self.add_mtxl_in(f'/i2c{i}/trigger')
+                self.add_mtxl_in(f"/i2c{i}/trigger")
             for i in range(len(self.spis)):
-                self.add_mtxl_in(f'/spi{i}/trigger')
+                self.add_mtxl_in(f"/spi{i}/trigger")
             for i in range(len(self.pgens)):
-                self.add_mtxl_in(f'/pgen{i}/out')
+                self.add_mtxl_in(f"/pgen{i}/out")
             for i in range(len(self.chains)):
-                self.add_mtxl_in(f'/chain{i}/trigger')
+                self.add_mtxl_in(f"/chain{i}/trigger")
 
         # FPGA left matrix output signals
         # Update this section when adding new modules with inputs
         for i in range(self.__UART_COUNT):
-            self.add_mtxl_out(f'/uart{i}/rx')
-        self.add_mtxl_out('/iso7816/io_in')
+            self.add_mtxl_out(f"/uart{i}/rx")
+        self.add_mtxl_out("/iso7816/io_in")
         for i in range(self.__PULSE_GENERATOR_COUNT):
-            self.add_mtxl_out(f'/pgen{i}/start')
+            self.add_mtxl_out(f"/pgen{i}/start")
         for i in range(self.__I2C_COUNT):
-            self.add_mtxl_out(f'/i2c{i}/sda_in')
-            self.add_mtxl_out(f'/i2c{i}/scl_in')
+            self.add_mtxl_out(f"/i2c{i}/sda_in")
+            self.add_mtxl_out(f"/i2c{i}/scl_in")
         for i in range(len(self.spis)):
-            self.add_mtxl_out(f'/spi{i}/miso')
+            self.add_mtxl_out(f"/spi{i}/miso")
         for i in range(len(self.spis)):
-            self.add_mtxl_out(f'/spi{i}/sck')
-            self.add_mtxl_out(f'/spi{i}/ss')
+            self.add_mtxl_out(f"/spi{i}/sck")
+            self.add_mtxl_out(f"/spi{i}/ss")
         for i in range(len(self.chains)):
             for j in range(3):  # 3 is the number of chain events
-                self.add_mtxl_out(f'/chain{i}/event{j}')
+                self.add_mtxl_out(f"/chain{i}/event{j}")
         for i in range(len(self.clocks)):
-            self.add_mtxl_out(f'/clock{i}/glitch')
+            self.add_mtxl_out(f"/clock{i}/glitch")
 
         # FPGA right matrix input signals
         # Update this section when adding new modules with outpus
-        self.add_mtxr_in('z')
-        self.add_mtxr_in('0')
-        self.add_mtxr_in('1')
-        self.add_mtxr_in('/power/dut_trigger')
-        self.add_mtxr_in('/power/platform_trigger')
+        self.add_mtxr_in("z")
+        self.add_mtxr_in("0")
+        self.add_mtxr_in("1")
+        self.add_mtxr_in("/power/dut_trigger")
+        self.add_mtxr_in("/power/platform_trigger")
         for i in range(self.__UART_COUNT):
-            self.add_mtxr_in(f'/uart{i}/tx')
-            self.add_mtxr_in(f'/uart{i}/trigger')
-        self.add_mtxr_in('/iso7816/io_out')
-        self.add_mtxr_in('/iso7816/clk')
-        self.add_mtxr_in('/iso7816/trigger')
+            self.add_mtxr_in(f"/uart{i}/tx")
+            self.add_mtxr_in(f"/uart{i}/trigger")
+        self.add_mtxr_in("/iso7816/io_out")
+        self.add_mtxr_in("/iso7816/clk")
+        self.add_mtxr_in("/iso7816/trigger")
         for i in range(self.__PULSE_GENERATOR_COUNT):
-            self.add_mtxr_in(f'/pgen{i}/out')
+            self.add_mtxr_in(f"/pgen{i}/out")
         for i in range(self.__I2C_COUNT):
-            self.add_mtxr_in(f'/i2c{i}/sda_out')
-            self.add_mtxr_in(f'/i2c{i}/scl_out')
-            self.add_mtxr_in(f'/i2c{i}/trigger')
+            self.add_mtxr_in(f"/i2c{i}/sda_out")
+            self.add_mtxr_in(f"/i2c{i}/scl_out")
+            self.add_mtxr_in(f"/i2c{i}/trigger")
         for i in range(len(self.spis)):
-            self.add_mtxr_in(f'/spi{i}/sck')
-            self.add_mtxr_in(f'/spi{i}/mosi')
-            self.add_mtxr_in(f'/spi{i}/ss')
-            self.add_mtxr_in(f'/spi{i}/trigger')
+            self.add_mtxr_in(f"/spi{i}/sck")
+            self.add_mtxr_in(f"/spi{i}/mosi")
+            self.add_mtxr_in(f"/spi{i}/ss")
+            self.add_mtxr_in(f"/spi{i}/trigger")
         for i in range(len(self.spis)):
-            self.add_mtxr_in(f'/spi{i}/miso')
+            self.add_mtxr_in(f"/spi{i}/miso")
         for i in range(len(self.chains)):
-            self.add_mtxr_in(f'/chain{i}/trigger')
+            self.add_mtxr_in(f"/chain{i}/trigger")
         for i in range(len(self.clocks)):
-            self.add_mtxr_in(f'/clock{i}/out')
+            self.add_mtxr_in(f"/clock{i}/out")
 
         # FPGA right matrix output signals
-        self.add_mtxr_out('/io/a0')
-        self.add_mtxr_out('/io/a1')
-        if self.version <= '0.3':
+        self.add_mtxr_out("/io/a0")
+        self.add_mtxr_out("/io/a1")
+        if self.version <= "0.3":
             # Scaffold hardware v1 only
-            self.add_mtxr_out('/io/b0')
-            self.add_mtxr_out('/io/b1')
-            self.add_mtxr_out('/io/c0')
-            self.add_mtxr_out('/io/c1')
+            self.add_mtxr_out("/io/b0")
+            self.add_mtxr_out("/io/b1")
+            self.add_mtxr_out("/io/c0")
+            self.add_mtxr_out("/io/c1")
         else:
             # Scaffold hardware v1.1
-            self.add_mtxr_out('/io/a2')
-            self.add_mtxr_out('/io/a3')
+            self.add_mtxr_out("/io/a2")
+            self.add_mtxr_out("/io/a3")
         for i in range(self.__IO_D_COUNT):
-            self.add_mtxr_out(f'/io/d{i}')
-        if self.version >= '0.6':
+            self.add_mtxr_out(f"/io/d{i}")
+        if self.version >= "0.6":
             for i in range(self.__IO_P_COUNT):
-                self.add_mtxr_out(f'/io/p{i}')
+                self.add_mtxr_out(f"/io/p{i}")
 
         self.reset_config(init_ios=init_ios)
 
     def reset_config(self, init_ios=False):
         """
         Reset the board to a default state.
         :param init_ios: True to enable I/Os peripherals initialization. Doing
             so will set all I/Os to a default state, but it may generate pulses
             on the I/Os. When set to False, I/Os connections are unchanged
             during initialization and keep the configuration set by previous
             sessions.
         """
         # Reset to a default configuration
-        # This will perform many writes to registers, so we start a lazy
-        # section for maximum speed! (about 7 times faster)
-        with self.lazy_section():
-            self.timeout = None
-            # Sometime we don't want the I/Os to be changed, since it may
-            # generate pulses and triggering stuff... Reseting the I/Os is an
-            # option.
-            if init_ios:
-                self.sig_disconnect_all()
-                self.a0.reset_registers()
-                self.a1.reset_registers()
-                if self.version <= '0.3':
-                    # Scaffold hardware v1 only
-                    self.b0.reset_registers()
-                    self.b1.reset_registers()
-                    self.c0.reset_registers()
-                    self.c1.reset_registers()
-                else:
-                    # Scaffold hardware v1.1
-                    self.a2.reset_registers()
-                    self.a3.reset_registers()
-                for i in range(self.__IO_D_COUNT):
-                    self.__getattribute__(f'd{i}').reset_registers()
-                if self.version >= '0.6':
-                    for i in range(self.__IO_P_COUNT):
-                        self.__getattribute__(f'p{i}').reset_registers()
-            for uart in self.uarts:
-                uart.reset()
-            for pgen in self.pgens:
-                pgen.reset_registers()
-            self.leds.reset()
-            self.iso7816.reset_config()
-            for i2c in self.i2cs:
-                i2c.reset_config()
-            for spi in self.spis:
-                spi.reset_registers()
+        self.timeout = None
+        # Sometime we don't want the I/Os to be changed, since it may
+        # generate pulses and triggering stuff... Reseting the I/Os is an
+        # option.
+        if init_ios:
+            self.sig_disconnect_all()
+            self.a0.reset_registers()
+            self.a1.reset_registers()
+            if self.version <= "0.3":
+                # Scaffold hardware v1 only
+                self.b0.reset_registers()
+                self.b1.reset_registers()
+                self.c0.reset_registers()
+                self.c1.reset_registers()
+            else:
+                # Scaffold hardware v1.1
+                self.a2.reset_registers()
+                self.a3.reset_registers()
+            for i in range(self.__IO_D_COUNT):
+                self.__getattribute__(f"d{i}").reset_registers()
+            if self.version >= "0.6":
+                for i in range(self.__IO_P_COUNT):
+                    self.__getattribute__(f"p{i}").reset_registers()
+        for uart in self.uarts:
+            uart.reset()
+        for pgen in self.pgens:
+            pgen.reset_registers()
+        self.leds.reset()
+        self.iso7816.reset_config()
+        for i2c in self.i2cs:
+            i2c.reset_config()
+        for spi in self.spis:
+            spi.reset_registers()
```

### Comparing `donjon-scaffold-0.8.0/scaffold/iso7816.py` & `donjon-scaffold-0.9.0/scaffold/iso7816.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,55 +19,60 @@
 
 from enum import Enum
 from scaffold import Pull
 from typing import Tuple, List, Union, Optional
 from . import Scaffold
 import requests
 import crcmod
+from time import sleep
 
 
 class ProtocolError(Exception):
     """
     Exception raised when a protocol error between the terminal and the
     smartcard occurs.
     """
+
     def __init__(self, message):
         super().__init__(message)
 
 
 class Convention(Enum):
     """
     Possible ISO-7816 communication convention. This is given by the first byte
     of the ATR returned by the card.
     """
-    INVERSE = 0x3f
-    DIRECT = 0x3b
+
+    INVERSE = 0x3F
+    DIRECT = 0x3B
 
 
 class T1RedundancyCode(Enum):
     """
     Possible ISO78-16 possible error detection codes that can be used for T=1
     protocol. It is indicated in the first TC byte for T=1 of the ATR.
     """
+
     LRC = 0
     CRC = 1
 
 
 class T1RedundancyCodeError(Exception):
-    """ Thrown when the redundancy code of a received block is invalid. """
+    """Thrown when the redundancy code of a received block is invalid."""
+
     pass
 
 
 def inverse_byte(byte):
     """
     Inverse order and polarity of bits in a byte. Used for ISO-7816 inverse
     convention decoding.
     """
-    byte ^= 0xff
-    return int(f'{byte:08b}'[::-1], 2)
+    byte ^= 0xFF
+    return int(f"{byte:08b}"[::-1], 2)
 
 
 def apply_convention(data: bytes, convention: Convention) -> bytes:
     """
     :return: `data` if convention is `DIRECT`, `data` with all bytes inversed
         if convention is `INVERSE`.
     """
@@ -84,26 +89,28 @@
         self.atr = bytearray()
         self.convention = None
         self.protocols = set()
         self.t_abcd_n = []
 
 
 class ScaffoldISO7816ByteReader:
-    """ Used for `parse_atr` function with a Scaffold device. """
+    """Used for `parse_atr` function with a Scaffold device."""
+
     def __init__(self, iso7816):
-        """ :param iso7816: Scaffold ISO7816 module. """
+        """:param iso7816: Scaffold ISO7816 module."""
         self.iso7816 = iso7816
         self.convention = Convention.DIRECT
 
     def read(self, n: int) -> bytes:
         return apply_convention(self.iso7816.receive(n), self.convention)
 
 
 class BasicByteReader:
-    """ Used for `parse_atr` function with a test vector. """
+    """Used for `parse_atr` function with a test vector."""
+
     def __init__(self, data: bytes):
         self.data = data
 
     def read(self, n: int) -> bytes:
         if len(self.data) < n:
             raise EOFError()
         chunk = self.data[:n]
@@ -123,71 +130,71 @@
     atr = info.atr
     # Receive and parse TS
     atr.append(reader.read(1)[0])
     ts = atr[0]
     try:
         info.convention = Convention(ts)
     except ValueError as e:
-        raise ProtocolError(f'Invalid TS byte in ATR: 0x{ts:02x}') from e
+        raise ProtocolError(f"Invalid TS byte in ATR: 0x{ts:02x}") from e
     reader.convention = info.convention
     # Receive T0
     atr += reader.read(1)
     # Parse the rest of the ATR
     i = 1
     td = atr[i]
     while td is not None:
-        has_t_abcd = list(bool(td & (1 << (j+4))) for j in range(4))
+        has_t_abcd = list(bool(td & (1 << (j + 4))) for j in range(4))
         count = has_t_abcd.count(True)
         atr += reader.read(count)
         t_abcd = [None, None, None, None]
         offset = 0
         for j in range(4):
             if has_t_abcd[j]:
                 t_abcd[j] = atr[-count + offset]
                 offset += 1
         info.t_abcd_n.append(t_abcd)
         # Test to skip T0 byte
         if i != 1:
-            info.protocols.add(td & 0x0f)
+            info.protocols.add(td & 0x0F)
         # Test TD presence
         if has_t_abcd[3]:
             td = atr[-1]
         else:
             td = None
         i += 1
     # If no protocol is specified, then T=0 is available by default
     if len(info.protocols) == 0:
         info.protocols.add(0)
     # Fetch historical bytes
     # Number of historical bytes is the low nibble of T0
-    atr += reader.read(atr[1] & 0x0f)
+    atr += reader.read(atr[1] & 0x0F)
     # Parse TCK (check byte)
     # This byte is absent if only T=0 is supported
     if info.protocols != {0}:
         # TCK expected
         atr += reader.read(1)
         # tck = atr[-1]
         # Verify the checksum
         xored = 0x00
         for b in atr[1:]:
             xored ^= b
         if xored != 0x00:
-            raise ProtocolError('ATR checksum error')
+            raise ProtocolError("ATR checksum error")
     return info
 
 
 class NoATRDatabase(Exception):
     """
     Thrown during card information lookup if no ATR database could be loaded
     """
+
     pass
 
 
-def load_atr_info_db(allow_web_download: bool = False) \
-        -> List[Tuple[str, List[str]]]:
+def load_atr_info_db(allow_web_download: bool = False) -> List[Tuple[str, List[str]]]:
     """
     Parse the smartcard ATR list database from Ludovic Rousseau to get list of
     known ATR.
 
     The database file cannot be embedded in the library because it uses GPL
     and not LGPL license. On debian systems, this file is provided in the
     pcsc-tools package. If this file is missing and `allow_web_download` is
@@ -201,38 +208,40 @@
     :param allow_web_download: If enabled, allow the method to download the
         database from the web as a fallback when it is missing from the system.
     :raises NoATRDatabase: When database file is missing and download is not
         allowed, or when database file is missing and download failed.
     """
     tab = []
     try:
-        text_file = open('/usr/share/pcsc/smartcard_list.txt', 'r')
+        text_file = open("/usr/share/pcsc/smartcard_list.txt", "r")
         # We don't want to keep end lines such as LR or CR LF
         lines = text_file.read().splitlines()
         text_file.close()
     except FileNotFoundError:
         if allow_web_download:
-            url = "http://ludovic.rousseau.free.fr/softwares/pcsc-tools/" \
+            url = (
+                "http://ludovic.rousseau.free.fr/softwares/pcsc-tools/"
                 + "smartcard_list.txt"
+            )
             try:
                 res = requests.get(url)
             except Exception:
                 raise NoATRDatabase()
             if res.status_code != 200:
                 raise NoATRDatabase()
             lines = res.content.decode().splitlines()
         else:
             raise NoATRDatabase()
     # Parse the file and build a table with ATR patterns and infos
     for line in lines:
-        if (len(line) > 0) and (line[0] not in ('#', '\t')):
+        if (len(line) > 0) and (line[0] not in ("#", "\t")):
             # ATR line
-            atr = line.replace(' ', '').lower()
+            atr = line.replace(" ", "").lower()
             tab.append((atr, []))
-        elif (len(line) > 0) and (line[0] == '\t'):
+        elif (len(line) > 0) and (line[0] == "\t"):
             # Info line
             # Remove first character \t
             tab[-1][1].append(line[1:])
     return tab
 
 
 class Smartcard:
@@ -251,14 +260,15 @@
 
     :var bytes atr: ATR received from card after reset.
     :var Convention convention: Communication convention between card
         and terminal. Updated when first byte TS of ATR is received.
     :var set protocols: Communication protocols found in ATR. This set contains
         integers, for instance 0 if T=0 is supported, 1 if T=1 is supported...
     """
+
     def __init__(self, scaffold: Scaffold = None):
         """
         Configure a Scaffold board for use with smartcards.
 
         :param scaffold: Board instance which will be configured as a smartcard
             reader. :class:`scaffold.Scaffold` instance.
         """
@@ -307,14 +317,15 @@
         If only T=1 is supported, exchanges using :meth:`apdu` will use I-block
         transmission automatically.
 
         :return: ATR from the card.
         :raises ProtocolError: if the ATR is not valid.
         """
         self.sig_nrst << 0
+        sleep(0.05)
         self.iso7816.flush()
         self.sig_nrst << 1
         info = parse_atr(ScaffoldISO7816ByteReader(self.iso7816))
         self.atr = info.atr
         self.convention = info.convention
         self.protocols = info.protocols
         self.atr_info = info
@@ -328,18 +339,18 @@
                 self.t1_redundancy_code = T1RedundancyCode(tc1 & 1)
             else:
                 self.t1_redundancy_code = T1RedundancyCode.LRC
         else:
             self.t1_redundancy_code = None
         # Verify that there are no more bytes
         if not self.iso7816.empty:
-            raise ProtocolError('Unexpected bytes after ATR')
+            raise ProtocolError("Unexpected bytes after ATR")
         return info.atr
 
-    def apdu(self, the_apdu: Union[bytes, str], trigger: str = '') -> bytes:
+    def apdu(self, the_apdu: Union[bytes, str], trigger: str = "") -> bytes:
         """
         Send an APDU to the smartcard and retrieve the response.
 
         If only T=1 protocol is supported, this method use `transmit_block` and
         `receive_block` to send the APDU by sending information blocks.
 
         :param the_apdu: APDU to be sent. str hexadecimal strings are allowed,
@@ -357,24 +368,23 @@
         :raises T1RedundancyCodeError: If LRC or CRC is wrong in T=1 protocol.
         :return: Response data, with status word.
         """
         if type(the_apdu) is str:
             the_apdu = bytes.fromhex(the_apdu)
         apdu_len = len(the_apdu)
         if apdu_len < 5:
-            raise ValueError('APDU too short')
+            raise ValueError("APDU too short")
         if 0 in self.protocols:
             return self.__apdu_t0(the_apdu, trigger)
         elif 1 in self.protocols:
-            return self.__apdu_t1(
-                the_apdu, ('a' in trigger) or ('b' in trigger))
+            return self.__apdu_t1(the_apdu, ("a" in trigger) or ("b" in trigger))
         else:
             raise RuntimeError("Neither T=0 or T=1 are supported by the card")
 
-    def __apdu_t0(self, the_apdu: bytes, trigger: str = '') -> bytes:
+    def __apdu_t0(self, the_apdu: bytes, trigger: str = "") -> bytes:
         """
         Send an APDU to the smartcard and retrieve the response, using T=0
         protocol.
 
         :param the_apdu: APDU to be sent.
         :param trigger: If 'a' is in this string, trigger is raised after
             ISO-7816 header is sent, and cleared when the following response
@@ -383,75 +393,75 @@
             response byte is received.
         :raises ValueError: if APDU data is invalid.
         :raises RuntimeError: if the received procedure byte is invalid.
         :return: Response data, with status word.
         """
         out_data_len = len(the_apdu) - 5
         if out_data_len > 256:
-            raise ValueError('APDU too long')
+            raise ValueError("APDU too long")
         if out_data_len > 0:
             # This is an outgoing data transfer
             # Verify APDU P3 field correctness
             p3 = the_apdu[4]
             expected_p3 = out_data_len % 256
             if p3 != expected_p3:
                 raise ValueError(
-                    'Expected P3 (length) in APDU is '
-                    f'0x{expected_p3:02x}, got 0x{p3:02x}')
+                    "Expected P3 (length) in APDU is "
+                    f"0x{expected_p3:02x}, got 0x{p3:02x}"
+                )
             in_data_len = 0
         else:
             if the_apdu[4] > 0:
                 in_data_len = the_apdu[4]
             else:
                 in_data_len = 256
         # Transmit the header
-        if 'a' in trigger:
-            with self.scaffold.lazy_section():
-                self.iso7816.transmit(the_apdu[:4])
-                self.iso7816.trigger_long = 1
-                self.iso7816.transmit(the_apdu[4:5])
+        if "a" in trigger:
+            self.iso7816.transmit(the_apdu[:4])
+            self.iso7816.trigger_long = 1
+            self.iso7816.transmit(the_apdu[4:5])
         else:
             # Send all the header at once
-            with self.scaffold.lazy_section():
-                self.iso7816.trigger_long = 0
-                self.iso7816.transmit(the_apdu[:5])
+            self.iso7816.trigger_long = 0
+            self.iso7816.transmit(the_apdu[:5])
         # Receive procedure byte
         procedure_byte = self.iso7816.receive(1)[0]
-        if 'a' in trigger:  # Disable only if enabled previously
+        if "a" in trigger:  # Disable only if enabled previously
             self.iso7816.trigger_long = 0
         while procedure_byte == 0x60:
             procedure_byte = self.iso7816.receive(1)[0]
         response = bytearray()
         ins = the_apdu[1]
-        if (procedure_byte & 0xf0) in (0x60, 0x90):
+        if (procedure_byte & 0xF0) in (0x60, 0x90):
             # Received SW1 byte.
             response.append(procedure_byte)
             # Received SW2
             response.append(self.iso7816.receive(1)[0])
             return response
         elif procedure_byte in (ins, ~ins):
             # Acknowledge byte.
             # Transfer the remaining data
             if out_data_len > 0:
-                if 'b' in trigger:
+                if "b" in trigger:
                     # Enable trigger on last byte only
                     self.iso7816.transmit(the_apdu[5:-1])
                     self.iso7816.trigger_long = 1
                     self.iso7816.transmit(the_apdu[-1:])
                 else:
                     # Send all remaining data at once
                     self.iso7816.transmit(the_apdu[5:])
             # Receive the response data and status word
             response += self.iso7816.receive(in_data_len + 2)
-            if 'b' in trigger:  # Disable only if enabled previously
+            if "b" in trigger:  # Disable only if enabled previously
                 self.iso7816.trigger_long = 0
             return response
         else:
             raise RuntimeError(
-                f'Unexpected procedure byte 0x{procedure_byte:02x} received')
+                f"Unexpected procedure byte 0x{procedure_byte:02x} received"
+            )
 
     def __apdu_t1(self, the_apdu: bytes, trigger: bool = False) -> bytes:
         """
         Send an APDU to the smartcard and retrieve the response, using T=1
         protocol. Transmission supports chaining for both command and response.
 
         :param the_apdu: APDU to be sent.
@@ -467,61 +477,59 @@
         while len(apdu_remaining):
             chunk = apdu_remaining[:254]
             apdu_remaining = apdu_remaining[254:]
             has_more = min(1, len(apdu_remaining))
             enable_trigger = trigger and not has_more
             # Send I-block
             self.transmit_block(
-                0, (self.t1_ns_tx << 6) + (has_more << 5), chunk,
-                enable_trigger)
+                0, (self.t1_ns_tx << 6) + (has_more << 5), chunk, enable_trigger
+            )
             # Increment sequence number
             self.t1_ns_tx = (self.t1_ns_tx + 1) % 2
             if has_more:
                 # We expect a R-block before sending the next info block
                 block = self.receive_block()
                 pcb = block[1]
                 if pcb & (1 << 7) == 0:  # I-block
-                    raise ProtocolError('Expected R-block, received I-block')
+                    raise ProtocolError("Expected R-block, received I-block")
                 elif pcb & (1 << 6) == 0:  # R-block
-                    if pcb & 0x0f == 0:  # Error free acknowledgement
+                    if pcb & 0x0F == 0:  # Error free acknowledgement
                         pass
-                    elif pcb & 0x0f == 1:
-                        raise ProtocolError(
-                            'Redundancy code error reported by card')
+                    elif pcb & 0x0F == 1:
+                        raise ProtocolError("Redundancy code error reported by card")
                     else:
-                        raise ProtocolError(
-                            'Unspecified error reported by card')
+                        raise ProtocolError("Unspecified error reported by card")
                 else:  # S-block
-                    raise ProtocolError('Expected R-block, received I-block')
+                    raise ProtocolError("Expected R-block, received I-block")
 
         response = bytearray()
         has_more = True
         while has_more:
             block = self.receive_block()
             if enable_trigger:
                 self.iso7816.trigger_long = 0
             pcb = block[1]
             if pcb & (1 << 7) == 0:  # I-block
                 # Check that the sequence number is correct
                 if (pcb >> 6) & 1 != self.t1_ns_rx:
                     raise ProtocolError(
-                        'Incorrect received sequence number in I-block '
-                        + block.hex())
+                        "Incorrect received sequence number in I-block " + block.hex()
+                    )
                 has_more = bool((pcb >> 5) & 1)
                 edc_len = edc_len_dict[self.t1_redundancy_code]
                 response += block[3:-edc_len]  # Trim header and EDC
             elif pcb & (1 << 6) == 0:  # R-block
-                raise ProtocolError('Expected I-block, received R-block')
+                raise ProtocolError("Expected I-block, received R-block")
             else:  # S-block
-                raise ProtocolError('Expected I-block, received S-block')
+                raise ProtocolError("Expected I-block, received S-block")
 
             self.t1_ns_rx = (self.t1_ns_rx + 1) % 2
             if has_more:
                 # Send R block
-                self.transmit_block(0, 0b10000000 + (self.t1_ns_rx << 4), b'')
+                self.transmit_block(0, 0b10000000 + (self.t1_ns_rx << 4), b"")
 
         return response
 
     def pps(self, pps1: int) -> int:
         """
         Send a PPS request to change the communication speed parameters Fi and
         Di (as specified in ISO-7816-3). PPS0 and PPS1 are sent. PPS2 is
@@ -533,50 +541,67 @@
         :param pps1: Value of the PPS1 byte.
         :return: New etu value.
         :raises ValueError: if Fi or Di parameters in PPS1 are reserved.
         :raises ValueError: if target ETU has a fractional part.
         :raises RuntimeError: if response to PPS request is invalid.
         """
         if pps1 not in range(0x100):
-            raise ValueError('Invalid PPS1 value')
-        fi = ([372, 372, 558, 744, 1116, 1488, 1860, None, None, 512, 768,
-               1024, 1536, 2048, None, None][pps1 >> 4])
+            raise ValueError("Invalid PPS1 value")
+        fi = [
+            372,
+            372,
+            558,
+            744,
+            1116,
+            1488,
+            1860,
+            None,
+            None,
+            512,
+            768,
+            1024,
+            1536,
+            2048,
+            None,
+            None,
+        ][pps1 >> 4]
         if fi is None:
-            raise ValueError('Fi parameter in PPS1 has a reserved value')
-        di = ([None, 1, 2, 4, 8, 16, 32, 64, 12, 20, None, None, None, None,
-               None, None][pps1 & 0x0f])
+            raise ValueError("Fi parameter in PPS1 has a reserved value")
+        di = [None, 1, 2, 4, 8, 16, 32, 64, 12, 20, None, None, None, None, None, None][
+            pps1 & 0x0F
+        ]
         if di is None:
-            raise ValueError('Di parameter in PPS1 has a reserved value')
+            raise ValueError("Di parameter in PPS1 has a reserved value")
         # PPSS = 0xff
         # PPS0 = 0x10 to indicate presence of PPS1
-        request = bytearray(b'\xff\x10')
+        request = bytearray(b"\xff\x10")
         request.append(pps1)
         etu = round(fi / di)
         if etu != fi / di:
             raise ValueError(
-                f'Cannot set ETU to {etu} because of the '
-                'fractional part (hardware limitation)')
+                f"Cannot set ETU to {etu} because of the "
+                "fractional part (hardware limitation)"
+            )
         # Checksum
         pck = 0
         for b in request:
             pck ^= b
         request.append(pck)
         # Send the request
         self.iso7816.transmit(request)
         # Get the response
         res = self.iso7816.receive(4, timeout=1)
         if res == request:
             # Negociation is successfull
             self.iso7816.etu = etu
             return etu
         else:
-            raise RuntimeError('PPS request failed')
+            raise RuntimeError("PPS request failed")
 
-    def find_info(self, allow_web_download: bool = False) \
-            -> Optional[List[str]]:
+    def find_info(self, allow_web_download: bool = False) -> Optional[List[str]]:
         """
         Parse the smartcard ATR list database available at
         http://ludovic.rousseau.free.fr/softwares/pcsc-tools/smartcard_list.txt
         and try to match the current ATR to retrieve more info about the card.
 
         The database file cannot be embedded in the library because it uses GPL
         and not LGPL license. On debian systems, this file is provided in the
@@ -596,15 +621,15 @@
         for item in tab:
             pattern = item[0]
             atr = self.atr.hex()
             if len(pattern) != len(atr):
                 continue
             match = True
             for i in range(len(pattern)):
-                if pattern[i] != '.':
+                if pattern[i] != ".":
                     if pattern[i] != atr[i]:
                         match = False
                         break
             if match:
                 return item[1]
                 break
 
@@ -634,43 +659,42 @@
                 result = result ^ b
             return bytes([result])
         elif self.t1_redundancy_code == T1RedundancyCode.CRC:
             # CRC is CRC-16-CCITT, with initial value 0xffff
             # I cannot tell if this is correct as it does not seem very well
             # documented and I don't have any card to test this...
             if self.crc16 is None:
-                self.crc16 = crcmod.mkCrcFun(0x11021, 0xffff, rev=False)
-            return self.crc16(data).to_bytes(2, 'big')
+                self.crc16 = crcmod.mkCrcFun(0x11021, 0xFFFF, rev=False)
+            return self.crc16(data).to_bytes(2, "big")
         else:
             raise RuntimeError("invalid t1_redundancy_code value")
 
-    def transmit_block(self, nad: int, pcb: int, info: bytes = b"",
-                       trigger: bool = False):
+    def transmit_block(
+        self, nad: int, pcb: int, info: bytes = b"", trigger: bool = False
+    ):
         """
         Transmit a T=1 protocol block.
         Error detection code is calculated and appended automatically.
 
         :param nad: Node address byte.
         :param pcb: Protocol control byte.
         :param info: Information field.
         :param trigger: If True, raise trigger on last byte transmission.
         """
         if len(info) > 254:
-            raise ValueError(
-                f"info field is too long ({len(info)} > 254)")
+            raise ValueError(f"info field is too long ({len(info)} > 254)")
         data = bytearray([nad, pcb, len(info)]) + info
         data += self.calculate_edc(data)
-        with self.scaffold.lazy_section():
-            if trigger:
-                self.iso7816.transmit(data[:-1])
-                self.iso7816.trigger_long = 1
-                self.iso7816.transmit(data[-1:])
-            else:
-                self.iso7816.trigger_long = 0
-                self.iso7816.transmit(data)
+        if trigger:
+            self.iso7816.transmit(data[:-1])
+            self.iso7816.trigger_long = 1
+            self.iso7816.transmit(data[-1:])
+        else:
+            self.iso7816.trigger_long = 0
+            self.iso7816.transmit(data)
 
     def receive_block(self) -> bytes:
         """
         Receive a T=1 protocol block.
 
         :raises T1RedundancyCodeError: If LRC or CRC is wrong.
         """
```

### Comparing `donjon-scaffold-0.8.0/scaffold/stm32.py` & `donjon-scaffold-0.9.0/scaffold/stm32.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,40 +22,43 @@
 
 
 class NACKError(Exception):
     """
     This error is thrown when a STM32 devices responds with NACK byte to a
     command.
     """
+
     def __init__(self, tag=None):
-        super().__init__('Device returned NACK to a command')
+        super().__init__("Device returned NACK to a command")
         self.tag = tag
 
 
 class MemorySection:
-    """ Describes a memory section of a device. """
+    """Describes a memory section of a device."""
+
     def __init__(self, start, end):
         """
         :param start: First address of the section.
         :param end: End address of the section (excluded from section, address
             of next section).
         """
         if end < start:
-            raise ValueError('Invalid section addresses')
+            raise ValueError("Invalid section addresses")
         self.start = start
         self.end = end
 
     @property
     def size(self):
-        """ Size in bytes of the section. """
+        """Size in bytes of the section."""
         return self.end - self.start
 
 
 class STM32Device:
-    """ Possible name and product ID tuple. """
+    """Possible name and product ID tuple."""
+
     def __init__(self, name, pid, memory_mapping, offset_rdp=0):
         self.name = name
         self.pid = pid
         self.memory_mapping = memory_mapping
         self.offset_rdp = offset_rdp
 
 
@@ -76,60 +79,64 @@
     This class can communicate with the ST bootloader via USART1. This allows
     programming the Flash memory and then execute the loaded code.
     """
 
     # Acknoledge byte returned by STM32 bootloader.
     ACK = 0x79
     # Error byte returned by STM32 bootloader.
-    NACK = 0x1f
+    NACK = 0x1F
 
     # Memory layout for STM32F20xxx
     map_f20xxx = {
-        'option_bytes': MemorySection(0x1fffc000, 0x1fffc008),
-        'system': MemorySection(0x1fff0000, 0x1fff7a10),
-        'flash': MemorySection(0x08000000, 0x08100000)}
+        "option_bytes": MemorySection(0x1FFFC000, 0x1FFFC008),
+        "system": MemorySection(0x1FFF0000, 0x1FFF7A10),
+        "flash": MemorySection(0x08000000, 0x08100000),
+    }
 
     # Memory layout for STM32F100xx written by Hugo LE GUEN, intern at IETR
     map_f100xx = {
-        'option_bytes': MemorySection(0x1ffff800, 0x1ffff80f),
-        'system': MemorySection(0x1ffff000, 0x1ffff7ff),
-        'flash': MemorySection(0x08000000, 0x0801ffff)}
+        "option_bytes": MemorySection(0x1FFFF800, 0x1FFFF80F),
+        "system": MemorySection(0x1FFFF000, 0x1FFFF7FF),
+        "flash": MemorySection(0x08000000, 0x0801FFFF),
+    }
 
     # Memory layout for STM32F4xxx
     map_f40xxx = map_f20xxx
 
     # Memory layout for STM32L431xx
     map_l431xx = {
-        'option_bytes': MemorySection(0x1fff7800, 0x1fff7810),
-        'otp': MemorySection(0x1fff7000, 0x1fff7400),
-        'system': MemorySection(0x1fff0000, 0x1fff7000),
-        'flash': MemorySection(0x08000000, 0x08040000)}
+        "option_bytes": MemorySection(0x1FFF7800, 0x1FFF7810),
+        "otp": MemorySection(0x1FFF7000, 0x1FFF7400),
+        "system": MemorySection(0x1FFF0000, 0x1FFF7000),
+        "flash": MemorySection(0x08000000, 0x08040000),
+    }
 
     # Memory layout for STM32U5A9
     map_u5 = {
-        'otp': MemorySection(0x0bfa0000, 0x0bfa0200),
-        'system': MemorySection(0x0bf90000, 0x0bf98000),
-        'flash': MemorySection(0x08000000, 0x08080000)
+        "otp": MemorySection(0x0BFA0000, 0x0BFA0200),
+        "system": MemorySection(0x0BF90000, 0x0BF98000),
+        "flash": MemorySection(0x08000000, 0x08080000),
     }
 
     # See AN2606 for PID values
     PIDS = [
-        STM32Device('STM32F05xxx', 0x440, {}),
-        STM32Device('STM32F030x8', 0x440, {}),
-        STM32Device('STM32F03xx4/6', 0x444, {}),
-        STM32Device('STM32F100xx', 0x420, map_f100xx),
-        STM32Device('STM32F2xxxx', 0x411, map_f20xxx, offset_rdp=1),
-        STM32Device('STM32F40xxx/41xxx', 0x413, map_f40xxx, offset_rdp=1),
-        STM32Device('STM32F42xxx/43xxx', 0x419, map_f40xxx, offset_rdp=1),
-        STM32Device('STM32L43xxx/44xxx', 0x435, map_l431xx),
-        STM32Device('STM32L45xxx/46xxx', 0x462, {}),
-        STM32Device('STM32L47xxx/48xxx', 0x415, {}),
-        STM32Device('STM32L496xx/4A6xx', 0x461, {}),
-        STM32Device('STM32L4Rxx/4Sxx', 0x470, {}),
-        STM32Device('STM32U59x/5Ax', 0x481, map_u5)]
+        STM32Device("STM32F05xxx", 0x440, {}),
+        STM32Device("STM32F030x8", 0x440, {}),
+        STM32Device("STM32F03xx4/6", 0x444, {}),
+        STM32Device("STM32F100xx", 0x420, map_f100xx),
+        STM32Device("STM32F2xxxx", 0x411, map_f20xxx, offset_rdp=1),
+        STM32Device("STM32F40xxx/41xxx", 0x413, map_f40xxx, offset_rdp=1),
+        STM32Device("STM32F42xxx/43xxx", 0x419, map_f40xxx, offset_rdp=1),
+        STM32Device("STM32L43xxx/44xxx", 0x435, map_l431xx),
+        STM32Device("STM32L45xxx/46xxx", 0x462, {}),
+        STM32Device("STM32L47xxx/48xxx", 0x415, {}),
+        STM32Device("STM32L496xx/4A6xx", 0x461, {}),
+        STM32Device("STM32L4Rxx/4Sxx", 0x470, {}),
+        STM32Device("STM32U59x/5Ax", 0x481, map_u5),
+    ]
 
     def __init__(self, scaffold):
         """
         :param scaffold: An instance of :class:`scaffold.Scaffold` which will
             be configured and used to communicate with STM32 daughter board.
         """
         self.scaffold = scaffold
@@ -173,15 +180,15 @@
         sleep(0.1)
         self.scaffold.power.dut = 1
         sleep(0.1)
         self.nrst << 1
         sleep(0.1)
         # Send 0x7f byte for initiating communication
         self.uart.flush()
-        self.uart.transmit(b'\x7f')
+        self.uart.transmit(b"\x7f")
         self.wait_ack()
 
     def startup_flash(self):
         """
         Power-cycle and reset target device and boot from user Flash memory.
         """
         self.scaffold.power.dut = 0
@@ -197,33 +204,33 @@
     def command(self, index):
         """
         Send a command and return the response.
 
         :param index: Command index.
         :return: Response bytes.
         """
-        self.uart.transmit(bytes([index, 0xff ^ index]))
+        self.uart.transmit(bytes([index, 0xFF ^ index]))
         res = self.uart.receive(2)
         assert res[0] == self.ACK
-        data = self.uart.receive(res[1]+2)
+        data = self.uart.receive(res[1] + 2)
         assert data[-1] == self.ACK
         return data[0:-1]
 
     def wait_ack(self, tag=None):
         """
         Wait for ACK byte.
 
         :param tag: Tag which is set when NACKError are thrown. Useful for
             error diagnostic.
         """
         b = self.uart.receive(1)[0]
         if b == self.NACK:
             raise NACKError(tag)
         if b != self.ACK:
-            raise Exception(f'Received 0x{b:02x} byte instead of ACK or NACK.')
+            raise Exception(f"Received 0x{b:02x} byte instead of ACK or NACK.")
 
     def wait_ack_or_nack(self):
         """
         Wait for ACK or NACK byte.
 
         :return: True if ACK has been received, False if NACK has been
             received.
@@ -243,22 +250,22 @@
     def get_id(self):
         """
         Execute the Get ID command. The result is interpreted and the class
         will try to find information if the ID matches a known device.
         """
         self.device = None
         response = self.command(0x02)
-        pid = int.from_bytes(response, 'big', signed=False)
+        pid = int.from_bytes(response, "big", signed=False)
         for dev in self.PIDS:
             if dev.pid == pid:
                 self.device = dev
         return pid
 
     def get_version_and_read_protection_status(self):
-        self.uart.transmit(b'\x01\xfe')
+        self.uart.transmit(b"\x01\xfe")
         response = self.uart.receive(5)
         assert response[0] == self.ACK
         assert response[-1] == self.ACK
         return response[1:-1]
 
     def read_memory(self, address, length, trigger=0):
         """
@@ -269,23 +276,23 @@
         :param size: Number of bytes to be read.
         :param trigger: 1 to enable trigger on command transmission.
         """
         result = bytearray()
         remaining = length
         while remaining > 0:
             chunk_size = min(256, remaining)
-            self.uart.transmit(b'\x11\xee', trigger=trigger)
+            self.uart.transmit(b"\x11\xee", trigger=trigger)
             self.wait_ack()
-            buf = bytearray(address.to_bytes(4, 'big', signed=False))
+            buf = bytearray(address.to_bytes(4, "big", signed=False))
             buf.append(self.checksum(buf))
             self.uart.transmit(buf)
             self.wait_ack()
             buf = bytearray()
-            buf.append(chunk_size-1)
-            buf.append((chunk_size-1) ^ 0xff)
+            buf.append(chunk_size - 1)
+            buf.append((chunk_size - 1) ^ 0xFF)
             self.uart.transmit(buf)
             self.wait_ack()
             result += self.uart.receive(chunk_size)
             remaining -= chunk_size
             address += chunk_size
         return result
 
@@ -299,62 +306,62 @@
         :param data: Data to be written. bytes or bytearray.
         :param trigger: 1 to enable trigger on each command transmission.
         """
         remaining = len(data)
         offset = 0
         while remaining > 0:
             chunk_size = min(256, remaining)
-            self.uart.transmit(b'\x31\xce', trigger=trigger)
+            self.uart.transmit(b"\x31\xce", trigger=trigger)
             self.wait_ack(0)
-            buf = bytearray(
-                (address + offset).to_bytes(4, 'big', signed=False))
+            buf = bytearray((address + offset).to_bytes(4, "big", signed=False))
             buf.append(self.checksum(buf))
             self.uart.transmit(buf)
             self.wait_ack(1)
             buf = bytearray()
             buf.append(chunk_size - 1)
-            buf += data[offset:offset + chunk_size]
+            buf += data[offset : offset + chunk_size]
             buf.append(self.checksum(buf))
             self.uart.transmit(buf)
             self.wait_ack(2)
             offset += chunk_size
             remaining -= chunk_size
 
     def assert_device(self):
-        """ Raise a RuntimeError is device is unknown (None). """
+        """Raise a RuntimeError is device is unknown (None)."""
         if self.device is None:
             raise RuntimeError(
-                'Unknown device or not discovered yet. Call get_id or set the '
-                'device attribute.')
+                "Unknown device or not discovered yet. Call get_id or set the "
+                "device attribute."
+            )
 
     def read_option_bytes(self):
         """
         Read the option bytes of the device. The method get_id must have been
         called previously for device identification.
 
         :return: Memory content of 'option_bytes' section.
         """
         self.assert_device()  # We need the memory mapping
-        section = self.device.memory_mapping['option_bytes']
+        section = self.device.memory_mapping["option_bytes"]
         return self.read_memory(section.start, section.size)
 
     def readout_protect(self):
         """
         Execute the Readout Unprotect command.
         """
-        self.uart.transmit(b'\x82\x7d', 1)
+        self.uart.transmit(b"\x82\x7d", 1)
         self.wait_ack()
         self.wait_ack()
 
     def readout_unprotect(self):
         """
         Execute the Readout Unprotect command. If the device is locked, it will
         perform mass flash erase, which can be very very long.
         """
-        self.uart.transmit(b'\x92\x6d', 1)
+        self.uart.transmit(b"\x92\x6d", 1)
         self.wait_ack()
         # When the chip is in RDP1 it will perform mass flash erase. This can
         # take a lot of time, so we must change the timeout setting.
         previous_timeout = self.scaffold.timeout
         self.scaffold.timeout = 30
         try:
             self.wait_ack()
@@ -366,39 +373,39 @@
         """
         Execute Write Protect command.
 
         :param sectors: List of sectors to be write protected.
         """
         if len(sectors) not in range(1, 0x100):
             raise ValueError("Invalid sector count")
-        self.uart.transmit(b'\x63\x9c')
+        self.uart.transmit(b"\x63\x9c")
         self.wait_ack()
         buf = bytearray()
-        buf.append(len(sectors)-1)
+        buf.append(len(sectors) - 1)
         buf += bytes(sectors)
         buf.append(self.checksum(buf))
         self.uart.transmit(buf)
         self.wait_ack()
 
     def write_unprotect(self):
         """
         Execute Write Unprotect command.
         """
-        self.uart.transmit(b'\x73\x8c')
+        self.uart.transmit(b"\x73\x8c")
         self.wait_ack()
         self.wait_ack()
 
     def extended_erase(self):
         """
         Execute the Extended Erase command to erase all the Flash memory of the
         device.
         """
-        self.uart.transmit(b'\x44\xbb')
+        self.uart.transmit(b"\x44\xbb")
         self.wait_ack()
-        buf = bytearray(b'\xff\xff')
+        buf = bytearray(b"\xff\xff")
         buf.append(self.checksum(buf))
         self.uart.transmit(buf, 1)
         previous_timeout = self.scaffold.timeout
         self.scaffold.timeout = 30
         try:
             self.wait_ack()
         finally:
@@ -411,26 +418,26 @@
         Unlike a chip that has a bootloader version higher or equal to 3.0,
         the command to erase the Flash memory is x43/xbc instead of x44/xbb.
         The function is based on the translation of the diagram in the
         documentation "USART protocol used in the STM32" in
         the category "Erase Memory command: host side".
         Written by Hugo LE GUEN, intern at IETR.
         """
-        self.uart.transmit(b'\x43\xbc')
+        self.uart.transmit(b"\x43\xbc")
         self.wait_ack()
-        self.uart.transmit(b'\xff')
-        self.uart.transmit(b'\x00')
+        self.uart.transmit(b"\xff")
+        self.uart.transmit(b"\x00")
         self.wait_ack()
 
     def go(self, address, trigger=0):
         """
         Execute the Go command.
 
         :param address: Jump address.
         :param trigger: 1 to enable trigger on command transmission.
         """
-        self.uart.transmit(b'\x21\xde', trigger=trigger)
+        self.uart.transmit(b"\x21\xde", trigger=trigger)
         self.wait_ack()
-        buf = bytearray(address.to_bytes(4, 'big', signed=False))
+        buf = bytearray(address.to_bytes(4, "big", signed=False))
         buf.append(self.checksum(buf))
         self.uart.transmit(buf)
         self.wait_ack()
```

### Comparing `donjon-scaffold-0.8.0/setup.py` & `donjon-scaffold-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="donjon-scaffold",
-    version="0.8.0",
+    version="0.9.0",
     author="Olivier Heriveaux",
     description="Python3 API for the Scaffold board",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ledger-Donjon/scaffold",
     install_requires=["pyserial", "crcmod", "requests"],
     packages=find_packages(),
-    python_requires=">=3.6")
+    python_requires=">=3.6",
+)
```
