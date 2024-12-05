---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Science"
---

{% for post in site.posts %} {% if post.tag == 'fen bilimleri' or post.tag ==
'küresel ısınma' or post.tag == 'sürdürülebilirlik' or post.tag == 'permakültür'
or post.tag == 'bahçe tarımı' or post.tag == 'çevre' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign sciencetags1 = site.posts | where: "tag", "fen bilimleri" | size %}
{% assign sciencetags2 = site.posts | where: "tag", "küresel ısınma" | size %}
{% assign sciencetags3 = site.posts | where: "tag", "sürdürülebilirlik" | size %}
{% assign sciencetags4 = site.posts | where: "tag", "permakültür" | size %}
{% assign sciencetags5 = site.posts | where: "tag", "bahçe tarımı" | size %}
{% assign sciencetags6 = site.posts | where: "tag", "çevre" | size %}

{{ sciencetags1 | plus: sciencetags2 | plus: sciencetags3 | plus: sciencetags4 | plus: sciencetags5 | plus: sciencetags6 }}
