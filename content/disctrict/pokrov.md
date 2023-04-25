---
layout: layouts/base.njk
---
# Гуманітарні центри в Покровському районі

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