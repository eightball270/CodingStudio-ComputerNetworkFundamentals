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
Untuk terhubung dengan network yang tidak terkoneksi secara langsung (dalam kasus ini 2 router), harus dilakukan routing. Cara untuk melakukan static routing pada Cisco adalah dengan menambahkan alamat network tujuan, subnet mask, dan ip router ke-2 yang terhubung langsung dengan router ke-1.
- ip route [alamat network tujuan] [subnet mask] [ip router lain yang terhubung langsung]
- contoh command : Router(config)#ip route 192.168.3.0 255.255.255.0 192.168.1.2

![CodingStudio - Static Routing](https://github.com/user-attachments/assets/122e67aa-a94e-4129-a12e-4a1d57b54ff4)

## Telnet dan SSH
