# Comparing `tmp/linkedin_user_scrape-1.0.4.tar.gz` & `tmp/linkedin_user_scrape-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_user_scrape-1.0.4.tar", last modified: Tue May 14 13:18:48 2024, max compression
+gzip compressed data, was "linkedin_user_scrape-1.0.5.tar", last modified: Tue May 14 17:16:47 2024, max compression
```

## Comparing `linkedin_user_scrape-1.0.4.tar` & `linkedin_user_scrape-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:18:48.694095 linkedin_user_scrape-1.0.4/
--rw-r--r--   0 harikabv   (501) staff       (20)      392 2024-05-14 13:18:48.693880 linkedin_user_scrape-1.0.4/PKG-INFO
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:18:48.692803 linkedin_user_scrape-1.0.4/linkedin_user_scrape/
--rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape/__init__.py
--rw-r--r--   0 harikabv   (501) staff       (20)     7464 2024-05-14 11:30:25.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape/scraper.py
--rw-r--r--   0 harikabv   (501) staff       (20)     1601 2024-05-14 11:28:22.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape/utils.py
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:18:48.693677 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/
--rw-r--r--   0 harikabv   (501) staff       (20)      392 2024-05-14 13:18:48.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/PKG-INFO
--rw-r--r--   0 harikabv   (501) staff       (20)      322 2024-05-14 13:18:48.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 13:18:48.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       24 2024-05-14 13:18:48.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/requires.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 13:18:48.000000 linkedin_user_scrape-1.0.4/linkedin_user_scrape.egg-info/top_level.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 13:18:48.694145 linkedin_user_scrape-1.0.4/setup.cfg
--rw-r--r--   0 harikabv   (501) staff       (20)      524 2024-05-14 13:18:38.000000 linkedin_user_scrape-1.0.4/setup.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.229719 linkedin_user_scrape-1.0.5/
+-rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-14 17:16:47.229498 linkedin_user_scrape-1.0.5/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)     1802 2024-05-14 17:09:46.000000 linkedin_user_scrape-1.0.5/README.md
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.228363 linkedin_user_scrape-1.0.5/linkedin_user_scrape/
+-rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/__init__.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     9913 2024-05-14 17:08:58.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/scraper.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     3368 2024-05-14 16:36:09.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/utils.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.229286 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/
+-rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)      332 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       24 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/requires.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/top_level.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 17:16:47.229774 linkedin_user_scrape-1.0.5/setup.cfg
+-rw-r--r--   0 harikabv   (501) staff       (20)      844 2024-05-14 17:12:34.000000 linkedin_user_scrape-1.0.5/setup.py
```

### Comparing `linkedin_user_scrape-1.0.4/linkedin_user_scrape/scraper.py` & `linkedin_user_scrape-1.0.5/linkedin_user_scrape/scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,74 @@
-from bs4 import BeautifulSoup
+import re
 from .utils import *
+from bs4 import BeautifulSoup
 
-def getUserBasicDetails(driver, userId):
-    if(not driver):
-        driver = getWebDriver(cookie, email, password)
-    
-    url = f"https://www.linkedin.com/in/{userId}"
-    src = getDriverData(driver, url)
-    
-    soup = BeautifulSoup(src, 'lxml')
+def get_user_basic_details(driver, user_id, cookie, email, password):
+    """
+    Retrieves basic user details from a LinkedIn profile using the provided WebDriver.
+
+    Args:
+        driver (WebDriver): An instance of the WebDriver.
+        user_id (str): The user's LinkedIn ID.
+        cookie (str) : li_at linkedin cookie
+        email (str) : Email address for linkedin login
+        password (str) : Password for linkedin login
+
+
+    Returns:
+        dict: A dictionary containing the user's basic details (name, title, summary, location).
+    """
 
