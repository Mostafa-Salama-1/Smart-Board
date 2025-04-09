# 🧠 Smart Board

An AI-powered virtual whiteboard that lets you **write in the air** using **hand gestures**, recognize your handwriting, and **solve math problems in real time** — all through your webcam!


https://github.com/user-attachments/assets/a55032fb-66fb-4989-b742-18e513231a8e
---

## 📌 Features

- ✍️ **Air Writing** – Write digits and symbols using your index finger.
- 🧠 **Handwriting Recognition** – Powered by [TrOCR](https://huggingface.co/microsoft/trocr-base-handwritten), a Transformer OCR model.
- ✋ **Hand Tracking** – Detects and tracks your finger using [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html).
- ➗ **Math Solver** – Automatically parses and solves handwritten expressions like `5 x 2`.
- 🧼 **Clear / Solve Buttons** – Intuitive interface to clear the board or trigger solving.
- 🎥 **Live Webcam Feed** – Everything happens in real time through your camera.
- 🔲 **Bounding Box & Points** – Visual feedback for your finger and drawing path.

---

## 🚀 How It Works

1. Open webcam feed with OpenCV.
2. Track hand landmarks using MediaPipe.
3. Use the index finger tip to draw in the air.
4. Collect strokes until the user clicks **Solve**.
5. Use TrOCR to recognize the handwritten expression.
6. Evaluate and display the result on screen.

---

## 🧰 Tech Stack

| Tool/Library            | Purpose                                 |
|-------------------------|-----------------------------------------|
| Python                  | Programming Language                    |
| OpenCV                  | Webcam handling & drawing               |
| MediaPipe Hands         | Hand tracking and finger detection      |
| PyTorch                 | For TrOCR model inference               |
| HuggingFace Transformers| Pre-trained TrOCR model                 |
| Math parsing logic      | Safely compute handwritten expressions  |

---

## 🖼️ Screenshots

| Air Writing | Recognition | Result |
|-------------|-------------|--------|
| ![Image](https://github.com/user-attachments/assets/beb6f057-edad-4a88-bf8a-1bbeff817b55) | `5 x 2` recognized | Result = `10.0` |


