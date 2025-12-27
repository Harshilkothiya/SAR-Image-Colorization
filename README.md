# SAR Image Colorization using GANs with U-Net Generator

## 📌 Overview
Synthetic Aperture Radar (SAR) images are widely used in remote sensing because they can capture information under all weather and lighting conditions. However, SAR images are typically grayscale and difficult to interpret visually.

**SAR-GAN** is a deep learning–based solution developed for the **Smart India Hackathon (SIH) 2017 SAR Image Colorization problem**. This project employs a **Generative Adversarial Network (GAN)** where a **U-Net–based Generator** is used to convert grayscale SAR images into realistic **RGB color images**.

---

## 🚀 Features
- U-Net based Generator for SAR image colorization
- GAN framework for realistic RGB image generation
- Preserves spatial and structural details using skip connections
- Enhances interpretability of SAR images
- Suitable for remote sensing and disaster monitoring tasks

---

## 🧠 Model Architecture

### Generator (U-Net)
- Based on **U-Net architecture**
- Encoder–decoder structure with **skip connections**
- Input: Grayscale SAR image
- Output: Colorized RGB image
- Skip connections help preserve fine-grained spatial details

### Discriminator
- Convolutional neural network
- Distinguishes real optical images from generated RGB images
- Guides the Generator to produce realistic color distributions

---

## 🗂 Dataset
- Paired SAR and optical (RGB) images
- Images are resized and normalized before training

> *Note: Dataset is not included in this repository due to size and licensing constraints.*

---

## ⚙️ Technology Stack
- Python
- TensorFlow / PyTorch
- NumPy
- streamlit
- Matplotlib

---

## 🏗️ Training Process
1. Grayscale SAR images are passed to the U-Net Generator
2. Generator produces corresponding RGB images
3. Discriminator evaluates real vs generated images
4. Adversarial and reconstruction losses are optimized
5. Model improves color realism across training epochs

---

## 📊 Results
- U-Net skip connections preserve structural information
- Improved color consistency compared to basic CNN models
- Enhanced visual clarity for terrain and urban regions

![alt text](image-1.png)
![alt text](image-3.png)

---

## 🛠️ How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/SAR-GAN.git
cd SAR-GAN
