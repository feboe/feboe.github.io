---
layout: default
title: Felix Bötsch | Technical Project Portfolio
description: Selected projects in energy systems, optimization, simulation, and data-driven engineering by Felix Bötsch.
permalink: /
---

<header class="portfolio-hero" id="top">
  <p class="eyebrow">Technical Project Portfolio</p>
  <h1>Felix Bötsch</h1>
  <p class="hero-title">Optimization Engineer <span aria-hidden="true">|</span> Applied Data Scientist</p>
  <p class="hero-summary">
    I build optimization, simulation, and data tools for engineering decisions across energy and industrial systems.
    My work combines physical constraints, operational data, and transparent validation—from forecasting and
    mathematical programming to production-facing software.
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

      {% assign section_projects = site.projects | where: "category", section.id | sort: "order" %}
      <div class="project-overview-grid">
        {% for project in section_projects %}
          {% include project-overview-card.html project=project %}
        {% endfor %}
      </div>
    </section>
  {% endfor %}
</div>
