---
layout: layouts/base.njk
title: Про проєкт VPO.WIKI
eleventyNavigation:
  key: Про проєкт
  order: 3
---
# Про проєкт VPO.WIKI

Проєкт реалізований волонтерами і не представляє жодних громадських організацій. Вся інформація взята з інтернету і може містити неточності. 


Бачите помилку або щось не працює, пишіть на пошту kthopos@hey.com

<ul>
{% for post in collections.post %}
  <li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
  <ul>
    {% for tag in post.data.tags %}
        {% if tag !== "Покровський район" %}
          <li><a href="/tags/{{ tag }}"> {{ tag }} </a></li>
        {% ending %}
    {% endfor %}
  </ul>
{% endfor %}
</ul>