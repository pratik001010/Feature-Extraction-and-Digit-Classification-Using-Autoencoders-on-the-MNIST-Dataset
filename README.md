<h1 align="center"> Feature Extraction and Digit Classification Using Autoencoders on the MNIST Dataset</h1>

<p align="center">
  <b>Autoencoder-based approach for unsupervised feature learning and digit classification using Keras & TensorFlow.</b><br>
  <i>Compress • Learn • Visualize • Classify</i>
</p>

---

##  Overview

This project demonstrates how **autoencoders** can learn compact **latent representations** of images and how these representations can be used for **digit classification**.  
The work is based on the **MNIST dataset**, containing 70,000 handwritten digits (0–9). The autoencoder compresses 784-dimensional image data into a **32-dimensional latent space**, enabling efficient feature extraction and classification.

---

##  Objectives

- Implement an **autoencoder** to learn compressed image representations.  
- Use **latent features** as input for a dense classifier.  
- Visualize latent space clusters using **t-SNE**.  
- Evaluate model accuracy and visualize predictions.

---

##  Model Architecture

| Stage | Description |
|:------|:-------------|
| **Encoder** | Dense layers compress input (784 → 32) |
| **Decoder** | Reconstructs images (32 → 784) |
| **Classifier** | Predicts digits using latent features |
| **Visualization** | 2D t-SNE projection of 32-dimensional latent space |

---

##  Training Details

| Parameter | Value |
|:-----------|:-------|
| **Training Subset** | 10,000 samples |
| **Latent Dimension** | 32 |
| **Autoencoder Epochs** | 10 |
| **Classifier Epochs** | 10 |
| **Final Test Accuracy** | **84.29%** |

---

##  Visual Results

### **Figure 1 – Data Structure**
Shows the shape of the dataset after flattening: training subset (10,000×784) and test set (10,000×784).  
![Figure 1](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%201.png)

---

### **Figure 2 – Autoencoder Training Progress**
Depicts training and validation loss across 10 epochs, showing convergence and low reconstruction error.  
![Figure 2](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%202.png)

---

### **Figure 3 – Classifier Training**
Displays accuracy and loss progression for the classifier trained on the encoder’s latent features.  
![Figure 3](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%203.png)

---

### **Figure 4 – Latent Space Visualization (t-SNE)**
t-SNE projection of 32-D latent features into 2-D, forming clear clusters corresponding to each digit class.  
![Figure 4](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%204%20.png)

---

### **Figure 5 – Random Predictions**
Displays random MNIST test images and their prediction probability bars.  
![Figure 5](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%205%20.png)

---

### **Figure 6 – Inference Steps**
Shows prediction loop execution logs for individual test samples, verifying stable inference performance.  
![Figure 6](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%206%20.png)

---

### **Figure 7 – Final Summary**
Summarizes performance metrics and model insights — reconstruction, classification, and visualization outcomes.  
![Figure 7](https://github.com/pratik001010/Feature-Extraction-and-Digit-Classification-Using-Autoencoders-on-the-MNIST-Dataset/blob/main/Feature%20Extraction%20and%20Digit%20Classification%20Using%20Autoencoders%20on%20the%20MNIST%20Dataset/fig%207.png)

---

##  Summary

- Trained an **autoencoder** to compress MNIST digits (784 → 32 → 784).  
- Used **latent vectors** as compact features for classification.  
- Visualized **latent clusters** with t-SNE.  
- Achieved **~84% test accuracy** with a simple dense classifier.  

---

##  Tech Stack
- **Language:** Python  
- **Libraries:** TensorFlow / Keras, NumPy, Matplotlib, scikit-learn  

---

##  Keywords
`Autoencoder` · `MNIST` · `Feature Extraction` · `Latent Space` · `t-SNE` · `Deep Learning` · `Keras`
