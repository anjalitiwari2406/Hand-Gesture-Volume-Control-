# Hand Gesture Volume Control

## Overview
This project implements a hand gesture-based volume control system using Python. It utilizes OpenCV for video processing, MediaPipe for hand tracking, and PyAutoGUI for controlling system volume. The program detects the position of the index finger and thumb and adjusts the volume based on their distance.

## Requirements
Ensure you have the following dependencies installed:
- Python 3.x
- OpenCV (`cv2`)
- MediaPipe
- PyAutoGUI

Install the required packages using:
```sh
pip install opencv-python mediapipe pyautogui
```

## How It Works
1. The webcam captures video input.
2. MediaPipe processes the video stream to detect hand landmarks.
3. The program identifies the index finger (landmark ID 8) and thumb (landmark ID 4).
4. The distance between these two points is calculated.
5. If the distance is greater than a threshold (40), the system volume increases.
6. If the distance is smaller than the threshold, the system volume decreases.
7. The program continuously updates based on hand movements.

## Usage
Run the script using:
```sh
python hand_volume_control.py
```
Press `ESC` to exit the program.

## Features
- Real-time hand tracking
- Dynamic volume control based on finger distance
- Visual feedback with drawn landmarks and lines

## Limitations
- Requires a well-lit environment for accurate tracking.
- Works best with a single hand in the frame.
- Sensitivity may vary depending on camera resolution and angle.

## Future Enhancements
- Add more gestures for additional controls (e.g., mute/unmute).
- Improve accuracy with adaptive thresholds.
- Implement multi-hand support.

## Acknowledgments
This project is inspired by computer vision applications and utilizes MediaPipe's robust hand-tracking technology.

## License
This project is open-source and available for modification and distribution.

