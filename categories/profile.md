---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Profile"
---

{% for post in site.posts %} {% if post.tag == 'biyografi' or post.tag == 'marka
profili' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign profiletags1 = site.posts | where: "tag", "biyografi" | size %}
{% assign profiletags2 = site.posts | where: "tag", "marka profili" | size %}

{{ profiletags1 | plus: profiletags2 }}
