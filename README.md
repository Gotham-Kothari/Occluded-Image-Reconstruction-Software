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

```python
autoencoder.compile(loss='binary_crossentropy', optimizer='adam')
autoencoder.fit(train_ds, epochs=10, validation_data=val_ds)
```

### 🔹 U-Net
An encoder–decoder with **skip connections**, enabling sharper and more accurate reconstruction.

```python
model.compile(optimizer='adam',
              loss='mean_squared_error',
              metrics=['mean_absolute_error'])
```

---

## 🧩 Dataset
- **Dataset:** MNIST (28×28 grayscale images of digits)
- **Preprocessing:** Normalized to `[0,1]` and partially occluded before training

---

## 🚀 How to Run

1. **Install dependencies**
   ```bash
   pip install tensorflow keras numpy matplotlib
   ```
2. **Run Autoencoder**
   ```bash
   python autoencoder.py
   ```
3. **Run U-Net**
   ```bash
   python unet.py
   ```

---

## 📊 Results

| Input (Occluded) | Autoencoder Output | U-Net Output |
|------------------|--------------------|---------------|
| 🖼️ | 🧩 | ✅ |

U-Net produces sharper, clearer reconstructions, while Autoencoder captures basic structure effectively.

---

## 🧠 Summary

This project highlights how **deep learning can reconstruct occluded visual data**, paving the way for smarter restoration systems in photography, healthcare, and AI-driven design.

---
