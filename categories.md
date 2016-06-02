---
layout: page
title: "Categories"
permalink: /categories/
icon: "archive"
order: "4"
---

{% if site.categories != empty %}

  <ul class="tags-list">
    {% for cat in site.categories %}
      <a class="tags" href="#{{ cat[0] }}" title="{{ cat[0] }}" rel="tag"><i class="tags fa fa-folder fa-fw"></i> {{ cat[0] | join: "/" }} </a>
    {% endfor %}
  </ul>

  {% for cat in site.categories %}
  <ul class="tags-list">
    <h2 id="{{ cat[0] }}">{{ cat[0]}}</h2>
    {% for post in cat[1] %}
    <li>
      <a href="{{ post.url | prepend: site.baseurl }}" title="{{ post.title }}">
        {% if post.icon != null %}
          <i class="fa fa-{{ post.icon }}"></i>
        {% endif %}
        {{ post.title }}
      </a>      
      <i class="fa fa-calendar fa-fw"></i>
      <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date_to_string }}</time>
    </li>
    {% endfor %}
  </ul>
  {% endfor %}

{% else %}
  <h2>Empty</h2>
{% endif %}
