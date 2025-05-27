🚗 Blink, Pause, Alert: Intelligent Drowsiness Detection for Safer Journeys

A real-time driver drowsiness and yawning detection system using deep learning and computer vision to enhance road safety.
📌 Overview

Drowsiness is one of the major contributors to road accidents. This project implements a non-intrusive, real-time monitoring system that uses facial landmarks to detect driver fatigue based on eye closure (EAR) and yawning (MAR).

When the system detects signs of fatigue, an audio alert is triggered, helping drivers stay attentive and avoid potential accidents.
👨‍💻 Authors

    Shambhavi Palak

    Somraj Bose

    Ayush Sandilya

    Sounak Dutta

    Divyam

Under the guidance of Prof. Anil Kumar Swain
School of Computer Engineering, KIIT University
📷 Features

    Real-time webcam video stream analysis

    Facial landmark detection using dlib

    Eye Aspect Ratio (EAR) for drowsiness detection

    Mouth Aspect Ratio (MAR) for yawning detection

    Audio alert system using playsound

    Deep learning (CNN) based classification

    GUI for visualization and user interaction

🧠 Technologies Used

    Python

    OpenCV

    dlib

    TensorFlow / Keras

    imutils

    NumPy

    playsound

    scikit-learn

    pickle

🛠️ Installation

    Clone the repository:

git clone https://github.com/your-username/drowsiness-detection.git
cd drowsiness-detection

Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows

Install the required libraries:

    pip install -r requirements.txt

📂 Folder Structure

DROWSINESS DETECT/
├── models/
│   └── drowsiness_model.h5
├── utils/
│   └── landmark_utils.py
├── main.py
├── requirements.txt
├── README.md
└── assets/
    └── sample_images/

    You may need to adjust the paths if your structure differs.

▶️ Usage

    Run the main script:

    python main.py

    The system will activate your webcam. Stay in front of the camera.

    If the EAR goes below 0.25 for 20 frames or MAR exceeds 0.6 for 20 frames, an alert will be triggered.

✅ Test Cases
Test Condition	Expected Result
Eyes open, front-facing (with/without glasses)	Not Drowsy
Eyes closed for > 20 frames	Drowsy
Yawning for > 20 frames	Drowsy
Side facing with eyes open	Not Drowsy
📈 Model Performance (CNN)
Metric	Training	Testing
Precision	0.81	0.81
Recall	0.81	0.81
F1-Score	0.81	0.81
Accuracy	-	93.2%
📦 Future Enhancements

    Integration with IoT sensors for physiological data (e.g., HRV, GSR)

    Cloud-based alert systems and analytics dashboard

    Deployment on Raspberry Pi / Jetson Nano

    Adaptive thresholds based on driver profile

📜 License

This project is for academic use only. Licensing details can be provided upon request.
