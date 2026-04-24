---
layout: default
title: "Research"
permalink: /research/
description: "Research interests and conference presentations by Willis Chun Lai Wong — generative morphology, morphology–syntax interface, prosody–morphology interface."
---

<h1>Research</h1>

<h2 class="section-heading">Interests</h2>

<div class="card">
  <h3>Generative Morphology</h3>
  <p>Distributed Morphology; reduplication — especially in Cantonese.</p>
</div>

<div class="card">
  <h3>Morphology–Syntax Interface</h3>
  <p>Phase locality; labelling algorithm; linearisation; interface conditions.</p>
</div>

<div class="card">
  <h3>Prosody–Morphology Interface</h3>
  <p>Syllable fusion; prosodic structure; ideophones.</p>
</div>

<h2 class="section-heading">Conference presentations</h2>

{% assign pubs = site.data.publications | sort: "year" | reverse %}
{% if pubs and pubs.size > 0 %}
<ul class="pub-list">
  {% for p in pubs %}
  <li>
    <div>
      <span class="pub-year">{{ p.date | default: p.year }}</span>
      <span class="pub-title">{{ p.title }}</span>
    </div>
    <div class="pub-venue">{{ p.authors }}. <em>{{ p.venue }}</em>.</div>
    {% if p.links %}
    <div class="pub-links">
      {% if p.links.doi and p.links.doi != "" %}<a href="https://doi.org/{{ p.links.doi }}">doi</a>{% endif %}
      {% if p.links.pdf and p.links.pdf != "" %}<a href="{{ p.links.pdf }}">pdf</a>{% endif %}
      {% if p.links.preprint and p.links.preprint != "" %}<a href="{{ p.links.preprint }}">preprint</a>{% endif %}
      {% if p.links.publisher and p.links.publisher != "" %}<a href="{{ p.links.publisher }}">publisher</a>{% endif %}
      {% if p.links.slides and p.links.slides != "" %}<a href="{{ p.links.slides }}">slides</a>{% endif %}
      {% if p.links.handout and p.links.handout != "" %}<a href="{{ p.links.handout | relative_url }}">handout</a>{% endif %}
      {% if p.links.poster and p.links.poster != "" %}<a href="{{ p.links.poster }}">poster</a>{% endif %}
      {% if p.links.code and p.links.code != "" %}<a href="{{ p.links.code }}">code</a>{% endif %}
    </div>
    {% endif %}
  </li>
  {% endfor %}
</ul>
{% else %}
<p class="muted">Presentations list coming soon.</p>
{% endif %}
