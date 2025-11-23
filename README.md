Eye Mouse

Eye Mouse is a hands-free cursor control system built with Python. It uses MediaPipe Face Mesh to track face landmarks in real time and moves the mouse pointer using the position of the nose. A simple left-eye blink is used to trigger mouse clicks. The project runs entirely on a webcam and requires no external hardware.

Features

Cursor movement using nose tracking

Blink-based left-click

Real-time detection using Face Mesh

Works with any standard webcam

Lightweight and easy to customize

Requirements

Python 3.7+

Webcam

Install required libraries:

pip install opencv-python mediapipe pyautogui

How It Works

MediaPipe Face Mesh detects 468+ facial landmarks

The script tracks a specific nose landmark to control cursor position

Two upper–lower eyelid points are monitored; when they come close, a click is triggered

The cursor position is mapped from webcam space to screen space

Usage

Clone the repository:

git clone https://github.com/yourusername/eye-mouse.git


Run the script:

python eye_mouse.py


Sit in front of your webcam and move your head gently.

Blink your left eye to click.

Tips

Works best with stable lighting

Keep your face centered in the camera frame

Avoid rapid head movements for smoother control

File Overview

eye_mouse.py — Main script for nose-tracking and blink-click control

License

This project is available under the MIT License.
