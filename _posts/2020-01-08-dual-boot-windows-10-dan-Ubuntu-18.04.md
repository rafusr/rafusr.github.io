---
layout: post
title: Dual Boot Windows 10 dan Ubuntu 18.04
subtitle: 
cover-img: 
thumbnail-img: /assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/windows10xubuntu.png
share-img: /assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/windows10xubuntu.png
tags: [install]
comments: true
---

Dual boot adalah istilah dimana satu komputer dapat terpasang 2 sistem operasi yang dapat dijalankan secara bergantian.

## Kelebihan dari dual booting

- Ketika salah satu sistem operasi terkendala masalah, maka sistem operasi yang lainnya lagi dapat memperbaiki masalah tersebut.

- Mengurangi biaya hardware. Jadi gaperlu beli 1 PC hanya untuk 1 sistem operasi. karena 1 PC tersebut dapat menjalankan lebih dari 1 OS.

- Kompatibilitas software. Ada 1 software yang dapat berjalan baik di Linux, tapi buruk di Windows, tapi lebih baik di Mac OS. begitu sebaliknya. Nah dengan dual booting, Anda dapat lebih mudah dalam mengakses software ini dalam 1 jenis komputer. sekali lagi, mengurangi biaya hardware.

## Langkah-langkah dual boot Windows 10 dan Ubuntu 18.04

{% highlight javascript linenos %}
Download ISO ubuntu 18.04
Kosongkan partisi untuk ubuntu terlebih dahulu
Siapkan flash drive untuk diisi file ubuntu (disarankan mem-backup / memindahkan file di flash drive tersebut)
Buka aplikasi rufus > pilih flash drive yang digunakan > pilih file ISO ubuntu 18.04 > lalu klik start
{% endhighlight %}

![dual-boot-1](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-1.png)

{% highlight javascript linenos %}
Setelah selesai, shutdown pc, lalu masuk bios > pilih flash drive tadi sebagai boot utama
Setelah masuk ke menu ubuntu, klik install di pojok kiri atas
Pilih bahasa, lalu klik continue
{% endhighlight %}

![dual-boot-2](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-2.png)

![dual-boot-3](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-3.png)

{% highlight javascript linenos %}
Pilih instalasi normal atau minimal, dan centang install third-party software
{% endhighlight %}

![dual-boot-4](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-4.png)

{% highlight javascript linenos %}
Pilih Something else, lalu klik continue
{% endhighlight %}

![dual-boot-5](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-5.png)

{% highlight javascript linenos %}
Lalu pilih partisi yang telah dikosongkan tadi > tekan icon +
Untuk partisi home berikan 30gb (atau sesuai selera)
Untuk swap area, jika pc anda memiliki ram 4gb sebaiknya berikan 2x lipatnya yaitu 8gb (atau lebih)
Untuk partisi root berikan sisa dari partisi kosong yang telah dibagi tadi
Lalu klik install now
{% endhighlight %}

![dual-boot-6](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-6.png)

{% highlight javascript linenos %}
Selanjutnya pilih zona waktu Jakarta (jika anda berada di zona waktu Jakarta)
Akan muncul perintah untuk restart
Setelah restart akan muncul perintah untuk mencabut flash drive, cabut flash drive lalu tekan enter
Pada menu boot manager pilih ubuntu
{% endhighlight %}

![dual-boot-7](/assets/img/dual-boot-windows-10-dan-Ubuntu-18.04/dual-boot-7.png)
