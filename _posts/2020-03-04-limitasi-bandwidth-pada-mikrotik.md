---
layout: post
title: Limitasi Bandwidth pada Mikrotik
subtitle: 
cover-img: 
thumbnail-img: /assets/img/limitasi-bandwidth-pada-mikrotik/mikrotik.png
share-img: /assets/img/limitasi-bandwidth-pada-mikrotik/mikrotik.png
tags: [tutorial, bandwidth, mikrotik, virtualbox]
comments: true
---

Mikrotik RouterOS adalah sistem operasi Linux base yang diperuntukkan sebagai network router yang instalasinya dapat dilakukan pada Standard komputer PC.  
PC yang akan dijadikan router mikrotik pun tidak memerlukan resource yang cukup besar untuk penggunaan standard, misalnya hanya sebagai gateway.  
  
Bandwidth adalah maksimal besar transfer yang dapat dilakukan pada satu waktu dalam pertukaran data.  

##   Limitasi Bandwidth Mikrotik

{: .box-note}
Masuk ke winbox lalu masuk ke menu **queue** > klik icon **+** pada menu **simple queue**. Anda bisa memasukkan IP address/interface yang akan dilimit bandwidth nya (disini saya memerikan limit bandwidth pada **interface bridge1**), untuk melimit kecepatan upload dan download anda dapat mengubah **max.limit** pada **target upload** dan **target download**.

![bandwidth-mikrotik-1](/assets/img/limitasi-bandwidth-pada-mikrotik/bandwidth-mikrotik-1.png)

![bandwidth-mikrotik-1](/assets/img/limitasi-bandwidth-pada-mikrotik/bandwidth-mikrotik-2.png)

{: .box-note}
Setelah selesai coba tes kecepatan internet pada clien.

![bandwidth-mikrotik-1](/assets/img/limitasi-bandwidth-pada-mikrotik/bandwidth-mikrotik-3.png)

![bandwidth-mikrotik-4](/assets/img/limitasi-bandwidth-pada-mikrotik/bandwidth-mikrotik-4.png)
