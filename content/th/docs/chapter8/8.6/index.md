---
title: "8.6 กำลังในระบบสมดุล"
description: "Doks is a Hugo theme for building secure, fast, and SEO-ready documentation websites, which you can easily update and customize."
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "chapter8"
weight: 860
toc: true
---

## กำลังในระบบสมดุล

หากำลังในระบบสมดุลโดยวิเคราะห์จากโดเมนเวลา ค่ากำลังปัจจุบัน (instantaneous power) ที่โหลดใช้คือ $p(t)=v(t)i(t)$ 

สำหรับโหลดที่ต่อแบบ Y ค่าแรงดันเฟสคือ
\begin{align}
    v_{AN}&=\sqrt{2}V_p\cos\omega t\notag\\\\ v_{BN}&=\sqrt{2}V_p\cos (\omega t -120^{\circ})\tag{8.43}\\\\ v_{CN}&=\sqrt{2}V_p\cos (\omega t + 120^{\circ})\notag
\end{align}
โดยที่ $\sqrt{2}$ จำเป็นต้องมีเนื่องจาก ค่า $V_p$ ถูกกำหนดให้เป็นค่า rms ของแรงดันเฟส ถ้า $\mathbf{Z}\_Y=Z\angle{\theta}$ กระแสเฟสตามหลังแรงดันเฟสอยู่ $\theta$ ดังนั้น
\begin{align}
    i_a&=\sqrt{2}I_p\cos (\omega t -\theta)\notag\\\\ i_b&=\sqrt{2}I_p\cos (\omega t -\theta-120^{\circ})\tag{8.44}\\\\ i_c&=\sqrt{2}I_p\cos (\omega t -\theta+120^{\circ})\notag
\end{align}
โดยที่ $I_p$ เป็นค่า rms ของกระแสเฟส

ค่ากำลังปัจจุบันทั้งหมดคือ
\begin{align}
    p&=p_a+p_b+p_c=v_{AN}i_a+v_{BN}i_b+
v_{CN}i_c\nonumber\\\\
&=2V_pI_p[\cos\omega t\cos (\omega t -\theta) +\cos (\omega t -120^{\circ})\cos (\omega t -\theta-120^{\circ}) \nonumber \\\\
&+ \cos (\omega t +120^{\circ})\cos (\omega t -\theta+120^{\circ})]\tag{8.45}
\end{align} 

ใช้คุณสมบัติของตรีโกณ
\begin{align}
    \cos A \cos B &= \dfrac{1}{2}[\cos(A+B)+\cos(A-B)]\tag{8.46}\\\\
    \cos\omega t\cos (\omega t -\theta) &= \dfrac{1}{2}[\cos(\omega t+\omega t -\theta)+\cos(\omega t-\omega t +\theta)]\notag\\\\
    &= \dfrac{1}{2}[\cos(2\omega t -\theta)+\cos(\theta)]\notag\\\\
    \cos(\omega t -120^{\circ})\cos (\omega t -\theta -120^{\circ}) 
    &= \dfrac{1}{2}[\cos(2\omega t -\theta-240^{\circ})+\cos(\theta)]\notag\\\\
    \cos(\omega t +120^{\circ})\cos (\omega t -\theta +120^{\circ}) 
    &= \dfrac{1}{2}[\cos(2\omega t -\theta+240^{\circ})+\cos(\theta)]\notag\\\\
\end{align}

