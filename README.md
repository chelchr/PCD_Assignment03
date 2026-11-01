# PCD Assignment 03
## Segmentasi Citra dan Pengolahan Morfologi
Nama: Chelsea Christofera Antonioli Purnomo  
NIM: 25/558145/PA/23462  
Kelas: KOM B

## Tujuan
1. Mengimplementasikan salah satu metode segmentasi citra.
2. Mengimplementasikan beberapa operasi morfologi tanpa menggunakan fungsi siap pakai dari library pengolahan citra.
3. Membandingkan hasil segmentasi sebelum dan sesudah penerapan operasi morfologi.
4. Mengamati pengaruh setiap operasi morfologi terhadap bentuk dan ukuran objek.

## Dataset
Eksperimen menggunakan dua gambar:

| Gambar | Deskripsi | Penggunaan |
|---|---|---|
| Gambar 1 – Coins | Gambar koin dengan latar belakang bertekstur | Segmentasi Otsu dan operasi morfologi |
| Gambar 2 – Profile | Gambar profile pria dan noise pada foreground | Segmentasi Otsu dan operasi morfologi |

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
