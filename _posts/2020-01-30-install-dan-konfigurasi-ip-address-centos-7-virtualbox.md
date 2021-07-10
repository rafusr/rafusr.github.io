---
layout: post
title: Install dan Konfigurasi IP Address CentOS 7 - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/cent_7.png
share-img: /assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/cent_7.png
tags: [install, centos, virtualbox]
comments: true
---

CentOS (Community Enterprise Operating System) adalah sebuah distribusi linux sebagai bentuk dari usaha untuk menyediakan platform komputasi berkelas enterprise yang memiliki kompatibilitas kode biner sepenuhnya dengan kode sumber yang menjadi induknya, Red Hat Enterprise Linux (RHEL).  
  
Anda bisa mendownload [ISO CentOS](http://kartolo.sby.datautama.net.id/Centos/7/isos/x86_64/CentOS-7-x86_64-Minimal-1810.iso) terlebih dahulu.  

## Install CentOS 7 Di VirtualBox

{: .box-note}
Buat File baru untuk CentOS 7 di VirtualBox, Anda bisa ikuti langkah di bawah ini.

![install-centos-1](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-1.png)

![install-centos-2](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-2.png)

![install-centos-3](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-3.png)

![install-centos-4](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-4.png)

![install-centos-5](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-5.png)

![install-centos-6](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-6.png)

{: .box-note}
Setelah selesai, klik **start** lalu masukkan file ISO CentOS 7 yang telah didownload lalu klik **start**.

![install-centos-7](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-7.png)

{: .box-note}
Pilih bahasa lalu klik **Continue**.

![install-centos-8](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-8.png)

{: .box-note}
Pilih **DATE & TIME** untuk mengatur zona waktu.

![install-centos-9](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-9.png)

{: .box-note}
Pilih zona waktu lalu klik **Done**.

![install-centos-10](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-10.png)

{: .box-note}
Selanjutnya pilih **INSTALLATION DESTINATION**.

![install-centos-11](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-11.png)

{: .box-note}
Atur menjadi otomatis lalu klik **Done**.

![install-centos-12](/assets/img//assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-12.png)

{: .box-note}
Setelah selesai, klik **Begin Installation**.

{: .box-note}
Selanjutnya atur password dan pengguna.

![install-centos-13](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-13.png)

![install-centos-14](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-14.png)

![install-centos-15](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-15.png)

{: .box-note}
Tunggu hingga proses selesai, setelah itu klik **Reboot**.

![install-centos-16](/assets/img//assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-16.png)

![install-centos-17](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-17.png)

![install-centos-18](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-18.png)

  

## Konfigurasi IP Address pada CentOS 7

{: .box-note}
Buat host network terlebih dahulu di menu **file** > **host network manager** atau dengan mengetik ctrl+h.

![install-centos-19](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-19.png)

{: .box-note}
Selanjutnya login ke CentOS dalam mode **super user**, lalu ubah hostname dengan mengetikkan `hostnamectl set-hostname (nama hostname)`, untuk melihat daftar hostname anda bisa mengetikkan `hostname`.

![install-centos-20](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-20.png)

{: .box-note}
Setelah selesai, masuk ke direktori **/etc/sysconfig** dengan mengetikkan `cd /etc/sysconfig`, lalu ketik `ls` untuk melihat daftar, selanjutnya masuk ke network scripts dengan mengetikkan `cd network-scripts`, ketik `ls` lagi untuk melihat daftar.

![install-centos-21](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-21.png)

{: .box-note}
Masuk ke **ifcfg-enp0s3** dengan mengetikkan `vi ifcfg-enp0s3`, setting sesuai gambar, untuk masuk ke mode edit tekan `i`, dan untuk keluar dari mode edit tekan **ctrl+c** lalu ketik `:wq` untuk **save and exit** dan ketik `:q!` untuk **discard change and exit**.

![install-centos-23](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-22.png)

{: .box-note}
Setelah selesai, restart dengan mengetikkan `systemctl network restart`, lalu ketik `ip a` untuk melihat apakah ip berhasil dikonfigurasi.

![install-centos-23](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-23.png)

{: .box-note}
Untuk mengetes anda dapat ping ip tersebut lewat CentOS ataupun terminal/cmd.

![install-centos-24](/assets/img/install-dan-konfigurasi-ip-address-centos-7-virtualbox/install-centos-24.png)
