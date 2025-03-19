## Perpuspedia – Sistem Perpustakaan Berbasis QR Code 📚

🚀 Perpuspedia adalah solusi modern untuk manajemen perpustakaan berbasis QR Code, memudahkan proses peminjaman, pengembalian, hingga sistem denda dengan fitur canggih dan tampilan yang responsif.

> ## Fitur Utama ✨

- QR Code untuk Anggota & Peminjaman – Tak perlu kartu fisik lagi!
- Dashboard Admin – Kelola perpustakaan dengan tampilan yang intuitif.
- Sistem Denda Otomatis – Tidak perlu hitung manual!
- Magic Login Link – Akses lebih mudah tanpa perlu mengingat password.

> ## Teknologi yang Digunakan 🛠

- Framework: [CodeIgniter 4](https://codeigniter.com/) 🚀
- UI & Template: [Bootstrap 5](https://getbootstrap.com/),
  [Modernize Admin Template](https://adminmart.com/product/modernize-free-bootstrap-5-admin-template/) 🎨
- Grafik & Statistik: [Apex Charts](https://apexcharts.com/) 📊
- QR Code & Scanner: [Endroid QR Code Generator](https://github.com/endroid/qr-code), [Mebjas Html5-QRCode](https://github.com/mebjas/html5-qrcode) 📷

## Cara Penggunaan

### Persyaratan

- [Composer](https://getcomposer.org/).
- PHP 8.1+ dan MySQL atau [XAMPP](https://www.apachefriends.org/download.html) versi 8.1+ dengan mengaktifkan extension `-intl` dan `-gd`.
- (Opsional) Kamera/webcam untuk menjalankan qr scanner. Bisa juga menggunakan kamera HP dengan bantuan software DroidCam.

### Instalasi

- Unduh dan impor kode proyek ini ke dalam direktori proyek anda (htdocs).
- Penting ⚠️. Jika belum memiliki file `.env`, salin/rename file `.env.example` menjadi `.env`
- (Opsional) Konfigurasi file `.env` untuk mengatur parameter seperti koneksi database dan pengaturan lainnya sesuai dengan lingkungan pengembangan Anda.
- Penting ⚠️. Install dependencies yang diperlukan dengan cara menjalankan perintah berikut di terminal:

```shell
composer install
```

- Buat database `db_book_library` di phpMyAdmin / mysql
- Penting ⚠️. Jalankan migrasi database untuk membuat struktur tabel yang diperlukan. Ketikkan perintah berikut di terminal:

```shell
php spark migrate --all
```

- Penting ⚠️. Karena belum memiliki akun admin, untuk mengakses halaman admin, anda memerlukan user/akun dengan level `superadmin`. Jalankan perintah berikut untuk membuat akun `superadmin`:

```shell
php spark db:seed SuperAdminSeeder
```

> [!TIP]
>
> - (Opsional) Isi database dengan data dummy / seeder.

```shell
php spark db:seed Seeder # semua seeder
```

- Jalankan website

```shell
php spark serve
```

- Buka [http://localhost:8080](http://localhost:8080)
- Login dengan kredensial `superadmin` berikut:

```txt
username : superadmin
email    : superadmin@admin.com
password : superadmin
```

-- Terima kasih telah menggunakan Perpuspedia! Jika ada pertanyaan atau saran, jangan ragu untuk menghubungi kami. --
