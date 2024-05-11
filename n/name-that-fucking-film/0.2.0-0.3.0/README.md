# Comparing `tmp/name_that_fucking_film-0.2.0.tar.gz` & `tmp/name_that_fucking_film-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name_that_fucking_film-0.2.0.tar", max compression
+gzip compressed data, was "name_that_fucking_film-0.3.0.tar", max compression
```

## Comparing `name_that_fucking_film-0.2.0.tar` & `name_that_fucking_film-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1804 2024-05-09 19:44:12.204372 name_that_fucking_film-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.2.0/name_that_fucking_film/__init__.py
--rw-r--r--   0        0        0     8056 2024-05-09 21:49:28.935186 name_that_fucking_film-0.2.0/name_that_fucking_film/main.py
--rw-r--r--   0        0        0      397 2024-05-09 23:55:02.817411 name_that_fucking_film-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 name_that_fucking_film-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1722 2024-05-11 15:23:46.970929 name_that_fucking_film-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:14:37.807976 name_that_fucking_film-0.3.0/name_that_fucking_film/__init__.py
+-rw-r--r--   0        0        0    10239 2024-05-11 15:50:33.041350 name_that_fucking_film-0.3.0/name_that_fucking_film/name_that_fucking_film.py
+-rw-r--r--   0        0        0      608 2024-05-11 16:14:18.326155 name_that_fucking_film-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 name_that_fucking_film-0.3.0/PKG-INFO
```

### Comparing `name_that_fucking_film-0.2.0/README.md` & `name_that_fucking_film-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 git clone https://github.com/jkarenko/name-that-fucking-film.git
 cd name-that-fucking-film
 
 # Install dependencies using Poetry
 poetry install
 
 # run
-poetry run python name_that_fucking_film/main.py {path_to_dir_containing_resources}
+poetry run python name_that_fucking_film/name_that_fucking_film.py
 ```
 
 Or using PIP
 ```bash
 # Install from PyPI
 pip install name-that-fucking-film
 
 # Run
 name-that-fucking-film {path_to_dir_containing_resources}
 ```
 
-Download [resources.zip](https://www.dropbox.com/scl/fi/3p4r5drnp8s79lz7fmt8k/resources.zip?rlkey=hnubde0f9jadzthscimz2nx5b&st=54mjk0kb&dl=0) and unzip it somewhere convenient (e.g. `c:\name-that-fucking-film` or `~/name-that-fucking-film`)
+Download [resources.zip](https://www.dropbox.com/scl/fi/3p4r5drnp8s79lz7fmt8k/resources.zip?rlkey=hnubde0f9jadzthscimz2nx5b&st=54mjk0kb&dl=0) and unzip it in the project root,
 
 Zip file contains excerpts from https://www.kaggle.com/datasets/gufukuro/movie-scripts-corpus
 and https://github.com/chucknorris-io/swear-words/tree/master
```

### Comparing `name_that_fucking_film-0.2.0/name_that_fucking_film/main.py` & `name_that_fucking_film-0.3.0/name_that_fucking_film/name_that_fucking_film.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,32 @@
 import pathlib
 import re
 import sys
 from collections import Counter
 from random import choice
 
 import pandas as pd
+from nltk.stem import WordNetLemmatizer
 from rich.console import Console
 
+lemmatizer = WordNetLemmatizer()
+
 console = Console(highlight=False)
-resources_path = sys.argv[1]
+
+
+def resource_path(relative_path):
+    """ Get absolute path to resource, works for dev and for PyInstaller """
+    try:
+        base_path = sys._MEIPASS
+    except Exception:
+        base_path = os.path.abspath(".")
+    return os.path.join(base_path, relative_path)
+
+
+resources_path = resource_path('')
 
 
 def levenshtein(s1, s2):
     if len(s1) > len(s2):
         s1, s2 = s2, s1
     distances = range(len(s1) + 1)
     for i2, c2 in enumerate(s2):
@@ -46,20 +60,28 @@
     files = os.listdir(directory)
     return os.path.join(directory, choice(files))
 
 
 def count_words(file_path, swear_words):
     with open(file_path, 'r') as file:
         content = file.read().lower().split()
-    return {word: content.count(word) for word in swear_words}
+    content = [lemmatizer.lemmatize(word) for word in content if word.isalpha()]
+    swears = {word: content.count(word) for word in swear_words}
+    return Counter(swears).most_common(10)
 
 
 def get_most_common_words(file_path):
     with open(file_path, 'r') as file:
         content = file.read().lower().split()
