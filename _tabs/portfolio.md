---
title: 포트폴리오
icon: fas fa-briefcase
order: 1
---

{% assign posts = site.categories["포트폴리오"] %}

완성한 프로젝트와 주요 결과물을 정리합니다.

{% if posts.size > 0 %}
{% for post in posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description | default: post.excerpt | strip_html | truncate: 160 }}

`{{ post.date | date: "%Y-%m-%d" }}`

{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
