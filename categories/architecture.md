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

{% assign architecture = site.posts %}
{% assign architectureposts = architecture | size %} {% assign architecturetags = architecture | where: "tag", "mimarlik" or "mühendislik" | size %} {{ architectureposts }}
