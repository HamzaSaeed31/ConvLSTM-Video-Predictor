<h1 align="center">🎬 ConvLSTM Video Predictor</h1>

<p align="center">
  <strong>Deep learning model that predicts future video frames from human action sequences</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
</p>

---

## 📖 About

A Deep Learning project that trains a **ConvLSTM** (Convolutional LSTM) model to predict future frames in human action videos. Given a sequence of past frames, the model learns spatiotemporal patterns and generates plausible predictions of what comes next.

## ✨ Features

- 🧠 ConvLSTM architecture combining CNNs and LSTMs
- 🎥 Trained on human action video sequences (bench press, jumping jacks, etc.)
- 📊 Frame-level preprocessing and normalisation pipeline
- 📈 Loss curves and prediction visualisations
- 🔮 Multi-step future frame prediction

## 🛠️ Tech Stack

| | |
|---|---|
| Language | Python |
| Framework | TensorFlow / Keras |
| Model | ConvLSTM2D |
| Environment | Jupyter Notebook |
| Libraries | NumPy, Matplotlib, OpenCV |

## 🚀 Getting Started

```bash
git clone https://github.com/HamzaSaeed31/ConvLSTM-Video-Predictor.git
cd ConvLSTM-Video-Predictor

pip install tensorflow keras numpy matplotlib opencv-python jupyter

jupyter notebook DL_Project.ipynb
```

## 📐 Model Architecture

```
Input: (batch, time_steps, height, width, channels)
  → ConvLSTM2D layers (spatiotemporal feature extraction)
  → BatchNormalization
  → Conv3D (output frame generation)
Output: predicted next frame(s)
```
