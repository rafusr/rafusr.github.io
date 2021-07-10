---
layout: post
title: Install NGINX Ubuntu Server 18.04 - VirtualBox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx.png
share-img: /assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx.png
tags: [install, nginx, ubuntu, server, virtualbox]
comments: true
---

NGINX (engine-x) adalah web server open-source yang sekarang juga digunakan sebagai reverse proxy, HTTP cache, dan load balancer. NGINX awalnya dibuat oleh Igor Sysoev, dengan dirilis untuk publik pertama kali pada bulan Oktober 2004.  
Selain menawarkan kemampuan server HTTP, NGINX juga dapat beroperasi sebagai server proxy surat IMAP / POP3 serta berfungsi sebagai load balancer dan server cache HTTP.

## Install NGINX Ubuntu Server 18.04

{: .box-note}
Login sebagai **super user**, lalu ketikkan `apt install nginx`, lalu ikuti instruksinya.

![nginx-ubuntu-1](/assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx-ubuntu-1.png)

{: .box-note}
Setelah install selesai, anda dapat mengecek status nginx dengan mengetikkan `systemctl status nginx`.

![nginx-ubuntu-2](/assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx-ubuntu-2.png)

{: .box-note}
Anda bisa membuka pada browser anda dan ketikkan ip ubuntu.

![nginx-ubuntu-3](/assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx-ubuntu-3.png)

{: .box-note}
Anda juga bisa mengedit teks pada web dengan mengedit `nano /var/www/html/index.nginx-debian.html`.

![nginx-ubuntu-4](/assets/img/install-nginx-ubuntu-server-18.04-virtualbox/nginx-ubuntu-4.png)
