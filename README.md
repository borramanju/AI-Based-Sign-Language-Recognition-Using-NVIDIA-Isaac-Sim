# SignSpeak: AI-Based Sign Language Recognition Using NVIDIA Isaac Sim

**SignSpeak** is a real-time AI system that translates sign language gestures into **text** and **audio output** using synthetic training data generated with **NVIDIA Isaac Sim**. It aims to empower non-verbal individuals with a communication tool powered by deep learning and simulation.

---

##  Project Summary

This project simulates hand gestures using Isaac Sim and Omniverse Replicator to create a diverse and labeled synthetic dataset. A CNN model is trained on this dataset to classify static hand signs. In real-time, a webcam captures hand gestures, which are recognized and translated into spoken words using text-to-speech.

---

##  System Overview

- **Isaac Sim** is used to simulate hand gestures and export labeled synthetic images.
- A **CNN classifier** is trained on this data using **PyTorch**.
- **OpenCV** is used to capture live input from a webcam.
- Recognized signs are displayed on-screen and converted to **audio** using **gTTS**.

---

##  Key Features

-  Synthetic Dataset Generation with Isaac Sim
-  Deep Learning Model for Gesture Classification
-  Real-Time Webcam-Based Inference
-  Text and Audio Feedback
-  Scalable Vocabulary and Modular Pipeline

---

##  Hardware Requirements

- Windows or Ubuntu PC with **NVIDIA RTX GPU**
- Webcam
- USB Speaker or Headphones

---

##  Software Architecture

| Component       | Technology              |
|----------------|--------------------------|
| Simulation      | NVIDIA Isaac Sim, Omniverse Replicator |
| Model Training  | PyTorch, CNN/ResNet     |
| Video Input     | OpenCV                  |
| Audio Feedback  | gTTS (Google Text-to-Speech) |
| GUI (Optional)  | Tkinter or Streamlit    |
| Dataset Handling| NumPy, Pandas           |

---

##  Pre-requisites

### 1. Isaac Sim Installation

Follow the official [Isaac Sim installation guide](https://docs.omniverse.nvidia.com/isaacsim/latest/installation/install_launcher.html).

### 2. Python Environment Setup

Create and activate a conda environment:

```bash
conda create -n signspeak python=3.10
conda activate signspeak
pip install -r requirements.txt
