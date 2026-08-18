---
title: 임베디드
icon: fas fa-microchip
order: 2
---

{% assign posts = site.categories["임베디드"] %}

ESP32, ESP8266, STM32, 센서, 통신, 회로 관련 학습과 프로젝트 기록입니다.

{% if posts.size > 0 %}
{% for post in posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description | default: post.excerpt | strip_html | truncate: 160 }}

{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
