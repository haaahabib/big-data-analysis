# Analisis dan Prediksi Hotel Bookings Data

## Daftar Isi

1. [Deskripsi](#deskripsi)
2. [Tujuan](#tujuan)
3. [Dataset](#dataset)
4. [Data Dictionary](#data-dictionary)
5. [Library yang Diperlukan](#library-yang-diperlukan)
6. [Proses Analisis](#proses-analisis)
7. [Cara Menjalankan Proyek](#cara-menjalankan-proyek)

## Deskripsi

Proyek ini bertujuan untuk menganalisis dan memprediksi pembatalan reservasi hotel menggunakan dataset *Hotel Bookings Data*. Dengan menggunakan algoritma *Random Forest Classifier*, model ini dapat memprediksi kemungkinan pembatalan berdasarkan berbagai fitur pemesanan, yang membantu manajemen hotel dalam pengambilan keputusan yang lebih baik.

## Tujuan

- Melakukan analisis statistik untuk menemukan pola pembatalan reservasi dalam data hotel.
- Membangun model prediksi pembatalan reservasi menggunakan algoritma *Random Forest Classifier*.
- Memberikan rekomendasi untuk meningkatkan strategi pengelolaan reservasi hotel berdasarkan analisis data.

## Dataset

Data ini berasal dari kumpulan data permintaan pemesanan hotel terbuka dari [Antonio, Almeida dan Nunes, 2019](https://www.sciencedirect.com/science/article/pii/S2352340918315191#f0010).

## Data Dictionary

| Variabel | Tipe Data | Deskripsi |
| :--- | :--- | :--- |
| **hotel** | Kategorikal | Jenis hotel ('Resort Hotel' atau 'City Hotel'). |
| **is_canceled** | Kategorikal | Status pembatalan (0: Tidak Batal, 1: Batal). |
| **lead_time** | Numerik | Jumlah hari antara tanggal pemesanan dan tanggal kedatangan. |
| **arrival_date_year** | Numerik | Tahun kedatangan. |
| **arrival_date_month** | Kategorikal | Bulan kedatangan. |
| **arrival_date_week_number** | Numerik | Nomor minggu dalam tahun untuk tanggal kedatangan. |
| **arrival_date_day_of_month**| Numerik | Hari dalam bulan untuk tanggal kedatangan. |
| **stays_in_weekend_nights** | Numerik | Jumlah malam menginap pada akhir pekan (Sabtu atau Minggu). |
| **stays_in_week_nights** | Numerik | Jumlah malam menginap pada hari kerja (Senin sampai Jumat). |
| **adults** | Numerik | Jumlah tamu dewasa. |
| **children** | Numerik | Jumlah anak-anak. |
| **babies** | Numerik | Jumlah bayi. |
| **meal** | Kategorikal | Jenis paket makan yang dipesan. |
| **country** | Kategorikal | Negara asal tamu (kode 3 huruf). |
| **market_segment** | Kategorikal | Segmen pasar pemesanan (misalnya, 'Online TA'). |
| **distribution_channel** | Kategorikal | Saluran distribusi pemesanan (misalnya, 'TA/TO'). |
| **is_repeated_guest** | Kategorikal | Apakah tamu pernah menginap sebelumnya (0: Tidak, 1: Ya). |
| **previous_cancellations** | Numerik | Jumlah pembatalan sebelumnya oleh tamu ini. |
| **previous_bookings_not_canceled** | Numerik | Jumlah pemesanan yang tidak dibatalkan sebelumnya oleh tamu ini. |
| **reserved_room_type** | Kategorikal | Kode untuk tipe kamar yang dipesan. |
| **assigned_room_type** | Kategorikal | Kode untuk tipe kamar yang didapat saat check-in. |
| **booking_changes** | Numerik | Jumlah perubahan yang dibuat pada pemesanan. |
| **deposit_type** | Kategorikal | Jenis deposit yang diberikan ('No Deposit', 'Non Refund', 'Refundable'). |
| **agent** | Numerik | ID agen perjalanan yang melakukan pemesanan. |
| **company** | Numerik | ID perusahaan yang melakukan pemesanan. |
| **days_in_waiting_list** | Numerik | Jumlah hari pemesanan berada di daftar tunggu. |
| **customer_type** | Kategorikal | Tipe pelanggan ('Transient', 'Contract', 'Transient-Party', 'Group'). |
| **adr** | Numerik | *Average Daily Rate* (rata-rata harga kamar per hari). |
| **required_car_parking_spaces** | Numerik | Jumlah tempat parkir yang dibutuhkan. |
| **total_of_special_requests** | Numerik | Jumlah permintaan khusus yang dibuat oleh tamu. |
| **reservation_status** | Kategorikal | Status terakhir reservasi ('Canceled', 'Check-Out', 'No-Show'). |
| **reservation_status_date** | Tanggal | Tanggal saat status terakhir ditetapkan. |

## Library yang Diperlukan

- pandas==2.0.3
- numpy==1.25.2
- matplotlib==3.7.2
- seaborn==0.12.2
- scikit-learn

## Proses Analisis

1.  **Muat Data**: Mengimpor dataset `hotels.csv` ke dalam DataFrame pandas.
2.  **Pembersihan Data**: Menangani nilai yang hilang dan memperbaiki tipe data yang tidak konsisten.
3.  **Eksplorasi Data**: Membuat visualisasi data untuk memahami distribusi dan korelasi antar fitur.
4.  **Modeling**: Membangun model prediksi menggunakan *Random Forest Classifier* setelah membagi data menjadi set pelatihan dan pengujian.
5.  **Evaluasi Model**: Menilai performa model menggunakan metrik seperti akurasi, presisi, recall, dan F1-score.
6.  **Rekomendasi**: Memberikan wawasan dan rekomendasi bisnis berdasarkan hasil analisis.

## Cara Menjalankan Proyek

### 1. Cloning di VS Code

1.  Buka **VS Code** dan buka **Terminal**.
2.  Jalankan perintah berikut untuk meng-clone repositori:
    ```bash
    git clone https://github.com/haaahabib/big-data-analysis.git
    ```

### 2. Cloning di Google Colab

1.  Buka [Google Colab](https://colab.research.google.com/) dan buat **Notebook baru**.
2.  Jalankan perintah berikut di dalam cell untuk meng-clone repositori:
    ```bash
    !git clone https://github.com/haaahabib/big-data-analysis.git
    ```
3.  Pindah ke direktori proyek:
    ```bash
    cd Big-Data-Analysis
    ```
4.  Setelah itu, Anda dapat membuka file `notebook.ipynb` dan menjalankannya. Pastikan semua library sudah terinstal dengan menjalankan cell pertama di notebook.
