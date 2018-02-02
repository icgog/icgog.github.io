---
layout: page
permalink: /blog/
title: blog
description: Index
---

<ul class="post-list">
{% for post in site.posts reversed %}
    <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }} ({{ post.date | date: '%-d %b %Y' }})</a></h3>
     </li>
{% endfor %}
</ul>