ได้เป็น
\begin{align}
    p&=V_pI_p[3\cos \theta +\cos (2\omega t-\theta) +\cos (2\omega t-\theta -240^{\circ})+\cos (2\omega t -\theta +240^{\circ}]\nonumber\\\\
    \tag{8.47}
\end{align}

จากคุณสมบัติ
$$
  \begin{align*}
  \sin(A \pm B) &= \sin A \cos B \pm \cos A \sin B\notag\\\\
  \cos(A \pm B) &= \cos A \cos B \mp \sin A \sin B\\\\
  \cos (2\omega t-\theta -240^{\circ})&= \cos(2\omega t -\theta) \cos (240^{\circ}) + \sin(2\omega t -\theta) \sin (240^{\circ})\\\\
  \cos (2\omega t-\theta +240^{\circ})&= \cos(2\omega t -\theta) \cos (240^{\circ}) - \sin(2\omega t -\theta) \sin (240^{\circ}) 
  \end{align*}
$$

กำหนดให้  $ \alpha = (2\omega t-\theta)$

ทำให้ได้
\begin{align}
    p&=V_pI_p[3\cos \theta +\cos \alpha +\cos \alpha \cos 240^{\circ} + \sin \alpha \sin 240^{\circ}\nonumber \\\\&+\cos \alpha \cos 240^{\circ} -\sin \alpha \sin 240^{\circ} ]\notag\\\\&=V_pI_p[3\cos \theta +\cos \alpha + 2\left(-\dfrac{1}{2}\right)\cos\alpha]=3V_pI_p\cos\theta \tag{8.48}
\end{align}
ดังนั้นค่ากำลังปัจจุบันมีค่าคงที่ไม่ขึ้นกับเวลา ซึ่งไม่ว่าโหลดต่อแบบ $\Delta$ หรือ $Y$ ก็ได้ค่าคงที่เหมือนกัน และค่ากำลังเฉลี่ยต่อเฟสทั้งกรณีที่โหลดต่อแบบ $\Delta$ และ ต่อแบบ $Y$ คือ $p/3$ ดังนั้น ค่ากำลังเฉลี่ยต่อเฟสคือ
\begin{align}
    P_p=V_pI_p\cos \theta \tag{8.49}
\end{align}
และค่ากำลังรีแอคทีฟต่อเฟสคือ
\begin{align}
    Q_p=V_pI_p\sin \theta \tag{8.50}
\end{align}
ค่ากำลังปรากฏต่อเฟสคือ
\begin{align}
    S_p=V_pI_p \tag{8.51}
\end{align}
และค่ากำลังเชิงซ้อนต่อเฟสคือ
\begin{align}
    \mathbf{S}_p=P_p+jQ_p=\mathbf{V}_p\mathbf{I}_p^\ast \tag{8.52}
\end{align}
โดยที่ $\mathbf{V}_p$  และ $\mathbf{I}_p$ คือแรงดันเฟสและกระแสเฟสที่มีขนาด $V_p$ และ $I_p$ ตามลำดับ ค่ากำลังเฉลี่ยรวมคือ ผลรวมของค่ากำลังเฉลี่ยแต่ละเฟส
\begin{align}
    P=P_a+P_b+P_c=3P_p=3V_pI_p\cos \theta = \sqrt{3}V_LI_L \cos \theta \label{eq8:p} \tag{8.53}
\end{align}
สำหรับโหลดที่ต่อแบบ $Y$ ค่า $I_L=I_p$ แต่ $V_L=\sqrt{3}I_p$ แต่กรณีที่โหลดต่อแบบ $\Delta$ ค่า $I_L=\sqrt{3}I_p$ แต่ $V_L=V_p$ ดังนั้นสมการ  \eqref{eq8:p} ใช้ได้ทั้งกรณีที่โหลดต่อแบบ Y และต่อแบบ $\Delta$ ในทำนองเดียวกันกำลังรีแอคทีฟรวมคือ
\begin{align}
    Q=Q_a+Q_b+Q_c=3Q_p=3V_pI_p\sin \theta = \sqrt{3}V_LI_L \sin \theta \tag{8.54}
\end{align}
กำลังเชิงซ้อนรวมคือ
\begin{align}
    \mathbf{S}=3\mathbf{S}_p=3\mathbf{V}_p\mathbf{I}_p^\ast=3I_p^2\mathbf{Z}_p=\dfrac{3V_p^2}{\mathbf{Z}_p^\ast} \label{eq8:stotal} \tag{8.55}
\end{align}
โดยที่ $\mathbf{Z}_p=Z\angle{\theta}$ คืออิมพีแดนซ์โหลดต่อเฟส ($\mathbf{Z}_p$  อาจเป็นได้ทั้ง $\mathbf{Z}\_Y$ หรือ $\mathbf{Z}\_{\Delta}$)
สมการ \eqref{eq8:stotal} อาจเขียนอีกแบบคือ

\begin{align}
    \mathbf{S}=P+jQ=\sqrt{3}V_LI_L\angle{\theta}  \tag{8.56}
\end{align}

อย่าลืมว่าค่า $V_p, I_p, V_L, I_L$ เป็นค่า rms ทั้งหมด และมุม $\theta$ เป็นมุมของอิมพีแดนซ์โหลด หรือมุมผลต่างระหว่างมุมเฟสของแรงดันและมุมเฟสของกระแส

## ตัวอย่าง 8.6
{{<admonition abstract "ตัวอย่าง 8.6" false>}}

จากรูปที่ 8.8 จงหากำลังเฉลี่ยรวม กำลังรีแอคทีฟ และกำลังเชิงซ้อน ที่แหล่งจ่าย และที่โหลด

คำตอบ

เนื่องจากระบบสมดุล ดังนั้นพิจารณาเพียงเฟสเดียวดังนี้ สำหรับ เฟส a
\begin{align*}
    \mathbf{V}_p=110\angle{0^{\circ}}\\;\mathrm{V} \qquad \text{และ} \qquad \mathbf{I}_p=6.81\angle{-21.8^{\circ}}\\;\mathrm{A}
\end{align*}
กำลังเชิงซ้อนที่แหล่งจ่ายคือ
\begin{align*}
    \mathbf{S}_s=-3V_pI_p^\ast&=-3(110\angle{0^{\circ}}(6.81\angle{21.8^{\circ}}))\\\\
    &=-2247\angle{21.8^{\circ}}=-(2087+j834.6)\\;\mathrm{VA}
\end{align*}

{{<admonition warning "สำคัญ" false>}}
การคิดกำลังของแหล่งจ่ายให้ใช้เครื่องหมายลบ กรณีที่ไม่ได้กลับทิศกระแส (กระแสไหลออกจากแหล่งจ่าย)
{{</admonition >}}

กำลังจริงที่แหล่งจ่ายจ่ายให้เท่ากับ $-2087\\;\mathrm{W}$ และกำลังรีแอคทีฟที่แหล่งจ่ายใช้คือ  $-834.6\\;\mathrm{VAR}$

ที่โหลด กำลังเชิงซ้อนที่โหลดใช้คือ
\begin{align*}
    \mathbf{S}_L=3|\mathbf{I}_p|^2\mathbf{Z}_p
\end{align*}
โดยที่ $\mathbf{Z}_p=10+j8=12.81\angle{38.66^{\circ}}$ และ $\mathbf{I}_p=\mathbf{I}_a=6.81\angle{-21.8^{\circ}}$ 
ดังนั้น

\begin{align*}
    \mathbf{S}\_L&=3(6.81)^2(12.81)\angle{38.66^{\circ}}=1782\angle{38.66^{\circ}}\\\\
    &=(1392+j1113)\\;\mathrm{VA}
\end{align*}

กำลังเฉลี่ยที่โหลดใช้คือ $1391.7\\;\mathrm{W}$ และกำลังรีแอคทีฟที่โหลดใช้คือ $1113.3\\;\mathrm{VAR}$ 

ผลต่างของกำลังเชิงซ้อนทั้งสองคือค่าที่ถูกใช้โดยอิมพีแดนซ์ของสายส่งซึ่งมีค่าอิมพีแดนซ์เป็น $(5-j2)\\;\Omega$ 

เพื่อพิสูจน์ว่าใช่ลองคำนวณกำลังเชิงซ้อนที่ใช้โดยสายส่งดังนี้

\begin{align*}
    \mathbf{S}\_\ell=3|\mathbf{I}\_p|^2\mathbf{Z}\_\ell=3(6.81)^2(5-j2)=695.6-j278.3 \\;\mathrm{VA}
\end{align*}

ซึ่งเป็นผลต่างของ $\mathbf{S}_s$ และ $\mathbf{S}_L$ 

ดังนั้น 
$$\mathbf{S}\_s+\mathbf{S}\_{\ell}+\mathbf{S}
_L=0\notag
$$ 