+    content = [lemmatizer.lemmatize(word) for word in content if word.isalpha()]
+    content = [word for word in content if
+               word not in ['a', 'the', 'i', 'me', 'you', 'your', 'are', 'to', 'from', 'and', 'or', 'of', 'in',
+                            'as', 'that', 'he', 'him', 'his', 'she', 'her', 'hers', 'is', 'at', 'it', 'we',
+                            'us', 'they', 'them', 'on', 'with', '-', '--']]
+
     return Counter(content).most_common(10)
 
 
 def underscore_words(title):
     return re.sub(r'[A-Za-z]', '_', title)
 
 
@@ -82,90 +104,114 @@
 def play(score):
     filepath = get_random_filepath()
     imdb_url_id = pathlib.Path(filepath).name.split('_')[-1].split('.')[0]
     imdb_id = filepath.split('/')[-1].split('.')[0].split('_')[-1]
     imdb_id = int(imdb_id)
     meta_data = get_meta_data(imdb_id)
     title = meta_data['title'].iloc[0]
-    num_fucks = count_words(filepath, read_swears_file())
-    console.print("Naughty words used:", style="blue")
-    for word, count in num_fucks.items():
-        if count > 0:
-            print(f"{word}: {count}")
     underscored_title = underscore_words(title)
 
     letter_reveals = 0
     straws_used = set()
     while True:
         if title.lower() == underscored_title.lower():
             console.print("Aww shucks... You didn't quite guess the title.", style="bold yellow")
             calculated_score = 0
             break
-        calculated_score = score - [3 + x * 3 * len(straws_used) for x in range(0, len(straws_used))][-1] if straws_used else score
+        calculated_score = score - [3 + x * 3 * len(straws_used) for x in range(0, len(straws_used))][
+            -1] if straws_used else score
         calculated_score -= letter_reveals * 3
         console.print(f"\nTitle: {underscored_title}", style="green")
         guess = console.input(f"[green][Enter][/] to get random letter, "
                               f"[{'strike' if '1' in straws_used else 'green'}]1) Decade[/], "
                               f"[{'strike' if '2' in straws_used else 'green'}]2) Awards[/], "
                               f"[{'strike' if '3' in straws_used else 'green'}]3) Genre[/], "
                               f"[{'strike' if '4' in straws_used else 'green'}]4) Budget[/], "
                               f"[{'strike' if '5' in straws_used else 'green'}]5) Keywords[/], "
-                              f"[{'strike' if '6' in straws_used else 'green'}]6) Cast[/], "
-                              f"[{'strike' if '7' in straws_used else 'green'}]7) Common Words[/], "
+                              f"[{'strike' if '6' in straws_used else 'green'}]6) Taglines[/], "
+                              f"[{'strike' if '7' in straws_used else 'green'}]7) Cast[/], "
+                              f"[{'strike' if '8' in straws_used else 'green'}]8) Top-10 Words[/], "
+                              f"[{'strike' if '9' in straws_used else 'green'}]9) Top-10 Swears[/], "
                               f"[green]0) Give up[/] or guess a letter or the whole title\n[blue](Score: {calculated_score})>[/] ")
         try:
-            straws_used.add(guess) if int(guess) in list(range(0, 8)) else ""
+            straws_used.add(guess) if int(guess) in list(range(0, 10)) else ""
         except ValueError:
             pass
+
+        console.print("")
         match guess.lower():
             case "1":
-                console.print(str(meta_data['year'].iloc[0])[0:3] + "0", style="blue")
+                console.print("Decade of release", style="blue underline")
+                console.print(str(meta_data['year'].iloc[0])[0:3] + "0")
                 continue
             case "2":
-                console.print(re.sub(r'\b \d{4}\b', '', str(meta_data['awards'].iloc[0])), style="blue")
+                console.print("Awards received", style="blue underline")
+                console.print(re.sub(r'\b \d{4}\b', '', str(meta_data['awards'].iloc[0])))
                 continue
             case "3":
-                console.print(meta_data['genres'].iloc[0], style="blue")
+                console.print("Genres", style="blue underline")
+                console.print(meta_data['genres'].iloc[0])
                 continue
             case "4":
-                console.print(meta_data['budget'].iloc[0], style="blue")
+                console.print("Budget", style="blue underline")
+                console.print(meta_data['budget'].iloc[0])
                 continue
             case "5":
-                console.print(', '.join(meta_data['keywords'].iloc[0].split(',')[:5]), style="blue")
+                console.print("Keywords", style="blue underline")
+                console.print(', '.join(meta_data['keywords'].iloc[0].split(',')[:5]))
                 continue
             case "6":
-                console.print(', '.join(meta_data['cast'].iloc[0].split(',')[:3]), style="blue")
+                console.print("Taglines", style="blue underline")
+                console.print(', '.join(meta_data['taglines'].iloc[0].split(',')[:5]))
                 continue
             case "7":
