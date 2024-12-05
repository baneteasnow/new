---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Planning"
---

{% for post in site.posts %} {% if post.tag == 'öğrenmeyi öğrenmek' or post.tag
== 'üretkenlik ve teknoloji' or post.tag == 'yazmak ve yaratıcılık' or post.tag
== 'zaman planlaması' or post.tag == 'kitap okumak ve kitaplar' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign planningtags1 = site.posts | where: "tag", "öğrenmeyi öğrenmek" | size %}
{% assign planningtags2 = site.posts | where: "tag", "üretkenlik ve teknoloji" | size %}
{% assign planningtags3 = site.posts | where: "tag", "yazmak ve yaratıcılık" | size %}
{% assign planningtags4 = site.posts | where: "tag", "zaman planlaması" | size %}
{% assign planningtags5 = site.posts | where: "tag", "kitap okumak ve kitaplar" | size %}

{{ planningtags1 | plus: planningtags2 | plus: planningtags3 | plus: planningtags4 | plus: planningtags5 }}
