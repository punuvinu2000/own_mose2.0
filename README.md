# 🖱️ Virtual Mouse Using Finger Tracking

This Python project allows you to control your computer mouse using just your fingers and a webcam! By using computer vision and hand tracking, you can move the mouse and click without touching any hardware.

https://user-images.githubusercontent.com/your-demo-video.mp4 *(Add a demo if you have one)*

## 🚀 Features

- Tracks your hand and finger movements in real time
- Uses your index finger to move the cursor
- Clicks when the thumb and index finger come close together
- Hands-free control using only a webcam

---

## 🛠️ Built With

- [OpenCV](https://opencv.org/) - Image processing
- [MediaPipe](https://google.github.io/mediapipe/) - Real-time hand landmark detection
- [PyAutoGUI](https://pyautogui.readthedocs.io/) - Mouse control in Python

---

## 📦 Requirements

Make sure you have **Python 3.6+** installed. Then install the required libraries using pip:

```bash
pip install opencv-python mediapipe pyautogui
```

## 📸 How to Use

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/virtual-mouse.git
   cd virtual-mouse
   ```

2. **Run the Program**

   ```bash
   python main.py
   ```

3. **How It Works**

   * Make sure your webcam is enabled.
   * Move your index finger to move the mouse cursor.
   * Touch your thumb and index finger together to **click**.



## 🧠 How It Works

* The program uses MediaPipe to detect hand landmarks.
* Landmark `8` (index finger tip) is used to control cursor position.
* When the distance between the thumb (`id 4`) and index finger (`id 8`) is small, a mouse click is triggered.

---

## 📝 Notes

* Works best in good lighting conditions.
* Ensure your webcam is properly positioned.
* You can adjust the click sensitivity in the code by changing the distance threshold (currently `20` pixels).

