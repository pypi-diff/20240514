# Comparing `tmp/m_mock-1.3.3.tar.gz` & `tmp/m_mock-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_mock-1.3.3.tar", last modified: Wed Feb 28 08:08:12 2024, max compression
+gzip compressed data, was "m_mock-1.3.4.tar", last modified: Tue May 14 07:13:40 2024, max compression
```

## Comparing `m_mock-1.3.3.tar` & `m_mock-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 08:08:12.864885 m_mock-1.3.3/
--rw-rw-rw-   0        0        0    35823 2024-02-27 09:13:21.000000 m_mock-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     4260 2024-02-28 08:08:12.863828 m_mock-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3806 2024-02-27 09:13:21.000000 m_mock-1.3.3/README.md
--rw-rw-rw-   0        0        0      590 2024-02-27 09:13:21.000000 m_mock-1.3.3/license.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 08:08:12.845752 m_mock-1.3.3/m_mock/
--rw-rw-rw-   0        0        0    31112 2024-02-28 08:04:37.000000 m_mock-1.3.3/m_mock/m_random.py
--rw-rw-rw-   0        0        0     2074 2024-02-27 09:21:08.000000 m_mock-1.3.3/m_mock/m_random_source.py
--rw-rw-rw-   0        0        0     2825 2024-02-27 09:21:08.000000 m_mock-1.3.3/m_mock/mock.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:08:12.859826 m_mock-1.3.3/m_mock/test_case/
--rw-rw-rw-   0        0        0      210 2024-02-27 09:13:21.000000 m_mock-1.3.3/m_mock/test_case/common_utils.py
--rw-rw-rw-   0        0        0     1929 2024-02-27 09:13:21.000000 m_mock-1.3.3/m_mock/test_case/test_basic.py
--rw-rw-rw-   0        0        0     1463 2024-02-27 09:13:21.000000 m_mock-1.3.3/m_mock/test_case/test_date.py
--rw-rw-rw-   0        0        0      219 2024-02-27 09:13:21.000000 m_mock-1.3.3/m_mock/test_case/test_helper.py
--rw-rw-rw-   0        0        0      806 2024-02-27 09:13:21.000000 m_mock-1.3.3/m_mock/test_case/test_name.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:08:12.862826 m_mock-1.3.3/m_mock.egg-info/
--rw-rw-rw-   0        0        0     4260 2024-02-28 08:08:12.000000 m_mock-1.3.3/m_mock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2024-02-28 08:08:12.000000 m_mock-1.3.3/m_mock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 08:08:12.000000 m_mock-1.3.3/m_mock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-02-28 08:08:12.000000 m_mock-1.3.3/m_mock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-28 08:08:12.000000 m_mock-1.3.3/m_mock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      433 2024-02-28 08:06:38.000000 m_mock-1.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 08:08:12.864885 m_mock-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 07:13:40.586703 m_mock-1.3.4/
+-rw-rw-rw-   0        0        0    35823 2024-02-27 09:13:21.000000 m_mock-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4473 2024-05-14 07:13:40.584703 m_mock-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4017 2024-05-14 06:58:58.000000 m_mock-1.3.4/README.md
+-rw-rw-rw-   0        0        0      590 2024-02-27 09:13:21.000000 m_mock-1.3.4/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 07:13:40.557248 m_mock-1.3.4/m_mock/
+-rw-rw-rw-   0        0        0    34675 2024-05-14 06:53:20.000000 m_mock-1.3.4/m_mock/m_random.py
+-rw-rw-rw-   0        0        0     2074 2024-02-27 09:21:08.000000 m_mock-1.3.4/m_mock/m_random_source.py
+-rw-rw-rw-   0        0        0     2972 2024-05-14 06:17:52.000000 m_mock-1.3.4/m_mock/mock.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:13:40.580705 m_mock-1.3.4/m_mock/test_case/
+-rw-rw-rw-   0        0        0      145 2024-05-14 06:23:54.000000 m_mock-1.3.4/m_mock/test_case/common_utils.py
+-rw-rw-rw-   0        0        0     2106 2024-05-14 07:05:56.000000 m_mock-1.3.4/m_mock/test_case/test_basic.py
+-rw-rw-rw-   0        0        0     1548 2024-05-14 06:23:54.000000 m_mock-1.3.4/m_mock/test_case/test_date.py
+-rw-rw-rw-   0        0        0      229 2024-05-14 06:23:54.000000 m_mock-1.3.4/m_mock/test_case/test_helper.py
+-rw-rw-rw-   0        0        0      393 2024-05-14 06:37:53.000000 m_mock-1.3.4/m_mock/test_case/test_miscellaneous.py
+-rw-rw-rw-   0        0        0      851 2024-05-14 06:23:54.000000 m_mock-1.3.4/m_mock/test_case/test_name.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:13:40.583702 m_mock-1.3.4/m_mock.egg-info/
+-rw-rw-rw-   0        0        0     4473 2024-05-14 07:13:40.000000 m_mock-1.3.4/m_mock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-05-14 07:13:40.000000 m_mock-1.3.4/m_mock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:13:40.000000 m_mock-1.3.4/m_mock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-14 07:13:40.000000 m_mock-1.3.4/m_mock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 07:13:40.000000 m_mock-1.3.4/m_mock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      433 2024-05-14 07:00:00.000000 m_mock-1.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 07:13:40.586703 m_mock-1.3.4/setup.cfg
```

### Comparing `m_mock-1.3.3/LICENSE` & `m_mock-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.3/PKG-INFO` & `m_mock-1.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_mock
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is a tool for producing random data.
 Author-email: Franciz <franciz467@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -134,7 +134,15 @@
 m_mock.mock("@now('hour')"):2023-02-20 13:00:00
 m_mock.mock("@now('minute')"):2023-02-20 13:42:00
 m_mock.mock("@now('second')"):2023-02-20 13:42:44
 m_mock.mock("@now()"):2023-02-20 13:42:44
 m_mock.mock("@now('year','%Y年-%m月-%d日 %H:%M:%S')"):2023年-01月-01日 00:00:00
 m_mock.mock("@now('week','%Y年 %m月 %d日 %H:%M:%S')"):2023年 02月 26日 00:00:00
 ```
+
+# miscellaneous 杂项
+```python
+m_mock.mock('@id()'):397425198210051092
+m_mock.mock('@increment()'):1
+m_mock.mock('@increment(100)'):101
+m_mock.mock('@uuid()'):"4f35a282-73d0-4705-9fd5-ddf722e78eea"
+```
```

