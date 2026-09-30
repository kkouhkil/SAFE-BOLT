---
layout: page
title: News
permalink: /news/
eyebrow: PROJECT UPDATES
intro: Milestones, demonstrations and public SAFE-BOLT updates.
---

{% for post in site.posts %}
<article class="news-item">
  <span class="post-date">{{ post.date | date: "%d %b %Y" }}</span>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt | strip_html }}</p>
</article>
{% endfor %}
