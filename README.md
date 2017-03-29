
# Kelompok 1
- Moh. Azis | G64140033
- Adhimas Luqman | G64140053
- Ayub Eko Prasetyo | G64140057
- Respati Widrantara Putra | G64140028



# Aplikasi Web "ICEHRM"

## Sekilas Tentang 

Icehrm adalah salah satu aplikasi Human Resources Information System(HRIS) berbasis opensource yang diperuntukan bagi perusahaan berskala kecil sampai menengah. Pada dasarnya Icehrm dapat menangani berbagai kebutuhan managemen sumberdaya manusia seperti time management, employee information dan sebagainya.

Human Resources Information System (HRIS) adalah program aplikasi komputer yang mengorganisir tatakelola dan tatalaksana manajemen SDM di perusahaan guna mendukung proses pengambilan keputusan atau biasa disebut dengan Decision Support System dengan menyediakan berbagai informasi yang diperlukan.

## Instalasi

##### Requirements
- PHP 5.3 or Higher
- apache2
- phpmysql
- libapache2
- MySQL v7.0.15
- phpmyadmin

##### Langkah instalasi Requirement awal dalam CLI.
```sh
$ sudo apt install apache2
$ sudo apt install mysql-server
$ sudo apt install php
$ sudo apt install libapache2-mod-php
$ sudo apt install php-mysql
$ sudo apt install php-gd php-mcrypt php-mbstring php-xml php-ssh2
$ sudo apt install phpmyadmin
$ sudo ln -s /usr/share/phpmyadmin /var/www/
$ sudo nano /etc/apache2/apache2.conf

# masukkan kedalam script apache2.conf (Include /etc/phpmyadmin/apache.conf)
$ sudo service apache2 restart
 ```

##### Instalasi Aplikasi Web Icehrm
- Langkah instalasi aplikasi dalam CLI.
```sh
# membuat direktori baru
    $ mkdir icehrm
# download sourcecode
    $ wget "https://github.com/gamonoid/icehrm/releases/download/v19.0.OS/icehrm_v19.0.OS.tar.gz" 
# extract ke direktori web
    $ sudo tar -xzf icehrm_v19.0.OS.tar.gz -C /var/www/html
# untuk mengganti mode dari sebuah file
    $ sudo touch /var/www/html/icehrm_v19.0.OS/app/config.php
    $ sudo chmod 777 /var/www/html/icehrm_v19.0.OS/app/config.php
    $ sudo chmod 777 /var/www/html/icehrm_v19.0.OS/app/data
# membuat database baru
    mysql -u root -p
    CREATE database icehrmdb;
    GRANT ALL on icehrmdb.* to 'root'@'localhost' identified by 'first';
 ```
## Instalasi di Web Browser
![N|Solid](https://pbs.twimg.com/media/C8F8gTSUwAES3E-.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8F8jRwVUAEB3JJ.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8F8li9VMAAWHAK.jpg:large)

```sh
# Rename or remove folder install
$ var/www/html/icehrm_v19.0.OS/app$rm -rf install

```


![N|Solid](https://pbs.twimg.com/media/C8GEzbtUwAAWhtD.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8GCzHmVYAEej7m.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8GC13rVYAEclFo.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8F_5_JV4AASPxq.jpg:large)


## Cara Pemakaian
![N|Solid](https://pbs.twimg.com/media/C8FtV-CVYAEXrqL.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FthNaVYAE7PmZ.jpg:large)

- Fungsi-fungsi utama

![N|Solid](https://pbs.twimg.com/media/C8Ftj1AVMAIs8t0.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FtwxzU8AA5tVv.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8Ft35PVwAALzPg.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8Ft8keV4AAZlw2.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FuBjTVYAENkli.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FuGErVsAA4Dzw.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FuKuKVQAQbzMO.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FuRW8VwAQD0tO.jpg:large)

![N|Solid](https://pbs.twimg.com/media/C8FuVioUwAA_j6N.jpg:large)





## Pembahasan

Dengan salah satu antarmuka modern diantara pesain HRIS opensoruce lainnya, Icehrm datang dengan penggunaan yang mudah. Icehrm menyediakan leave management, time and attendance tracking,employee information, serta upload document yang juga merupakan kemampuan untuk mendownload report dalam format .CSV. Dukungan support issue juga membantu icehrm menjadi salah satu opsi opensource HRIS yang kuat
- Pros:
 1. Pengamanan Informasi Karyawan : IceHrm employee management mengizinkan perusahaan untuk mensentralisasi informasi karyawan dan akses izin untuk memastikan bahwa semua karyawan informasi aman dan dapat diakses sesuai izin.
 2. Otomatisasi leave management : Icehrm mengizinkan untuk mengehentikan segala tipe pelanggaran. Juga bisa dapat membuat tipe leave sendiri, membuat pengecualian karyawan dan grup untuk menggunakan peraturan leave
 3. Track Every Bit of Time Spent : Karyawan dapat memperbaharui lembaran waktu milik mereka sendiri dan mengirim persetujuan ke supervisors.
 4. Easy Payroll Processing : Icehrm juga menyediakan proses rotasi pembayaran.
 5. Recruitment and Applicant Tracking : Icehrm juga dapat melakukan manajemen terhadap pencarian karyawan baru dan juga dapat mengatur proses wawancara secara berkala
 6. Staff Training : Mempermudah melakukan manajemen terhadap pelatihan karyawan yang ada pada perusahaan
    
- Cons:
    Karena ditargetkan hanya untuk pasar kecil hingga menengah, Icehrm tidak            memiliki fungsi yang mendalam untuk perusahaan yang berskala besar
  

##### Perbandingan dengan Aplikasi lain yang sejenis (Admidio)

Admidio adalah software management (opensource) yang fokus pada membership dan event management. Walaupun mendasar, fitur yang disediakan admidio dimulai dari pembuatan list membership dan integrasi managemen dengan posting onine dan iklan.

Pros/Cons :
(+) Admidio menyediakan fitur membership manajemen, admidio dapat membuat list terupdate, dapat diintegrasikan dengan Excel dan dapat di ekspor dalam format pdf dan memperbolehkan untuk posting online dan periklanan bagi setiap member.

(-) Ada beberapa fitur esensial yang tidak disediakan seperti proses pembayaran, otomatisasi pembaruan, serta accounting. 

##### Kesimpulan

Kesimpulannya adalah Admidio merupakan management sumberdaya manusia yang berfokuskan pada membership manajemen walaupun memang fitur yang disediakan masih belum lengkap. Sedangkan IceHrm adalah manajemen sumberdaya manusia yang berfokuskan pada sentralisasi dan mengatur kegiatan sumberdayamanusia mulai dari informasi karyawan, otomatisasi leave management, track karyawan, pemberian gaji karyawan, pembukaan lowongan pekerjaan, serta manajemen pelatihan bagi karyawan.



## Referensi
- Instalasi icehrm | https://github.com/gamonoid/icehrm
- PHPmyadmin Documentation | https://help.ubuntu.com/lts/serverguide/phpmyadmin.html
- Icehrm's Features | https://icehrm.com/learn-more-about-icehrm-features
- Aplikasi Icehrm | http://blog.icehrm.com/docs/home/
- Pengertian HRIS | pakarkinerja.com/elemen-utama-dalam-human-resource-information-system-hris/
- Admidio | https://www.admidio.org/dokuwiki/doku.php?id=en:2.0:index
