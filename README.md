# Gesture Recognition using CNN-RNN (VGG16 + GRU)

This project implements a deep learning model for **video-based hand gesture recognition** using a combination of Convolutional Neural Networks and Recurrent Neural Networks.

The model uses a pretrained **VGG16 CNN** to extract spatial features from individual video frames and **GRU recurrent layers** to learn the temporal relationship between consecutive frames.

The system classifies each video sequence into one of **5 gesture classes**.

---

## Project Overview

Gesture recognition requires understanding two different types of information:

- **Spatial information** — what appears inside each video frame
- **Temporal information** — how the gesture changes across consecutive frames

A normal image classification CNN only understands individual frames. Therefore, this project combines:

```text
Video Frames
     ↓
CNN Feature Extraction
     ↓
Temporal Sequence
     ↓
GRU / RNN
     ↓
Gesture Classification
