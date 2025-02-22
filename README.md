# CodingStudio-ComputerNetworkFundamentals
Materi tentang Fundamental Jaringan Komputer dari CodingStudio yang telah dipelajari:
1. Jenis-Jenis Topologi Jaringan
2. Static IP Address dan Ping (ICMP)
3. Static Routing
4. Telnet dan SSH

## Jenis-Jenis Topologi Jaringan
Topologi jaringan komputer memiliki 5 jenis, yaitu:
1. Topologi Bus
2. Topologi Ring
3. Topologi Tree
4. Topologi Star
5. Topologi Mesh

![CodingStudio - Jenis-Jenis Topologi Jaringan](https://github.com/user-attachments/assets/7536e634-8e16-400b-84f6-e859251a0f2e)

## Static IP Address dan Ping (ICMP)
Sebuah jaringan dapat terkoneksi satu sama lain jika dilakukan konfigurasi alamat IP secara static pada masing-masing perangkat jaringan, kemudian lakukan ping untuk memastikan satu perangkat terhubung ke perangkat lainnya.

![CodingStudio - Static IP dan ICMP (Pinging)](https://github.com/user-attachments/assets/065238e0-1a3b-46e7-811b-2377bf828bce)

## Static Routing
Dalam praktik ini menggunakan 2 buah router, router A terhubung network 192.168.2.0/24, router B terhubung network 192.168.3.0/24, dan network antar router 192.168.1.0/24. Agar network 192.168.2.0 terjangkau ke network 192.168.3.0 harus dilakukan konfigurasi routing untuk meneruskan trafik ke network lain. Metode yang digunakan adalah static routing, yaitu membuat routing table secara manual. Cara untuk melakukan static routing pada router A adalah dengan menambahkan alamat network tujuan (network address dan subnet mask) dan ip interface router B yang terhubung langsung dengan router A.
- ip route [alamat network tujuan] [subnet mask] [ip router lain yang terhubung langsung]
- contoh command : RouterA(config)#ip route 192.168.3.0 255.255.255.0 192.168.1.2

![CodingStudio - Static Routing](https://github.com/user-attachments/assets/122e67aa-a94e-4129-a12e-4a1d57b54ff4)

## Telnet dan SSH
Untuk melakukan remote perangkat jaringan seperti router atau switch dari PC/Laptop, dapat dilakukan dengan 2 metode yaitu Telnet dan SSH. Telnet dan SSH adalah protokol jaringan yang digunakan untuk mengakses perangkat jarak jauh. Perbedaan keduanya adalah Telnet tidak menggunakan enkripsi data, sedangkan SSH menggunakan enkripsi data. SSH yang digunakan adalah SSH versi 2, dengan syarat rsa key minimal 768 bits, disini dilakukan konfigurasi generate rsa key sebesar 1024 bits.

![CodingStudio - Telnet dan SSH](https://github.com/user-attachments/assets/c01b656c-235e-494e-96ff-339d4a96f845)
