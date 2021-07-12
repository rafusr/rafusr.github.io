---
layout: post
title: Konfigurasi File Server SAMBA CentOS 8
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-file-server-samba-centos-8/file-server.png
share-img: /assets/img/konfigurasi-file-server-samba-centos-8/file-server.png
tags: [tutorial, file, server, samba, centos]
comments: true
---

File Server adalah sebuah komputer terpasang ke jaringan yang memiliki tujuan utama memberikan lokasi untuk akses disk bersama , yaitu penyimpanan bersama file komputer yang dapat diakses oleh workstation yang melekat pada jaringan komputer.  

## Install SAMBA CentOS 8

{: .box-note}
Login sebagai **super user**, lalu install samba dengan mengetikkan `dnf install samba samba-common samba-client`.

![samba-centos-1](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-1.png)

{: .box-note}
Buat folder khusus untuk share.

![samba-centos-2](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-2.png)

## Konfigurasi SAMBA CentOS 8

{: .box-note}
Edit file pada **/etc/samba/smb.conf**.

![samba-centos-3](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-3.png)

{: .box-note}
Ketikkan `testparm` untuk mengecek apakah konfigurasi sudah benar.

![samba-centos-4](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-4.png)

{: .box-note}
Berikan akses **firewall** untuk **SAMBA**.

![samba-centos-5](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-5.png)

{: .box-note}
Untuk memulai dan melihat status **SAMBA**, anda bisa mengetikkan  
`systemctl start smb`  
`systemctl enable smb`  
`systemctl status smb`

![samba-centos-6](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-6.png)

{: .box-note}
Untuk mengakses file server, anda bisa mengaksesnya melalui menu network, lalu ketikkan  
`smb://(hostname dari samba server)` atau `smb://(ip address dari samba server)`.

![samba-centos-7](/assets/img/konfigurasi-file-server-samba-centos-8/samba-centos-7.png)
