---
title:  "界面设计之首页jeklly的架构"
modified: 2018-07-01 
categories: 
  - 界面设计
tags:
  - 笔记
classes: wide
excerpt: "学会架构JEKLLY，是你做网页的第一步"
header:
  overlay_image: /assets/images/marvel10.PNG.jpg
  teaser: /images/张杰学猫叫.gif
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  cta_label: "了解更多"
  cta_url: "https://unsplash.com"
---

{% include base_path %}

{% include toc title="目录" %}

### 首次修改jeklly设置档

- 首先：需要找到一个**.project**文件夹并且在里面添加以下图示代码：

![project](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/project.png){: .align-center}
- 其次，你需要找打到**_config.yml**文件夹，并且按照模板修改里面的一些代码，因为这个原模板并不是你自己的，如果不修改，在浏览器中打开就会产生乱码。

![navigation](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/navigation.png){: .align-center}
- 再然后，当你修改完之后，记得要做的一步就是根据yml格式更正对齐，对齐是很关键性的一步。

![navigation1](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/navigation1.png){: .align-center}


### 在导航栏中新增了导航
- 首先，你要先找到一个**data**文件夹，找到 **navigation.yml** 文件，并且根据自己的需要添加导航。值得一提的就是，在导航栏中可以添加内连接
，也可以添加外链接。外链接很简单，就是直接把网址粘贴在url上即可。
![home](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/home.png){: .align-center}

 > 接下来是内连接的导航搜索的架设：
 
- 要先在gitee destdop将**current branch**切换到**3.1.6**分支（因为这个文档是作者本身的，里面有很多MD档是我们需要的）。

- 然后在你之前folk的minimal-mistake 中的_post文档中复制几篇MD文档，最好是先在桌面新建一个，然后把复制的文章放进去，以免直接放在桌面上会很乱，而且还会出现被不小心删掉的情况。

- 复制完之后，就就将gitee destdop的current branch切换到master分支上，自己新建一个**_post**文档，将刚刚复制的文章放进去。这一步操作呢，是让你新增几个占位符，以便写文章。

![insert](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/insert.png){: .align-center}

![insert1](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/insert1.png){: .align-center}

- 如果你点开我的网页的话，你会发现我的导航栏有一个“关于我”的导航键，点进去，网址不会连接到新的网页，而是会跳转在内部，这就是内链。

- 和上一步骤一样，先在gitee destdop将current branch切换到3.1.6分支，找到minimal-mistake的_page中about.md，复制粘贴。

- 然后再跳转到自己的master，新建**_page**，然后把文章放在里面。

- 点进去修改基本信息。打开网页，如果你看到以下的页面，那恭喜你，成功了。而SVG制作这一栏的内导航也是相似的道理，只是要在原作者那个文档里面复制的
稳当不一样而已。

![insert2](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/insert2.png){: .align-center}

![insert3](https://gitee.com/NFUNM104/minimal-mistakes/raw/master/images/insert3.png){: .align-center}

### 导航栏添加搜索功能
- 如果你想要你的导航栏像其他浏览器那样具有搜索的功能，你可以自己设置：

```ruby
- 在_config.yml中寻找以下代码，将它开启
search                   : true # true, false (default)

```