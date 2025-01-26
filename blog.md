---
layout: page
title: "Blog"
permalink: /blog/
main_nav: true
weight: 3
---

# Blog

A Roadmap of some pieces I will post shortly
I have all of these pieces outlined, and will post as time allows:
 
1) Why SALT?
2) Inflation Reduction Act as a Discrete Change in Federal Tax Policy
3) What’s a Bienium?
4) The Oil and Gas States

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