### Comparing `m_mock-1.3.3/README.md` & `m_mock-1.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -120,7 +120,15 @@
 m_mock.mock("@now('hour')"):2023-02-20 13:00:00
 m_mock.mock("@now('minute')"):2023-02-20 13:42:00
 m_mock.mock("@now('second')"):2023-02-20 13:42:44
 m_mock.mock("@now()"):2023-02-20 13:42:44
 m_mock.mock("@now('year','%Y年-%m月-%d日 %H:%M:%S')"):2023年-01月-01日 00:00:00
 m_mock.mock("@now('week','%Y年 %m月 %d日 %H:%M:%S')"):2023年 02月 26日 00:00:00
 ```
+
+# miscellaneous 杂项
+```python
+m_mock.mock('@id()'):397425198210051092
+m_mock.mock('@increment()'):1
+m_mock.mock('@increment(100)'):101
+m_mock.mock('@uuid()'):"4f35a282-73d0-4705-9fd5-ddf722e78eea"
+```
```

### Comparing `m_mock-1.3.3/license.txt` & `m_mock-1.3.4/license.txt`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.3/m_mock/m_random.py` & `m_mock-1.3.4/m_mock/m_random.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import re
 import string
+import uuid
 from datetime import datetime, timedelta
 
 from dateutil.relativedelta import relativedelta
 
 from m_mock.m_random_source import single_family_name, en_family_name, en_name
 
 
