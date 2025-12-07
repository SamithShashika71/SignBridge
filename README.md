# 🧏‍♂️ SignBridge — Real-Time Sri Lankan Sign Language (SLSL) Translation App  
### *Final Year Software Engineering Capstone Project – Group 36*  

SignBridge is an AI-powered **two-way communication mobile application** designed to bridge the gap between **Sri Lankan Sign Language (SLSL) users** and the general public.  

It provides **real-time Sign-to-Text** and **Text-to-Sign** translation using **AI-powered gesture recognition**, **LSTM models**, and a **3D animated avatar** to display SLSL gestures accurately.

This is **Sri Lanka’s first mobile application** to support *both* real-time SLSL gesture recognition and 3D avatar-based reverse translation.

---

## ✨ Key Features

- **Real-time Gesture Recognition** — Uses hand and pose landmark detection for accurate sign classification.  
- **AI-Powered Inference** — Machine learning model (LSTM) to predict sign language gestures reliably.  
- **3D Avatar Rendering** — Animated 3D avatar for clear Text-to-Sign translation.  
- **Cross-Platform Mobile App** — Built with Flutter for wide device compatibility.  
- **Support for Static & Dynamic Signs** — Covers static alphabet gestures and dynamic multi-frame signs.  
- **Extensible Design** — Architecture allows scaling to phrase-level translation, other regional sign languages, and future enhancements.  

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|--------------|
| **Mobile App** | Flutter, Dart |
| **Backend / ML Server** | Python, MediaPipe, TensorFlow / LSTM, Flask API |
| **3D Animation & Avatar** | Blender (modeling & rigging), 3D asset export |
| **Data Processing** | NumPy, OpenCV, custom preprocessing pipelines |
| **Communication** | HTTP / WebSocket API for real-time inference & response |

---

## 🏗 System Architecture

![WhatsApp Image 2025-11-23 at 16 47 51_dc6c75a8](https://github.com/user-attachments/assets/0bebd1ae-d855-494d-982c-8a7f4f47fda6)

---

## 📁 Project Structure

        signbridge/
        ├── backend/ # ML model, preprocessing, Flask API
        │ ├── models/ # Trained LSTM model & checkpoints
        │ ├── preprocessing/ # Landmark extraction & data cleaning
        │ ├── api.py # REST / WebSocket endpoints
        │ └── requirements.txt
        │
        ├── mobile_app/ # Flutter project
        │ ├── lib/ # App source code
        │ ├── assets/ # Avatar assets, configuration
        │ └── pubspec.yaml
        │
        ├── avatar/ # 3D model & animations (Blender files / exports)
        │ └── <.blend, .glb, .json animation data>
        │
        └── README.md # Project documentation


---

## 🔄 Figma Prototype — UI / UX Design  

You can interact with the full prototype and test UI flows directly.  
[View the SignBridge Figma Prototype →](https://www.figma.com/design/7mUHZcsbdboePbW8VL9qIq?node-id=0-1)


---

## 🚀 How to Run / Setup  

### 1. Backend (Gesture Recognition API)  
        ```bash
        cd backend
        pip install -r requirements.txt
        python api.py         # Starts Flask server for real-time inference


### 2. Flutter Mobile App
        cd mobile_app
        flutter pub get
        flutter run           # Runs the app on connected device / emulator


### 3. Avatar Animations
        assets/avatar/

---

### ✅ Achievements & Impact

* First SLSL translator app combining real-time recognition + avatar-based reverse translation.
* Demonstrated success in departmental demo/testing.
* Provides accessible communication tools for hearing-impaired community in Sri Lanka.

---

### 🔮 Future Enhancements

* Expand Dataset: Include more signers, lighting conditions, and backgrounds to improve accuracy.
* Larger Vocabulary: Add more signs and support sentence-level recognition.
* Better Dynamic Gesture Recognition: Use advanced models (e.g., transformers, CNN-LSTM) for continuous gesture tracking.
* Multi-Language Output: Translate SLSL into Sinhala, Tamil, and English.
* Voice Output: Convert recognized signs into spoken audio for better accessibility.

---

### 👥 Team — Group 36

        Name	                          Role / Contribution
        -----------------------------------------------------------------------------------------------------
        P.B.B. Balasuriya (22UG1-0463) -  Dataset creation, preprocessing, and MediaPipe landmark extraction.
                                          LSTM model training and optimization.
                                          Flask backend development and integration.
        
        
        U.S. Shashika (22UG1-0495)     -  Mobile UI/UX design, select color themes and olayouts. 
                                          App logo design, creation and Flutter app development.
                                          Assisted with avatar pose correction and animation adjustments.
        
        U.R. Samarappuli (22UG1-0465)	- Designed and rigged the 3D avatar in Blender.
                                          created SLSL gesture animations and integrated avatar system .
                                          Supported Flutter app development.

Supervisor: Ms. Nilupuli Ekanayake

---

### 🪪 License

This project is licensed under the MIT License.

---

### 🙌 Credits

Developed by Team SignBridge (Group 36) to advance accessibility through AI-powered Sri Lankan Sign Language recognition and interactive 3D avatar visualization.

Built with ❤️ using Flutter, MediaPipe, LSTM deep learning, Flask, and 3D animation technologies.
