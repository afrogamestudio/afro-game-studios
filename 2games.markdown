---
layout: page
title: Our Games
permalink: /games/
---

<section class="hero">



    {% for game in site.games %}
  {% if game.is_index %}
      <li>
        <h2>
          <a class="post-link" href="{{ game.url | prepend: site.baseurl }}">{{ game.title | escape }}</a>
        </h2>
        <p>
          <img src="{{ site.baseurl }}/{{ game.thumbnail }}" style="width: 150px; float: left; padding: 5px" alt="{{game.title}}" />
          {{ game.excerpt | strip_html }}
        </p>
      </li>
  {% endif %}
    {% endfor %}


</section>