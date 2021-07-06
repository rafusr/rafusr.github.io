---
layout: post
title: Konfigurasi DNS - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-dns-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-dns-cisco-packet-tracer/cisco.png
tags: [dns, cisco]
---

## Mengenal Apa Itu DNS

Domain Name System (DNS) adalah sebuah sistem yang menyimpan informasi tentang nama host ataupun nama domain dalam bentuk database,
DNS menyediakan alamat IP untuk setiap nama host dan mendata setiap server transmisi yang menerima surel (email) untuk setiap domain.

## Cara Kerja DNS
Sebuah program klien (browser) yang berjalan di komputer pengguna meminta IP Address untuk domain.
DNS lokal akan mengecek di dalam cache server DNS server lokal, jika data itu ada di dalam cache server, maka server akan memberikan IP Address domain tsb.
Jika tidak ada, maka server akan menghubungi root name server untuk mengetahui IP Address sebuah domain.

## Tipe DNS Record
**A Record**, bertugas untuk mengarahkan domain / subdomain ke alamat ip domain tsb.
**CNAME**, bertugas untuk mengarahkan subdomain kepada domain.
**SOA (Start Of Authorit)**, merupakan server DNS yang menyediakan informasi tentang sebuah domain.
**NS Record**, merupakan server yang memiliki database domain name dan IP Address yang berfungsi untuk menyimpan nama domain dan record DNS dari domain tsb.

## Cara Mengecek NS record sebuah domain

1. Masuk ke situs who.is
2. Ketikkan domain lalu enter
3. Disitu akan ada informasi tentang domain tsb.
