---
title: UI设计规范总结
url: 1453.html
id: 1453
categories:
  - huhuの文章
  - 设计心得
date: 2017-06-01 13:40:37
tags:
---

#### 尺寸

iOS用750*1334即可； android的尺寸众多，建议使用分辨率为720x1280 的尺寸设计。这个尺寸 720x1280中显示完美，在 1080x1920 中看起来也比较清晰；切图后的图片文件大小也适中，应用的内存消耗也不会过高。

#### 颜色值

IOS颜色值取 RGB各颜色的值比如某个色值，给予IOS开发的色值为 R:12 G:34 B:56 给出的值就是 12,34,56(有时也要根据开发的习惯，有时也用十六进制) Android颜色值取值为十六进制的值

#### 内部设计

1、所有能点击的图片不得小于44px（Retina需要88px） 2、单独存在的部件必须是双数尺寸 3、两倍图以@2x作为命名后缀 4、充分考虑每个控制按钮在4中状态下的样式

#### 字体

iPhone默认字体：中文—Heiti SC，英文— helvetica； 安卓默认字体：中文——思源黑，英文——Roboto。  

[DPI、PPI、DP、PX 的详细计算方法及算法来源是什么？](https://www.zhihu.com/question/21220154)

1\. dpi是dot per inch，每英寸多少点，ppi是 Pixel per inch，每英寸像素数，针对显示器的设计时，dpi=ppi。 ppi计算方法是长宽各自平方之和开方，除以对角线长度（单位英寸）。原理可以自己画个矩形勾股定理算一算。 2. ppi表示显示设备的点密度，dpi表示印刷品点密度。 3. dip或dp，是安卓开发用的单位，1dp表示在屏幕点密度为160ppi时1px长度。 因为安卓设备屏幕众多不可能为每个屏幕单独开发，所以用公式 px=dp*(ppi/160)计算在不同屏幕上的像素数。 举例：HVGA屏320\*480，一般是3.5寸，计算点密度为√ (320^2 + 480^2) / 3.5 = 164，约等于160，1pd=1px WVGA屏480\*800，按3.8寸屏算，点密度 √ (480^2 + 800^2) / 3.8 = 245，约等于240，1dp=1.5px。 还有更高分辨率的屏幕就不一一列举了，总之dp是为了方便适配不同屏幕的单位，在不同屏幕密度下，1dp的物理长度也相同。

iPhone X设计规范：[http://www.tuyiyi.com/v/55463.html](http://www.tuyiyi.com/v/55463.html)