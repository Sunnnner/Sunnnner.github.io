---
title: "什么是RPC"
date: 2019-09-07T11:36:55+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["linux"]
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

RPC

    远程过程中调用(RPC) 是一种协议， 程序可使用这种协议向网络中的另一台计算机上的程序请求服务

    RPC采用客户机/ 服务器模式， 请求程序就是一个客户机， 而服务提供程序就是一个服务器

    first 客户机调用进程发送一个有进程参数的调用信息到服务进程，然后等待应答信息

    second 在服务端， 进程保持睡眠状态知道调用信息到达为止， 当一个调用到达， 服务器或得晋城参数， 结果， 发送答复信息， 然后等待下一个调用信息

    next 客户端调用进程接受答复信息， 或得进程结果， 然后调用执行继续进行

为什么要使用API

    系统之间为了调用数据
    数据的传输格式：json, xml
