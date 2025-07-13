# Hospital LOS Prediction with LightGBM

Repositori ini berisi kode dan sumber daya untuk memprediksi Lama Rawat Inap atau *Length of Stay* (LOS) pasien di rumah sakit menggunakan model **LightGBM**. Proyek ini bertujuan untuk membantu manajemen rumah sakit dalam mengalokasikan sumber daya secara lebih efisien.

-----

## 📜 Daftar Isi

  * [Ringkasan Proyek](https://www.google.com/search?q=%23-ringkasan-proyek)
  * [Dataset](https://www.google.com/search?q=%23-dataset)
  * [Metodologi](https://www.google.com/search?q=%23-metodologi)
  * [Hasil](https://www.google.com/search?q=%23-hasil)
  * [Cara Menggunakan](https://www.google.com/search?q=%23-cara-menggunakan)

-----

## 📌 Ringkasan Proyek

Memprediksi lama rawat inap pasien adalah tantangan penting dalam manajemen operasional rumah sakit. Prediksi yang akurat dapat membantu mengoptimalkan penggunaan tempat tidur, mengurangi waktu tunggu pasien, dan meningkatkan kualitas layanan secara keseluruhan. Proyek ini memanfaatkan model *machine learning* **LightGBM** yang dikenal cepat dan efisien untuk menangani kumpulan data berukuran besar dan melakukan prediksi regresi pada data tabular.

-----

## 📊 Dataset

Dataset yang digunakan dalam proyek ini berisi informasi demografis dan klinis anonim dari pasien. Fitur-fitur utama yang dianalisis meliputi:

  * **Informasi Pasien**: Usia, jenis kelamin, dan data demografis lainnya.
  * **Detail Kunjungan**: Tipe admisi, departemen tujuan, dan sumber rujukan.
  * **Kondisi Klinis**: Diagnosis awal dan indikator kesehatan lainnya.
  * **Target Variabel**: `Length of Stay` (dalam hari), yang merupakan variabel target untuk diprediksi.

-----

## ⚙️ Metodologi

Alur kerja proyek ini dibagi menjadi beberapa tahap utama:

1.  **Pra-pemrosesan Data**: Membersihkan data dari nilai yang hilang (*missing values*), mengonversi tipe data, dan melakukan *encoding* pada fitur-fitur kategorikal agar dapat diproses oleh model.
2.  **Analisis Data Eksploratif (EDA)**: Menganalisis distribusi data dan hubungan antar fitur untuk mendapatkan wawasan yang lebih dalam.
3.  **Rekayasa Fitur (*Feature Engineering*)**: Membuat fitur-fitur baru dari data yang ada untuk meningkatkan performa model.
4.  **Pelatihan Model**: Melatih model regresi menggunakan algoritma **LightGBM**. Data dibagi menjadi set pelatihan dan set pengujian untuk evaluasi yang objektif.
5.  **Evaluasi Model**: Kinerja model dievaluasi menggunakan metrik **Mean Absolute Error (MAE)** untuk mengukur rata-rata selisih antara nilai prediksi dan nilai aktual.

-----

## ✨ Hasil

Model LightGBM yang telah dilatih menunjukkan kinerja yang baik dalam memprediksi lama rawat inap pasien. Metrik evaluasi utama yang diperoleh adalah:

  * **R2-Score**: 0.97 

Hasil ini menunjukkan bahwa model mampu memberikan estimasi lama rawat inap dengan tingkat akurasi yang memuaskan untuk keperluan praktis di lingkungan rumah sakit.

-----

## 🚀 Cara Menggunakan

Untuk menjalankan proyek ini di lingkungan lokal Anda, ikuti langkah-langkah berikut:

**1. Klon Repositori**

```bash
git clone https://github.com/your-username/hospital-los-prediction-lightgbm.git
cd hospital-los-prediction-lightgbm
```

**2. Instal Dependensi**
Pastikan Anda memiliki Python 3.9 atau versi yang lebih baru. Instal semua pustaka yang diperlukan menggunakan `pip`.

```bash
pip install pandas numpy scikit-learn lightgbm jupyter
```

**3. Jalankan Notebook**
Buka dan jalankan Jupyter Notebook `Datathon_update (2).ipynb` untuk melihat seluruh proses, mulai dari analisis data hingga evaluasi model.

```bash
jupyter notebook "Datathon_update (2).ipynb"
```
