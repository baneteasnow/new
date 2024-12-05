---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Media"
---

{% for post in site.posts %} {% if post.tag == 'dijital kültür' or post.tag ==
'sosyal medya' or post.tag == 'medya' or post.tag == 'sanat' or post.tag ==
'iletişim' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign mediatags1 = site.posts | where: "tag", "dijital kültür" | size %}
{% assign mediatags2 = site.posts | where: "tag", "sosyal medya" | size %}
{% assign mediatags3 = site.posts | where: "tag", "medya" | size %}
{% assign mediatags4 = site.posts | where: "tag", "sanat" | size %}
{% assign mediatags5 = site.posts | where: "tag", "iletişim" | size %}

{{ mediatags1 | plus: mediatags2 | plus: mediatags3 | plus: mediatags4 | plus: mediatags5 }}
