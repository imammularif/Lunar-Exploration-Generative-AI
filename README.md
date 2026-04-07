# Belajar-Fundamental-Generative-AI

# Lunar Exploration: Generative AI & Image Manipulation

Proyek ini mendemonstrasikan implementasi **Stable Diffusion** dan **Segment Anything Model (SAM)** untuk pembuatan dan penyuntingan gambar berbasis kecerdasan buatan. Proyek ini mencakup alur kerja lengkap dari *Text-to-Image*, *Image-to-Image*, hingga teknik manipulasi tingkat lanjut seperti *Inpainting* dan *Outpainting*.

## 🚀 Fitur Utama

* **Text-to-Image Generation**: Menghasilkan gambar astronot di bulan dengan konfigurasi parameter (Guidance Scale & Inference Steps).
* **Image-to-Image Refinement**: Meningkatkan detail gambar dasar menggunakan teknik *refiner pipeline*.
* **Smart Inpainting**: Mengganti objek spesifik dalam gambar menggunakan bantuan **SAM (Segment Anything Model)** untuk pembuatan mask otomatis.
* **Outpainting & Zoom Out**: Memperluas dimensi gambar dan menciptakan latar belakang baru yang koheren dengan objek asli.

## 🛠️ Teknologi yang Digunakan

* **Python**: Bahasa pemrograman utama.
* **PyTorch**: Framework *deep learning*.
* **Hugging Face Diffusers**: Library untuk menjalankan model Stable Diffusion (v1-5 & Inpainting).
* **Segment Anything Model (SAM)**: Meta AI model untuk segmentasi objek secara presisi.
* **Matplotlib & PIL**: Untuk visualisasi dan pemrosesan citra.

## 📊 Analisis Parameter

Dalam proyek ini, dilakukan eksperimen terhadap dua parameter krusial dalam model difusi:

1.  **Guidance Scale (CFG)**: Menentukan seberapa patuh model terhadap prompt teks. Skala rendah memberikan hasil lebih variatif, sedangkan skala tinggi meningkatkan kesesuaian teks namun berisiko saturasi warna.
2.  **Inference Steps**: Menentukan jumlah iterasi *denoising*. Langkah yang lebih banyak (50+) secara signifikan meningkatkan ketajaman dan detail tekstur gambar.

## 🖼️ Hasil Demonstrasi

### 1. Inpainting (Manual & Auto)
Mengubah area tertentu pada permukaan bulan menjadi objek lain (seperti rongsokan satelit) tanpa merusak sisa gambar asli.

### 2. Outpainting & Zoom Out
Memperluas pemandangan galaksi di sekitar astronot untuk menciptakan komposisi foto yang lebih luas (*wide angle*).

## 📝 Cara Menjalankan

1. Clone repositori ini:
   ```bash
   git clone [https://github.com/username/lunar-gen-ai.git](https://github.com/username/lunar-gen-ai.git)
