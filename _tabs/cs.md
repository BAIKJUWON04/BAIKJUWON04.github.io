---
title: CS공부
icon: fas fa-book
order: 4
---

{% assign posts = site.categories["CS공부"] %}

자료구조, 알고리즘, 운영체제, 컴퓨터구조, 네트워크, 데이터베이스 등을 정리합니다.

{% if posts.size > 0 %}
{% for post in posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description | default: post.excerpt | strip_html | truncate: 160 }}

{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
