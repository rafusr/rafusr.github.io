---
layout: post
title: Konfigurasi File Server SAMBA Ubuntu Server 18.04
subtitle: 
cover-img: 
thumbnail-img: /assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/file-server.png
share-img: /assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/file-server.png
tags: [tutorial, file, server, samba, ubuntu]
comments: true
---

File Server adalah sebuah komputer terpasang ke jaringan yang memiliki tujuan utama memberikan lokasi untuk akses disk bersama , yaitu penyimpanan bersama file komputer yang dapat diakses oleh workstation yang melekat pada jaringan komputer.  

## Install SAMBA Ubuntu Server 18.04

{: .box-note}
Install **tasksel**, lalu install **SAMBA** dengan **tasksel**.  
`apt install tasksel`  
`tasksel install samba-server `

![samba-ubuntu-1](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-1.png)

## Konfigurasi SAMBA Ubuntu Server 18.04

{: .box-note}
Buat username dan password dengan mengetikkan `smbpasswd -a (username)`.

![samba-ubuntu-2](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-2.png)

{: .box-note}
Edit file pada **/etc/samba/smb.conf**, tambahkan direktori untuk public.

![samba-ubuntu-3](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-3.png)

{: .box-note}
Buat direktori public pada ubuntu, ketikkan  
`mkdir /var/samba/`  
`chmod 777 /var/samba`

![samba-ubuntu-4](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-4.png)

{: .box-note}
Ketikkan **testparm** untuk mengecek apakah konfigurasi sudah benar.

![samba-ubuntu-5](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-5.png)

{: .box-note}
Restart **SAMBA** dengan mengetikkan `service smbd restart` dan `service smbd status` untuk melihat status **SAMBA**.

![samba-ubuntu-6](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-6.png)

{: .box-note}
Selanjutnya coba masuk dengan client ke samba dengan mengetikkan `smb://(ip address ubuntu)`.

![samba-ubuntu-7](/assets/img/konfigurasi-file-server-samba-ubuntu-server-18.04/samba-ubuntu-7.png)
