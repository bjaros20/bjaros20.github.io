---
layout: page
title: "Blog"
permalink: /blog/
main_nav: true
weight: 3
---

# Blog

Welcome — this blog features brief policy reflections, previews of ongoing research, and links to outside work.


<ul class="posts-list">
  {% for post in site.posts %}
    <li>
      <strong>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </strong>
      <span class="post-date">- {{ post.date | date_to_long_string }}</span>
      <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
    </li>
  {% endfor %}
</ul>
