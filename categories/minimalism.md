---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Minimalism"
---

{% for post in site.posts %} {% if post.tag == 'sıfır atık yaşam' or post.tag ==
'minimalizm' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign minimalismtags1 = site.posts | where: "tag", "sıfır atık yaşam" | size %}
{% assign minimalismtags2 = site.posts | where: "tag", "minimalizm" | size %}

{{ minimalismtags1 | plus: minimalismtags2 }}
