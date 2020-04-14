---
layout: default
title: Tags
---

<!-- Begin code @ tags/index.md -->
<style>
sitetags {
    background: rgba(0, 0, 0, 0.1);
    width: 100%;
    border-top: 1px dashed #b5e853;
    padding: 10px 0;
    margin:0 0 40px 0
}

sitetags h3 {
    left: 0;
    bottom: 0;
    width: 100%;
    text-align: center;
    font-size: 14px;
    font-weight: 300;
    color:#666
}
</style>

# Tag listing

<div class="sitetags">
{% for tags in site.tags %}
  <a href="#{{ tags[0] }}"><h3 style="display:inline;">{{ tags[0] }}</h3></a>
{% endfor %}
</div>

{% for tags in site.tags %}
  <h3>{{ tags[0] }}</h3>
  <ul>
    {% for post in tags[1] %}
      <li><a href="{{ post.url| relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

<!-- End code @ tags/index.md -->