-    try:
-        name = soup.find('h1', {'class': 'text-heading-xlarge inline t-24 v-align-middle break-words'}).text.strip()
-    except Exception as e:
-        name = ""
-    
-    try:
-        title = soup.find('div', {'class': 'text-body-medium break-words'}).text.strip()
-    except Exception as e:
-        title = ""
-
-    try:
-        summary = soup.find('div', {'class':'display-flex ph5 pv3'}).text.strip()
-    except Exception as e:
-        summary = ""
-
-    try:
-        location = soup.find('span', {'class' : 'text-body-small inline t-black--light break-words'}).text.strip()
-    except Exception as e:
-        location = ""
+    if not driver:
+        driver = get_webdriver(cookie, email, password)
 
-    return {
-        "Name" : name,
-        "Title" : title,
-        "Summary" : summary,
-        "Location" : location
+    url = f"https://www.linkedin.com/in/{user_id}"
+    src = get_driver_data(driver, url)
+    soup = BeautifulSoup(src, 'lxml')
+
+    details = {}
+    selectors = {
+        "name": 'h1',
+        "title": 'div',
+        "summary": 'div',
+        "location": 'span'
     }
+    classes = {
+        "name": {'class': 'text-heading-xlarge inline t-24 v-align-middle break-words'},
+        "title": {'class': 'text-body-medium break-words'},
+        "summary": {'class': 'display-flex ph5 pv3'},
+        "location": {'class': 'text-body-small inline t-black--light break-words'}
+    }
+
+    for field, selector in selectors.items():
+        try:
+            element = soup.find(selector, attrs=classes.get(field))
+            details[field] = element.text.strip() if element else ""
+        except Exception as e:
+            details[field] = ""
+
+    return details
+
+def get_work_experience_detais(driver, userId, cookie, email, password):
+    """
+    Retrieves work experience details from a LinkedIn profile using the provided WebDriver.
+
+    Args:
+        driver (WebDriver): An instance of the WebDriver.
+        user_id (str): The user's LinkedIn ID.
+
+    Returns:
+        list: A list of dictionaries, each containing work experience details (title, company, duration, summary).
+    """
 
-def getWorkExperienceDetails(driver, userId):
     if(not driver):
-        driver = getWebDriver(cookie, email, password)
+        driver = get_webdriver(cookie, email, password)
     
     url = f"https://www.linkedin.com/in/{userId}/details/experience"
-    src = getDriverData(driver, url)
+    src = get_driver_data(driver, url)
     
     soup = BeautifulSoup(src, 'lxml')
     
     soup = BeautifulSoup(src, 'html.parser')
     container_div = soup.find('div', class_='pvs-list__container')
     companyCache = ""
 
@@ -107,32 +129,41 @@
                     }]
                 )
             else:
                 companyCache = titleUnique
 
     return workExperience
 
-def getEducationDetails(driver, userId):
+def get_education_details(driver, userId, cookie, email, password):
+    """
+    Retrieves education details from a LinkedIn profile using the provided WebDriver (if credentials provided) or potentially cached data (if cookie provided).
+
+    Args:
+        driver (Optional[WebDriver]): An instance of the WebDriver (used if no cookie provided). Defaults to None.
+        user_id (str): The user's LinkedIn ID.
+        cookie (Optional[str]): A valid LinkedIn session cookie for the target user (avoids login if provided). Defaults to None.
+        email (Optional[str]): The user's email address (required for login if no cookie provided). Defaults to None.
+        password (Optional[str]): The user's password (required for login if no cookie provided). Defaults to None.
+
+    Returns:
+        List[Dict]: A list of dictionaries, each containing education details (institute, course, duration, summary).
+    """
     education = []
     if(not driver):
-        driver = getWebDriver(cookie, email, password)
+        driver = get_webdriver(cookie, email, password)
     
     url = f"https://www.linkedin.com/in/{userId}/details/education"
-    src = getDriverData(driver, url)
-    
-    soup = BeautifulSoup(src, 'lxml')
+    src = get_driver_data(driver, url)
     
     soup = BeautifulSoup(src, 'html.parser')
     container_div = soup.find('div', class_='pvs-list__container')
 
     if container_div:
   
         list_items = container_div.find_all('div', class_='display-flex flex-column full-width align-self-center')
