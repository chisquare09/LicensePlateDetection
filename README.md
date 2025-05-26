# Vietnamese License Plate Detection System

A machine learning project for detecting and recognizing Vietnamese license plates using YOLOv8 for object detection and EasyOCR/PyTesseract for OCR.

## ✨ Features
- **High-Accuracy Detection**: YOLOv8 model achieves 99% precision and 100% recall.
- **OCR Integration**: Supports both EasyOCR (84% accuracy) and PyTesseract.
- **Preprocessing Pipeline**: Resizing, noise removal, contrast enhancement, and edge detection.
- **Custom Dataset**: 550 manually collected and labeled Vietnamese license plate images.

## 🔧 Project Pipeline
1. **Data Collection**: 550 images with varied angles, brightness, and positions.
2. **Preprocessing**:
   - Resize images to 640x640.
   - Label using Roboflow Annotate.
   - Split dataset (80% train, 10% validation, 10% test).
3. **Object Detection**: Train YOLOv8 model (`yolov8n.pt`) for license plate localization.
4. **Image Processing**: Enhance contrast, remove noise, and sharpen edges.
5. **OCR**: Extract text using EasyOCR or PyTesseract.
6. **Evaluation**: Metrics include Precision, Recall, mAP50, CER, and Accuracy.

## 📥 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/chisquare09/LicensePlateDetection.git
   cd LicensePlateDetection
