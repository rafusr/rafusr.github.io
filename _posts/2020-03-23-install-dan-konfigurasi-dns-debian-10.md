---
layout: post
title: Install dan Konfigurasi DNS Debian 10
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-dan-konfigurasi-dns-debian-10/bind9.png
share-img: /assets/img/install-dan-konfigurasi-dns-debian-10/bind9.png
tags: [install, dns, debian]
comments: true
---

Domain Name System (DNS) adalah sebuah sistem yang menyimpan informasi tentang nama host ataupun nama domain dalam bentuk database, DNS menyediakan alamat IP untuk setiap nama host dan mendata setiap server transmisi yang menerima surel (email) untuk setiap domain.  

## Install DNS Debian 10

{: .box-note}
Masuk sebagai **super user**, lalu install **bind9** dan utility-nya dengan mengetikkan  
`apt install bind9` dan `apt install dnsutils`.

![dns-debian-1](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-1.png)

## Konfigurasi DNS Debian 10

{: .box-note}
Masuk ke direktori bind dengan mengetikkan `cd /etc/bind` , lalu tambahkan **zone forward** dan **reverse** pada file **named.conf.local**.

![dns-debian-2](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-2.png)

![dns-debian-3](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-3.png)

{: .box-note}
Copy **db.local** ke **forward** dan **db.127** ke **reverse**.

![dns-debian-4](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-4.png)

{: .box-note}
Edit file **forward**.

![dns-debian-5](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-5.png)

{: .box-note}
Edit juga file **reverse**.

![dns-debian-6](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-6.png)

{: .box-note}
Selanjutnya restart bind9.

![dns-debian-7](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-7.png)

{: .box-note}
Masuk ke **/etc/resolv.conf** lalu tambahkan domain dan nameserver anda.

![dns-debian-8](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-8.png)

{: .box-note}
Anda bisa mengeceknya menggunakan **nslookup** ataupun **dig**.

![dns-debian-9](/assets/img/install-dan-konfigurasi-dns-debian-10/dns-debian-9.png)
