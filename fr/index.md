---
layout: home
lang: fr
title: Les Protocoles Fondamentaux
title_top: Les Protocoles
title_bottom: Fondamentaux
subtitle: "Les engagements et les protocoles pour un excellent travail d’équipe."
band: Basé sur les travaux de Jim McCarthy et Michele McCarthy
---
{% assign nav = site.data.nav.fr %}
<section class="home-section">
  <p class="lede">Les Protocoles Fondamentaux regroupent des engagements et des protocoles. Commencez par les engagements, puis utilisez les protocoles ensemble.</p>
  {% for item in nav.commitments %}
  <a class="card card-feature" href="{{ item.url | relative_url }}">
    <span class="card-title">{{ item.title }}</span>
    <span class="card-summary">{{ item.summary }}</span>
  </a>
  {% endfor %}
</section>

<section class="home-section" id="protocoles">
  <h2>Les Protocoles Fondamentaux</h2>
  <ol class="card-grid">
    {% for item in nav.protocols %}
    <li><a class="card" href="{{ item.url | relative_url }}">
      <span class="card-num">{{ forloop.index }}</span>
      <span class="card-title">{{ item.title }}</span>
      <span class="card-summary">{{ item.summary }}</span>
    </a></li>
    {% endfor %}
  </ol>
</section>

<section class="home-section">
  <h2>Aller plus loin</h2>
  <ul class="card-grid card-grid-small">
    {% for item in nav.related %}
    <li><a class="card" href="{{ item.url | relative_url }}">
      <span class="card-title">{{ item.title }}</span>
      <span class="card-summary">{{ item.summary }}</span>
    </a></li>
    {% endfor %}
  </ul>
</section>
