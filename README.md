# Task-through-Blink-EYE
This Python script detects eyes using OpenCV's Haar cascades and automates tasks in the browser based on eye blinks. When you blink your left eye, then it automatically run the youTube and Similarly, when you blink your right eye, the it will open the google for you 

# Requirements
+ Python 3.x
+ OpenCV (```pip install opencv-python```)
+ PyAutoGUI (```pip install pyautogui```)

# Setup
+ Install Python 3.x from python.org.
+ Install required dependencies: -  ```pip install opencv-python pyautogui```


# Usage
+ Run the script eye_detection.py.
+ Position yourself in front of the camera with adequate lighting.
+ Blink your left eye to open a specific YouTube video.
+ Blink your right eye to open Google in a browser.

# Code Explanaition
+ The script captures video from the default camera (cap = cv2.VideoCapture(0)).
+ It detects faces and eyes using Haar cascades (face_cascade and eye_cascade).
+ Eye blinks are detected by counting frames where the eyes are closed.
+ pyautogui is used to simulate key presses to open URLs in a browser.

# Configuration
+ Adjust blink_threshold in the script to control sensitivity to eye blinks.
+ Ensure proper lighting and camera setup for accurate detection.

# Notes 
+ This script uses OpenCV for face and eye detection.
+ pyautogui is employed for simulating keyboard inputs to open URLs in a browser.
+ The program terminates upon pressing 'q' in the window displaying the video feed.
