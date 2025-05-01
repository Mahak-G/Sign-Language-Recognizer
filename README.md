# Real-Time Sign Language Recognition

## Overview
Sign language is an essential form of communication among the hearing-impaired population, but there is still a technological lag in effectively converting it to fill the gaps in communication. The project thoroughly investigates real-time American Sign Language (ASL) recognition using two different yet complementary deep learning methods. The development of sign language recognition (SLR) systems is an essential step towards creating inclusive technologies that close the communication gap between the hearing and non-hearing communities. In order to tackle this, this project suggests and puts into practice two deep learning-based pipelines for isolated ASL recognition, each focusing on a different facet of gesture interpretation: real-time sign prediction from video sequences and static hand gesture classification.

The first model recognizes static ASL alphabets using a ConvLSTM2D architecture and the Sign Language MNIST dataset. The approach learns spatiotemporal features from grayscale images and achieves an accuracy of 97.10% when classifying 25 alphabetic gestures. The second, more advanced pipeline is dedicated to real-time sign word recognition with the WLASL dataset. It obtains 3D skeletal keypoints from pose, hand, and face landmarks through MediaPipe Holistic and constructs temporal sequences of 10 frames per video. These are fed into a Bidirectional GRU network with Multi-Head Attention added for learning complex temporal dependencies and providing contextual awareness for predictions. It has a classification accuracy of 91.01%.

Through the removal of dependence on pixel-based CNNs and concentrating solely on keypoint-based representations, this work obtains a light-weight but efficient framework deployable in real-time.The synergy of MediaPipe efficiency coupled with temporal modeling makes this dual-model strategy a scalable one for future sign language recognition systems in assistive communication and human-computer interaction applications.

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

