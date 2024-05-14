# Comparing `tmp/omopsurvey-0.0.5.tar.gz` & `tmp/omopsurvey-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omopsurvey-0.0.5.tar", max compression
+gzip compressed data, was "omopsurvey-0.0.6.tar", max compression
```

## Comparing `omopsurvey-0.0.5.tar` & `omopsurvey-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     5369 2024-05-10 04:47:09.981340 omopsurvey-0.0.5/README.md
--rw-r--r--   0        0        0      258 2024-05-11 22:40:02.259765 omopsurvey-0.0.5/omopsurvey/__init__.py
--rw-r--r--   0        0        0     3921 2024-05-12 03:53:34.300366 omopsurvey-0.0.5/omopsurvey/codebooks.py
--rw-r--r--   0        0        0     1566 2024-05-12 03:58:00.406974 omopsurvey-0.0.5/omopsurvey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omopsurvey-0.0.5/omopsurvey/recode_missing.py
--rw-r--r--   0        0        0     4581 2024-05-11 22:35:34.376582 omopsurvey-0.0.5/omopsurvey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.5/omopsurvey/survey_key.csv
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.5/omopsurvey/tests/codebook_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.5/omopsurvey/tests/map_responses_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.5/omopsurvey/tests/pivot_data_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.5/omopsurvey/tests/recode_missing_test.py
--rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.5/omopsurvey/vignettes/example_basics.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.5/omopsurvey/vignettes/example_healthcare.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.5/omopsurvey/vignettes/example_sdoh.ipynb
--rw-r--r--   0        0        0      722 2024-05-12 04:24:32.235654 omopsurvey-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 omopsurvey-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5199 2024-05-14 07:32:18.341601 omopsurvey-0.0.6/README.md
+-rw-r--r--   0        0        0      273 2024-05-13 21:25:29.218835 omopsurvey-0.0.6/omopsurvey/__init__.py
+-rw-r--r--   0        0        0     3921 2024-05-12 03:53:34.300366 omopsurvey-0.0.6/omopsurvey/codebooks.py
+-rw-r--r--   0        0        0     5756 2024-05-14 07:10:39.939569 omopsurvey-0.0.6/omopsurvey/newdummy.csv
+-rw-r--r--   0        0        0     1566 2024-05-14 07:33:19.226040 omopsurvey-0.0.6/omopsurvey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omopsurvey-0.0.6/omopsurvey/recode_missing.py
+-rw-r--r--   0        0        0     7436 2024-05-14 07:33:20.872482 omopsurvey-0.0.6/omopsurvey/response_set.py
+-rw-r--r--   0        0        0     4703 2024-05-14 06:41:25.978692 omopsurvey-0.0.6/omopsurvey/samplefordummy.csv
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.6/omopsurvey/survey_key.csv
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.6/omopsurvey/tests/codebook_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.6/omopsurvey/tests/map_responses_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.6/omopsurvey/tests/pivot_data_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.6/omopsurvey/tests/recode_missing_test.py
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.6/omopsurvey/vignettes/example_basics.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.6/omopsurvey/vignettes/example_healthcare.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.6/omopsurvey/vignettes/example_sdoh.ipynb
+-rw-r--r--   0        0        0      722 2024-05-13 21:29:00.666148 omopsurvey-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 omopsurvey-0.0.6/PKG-INFO
```

### Comparing `omopsurvey-0.0.5/README.md` & `omopsurvey-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 The **'omopsurvey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
 ## response_set.py
+
 >
->**load_survey_data(filename='survey.csv')**: Loads survey data from a CSV file into a pandas DataFrame. This function takes an optional filename argument, which defaults to 'healthcare_survey.csv'. It constructs the file path by joining the current working directory with the specified filename. If the file does not exist at the constructed path, it raises a FileNotFoundError. Finally, it reads the CSV file into a DataFrame using pandas and returns this DataFrame.
->
->
->**map_responses(input_data)**: Maps numeric and text responses from a survey to their corresponding questions based on a preloaded survey data file. This function first calls load_survey_data() without arguments to load the default survey dataset. It then creates two mappings: one for numeric answers (mapping_numeric) and one for text answers (mapping_text), grouped by question_concept_id. 
->
->The function iterates over the input_data DataFrame, updating each row with the corresponding answer_numeric and answer_text based on the mappings. If an answer_text is numeric (detected as either int, float, or digit-containing string), it ensures the text remains as a string. The function returns the updated input_data DataFrame with the mapped answers.
->
+>**map_items(input_data)**: Maps survey responses to corresponding numeric and text labels based on predefined special cases and mappings defined in a loaded survey key. This function also handles survey responses that fall outside the predefined cases by attempting to fetch mappings from the loaded survey data.
+> Parameters: <input_data>: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
+> 
+> Returns: The modified DataFrame with added columns answer_numeric and answer_text containing the mapped values.
 >
