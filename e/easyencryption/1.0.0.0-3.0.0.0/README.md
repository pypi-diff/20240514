# Comparing `tmp/easyencryption-1.0.0.0.tar.gz` & `tmp/easyencryption-3.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-1.0.0.0.tar", last modified: Sat Apr 13 13:05:18 2024, max compression
+gzip compressed data, was "easyencryption-3.0.0.0.tar", last modified: Sat Apr 13 23:38:36 2024, max compression
```

## Comparing `easyencryption-1.0.0.0.tar` & `easyencryption-3.0.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 13:05:18.343004 easyencryption-1.0.0.0/
--rw-rw-rw-   0        0        0     3921 2024-04-13 13:05:18.341977 easyencryption-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2024-04-13 12:14:15.000000 easyencryption-1.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 13:05:18.340955 easyencryption-1.0.0.0/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3921 2024-04-13 13:05:18.000000 easyencryption-1.0.0.0/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-13 13:05:18.000000 easyencryption-1.0.0.0/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 13:05:18.000000 easyencryption-1.0.0.0/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-13 13:05:18.000000 easyencryption-1.0.0.0/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 13:05:18.000000 easyencryption-1.0.0.0/easyencryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 13:05:18.343004 easyencryption-1.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1780 2024-04-13 12:57:42.000000 easyencryption-1.0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:38:36.939563 easyencryption-3.0.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-13 23:38:36.939563 easyencryption-3.0.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 23:38:33.000000 easyencryption-3.0.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:38:36.939563 easyencryption-3.0.0.0/easyencryption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-13 23:38:36.000000 easyencryption-3.0.0.0/easyencryption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-13 23:38:36.000000 easyencryption-3.0.0.0/easyencryption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:38:36.000000 easyencryption-3.0.0.0/easyencryption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 23:38:36.000000 easyencryption-3.0.0.0/easyencryption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:38:36.000000 easyencryption-3.0.0.0/easyencryption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:38:36.939563 easyencryption-3.0.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 23:38:33.000000 easyencryption-3.0.0.0/setup.py
```

### Comparing `easyencryption-1.0.0.0/PKG-INFO` & `easyencryption-3.0.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: easyencryption
-Version: 1.0.0.0
-Summary: A very easy way to encrypt data.
-Home-page: https://github.com/BlazenBoi/easyencryption/issues
-Author: Blazen
-Author-email: contact@fireballbot.com
-License: MIT
-Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
-Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
-Project-URL: Source, https://github.com/BlazenBoi/easyencryption
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools>=42
-Requires-Dist: cryptography
-Requires-Dist: pycryptodomex
-Requires-Dist: pycryptodome
-Requires-Dist: wheel
-Requires-Dist: eciespy
-
-In Progress...
-
-# Algorithms
-
-## Encryption Algorithms
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
-
-## Hashing Algorithms
-
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
+Metadata-Version: 2.1
+Name: easyencryption
+Version: 3.0.0.0
+Summary: A very easy way to encrypt data.
+Home-page: https://github.com/BlazenBoi/easyencryption/issues
+Author: Blazen
+Author-email: contact@fireballbot.com
+License: MIT
+Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
+Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
+Project-URL: Source, https://github.com/BlazenBoi/easyencryption
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
+
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-1.0.0.0/README.md` & `easyencryption-3.0.0.0/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-In Progress...
-
-# Algorithms
-
-## Encryption Algorithms
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
-
-## Hashing Algorithms
-
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
 [![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-1.0.0.0/easyencryption.egg-info/PKG-INFO` & `easyencryption-3.0.0.0/easyencryption.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-Metadata-Version: 2.1
-Name: easyencryption
-Version: 1.0.0.0
-Summary: A very easy way to encrypt data.
-Home-page: https://github.com/BlazenBoi/easyencryption/issues
-Author: Blazen
-Author-email: contact@fireballbot.com
-License: MIT
-Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
-Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
-Project-URL: Source, https://github.com/BlazenBoi/easyencryption
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: setuptools>=42
-Requires-Dist: cryptography
-Requires-Dist: pycryptodomex
-Requires-Dist: pycryptodome
-Requires-Dist: wheel
-Requires-Dist: eciespy
-
-In Progress...
-
-# Algorithms
-
-## Encryption Algorithms
-
-Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
-AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
-RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
-Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
-
-## Hashing Algorithms
-
-SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
-Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
-
-This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
-
-**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
-
-# Information
-
-[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
-[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
-
-# Downloads
-
-[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
-[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
+Metadata-Version: 2.1
+Name: easyencryption
+Version: 3.0.0.0
+Summary: A very easy way to encrypt data.
+Home-page: https://github.com/BlazenBoi/easyencryption/issues
+Author: Blazen
+Author-email: contact@fireballbot.com
+License: MIT
+Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
+Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
+Project-URL: Source, https://github.com/BlazenBoi/easyencryption
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
+
+In Progress...
+
+# Algorithms
+
+## Encryption Algorithms
+
+Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
+AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
+RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created.<br /><br />
+
+## Hashing Algorithms
+
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br /><br />
+
+This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
+
+**WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
+
+# Information
+
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
+[![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
+
+# Downloads
+
+[![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
+[![Downloads](https://pepy.tech/badge/easyencryption/week)](https://pepy.tech/project/easyencryption)
```

### Comparing `easyencryption-1.0.0.0/setup.py` & `easyencryption-3.0.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_desc = open("README.md", "r")
-long_description = long_desc.read()
-version = "1.0.0.0"
-
-setup(
-    name='easyencryption',
-    version=version,
-    description='A very easy way to encrypt data.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    license='MIT',
-    url='https://github.com/BlazenBoi/easyencryption/issues',
-    author='Blazen',
-    author_email='contact@fireballbot.com',
-    keywords='',
-    packages=find_packages(include=['easyencryption']),
-    python_requires='>=3.7',
-    install_requires=[
-    "setuptools>=42",
-    "cryptography",
-    "pycryptodomex",
-    "pycryptodome",
-    "wheel",
-    "eciespy",
-    ],
-    project_urls={
-        'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
-        'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
-        'Source': 'https://github.com/BlazenBoi/easyencryption',
-    },
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Internet',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-      ]
-)
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_desc = open("README.md", "r")
+long_description = long_desc.read()
+version = "3.0.0.0"
+
+setup(
+    name='easyencryption',
+    version=version,
+    description='A very easy way to encrypt data.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    license='MIT',
+    url='https://github.com/BlazenBoi/easyencryption/issues',
+    author='Blazen',
+    author_email='contact@fireballbot.com',
+    keywords='',
+    packages=find_packages(include=['easyencryption']),
+    python_requires='>=3.7',
+    install_requires=[
+    "setuptools>=42",
+    "cryptography",
+    "pycryptodomex",
+    "pycryptodome",
+    "wheel",
+    "eciespy",
+    ],
+    project_urls={
+        'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
+        'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
+        'Source': 'https://github.com/BlazenBoi/easyencryption',
+    },
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Internet',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+      ]
+)
 #© 2021 GitHub, Inc.
```

