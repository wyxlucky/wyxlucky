---
title: 时序逻辑与组合逻辑
date: 2023/10/26
categories: FPGA
tags: [FPGA,时序逻辑,组合逻辑]
---

<!-- toc -->

<!-- more -->





# 组合逻辑

## 一、always @（*）

- 从代码层面来看，如果always是没有上升沿或者是带有“*”号的代码，为组合逻辑。

- <font color='red'>组合逻辑的波形or信号是即刻反映变化的，与时钟无关</font>。

- 组合逻辑竞争冒险 ： 只要输入信号同时变化，组合逻辑就必然产生毛刺。

- always中定义的是**reg型**。

- **通常用阻塞赋值（=）**

  ```
  reg sum;
  always @(*)
  	begin
      	sum=a+b;
  	end
  end
  
  ```

## 二、assign

- assign语句描述的电路：利于条件“？”可以描述一些相对简单的组合逻辑电路，**信号只能被定义为wire型**，**必须用阻塞语句（=）**。当组合逻辑比较复杂时，代码的可读性就差。

  ```
  wire sum;
  assign  sum = b? a : b 
  ```

  

# 时序逻辑

## always @（poseedge clk）

- 从代码层面来看，时序逻辑即敏感列表里面带有时钟上升沿。

- <font color='red'>时序逻辑的波形or信号不会立刻反映出来，只有在时钟的上升沿发生变化。</font>

- 在代码层面，时序逻辑代码表示如下，可以看到此代码有“posedge“时钟上升沿，即表示有一个**D触发器**，a+b的结果sum是在D触发器发出指令后才进行输出的。

  ```
  wire sum;
  always @(poseedge clk)
  	begin
      	sum <= a+b;
  	end
  end
  ```

  更多可参考：[【技巧分享】时序逻辑和组合逻辑的区别和使用 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/110543798)

