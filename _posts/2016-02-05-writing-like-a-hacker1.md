---
layout: post
title:  "Writing like a hacker"
date:   2016-02-05 19:08:12 +0800
categories: Programming
---
## 缘起
很早就有看到阮一峰和阳志平有提到过，在github上创建自己的blog，当时就很想尝试，觉得这种方式很酷。不过当时实在是技术小白，安装Jekyll各种纠结，各种搞不定，最后实在是觉得部署网站得都没心思写文章了。

另外当时scriptogr.am也真的是很漂亮很好用，也就决定不折腾了，直接在scriptogr上开写了。

只是没想到scriptogr在去年也关闭了。我网站的blog也随之荒废掉。

这次决定还是继续用markdown在网站上写文，有试用过farbox和简书，不过还是觉得有不顺的地方，很怀念那种单纯的写文字的感觉，加上真的很怀念用github的生活，于是决定继续折腾一把。

## 安装Jekyll
根据[jekyll的官方网站](http://jekyllrb.com/)，运行以下代码

``` 
$ gem install jekyll
~ $ jekyll new my-awesome-site
~ $ cd my-awesome-site
~/my-awesome-site $ jekyll serve
```
### 1.解决gem服务器问题
第一步gem install的时候，就发现连不上，  
提示 "Unable to download data from http://ruby.taobao.org/"。  
回想自己在rails girls活动中的经历，觉得应该是gem服务器连不上的问题，  
搜索google后，得到答案；

```
1.gem sources --remove http://ruby.taobao.org/
2.gem sources -a https://ruby.taobao.org/
3. 查看源对不对
gem sources -l 
```
顺利搞定。

### 2.解决没有安装权限的问题
运行gem install jekyll，结果提示我没有written的权利。  
这时候，猜想sudo应该可以解决。  
果然，sudo gem install jekyll后，顺利安装成功。

### 3.运行jekyll网站
顺利按照官方代码，在本机上运行出了自己第一个jekyll网站，心情特别开心，看来jekyll也不难的嘛。

## 在GitHub上建立自己的主页

在[jekyll的官方网站](http://jekyllrb.com/)上就有建立自己[GitHub Pages](http://pages.github.com/)的链接，  
里面有非常详尽的步骤，  
我也顺利的搭建了自己的GitHub主页 [zoejane.github.io](http://zoejane.github.io)  

看到网站从Error404变成了熟悉的“Hello，world!"，心情特别舒畅，  
而且我发现原来在GitHub上搭建主页居然这么简单，而且自主性也好强，顿时更坚定了在GitHub上安家的想法。

## 将Jekyll网站搬到GitHub上
将之前用jekyll创建的my-awesome-site文件夹，  
复制到GitHub的zoejane.github.io的repo下，  
打开网页zoejane.github.io，  
之前的Jekyll网站就从本地传到了互联网上啦。

## 在Jekyll上创建自己的第一个post
### 1.文章的书写
复制原来post文件夹下的默认文档，仿照其格式，将相应的标题、内容等替换成“hello,world”。  
以后自己写文章，就可以方便的在本地用markdown书写，然后方便的通过github存档和上传啦，想到这里，心情顿时很轻松。  
不过写完后发现，文章在网站上并没有显示出来。  
搜索了整理Jekyll的文件夹，也暂时不知道如何改起。

### 2.运行jekyll serve并同步
阅读默认的第一篇文章”Welcome to Jekyll!“，决定在本地先运行jekyll serve测试一下，发现自己的文章已经成功发布在本地网站上啦。   
然后在GitHub上同步，这时发现，运行jekyll serve后，网站文件夹下有些文件已经自动进行了相应的更新，使我新撰写的文章能够自动显示在网站上。  
同步后，测试zoejane.github.io，顺利运行成功，新的文章发布到互联网上去啦！

## 小结
一番折腾下来，发现也没有我想象中那么难。而且觉得markdown+github的形式，使用起来很清爽，自主性也很高，我觉得我还挺喜欢这种写作方式的。  
在GitHub上顺利安家，以后决定要多多练习写文章啦。  
我终于又有了一片让我自由书写的地方，感觉真好。我又回来啦！