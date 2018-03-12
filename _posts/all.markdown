---
layout: post
title:  "全部文章"
date:   2018-04-01
categories: all
permalink: "/all.html"
---

{% assign weeklyPosts = site.posts | where: "categories", "weekly" | sort: "date" %}

<ul>
{% for post in weeklyPosts %}

  <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>

{% endfor %}
</ul>


