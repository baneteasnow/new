---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Economics"
---

{% for post in site.posts %} {% if post.tag == 'ekonomi' or post.tag ==
'küreselleşme' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign economicstags1 = site.posts | where: "tag", "ekonomi" | size %}
{% assign economicstags2 = site.posts | where: "tag", "küreselleşme" | size %}

{{ economicstags1 | plus: economicstags2 }}
