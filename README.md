# Aplikasi Data Siswa

## Deskripsi Project

Aplikasi **Data Siswa** merupakan aplikasi berbasis Android yang dikembangkan menggunakan Kotlin dan Jetpack Compose. Aplikasi ini bertujuan untuk mengelola data siswa melalui fitur penambahan, penyimpanan, dan penampilan data siswa.

Project ini menerapkan arsitektur **MVVM (Model-View-ViewModel)**, menggunakan **Room Database** sebagai penyimpanan data lokal, serta Navigation untuk mengatur perpindahan antarhalaman aplikasi.

## Teknologi yang Digunakan

- Kotlin
- Jetpack Compose
- Room Database
- MVVM Architecture
- Navigation Compose
- Android Studio

## Dokumentasi Hasil Aplikasi

### 1. Tampilan Awal (Data Siswa)


<img width="394" height="846" alt="image" src="https://github.com/user-attachments/assets/1047bb43-7675-4e43-8737-60f725a6c395" />


Menampilkan halaman utama aplikasi. Ketika belum terdapat data siswa, aplikasi menampilkan pesan bahwa data masih kosong serta tombol (+) untuk menambahkan data siswa.

### 2. Form Tambah Siswa


<img width="391" height="847" alt="image" src="https://github.com/user-attachments/assets/b75af84d-fc59-43af-9f7b-f7d880cfc45c" />


Menampilkan formulir input data siswa yang terdiri dari tiga kolom, yaitu Nama Siswa, Alamat Siswa, dan Telpon Siswa. Tombol Submit belum aktif sebelum seluruh kolom wajib diisi.

### 3. Pengisian Form Data Siswa


<img width="403" height="853" alt="image" src="https://github.com/user-attachments/assets/c1bb93c8-8f89-45da-a4b7-16774a612b30" />



Pengguna mengisi formulir dengan nama, alamat, dan nomor telepon siswa. Setelah seluruh data terisi, tombol Submit menjadi aktif dan dapat digunakan untuk menyimpan data.

### 4. Hasil Data Siswa Berhasil Ditambahkan


<img width="385" height="837" alt="image" src="https://github.com/user-attachments/assets/14d8f104-c1b6-47c6-9095-cb3a54e05eb8" />


Setelah tombol Submit ditekan, aplikasi kembali ke halaman utama dan menampilkan data siswa yang berhasil disimpan dalam bentuk kartu informasi berisi nama, alamat, dan nomor telepon.

### 5. Edit Data Siswa

<img width="397" height="846" alt="image" src="https://github.com/user-attachments/assets/49a00d51-7f72-4868-9122-8c78aedf3b3f" />


Menampilkan halaman Edit Siswa yang digunakan untuk memperbarui data siswa yang sudah tersimpan. Formulir menampilkan data sebelumnya, meliputi Nama Siswa, Alamat Siswa, dan Telpon Siswa. Pengguna dapat mengubah informasi yang diperlukan, kemudian menekan tombol Submit untuk menyimpan perubahan data.

### 6. Hapus Data Siswa

<img width="394" height="850" alt="image" src="https://github.com/user-attachments/assets/3ff6c2c0-6ada-4cdd-97f3-861234f2de33" />


Menampilkan halaman Detail Siswa dengan dialog konfirmasi sebelum melakukan penghapusan data. Aplikasi menampilkan pesan "Apakah anda yakin menghapus ini?" dengan dua pilihan, yaitu Tidak untuk membatalkan proses penghapusan dan Ya untuk melanjutkan penghapusan data siswa. Fitur ini membantu mencegah penghapusan data secara tidak sengaja.

## Kesimpulan

Berdasarkan hasil pengujian, aplikasi Data Siswa berhasil menjalankan proses penambahan, penampilan, pengubahan, dan penghapusan data siswa. Validasi formulir juga berfungsi untuk memastikan seluruh kolom wajib diisi sebelum data disimpan. Penggunaan Room Database membantu menyimpan data secara lokal, sedangkan arsitektur MVVM membantu memisahkan tampilan, pengelolaan state, dan pengelolaan data aplikasi.
