# Comparing `tmp/helpers_ai-0.0.2.tar.gz` & `tmp/helpers_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpers_ai-0.0.2.tar", max compression
+gzip compressed data, was "helpers_ai-0.0.3.tar", max compression
```

## Comparing `helpers_ai-0.0.2.tar` & `helpers_ai-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,42 @@
--rw-r--r--   0        0        0       27 2024-04-10 16:32:01.434593 helpers_ai-0.0.2/helpers_ai/__init__.py
--rw-r--r--   0        0        0       27 2024-04-10 16:31:22.228001 helpers_ai-0.0.2/helpers_ai/annotator/__init__.py
--rw-r--r--   0        0        0    11060 2024-04-14 07:40:23.085747 helpers_ai-0.0.2/helpers_ai/annotator/image_convertor.py
--rw-r--r--   0        0        0     7623 2024-04-14 08:06:53.339787 helpers_ai-0.0.2/helpers_ai/annotator/video_convertor.py
--rw-r--r--   0        0        0       27 2024-04-10 16:31:13.476929 helpers_ai-0.0.2/helpers_ai/dataset_convertors/__init__.py
--rw-r--r--   0        0        0     3229 2024-04-13 14:54:48.115576 helpers_ai-0.0.2/helpers_ai/dataset_convertors/coco2voc.py
--rw-r--r--   0        0        0     4474 2024-04-13 14:55:16.399819 helpers_ai-0.0.2/helpers_ai/dataset_convertors/coco2yolo.py
--rw-r--r--   0        0        0     7650 2024-04-13 04:03:05.932309 helpers_ai-0.0.2/helpers_ai/dataset_convertors/jm2mmocr.py
--rw-r--r--   0        0        0     4471 2024-04-13 14:56:01.662344 helpers_ai-0.0.2/helpers_ai/dataset_convertors/voc2coco.py
--rw-r--r--   0        0        0     4628 2024-04-13 14:56:23.184744 helpers_ai-0.0.2/helpers_ai/dataset_convertors/voc2yolo.py
--rw-r--r--   0        0        0     5184 2024-04-13 14:56:48.605840 helpers_ai-0.0.2/helpers_ai/dataset_convertors/yolo2coco.py
--rw-r--r--   0        0        0     3938 2024-04-13 14:57:19.925083 helpers_ai-0.0.2/helpers_ai/dataset_convertors/yolo2voc.py
--rw-r--r--   0        0        0    10151 2024-04-07 04:03:19.135008 helpers_ai-0.0.2/helpers_ai/losses.py
--rw-r--r--   0        0        0       27 2024-04-10 16:31:50.015628 helpers_ai-0.0.2/helpers_ai/utils/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-06 10:18:24.708387 helpers_ai-0.0.2/helpers_ai/utils/jm2mm.py
--rw-r--r--   0        0        0     4392 2024-04-13 12:33:43.188543 helpers_ai-0.0.2/helpers_ai/utils/util.py
--rw-r--r--   0        0        0     9101 2024-04-13 12:35:54.884669 helpers_ai-0.0.2/helpers_ai/utils/validator.py
--rw-r--r--   0        0        0     1330 2024-04-13 12:41:31.627096 helpers_ai-0.0.2/helpers_ai/utils/voc.py
--rw-r--r--   0        0        0    35182 2024-04-10 14:36:58.350917 helpers_ai-0.0.2/LICENSE
--rw-r--r--   0        0        0      962 2024-04-14 08:44:44.851479 helpers_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-14 08:41:32.551770 helpers_ai-0.0.2/README.md
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 helpers_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-05-11 05:30:53.834372 helpers_ai-0.0.3/helpers_ai/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-11 14:17:21.257352 helpers_ai-0.0.3/helpers_ai/__main__.py
+-rw-r--r--   0        0        0       27 2024-04-10 16:31:22.228001 helpers_ai-0.0.3/helpers_ai/annotator/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-11 09:13:48.126394 helpers_ai-0.0.3/helpers_ai/annotator/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    18353 2024-05-11 09:45:13.711280 helpers_ai-0.0.3/helpers_ai/annotator/__pycache__/annotate.cpython-311.pyc
+-rw-r--r--   0        0        0     3921 2024-05-11 10:31:00.448316 helpers_ai-0.0.3/helpers_ai/annotator/__pycache__/image_convertor.cpython-311.pyc
+-rw-r--r--   0        0        0    13623 2024-05-11 13:14:55.774005 helpers_ai-0.0.3/helpers_ai/annotator/__pycache__/video_convertor.cpython-311.pyc
+-rw-r--r--   0        0        0    10797 2024-05-11 09:44:57.511767 helpers_ai-0.0.3/helpers_ai/annotator/annotate.py
+-rw-r--r--   0        0        0     1930 2024-05-11 10:30:28.573922 helpers_ai-0.0.3/helpers_ai/annotator/image_convertor.py
+-rw-r--r--   0        0        0     7740 2024-05-11 13:13:40.262903 helpers_ai-0.0.3/helpers_ai/annotator/video_convertor.py
+-rw-r--r--   0        0        0       27 2024-04-10 16:31:13.476929 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-11 13:31:29.075348 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6490 2024-05-11 13:31:29.086416 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/coco2voc.cpython-311.pyc
+-rw-r--r--   0        0        0     9518 2024-05-11 13:31:29.113005 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/coco2yolo.cpython-311.pyc
+-rw-r--r--   0        0        0    13719 2024-05-11 13:31:29.147849 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/jm2mmocr.cpython-311.pyc
+-rw-r--r--   0        0        0     6765 2024-05-11 13:31:29.135531 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/voc2coco.cpython-311.pyc
+-rw-r--r--   0        0        0     9312 2024-05-11 13:31:29.142115 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/voc2yolo.cpython-311.pyc
+-rw-r--r--   0        0        0     9569 2024-05-11 13:31:29.122002 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/yolo2coco.cpython-311.pyc
+-rw-r--r--   0        0        0     8665 2024-05-11 13:31:29.129079 helpers_ai-0.0.3/helpers_ai/dataset_convertors/__pycache__/yolo2voc.cpython-311.pyc
+-rw-r--r--   0        0        0     3229 2024-05-11 13:28:50.668864 helpers_ai-0.0.3/helpers_ai/dataset_convertors/coco2voc.py
+-rw-r--r--   0        0        0     4474 2024-04-13 14:55:16.399819 helpers_ai-0.0.3/helpers_ai/dataset_convertors/coco2yolo.py
+-rw-r--r--   0        0        0     7650 2024-04-13 04:03:05.932309 helpers_ai-0.0.3/helpers_ai/dataset_convertors/jm2mmocr.py
+-rw-r--r--   0        0        0     4471 2024-04-13 14:56:01.662344 helpers_ai-0.0.3/helpers_ai/dataset_convertors/voc2coco.py
+-rw-r--r--   0        0        0     4628 2024-04-13 14:56:23.184744 helpers_ai-0.0.3/helpers_ai/dataset_convertors/voc2yolo.py
+-rw-r--r--   0        0        0     5184 2024-04-13 14:56:48.605840 helpers_ai-0.0.3/helpers_ai/dataset_convertors/yolo2coco.py
+-rw-r--r--   0        0        0     3938 2024-04-13 14:57:19.925083 helpers_ai-0.0.3/helpers_ai/dataset_convertors/yolo2voc.py
+-rw-r--r--   0        0        0    10151 2024-04-07 04:03:19.135008 helpers_ai-0.0.3/helpers_ai/losses.py
+-rw-r--r--   0        0        0    11037 2024-05-11 14:34:30.382700 helpers_ai-0.0.3/helpers_ai/main.py
+-rw-r--r--   0        0        0       27 2024-04-10 16:31:50.015628 helpers_ai-0.0.3/helpers_ai/utils/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-11 09:13:48.492637 helpers_ai-0.0.3/helpers_ai/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4437 2024-05-11 13:31:29.173593 helpers_ai-0.0.3/helpers_ai/utils/__pycache__/jm2mm.cpython-311.pyc
+-rw-r--r--   0        0        0     7588 2024-05-11 09:13:48.499398 helpers_ai-0.0.3/helpers_ai/utils/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0    20304 2024-05-11 09:13:48.493640 helpers_ai-0.0.3/helpers_ai/utils/__pycache__/validator.cpython-311.pyc
+-rw-r--r--   0        0        0     3033 2024-05-11 13:31:29.105968 helpers_ai-0.0.3/helpers_ai/utils/__pycache__/voc.cpython-311.pyc
+-rw-r--r--   0        0        0     2522 2024-04-06 10:18:24.708387 helpers_ai-0.0.3/helpers_ai/utils/jm2mm.py
+-rw-r--r--   0        0        0     4392 2024-04-13 12:33:43.188543 helpers_ai-0.0.3/helpers_ai/utils/util.py
+-rw-r--r--   0        0        0     9101 2024-04-13 12:35:54.884669 helpers_ai-0.0.3/helpers_ai/utils/validator.py
+-rw-r--r--   0        0        0     1330 2024-04-13 12:41:31.627096 helpers_ai-0.0.3/helpers_ai/utils/voc.py
+-rw-r--r--   0        0        0    35182 2024-04-10 14:36:58.350917 helpers_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1023 2024-05-11 15:09:10.449711 helpers_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      476 2024-05-11 14:46:47.436801 helpers_ai-0.0.3/README.md
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 helpers_ai-0.0.3/PKG-INFO
```

### Comparing `helpers_ai-0.0.2/helpers_ai/annotator/image_convertor.py` & `helpers_ai-0.0.3/helpers_ai/annotator/annotate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,51 @@
 import os
 import cv2
 import yaml
 import tqdm
