---
layout: default
title: "Home"
description: "Willis Chun Lai Wong — theoretical linguist, MPhil in Linguistics at CUHK. Research on syntactic symmetry, labeling theory, the Choiceless Computation Theorem, Distributed Morphology, and the syntax–morphology–prosody interfaces."
---

<section class="hero">
  <img class="hero-avatar" src="{{ '/assets/img/avatar.jpg' | relative_url }}"
       alt="Portrait of Willis Chun Lai Wong"
       onerror="this.style.visibility='hidden'" />
  <div>
    <h1>Hi, I'm Willis.</h1>
    <p class="tagline">Theoretical Linguist · MPhil in Linguistics, CUHK</p>
    <p class="lead">
      I'm currently pursuing an MPhil in Linguistics at
      <strong>The Chinese University of Hong Kong</strong>. My work asks how
      the computational system of language handles <strong>structural
      symmetry</strong> — when two objects in a derivation are indistinguishable
      to the grammar, what does it have to do? I pursue this across the
      <strong>syntax–morphology–prosody interfaces</strong>, with Sinitic
      reduplication, coordination, and Right Node Raising as recurring empirical
      anchors.
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
  <h3>Syntactic symmetry &amp; the Choiceless Computation Theorem</h3>
  <p>
    A crash-tolerant view of syntax on which Merge generates freely and
    deterministic interface evaluators (Minimal Search, Linearization,
    Vocabulary Insertion) cannot arbitrarily break symmetry. The Choiceless
    Computation Theorem (CCT) gives a 2×2 typology of symmetry resolution that
    unifies ATB extraction, Right Node Raising, and Sinitic AABB / ABAB
    reduplication.
  </p>
</div>

<div class="card">
  <h3>Labeling theory &amp; the Merge–interface boundary</h3>
  <p>
    Recasting Chomsky's (2013, 2015) labeling algorithm in
    automorphism-theoretic terms; the ignition problem; what the syntax owes
    PF and LF when symmetry persists past Narrow Syntax.
  </p>
</div>

<div class="card">
  <h3>Distributed Morphology &amp; Sinitic reduplication</h3>
  <p>
    Cantonese and Mandarin coordinative adjectives; why <em>*AB</em> is
    systematically excluded while AABB / ABAB are obligatory; phase-locality
    accounts of reduplication; ideophones and phonological integrity.
  </p>
</div>

<p>
  <a class="btn" href="{{ '/research/' | relative_url }}">See my research →</a>
  <a class="btn btn-ghost" href="{{ '/cv/' | relative_url }}">CV</a>
</p>
