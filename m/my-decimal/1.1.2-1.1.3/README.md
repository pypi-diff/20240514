# Comparing `tmp/my_decimal-1.1.2.tar.gz` & `tmp/my_decimal-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_decimal-1.1.2.tar", last modified: Tue May  7 14:47:37 2024, max compression
+gzip compressed data, was "my_decimal-1.1.3.tar", last modified: Mon May 13 22:18:52 2024, max compression
```

## Comparing `my_decimal-1.1.2.tar` & `my_decimal-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:47:37.988832 my_decimal-1.1.2/
--rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2092 2024-05-07 14:47:37.988832 my_decimal-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2024-05-07 14:45:46.000000 my_decimal-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:47:37.987831 my_decimal-1.1.2/my_decimal.egg-info/
--rw-rw-rw-   0        0        0     2092 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 14:47:37.000000 my_decimal-1.1.2/my_decimal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2024-05-06 17:10:58.000000 my_decimal-1.1.2/my_decimal.py
--rw-rw-rw-   0        0        0       42 2024-05-07 14:47:37.989831 my_decimal-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-05-07 14:47:34.000000 my_decimal-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 22:18:52.750656 my_decimal-1.1.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2152 2024-05-13 22:18:52.749657 my_decimal-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1913 2024-05-13 22:18:46.000000 my_decimal-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 22:18:52.748658 my_decimal-1.1.3/my_decimal.egg-info/
+-rw-rw-rw-   0        0        0     2152 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       61 2024-05-06 17:10:58.000000 my_decimal-1.1.3/my_decimal.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 22:18:52.750656 my_decimal-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-13 22:18:46.000000 my_decimal-1.1.3/setup.py
```

### Comparing `my_decimal-1.1.2/LICENSE` & `my_decimal-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `my_decimal-1.1.2/PKG-INFO` & `my_decimal-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_decimal
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small library for formatting decimals
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,44 +23,50 @@
 ## Пример использования
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
-result = f'{num1}+{num2}'
+result = num1 + num2
 
-print(result)
-# Вывод: 0.3
+print(f'{result:.3f}')
+# Вывод: 0.300
 ```
 
 2. ### c модулем decimal
 ```python
 from decimal import Decimal
 
-num1 = 0.1
-num2 = 0.2
+num1 = Decimal('0.1')
+num2 = Decimal('0.2')
 
-result = Decimal(num1) + Decimal(num2)
+result = num1 + num2
 
 print(result)
+
 # Вывод: 0.3
 
 ```
 3. ### c модулем my_decimal
 ```python
 from my_decimal import my_decimal
 
 num1 = 0.1
 num2 = 0.2
 
 result = my_decimal(num1+num2)
 
 print(result)  
-# Вывод: 0.3
+# Вывод: 0.300
 ```
 ## как мы видим использование модуля my_decimal самое удобное
 
 #### Функция принимает числовое выражение и возвращает его в формате строки с округлением до трех знаков после запятой.
 ***
 ## Важно
 *Функция my_decimal предполагает, что входное выражение является числом. При передаче нечисловых значений будут возникать ошибки.*
+
+***
+### Автор
+
+Автор: k0ng999
```

### Comparing `my_decimal-1.1.2/README.md` & `my_decimal-1.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,44 +13,50 @@
 ## Пример использования
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
-result = f'{num1}+{num2}'
+result = num1 + num2
 
-print(result)
-# Вывод: 0.3
+print(f'{result:.3f}')
+# Вывод: 0.300
 ```
 
 2. ### c модулем decimal
 ```python
 from decimal import Decimal
 
-num1 = 0.1
-num2 = 0.2
+num1 = Decimal('0.1')
+num2 = Decimal('0.2')
 
-result = Decimal(num1) + Decimal(num2)
+result = num1 + num2
 
 print(result)
+
 # Вывод: 0.3
 
 ```
 3. ### c модулем my_decimal
 ```python
 from my_decimal import my_decimal
 
 num1 = 0.1
 num2 = 0.2
 
 result = my_decimal(num1+num2)
 
 print(result)  
-# Вывод: 0.3
+# Вывод: 0.300
 ```
 ## как мы видим использование модуля my_decimal самое удобное
 
 #### Функция принимает числовое выражение и возвращает его в формате строки с округлением до трех знаков после запятой.
 ***
 ## Важно
-*Функция my_decimal предполагает, что входное выражение является числом. При передаче нечисловых значений будут возникать ошибки.*
+*Функция my_decimal предполагает, что входное выражение является числом. При передаче нечисловых значений будут возникать ошибки.*
+
+***
+### Автор
+
+Автор: k0ng999
```

### Comparing `my_decimal-1.1.2/my_decimal.egg-info/PKG-INFO` & `my_decimal-1.1.3/my_decimal.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_decimal
-Version: 1.1.2
+Version: 1.1.3
 Summary: A small library for formatting decimals
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,44 +23,50 @@
 ## Пример использования
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
-result = f'{num1}+{num2}'
+result = num1 + num2
 
-print(result)
-# Вывод: 0.3
+print(f'{result:.3f}')
+# Вывод: 0.300
 ```
 
 2. ### c модулем decimal
 ```python
 from decimal import Decimal
 
-num1 = 0.1
-num2 = 0.2
+num1 = Decimal('0.1')
+num2 = Decimal('0.2')
 
-result = Decimal(num1) + Decimal(num2)
+result = num1 + num2
 
 print(result)
+
 # Вывод: 0.3
 
 ```
 3. ### c модулем my_decimal
 ```python
 from my_decimal import my_decimal
 
 num1 = 0.1
 num2 = 0.2
 
 result = my_decimal(num1+num2)
 
 print(result)  
-# Вывод: 0.3
+# Вывод: 0.300
 ```
 ## как мы видим использование модуля my_decimal самое удобное
 
 #### Функция принимает числовое выражение и возвращает его в формате строки с округлением до трех знаков после запятой.
 ***
 ## Важно
 *Функция my_decimal предполагает, что входное выражение является числом. При передаче нечисловых значений будут возникать ошибки.*
+
+***
+### Автор
+
+Автор: k0ng999
```

