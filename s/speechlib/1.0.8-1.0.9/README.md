# Comparing `tmp/speechlib-1.0.8.tar.gz` & `tmp/speechlib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\speechlib-1.0.8.tar", last modified: Mon Jan 22 11:40:15 2024, max compression
+gzip compressed data, was "dist\speechlib-1.0.9.tar", last modified: Mon Jan 22 13:20:55 2024, max compression
```

## Comparing `speechlib-1.0.8.tar` & `speechlib-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-01-22 11:40:15.083425 speechlib-1.0.8/
--rw-rw-rw-   0        0        0     6823 2024-01-22 11:40:15.082213 speechlib-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6106 2024-01-22 11:37:45.000000 speechlib-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-01-22 11:40:15.083425 speechlib-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1025 2024-01-22 11:12:11.000000 speechlib-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-22 11:40:15.065839 speechlib-1.0.8/speechlib/
--rw-rw-rw-   0        0        0       65 2024-01-19 11:15:11.000000 speechlib-1.0.8/speechlib/__init__.py
--rw-rw-rw-   0        0        0     1202 2023-10-02 00:51:33.000000 speechlib-1.0.8/speechlib/convert_to_mono.py
--rw-rw-rw-   0        0        0      611 2024-01-22 10:35:56.000000 speechlib-1.0.8/speechlib/convert_to_wav.py
--rw-rw-rw-   0        0        0     4701 2024-01-22 10:36:43.000000 speechlib-1.0.8/speechlib/core_analysis.py
--rw-rw-rw-   0        0        0       52 2024-01-07 16:08:30.000000 speechlib-1.0.8/speechlib/hf_access.py
--rw-rw-rw-   0        0        0     1296 2023-10-02 00:51:35.000000 speechlib-1.0.8/speechlib/re_encode.py
--rw-rw-rw-   0        0        0      256 2024-01-08 18:26:03.000000 speechlib-1.0.8/speechlib/run.py
--rw-rw-rw-   0        0        0     2839 2024-01-22 09:30:21.000000 speechlib-1.0.8/speechlib/speaker_recognition.py
--rw-rw-rw-   0        0        0     5396 2024-01-22 10:45:48.000000 speechlib-1.0.8/speechlib/speechlib.py
--rw-rw-rw-   0        0        0     1283 2024-01-22 10:26:00.000000 speechlib-1.0.8/speechlib/transcribe.py
--rw-rw-rw-   0        0        0     1125 2024-01-19 10:59:16.000000 speechlib-1.0.8/speechlib/wav_segmenter.py
--rw-rw-rw-   0        0        0      222 2024-01-19 11:44:23.000000 speechlib-1.0.8/speechlib/whisper_sinhala.py
--rw-rw-rw-   0        0        0      755 2024-01-22 09:11:36.000000 speechlib-1.0.8/speechlib/write_log_file.py
-drwxrwxrwx   0        0        0        0 2024-01-22 11:40:15.082213 speechlib-1.0.8/speechlib.egg-info/
--rw-rw-rw-   0        0        0     6823 2024-01-22 11:40:14.000000 speechlib-1.0.8/speechlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2024-01-22 11:40:14.000000 speechlib-1.0.8/speechlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-22 11:40:14.000000 speechlib-1.0.8/speechlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-01-22 11:40:14.000000 speechlib-1.0.8/speechlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-22 11:40:14.000000 speechlib-1.0.8/speechlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-22 13:20:55.881609 speechlib-1.0.9/
+-rw-rw-rw-   0        0        0     7093 2024-01-22 13:20:55.881609 speechlib-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6481 2024-01-22 13:18:53.000000 speechlib-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-01-22 13:20:55.881609 speechlib-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2024-01-22 12:46:28.000000 speechlib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-22 13:20:55.865558 speechlib-1.0.9/speechlib/
+-rw-rw-rw-   0        0        0       65 2024-01-19 11:15:11.000000 speechlib-1.0.9/speechlib/__init__.py
+-rw-rw-rw-   0        0        0     1202 2023-10-02 00:51:33.000000 speechlib-1.0.9/speechlib/convert_to_mono.py
+-rw-rw-rw-   0        0        0      611 2024-01-22 10:35:56.000000 speechlib-1.0.9/speechlib/convert_to_wav.py
+-rw-rw-rw-   0        0        0     4735 2024-01-22 12:37:23.000000 speechlib-1.0.9/speechlib/core_analysis.py
+-rw-rw-rw-   0        0        0       52 2024-01-07 16:08:30.000000 speechlib-1.0.9/speechlib/hf_access.py
+-rw-rw-rw-   0        0        0     1296 2023-10-02 00:51:35.000000 speechlib-1.0.9/speechlib/re_encode.py
+-rw-rw-rw-   0        0        0      256 2024-01-08 18:26:03.000000 speechlib-1.0.9/speechlib/run.py
+-rw-rw-rw-   0        0        0     2839 2024-01-22 09:30:21.000000 speechlib-1.0.9/speechlib/speaker_recognition.py
+-rw-rw-rw-   0        0        0     5700 2024-01-22 12:50:45.000000 speechlib-1.0.9/speechlib/speechlib.py
+-rw-rw-rw-   0        0        0     1506 2024-01-22 12:55:51.000000 speechlib-1.0.9/speechlib/transcribe.py
+-rw-rw-rw-   0        0        0     1153 2024-01-22 12:36:34.000000 speechlib-1.0.9/speechlib/wav_segmenter.py
+-rw-rw-rw-   0        0        0      222 2024-01-19 11:44:23.000000 speechlib-1.0.9/speechlib/whisper_sinhala.py
+-rw-rw-rw-   0        0        0      830 2024-01-22 12:01:35.000000 speechlib-1.0.9/speechlib/write_log_file.py
+drwxrwxrwx   0        0        0        0 2024-01-22 13:20:55.878829 speechlib-1.0.9/speechlib.egg-info/
+-rw-rw-rw-   0        0        0     7093 2024-01-22 13:20:55.000000 speechlib-1.0.9/speechlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-01-22 13:20:55.000000 speechlib-1.0.9/speechlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-22 13:20:55.000000 speechlib-1.0.9/speechlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-01-22 13:20:55.000000 speechlib-1.0.9/speechlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-01-22 13:20:55.000000 speechlib-1.0.9/speechlib.egg-info/top_level.txt
```

### Comparing `speechlib-1.0.8/PKG-INFO` & `speechlib-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: speechlib is a library that can do speaker diarization, transcription and speaker recognition on an audio file to create transcripts with actual speaker names. This library also contain audio preprocessor functions.
 Home-page: https://github.com/Navodplayer1/speechlib
 Author: Navod Peiris
 Author-email: navodpeiris1234@gmail.com
 License: MIT
 Description: ### Requirements
         
