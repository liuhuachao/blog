---
layout: post
title: Entity/Model/DTO 等用法区别
categories: [EntityFramewor]
description: Entity/Model/DTO 等用法区别
keywords: entity,model,dto,bean,pojo,ejb
---

## Entity

    数据表对应到实体类的映射


## Model

    Model是MVC中一个概念，可能不和Entity一一对应，因为展示在View层中数据可能是一个Entity的精简，也可能是多个Entity的组合。

    Model是一个高度优化组合或者精简后的一个用于在View层展示数据的对象。

## DTO

    数据传输对象（Data Transfer Object）。

    用于系统间数据传输的对象，数据传输目标往往是数据访问对象从数据库中检索数据。

## Bean

    对于Bean而言，只要是Java的类的就可以称为一个Bean，

    更用在Spring上，被Spring管理的对象就可以将其称作为Bean。

    它不仅仅可以包括对象的属性以及get,set方法，还可以有具体的业务逻辑。

## POJO

    简单Java对象，貌似没有经常提到或作为类的后缀存在？

    其特点是：除了属性和get、set方法外不包含具体的业务逻辑方法，这个和上文表述的Model很相像，和Entity区别在于没有和数据表中字段一一对应。


## EJB

    即EnterpriseBean，也就是Enterprise JavaBean（EJB）。

    被称为Java企业Bean，是java的核心代码，

    分别是会话Bean（Session Bean）、实体Bean（Entity Bean）、和消息驱动Bean（MessageDriven Bean）。