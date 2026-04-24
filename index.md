---
layout: default
title: "Home"
description: "Willis Chun Lai Wong — MPhil in Linguistics at CUHK. Syntax–morphology interface; Distributed Morphology; Cantonese reduplication; Choiceless Computation Theorem."
---

<section class="hero">
  <h1>Willis Chun Lai Wong</h1>
  <p class="tagline">MPhil in Linguistics, The Chinese University of Hong Kong</p>

  <p class="lead">
    I'm a linguist working on the <strong>syntax–morphology interface</strong>
    and the <strong>morphology–prosody interface</strong>. My MPhil thesis,
    <em>The Architecture of Reduplication: Structural (A)symmetries in
    Cantonese Adjectives</em>, develops a crash-tolerant account of syntactic
    symmetry — formalized as the <em>Choiceless Computation Theorem</em> —
    and applies it to Sinitic reduplication, coordination, and Right Node Raising.
  </p>

  <ul class="social">
    {% if site.email != "" %}<li><a href="mailto:{{ site.email }}">{{ site.email }}</a></li>{% endif %}
    {% if site.social.github != "" %}<li><a href="https://github.com/{{ site.social.github }}" rel="me">GitHub</a></li>{% endif %}
    {% if site.social.google_scholar != "" %}<li><a href="{{ site.social.google_scholar }}" rel="me">Scholar</a></li>{% endif %}
    {% if site.social.orcid != "" %}<li><a href="https://orcid.org/{{ site.social.orcid }}" rel="me">ORCID</a></li>{% endif %}
    {% if site.social.linkedin != "" %}<li><a href="https://www.linkedin.com/in/{{ site.social.linkedin }}/" rel="me">LinkedIn</a></li>{% endif %}
    {% if site.social.instagram != "" %}<li><a href="https://www.instagram.com/{{ site.social.instagram }}/" rel="me">@{{ site.social.instagram }}</a></li>{% endif %}
  </ul>
</section>

<h2 class="section-heading">Research interests</h2>

<p>
  <strong>Syntax–morphology interface.</strong>
  Distributed Morphology, Minimalism, reduplication, roots, the labelling
  algorithm. I develop a crash-tolerant architecture in which Merge generates
  freely and deterministic interface evaluators cannot arbitrarily break
  structural symmetry. The Choiceless Computation Theorem delivers a 2×2
  typology unifying ATB extraction, Right Node Raising, and Sinitic AABB /
  ABAB reduplication.
</p>

<p>
  <strong>Morphology–prosody interface.</strong>
  Iconicity, syllable fusion, prosodic structure. Cantonese ideophones and
  cophonological accounts of iconic phonology — how expressive material
  resists phonological erosion at PF.
</p>

<p>
  See <a href="{{ '/research/' | relative_url }}">research</a> for working
  papers and talks, or <a href="{{ '/cv/' | relative_url }}">CV</a>.
</p>
