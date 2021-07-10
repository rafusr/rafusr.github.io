---
layout: post
title: install-nginx-centos-7-virtualbox
subtitle: 
cover-img: 
thumbnail-img: /assets/img/install-nginx-centos-7-virtualbox/nginx.png
share-img: /assets/img/install-nginx-centos-7-virtualbox/nginx.png
tags: [install, nginx, centos, virtualbox]
comments: true
---

NGINX (engine-x) adalah web server open-source yang sekarang juga digunakan sebagai reverse proxy, HTTP cache, dan load balancer. NGINX awalnya dibuat oleh Igor Sysoev, dengan dirilis untuk publik pertama kali pada bulan Oktober 2004.  
Selain menawarkan kemampuan server HTTP, NGINX juga dapat beroperasi sebagai server proxy surat IMAP / POP3 serta berfungsi sebagai load balancer dan server cache HTTP.

## Install NGINX CentOS 7

{: .box-note}
Masuk sebagai root pada centos 7

[nginx-centos-1](/assets/img/install-nginx-centos-7-virtualbox/nginx-centos-1.png)

{: .box-note}
Tambahkan **repository** untuk nginx dengan mengetikkan `yum install epel-release`, setelah selesai anda bisa mulai install nginx dengan mengetikkan `yum install nginx`.

[nginx-centos-2](/assets/img/install-nginx-centos-7-virtualbox/nginx-centos-2.png)

{: .box-note}
Aktifkan nginx dengan mengetikkan `systemctl start nginx`, dan untuk melihat statusnya anda dapat mengetikkan `systemctl status nginx`.

[nginx-centos-3](/assets/img/install-nginx-centos-7-virtualbox/nginx-centos-3.png)

{: .box-note}
Lalu buka browser anda dan ketikkan ip centos.

[nginx-centos-4](/assets/img/install-nginx-centos-7-virtualbox/nginx-centos-4.png)

{: .box-note}
Jika masih belum bisa, anda bisa mencoba untuk mengetikkan command di bawah ini.  

`firewall-cmd --permanent --zone=public --add-service=http`  

`firewall-cmd --permanent --zone=public --add-service=https`  

`firewall-cmd --reload`  

{: .box-note}
Anda juga bisa mengganti teks pada website dengan mengedit file pada index.html, ketikkan `nano /usr/share/nginx/html/index.html`.

[nginx-centos-5](/assets/img/install-nginx-centos-7-virtualbox/nginx-centos-5.png)