-import natsort
 import imageio as iio
 from pycocotools.coco import COCO
 import xml.etree.ElementTree as et
 
 from helpers_ai.utils.validator import coco_validator, yolo_validator, voc_validator
 from helpers_ai.utils.util import annot_bbox, annot_seg, coco_rle2mask, annot_color
 
 
 
 
-def img2vid(images_path:str, destination_path:str=".", filename:str="output",
-             fps:int=25, size:tuple[int,int]=(640,640)) -> None:
-
-    assert os.path.isdir(images_path), "image_path must be a directory."
-    assert len(size) == 2, "size must contain two integers."
-    assert len(filename.split(".")) == 1, "filename must not contain extensions."
-
-    vid_wr = cv2.VideoWriter(os.path.join(destination_path,filename+".mp4"), cv2.VideoWriter.fourcc(*"mp4v"), fps=fps, frameSize=size)
-
-    for file in tqdm.tqdm(natsort.natsorted(os.listdir(images_path))):
-        if file.endswith((".jpg",".png",".jpeg")):
-            img = cv2.imread(os.path.join(images_path, file))
-            img = cv2.resize(img, size)
-            vid_wr.write(img)
-    
-    vid_wr.release()
-
-    print("\nConversion Completed.\n")
-
-    print("The video file is saved at '{}' named '{}'.".format(destination_path, filename+".mp4"))
-
-
-
-
-def img2gif(images_path:str, destination_path:str=".", filename:str="output.gif", size:tuple[int,int]=(640,640),
-            duration_of_frame:int=100, loop:int=0) -> None:
-
-    assert os.path.isdir(images_path), "image_path must be a directory."
-    assert filename[-4:] == ".gif", "filename must endswith '.gif' extensions."
-
-    with iio.get_writer(os.path.join(destination_path,filename), mode="I", duration=duration_of_frame, loop=loop) as writer:
-        
-        for file in tqdm.tqdm(natsort.natsorted(os.listdir(images_path))):
-            if file.endswith((".jpg",".png",".jpeg")):   
-                img = cv2.imread(os.path.join(images_path, file))
-                img = cv2.resize(img, size)
-                writer.append_data(cv2.cvtColor(img,cv2.COLOR_BGR2RGB))
-
-    print("\nConversion Completed.\n")
-
-    print("The gif file is saved at '{}' named '{}'.".format(destination_path, filename))
-
-
-
-
-def coco_annotator(image_folder:str, json_path:str, destination_path:str=".",
-                   segmentation:bool=False, bbox:bool=True, class_names:tuple[str]=None,
-                   video_out:bool=False, vid_name:str="output.mp4", fps:int=24, size:tuple[int,int]=(640,640)) -> None:
+def coco_annotator(image_folder:str, json_path:str, destination_path:str, segmentation:bool,
+                   bbox:bool, class_names:tuple[str], file_name:str, size:tuple[int,int],
+                   video_out:bool, fps:int, gif_out:bool, duration_of_frame:int, loop:int) -> None:
     
     assert (bbox and segmentation) or bbox or segmentation, "Either segmentation or bbox must be True or both may be True."
     assert json_path.endswith(".json") and os.path.isfile(json_path), "annotation file must be a json file."
     assert os.path.isdir(image_folder), "image_folder must be a folder."
