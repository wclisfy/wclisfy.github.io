---
layout: default
title: "Home"
description: "Willis Chun Lai Wong — generative morphologist, MPhil in Linguistics at CUHK. Research on Distributed Morphology, reduplication, phase locality, and the prosody–morphology interface."
---

<section class="hero">
  <img class="hero-avatar" src="{{ '/assets/img/avatar.jpg' | relative_url }}"
       alt="Portrait of Willis Chun Lai Wong"
       onerror="this.style.visibility='hidden'" />
  <div>
    <h1>Hi, I'm Willis.</h1>
    <p class="tagline">Generative Morphologist · MPhil in Linguistics, CUHK</p>
    <p class="lead">
      I'm currently pursuing an MPhil in Linguistics at
      <strong>The Chinese University of Hong Kong</strong>.
      I work on <strong>generative morphology</strong> and its interfaces —
      how morphological structure is built, how it meets syntax, and how it
      lands on prosody.
    </p>

    <ul class="social">
      {% if site.social.google_scholar != "" %}<li><a href="{{ site.social.google_scholar }}" rel="me">Google Scholar</a></li>{% endif %}
      {% if site.social.orcid != "" %}<li><a href="https://orcid.org/{{ site.social.orcid }}" rel="me">ORCID</a></li>{% endif %}
      {% if site.social.github != "" %}<li><a href="https://github.com/{{ site.social.github }}" rel="me">GitHub</a></li>{% endif %}
      {% if site.social.linkedin != "" %}<li><a href="https://www.linkedin.com/in/{{ site.social.linkedin }}/" rel="me">LinkedIn</a></li>{% endif %}
      {% if site.social.instagram != "" %}<li><a href="https://www.instagram.com/{{ site.social.instagram }}/" rel="me">@{{ site.social.instagram }}</a></li>{% endif %}
      {% if site.email != "" %}<li><a href="mailto:{{ site.email }}">Email</a></li>{% endif %}
    </ul>
  </div>
</section>

<h2 class="section-heading">What I work on</h2>

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

<p>
  <a class="btn" href="{{ '/research/' | relative_url }}">See my research →</a>
  <a class="btn btn-ghost" href="{{ '/cv/' | relative_url }}">CV</a>
</p>
