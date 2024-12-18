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

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/auto-annotation-yolov8-sam.git
   cd auto-annotation-yolov8-samInstall the required dependencies:
pip install -r requirements.txt
Download the YOLOv8 model (yolov8n.pt) from Ultralytics GitHub.
Download or obtain the Segment Anything Model (SAM).
How to Use

Prepare Input Images: Place your input images in the images/ folder.
Generate YOLO and SAM Annotations: The SAM model will generate annotations for each image, saved in a text file. The YOLOv8 model will also provide predictions for the objects detected in the images.
Run the Tool: Use the tool to combine the SAM-generated annotations and YOLO predictions, producing an annotated output image.
Example of how to run the function:

image_path = 'path/to/your/image.jpg'
label_path = 'path/to/your/label.txt'  # SAM generated label file
output_path = 'path/to/output/image.jpg'
model_path = 'path/to/yolov8n.pt'  # YOLOv8 model
draw_yolo_labels_and_predictions(image_path, label_path, output_path, model_path=model_path, conf_threshold=0.25)
Output: The final image will be saved at the specified output path, with SAM-generated annotations (blue boxes and polygons) and YOLOv8 predictions (green bounding boxes) overlaid on the image.
Example Output:
Before Annotation:


This is the original image where objects are to be segmented and detected.

After Annotation:


This is the output image after SAM and YOLOv8 annotations are applied. The blue boxes represent SAM annotations, and the green boxes represent YOLOv8 predictions.
Customization

Confidence Threshold: Adjust the conf_threshold parameter to filter YOLOv8 predictions based on confidence. A value of 0.25 means that only predictions with at least 25% confidence will be displayed.
Label Customization: You can modify the position, size, and color of labels (for both SAM and YOLO annotations) using OpenCV’s text functions.
Contribution

We welcome contributions to improve the tool! If you have suggestions or improvements, feel free to submit a pull request or open an issue.

How to contribute:
Fork the repository.
Create a new branch for your changes.
Make your modifications.
Submit a pull request with a description of your changes.
License

This project is licensed under the MIT License - see the LICENSE file for more details.


