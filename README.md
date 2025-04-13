# 🦺 PPE Detection using YOLOv9

![YOLOv9](https://img.shields.io/badge/YOLOv9-Real--Time--Detection-blue?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.8%2B-yellow?style=for-the-badge)
![License](https://img.shields.io/github/license/yourusername/PPE-Detector-YOLOv9?style=for-the-badge)

A powerful and real-time **PPE (Personal Protective Equipment) Detection System** using the state-of-the-art **YOLOv9** architecture. Designed to identify helmets, safety vests, gloves, and masks in live video feeds or images — ensuring safety compliance across industrial, construction, and healthcare environments.

---

## 🚀 Features

- ⚡ Real-time PPE detection using YOLOv9
- 🧠 Detects multiple PPE items (helmet, vest, gloves, masks, etc.)
- 📹 Supports both image and live webcam input
- 📦 Lightweight and optimized for deployment
- 🛠️ Easily customizable to add more PPE classes

---

## 📸 Demo

https://user-images.githubusercontent.com/yourusername/demo_video.mp4

*(Insert a video/gif showing your model detecting PPE in real time)*

---

## 🧠 Model Architecture

This project uses the latest YOLOv9 model for detection, trained on custom-labeled PPE datasets. YOLOv9 offers:

- Transformer-enhanced architecture
- Higher accuracy and speed than YOLOv5/v8
- Better object localization in cluttered environments

---

## 🛠️ Installation

```bash
git clone https://github.com/yourusername/PPE-Detector-YOLOv9.git
cd PPE-Detector-YOLOv9
pip install -r requirements.txt
```

Make sure you have PyTorch and CUDA set up for GPU acceleration.

---

## 📂 Project Structure

```
PPE-Detector-YOLOv9/
├── weights/                 # Trained YOLOv9 weights
├── data/                    # Images / videos for testing
├── detections/              # Output images with bounding boxes
├── utils/                   # Helper scripts
├── detect.py                # Inference script
├── train.py                 # Training script
├── README.md
└── requirements.txt
```

---

## 🧪 Usage

### ▶️ Inference on Images

```bash
python detect.py --source data/sample.jpg --weights weights/ppe_yolov9.pt
```

### 🎥 Inference on Webcam

```bash
python detect.py --source 0 --weights weights/ppe_yolov9.pt
```

### 🏋️‍♂️ Training (if you want to retrain)

```bash
python train.py --data data/ppe.yaml --epochs 100 --weights yolov9.pt
```

---

## 📊 Dataset

- You can use [Roboflow](https://roboflow.com) or any annotated dataset with PPE labels.
- Ensure labels are YOLO format (`.txt` files with class and bbox coordinates).
- Sample classes: `helmet`, `glove`, `mask`, `vest`, `goggles`

---

## 📦 Requirements

- Python 3.8+
- PyTorch
- OpenCV
- numpy
- tqdm
- matplotlib
- (and YOLOv9-specific dependencies)

Install via:

```bash
pip install -r requirements.txt
```

---

## ✨ Future Work

- Add alert system (email/SMS when no PPE is detected)
- Integrate with CCTV systems
- Deploy as a web or mobile app using Flask/Streamlit or React Native
- Edge deployment (Jetson Nano / Raspberry Pi)

---

## 🤝 Contributing

Pull requests are welcome! Feel free to open issues or submit new features, bug fixes, or improvements.

---

## 📜 License

This project is licensed under the MIT License.

---

## 🌐 Connect with Me

- LinkedIn: [YourName](https://linkedin.com/in/yourprofile)
- Twitter: [@yourhandle](https://twitter.com/yourhandle)
- Portfolio: [yourportfolio.com](https://yourportfolio.com)

---
