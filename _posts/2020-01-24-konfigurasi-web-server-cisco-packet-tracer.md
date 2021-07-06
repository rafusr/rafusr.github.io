---
layout: post
title: Konfigurasi Web Server - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco.png
tags: [web server, cisco]
comments: true
---

Web server adalah sebuah software (perangkat lunak) yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan HTTP atau HTTPS dari klien atau kita kenal dengan web browser (Chrome, Firefox). Selanjutnya ia akan mengirimkan respon atas permintaan tersebut kepada client dalam bentuk halaman web.

## Fungsi Web Server

Web Server memiliki peran dalam memproses berbagai data yang diminta oleh klien (web browser). Kemudian ia memberikan hasil atau jawaban berupa dokumen, video, foto, atau beragam bentuk berkas lainnya.

Beberapa bagian fungsi dari web server:

- Membersihkan berbagai cache yang terdapat pada penyimpanan serta semua dokumen yang tidak terpakai lagi.
- Melakukan pemeriksaan terhadap sistem security yang berasal dari permintaan HTTP berdasarkan request klien atau web browser.
- Menyediakan data berdasarkan request atau permintaan yang masuk agar dapat menjamin keamanan sistem yang berjalan dengan lancar.

## Jenis-jenis Web Server

- Web Server Apache
- Web Server Nginx
- Web Server IIS
- Web Server Lighttpd

## Konfigurasi Web Server

{% highlight javascript linenos %}
Siapkan 1 server, 1 switch, dan 3 pc
{% endhighlight %}

![cisco-web-1](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-1.png)

{% highlight javascript linenos %}
Setting IP Address dan DNS pada server
{% endhighlight %}

![cisco-web-2](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-2.png)

{% highlight javascript linenos %}
Tambahkan DNS pada server dengan klik service > DNS > DNS Service : On > Name : (diisi dengan domain) > Address : (diisi dengan IP DNS pada server) > klik "Add"
{% endhighlight %}

![cisco-web-3](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-3.png)

{% highlight javascript linenos %}
Berikan IP pada ketiga PC
{% endhighlight %}

![cisco-web-4](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-4.png)

![cisco-web-5](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-5.png)

![cisco-web-6](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-6.png)

{% highlight javascript linenos %}
Tes dengan masuk ke web browser pada salah satu PC
{% endhighlight %}

![cisco-web-7](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-7.png)

![cisco-web-8](/assets/img/konfigurasi-web-server-cisco-packet-tracer/cisco-web-8.png)
