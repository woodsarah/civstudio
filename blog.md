---
layout: default
title: blog
permalink: /blog/
---

<div class="header-bar">
  <h1>blog</h1>
  <br/>
  <hr>
  <br/>
</div>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
		<br/>
        <hr/>
    </li>
  {% endfor %}
</ul>