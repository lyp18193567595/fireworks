# fireworks
春节烟花
整个内容氛围两部分：倒计时展示和烟花播放效果
HTML 部分:
包含一个用于显示倒计时的 div 元素和一个用于显示烟花效果的 div 元素。0
CSS 部分:
0body 元素的样式设置为占满整个窗口，去除默认边距，隐藏滚动条，背景颜色为黑色。
0
O
#countdown 元素的样式设置为居中显示，白色文字，字体大小为 36px。
#fireworks 元素的样式设置为覆盖整个窗口。
.particle 元素的样式设置为绝对定位，圆形，随机颜色。
JavaScript 部分:
updateCountdown 函数:计算并更新距离 2025 年春节的倒计时，每秒调用一次。0
。
createParticle 函数:创建一个烟花粒子，并为其添加动画效果。
createFirework 函数:随机生成烟花爆炸的位置和颜色，创建多个粒子模拟烟花爆炸效果。0setInterval(createFirework，1500):每隔 1.5 秒创建一个新的烟花。0