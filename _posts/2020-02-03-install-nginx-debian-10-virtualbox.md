---
layout: post
title: Install NGINX Debian 10 - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-nginx-debian-10-virtualbox/nginx.png
share-img: /assets/img/install-nginx-debian-10-virtualbox/nginx.png
tags: [dns, cisco]
comments: true
---

NGINX (engine-x) adalah web server open-source yang sekarang juga digunakan sebagai reverse proxy, HTTP cache, dan load balancer. NGINX awalnya dibuat oleh Igor Sysoev, dengan dirilis untuk publik pertama kali pada bulan Oktober 2004.  
Selain menawarkan kemampuan server HTTP, NGINX juga dapat beroperasi sebagai server proxy surat IMAP / POP3 serta berfungsi sebagai load balancer dan server cache HTTP.  

## Install NGINX pada Debian 10

{: .box-note}
Masuk dengan mode **super user** pada debian 10 lalu ketikkan `apt install nginx`, lalu tunggu hingga instalasi selesai.

{: .box-note}
Jika sudah selesai, ketikkan `systemctl status nginx` untuk mengecek.

![nginx-deb-1](/assets/img/install-nginx-debian-10-virtualbox/nginx-deb-1.png)

{: .box-note}
Masuk ke web browser, lalu ketikkan ip debian untuk melihat apakah nginx sudah terinstall.

![nginx-deb-2](/assets/img/install-nginx-debian-10-virtualbox/nginx-deb-2.png)

{: .box-note}
Anda juga bisa mengganti teks pada web dengan mengedit file html dari **/var/www/html/index.nginx-debian.html**.

![nginx-deb-3](/assets/img/install-nginx-debian-10-virtualbox/nginx-deb-3.png)
