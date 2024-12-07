# Analisis dan Prediksi Hotel Bookings Data

## Table of Content

1. [Deskripsi](#Deskripsi)
2. [Tujuan](#Tujuan)
3. [Dataset](#Dataset)
4. [Data Dictionary](#Data-Dictionary)
5. [Library](#library-yang-diperlukan)
6. [Proses Analisis](#Proses-analisis-dan-prediksi-sebagai-berikut)
7. [Cloning Project](#Cara-Cloning-Repositori)
8. [Profil Pembuat](#Profil-Pembuat)

## Deskripsi 

Project ini bertujuan untuk menganalisis dan memprediksi pembatalan reservasi hotel menggunakan dataset *Hotel Bookings Data*. Dengan menggunakan algoritma *Random Forest Classifier*, model ini dapat memprediksi kemungkinan pembatalan berdasarkan berbagai fitur pemesanan, yang membantu manajemen hotel dalam pengambilan keputusan yang lebih baik.

## Tujuan

- Melakukan analisis statistik untuk menemukan pola pembatalan reservasi dalam data hotel.
- Membangun model prediksi pembatalan reservasi menggunakan algoritma *Random Forest Classifier*.
- Memberikan rekomendasi untuk meningkatkan strategi pengelolaan reservasi hotel berdasarkan analisis data.

## Dataset
Data ini berasal dari kumpulan data permintaan pemesanan hotel terbuka dari [Antonio, Almeida dan Nunes, 2019](https://www.sciencedirect.com/science/article/pii/S2352340918315191#f0010) 

## Data Dictionary
![Variabel Hotel Bookings Data](https://github.com/user-attachments/assets/07dddc03-d9d8-49d1-ade5-18bf1db4dde9)


## Library yang diperlukan

-   **pandas (v2.0.3)** - Untuk manipulasi dan analisis data
-   **numpy (v1.25.2)** - Untuk komputasi numerik
-   **matplotlib (v3.7.2)** - Untuk visualisasi data
-   **seaborn (v0.12.2)** - Untuk visualisasi data statistik

## Proses analisis dan prediksi sebagai berikut:

1. **Eksplorasi Data (EDA)**: 
   - Memahami struktur data dan melihat statistik deskriptif.
   - Memeriksa nilai yang hilang dan mendeteksi outliers.
2. **Pembersihan Data**:
   - Menangani nilai kosong dan mengonversi data kategorikal.
   - Transformasi data agar siap digunakan untuk model.
3. **Visualisasi Data**:
   - Membuat grafik distribusi dan korelasi antar fitur.
4. **Modeling**:
   - Membangun model prediksi menggunakan *Random Forest Classifier*.
   - Membagi data menjadi set pelatihan dan pengujian.
5. **Evaluasi Model**:
   - Menilai model menggunakan metrik seperti akurasi, precision, recall, dan F1-score.
6. **Rekomendasi**:
   - Memberikan wawasan dan rekomendasi berdasarkan hasil analisis.

## Cara Cloning Repositori

### 1. **Cloning di VS Code**
1. Buka **VS Code**.
2. Buka **Terminal** di VS Code.
3. Jalankan perintah berikut untuk meng-clone repositori:
   ```bash
   git clone https://github.com/haaahabib/Big-Data-Analysis.git

### 2. **Cloning di Google Colab**
1. Buka **Google Colab** di browser Anda dengan mengunjungi [Google Colab](https://colab.research.google.com/).
2. Buat **Notebook baru** dengan memilih **File > New Notebook**.
3. Jalankan perintah berikut di dalam sebuah cell untuk meng-clone repositori ke dalam Google Colab:
   ```python
   !git clone https://github.com/haaahabib/Big-Data-Analysis.git
4. Setelah repositori di-clone, jalankan perintah berikut di dalam cell untuk menginstal library yang diperlukan
   ```bash
   !pip install pandas==2.0.3
   !pip install numpy==1.25.2
   !pip install matplotlib==3.7.2
   !pip install seaborn==0.12.2

## Profil Pembuat
- **Nama**: [Muhammad Habibulloh](https://github.com/haaahabib)
- **NIM**: 202110370311259
- **Kelas**: Analisis Big Data (C)
- [**LinkedIn**](https://www.linkedin.com/in/mhabibulloh/)


