Menginstal firewalld pada semua app server (stapp01, stapp02, stapp03).
Mengizinkan semua koneksi masuk pada port 80/tcp (Nginx) di zona public.
Memblokir semua koneksi masuk pada port 8080/tcp (Apache) di zona public.
Memastikan semua aturan firewall bersifat permanen (bertahan setelah reboot).
Memastikan layanan Nginx dan Apache berjalan pada setiap server.

Langkah1: Aktifkan dan Jalankan Layanan firewalld

![alt text](image-23.png)

Langkah 2: Atur Zona Default ke Public

![alt text](image-24.png)

Langkah 3:Tambahkan Aturan untuk Port 80/tcp (Nginx)

![alt text](image-25.png)

Langkah 4: Blokir Port 8080/tcp (Apache)

![alt text](image-26.png)

Langkah 5: Muat Ulang Konfigurasi Firewall

![alt text](image-27.png)

Langkah 6: Verifikasi Aturan Firewall

![alt text](image-28.png)

Langkah 7: Pastikan Layanan Nginx dan Apache Berjalan

![alt text](image-29.png)

Langkah 8: Verifikasi Konektivitas Port

![alt text](image-30.png)

Mengizinkan hanya port 80/tcp dan memblokir 8080/tcp memastikan Nginx (reverse proxy) dapat diakses publik, sementara Apache (backend) hanya diakses melalui proxy, meningkatkan keamanan.