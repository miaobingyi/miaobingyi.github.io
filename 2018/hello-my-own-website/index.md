# 个人网站使用指北和花絮


<!--more-->


## 写在前面的话

{{< admonition  type=warning  title="声明" >}}
本文首发于[个人网站](https://miaobingyi.com/)，转载请保留本声明，请勿用于任何商业用途。
{{< /admonition >}}


本文档是对使用和浏览本博客的一个浅显导图，根据自己的蛋疼程度而保持文档更新。也是自嗨对博客网站Say Hello，用于文档排版的试验。

Hello，My Own Website!

## 个人网站使用指南

本博客网站主要是用于和外接互联网联系的一个中间站点。里面呈现的内容多是自己的学习笔记和一小丢丢生活杂感。而学习笔记部分自己又大多会以GitHub中Repository的形式存储，而GitHub对百度的爬虫又屏蔽了，所以个人博客是一个折中的提供搜索入口方案。



## 个人网站基本工具

### 网站的基础框架模板

网站的框架是从 [QiubaiYing](https://github.com/qiubaiying) folk的，感谢原作者。自己修改了里面个性化的参数，同时将打开网站的时候的icon换成了"苗"，以便自己标识。

2019.10.27 注：网站已经完全迁移到[Hugo](https://gohugo.io/)平台了。

2019.11.08 注：网站更名为XXX个人网站，因为自己不仅仅想写字，考虑开展图片专栏和视频等专栏。

### 网站的图床

使用的Markdown软件是：Typora，文档中使用的图床工具是**腾讯云COS**搭建的存储桶（如图1，访问速度还可以，这幅图的故事来自于：[一位叙利亚女孩的遭遇](http://time.com/13009/most-shocking-second-a-day/)）。

 2019年3月5日注：后期也有在用阿里云的OSS以及百度云的BOS功能。

使用的Markdown软件是：Typora，文档中使用的图床工具是腾讯云搭建的存储桶。

2019.10.27 注：现在基本只用[Visual Studio Code编辑器](https://code.visualstudio.com/)，配合各种插件真是太好用了。

网站主页的背景图是美剧**绝命毒师**中，老白和小粉在荒野*Cook*的写实图。（如图2:所示）

![腾讯COS存储桶作为图床](https://miaobingyigithubio-1251360589.cos.ap-chengdu.myqcloud.com/img404-bg.jpg)

<center>图1. 腾讯COS存储桶作为图床</center>



![](https://miaobingyigithubio-1251360589.cos.ap-chengdu.myqcloud.com/post-bg-desk.jpg)

<center>图2. 老白和小粉在荒野中Cook</center>

### 数学公式显示

在写论文的时候，接触到$ \TeX $和$ \LaTeX $，原来可以将公式用编译的方式表现出来，而不是机械地需要插入特殊字符。在文档的模板里面添加的是MathJax，它可以按照$ \LaTeX $的语法漂亮的显示数学公式。示例如下：

输入的内容：（为了防止$ \LaTeX $自动编译，这里仅仅示意双$符号里面的内容）

> \prod   \int  \bigcup   \bigcap  \iint  \iiint  \idotsint
>
> \approx   \sim   \simeq   \cong   \equiv   \prec   \lhd   \therefore
>
> \sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}

实际显示效果是：

$$  \prod   \int   \bigcup   \bigcap   \iint   \iiint   \idotsint$$

$$ \approx   \sim   \simeq   \cong   \equiv   \prec   \lhd   \therefore $$

$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$




### “添加赞赏”功能幕后花絮

在自己的每篇博客的末尾添加打赏的按钮，本来很简单的事情，自己硬生生花了将近8个小时。从最开始的自己在GitHub上面找到个人建站的一些模板，fork ,然后研究相近的网站上面的打赏的按钮的代码的不同。然后再在自己网站上面试运行。结果发现，虽然也是有一点模样，但是在打赏页面出来之后，支付宝和微信的扫一扫的二维码图像总是挨在一起。自己心里想，这一定是设置的格式的问题吧。

于是自己费尽很大的力气找到了设置这块格式的代码。

打开之后，一脸懵逼。HTML和CSS语言自己只是听过，完全没有接触过，自己就硬着头皮开始看。这个时候才意识到了在写代码的时候规范的代码和命名是多么的重要。自己勉强找到了控制按钮和图像的代码块，然后开始修改一些参数，常见的就是位置、大小等。

过程并不是特别的顺利，自己每次的修改都需要通过Github首先Commit然后等repositories刷新之后，自己疯狂地刷新自己的网站，然后再看网站修改之后的结果，自己对于自己真正修改的内容可能带来的变化没有任何的预判，以及对自己向什么方向修改也没有预判。自己就是在使劲的改，非常的受打击，晚上12:30自己都没有整出来。

**2019.10.27 注**：　已弃用，考虑到未来看到本篇文章很大可能不是电脑终端，所以扫码打赏的形式非常的愚蠢。自己的网站永远做不到微信公众号和支付宝动态的付款便捷，所以考虑之后弃用。

回寝室的路上，自己突然问自己这样一个问题：

> 我究竟在做什么？我怎么才能做到？

短暂的思考之后，自己的问题是：两幅图片的间距不符合自己的要求，自己应该首先看懂代码块里面讲述的关于边距的含义。所以接下来的问题是：

> 代码是什么意思？看着头大的究竟是什么语言？

CSS语言。接下来的问题是：

> CSS语言的基本语法是什么？我从哪里了解到？

CSS +菜鸟 +间距  关键字搜索，自己找到了先关的网页。

> margin，padding，border什么意思？
>
> 自己在看的代码的间距画出来是怎么样的？

就这样，自己慢慢分解问题，最后解决了（附录自己反复修改的代码块，自己画出的草图和最后的成果图）。

```css
<style type="text/css">		  
              .shang_payimg{width:140px; margin-left:80px; padding-left:15px;auto;  margin-rirht:50px;padding-right:5px;auto;border-radius:3px; height:140px;  display:inline-block;}		  
              .shang_payimg img{display:inline-block;padding-left:10px；margin-right:0px; float:right;text-align:center; width:140px;
			  height:140px; }			  
              .pay_explain{text-align:center;margin:10px auto;font-size:12px;color:#545454;}
              .shang_payselect{text-align:center;margin:0 auto;margin-top:40px;cursor:pointer;height:60px;width:500px;margin-left:110px;}
              .shang_payselect .pay_item{display:inline-block;margin-right:140px;float:left;}
              .shang_info-play{clear:both;}
              .shang_info-play p,.shang_info-play a{color:#C3C3C3;text-align:center;font-size:12px;text-decoration:none;line-height:2em;}
            </style>
```



![](https://miaobingyigithubio-1251360589.cos.ap-chengdu.myqcloud.com/20181017001.png)




## 其他思考

在看代码的过程中，表示`color`属性的参数是十六进制的数字，自己好奇心的将数字通过Google搜索，发现了一个[神奇的网站](https://www.color-hex.com/)，这个网站在你输入数字的时候，大面积都变成了你输入的数字代表的颜色。颜色=数字。数字化的一个生动体现吧。附录一张一窥。



![](https://miaobingyigithubio-1251360589.cos.ap-chengdu.myqcloud.com/20181017003.png)

首先搞清楚核心问题是什么？

分解问题，一步步解决。而非一上来不明所以地就想要直接KO.


## 测试新功能

[给文字的上方加字母或汉字]^(acdc & 拼音)



{{< admonition >}}
一个 **注意** 横幅
{{< /admonition >}}

{{< admonition abstract  >}}
一个 **摘要** 横幅
{{< /admonition >}}

{{< admonition info >}}
一个 **信息** 横幅
{{< /admonition >}}

{{<  admonition type=tip title="技巧" details=false >}}
一个 **技巧** 横幅
这是一条无聊的条幅，无所谓怎么写，但是这如果是引用的话，一条条的很好看。一个 技巧 横幅 这是一条无聊的条幅，无所谓怎么写，但是这如果是引用的话，一条条的很好看。一个 技巧 横幅 这是一条无聊的条幅，无所谓怎么写，但是这如果是引用的话，一条条的很好看。
{{< /admonition >}}

{{< admonition success >}}
一个 **成功** 横幅
{{< /admonition >}}

{{< admonition question >}}
一个 **问题** 横幅
{{< /admonition >}}

{{< admonition warning >}}
一个 **警告** 横幅
{{< /admonition >}}

{{< admonition failure >}}
一个 **失败** 横幅
{{< /admonition >}}

{{< admonition danger >}}
一个 **危险** 横幅
{{< /admonition >}}

{{< admonition bug >}}
一个 **Bug** 横幅
{{< /admonition >}}

{{< admonition example >}}
一个 **示例** 横幅
{{< /admonition >}}

{{< admonition quote >}}
一个 **引用** 横幅
{{< /admonition >}}

###  Youtube视频（WHY CODE）

{{< youtube nKIu9yen5nc >}}


###  纪念大学室友带自己看的人生第一个B站视频

{{< bilibili  id=BV1Nx411w7qW >}}




如果加载时间超过耐心时长，直接点击 {{< link href="https://www.bilibili.com/video/BV1Nx411w7qW" content=【金坷垃】千本垃 >}}






## 参考资料


[1]. [题图来源链接](http://angularjstutorials.net/bet/angularjs-hello-world/)


## 尾巴
写是更好的思考，做是更好的证伪。本公众号/博客旨在自娱自乐，自总结每一段时间内的心路和学习的历程。 所有之前写的都可能之后被推翻、补充和修正。所以每一篇文章都（可能）是一个**Update**系列。典当过去，写点东西，典当自己，写点文字。每个人自己就是一部历史，研究不假设，反思不反悔。

本网站的**使用指北**以及幕后花絮，请转至：[Hello-World-2-My-Blog](https://miaobingyi.com/2018/hello-my-own-website/)

如果微信跳转观看不适，请使用浏览器阅读或欢迎关注**微信公众号**，与本博客**不同步**更新。

{{< figure src="/posts/mpQRcode.jpg" title="1.01的365次方公众号">}}

<center>  ---End---  </center>

本站[公益404页面](https://miaobingyi.com/404)，帮忙寻找遗失儿童！