-    assert vid_name[-4:] == ".mp4", "video_name must be in mp4 format."
+    assert file_name[-4:] in [".mp4",".gif"], "video_name must be in .gif or .mp4 format."
 
     coco = COCO(json_path)
 
     print("\nAnnotation Validator in progress.....")
 
     coco_validator(coco,image_folder)
 
     print("\nAnnotation in progress...........")
     
-    if class_names is None:
+    if class_names != ():
         imgid = coco.getImgIds()
         cat_id = coco.getCatIds()
     else:
         cat_id = coco.getCatIds(catNms=class_names)
         imgid = coco.getImgIds(catIds=cat_id)
 
     if video_out:
-        vid_wr = cv2.VideoWriter(os.path.join(destination_path, vid_name), cv2.VideoWriter.fourcc(*"mp4v"),
+        vid_wr = cv2.VideoWriter(os.path.join(destination_path, file_name[:-4]+".mp4"), cv2.VideoWriter.fourcc(*"mp4v"),
                                  fps, size)
+    
+    elif gif_out:
+        gif_wr = iio.get_writer(os.path.join(destination_path,file_name[:-4]+".gif"), mode="I", duration=duration_of_frame, loop=loop) 
 
     print("")
 
     for imid in tqdm.tqdm(imgid):
         image = coco.loadImgs(imid)
         annot = coco.loadAnns(coco.getAnnIds(imgIds=imid, catIds=cat_id))
         img = os.path.join(image_folder,image[0]["file_name"])
@@ -96,17 +53,19 @@
         for ann in annot:
             classes = int(ann["category_id"])
             ann_seg = ann["segmentation"]
             ann_bbox =  ann["bbox"]
 
             if segmentation and ann_seg != [[]]:
                 if isinstance(ann_seg, dict):
+                    continue
                     seg_lst = coco_rle2mask(ann_seg["counts"], ann_seg["size"], 255, False, 50)
                     for k in seg_lst:
                         seg = k.ravel()
+                        print(seg)
                         seg_x = seg[0][::2]
                         seg_y = seg[0][1::2]
                         img = annot_seg(img, [[x,y] for x,y in zip(seg_x,seg_y)], annot_color(classes))
                 else:
                     seg_x = ann_seg[0][::2]
                     seg_y = ann_seg[0][1::2]
                     img = annot_seg(img, [[x,y] for x,y in zip(seg_x,seg_y)], annot_color(classes))
@@ -114,55 +73,70 @@
             if bbox and ann_bbox != []:
                 x,y,w,h = [int(i) for i in ann_bbox]
                 img = annot_bbox(img, [x, y, x+w, y+h], annot_color(classes), 2, coco.loadCats(classes)[0]["name"], 1)
         
         if video_out:
             img = cv2.resize(img, size)
             vid_wr.write(img)
+        
+        elif gif_out:
+            img = cv2.resize(img, size)
+            gif_wr.append_data(cv2.cvtColor(img,cv2.COLOR_BGR2RGB))
+        
         else:
             cv2.imwrite(os.path.join(destination_path, image[0]["file_name"]), img)
     
     if video_out:
         vid_wr.release()
+    elif gif_out:
+        gif_wr.close()
 
     print("\nSave Completed.")
 
     print("\nThe annotation process is Completed.")
 
     if video_out:
-        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, vid_name))
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".mp4"))
+    elif gif_out:
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".gif"))
     else:
         print("\nThe files are saved at '{}'.".format(destination_path))
 
 
 
