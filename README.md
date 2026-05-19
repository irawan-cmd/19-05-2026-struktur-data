# 🧩 Algoritma Backtracking — Python

Kumpulan implementasi algoritma **backtracking** dan **rekursif** untuk menyelesaikan tiga masalah klasik dalam ilmu komputer.

---

## 📋 Daftar Isi

- [Tentang Proyek](#tentang-proyek)
- [Masalah yang Diselesaikan](#masalah-yang-diselesaikan)
  - [1. N-Queens (N-Ratu)](#1-n-queens-n-ratu)
  - [2. Knight's Tour (Tur Kuda)](#2-knights-tour-tur-kuda)
  - [3. Knapsack Problem](#3-knapsack-problem)
- [Struktur Proyek](#struktur-proyek)
- [Cara Menjalankan](#cara-menjalankan)
- [Kompleksitas Algoritma](#kompleksitas-algoritma)
- [Teknologi](#teknologi)

---

## 📖 Tentang Proyek

Proyek ini berisi implementasi tiga algoritma klasik menggunakan pendekatan **backtracking** dan **rekursif** dalam bahasa Python. Setiap program menerima input dari pengguna dan menghasilkan solusi secara interaktif.

---

## 🔢 Masalah yang Diselesaikan

### 1. N-Queens (N-Ratu)

> Tempatkan N ratu di papan catur N×N sehingga tidak ada dua ratu yang saling menyerang.

**Algoritma:** Backtracking rekursif baris per baris

**Cara kerja:**
- Coba tempatkan ratu di setiap kolom pada baris saat ini
- Periksa apakah posisi aman (tidak satu kolom, baris, atau diagonal)
- Jika aman, lanjut ke baris berikutnya
- Jika gagal, mundur (*backtrack*) dan coba kolom lain

```
Contoh solusi untuk N=4:

. Q . .
. . . Q
Q . . .
. . Q .
```

---

### 2. Knight's Tour (Tur Kuda)

> Temukan urutan langkah kuda catur sehingga mengunjungi setiap petak di papan N×N tepat satu kali.

**Algoritma:** Backtracking + Warnsdorff's Heuristic

**Cara kerja:**
- Kuda bergerak dalam pola huruf "L" (2+1 atau 1+2 kotak)
- Gunakan heuristik Warnsdorff: selalu pilih petak dengan paling sedikit kemungkinan gerakan lanjutan
- Jika tidak ada solusi, mundur dan coba jalur lain

---

### 3. Knapsack Problem (Masalah Ransel)

> Cari kombinasi barang dari sekumpulan barang dengan berat berbeda yang totalnya tepat sama dengan berat target.

**Algoritma:** Rekursif + Backtracking (Subset Sum)

**Cara kerja:**
- Untuk setiap barang, ada dua pilihan: ambil atau lewati
- Rekursif mencoba semua kombinasi
- Kembalikan kombinasi yang totalnya sama dengan target

```
Contoh:
Barang  : [2, 5, 6, 9, 12, 14, 20]
Target  : 30
Solusi  : [2, 5, 9, 14] → Total: 30 ✓
```

---

## 📁 Struktur Proyek

```
backtracking-python/
├── nqueens.py
├── knights_tour.py
├── knapsack.py
└── README.md
```

---

## ▶️ Cara Menjalankan

Prasyarat: Python 3.x

```bash
git clone https://github.com/username/backtracking-python.git
cd backtracking-python
```

```bash
python nqueens.py
python knights_tour.py
python knapsack.py
```

---

## 📊 Kompleksitas Algoritma

| Masalah | Algoritma | Waktu | Ruang |
|---|---|---|---|
| N-Queens | Backtracking | O(N!) | O(N²) |
| Knight's Tour | Backtracking + Warnsdorff | O(N²) | O(N²) |
| Knapsack | Rekursif / Backtracking | O(2ᴺ) | O(N) |

---

## 🛠️ Teknologi

- Python 3.x
- Algoritma: Backtracking & Rekursif
- Lisensi: MIT

---
