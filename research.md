---
layout: default
title: "Research"
permalink: /research/
description: "Research by Willis Chun Lai Wong — syntactic symmetry, the Choiceless Computation Theorem, labeling theory, Distributed Morphology, Sinitic reduplication, Right Node Raising."
---

<h1>Research</h1>

<h2 class="section-heading">Interests</h2>

<p>
  <strong>Syntax–morphology interface.</strong>
  Distributed Morphology; Minimalism; reduplication; roots; labelling algorithm.
  A crash-tolerant architecture in which Merge generates freely while
  deterministic interface evaluators cannot arbitrarily break structural
  symmetry. The <em>Choiceless Computation Theorem</em> delivers a 2×2
  typology unifying ATB extraction, Right Node Raising, and Sinitic AABB /
  ABAB reduplication.
</p>

<p>
  <strong>Morphology–prosody interface.</strong>
  Iconicity; syllable fusion; prosodic structure. Cantonese ideophones and
  cophonological accounts of iconic phonology — how expressive material
  resists phonological erosion at PF.
</p>

<h2 class="section-heading">Working papers</h2>

<p>
  <em>If You Can't Break It, Keep It: Choiceless Computation under Syntactic
  Symmetry.</em>
  <span class="muted small"> Manuscript · under submission.</span>
  <a href="{{ '/docs/if-you-cant-break-it-keep-it-manuscript.pdf' | relative_url }}">manuscript</a>
</p>

<p>
  Sinitic adjectival coordinatives systematically exclude the simplex
  <em>*AB</em> form while requiring reduplicated outputs AABB or ABAB.
  I argue that this gap follows from a restriction on deterministic evaluation
  over symmetric domains, formalized as the Choiceless Computation Theorem.
  The CCT recasts Chomsky's labeling theory in automorphism-theoretic terms,
  adds a fourth case (the Null Label), and yields a falsifiable 2×2 typology
  unifying AABB distributive exponence, ABAB pied-piping, ATB extraction,
  and Right Node Raising.
</p>

<p>
  <em>Caught Between Two Nodes: The Choiceless Computation of Right Node
  Raising.</em>
  <span class="muted small"> Abstract · Rightward Movement Workshop.</span>
  <a href="{{ '/docs/2026-RNR-workshop-abstract.pdf' | relative_url }}">abstract</a>
</p>

<p>
  RNR obeys a Right-Edge Restriction, requires identity between conjuncts,
  and disallows selective deletion. I recover Sabbagh's (2007) architectural
  unification of RNR with ATB — as independent resolutions of structural
  symmetry — while relocating its mechanism: the uniformity is real, the
  rightward displacement is not. A corollary predicts Left Node Raising in
  head-final languages, and places Suspended Affixation in the RNR cell.
</p>

{% assign proc = site.data.publications | where: "type", "proceedings" %}
{% if proc and proc.size > 0 %}
<h2 class="section-heading">Proceedings</h2>
<ul class="pub-list">
  {% for p in proc %}
  <li>
    <span class="pub-year">{{ p.year }}</span>
    <span class="pub-title">{{ p.title }}</span>
    <div class="pub-venue">{{ p.authors }}. <em>{{ p.venue }}</em>.</div>
  </li>
  {% endfor %}
</ul>
{% endif %}

{% assign invited = site.data.publications | where: "type", "invited" %}
{% if invited and invited.size > 0 %}
<h2 class="section-heading">Invited presentations</h2>
<ul class="pub-list">
  {% for p in invited %}
  <li>
    <span class="pub-year">{{ p.date | default: p.year }}</span>
    <span class="pub-title">{{ p.title }}</span>
    <div class="pub-venue">{{ p.authors }}. <em>{{ p.venue }}</em>.</div>
  </li>
  {% endfor %}
</ul>
{% endif %}

<h2 class="section-heading">Conference presentations</h2>
{% assign pres = site.data.publications | where: "type", "presentation" | sort: "year" | reverse %}
{% if pres and pres.size > 0 %}
<ul class="pub-list">
  {% for p in pres %}
  <li>
    <span class="pub-year">{{ p.date | default: p.year }}</span>
    <span class="pub-title">{{ p.title }}</span>{% if p.status and p.status != "" %} <span class="muted small">· {{ p.status }}</span>{% endif %}
    <div class="pub-venue">{{ p.authors }}. <em>{{ p.venue }}</em>.</div>
    {% if p.links %}
    <div class="pub-links">
      {% if p.links.doi and p.links.doi != "" %}<a href="https://doi.org/{{ p.links.doi }}">doi</a>{% endif %}
      {% if p.links.pdf and p.links.pdf != "" %}<a href="{{ p.links.pdf | relative_url }}">pdf</a>{% endif %}
      {% if p.links.abstract and p.links.abstract != "" %}<a href="{{ p.links.abstract | relative_url }}">abstract</a>{% endif %}
      {% if p.links.preprint and p.links.preprint != "" %}<a href="{{ p.links.preprint }}">preprint</a>{% endif %}
      {% if p.links.publisher and p.links.publisher != "" %}<a href="{{ p.links.publisher }}">publisher</a>{% endif %}
      {% if p.links.slides and p.links.slides != "" %}<a href="{{ p.links.slides }}">slides</a>{% endif %}
      {% if p.links.handout and p.links.handout != "" %}<a href="{{ p.links.handout | relative_url }}">handout</a>{% endif %}
    </div>
    {% endif %}
  </li>
  {% endfor %}
</ul>
{% endif %}
