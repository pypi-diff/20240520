# Comparing `tmp/jzai-59.83.43.tar.gz` & `tmp/jzai-59.83.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.43.tar", last modified: Mon May 20 03:24:18 2024, max compression
+gzip compressed data, was "jzai-59.83.44.tar", last modified: Mon May 20 08:22:13 2024, max compression
```

## Comparing `jzai-59.83.43.tar` & `jzai-59.83.44.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.248667 jzai-59.83.43/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:24:18.246669 jzai-59.83.43/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.43/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.183178 jzai-59.83.43/jzai/
--rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.43/jzai/__init__.py
--rw-rw-rw-   0        0        0     8625 2024-05-20 03:23:03.000000 jzai-59.83.43/jzai/bot.py
--rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.43/jzai/cli.py
--rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.43/jzai/db.py
--rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.43/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:24:18.243667 jzai-59.83.43/jzai.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 03:24:18.000000 jzai-59.83.43/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 03:24:17.000000 jzai-59.83.43/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 03:24:18.249669 jzai-59.83.43/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-05-20 03:24:08.000000 jzai-59.83.43/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:13.761855 jzai-59.83.44/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:22:13.759852 jzai-59.83.44/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.44/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:13.740782 jzai-59.83.44/jzai/
+-rw-rw-rw-   0        0        0       58 2024-05-17 02:22:27.000000 jzai-59.83.44/jzai/__init__.py
+-rw-rw-rw-   0        0        0     9366 2024-05-20 08:20:05.000000 jzai-59.83.44/jzai/bot.py
+-rw-rw-rw-   0        0        0      179 2024-05-17 02:23:18.000000 jzai-59.83.44/jzai/cli.py
+-rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.44/jzai/db.py
+-rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.44/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:22:13.758855 jzai-59.83.44/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 08:22:13.000000 jzai-59.83.44/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:22:13.761855 jzai-59.83.44/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-20 08:22:10.000000 jzai-59.83.44/setup.py
```

### Comparing `jzai-59.83.43/jzai/bot.py` & `jzai-59.83.44/jzai/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,123 +6,127 @@
 import speech_recognition as sr
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
 from textblob import TextBlob
 import nltk
 import random
 import pwinput as pw
+import asyncio
+import aiofiles
 
 # Ensure necessary NLTK data is downloaded
-nltk.download('punkt')
-nltk.download('stopwords')
+nltk_data_path = 'nltk_data'
+if not os.path.exists(nltk_data_path):
+    nltk.download('punkt', download_dir=nltk_data_path)
+    nltk.download('stopwords', download_dir=nltk_data_path)
+nltk.data.path.append(nltk_data_path)
 
 class Bot:
     def __init__(self, name):
         self.name = name
         self.engine = pyttsx3.init()
         self.users = {}
         self.current_user = None
+        self.non_alpha_re = re.compile(r'[^a-zA-Z]')
         self.conversations = self.load_conversations("conversations.json")
+        self.preprocessed_questions = [(entry["question"], self.preprocess_text(entry["question"])) for entry in self.conversations]
 
     def preprocess_text(self, text):
         corrected_text = str(TextBlob(text).correct())
         tokens = word_tokenize(corrected_text)
         stop_words = set(stopwords.words('english'))
-        tokens = [re.sub(r'[^a-zA-Z]', '', token).lower() for token in tokens if token.lower() not in stop_words]
+        tokens = [self.non_alpha_re.sub('', token).lower() for token in tokens if token.lower() not in stop_words]
         tokens = [token for token in tokens if token]
         return tokens
 
     def generate_response(self, user_input):
         max_similarity = 0
         best_response = None
         if not self.conversations:
             return "I'm sorry, I don't have any conversations to reference."
         try:
-            for entry in self.conversations:
-                question = entry["question"]
-                question_tokens = self.preprocess_text(question)
-                user_input_tokens = self.preprocess_text(user_input)
+            user_input_tokens = self.preprocess_text(user_input)
+            for question, question_tokens in self.preprocessed_questions:
                 common_tokens = set(question_tokens) & set(user_input_tokens)
-                if len(question_tokens) == 0 or len(user_input_tokens) == 0:
-                    similarity = 0
-                else:
-                    similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
+                similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens)) if len(question_tokens) and len(user_input_tokens) else 0
                 if similarity > max_similarity:
                     max_similarity = similarity
-                    best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
+                    best_response = next(entry["answers"] for entry in self.conversations if entry["question"] == question)
             if best_response:
                 return random.choice(best_response)
             else:
                 return "I'm sorry, I didn't understand your question."
         except BaseException as e:
             return f"Error: {e}"
 
     def speak(self, text):
         try:
             self.engine.say(text)
             self.engine.runAndWait()
         except Exception as e:
             print(f"Error with TTS engine: {e}")
 
-    def load_users(self):
+    async def load_users(self):
         try:
-            with open("users.json", 'r') as file:
-                self.users = json.load(file)
+            async with aiofiles.open("users.json", 'r') as file:
+                self.users = json.loads(await file.read())
         except FileNotFoundError:
             pass
 
-    def save_users(self):
-        with open("users.json", 'w') as file:
-            json.dump(self.users, file, indent=4)
+    async def save_users(self):
+        async with aiofiles.open("users.json", 'w') as file:
+            await file.write(json.dumps(self.users, indent=4))
 
     def is_admin(self, username):
         if username in self.users:
             return self.users[username].get('is_admin', False)
         return False
 
     def edit_username(self, username, new_name):
         if username in self.users:
             self.users[username]['username'] = new_name
