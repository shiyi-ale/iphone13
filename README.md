# Apple？apple！



## 今天是day1

通过使用Codingstartup的TriggerJs

先跟着Steven实现了Iphone13的开场推送

无意间找到了Steven老师的页面制作

感觉收益颇多

澳门独特的口音

给大陆的我带来许多惊喜

跟着steven老师学习第一天

## 心得体会

```html
background-image: conic-gradient(
        #0f2257,
        #1d41a5,
        #1d3781,
        #90f1fe,
        #06153e,
        #06153e
);
```

通过渐变旋转的形式实现的背景图片

逼格满满

## 原效果：

https://www.apple.com/iphone-13-pro/

![image-20211025193314069](https://i.loli.net/2021/10/25/3xG8WsVlbN5YckQ.png)

## 模仿效果





![image-20211025191834074](https://i.loli.net/2021/10/25/ON1Tv4gK9Mns8ze.png)

## 实现的效果一览

![image-20211025192614996](https://i.loli.net/2021/10/25/2tZakQCsuHegmxq.png)

核心实现：

```html

<div id="container2"tg-ref="container" tg-name="opacity" tg-from="-1" tg-to="10"tg-step="1">


    <span tg-name="opacity" tg-filter="2!"tg-map="2: 1"tg-follow="container"> A dramatically more powerful camera system. </span>
    <span tg-name="opacity" tg-filter="3!"tg-map="3: 1"tg-follow="container"> A display so responsive, every interaction feels new again.</span>
    <span tg-name="opacity" tg-filter="4!"tg-map="4: 1"tg-follow="container"> The world’s fastest smartphone chip. Exceptional durability.</span>
    <span tg-name="opacity" tg-filter="5!"tg-map="5: 1"tg-follow="container"> And a huge leap in battery life.</span>
    <span tg-name="opacity" tg-filter="6,7"tg-map="6: 0.3;7: 1"tg-follow="container"> Let’s Pro.</span>
    <br>
    <span tg-name="opacity" tg-filter="7,8"tg-map="7: 0.3 ;8: 1" style=" font-size: 24px ">
        From $41.62/mo. for 24 mo. or $999 </span>

```

> 利用TriggerJs库中的tg-from， tg-filter，tg-map，tg-follow
>
> 通过 CSS 变量，获取制作页面滚动动画所需的值，毋须编写任何 JavaScript 代码。
>
> tg-name 为接收滚动值的 CSS 变量名称，是否加上 `--` 前缀都可。
>
> tg-from 根据页面卷动情况由from处逐渐增加
>
> tg-map 将一个值映射至另一个值。格式：`value: newValue; value2: newValue2`。也支持同时将多个值映射至另一个值：`value,value2,value3: newValue`
>
> tg-steps from与to 之间触发多少次
>
> tg-step 步长
>
> tg-filter   仅当滚动值在列表当中时才触发，格式：`1,3,5,7,9`。默认情况下，过滤模式是 `retain`（保留值），在设定值末端加入 `!`
>
> 很容易就实现了自己对于诸如
>

1. 文字缩小放大
2. 文字渐入
3. 文字亮灯效果
4. 文字跳转
5. 文字打字机模式打入
6. …….




