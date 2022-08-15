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


## ทิศของกระแสไฟฟ้า

การบอกทิศของกระแสไฟฟ้าสามารถบอกได้โดยใช้ทิศของหัวลูกศร

<img src="fig1.2.png" alt="fig 1.2" width="500" align="center"/>


ตัวอย่าง 1.1 จงคำนวณขนาดประจุของอิเลคตรอน $400$ ตัว

คำตอบ 

<span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><semantics><mtable rowspacing="0.16em" columnalign="right center left center left" columnspacing="1em"><mtr><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow><mtext>จำนวนประจุของอิเลคตรอน</mtext>  <mn>400</mn>  <mtext>ตัว</mtext></mrow></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mo lspace="0em" rspace="0em">=</mo></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow><mn>400</mn><mo>×</mo><mo stretchy="false">(</mo><mo>−</mo><mn>1.602</mn><mo>×</mo><mn>1</mn><msup><mn>0</mn><mrow><mo>−</mo><mn>19</mn></mrow></msup><mo stretchy="false">)</mo></mrow></mstyle></mtd></mtr><mtr><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow></mrow></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mo lspace="0em" rspace="0em">=</mo></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow><mo>−</mo><mn>6.408</mn><mo>×</mo><mn>1</mn><msup><mn>0</mn><mrow><mo>−</mo><mn>17</mn></mrow></msup></mrow></mstyle></mtd></mtr><mtr><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow></mrow></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mo lspace="0em" rspace="0em">=</mo></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow><mo>−</mo><mn>64.08</mn><mo>×</mo><mn>1</mn><msup><mn>0</mn><mrow><mo>−</mo><mn>18</mn></mrow></msup></mrow></mstyle></mtd></mtr><mtr><mtd><mstyle scriptlevel="0" displaystyle="false"><msub><mi>Q</mi><mn>400</mn></msub></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mo lspace="0em" rspace="0em">=</mo></mstyle></mtd><mtd><mstyle scriptlevel="0" displaystyle="false"><mrow><mo>−</mo><mn>64.08</mn>  <mi>a</mi><mi>C</mi>  <mtext>(atto&nbsp;coulomb)</mtext></mrow></mstyle></mtd></mtr></mtable><annotation encoding="application/x-tex">\begin{array}{rclcl}
\text{จำนวนประจุของอิเลคตรอน} \;400\;\text{ตัว} &amp;=&amp; 400\times (- 1.602 \times 10^{-19}) \\
       &amp;=&amp; -6.408 \times 10^{-17} \\
      &amp;=&amp; -64.08\times 10^{-18} \\
      Q_{400} &amp;=&amp; -64.08\;aC \;\text{(atto coulomb)}
    \end{array}</annotation></semantics></math></span>
    <span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 4.8em; vertical-align: -2.15em;"></span><span class="mord"><span class="mtable"><span class="arraycolsep" style="width: 0.5em;"></span><span class="col-align-r"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 2.65em;"><span class="" style="top: -4.81em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord text"><span class="mord brahmic_fallback">จำนวนประจุของอิเลคตรอน</span></span><span class="mspace" style="margin-right: 0.2778em;"></span><span class="mord">400</span><span class="mspace" style="margin-right: 0.2778em;"></span><span class="mord text"><span class="mord brahmic_fallback">ตัว</span></span></span></span><span class="" style="top: -3.61em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"></span></span><span class="" style="top: -2.41em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"></span></span><span class="" style="top: -1.21em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord"><span class="mord mathnormal">Q</span><span class="msupsub"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.3011em;"><span class="" style="top: -2.55em; margin-left: 0em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">400</span></span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.15em;"><span class=""></span></span></span></span></span></span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 2.15em;"><span class=""></span></span></span></span></span><span class="arraycolsep" style="width: 0.5em;"></span><span class="arraycolsep" style="width: 0.5em;"></span><span class="col-align-c"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 2.65em;"><span class="" style="top: -4.81em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mrel">=</span></span></span><span class="" style="top: -3.61em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mrel">=</span></span></span><span class="" style="top: -2.41em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mrel">=</span></span></span><span class="" style="top: -1.21em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mrel">=</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 2.15em;"><span class=""></span></span></span></span></span><span class="arraycolsep" style="width: 0.5em;"></span><span class="arraycolsep" style="width: 0.5em;"></span><span class="col-align-l"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 2.65em;"><span class="" style="top: -4.81em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord">400</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mbin">×</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mopen">(</span><span class="mord">−</span><span class="mord">1.602</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mbin">×</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mord">1</span><span class="mord"><span class="mord">0</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.8141em;"><span class="" style="top: -3.063em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">−</span><span class="mord mtight">19</span></span></span></span></span></span></span></span></span><span class="mclose">)</span></span></span><span class="" style="top: -3.61em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord">−</span><span class="mord">6.408</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mbin">×</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mord">1</span><span class="mord"><span class="mord">0</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.8141em;"><span class="" style="top: -3.063em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">−</span><span class="mord mtight">17</span></span></span></span></span></span></span></span></span></span></span><span class="" style="top: -2.41em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord">−</span><span class="mord">64.08</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mbin">×</span><span class="mspace" style="margin-right: 0.2222em;"></span><span class="mord">1</span><span class="mord"><span class="mord">0</span><span class="msupsub"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.8141em;"><span class="" style="top: -3.063em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mtight">−</span><span class="mord mtight">18</span></span></span></span></span></span></span></span></span></span></span><span class="" style="top: -1.21em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord">−</span><span class="mord">64.08</span><span class="mspace" style="margin-right: 0.2778em;"></span><span class="mord mathnormal">a</span><span style="margin-right: 0.0715em;" class="mord mathnormal">C</span><span class="mspace" style="margin-right: 0.2778em;"></span><span class="mord text"><span class="mord">(atto&nbsp;coulomb)</span></span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 2.15em;"><span class=""></span></span></span></span></span><span class="arraycolsep" style="width: 0.5em;"></span></span></span></span></span></span>


{{< admonition >}}
อย่าลืมว่าอิเลคตรอนมีประจุเป็นลบ และการตอบต้องให้ค่ามากกว่า 1 
    และต้องอยู่ในเลขกำลังตามตารางสัญกรณ์เติมหน้า

{{< /admonition >}}

  

