# **LAPORAN FINAL PROJECT**: Hotel Bookings Data
## Kelompok 8

> 5052241009 Violita Karina Putri
> 
> 5052241027 Azizah Adilah
> 
> 5052241032 Aqila Ikhza Kusumawardani
> 
> 5052241035 Najwa Aulia

# 🏨 FINAL PROJECT TSDW: Analisis Permintaan Pemesanan Hotel

Proyek ini bertujuan untuk mendemonstrasikan proses **Data Wrangling** (pembersihan, transformasi, dan rekayasa fitur) pada dataset permintaan pemesanan hotel. Dilanjutkan dengan analisis eksploratif (EDA) untuk mendapatkan *insight* mengenai tingkat pembatalan dan perbedaan profil pemesanan antara dua tipe hotel: Resort Hotel dan City Hotel.

**Dataset:** Hotel Booking Demand Dataset (hotels.csv)

## 📌 Tujuan Utama Analisis

1.  **Mengatasi Kualitas Data:** Mengidentifikasi dan mengatasi masalah kualitas data (nilai hilang, duplikasi, format yang tidak sesuai).
2.  **Menganalisis Pembatalan:** Variabel manakah (misalnya `lead_time`, `deposit_type`, atau `booking_changes`) yang paling berkorelasi dengan status pembatalan (`is_canceled`)?
3.  **Membandingkan Hotel:** Bagaimana rata-rata Harga Harian (`adr`) bervariasi antara City Hotel dan Resort Hotel berdasarkan musim kedatangan?
4.  **Menangani Missing Values:** Bagaimana *missing values* di kolom `company` dan `agent` dapat diolah sedemikian rupa sehingga tetap memberikan *insight* dalam analisis akhir?

## 📁 Struktur Repositori

Repositori ini mengikuti struktur standar proyek Data Science, memastikan pemisahan data mentah, data bersih, dan *notebook* analisis:

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


