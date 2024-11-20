## README

## Hand Gesture-Based Screen Brightness Control

This project is a Python-based application that uses a webcam to detect hand gestures and adjust the screen brightness accordingly. It leverages **OpenCV**, **MediaPipe**, and **Screen Brightness Control (sbc)** libraries.

---

## Features

- **Real-time Hand Gesture Recognition**: Detects hand gestures using MediaPipe's hand landmarks.
- **Brightness Adjustment**:
  - **Pointing Up Gesture**: Increases screen brightness.
  - **Pointing Down Gesture**: Decreases screen brightness.

---

## Prerequisites

Ensure you have the following dependencies installed:

- Python 3.x
- OpenCV
- MediaPipe
- Screen Brightness Control (`screen-brightness-control`)

Install the required libraries using pip:

```bash
pip install opencv-python mediapipe screen-brightness-control
```

---

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Adarash13/Hand-Gesture-Brightness-Controller.git
   cd Hand-Gesture-Brightness-Controller
   ```

2. **Run the Script**:
   ```bash
   python hand_gesture_brightness_control.py
   ```

3. Use gestures:
   - Point **upwards** with your index finger to **increase** brightness.
   - Point **downwards** with your index finger to **decrease** brightness.

4. Press **'q'** or close the window to exit the application.

---

## How It Works

1. **Hand Tracking**:
   - MediaPipe tracks hand landmarks in real-time.
   - The script identifies the positions of the **index finger tip** and **thumb tip**.

2. **Gesture Recognition**:
   - If the index finger is above the thumb → **Gesture: Pointing Up**.
   - If the index finger is below the thumb → **Gesture: Pointing Down**.

3. **Brightness Control**:
   - Adjusts screen brightness by increasing or decreasing in increments of 10%.
   - Brightness values are constrained between 0% and 100%.

---

## Requirements and Limitations

- A functional **webcam**.
- Administrator permissions might be required for brightness adjustments.
- Only works on platforms supported by the **screen-brightness-control** library.

---

## Future Improvements

- Add support for multiple gestures and actions.
- Implement platform-specific optimizations.
- Provide an on-screen indicator for the current brightness level.

---

## Troubleshooting

- **Webcam Not Detected**: Ensure the camera is functional and not in use by other applications.
- **Brightness Adjustment Not Working**: Verify platform compatibility with the `screen-brightness-control` library.
- **Slow Performance**: Reduce the resolution of the webcam feed for smoother execution.

---

## Contributing

Feel free to open issues or submit pull requests for new features or bug fixes. Contributions are always welcome!

---

## Contact

**Adarsh Sainath H**

For any queries, please contact [sainathadarsh13@gmail.com].

