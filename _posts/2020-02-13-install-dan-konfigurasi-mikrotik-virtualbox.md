---
layout: post
title: Install dan Konfigurasi Mikrotik - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-dan-konfigurasi-mikrotik-virtualbox/mikrotik.png
share-img: /assets/img/install-dan-konfigurasi-mikrotik-virtualbox/mikrotik.png
tags: [install, mikrotik, virtualbox]
comments: true
---

Mikrotik RouterOS adalah sistem operasi Linux base yang diperuntukkan sebagai network router yang instalasinya dapat dilakukan pada Standard komputer PC.  
PC yang akan dijadikan router mikrotik pun tidak memerlukan resource yang cukup besar untuk penggunaan standard, misalnya hanya sebagai gateway.  

Anda bisa mendownload [ISO Mikrotik](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwiklsnO2s3nAhU6zzgGHWfdArkQFjAAegQIAhAB&url=http%3A%2F%2Fwww.routeros.co.id%2F%3Fact%3Dpreview%26versi%3D6.33%26nf%3Dmikrotik-6.33.iso%26key%3D9d8d81f60c61c94c09d78be766c21a76&usg=AOvVaw3cJg-wev7bgJx_5XhVSyp9) terlebih dahulu.

## Install MikroTik

{: .box-note}
Buat file baru pada VirtualBox untuk mikrotik (type & version = other), lalu masukkan file ISO mikrotik > **start**.

![install-mikrotik-1](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-1.png)

{: .box-note}
Klik `a` untuk mencentang semua pilihan, lalu klik `i` untuk install selanjutnya ikuti instruksinya.

![install-mikrotik-2](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-2.png)

{: .box-note}
Setelah selesai, remove file iso mikrotik pada menu **Device** > **Optical drive** > **Remove disk from virtual drive**, lalu klik **Force Unmount** > tekan **enter**.

![install-mikrotik-3](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-3.png)

{: .box-note}
Login dengan **username** = **admin** dan **password** = (kosongkan saja).

![install-mikrotik-4](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-4.png)

## Konfigurasi IP address Mikrotik

{: .box-note}
Buat **host network** untuk mikrotik terlebih dahulu.

![install-mikrotik-5](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-5.png)

{: .box-note}
Buat **adapter 1** menjadi **Bridge Adapter** dan **Adapter 2** menjadi **Host-only Adapter**.

![install-mikrotik-6](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-6.png)

![install-mikrotik-7](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-7.png)

{: .box-note}
Masuk ke mikrotik, lalu ketikkan `interface print` untuk melihat daftar jaringan, dan ketikkan `ip address print` untuk melihat daftar ip address.

![install-mikrotik-8](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-8.png)

{: .box-note}
Anda juga bisa **ping** ip local melalui mikrotik ataupun melalui terminal/cmd.

![install-mikrotik-9](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-9.png)

{: .box-note}
Anda juga bisa mengakses dan melakukan konfigurasi lainnya lewat **winbox**.

![install-mikrotik-10](/assets/img/install-dan-konfigurasi-mikrotik-virtualbox/install-mikrotik-10.png)