@@ -41,26 +41,28 @@
         
         1. convert mp3 to wav
         
         2. convert stereo wav file to mono
         
         3. re-encode the wav file to have 16-bit PCM encoding
         
-        Transcriptor method takes 5 arguments. 
+        Transcriptor method takes 6 arguments. 
         
         1. file to transcribe
         
         2. log_folder to store transcription
         
         3. language used for transcribing (language code is used)
         
         4. model size ("tiny", "small", "medium", "large", "large-v1", "large-v2", "large-v3")
         
         5. voices_folder (contains speaker voice samples for speaker recognition)
         
+        6. quantization: this determine whether to use int8 quantization or not. Quantization may speed up the process but lower the accuracy.
+        
         voices_folder should contain subfolders named with speaker names. Each subfolder belongs to a speaker and it can contain many voice samples. This will be used for speaker recognition to identify the speaker.
         
         if voices_folder is not provided then speaker tags will be arbitrary.
         
         log_folder is to store the final transcript as a text file.
         
         transcript will also indicate the timeframe in seconds where each speaker speaks.
@@ -71,16 +73,17 @@
         from speechlib import Transcriptor
         
         file = "obama_zach.wav"
         voices_folder = "voices"
         language = "en"
         log_folder = "logs"
         modelSize = "medium"
+        quantization = False   # setting this 'True' may speed up the process but lower the accuracy
         
-        transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder)
+        transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder, quantization)
         
         res = transcriptor.transcribe()
         
         res --> [["start", "end", "text", "speaker"], ["start", "end", "text", "speaker"]...]
         ```
         
         start: starting time of speech in seconds
```

