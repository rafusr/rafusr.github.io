---
layout: post
title: Tutorial GNS3
subtitle: 
cover-img: 
thumbnail-img: /assets/img/tutorial-gns3/gns3.png
share-img: /assets/img/tutorial-gns3/gns3.png
tags: [tutorial, gns3]
comments: true
---

GNS3 (Graphic Simulator Network) adalah aplikasi simulator jaringan berbasis GUI yang di rilis pada tahun 2008. Dengan GNS3 kita bisa mensimulasikan perangkat asli baik dengan bantuan emulator ataupun teknologi virtualisasi. Salah satu teknologi emulator yaitu dynamips, yang digunakan untuk mensimulasikan Cisco IOS.  

### Workspace GNS3

![tutorial-gns3-1](/assets/img/tutorial-gns3/tutorial-gns3-1.png)

### Toolbar pada GNS3

{: .box-note}
Anda dapat menyimpan/membuka file pada gns3, atau mengontrol view pada tampilan, dll.

![tutorial-gns3-2](/assets/img/tutorial-gns3/tutorial-gns3-2.png)

{: .box-note}
Di menu ini anda dapat mengontrol projek anda.

![tutorial-gns3-3](/assets/img/tutorial-gns3/tutorial-gns3-3.png)

{: .box-note}
Terdapat berbagai pilihan device yang cocok untuk projek anda.

![tutorial-gns3-4](/assets/img/tutorial-gns3/tutorial-gns3-4.png)

### Pembuatan Topologi GNS3

{: .box-note}
Pertama, buat projek baru pada gns3 bisa melalui **file** > **new blank project**,
Diperlukan router pada topology ini, maka anda harus mendownload filenya terlebih dahulu, anda bisa mendownloadnya [disini](https://semawur.com/3zkPJOA0).

{: .box-note}
Selanjutnya masuk ke menu **edit** > **preference** > **Dynamips** > **IOS routers**, masukkan file tadi lalu ikuti saja langkah selanjutnya > apply > ok.

![tutorial-gns3-5](/assets/img/tutorial-gns3/tutorial-gns3-5.png)

{: .box-note}
Buat topologi menggunakan 2 router, 2 ethernet switch, dan 2 vpcs.

![tutorial-gns3-6](/assets/img/tutorial-gns3/tutorial-gns3-6.png)

{: .box-note}
Tambahkan kabel.

![tutorial-gns3-7](/assets/img/tutorial-gns3/tutorial-gns3-7.png)

![tutorial-gns3-8](/assets/img/tutorial-gns3/tutorial-gns3-8.png)

### Setting Idle-PC

{: .box-note}
Klik **start** lalu tunggu hingga semua kabel berwarna hijau.

![tutorial-gns3-9](/assets/img/tutorial-gns3/tutorial-gns3-9.png)

{: .box-note}
Selanjutnya pilih router r1 lalu klik kanan > pilih **idle pc** lalu pilih yang terdapat icon *****.

![tutorial-gns3-10](/assets/img/tutorial-gns3/tutorial-gns3-10.png)

### Konfigurasi IP Address Device

{: .box-note}
Klik kanan pada router lalu pilih **console**.

![tutorial-gns3-11](/assets/img/tutorial-gns3/tutorial-gns3-11.png)

{: .box-note}
Berikan ip pada masing masing port di router.

![tutorial-gns3-12](/assets/img/tutorial-gns3/tutorial-gns3-12.png)

{: .box-note}
Ketikkan `do show ip interface brief` dan lihat apakah ip sudah berada pada port yang benar.

![tutorial-gns3-13](/assets/img/tutorial-gns3/tutorial-gns3-13.png)

![tutorial-gns3-14](/assets/img/tutorial-gns3/tutorial-gns3-14.png)

{: .box-note}
Berikan ip pada pc dengan mengetikkan `ip (IP Address) (netmask) (gateway)`, lalu ketikkan `save` untuk menyimpan.  
Ping gateway untuk memastikan apakah sudah terkoneksi.

![tutorial-gns3-15](/assets/img/tutorial-gns3/tutorial-gns3-15.png)

![tutorial-gns3-16](/assets/img/tutorial-gns3/tutorial-gns3-16.png)

{: .box-note}
Lakukan **routing** pada router, lalu coba ping ip pc2 dari pc1 dan juga sebaliknya.

![tutorial-gns3-17](/assets/img/tutorial-gns3/tutorial-gns3-17.png)

![tutorial-gns3-18](/assets/img/tutorial-gns3/tutorial-gns3-18.png)

![tutorial-gns3-19](/assets/img/tutorial-gns3/tutorial-gns3-19.png)

![tutorial-gns3-20](/assets/img/tutorial-gns3/tutorial-gns3-20.png)
