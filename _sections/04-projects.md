---
title: "Projects"
eyebrow: This year
section_id: projects
weight: 40
section_class: "section--alt"
---

Each team's project — click through for goals, methods, and outcomes.

<div class="project-grid">
{% assign sorted_projects = site.projects | sort: 'title' %}
{% for project in sorted_projects %}
  <a class="project-card" href="{{ project.url | relative_url }}">
    {% if project.theme %}<span class="project-card__theme">{{ project.theme }}</span>{% endif %}
    <h3 class="card__title">{{ project.title }}</h3>
    {% if project.lead %}<p class="card__body">{{ project.lead }}</p>{% endif %}
    {% if project.lead_author %}
      <p class="project-card__lead">
        Lead: {{ project.lead_author }}{% if project.lead_affiliation %}, {{ project.lead_affiliation }}{% endif %}
      </p>
    {% endif %}
    <span class="card__cta">View project</span>
  </a>
{% endfor %}
</div>
