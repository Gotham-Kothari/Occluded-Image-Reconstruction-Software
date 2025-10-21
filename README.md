# 🧠 Image Reconstruction using U-Net and Autoencoder (MNIST)

This project demonstrates **image reconstruction from occluded MNIST digits** using two deep learning models — a **Convolutional Autoencoder** and a **U-Net**.  
It shows how AI can “fill in missing pixels” and restore clarity in images where information is partially hidden.

---

## 🌍 Why Occlusion Removal?

In real-world scenarios, objects or noise often hide parts of an image.  
Occlusion removal helps in:
- 🖼️ Restoring damaged photos or documents  
- 🚗 Enhancing vision for autonomous vehicles  
- 🩺 Completing missing data in medical scans  
- 🎨 Inpainting for creative or design workflows  

---

## ⚙️ Model Overview

### 🔹 Autoencoder
A simple encoder–decoder that learns to compress and reconstruct input images.
### 🔹 U-Net
An encoder–decoder with **skip connections**, enabling sharper and more accurate reconstruction.

## 🧩 Dataset
- **Dataset:** MNIST (28×28 grayscale images of digits)
- **Preprocessing:** Normalized to `[0,1]` and partially occluded before training

---

## 📊 Results

U-Net produces sharper, clearer reconstructions, while Autoencoder captures basic structure effectively.

---

## 🧠 Summary

This project highlights how **deep learning can reconstruct occluded visual data**, paving the way for smarter restoration systems in photography, healthcare, and AI-driven design.

---