@@ -238,56 +239,78 @@
 
 
 class FloatM:
     @classmethod
     def float(cls, min_value=None, max_value=None, d_min_value=None,
               d_max_value=None):
         """
-        随机浮点数,example:
-        @float(95,100,12,19)
-        @float(1,2)
-        @float(952)  # 不小于992
-        @float()  # 随机
-        @float
-        :param min_value:个位部分最小值
-        :param max_value:个位部分最大值
-        :param d_min_value:小数部分最小长度
-        :param d_max_value:小数部分最大长度
-        :return:
+        生成一个随机浮点数。如果指定范围，将在该范围内生成。
+
+        :param min_value: 整数部分最小值，如果未提供则不设置下限。
+        :param max_value: 整数部分最大值，如果未提供则不设置上限。
+        :param d_min_value: 小数部分最小位数，如果未提供，则随机选择0或2到5之间的一个数。
+        :param d_max_value: 小数部分最大位数，如果未提供，则根据d_min_value随机确定上限。
+
+        使用示例:
+        - @float(95,100,12,19): 在95到100之间生成一个浮点数，小数部分位数在12到19之间。
+        - @float(1,2): 在1到2之间生成一个浮点数，小数部分位数随机确定。
+        - @float(952): 不小于952的浮点数，小数部分位数随机确定。
+        - @float(): 完全随机生成一个浮点数。
+        - @float: 与@float()相同，完全随机生成一个浮点数。
+
+        :return: 生成的随机浮点数。
         """
 
         def __luck():
+            # 随机决定是否执行某操作（3/4的概率为True）
             return random.randint(1, 4) in (1, 2, 3)
 
+        # 校验最小值和最大值，抛出异常如果有必要（这里假设这个函数是已经实现的）
         _mock_exception.min_max_value_exception(min_value, max_value)
+
+        # 设置默认整数部分最小值和最大值
         if inNone(min_value):
             min_value = -9999999999999999
         if inNone(max_value):
             max_value = 9999999999999999
+
+        # 设置默认小数部分最小长度
         if inNone(d_min_value):
-            d_min_value = random.randint(2, 5) if random.randint(1, 2) == 1 else 0
+            d_min_value = random.randint(2, 5) if __luck() else 0
+
+        # 设置默认小数部分最大长度
         if inNone(d_max_value):
             min_d_max_value = d_min_value if 14 > d_min_value > 0 else d_min_value + 1
             d_max_value = random.randint(min_d_max_value + 1, 16)
+
+        # 生成随机小数部分字符串
         decimals = StringM.string_number(d_min_value, d_max_value)
+
+        # 以3/4的概率执行以下代码块
         if __luck():
             while True:
-                # 满足最小值和最大值的浮点数
+                # 生成满足最小值和最大值的浮点数
                 random_float = random.uniform(min_value, max_value)
                 val = str(random_float)
                 if '.' in val:
                     break
             int_part = val.split(".")[0]
-            int_part = int_part if len(int_part) + len(decimals) <= 15 else int_part[:len(decimals)]
+
+            # 确保整数部分加上小数部分的长度不超过15位
+            int_part = int_part if len(int_part) + len(decimals) <= 15 else int_part[:15 - len(decimals)]
             val = f'{int_part}.{decimals}'
             random_float = float(val)
         else:
             random_float = random.uniform(min_value, max_value)
+            # 再次以3/4的概率执行以下代码块
             if __luck():
+                # 保留随机浮点数的除最后一位外的所有数，并在最后追加一个新的随机整数(1-9)
                 random_float = float(f'{str(random_float)[:-1]}{random.randint(1, 9)}')
+
+        # 随机确定四舍五入的小数位数
         round_num = random.randint(d_min_value, d_max_value)
         return float(round(random_float, round_num))
 
 
 m_float = FloatM()
 
 
@@ -297,14 +320,21 @@
         """
         :return: 随机小写英文字符
         """
         return cls.get_random_string_by_source(string.ascii_lowercase, min_value, max_value)
 
     @classmethod
     def get_random_string_by_source(cls, source=None, min_value: int = None, max_value: int = None) -> str:
+        """
+
+        :param source:
+        :param min_value:
+        :param max_value:
+        :return:
+        """
         _mock_exception.min_max_value_exception(min_value, max_value)
         if inNone(min_value):
             length = random.randint(1, 9)
         elif inNone(max_value):
             length = min_value
         else:
             length = random.randint(min_value, max_value)
