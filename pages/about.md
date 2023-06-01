---
layout: page
title: About
description: 生活即是艺术
keywords: 碎碎念, Wei
comments: true
menu: 关于
permalink: /about/
---

我是vv。。。。

行万里路，读万卷书。

 记录生活与工作的点滴。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'weipeng.co' %}
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