### Comparing `speechlib-1.0.8/README.md` & `speechlib-1.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -50,26 +50,28 @@
 
 1. convert mp3 to wav
 
 2. convert stereo wav file to mono
 
 3. re-encode the wav file to have 16-bit PCM encoding
 
-Transcriptor method takes 5 arguments. 
+Transcriptor method takes 6 arguments. 
 
 1. file to transcribe
 
 2. log_folder to store transcription
 
 3. language used for transcribing (language code is used)
 
 4. model size ("tiny", "small", "medium", "large", "large-v1", "large-v2", "large-v3")
 
 5. voices_folder (contains speaker voice samples for speaker recognition)
 
+6. quantization: this determine whether to use int8 quantization or not. Quantization may speed up the process but lower the accuracy.
+
 voices_folder should contain subfolders named with speaker names. Each subfolder belongs to a speaker and it can contain many voice samples. This will be used for speaker recognition to identify the speaker.
 
 if voices_folder is not provided then speaker tags will be arbitrary.
 
 log_folder is to store the final transcript as a text file.
 
 transcript will also indicate the timeframe in seconds where each speaker speaks.
@@ -80,34 +82,42 @@
 from speechlib import Transcriptor
 
 file = "obama_zach.wav"
 voices_folder = "voices"
 language = "en"
 log_folder = "logs"
 modelSize = "medium"
+quantization = False   # setting this 'True' may speed up the process but lower the accuracy
 
-transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder)
+transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder, quantization)
 
 res = transcriptor.transcribe()
 
 res --> [["start", "end", "text", "speaker"], ["start", "end", "text", "speaker"]...]
 ```
 
 start: starting time of speech in seconds  
 end: ending time of speech in seconds  
 text: transcribed text for speech during start and end  
 speaker: speaker of the text 
 
 voices_folder structure:  
-
-![voices_folder structure](voices_folder_structure1.png)
-
-Generated transcript:  
-
-![Transcript](transcript.png)  
+```
+voices_folder    
+|---> person1      
+|        |---> sample1.wav   
+|        |---> sample2.wav     
+|                ...
+|
+|---> person2  
+|        |---> sample1.wav  
+|        |---> sample2.wav   
+|                ...
+|--> ...  
+```
 
 supported language codes:  
 
 ```
 "af", "am", "ar", "as", "az", "ba", "be", "bg", "bn", "bo", "br", "bs", "ca", "cs", "cy", "da", "de", "el", "en", "es", "et", "eu", "fa", "fi", "fo", "fr", "gl", "gu", "ha", "haw", "he", "hi", "hr", "ht", "hu", "hy", "id", "is","it", "ja", "jw", "ka", "kk", "km", "kn", "ko", "la", "lb", "ln", "lo", "lt", "lv", "mg", "mi", "mk", "ml", "mn","mr", "ms", "mt", "my", "ne", "nl", "nn", "no", "oc", "pa", "pl", "ps", "pt", "ro", "ru", "sa", "sd", "si", "sk","sl", "sn", "so", "sq", "sr", "su", "sv", "sw", "ta", "te", "tg", "th", "tk", "tl", "tr", "tt", "uk", "ur", "uz","vi", "yi", "yo", "zh", "yue"
 ```
```

#### html2text {}

