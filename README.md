# AHP Decision Support Tool (DSS) 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://en.wikipedia.org/wiki/HTML5)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Sebuah alat bantu pengambilan keputusan berbasis web yang mengimplementasikan metode **Analytic Hierarchy Process (AHP)**. Proyek ini dirancang untuk mempermudah perhitungan bobot kriteria dan pemeringkatan alternatif secara sistematis dan objektif.

---

## 👨‍🏫 Author
**Denny JC Sihombing**
- **Lecturer** at Information Systems Study Program, Atma Jaya Catholic University of Indonesia.
- **Website**: [dsihombing.github.io](https://dsihombing.github.io)
- **Lab**: DS LAB (Data Science & Decision Support)

---

## 🛠 Fitur Utama

- **Inisialisasi Dinamis**: Menentukan jumlah kriteria dan alternatif secara bebas.
- **Pairwise Comparison**: Input matriks perbandingan berpasangan yang interaktif dengan sinkronisasi nilai kebalikan (*reciprocal*) otomatis.
- **Cek Konsistensi (CR)**: Perhitungan otomatis *Consistency Index* (CI) dan *Consistency Ratio* (CR) sesuai standar Thomas L. Saaty ($CR < 0.1$).
- **Sintesis Akhir**: Perhitungan skor global untuk setiap alternatif.
- **Visualisasi Data**: Grafik batang hasil ranking menggunakan **Chart.js**.
- **Print Friendly**: Optimal untuk diekspor ke format PDF sebagai laporan keputusan.

---

## 📐 Landasan Teoretis

Alat ini menghitung bobot prioritas menggunakan metode normalisasi kolom (*Eigenvector approximation*). Rumus yang digunakan untuk mengecek konsistensi adalah:

$$CI = \frac{\lambda_{max} - n}{n - 1}$$

$$CR = \frac{CI}{RI}$$

Di mana $RI$ adalah *Random Index* yang disesuaikan dengan ordo matriks $n$.

---

## 🚀 Cara Penggunaan

1. **Clone Repositori**:
   ```bash
   git clone [https://github.com/username-anda/nama-repo.git](https://github.com/username-anda/nama-repo.git)
