# Comparing `tmp/jzai-59.83.42.tar.gz` & `tmp/jzai-59.83.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.42.tar", last modified: Mon May 20 03:17:51 2024, max compression
+gzip compressed data, was "jzai-59.83.43.tar", last modified: Mon May 20 03:24:18 2024, max compression
```

## Comparing `jzai-59.83.42.tar` & `jzai-59.83.43.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.235938 jzai-59.83.42/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:17:51.233255 jzai-59.83.42/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.42/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.185450 jzai-59.83.42/jzai/
--rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.42/jzai/__init__.py
--rw-rw-rw-   0        0        0     8770 2024-05-20 03:17:35.000000 jzai-59.83.42/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.42/jzai/cli.py
--rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.42/jzai/db.py
--rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.42/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:17:51.230842 jzai-59.83.42/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 03:17:51.000000 jzai-59.83.42/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 03:17:50.000000 jzai-59.83.42/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 03:17:51.235938 jzai-59.83.42/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-20 03:17:48.000000 jzai-59.83.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.248667 jzai-59.83.43/
+-rw-rw-rw-   0        0        0      226 2024-05-20 03:24:18.246669 jzai-59.83.43/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.43/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.183178 jzai-59.83.43/jzai/
+-rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.43/jzai/__init__.py
+-rw-rw-rw-   0        0        0     8625 2024-05-20 03:23:03.000000 jzai-59.83.43/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.43/jzai/cli.py
+-rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.43/jzai/db.py
+-rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.43/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.243667 jzai-59.83.43/jzai.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 03:24:18.000000 jzai-59.83.43/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 03:24:18.249669 jzai-59.83.43/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-05-20 03:24:08.000000 jzai-59.83.43/setup.py
```

### Comparing `jzai-59.83.42/jzai/bot.py` & `jzai-59.83.43/jzai/bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,70 +11,61 @@
 import random
 import pwinput as pw
 
 # Ensure necessary NLTK data is downloaded
 nltk.download('punkt')
 nltk.download('stopwords')
 
-
 class Bot:
     def __init__(self, name):
         self.name = name
         self.engine = pyttsx3.init()
         self.users = {}
         self.current_user = None
-        self.conversations = self.load_conversations("./conversations.json")
+        self.conversations = self.load_conversations("conversations.json")
 
     def preprocess_text(self, text):
-        # Correct spelling mistakes using TextBlob
         corrected_text = str(TextBlob(text).correct())
-
-        # Tokenization
         tokens = word_tokenize(corrected_text)
-
-        # Stopword removal and remove non-alphabetic characters
         stop_words = set(stopwords.words('english'))
         tokens = [re.sub(r'[^a-zA-Z]', '', token).lower() for token in tokens if token.lower() not in stop_words]
-
-        # Remove empty tokens
         tokens = [token for token in tokens if token]
-
         return tokens
 
     def generate_response(self, user_input):
         max_similarity = 0
         best_response = None
+        if not self.conversations:
+            return "I'm sorry, I don't have any conversations to reference."
         try:
             for entry in self.conversations:
                 question = entry["question"]
                 question_tokens = self.preprocess_text(question)
                 user_input_tokens = self.preprocess_text(user_input)
                 common_tokens = set(question_tokens) & set(user_input_tokens)
-
-                # Check for division by zero
                 if len(question_tokens) == 0 or len(user_input_tokens) == 0:
                     similarity = 0
                 else:
                     similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
-
                 if similarity > max_similarity:
                     max_similarity = similarity
                     best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
-
             if best_response:
                 return random.choice(best_response)
             else:
                 return "I'm sorry, I didn't understand your question."
-
         except BaseException as e:
             return f"Error: {e}"
 
     def speak(self, text):
-        self.engine.say(text)
-        self.engine.runAndWait()
+        try:
+            self.engine.say(text)
+            self.engine.runAndWait()
+        except Exception as e:
+            print(f"Error with TTS engine: {e}")
 
     def load_users(self):
         try:
             with open("users.json", 'r') as file:
                 self.users = json.load(file)
         except FileNotFoundError:
             pass
@@ -94,15 +85,14 @@
             self.save_users()
             print(f"Username for {username} has been changed to {new_name}.")
         else:
             print("User not found.")
 
     def manage_chats(self, username):
         if self.is_admin(username):
