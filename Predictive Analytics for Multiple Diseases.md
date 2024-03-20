# Laporan Proyek Machine Learning - Syaiful Hendri Irawan

## Project Overview

Proyek ini bertujuan untuk membuat model machine learning yang dapat memprediksi apakah seseorang memiliki penyakit tertentu berdasarkan parameter-parameter darah yang diberikan. Data yang digunakan telah disiapkan sebelumnya dan merupakan simulasi dari data medis, termasuk parameter seperti glukosa, kolesterol, hemoglobin, dan lainnya. Penting untuk menyelesaikan proyek ini karena dapat membantu dalam diagnosa penyakit dengan cepat dan akurat, serta memberikan wawasan tentang hubungan antara parameter-parameter darah dan kondisi kesehatan seseorang.

## Business Understanding

### Problem Statements

- Bagaimana cara memprediksi apakah seseorang memiliki penyakit tertentu berdasarkan parameter darah yang diberikan?
- Bagaimana hubungan antara parameter-parameter darah tertentu dengan risiko terkena penyakit tertentu?

### Goals

- Mengembangkan model machine learning yang dapat memprediksi penyakit berdasarkan parameter darah.
- Menganalisis hubungan antara parameter-parameter darah tertentu dengan risiko terkena penyakit.

### Solution Approach 

- Menggunakan algoritma klasifikasi seperti Logistic Regression, Random Forest, dan Support Vector Machine untuk membangun model prediksi.
- Menerapkan analisis fitur untuk menentukan fitur yang paling berpengaruh dalam prediksi.

## Data Understanding

Dataset yang digunakan telah disiapkan sebelumnya dan mencakup parameter-parameter darah berikut:

- Glukosa
- Kolesterol
- Hemoglobin
- Platelets
- White Blood Cells
- Red Blood Cells
- Hematocrit
- Mean Corpuscular Volume
- Mean Corpuscular Hemoglobin
- Mean Corpuscular Hemoglobin Concentration
- Insulin
- BMI
- Systolic Blood Pressure
- Diastolic Blood Pressure
- Triglycerides
- HbA1c
- LDL Cholesterol
- HDL Cholesterol
- ALT
- AST
- Heart Rate
- Creatinine
- Troponin
- C-reactive Protein

Dataset telah disesuaikan dan dinormalisasi dalam rentang (0,1).

## Data Preparation

Dataset yang digunakan diambil dari Kaggle, yaitu [Multiple Disease Prediction](https://www.kaggle.com/datasets/ehababoelnaga/multiple-disease-prediction/data). Dataset ini telah dibersihkan dan siap digunakan, sehingga tidak diperlukan proses pembersihan data tambahan. Pada tahap ini, teknik-teknik data preparation yang digunakan meliputi:
- Mengecek nilai yang hilang.
- Menganalisis parameter yang dibutuhkan.
- Membagi dataset menjadi subset pelatihan dan pengujian untuk validasi model.

## Modeling

Dua solusi rekomendasi yang digunakan adalah:

- Logistic Regression : Digunakan untuk memprediksi probabilitas bahwa seorang pasien akan mengidap suatu penyakit tertentu berdasarkan nilai-nilai parameter darah yang diukur
- Random Forest Classifier: Menggunakan ensemble dari pohon keputusan untuk memprediksi kategori penyakit berdasarkan parameter darah.
- Support Vector Machine (SVM): Memanfaatkan pemisah linear dan fungsi kernel untuk mengklasifikasikan pasien ke dalam kategori penyakit.

## Evaluation

Metrik evaluasi yang digunakan untuk kedua model adalah akurasi, presisi, recall, dan F1 Score. Hasil model dievaluasi berdasarkan kemampuannya untuk memprediksi penyakit berdasarkan parameter darah. Metrik tersebut dihitung sebagai berikut:

- Akurasi : Proporsi prediksi yang benar dari total prediksi.
- Presisi : Proporsi prediksi positif yang benar dari semua prediksi positif.
- Recall : Proporsi sampel positif yang diprediksi dengan benar dari semua sampel positif.
- F1 Score : Ukuran yang menggabungkan akurasi, presisi, dan recall dalam satu angka tunggal
