---
title:  "界面设计之链接的修改和替换"
modified: 2018-07-01 
categories: 
  - 界面设计
tags:
  - 笔记
classes: wide
excerpt: "页面边栏的链接，可以让你高效快速的去找到你想要的东西"
header:
  overlay_image: /assets/images/design2.jpg
  teaser: /images/张杰学猫叫.gif
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "了解更多"
  cta_url: "https://unsplash.com"
---

{% include base_path %}

{% include toc title="目录" %}

### 侧边栏链接的故事

- 侧边栏，主要放置在页面的左边，一般的网站会将它设置成空白，但大部分还是会将它作为一个类似导航的功能来使用，因为毕竟还是有它的好处在的。
一般侧边栏能够显示作者个人资料，比如：姓名、电话、邮箱和社交链接等等。
- 如果你想要开启侧边栏显示的功能的话，你可以进行设置**首页显示author**的操作。（如图所示）

![side](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side.png){: .align-center}

- 更好的是，在进行上面的步骤成功的情况下启用它**_config.yml**。

```ruby
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      author_profile: true

```
![side1](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side1.png){: .align-center}

 > 如果要禁用特定帖子或页面的作者侧栏配置文件，请添加**author_profile: false**到**index.html**，或者一开始就直接不要生效它。
 
 - 当你看到我的第一张截图，你可能会发现，我的侧边栏不仅有一些大家都有的链接（或者是源文件自带的）比如：邮箱、微博等等，还新添加了其他的，
比如：- [`Fontawesome`](https://fontawesome.com/icons?d=gallery)和- [`Reddit`](https://www.reddit.com/user/username)，要实现这样的效果并不是很难。

- 现在先在**_cinfig.yml**文件中把一些基本的社交链接生效。
 > 注意：一定要注意对齐、地址正确、要看看地址有没有增加“”。

![side2](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side2.png){: .align-center}

- 新增外链接：
 > 首先，需要打开**_includes/author-profile-custom-links.html**。并添加<li>下面显示的相应标记。
 
 ```ruby
<li>
  <a href="https://fontawesome.com/icons?d=gallery">
    <i class="fab fa-accessible-icon"></i>Fontawesome
  </a>
</li>

```

![side3](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side3.png){: .align-center}

- 一般这些外链接的图标都是黑色的，如果你想要将它变换颜色，也是可以实现的。你需要打开**_utilities.scss**找到_sass.social-icons，然后在下面添加代码即可。

![side4](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side4.png){: .align-center}

![side5](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side5.png){: .align-center}

 > 添加代码的时候注意要空一行。
 
 ```ruby
.fa-reddit {
    color: #ff4500;
  }

```

![side6](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side6.png){: .align-center}

### 底边社交链接的故事
- 和侧边栏一样，文章的底部也有一些社交链接，以便在Twitter，Facebook，Google +和LinkedIn上进行共享。主题附带最常见社交网络的默认值。

- 如果想添加，删除或更改这些默认链接的顺序，可以通过编辑来完成**_includes/social-share.html**。

![side8](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side8.png){: .align-center}

- 要更改按钮的颜色，可以创建一个新的按钮类来匹配您想要的任何颜色。

![side9](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side9.png){: .align-center}

- 最终效果：

[side10](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/side10.png){: .align-center}















