---
layout: page
title: "Matlab Skills"
date: 2019-11-03 16:13:00 +0800
categories: Master Study
---
## Figure Properties Setup

#### Using command line

In **paper writing**, usually we want to make sure the figures plotted by Matlab keep the same dimensions. In the script, we can specify the dimension of figures. The relationship among screen, figure and axis  is worth noting. 

```matlab
set (gcf, 'position', [200, 100, 500, 300]);
```

This command specifies the location of the figure origin point in the screen is (200, 100), and the dimension is 500 pixels * 300 pixels. `gcf` gets the current figure handle.

```matlab
set(gca,'position',[0.1,0.1,0.8,0.8], 'Fontsize', 15);
```

This command specifies the axis scale to the figure. Specifically, the origin point of the axis is located in 0.1 * (figure width), and the axis width is 0.8 * (figure width).  `gca` gets the current axis handle.

```matlab
plot(x, y, '-b*', 'LineWidth', 1 , 'MarkerSize', 8);
```

This command set the line specification. `'-b*'` means solid blue line with asterisk marker. 

```matlab
lgd=legend('a', 'b', 'c', 'd', 'Location', 'southeast', NumColumns, 2);
set(lgd, 'Fontsize', 14);
```

This command adds a legend with specific location and column numbers requirements.

#### Using export setup (GUI)

In the displayer figure GUI, choose 'File' and then 'Export Setup'. In the properties, choose 'Size' and specify the width and height.