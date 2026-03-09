# Movie Watchlist
Program **Movie Watchlist** adalah sistem manajemen daftar film berbasis web yang dirancang menggunakan 
**PHP Native** dengan pendekatan **Object-Oriented Programming (OOP)**. 
Program ini memungkinkan pengguna untuk mencatat film yang ingin ditonton, 
serta mengelola status tontonan secara interaktif.

## 🚀 Fitur Utama

* **Manajemen CRUD Lengkap**: Menambah, membaca, memperbarui, dan menghapus data film.
* **Sistem Upload Gambar**: Mendukung pengunggahan poster film secara dinamis.
* **Fitur Toggle Status**: Mengubah status film (Selesai/Belum Ditonton) dengan satu klik.
* **Antarmuka Responsif**: Dibangun dengan Bootstrap 5 agar nyaman diakses dari perangkat apa pun.
* **Notifikasi Interaktif**: Menggunakan SweetAlert2 untuk konfirmasi penghapusan data.
* **Keamanan Dasar**: Validasi input untuk mencegah SQL Injection.

## 🛠️ Teknologi yang Digunakan
* **Bahasa Pemrograman**: PHP 8.x
* **Database**: MySQL
* **Frontend**: Bootstrap 5, FontAwesome 6
* **Library JS**: SweetAlert2, JQuery (opsional)
* **Konsep Pemrograman**: Object-Oriented Programming (OOP), Namespaces, Interfaces, Inheritance.

## 📂 Struktur Proyek
```text
movie-watchlist/
│   ├── media.php          # Base Class (Inheritance)
│   ├── movielogic.php     # Logic Class & Interface
├── uploads/               # Folder penyimpanan poster film
├── db.php                 # Koneksi Database
├── index.php              # Halaman Utama (Daftar Film)
├── detail.php             # Halaman Detail Film
├── tambah.php             # Proses Tambah Data
├── edit.php               # Proses Edit Data
├── hapus.php              # Proses Hapus Data & File
└── update_status.php      # Toggle Status Tontonan

```

## ⚙️ Persiapan & Instalasi
1. **Clone atau Unduh Proyek**:
Simpan folder proyek di direktori server lokal (misal: `htdocs` untuk XAMPP).
2. **Konfigurasi Database**:
* Buka **phpMyAdmin**.
* Buat database baru dengan nama `movie_watchlist`.
* Impor tabel `movies` atau buat tabel dengan struktur berikut:
```sql
CREATE TABLE movies (
    id_movie INT PRIMARY KEY AUTO_INCREMENT,
    judul_film VARCHAR(255),
    genre VARCHAR(100),
    rating DECIMAL(3,1),
    poster VARCHAR(255),
    deskripsi TEXT,
    status ENUM('Belum', 'Selesai') DEFAULT 'Belum'
);

```
3. **Sesuaikan Koneksi**:
Pastikan kredensial pada `db.php` sesuai dengan konfigurasi server lokal (host, user, pass, db_name).
4. **Jalankan Aplikasi**:
Akses melalui browser di alamat `http://localhost/movie_watchlist/index.php`.

## 📝 Konsep OOP yang Diterapkan
Program ini mendemonstrasikan pemahaman mendalam tentang OOP di PHP:
* **Encapsulation**: Penggunaan akses properti `protected`.
* **Inheritance**: `MovieLogic` mewarisi sifat dari class `Media`.
* **Interface**: Penggunaan `interface Watchable` untuk standarisasi metode.
* **Namespace**: Menggunakan `namespace App` untuk manajemen paket kode yang rapi.
