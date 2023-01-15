---
layout: page
title: Tags
---

{% assign manage_tag = site.pages | map: "manage_tag" %}
{% for tag in site.tags %}
  {% if manage_tag contains tag[0] %}
  <h3><a href="/tags/{{ tag[0] }}">{{ tag[0] }}</a></h3>
  {% else %}
  <h3>{{ tag[0] }}</h3>
  {% endif %}
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

