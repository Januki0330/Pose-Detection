# Pose Detection with OpenCV and Mediapipe

## Overview
This project uses OpenCV and Mediapipe to perform real-time human pose detection using a webcam. It captures live video, processes each frame to detect human poses, and visualizes the detected landmarks using Mediapipe's Pose module.

## Prerequisites
Before running the script, ensure you have the following dependencies installed:

- Python 3.x
- OpenCV
- Mediapipe
- NumPy

You can install the required libraries using pip:
```sh
pip install opencv-python mediapipe numpy
```

## How It Works
1. The script initializes a webcam feed using OpenCV.
2. It processes each video frame to detect human pose landmarks.
3. The detected landmarks are drawn on the frame and displayed in real-time.
4. Press 'q' to exit the program.

## Code Structure
- **Initialize Webcam:** The script starts by capturing video from the default webcam.
- **Setup Mediapipe:** A Pose instance is created with a confidence threshold for detection and tracking.
- **Process Frames:** Each frame is converted to RGB, processed by Mediapipe, and then converted back to BGR.
- **Render Detections:** The detected landmarks are drawn on the frame.
- **Display Output:** The processed video feed is displayed in a window.

## Running the Script
To run the script, execute the following command in your terminal:
```sh
python pose_detection.py
```

## Controls
- Press 'q' to exit the video feed.

## Notes
- Ensure your webcam is connected and accessible.
- Adjust the `min_detection_confidence` and `min_tracking_confidence` parameters to optimize detection accuracy.

## License
This project is open-source and available for educational purposes. You may modify and distribute it as needed.

## Author
Januki Manage

