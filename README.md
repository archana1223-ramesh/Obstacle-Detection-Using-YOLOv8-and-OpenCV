# 🚧 Real-Time Obstacle Detection using YOLOv8 and OpenCV

An AI-powered computer vision project that detects obstacles such as **people, cars, buses, trucks, bicycles, and motorcycles** from images and videos using the **YOLOv8** deep learning model. The system identifies objects, draws bounding boxes around them, and displays confidence scores, making it suitable for real-time obstacle detection applications.

---

## 📌 Project Overview

This project uses the pre-trained **YOLOv8** model from Ultralytics for object detection. Instead of training a model from scratch, it leverages transfer learning to detect common objects efficiently.

The project can process:

- 🖼️ Images
- 🎥 Videos
- 📦 Multiple objects in a single frame

---

## ✨ Features

- Detects multiple objects simultaneously
- Supports both image and video input
- Displays bounding boxes with confidence scores
- Built using Python, OpenCV, and YOLOv8
- Compatible with Google Colab
- Saves processed output automatically

---

## 🛠️ Technologies Used

- Python
- OpenCV
- YOLOv8
- Ultralytics
- Google Colab

---

## 📂 Project Structure

```
Obstacle-Detection-Using-YOLOv8-and-OpenCV/
│
├── Obstacle_Detection_YOLO.ipynb
├── README.md
├── requirements.txt
│
├── input/
│   ├── classroom.jpg
│   └── bike and car.mp4
│
├── output/
│   ├── classroom_output.png
│   └── bike_and_car_output.mp4
│
└── screenshots/
    ├── detection_image.png
    └── detection_video.png
```

---

## 🔄 Workflow

```
Input Image / Video
        │
        ▼
Load YOLOv8 Model
        │
        ▼
Detect Objects
        │
        ▼
Draw Bounding Boxes
        │
        ▼
Display Results
        │
        ▼
Save Output
```

---

## 📷 Sample Output

### Image Detection

<img src="screenshots/detection_image.png" width="700">

### Video Detection

<img src="screenshots/detection_video.png" width="700">

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/Obstacle-Detection-Using-YOLOv8-and-OpenCV.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

or

```bash
pip install ultralytics
pip install opencv-python
pip install matplotlib
```

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**.
2. Upload an image or video.
3. Run all notebook cells.
4. The processed output will be saved in:

```
runs/detect/predict/
```

---

## 📊 Detection Classes

The model can detect several common objects including:

- Person
- Car
- Bus
- Truck
- Bicycle
- Motorcycle

Each detected object is displayed with:

- Bounding Box
- Class Label
- Confidence Score

---

## 📈 Future Improvements

- Real-time webcam detection
- Distance estimation
- Obstacle warning system
- Object tracking
- Raspberry Pi deployment
- Lane detection integration

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👩‍💻 Author

**Archana Ramesh**

If you found this project useful, feel free to ⭐ the repository.
