# Aplikasi Perpustakaan
### _Aplikasi Perpustakaan Ini Merupakan Aplikasi Peminjaman Buku Online_

[![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)](https://nextjs.org/) [![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)](https://react.dev/) [![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/) [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/) [![Zustand](https://img.shields.io/badge/Zustand-5-orange)](https://zustand-demo.pmnd.rs/) [![Vercel](https://img.shields.io/badge/Deployed_on-Vercel-black?logo=vercel)](https://dillinger.io) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


## Features Aplikasi Perpustakaan

- **Login, register, logout** Akun user bisa dibuat dan dipakai untuk masuk ke sistem.
- **Role user dan admin** Website membedakan hak akses antara user dan admin.
- **Daftar Buku Di Halaman Utama** semua pengunjung bisa melihat daftar buku yang tersedia
- **Pencarian Buku** — buku bisa dicari judul, penulis, kategori, dan detail.
- **Detail Buku** setiap buku punya halaman detail untuk melihat informasi lengkap
- **Peminjaman buku oleh user** User bisa meminjam buku jika stok tersedia.
- **Proteksi pinjam buku yang sama** — User tidak bisa meminjam buku yang sama lebih dari satu kali selama statusnya masih dipinjam.
- **Riwayat peminjaman user** — User bisa melihat daftar buku yang pernah atau sedang dipinjam.
- **Manajemen buku oleh admin** — 
Admin Bisa 
-- Tambah Buku
-- Liat Daftar Buku
-- Lihat Detail Buku
-- Edit Buku
-- Hapus Buku
- **Manajemen peminjaman oleh admin** — Admin bisa melihat semua data peminjaman dan memproses pengembalian buku.
- **Pengembalian buku + denda** — Saat admin mengembalikan buku, sistem menghitung denda keterlambatan otomatis.
- **Stok buku otomatis** — Saat buku dipinjam stok berkurang, saat dikembalikan stok bertambah.
- **Profil pengguna** — User bisa ubah profil, password, dan hapus akun.
- **Tampilan branding perpustakaan** — Login dan register sudah memakai branding Perpustakaan dan logo.

## Tech

Aplikasi Perpustakaan Dibangun Dengan Menggunakan:

Website perpustakaan ini dibangun menggunakan Laravel sebagai framework utama dalam pengembangan aplikasi. Laravel digunakan karena memiliki struktur yang rapi, mudah dikembangkan, dan menyediakan banyak fitur bawaan yang membantu dalam pembuatan website, seperti routing, autentikasi, pengelolaan database, dan sistem template. Bahasa pemrograman yang digunakan dalam project ini adalah PHP, karena Laravel berjalan di atas PHP dan sangat cocok digunakan untuk membangun aplikasi web dinamis seperti sistem perpustakaan.

Untuk pengelolaan data, website ini menggunakan MySQL sebagai database. Database ini berfungsi untuk menyimpan seluruh informasi penting di dalam sistem, seperti data pengguna, data buku, data peminjaman, data pengembalian, serta denda keterlambatan. Selama proses pengembangan, website ini dijalankan menggunakan XAMPP, yang berfungsi sebagai server lokal. XAMPP membantu menjalankan Apache sebagai web server dan MySQL sebagai database server, sehingga website dapat diuji dan dijalankan di komputer lokal sebelum dipublikasikan.

Pada bagian tampilan, website ini dibuat menggunakan Blade sebagai template engine bawaan Laravel. Blade memudahkan pembuatan halaman web agar lebih terstruktur, rapi, dan mudah dikelola. Selain itu, tampilan antarmuka website juga menggunakan HTML, CSS, dan JavaScript agar halaman dapat tampil lebih menarik, responsif, dan interaktif. Dengan kombinasi teknologi tersebut, website perpustakaan ini dapat digunakan untuk menampilkan daftar buku, melakukan pencarian, meminjam buku, mengelola data buku, serta memproses pengembalian dengan lebih mudah dan efisien.

Secara keseluruhan, website ini dibangun dengan menggabungkan Laravel, PHP, MySQL, XAMPP, Blade, HTML, CSS, dan JavaScript untuk menghasilkan sistem perpustakaan berbasis web yang modern, terstruktur, dan mudah digunakan oleh admin maupun user.

## Requirement
- Versi yang dipakai di project ini adalah:

- Laravel 10.50.0
- PHP 8.2.12 pada lingkungan yang sedang dipakai
- MySQL dipakai sebagai database
- Laravel Breeze ^1.29
- Vite ^5.0.0
- Tailwind CSS ^3.1.0

## structure
📦routes
 ┣ 📜api.php
 ┣ 📜auth.php
 ┣ 📜channels.php
 ┣ 📜console.php
 ┗ 📜web.php
 📦Controllers
 ┣ 📂Auth
 ┃ ┣ 📜AuthenticatedSessionController.php
 ┃ ┣ 📜ConfirmablePasswordController.php
 ┃ ┣ 📜EmailVerificationNotificationController.php
 ┃ ┣ 📜EmailVerificationPromptController.php
 ┃ ┣ 📜NewPasswordController.php
 ┃ ┣ 📜PasswordController.php
 ┃ ┣ 📜PasswordResetLinkController.php
 ┃ ┣ 📜RegisteredUserController.php
 ┃ ┗ 📜VerifyEmailController.php
 ┣ 📜bukucontroller.php
 ┣ 📜Controller.php
 ┣ 📜peminjamancontroller.php
 ┗ 📜ProfileController.php
 📦Models
 ┣ 📜Buku.php
 ┣ 📜peminjaman.php
 ┗ 📜User.php
 📦views
 ┣ 📂Admin
 ┃ ┣ 📂buku
 ┃ ┃ ┣ 📜create.blade.php
 ┃ ┃ ┣ 📜edit.blade.php
 ┃ ┃ ┣ 📜index.blade.php
 ┃ ┃ ┗ 📜show.blade.php
 ┃ ┗ 📂peminjaman
 ┃ ┃ ┗ 📜index.blade.php
 ┣ 📂auth
 ┃ ┣ 📜confirm-password.blade.php
 ┃ ┣ 📜forgot-password.blade.php
 ┃ ┣ 📜login.blade.php
 ┃ ┣ 📜register.blade.php
 ┃ ┣ 📜reset-password.blade.php
 ┃ ┗ 📜verify-email.blade.php
 ┣ 📂buku
 ┃ ┗ 📜show.blade.php
 ┣ 📂components
 ┃ ┣ 📜application-logo.blade.php
 ┃ ┣ 📜auth-session-status.blade.php
 ┃ ┣ 📜danger-button.blade.php
 ┃ ┣ 📜dropdown-link.blade.php
 ┃ ┣ 📜dropdown.blade.php
 ┃ ┣ 📜input-error.blade.php
 ┃ ┣ 📜input-label.blade.php
 ┃ ┣ 📜modal.blade.php
 ┃ ┣ 📜nav-link.blade.php
 ┃ ┣ 📜primary-button.blade.php
 ┃ ┣ 📜responsive-nav-link.blade.php
 ┃ ┣ 📜secondary-button.blade.php
 ┃ ┗ 📜text-input.blade.php
 ┣ 📂layouts
 ┃ ┣ 📜app.blade.php
 ┃ ┣ 📜guest.blade.php
 ┃ ┗ 📜navigation.blade.php
 ┣ 📂profile
 ┃ ┣ 📂partials
 ┃ ┃ ┣ 📜delete-user-form.blade.php
 ┃ ┃ ┣ 📜update-password-form.blade.php
 ┃ ┃ ┗ 📜update-profile-information-form.blade.php
 ┃ ┗ 📜edit.blade.php
 ┣ 📂user
 ┃ ┗ 📜riwayat.blade.php
 ┣ 📜dashboard.blade.php
 ┗ 📜welcome.blade.php
 📦migrations
 ┣ 📜2014_10_12_000000_create_users_table.php
 ┣ 📜2014_10_12_100000_create_password_reset_tokens_table.php
 ┣ 📜2019_08_19_000000_create_failed_jobs_table.php
 ┣ 📜2019_12_14_000001_create_personal_access_tokens_table.php
 ┣ 📜2026_04_01_000001_add_role_to_users_table.php
 ┣ 📜2026_04_01_000002_create_buku_table.php
 ┣ 📜2026_04_01_000003_create_peminjaman_table.php
 ┣ 📜2026_04_05_000004_add_detail_to_buku_table.php
 ┗ 📜2026_04_05_000005_optimize_library_tables.php
 📦public
 ┣ 📂build
 ┃ ┣ 📂assets
 ┃ ┃ ┣ 📜app-BR77_l1h.js
 ┃ ┃ ┗ 📜app-CKcAoPeL.css
 ┃ ┗ 📜manifest.json
 ┣ 📂storage
 ┃ ┣ 📂buku
 ┃ ┃ ┣ 📜5V6QyyjchHIQ4AufVcUnlyseO18iZDuFyd1qgmc3.jpg
 ┃ ┃ ┣ 📜dBSxr3rIlKSdfKzWwU3VYBmNZuKILtLliEhmVqyj.jpg
 ┃ ┃ ┣ 📜NtFow62DeETUr2wCjZaIQOJm1M23ht0OUFW0KvLa.jpg
 ┃ ┃ ┗ 📜rbjIegVbWPbEUPnTTmPceIlhHmLlGpsiXjb6GNWF.jpg
 ┃ ┗ 📜.gitignore
 ┣ 📜.htaccess
 ┣ 📜favicon.ico
 ┣ 📜index.php
 ┗ 📜robots.txt
## Instalation
- 1 . Pindahkan project ke folder htdocs
Simpan folder project website perpustakaan ke dalam folder htdocs yang ada di XAMPP.
Contoh:
C:\xampp\htdocs\perpustakaan

- 2 . Jalankan XAMPP
Buka aplikasi XAMPP, lalu aktifkan:
Apache
MySQL

- 3 . Buka project di terminal
Masuk ke folder project melalui terminal atau CMD:
cd C:\xampp\htdocs\perpustakaan
- 4 . Install dependency Laravel
Jalankan perintah berikut untuk menginstall semua dependency:
composer install

- 5 . Buat file .env
Jika file .env belum ada, salin dari .env.example:
copy .env.example .env
- 6 . Generate application key
Jalankan perintah berikut:
php artisan key:generate
- 7 . Buat database
Buka phpMyAdmin dari XAMPP, lalu buat database baru dengan nama:
perpustakaan
- 8 . Atur konfigurasi database
Buka file .env, lalu sesuaikan bagian database seperti berikut:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=perpustakaan
DB_USERNAME=root
DB_PASSWORD=
- 9 . Jalankan migration
Setelah database dibuat, jalankan perintah:
php artisan migrate
- 10 . Jalankan server Laravel
Jalankan project dengan perintah:
php artisan serve
- 11 . Buka website di browser
Setelah server berjalan, buka:
http://127.0.0.1:8000



**Free Software, Hell Yeah!**
