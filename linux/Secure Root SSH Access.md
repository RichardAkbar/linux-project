Menonaktifkan login SSH langsung untuk pengguna root pada semua app server (stapp01, stapp02, stapp03) di Stratos Datacenter.
Memastikan konfigurasi aman tanpa mengganggu akses pengguna non-root (seperti tony, steve, banner).
Langkah Pengerjaan:
Login ke akun stapp01

![alt text](image.png)

Langkah 2: Buat Cadangan File /etc/ssh/sshd_config

![alt text](image-1.png)


Langkah 3: Edit File /etc/ssh/sshd_config
Cari baris yang berisi PermitRootLogin

![alt text](image-2.png)


Langkah 4: Verifikasi Perubahan pada sshd_config

![alt text](image-3.png)


Langkah 5: Restart Layanan SSH

![alt text](image-4.png)

Langkah 6: Verifikasi bahwa Login Root Dinonaktifkan

![alt text](image-5.png)


Menguji bahwa login SSH sebagai root ditolak.
menonaktifkan login SSH root, mengurangi risiko serangan terhadap akun dengan hak istimewa penuh.