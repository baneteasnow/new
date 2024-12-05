---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Fashion"
---

{% for post in site.posts %} {% if post.tag == 'moda markaları' or post.tag ==
'moda tasarım' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign fashiontags1 = site.posts | where: "tag", "moda markaları" | size %}
{% assign fashiontags2 = site.posts | where: "tag", "moda tasarım" | size %}

{{ fashiontags1 | plus: fashiontags2 }}
