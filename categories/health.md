---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Health"
---

{% for post in site.posts %} {% if post.tag == 'sağlık' or post.tag ==
'beslenme' or post.tag == 'tıp' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign healthtags1 = site.posts | where: "tag", "sağlık" | size %}
{% assign healthtags2 = site.posts | where: "tag", "beslenme" | size %}
{% assign healthtags3 = site.posts | where: "tag", "tıp" | size %}

{{ healthtags1 | plus: healthtags2 | plus: healthtags3 }}
