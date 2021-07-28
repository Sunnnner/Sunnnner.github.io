---
title: "Shell 如何传参"
date: 2019-08-18T11:21:09+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["shell"]
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


```shell

# how to pass arguments to shell script 

# 利用echo打印你传入的参数
# 上面可以看到$0表示 我们运行sh文件的语句 ./demo.sh，这个不是一个我们提供的真实的参数。

# echo $0 $1 $2 $3 

# 换成args 数组方式去存储参数列表

args=("$@")
# echo ${args[0]} ${args[1]} ${args[2]} ${args[3]}
# 更简单的方法 $@可以表示传入的参数列表，直接打印出来
# echo $@

# 如何计算参数的个数
# $#可以存储参数的个数值
echo $#
```