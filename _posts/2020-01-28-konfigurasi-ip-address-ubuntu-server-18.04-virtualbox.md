---
layout: post
title: Konfigurasi IP Address Ubuntu Server 18.04 - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ubuntu.png
share-img: /assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ubuntu.png
tags: [virtual box, ubuntu, server]
comments: true
---

Ubuntu adalah sistem operasi desktop yang pertama kali dirilis pada 20 Oktober 2004 dan dikembangkan oleh Cannonical Ltd. Sementara itu, Ubuntu Server adalah Ubuntu yang dikembangkan khusus untuk sistem operasi server.  

Pada Ubuntu Server tidak disediakan Graphical User Interface (GUI). Hal itu berarti semua bentuk eksekusi program dijalankan melalui baris perintah yang disebut dengan Command Line Interface (CLI).

## Konfigurasi IP Address Ubuntu Server 18.04

{: .box-note}
Masuk ke VirtualBox, lalu tambahkan network baru pada menu **File** > **Host Network Manager** (ctrl+h).

![ip-ubuntu-1](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-1.png)

{: .box-note}
Lalu ubah setting network pada ubuntu server menjadi **Host Only Adapter** dan pilih network yang kita buat tadi.

![ip-ubuntu-2](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-2.png)

{: .box-note}
Selanjutnya masuk ke Ubuntu server ubah pada mode super user (su)  
Lalu masuk ke `/etc/network/interfaces` untuk mengubah ip, setelah selesai, **exit** > **save**.

![ip-ubuntu-3](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-3.png)

{: .box-note}
Restart networking service dengan mengetikkan `/etc/init.d/networking restart` (jika muncul tulisan yang menunjukkan tidak ada direktori, silahkan install `ifupdown` terlebih dahulu).

![ip-ubuntu-4](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-4.png)

{: .box-note}
Untuk mengetesnya anda dapat ping melalui ubuntu server ataupun pc anda.

![ip-ubuntu-5](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-5.png)

![ip-ubuntu-6](/assets/img/konfigurasi-ip-address-ubuntu-server-18.04-virtualbox/ip-ubuntu-6.png)
