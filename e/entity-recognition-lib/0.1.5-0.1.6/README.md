# Comparing `tmp/entity_recognition_lib-0.1.5.tar.gz` & `tmp/entity_recognition_lib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_recognition_lib-0.1.5.tar", max compression
+gzip compressed data, was "entity_recognition_lib-0.1.6.tar", max compression
```

## Comparing `entity_recognition_lib-0.1.5.tar` & `entity_recognition_lib-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1054 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/LICENSE
--rw-r--r--   0        0        0     3696 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/README.md
--rw-r--r--   0        0        0     1828 2024-05-13 13:02:31.478689 entity_recognition_lib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1821 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/EntityRecognizer.py
--rw-r--r--   0        0        0       61 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/__init__.py
--rw-r--r--   0        0        0    31573 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/data/tech_entities.json
--rw-r--r--   0        0        0        0 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/__init__.py
--rw-r--r--   0        0        0     2868 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/entity_extraction.py
--rw-r--r--   0        0        0     5314 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/recommendation_generation.py
--rw-r--r--   0        0        0     1271 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/topic_classification.py
--rw-r--r--   0        0        0     1725 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/models.py
--rw-r--r--   0        0        0     3279 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/utils.py
--rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-14 12:10:36.210043 entity_recognition_lib-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2741 2024-05-14 12:10:36.210043 entity_recognition_lib-0.1.6/README.md
+-rw-r--r--   0        0        0     1828 2024-05-14 12:12:09.146321 entity_recognition_lib-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1821 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/EntityRecognizer.py
+-rw-r--r--   0        0        0       61 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/__init__.py
+-rw-r--r--   0        0        0    31573 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/data/tech_entities.json
+-rw-r--r--   0        0        0        0 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/__init__.py
+-rw-r--r--   0        0        0     2868 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/entity_extraction.py
+-rw-r--r--   0        0        0     5314 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/recommendation_generation.py
+-rw-r--r--   0        0        0     1271 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/topic_classification.py
+-rw-r--r--   0        0        0     1725 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/models.py
+-rw-r--r--   0        0        0     3279 2024-05-14 12:10:36.214043 entity_recognition_lib-0.1.6/src/entity_recognition_lib/utils.py
+-rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.6/PKG-INFO
```

### Comparing `entity_recognition_lib-0.1.5/LICENSE` & `entity_recognition_lib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/pyproject.toml` & `entity_recognition_lib-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entity-recognition-lib"
-version = "0.1.5"
+version = "0.1.6"
 description = "A library for technology entity recognition and recommendation"
 authors = ["Cesar Goncalves <goncalves.cesaraugusto94@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/EntityRecognizer.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/EntityRecognizer.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/data/tech_entities.json` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/data/tech_entities.json`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/entity_extraction.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/recommendation_generation.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/recommendation_generation.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/topic_classification.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/functions/topic_classification.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/models.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/models.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/src/entity_recognition_lib/utils.py` & `entity_recognition_lib-0.1.6/src/entity_recognition_lib/utils.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.5/PKG-INFO` & `entity_recognition_lib-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-recognition-lib
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for technology entity recognition and recommendation
 License: MIT
 Author: Cesar Goncalves
 Author-email: goncalves.cesaraugusto94@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,147 +18,95 @@
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# Entity-Recognition
+# Entity Recognition Library
 
-The Entity-Recognition library utilizes `spaCy`, `BERTopic`, and `Transformers` to provide a robust technology entity
-recognition system capable of identifying technological entities within texts and suggesting relevant technologies using
-advanced NLP techniques.
+## Purpose
 
-The library automatically downloads the required spaCy model if not installed, making it easy to get started.
+The Entity Recognition serves as a library for identifying technological entities within texts and suggesting relevant
+ technologies using advanced NLP techniques.
 
-## Features
+## Installing the Library
 
-- **Technology Entity Extraction**: Automatically extract technology-related terms and tools from texts.
-- **Recommendation System**: Provides context-based technology recommendations.
-- **BERTopic Integration**: Leverages topic modeling to enhance the relevance of recommendations.
-- **spaCy Matchers**: Utilizes custom NLP patterns for precise entity recognition.
-
-## Installation
-
-### Prerequisites
-
-- Python 3.11+
-- pip
-
-### Getting Started
-
-Install the library directly from PyPI:
+Integrate our library into your project by installing it directly from [PyPI](https://pypi.org/project/entity-recognition-lib/#description):
 
 ```bash
 pip install entity-recognition-lib
 ```
 
 The required spaCy model (`en_core_web_sm`) will be automatically downloaded and installed if not already present on
-your system.
+ your system.
 
-## Usage
+## Using the Library
 
 Here's how to use the Entity Recognition library in your Python scripts:
 
 ```python
 from entity_recognition_lib import EntityRecognizer
 
-# Create an instance of the recognizer
 recognizer = EntityRecognizer()
-
-# Example texts
-texts = ["I need an Express.js Mongo database backend"]
-
-# Process texts
+texts = ["Your text here"]
 results = recognizer.process_texts(texts)
 print(results)
 ```
 
-Expected output:
+## Expected Output
+
+The library processes text to identify and categorize technology entities, delivering structured output that includes
+ identified entities and contextual recommendations.
+
+Example output:
 
 ```json
 [
-    {
-        "input_text": "I need an Express.js Mongo database backend",
-        "predicted_topic_name": "575_databases_database_tables_schema",
-        "extracted_entities": [
-            {
-                "entity_name": "Express.js",
-                "score": 1.0,
-                "category": "Backend Web Frameworks"
-            },
-            {
-                "entity_name": "MongoDB",
-                "score": 1.0,
-                "category": "Databases"
-            }
-        ],
-        "recommendations": [
-            {
-                "category": "Backend Web Frameworks",
-                "recommendation": "Express.js"
-            },
-            {
-                "category": "Databases",
-                "recommendation": "MongoDB"
-            }
-        ]
-    }
+  {
+    "input_text": "Example text with technology entities",
+    "predicted_topic_name": "topic_name",
+    "extracted_entities": [
+      {
+        "entity_name": "entity_1",
+        "score": 0.9,
+        "category": "Category 1"
+      },
+      {
+        "entity_name": "entity_2",
+        "score": 0.8,
+        "category": "Category 1"
+      }
+    ],
+    "recommendations": [
+      {
+        "category": "Category 1",
+        "recommendation": "entity_1"
+      }
+    ]
+  }
 ]
 ```
 
-For detailed usage examples and code snippets, please refer to the [examples directory](examples/EXAMPLES.md) in the repository.
+For detailed usage examples and code snippets, please refer to the
+ [examples directory](https://github.com/warestack/entity-recognition/blob/main/examples/EXAMPLES.md) in the repository.
 The examples cover various scenarios, including:
 
 - Basic usage of the library for entity recognition and recommendation generation
 - Advanced features such as result analysis and visualization
 - Integration samples with popular frameworks like Flask and Streamlit
 
-We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your
-projects.
-
-## Development
-
-### Setting Up a Development Environment
-
-- **Clone the repository**:
-
-   ```bash
-   git clone https://github.com/cgoncalves94/entity-recognition.git
-   cd entity-recognition
-   ```
-
-- **Create and Activate a Virtual Environment**:
-
-   ```bash
-   python -m venv .venv
-   source .venv/bin/activate  # On Windows use `venv\Scripts\activate`
-   ```
-
-- **Install Dependencies**:
-
-    ```bash
-    pip install -r requirements.txt
-    ```
-
-## Testing
-
-Run tests to ensure the setup is correct:
-
-```bash
-pytest
-```
+We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your projects.
 
 ## Contributing
 
-Contributions are welcome! Please follow these steps:
-
-- Fork the repository on GitHub.
-- Clone the forked repository to your machine.
-- Create a new branch for your changes.
-- Make changes and test.
-- Submit a pull request with a comprehensive description of changes.
+If you consider contributing to the Entity Recognition library, make sure to check out our
+ [Contributing Guide](https://github.com/warestack/entity-recognition/blob/main/CONTRIBUTING.md) and our
+  [Development Guide](https://github.com/warestack/entity-recognition/blob/main/DEVELOPMENT.md), for more information
+   on how to run and test the project locally.
+You are welcome to expand the technology entities corpus or add a new feature.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the
+ [LICENSE](https://github.com/warestack/entity-recognition/blob/main/LICENSE) file for details.
```

