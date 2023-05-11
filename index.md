---
layout: home
---

<h1>Welcome to My Blog!</h1>

{% raw %}{% for post in site.posts limit:5 %}
<article>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p class="post-meta">
    <span class="author">{{ post.author }}</span>
    <span class="date">{{ post.date | date: "%B %-d, %Y" }}</span>
  </p>
  <p>{{ post.excerpt }}</p>
</article>
{% endfor %}{% endraw %}
