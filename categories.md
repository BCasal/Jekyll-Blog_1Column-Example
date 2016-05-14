---
layout: page
title: Categories
permalink: /categories/
icon: "folder"
---

{% if site.categories != empty %}

  <ul class="tags-list">
    {% for cat in site.categories %}
      <a class="tags" href="#{{ cat[0] }}" title="{{ cat[0] }}" rel="tag">{{ cat[0] | join: "/" }}</a>
    {% endfor %}
  </ul>

  {% for cat in site.categories %}
  <ul class="tags-list">
    <h2 id="{{ cat[0] }}">{{ cat[0]}}</h2>
    {% for post in cat[1] %}
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
