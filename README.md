# Image Classification Model - TensorFlow + TFLite + TFJS

Proyek ini berisi model deep learning untuk klasifikasi citra menggunakan TensorFlow, yang telah dikonversi ke dua format untuk kebutuhan inferensi: **TensorFlow.js** (untuk web) dan **TFLite** (untuk mobile). Semua langkah pelatihan dan konversi dilakukan menggunakan Google Colab.

🔗 Notebook Google Colab: Klik di sini untuk membuka (https://colab.research.google.com/drive/1nSQ--PrSrc_SHxjZGCKjQWgObab4bdTF?usp=chrome_ntp)

## Struktur Folder

```
model_tfjs/              # Model dalam format TensorFlow.js
     model.json
     group1-shard1of1.bin

tflite/                  # Model dalam format TensorFlow Lite
     model.tflite
     label.txt

saved_model/            # Format SavedModel asli dari TensorFlow
     saved_model.pb
     variables/
     variables.index
     variables.data-00000-of-00001
 Gambar Arif Kurniawan.ipynb       # Notebook Colab untuk pelatihan dan konversi
 requirements.txt          # Daftar dependensi (opsional)
 README.md                # Dokumentasi ini
```

## 🧠 Model

Model adalah CNN (Convolutional Neural Network) sederhana yang dilatih pada dataset klasifikasi gambar berisi ≥3 kelas. Model ini mencapai akurasi tinggi (>95%) pada training dan testing set.

## Konversi Model

Model disimpan dalam 3 format:

- **SavedModel**: format asli TensorFlow, cocok untuk deployment server.
- **TFLite (.tflite)**: ringan untuk perangkat Android dan IoT.
- **TensorFlow.js**: untuk inferensi di browser/web.

##  Label

Label disimpan dalam file `label.txt`:

```

Black Sea Sprat
Gilt-Head Bream
Hourse Mackerel
Red Mullet
Red Sea Bream
Sea Bass
Shrimp
Striped Red Mullet
Trout


```

## Kontributor

**Arif Kurniawan**  
Universitas Pendidikan Indonesia  
Program Studi Sistem Informasi Kelautan