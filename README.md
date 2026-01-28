🚦 Integrated Cloud-Based Image Processing for Android and CCTV System

An AI-powered cloud-based traffic surveillance system for helmet violation detection and number plate recognition using YOLOv8, OCR, Android, and AWS EC2.

📌 Project Overview

Road safety enforcement is a major challenge due to manual monitoring and limited scalability.
This project introduces an automated, AI-driven, cloud-based surveillance system that detects helmet violations and extracts vehicle number plates from CCTV or mobile videos, enabling efficient traffic law enforcement.

The system integrates:

📱 Android Application for video upload & result viewing

☁️ Cloud backend hosted on AWS EC2

🤖 Deep learning models (YOLOv8 for detection, OCR for text extraction)

🗄️ Cloud databases (AWS RDS + Firebase)

🎯 Features

Automated helmet violation detection using YOLOv8

Automatic number plate recognition (ANPR) using EasyOCR / Tesseract

Android app for uploading CCTV or mobile videos

Cloud-based processing on AWS EC2 (GPU enabled)

Secure authentication with Firebase

Centralized cloud storage of violation records

Scalable architecture for smart city integration

Ready for e-challan and government database integration

🧠 System Architecture
Android App
     ↓
AWS S3 (Video Storage)
     ↓
AWS EC2 (Flask Backend + YOLOv8 + OCR)
     ↓
AWS RDS (PostgreSQL) + Firebase
     ↓
Results displayed in Android App

🛠️ Technology Stack
AI / Machine Learning

YOLOv8 (Ultralytics)

PyTorch

EasyOCR / Tesseract

OpenCV

Backend

Python

Flask (REST APIs)

Cloud

AWS EC2 (GPU instances)

AWS S3 (Storage)

AWS RDS (PostgreSQL)

AWS IAM

CloudWatch

Mobile App

Android (Java / Kotlin)

Firebase Authentication

Retrofit (API integration)

📂 Project Structure
Integrated-CLOUD-based-Image-Processing-for-Android-and-CCTV-System/
│
├── app.py                  # Flask backend
├── main.py                 # Detection pipeline
├── my_functions.py         # Helper functions
├── requirements.txt        # Dependencies
│
├── models/
│   ├── helment_no_helmet98.6.pth
│   └── rider_helmet_number_small.pt
│
├── videos/
│   ├── test.mp4
│   └── sample.mp4
│
├── output/
│   └── output.avi
│
└── README.md

⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/RiyaJadhao/Integrated-CLOUD-based-Image-Processing-for-Android-and-CCTV-System.git
cd Integrated-CLOUD-based-Image-Processing-for-Android-and-CCTV-System

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Run Backend
python app.py

4️⃣ Upload Video

Upload video from Android app or Postman

Backend processes video on AWS EC2

Detection results returned with bounding boxes and plate numbers

📱 Android App Features

Secure login (Firebase)

Upload CCTV or mobile videos

View helmet detection results

View number plate text

View history of violations

Cloud synced records

📊 Performance
Metric	Value
Helmet Detection Accuracy	~95%
Number Plate OCR Accuracy	~90%
Processing Speed	~1–1.5 sec/frame
Cloud Scalability	Auto-scaling enabled
🔐 Security

Firebase authentication

IAM role-based access

HTTPS APIs

Encrypted S3 & RDS

CloudWatch monitoring

🌍 Use Cases

Traffic police enforcement

Smart city surveillance

Automated e-challan systems

Highway monitoring

Accident prevention

Industrial helmet compliance

🚀 Future Enhancements

Live CCTV stream processing

Edge AI (Jetson / Raspberry Pi)

Speed & signal violation detection

AI-based traffic analytics dashboard

Government RTO API integration

