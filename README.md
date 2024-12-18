# AI-Image-Labeler

## Project Overview
The **Auto Annotation using YOLOv8 and SAM** project aims to streamline the process of annotating images using automatic segmentation and object detection. By combining the **Segment Anything Model (SAM)** for segmentation and **YOLOv8** for object detection, this project provides an efficient way to automatically generate annotations for images. The SAM model generates annotations in the form of bounding boxes and polygons, while YOLOv8 is used for object detection and labeling. This tool is designed for improving the efficiency of image annotation workflows in tasks like object detection and segmentation.

## Features
- **Automatic Image Annotation:** Combines SAM-generated segmentations with YOLOv8 predictions for comprehensive image annotations.
- **SAM Segmentation Labels:** The SAM model generates segmentation labels for objects in the image.
- **YOLOv8 Object Detection:** YOLOv8 detects objects and overlays bounding boxes with class names and confidence scores.
- **Customizable Label Formatting:** Customize the position, size, and font of labels.
- **Image Visualization:** Displays the input image with both SAM-generated and YOLO model annotations overlaid.

## Requirements
- Python 3.x
- OpenCV
- NumPy
- `ultralytics` (for YOLOv8)
- `torch` (for YOLO model)
- **Segment Anything Model (SAM)**

### Example Output:  
**Before Annotation:**  

![dog1](https://github.com/user-attachments/assets/b36808df-e5b2-43f1-839d-d9abb4348016)  
This is the original image where objects are to be segmented and detected.  

**After Annotation:**  

![dog1_annotated](https://github.com/user-attachments/assets/2e9c2d7e-4210-4189-ad09-546b67646e2a)  



This is the output image after SAM and YOLOv8 annotations are applied. The blue boxes represent SAM annotations, and the text represent YOLOv8 predictions.


This project is licensed under the MIT License - see the LICENSE file for more details.


