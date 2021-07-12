---
layout: post
title: Install dan Konfigurasi DNS Ubuntu
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-dan-konfigurasi-dns-ubuntu/bind9.png
share-img: /assets/img/install-dan-konfigurasi-dns-ubuntu/bind9.png
tags: [tutorial, install, dns, ubuntu]
comments: true
---

Domain Name System (DNS) adalah sebuah sistem yang menyimpan informasi tentang nama host ataupun nama domain dalam bentuk database, DNS menyediakan alamat IP untuk setiap nama host dan mendata setiap server transmisi yang menerima surel (email) untuk setiap domain.

## Install DNS Ubuntu

{: .box-note}
Install bind dan utility-nya pada ubuntu dengan mengetikkan `sudo apt install -y bind9 bind9utils bind9-doc dnsutils`.

![dns-ubuntu-1](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-1.png)

## Konfigurasi DNS Ubuntu

{: .box-note}
Masuk ke direktori bind, lalu edit file **named.conf.local**.

![dns-ubuntu-2](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-2.png)

{: .box-note}
Copy **db.local** ke file **forward** dan **db.127** ke file **reverse**.

![dns-ubuntu-3](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-3.png)

{: .box-note}
Edit **forward** dan **reverse**.

![dns-ubuntu-4](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-4.png)

![dns-ubuntu-5](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-5.png)

{: .box-note}
Setelah selesai, restart bind.

![dns-ubuntu-6](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-6.png)

{: .box-note}
Tambahkan domain dan ip pada **resolv.conf**, anda bisa mengetikkan `nano /etc/resolv.conf`.

![dns-ubuntu-7](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-7.png)

{: .box-note}
Coba tes menggunakan **nslookup** atau **dig**.

![dns-ubuntu-8](/assets/img/install-dan-konfigurasi-dns-ubuntu/dns-ubuntu-8.png)
