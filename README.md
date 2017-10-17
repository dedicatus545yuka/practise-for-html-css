# practise-for-html-css
魅族官网页面的一些练习（HTML，CSS）
### 写是写的差不多了，但是最后一个效果没实现。。。。那就只能是明天再传上来了-_-ll  
### 其实说难也不难，效果做出来再进行调试，到正确的位置，那整个页面就会好看很多了  
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>页头</title>
    <link href="http://a4.qpic.cn/psb?/V118JuTr3rHMrA/1Vvd9V3.kdDArJBEL2sDiCL79cJsDCTss*cUntnJiLY!/m/dPMAAAAAAAAA&bo=IAAgAAAAAAADByI!&rf=photolist" rel="shortcut icon" type="image/x-icon">
    <link href="http://a4.qpic.cn/psb?/V118JuTr3rHMrA/1Vvd9V3.kdDArJBEL2sDiCL79cJsDCTss*cUntnJiLY!/m/dPMAAAAAAAAA&bo=IAAgAAAAAAADByI!&rf=photolist" rel="icon" type="image/x-icon">
    <!-- 设置页顶的一个小图标-->
    <meta name="Keywords" content="魅族手机官网商城、魅族官方在线商店、魅族在线商城、魅族官网在线商店、魅族商城">
    <meta name="description" content="魅族在线商城是魅族面向全国服务的官方电商平台，提供魅族PRO系列、MX系列、魅蓝（Note）系列的手机、配件和智能硬件的预约和购买。官方正品，全场包邮。">
    <!-- 设置关键字和页面描述从而利于搜素引擎的抓取 -->
    <meta http-equiv="x-ua-compatible" content="ie=edge">
    <!-- 兼容ie浏览器 - 固定的 -->
    <link rel="stylesheet" href="页头.css">
</head>
<body>
<div class="zwrq">
    <div class="zrq">
        <div class="nrq1">
            <a class="1-link" href="#">
                <i class="logo"></i>
            </a>
        </div>
        <div class="nrq2">
            <ul class="yb">
                <li class="sst ybli">
                    <input type="text" placeholder="魅蓝6">
                    <i class="sous">
                        <!-- 这里是通过i标签来达到引入图片的效果 -->
                    </i>
                </li>
                <li class="rt ybli">
                    <a href="#" class="rt1"><img src="http://a4.qpic.cn/psb?/V118JuTr3rHMrA/eST.kte*G4ruypQRZwytr3aw1yaAsqS*01TzKfZNtyk!/m/dPMAAAAAAAAA&bo=MAAwAAAAAAADByI!&rf=photolist"></a>
                </li>
                <li class="gwc ybli">
                    <a href="#" class="gwc1">
                        <i class="gwc2"></i>
                        <!-- 用于插入图片 -->
                    </a>
                    <span class="gwc3">0</span>
                </li>
            </ul>
        </div>
        <div class="nrq3">
            <ul class="dhb">
                <li class="dh"><a class="dhl" href="#">魅族商城</a></li>
                <li class="dh"><a class="dhl" href="#">魅蓝手机</a></li>
                <li class="dh"><a class="dhl" href="#">魅族手机</a></li>
                <li class="dh"><a class="dhl" href="#">魅族声学</a></li>
                <li class="dh"><a class="dhl" href="#">智能配件</a></li>
                <li class="dh"><a class="dhl" href="#">服务</a></li>
                <li class="dh"><a class="dhl" href="#">专卖店</a></li>
                <li class="dh"><a class="dhl" href="#">flyme</a></li>
                <li class="dh"><a class="dhl" href="#">社区</a></li>
            </ul>
        </div>
    </div>
