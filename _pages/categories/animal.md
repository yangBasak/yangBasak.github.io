---
# layout: category는 한 카테고리만 보여준다. permalink에 /categories/카테고리명 형식으로 작성한다
# taxonomy는 이 페이지에 보여질 카테고리를 표기함
title: "반려동물 입양 앱"
permalink: categories/animal
layout: archive
author_profile: true
taxonomy: project
sidebar:
  nav: sidebar
---

{% assign posts = site.categories.animal %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
