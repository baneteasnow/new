---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Technology"
---

{% for post in site.posts %} {% if post.tag == 'teknoloji' or post.tag == 'yapay
zeka' or post.tag == 'gelecek ve trendler' or post.tag == 'internet' or post.tag
== 'internet of things' or post.tag == 'yazılım' or post.tag == 'bilgi
sistemleri' or post.tag == 'siber güvenlik' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign technologytags1 = site.posts | where: "tag", "teknoloji" | size %}
{% assign technologytags2 = site.posts | where: "tag", "yapay
zeka" | size %}
{% assign technologytags3 = site.posts | where: "tag", "gelecek ve trendler" | size %}
{% assign technologytags4 = site.posts | where: "tag", "internet" | size %}
{% assign technologytags5 = site.posts | where: "tag", "internet of things" | size %}
{% assign technologytags6 = site.posts | where: "tag", "yazılım" | size %}
{% assign technologytags7 = site.posts | where: "tag", "bilgi
sistemleri" | size %}
{% assign technologytags8 = site.posts | where: "tag", "siber güvenlik" | size %}

{{ technologytags1 | plus: technologytags2 | plus: technologytags3 | plus: technologytags4 | plus: technologytags5 | plus: technologytags6 | plus: technologytags7 | plus: technologytags8 }}
