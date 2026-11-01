# PCD Assignment 03
## Segmentasi Citra dan Pengolahan Morfologi

Repository ini berisi implementasi segmentasi citra dan operasi morfologi sebagai bagian dari tugas mata kuliah **Pengolahan Citra Digital (PCD)**.

## Tujuan

1. Mengimplementasikan salah satu metode segmentasi citra menggunakan Python.
2. Mengimplementasikan beberapa operasi morfologi tanpa menggunakan fungsi siap pakai dari library pengolahan citra.
3. Membandingkan hasil segmentasi sebelum dan sesudah penerapan operasi morfologi.
4. Mengamati pengaruh setiap operasi morfologi terhadap bentuk dan ukuran objek.

## Dataset

Eksperimen menggunakan dua gambar:

| Gambar | Deskripsi | Penggunaan |
|---|---|---|
| Gambar 1 – Coins | Gambar koin dengan latar belakang bertekstur | Segmentasi Otsu dan operasi morfologi |
| Gambar 2 – Binary Objects | Gambar objek putih dengan latar belakang hitam dan noise | Pengujian operasi morfologi |

## Metode yang Digunakan

### 1. Otsu Thresholding

Metode segmentasi berbasis threshold otomatis yang digunakan untuk memisahkan foreground dan background berdasarkan distribusi intensitas piksel.

### 2. Morphological Processing

Operasi morfologi diimplementasikan menggunakan structuring element berbentuk persegi berukuran 3 × 3.

| Operasi | Fungsi |
|---|---|
| Dilation | Memperluas area foreground |
| Erosion | Memperkecil area foreground |
| Opening | Mengurangi noise foreground berukuran kecil |
| Closing | Mengisi lubang dan celah kecil pada objek |

## Struktur Repository

```text
PCD_Assignment03/
├── dataset/
│   ├── coins.png
│   └── binary_objects.png
├── results/
│   ├── coins/
│   └── binary_objects/
├── PCD_Assignment03.ipynb
└── README.md
```

## Teknologi yang Digunakan

- Python
- NumPy
- Matplotlib
- PIL (Pillow)
- Google Colab

## Cara Menjalankan

1. Clone repository ini atau unduh seluruh file yang tersedia.
2. Buka `PCD_Assignment03.ipynb` menggunakan Google Colab.
3. Jalankan setiap cell secara berurutan.
4. Unggah kedua gambar dataset apabila diminta oleh notebook.
5. Amati hasil segmentasi dan perbandingan operasi morfologi.

## Implementasi

Algoritma Otsu Thresholding, dilation, erosion, opening, dan closing diimplementasikan secara mandiri menggunakan Python dan NumPy.

Library digunakan untuk membantu proses pembacaan gambar, perhitungan numerik, serta visualisasi hasil, bukan untuk menggantikan implementasi algoritma utama.

---

**Mata Kuliah:** Pengolahan Citra Digital  
**Tugas:** PCD Assignment 03
