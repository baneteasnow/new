---
#mimarlık + mühendislik + endüstriyel tasarım + şehir planlama
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Architecture"
---

{% for post in site.posts %} {% if post.tag == 'mimarlık' or post.tag ==
'mühendislik' or post.tag == 'şehir planlama' or post.tag == 'endüstriyel
tasarım' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign architecturetags1 = site.posts | where: "tag", "mimarlık" | size %}
{% assign architecturetags2 = site.posts | where: "tag", "mühendislik" | size %}
{% assign architecturetags3 = site.posts | where: "tag", "şehir planlama" | size %}
{% assign architecturetags4 = site.posts | where: "tag", "endüstriyel
tasarım" | size %}

{{ architecturetags1 | plus: architecturetags2 | plus: architecturetags3 | plus: architecturetags4 }}
