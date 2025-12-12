# **LAPORAN FINAL PROJECT**: Hotel Bookings Data
## Kelompok 8

> 5052241009 Violita Karina Putri
> 
> 5052241027 Azizah Adilah
> 
> 5052241032 Aqila Ikhza Kusumawardani
> 
> 5052241035 Najwa Aulia

# 🏨 Final Project: Data Wrangling dan Analisis Permintaan Pemesanan Hotel

Proyek ini bertujuan untuk mendemonstrasikan proses Data Wrangling (pembersihan, transformasi, dan rekayasa fitur) pada dataset permintaan pemesanan hotel, yang kemudian dilanjutkan dengan analisis eksploratif (EDA) untuk mendapatkan *insight* mengenai tingkat pembatalan dan perbedaan profil pemesanan antara berbagai tipe hotel.

**Dataset:** Hotel Booking Demand Dataset (hotels.csv)

## 📌 Tujuan Utama Analisis

1.  **Mengatasi Kualitas Data:** Mengidentifikasi dan menangani *missing values* (terutama pada kolom `company` dan `agent`), nilai duplikat, serta inkonsistensi data kategorikal.
2.  **Feature Engineering:** Menggabungkan kolom tanggal untuk analisis musiman dan membuat fitur total lama menginap.
3.  **Analisis Pembatalan:** Menganalisis faktor-faktor (misalnya, `lead_time`, `deposit_type`, `adr`) yang paling memengaruhi tingkat pembatalan (`is_canceled`).
4.  **Perbandingan Hotel:** Membandingkan rata-rata harga harian (`adr`) dan profil pemesanan antara **City Hotel** dan **Resort Hotel**.

## 📁 Struktur Repositori

Repositori ini mengikuti struktur standar proyek Data Science memastikan pemisahan data mentah, data bersih, dan *notebook* analisis.

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
