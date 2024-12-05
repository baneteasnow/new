---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Behavioural"
---

{% for post in site.posts %} {% if post.tag contains 'davranışsal iktisat' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign behaviouraltags1 = site.posts | where: "tag", "mimarlık" | size %}

{{ behaviouraltags1 }}
