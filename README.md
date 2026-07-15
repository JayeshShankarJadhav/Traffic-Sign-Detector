# Smart Traffic Sign Identifier

A deep learning–based system that recognizes and classifies traffic signs from images or real-time video, built with a Convolutional Neural Network (CNN) and served through a Flask web application.

## Overview

This project uses a CNN trained on a labelled traffic-sign dataset (based on the German Traffic Sign Recognition Benchmark, GTSRB, with 43 classes) to classify traffic signs such as stop signs, speed limits, and yield signs. Users can either upload an image or use a live webcam feed to get real-time predictions along with confidence scores.

## Features

- Image upload and classification via a Flask web interface
- Live webcam-based real-time traffic sign detection
- CNN model built with TensorFlow/Keras (convolutional, pooling, dropout, and dense layers)
- Image preprocessing with OpenCV (resizing, normalization, augmentation)
- Desktop GUI variant (`gui.py`) built with Tkinter for standalone image classification

## Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | HTML, CSS, JavaScript, Bootstrap, Jinja2 |
| Backend | Python, Flask |
| Machine Learning | TensorFlow / Keras, OpenCV, NumPy, Pandas |
| Storage | File-based (`uploads/` and `results/` folders) |

## Project Structure

```
├── train/              # Training images, organized by class folder
├── uploads/             # User-uploaded images/videos
├── results/              # Processed outputs with classified signs
├── my_model.h5            # Trained CNN model
├── gui.py                  # Tkinter desktop GUI application
├── app.py                   # Flask web application (entry point)
└── Smart_Traffic_Sign_Identifier_Report.pdf  # Full project documentation
```

## Requirements

- Python 3.x
- TensorFlow / Keras
- OpenCV
- Flask
- NumPy, Pandas
- Pillow (PIL)
- scikit-learn

Install dependencies with:

```bash
pip install tensorflow opencv-python flask numpy pandas pillow scikit-learn
```

## Dataset

The training and test dataset used for this project is available on Google Drive:

**Dataset link:** _[paste your Google Drive link here]_

Download the dataset and place the `train/` folder (and `Test.csv`, if applicable) in the project's root directory before running the training script.

## Usage

1. Clone or download this repository.
2. Install the required dependencies (see above).
3. Download the dataset from the Google Drive link above and place it in the project directory.
4. Train the model (or use the pre-trained `my_model.h5` if provided).
5. Run the Flask app:
   ```bash
   python app.py
   ```
6. Open the app in your browser and upload an image or start the live webcam feed to classify traffic signs.

## Documentation

Full project documentation, including system architecture, methodology, code, and results, is available in `Smart_Traffic_Sign_Identifier_Report.pdf`.

## Author

**Jayesh Jadhav**
M.Sc. (Data Analytics), Pillai College of Arts, Commerce and Science (Autonomous), New Panvel
Under the guidance of Mr. Omkar Sherkhane, Assistant Professor
