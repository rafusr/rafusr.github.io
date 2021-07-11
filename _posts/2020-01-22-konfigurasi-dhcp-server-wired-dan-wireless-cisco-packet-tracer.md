---
layout: post
title: Konfigurasi DHCP Server Wired dan Wireless - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco.png
tags: [tutorial, dhcp, server, cisco]
comments: true
---

DHCP (Dynamic Host Configuration Protocol) adalah protokol yang dipakai untuk memudahkan penyebaran alamat IP (internet protocol) secara otomatis ke perangkat lainnya. Dengan menggunakan DHCP, alamat IP dapat dibagikan ke banyak perangkat dalam satu waktu secara otomatis.  

DHCP server adalah sebuah perangkat yang bertugas untuk mengatur dan memberikan alamat IP secara otomatis kepada komputer client yang ada. Sementara itu, komputer / perangkat lain seperti handphone yang menerima alamat IP dari DHCP server disebut DHCP client. 

## Fungsi DHCP Server

- Mengelola dan Mendistribusikan Alamat IP 
- Mencegah IP Conflict 
- Memperbarui Alamat IP secara Otomatis
- Mendukung Penggunaan Kembali Alamat IP

## Konfigurasi DHCP Server

{: .box-note}
Buat topologinya.

![cisco-dhcp-1](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-1.png)

{: .box-note}
Berikan IP untuk server.

![cisco-dhcp-2](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-2.png)

{: .box-note}
Selanjutnya masuk ke **Services** > **DHCP** > **on**, lalu buat seperti ini > klik **add**.

![cisco-dhcp-3](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-3.png)

{: .box-note}
Masuk ke **router** > **GUI**, lalu setting seperti ini.

![cisco-dhcp-4](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-4.png)

{: .box-note}
Berikan SSID dan Password untuk jaringan wireless.

![cisco-dhcp-5](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-5.png)

![cisco-dhcp-6](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-6.png)

{: .box-note}
Masuk ke PC dan ubah IP Address dari Static menjadi DHCP.

![cisco-dhcp-7](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-7.png)

{: .box-note}
Untuk koneksi wireless ubah port lan pada laptop menjadi **WPC300N**.

![cisco-dhcp-8](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-8.png)

![cisco-dhcp-9](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-9.png)

{: .box-note}
Selanjutnya pilih **Desktop** > **PC Wireless** > **Connect**, 
lalu pilih jaringan yang kita buat dan masukkan passwordnya > klik **Connect**.

![cisco-dhcp-10](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-10.png)

{: .box-note}
Ping untuk mengetes.

![cisco-dhcp-11](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-11.png)

![cisco-dhcp-12](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-12.png)
