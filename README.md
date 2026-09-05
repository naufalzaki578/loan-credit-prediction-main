# 🏦 AI Credit Scoring: Prediksi Kelayakan Kredit Bank

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-1.5+-brightgreen.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/naufalzaki578/loan-credit-prediction-main/blob/main/loan_credit_project.ipynb)


## 📌 Deskripsi Proyek
Proyek ini adalah implementasi **Machine Learning (*End-to-End*)** untuk mengotomatisasi keputusan persetujuan pengajuan kredit bank. Tujuannya adalah menekan angka **Kredit Macet (Non-Performing Loan / NPL)** dengan membedah 10 dimensi profil finansial nasabah secara simultan menggunakan algoritma **XGBoost**.

Proyek ini dibuat khusus (dan didemonstrasikan secara *live* pada sesi Webinar Data Science) guna menunjukkan bagaimana kecerdasan buatan menangani data multivariabel kompleks yang mustahil dihitung menggunakan logika matematika manual (IF-ELSE).

## ✨ Fitur Utama
1. **Data Preprocessing & Encoding:** Menangani *missing values* (imputasi) dan mengonversi data kategorik (seperti *Gender, Area Tempat Tinggal, Pekerjaan*) menjadi *machine-readable format*.
2. **Advanced Feature Engineering:** Penciptaan metrik bisnis perbankan riil, yaitu **Rasio Beban Hutang (*Debt-to-Income Ratio*)** dengan memadukan gaji gabungan dan estimasi cicilan.
3. **Machine Learning (XGBoost):** Memanfaatkan algoritma *Extreme Gradient Boosting* yang terkenal sangat tangguh dalam menaklukkan data tabular dan menangkap pola *non-linear*.
4. **Explainable AI (Kajian Data Bias):** Eksplorasi fenomena *Data Bias*, di mana AI secara statistik menganggap nasabah dengan 3 anak (*Dependents=3+*) lebih layak disetujui akibat korelasi tersembunyi antara kematangan usia dan tanggung jawab di masa lalu.
5. **Interactive UI Widget:** Simulator *live* berbasis *Dashboard UI* yang bertindak layaknya aplikasi *core banking* modern.

## 📊 Tentang Dataset
Data historis nasabah (*Loan Prediction Dataset*) yang diekstrak menggunakan 10 variabel independen:
* `Gender`, `Married`, `Dependents` (Jumlah Anak)
* `Education`, `Self_Employed` (Karyawan/Freelancer)
* `Property_Area` (Urban/Semi-Urban/Rural)
* `ApplicantIncome` (Gaji Utama) & `CoapplicantIncome` (Gaji Pasangan)
* `LoanAmount` (Nilai Pinjaman) & `Credit_History` (Riwayat Tunggakan)

## 🚀 Cara Menjalankan (*How to Run*)
1. **Clone repository ini** ke komputer Anda:
   ```bash
   git clone https://github.com/username/repo-name.git
   ```
2. **Install library** yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn xgboost ipywidgets
   ```
3. Buka file **`Prediksi_Persetujuan_Kredit.ipynb`** menggunakan Jupyter Notebook atau unggah ke Google Colab.
4. Jalankan semua baris kode (*Run All*).
5. Pada *cell* paling bawah, Anda akan menemukan **Simulator Form Aplikasi Kredit**. Ubah inputan pada *slider* dan *dropdown* untuk melihat bagaimana AI secara *real-time* mengeksekusi vonis kelayakan (*Approve/Pending/Reject*).

## 💡 Dampak Bisnis (Business Impact)
Penerapan *Machine Learning* dalam proses *Underwriting* perbankan membuktikan bahwa:
* Proses verifikasi kelayakan yang secara tradisional memakan waktu berhari-hari oleh analis manusia dapat dipersingkat menjadi **kurang dari 1 detik**.
* Meskipun kapabilitas analitik AI sangat tinggi, pengawasan dari Praktisi Data (*Data Scientist*) tetap diwajibkan untuk mencegah model bertindak diskriminatif akibat bias data dari masa lampau.

---
**👨‍💻 
