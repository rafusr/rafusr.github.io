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
Masukkan **port 232** pada pc dan **port console** pada router/switch untuk konfigurasi router/switch melalui pc, selanjutnya masuk ke **Desktop** > **Terminal** lalu klik ok.

![tutorial-cisco-22](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-22.png)

![tutorial-cisco-23](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-23.png)

### Penyimpanan Konfigurasi dan Topologi

{: .box-note}
Untuk melakukan penyimpanan konfigurasi, anda dapat melakukannya melalui router dan switch, anda bisa mengikuti command pada gambar berikut.

![tutorial-cisco-24](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-24.png)

![tutorial-cisco-25](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-25.png)

{: .box-note}
Ketikkan `reload` lalu **enter** pada keduanya.

![tutorial-cisco-26](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-26.png)

![tutorial-cisco-27](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-27.png)

{: .box-note}
Saat warna arah panah masih orange, anda dapat mempercepatnya menggunakan fitur **fast forward time** (ctrl + d) dengan icon **>>**.

![tutorial-cisco-28](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-28.png)

{: .box-note}
Ketikkan `show ip interface brief` untuk melihat apakah konfigurasi masih tetap.

![tutorial-cisco-29](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-29.png)

![tutorial-cisco-30](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-30.png)

### Pengetesan Clien-Server Mode Realtime dan Simulation

{: .box-note}
Cobalah ping dari pc ke server, apakah gagal? anda dapat menemukan sumber permasalahannya melalui mode **simulation** di sebelah mode **realtime**.

![tutorial-cisco-31](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-31.png)

{: .box-note}
Anda harus menghubungkan kedua router tersebut agar pc dapat terhubung juga pada server.  
Buka **Router**, konfigurasi routing statis melalui cli, anda bisa mengetikkan command berikut.  
`ip route (ip address tujuan) (netmask) (port yang digunakan router. ex:g0/1 atau berbentuk ip)`  
Jika sudah, coba lagi ping dari pc ke server.

![tutorial-cisco-32](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-32.png)

![tutorial-cisco-33](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-33.png)

![tutorial-cisco-34](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-34.png)

### Mode Command Router dan Switch

{: .box-note}
**Mode user**,
mode ini merupakan mode dasar yang akan muncul ketika membuka cli pada router ataupun switch. Untuk melihat command lainnya anda bisa mengetikkan `?` pada mode tersebut.

![tutorial-cisco-35](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-35.png)

{: .box-note}
**Mode privilege**,
dimode ini, anda dapat memverifikasi, konfigurasi, penyimpanan, dll. Anda juga harus menggunakan mode ini untuk memasuki mode selanjutnya (global). Untuk melihat command lainnya anda bisa mengetikkan `?` pada mode tersebut.

![tutorial-cisco-36](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-36.png)

{: .box-note}
**Mode global**,
Mode ini digunakan untuk melakukan konfigurasi pada router/switch. Untuk melihat command lainnya anda bisa mengetikkan `?` pada mode tersebut.

![tutorial-cisco-37](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-37.png)

{: .box-note}
**Mode Context**,
Sebenarnya mode ini hampir sama dengan mode global, hanya saja lebih spesifik. Untuk melihat command lainnya anda bisa mengetikkan `?` pada mode tersebut.

![tutorial-cisco-38](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-38.png)

### Reset Konfigurasi Router

{: .box-note}
Untuk mereset konfigurasi pada router anda dapat menggunakan command `erase startup-config`, setelah itu ketikkan `reload`.

![tutorial-cisco-39](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-39.png)

### Hostname

{: .box-note}
Setelah mereset router, pada menu ini pilih **no**.

![tutorial-cisco-40](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-40.png)

{: .box-note}
Untuk mengubah **hostname** router, anda harus masuk terlebih dahulu ke **mode global** lalu ketikkan `hostname (nama hostname)`.

![tutorial-cisco-41](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-41.png)

### Enable Password dan Enable Secret

{: .box-note}
Untuk memberikan password pada **mode privilege**, anda bisa mengetikkan command `enable password (password anda)`.

![tutorial-cisco-42](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-42.png)

{: .box-note}
Untuk mengetesnya anda dapat kembali ke mode user lalu masuk lagi ke mode privilege.

![tutorial-cisco-43](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-43.png)

{: .box-note}
Untuk mengunci **mode privilege** menggunakan **secret**, anda bisa mengetikkan `enable secret (password anda)`.

![tutorial-cisco-44](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-44.png)

{: .box-note}
Lalu coba tes dengan **relog** pada **mode privilege**, di sini anda sudah tidak dapat menggunakan password biasa, yang digunakan sebagai password adalah **secret**.

![tutorial-cisco-45](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-45.png)

### Line Console

{: .box-note}
Anda bisa memberikan password pada **console**, agar client perlu mengetahui password untuk bisa konfigurasi melalui **console**. Anda bisa mengikuti command pada gambar di bawah ini.

![tutorial-cisco-46](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-46.png)

{: .box-note}
Setelah itu coba konfigurasi router melalui client. Masuk ke menu **Desktop** > **Terminal** lalu klik **ok**.

![tutorial-cisco-47](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-47.png)

### Interface Setting

{: .box-note}
Anda bisa konfigurasi ulang IP Address pada masing masing port yang terhubung pada router.

![tutorial-cisco-48](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-48.png)

{: .box-note}
Anda juga bisa memberikan deskripsi pada masing masing port.

![tutorial-cisco-49](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-49.png)

{: .box-note}
Anda bisa mengetikkan `do show run` lalu scroll dengan klik enter sampai anda melihat konfigurasi ip pada masing masing port beserta deskripsinya.

![tutorial-cisco-50](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-50.png)

### Telnet

{: .box-note}
Untuk melakukan remote management anda dapat menggunakan **telnet**.  
**Line vty** adalah virtual interface untuk melakukan remote via network.

![tutorial-cisco-51](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-51.png)

{: .box-note}
Coba akses telnet melalui client, masuk ke tab **Desktop** > **Command prompt** lalu ketikkan `telnet (IP Address router)`.

![tutorial-cisco-52](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-52.png)

### SSH

{: .box-note}
Selain menggunakan **telnet**, anda juga bisa menggunakan **SSH** sebagai remote via network.

![tutorial-cisco-53](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-53.png)

![tutorial-cisco-54](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-54.png)

{: .box-note}
Selanjutnya coba masuk menggunakan **SSH** dari client dengan mengetikkan `ssh -l (username) (ip router)` lalu masukkan password tadi.

![tutorial-cisco-55](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-55.png)

### Banner

{: .box-note}
**Banner** di sini berfungsi sebagai peringatan ketika ada yang mengakses perangkat.

![tutorial-cisco-56](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-56.png)

{: .box-note}
**Authorized users only. Access prohibited** adalah peringatan yang akan dimunculkan, anda bisa menggantinya dengan yang lain.  
Untuk mengeceknya coba masuk melalui telnet pada client.

![tutorial-cisco-57](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-57.png)

### Enkripsi Password

{: .box-note}
Terdapat beberapa level password pada cisco.
- Level 0 : Aktual (tidak dienkripsi)
- Level 5 : MD5
- Level 7 : Cisco

![tutorial-cisco-58](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-58.png)

{: .box-note}
Anda juga bisa mengubah password **aktual** menjadi **enkripsi**, ketikkan `Service password-encryption` lalu cek lagi apakah password tadi telah dienkripsi.

![tutorial-cisco-59](/assets/img/tutorial-cisco-packet-tracer/tutorial-cisco-59.png)
