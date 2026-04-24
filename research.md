---
layout: default
title: "Research"
permalink: /research/
description: "Research by Willis Chun Lai Wong — syntactic symmetry, the Choiceless Computation Theorem, labeling theory, Distributed Morphology, Sinitic reduplication, Right Node Raising."
---

<h1>Research</h1>

<h2 class="section-heading">Interests</h2>

<div class="card">
  <h3>Syntactic symmetry &amp; Choiceless Computation</h3>
  <p>
    A crash-tolerant architecture in which Merge generates freely while
    deterministic interface evaluators cannot arbitrarily break structural
    symmetry. The <em>Choiceless Computation Theorem</em> delivers a 2×2
    typology unifying ATB extraction, Right Node Raising, and Sinitic
    AABB / ABAB reduplication.
  </p>
</div>

<div class="card">
  <h3>Labeling theory &amp; the Merge–interface boundary</h3>
  <p>
    Recasting the labeling algorithm (Chomsky 2013, 2015) in
    automorphism-theoretic terms; the ignition problem; when symmetry must be
    broken in Narrow Syntax versus when it can persist to PF / LF.
  </p>
</div>

<div class="card">
  <h3>Coordination, ellipsis, and rightward effects</h3>
  <p>
    Right Node Raising, ATB extraction, Suspended Affixation. Deriving the
    Right-Edge Restriction, the ban on selective deletion, and featural
    identity requirements from a single algebraic trigger — without rightward
    movement.
  </p>
</div>

<div class="card">
  <h3>Distributed Morphology &amp; Sinitic reduplication</h3>
  <p>
    Cantonese and Mandarin adjectival coordinatives and the <em>*AB</em> gap;
    phase-locality accounts of reduplication; ideophones and prosodic integrity.
  </p>
</div>

<h2 class="section-heading">Working papers</h2>

<div class="card">
  <h3>If You Can't Break It, Keep It: Choiceless Computation under Syntactic Symmetry</h3>
  <p class="muted small">Manuscript · under submission</p>
  <p>
    Sinitic adjectival coordinatives systematically exclude the simplex
    <em>*AB</em> form while requiring reduplicated outputs AABB or ABAB. I
    argue that this gap follows from a restriction on deterministic evaluation
    over symmetric domains, formalized as the Choiceless Computation Theorem
    (CCT). The CCT recasts Chomsky's labeling theory in automorphism-theoretic
    terms, adds a fourth case (the Null Label), and yields a falsifiable 2×2
    typology unifying AABB distributive exponence, ABAB pied-piping, ATB
    extraction, and Right Node Raising.
  </p>
  <p class="pub-links">
    <a href="{{ '/docs/if-you-cant-break-it-keep-it-manuscript.pdf' | relative_url }}">manuscript</a>
  </p>
</div>

<div class="card">
  <h3>Caught Between Two Nodes: The Choiceless Computation of Right Node Raising</h3>
  <p class="muted small">Abstract · Rightward Movement Workshop</p>
  <p>
    RNR obeys a Right-Edge Restriction, requires identity between conjuncts,
    and disallows selective deletion. I recover Sabbagh's (2007) architectural
    unification of RNR with ATB — as independent resolutions of structural
    symmetry — while relocating its mechanism: the uniformity is real, the
    rightward displacement is not. A corollary predicts Left Node Raising in
    head-final languages, and places Suspended Affixation in the RNR cell.
  </p>
  <p class="pub-links">
    <a href="{{ '/docs/2026-RNR-workshop-abstract.pdf' | relative_url }}">abstract</a>
  </p>
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
