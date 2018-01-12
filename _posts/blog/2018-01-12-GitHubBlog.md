---
layout: post
title: "Github 三部曲之 个人独立博客网站篇"
description: "用GitHub + Jeklly 建独立博客"
category: blog
---

# Github 三部曲之 个人独立博客网站篇

GitHub 作为一个开源社区，除了给程序员用着开源社区编码，还能给普通大众用来干点别点什么吗？

2017年自己学着用 GitHub + Jeklly 做了一个独立博客，整理简单的步骤，供同好者参考。

## Why

### 为什么要建一个独立博客？

自由的分享有的一切。（参考：[我为什么写博客](http://beiyuu.com/why-blog)) 


### 为什么要用 GitHub ？

GitHub 创始人的文章 [像黑客一样写博客](http://tom.preston-werner.com/2008/11/17/blogging-like-a-hacker.html)

让人不再担心备份与远程协作，一切提交，均有记录。

不用购买单独服务器空间。

> 工具远远不止是工具。它是一种「用手思考」的工作方式；它用「技术+设计」不动声色地改变了世界，再经由工具实施「教育」，润物细无声。但你要看见那雨丝，赞叹这造物。—— 许豆浆

### 为什么要用Jeklly？（此段可以忽略）

Jekyll的核心其实就是一个文本的转换引擎，用你最喜欢的标记语言写文档，可以是Markdown、Textile或者HTML等等（我用的Markdown），再通过layout将文档拼装起来，根据你设置的URL规则来展现，这些都是通过严格的配置文件来定义，最终的产出就是web页面。
基本的Jekyll结构如下：
|-- _config.yml |-- _includes |-- _layouts | |-- default.html | -- post.html |-- _posts | |-- 2007-10-29-why-every-programmer-should-play-nethack.md |-- 2009-04-26-barcamp-boston-4-roundup.md |-- _site -- index.html

## How
 
### 网站肉身
 
 1、 申请GitHub 账号 （注意这里的用户名会和你后面 仓库里的 username.github.io 的一样）
    如：我的用户名是 violettianjie。
 
 2、 新建仓库repositories 。仓库名和你上一步的username一样。完成后在浏览器里访问violettianjie.github.io，可以看到简单的页面。
 （此步参考官方[help文档](https://pages.github.com))
 
 3、 服务端的仓库克隆即fork （ 这是GitHub 鼓励和允许的，对于原仓库Owner来说，鼓励别人Fork自己的仓库，通过PullRequest给自己的仓库做贡献，也能提高了自己仓库的知名度。）别人的网站仓库。我fork的仓库 https://github.com/camscofie/camscofie.github.io（源码来源 http://beiyuu.com/。）
 
 4、在仓库code里修改、删除多余，改成自己的内容。
 
### 你的名字你做主
 
如果你希望自己的博客有独立的域名，需要如下步骤：

 
 1、 选一个好记的域名（费用会因为你选择的域名不同而不同），购买申请自己的域名（可以选择Godaddy 或者 [DNSPod](https://www.dnspod.cn)，我用的后者）。比如：我的域名violettianjie.com。
 
 
 2、 解析域名。
 
 3、 实名认证，上传身份证相关材料。
 
 4、 在 GitHub 仓库里绑定域名
 
 在设置下方激活 GitHub Pages 。
 
### 评论

如果要比较好的交互，那么可以增加 [Disque](http://disqus.com) 评论。这个需要用到vpn，推荐 付费的 [ExpressVPN](https://www.xpress-vpn.com)

## Then

完成以上，最重要的就是写啦，写作我会用 Markdown 格式（我用的Mweb Lite 软件），专注内容，比word等更高效， 生长你自己的内容树。然后可以通过Github 客户端或者网页版更新内容。 

以我的博客为例：

要用当前的模板，发布文章就在 _posts/ 里面，要发布在 Blog/，就打开 Blog/，然后 creat new file,
violettianjie.github.io/_posts/Blog/ 后边接上日期和文件名.md， 比如2017-09-02-helloworld.md。（注意日期格式）

下面就是文章内容：
页头都要加如下内容：

layout: post

title: About Me

description: 关于我自己

category: blog

（前后加"---"，顶行不要有空行。）



这样你的独立博客会同步更新。



恭喜，第一个独立博客上线。



 
### ChangeLog 

1、 20180112 ： 田捷创建

