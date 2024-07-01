# border-box

border-box: content-box;
border or padding will be added to final rendered width, making the element wider than 100px.

border-box: border-box;
If you set the width to 100 pixels, that 100 pixels will includes any border or padding you added,
and the content box will shrink to absorb that extra width

# transform
```css
.cane-image {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

```
常见的居中技巧
## 使用场景：
需要将一个元素在其定位的父元素中居中
希望居中的效果不会受元素内容变化影响时
## 缺点：
需要定位父元素: 元素的定位是相对于其定位父元素而言的，因此需要确保父元素设置了 position: relative、 position: absolute 或 position: fixed。

# transition

transition属性可以分解为以下几个子属性：
transition-property: 指定要应用过渡效果的CSS属性，例如 width、height、background-color、opacity等等，可以设置为all来应用于所有可动画的属性
transition-duration: 设置过渡效果的持续时间，单位可以是秒(s)或毫秒(ms)。
transition-timing-function: 定义过渡的速度曲线，控制过渡过程中变化的节奏。常见的速度曲线包括ease、linear、ease-in、ease-out、ease-in-out以及cubic-bezier()自定义函数
transition-delay: 设置过渡的延迟时间，单位同样是秒(s)或毫秒(ms)。


该项目编写流程：

先添加common Style，设置盒模型，清除a元素默认样式，引入字体
然后使用:root伪类选择器定义颜色变量，以便在全局使用。

然后添加html元素，编写header，main布局，然后定义cane-image做main元素的背景图
接下来定义三组水果图片section元素

引入字体文件
设置header样式设置Cane image样式将其定位到页面中间
将label三种饮料图片宽度设为当前页面的三倍，定位到左侧位置，占满屏幕
设置三种水果的四张图片，在页面四角漂浮旋转，每组水果的盒子进行相对定位以便每个水果单独进行绝对定位并单独设置颜色
随后设置四张图片的阴影
最后设置两侧按钮的固定定位