->**create_dummies(input_data)**: Transforms responses from "select all that apply" questions in a survey dataset into individual rows for each selected answer. This function utilizes a preloaded question_key integrated within the package, which includes a select_all flag to identify questions that allow multiple answers. 
+>**create_dummies(input_data)**: create_dummies(user_data)
+Transforms survey data to include dummy variables for questions that allow multiple answers. Each response is converted into a separate row with a unique identifier, allowing for easier analysis in statistical software. 
+> 
+> Parameters: <user_data>: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
+> 
+> Returns: A new DataFrame with additional rows for select-all-that-apply questions, properly formatted for further analysis.
+> 
+>**scale(data, variables, scale_name)**: Transforms responses from "select all that apply" questions in a survey dataset into individual rows for each selected answer. This function utilizes a preloaded question_key integrated within the package, which includes a select_all flag to identify questions that allow multiple answers. 
 > 
 > Upon execution, the function identifies all "select all that apply" questions based on the select_all flag from the question_key. For each response to these questions in the user_data DataFrame, it creates a new row, modifying the question_concept_id to append the answer_concept_id. This adjustment effectively treats each answer as a unique sub-question, allowing for detailed data analysis of multi-select responses.
 > 
 > The function then removes the original rows corresponding to "select all" questions to prevent data redundancy. 
 > 
 ## pivot_data.py
 
 >
