# 🍿 My Watchlist App

**My Watchlist App** adalah aplikasi berbasis web sederhana yang dirancang untuk membantu pengguna mengelola daftar tontonan film pribadi.
Aplikasi ini memungkinkan pengguna untuk mencatat film yang ingin ditonton.

## 🚀 Fitur Utama
* **Manajemen Data (CRUD):** Tambah, lihat, edit, dan hapus daftar film dengan mudah.
* **Upload Poster:** Fitur unggah gambar poster film secara lokal ke server.
* **Status Tontonan:** Fitur interaktif untuk menandai film yang sudah selesai ditonton dengan efek visual *opacity*.
* **Desain Responsif:** Antarmuka modern ala *streaming platform* menggunakan **Bootstrap 5.3**.
* **Notifikasi Modern:** Integrasi **SweetAlert2** untuk dialog konfirmasi penghapusan data yang lebih user-friendly.

---

## 🛠️ Teknologi yang Digunakan
* **Bahasa Pemrograman:** PHP Native & JavaScript.
* **Database:** MySQL.
* **Framework CSS:** Bootstrap 5.3.
* **Library:** FontAwesome (Ikon) & SweetAlert2 (Pop-up).

---

## 📂 Struktur Proyek
```text
movie-watchlist/
├── db.php               # Konfigurasi koneksi database MySQL
├── index.php            # Halaman utama (Daftar Film & Skala Rating)
├── tambah.php           # Form input data film baru
├── edit.php             # Form pembaruan data film
├── hapus.php            # Logika penghapusan data dari database
├── update_status.php    # Logika perubahan status (Selesai/Belum)
├── uploads/             # Folder penyimpanan file fisik poster film
└── database/
    └── movies.sql       # File export skema database

Penjelasan Teknis & Alur Program:
    1. Bagian ini menjelaskan bagaimana logika pemrograman diimplementasikan dalam aplikasi:
    2. Koneksi Database (db.php): Menggunakan ekstensi mysqli untuk menghubungkan skrip PHP dengan server MySQL.
    3. Manajemen Data Dinamis: Data film diambil dari database menggunakan query SQL dan ditampilkan secara otomatis melalui perulangan while di halaman utama.
    4. Logika Interaktif: Perubahan status film menjadi "Selesai" akan memicu perubahan class CSS secara kondisional menggunakan PHP, memberikan efek visual transparan pada kartu film.
    5. Keamanan Sederhana: Proses penghapusan data divalidasi terlebih dahulu melalui fungsi JavaScript agar tidak terjadi kesalahan hapus yang tidak disengaja.

Cara Menjalankan Proyek
Persiapan Database:
    1. Buka XAMPP Control Panel dan aktifkan modul Apache dan MySQL.
    2. Akses localhost/phpmyadmin di browser.
    3. Buat database baru dengan nama movie_watchlist.
    4. Pilih menu Import dan unggah file movies.sql yang ada di folder database/.

Konfigurasi Proyek:
    1. Pastikan folder proyek berada di dalam direktori C:/xampp/htdocs/.
    2. Buka file db.php dan pastikan konfigurasi username (default: root) dan password (default: kosong) sudah sesuai dengan pengaturan XAMPP.

Menjalankan Aplikasi:
Buka browser dan ketik alamat http://localhost/movie_watchlist/index.php
