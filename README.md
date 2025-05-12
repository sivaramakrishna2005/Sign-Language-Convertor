# Hand Gesture Recognition with MediaPipe and OpenCV

This project utilizes MediaPipe and OpenCV to detect and recognize hand gestures using a webcam. It includes two versions:

1. **Hand Gesture Recognition with Speech Output**: Recognizes hand gestures and provides vocal feedback using `pyttsx3`.
2. **Hand Gesture Recognition (without Speech)**: Detects and displays recognized gestures visually on the screen.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Supported Gestures](#supported-gestures)
- [Technologies](#technologies)


## Installation

To run this project, ensure that you have Python installed (Python 3.6+ recommended).

### Dependencies

Install the required libraries using `pip`:

pip install opencv-python mediapipe pyttsx3

## Usage
1. Hand Gesture Recognition with Speech Output
The script uses a webcam to detect hand gestures.
When a gesture is recognized, it speaks the corresponding gesture name (e.g., "Thanks", "Yes", "I Love You").
It also displays the recognized gesture number or name on the video feed.
To run the script, execute the following command: python gesture_recognition_with_speech.py

2. Hand Gesture Recognition (without Speech)
This script detects hand gestures and displays the recognized gesture as text on the video feed.
Press the q key to exit the application.
To run the script, execute the following command: python RSLD 1.py


## Features
Real-time hand gesture detection using MediaPipe.
Gesture-to-number mapping (0-9) and custom gestures ("Thanks", "Yes", "I Love You", etc.).
Speech output for recognized gestures (in the version with speech).
Simple and efficient use of threading for speech synthesis.
Real-time display of the recognized gesture on the webcam feed.


## Supported Gestures
The following gestures are recognized:

Numbers 0-5: Open and closed finger combinations.

Numbers 6-9: Based on thumb proximity to other fingers.

Custom Gestures:

"Thanks" (Thumb, index, and middle fingers open, ring and pinky closed).

"Yes" (Thumb extended, other fingers closed).

"No" (Thumb and index extended, other fingers closed).

"I Love You" (Thumb, index, and pinky extended).

"Sorry" (Thumb and pinky extended, other fingers closed).

## Technologies
MediaPipe: A cross-platform framework for building multimodal applied machine learning pipelines, used here for hand tracking and gesture recognition.

OpenCV: A library used for computer vision, used here to capture video frames and display results.

pyttsx3: A Python library used for text-to-speech conversion in the version with speech feedback.
