# AI Object Detection Portal using YOLOv8 and OpenCV

An interactive object detection portal that uses **YOLOv8** to detect objects from uploaded **images and videos** through a single, user-friendly workflow.

## Project Overview

This project extends traditional YOLOv8 object detection into an interactive web-based portal using **Gradio**.

Instead of maintaining separate image and video workflows, the portal accepts a single uploaded file and automatically determines whether it is an image or a video. YOLOv8 then performs object detection and generates an annotated result with bounding boxes, object labels, and confidence scores.

## Key Features

* Upload either an image or video through a single interface
* Automatically identify the uploaded file type
* Detect objects using the pretrained YOLOv8 model
* Display bounding boxes, object labels, and confidence scores
* Process videos frame by frame
* Generate annotated image and video outputs
* Interactive web interface built with Gradio
* Simple and user-friendly detection workflow

## Workflow

```text
Upload Image / Video
        ↓
Automatic File Type Detection
        ↓
       YOLOv8
        ↓
Object Detection
        ↓
Annotated Image / Video
        ↓
Object Labels + Confidence Scores
```

## Technologies Used

* Python
* YOLOv8
* Ultralytics
* OpenCV
* Gradio
* Google Colab

## Model

The project uses the **pretrained YOLOv8n model** from Ultralytics for object detection.

The model is used directly for inference without custom training.

## Output

For images, the portal generates:

* Bounding boxes around detected objects
* Object names
* Confidence scores

For videos, the system:

* Processes the video frame by frame
* Applies YOLOv8 detection to each frame
* Generates an annotated output video

## Interactive Portal

The detection interface was developed using **Gradio**, providing a simple web-based workflow for uploading an image or video and viewing the detection results.

> The current Gradio interface is used for development and demonstration. A permanent public deployment using Hugging Face Spaces is planned as a future enhancement.

## Project Structure

```text
Obstacle-Detection-Using-YOLOv8-and-OpenCV/
│
├── Obstacle_Detection_YOLO.ipynb
├── requirements.txt
├── README.md
├── output/
└── screenshots/
```

## How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Open the notebook

Open:

```text
Obstacle_Detection_YOLO.ipynb
```

using Google Colab or Jupyter Notebook.

### 3. Load the YOLOv8 model

```python
from ultralytics import YOLO

model = YOLO("yolov8n.pt")
```

### 4. Run the detection portal

Execute the Gradio application cells and upload an image or video through the interface.

## Sample Results

The project includes sample detection outputs and screenshots demonstrating YOLOv8 object detection on images and videos.

## Future Enhancements

* Deploy the Gradio application permanently using Hugging Face Spaces
* Improve the web interface and result visualization
* Add downloadable detection results
* Support additional YOLO models and custom-trained datasets

## Author

**Archana Ramesh**

B.Tech (Hons.) Artificial Intelligence & Data Science
Velammal Institute of Technology
