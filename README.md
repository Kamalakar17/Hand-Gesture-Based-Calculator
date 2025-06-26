# ✋🧠 Hand Gesture Calculator using OpenCV and MediaPipe

This is a **real-time hand gesture-based calculator** that allows users to input and evaluate mathematical expressions using only hand gestures. Designed for accessibility and computer vision practice, it translates hand signs into digits, operators, and commands.

---

## 🚀 Features

- Real-time gesture detection using webcam
- Supports multi-digit input (e.g., showing 2 → 4 → 7 becomes `247`)
- Gesture-controlled arithmetic operations (`+`, `-`, `*`, `/`)
- Built-in evaluation and result display
- Hands-free Clear, Delete, and Exit commands
- Works using a standard webcam (no special hardware needed)

---

## 🧠 Tech Stack

| Tool      | Purpose                             |
|-----------|-------------------------------------|
| Python    | Core programming language           |
| OpenCV    | Video capture, frame rendering      |
| MediaPipe | Hand landmark detection (21 points) |
| NumPy     | Distance computation, math logic    |

---

## ✋ Supported Gestures

| Gesture                           | Function        |
|-----------------------------------|-----------------|
| 1–5 fingers (one hand)            | Digits 1–5      |
| 5 + 1–4 fingers (both hands)      | Digits 6–9      |
| Only one hand with 0 fingers      | Digit 0         |
| 1 finger on both hands            | `+` (Add)       |
| 1 + 2 fingers                     | `-` (Subtract)  |
| 1 + 3 fingers                     | `*` (Multiply)  |
| 1 + 4 fingers                     | `/` (Divide)    |
| Both hands with 0 fingers         | `=` (Evaluate)  |
| Both hands with 5 fingers         | Clear input     |
| Both hands with 2 fingers         | Delete input    |
| Right index < Left index (space) | Exit program    |

> Gestures are detected based on hand landmark positions and finger states.

---

## 📦 Installation

```bash
git clone https://github.com/sam-1409/hand-gesture-calculator.git
cd hand-gesture-calculator
pip install -r requirements.txt
