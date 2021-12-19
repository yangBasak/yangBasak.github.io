---
title: "완독 리스트 앱"
permalink: categories/bookList
layout: archive
author_profile: true
taxonomy: project
sidebar:
  nav: sidebar
---

{% assign posts = site.categories.bookList %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
