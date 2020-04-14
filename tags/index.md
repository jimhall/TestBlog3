---
layout: default
title: Tags
---

<!-- Begin code @ tags/index.md -->

# Tag listing

<div class="container">
<!-- {::nomarkdown} -->
{%- for tags in site.tags -%}
  {::nomarkdown}<a href="#{{ tags[0] }}"<h3 style="display:inline;">{{ tags[0] }}</h3></a>{::/nomarkdown}
{%- endfor -%}
<!-- {::/nomarkdown} -->
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
