# License-Plate-Recognition-Using-CNN-and-OCR
# 🚗 License Plate Recognition Using Deep Learning

This project aims to build an end-to-end system for Automatic License Plate Recognition (ALPR) using deep learning. The task includes detecting license plates from vehicle images and recognizing the alphanumeric characters using OCR.

---

## 🎯 Objective

1. **License Plate Detection**: Locate the license plate in vehicle images using object detection.
2. **Character Recognition**: Recognize the alphanumeric text from cropped license plate images.

---

## 📦 Dataset Description

The dataset is divided into:

### 🔹 Training Set 1 – Vehicle Images with Bounding Boxes
- 900 images of vehicles
- Annotated with bounding box coordinates: `(ymin, xmin, ymax, xmax)`

### 🔹 Training Set 2 – License Plate Images with Text Labels
- 900 cropped license plate images
- Annotated with the full license plate text

### 🔹 Test Set
- 201 vehicle images (similar to Training Set 1)
- Tasks: Detect license plates and recognize their content

---

## 📊 Planned Workflow

### 1. 📂 Data Preprocessing
- Load and inspect all datasets
- Visualize sample images
- Check for missing values, invalid formats, or mislabeled entries
- Split data into training and validation sets

### 2. 🧠 Model Training
- Detection: YOLOv5 / SSD / Faster R-CNN
- OCR: CRNN or CNN-LSTM with CTC loss
- Custom dataset loaders and training loops

### 3. 🔍 Model Evaluation
- IoU-based accuracy for detection
- Character-level and full-text accuracy for OCR

### 4. 📤 Testing & Inference
- Run the full pipeline on the test set
- Save predicted bounding boxes and text to a CSV

---

## 🛠️ Tools & Libraries

- Python 3.x
- OpenCV
- PyTorch or TensorFlow
- YOLOv8 or similar detection architecture
- Tesseract ocr
- Pandas, NumPy, Matplotlib, Seaborn


