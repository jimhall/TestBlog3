---
layout: default
title: Tags
---

<!-- Begin code @ tags/index.md -->
<style>
.tagcloud {
    width: 90%;
    max-width: 1000px;
    margin:0 auto
}
</style>

# Tag listing

<div class="tagcloud">
{% for tags in site.tags %}
  <a href="#{{ tags[0] }}"><h3 style="display:inline;">{{ tags[0] }}</h3></a>
{% endfor %}
</div>

<p></p>

{% for tags in site.tags %}
  <a name="{{ tags[0] }}"><h3>{{ tags[0] }}</h3></a>
  <ul>
    {% for post in tags[1] %}
      <li><a href="{{ post.url| relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

<!-- End code @ tags/index.md -->
