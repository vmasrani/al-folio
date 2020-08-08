---
layout: page
title: books
description: I always enjoy peering at other people's bookshelves, so here's mine.
importance: 3
---
<div class="projects grid">

  {% assign sorted = site.data.books | sort: 'author' %}
  {% for book in sorted %}
  <div class="grid-item">
    <a href="{{ book.main_link }}" target="_blank">
      <div class="card hoverable">
        {% if book.img %}
        <img src="{{ book.img | prepend: '/assets/img/books/' | relative_url }}" alt="project thumbnail">
        {% endif %}
        <div class="card-body">
          <h4 class="card-title">{{ book.name }}</h4>
            <p><em>{{ book.author }}</em></p>
          </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>


