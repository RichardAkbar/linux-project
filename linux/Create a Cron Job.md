Menginstal paket cronie pada semua app server (stapp01, stapp02, stapp03).
Memastikan layanan crond berjalan dan aktif secara otomatis setelah reboot.
Menambahkan cron job */5 * * * * echo hello > /tmp/cron_text untuk pengguna root pada setiap server.

Langkah 1: Akses Setiap App Server melalui SSH

![alt text](image-13.png)

Langkah 2:Instal Paket cronie

![alt text](image-14.png)

Langkah 3: Aktifkan dan Jalankan Layanan crond

![alt text](image-15.png)

Langkah 4: Tambahkan Cron Job untuk Root
jalankan sudo crontab -e

![alt text](image-16.png)

![alt text](image-17.png)

Verifikasi Hasil


![alt text](image-12.png)