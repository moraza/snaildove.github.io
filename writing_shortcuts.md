---
title: 博客写作的模板
date: 2019-07-01
copyright: true
categories: 中文, english
tags: [Improving Deep Neural Networks, deep learning]
mathjax: true
mathjax2: true
toc: true
top: true
---

# <font color="#9a161a">1级标题</font>

## <font color="#9a161a">2级标题</font>

### <font color="#00000">代码</font>

#### <font color="#3399cc">Classification</font>

<p><center><font face="constant-width" color="#c67171" size=4><strong>WARNING 警告</strong></font></center></p>


## 替换链接

%s%[^!]\[\(.*\)\]\((.*)\)%<u><a style="color:#0879e3" href="\2">\1</a></u>%cg

## 替换文章引用


%s#^\(\[\d*]\) #<a name="\1"></a>\1#cg

%s%\([^#>!"]\)\(\[\d*]\)%\1<a href=" #\2">\2</a>%cg

#### 图片注释
<p><center><br/><center></p>

#### 说明
<img src="第二章-Spark是如何工作的.assets/image-20200508114357885.png" alt="image-20200508114357885" style="zoom:35%;" />

#### 警告

<img src="第二章-Spark是如何工作的.assets/image-20200506181840680.png" alt="image-20200506181840680" style="zoom:35%;" />

#### 提示

<img src="第一章-本书导论.assets/image-20200505172543872.png" alt="image-20200505172543872" style="zoom:45%;" />

#### 译者附

<p><center><strong>译者附</strong></center></p>

<font color="#32cd32"><strong>词汇</strong></font>
<font color="green"><strong>词汇</strong></font>
<font color="#9a1647">**MULTIPLE DATACENTERS**</font>

<p><center><font face="constant-width" color="#737373" size=4><strong>NOTE 注意</strong></font></center></P>

<center><strong>旁注</strong></center>

<p><font face="constant-width" color="#000000" size=3>术语</font></p>

## <font color="#8e0012">

### <font color="#f68a1e">

#### <font color="#0a7ae5">

提醒颜色
<font color="red">

笔记背景色
<font style="background:yellow;">

专有名词
<font style="color:#008000">

逻辑助记符
<font style="color:#0979e3">


修正中文冒号为英文冒号
%s%\(-[a-zA-Z]*\)：%\1:%cg

给虚拟机参数加代码，需要先执行本行之上的一个替换命令
%s%-\([a-zA-Z]*\):\([\.\+\-a-zA-Z\d]*\)%`-\1:\2`%cg

给包加代码提示符：
,$s%\([a-zA-Z\[]\+\)\([\.\/]\)\([A-Za-z\.\/()$]\+\)%`\1\2\3`%cg

<p style="font-family:Consolas;color:#000000;">
    Submitted Time: 2017/04/08 16:24:41</br>
    Duration: 2 s</br>
    Succeeded Jobs: 2
</p>

s#\([\w,-]\)\n#\1 #cg
s#\([?.]\)\n#\1\r\n\r\n#cg



%s#^\([^<]*\)<font style=\"background\:yellow;\">\(.*\)<\/font>\(.*\)\n#<p>\1<font style=\"background\:yellow;\">\2<\/font>\3<\/p>\n#cg


%s&^## <font.*>\(.*\)<\/font>&{% raw %}<h2 style="color:#9a161a">\1<\/h2>{% endraw %}&cg
%s&^### <font.*>\(.*\)<\/font>&{% raw %}<h3 style="color:#3399cc">\1<\/h3>{% endraw %}&cg
%s&^#### <font.*>\(.*\)<\/font>&{% raw %}<h4 style="color:#3399cc">\1<\/h4>{% endraw %}&cg


%s#<font style=\"background\:yellow;\">\([^<]*\)<\/font>#\1#cg

%s%<font color="#32cd32"><strong>\([^<]*\)<\/strong><\/font>%\1%cg

%s%<font color="#32cd32">\([^<]*\)<\/font>%\1%cg

%s%<font color="#000080">\([^<]*\)<\/font>%\1%cg

%s%<font color="#000080">\([^<]*\)<\/font>%<font color="#000080"><strong>\1<\/strong><\/font>%cg

%s%<font style="color:#EA7500">\([^<]*\)<\/font>%\1%cg

:%s#\*\*\([^*]*\)\*\*#<font style="background:yellow;">\1<\/font>#cg

Family	Response type	Supported links
Gaussian	Continuous	Identity*, Log, Inverse
Binomial	Binary	Logit*, Probit, CLogLog
Poisson	Count	Log*, Identity, Sqrt
Gamma	Continuous	Inverse*, Idenity, Log
Tweedie	Zero-inflated	continuous Power link function

<font color="#32cd32">\([^<]*\)<\/font>
