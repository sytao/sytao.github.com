---
layout: page
title: sytao.net
header: Thoughts, Writings and Dreams
---

不知道sytao.net这次是第几次复活了，之前的版本因为服务器到期，截图也没留下一个，这次我保证不会了，这次的最新版本，使用了 [Jekyll](https://github.com/mojombo/jekyll) 搭建，跑在了[Github](https://github.com) 上。不会在半路夭折了。除非域名到期忘记续费，否则这地方将永远存在下去。


#### 最近发布的文章

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>