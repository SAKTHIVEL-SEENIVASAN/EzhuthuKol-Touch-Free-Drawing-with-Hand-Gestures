# ✍️ EzhuthuKol: Touch-Free Drawing with Hand Gestures
EzhuthuKol is a fun and interactive computer vision project that lets you draw in the air using hand gestures. No mouse, no touch — just your fingers act as the brush! Built using OpenCV and MediaPipe, it turns your webcam into a virtual canvas.
---

### Table of Contents

* [Overview](#overview)
* [Demo](#demo)
* [Key Features](#key-features)
* [Technical Requirements](#technical-requirements)
* [Installation Guide](#installation-guide)
* [Usage Instructions](#usage-instructions)
* [How It Works](#how-it-works)
* [Project Structure](#project-structure)
* [Troubleshooting](#troubleshooting)
* [Future Enhancements](#future-enhancements)
* [License](#license)
* [Acknowledgments](#acknowledgments)
* [Author & Contact](#author--contact)

---

## 🎨 Overview

**EzhuthuKol** is an interactive computer vision project that allows users to **draw in the air using hand gestures**.

💡 **Use (Tamil-English style):**
Indha project la webcam use pannitu kai movement detect panni, air la drawing panna mudiyum. Touch illa, mouse illa — finger move pannina automatic drawing varum.

Using **OpenCV** for image processing and **MediaPipe** for precise hand tracking, your index finger becomes a virtual brush. This project demonstrates **gesture-based AI drawing** in real-time.

---

## 🧠 Demo

*(You can later add screenshots or a short GIF here showing your project in action)*

---

## ⚙️ Key Features

* 🖐️ **Gesture-Based Drawing:** Draw freely using your hand tracked by your webcam.
* ✋ **Pinch Gesture Control:** Pinch open/closed to toggle drawing mode.
* 🎨 **Colour Picker:** Choose brush colours dynamically using a simple interface.
* 🖌️ **Brush Size Control:** Adjust brush size via keyboard shortcuts.
* 🧼 **Canvas Tools:** Clear the canvas or save your artwork as PNG files.
* ⚡ **Smooth Tracking:** Optimised hand tracking for fluid and accurate drawing.

---

## 🧾 Technical Requirements

* **Python:** 3.8 or higher
* **Libraries:**

  * OpenCV → Image processing & canvas rendering
  * MediaPipe → Hand tracking & gesture detection
  * NumPy → Numerical operations
  * Tkinter → Colour picker UI
* **Hardware:** Webcam (720p or above recommended)

---

## 🛠️ Installation Guide

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/EzhuthuKol.git
cd EzhuthuKol
```

### 2️⃣ (Optional) Create Virtual Environment

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage Instructions

### Run the Application

```bash
python code/ezhuthukol.py
```

### Gesture Controls

| Gesture               | Action               |
| --------------------- | -------------------- |
| Pinch Open (≥ 40px)   | Drawing mode ON      |
| Pinch Closed (< 40px) | Drawing mode OFF     |
| Index Finger          | Acts as brush cursor |

### On-Screen Buttons

* 🧼 **CLEAR:** Reset the canvas
* 🎨 **COLOR:** Open color picker dialog
* 💾 **SAVE:** Save drawing as timestamped PNG

### Keyboard Shortcuts

| Key       | Function            |
| --------- | ------------------- |
| `+` / `=` | Increase brush size |
| `-`       | Decrease brush size |
| `q`       | Quit application    |

---

## ⚙️ How It Works

1. **Video Capture:** Processes webcam frames in real-time.
2. **Hand Tracking:** MediaPipe identifies hand landmarks.
3. **Gesture Detection:** Measures index & thumb tip distance to toggle drawing.
4. **Drawing Logic:**

   * Stores drawing points in a deque for smooth lines.
   * Draws lines between consecutive points.
5. **Dual Canvas System:**

   * Persistent canvas stores the full drawing.
   * Temporary canvas used for frame display.

---

## 🗂️ Project Structure

```
EzhuthuKol/
├── code/
│   ├── ezhuthukol.py        # Main application
│   └── color_palette.py     # Colour picker implementation
├── assets/
│   ├── SS-1.png             # Screenshot 1
│   ├── SS-2.png             # Screenshot 2
│   ├── SS-3.png             # Screenshot 3
│   └── ezhuthukol_*.png     # Example drawings
├── requirements.txt         # Project dependencies
├── README.md                # Documentation
└── ezhuthukol_*.png         # Saved drawings
```

---

## 🧰 Troubleshooting

| Issue                    | Solution                                           |
| ------------------------ | -------------------------------------------------- |
| Hand not detected        | Ensure proper lighting and clear background        |
| Tracking unstable        | Adjust distance from camera (1–2 feet recommended) |
| Color picker not working | Ensure Tkinter is installed                        |
| Drawing appears jerky    | Move your hand more slowly for smoother lines           |
| App crashes              | Check webcam permissions and dependencies          |

---

## 🚀 Future Enhancements

* Multi-hand support for collaborative drawing
* Shape & eraser tools
* Background customisation
* Drawing session recording & replay
* Export to different formats (JPG, PDF, etc.)

---

## 🧾 License

This project is released under the **MIT License** — free to use and modify with credit.

---

## 🙌 Acknowledgments

* **MediaPipe Team** for a real-time hand tracking library
* **OpenCV Community** for powerful computer vision tools
* Original contributors for inspiring this implementation

---

## 👤 Author & Contact

**Author:** S.M. Sakthivel
**Email:** [s.m.sakthivelofficial@gmail.com](mailto:s.m.sakthivelofficial@gmail.com)
**Location:** Pondicherry, India

If you use or modify this project, I’d love to hear from you!
⭐ Feel free to reach out, share your version, or give feedback — collaboration is always welcome!



