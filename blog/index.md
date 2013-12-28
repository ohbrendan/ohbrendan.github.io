---
layout: blog
title: Blog
---

{% for p in site.tags.blog-post limit: 5 %}
  {% assign post = p %}
  {% include render-news-item.html %}
{% endfor %}

# Previous Posts
<ul class="post-list">
  {% for p in site.tags.blog-post limit: 30 %}
  <li>
    <a href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a>
    <span class="date">( {{ p.date | date: "%A, %B %d, %Y" }} )</span>
  </li>
  {% endfor %}
</ul>
