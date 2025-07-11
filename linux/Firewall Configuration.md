Mengizinkan semua koneksi masuk pada port 6400/tcp di Nautilus Backup Server (stbkp01).
Memastikan zona firewall diatur ke public.
Memverifikasi bahwa konfigurasi firewall aktif (bertahan setelah reboot).

Langkah 1: Akses Nautilus Backup Server (stbkp01)

![alt text](image-6.png)

Langkah 2: Verifikasi Status firewalld

![alt text](image-7.png)

Langkah 3: Periksa Zona Default

![alt text](image-8.png)

Langkah 4: Tambahkan Aturan untuk Port 6400/tcp

![alt text](image-9.png)


Langkah 5: Muat Ulang Konfigurasi Firewall

![alt text](image-10.png)

Langkah 6: Verifikasi Aturan Firewall

![alt text](image-11.png)

menerapkan konfigurasi firewalld untuk mengizinkan port 6400/tcp, memastikan hanya port yang diperlukan yang terbuka untuk aplikasi web UI.