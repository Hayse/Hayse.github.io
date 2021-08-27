---
title: another page
description: another page with new
tags: [life,study,worker]
---

![Coming soon](/assets/img/comingsoon.jpg)

请在文件头添加“category”字段，，注意：值内容为life,study,worker这三个中的一个，如果要再添加，需注意配套相关index文件(_docs)

<h3>site.posts</h3>
  {% for post in site.posts  -%}
<div><a href="{{ post.url }}">{{ post.title }}</a></div>
 {%- endfor %}
<h3>site.docs</h3>
  {% for post in site.docs  -%}
<div><a href="{{ post.url }}">{{ post.title }}</a></div>
 {%- endfor %}
<h3>site.pages</h3>
  {% for post in site.pages  -%}
<div><a href="{{ post.url }}">{{ post.title }}</a></div>
 {%- endfor %}
