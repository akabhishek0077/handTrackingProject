# Hand Tracking and Detection using OpenCV & MediaPipe

This project demonstrates **real-time hand tracking** and **basic detection techniques** using **OpenCV** and **MediaPipe**.  
It includes:
- A reusable **Hand Tracking Module**
- A **testing script** to verify the module
- A simple **face detection script** using Haar Cascades

The project is suitable for beginners learning **computer vision**, **gesture recognition**, and **MediaPipe Hands**.

---

## 📁 Project Structure

├── HandTrackingModule.py # Reusable hand tracking class
├── testhtm.py # Testing file for hand tracking module
├── Handtracking.py # Basic hand landmark detection demo
├── detect.py # Face detection using Haar Cascade
├── README.md # Project documentation


---

## 🛠️ Technologies Used

- **Python 3**
- **OpenCV**
- **MediaPipe**
- **NumPy**
- **Haar Cascade Classifier**

---

## ✋ HandTrackingModule.py

This file contains a **custom hand tracking class** built using MediaPipe.

### Features
- Detects up to **2 hands**
- Tracks **21 hand landmarks**
- Returns landmark positions in pixel coordinates
- Optional drawing of landmarks and connections
- FPS display

Important Methods
Method	Description
findHands(img)	Detects hands and draws landmarks
findPosition(img)	Returns landmark ID with (x, y) coordinates

This module can be imported and reused in other projects.

---

## 🧪 testhtm.py (Testing File)

This script is used to test the HandTrackingModule.

Functionality

Captures webcam video

Uses handDetector class

Prints the position of landmark ID 4 (thumb tip)

Displays FPS and hand landmarks in real-time

Usage
python testhtm.py

---

## ✋ Handtracking.py (Basic Demo)

This is a standalone demonstration file showing:

Direct use of MediaPipe Hands

Drawing each landmark manually

Printing landmark IDs and coordinates

FPS calculation

Useful for understanding how MediaPipe works internally before modularization.

---

## 😀 detect.py (Face Detection)

This script performs real-time face detection using OpenCV’s Haar Cascade.

Features

Uses webcam feed

Converts frame to grayscale

Detects faces and draws rectangles

Press 's' key to stop execution

⚠️ Make sure the Haar Cascade XML file path is correct on your system.

---

## ▶️ How to Run

Install dependencies:

pip install opencv-python mediapipe

---

Run hand tracking test:

python testhtm.py

---

Run basic hand tracking demo:

python Handtracking.py

---

Run face detection:

python detect.py

## 📌 Applications

Gesture Recognition

Virtual Mouse / Keyboard

Sign Language Recognition

Human-Computer Interaction

AI-based Vision Projects

---

## 📷 Output Preview

Real-time hand landmark detection

Finger tracking with landmark IDs

FPS displayed on screen

Face detection bounding boxes

---

## 📜 License

This project is for educational purposes.
Feel free to modify and extend it.