-                console.print(', '.join(meta_data['cast'].iloc[0].split(',')[:3]), style="blue")
+                console.print(', '.join(meta_data['cast'].iloc[0].split(',')[:3]))
+                continue
+            case "8":
+                common_words = get_most_common_words(filepath)
+                common_words.sort(key=lambda x: x[1], reverse=True)
+                console.print("Top-10 words used:", style="blue underline")
+                for word, count in common_words:
+                    console.print(f"{word}: {count}")
+                continue
+            case "9":
+                swears = count_words(filepath, read_swears_file())
+                swears.sort(key=lambda x: x[1], reverse=True)
+                console.print("Top-10 Naughty Words Used:", style="blue underline")
+                for word, count in swears:
+                    if count > 0:
+                        console.print(f"{word}: {count}")
                 continue
             case "0":
                 score = 0
                 break
             case "":
-                console.print("Revealing a random letter...", style="green")
+                before = underscored_title + ''
                 underscored_title = reveal_letter(underscored_title, title)
-                letter_reveals += 2
+                letter = ''.join(set(underscored_title.upper()) - set(before.upper()))
+                console.print(f"Revealed letter [green]{letter}[/]", style="blue")
+                letter_reveals += 1
                 continue
             case _ if len(guess) == 1:
                 before = underscored_title + ''
                 underscored_title = reveal_letter(underscored_title, title, guess)
                 if before == underscored_title:
                     letter_reveals += 1
-                    console.print(f"No letter {guess} found.", style="green")
+                    console.print(f"No letter [green]{guess.upper()}[/] found.", style="yellow")
                 else:
-                    console.print(f"Revealing any letter {guess} in the title...", style="green")
+                    console.print(f"Revealing letter [green]{guess.upper()}[/] in the title...", style="blue")
                 continue
 
         if guess_title(guess, title):
             console.print("Congratulations! You guessed the title correctly!", style="bold green")
             break
 
         console.print(f"Your guess is {levenshtein(guess.lower(), title.lower())} changes off.", style="blue")
-        console.print(f"You have {count_same_letters(guess.lower(), title.lower())} of the correct letters.", style="blue")
+        console.print(f"You have {count_same_letters(guess.lower(), title.lower())} of the correct letters.",
+                      style="blue")
 
         # underscored_title = reveal_letters(underscored_title, title)
     console.print(f"\n[blue underline]Title:[/] '{title}' ({meta_data['year'].iloc[0]})", style="italic")
     console.print(f"[blue underline]IMDb Link:[/] https://www.imdb.com/title/tt{imdb_url_id}/", style="italic")
     console.print(f"[blue underline]Genres:[/] {meta_data['genres'].iloc[0]}", style="italic")
     console.print(f"[blue underline]Budget:[/] {meta_data['budget'].iloc[0]}", style="italic")
     console.print(f"[blue underline]Awards:[/] {meta_data['awards'].iloc[0]}", style="italic")
```

### Comparing `name_that_fucking_film-0.2.0/PKG-INFO` & `name_that_fucking_film-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: name-that-fucking-film
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: jkarenko
 Author-email: juho.karenko@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Name That Fucking Film
 
 A Python-based command-line game that challenges players to guess movie titles based on limited information and strategically revealed letters.
@@ -36,25 +36,25 @@
 git clone https://github.com/jkarenko/name-that-fucking-film.git
 cd name-that-fucking-film
 
 # Install dependencies using Poetry
 poetry install
 
 # run
-poetry run python name_that_fucking_film/main.py {path_to_dir_containing_resources}
+poetry run python name_that_fucking_film/name_that_fucking_film.py
 ```
 
 Or using PIP
 ```bash
 # Install from PyPI
 pip install name-that-fucking-film
 
 # Run
 name-that-fucking-film {path_to_dir_containing_resources}
 ```
 
-Download [resources.zip](https://www.dropbox.com/scl/fi/3p4r5drnp8s79lz7fmt8k/resources.zip?rlkey=hnubde0f9jadzthscimz2nx5b&st=54mjk0kb&dl=0) and unzip it somewhere convenient (e.g. `c:\name-that-fucking-film` or `~/name-that-fucking-film`)
+Download [resources.zip](https://www.dropbox.com/scl/fi/3p4r5drnp8s79lz7fmt8k/resources.zip?rlkey=hnubde0f9jadzthscimz2nx5b&st=54mjk0kb&dl=0) and unzip it in the project root,
 
 Zip file contains excerpts from https://www.kaggle.com/datasets/gufukuro/movie-scripts-corpus
 and https://github.com/chucknorris-io/swear-words/tree/master
```

