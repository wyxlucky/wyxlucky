---
title: 高斯光束的变换
date: 2023/11/21
categories: 光学
tags: [高斯光束 透镜]
---

<!-- toc -->

<!-- more -->

[TOC]



# 高斯光束的变换（um）

- 入射光束的束腰半径：$$\omega_{0}$$
- 入射光束的波长：$$\lambda$$
- 透镜的焦距：$$f$$

## 高斯光束的传播

<img src="D:\blog\source\posts\2023-11-21 Gauss Beam\GAUSS.jpg" alt="GAUSS" style="zoom:33%;" />

- 高斯光束的发散角：
  $$
  \theta_{0}=\frac{2\lambda}{\pi*\omega_{0}}
  $$
  

<font color='red'>可见，束腰半径小，发散角越大；束腰半径大，发散角就越小；因此，要减小发散角，就必须扩大光斑束腰，所以激光的准直总是伴随着扩束。</font>

- 高斯光束的瑞利距离:

  高斯光束的瑞利长度定义为 $$z$$值，此长度是光束横截面积为束腰两倍的位置。$$\omega(z)$$ 增加至$$ \sqrt{2} \omega_{0}$$。
  $$
  \omega(z)=\frac{\pi*\omega_{0}^{2}}{\lambda}
  $$
  

- 高斯光束的传播：
  $$
  \omega(s) = \omega_{0}\sqrt{1+(\frac{\lambda*s }{\pi*\omega_{0}^{2}})^{2}}
  $$
  

  ## 高斯光束的透镜变换

  透镜前为物，透镜后为像。

  <img src="D:\blog\source\posts\2023-11-21 Gauss Beam\GASSS LEN.jpg" alt="GASSS LEN" style="zoom:33%;" />

- 入射的高斯光束经过经过一个焦距为$$f$$的透镜后，出射光束的束腰变化：

$$
\omega_{1}=\omega_{0}\frac{f}{\sqrt{(|s_{0}|-f)^{2}+\omega(z)^{2}}}=\omega_{0}\frac{f}{\sqrt{(|s_{0}|-f)^{2}+(\frac{\pi*\omega_{0}^{2}}{\lambda})^{2}}}
$$



可见，当$$s=f$$时，且$$f$$越小时，聚焦效果越好。

- 当入射光束的束腰到透镜的距离为$$s$$时,出射光束的焦距：
  $$
  s_{1}=f
  +\frac{f}{\sqrt{(|s_{0}|-f)^{2}+(\frac{\pi*\omega_{0}^{2}}{\lambda})^{2}}}(|s_{0}|-f)
  $$

​	<font color='red'>当$s_{0}=f$时，$s_{1}=f</font>时，

- 出射光束的发散角为：
  $$
  \theta_{1}=\frac{2\lambda}{\pi}\sqrt{\frac{1}{\omega_{0}^{2}}
  (1-\frac{s_{0}}{f})^{2}+\frac{1}{f^{2}}(\frac{\pi*\omega_{0}^{2}}{\lambda})^{2}}
  $$

​	所以，入射光束和出射光束的发散角之比是：
$$
\frac{\theta_{1}}{\theta_{0}}=\frac{\pi*\omega_{0}^{2}}{f*\lambda}\\
\theta_{1}=2\omega_{0}/f
$$

## 高斯光束的准直 -单个透镜

当高斯光束只过一个透镜，且<font color='red'>$s_{0}=f$</font>时，出射光束的束腰半径化简为：
$$
\omega_{1}=\frac{\lambda*f}{\pi*\omega_{0}}
$$
出射光束的发散角：
$$
\theta_{1}=\frac{2 \lambda}{\pi*\omega_{1}}
$$
可见，增大出射光的束腰半径就可以缩小出射光束的发散角。

所以，入射光束和出射光束的发散角之比是：
$$
\frac{\theta_{1}}{\theta_{0}}=\frac{\pi*\omega_{0}^{2}}{f*\lambda}\\
\theta_{1}=2\omega_{0}/f
$$
<font color='red'>有上两个公式可见，当入射光束的束腰半径越小，出射光束的束腰半径越大，或透镜的焦距越大，出射光束的发散角越小，准直效果越好。</font>

## 高斯光束的准直 -透镜组

选用两个透镜，短焦距的凸透镜( 减小光束束腰半径)和长焦距的凸透镜可以达到高斯光束准直的目的。

## 高斯光束的扩束与缩束

<img src="D:\blog\source\posts\2023-11-21 Gauss Beam\LENS.jpg" alt="LENS" style="zoom:33%;" />

