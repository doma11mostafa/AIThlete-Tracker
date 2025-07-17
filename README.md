# AIthlete Motion Tracker 📸🏋️

This repo contains a real-time workout motion tracking system using YOLOv11 pose estimation. It supports workouts like biceps curls, triceps dips, and leg raises. It also includes voice command recognition to switch between exercises.

## 🚀 Features
- Real-time pose detection using YOLOv11 pose
- Angle calculation between joints using keypoints
- Voice recognition to choose exercises (e.g., "start biceps")
- Visual feedback with joint overlays and rep counting

## 🧠 Technologies
- YOLOv11 Pose Estimation
- Python OpenCV
- SpeechRecognition for voice input
- NumPy for angle math

## 📐 Angle Calculation
We calculate the angle using 3 keypoints (e.g., shoulder, elbow, wrist, kip,ankle,knee):

```python
def calculate_angle(a, b, c):
    # a, b, c: points (x, y)
    angle = np.arccos(...)
    return angle
🗣️ Voice Commands
bash
Copy
Edit
