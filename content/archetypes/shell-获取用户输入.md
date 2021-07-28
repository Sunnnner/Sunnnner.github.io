---
title: "Shell 获取用户输入"
date: 2019-08-17T11:20:41+08:00
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
# learn about how to read from user input

echo "Places input your name"

read name

echo "your had input name is $name"
# -p 是promote ，提示的意思就是可以让用户在提示语相同
# 一行输入内容
read -p "Please input a name" user_var
echo "your had input name is: $user_var"

# 模拟用户输入密码操作
read -p "place input you name" users_var
# -s一般在输入密码的时候启用可以输入过程看不到操作
read -sp "place input you password" pas_var

echo "you had input name is $users_var"
echo "you had input password is $pas_var"

```