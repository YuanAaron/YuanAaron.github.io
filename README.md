# 个人博客

这是我的个人博客项目，里面会记录生活和技术的点点滴滴。

博客地址：[http://www.coderap.com](http://www.coderap.com)

# 致谢
+ 感谢[Yummy-Jekyll](https://github.com/DONGChuan/Yummy-Jekyll)的原作者创作了如此漂亮的作品，但无奈我前端太菜，没有弄到我想要的效果
+ 感谢[pony-maggie](https://github.com/pony-maggie/machengyu.github.io-theme)对原主题所做的工作，我的博客正基于此。

# 使用

## 下载
点击右上角的fork， 把项目拷贝到自己的github仓库。然后通过git clone命令下载到本地电脑进行修改即可。

## 配置
主要的配置都在`_config.yml`，根据自己的实际情况配置即可。_includes目录下有些html文件也进去看看吧，可能你也需要改点东西。

## 关于统计
我个人不喜欢在前台页面展示访问数量，所以本项目只使用了百度统计。

百度统计是后台统计，并没有再页面有任何展示，但是可以通过登录百度统计官网查看更详细的访问记录分析。

当Fork本项目之后需要去百度统计官网申请自己的baidu统计ID替换 `_config.yml` 文件中的 `baidu_analysis`。

+ [百度统计](https://tongji.baidu.com)

## 关于评论

第三方的评论系统有不少，我这里使用的是gitalk。

>Gitalk 是一个利用 Github API,基于 Github issue 和 Preact 开发的评论插件。在 gitalk 的评论框进行评论时，其实就是在对应的 issue 上提问题。

关于gitalk的配置，下面这篇文章说得比较详细：

https://www.jianshu.com/p/78c64d07124d


## 如何写文章

在`_posts`目录下新建一个文件，可以创建文件夹并在文件夹中添加文件，方便维护。在新建文件中粘贴如下信息，并修改以下的`titile`,`date`,`categories`,`tag`的相关信息，添加`* content {:toc}`为目录相关信息，在进行正文书写前需要在目录和正文之间输入至少2行空行。然后按照正常的Markdown语法书写正文。

``` bash
---
layout: post
#标题配置
title:  标题
#时间配置
date:   2016-08-27 01:08:00 +0800
#大类配置
categories: document
#小类配置
tag: 教程
---

* content
{:toc}


我是正文。我是正文。我是正文。我是正文。我是正文。我是正文。
```

## 执行

``` bash
bundle exec jekyll clean
```

``` bash
bundle exec jekyll build
```

``` bash
# 本地运行
bundle exec jekyll serve
```

生成的_site目录就是你的博客站点的全部静态文件了，拷贝到web服务器下运行即可。


