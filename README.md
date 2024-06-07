# Jarkom-Modul-4-IT31-2024

| No | Nama | NRP |
|---|---|---|
| 1 | M. Januar Eko Wicaksono | 50272221006 |
| 2 | SUbkhan Mas Udi | 50272221044 |

## SOAL SHIFT MODUL 4
### TOPOLOGI
![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/topo_modul4.png)

## VLSM - GNS
### TOPOLOGI
![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Topologi_GNS.jpg)

1. Arakis (Router(DHCP Relay))
```bash
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.232.1.0
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.232.2.0
	netmask 255.255.255.0

auto eth3
iface eth3 inet static
	address 192.232.3.0
	netmask 255.255.255.0

auto eth4
iface eth4 inet static
	address 192.232.4.0
	netmask 255.255.255.0
```



## CIDR - CPT
### TOPOLOGI
![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Topologi_CPT.png)

CIDR atau biasa dikenal Classless Inter-Domain Routing adalah suatu metode pengalamatan dan pengelompokan alamat IP yang memungkinkan penggunaan lebih efisien dari ruang alamat IP yang tersedia di Internet. Sebelum diperkenalkannya CIDR, pengalamatan IP didasarkan pada kelas-kelas, seperti kelas A, kelas B, dan kelas C. Setiap kelas memiliki ukuran tetap untuk jaringan dan host, yang seringkali mengakibatkan pemborosan alamat IP.

CIDR menggantikan pendekatan kelas dengan memperkenalkan notasi format baru yang memungkinkan fleksibilitas lebih besar dalam pengelompokan dan alokasi alamat IP. Format notasi CIDR terdiri dari alamat IP dan prefiks (subnet mask) yang diwakili dalam format bilangan biner, seperti contoh berikut:
```bash
192.232.0.0 / 24
```
Dalam contoh ini, "192.232.0.0" adalah alamat jaringan, dan "/24" menunjukkan bahwa 24 bit pertama dari alamat ini digunakan sebagai netmask (subnet mask). Dengan menggunakan CIDR, administrator jaringan dapat menentukan ukuran subnet yang sesuai dengan kebutuhan tanpa terikat pada batasan kelas tradisional.

Keuntungan utama CIDR melibatkan penghematan alamat IP dan pengurangan pemborosan. Dengan CIDR, tidak perlu lagi mengalokasikan blok alamat IP dengan ukuran yang tetap berdasarkan kelas. Sebagai contoh, jika suatu jaringan memerlukan 300 alamat IP, administrator dapat menggunakan CIDR untuk mengalokasikan subnet dengan panjang netmask yang sesuai tanpa harus memilih kelas yang lebih besar dari yang dibutuhkan.

CIDR juga mendukung agregasi rute, yang memungkinkan penyederhanaan tabel routing di Internet. Dengan menggabungkan beberapa blok alamat IP ke dalam satu entri routing, CIDR membantu mengurangi ukuran tabel routing dan efektif meningkatkan efisiensi dalam pengelolaan lalu lintas jaringan global.

### Penggabungan IP
Berikut merupakan inisialisasi kami yang akan digunakan untuk melakukan penggabungan IP: 
Untuk seluruh konfigurasi, dapat dilihat pada spreadsheet berikut:
[Tabel Konfigurasi.](https://docs.google.com/spreadsheets/d/117bRCcvrnNh4vzwL68N3XM7rk9DwiuP6AgQrCrIaLOE/edit?usp=sharing)

A. Kondisi Node Awal

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_Awal.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Rute_Awal.png)

B. Penggabungan Node Pertama (B)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_B.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_B.png)

C. Penggabungan Node Pertama (C)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_C.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_C.png)

D. Penggabungan Node Pertama (D)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_D.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_D.png)

E. Penggabungan Node Pertama (E)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_E.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_E.png)

F. Penggabungan Node Pertama (F)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_F.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_F.png)

G. Penggabungan Node Pertama (G)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_G.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_G.png)

H. Penggabungan Node Pertama (H)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_H.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_H.png)

I. Penggabungan Node Pertama (I)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_I.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_I.png)

J. Penggabungan Node Pertama (J)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_J.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_J.png)

K. Penggabungan Node Pertama (K)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Penggabungan_K.png)

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Node_K.png)


### TREE
Setelah dilakukannya penggabungan IP, sekarang kita melakukan pembagian IP dengan menggunakan tree pada masing-masing kelompok yang telah dibuat sebelumnya sebagai berikut:

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Modul4_CIDR_IT31.png)

### PEMBAGIAN IP
Berikut merupakan hasil dari pembagian IP berdasarkan Tree yang telah dibuat sebelumnya

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/pembagian_cidr.png)

### TESTING
Jika sudah mencoba ping antara client-router, router-client, client-client. Jika succesfull seperti di pojok bawah maka benar hasilnya:

![](https://github.com/mrvlvenom/Jarkom-Modul-4-IT31-2024/blob/main/img/Hasil.png)
