Menginstal HAProxy pada stlb01 menggunakan yum.
Mengkonfigurasi HAProxy untuk menyeimbangkan beban ke semua app server (stapp01, stapp02, stapp03) pada port 3000/tcp.
Memastikan HAProxy mendengarkan pada port 80/tcp untuk akses web.
Mempertahankan entri stats socket /var/lib/haproxy/stats di konfigurasi.
Memastikan layanan HAProxy berjalan dan website dapat diakses melalui stlb01

Langkah 1: Instal HAProxy

![alt text](image-31.png)

Langkah 2: Buat Cadangan File Konfigurasi HAProxy

![alt text](image-32.png)

Langkah 3: Konfigurasi HAProxy
sudo vi /etc/haproxy/haproxy.cfg

![alt text](image-33.png)

Langkah 4: Verifikasi Konfigurasi HAProxy
configuration file is valid

![alt text](image-34.png)

Langkah 5: Aktifkan dan Jalankan Layanan HAProxy

![alt text](image-35.png)

Langkah 6: Konfigurasi Firewall untuk Port 80/tcp

![alt text](image-36.png)

Langkah 7: Verifikasi Apache pada App Server
jalankan pada setiap app server:
Untuk stapp01

![alt text](image-37.png)


Verifikasi port 3000

![alt text](image-38.png)

Langkah 8: Uji Akses Website

![alt text](image-39.png)


website statis dapat diakses melalui HAProxy pada stlb01 port 80.


HAProxy sebagai reverse proxy pada port 80 memungkinkan akses publik ke website statis, sementara port 3000 pada app server dapat dibatasi oleh firewall untuk meningkatkan keamanan.