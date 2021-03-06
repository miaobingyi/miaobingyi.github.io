# 个人文章更新的平台说明


<!--more-->



<!-- 分类文章参考

 "Books|读书"   "Episodes|影视"    "做事"   
  "Chat|扯谈"   Tutorials|教程
  
description: 文章内容的描述.

添加图片使用下面的代码，同时将图片放到/static/posts下

{{< figure src="/posts/test.jpg" title=""  >}}

 -->

## 写在前面的话

{{< admonition  type=warning title="声明" >}}
本文首发于[个人网站](https://miaobingyi.com/)，转载请保留本声明，请勿用于任何商业用途。
{{< /admonition >}}

写个人博客还存在一个问题：在哪个平台上面更新自己的文章？如何在不同的平台同步自己的文章？而且有的文章是系列文章，存在后续的更新。如何实现呢？

## 文章的主要平台和优缺点

现在主要的平台有：**微信公众号**、**简书**、**个人网站**、**技术博客**等。

微信公众号：基于[月活超过10亿](http://tech.sina.com.cn/i/2018-11-14/doc-ihmutuec0177001.shtml)的微信平台，也就意味着自己的文章可以很方便地在这一个巨大的生态面前展示，而且依托着便捷的支付方式、广告推广形式的多样化，甚至很容易让自己变现。

缺点：目前除了通过[搜狗微信搜索文章](https://weixin.sogou.com/)，无法被其他的搜索引擎检索。也就是说无法直接在外网搜到自己的文章，无法有效地形成自己的品牌效益，除非你自己在微信公众号里面或者自己其他平台上面大力推广。

个人网站、简书和技术博客 ：基本可以被搜索引擎检索，比较容易形成网络效应；个人博客的缺点是在手机端跳转查看其他链接和支付不方便，简书和技术博客的缺点就是两侧的相关文章太嘈杂，很容易被超链接不知引向何处。

## 不同平台的有机统一

所以对于更新系列的文章，自己选择的是[个人博客](https://miaobingyi.com/)。对于需要在不同平台分发的同一文章，自己利用的是Typora+自己修改的CSS文件导出富文本文件在微信公众号里面直接粘贴。而简书和个人博客都支持使用markdown写作。虽然简书和微信公众号都有自己的图床，但是考虑到个人博客的因素，自己直接使用的是[腾讯云COS作为存储桶](https://cloud.tencent.com/document/product/436/14106)搭建自己的图床。



## 参考资料

[1]. [利用Typora实现微信公众号文章一键排版](https://sspai.com/post/40524)

[2].[模板：常见的CSS文件](https://github.com/huanxi007/markdown-here-css)

[3].[可能吧的文章是如何排版的？](https://mp.weixin.qq.com/s?__biz=MjM5ODQwMjA4MA==&mid=2649293603&idx=1&sn=57f38200555dcba76d6358594416c089&scene=19#wechat_redirect)



## 尾巴
写是更好的思考，做是更好的证伪。本公众号/博客旨在自娱自乐，自总结每一段时间内的心路和学习的历程。 所有之前写的都可能之后被推翻、补充和修正。所以每一篇文章都（可能）是一个**Update**系列。典当过去，写点东西，典当自己，写点文字。每个人自己就是一部历史，研究不假设，反思不反悔。

本网站的**使用指北**以及幕后花絮，请转至：[Hello-World-2-My-Blog](https://miaobingyi.com/2018/hello-my-own-website/)

如果微信跳转观看不适，请使用浏览器阅读或欢迎关注**微信公众号**，与本博客**不同步**更新。

{{< figure src="/posts/mpQRcode.jpg" title="1.01的365次方公众号">}}

<center>  ---End---  </center>

本站[公益404页面](https://miaobingyi.com/404)，帮忙寻找遗失儿童！
