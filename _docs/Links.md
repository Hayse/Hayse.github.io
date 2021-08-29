---
title: Links
description: Exchange link and Website navigation.
donav: 30
---

欢迎各位朋友与我建立友链，如需友链请发留言，我看到留言后会添加上的，本站的友链信息如下

```
名称：{{ site.title }}
描述：{{ site.description }}
地址：{{ site.domainUrl }}{{ site.baseurl }}
LOGO：{{ site.domainUrl }}{{ site.baseurl }}/favicon.ico
```

{% for tag in site.data.links  -%}
  <h3>{{ tag.part | capitalize }}</h3>
  <div class="links">
  {%- for link in tag.sites %}
      <a href="{{ link.url }}" target="_blank" class="link">{{ link.name }}</a>
  {%- endfor %}
  </div>
{%- endfor %}
