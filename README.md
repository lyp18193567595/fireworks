# fireworks
春节烟花
整个内容氛围两部分：倒计时展示和烟花播放效果

主要实现原理：

1、HTML 部分:
包含一个用于显示倒计时的 div 元素和一个用于显示烟花效果的 div 元素。

2、CSS 部分:
body 元素的样式设置为占满整个窗口，去除默认边距，隐藏滚动条，背景颜色为黑色。

3、JavaScript 部分:
updateCountdown 函数:计算并更新距离 2025 年春节的倒计时，每秒调用一次。
createParticle 函数:创建一个烟花粒子，并为其添加动画效果。
createFirework 函数:随机生成烟花爆炸的位置和颜色，创建多个粒子模拟烟花爆炸效果。0setInterval(createFirework，1500):每隔 1.5 秒创建一个新的烟花。

背景渐变:为 #countdown 元素设定线性渐变背景，涵盖红、橙、黄、绿、蓝、靛、紫这几种颜色
背景大小:把背景大小设定为 400%400%，从而让背景在动画期间有足够的空间移动。
文字填充:运用 background-clip:text 和 -webkit-text-fill-color: transparent 使文字显示为背景
动画效果:借助 @keyframes 定义了一个名为 rainbow 的动画，让背景位置在 10 秒内循环移动，产生炫彩效果。