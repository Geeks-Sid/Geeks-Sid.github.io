---
title: "What are you doing?"
date: 2023-03-10
---

{% raw %}{% for post in site.posts limit:5 %}
<article>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
</article>
{% endfor %}{% endraw %}
