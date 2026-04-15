# 🚗 Drowsy Driving Detection System

## 📌 Project Overview

The **Drowsy Driving Detection System** is a computer vision-based application that detects driver fatigue in real-time using a webcam. It monitors eye movements and triggers an alert when the driver appears drowsy, helping prevent road accidents.

---

## 🎯 Features

* 👁️ Real-time eye detection using facial landmarks
* ⚠️ Detects drowsiness based on Eye Aspect Ratio (EAR)
* 🔔 Alarm alert when eyes remain closed for a long time
* 📹 Live video stream processing using webcam
* 🧠 Uses machine learning and computer vision techniques

---

## 🛠️ Technologies Used

* Python
* OpenCV
* Dlib
* NumPy
* Imutils
* Scipy

---

## ⚙️ How It Works

1. Captures video from webcam
2. Detects face using Dlib’s face detector
3. Extracts eye landmarks
4. Calculates **Eye Aspect Ratio (EAR)**
5. If EAR is below threshold for consecutive frames → triggers alarm

---

## 📂 Project Structure

```bash
drowsy-driving-detection/
│── detect_drowsiness.py
│── alarm.wav
│── shape_predictor_68_face_landmarks.dat
│── README.md
```

---

## ▶️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/drowsy-driving-detection.git
cd drowsy-driving-detection
```

### 2️⃣ Install Dependencies

```bash
pip install opencv-python dlib imutils numpy scipy playsound
```

### 3️⃣ Download Required File

Download the facial landmark model:
👉 http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

Extract and place it in the project folder

---

## ▶️ Usage

```bash
python detect_drowsiness.py --shape-predictor shape_predictor_68_face_landmarks.dat
```

(Optional with alarm)

```bash
python detect_drowsiness.py --shape-predictor shape_predictor_68_face_landmarks.dat --alarm alarm.wav
```

---

## 📊 Output

* Displays live video feed
* Shows **EAR value on screen**
* Triggers **"DROWSINESS ALERT!"** when fatigue is detected

---

## 🚀 Future Improvements

* Add mobile app integration
* Use deep learning for better accuracy
* Add head pose detection
* Deploy on embedded systems (Raspberry Pi)

---

## 👩‍💻 Author

**Koteswari Seelam**

* GitHub: https://github.com/seelamkoteswari
* LinkedIn: https://www.linkedin.com/in/koteswari

---

## 📜 License

This project is for educational and research purposes.
