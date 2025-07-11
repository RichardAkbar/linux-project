Mengatur autentikasi SSH tanpa kata sandi dari pengguna thor pada jump host ke semua app server (stapp01, stapp02, stapp03) melalui pengguna sudo masing-masing (tony, steve, banner).
Memastikan konfigurasi aman dan mendukung skrip otomatisasi yang dijalankan oleh thor.

Langkah 1: Hasilkan Pasangan Kunci SSH untuk thor

![alt text](image-18.png)

Langkah 2: Salin Kunci Publik ke Setiap App Server

![alt text](image-19.png)

Langkah 3: Uji Akses SSH Tanpa Kata Sandi

![alt text](image-20.png)

Mengatur autentikasi SSH tanpa kata sandi dari thor pada jump host ke tony@stapp01.