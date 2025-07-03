# 🥦 Klasifikasi Gambar Sayuran (Vegetable Image Classification)

Proyek ini menggunakan deep learning untuk mengklasifikasikan gambar sayuran ke dalam 15 kelas berbeda. Dataset diambil dari Kaggle dan diolah menggunakan beberapa varian arsitektur Lightweight CNN.

---

## 📂 Dataset

- 🔗 [Vegetable Image Dataset – Kaggle](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset)  
- Total gambar: **21.000**
- Jumlah kelas: **15** (1.400 gambar per kelas)
- Ukuran gambar: **224×224 piksel**, format **.jpg**
- Pembagian data:
  - 70% Training
  - 15% Validation
  - 15% Testing

---

## ⚙️ Arsitektur Model

Model yang digunakan berbasis **Lightweight CNN**, dengan 3 variasi:

### 1. 🧠 Lightweight CNN (Dasar)
- Arsitektur sederhana dan efisien
- Cocok untuk pemrosesan cepat dan ukuran model kecil

### 2. 🧠 Lightweight CNN + Dropout
- Menambahkan **Dropout** untuk mengurangi overfitting
- Performa lebih stabil saat validasi

### 3. 🧠 Lightweight CNN + SGD Optimizer
- Menggunakan **Stochastic Gradient Descent (SGD)** sebagai optimisasi
- Mengganti default optimizer (misalnya Adam)

---

## 🧪 Evaluasi Model

Setiap model dievaluasi dengan metrik berikut:

- 🎯 **Akurasi** (Training, Validation, Testing)
- 📉 **Loss Curve**
- 🧾 **Confusion Matrix**
- ⏱️ **Kecepatan training dan inferensi**