---
layout: post
title: Konfigurasi Web Server - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco.png
tags: [web, server, cisco]
comments: true
---

Web server adalah sebuah software (perangkat lunak) yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan HTTP atau HTTPS dari klien atau kita kenal dengan web browser (Chrome, Firefox). Selanjutnya ia akan mengirimkan respon atas permintaan tersebut kepada client dalam bentuk halaman web.

## Fungsi Web Server

Web Server memiliki peran dalam memproses berbagai data yang diminta oleh klien (web browser). Kemudian ia memberikan hasil atau jawaban berupa dokumen, video, foto, atau beragam bentuk berkas lainnya.

### Beberapa bagian fungsi dari web server:

- Membersihkan berbagai cache yang terdapat pada penyimpanan serta semua dokumen yang tidak terpakai lagi.
- Melakukan pemeriksaan terhadap sistem security yang berasal dari permintaan HTTP berdasarkan request klien atau web browser.
- Menyediakan data berdasarkan request atau permintaan yang masuk agar dapat menjamin keamanan sistem yang berjalan dengan lancar.

## Jenis-jenis Web Server

- Web Server Apache
- Web Server Nginx
- Web Server IIS
- Web Server Lighttpd

## Konfigurasi Web Server

{: .box-note}
Siapkan 1 server, 1 switch, dan 3 pc.

![cisco-web-1](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-1.png)

{: .box-note}
Setting IP Address dan DNS pada server.

![cisco-web-2](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-2.png)

{: .box-note}
Tambahkan DNS pada server dengan klik **Service** > **DNS** > **DNS Service : On**  
Isi **Name** : (diisi dengan domain) dan **Address** : (diisi dengan IP DNS pada server)  
Lalu klik **Add**.

![cisco-web-3](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-3.png)

{: .box-note}
Berikan IP pada ketiga PC.

![cisco-web-4](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-4.png)

![cisco-web-5](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-5.png)

![cisco-web-6](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-6.png)

{: .box-note}
Tes dengan masuk ke web browser pada salah satu PC.

![cisco-web-7](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-7.png)

![cisco-web-8](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-8.png)
