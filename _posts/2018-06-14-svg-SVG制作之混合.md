---
title: "SVG制作之SVG动图的混合篇"
categories: 
  - 网页设计
tags:
  - svg
classes: wide
excerpt: "因为兼容的问题，所以只能开设另外一个文档"
header:
  overlay_image: /images/header14.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "了解更多"
  cta_url: "https://unsplash.com"
sidebar:
  nav: "docs"
---

{% include base_path %}

{% include toc title="Getting Started" %}

### scale+transition-delay的混合效果：
- 因为兼容的问题，所以只能将这个混合的另外开设一篇文章放置。

<head>
  <meta charset="UTF-8">
  <style>
    .demo1:hover {
    transform: scale(1.5);
  }
	.demo1 {
	    width: 120px;
	    height: 120px;
	    background-color: #FFF8DC;
	    transition: width 1s;
	}
	.demo1:hover {
	    width: 400px;
	}
  </style>
</head>

<body>
<div class="demo1" >🥗</div>
</body>


### 过度并变色效果：
- 这个是加了CSS的scale元素，最终会达到消失的效果是因为我设置了悬停的颜色。

<head>
  <meta charset="UTF-8">
  <style>
    .demo3 {
	    width: 130px;
        height: 130px;
        background-color: #FFF8DC;
        transition: width 2s linear,
                    height 2s linear,
                    background-color 2s 2s;
	}
	.demo3:hover {
	    width: 200px;
        height: 200px;
        background-color: #28505D;
	}
  </style>
</head>

<body>
<div class="demo3" >💘</div>
</body>
<br/>

### scale的缩小效果：

<head>
  <meta charset="UTF-8">
  <style>
    .demo {
	    width: 110px;
        height: 110px;
		transition: all 0.5S;
        background-color: #800000;
	}
	.demo:hover {
	  transform: scale(0.5); 
	}
  </style>
</head>

<body>
<div class="demo">🈲</div>
</body>


### scale的移动效果：

<head>
  <meta charset="UTF-8">
  <style>
    .translate {
	    width: 100px;
        height: 100px;
        background-color: #800000;
	}
	.translate:hover {
	  transform: translate(-40px, -40px); 
	}
  </style>
</head>

<body>
<div class="translate">😂</div>
</body>

 > 当translate的两个值都是正的话，图形就会想右下角发现变化，相反的，如果两个都是负的，那么值就会向左上角发生变化，
 （别问我是怎么知道的，考试多（补考）了就知道了）
 
### **matrix**效果：

<head>
  <meta charset="UTF-8">
  <style>
    .matrix {
	    width: 100px;
        height: 100px;
        background-color: #800000;
	}
	.matrix:hover {
	  transform: matrix(1.678,-0.256,1.522,2.333,-51.533,-1.989); 
	}
  </style>
</head>

<body>
<div class="matrix">🤣</div>
</body>
