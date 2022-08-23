---
title: "4.3 การแปลงแหล่งจ่าย"
description: "Doks is a Hugo theme for building secure, fast, and SEO-ready documentation websites, which you can easily update and customize."
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "chapter4"
weight: 430
toc: true
---

การแปลงแหล่งจ่ายเป็นอีกเครื่องมือช่วยให้การคำนวณหาค่าต่างๆง่ายขึ้น
การแปลงแหล่งจ่ายมีสองแบบคือ

1. การแปลงจากแหล่งจ่ายกระแสเป็นแหล่งจ่ายแรงดัน
2. การแปลงจากแหล่งจ่ายแรงดันเป็นแหล่งจ่ายกระแส
  
## หลักการแปลงแหล่งจ่าย

{{< admonition warning >}}
การแปลงแหล่งจ่ายคือการแทนแหล่งจ่ายแรงดัน $v_s$ ที่ต่ออนุกรมกับตัวต้านทาน $R$ ให้เป็นแหล่งจ่ายกระแส $i_s$ ที่ต่อขนานกับตัวต้านทาน $R$
{{< /admonition >}}


<figure>
<p align="center">
  <img src="fig4.8.png" alt="fig 4.8" style="width:100%">
</p>
  <figcaption style='text-align:center'>รูปที่ 4.8 การแปลงแหล่งจ่าย
</figcaption>
</figure>

โดยที่ $v_s$ และ $i_s$ มีความสัมพันธ์ตามกฏของโอห์มดังนี้
$$
\begin{equation*}
    v_s=i_sR \quad \text{หรือ} \quad i_s=\dfrac{v_s}{R}
\end{equation*}
$$

## ข้อระวังเมื่อทำการแปลงแหล่งจ่าย

{{< admonition tip>}}
1. ทิศหัวลูกศรของแหล่งจ่ายกระแสชี้ไปยังขั้วบวกของแหล่งจ่ายแรงดัน
2. การแปลงแหล่งจ่ายแรงดันเป็นแหล่งจ่ายกระแสไม่สามารถทำได้ ถ้าตัวต้านทาน $R=0$
3. การแปลงแหล่งจ่ายกระแสเป็นแหล่งจ่ายแรงดันไม่สามารถทำได้ถ้าตัวต้านทาน $R=\infty$
{{< /admonition >}}

## ตัวอย่าง 4.4 ##
{{<admonition abstract "ตัวอย่าง 4.4" false>}}
จงใช้การแปลงแหล่งจ่าย หาแรงดัน $v_o$

<figure>
<p align="center">
  <img src="fig4.9.png" alt="fig 4.9" style="width:100%">
</p>
  <figcaption style='text-align:center'>รูปที่ 4.9 วงจรสำหรับตัวอย่าง 4.4
</figcaption>
</figure>

คำตอบ 

แปลงแหล่งจ่ายดังนี้

<figure>
<p align="center">
  <img src="fig4.10.png" alt="fig 4.10" style="width:100%">
</p>
  <figcaption style='text-align:center'>รูปที่ 4.10 </figcaption>
</figure>


<figure>
<p align="center">
  <img src="fig4.11.png" alt="fig 4.11" style="width:100%">
</p>
  <figcaption style='text-align:center'>รูปที่ 4.11 </figcaption>
</figure>

ในรูปที่ 4.11(a) แหล่งจ่ายกระแสสองตัวรวมกันได้เนื่องจากไม่มีอุปกรณ์ไฟฟ้าตัวอื่นมาคั่น กลาง

{{% notice warning %}}
แหล่งจ่ายกระแสรวมกันไม่ได้ถ้ามีอุปกรณ์ไฟฟ้าตัวอื่นต่อคั่นอยู่ระหว่างแหล่งจ่ายกระแส
{{% /notice %}}

จากรูปที่ 4.11(b) ใช้กฏแบ่งกระแส
$$
    \begin{align*}
                i&=\left(\frac{2}{2+8}\right)2=0.4\mathrm{A}\nonumber\\\\
                v_o&=8i=8(0.4)=3.2\mathrm{V}\notag\\\\ \text{หรือ}\qquad \qquad  \nonumber \\\\ 
                v_o&=(8 || 2)(2\mathrm{A})=\frac{8\times2}{10}(2)=3.2\mathrm{V}\nonumber
    \end{align*}
$$
{{</admonition>}}
