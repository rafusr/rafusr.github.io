---
layout: post
title: Tutorial Cisco Packet Tracer
subtitle: 
cover-img: 
thumbnail-img: /assets/img/tutorial-cisco-packet-tracer/cisco.png
share-img: /assets/img/tutorial-cisco-packet-tracer/cisco.png
tags: [tutorial, cisco]
comments: true
---

Cisco Packet Tracer adalah software untuk simulasi alat-alat jaringan yang digunakan sebagai media pembelajaran. Program ini dibuat oleh Cisco System. Tujuan utama Packet Tracer adalah untuk menyediakan alat bagi siswa dan pengajar agar dapat memahami prinsip jaringan komputer dan juga membangun skill di bidang alat-alat jaringan.  

### Workspace pada Packet Tracer

{: .box-note}
Di pakcet tracer terdapat 2 jenis **workspace**, **Logical** yang berisi topologi secara logikal dan **Physical** yang berisi tentang penempatannya.

![tutorial-cisco-1](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-1.png)

![tutorial-cisco-2](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-2.png)

### Menu pada Packet Tracer

![tutorial-cisco-3](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-3.png)

![tutorial-cisco-4](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-4.png)

### Membuat topologi sederhana di Packet Tracer

{: .box-note}
Di sini saya menggunakan 2 Router 1941, 2 Switch 2960, 1 PC, dan 1 Server.  
Seperti yang dilihat, perangkat PC dan Server disebut **end device**, sedangkan router dan switch disebut **intermedia device**.

![tutorial-cisco-5](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-5.png)

{: .box-note}
Untuk pemasangan kabelnya anda dapat masuk ke menu **connections**, lalu pilih jenis kabelnya.

![tutorial-cisco-6](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-6.png)

### Optimalisasi Packet Tracer

{: .box-note}
Masuk ke menu **Option** > **Preference** (ctrl + r).  
Di menu **interface**, anda dapat memilih apa yang ditampilkan pada tampilan utama.

![tutorial-cisco-7](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-7.png)

{: .box-note}
Di menu **hide**, anda dapat menyembunyikan menu dalam perangkat yang ada dalam packet tracer, contohnya sebagai berikut.

![tutorial-cisco-8](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-8.png)

![tutorial-cisco-9](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-9.png)

{: .box-note}
Di menu **administrative**, anda dapat memasukkan password untuk mengunci topologi agar tidak dapat diubah.

![tutorial-cisco-10](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-10.png)

### Konfigurasi IP Address

![tutorial-cisco-11](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-11.png)

{: .box-note}
Masuk ke **Desktop** > **IP Address** untuk memberi ip pada pc.

![tutorial-cisco-12](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-12.png)

{: .box-note}
Selanjutnya berikan ip pada server, masuk ke tab **Desktop** > **IP Address**.

![tutorial-cisco-13](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-13.png)

{: .box-note}
Berikan ip pada switch melalui **CLI**, anda bisa mengikuti command pada gambar di bawah ini.

![tutorial-cisco-14](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-14.png)

![tutorial-cisco-15](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-15.png)

{: .box-note}
Ping pc hingga 100%.

![tutorial-cisco-16](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-16.png)

![tutorial-cisco-17](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-17.png)

{: .box-note}
Selanjutnya berikan ip juga pada kedua router, anda bisa melakukannya melalui **Config** maupun **CLI** (di sini saya menggunakan mode config).

![tutorial-cisco-18](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-18.png)

![tutorial-cisco-19](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-19.png)

![tutorial-cisco-20](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-20.png)

![tutorial-cisco-21](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-21.png)

{: .box-note}
Anda pun bisa mengkonfigurasi router dan switch menggunakan **console**.

![tutorial-cisco-22](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-22.png)

{: .box-note}
Masukkan **port 232** pada pc dan **port console** pada router/switch untuk konfigurasi router/switch melalui pc, selanjutnya masuk ke **Desktop** > **Terminal** lalu klik ok.

![tutorial-cisco-23](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-23.png)

![tutorial-cisco-24](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-24.png)

### Penyimpanan Konfigurasi dan Topologi

{: .box-note}
Untuk melakukan penyimpanan konfigurasi, anda dapat melakukannya melalui router dan switch, anda bisa mengikuti command pada gambar berikut.

![tutorial-cisco-25](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-25.png)

![tutorial-cisco-26](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-26.png)

{: .box-note}
Ketikkan `reload` lalu **enter** pada keduanya.

![tutorial-cisco-27](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-27.png)

![tutorial-cisco-28](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-28.png)

{: .box-note}
Saat warna arah panah masih orange, anda dapat mempercepatnya menggunakan fitur **fast forward time** (ctrl + d) dengan icon **>>**.

![tutorial-cisco-29](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-29.png)

{: .box-note}
Ketikkan `show ip interface brief` untuk melihat apakah konfigurasi masih tetap.

![tutorial-cisco-30](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-30.png)

![tutorial-cisco-31](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-31.png)

### Pengetesan Clien-Server Mode Realtime dan Simulation

{: .box-note}
Cobalah ping dari pc ke server, apakah gagal? anda dapat menemukan sumber permasalahannya melalui mode **simulation** di sebelah mode **realtime**.

![tutorial-cisco-32](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-32.png)

{: .box-note}
Anda harus menghubungkan kedua router tersebut agar pc dapat terhubung juga pada server.  
Buka **Router**, konfigurasi routing statis melalui cli, anda bisa mengetikkan command berikut.  
`ip route (ip address tujuan) (netmask) (port yang digunakan router. ex:g0/1 atau berbentuk ip)`
Jika sudah, coba lagi ping dari pc ke server.

![tutorial-cisco-33](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-33.png)

![tutorial-cisco-34](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-34.png)

![tutorial-cisco-35](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-35.png)
















