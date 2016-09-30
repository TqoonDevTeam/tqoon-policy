---
layout: page
title: 개인정보
permalink: /privacy/
categories: ['privacy']
tags: ['privacy', 'nav-all']
---

<!--<ul class="nav">
     <li><a href="home/2016/01/01/ho-all.html">home, main</a></li> 
</ul>-->

<ul class="post-list">
    {% for post in site.categories.privacy reversed %}
      {% if post.tags[0] == 'all' %}
      <li>
        <span class="post-meta">{{ post.categories[0] }} / {{ post.categories[1] }}</span>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.code }} <span>{{ post.title }}</span></a>
        </h2>
      </li>
      {% endif %}
    {% endfor %}
</ul>
