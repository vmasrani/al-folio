---
layout: page
title: podcasts
description: Podcasts are conversation fuel. Here are my favorites.
importance: 3
---
<div class="projects grid">

  {% assign sorted = site.data.podcasts | sort: 'name' %}
  {% for podcast in sorted %}
  <div class="grid-item">
    <a href="{{ podcast.link }}" target="_blank">
      <div class="card hoverable">
        {% if podcast.img %}
        <img src="{{ podcast.img | prepend: '/assets/img/podcasts/' | relative_url }}" alt="project thumbnail">
        {% endif %}
        <div class="card-body">
          <h2 class="card-title text-lowercase">{{ podcast.name }}</h2>
          <p class="card-text">{{ podcast.blurb }}</p>
            <p><b>Topic: </b>{{ podcast.topic }}</p>
            <p><a href="{{podcast.key_episode.url}}"> <b>Key Episode: </b> {{podcast.key_episode.display}}</a></p>
          </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>
