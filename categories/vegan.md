---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Vegan"
---

{% for post in site.posts %} {% if post.tag == 'veganlık' or post.tag == 'hayvan
hakları' or post.tag == 'etik' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign vegantags1 = site.posts | where: "tag", "veganlık" | size %}
{% assign vegantags2 = site.posts | where: "tag", "hayvan
hakları" | size %}
{% assign vegantags3 = site.posts | where: "tag", "etik" | size %}

{{ vegantags1 | plus: vegantags2 | plus: vegantags3 }}
