# Face-Cam-Tracker
I used pythons built in face recognition and cv2 libraries to create an application that uses face recognition.

Webcam Face Recognition Tracker
Overview

The Webcam Face Recognition Tracker is a computer vision application that detects and tracks human faces in real time using a webcam. The system captures video input from a computer’s camera, identifies faces in each frame, and visually tracks them by drawing bounding boxes around detected faces.

This project demonstrates practical applications of computer vision and machine learning, including real-time object detection and video processing.

Features
Real-Time Face Detection

The program continuously captures frames from the webcam and analyzes them to detect faces.

Face Tracking

When a face is detected, the system:

Draws a bounding box around the face

Updates the position of the box as the person moves

Live Video Processing

Frames from the webcam are processed in real time to maintain continuous tracking.

Technologies Used

Python

OpenCV

NumPy

Computer Vision Algorithms

Webcam Video Capture

How It Works

The program accesses the computer’s webcam.

Video frames are captured continuously.

Each frame is converted to grayscale for faster processing.

A face detection model scans the frame.

If a face is detected:

A rectangle is drawn around it.

The face location is tracked across frames.

Project Structure

Example structure:

webcam-face-tracker/
│
├── face_tracker.py
├── haarcascade_frontalface_default.xml
└── README.md

face_tracker.py – Main program that runs the webcam tracker

haarcascade_frontalface_default.xml – Pre-trained face detection model

Installation
1. Install Python Dependencies
pip install opencv-python
pip install numpy
2. Download the Haar Cascade Model

Download the face detection model from the OpenCV repository and place it in the project folder.

File:

haarcascade_frontalface_default.xml
Running the Program

Run the script using Python:

python face_tracker.py

The webcam will open and begin detecting faces.

Press Q to close the program.

Example Output

When a face is detected, the program displays:

A rectangle around the detected face

Live tracking as the person moves

Applications

Face detection and tracking systems like this are used in:

Security systems

Attendance tracking

Human-computer interaction

Camera autofocus systems

Driver monitoring systems

Limitations

Accuracy can decrease in poor lighting conditions

Multiple faces may affect detection speed

Performance depends on webcam resolution and system hardware

Future Improvements

Possible enhancements include:

Implementing face recognition (identifying specific people)

Adding multiple face tracking

Integrating deep learning models

Improving accuracy using CNN-based detectors

Logging detected faces

Author

Trevor Grafton
