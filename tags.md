---
layout: page
title: Tags
permalink: /tags/
icon: "tag"
---

{% if site.tags != empty %}

  <ul class="tags-list">
    {% for tag in site.tags %}
      <a class="tags" href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="tag">{{ tag[0] }}</a>
    {% endfor %}
  </ul>

  {% for tag in site.tags %}
  <ul class="tags-list">
    <h2  id="{{ tag[0] }}">{{ tag[0] }}</h2>
    {% for post in tag[1] %}
    <li>
      <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%d-%m-%Y" }}</time>
      <a href="{{ post.url | prepend: site.baseurl }}" title="{{ post.title }}">{{ post.title }}</a>
    </li>
    {% endfor %}
  </ul>
  {% endfor %}

{% else %}
  <h2>Empty</h2>
{% endif %}
