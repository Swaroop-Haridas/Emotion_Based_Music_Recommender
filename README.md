# Emotion-Based Music Recommender

## Overview

Emotion-Based Music Recommender is a real-time facial emotion recognition application that detects a user's emotional state through a webcam and recommends music accordingly. The system uses OpenCV for face detection, an LBPH (Local Binary Pattern Histogram) classifier for emotion recognition, and Streamlit for an interactive web interface.

The application analyzes facial expressions and recommends songs that match the detected emotion, creating a personalized music listening experience.

---

## Features

* Real-time webcam-based face detection
* Facial emotion recognition using LBPH
* Emotion-specific music recommendations
* Interactive Streamlit user interface
* Support for multiple emotions:

  * Angry
  * Disgust
  * Fear
  * Happy
  * Neutral
  * Sad
  * Surprise

---

## System Architecture

```text
Webcam Input
      │
      ▼
Face Detection (Haar Cascade)
      │
      ▼
Emotion Recognition (LBPH)
      │
      ▼
Emotion Prediction
      │
      ▼
Music Recommendation
      │
      ▼
Streamlit Interface
```

---

## Technologies Used

* Python
* OpenCV
* Streamlit
* NumPy
* Pandas

---

## Dataset Structure

```text
train/
├── angry/
├── disgust/
├── fear/
├── happy/
├── neutral/
├── sad/
└── surprise/
```

Each folder contains facial images corresponding to a specific emotion used for training the LBPH classifier.

---

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd Emotion_Music_Recommendation
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Training the Model

Train the emotion recognition model:

```bash
python train_model.py
```

This generates:

```text
model.h5
labels.npy
```

---

## Running the Application

Start the Streamlit application:

```bash
streamlit run app.py
```
