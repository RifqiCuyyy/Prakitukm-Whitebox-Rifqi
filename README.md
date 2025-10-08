Tentu, berikut adalah template penjelasan README yang baik dan profesional untuk repository GitHub Anda, yang menjelaskan konteks dan tujuan dari proyek praktikum ini.

Anda bisa menyalin semua teks di bawah ini dan memasukkannya ke dalam file `README.md` di repository Anda.

-----

# **Praktikum White Box Testing - Sistem Inventaris**

Repository ini berisi proyek untuk praktikum mata kuliah **Pengujian Perangkat Lunak**. Studi kasus yang digunakan adalah aplikasi konsol sederhana untuk manajemen inventaris.

Tujuan utama dari praktikum ini adalah untuk menerapkan teknik *white box testing* secara sistematis guna mencapai *test coverage* kode hingga 100% dengan menggunakan *tools* yang relevan seperti **JaCoCo**.

## **Deskripsi Proyek**

Aplikasi ini merupakan simulasi sistem manajemen inventaris sederhana yang memiliki fungsionalitas dasar seperti manajemen produk, kategori, dan stok. Proyek ini dibangun dengan Java dan dikelola menggunakan Apache Maven.

Fokus utama proyek bukanlah pada kompleksitas fitur aplikasi, melainkan pada **kualitas pengujian** terhadap kode yang ada.

## **Teknologi yang Digunakan**

  * **Java (JDK 21+)**: Bahasa pemrograman utama.
  * **Apache Maven**: Manajemen dependensi dan *build automation*.
  * **JUnit 5**: *Framework* untuk menjalankan *unit testing*.
  * **Mockito**: *Framework* untuk membuat *mock object* saat menguji kelas *service*.
  * **JaCoCo**: *Library* untuk mengukur dan membuat laporan *code coverage* dari hasil pengujian.

## **Fitur Aplikasi**

Aplikasi ini mencakup beberapa fungsionalitas inti, antara lain:

  * Manajemen Produk (tambah, hapus, cari).
  * Manajemen Kategori Produk.
  * Validasi data untuk stok dan harga.
  * Kalkulator Diskon berdasarkan kuantitas dan tipe pelanggan.
  * Perhitungan total nilai dan jumlah stok inventaris.

## **Cara Menjalankan dan Melakukan Pengujian**

Pastikan Anda memiliki **JDK (versi 21 atau lebih baru)** dan **Apache Maven** terinstal di sistem Anda.

1.  **Clone Repository**

    ```bash
    git clone [URL_REPOSITORY_ANDA]
    cd Praktikum-Whitebox-Rifqi
    ```

2.  **Menjalankan Semua Unit Test**
    Untuk menjalankan semua test case yang ada di dalam proyek, gunakan perintah:

    ```bash
    mvn test
    ```

3.  **Menghasilkan Laporan Code Coverage**
    Untuk menghasilkan laporan JaCoCo, jalankan perintah berikut setelah menjalankan `mvn test`:

    ```bash
    mvn jacoco:report
    ```

4.  **Melihat Laporan**
    Laporan *coverage* akan tersedia dalam format HTML. Buka file berikut di browser Anda:
    `target/site/jacoco/index.html`

## **Fokus Praktikum**

Praktikum ini berfokus pada proses iteratif untuk meningkatkan kualitas pengujian melalui langkah-langkah berikut:

1.  **Analisis Laporan Awal**: Menganalisis laporan *coverage* yang dihasilkan dari *test case* awal.
2.  **Identifikasi Celah**: Mengidentifikasi baris dan cabang logika (`if-else`, `switch`) yang belum teruji (ditandai merah atau kuning oleh JaCoCo).
3.  **Penambahan Test Case**: Menulis *unit test* baru secara spesifik untuk menutupi celah yang ditemukan, dengan menggunakan teknik seperti *Path Coverage* dan *Boundary Value Analysis*.
4.  **Verifikasi**: Menjalankan ulang pengujian dan menghasilkan laporan baru untuk memverifikasi bahwa *coverage* telah meningkat hingga mencapai target 100%.
