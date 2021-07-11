---
layout: post
title: Tutorial EVE-NG
subtitle: 
cover-img: 
thumbnail-img: /assets/img/tutorial-eve-ng/eve-ng.png
share-img: /assets/img/tutorial-eve-ng/eve-ng.png
tags: [tutorial, eve-ng]
comments: true
---

EVE-NG (Emulated Virtual Environment Next Generation) adalah perangkat lunak virtualisasi yang mendukung berbagai perangkat jaringan dan operasi system untuk melakukan simulasi jaringan atau server dengan nyata, dan emulator jaringan grafis yang mendukung gambar router komersial. Eve-ng merupakan versi terbaru dari Unetlab yang merupakan emulator jaringan versi stabil pada saat ini.
Emulator jaringan unetlab atau eve-ng berjalan di mesin virtual sehingga dapat diatur pada komputer windows, mac os, atau linux. Antar muka pengguna grafis berjalan di browser web. Pengguna dapat membuat topologi jaringan dari pustaka eve-ng, menghubungkan bersama dan mengkonfigurasikanya.  

### Pembuatan Topologi

{: .box-note}
Klik icon **+** pada menu kiri eve-ng lalu pilih **node**, cari **Cisco IOL** lalu buat 2 router.

![tutorial-eve-ng-1](/assets/img/tutorial-eve-ng/tutorial-eve-ng-1.png)

![tutorial-eve-ng-2](/assets/img/tutorial-eve-ng/tutorial-eve-ng-2.png)

{: .box-note}
Selanjutnya buat 2 switch.

![tutorial-eve-ng-3](/assets/img/tutorial-eve-ng/tutorial-eve-ng-3.png)

![tutorial-eve-ng-4](/assets/img/tutorial-eve-ng/tutorial-eve-ng-4.png)

{: .box-note}
Buat 2 VPC juga.

![tutorial-eve-ng-5](/assets/img/tutorial-eve-ng/tutorial-eve-ng-5.png)

![tutorial-eve-ng-6](/assets/img/tutorial-eve-ng/tutorial-eve-ng-6.png)

![tutorial-eve-ng-7](/assets/img/tutorial-eve-ng/tutorial-eve-ng-7.png)

{: .box-note}
Berikan kabel pada masing masing perangkat dengan mengklik icon kabel berwarna orange pada perangkat, tahan lalu arahkan ke perangkat yang lain.

![tutorial-eve-ng-8](/assets/img/tutorial-eve-ng/tutorial-eve-ng-8.png)

### Konfigurasi IP Address Device

{: .box-note}
Start terlebih dahulu semua perangkat, **More Actions** > **Start all nodes**, lalu tunggu hingga berwarna biru.

![tutorial-eve-ng-9](/assets/img/tutorial-eve-ng/tutorial-eve-ng-9.png)

![tutorial-eve-ng-10](/assets/img/tutorial-eve-ng/tutorial-eve-ng-10.png)

{: .box-note}
Klik pada router lalu klik pada menu popup pada web browser, pilih **no** pada **Would you like to enter the initial configuration dialog**.

![tutorial-eve-ng-11](/assets/img/tutorial-eve-ng/tutorial-eve-ng-11.png)

{: .box-note}
Berikan ip pada masing masing router.

![tutorial-eve-ng-12](/assets/img/tutorial-eve-ng/tutorial-eve-ng-12.png)

![tutorial-eve-ng-13](/assets/img/tutorial-eve-ng/tutorial-eve-ng-13.png)

{: .box-note}
Sekarang berikanlah ip static pada kedua pc.

![tutorial-eve-ng-14](/assets/img/tutorial-eve-ng/tutorial-eve-ng-14.png)

![tutorial-eve-ng-15](/assets/img/tutorial-eve-ng/tutorial-eve-ng-15.png)

{: .box-note}
Coba ping dari pc1 ke pc2, juga sebaliknya.

![tutorial-eve-ng-16](/assets/img/tutorial-eve-ng/tutorial-eve-ng-16.png)

{: .box-note}
Anda harus melakukan **routing** pada setiap router untuk bisa menghubungkan pc1 dan pc2, lalu coba ping lagi.

![tutorial-eve-ng-17](/assets/img/tutorial-eve-ng/tutorial-eve-ng-17.png)

![tutorial-eve-ng-18](/assets/img/tutorial-eve-ng/tutorial-eve-ng-18.png)