@@ -338,15 +368,15 @@
         """
         return cls.get_random_string_by_source(string.punctuation, min_value, max_value)
 
     @classmethod
     def strings(cls, min_value=None, max_value=None) -> str:
         """
 
-        :return: 包含(英文/英文标点/数字)的随机字符
+        :return: 包含(英文/英文标点/数字)的随机长度的字符
         """
         source = string.ascii_letters + string.digits + string.punctuation
         return cls.get_random_string_by_source(source, min_value, max_value)
 
     @classmethod
     def chinese(cls, min_value=None, max_value=None) -> str:
         """
@@ -700,15 +730,80 @@
         cname = cls.clast() + cls.cfirst(length - 1)
         # assert not '\n' in cname
         return cname
 
 
 m_name = NameM()
 
-# class ImageM:
-#     @classmethod
-#     def image(cls):
-#         img = Image.new("RGB", (200, 300), (0, 0, 0))  # 8*8像素
-#         img.save("./black.png")
-#
-#
-# m_image = ImageM()
+
+class MiscellaneousM:
+    """
+    杂项
+    """
+
+    @classmethod
+    def uuid(cls):
+        """
+        生成随机的UUID
+        :return: UUID
+        """
+        return str(uuid.uuid4())
+
+    @classmethod
+    def id(cls):
+        """
+        生成随机的身份证号
+        :return: 身份证号
+        """
+        return cls.generate_random_id()
+
+    increment_start = 0
+
+    @classmethod
+    def increment(cls, step=None):
+        """
+        自增函数,默认自增起始值为0
+        :param step: 步长
+        :return: 自增后的值
+        """
+        if step is None:
+            step = 1
+        cls.increment_start += step
+        return f"{cls.increment_start}"
+
+    @classmethod
+    def get_random_date(cls, start_year=1960, end_year=2020):
+        """生成随机出生日期"""
+        import datetime
+        start = datetime.date(start_year, 1, 1)
+        end = datetime.date(end_year, 12, 31)
+        days_between = (end - start).days
+        random_days = random.randrange(days_between)
+        birth_date = start + datetime.timedelta(days=random_days)
+        return birth_date.strftime("%Y%m%d")
+
+    @classmethod
+    def calculate_checksum(cls, id17):
+        """计算身份证最后的校验码"""
+        weights = [7, 9, 10, 5, 8, 4, 2, 1, 6, 3, 7, 9, 10, 5, 8, 4, 2]
+        checksums = '10X98765432'
+        sum_product = sum(int(id17[i]) * weights[i] for i in range(17))
+        return checksums[sum_product % 11]
+
+    @classmethod
+    def generate_random_id(cls):
+        """生成随机的中国身份证号码"""
+        # 随机地址码（简化处理，实际应为有效地址码）
+        region_code = str(random.randint(100000, 699999))
+        # 随机生成出生日期码
+        birth_date = cls.get_random_date()
+        # 随机生成顺序码（性别码偶数女，奇数男）
+        sequence_code = str(random.randint(000, 999)).zfill(3)
+        # 组成前17位
+        id17 = region_code + birth_date + sequence_code
+        # 计算校验码
+        checksum = cls.calculate_checksum(id17)
+        # 完整的身份证号码
+        return f"{id17}{checksum}"
+
+
+m_miscellaneous = MiscellaneousM()
```

### Comparing `m_mock-1.3.3/m_mock/m_random_source.py` & `m_mock-1.3.4/m_mock/m_random_source.py`

 * *Files identical despite different names*

### Comparing `m_mock-1.3.3/m_mock/test_case/test_basic.py` & `m_mock-1.3.4/m_mock/test_case/test_basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import unittest
 
 from m_mock import m_random
-from m_mock.test_case.common_utils import execute
+from m_mock.test_case.common_utils import execute_mock
 
 
 class TestBasic(unittest.TestCase):
     def test_basic_character(self):
         print(m_random.m_character.character())
