---
title: "1.3 แรงดันไฟฟ้า"
description: "Doks is a Hugo theme for building secure, fast, and SEO-ready documentation websites, which you can easily update and customize."
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "chapter1"
weight: 130
toc: true
---

อิเลคตรอนเคลื่อนที่ได้ต้องมีพลังงานกระทำต่อมัน พลังงานดังกล่าวได้มาจากแหล่งจ่ายภายนอก อาทิเช่น แบตเตอรี ซึ่งแบตเตอรี จะสร้าง แรงดัน ในการผลักอิเลคตรอนให้เคลื่อนที่ แรงดันอาจเรียกอีกอย่างว่าความต่างศักย์ ซึ่งเป็นการวัดผลต่างแรงดันระหว่างสองจุด

{{< admonition >}}
นิยาม 1.2
แรงดัน $v_{ab}$ ระหว่างจุด $a$ และ  $b$ คือพลังงานที่ต้องใช้ในการเคลื่อนประจุหน่วย จากจุด $b$ ไป  $a$ ซึ่งแสดงได้ดังสมการ
$$
  \\begin{equation}
    v_{ab}\\equiv \\frac{dw}{dq}
  \\end{equation}
$$
$w$ เป็นพลังงาน หน่วย จูล ($J$) $q$ คือประจุ หน่วย คูลอมบ์ (C)  

{{< /admonition >}}

## เครื่องหมายแรงดัน

การกำหนดเครื่องหมายแรงดันมีผลต่อทิศการไหลของกระแส โดยที่กระแสไหลจากแรงดันศักย์สูง (แรงดันมีเครื่องหมายบวก) ไปแรงดันศักย์ต่ำ (แรงดันมีเครื่องหมายลบ) เสมอ

- กำหนดให้ วงจรมีจุด a และ b ตามรูป ถ้าแรงดันที่จุด a มากกว่า แรงดันที่ b แรงดัน $V_{ab}$ มีค่าเป็นบวก 
- ในทางกลับกัน ถ้าแรงดันที่จุด a มีค่าน้อยกว่า แรงดันที่จุด b แรงดัน $V_{ab}$ มีค่าเป็นลบ 

<img src="fig1.3.png" alt="fig 1.3" width="500" align="center"/>

### สมการแสดงความสัมพันธ์ระหว่างแรงดันสองจุด

ถ้า กำหนดให้จุด a มีแรงดัน $v_{a}$ และ จุด b มีแรงดัน $v_{b}$ ความต่างศักย์ระหว่างจุด a และ จุด b คือ $v_{ab}$ มีความสัมพันธ์ดังนี้

$$
\\begin{equation}
    v_{ab} = v_{a} - v_{b} 
\\end{equation}
$$
ถ้า ต้องการหา $v_{ba}$ ซึ่งเป็นความต่างศักย์ระหว่าง จุด b และ จุด a
$$
\\begin{equation}
    v_{ba} = v_{b} - v_{a} 
\\end{equation}
$$

### $v_{ab}$ มีความสัมพันธ์อย่างไรกับ $v_{ba}$
$$
\\begin{equation}
    v_{ba} = -v_{ab} 
\\end{equation}
$$

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
