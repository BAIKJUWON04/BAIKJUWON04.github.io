---
title: 개발공부
icon: fas fa-code
order: 3
---

{% assign posts = site.categories["개발공부"] %}

프로그래밍 언어, Linux, Git, 웹 개발 등 개발 과정에서 공부한 내용을 기록합니다.

{% if posts.size > 0 %}
{% for post in posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description | default: post.excerpt | strip_html | truncate: 160 }}

{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
