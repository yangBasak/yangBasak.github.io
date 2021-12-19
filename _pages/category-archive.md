---
# layout: categories는 모든 카테고리 별로 글을 보여주는 템플릿
layout: categories
permalink: /categories/
title: "카테고리별 포스트"
author_profile: true
sidebar:
  nav: sidebar
---

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
{% assign posts = group_items[forloop.index0] %}

  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