-def yolo_annotator(image_folder:str, labels_folder:str, cls_file_path:str, n_classes:int, destination_path:str=".",
-                   segmentation:bool=False, bbox:bool=True, class_names:tuple[str]=(),
-                   video_out:bool=False, vid_name:str="output.mp4", fps:int=24, size:tuple[int,int]=(640,640)) -> None:
+def yolo_annotator(image_folder:str, labels_folder:str, cls_file_path:str, destination_path:str, segmentation:bool,
+                   bbox:bool, class_names:tuple[str], file_name:str, size:tuple[int,int], video_out:bool, fps:int, 
+                   gif_out:bool, duration_of_frame:int, loop:int) -> None:
     
     assert (bbox and segmentation) or bbox or segmentation, "Either segmentation or bbox must be True or both may be True."
     assert os.path.isfile(cls_file_path), "cls_file_path must be a class file in txt or yaml format."
     assert os.path.isdir(image_folder) and os.path.isdir(labels_folder), "images_folder and labels_folder must be a directory."
-    assert vid_name[-4:] == ".mp4", "video_name must be in mp4 format."
+    assert file_name[-4:] in [".mp4",".gif"], "video_name must be in .gif or .mp4 format."
 
     print("\nAnnotation Validator in progress.....")
 
-    yolo_validator(image_folder, labels_folder, list(range(n_classes)))
-
-    print("\nAnnotation in progress...........\n")
-
     with open(cls_file_path, "r") as f:
         if cls_file_path.endswith(".yaml"):
             cls_name = yaml.safe_load(f)["names"]
         else:
             cls_name = f.readlines()
