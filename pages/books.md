---
layout: platform
title: Inspection Guides
permalink: /books/
description: Practical inspection guides from the 18-book Inspector's Handbook Series.
---

<section class="guide-hero">
  <div class="shell guide-hero__inner">
    <p class="eyebrow">The Inspector's Handbook Series</p>
    <h1>Practical inspection guides built for the field.</h1>
    <p>Clear, focused guidance for inspectors, QA/QC personnel, supervisors, technicians, and industrial professionals. The complete 18-book series is available in paperback and Kindle formats on Amazon.</p>
    <div class="button-row">
      <a class="button button--primary" href="https://www.amazon.com/dp/B0H1GWNNQ8" target="_blank" rel="noopener noreferrer">View the 18-book series on Amazon</a>
      <a class="button button--secondary" href="#available-guides">Browse all guides</a>
    </div>
  </div>
</section>

<section class="section section--light" id="available-guides">
  <div class="shell">
    <div class="section-heading">
      <p class="eyebrow">Available now</p>
      <h2>Inspection Guides</h2>
      <p>Choose a discipline to see the guide details, or use the Amazon series link to browse every available format.</p>
    </div>
    <div class="guide-grid">
      {% assign guides = "general-fabrication-shop-inspector|General Fabrication Shop Inspector,welding-inspector|Welding Inspector,pressure-vessel-inspector|Pressure Vessel Inspector,piping-inspector|Piping Inspector,heat-exchanger-inspector|Heat Exchanger Inspector,boiler-inspector|Boiler Inspector,structural-steel-inspector|Structural Steel Inspector,pipeline-inspector|Pipeline Inspector,turnaround-inspector|Turnaround Inspector,nde-inspector|NDE Inspector,coating-inspector|Coating Inspector,fireproofing-refractory-inspector|Fireproofing & Refractory Inspector,tank-inspector|Tank Inspector,rotating-equipment-inspector|Rotating Equipment Inspector,crane-rigging-inspector|Crane & Rigging Inspector,valve-inspector|Valve Inspector,instrumentation-electrical-inspector|Instrumentation & Electrical Inspector,qaqc-documentation-records-inspector|QA/QC Documentation & Records Inspector" | split: "," %}
      {% for guide in guides %}
        {% assign parts = guide | split: "|" %}
        <article class="guide-card">
          <img src="{{ '/assets/book-covers/' | append: parts[0] | append: '-cover.jpg' | relative_url }}" alt="Cover of The {{ parts[1] }}">
          <div>
            <p class="guide-card__series">Inspector's Handbook Series</p>
            <h3>The {{ parts[1] }}</h3>
            <a href="{{ '/books/' | append: parts[0] | append: '/' | relative_url }}">View guide details <span aria-hidden="true">&rarr;</span></a>
          </div>
        </article>
      {% endfor %}
    </div>
    <p class="affiliate-note">Amazon opens in a new window. Toolbox to Table may earn a commission from qualifying affiliate purchases, at no additional cost to you, when affiliate links are used.</p>
  </div>
</section>
