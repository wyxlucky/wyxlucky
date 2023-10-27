---
title: 光的偏振
date: 2023/10/26
categories: 知识点
tags: [偏振]
---

<!-- toc -->

<!-- more -->



[TOC]



# 光的偏振

## 线偏振

在观察时间内，光矢量的大小随时间改变，但振动方向始终不变，可以写成
$$
\vec{E}(t) = A* cos(-\omega t)
$$

$$
\left\{  
             \begin{array}{**lr**}  
             E_{x}(t)=  A_{x}* cos(-\omega t), &  \\  
             E_{y}(t)= A_{y}* cos(-\omega t + \delta), &    
             \end{array}  
\right.
$$

其中，<font color='red'>$\delta = 0\ \  or \ \  \pi$</font>.

## 圆偏振

**圆偏振光**的光矢量的大小不变，但方向却随时间改变，沿（逆）着传播方向看矢量端点的轨迹是圆周，可以写成 
$$
\vec{E}(t) =  E_{x}(t)\vec{i}+ E_{y}(t)\vec{j}
$$

$$
\left\{  
             \begin{array}{**lr**}  
             E_{x}(t)=  A * cos(-\omega t), &  \\  
             E_{y}(t)= A * cos(-\omega t \pm \frac{\pi}{2}), &    
             \end{array}  
\right.
$$

<font color='red'>上式对于**左旋**圆偏光取**正**，而对于**右旋**圆偏光取**负**. </font>

## 椭圆偏振

**椭圆偏振光**的道理和圆偏振光类似，光矢量的大小和方向都随时间改变，矢量端点的轨迹是椭圆，同样有解析写法 
$$
\left\{  
             \begin{array}{**lr**}  
             E_{x}(t)=  A_{x} * cos(-\omega t), &  \\  
             E_{y}(t)= A_{y} * cos(-\omega t \pm \frac{\pi}{2}), &    
             \end{array}  
\right.
$$
即两个正交**分量的振幅不相等**.也同样是对于左旋取正，右旋取负。但对于斜椭圆相位差$\delta \neq \pm \frac{\pi}{2}$

## 部分偏振光

光波包含一切可能方向的横振动，但不同方向上的振幅不等，在两个互相垂直的方向上振幅具有最大值和最小值，这种光称为部分偏振光。

## 自然光

光波包含一切可能方向的横振动，但不同方向上的振幅相等。

# 波片

## 二分之一波片

- 产生<font color='red'>$\pi$奇数倍</font>的相位延迟，线偏振光通过二分之一波片后仍是线偏振光。
- 若入射线偏振光的振动方向与波片快轴（或慢轴）夹角为α，则出射线偏振光的振动方向向着快轴（或慢轴）的方向转过2α角度。
- **圆偏振光入射时，出射光是旋向相反的圆偏振光。**

## 四分之一波片 

- o光和e光的位相差等于<font color='red'>$\frac{\pi}{2}$或其奇数倍</font>。

- **四分之一波片可将线偏振光转变为圆偏振光。**

- **四分之一波片还可将圆偏振光转变为线偏振光。**

- 四分之一波片上有两根正交轴，一根称为快轴；一根称为慢轴。线偏振光垂直入射四分之一波片，且光振幅矢量与快轴成45°入射时，光沿快轴和慢轴分解成两个相等的分量，在通过四分之一波片后，沿快轴的分量比沿慢轴的分量超前四分之一光波波长，这样就可以产生圆偏振光。<font color='red'>如果光振幅矢量与快轴成0°和90°时为线偏振光，其他角度，则会产生椭圆偏振光</font>。

  链接：https://www.zhihu.com/question/481043646/answer/2537727697
  

## 偏振片

就是将任意偏振态的入射光转变为线偏光

## **BS（分光棱镜）**

**对入射偏振敏感，线偏振角度会影响分光比。若入射的是自然光或圆偏振光，则按50：50分光。分束的时候只管分能量，理想器件下出射的两路光偏振态还是原来的样子，实际工艺缺陷会造成一点点退偏振。对光强几乎无吸收。

## **PBS（偏振分光棱镜）**

对入射偏振敏感，线偏振角度会影响分光比。若入射的是自然光或圆偏振光，则按50：50分光。分束的时候除了分配能量外，出射的两路光一定是线偏振，而且一束是平行线偏振，一束是垂直线偏振，两种线偏振方向相差90°。

## **NPBS（消偏振分光棱镜）**

对偏振不敏感，不管入射光是什么偏振态的都不会影响到出射光的分光比，分光比在任何情况下都是50：50。分束的时候只管分能量，理想器件下出射的两路光偏振态还是原来的样子，实际工艺缺陷会造成一点点退偏振。对光强有一定的吸收。

# 反射与折射对偏振的影响

[(90 封私信 / 81 条消息) 反射光和入射光的偏振方向一致吗？ - 知乎 (zhihu.com)](https://www.zhihu.com/question/320686618)



## 反射镜对圆偏振光的影响

对于[反射光](https://www.zhihu.com/search?q=反射光&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"answer"%2C"sourceId"%3A1520662734})：由于两个偏振方向的[反射率](https://www.zhihu.com/search?q=反射率&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"answer"%2C"sourceId"%3A1520662734})不同，所以反射光通常的椭圆偏振光，但是当入射角大于[布儒斯特角](https://www.zhihu.com/search?q=布儒斯特角&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"answer"%2C"sourceId"%3A1520662734})时，所有光度反射，所以两个偏振分量一样大，反射光仍然是椭圆偏振光。

对于[折射光](https://www.zhihu.com/search?q=折射光&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"answer"%2C"sourceId"%3A1520662734})：由于两个偏振方向的[折射率](https://www.zhihu.com/search?q=折射率&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"answer"%2C"sourceId"%3A1520662734})不同，所以折射光是椭圆偏振光，同时随着角度增加，透射率越来越低。
链接：https://www.zhihu.com/question/421252099/answer/1520662734

入射光波的电矢量 (光矢量)可以分解为相互正交的两个偏振光分量，**p分量：平行于入射面振动，s分量：垂直于入射面振动**。 

## 反射镜对线偏振光的影响

- 一束线偏振光入射到界面上，由于s分量和p分量的振幅反射系数不同，振动方向发生改变，相对入射光而言，反射光的振动面将发生偏转。

- 可参考：[线偏振光经过界面反射后的偏振情况讨论.pdf (book118.com)](https://max.book118.com/html/2017/0706/120734489.shtm)
