---
title: "Python多态"
date: 2018-09-04T10:32:01+08:00
draft: true
# weight: 1
# aliases: ["/first"]
tags: ["python"]
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

```python
对象的多种形态
比如说动物，动物分为很多种但是动物都会吃东西，但是动物吃的东西又不一样
#  有三种动物：狗、猫、猪，
#	父类：动物、
#	子类：狗、猫、猪   可以添加子类自己的方法，自己扩展
#	动物的属性：动物的名字
#	动物的方法是eat（就是打印自己的名字）
#   有一个饲养员：饲养员
#	饲养员的方法：feed_animal(需要饲养的动物)
#		函数的实现是（其实就是调用动物的eat方法）
class Animal(object):
    name="动物"
    def eat(self):
        print("%s会吃东西"%(self.name))
class Dog(Animal):
    def eat(self):
        print("小狗吃骨头")

class Cat(Animal):
    def eat(self):
        print("小猫爱吃鱼")

class Pig(Animal):
    def eat(self):
        print("小猪不知道吃什么")


class Breeder(object):
    def feed_animal(self,animal):
        animal.eat()        

breeder=Breeder()
dog=Dog()
breeder.feed_animal(dog)
cat=Cat()
breeder.feed_animal(cat)
pig=Pig()
breeder.feed_animal(pig)

```