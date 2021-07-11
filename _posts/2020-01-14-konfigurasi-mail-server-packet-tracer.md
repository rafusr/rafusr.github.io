---
layout: post
title: Konfigurasi Mail Server - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-mail-server-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-mail-server-packet-tracer/cisco.png
tags: [tutorial, mail, server, cisco]
comments: true
---

Mail server adalah server yang bertugas mengirim dan menerima email. Email yang Anda kirim akan melewati serangkaian proses rumit di mail server untuk dapat sampai ke penerima.  
Secara sederhana, mail server berfungsi sama seperti kantor pos. Ia menyimpan surat masuk, lalu mengirimkannya ke penerima. 

## Komponen Mail Server

- MUA (Mail User Agent)
- MTA (Mail Transport Agent) 
- MDA (Mail Delivery Agent)

## Protokol Mail Server

- SMTP atau Simple Mail Transfer Protocol 
- POP3 atau Post Office Protocol 
- IMAP atau Internet Message Access

## Jenis-Jenis Mail Server

- Sendmail
- Postfix
- Qmail

## Konfigurasi Mail Server

{: .box-note}
Sediakan 1 server, 1 switch, dan 3 komputer.

![cisco-mail-1](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-1.png)

{: .box-note}
Masukkan IP Address dan DNS pada server.

![cisco-mail-2](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-2.png)

{: .box-note}
Siapkan email untuk 3 komputer. Klik **Services** > **EMAIL**.  
Lalu masukkan domain, user, dan password > klik **+** untuk menambahkan.  
Lakukan 3 kali dengan user yang berbeda untuk memberikan email pada 3 komputer.

![cisco-mail-3](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-3.png)

{: .box-note}
Sekarang berikan IP Address untuk semua komputer.

![cisco-mail-4](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-4.png)

![cisco-mail-5](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-5.png)

![cisco-mail-6](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-6.png)

{: .box-note}
Berikan Email untuk komputer dengan masuk ke **Desktop** > **Email**  
**nama** : (bebas), **email** : (nama)@(domain yang dibuat di server tadi),  
**incoming & outgoing mail server** diisi sesuai ip dns yang dibuat di server,  
username dan password diisi sesuai dengan yang dibuat di server.

![cisco-mail-7](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-7.png)

![cisco-mail-8](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-8.png)

![cisco-mail-9](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-9.png)

{: .box-note}
Tes dengan mengirim email dari komputer 1 ke komputer yang lain dengan klik **Desktop** > **Email** > **Compose**.  
Untuk mengirim klik **Send**.

![cisco-mail-10](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-10.png)

{: .box-note}
Untuk mengecek apakah email diterima, masuk ke komputer yang dijadikan tujuan pengiriman > **Desktop** > **Email** > **Receive**.

![cisco-mail-11](/assets/img/konfigurasi-mail-server-packet-tracer/cisco-mail-11.png)
