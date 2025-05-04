# Golden_biometrics
Elderly Biometric Authentication System
🚀 Elderly Biometric Authentication System is an AI-powered solution that enhances security and accessibility for elderly individuals using face and voice recognition. It ensures seamless authentication for seniors by overcoming challenges such as facial aging, voice tremors, and biometric degradation.

📌 Project Overview
👵 Elderly Biometric Authentication System is a machine learning-based authentication tool that combines facial recognition and voice verification to provide a secure and user-friendly access system for elderly users. The system is built using deep learning models to handle aging-related changes in biometric features.

🛠️ Key Features:
✅ Multimodal Authentication – Uses face + voice for improved accuracy.
✅ Elder-Friendly Design – Handles wrinkles, expression variations, and vocal changes.
✅ Real-Time Enrollment & Authentication – Users can enroll and authenticate via webcam and microphone.
✅ Custom Thresholding – Adjusts biometric confidence levels based on age-related variations.
✅ Secure Data Handling – Ensures privacy compliance and encrypted biometric storage.
✅ Web-Based Interface – Powered by Streamlit, allowing easy access via a browser.

🚀 Technologies Used
The project leverages modern AI, ML, and deep learning techniques:

Programming & Frameworks
Python – Core programming language

Streamlit – For the interactive user interface

OpenCV – Face detection and processing

Librosa – Audio processing for voice authentication

Machine Learning & AI
TensorFlow/Keras – Deep learning framework

VGGFace – Pre-trained face recognition model

LSTM Model – Used for voice recognition

Fusion Model – Combining face and voice scores for authentication

📂 Project Structure
elderly_biometrics/
├── data/                  # Stores face and voice datasets
│   ├── face/              # Enrolled face images
│   ├── voice/             # Enrolled voice samples
│
├── models/                # Machine learning models
│   ├── face_model.py      # Face recognition module
│   ├── voice_model.py     # Voice recognition module
│   ├── fusion_model.py    # Multimodal authentication logic
│
├── utils/                 # Utility functions
│   ├── preprocess.py      # Preprocessing for face & voice
│
├── elderly_biometrics_streamlit.py  # Main Streamlit GUI script
├── train_voice_model.py   # Training script for voice model
├── requirements.txt       # Python dependencies
└── README.md              # Documentation


🎤 How It Works?
1️⃣ Enrollment (New User)
The user enters their name and clicks "Enroll".

The system captures their face using a webcam.

The system records a voice sample using the microphone.

The extracted biometric features are stored for future authentication.

2️⃣ Authentication (Returning User)
The user enters their name and clicks "Authenticate".

The system captures a live face image and voice sample.

The face and voice data are compared with the stored biometric template.

The system computes a similarity score and decides:

✅ Access Granted (if score is above threshold)

❌ Access Denied (if score is below threshold)

📊 Evaluation Metrics
The authentication system is optimized for elderly users, considering biometric changes over time. We use the following evaluation metrics:

False Acceptance Rate (FAR) – Incorrectly granting access.

False Rejection Rate (FRR) – Incorrectly denying access.

Equal Error Rate (EER) – Trade-off between FAR and FRR.

Confidence Thresholding – Adaptive for different users.

🚀 How to Run This Project
📦 Install Required Libraries

Make sure you have Python 3.7+ installed. Then install dependencies:pip install streamlit keras tensorflow opencv-python-headless numpy librosa soundfile sounddevice scikit-learn keras-vggface

Folder Structure (Create These If Missing)
project_root/
├── elderly_biometrics_app.py       # Main Streamlit app
├── models/                         # Trained voice model will be saved here
├── data/
│   ├── face/                       # Stores enrolled face images
│   └── voice/                      # Stores enrolled voice feature .npy files

▶️ Run the Streamlit App  : streamlit run elderly_biometrics_app.py




