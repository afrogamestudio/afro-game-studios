---
layout: page
title: News & Events
permalink: /news/
---

<section class="hero">

    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
        <p>
          <img src="{{ site.baseurl }}/{{ post.thumbnail }}" style="width: 150px; float: left; padding: 5px" alt="{{post.title}}" />
          {{ post.excerpt | strip_html }}
        </p>
      </li>
    {% endfor %}

</section>

