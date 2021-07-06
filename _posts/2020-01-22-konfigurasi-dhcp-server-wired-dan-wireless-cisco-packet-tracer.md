---
layout: post
title: Konfigurasi DHCP Server Wired dan Wireless - Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco.png
share-img: /assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco.png
tags: [dhcp, cisco]
comments: true
---

DHCP (Dynamic Host Configuration Protocol) adalah protokol yang dipakai untuk memudahkan penyebaran alamat IP (internet protocol) secara otomatis ke perangkat lainnya. 
Dengan menggunakan DHCP, alamat IP dapat dibagikan ke banyak perangkat dalam satu waktu secara otomatis.

DHCP server adalah sebuah perangkat yang bertugas untuk mengatur dan memberikan alamat IP secara otomatis kepada komputer client yang ada. Sementara itu, komputer / perangkat lain seperti handphone yang menerima alamat IP dari DHCP server disebut DHCP client. 

## Fungsi DHCP Server

- Mengelola dan Mendistribusikan Alamat IP 
- Mencegah IP Conflict 
- Memperbarui Alamat IP secara Otomatis
- Mendukung Penggunaan Kembali Alamat IP

## Konfigurasi DHCP Server

{% highlight javascript linenos %}
Buat topologinya
{% endhighlight %}

![cisco-dhcp-1](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-1.png)

{% highlight javascript linenos %}
Berikan IP untuk server
{% endhighlight %}

![cisco-dhcp-2](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-2.png)

{% highlight javascript linenos %}
Selanjutnya masuk ke Services > DHCP > on, lalu buat seperti ini > klik add
{% endhighlight %}

![cisco-dhcp-3](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-3.png)

{% highlight javascript linenos %}
Masuk ke router > GUI > setting seperti ini
{% endhighlight %}

![cisco-dhcp-4](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-4.png)

{% highlight javascript linenos %}
Berikan SSID dan Password untuk jaringan wireless
{% endhighlight %}

![cisco-dhcp-5](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-5.png)

![cisco-dhcp-6](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-6.png)

{% highlight javascript linenos %}
Masuk ke PC dan ubah IP Address dari Static menjadi DHCP
{% endhighlight %}

![cisco-dhcp-7](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-7.png)

{% highlight javascript linenos %}
Untuk koneksi wireless ubah port lan pada laptop menjadi WPC300N
{% endhighlight %}

![cisco-dhcp-8](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-8.png)

![cisco-dhcp-9](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-9.png)

{% highlight javascript linenos %}
Selanjutnya pilih Desktop > PC Wireless > Connect, lalu pilih jaringan yang kita buat dan masukkan passwordnya > klik Connect
{% endhighlight %}

![cisco-dhcp-10](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-10.png)

{% highlight javascript linenos %}
Ping untuk mengetes
{% endhighlight %}

![cisco-dhcp-11](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-11.png)

![cisco-dhcp-12](/assets/img/konfigurasi-dhcp-server-wired-dan-wireless-cisco-packet-tracer/cisco-dhcp-12.png)
