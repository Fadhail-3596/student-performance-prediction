# Prediksi Performa Siswa (Student Performance Prediction)

Proyek *Machine Learning* untuk memprediksi nilai akhir siswa menggunakan dataset Student Performance dari UCI Machine Learning Repository.

## 📌 Gambaran Umum

Proyek ini bertujuan untuk mempelajari pola performa siswa dan membangun model regresi untuk memprediksi nilai akhir siswa (`G3`) berdasarkan faktor demografis, sosial, dan akademik.

Fitur nilai periode sebelumnya (`G1` dan `G2`) tidak digunakan agar prediksi berfokus pada fitur lainnya, bukan pada nilai yang sudah diperoleh siswa di periode sebelumnya.

## 🎯 Tujuan Proyek

- Memahami dan mengeksplorasi dataset.
- Melakukan analisis data eksploratif (*Exploratory Data Analysis* / EDA).
- Menyiapkan fitur dan melakukan preprocessing data.
- Melatih dan membandingkan beberapa model regresi.
- Mengevaluasi performa model menggunakan MAE, RMSE, dan R².
- Menganalisis kesalahan prediksi untuk memahami keterbatasan model.

## 📊 Dataset

- **Sumber:** [UCI Student Performance Dataset](https://doi.org/10.24432/C5TG7T)
- **Jumlah data:** 649 siswa
- **Target prediksi:** `G3` (nilai akhir siswa)
- **Jenis permasalahan:** Regresi

Informasi lengkap mengenai dataset dan ketentuan penggunaannya dapat dilihat pada sumber resmi UCI.

## 🛠️ Teknologi yang Digunakan

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Google Colab

## ⚙️ Tahapan Pengerjaan

1. Memuat dan memeriksa dataset.
2. Melakukan eksplorasi dan visualisasi data.
3. Memilih fitur dan membagi data menjadi data latih dan data uji.
4. Melakukan preprocessing menggunakan pipeline.
5. Membuat model baseline sebagai pembanding.
6. Melatih tiga model regresi.
7. Membandingkan hasil evaluasi model.
8. Menganalisis kesalahan prediksi.
9. Melakukan pemeriksaan akhir untuk memvalidasi hasil.

## 📈 Hasil Evaluasi Model

Evaluasi dilakukan menggunakan tiga metrik, yaitu Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), dan R².

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Random Forest | 2.0264 | 2.8215 | 0.1837 |
| Gradient Boosting | 2.1049 | 2.8010 | 0.1955 |
| Linear Regression | 2.1564 | 2.8618 | 0.1602 |
| Baseline (Mean) | 2.3946 | 3.1726 | -0.0322 |

### Kesimpulan Hasil

- **Random Forest** menghasilkan MAE terendah, yaitu 2.0264.
- **Gradient Boosting** menghasilkan RMSE terendah, yaitu 2.8010, serta R² tertinggi, yaitu 0.1955.
- Ketiga model regresi menghasilkan performa yang lebih baik daripada baseline berdasarkan ketiga metrik yang digunakan.

Meskipun demikian, nilai R² menunjukkan bahwa kemampuan model dalam menjelaskan variasi nilai akhir siswa masih terbatas. Hasil prediksi perlu dipahami dengan mempertimbangkan keterbatasan tersebut.

## 🖼️ Dokumentasi Proyek

Screenshot eksplorasi data, perbandingan model, dan hasil analisis dapat dilihat pada folder `screenshots/`.

<!-- Tambahkan gambar setelah diunggah ke repository GitHub. -->

## 🚀 Cara Menjalankan Proyek

1. Unduh atau salin repository ini ke komputer.
2. Pasang library yang diperlukan dengan perintah berikut:

   ```bash
   pip install -r requirements.txt
   ```

3. Buka file `Student_Performance_Prediction.ipynb` menggunakan Google Colab atau Jupyter Notebook.
4. Jalankan seluruh sel notebook secara berurutan dari awal hingga akhir.

## ⚠️ Keterbatasan Proyek

- Performa model masih terbatas dalam menjelaskan variasi nilai akhir siswa.
- Tidak semua faktor yang memengaruhi performa siswa tersedia dalam dataset.
- Hasil evaluasi bergantung pada data, pemilihan fitur, dan pembagian data latih serta data uji.
- Model ini merupakan proyek pembelajaran dan eksplorasi, bukan alat untuk menentukan kemampuan siswa secara mutlak.

## 👤 Tentang Proyek

Proyek ini dibuat sebagai bagian dari pembelajaran dan pengembangan portofolio di bidang *Data Science* dan *Machine Learning*.