+
+    yolo_validator(image_folder, labels_folder, list(range(len(cls_name))))
+
+    print("\nAnnotation in progress...........\n")
+
+    
     
     if video_out:
-        vid_wr = cv2.VideoWriter(os.path.join(destination_path, vid_name), cv2.VideoWriter.fourcc(*"mp4v"),
+        vid_wr = cv2.VideoWriter(os.path.join(destination_path, file_name[:-4]+".mp4"), cv2.VideoWriter.fourcc(*"mp4v"),
                                  fps, size)
+    
+    elif gif_out:
+        gif_wr = iio.get_writer(os.path.join(destination_path,file_name[:-4]+".gif"), mode="I", duration=duration_of_frame, loop=loop) 
+
        
     for file in tqdm.tqdm(os.listdir(image_folder)):
 
         img = cv2.imread(os.path.join(image_folder, file))
         height, width = img.shape[:2]
 
         with open(os.path.join(labels_folder, file[:-4]+".txt"), "r") as f:
@@ -185,55 +159,68 @@
             if bbox and len(ann_data) > 3:
                 x, y, x1, y1 = [int(min(seg_x)), int(min(seg_y)), int(max(seg_x)), int(max(seg_y))]
                 img = annot_bbox(img, [x, y, x1, y1], annot_color(cls), 2, cls_name[cls], 1)
 
         if video_out:
             img = cv2.resize(img, size)
             vid_wr.write(img)
+
+        elif gif_out:
+            img = cv2.resize(img, size)
+            gif_wr.append_data(cv2.cvtColor(img,cv2.COLOR_BGR2RGB))
+
         else:
             cv2.imwrite(os.path.join(destination_path, file), img)
     
     if video_out:
         vid_wr.release()
+    elif gif_out:
+        gif_wr.close()
 
     print("\nSave Completed.")
 
     print("\nThe annotation process is Completed.")
 
     if video_out:
-        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, vid_name))
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".mp4"))
+    elif gif_out:
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".gif"))
     else:
         print("\nThe files are saved at '{}'.".format(destination_path))
             
         
 
 
-def voc_annotator(image_folder:str, labels_folder:str, destination_path:str=".",
-                  segmentation:bool=False, bbox:bool=True, class_names:tuple[str]=(),
-                  video_out:bool=False, vid_name:str="output.mp4", fps:int=24, size:tuple[int,int]=(640,640)) -> None:
+def voc_annotator(image_folder:str, labels_folder:str, destination_path:str, segmentation:bool,
+                  bbox:bool, class_names:tuple[str], file_name:str, size:tuple[int,int], video_out:bool, fps:int,
+                  gif_out:bool, duration_of_frame:int, loop:int) -> None:
         
     assert (bbox and segmentation) or bbox or segmentation, "Either segmentation or bbox must be True or both may be True."
     assert os.path.isdir(image_folder) and os.path.isdir(labels_folder), "images_folder and labels_folder must be a directory."
-    assert vid_name[-4:] == ".mp4", "video_name must be in mp4 format."
+    assert file_name[-4:] in [".mp4",".gif"], "video_name must be in .gif or .mp4 format."
 
     print("\nAnnotation Validator in progress.....")
 
     cls = voc_validator(image_folder,labels_folder)
 
     print("\nAnnotation in progress...........\n")
 
     if video_out:
