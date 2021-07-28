---
title: "Github Page自定义域名开启https"
date: 2019-11-03T15:36:46+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["git"]
author: "whitek"
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "Desc Text."
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/Sunnnner/Sunnnner.github.io/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---

博主使用的cloudflare的cdn之前查了很久不清楚怎么使用github-page的https，
因github与Let’s Encrypt 合作提供自带cdn所以我们来配置一下，
首先关闭自定义域名的cdn服务其实就是关了他的域名解析

首先我们看域名还是active状态

其次我们关闭cloudflare站点cdn

查看站点状态

添加对github-Page的解析记录

如果github-Page你的Custom domain上已经填写了自定义域名，删除掉域名保存一下，随后再次输入一次保存你会看到你的https已经开启了
