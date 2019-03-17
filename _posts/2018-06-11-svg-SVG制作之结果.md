---
title:  "SVG制作之SVG总的动图"
classes: wide
excerpt: "不管走多远，最后还是会回到起点--等你"
header:
  overlay_image: /images/sj-baren-714643-unsplash.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "了解更多"
  cta_url: "https://unsplash.com"
  
  sidebar:
  nav: "docs"
---

{% include base_path %}

{% include toc title="目录" %}
{% include gallery caption="This is a sample gallery with **Markdown support**." %}


### SVG的动画效果
- svg动图其实就是SVG矢量图加上CSS动画的总的效果。这篇文章中，我运用了animation的两种效果，看起来还不错。

<head>
 <meta charset="UTF-8">
 <style> 
 .animation-fill-mode {
     width:100px;
     height:100px;
     background:#800000;
     position:relative;
     animation:myfirst 5s infinite;
     animation-direction:alternate;

    }

@keyframes myfirst
{
0%   {background:#F5DEB3; left:0px; top:0px;}
25%  {background:#556B2F; left:200px; top:0px;}
50%  {background:#F08080; left:200px; top:200px;}
75%  {background:#800000; left:0px; top:200px;}
100% {background:#28505D; left:0px; top:0px;}
}

@-moz-keyframes myfirst /* Firefox */
{
0%   {background:#F5DEB3; left:0px; top:0px;}
25%  {background:#556B2F; left:200px; top:0px;}
50%  {background:#F08080; left:200px; top:200px;}
75%  {background:#800000; left:0px; top:200px;}
100% {background:#28505D; left:0px; top:0px;}
}

@-webkit-keyframes myfirst /* Safari and Chrome */
{
0%   {background:#F5DEB3; left:0px; top:0px;}
25%  {background:#556B2F; left:200px; top:0px;}
50%  {background:#F08080; left:200px; top:200px;}
75%  {background:#800000; left:0px; top:200px;}
100% {background:#28505D; left:0px; top:0px;}
}

@-o-keyframes myfirst /* Opera */
{
0%   {background:#F5DEB3; left:0px; top:0px;}
25%  {background:#556B2F; left:200px; top:0px;}
50%  {background:#F08080; left:200px; top:200px;}
75%  {background:#800000; left:0px; top:200px;}
100% {background:#28505D; left:0px; top:0px;}
}
</style>
</head>
<body>
<div class="animation-fill-mode"></div>

</body>















### animation-timing-function效果


<head>
   <meta charset="UTF-8">
   <style> 
    .animation {
      width:100px;
      height:100px;
      background:#800000;
      position:relative;
      animation:mymove 5s infinite;
      animation-timing-function:linear;
    }

@keyframes mymove
{
from {left:0px;}
to {left:200px;}
}

@-webkit-keyframes mymove /* Safari and Chrome */
{
from {left:0px;}
to {left:200px;}
}
</style>
</head>
<body>
<div class="animation"></div>
</body>