-            self.save_users()
+            asyncio.run(self.save_users())
             print(f"Username for {username} has been changed to {new_name}.")
         else:
             print("User not found.")
 
     def manage_chats(self, username):
         if self.is_admin(username):
             print("Admin access granted. You can manage chats here.")
         else:
             print("You do not have permission to manage chats.")
 
-    def load_chat_logs(self, username):
+    async def load_chat_logs(self, username):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
         if os.path.exists(chat_log_file):
-            with open(chat_log_file, 'r') as file:
+            async with aiofiles.open(chat_log_file, 'r') as file:
                 try:
-                    return json.load(file)
+                    return json.loads(await file.read())
                 except json.decoder.JSONDecodeError:
                     return []
         else:
             return []
 
-    def save_chat_log(self, username, chat_log):
+    async def save_chat_log(self, username, chat_log):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
-        with open(chat_log_file, 'w') as file:
-            json.dump(chat_log, file, indent=4)
+        async with aiofiles.open(chat_log_file, 'w') as file:
+            await file.write(json.dumps(chat_log, indent=4))
 
     def view_chat(self, username):
         chat_log_file = os.path.join("chat_logs", f"{username}.json")
         if os.path.exists(chat_log_file):
-            with open(chat_log_file, 'r') as file:
-                chat_log = json.load(file)
-                print(f"Chat log for {username}:")
-                for entry in chat_log:
-                    print(f"User: {entry['user']}")
-                    print(f"Bot: {entry['bot']}")
-                    print("-" * 20)
+            async def read_chat_log():
+                async with aiofiles.open(chat_log_file, 'r') as file:
+                    return json.loads(await file.read())
+            chat_log = asyncio.run(read_chat_log())
+            print(f"Chat log for {username}:")
+            for entry in chat_log:
+                print(f"User: {entry['user']}")
+                print(f"Bot: {entry['bot']}")
+                print("-" * 20)
         else:
             print(f"No chat log found for {username}.")
 
     def process_input(self, user_input):
         user_input_lower = user_input.lower()
         if user_input_lower == "login":
             self.login()
@@ -140,17 +144,17 @@
             else:
                 print("You do not have permission to view chats.")
         else:
             bot_response = self.generate_response(user_input)
             print(f"{self.name}: {bot_response}")
             self.speak(bot_response)
             if self.current_user:
-                chat_log = self.load_chat_logs(self.current_user)
+                chat_log = asyncio.run(self.load_chat_logs(self.current_user))
                 chat_log.append({'user': user_input, 'bot': bot_response})
-                self.save_chat_log(self.current_user, chat_log)
+                asyncio.run(self.save_chat_log(self.current_user, chat_log))
 
     def login(self):
         username = input("Username: ")
         password = pw.pwinput(prompt="Password: ", mask="*")
         password_hash = hashlib.sha256(password.encode()).hexdigest()
         if username in self.users and self.users[username]['password'] == password_hash:
             print(f"Welcome back, {username}!")
@@ -160,15 +164,15 @@
 
     def signup(self):
         username = input("Choose a username: ")
         password = pw.pwinput(prompt="Choose a password: ", mask="*")
         password_hash = hashlib.sha256(password.encode()).hexdigest()
         if username not in self.users:
             self.users[username] = {'password': password_hash}
-            self.save_users()
+            asyncio.run(self.save_users())
             print(f"Account created successfully for {username}.")
         else:
             print("Username already exists. Please choose another one.")
 
     def load_conversations(self, file_path):
         try:
             with open(file_path, 'r') as file:
@@ -189,32 +193,37 @@
             print(f"{self.current_user if self.current_user else 'You'}: {user_input}")
             self.process_input(user_input)
         except sr.UnknownValueError:
             print(f"{self.name}: Sorry, I could not understand your speech.")
         except sr.RequestError as e:
             print(f"{self.name}: Speech recognition request failed:", e)
 
-bot = Bot(name="JZ")
-bot.load_users()
-
-try:
-    while True:
-        if not bot.current_user:
-            user_choice = input("Do you want to (login) or (signup)? ")
-            if user_choice.lower() == "login":
-                bot.login()
-            elif user_choice.lower() == "signup":
-                bot.signup()
+def main():
+    bot = Bot(name="JZ")
+    asyncio.run(bot.load_users())
+
+    try:
+        while True:
+            if not bot.current_user:
+                user_choice = input("Do you want to (login) or (signup)? ")
+                if user_choice.lower() == "login":
+                    bot.login()
+                elif user_choice.lower() == "signup":
+                    bot.signup()
+                else:
+                    print("Invalid choice. Please enter 'login' or 'signup'.")
+                    continue
+            user_input = input(f"{bot.current_user if bot.current_user else 'You'}: ")
+            if user_input.lower() == 'exit':
+                break
+            if user_input.lower() == '/m':
+                bot.listen_for_input()
             else:
-                print("Invalid choice. Please enter 'login' or 'signup'.")
-                continue
-        user_input = input(f"{bot.current_user if bot.current_user else 'You'}: ")
-        if user_input.lower() == 'exit':
-            break
-        if user_input.lower() == '/m':
-            bot.listen_for_input()
-        else:
-            bot.process_input(user_input)
-except KeyboardInterrupt:
-    print("\nExiting...")
-finally:
-    bot.engine.stop()
+                bot.process_input(user_input)
+    except KeyboardInterrupt:
+        print("\nExiting...")
+    finally:
+        bot.engine.stop()
+
+if __name__ == "__main__":
+    import cProfile
+    cProfile.run('main()')
```

### Comparing `jzai-59.83.43/jzai/db.py` & `jzai-59.83.44/jzai/db.py`

 * *Files identical despite different names*

