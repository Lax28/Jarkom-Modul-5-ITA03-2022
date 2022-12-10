# Jarkom-Modul-5-ITA03-2022
## Anggota Kelompok
1. Muhammad Jovan Adiwijaya Yanuarsyah (5027201025)
2. Muhammad Naufal Pasya (5027201045)
3. Fatchia Farhan (5027201044)

## Deskripsi
Laporan ini dibuat dengan tujuan untuk menjelaskan pengerjaan serta permasalahan yang kami alami dalam pengerjaan soal shift Jaringan Komunikasi modul 5 tahun 2022.

## Soal
Setelah kalian mempelajari semua modul yang telah diberikan, Loid ingin meminta bantuan untuk terakhir kalinya kepada kalian. Dan kalian dengan senang hati mau membantu Loid.

1. Tugas pertama kalian yaitu membuat topologi jaringan sesuai dengan rancangan yang diberikan Loid dibawah ini:

![image](https://user-images.githubusercontent.com/90241858/206861072-2a49fbc3-bd49-476d-ada6-055d1284759c.png)

Keterangan :	- Eden adalah DNS Server
              - WISE adalah DHCP Server
		          - Garden dan SSS adalah Web Server
		          - Jumlah Host pada Forger adalah 62 host
		          - Jumlah Host pada Desmond adalah 700 host
		          - Jumlah Host pada Blackbell adalah 255 host
		          - Jumlah Host pada Briar adalah 200 host

2. Untuk menjaga perdamaian dunia, Loid ingin meminta kalian untuk membuat topologi tersebut menggunakan teknik CIDR atau VLSM setelah melakukan subnetting.
3. Anya, putri pertama Loid, juga berpesan kepada anda agar melakukan Routing agar setiap perangkat pada jaringan tersebut dapat terhubung.

4. Tugas berikutnya adalah memberikan ip pada subnet Forger, Desmond, Blackbell, dan Briar secara dinamis menggunakan bantuan DHCP server. Kemudian kalian ingat bahwa  kalian harus setting DHCP Relay pada router yang menghubungkannya.
    a. Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi Strix menggunakan iptables, tetapi Loid tidak ingin menggunakan             MASQUERADE.
    b. Kalian diminta untuk melakukan drop semua TCP dan UDP dari luar Topologi kalian pada server yang merupakan DHCP Server demi menjaga keamanan.
    c. Loid meminta kalian untuk membatasi DHCP dan DNS Server hanya boleh menerima maksimal 2 koneksi ICMP secara bersamaan menggunakan iptables, selebihnya didrop.
    d. Akses menuju Web Server hanya diperbolehkan disaat jam kerja yaitu Senin sampai Jumat pada pukul 07.00 - 16.00.
    e. Karena kita memiliki 2 Web Server, Loid ingin Ostania diatur sehingga setiap request dari client yang mengakses Garden dengan port 80 akan didistribusikan              secara bergantian pada SSS dan Garden secara berurutan dan request dari client yang mengakses SSS dengan port 443 akan didistribusikan secara bergantian pada          Garden dan SSS secara berurutan.
    f. Karena Loid ingin tau paket apa saja yang di-drop, maka di setiap node server dan router ditambahkan logging paket yang di-drop dengan standard syslog level.
Loid berterima kasih pada kalian karena telah membantunya. Loid juga mengingatkan agar semua aturan iptables harus disimpan pada sistem atau paling tidak kalian menyediakan script sebagai backup.
