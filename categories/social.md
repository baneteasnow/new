---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Social"
---

{% for post in site.posts %} {% if post.tag == 'psikoloji' or post.tag ==
'felsefe' or post.tag == 'sosyoloji' or post.tag == 'siyaset bilimi' or post.tag
== 'sosyal bilimler' or post.tag == 'eğitim' or post.tag == 'tarih' or post.tag
== 'kişisel gelişim' or post.tag == 'sosyal psikoloji' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign socialtags1 = site.posts | where: "tag", "psikoloji" | size %}
{% assign socialtags2 = site.posts | where: "tag", "felsefe" | size %}
{% assign socialtags3 = site.posts | where: "tag", "sosyoloji" | size %}
{% assign socialtags4 = site.posts | where: "tag", "siyaset bilimi" | size %}
{% assign socialtags5 = site.posts | where: "tag", "sosyal bilimler" | size %}
{% assign socialtags6 = site.posts | where: "tag", "eğitim" | size %}
{% assign socialtags7 = site.posts | where: "tag", "tarih" | size %}
{% assign socialtags8 = site.posts | where: "tag", "kişisel gelişim" | size %}
{% assign socialtags9 = site.posts | where: "tag", "sosyal psikoloji" | size %}

{{ socialtags1 | plus: socialtags2 | plus: socialtags3 | plus: socialtags4 | plus: socialtags5 | plus: socialtags6 | plus: socialtags7 | plus: socialtags8 | plus: socialtags9 }}
