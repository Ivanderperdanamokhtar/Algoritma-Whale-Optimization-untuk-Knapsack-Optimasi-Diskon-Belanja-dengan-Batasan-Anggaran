# Algoritma-Whale-Optimization-untuk-Knapsack-Optimasi-Diskon-Belanja-dengan-Batasan-Anggaran
Implementasi Whale Optimization Algorithm (WOA) untuk menyelesaikan masalah knapsack, dengan fokus pada optimasi diskon belanja dalam batasan anggaran. Proyek ini mencakup script Python, dataset, dan visualisasi hasil
# Penerapan Algoritma Whale Optimization untuk Permasalahan Knapsack

## Deskripsi Proyek

Proyek ini menerapkan **Whale Optimization Algorithm (WOA)** untuk menyelesaikan masalah **knapsack** dengan fokus pada optimasi diskon belanja dalam batasan anggaran tertentu. Algoritma ini mensimulasikan perilaku berburu paus bungkuk untuk menemukan solusi optimal.

Dataset yang digunakan adalah data simulasi dari situs belanja online yang mencakup informasi barang, harga diskon, harga asli, dan besaran diskon. Algoritma WOA diterapkan untuk memilih kombinasi barang yang memberikan keuntungan maksimal tanpa melebihi anggaran yang ditentukan.

## Fitur Utama

- **Penggunaan Whale Optimization Algorithm**: Menyelesaikan permasalahan knapsack dengan metode metaheuristik.
- **Visualisasi Hasil**: Menampilkan grafik hubungan antara modal dan keuntungan.
- **Fleksibilitas Parameter**: Memungkinkan pengaturan jumlah paus, iterasi maksimum, dan batasan modal.

## Struktur File

- `main.py`: Script utama untuk menjalankan algoritma WOA.
- `Data Barang UMKM Flodista Gallery - Sheet1.csv`: Dataset yang digunakan dalam penelitian ini.
- `hasil_woa.png`: Grafik hasil yang menunjukkan hubungan modal dan keuntungan.

## Prasyarat

Proyek ini menggunakan Python 3. Silakan pastikan library berikut telah diinstal:

- `pandas`
- `numpy`
- `matplotlib`

Untuk menginstalnya, jalankan perintah berikut:

```bash
pip install pandas numpy matplotlib
```

## Cara Menjalankan

1. Clone repository ini:
   ```bash
   git clone https://github.com/username/woa-knapsack.git
   ```
2. Pindah ke direktori proyek:
   ```bash
   cd woa-knapsack
   ```
3. Jalankan script utama:
   ```bash
   python main.py
   ```
4. Output akan ditampilkan di konsol dan grafik akan disimpan sebagai `hasil_woa.png`.

## Dataset

Dataset yang digunakan terdiri dari:

- **item**: Nama barang.
- **harga\_diskon**: Harga barang setelah diskon.
- **harga\_asli**: Harga asli barang sebelum diskon.
- **diskon**: Besaran diskon dalam satuan mata uang.

Contoh format data:

| item                    | harga\_diskon | harga\_asli | diskon |
| ----------------------- | ------------- | ----------- | ------ |
| Robotics Vacuum Cleaner | 149           | 229         | 80     |
| Wireless Earbuds        | 39            | 49          | 10     |

## Penjelasan Kode

### Kelas `WOA`

Kelas utama yang mengimplementasikan algoritma WOA untuk menyelesaikan masalah knapsack. Fitur utama:

- **Inisialisasi paus**: Mengatur posisi awal setiap paus dalam ruang pencarian.
- **Evaluasi kebugaran**: Menghitung keuntungan total berdasarkan solusi sementara.
- **Pembaruan posisi**: Memperbarui posisi paus berdasarkan solusi terbaik saat ini.
- **Visualisasi hasil**: Menampilkan grafik hubungan modal dan keuntungan.

### Fungsi Pendukung

- `fungsi_maks`: Menghitung total keuntungan dengan memperhatikan batasan modal maksimum.
- `total_keuntungan`: Menghitung total diskon dari solusi yang dipilih.
- `total_modal`: Menghitung total modal yang digunakan untuk solusi yang dipilih.

## Hasil

- Dari batasan modal \$750, algoritma menemukan kombinasi barang yang memberikan keuntungan maksimal sebesar \$1,311 dengan modal \$747.
- Grafik hasil menunjukkan hubungan linear positif antara modal dan keuntungan.

## Referensi

- Mirjalili, S., & Lewis, A. (2016). The Whale Optimization Algorithm. Advances in Engineering Software.

## Kontributor:
- Ivander Perdana Mokhtar 
- Christian A. N. Biran
- Andrian Agustinus L. Gaul 
- Siti Nur Azizah
- Rahmi Agustin 



