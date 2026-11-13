---
layout: home
title: The Core Protocols
title_top: The Core
title_bottom: Protocols
subtitle: "Version 3.1: the commitments and protocols for great teamwork."
band: Based on the work of Jim McCarthy and Michele McCarthy
---
{% assign nav = site.data.nav.en %}
<section class="home-section">
  <p class="lede">The Core Protocols are made up of both commitments and protocols. Start with the commitments, then use the protocols together.</p>
  {% for item in nav.commitments %}
  <a class="card card-feature" href="{{ item.url | relative_url }}">
    <span class="card-title">{{ item.title }}</span>
    <span class="card-summary">{{ item.summary }}</span>
  </a>
  {% endfor %}
</section>

<section class="home-section" id="protocols">
  <h2>The Core Protocols</h2>
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
  <h2>Related protocols, applications, and commitments</h2>
  <ul class="card-grid card-grid-small">
    {% for item in nav.related %}
    <li><a class="card" href="{{ item.url | relative_url }}">
      <span class="card-title">{{ item.title }}</span>
      <span class="card-summary">{{ item.summary }}</span>
    </a></li>
    {% endfor %}
  </ul>
</section>
