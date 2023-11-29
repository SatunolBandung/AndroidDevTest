# Android Application Development Testing

## 1. Uji kemampuan teknis menggabungkan penggunaan canvas, SQLite, dan manipulasi elemen UI.

Catatan: Pastikan Anda memiliki pengetahuan dasar tentang pengembangan aplikasi Android dan telah menyiapkan proyek Android Studio.

1. Buat Database SQLite:
- Tentukan tabel untuk menyimpan data titik (x, y).
```
CREATE TABLE IF NOT EXISTS points (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    x REAL,
    y REAL
);
```
2. Inisialisasi Database
- Buat kelas DatabaseHelper untuk membantu dalam manajemen database.
- Isi database dengan random point seusai luas canvas 

3. Buat Model Point:
- Definisikan model untuk merepresentasikan titik pada canvas.

4. Manipulasi Canvas dan Tampilan:
- Buat kelas CanvasView yang merupakan subclass dari View untuk menggambar titik dan memanipulasi persegi di atas canvas. 

5. Aktivitas Utama:
- sediakan input posisi untuk membuat persegi pada canvas dengan ukuran sisi yang anda tentukan.
- seleksi titik pada database sesuai dengan range luas persegi.
- tampilkan titik yang berpotongan.

![Contoh Alt Text](img.png)

## 2. Pengembangan Aplikasi Google Calendar Sync
Catatan: Pada tugas ini, peserta diharapkan untuk membuat aplikasi Android sederhana yang memungkinkan pengguna untuk menambahkan event baru ke Google Calendar dan membaca daftar event yang sudah ada. Peserta dapat menggunakan API resmi Google Calendar untuk mencapai ini.

1. Menambahkan Event Baru:
- Buat fitur untuk menambahkan event baru ke Google Calendar. 
- Event harus memiliki setidaknya informasi dasar seperti judul, deskripsi, tanggal, dan waktu. 
- Pastikan bahwa pengguna dapat memasukkan informasi ini melalui User Interface.

2. Membaca Daftar Event:
- Aplikasi harus dapat menampilkan daftar event yang sudah ada pada Google Calendar pengguna. 
- Peserta dapat menggunakan komponen UI seperti RecyclerView untuk menampilkan daftar event dengan baik.

3. Otentikasi Pengguna:
- Pastikan bahwa aplikasi meminta izin otentikasi dari pengguna untuk mengakses Google Calendar. 
- Peserta harus mengimplementasikan autentikasi OAuth 2.0 menggunakan Google Sign-In atau mekanisme otentikasi lainnya yang sesuai.

3. Penanganan Kesalahan:
- Peserta diharapkan untuk menangani kemungkinan kesalahan, seperti ketidakmampuan untuk terhubung ke Google Calendar atau kesalahan saat menambahkan event. 
- Berikan umpan balik yang sesuai kepada pengguna.

4. Optimasi Kinerja:
- Pastikan bahwa aplikasi dioptimalkan untuk kinerja dengan menghindari pemanggilan API yang berulang-ulang dan mempertimbangkan implementasi caching untuk mengurangi waktu respons.