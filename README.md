# Hand Gesture Finger Counter & Calculator

This project uses OpenCV, MediaPipe, and Python to detect hand gestures in real time and count the number of extended fingers on each hand.
When two hands are detected, the program performs addition, subtraction, multiplication, and division using the finger counts.

---

## Features

* Real-time hand tracking using MediaPipe Hands
* Accurate finger counting for both left and right hands
* Automatically performs:

  * Addition
  * Subtraction
  * Multiplication
  * Division (handles divide-by-zero safely)
* Displays results directly on the video feed
* Works with any built-in or external webcam

---

## Technologies Used

* Python
* OpenCV
* MediaPipe

---

## Project Structure

```
finger-calculator/
│
├── finger_calculator.py   # Main program
├── README.md              # Project documentation
└── requirements.txt       # Required libraries
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YourUsername/finger-calculator.git
cd finger-calculator
```

### 2. Install dependencies

```bash
pip install opencv-python mediapipe
```

Or install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## How to Run

Run the main script:

```bash
python finger_calculator.py
```

Press `ESC` to exit the program.

---

## How It Works

### Hand Detection

MediaPipe detects both hands and identifies whether they are left or right.

### Finger Counting

The number of extended fingers is calculated using hand landmark positions.

* The thumb uses x-coordinate comparison.
* Other fingers use y-coordinate comparison.

### Arithmetic Operations

If two hands are detected, the program calculates:

* A + B
* A - B
* A * B
* A / B (if B is not zero)

The results are shown on the video stream in real time.

---

## Requirements

* Python 3.8 or newer
* Webcam
* Required packages:

  * opencv-python
  * mediapipe

---

## Author

Developed by **[Your Name]**.
Contributions and improvements are welcome.



Just tell me!
