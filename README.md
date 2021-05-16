## We're Silvia and Ramón.

{% for episode in site.podcast_episodes reversed %}
  <h3 class="h2">
    <a href="{{ episode.url | prepend: site.baseurl }}" class="title">
      {{ episode.title }}
    </a>
  </h3>
  <p>{{ episode.date | date: site.date_format }}</p>
{% endfor %}
