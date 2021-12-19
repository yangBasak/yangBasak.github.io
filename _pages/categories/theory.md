---
# layout: category는 한 카테고리만 보여준다. permalink에 /categories/카테고리명 형식으로 작성한다
# taxonomy는 이 페이지에 보여질 카테고리를 표기함
title: "이론 정리"
permalink: /categories/theory/
layout: archive
author_profile: true
taxonomy: theory
sidebar:
  nav: sidebar
---

{% assign posts = site.categories.theory %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
