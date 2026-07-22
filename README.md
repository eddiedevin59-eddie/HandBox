GestureBox is a computer vision-based interactive system developed using OpenCV and MediaPipe Hands. By analyzing real-time video streams from a webcam, the application detects 21 hand landmarks and enables intuitive gesture interactions—allowing users to "pinch" and "drag" a virtual block on screen using simple finger movements.
Key Features
Real-time Pinch Gesture Detection: Calculates the Euclidean distance between the index fingertip and thumb tip in real time using MediaPipe to detect pinching action with high accuracy.
Touchless Object Dragging: Activates a "grab" state when a pinch gesture occurs within the block boundaries, smoothly moving the virtual box alongside hand movements and releasing it when the fingers separate.
Dynamic Visual Feedback: Features status-based color shifts for the virtual object and semi-transparent alpha blending for enhanced UI aesthetics and user responsiveness.
opencv-python>=4.8.0
mediapipe>=0.10.0
Markdown
# 🤏 GestureBox (AirGrip Vision)

> A lightweight computer vision application built with OpenCV and MediaPipe Hands, enabling touchless virtual object dragging using pinch gestures.

---

## 📌 Features

* 🖐️ **21-Landmark Hand Tracking**: Uses MediaPipe Hands to capture keypoints in real time.
* 🤏 **Pinch Gesture Recognition**: Detects finger closeness (Index-to-Thumb distance) to trigger a "grab" action.
* 📦 **Interactive Virtual Box**: Features a semi-transparent box that dynamically follows your fingers and changes color when active.
* ⚡ **Real-time Performance**: Runs smoothly on standard webcam streams.

---

## 🎮 How to Interact

1. **Grab/Pinch**: Bring your **Index Fingertip** and **Thumb Tip** close together (distance < 30px) inside the green box to grab it.
2. **Move/Drag**: Keep your fingers pinched to move the virtual box around the screen (box turns yellow when activated).
3. **Release**: Separate your fingers to release the box.
4. **Exit**: Press `ESC` on your keyboard to close the application.

---

## 🛠️ Requirements & Installation

### Requirements
* Python 3.8 or higher
* Webcam / Camera module

### 1. Install Dependencies
```bash
pip install -r requirements.txt