-        cleaned_list = []
-        # Loop through each 'li' element
         for item in list_items:
 
             try: 
                 edu_details = item.find('div', {'class': 'display-flex flex-row justify-space-between'})
                 
                 try:
                     institute = edu_details.find('div', {'class' : 'display-flex align-items-center mr1 hoverable-link-text t-bold'})
@@ -162,50 +193,56 @@
                 summaryDetails = ""
 
             summaryDetailsData = ""
             for data in summaryDetails:
                 summaryDetailsData = summaryDetailsData + " " + data.text.strip()
             
             education.append([
-                    {
-                        "Institute" : instituteDetails,
-                        "Course" : courseDetails,
-                        "Duration" : duration,
-                        "Summary" : summaryDetailsData
-                    }]
-                )
+                {
+                    "Institute" : instituteDetails,
+                    "Course" : courseDetails,
+                    "Duration" : duration,
+                    "Summary" : summaryDetailsData
+                }]
+            )
     return education
 
-def getProjectDetails(driver, userId):
+def get_project_details(driver, userId, cookie, email, password):
     projects = []
     return projects
 
-def getRecommendations(driver, userId):
+def get_recommendations(driver, userId, cookie, email, password):
     recommendations = []
 
     return recommendations
 
-def getUserProfileData(userId, cookie, email, password):
-    driver = getWebDriver(cookie, email, password)
-
-    # Get Basic Details
-    basic_details = getUserBasicDetails(driver, userId)
-
-    # Get Work Experience
-    work_experience_details = getWorkExperienceDetails(driver, userId)
-
-    # Get Education
-    education_details = getEducationDetails(driver, userId)
-
-    # Get Projects
-    projects_details = getProjectDetails(driver, userId)
-
-    # Get Recommendations
-    recommendations = getRecommendations(driver, userId)
+def get_user_profile_data(userId, cookie, email, password):
+    """
+    Retrieves user profile data from LinkedIn using a WebDriver (if credentials provided) or a cached version (if cookie provided).
+
+    Args:
+        user_id (str): The user's LinkedIn ID.
+        cookie (str, optional): A valid LinkedIn session cookie for the target user (avoids login if provided). Defaults to None.
+        email (str, optional): The user's email address (required for login if no cookie provided). Defaults to None.
+        password (str, optional): The user's password (required for login if no cookie provided). Defaults to None.
+
+    Returns:
+        dict: A dictionary containing user profile data with sections for basic details, work experience, education, projects, and recommendations.
+    """
+
+    driver = get_webdriver(cookie, email, password)
+
+    basic_details = get_user_basic_details(driver, userId, cookie, email, password)
+    work_experience_details = get_work_experience_detais(driver, userId, cookie, email, password)
+    education_details = get_education_details(driver, userId, cookie, email, password)
+    projects_details = get_project_details(driver, userId, cookie, email, password)
+    recommendations = get_recommendations(driver, userId, cookie, email, password)
 
+    if driver:
+        driver.quit()
 
     return {
         "Basic Details" : basic_details,
         "Work Experience Details" : work_experience_details,
         "Education Details" : education_details,
         "Project Details" : projects_details,
         "Recommendations" : recommendations
```

### Comparing `linkedin_user_scrape-1.0.4/setup.py` & `linkedin_user_scrape-1.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='linkedin_user_scrape',
-    version='1.0.4',
+    version='1.0.5',
     author='Harika B V',
     author_email='harikabv.dev@gmail.com',
     description='LinkedIn scraper to parse user profiles',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     install_requires=[
         'selenium',
         'beautifulsoup4'
     ],
     python_requires='>=3.6',
+    project_urls = {
+        'Home page' : 'https://github.com/Harika-BV/LinkedIn-User-Scraper',
+    },
+    long_description=long_description,
+    long_description_content_type='text/markdown',
 )
```