```diff
@@ -15,41 +15,45 @@
 Colab: on google colab run this to install CUDA dependencies: ``` !apt install
 libcublas11 ``` You can see this example [notebook]() ### installation: ``` pip
 install speechlib ``` This library does speaker diarization, speaker
 recognition, and transcription on a single wav file to provide a transcript
 with actual speaker names. This library will also return an array containing
 result information. â This library contains following audio preprocessing
 functions: 1. convert mp3 to wav 2. convert stereo wav file to mono 3. re-
-encode the wav file to have 16-bit PCM encoding Transcriptor method takes 5
+encode the wav file to have 16-bit PCM encoding Transcriptor method takes 6
 arguments. 1. file to transcribe 2. log_folder to store transcription 3.
 language used for transcribing (language code is used) 4. model size ("tiny",
 "small", "medium", "large", "large-v1", "large-v2", "large-v3") 5.
-voices_folder (contains speaker voice samples for speaker recognition)
-voices_folder should contain subfolders named with speaker names. Each
-subfolder belongs to a speaker and it can contain many voice samples. This will
-be used for speaker recognition to identify the speaker. if voices_folder is
-not provided then speaker tags will be arbitrary. log_folder is to store the
-final transcript as a text file. transcript will also indicate the timeframe in
-seconds where each speaker speaks. ### Transcription example: ``` from
-speechlib import Transcriptor file = "obama_zach.wav" voices_folder = "voices"
-language = "en" log_folder = "logs" modelSize = "medium" transcriptor =
-Transcriptor(file, log_folder, language, modelSize, voices_folder) res =
-transcriptor.transcribe() res --> [["start", "end", "text", "speaker"],
-["start", "end", "text", "speaker"]...] ``` start: starting time of speech in
-seconds end: ending time of speech in seconds text: transcribed text for speech
-during start and end speaker: speaker of the text voices_folder structure: !
-[voices_folder structure](voices_folder_structure1.png) Generated transcript: !
-[Transcript](transcript.png) supported language codes: ``` "af", "am", "ar",
-"as", "az", "ba", "be", "bg", "bn", "bo", "br", "bs", "ca", "cs", "cy", "da",
-"de", "el", "en", "es", "et", "eu", "fa", "fi", "fo", "fr", "gl", "gu", "ha",
-"haw", "he", "hi", "hr", "ht", "hu", "hy", "id", "is","it", "ja", "jw", "ka",
-"kk", "km", "kn", "ko", "la", "lb", "ln", "lo", "lt", "lv", "mg", "mi", "mk",
-"ml", "mn","mr", "ms", "mt", "my", "ne", "nl", "nn", "no", "oc", "pa", "pl",
-"ps", "pt", "ro", "ru", "sa", "sd", "si", "sk","sl", "sn", "so", "sq", "sr",
-"su", "sv", "sw", "ta", "te", "tg", "th", "tk", "tl", "tr", "tt", "uk", "ur",
+voices_folder (contains speaker voice samples for speaker recognition) 6.
+quantization: this determine whether to use int8 quantization or not.
+Quantization may speed up the process but lower the accuracy. voices_folder
+should contain subfolders named with speaker names. Each subfolder belongs to a
+speaker and it can contain many voice samples. This will be used for speaker
+recognition to identify the speaker. if voices_folder is not provided then
+speaker tags will be arbitrary. log_folder is to store the final transcript as
+a text file. transcript will also indicate the timeframe in seconds where each
+speaker speaks. ### Transcription example: ``` from speechlib import
+Transcriptor file = "obama_zach.wav" voices_folder = "voices" language = "en"
+log_folder = "logs" modelSize = "medium" quantization = False # setting this
+'True' may speed up the process but lower the accuracy transcriptor =
+Transcriptor(file, log_folder, language, modelSize, voices_folder,
+quantization) res = transcriptor.transcribe() res --> [["start", "end", "text",
+"speaker"], ["start", "end", "text", "speaker"]...] ``` start: starting time of
+speech in seconds end: ending time of speech in seconds text: transcribed text
+for speech during start and end speaker: speaker of the text voices_folder
+structure: ``` voices_folder |---> person1 | |---> sample1.wav | |---
+> sample2.wav | ... | |---> person2 | |---> sample1.wav | |---> sample2.wav |
+... |--> ... ``` supported language codes: ``` "af", "am", "ar", "as", "az",
+"ba", "be", "bg", "bn", "bo", "br", "bs", "ca", "cs", "cy", "da", "de", "el",
+"en", "es", "et", "eu", "fa", "fi", "fo", "fr", "gl", "gu", "ha", "haw", "he",
+"hi", "hr", "ht", "hu", "hy", "id", "is","it", "ja", "jw", "ka", "kk", "km",
+"kn", "ko", "la", "lb", "ln", "lo", "lt", "lv", "mg", "mi", "mk", "ml",
+"mn","mr", "ms", "mt", "my", "ne", "nl", "nn", "no", "oc", "pa", "pl", "ps",
+"pt", "ro", "ru", "sa", "sd", "si", "sk","sl", "sn", "so", "sq", "sr", "su",
+"sv", "sw", "ta", "te", "tg", "th", "tk", "tl", "tr", "tt", "uk", "ur",
 "uz","vi", "yi", "yo", "zh", "yue" ``` supported language names: ```
 "Afrikaans", "Amharic", "Arabic", "Assamese", "Azerbaijani", "Bashkir",
 "Belarusian", "Bulgarian", "Bengali","Tibetan", "Breton", "Bosnian", "Catalan",
 "Czech", "Welsh", "Danish", "German", "Greek", "English", "Spanish","Estonian",
 "Basque", "Persian", "Finnish", "Faroese", "French", "Galician", "Gujarati",
 "Hausa", "Hawaiian","Hebrew", "Hindi", "Croatian", "Haitian", "Hungarian",
 "Armenian", "Indonesian", "Icelandic", "Italian", "Japanese","Javanese",
