---
layout: default
title: Home
---

{% assign latest_post = site.posts.first %}

# {{ latest_post.title }}

<small>Posted on {{ latest_post.date | date: "%B %d, %Y" }}</small>

<p>{{ latest_post.content }}</p>

<!-- <a href="{{ latest_post.url }}">Read more</a> -->