->**pivot_data_numeric(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
+>**pivot(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
 >
 >The column names are prefixed with 'q' to denote question IDs. The pivoted DataFrame is then saved to a new CSV file with a filename prefixed by 'pivot_n_'. The function concludes by printing the name of the newly saved file.
 >
->**pivot_data_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
+>**pivot_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
 >
 
 ## recode_missing.py
 >
->**recode_missing_values(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-999,..., -980]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
+>**recode(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-999,..., -980]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
 >
 
-## codebook.py
+## codebooks.py
 >
->**create_codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
+>**codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
 >
 >**print_codebook(codebook_df)**: Prints the provided codebook DataFrame in a readable format. It attempts to use the tabulate library to print the DataFrame with headers, formatted as an SQL-style table. If tabulate is not installed, it falls back to pandas' built-in printing options, adjusting the display settings to ensure that all data is visible without truncation. This function is useful for displaying the codebook in a terminal or other environments where a visual representation of the DataFrame is beneficial.
```

### Comparing `omopsurvey-0.0.5/omopsurvey/codebooks.py` & `omopsurvey-0.0.6/omopsurvey/codebooks.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/pivot_data.py` & `omopsurvey-0.0.6/omopsurvey/pivot_data.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/recode_missing.py` & `omopsurvey-0.0.6/omopsurvey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/response_set.py` & `omopsurvey-0.0.6/omopsurvey/response_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     file_path = os.path.join(current_dir, filename)
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File path {file_path} does not exist.")
     return pd.read_csv(file_path)
 
 
-def mapitems(input_data):
+def map_items(input_data):
     special_cases = {
         903087: (-999, "Don't Know"),
         903096: (-998, "Skip"),
         903072: (-997, "Does Not Apply To Me"),
         903079: (-996, "Prefer Not To Answer"),
         903070: (-995, "Other"),
         903092: (-994, "Not Sure"),
@@ -65,15 +65,15 @@
 
         if isinstance(input_data.at[idx, 'answer_text'], (int, float)):
             input_data.at[idx, 'answer_text'] = str(input_data.at[idx, 'answer_text'])
 
     return input_data
 
 
-def createdummies(user_data):
+def create_dummies(user_data):
     question_key = load_survey_data()
 
     select_all_questions = question_key[question_key['select_all'] == 1]['question_concept_id'].unique()
 
     new_rows = []
 
     for question_id in select_all_questions:
@@ -87,30 +87,100 @@
     new_rows_df = pd.DataFrame(new_rows)
     filtered_data = user_data[~user_data['question_concept_id'].isin(select_all_questions)]
     result_data = pd.concat([filtered_data, new_rows_df], ignore_index=True)
 
     return result_data
 
 
-def scale(data, variables, na=False, method='sum'):
+
+def scale(data, variables, score_name, na=False, method='sum'):
     df = data[['person_id'] + variables]
+
     if na:
         df['valid_count'] = df[variables].apply(lambda x: x[x >= 0].count(), axis=1)
         min_valid_count = len(variables) * 0.8
         df = df[df['valid_count'] >= min_valid_count]
     else:
         df = df.dropna(subset=variables)
         df = df[(df[variables] >= 0).all(axis=1)]
 
     if method == 'mean':
-        df['score'] = df[variables].mean(axis=1)
-        df['score'] = df[variables].sum(axis=1)
+        df[score_name] = df[variables].mean(axis=1)
+    elif method == 'sum':
+        df[score_name] = df[variables].sum(axis=1)
+
+    data = pd.merge(data, df[['person_id', score_name]], on='person_id', how='left')
 
-    data = pd.merge(data, df[['person_id', 'score']], on='person_id', how='left')
 
-    print('Minimum score calculated:', df['score'].min())
-    print('Maximum score calculated:', df['score'].max())
-    print('Number of person_ids with NaN assigned:', data['score'].isna().sum())
-    print('Number of person_ids with score calculated:', data['score'].notna().sum())
+    print('Minimum score calculated:', df[score_name].min())
+    print('Maximum score calculated:', df[score_name].max())
+    print('Number of person_ids with NaN assigned:', data[score_name].isna().sum())
+    print('Number of person_ids with score calculated:', data[score_name].notna().sum())
 
     return data
 
+
+def map_answers(input_data):
+    special_cases = {
+        903087: (-999, "Don't Know"),
+        903096: (-998, "Skip"),
+        903072: (-997, "Does Not Apply To Me"),
+        903079: (-996, "Prefer Not To Answer"),
+        903070: (-995, "Other"),
+        903092: (-994, "Not Sure"),
+        903095: (-993, "None"),
+        903103: (-992, "Unanswered"),
+        40192432: (-991, "I am not religious"),
+        40192487: (-990, "I do not believe in God (or a higher power)"),
+        40192520: (-989, "Does not apply to my neighborhood"),
+        903081: (-988, "Free Text"),
+        596889: (998, "Text"),
+        596883: (-994, "Not Sure"),
+        1332844: (-994, "Not Sure"),
+        903598: (-996, "Prefer Not To Answer"),
+        903596: (-996, "Prefer Not To Answer"),
+        903601: (-996, "Prefer Not To Answer"),
+        903607: (-996, "Prefer Not To Answer"),
+        903610: (-996, "Prefer Not To Answer"),
+        903604: (-996, "Prefer Not To Answer"),
+        43529089: (-997, "No Blood Related Daughters"),
+        43529086: (-997, "No Blood Related Siblings"),
+        43529092: (-997, "No Blood Related Sons"),
+        43529090: (-997, "No Daughters Related")
+    }
+
+    survey_data = load_survey_data()
+
+    mapping_numeric = survey_data.groupby('question_concept_id').apply(
+        lambda g: g.set_index('answer_concept_id')['answer_numeric'].to_dict()
+    ).to_dict()
+
+    mapping_text = survey_data.groupby('question_concept_id').apply(
+        lambda g: g.set_index('answer_concept_id')['answer_text'].str.strip().to_dict()
+    ).to_dict()
+
+    input_data['answer_numeric'] = pd.NA
+    input_data['answer_text'] = pd.NA
+
+    for answer_id, (num, text) in special_cases.items():
+        mask = input_data['answer_concept_id'] == answer_id
+        input_data.loc[mask, 'answer_numeric'] = num
+        input_data.loc[mask, 'answer_text'] = text
+
+    def apply_mappings(row):
+        if pd.notna(row['answer_numeric']) and pd.notna(row['answer_text']):
+            return row['answer_numeric'], row['answer_text']
+
+        question_id = row['question_concept_id']
+        answer_id = row['answer_concept_id']
+        numeric = mapping_numeric.get(question_id, {}).get(answer_id, pd.NA)
+        text = mapping_text.get(question_id, {}).get(answer_id, pd.NA)
+        return numeric, text
+
+    result = input_data.apply(apply_mappings, axis=1, result_type='expand')
+    input_data[['answer_numeric', 'answer_text']] = result
+
+    numeric_mask = pd.isna(input_data['answer_concept_id']) & input_data['answer'].apply(lambda x: str(x).isdigit())
+    input_data.loc[numeric_mask, 'answer_numeric'] = input_data.loc[numeric_mask, 'answer'].astype(int)
+    input_data.loc[numeric_mask, 'answer_text'] = input_data.loc[numeric_mask, 'answer'].astype(str)
+
+    return input_data
```

### Comparing `omopsurvey-0.0.5/omopsurvey/survey_key.csv` & `omopsurvey-0.0.6/omopsurvey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/vignettes/example_basics.ipynb` & `omopsurvey-0.0.6/omopsurvey/vignettes/example_basics.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/vignettes/example_healthcare.ipynb` & `omopsurvey-0.0.6/omopsurvey/vignettes/example_healthcare.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/omopsurvey/vignettes/example_sdoh.ipynb` & `omopsurvey-0.0.6/omopsurvey/vignettes/example_sdoh.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.5/pyproject.toml` & `omopsurvey-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omopsurvey"
-version = "0.0.5"
+version = "0.0.6"
 description = "The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omopsurvey.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `omopsurvey-0.0.5/PKG-INFO` & `omopsurvey-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omopsurvey
-Version: 0.0.5
+Version: 0.0.6
 Summary: The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omopsurvey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,42 +17,47 @@
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omopsurvey.git
 Description-Content-Type: text/markdown
 
 The **'omopsurvey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
 ## response_set.py
+
 >
->**load_survey_data(filename='survey.csv')**: Loads survey data from a CSV file into a pandas DataFrame. This function takes an optional filename argument, which defaults to 'healthcare_survey.csv'. It constructs the file path by joining the current working directory with the specified filename. If the file does not exist at the constructed path, it raises a FileNotFoundError. Finally, it reads the CSV file into a DataFrame using pandas and returns this DataFrame.
->
->
->**map_responses(input_data)**: Maps numeric and text responses from a survey to their corresponding questions based on a preloaded survey data file. This function first calls load_survey_data() without arguments to load the default survey dataset. It then creates two mappings: one for numeric answers (mapping_numeric) and one for text answers (mapping_text), grouped by question_concept_id. 
->
->The function iterates over the input_data DataFrame, updating each row with the corresponding answer_numeric and answer_text based on the mappings. If an answer_text is numeric (detected as either int, float, or digit-containing string), it ensures the text remains as a string. The function returns the updated input_data DataFrame with the mapped answers.
->
+>**map_items(input_data)**: Maps survey responses to corresponding numeric and text labels based on predefined special cases and mappings defined in a loaded survey key. This function also handles survey responses that fall outside the predefined cases by attempting to fetch mappings from the loaded survey data.
+> Parameters: <input_data>: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
+> 
+> Returns: The modified DataFrame with added columns answer_numeric and answer_text containing the mapped values.
 >
->**create_dummies(input_data)**: Transforms responses from "select all that apply" questions in a survey dataset into individual rows for each selected answer. This function utilizes a preloaded question_key integrated within the package, which includes a select_all flag to identify questions that allow multiple answers. 
+>**create_dummies(input_data)**: create_dummies(user_data)
+Transforms survey data to include dummy variables for questions that allow multiple answers. Each response is converted into a separate row with a unique identifier, allowing for easier analysis in statistical software. 
+> 
+> Parameters: <user_data>: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
+> 
+> Returns: A new DataFrame with additional rows for select-all-that-apply questions, properly formatted for further analysis.
+> 
+>**scale(data, variables, scale_name)**: Transforms responses from "select all that apply" questions in a survey dataset into individual rows for each selected answer. This function utilizes a preloaded question_key integrated within the package, which includes a select_all flag to identify questions that allow multiple answers. 
 > 
 > Upon execution, the function identifies all "select all that apply" questions based on the select_all flag from the question_key. For each response to these questions in the user_data DataFrame, it creates a new row, modifying the question_concept_id to append the answer_concept_id. This adjustment effectively treats each answer as a unique sub-question, allowing for detailed data analysis of multi-select responses.
 > 
 > The function then removes the original rows corresponding to "select all" questions to prevent data redundancy. 
 > 
 ## pivot_data.py
 
 >
->**pivot_data_numeric(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
+>**pivot(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
 >
 >The column names are prefixed with 'q' to denote question IDs. The pivoted DataFrame is then saved to a new CSV file with a filename prefixed by 'pivot_n_'. The function concludes by printing the name of the newly saved file.
 >
->**pivot_data_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
+>**pivot_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
 >
 
 ## recode_missing.py
 >
->**recode_missing_values(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-999,..., -980]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
+>**recode(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-999,..., -980]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
 >
 
-## codebook.py
+## codebooks.py
 >
->**create_codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
+>**codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
 >
 >**print_codebook(codebook_df)**: Prints the provided codebook DataFrame in a readable format. It attempts to use the tabulate library to print the DataFrame with headers, formatted as an SQL-style table. If tabulate is not installed, it falls back to pandas' built-in printing options, adjusting the display settings to ensure that all data is visible without truncation. This function is useful for displaying the codebook in a terminal or other environments where a visual representation of the DataFrame is beneficial.
```