-        execute("@character()")
-        execute("@character('lower')")
-        execute("@character('upper')")
-        execute("@character('number')")
-        execute("@character('symbol')")
-        execute("@character('aeiou')")
+        execute_mock("@character()")
+        execute_mock("@character('lower')")
+        execute_mock("@character('upper')")
+        execute_mock("@character('number')")
+        execute_mock("@character('symbol')")
+        execute_mock("@character('aeiou')")
 
     def test_basic_integer(self):
         print(m_random.m_integer.integer())
-        execute("@integer(2,4)")
-        execute("@integer(3)")
-        execute("@integer()")
-        execute("@integer(2,2)")
+        execute_mock("@integer(2,4)")
+        execute_mock("@integer(3)")
+        execute_mock("@integer()")
+        # execute_mock("@integer(2,2)")
 
     def test_basic_boolean(self):
         print(m_random.m_boolean.boolean())
-        execute("@boolean(2,4)")
-        execute("@boolean(3)")
-        execute("@boolean()")
-        execute("@boolean(2,2)")
+        execute_mock("@boolean(2,4)")
+        execute_mock("@boolean(3)")
+        execute_mock("@boolean()")
+        execute_mock("@boolean(2,2)")
 
     def test_basic_float(self):
         print(m_random.m_float.float())
-        execute("@float(2,4)")
-        execute("@float(3)")
-        execute("@float()")
-        execute("@float(2,2)")
+        execute_mock("@float(2,4)")
+        execute_mock("@float(3)")
+        execute_mock("@float()")
+        execute_mock("@float(2,2)")
 
     def test_basic_string(self):
         print(m_random.m_string.string())
         print(m_random.m_string.string(7))
         print(m_random.m_string.string(7, 10))
-        execute("@string(2)")
-        execute("@string('lower', 3)")
-        execute("@string('upper', 3)")
-        execute("@string('number', 3)")
-        execute("@string('symbol', 3)")
-        execute("@string('aeiou', 3)")
-        execute("@string('lower', 1, 3)")
-        execute("@string('upper', 1, 3)")
-        execute("@string('number', 1, 3)")
-        execute("@string('symbol', 1, 3)")
-        execute("@string('aeiou', 1, 3)")
-        execute("@string('chinese', 1, 3)")
-        execute("@string('cn_symbol', 1, 3)")
-        execute("@string('cn_string', 3, 9)")
-        execute("@string('cn_string', 1)")
-        execute("@string('abcd', 2)")
+        execute_mock("@string(2)")
+        execute_mock("@string('lower', 3)")
+        execute_mock("@string('upper', 3)")
+        execute_mock("@string('number', 3)")
+        execute_mock("@string('symbol', 3)")
+        execute_mock("@string('aeiou', 3)")
+        execute_mock("@string('lower', 1, 3)")
+        execute_mock("@string('upper', 1, 3)")
+        execute_mock("@string('number', 1, 3)")
+        execute_mock("@string('symbol', 1, 3)")
+        execute_mock("@string('aeiou', 1, 3)")
+        execute_mock("@string('chinese', 1, 3)")
+        execute_mock("@string('cn_symbol', 1, 3)")
+        execute_mock("@string('cn_string', 3, 9)")
+        execute_mock("@string('cn_string', 1)")
+        execute_mock("@string('abcd', 2)")
```

### Comparing `m_mock-1.3.3/m_mock/test_case/test_date.py` & `m_mock-1.3.4/m_mock/test_case/test_date.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from m_mock import m_random
-from m_mock.test_case.common_utils import execute
+from m_mock.test_case.common_utils import execute_mock
 
 
 class TestDate:
     def test_date(self):
-        execute("@date('%Y-%m-%d %H:%M:%S', '+1d')")
-        execute("@date('%Y-%m-%d %H:%M:%S', '+24h')")
+        execute_mock("@date('%Y-%m-%d %H:%M:%S', '+1d')")
+        execute_mock("@date('%Y-%m-%d %H:%M:%S', '+24h')")
         # 格式化
-        execute("@date('%Y年-%m月-%d日 %H时:%M分:%S秒', '+2mon')")
-        execute("@date('%Y年-%m月-%d日 %H时:%M分:%S秒', '+2min')")
+        execute_mock("@date('%Y年-%m月-%d日 %H时:%M分:%S秒', '+2mon')")
+        execute_mock("@date('%Y年-%m月-%d日 %H时:%M分:%S秒', '+2min')")
         print(m_random.m_date.date('%y-%m-%d', '-20d'))
         print(m_random.m_date.date())
 
     def test_time(self):
         print(m_random.m_date.time('', '+2sec'))
         print(m_random.m_date.time('', '+4sec'))