```

### Comparing `speechlib-1.0.8/setup.py` & `speechlib-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("library.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speechlib",
-    version="1.0.8",  
+    version="1.0.9",  
     description="speechlib is a library that can do speaker diarization, transcription and speaker recognition on an audio file to create transcripts with actual speaker names. This library also contain audio preprocessor functions.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Navodplayer1/speechlib",
     author="Navod Peiris",
     author_email="navodpeiris1234@gmail.com",
```

### Comparing `speechlib-1.0.8/speechlib/convert_to_mono.py` & `speechlib-1.0.9/speechlib/convert_to_mono.py`

 * *Files identical despite different names*

### Comparing `speechlib-1.0.8/speechlib/convert_to_wav.py` & `speechlib-1.0.9/speechlib/convert_to_wav.py`

 * *Files identical despite different names*

### Comparing `speechlib-1.0.8/speechlib/core_analysis.py` & `speechlib-1.0.9/speechlib/core_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .re_encode import (re_encode)
 from .convert_to_mono import (convert_to_mono)
 from .convert_to_wav import (convert_to_wav)
 
 # by default use google speech-to-text API
 # if False, then use whisper finetuned version for sinhala
-def core_analysis(file_name, voices_folder, log_folder, language, modelSize):
+def core_analysis(file_name, voices_folder, log_folder, language, modelSize, quantization=False):
 
     # <-------------------PreProcessing file-------------------------->
 
     # check if file is in wav format, if not convert to wav
     file_name = convert_to_wav(file_name)
 
     # convert file to mono
@@ -107,15 +107,15 @@
         del speaker_map[key]
 
     # transcribing the texts differently according to speaker
     start_time = int(time.time())
     print("running transcription...")
     for spk_tag, spk_segments in speakers.items():
         spk = speaker_map[spk_tag]
-        segment_out = wav_file_segmentation(file_name, spk_segments, language, modelSize)
+        segment_out = wav_file_segmentation(file_name, spk_segments, language, modelSize, quantization)
         speakers[spk_tag] = segment_out
     end_time = int(time.time())
     elapsed_time = int(end_time - start_time)
     print(f"transcription done. Time taken: {elapsed_time} seconds.")
 
     common_segments = []
```

### Comparing `speechlib-1.0.8/speechlib/re_encode.py` & `speechlib-1.0.9/speechlib/re_encode.py`

 * *Files identical despite different names*

### Comparing `speechlib-1.0.8/speechlib/speaker_recognition.py` & `speechlib-1.0.9/speechlib/speaker_recognition.py`

 * *Files identical despite different names*

### Comparing `speechlib-1.0.8/speechlib/speechlib.py` & `speechlib-1.0.9/speechlib/speechlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,242 +1,245 @@
 from .core_analysis import (core_analysis)
 from .re_encode import (re_encode)
 from .convert_to_mono import (convert_to_mono)
 from .convert_to_wav import (convert_to_wav)
 
 class Transcriptor:
-    '''transcribe a wav file 
-    
-        arguments:
 
-        file: name of wav file with extension ex: file.wav
+    def __init__(self, file, log_folder, language, modelSize, voices_folder=None, quantization=False):
+        '''transcribe a wav file 
+        
+            arguments:
 
-        log_folder: name of folder where transcript will be stored
+            file: name of wav file with extension ex: file.wav
 
-        language: language of wav file
+            log_folder: name of folder where transcript will be stored
 
-        modelSize: tiny, small, medium, large, large-v1, large-v2, large-v3 (bigger model is more accurate but slow!!)
+            language: language of wav file
 
-        voices_folder: folder containing subfolders named after each speaker with speaker voice samples in them. This will be used for speaker recognition
+            modelSize: tiny, small, medium, large, large-v1, large-v2, large-v3 (bigger model is more accurate but slow!!)
 
-        see documentation: https://github.com/Navodplayer1/speechlib
-    '''
+            voices_folder: folder containing subfolders named after each speaker with speaker voice samples in them. This will be used for speaker recognition
 
-    def __init__(self, file, log_folder, language, modelSize, voices_folder=None):
-        '''
+            quantization: whether to use int8 quantization or not (default=False)
+
+            see documentation: https://github.com/Navodplayer1/speechlib
+        
+            
         supported languages:  
-        ### Afrikaans
+        #### Afrikaans
         "af",
-        ### Amharic
+        #### Amharic
         "am",
-        ### Arabic
+        #### Arabic
         "ar",
-        ### Assamese
+        #### Assamese
         "as",
-        ### Azerbaijani
+        #### Azerbaijani
         "az",
-        ### Bashkir
+        #### Bashkir
         "ba",
-        ### Belarusian
+        #### Belarusian
         "be",
-        ### Bulgarian
+        #### Bulgarian
         "bg",
-        ### Bengali
+        #### Bengali
         "bn",
-        ### Tibetan
+        #### Tibetan
         "bo",
-        ### Breton
+        #### Breton
         "br",
-        ### Bosnian
+        #### Bosnian
         "bs",
-        ### Catalan
+        #### Catalan
         "ca",
-        ### Czech
+        #### Czech
         "cs",
-        ### Welsh
+        #### Welsh
         "cy",
-        ### Danish
+        #### Danish
         "da",
-        ### German
+        #### German
         "de",
-        ### Greek
+        #### Greek
         "el",
-        ### English
+        #### English
         "en",
-        ### Spanish
+        #### Spanish
         "es",
-        ### Estonian
+        #### Estonian
         "et",
-        ### Basque
+        #### Basque
         "eu",
-        ### Persian
+        #### Persian
         "fa",
-        ### Finnish
+        #### Finnish
         "fi",
-        ### Faroese
+        #### Faroese
         "fo",
-        ### French
+        #### French
         "fr",
-        ### Galician
+        #### Galician
         "gl",
-        ### Gujarati
+        #### Gujarati
         "gu",
-        ### Hausa
+        #### Hausa
         "ha",
-        ### Hawaiian
+        #### Hawaiian
         "haw",
-        ### Hebrew
+        #### Hebrew
         "he",
-        ### Hindi
+        #### Hindi
         "hi",
-        ### Croatian
+        #### Croatian
         "hr",
-        ### Haitian
+        #### Haitian
         "ht",
-        ### Hungarian
+        #### Hungarian
         "hu",
-        ### Armenian
+        #### Armenian
         "hy",
-        ### Indonesian
+        #### Indonesian
         "id",
-        ### Icelandic
+        #### Icelandic
         "is",
-        ### Italian
+        #### Italian
         "it",
-        ### Japanese
+        #### Japanese
         "ja",
-        ### Javanese
+        #### Javanese
         "jw",
-        ### Georgian
+        #### Georgian
         "ka",
-        ### Kazakh
+        #### Kazakh
         "kk",
-        ### Khmer
+        #### Khmer
         "km",
-        ### Kannada
+        #### Kannada
         "kn",
-        ### Korean
+        #### Korean
         "ko",
-        ### Latin
+        #### Latin
         "la",
-        ### Luxembourgish
+        #### Luxembourgish
         "lb",
-        ### Lingala
+        #### Lingala
         "ln",
-        ### Lao
+        #### Lao
         "lo",
-        ### Lithuanian
+        #### Lithuanian
         "lt",
-        ### Latvian
+        #### Latvian
         "lv",
-        ### Malagasy
+        #### Malagasy
         "mg",
-        ### Maori
+        #### Maori
         "mi",
-        ### Macedonian
+        #### Macedonian
         "mk",
-        ### Malayalam
+        #### Malayalam
         "ml",
-        ### Mongolian
+        #### Mongolian
         "mn",
-        ### Marathi
+        #### Marathi
         "mr",
-        ### Malay
+        #### Malay
         "ms",
-        ### Maltese
+        #### Maltese
         "mt",
-        ### Burmese
+        #### Burmese
         "my",
-        ### Nepali
+        #### Nepali
         "ne",
-        ### Dutch
+        #### Dutch
         "nl",
-        ### Norwegian Nynorsk
+        #### Norwegian Nynorsk
         "nn",
-        ### Norwegian
+        #### Norwegian
         "no",
-        ### Occitan
+        #### Occitan
         "oc",
-        ### Punjabi
+        #### Punjabi
         "pa",
-        ### Polish
+        #### Polish
         "pl",
-        ### Pashto
+        #### Pashto
         "ps",
-        ### Portuguese
+        #### Portuguese
         "pt",
-        ### Romanian
+        #### Romanian
         "ro",
-        ### Russian
+        #### Russian
         "ru",
-        ### Sanskrit
+        #### Sanskrit
         "sa",
-        ### Sindhi
+        #### Sindhi
         "sd",
-        ### Sinhalese
+        #### Sinhalese
         "si",
-        ### Slovak
+        #### Slovak
         "sk",
-        ### Slovenian
+        #### Slovenian
         "sl",
-        ### Shona
+        #### Shona
         "sn",
-        ### Somali
+        #### Somali
         "so",
-        ### Albanian
+        #### Albanian
         "sq",
-        ### Serbian
+        #### Serbian
         "sr",
-        ### Sundanese
+        #### Sundanese
         "su",
-        ### Swedish
+        #### Swedish
         "sv",
-        ### Swahili
+        #### Swahili
         "sw",
-        ### Tamil
+        #### Tamil
         "ta",
-        ### Telugu
+        #### Telugu
         "te",
-        ### Tajik
+        #### Tajik
         "tg",
-        ### Thai
+        #### Thai
         "th",
-        ### Turkmen
+        #### Turkmen
         "tk",
-        ### Tagalog
+        #### Tagalog
         "tl",
-        ### Turkish
+        #### Turkish
         "tr",
-        ### Tatar
+        #### Tatar
         "tt",
-        ### Ukrainian
+        #### Ukrainian
         "uk",
-        ### Urdu
+        #### Urdu
         "ur",
-        ### Uzbek
+        #### Uzbek
         "uz",
-        ### Vietnamese
+        #### Vietnamese
         "vi",
-        ### Yiddish
+        #### Yiddish
         "yi",
-        ### Yoruba
+        #### Yoruba
         "yo",
-        ### Chinese
+        #### Chinese
         "zh",
-        ### Cantonese
+        #### Cantonese
         "yue",
         '''
         self.file = file
         self.voices_folder = voices_folder
         self.language = language
         self.log_folder = log_folder
         self.modelSize = modelSize
+        self.quantization = quantization
 
     def transcribe(self):
-        res = core_analysis(self.file, self.voices_folder, self.log_folder, self.language, self.modelSize)
+        res = core_analysis(self.file, self.voices_folder, self.log_folder, self.language, self.modelSize, self.quantization)
         return res
 
 class PreProcessor:
     '''
     class for preprocessing audio files.
 
     methods:
```

### Comparing `speechlib-1.0.8/speechlib/transcribe.py` & `speechlib-1.0.9/speechlib/transcribe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import torch
 from .whisper_sinhala import (whisper_sinhala)
 from faster_whisper import WhisperModel
 
-def transcribe(file, language, model_size):
+def transcribe(file, language, model_size, quantization):
     res = ""
-    if language == "sin" or language == "Sin":
+    if language == "si" or language == "Si":
         res = whisper_sinhala(file)
         return res
     elif model_size == "tiny" or model_size == "small" or model_size == "medium" or model_size == "large" or model_size == "large-v1" or model_size == "large-v2" or model_size == "large-v3":
 
         if torch.cuda.is_available():
-            # run on GPU with INT8
-            model = WhisperModel(model_size, device="cuda", compute_type="int8_float16")
+            if quantization:
+                model = WhisperModel(model_size, device="cuda", compute_type="int8_float16")
+            else:
+                model = WhisperModel(model_size, device="cuda", compute_type="float16")
         else:
-            # run on CPU with INT8
-            model = WhisperModel(model_size, device="cpu", compute_type="int8")
+            if quantization:
+                model = WhisperModel(model_size, device="cpu", compute_type="int8")
+            else:
+                model = WhisperModel(model_size, device="cpu", compute_type="float32")
 
         if language in model.supported_languages:
-            segments, info = model.transcribe(file, language=language, beam_size=1)
+            segments, info = model.transcribe(file, language=language, beam_size=5)
 
             for segment in segments:
                 res += segment.text + " "
                 return res
         else:
             Exception("Language code not supported.\nThese are the supported languages:\n", model.supported_languages)
     else:
```

### Comparing `speechlib-1.0.8/speechlib/wav_segmenter.py` & `speechlib-1.0.9/speechlib/wav_segmenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pydub import AudioSegment
 from .transcribe import (transcribe)
 
 # segment according to speaker
-def wav_file_segmentation(file_name, segments, language, modelSize):
+def wav_file_segmentation(file_name, segments, language, modelSize, quantization):
     # Load the WAV file
     audio = AudioSegment.from_file(file_name, format="wav")
     trans = ""
 
     texts = []
 
     folder_name = "segments"
@@ -23,15 +23,15 @@
         end = segment[1] * 1000     # end time in miliseconds
         clip = audio[start:end]
         i = i + 1
         file = folder_name + "/" + "segment"+ str(i) + ".wav"
         clip.export(file, format="wav")
 
         try:
-            trans = transcribe(file, language, modelSize)  
+            trans = transcribe(file, language, modelSize, quantization)  
             
             # return -> [[start time, end time, transcript], [start time, end time, transcript], ..]
             texts.append([segment[0], segment[1], trans])
         except:
             pass
         # Delete the WAV file after processing
         os.remove(file)
```

### Comparing `speechlib-1.0.8/speechlib/write_log_file.py` & `speechlib-1.0.9/speechlib/write_log_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 from datetime import datetime
 
 def write_log_file(common_segments, log_folder):
 
+    if not os.path.exists(log_folder):
+        os.makedirs(log_folder)
+
     file_name = "output"
     current_datetime = datetime.now().strftime("%Y-%m-%d")
 
     #---------------------log file part-------------------------
 
     log_file = log_folder + "/" + file_name + "_" + current_datetime + ".txt"
```

### Comparing `speechlib-1.0.8/speechlib.egg-info/PKG-INFO` & `speechlib-1.0.9/speechlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: speechlib is a library that can do speaker diarization, transcription and speaker recognition on an audio file to create transcripts with actual speaker names. This library also contain audio preprocessor functions.
 Home-page: https://github.com/Navodplayer1/speechlib
 Author: Navod Peiris
 Author-email: navodpeiris1234@gmail.com
 License: MIT
 Description: ### Requirements
         
@@ -41,26 +41,28 @@
         
         1. convert mp3 to wav
         
         2. convert stereo wav file to mono
         
         3. re-encode the wav file to have 16-bit PCM encoding
         
-        Transcriptor method takes 5 arguments. 
+        Transcriptor method takes 6 arguments. 
         
         1. file to transcribe
         
         2. log_folder to store transcription
         
         3. language used for transcribing (language code is used)
         
         4. model size ("tiny", "small", "medium", "large", "large-v1", "large-v2", "large-v3")
         
         5. voices_folder (contains speaker voice samples for speaker recognition)
         
+        6. quantization: this determine whether to use int8 quantization or not. Quantization may speed up the process but lower the accuracy.
+        
         voices_folder should contain subfolders named with speaker names. Each subfolder belongs to a speaker and it can contain many voice samples. This will be used for speaker recognition to identify the speaker.
         
         if voices_folder is not provided then speaker tags will be arbitrary.
         
         log_folder is to store the final transcript as a text file.
         
         transcript will also indicate the timeframe in seconds where each speaker speaks.
@@ -71,16 +73,17 @@
         from speechlib import Transcriptor
         
         file = "obama_zach.wav"
         voices_folder = "voices"
         language = "en"
         log_folder = "logs"
         modelSize = "medium"
+        quantization = False   # setting this 'True' may speed up the process but lower the accuracy
         
-        transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder)
+        transcriptor = Transcriptor(file, log_folder, language, modelSize, voices_folder, quantization)
         
         res = transcriptor.transcribe()
         
         res --> [["start", "end", "text", "speaker"], ["start", "end", "text", "speaker"]...]
         ```
         
         start: starting time of speech in seconds
```

### Comparing `speechlib-1.0.8/speechlib.egg-info/SOURCES.txt` & `speechlib-1.0.9/speechlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

