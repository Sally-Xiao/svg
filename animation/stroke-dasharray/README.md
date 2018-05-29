// 利用stroke-dasharray和stroke-dashoffset实现边框变化的效果
stroke-dasharray: x y, x为实线部分的长度，y为虚线部分的长度
stroke-dashoffset: 起始位置偏移长度, 相当于把线往前面拉拽多长。

本效果的实现原理为: 利用图像的重叠和stroke-dashoffset来实现错位，达到视觉上的不同颜色的线条走动的效果，动画的起始偏移量差异应等于stroke-dasharray中的实线长度。三条线的stroke-dasharray需设置一致，动画时长设置一致，为了保持持续运动，需设置infinite。为了保持动画看起来顺畅，需设置antimation-direction为alternate。

[参考地址](https://www.w3cplus.com/svg/svg-animation.html)