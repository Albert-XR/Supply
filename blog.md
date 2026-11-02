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

<div class="blog-list answer-list">
  <h2>Buyer Questions — Direct Answers</h2>
  <p class="answer-intro">Short, factual answers to the questions importers, wholesalers and hospitality buyers ask us most.</p>
  <ul>
    {% for a in site.answers %}
    <li><a href="{{ a.url }}">{{ a.title }}</a><span>{{ a.description }}</span></li>
    {% endfor %}
  </ul>
</div>

<style>
.answer-list {
  border-top: 1px solid #eee;
  margin-top: 34px;
  padding-top: 10px;
}

.answer-list h2 {
  color: #1a1a2e;
  font-size: 1.4em;
  margin: 22px 0 8px;
}

.answer-intro {
  color: #666;
  font-size: 0.95em;
  margin: 0 0 16px;
}

.answer-list ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.answer-list li {
  padding: 12px 0;
  border-bottom: 1px solid #f0f0f0;
}

.answer-list li a {
  display: block;
  color: #1a1a2e;
  font-weight: 600;
  text-decoration: none;
  line-height: 1.45;
}

.answer-list li a:hover {
  color: #e94560;
}

.answer-list li span {
  display: block;
  color: #888;
  font-size: 0.88em;
  line-height: 1.6;
  margin-top: 4px;
}

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
