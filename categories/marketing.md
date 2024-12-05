---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Marketing"
---

{% for post in site.posts %} {% if post.tag == 'pazarlama' or post.tag ==
'reklam' or post.tag == 'tüketici davranışları' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign marketingtags1 = site.posts | where: "tag", "pazarlama" | size %}
{% assign marketingtags2 = site.posts | where: "tag", "reklam" | size %}
{% assign marketingtags3 = site.posts | where: "tag", "tüketici davranışları" | size %}

{{ marketingtags1 | plus: marketingtags2 | plus: marketingtags3 }}
