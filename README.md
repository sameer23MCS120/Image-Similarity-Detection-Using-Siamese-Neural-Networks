# Siamese Neural Network for Face Verification

This project implements a **Siamese Neural Network** using **TensorFlow** and **Keras** for real-time face verification and similarity detection.
The model learns to determine whether two face images belong to the same person by comparing image embeddings using distance metrics.

---

##  Features

* Siamese Neural Network architecture
* Face verification using image similarity
* Custom embedding model
* Real-time webcam image capture
* Positive and negative image pair generation
* TensorFlow data pipeline
* Model training and evaluation
* Verification threshold-based prediction

---

##  Technologies Used

* Python
* TensorFlow
* Keras
* OpenCV
* NumPy
* Matplotlib
* Jupyter Notebook

---

##  Project Structure

```bash
Siamese-Face-Verification/
│
├── Siamese.ipynb
├── data/
│   ├── anchor/
│   ├── positive/
│   └── negative/
│
├── application_data/
│   ├── input_image/
│   └── verification_images/
│
└── README.md
```

---

##  About Siamese Network

A Siamese Network consists of:

* Two identical neural networks
* Shared weights
* Feature embedding generation
* Distance comparison between embeddings

The model predicts whether two images are:

✅ Same Person
❌ Different Person

---

##  Dataset Structure

### Anchor Images

Images of the target person.

### Positive Images

Different images of the same person.

### Negative Images

Images of different people.

---

##  Model Architecture

The embedding network uses:

* Convolutional Layers
* MaxPooling Layers
* Flatten Layer
* Dense Layer (4096 units)

Distance calculation is performed using:

```python
L1 Distance = |Embedding1 - Embedding2|
```

---

##  Installation

### 1️ Clone Repository

```bash
git clone https://github.com/your-username/Siamese-Face-Verification.git
```

### 2️Install Dependencies

```bash
pip install tensorflow opencv-python matplotlib numpy
```

### 3️ Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
Siamese.ipynb
```

---

##  How It Works

1. Capture face images using webcam.
2. Create anchor, positive, and negative pairs.
3. Preprocess images.
4. Train Siamese Network.
5. Generate embeddings.
6. Compare embeddings using L1 distance.
7. Verify identity based on similarity score.

---

##  Training Pipeline

* Image preprocessing
* TensorFlow dataset creation
* Pair generation
* Batch processing
* Model training
* Accuracy evaluation

---

##  Evaluation Metrics

The model uses:

* Precision
* Recall
* Binary Crossentropy Loss

---

##  Real-Time Verification

The system supports real-time face verification using webcam input.

Verification process:

* Capture live image
* Compare with stored verification images
* Generate similarity scores
* Final verification decision

---

##  Future Improvements

* Face recognition with multiple users
* Higher accuracy models
* Mobile deployment
* Real-time attendance system
* GPU optimization
* DeepFace integration

---



