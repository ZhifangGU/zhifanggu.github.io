---
layout: page
title: "Matlab Skills"
date: 2019-11-03 16:13:00 +0800
categories: Master Study
---
## Figure Dimensions Setup

#### Using command line

In **paper writing**, usually we want to make sure the figures plotted by Matlab keep the same dimensions. In the script, we can specify the dimension of figures. The relationship among screen, figure and axis  is worth noting. 

```matlab
set (gca, 'position', [200, 100, 500, 300]);
```

This command specifies the location of the figure origin point in the screen is (200, 100), and the dimension is 500 pixels * 300 pixels.

```matlab
set(gca,'position',[0.1,0.1,0.5,0.5]);
```

This command specifies the axis scale to the figure. Specifically, the origin point of the axis is located in 0.1 * (figure width), and the axis width is 0.5 * (figure width).  

#### Using export setup (GUI)

In the displayer figure GUI, choose 'File' and then 'Export Setup'. In the properties, choose 'Size' and specify the width and height.