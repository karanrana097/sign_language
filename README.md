## Hand Gesture Recognition using MediaPipe and Machine Learning

This project demonstrates real-time hand gesture recognition using the MediaPipe library for hand landmark detection and a machine learning model trained to classify gestures based on these landmarks. The application captures video from a webcam, processes each frame to detect hand landmarks, and predicts corresponding gestures in real-time.

### Features:
- **Real-time Hand Landmark Detection**: Utilizes MediaPipe Hands module to detect and track hand landmarks (key points) from webcam feed.
- **Gesture Classification**: Applies a pre-trained machine learning model (saved as `model.p`) to classify gestures based on the extracted hand landmarks.
- **Visual Feedback**: Draws bounding boxes around detected hands and displays predicted gestures as text overlays on the video frames using OpenCV.
- **User Interaction**: Supports interactive gesture recognition suitable for applications like sign language translation, virtual controls, and more.

### Dependencies:
- Python 3.x
- OpenCV (cv2)
- NumPy
- MediaPipe
- scikit-learn (for model training and prediction)

### How to Use:
1. **Setup Environment**: Ensure all dependencies are installed (`pip install -r requirements.txt`).
2. **Run the Application**: Execute `python hand_gesture_recognition.py` to start capturing and processing webcam feed.
3. **Interact**: Make hand gestures in front of the webcam and observe the predicted gestures displayed on the screen.

### Repository Structure:
- `hand_gesture_recognition.py`: Main script that captures webcam feed, processes hand landmarks, and displays predictions.
- `model.p`: Serialized machine learning model (`DecisionTreeClassifier`, `RandomForestClassifier`, etc.) trained on hand gesture data.
- `README.md`: Instructions and overview of the project.
- `requirements.txt`: List of Python dependencies for easy installation.

### Notes:
- This project is intended for educational purposes and showcases integration of MediaPipe with machine learning for real-time applications.
- Adjust `min_detection_confidence` and other parameters in `hand_gesture_recognition.py` as needed for optimal performance based on lighting conditions and hand gestures.

Feel free to explore and contribute to enhance the functionality and performance of this hand gesture recognition system. For any issues or improvements, please create a pull request or submit an issue.
