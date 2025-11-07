Blink Alert 🚨: Real-Time Blink & Drowsiness Detection

Stay alert and safe! A real-time Python system to detect eye blinks and drowsiness using OpenCV and dlib.

Features

✅ Detects blinks in real-time

✅ Monitors eye aspect ratio (EAR) to identify drowsiness

✅ Alerts the user if drowsy for prolonged frames

✅ Uses Python, OpenCV, and dlib (no heavy ML/DL models required)

✅ Works on any webcam


Download dataset from https://huggingface.co/matt3ounstable/dlib_predictor_recognition/blob/main/shape_predictor_68_face_landmarks.dat 


Technologies Used

Python 🐍

OpenCV

dlib

imutils

NumPy

This project implements a real-time eye drowsiness detection system using Python, OpenCV, Dlib, and Numpy. The program captures video from the webcam, detects the user's face and eyes, and calculates the eye aspect ratio (EAR) to monitor drowsiness levels based on eye blinks or whether they are blinking at the moment. You can customize parameters such as the number of frames for which the user appears to be dull, which when exceeded triggers a drowsy alert, the minimum eye aspect ratio, below which the user is perceived to be blinking, and the minimum eye aspect ratio for drowsiness which allows the program more leeway to detect whether a user has sustained droopy eyelids.

Crux of the program:
Video Capture: Opens the webcam and reads frames.
Face Detection: Uses Dlib's frontal face detector to locate faces in the frame.
Eye Aspect Ratio Calculation: For each detected face, computes the EAR for both eyes.
Drowsiness Detection:
Displays a message if the user is found to be blinking.
Increments a counter if the user appears drowsy.
If drowsiness is detected for more than the allowed frames, an alert is displayed and the counter reset.
Real-time Display: Shows the live feed with contours around the eyes and messages indicating the state of the user.
Exiting the Program: The application can be exited by pressing q.


<img width="784" height="429" alt="Screenshot 2025-11-07 161719" src="https://github.com/user-attachments/assets/d0980493-0ad8-4730-bbde-b7bc12ac9e2c" />








   
Running the script
Clone the Blinking-Detection repository:

❯ git clone https://github.com/Aryan-Chharia/Computer-Vision-Projects
Navigate to the project directory:

❯ cd 'Blinking and Drowsiness Detection'
Install the required dependencies:

❯ opencv-python, dlib, imutils, numpy
To run the project, execute the following command:

❯ python main.py
