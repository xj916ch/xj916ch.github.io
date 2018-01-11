---
layout: post
category: "kit"
title:  "jekyll + Github Pages设置"
tags: [jekyll,Github Pages]
---

参考：

[Github Pages + Jekyll 独立博客一小时快速搭建&上线指南](http://playingfingers.com/2016/03/26/build-a-blog/)

[搭建一个免费的，无限流量的Blog----github Pages和Jekyll入门](http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html)

[在Github上搭建Jekyll博客和创建主题](http://blog.csdn.net/garfielder007/article/details/50224513)

[怎么搭建个人博客网站——我的建站过程](https://www.cnblogs.com/shenjieblog/p/5060927.html)

[迁移博客图片者的福音：使用GitHub做免费不限流量图床](http://jingpin.jikexueyuan.com/article/36279.html)

### jekyll安装
1. 安装[Ruby](https://rubyinstaller.org/downloads/)，记得添加到环境变量。
2. 安装[RubyGems](https://rubygems.org/pages/download)，下载ZIP文件解压，输入：
```
$cd {unzip-path}
$ruby setup.rb
```
3. 安装jekyll，这里可以更改[Ruby源](https://gems.ruby-china.org/)。
```
$gem install jekyll
$gem install jekyll-paginate
```

### jekyll配置使用

- **jekyll使用**

```
$jekyll new blog
$jekyll server
```

浏览器打开http://localhost:4000/出现如下图所示，说明安装成功：
![image](https://github.com/xj916ch/xj916ch.github.io/raw/master/_posts/pictures/kit/jekyll-github-pages-environment-jekyll-default.png)

或者从http://jekyllthemes.org/里下载一个。

- **jekyll配置：**

1.时区设置

timezone: Asia/Shanghai

2.插入图片：

可以使用Github当作图床。

可以把图片放到blog下的_post目录。这里注意，图片外链地址tree需要替换为raw。

### Github Pages

新建一个github repository，命名为username.githug.io，不能放到其他repo下。

repo setting下找到Github Pages，只能是master branch。

其他一切如git操作。

push前可以使用`jekeyll server`在本地预览验证。

### 域名绑定