-        vid_wr = cv2.VideoWriter(os.path.join(destination_path, vid_name), cv2.VideoWriter.fourcc(*"mp4v"),
+        vid_wr = cv2.VideoWriter(os.path.join(destination_path, file_name[:-4]+".mp4"), cv2.VideoWriter.fourcc(*"mp4v"),
                                  fps, size)
+    
+    elif gif_out:
+        gif_wr = iio.get_writer(os.path.join(destination_path,file_name[:-4]+".gif"), mode="I", duration=duration_of_frame, loop=loop) 
+
 
     for file in tqdm.tqdm(os.listdir(labels_folder)):
         if file.endswith(".xml"):
             tree = et.parse(os.path.join(labels_folder,file))
-            file_name = tree.find("filename").text
-            img = cv2.imread(os.path.join(image_folder, file_name))
+            f_name = tree.find("filename").text
+            img = cv2.imread(os.path.join(image_folder, f_name))
                 
             for ann in tree.findall("object"):
                 classes = ann.find("name").text
 
                 if class_names != () and classes not in class_names:
                     continue
 
@@ -250,21 +237,30 @@
                     xmax = int(rd_bbox.find("xmax").text)
                     ymax = int(rd_bbox.find("ymax").text)
                     img = annot_bbox(img, [xmin, ymin, xmax, ymax], annot_color(cls.index(classes)), 2, classes, 1)
 
             if video_out:
                 img = cv2.resize(img, size)
                 vid_wr.write(img)
+            
+            elif gif_out:
+                img = cv2.resize(img, size)
+                gif_wr.append_data(cv2.cvtColor(img,cv2.COLOR_BGR2RGB))
+
             else:
-                cv2.imwrite(os.path.join(destination_path, file_name), img)
+                cv2.imwrite(os.path.join(destination_path, f_name), img)
     
     if video_out:
         vid_wr.release()
+    elif gif_out:
+        gif_wr.close()
     
     print("\nSave Completed.")
 
     print("\nThe annotation process is Completed.")
 
     if video_out:
-        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, vid_name))
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".mp4"))
+    elif gif_out:
+        print("\nThe files are saved at '{}' named '{}'.".format(destination_path, file_name[:-4]+".gif"))
     else:
         print("\nThe files are saved at '{}'.".format(destination_path))
```

### Comparing `helpers_ai-0.0.2/helpers_ai/annotator/video_convertor.py` & `helpers_ai-0.0.3/helpers_ai/annotator/video_convertor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tqdm
 import imageio as iio
 from dateutil import relativedelta
 
 
 
 
-def vid2img(video_path:str, destination_path:str=".", size:tuple[int,int]=None) -> None:
+def vid2img(video_path:str, destination_path:str, size:tuple[int,int]) -> None:
 
     assert os.path.isfile(video_path), "video_path must be a path to a video file."
 
     vid = cv2.VideoCapture(video_path)
 
     total_length = int(vid.get(cv2.CAP_PROP_FRAME_COUNT))
     vid_fps = int(vid.get(cv2.CAP_PROP_FPS))
@@ -34,16 +34,16 @@
     print(f"\nA Total of \033[1m\033[4m{total_length} images\033[0m has been extracted.")
 
     print("\nThe Extracted images are saved at '{}'.".format(destination_path))
 
 
 
 
-def fps_changer(video_path:str, fps:int, destination_path:str=".", filename:str=None,
-                size:tuple[int,int]=None, is_fast:bool=False) -> None:
+def fps_changer(video_path:str, fps:int, destination_path:str, filename:str,
+                size:tuple[int,int], is_fast:bool) -> None:
 
     assert os.path.isfile(video_path), "video_path must be a path to a video file."
 
     vid = cv2.VideoCapture(video_path)
 
     if size is None:
         size = (int(vid.get(cv2.CAP_PROP_FRAME_WIDTH)), int(vid.get(cv2.CAP_PROP_FRAME_HEIGHT)))
