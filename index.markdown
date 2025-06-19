---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% raw %}
{% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</p>
    <div class="post-excerpt">
      {{ post.excerpt }}
    </div>
  </article>
{% endfor %}
{% endraw %}