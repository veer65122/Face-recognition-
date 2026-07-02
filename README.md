# Face-recognition-
A deep learning-based Face Verification System built using TensorFlow, Keras, and OpenCV

------

## Features

- Face image collection using webcam
- Automatic dataset creation (Anchor, Positive, Negative)
- Siamese Neural Network architecture
- Custom L1 Distance Layer
- Face verification using image similarity
- Model training and evaluation with TensorFlow
- Real-time verification using OpenCV

---

## Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- UUID
- OS Module

---

## Dataset

The project uses three categories of images:

- **Anchor Images** – Images of the user.
- **Positive Images** – Different images of the same user.
- **Negative Images** – Images of different people (LFW Dataset).

The negative dataset is created using the **Labeled Faces in the Wild (LFW)** dataset.

---

## Workflow

1. Collect Anchor Images using webcam.
2. Collect Positive Images.
3. Import Negative Images from the LFW dataset.
4. Preprocess images.
5. Create Anchor–Positive and Anchor–Negative pairs.
6. Train the Siamese Neural Network.
7. Save the trained model.
8. Verify a person's identity using image similarity.

---
## 📸 Sample Workflow

```
Capture Face
      │
      ▼
Preprocess Image
      │
      ▼
Generate Embeddings
      │
      ▼
Compute L1 Distance
      │
      ▼
Verification Score
      │
      ▼
Verified / Not Verified
```
## Siamese Network Architecture

The model consists of:

- Convolution Layers
- Max Pooling Layers
- Dense Embedding Layer (4096 units)
- Custom L1 Distance Layer
- Binary Classification Output

The network learns embeddings instead of directly classifying faces.

---
## 📦 Installation

### Clone the repository

```bash
git clone https://github.com/veer65122/Face-recognition-.git
cd Face-recognition-
```

### Install dependencies

```bash
pip install tensorflow opencv-python numpy matplotlib
```
## ▶️ Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run all cells in sequence.

---
## 📈 Training

The model is trained using image pairs:

- Positive Pair → Label = 1
- Negative Pair → Label = 0

**Loss Function:** Binary Cross Entropy

**Optimizer:** Adam

---
## 🎯 Applications

- Face Verification
- Smart Attendance Systems
- Secure Login Systems
- Access Control
- Identity Verification
- AI Security Solutions

---
## 🚀 Future Improvements

- Deploy using Flask or FastAPI
- Build a Streamlit web application
- Mobile application integration
- Face anti-spoofing
- Cloud deployment on AWS
- Improve accuracy using FaceNet or ArcFace embeddings

---
## 👨‍💻 Author

**Veer**

B.Tech – Computer Science & Engineering (Data Science)

**Interests:**
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Computer Vision
- Data Engineering

GitHub: https://github.com/veer65122

---
## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---
