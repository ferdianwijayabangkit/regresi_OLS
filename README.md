# 📊 Analisis Regresi Linier Berganda (OLS) dengan Python & R

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![R](https://img.shields.io/badge/R-4.0+-purple.svg)
![License](https://img.shields.io/badge/License-MIT-red.svg)
![Affiliation](https://img.shields.io/badge/Affiliation-UNTIRTA-orange.svg)

Repositori ini menyajikan alur kerja lengkap untuk analisis regresi linier berganda menggunakan metode *Ordinary Least Squares* (OLS). Proyek ini menyediakan implementasi paralel di **Python** dan **R** untuk memodelkan hubungan antara variabel dependen dan independen, serta melakukan validasi asumsi klasik secara komprehensif.

## ✨ Fitur Utama

- **🧠 Pemodelan Lintas Platform**: Membangun model OLS yang identik menggunakan `statsmodels` di Python dan fungsi `lm()` di R, memungkinkan perbandingan langsung.
- **🔬 Uji Asumsi Klasik Lengkap**: Melakukan serangkaian uji statistik formal untuk memastikan validitas dan reliabilitas model, mencakup:
  - **Normalitas Sisaan** (Uji Shapiro-Wilk)
  - **Homoskedastisitas** (Uji Breusch-Pagan)
  - **Autokorelasi** (Uji Durbin-Watson)
  - **Multikolinearitas** (Variance Inflation Factor - VIF)
- **📈 Diagnostik Visual Komparatif**: Menghasilkan plot diagnostik standar di kedua platform (seperti *Residuals vs Fitted* dan *Normal Q-Q Plot*) untuk evaluasi visual.
- **✔️ Evaluasi Kebaikan Model**: Menghitung dan menyajikan metrik evaluasi kunci (*R-squared*, *Adjusted R-squared*, AIC, dan BIC) untuk menilai performa model.

## 🔧 Tumpukan Teknologi (Tech Stack)

- **Bahasa**: `Python 3.7+`, `R 4.0+`
- **Pustaka Python**: `statsmodels`, `pandas`, `scipy`, `matplotlib`, `seaborn`, `openpyxl`
- **Pustaka R**: `lmtest`, `car`, `readxl`, `knitr`, `rmarkdown`
- **Lingkungan**: `Jupyter Notebook / Lab`, `RStudio`

## 🚀 Cara Memulai

### Prasyarat
- **Perangkat Lunak**: Python 3.7+, R 4.0+, Jupyter Notebook/Lab, dan RStudio.
- **File Data**: Pastikan file `data_simulasi_gls.xlsx` berada di dalam direktori proyek Anda.

### Instalasi & Penggunaan

1.  **Unduh Repositori**: *Clone* atau unduh proyek ini ke komputer Anda.

2.  **Untuk Pengguna Python (`.ipynb` atau `.py`)**:
    - Buka terminal atau command prompt, lalu instal paket yang diperlukan:
      ```bash
      pip install pandas openpyxl statsmodels scipy matplotlib seaborn jupyterlab
      ```
    - Jalankan Jupyter Lab/Notebook dan buka file Python.
    - **Penting**: Ubah `file_path` di dalam skrip agar sesuai dengan lokasi file `data_simulasi_gls.xlsx` di komputer Anda.

3.  **Untuk Pengguna R (`.Rmd` atau `.R`)**:
    - Buka RStudio, lalu instal paket yang diperlukan dengan menjalankan perintah berikut di *console*:
      ```r
      install.packages(c("lmtest", "car", "readxl", "knitr", "rmarkdown"))
      ```
    - Buka file `.Rmd` atau `.R`.
    - **Penting**: Ubah `file_path` di dalam skrip agar sesuai dengan lokasi file `data_simulasi_gls.xlsx` di komputer Anda.

4.  **Jalankan Analisis**: Eksekusi semua sel (Python) atau *chunks* (R) untuk mereplikasi seluruh proses analisis.

## 📊 Metrik Hasil & Ringkasan Output

Analisis ini menghasilkan ringkasan model yang detail serta hasil dari berbagai uji diagnostik. Metrik utama yang dievaluasi adalah sebagai berikut:

| Metrik              | Deskripsi                                                                 | Contoh Nilai  |
| ------------------- | ------------------------------------------------------------------------- | ------------- |
| `R-squared`         | Persentase varians variabel dependen yang dijelaskan oleh model.          | `0.152`       |
| `Adj. R-squared`    | `R-squared` yang disesuaikan dengan jumlah prediktor dalam model.         | `0.125`       |
| `F-statistic`       | Statistik uji untuk signifikansi keseluruhan model regresi.               | `5.613`       |
| `Prob (F-statistic)`| P-value yang terkait dengan F-statistic.                                  | `0.00148`     |
| `AIC` / `BIC`       | Kriteria informasi untuk perbandingan model (nilai lebih rendah lebih baik). | `1158` / `1168` |
| `Durbin-Watson`     | Statistik untuk mendeteksi autokorelasi pada sisaan.                      | `0.697`       |
| `VIF`               | Ukuran untuk mendeteksi multikolinearitas antar variabel independen.      | `< 5`         |


## ⚖️ Lisensi & Ketentuan Penggunaan

- **Hak Cipta**: © 2025 Ferdian Bangkit Wijaya - Seluruh Hak Dilindungi.
- **Penggunaan Akademik**: Diizinkan secara bebas untuk keperluan penelitian, tesis, dan pendidikan non-komersial dengan atribusi.
- **Penggunaan Komersial**: Memerlukan izin tertulis dari pengembang.

## 👨‍💻 Author

- **Ferdian Bangkit Wijaya**
- Program Studi Statistika, Fakultas Teknik
- **Universitas Sultan Ageng Tirtayasa (UNTIRTA)**
- Banten, Indonesia 🇮🇩

---

> Proyek ini dirancang sebagai panduan komparatif, menunjukkan bagaimana analisis statistik fundamental dapat dilakukan secara konsisten di dua ekosistem ilmu data terpopuler.
