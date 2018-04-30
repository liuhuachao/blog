---
layout: page
title: About
description: 打码改变世界
keywords: 刘华超，故乡的风，博客，blog，Github
comments: true
menu: 关于
permalink: /about/
---

我是刘华超~仰望星空，脚踏实地！


## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
