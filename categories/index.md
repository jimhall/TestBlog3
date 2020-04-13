---
layout: default
title: Categories
---

<!-- Begin code @ categories/index.md -->

# Category listing

{% for category in site.categories %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url| relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

<!-- End code @ categories/index.md -->
