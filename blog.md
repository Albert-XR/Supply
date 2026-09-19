---
layout: page
title: Blog
permalink: /blog/
description: "Buying guides and industry knowledge for stainless steel cutlery importers, wholesalers and hospitality buyers."
---

<div class="blog-list">
  {% for post in site.posts %}
  <div class="blog-card">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="blog-meta">{{ post.date | date: "%b %-d, %Y" }} · {{ post.read_time }} min read</p>
    <p class="blog-excerpt">{{ post.description }}</p>
    <a class="blog-readmore" href="{{ post.url }}">Read article →</a>
  </div>
  {% endfor %}
</div>

<style>
.blog-list {
  max-width: 820px;
  margin: 0 auto;
}

.blog-card {
  padding: 26px 0;
  border-bottom: 1px solid #eee;
}

.blog-card:first-child {
  padding-top: 6px;
}

.blog-card h2 {
  margin: 0 0 6px;
  font-size: 1.35em;
  line-height: 1.35;
}

.blog-card h2 a {
  color: #1a1a2e;
  text-decoration: none;
}

.blog-card h2 a:hover {
  color: #e94560;
}

.blog-meta {
  color: #999;
  font-size: 0.85em;
  margin: 0 0 8px;
}

.blog-excerpt {
  color: #555;
  line-height: 1.7;
  margin: 0 0 10px;
}

.blog-readmore {
  color: #e94560;
  font-weight: 600;
  text-decoration: none;
  font-size: 0.95em;
}
</style>
