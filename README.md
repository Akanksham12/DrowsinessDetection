# Real-time Drowsiness Detection System

## Overview

The Real-time Drowsiness Detection System is a Python-based application designed to monitor driver alertness by detecting drowsiness through real-time video feeds. Utilizing deep learning techniques and the InceptionV3 model, this system classifies eye states as either open or closed and triggers alerts when drowsiness is detected, enhancing safety for drivers and operators.

## Technologies Used

- **Python:** Core programming language
- **TensorFlow & Keras:** For deep learning and model training
- **OpenCV:** For real-time video capture and image processing
- **InceptionV3:** Pre-trained deep learning model used for transfer learning
- **Pillow:** For image processing
- **Flask & Socket.IO:** For potential web-based integrations (not used in the provided code snippet)

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Akanksham12/real-time-drowsiness-detection.git
   cd real-time-drowsiness-detection
   ```

2. **Install Dependencies:**

   Ensure you have Python installed. Then, install the required libraries using pip:

   ```bash
   pip install tensorflow keras opencv-python pillow
   ```

## Usage

1. **Prepare Dataset:**

   - Organize eye images into directories labeled `closed_eyes` and `open_eyes`.
   - Ensure the dataset directory structure matches the paths specified in the script.

2. **Run the Script:**

   Execute the Python script to start the drowsiness detection system:

   ```bash
   python drowsiness_detection.py
   ```

   The system will open a video feed from your webcam. It will monitor the eye states and display alerts if drowsiness is detected.

## Model Details

- **Base Model:** InceptionV3 (pre-trained on ImageNet)
- **Fine-tuning:** Transfer learning applied for eye state classification
- **Layers:** Includes Flatten, Dense (ReLU activation), Dropout, and Dense (Softmax activation)

## Evaluation Metrics

- **Accuracy (Training):** 93.77%
- **Accuracy (Validation):** 89.91%
- **Accuracy (Test):** 94.34%

