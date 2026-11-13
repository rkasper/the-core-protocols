---
layout: home
lang: es
title: Los protocolos fundamentales
title_top: Los protocolos
title_bottom: fundamentales
subtitle: "Versión 3.1: los compromisos y protocolos para un gran trabajo en equipo."
band: Basado en el trabajo de Jim McCarthy y Michele McCarthy
---
{% assign nav = site.data.nav.es %}
<section class="home-section">
  <p class="lede">Los protocolos fundamentales están compuestos tanto por compromisos como por protocolos. La traducción al español está en curso.</p>
</section>

<section class="home-section" id="protocolos">
  <h2>Ya disponibles</h2>
  <ul class="card-grid">
    {% for item in nav.protocols %}
    <li><a class="card" href="{{ item.url | relative_url }}">
      <span class="card-title">{{ item.title }}</span>
      <span class="card-summary">{{ item.summary }}</span>
    </a></li>
    {% endfor %}
  </ul>
</section>

<section class="home-section">
  <h2>Próximamente</h2>
  <ul class="coming">
    {% for title in nav.coming %}<li>{{ title }}</li>{% endfor %}
  </ul>
  <p class="fine">Mientras tanto, puedes leer todos los protocolos <a href="{{ '/' | relative_url }}" lang="en">en inglés</a>.</p>
</section>
