---
layout: post
title: Install dan Konfigurasi DNS CentOS 7
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-dan-konfigurasi-dns-centos-7/bind9.png
share-img: /assets/img/install-dan-konfigurasi-dns-centos-7/bind9.png
tags: [tutorial, install, dns, centos]
comments: true
---

Domain Name System (DNS) adalah sebuah sistem yang menyimpan informasi tentang nama host ataupun nama domain dalam bentuk database, DNS menyediakan alamat IP untuk setiap nama host dan mendata setiap server transmisi yang menerima surel (email) untuk setiap domain.  

## Install DNS CentOS 7

{: .box-note}
Install bind dan utility nya dengan mengetikkan `yum install bind bind-utils -y`.

![dns-centos-1](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-1.png)

## Konfigurasi DNS CentOS 7

{: .box-note}
Masuk ke direktori **etc** dengan mengetikkan `cd /etc` lalu edit file **named.conf**, scroll ke bawah, lalu tambahkan **zone**.

![dns-centos-2](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-2.png)

![dns-centos-3](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-3.png)

![dns-centos-4](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-4.png)

{: .box-note}
Masuk ke direktori **/etc/named** dan tambahkan file **forward** dan **reverse** yang ada pada zona tadi.

![dns-centos-5](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-5.png)

![dns-centos-6](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-6.png)

{: .box-note}
Selanjutnya ketikkan `systemctl enable named` lalu ketikkan `systemctl restart named` untuk mengaktifkan file **forward** dan **reverse** tadi, untuk melihat apakah sudah aktif anda dapat mengetikkan `systemctl status named`.

![dns-centos-7](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-7.png)

{: .box-note}
Masuk dan edit file **/etc/resolv.conf**, lalu cek dengan **nslookup** atau **dig**.

![dns-centos-8](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-8.png)

![dns-centos-9](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-9.png)

## Membuat Authoritative-only DNS

### Primary DNS (Master)

{: .box-note}
Edit file **named.conf** dengan mengetikkan `nano /etc/named.conf`.  

![dns-centos-10](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-10.png)

![dns-centos-11](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-11.png)

{: .box-note}
Edit file **forward** dan **reverse**.

![dns-centos-12](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-12.png)

![dns-centos-13](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-13.png)

{: .box-note}
Restart dengan mengetikkan `systemctl restart named` lalu tambahkan domain dan ip anda pada **/etc/resolv.conf**.

![dns-centos-14](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-14.png)

### Secondary DNS (Slave)

{: .box-note}
Edit file **named.conf**.

![dns-centos-15](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-15.png)

![dns-centos-16](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-16.png)

![dns-centos-17](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-17.png)

{: .box-note}
Ketikkan `setsebool -P named_write_master_zones on`.

![dns-centos-18](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-18.png)

### Primary DNS (Master)

{: .box-note}
Masuk ke **Primary DNS** lalu edit file **named.conf**.

![dns-centos-19](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-19.png)

{: .box-note}
Tambahkan ip dari **Secondary DNS** pada file **forward** dan **reverse**.

![dns-centos-20](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-20.png)

![dns-centos-21](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-21.png)

{: .box-note}
 Restart **named**, lalu tambahkan ip **Secondary DNS** pada file **resolv.conf**.

![dns-centos-22](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-22.png)

{: .box-note}
Selanjutnya cek **Secondary DNS** melalui **Primary DNS** dengan mengetikkan `dig @(ip secondary dns) mail.(domain)`.

![dns-centos-23](/assets/img/install-dan-konfigurasi-dns-centos-7/dns-centos-23.png)
