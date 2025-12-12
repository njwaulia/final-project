# 🏨 FINAL PROJECT TSDW: Analisis Permintaan Pemesanan Hotel
## Kelompok 8

> 5052241009 Violita Karina Putri
> 
> 5052241027 Azizah Adilah
> 
> 5052241032 Aqila Ikhza Kusumawardani
> 
> 5052241035 Najwa Aulia

## ✨ Deskripsi 

Proyek ini bertujuan untuk mendemonstrasikan proses **Data Wrangling** (pembersihan, transformasi, dan rekayasa fitur) pada dataset permintaan pemesanan hotel. Dilanjutkan dengan analisis eksploratif (EDA) untuk mendapatkan *insight* mengenai tingkat pembatalan dan perbedaan profil pemesanan antara dua tipe hotel: Resort Hotel dan City Hotel.

**Dataset:** Hotel Booking Demand Dataset (hotels.csv)

## 📌 Tujuan Utama Analisis

1.  **Mengatasi Kualitas Data:** Mengidentifikasi dan mengatasi masalah kualitas data (nilai hilang, duplikasi, format yang tidak sesuai).
2.  **Menganalisis Pembatalan:** Variabel manakah (misalnya `lead_time`, `deposit_type`, atau `booking_changes`) yang paling berkorelasi dengan status pembatalan (`is_canceled`)?
3.  **Membandingkan Hotel:** Bagaimana rata-rata Harga Harian (`adr`) bervariasi antara City Hotel dan Resort Hotel berdasarkan musim kedatangan?
4.  **Menangani Missing Values:** Bagaimana *missing values* di kolom `company` dan `agent` dapat diolah sedemikian rupa sehingga tetap memberikan *insight* dalam analisis akhir?

### Tujuan Exploratory Data Analysis (EDA)

* **Mengukur Proporsi Pembatalan:** Melihat distribusi status pemesanan (`is_canceled`).
* **Menganalisis Tren Musiman:** Memvisualisasikan total pemesanan berdasarkan bulan kedatangan (`arrival_date_month`).
* **Membandingkan Harga:** Melihat distribusi harga harian rata-rata (`adr`) antara City Hotel dan Resort Hotel.
* **Korelasi Lead Time:** Membandingkan durasi waktu tunggu (`lead_time`) antara pemesanan yang dibatalkan dan yang tidak dibatalkan.

## 📁 Struktur Repositori

Repositori ini mengikuti struktur standar proyek Data Science, memastikan pemisahan data mentah, data bersih, dan *notebook* analisis:

## Tipe Data Setelah Cleaning

| Kolom                        | Tipe Data (dtype)      | Keterangan                              |
|------------------------------|------------------------|-----------------------------------------|
| hotel                        | object                 | Kategori (Resort Hotel / City Hotel)    |
| is_canceled                  | int64                  | 0 = tidak batal, 1 = batal              |
| lead_time                    | int64                  | Hari sebelum tanggal kedatangan         |
| arrival_date_year            | int64                  | Tahun kedatangan                        |
| arrival_date_month           | int64                 | Bulan kedatangan                        |
| arrival_date_week_number     | int64                  | Nomor minggu dalam tahun                |
| arrival_date_day_of_month    | int64                  | Tanggal dalam bulan                     |
| stays_in_weekend_nights      | int64                  | Malam akhir pekan                       |
| stays_in_week_nights         | int64                  | Malam hari biasa                        |
| adults                       | int64                  | Jumlah dewasa                           |
| children                     | int64                  | Jumlah anak (setelah imputasi)          |
| babies                       | int64                  | Jumlah bayi                             |
| meal                         | object                 | Tipe makan (BB, HB, FB, SC, dll)        |
| country                      | object                 | Kode negara (imputasi Unknown)          |
| market_segment               | object                 | Segmen pasar                            |
| distribution_channel         | object                 | Kanal distribusi                        |
| is_repeated_guest            | int64                  | Tamu berulang                           |
| previous_cancellations       | int64                  | Pembatalan sebelumnya                   |
| previous_bookings_not_canceled | int64                | Booking sebelumnya tidak dibatalkan     |
| reserved_room_type           | object                 | Tipe kamar yang dipesan                 |
| assigned_room_type           | object                 | Tipe kamar yang diberikan               |
| booking_changes              | int64                  | Jumlah perubahan booking                |
| deposit_type                 | object                 | Tipe deposit                            |
| agent                        | float64                  | Kode agen (0 = tidak pakai agen)        |
| company                      | float64                  | Kode company                            |
| days_in_waiting_list         | int64                  | Hari menunggu                           |
| customer_type                | object                 | Tipe pelanggan                          |
| adr                          | float64                | Average Daily Rate (setelah cleaning)   |
| required_car_parking_spaces  | int64                  | Tempat parkir dibutuhkan                |
| total_of_special_requests    | int64                  | Permintaan khusus                       |
| reservation_status           | object                 | Status reservasi                        |
| reservation_status_date      | datetime64[ns]         | Tanggal status reservasi                |
| arrival_date                 | datetime64[ns]         | Tanggal kedatangan (feature baru)       |
| total_stays                  | int64                  | Total malam menginap (feature baru)     |

## 🛠️ Cara Menjalankan Proyek

1.  **Clone Repositori:**
    ```bash
    git clone [https://github.com/najwaauliaaa/final-project.git](https://github.com/najwaauliaaa/final-project.git)
    cd final-project-tsdw
    ```

2.  **Instal Dependencies:**
    Instal semua package Python yang diperlukan agar *notebook* dapat berjalan dengan lingkungan yang sama:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Jalankan Notebook:**
    Buka `notebooks/final_project.ipynb` di Google Colab atau Jupyter Notebook dan eksekusi setiap *cell* secara berurutan.








