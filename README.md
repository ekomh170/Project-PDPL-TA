# SIPERPUS (Sistem Informasi Perpustakaan)

SIPERPUS adalah aplikasi sistem informasi perpustakaan berbasis web yang memungkinkan pengelolaan buku, anggota, peminjaman buku, dan laporan dengan antarmuka yang sederhana dan user-friendly.

---

## Tugas Akhir Mata Kuliah PDPL

Aplikasi ini dikembangkan sebagai bagian dari tugas akhir mata kuliah **Pengembangan dan Desain Perangkat Lunak (PDPL)**. Proyek ini bertujuan untuk memahami penerapan **design pattern** dalam pengembangan perangkat lunak.

### Anggota Kelompok

| **Nama**                | **Peran**         |
|-------------------------|-------------------|
| EKO MUCHAMAD HARYONO    | Ketua  & Developer           |
| FAJAR NURZAMAN          | Developer         |
| DEDEN RAFI AKBAR        | Copy Writer       |
| RAEHAN NURMISHUARI      | Developer         |
| ILYAS ABDUL AZIZ        | Developer         |
| MUHAMMAD AFIF NAUFAL    | Copy Writer       |

---

## Fitur

### **Admin**
- **Dashboard**: Statistik buku & anggota.
- **Manajemen Buku**: Tambah, ubah, hapus, dan cari buku.
- **Manajemen Anggota**: Tambah, ubah, hapus, dan kelola status anggota.
- **Peminjaman Buku**: Kelola proses peminjaman dan pengembalian buku.
- **Laporan**: Laporan peminjaman buku.

### **Member**
- **Dashboard**: Informasi statistik buku dan peminjaman aktif.
- **Cari Buku**: Cari buku berdasarkan judul atau kategori.
- **Riwayat Peminjaman**: Lihat daftar peminjaman buku.

---

## Instalasi

1. **Clone Repository**

2. **Instal Dependencies**
   Jalankan perintah berikut untuk menginstal semua dependencies:
   ```bash
   composer install
   npm install
   npm run dev
   ```

3. **Konfigurasi Database**
   - Gunakan SQLite sebagai database:
     ```bash
     touch database/database.sqlite
     ```
   - Salin file `.env.example` menjadi `.env`:
     ```bash
     cp .env.example .env
     ```
   - Konfigurasikan database pada file `.env`:
     ```env
     DB_CONNECTION=sqlite
     DB_DATABASE=/path/to/your/project/database/database.sqlite
     ```

4. **Migrate dan Seed Database**
   ```bash
   php artisan migrate:fresh
   php artisan db:seed
   ```

5. **Jalankan Aplikasi**
   Jalankan server aplikasi:
   ```bash
   php artisan serve
   ```
   Akses aplikasi di: [http://localhost:8000](http://localhost:8000)

---

## Pengguna Default

| **Role**  | **Email**            | **Password** |
|-----------|----------------------|--------------|
| Admin     | ekomh13@example.com    | admin2829     |
| Member    | member123@example.com   | member123     |

---

## Teknologi yang Digunakan

- **Framework**: Laravel 11
- **Database**: SQLite
- **Frontend**: AdminLTE, Bootstrap
- **Authentication**: Laravel Breeze
