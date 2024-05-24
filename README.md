# GestureRecognition

This project enables users to access frequently used websites through hand gestures using a webcam. The application recognizes hand gestures for 2, 3, and 4 fingers, opening specified websites in new tabs of the default web browser. Additionally, a gesture for 5 fingers will close all tabs of the web browser.

**Features**
2 Finger Gesture: Opens a user-specified website.
3 Finger Gesture: Opens a different user-specified website.
4 Finger Gesture: Opens another user-specified website.
5 Finger Gesture: Closes all open tabs of the web browser.
Real-time Gesture Recognition: Uses OpenCV for real-time hand gesture recognition.
**Installation**
To run this project, ensure you have the following installed:

Python 3.x
OpenCV
NumPy
You can install the necessary packages using pip:
pip install opencv-python numpy

**Usage**
Clone the repository:
git clone https://github.com/vibhusharan2407/GestureRecognition
cd GestureRecognition

Run the Python script:
python gesture_recognition.py

Follow the prompts to enter the URLs for the 2-finger, 3-finger, and 4-finger gestures.
Show your hand within the rectangle area displayed on the webcam feed to perform the gestures.

**How It Works**
Capture Video: The webcam captures video frames.
Hand Detection: A sub-region of the frame is processed to detect the hand.
Preprocessing: The sub-region is converted to grayscale and blurred for better contour detection.
Thresholding: Otsu's binarization is applied to create a binary image.
Contour Detection: Contours are detected in the binary image.
Convex Hull and Defects: The convex hull of the hand contour is found, and convexity defects are used to count the number of fingers.
Gesture Recognition: Based on the number of fingers detected, the corresponding action is taken (opening a URL or closing the browser).

**Contributing**
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue.

**License**
This project is licensed under the MIT License. See the LICENSE file for details.

**Acknowledgements**
OpenCV for providing an extensive library for computer vision tasks.
NumPy for numerical computations.
