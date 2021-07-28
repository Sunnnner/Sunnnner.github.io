---
title: "Shell 文件测试操作"
date: 2019-08-20T11:22:13+08:00
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
#! /bin/bash
# file test operators

# 检查文件是否存在 -e 表示empty 默认文件是不为空
echo -e "Enter the name of file: ~"
read filename

# 注意括号内空格 -e 就是exist的意思,表示文件是否存在
if [ -e $filename ]
then
    echo 'File found'
else
    echo 'file is not exist or not found'

fi

# 检查是否是常规文件或者目录
-f表示file 判断是否是常规的文件
if [ -f $filename ]
then
    echo "$filename found"
else
    echo "$filename is not exist or not fount"
fi

# 检查文件是否是空

if [ -s $filename ]
then
    echo "$filename is not empty"
else
    echo "$filename is empty"
fi

```