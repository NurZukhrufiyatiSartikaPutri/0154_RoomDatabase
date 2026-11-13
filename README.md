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

## Struktur Project

```text
com.example.roomdb/
│
├── repository/
│   ├── ContainerApp.kt
│   └── RepositoriSiswa.kt
│
├── room/
│   ├── DatabaseSiswa
│   ├── Siswa
│   └── SiswaDao
│
├── ui.theme/
│
├── uicontroller/
│   ├── DestinasiEntry
│   ├── DestinasiHome
│   ├── DestinasiNavigasi
│   └── PetaNavigasi.kt
│
├── view/
│   ├── HalamanEntry.kt
│   └── HalamanHome.kt
│
├── viewmodel/
│   ├── EntryViewModel.kt
│   ├── HomeViewModel
│   └── PenyediaViewModel.kt
│
├── AplikasiSiswa
└── MainActivity
```

### Penjelasan Struktur Project

| Folder/File | Fungsi |
|---|---|
| `repository` | Mengatur akses dan pengelolaan data melalui repository. |
| `room` | Menyimpan komponen database, Entity, dan DAO. |
| `ui.theme` | Mengatur tema, warna, dan tampilan aplikasi. |
| `uicontroller` | Mengatur tujuan dan navigasi antarhalaman. |
| `view` | Menampilkan antarmuka aplikasi. |
| `viewmodel` | Mengelola state dan logika aplikasi. |
| `AplikasiSiswa` | Menginisialisasi kebutuhan aplikasi. |
| `MainActivity` | Activity utama sebagai titik awal aplikasi. |

### Dokumentasi Struktur Project

<img width="263" height="515" alt="image" src="https://github.com/user-attachments/assets/ddbecb26-be8d-4a32-8300-bc10d5ad4870" />


<!-- Tempat screenshot struktur project -->

![Struktur Project](screenshots/05-struktur-project.png)

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

## Kesimpulan

Berdasarkan hasil pengujian, aplikasi Data Siswa berhasil menjalankan proses penambahan dan penampilan data siswa. Validasi formulir juga berfungsi untuk memastikan seluruh kolom wajib diisi sebelum data disimpan. Penggunaan Room Database membantu menyimpan data secara lokal, sedangkan arsitektur MVVM membantu memisahkan tampilan, pengelolaan state, dan pengelolaan data aplikasi.
