---
layout: post
title: Konfigurasi DNS - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-dns-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-dns-cisco-packet-tracer/cisco.png
tags: [dns, cisco]
comments: true
---

Domain Name System (DNS) adalah sebuah sistem yang menyimpan informasi tentang nama host ataupun nama domain dalam bentuk database,
DNS menyediakan alamat IP untuk setiap nama host dan mendata setiap server transmisi yang menerima surel (email) untuk setiap domain.

## Cara Kerja DNS

Sebuah program klien (browser) yang berjalan di komputer pengguna meminta IP Address untuk domain.
DNS lokal akan mengecek di dalam cache server DNS server lokal, jika data itu ada di dalam cache server, maka server akan memberikan IP Address domain tsb.
Jika tidak ada, maka server akan menghubungi root name server untuk mengetahui IP Address sebuah domain.

## Tipe DNS Record

- **A Record**, bertugas untuk mengarahkan domain / subdomain ke alamat ip domain tsb.
- **CNAME**, bertugas untuk mengarahkan subdomain kepada domain.
- **SOA (Start Of Authorit)**, merupakan server DNS yang menyediakan informasi tentang sebuah domain.
- **NS Record**, merupakan server yang memiliki database domain name dan IP Address yang berfungsi untuk menyimpan nama domain dan record DNS dari domain tsb.

## Cara Mengecek NS record sebuah domain

1. Masuk ke situs who.is
2. Ketikkan domain lalu enter
3. Disitu akan ada informasi tentang domain tsb.

## Konfigurasi DNS
{% highlight javascript linenos %}
Siapkan 1 buah server, 1 buah switch, dan  buah komputer
{% endhighlight %}

![cisco-dns-1](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-1.png)

{% highlight javascript linenos %}
Konfigurasi IP Address server dan pc seperti ini seperti ini
{% endhighlight %}

![cisco-dns-2](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-2.png)

![cisco-dns-3](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-3.png)

![cisco-dns-4](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-4.png)

![cisco-dns-5](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-5.png)

{% highlight javascript linenos %}
Berikan DNS untuk server dan masing-masing PC
{% endhighlight %}

![cisco-dns-6](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-6.png)

{% highlight javascript linenos %}
Tes dengan ping semua domain pada masing-masing PC
{% endhighlight %}

![cisco-dns-7](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-7.png)

![cisco-dns-8](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-8.png)

![cisco-dns-9](/assets/img/konfigurasi-dns-cisco-packet-tracer/cisco-dns-9.png)
