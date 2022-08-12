---
title: "1.2 ประจุ และ กระแสไฟฟ้า"
description: "Doks is a Hugo theme for building secure, fast, and SEO-ready documentation websites, which you can easily update and customize."
lead: " "
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "chapter1"
weight: 120
toc: true
---

## ประจุ

ประจุเป็นคุณสมบัติพื้นฐานของวัสดุมีหน่วยวัดเป็นคูลอมบ์ (C) อย่างที่ทราบกันดีว่าสสารทุกชนิดประกอบด้วยอะตอม ขณะที่อะตอมประกอบด้วยนิวตรอน โปรตรอนและอิเลคตรอน ซึ่งนิวตรอนไม่มีประจุ ขณะที่โปรตรอนมีประจุเป็นบวกส่วนอิเลคตรอนมีประจุเป็นลบ ขนาดของประจุของอิเลคตรอนคือ $1.602\times 10^{-19}$ C 

### ข้อสำคัญเกี่ยวกับประจุไฟฟ้า
1. ประจุขนาด 1 คูลอมบ์เป็นขนาดที่ใหญ่มาก โดยทั่วไปค่าที่พบเจอจะเป็นขนาด pC, nC, $\mu$C
1. ประจุที่พบจะมีขนาดเป็นจำนวนเท่าของประจุของอิเลคตรอน

1. กฏอนุรักษ์ประจุกล่าว ประจุไม่สามารถถูกทำลาย หรือ สร้างขึ้นใหม่ได้ แต่สามารถถ่ายโอนได้

## กระแส

ในปัจจุบันเราทราบแล้วว่าโปรตรอนเคลื่อนที่ไม่ได้แต่อิเลคตรอนเคลื่อนที่ได้ แต่ในอดีตเมื่อเริ่มค้นพบปรากฏการณ์ใหม่ๆ นักวิทยาศาสตร์คิดว่าเป็นประจุบวกที่เคลื่อนที่ได้ แต่เมื่อภายหลังทราบความจริงแล้ว แต่เรายังก็กำหนดให้ประจุบวกเคลื่อนที่ได้ ดังนั้นทิศการเคลื่อนทีของกระแสจึงตรงกันข้ามกับทิศของอิเลคตรอน

{{< alert icon="👉" context="info" text="นิยาม" />}}

กระแสไฟฟ้าคืออัตราการเคลื่อนที่ของประจุสุทธิต่อหน่วยเวลา 
$$
  \begin{equation}
    i\equiv \frac{dq}{dt} 
  \end{equation}
$$

{{< alert icon="👉" text="  ทิศการเคลื่อนที่ของกระแสตรงกันข้ามกับทิศการเคลื่อนที่ของอิเลคตรอน" />}}

## ความสัมพันธ์ของประจุกับกระแสไฟฟ้า

ถ้าเราทราบขนาดกระแส (ซึ่งมีหน่วยวัดเป็นแอมแปร์) เราสามารถหาปริมาณประจุที่เคลื่อนที่ผ่านในช่วงเวลา $t_o$ ถึง $t_1$ ได้ดังนี้
$$
  \begin{equation}
     Q=\int_{t_{0}}^{t_{1}}i \, dt
  \end{equation}
$$

{{< details "<span class=\"fw-bold\">ขนาดของประจุของอิเลคตรอนคือ</span>" >}}
$1.602\times 10^{-19}$ C 
{{< /details >}}

## ประเภทของกระแสไฟฟ้า

  1. ไฟกระแสตรง เป็นกระแสไฟที่มีขนาดคงที่ตลอดเวลา
  1. ไฟกระแสสลับ เป็นกระแสไฟที่มีขนาดเปลี่ยนแปลงตามเวลา ซึ่งการเปลี่ยนแปลงจะเป็นฟังก์ชันตระกูลซายน์

DC current  |  AC current
:-------------------------:|:-------------------------:
![](fig-dc.png)  |  ![](fig-ac.png)
รูปที่ ๑ ไฟตรง      |  ไฟสลับ

Step-by-step instructions on how to start a new Doks project. [Tutorial →](https://getdoks.org/tutorial/introduction/)

### Quick Start

{{< alert icon="👉" text="The Quick Start is intended for intermediate to advanced users." />}}


## Go further

Recipes, Reference Guides, Extensions, and Showcase.

### Recipes

Get instructions on how to accomplish common tasks with Doks. [Recipes →](https://getdoks.org/docs/recipes/project-configuration/)

### Reference Guides

Learn how to customize Doks to fully make it your own. [Reference Guides →](https://getdoks.org/docs/reference-guides/security/)

### Extensions

Get instructions on how to add even more to Doks. [Extensions →](https://getdoks.org/docs/extensions/breadcrumb-navigation/)

### Showcase

See what others have build with Doks. [Showcase →](https://getdoks.org/showcase/electric-blocks/)

## Contributing

Find out how to contribute to Doks. [Contributing →](https://getdoks.org/docs/contributing/how-to-contribute/)

## Help

Get help on Doks. [Help →]({{< relref "how-to-update" >}})