-            # Access all chat logs or perform other admin actions
             print("Admin access granted. You can manage chats here.")
         else:
             print("You do not have permission to manage chats.")
 
     def load_chat_logs(self, username):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
         if os.path.exists(chat_log_file):
@@ -110,16 +100,14 @@
                 try:
                     return json.load(file)
                 except json.decoder.JSONDecodeError:
                     return []
         else:
             return []
 
-
-
     def save_chat_log(self, username, chat_log):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
         with open(chat_log_file, 'w') as file:
             json.dump(chat_log, file, indent=4)
 
     def view_chat(self, username):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
@@ -137,15 +125,15 @@
     def process_input(self, user_input):
         user_input_lower = user_input.lower()
         if user_input_lower == "login":
             self.login()
         elif user_input_lower == "signup":
             self.signup()
         elif user_input_lower == "what's my name?":
-            print(f"Your name is {self.get_user_name()}.")
+            print(f"Your name is {self.current_user}.")
         elif user_input_lower.startswith("change my name to "):
             new_name = user_input[17:].strip()
             self.edit_username(self.current_user, new_name)
         elif user_input_lower.startswith("view chat log for "):
             username = user_input[18:].strip()
             if self.is_admin(self.current_user):
                 self.view_chat(username)
@@ -160,75 +148,73 @@
                 chat_log.append({'user': user_input, 'bot': bot_response})
                 self.save_chat_log(self.current_user, chat_log)
 
     def login(self):
         username = input("Username: ")
         password = pw.pwinput(prompt="Password: ", mask="*")
         password_hash = hashlib.sha256(password.encode()).hexdigest()
-
         if username in self.users and self.users[username]['password'] == password_hash:
             print(f"Welcome back, {username}!")
             self.current_user = username
         else:
             print("Invalid username or password.")
 
     def signup(self):
         username = input("Choose a username: ")
         password = pw.pwinput(prompt="Choose a password: ", mask="*")
         password_hash = hashlib.sha256(password.encode()).hexdigest()
-
         if username not in self.users:
             self.users[username] = {'password': password_hash}
             self.save_users()
             print(f"Account created successfully for {username}.")
         else:
             print("Username already exists. Please choose another one.")
 
     def load_conversations(self, file_path):
-        with open(file_path, 'r') as file:
-            return json.load(file)
+        try:
+            with open(file_path, 'r') as file:
+                return json.load(file)
+        except (FileNotFoundError, json.JSONDecodeError):
+            print(f"Error loading conversations from {file_path}")
+            return []
 
     def listen_for_input(self):
         recognizer = sr.Recognizer()
         with sr.Microphone() as source:
             print("Listening...")
-            recognizer.adjust_for_ambient_noise(source)  # Adjust microphone for ambient noise
-            audio = recognizer.listen(source)  # Listen for audio input
-
+            recognizer.adjust_for_ambient_noise(source)
+            audio = recognizer.listen(source)
         try:
             print("Recognizing...")
-            user_input = recognizer.recognize_google(audio)  # Recognize speech using Google Speech Recognition
-            print(f"{self.user_name if self.user_name else 'You'}: {user_input}")  # Print "You: " before the recognized user input
-            # Process the recognized user input here
+            user_input = recognizer.recognize_google(audio)
+            print(f"{self.current_user if self.current_user else 'You'}: {user_input}")
             self.process_input(user_input)
         except sr.UnknownValueError:
             print(f"{self.name}: Sorry, I could not understand your speech.")
         except sr.RequestError as e:
             print(f"{self.name}: Speech recognition request failed:", e)
 
-
 bot = Bot(name="JZ")
 bot.load_users()
 
 try:
     while True:
         if not bot.current_user:
             user_choice = input("Do you want to (login) or (signup)? ")
             if user_choice.lower() == "login":
                 bot.login()
             elif user_choice.lower() == "signup":
                 bot.signup()
             else:
                 print("Invalid choice. Please enter 'login' or 'signup'.")
                 continue
-
         user_input = input(f"{bot.current_user if bot.current_user else 'You'}: ")
         if user_input.lower() == 'exit':
             break
         if user_input.lower() == '/m':
             bot.listen_for_input()
         else:
             bot.process_input(user_input)
 except KeyboardInterrupt:
     print("\nExiting...")
 finally:
-    bot.engine.stop()
+    bot.engine.stop()
```

### Comparing `jzai-59.83.42/jzai/db.py` & `jzai-59.83.43/jzai/db.py`

 * *Files identical despite different names*

