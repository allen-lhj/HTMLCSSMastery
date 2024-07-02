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

# writing process

First, we add common styles to the page to reset the browser's default styles and import the necessary font files.

Secondly, we define the :root class to set the colors that are frequently used throughout the design.

Next, we define the structure of the page, which includes the header element and the main content area. Inside the main area, there are two navigation buttons and three sections, each containing image elements.

We then set the background image styles, positioning the .cane-image at the center of the page. The .cane-image box has two images one is a bottle picture, and the other one is  backgrounds are the three different designs for the bottle. Therefore, we set the Labels img widths to three times the body width. This allows us to show the second design by simply moving the Labels left by one body width using JavaScript.

After that, we set the styles for the four images within each section. We center these images and apply some transformations, such as rotations and other effects.

Next, we use JavaScript to control the display of the images and apply keyframe animations for dynamic changes.

Finally, we implement media queries to ensure the layout and styles adapt to different screen widths.