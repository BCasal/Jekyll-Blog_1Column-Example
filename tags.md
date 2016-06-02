---
layout: page
title: "Tags"
permalink: /tags/
icon: "tags"
order: "3"
---

{% if site.tags != empty %}

  <ul class="tags-list">
    {% for tag in site.tags %}
      <a class="tags" href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="tag"><i class="fa fa-tag fa-fw"></i> {{ tag[0] }} </a>
    {% endfor %}
  </ul>

  {% for tag in site.tags %}
  <ul class="tags-list">
    <h2  id="{{ tag[0] }}">{{ tag[0] }}</h2>
    {% for post in tag[1] %}
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
