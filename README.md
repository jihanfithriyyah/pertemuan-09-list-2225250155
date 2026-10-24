# Pertemuan 09: List dan Pengolahan Data Numerik

- **Nama:** [Jihan Fithriyyah]
- **NIM:** [2225250155]
- **Kelas:** [3A]
- **Program Studi:** S1 Pendidikan Matematika

---

## Tujuan
Praktikum ini bertujuan untuk:
1. Memahami konsep struktur data list/array dalam Python.
2. Mengakses, memodifikasi, dan memanipulasi elemen list dengan indeks dan *slicing*.
3. Mengolah data numerik menggunakan fungsi bawaan (`sum`, `len`, `min`, `max`) serta perulangan (*looping*).
4. Mengimplementasikan fungsi yang menerima *parameter* berupa list.
5. Menguji program di VS Code dan mengunggah hasil kerja secara bertahap ke GitHub.

---

## Struktur Program

```text
pertemuan-09-list-NIM/
├── README.md
├── .gitignore
├── latihan/
│   ├── 01_buat_list.py
│   ├── 02_indeks_slicing.py
│   ├── 03_manipulasi_list.py
│   ├── 04_agregasi_nilai.py
│   ├── 05_filter_kelulusan.py
│   └── 06_fungsi_statistik.py
└── praktik/
    └── analisis_nilai_mahasiswa.py

## Penjelasan File
latihan/: Berisi file-file latihan dasar pengolahan list (membuat list, akses indeks/slicing, manipulasi elemen, perhitungan agregasi, filtering, dan penerapan fungsi statistik).
praktik/analisis_nilai_mahasiswa.py: Program utama yang menyimpan sekumpulan nilai mahasiswa, menghitung ringkasan statistik (total, rata-rata, min, max), serta mengklasifikasikan kelulusan mahasiswa.

## Cara Menjalankan Program
Buka terminal di VS Code pada direktori utama proyek, lalu jalankan perintah berikut:
Menjalankan File Latihan
```Bash
python3 latihan/01_buat_list.py
python3 latihan/02_indeks_slicing.py
python3 latihan/03_manipulasi_list.py
python3 latihan/04_agregasi_nilai.py
python3 latihan/05_filter_kelulusan.py
python3 latihan/06_fungsi_statistik.py

Menjalankan Program Praktik Utama
Bash
python3 praktik/analisis_nilai_mahasiswa.py

## Test Case
Berikut adalah tabel hasil pengujian untuk program analisis_nilai_mahasiswa.py:
Data Input / Kondisi	Hal yang Diperiksa	Hasil yang Diharapkan	Hasil Aktual	Status
[60, 70, 80]	Rata-rata	70.00	70.00	Pass
[60, 70, 80]	Minimum / Maksimum	Minimum = 60, Maksimum = 80	Minimum = 60, Maksimum = 80	Pass
[60, 70, 80]	Jumlah Lulus (Batas 60)	3	3	Pass
[59, 60, 61]	Batas Kelulusan (Batas 60)	2 lulus	2 lulus	Pass
[] (List Kosong)	Penanganan List Kosong	Mengembalikan 0 (Tidak Error/ZeroDivisionError)	0	Pass
[78, 55, 90, 67, 60, 82, 45, 71, 88, 59]	Data Praktik Utama	Total = 695, Rata-rata = 69.50, Lulus = 7, Belum Lulus = 3	Total = 695, Rata-rata = 69.50, Lulus = 7, Belum Lulus = 3	Pass

## Refleksi
Hal yang Dipahami: Saya memahami bahwa penggunaan struktur data list jauh lebih efisien dibandingkan menggunakan banyak variabel terpisah saat mengolah kumpulan data. Saya juga memahami bahwa indeks Python dimulai dari 0 dan indeks negatif (-1) berguna untuk mengakses elemen dari arah belakang.
Kesalahan yang Berhasil Diperbaiki: Saat menghitung rata-rata dari list kosong, program awalnya berpotensi mengalami ZeroDivisionError. Hal ini berhasil diatasi dengan menambahkan pengecekan if len(data) == 0: sebelum melakukan pembagian.
