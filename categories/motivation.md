---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Motivation"
---

{% for post in site.posts %} {% if post.tag == 'lifestyle' or post.tag ==
'motivasyon' or post.tag == 'mindfulness' or post.tag == 'seyahat' or post.tag
== 'yaratıcılık' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign motivationtags1 = site.posts | where: "tag", "lifestyle" | size %}
{% assign motivationtags2 = site.posts | where: "tag", "motivasyon" | size %}
{% assign motivationtags3 = site.posts | where: "tag", "mindfulness" | size %}
{% assign motivationtags4 = site.posts | where: "tag", "seyahat" | size %}
{% assign motivationtags5 = site.posts | where: "tag", "yaratıcılık" | size %}

{{ motivationtags1 | plus: motivationtags2 | plus: motivationtags3 | plus: motivationtags4 | plus: motivationtags5 }}