</div>
<!-- 给页面设置外中内三大容器 -->
</body>
</html>
```

`页头.css`

```CSS
body {
    margin: 0 auto ;
    /* 解决默认8px的问题*/
    font-family: "PingFang SC", "\5FAE\8F6F\96C5\9ED1", "Microsoft Yahei", Arial, Helvetica, sans-serif, "\5B8B\4F53";
    font-size: 14px;
    min-width: 1240px;
    min-height: 100%;
    /* 设置了字体的样式大小和最小的高度宽度 */
}
@font-face {
    /* 定义网络字体的字体系列名称 */
    font-family: layout-font;
    /* 引入指定的网络字体文件 */
    src: url(https://store.res.meizu.com//layout/font/iconfont-7fe3aaa151.eot);
    src: url(https://store.res.meizu.com//layout/font/iconfont-7fe3aaa151.eot#iefix) format("embedded-opentype"), url(https://store.res.meizu.com//layout/font/iconfont-d91c6d8c6e.woff) format("woff"), url(https://store.res.meizu.com//layout/font/iconfont-43e1f7b40d.ttf) format("truetype")
}
.zwrq {
    height: 80px;
    border-bottom: 1px solid #efefef;
}
/* 给最外容器设置高度80px */
.zrq {
    width: 80%;
    margin: 0 auto;
    /*设置中容器的基本数值并让其居中，高度由内容撑起*/
    overflow: hidden;
}
.logo {
    font-family: layout-font !important;
    font-size: 115px;
    color: #00c3f5;
    /* 设置字体样式属性和颜色 */
    position: absolute;
    top: -16px;
    /* 开启定位调整元素的偏移量 */
}
.logo::before {
    content: "\E608";
}
/* 设置伪元素 */
i {
    font-style: normal;
}
/* 改变I标签带来的斜体样式 */
.nrq2,.nrq3 {
    height: 80px;
    margin: 0;
    padding: 0;
    font-weight: 400;
    /* 给内容器添加基本的样式 */
    float: right;
    /* 设置元素右浮动与其他内容器水平排列 */
}
.yb {
    list-style: none;
    /* 去除无序列表的黑点样式*/
    height: 80px;
    /* 解决高度塌陷的问题 */
    margin-top: -1px;
    /* 设置偏移量让元素垂直居中 */
}
.ybli {
    float: left;
    /* 设置浮动让元素水平排列 */
    padding: 30px 17px 0;
}
.sst {
    height: 30px;
    border-radius: 20px;
    /* 给div元素添加圆角的边框 */
    padding: 0;
    margin: 25px 17px 30px;
    width: 180px;
    text-align: right;
    /* 把文本框排列到右边 */
    white-space: nowrap;
    /* 规定段落中的文本不进行换行 */
    border: 1px solid #e5e5e5;
    line-height: 28px;
    vertical-align: middle;
}
input {
    vertical-align: middle;
    /* 设置元素垂直居中 */
    border: none;
    outline: 0;
    /* 文本输入框当获取焦点时 - 设置没有边框效果 */
    width: 135px;
    height: 20px;
    margin-left: 15px;
    font-size: 12px;
    line-height: 20px;
    color: #333;
}
.sous {
    font-family: layout-font !important;
    vertical-align: middle;
    font-size: 18px;
    cursor: pointer;
    /* 鼠标样式改为手指 */
    margin-right: 9px;
}
.sous::before{
    content: "\E634";
    /* 设置一个搜索框的图片 */
}
img {
    display: block;
    width: 24px;
    /* 将图片显示为块级元素以便设置图片的大小 */
}
.gwc1 {
    display: inline-block;
    vertical-align: middle;
    width: 24px;
    height: 24px;
    line-height: 24px;
    color: #666;
    text-decoration: none;
    /* 给购物车图片设置一些基本的样式 */
}
.gwc2 {
    font-family: layout-font !important;
    margin-left: -5px;
    font-size: 30px;
    /* 设置字体的样式，其实就是显示的图片的样式 */
}
.gwc2::before{
    content: '\E635';
    /* 通过伪元素改变字体的显示 */
}
.gwc3 {
    position: relative;
    left: -20px;
    top: -2px;
    /* 设置偏移量调整数字位置 */
    width: 100%;
    height: 100%;
    color: #e02b41;
    font-size: 12px;
    line-height: 14px;
    /* 给元素设置一些基本的样式 */
    text-align: center;
}
.nrq3 {
    position: relative;
    left: 50px;
    /* 开启定位设置偏移量让内容3往右靠一点 */
}
.dhb {
    margin: 0;
    padding: 0;
    list-style: none;
    font-weight: 400;
    /* 给整个表设置一些样式，取消前面的点 */
}
.dh {
    float: left;
    margin: 0 10px;
    /* 给li设置浮动让它们脱离文档流可以水平排列和可以设置高宽什么的 */
}
.dhl {
    /* 这是导航link，看成1就完蛋*/
    text-decoration: none;
    color: #333;
    height: 80px;
    line-height: 80px;
    /* 给a标签设置基本样式 */
}
.dhl:hover {
    color: #00c3f5;
}
/* 给元素设置伪类改变鼠标指向元素时的颜色 */
```
### 放下一些思路图和效果图  
![项目头部内容分析图](http://a1.qpic.cn/psb?/V118JuTr3rHMrA/5GJuhwf3u*Dln8PV7WwUN2agsQnrkyT.nh9lTWl*PgI!/b/dPMAAAAAAAAA&bo=GwWAAgAAAAADALk!&rf=viewer_4)
![页面头部相关功能分析图](http://a3.qpic.cn/psb?/V118JuTr3rHMrA/Ymf7eafdQU5LPzCiwuguRQxI2xDCDqetOH*LWtV4n5k!/b/dPIAAAAAAAAA&bo=GwWAAgAAAAADB74!&rf=viewer_4)
![效果图](http://a1.qpic.cn/psb?/V118JuTr3rHMrA/rjENsDuKtuOhCglW8RVqjPAUgeCq7bRJUQopZVBudUU!/b/dPMAAAAAAAAA&bo=KguQAAAAAAADAJQ!&rf=viewer_4)



