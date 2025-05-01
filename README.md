# Real-Time Sign Language Recognition

## Overview
This project implements real-time recognition of both static and dynamic sign language using deep learning. It uses:
- **ConvLSTM2D** for static hand signs (Sign MNIST)
- **Bi-GRU + Attention** for dynamic gestures (WLASL)

## Key Features
- Real-time sign prediction using webcam
- Keypoint extraction with MediaPipe
- Lightweight models, optimized for CPU

## Datasets
- **Sign MNIST**: 28×28 grayscale alphabet signs
- **WLASL (Top-10)**: Video-based word-level ASL signs

## Technologies
- Python, TensorFlow, OpenCV
- MediaPipe Holistic, Keras

## Results
| Model | Accuracy |
|-------|----------|
| Static (ConvLSTM2D) | 97.1% |
| Dynamic (Bi-GRU + Attention) | 91.01% |

## License
For academic and research purposes.

