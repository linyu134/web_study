## 1.浏览器渲染原理

1. 根据 `HTML` 构建 `HTML` 树(`DOM`).
2. 根据 `CSS` 构建 `CSS` 树(`CSSOM`).
3. 将两棵树合并成一颗渲染树(`render tree`).
4. `Layout` 布局(文档流、盒模型、计算大小和位置).
5. `Paint` 绘制(把边框颜色、文字颜色、阴影等画出来).
6. `Compose` 合成(根据层叠关系展示画面).

## 2.CSS 动画的两种做法（transition 和 animation）

```CSS
transition:all 1s;                 /* 变化过程1s */
transform:translate(100px,100px);  /* x轴位移100px，y轴位移100px */
transform:rotate(45deg)            /* 旋转45度 */
transform:scale(1.5)              /* 放大1.5倍 */
```

```CSS


animation: heart linear 800ms infinite alternate;/*animation:动画名 过度方式 延时 次数 方向*/
@keyframes heart {                /*@keyframes 动画名{}*/
    0% {
        transform: scale(0);
    }

    100% {
        transform: scale(1.2);
    }
}
```

## 3.其他知识

1. css 学习时，不问为什么，只说原来如此。
2. 代码运行后再得出结论。
3. 关于定位，绝对定位 `absolute` 是根据祖先中最近的非 `static` 值来定位的.
4. 浮动，需要在父元素上加上三行代码:

```CSS
clear:both;
content:'';
display:block;
```

5. flex 布局居中：

```CSS
display:flex;
justify-content:center;
align-items: center;
```

6. grid 布局：

```CSS
.container{
    display:grid;
    grid-template-areas:     /*布局结构*/
    "header header header"
    "aside main ad"
    "footer footer footer";
    grid-gap: 10px;     /*内容模块间隔10px*/
}

header{
    grid-area:header;
}
aside{
    grid-area:aside;
}
main{
    grid-area:main;
}
.ad{
    grid-area:ad;
}
footer{
    grid-area:footer;
}


```
