---
layout: page-15
published: true
last_modified_at: 2024-12-04
title: "Work"
---

{% for post in site.posts %} {% if post.tag == 'çalışma yaşamı' or post.tag ==
'kariyer' or post.tag == 'girişimcilik' or post.tag == 'hukuk' or post.tag ==
'insan kaynakları' or post.tag == 'yönetim' %}

<p class="cat1"><a href="{{ post.url }}">{{ post.title | downcase }}</a></p>
{% endif %} {% endfor %}
<br />

{% assign worktags1 = site.posts | where: "tag", "çalışma yaşamı" | size %}
{% assign worktags2 = site.posts | where: "tag", "kariyer" | size %}
{% assign worktags3 = site.posts | where: "tag", "girişimcilik" | size %}
{% assign worktags4 = site.posts | where: "tag", "hukuk" | size %}
{% assign worktags1 = site.posts | where: "tag", "insan kaynakları" | size %}
{% assign worktags2 = site.posts | where: "tag", "yönetim" | size %}

{{ worktags1 | plus: worktags2 | plus: worktags3 | plus: worktags4 | plus: worktags5 | plus: worktags6 }}
