---
layout: page
title: Blog
permalink: /blog/
---

<section class="hero">

    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
          <p>{{ post.summary }}
        </h2>
      </li>
    {% endfor %}
</section>