@@ -58,15 +58,15 @@
     vid_time = relativedelta.relativedelta(seconds=(total_length//vid_fps))
 
     if fps is None:
         fps = vid_fps
 
     print(f"\nThe video FPS : \033[1m\033[4m{vid_fps} fps\033[0m .")
 
-    assert fps <= vid_fps and fps > 0, "fps must be less than video fps"
+    assert (not is_fast and fps > vid_fps) or (is_fast and fps <= vid_fps and fps > 0), "'is_fast' must be set to false if 'fps' is greater than video fps."
 
     vid_wr = cv2.VideoWriter(os.path.join(destination_path, filename), cv2.VideoWriter.fourcc(*"mp4v"), fps, size)
 
     step = vid_fps//fps
 
     if is_fast and step > 1:  
         spots = list(range(0,total_length,step))
@@ -95,16 +95,16 @@
     print(f"\nA Total of \033[1m\033[4m{total_length//step if is_fast and step > 1 else 0} images\033[0m has been dropped from the video.")
 
     print("\nThe Converted video is saved at '{}' named '{}'.".format(destination_path, filename))
 
 
 
 
-def vid_cropper(video_path:str, start_time:str, end_time:str, destination_path:str=".",
-                filename:str=None, fps:int=None, size:tuple[int,int]=None) -> None:
+def vid_cropper(video_path:str, start_time:str, end_time:str, destination_path:str,
+                filename:str, fps:int, size:tuple[int,int]) -> None:
 
     assert os.path.isfile(video_path), "video_path must be a path to a video file."
     assert len(start_time.strip().split(":")) == 3 and len(end_time.strip().split(":")) == 3, "start_time and end_time must be in h:m:s format."
 
     st_hr, st_mnt, st_sec= start_time.strip().split(":")
     ed_hr, ed_mnt, ed_sec= end_time.strip().split(":")
     test = st_hr+st_mnt+st_sec+ed_hr+ed_mnt+ed_sec
@@ -149,15 +149,15 @@
     start_frame = start_second*vid_fps
     end_frame = end_second*vid_fps
 
     for i in tqdm.tqdm(range(total_length)):
         
         ret, frame = vid.read()
         
-        if i >= start_frame and i < end_frame and ret:
+        if i >= start_frame and i <= end_frame and ret:
             if size is not None:
                 frame = cv2.resize(frame, size)
 
             vid_wr.write(frame)
         
         elif i == end_frame:
             break
@@ -170,19 +170,24 @@
     print("\nA Total duration of cropped video : [ {}:{}:{} ]".format(crp_vid_time.hours, crp_vid_time.minutes, crp_vid_time.seconds))
 
     print("\nThe Cropped video is saved at '{}' named '{}'.".format(destination_path, filename))
 
             
 
 
-def vid2gif(video_path:str, destination_path:str=".", filename:str="output-video.gif", size:tuple[int,int]=None,
-            duration_of_frame:int=100, loop:int=0) -> None:
+def vid2gif(video_path:str, destination_path:str, filename:str, size:tuple[int,int],
+            duration_of_frame:int, loop:int) -> None:
     
+    print(size)
     assert os.path.isfile(video_path), "video_path must be a path to a video file."
-    assert filename[-4:] == ".gif", "filename must endswith '.gif' extensions."
+
+    if filename is not None:
+        assert filename.endswith(".gif"), "filename must ends with '.gif'."
+    else:
+        filename = video_path.split("/")[-1][:-4]+".gif"
 
     vid = cv2.VideoCapture(video_path)
 
     if size is None:
         size = (int(vid.get(cv2.CAP_PROP_FRAME_WIDTH)), int(vid.get(cv2.CAP_PROP_FRAME_HEIGHT)))
 
     total_length = int(vid.get(cv2.CAP_PROP_FRAME_COUNT))
@@ -190,15 +195,15 @@
     tot_sec = (total_length//vid_fps)
     vid_time = relativedelta.relativedelta(seconds=tot_sec)
 
     print("\nTotal time of the video : [ {}:{}:{} ]\n".format(vid_time.hours, vid_time.minutes, vid_time.seconds))
 
     with iio.get_writer(os.path.join(destination_path,filename), mode="I", duration=duration_of_frame, loop=loop) as writer:
 
-        for i in tqdm.tqdm(range(total_length)):
+        for _ in tqdm.tqdm(range(total_length)):
 
             ret, frame = vid.read()
             if ret:
                 if size is not None:
                     frame = cv2.resize(frame, size)
 
                 writer.append_data(cv2.cvtColor(frame,cv2.COLOR_BGR2RGB))
```

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/coco2voc.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/coco2voc.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/coco2yolo.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/jm2mmocr.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/jm2mmocr.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/voc2coco.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/voc2coco.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/voc2yolo.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/voc2yolo.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/yolo2coco.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/yolo2coco.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/dataset_convertors/yolo2voc.py` & `helpers_ai-0.0.3/helpers_ai/dataset_convertors/yolo2voc.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/losses.py` & `helpers_ai-0.0.3/helpers_ai/losses.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/utils/jm2mm.py` & `helpers_ai-0.0.3/helpers_ai/utils/jm2mm.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/utils/util.py` & `helpers_ai-0.0.3/helpers_ai/utils/util.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/utils/validator.py` & `helpers_ai-0.0.3/helpers_ai/utils/validator.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/helpers_ai/utils/voc.py` & `helpers_ai-0.0.3/helpers_ai/utils/voc.py`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/LICENSE` & `helpers_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helpers_ai-0.0.2/pyproject.toml` & `helpers_ai-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2268 656c 7065 7273 2d61  ame = "helpers-a
 00000020: 6922 0d0a 7665 7273 696f 6e20 3d20 2230  i"..version = "0
-00000030: 2e30 2e32 220d 0a64 6573 6372 6970 7469  .0.2"..descripti
+00000030: 2e30 2e33 220d 0a64 6573 6372 6970 7469  .0.3"..descripti
 00000040: 6f6e 203d 2022 4974 2063 6f6e 7461 696e  on = "It contain
 00000050: 7320 6665 7720 6865 6c70 696e 6720 6669  s few helping fi
 00000060: 6c65 7320 7768 6963 6820 6865 6c70 7320  les which helps 
 00000070: 696e 2074 6865 2070 726f 6365 7373 206f  in the process o
 00000080: 6620 6372 6561 7469 6e67 2061 6e20 4149  f creating an AI
 00000090: 2070 726f 6a65 6374 2e22 0d0a 6175 7468   project."..auth
 000000a0: 6f72 7320 3d20 5b22 414b 203c 616b 696c  ors = ["AK <akil
@@ -54,8 +54,11 @@
 00000350: 0d0a 696d 6167 6569 6f20 3d20 225e 322e  ..imageio = "^2.
 00000360: 3334 2e30 220d 0a0d 0a0d 0a5b 6275 696c  34.0"......[buil
 00000370: 642d 7379 7374 656d 5d0d 0a72 6571 7569  d-system]..requi
 00000380: 7265 7320 3d20 5b22 706f 6574 7279 2d63  res = ["poetry-c
 00000390: 6f72 6522 5d0d 0a62 7569 6c64 2d62 6163  ore"]..build-bac
 000003a0: 6b65 6e64 203d 2022 706f 6574 7279 2e63  kend = "poetry.c
 000003b0: 6f72 652e 6d61 736f 6e72 792e 6170 6922  ore.masonry.api"
-000003c0: 0d0a                                     ..
+000003c0: 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574  ......[tool.poet
+000003d0: 7279 2e73 6372 6970 7473 5d0d 0a68 656c  ry.scripts]..hel
+000003e0: 7065 7220 3d20 2268 656c 7065 7273 5f61  per = "helpers_a
+000003f0: 692e 5f5f 6d61 696e 5f5f 3a63 6c69 22    i.__main__:cli"
```

### Comparing `helpers_ai-0.0.2/PKG-INFO` & `helpers_ai-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpers-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: It contains few helping files which helps in the process of creating an AI project.
 License: AGPL-3.0-or-later
 Author: AK
 Author-email: akilangms542@gmail.com
 Maintainer: AK
 Maintainer-email: akilangms542@gmail.com
 Requires-Python: >=3.11
@@ -24,15 +24,15 @@
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: torch (==2.2.2)
 Requires-Dist: torchvision (==0.17.2)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Helpers
-contains some useful helper functions for ML.
+Contains some useful helper functions for ML. It is now available in cli operatable command for ease access.
 
 # Installation
 
 Install directly through pip using the command below,
 ```
 pip install helpers-ai
 ```
@@ -42,8 +42,7 @@
 git clone https://github.com/code63ReaPer/helpers-ai.git
 ```
 then install the package through pip using the command below,
 ```
 cd helpers-ai
 pip install .
 ```
-
```

