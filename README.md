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
## Siamese Network Architecture

The model consists of:

- Convolution Layers
- Max Pooling Layers
- Dense Embedding Layer (4096 units)
- Custom L1 Distance Layer
- Binary Classification Output

The network learns embeddings instead of directly classifying faces.

---