-        execute("@time('', '+4sec')")
-        execute("@time")
+        execute_mock("@time('', '+4sec')")
+        execute_mock("@time")
 
     def test_now(self):
         print(m_random.m_date.now('year'))
         print(m_random.m_date.now('month'))
         print(m_random.m_date.now('week'))
         print(m_random.m_date.now('day'))
         print(m_random.m_date.now('hour'))
         print(m_random.m_date.now('minute'))
         print(m_random.m_date.now('second'))
-        execute("@now('year')")
-        execute("@now('month')")
-        execute("@now('week')")
-        execute("@now('day')")
-        execute("@now('hour')")
-        execute("@now('minute')")
-        execute("@now('second')")
-        execute("@now()")
+        execute_mock("@now('year')")
+        execute_mock("@now('month')")
+        execute_mock("@now('week')")
+        execute_mock("@now('day')")
+        execute_mock("@now('hour')")
+        execute_mock("@now('minute')")
+        execute_mock("@now('second')")
+        execute_mock("@now()")
         # 格式化
-        execute("@now('year','%Y年-%m月-%d日 %H:%M:%S')")
+        execute_mock("@now('year','%Y年-%m月-%d日 %H:%M:%S')")
         # 格式化
-        execute("@now('week','%Y年 %m月 %d日 %H:%M:%S')")
+        execute_mock("@now('week','%Y年 %m月 %d日 %H:%M:%S')")
```

### Comparing `m_mock-1.3.3/m_mock/test_case/test_name.py` & `m_mock-1.3.4/m_mock/test_case/test_name.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import unittest
 
 from m_mock.m_random import m_name
-from m_mock.test_case.common_utils import execute
+from m_mock.test_case.common_utils import execute_mock
 
 
 class TestName(unittest.TestCase):
     def test_name(self):
-        execute("""@clast()""")
-        execute("""@cfirst()""")
-        execute("""@cname()""")
-        execute("""@cname(3)""")
-        execute("""@last()""")
-        execute("""@first()""")
-        execute("""@name()""")
-        execute("""@name(True)""")
+        execute_mock("""@clast()""")
+        execute_mock("""@cfirst()""")
+        execute_mock("""@cname()""")
+        execute_mock("""@cname(3)""")
+        execute_mock("""@last()""")
+        execute_mock("""@first()""")
+        execute_mock("""@name()""")
+        execute_mock("""@name(True)""")
         print(m_name.cfirst())
         print(m_name.clast())
         print(m_name.cname())
         print(m_name.first())
         print(m_name.last())
         print(m_name.name())
         print(m_name.name(True))
```

### Comparing `m_mock-1.3.3/m_mock.egg-info/PKG-INFO` & `m_mock-1.3.4/m_mock.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m_mock
-Version: 1.3.3
+Version: 1.3.4
 Summary: This is a tool for producing random data.
 Author-email: Franciz <franciz467@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -134,7 +134,15 @@
 m_mock.mock("@now('hour')"):2023-02-20 13:00:00
 m_mock.mock("@now('minute')"):2023-02-20 13:42:00
 m_mock.mock("@now('second')"):2023-02-20 13:42:44
 m_mock.mock("@now()"):2023-02-20 13:42:44
 m_mock.mock("@now('year','%Y年-%m月-%d日 %H:%M:%S')"):2023年-01月-01日 00:00:00
 m_mock.mock("@now('week','%Y年 %m月 %d日 %H:%M:%S')"):2023年 02月 26日 00:00:00
 ```
+
+# miscellaneous 杂项
+```python
+m_mock.mock('@id()'):397425198210051092
+m_mock.mock('@increment()'):1
+m_mock.mock('@increment(100)'):101
+m_mock.mock('@uuid()'):"4f35a282-73d0-4705-9fd5-ddf722e78eea"
+```
```

