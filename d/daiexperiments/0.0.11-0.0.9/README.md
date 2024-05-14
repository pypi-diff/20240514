# Comparing `tmp/daiexperiments-0.0.11.tar.gz` & `tmp/daiexperiments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daiexperiments-0.0.11.tar", last modified: Tue May 14 06:16:52 2024, max compression
+gzip compressed data, was "daiexperiments-0.0.9.tar", last modified: Tue May 14 03:44:14 2024, max compression
```

## Comparing `daiexperiments-0.0.11.tar` & `daiexperiments-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:16:52.318527 daiexperiments-0.0.11/
--rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 daiexperiments-0.0.11/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 daiexperiments-0.0.11/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 daiexperiments-0.0.11/MANIFEST.in
--rw-rw-rw-   0        0        0      609 2024-05-14 06:16:52.317753 daiexperiments-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 daiexperiments-0.0.11/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 06:16:52.282997 daiexperiments-0.0.11/daiexperiments/
--rw-rw-rw-   0        0        0      354 2024-05-14 06:16:29.000000 daiexperiments-0.0.11/daiexperiments/__init__.py
--rw-rw-rw-   0        0        0    17248 2024-05-14 06:05:58.000000 daiexperiments-0.0.11/daiexperiments/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:16:52.307057 daiexperiments-0.0.11/daiexperiments.egg-info/
--rw-rw-rw-   0        0        0      609 2024-05-14 06:16:52.000000 daiexperiments-0.0.11/daiexperiments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-14 06:16:52.000000 daiexperiments-0.0.11/daiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:16:52.000000 daiexperiments-0.0.11/daiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 06:16:52.000000 daiexperiments-0.0.11/daiexperiments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 06:16:52.314855 daiexperiments-0.0.11/ishandaiexperiments.egg-info/
--rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 daiexperiments-0.0.11/ishandaiexperiments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 daiexperiments-0.0.11/ishandaiexperiments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 daiexperiments-0.0.11/ishandaiexperiments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 06:16:52.319026 daiexperiments-0.0.11/setup.cfg
--rw-rw-rw-   0        0        0      709 2024-05-14 06:16:39.000000 daiexperiments-0.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:44:14.536836 daiexperiments-0.0.9/
+-rw-rw-rw-   0        0        0       82 2024-05-13 17:39:14.000000 daiexperiments-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-05-13 17:40:13.000000 daiexperiments-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-13 17:39:48.000000 daiexperiments-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      608 2024-05-14 03:44:14.534484 daiexperiments-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-05-13 17:37:56.000000 daiexperiments-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:44:14.457671 daiexperiments-0.0.9/daiexperiments/
+-rw-rw-rw-   0        0        0      198 2024-05-14 03:44:10.000000 daiexperiments-0.0.9/daiexperiments/__init__.py
+-rw-rw-rw-   0        0        0    11776 2024-05-14 03:44:08.000000 daiexperiments-0.0.9/daiexperiments/main.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:44:14.519921 daiexperiments-0.0.9/daiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      608 2024-05-14 03:44:14.000000 daiexperiments-0.0.9/daiexperiments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-14 03:44:14.000000 daiexperiments-0.0.9/daiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:44:14.000000 daiexperiments-0.0.9/daiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 03:44:14.000000 daiexperiments-0.0.9/daiexperiments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:44:14.531303 daiexperiments-0.0.9/ishandaiexperiments.egg-info/
+-rw-rw-rw-   0        0        0      289 2024-05-13 20:00:47.000000 daiexperiments-0.0.9/ishandaiexperiments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:00:47.000000 daiexperiments-0.0.9/ishandaiexperiments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 20:00:47.000000 daiexperiments-0.0.9/ishandaiexperiments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 03:44:14.537789 daiexperiments-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-14 03:21:11.000000 daiexperiments-0.0.9/setup.py
```

### Comparing `daiexperiments-0.0.11/LICENSE.txt` & `daiexperiments-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daiexperiments-0.0.11/PKG-INFO` & `daiexperiments-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daiexperiments
-Version: 0.0.11
+Version: 0.0.9
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `daiexperiments-0.0.11/daiexperiments/main.py` & `daiexperiments-0.0.9/daiexperiments/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -54,78 +54,99 @@
             result[0][1]
             """
     return code
     
 def genetic_algorithm():
     code = """
             import numpy as np
-
-            # Parameters
             num_genes = 10
             population_size = 50
             mutation_rate = 0.01
             num_generations = 15
-
-            # Initialize population
             population = np.random.randint(0, 10, size=(population_size, num_genes))
+            print(population[:10])
 
-            # Define fitness function
-            def fitness(chromosome):
-                return -np.sum(chromosome)
-
-            # Evolution loop
+            def soft_tissue_characterization(chromosome):
+                return np.sum(chromosome)
+            def fitness_function(chromosome):
+                return -soft_tissue_characterization(chromosome)
+            
             for generation in range(num_generations):
-                fitness_values = [fitness(chromosome) for chromosome in population]
+                fitness_values = np.apply_along_axis(fitness_function, 1, population)
+
+
+                selected_indices = []
+                for _ in range(population_size):
+                    tournament_indices = np.random.choice(range(population_size), size=3, replace=False)
+                    tournament_fitness = fitness_values[tournament_indices]
+                    winner_index = tournament_indices[np.argmax(tournament_fitness)]
+                    selected_indices.append(winner_index)
+                selected_population = population[selected_indices]
+
 
-                # Select individuals for next generation
-                selected_indices = np.random.choice(range(population_size), size=population_size, replace=True)
-                population = population[selected_indices]
-
-                # Apply mutation
-                mutation_mask = np.random.random(size=population.shape) < mutation_rate
-                population ^= mutation_mask
+                crossover_points = np.random.randint(1, num_genes, size=population_size // 2)
+                offspring = np.empty_like(population)
+                for i in range(0, population_size, 2):
+                    parent1, parent2 = selected_population[i], selected_population[i + 1]
+                    crossover_point = crossover_points[i // 2]
+                    offspring[i, :] = np.concatenate((parent1[:crossover_point], parent2[crossover_point:]))
+                    offspring[i + 1, :] = np.concatenate((parent2[:crossover_point], parent1[crossover_point:]))
+
+
+                mutation_mask = np.random.random(size=offspring.shape) < mutation_rate
+                offspring ^= mutation_mask
+
+                population = offspring
 
                 best_fitness = np.max(fitness_values)
                 average_fitness = np.mean(fitness_values)
                 print(f"Generation {generation+1}, Best Fitness: {best_fitness}, Average Fitness: {average_fitness}")
 
                 best_solution_index = np.argmax(fitness_values)
                 best_solution = population[best_solution_index]
+                best_soft_tissue_characterization = soft_tissue_characterization(best_solution)
                 print("Best Solution:", best_solution)
-
+                print("Best Soft Tissue Characterization:", best_soft_tissue_characterization)
            """
     return code
 
 def face_detection():
     code = """
-            # library
+            pip install opencv-python
             import cv2
+            import numpy as np
+            import warnings
+            warnings.filterwarnings("ignore")
+            import matplotlib.pyplot as plt
+            import numpy as np
+            face_haar_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
+            cap = cv2.VideoCapture(0)
 
-            # open the image
-            img = cv2.imread('id.jpg')
-
-            # face cascade
-            face_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
-
-            # face detection function
-            def detect_face(img):
-                face_img = img.copy()
-                face_rects = face_cascade.detectMultiScale(face_img, scaleFactor=1.3, minNeighbors=3)
-                for (x,y,w,h) in face_rects:
-                    cv2.rectangle(face_img, (x,y), (x+w,y+h), (0,0,255), 2)
-                return face_img
+            while True:
+                ret, test_img = cap.read()  # captures frame and returns boolean value and captured image
+                if not ret:
+                    continue
+                gray_img = cv2.cvtColor(test_img, cv2.COLOR_BGR2RGB)
+
+                faces_detected = face_haar_cascade.detectMultiScale(gray_img, 1.32, 5)
+
+                for (x, y, w, h) in faces_detected:
+                    cv2.rectangle(test_img, (x, y), (x + w, y + h), (255, 0, 0), thickness=7)
+                    roi_gray = gray_img[y:y + w, x:x + h]  # cropping region of interest i.e. face area from  image
+                    roi_gray = cv2.resize(roi_gray, (224, 224))
+                    cv2.putText(test_img, "Face Detected " , (int(x), int(y)), cv2.FONT_HERSHEY_SIMPLEX, 1, (0, 0, 255), 2)
 
-            # apply the face detection function
-            face_img = detect_face(img)
+                resized_img = cv2.resize(test_img, (1000, 700))
+                cv2.imshow('Facial emotion analysis ', resized_img)
 
+                if cv2.waitKey(10) == ord('q'):  # wait until 'q' key is pressed
+                    break
 
-            import matplotlib.pyplot as plt
-            # display the result
-            face_img_np = np.array(face_img)
-            plt.imshow(face_img_np)
+            cap.release()
+            cv2.destroyAllWindows
             """
     return code
 
 def three_cross_three_grid():
     code = """
             import numpy as np
 
@@ -264,212 +285,8 @@
                     next_state, reward, done, _ = env.step(action)
                     total_rewards += reward
                     state = next_state
 
             avg_reward = total_rewards / num_test_episodes
             print(f"Average reward over {num_test_episodes} test episodes: {avg_reward}")
            """
-    return code
-
-def magic_square():
-    code = """
-            import random
-
-            def create_magic_square():
-            
-                nums = list(range(1, 10))
-                random.shuffle(nums)
-                square = []
-                for i in range(0, 9, 3):
-                    square.append(nums[i:i+3])
-
-                return square
-
-            def is_magic_square(square):
-
-                target_sum = sum(square[0])  # Sum of the first row
-
-                # Check rows
-                for row in square:
-                    if sum(row) != target_sum:
-                        return False
-
-                # Check columns
-                for col in range(3):
-                    if sum(row[col] for row in square) != target_sum:
-                        return False
-
-                # Check diagonals
-                if sum(square[i][i] for i in range(3)) != target_sum:
-                    return False
-                if sum(square[i][2-i] for i in range(3)) != target_sum:
-                    return False
-
-                return True
-
-            def play_game():
-            
-                print("Welcome to the 3x3 Magic Square Game!")
-                square = create_magic_square()
-                print("Here's the initial square:")
-                for row in square:
-                    print(row)
-
-                while True:
-                    row1, col1, row2, col2 = map(int, input("Enter the indices of the two numbers you want to swap (row1 col1 row2 col2): ").split())
-                    row1 -= 1
-                    col1 -= 1
-                    row2 -= 1
-                    col2 -= 1
-
-                    if (
-                        row1 < 0 or row1 > 2 or col1 < 0 or col1 > 2 or
-                        row2 < 0 or row2 > 2 or col2 < 0 or col2 > 2
-                    ):
-                        print("Invalid indices. Try again.")
-                        continue
-
-                    square[row1][col1], square[row2][col2] = square[row2][col2], square[row1][col1]
-
-                    print("Updated square:")
-                    for row in square:
-                        print(row)
-
-                    if is_magic_square(square):
-                        print("Congratulations! You have created a magic square!")
-                        break
-
-                    print("Keep trying!")
-
-            play_game()
-           """
-    return code
-
-def genetic_algorithm_meghs():
-    code = """
-            import gym
-            import numpy as np
-
-            # Create FrozenLake environment
-            env = gym.make("FrozenLake-v1")
-
-            # Initialize Q-table
-            num_states = env.observation_space.n
-            num_actions = env.action_space.n
-            Q = np.zeros((num_states, num_actions))
-
-            # Q-learning parameters
-            alpha = 0.8  # Learning rate
-            gamma = 0.95  # Discount factor
-            epsilon = 0.1  # Exploration rate
-
-            # Q-learning algorithm
-            num_episodes = 10000
-            for episode in range(num_episodes):
-                state = env.reset()
-                done = False
-                while not done:
-                    # Choose action
-                    if np.random.uniform(0, 1) < epsilon:
-                        action = env.action_space.sample()  # Explore
-                    else:
-                        action = np.argmax(Q[state])  # Exploit
-
-                    # Take action
-                    next_state, reward, done, _ = env.step(action)
-
-                    # Update Q-table
-                    Q[state, action] += alpha * (reward + gamma * np.max(Q[next_state]) - Q[state, action])
-
-                    state = next_state
-
-            # Print the Q-table
-            print("Q-table:")
-            print(Q)
-
-            # Test the trained agent
-            num_test_episodes = 10
-            total_rewards = 0
-            for _ in range(num_test_episodes):
-                state = env.reset()
-                done = False
-                while not done:
-                    action = np.argmax(Q[state])
-                    next_state, reward, done, _ = env.step(action)
-                    total_rewards += reward
-                    state = next_state
-
-            avg_reward = total_rewards / num_test_episodes
-            print(f"Average reward over {num_test_episodes} test episodes: {avg_reward}")
-           """
-    
-def least_square_regression():
-    code = """
-            # Importing necessary libraries
-            import numpy as np
-            from sklearn.model_selection import train_test_split
-            from sklearn.linear_model import LinearRegression
-            from sklearn.metrics import mean_squared_error
-
-            # Generating some sample data
-            np.random.seed(0)
-            X = 2 * np.random.rand(100, 1)  # Generating 100 random numbers between 0 and 2
-            y = 4 + 3 * X + np.random.randn(100, 1)  # Linear equation with some noise
-
-            # Splitting the data into training and testing sets
-            X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
-
-            # Creating a linear regression model
-            model = LinearRegression()
-
-            # Fitting the model to the training data
-            model.fit(X_train, y_train)
-
-            # Making predictions on the testing data
-            y_pred = model.predict(X_test)
-
-            # Calculating the mean squared error
-            mse = mean_squared_error(y_test, y_pred)
-            print("Mean Squared Error:", mse)
-           """
-    return code
-
-def k_means_clustering():
-
-    code = '''
-            from sklearn.datasets import load_iris
-            import pandas as pd
-            from sklearn.model_selection import train_test_split
-            import matplotlib.pyplot as plt
-            from sklearn.cluster import KMeans
-
-            # Load iris dataset
-            iris = load_iris()
-            df = pd.DataFrame(iris.data, columns=iris.feature_names)
-            y = iris.target
-
-            # Concatenate features and labels
-            data = pd.concat([df, pd.Series(y, name='label')], axis=1)
-
-            inertias = []
-            for i in range(1, 11):
-                kmeans = KMeans(n_clusters=i)
-                kmeans.fit(data)
-                inertias.append(kmeans.inertia_)
-
-            plt.plot(range(1, 11), inertias, marker='o')
-            plt.title('Elbow method')
-            plt.xlabel('Number of clusters')
-            plt.ylabel('Inertia')
-            plt.show()
-            kmeans = KMeans(n_clusters=3)
-            kmeans.fit(data)
-
-            plt.scatter(df.iloc[:, 0], df.iloc[:, 1], c=kmeans.labels_, cmap='viridis')
-            centers = kmeans.cluster_centers_
-            plt.scatter(centers[:, 0], centers[:, 1], c='red', s=200, alpha=0.5) 
-            plt.xlabel(iris.feature_names[0])
-            plt.ylabel(iris.feature_names[1])
-            plt.title('KMeans Clustering')
-            plt.show()
-           '''
     return code
```

### Comparing `daiexperiments-0.0.11/daiexperiments.egg-info/PKG-INFO` & `daiexperiments-0.0.9/daiexperiments.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daiexperiments
-Version: 0.0.11
+Version: 0.0.9
 Summary: dai experiments
 Home-page: 
 Author: S Ishan
 Author-email: is9678@srmist.edu.in
 License: MIT
 Keywords: dai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `daiexperiments-0.0.11/setup.py` & `daiexperiments-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='daiexperiments',
-  version='0.0.11',
+  version='0.0.9',
   description='dai experiments',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='S Ishan',
   author_email='is9678@srmist.edu.in',
   license='MIT', 
   classifiers=classifiers,
```

