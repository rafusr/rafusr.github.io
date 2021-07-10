---
layout: post
title: Konfigurasi Bridge Mikrotik - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-bridge-mikrotik-virtualbox/mikrotik.png
share-img: /assets/img/konfigurasi-bridge-mikrotik-virtualbox/mikrotik.png
tags: [bridge, mikrotik, virtualbox]
comments: true
---

Mikrotik RouterOS adalah sistem operasi Linux base yang diperuntukkan sebagai network router yang instalasinya dapat dilakukan pada Standard komputer PC.  
PC yang akan dijadikan router mikrotik pun tidak memerlukan resource yang cukup besar untuk penggunaan standard, misalnya hanya sebagai gateway.  
  
Sementara itu Bridge adalah suatu alat yang dapat menghubungkan jaringan komputer LAN dengan jaringan LAN yang lain. Bridge dapat menghubungkan tipe jaringan komputer berbeda-beda (misalnya seperti Ethernet & Fast Ethernet), ataupun tipe jaringan yang serupa atau sama.  

Anda bisa membuat client pada VirtualBox terlebih dahulu, disini Saya menggunakan Windows XP.  

## Konfigurasi Bridge

{: .box-note}
Tambahkan **Internal Network** pada setting network mikrotik.

![bridge-mikrotik-1](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-1.png)

![bridge-mikrotik-2](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-2.png)

{: .box-note}
Login ke mikrotik, lalu masuk ke winbox dan tambahkan **bridge**.

![bridge-mikrotik-3](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-3.png)

{: .box-note}
Tambahkan IP Address untuk **bridge**.

![bridge-mikrotik-4](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-4.png)

{: .box-note}
Hubungkan **bridge** pada **internal network**.

![bridge-mikrotik-5](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-5.png)

{: .box-note}
Masuk ke **DHCP Server**, klik **DHCP Setup** lalu klik next sampai selesai.

![bridge-mikrotik-6](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-6.png)

{: .box-note}
Setting network Windows XP (client) menjadi **Internal Network** lalu masuk ke Windows XP (client).

![bridge-mikrotik-7](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-7.png)

{: .box-note}
Cek apaka Windows XP (client) telah conncet pada **bridge**.

![bridge-mikrotik-8](/assets/img/konfigurasi-bridge-mikrotik-virtualbox/bridge-mikrotik-8.png)
