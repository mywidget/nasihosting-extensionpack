# nasihosting-extensionpack


Nasihosting Extension Pack 2.6 Full version
--------------------
![alt text](http://xcode.or.id/04_small-logo.png)

Hanya mendukung Ubuntu Server 16.04 dan 18.04, untuk untuk Ubuntu 20.04 tidak didukung, jika dipaksakan, maka user tidak bisa login ke phpmyadmin tapi bisa untuk file manager. 

Script untuk membangun hosting yang berjalan otomatis dari sisi client, subdomain langsung aktif dan bisa langsung dipakai. 

Cara menggunakan Nasihosting-ExtensionPack
------------------------------------------
ExtensionPack hanya boleh dijalankan jika Nasihosting v3.1 sudah aktif dan berjalan normal di server
1. cd /home (harus di /home)
2. git clone https://github.com/kurniawandata/nasihosting-extensionpack
3. cd nasihosting-extensionpack
4. chmod -R 777 *
5. ./install-httponly.sh (tanpa https)
6. ./install.sh (pakai https, pastikan sertifikat untuk SSL sudah punya)
7. Edit aktivasi3.sh, sesuaikan dengan setting di akun cloudflare

Untuk point 7, jika ingin aktivasi manual, tidak otomatis maka hapus kode sumber di bawah ini :

Kode sumber yang dihapus pada file aktivasi3.sh, jika tidak ingin aktivasi otomatis (Aktivasi manual)
-------------
sudo cp /usr/lib/cgi-bin/aktivasi3.sh aktivasi4.sh

sed -i "s/unik/$name/g" /usr/lib/cgi-bin/aktivasi4.sh

chmod 777 aktivasi4.sh

./aktivasi4.sh

rm aktivasi4.sh

Ganti domain utama
------------
./gantidomain.sh (mendukung https)

./gantidomain-httponly.sh (hanya mendukung http)


Melihat subdomain user, password dan tanggal dibuat
------------
/home/datauser


Licensi
-------
GNU General Public License v3

Program ini dibuat oleh :
--------------------------------------------
Kurniawan. E-mail : kurniawan@securityhub.id
xcode.or.id


Donasi :
--------
Jika ingin donasi untuk Kurniawan

Gopay :

![alt text](http://xcodeserver.my.id/gofood.png)

![alt text](http://xcodeserver.my.id/gopay.png)

Ovo :

![alt text](http://xcodeserver.my.id/ovo3.png)

![alt text](http://xcodeserver.my.id/ovo2.png)
