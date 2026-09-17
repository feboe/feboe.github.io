---
layout: default
title: Technical Project Portfolio
description: Selected projects in energy systems, optimization, simulation, and data-driven engineering by Felix Bötsch.
permalink: /
---

<header class="portfolio-hero" id="top">
  <p class="eyebrow">Technical Project Portfolio</p>
  <h1>Felix Bötsch</h1>
  <p class="hero-title">Optimization Engineer <span aria-hidden="true">|</span> Applied Data Scientist</p>
  <p class="hero-summary">
    I develop data-driven tools for engineering decisions: from mathematical optimization and simulation
    to energy analytics and industrial data workflows. My work focuses on translating physical constraints,
    operational requirements, and measured data into transparent, testable solutions.
  </p>
  <div class="hero-actions" aria-label="Profile links">
    <a class="button button-primary" href="https://github.com/feboe" target="_blank" rel="noopener noreferrer">
      <i class="fab fa-github" aria-hidden="true"></i>
      GitHub profile
    </a>
    <a class="button button-secondary" href="#energy">Explore projects</a>
  </div>
</header>

<div class="portfolio-content">
  {% for section in site.data.projects.sections %}
    <section class="project-section" id="{{ section.id }}" aria-labelledby="{{ section.id }}-title">
      <div class="section-heading">
        <p class="section-index">0{{ forloop.index }}</p>
        <div>
          <h2 id="{{ section.id }}-title">{{ section.title }}</h2>
          <p>{{ section.intro }}</p>
        </div>
      </div>

      <div class="project-grid{% if section.compact %} project-grid-compact{% endif %}">
        {% for project in section.projects %}
          {% include project-card.html project=project compact=section.compact %}
        {% endfor %}
      </div>
    </section>
  {% endfor %}
</div>
