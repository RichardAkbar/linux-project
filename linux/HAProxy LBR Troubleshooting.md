Mendiagnosis dan memperbaiki masalah dengan layanan HAProxy pada stlb01.


Memastikan HAProxy berjalan dan menyeimbangkan beban ke app server (stapp01, stapp02, stapp03) pada port 3000/tcp.


Memverifikasi bahwa website statis dapat diakses melalui stlb01:80 (via "StaticApp" button).

Langkah 1: Periksa Status Layanan HAProxy

![alt text](image-40.png)

Mengidentifikasi apakah HAProxy berjalan atau tidak.

![alt text](image-41.png)

Langkah 2: Mulai atau Restart Layanan HAProxy

![alt text](image-42.png)

Langkah 3: Periksa Konfigurasi HAProxy

![alt text](image-43.png)

Jika ada error, edit file konfigurasi
sudo nano /etc/haproxy/haproxy.cfg

![alt text](image-44.png)

error bagian user harusnya haproxy bukan haprox

![alt text](image-45.png)

configuration file is valid