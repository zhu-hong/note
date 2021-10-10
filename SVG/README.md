# SVG

## 标准开头

```html
<svg width="a" height="b" viewBox="0 0 a b"></svg>
```

+ 规定高度，宽度、
+ viewBox等比例缩放

## 圆

### circle

```html
<circle cx="50%" cy="50% r="40" fill="none" stroke="blue" stroke-width="xx"></circle>
```

cx="xx"	cy="xx"	==规定圆心的位置==在x,y轴上的位置

r="xx"	半径大小

fill="color/none"	填充	==通用==

stroke="color"	边框颜色	==通用==

stroke-width="xx"	边框宽度	==通用==

stroke-opacity="0.x"	边框透明度	==通用==

## 矩形

### rect

```xml
<rect width="100" height="100" x="50" y="50" rx="20"></rect>
```

width="xx"	规定宽

height="xx"	规定高

x="xx"	距离X轴的距离

y="xx"	距离Y轴的距离

rx="xx"	为矩形设置圆角	ry未写默认与rx的值相同

## 线

### line

```xml
<line x1="0" y1="0" x2="100" y2="100"></line>
```

x1,y1	x2,y2	直线两个端点的坐标

## 折线

### polyline

```xml
<polyline points="50 50 200 200 50 24"></polyline>
```

pointts="xx xx xx xx xx xx"	两个点一个坐标，然后连起来，首尾不连

## 多边形

### polygon

```xml
<polygon points="50 50 200 200 50 24"></polygon>
```

pointts="xx xx xx xx xx xx"	两个点一个坐标，然后连起来，首尾相连

## 路径

### path

```xml
<path d="M L H V A Z"></path>
```

Mxx xx	起点坐标

Lxx xx	终点指标

H/hxx	水平方向直线

V/v	垂直方向直线

Z 闭合

#### A 

AX半径^1^Y半径^2^角度^3^弧长^4^顺逆时针^5^终点X坐标^6^终点Y坐标^7^

+ 弧长：0 小弧	1 大弧
+ 顺逆时针：0 逆时针 1顺时针

