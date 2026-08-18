---
title: 외부활동
icon: fas fa-person-hiking
order: 5
---

{% assign posts = site.categories["외부활동"] %}

해커톤, 공모전, 동아리, 교육활동, 해외봉사 등의 경험을 기록합니다.

{% if posts.size > 0 %}
{% for post in posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description | default: post.excerpt | strip_html | truncate: 160 }}

{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