高斯光束经过两个透镜，两个透镜的距离为$$f_{1}+f_{2}$$，则高斯光束经过如下变换：
$$
\omega_{1}=\frac{\lambda*f_{1}}{\pi*\omega(s_{0})}\\
\omega_{2}=\frac{\lambda*f_{2}}{\pi*\omega_{1}}
$$
$$\omega(s)$$为入射在第一个透镜表面时的光斑半径。所以，出射光束的束腰半径为：
$$
\omega_{2}=\frac{f_{2}}{f_{1}}\omega(s_{0})
$$
可见，<font color='red'>当第二个透镜的焦距大于第一个透镜的焦距时($f_{2}>f_{1}$)，缩束的目的；当第二个透镜的焦距小于第一个透镜的焦距时($f_{1}>f_{2}$)，可以起到扩束的目的。</font>

- $$M=\frac{f_{2}}{f_{1}}$$，为透镜组的焦距比，也就是透镜组的几何压缩比；

经过透镜组前入射光束与出射光束的发散角之比：
$$
\frac{\theta_{0}}{\theta_{2}}=\frac{f_{2}}{f_{1}}\frac{\omega(s_{0})}{\omega_{0}}
$$

## 准直光的扩束与缩束

<font color='red'>可先将高斯光束准直后在进行扩束或缩束。</font>

因为激光器的输出光束直径一般较小，使用前有时需要先扩束，这时可以通过望远镜光路实现，扩束比就是两透镜焦距的比值。此时在焦点附近加一个针孔可消除光束的强度噪声，得到更干净的输出光。为了达到最佳性能应使用平凸透镜，并且将平面一侧朝向焦点，如下图所示。

![1](D:\blog\source\posts\2023-11-21 Gauss Beam\1.png) 

## Mathmatic代码

```
\[Omega]0 = 580;(*初始束腰半径*)
\[Lambda] = 369 10^-3;(*波长*)
f = 100 10^3;(*焦距*)
s0 = f;(*透镜距入射光束束腰处为s0*)
s1 = f;(*透镜距出射光束束腰处为s1*)
(***高斯光束距束腰s处的光斑半径***)
\[Omega]s[s0_] := \[Omega]0 Sqrt[
  1 + ((\[Lambda] s0)/(\[Pi] \[Omega]0^2))^2]
(***瑞利距离***)
\[Omega]z = N@(( \[Pi] \[Omega]0^2)/\[Lambda])
(***经过透镜后的光斑束腰半径***)
\[Omega]1 = 
 N@ \[Omega]0 f/
  Sqrt[(Abs[s] - f)^2 + (( \[Pi] \[Omega]0^2)/\[Lambda])^2]
(*当入射光束束腰距透镜距离s时，出射光束的焦距是s1:*)
s1 = N[f + (f/
     Sqrt[(Abs[s] - 
        f)^2 + (( \[Pi] \[Omega]0^2)/\[Lambda])^2])^2 (Abs[s] - f)]
(*Subscript[腰斑大小为\[Omega], 0]的物高斯光束的发散角为*)
\[Theta]0 = N@(\[Lambda]/(\[Pi] \[Omega]0))(*入射光束*)
\[Theta]1 = N@(\[Lambda]/(\[Pi] \[Omega]1))(*出射光束*)
(*即通过增大出射光束到的束腰半径来减小发散角--出射光束*)


(***经过一个透镜后出射光束的发散角***)
\[Theta]1 = (2 \[Lambda])/\[Pi] Sqrt[
  1/\[Omega]0^2 (1 - s0/f)^2 + 1/f^2 ((\[Pi] \[Omega]0^2)/\[Lambda])^2]



(***高斯光束经过透镜组后的束腰变化***)
f2 = f;
f1 = f/2;
\[Omega]2 = f2/f1 \[Omega]s[s0]
```



## 参考笔记

- [高斯光束光学（八）-高斯光束的准直 (optkt.com)](https://www.optkt.com/fa/399/1#:~:text=在l%3DF的条件下，像高斯光束的方向性不但与F的大小有关%2C而且也与ω0的大小有关。,ω0愈小，则像高斯光束的方向性愈好。 因此，如果先用一个短焦距的透镜将高斯光束聚焦，以便获得极小的腰斑，然后再用一个长焦距的透镜来改善其方向性，就可得到很好的准直效果。)
- [高斯光束传播 | 爱特蒙特光学 (edmundoptics.cn)](https://www.edmundoptics.cn/knowledge-center/application-notes/lasers/gaussian-beam-propagation/)
- [高斯光束的透镜变换.ppt (book118.com)](https://max.book118.com/html/2017/0528/109763935.shtm)

## 高斯光束变化的小程序

- 链接: https://pan.baidu.com/s/1-IJ2AZ_6Wgdoh0P3QFC6mQ 提取码: 43d8 复制这段内容后打开百度网盘手机App，操作更方便哦
