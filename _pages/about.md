---
layout: lab
home: true
permalink: /
title: "Information and Decision Systems (IDS) Lab"
description: "Research on AI and Physical AI, communication and edge systems, quantum information, and emerging public-sector decision support."
redirect_from:
  - /about/
  - /about.html
---

<figure class="research-banner">
  <img src="{{ '/assets/images/nds-research-hero.webp' | relative_url }}" width="2172" height="724" alt="Conceptual illustration of quantum information, terrestrial and aerial networks, and decision paths." fetchpriority="high" decoding="async">
</figure>

<div class="home-columns">
  <div class="home-about">
    <section class="hero" aria-label="About IDS Lab">
      <p class="hero-intro">We study how information and decisions shape one another in classical and quantum systems under constraints and uncertainty. We investigate the resulting performance limits and trade-offs to guide the design of communication networks, AI systems, and decision algorithms.</p>
    </section>
    <section class="research-overview" aria-label="Research themes">
      <div class="research-grid">
        <a class="research-area" href="{{ '/research/#limits' | relative_url }}"><span class="area-number">01</span><div><h3>Performance Limits and Trade-offs</h3><p>What is achievable, and what performance can be guaranteed?</p></div><span class="area-arrow" aria-hidden="true">↗</span></a>
        <a class="research-area" href="{{ '/research/#networks' | relative_url }}"><span class="area-number">02</span><div><h3>System Design and Resource Management</h3><p>How should systems be configured and resources shared?</p></div><span class="area-arrow" aria-hidden="true">↗</span></a>
        <a class="research-area" href="{{ '/research/#decisions' | relative_url }}"><span class="area-number">03</span><div><h3>Learning and Decision-Making</h3><p>How should systems act when their environment is not fully known?</p></div><span class="area-arrow" aria-hidden="true">↗</span></a>
      </div>
      <a class="text-link research-details" href="{{ '/research/' | relative_url }}">Explore our research <span aria-hidden="true">→</span></a>
    </section>
  </div>
  <section class="home-news" aria-labelledby="news-title">
    <div class="section-heading"><h2 id="news-title">News</h2><a href="{{ '/news/' | relative_url }}">All news <span aria-hidden="true">→</span></a></div>
    {% include lab-news.html limit=6 %}
  </section>
</div>

<aside class="join-strip"><div><h2>Join IDS Lab</h2><p>We welcome inquiries from prospective M.S. and Ph.D. students.</p></div><a class="text-link" href="{{ '/contact/' | relative_url }}">Get in touch <span aria-hidden="true">→</span></a></aside>
