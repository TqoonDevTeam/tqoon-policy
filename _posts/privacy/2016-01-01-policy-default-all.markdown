---
layout: post
code: "<i></i>"
title: "개인정보"
date: 2016-01-01 12:00:00 +0900
categories: ['privacy', 'default']
tags: ['all']
---
 
<a href="/tqoon-policy/">HOME</a> > <a href="/tqoon-policy/privacy/">개인정보</a>

<ul class="post-list">
    {% for post in site.categories.function-define reversed %}
      {% if post.categories[1] == 'about' and post.tags[0] <> 'all' %}
      <li>
        <span class="post-meta">{{ post.categories[0] }} / {{ post.categories[1] }}</span>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.code }} <span>{{ post.title }}</span></a>
        </h2>
      </li>
      {% endif %}
    {% endfor %}
</ul>