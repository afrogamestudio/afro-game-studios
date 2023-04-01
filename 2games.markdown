---
layout: page
title: Our Games
permalink: /games/
---

<section id="games" class="section">

  {% for game in site.games %}
  {% if game.is_index %}
  <h2>
    <a href="{{ site.baseurl }}/{{ game.url }}">
      {{ game.title }}
    </a>
  </h2>
  <p>{{ game.excerpt }}</p>
  {% endif %}
{% endfor %}




</section>