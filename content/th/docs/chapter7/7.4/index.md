---
title: "7.4 กำลังปรากฏและตัวประกอบกำลัง"
description: "Doks is a Hugo theme for building secure, fast, and SEO-ready documentation websites, which you can easily update and customize."
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "chapter7"
weight: 740
toc: true
---

{{<admonition info "นิยาม 7.4 ค่าแอฟแฟคทีฟ" false>}}
กำลังปรากฏ (apparent power) S คือผลคูณของแรงดัน rms กับกระแส rms
\begin{align}
    S=V_\text{rms}I_\text{rms} \tag{7.43}
\end{align}
จากสมการ $(7.41)$ นำมาเขียนใหม่ในรูปของกำลังปรากฏได้เป็น
\begin{align}
    P=V_\text{rms}I_\text{rms}\cos (\theta_v - \theta_i)=S\cos (\theta_v - \theta_i) \tag{7.44}
\end{align}
โดยที่ $S$ มีหน่วยเป็น VA (volt-ampere)

{{</admonition>}}

{{<admonition warning "สำคัญ" false>}}
$\cos (\theta_v - \theta_i)$ มีชื่อเรียกเป็นพิเศษว่า ตัวประกอบกำลัง (power factor)
{{</admonition>}}

## **power factor หรือ pf** ##

ค่าตัวประกอบกำลังเป็นค่าที่ไม่มีหน่วย และหาได้จาก
\begin{align}
    pf=\dfrac{P}{S}=\cos (\theta_v - \theta_i) \tag{7.45}
\end{align}
มุม $(\theta_v - \theta_i)$ เป็นมุมของอิมพีแดนซ์ $Z$ ด้วย 
\begin{align}
    \mathbf{Z}=\dfrac{\mathbf{V}}{\mathbf{I}}=\dfrac{V_m\angle{\theta_v}}{I_m\angle{\theta_i}}=\dfrac{V_m}{I_m}\angle{\theta_v-\theta_i}\tag{7.46}
\end{align}
ค่าอิมพีแดนซ์ $Z$ ในรูป rms คือ
\begin{align}
    \mathbf{Z}=\dfrac{\mathbf{V}}{\mathbf{I}}=\dfrac{\mathbf{V_\text{rms}}}{\mathbf{I_\text{rms}}}=\dfrac{V_\text{rms}}{I_\text{rms}}\angle{\theta_v-\theta_i}\tag{7.47}
\end{align}

### ช่วงค่าของ pf ###

ค่าของ pf ขึ้นอยู่กับชนิดของโหลดดังนี้

1. ในกรณีที่โหลดเป็นตัวต้านทาน ค่า pf = 1 เนื่องจากมุมเฟสของแรงดันและกระแสเท่ากัน $\mathrm{pf}=\cos (\theta_v - \theta_i)=\cos 0 = 1$ 
2. ในกรณีที่โหลดเป็นตัวเหนี่ยวนำหรือตัวเก็บประจุ ค่า pf = 0 เนื่องจากมุมเฟสของแรงดันและกระแสต่างกันเป็น $90^{\circ}$ ดังนั้น $\mathrm{pf}=\cos (\pm 90^{\circ})=0$

3. ในกรณีที่โหลดมีทั้งตัวต้านทาน และ ตัวเหนี่ยวนำ หรือ ตัวเก็บประจุ ค่า pf อยู่ระหว่าง 0 กับ 1 โดยที่ค่า pf จะเป็น 
    - leading ถ้ามุมเฟสกระแสนำมุมเฟสของแรงดัน มันบอกเป็นนัยว่าโหลดเป็นตัวเก็บประจุ (เป็นส่วนใหญ่)
    - laggin ถ้ามุมเฟสของกระแสตามมุมเฟสของแรงดันและมันบอกเป็นนัยว่าโหลดเป็นตัวเหนี่ยวนำ (เป็นส่วนใหญ่)
