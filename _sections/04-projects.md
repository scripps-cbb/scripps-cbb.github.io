---
title: "Projects"
eyebrow: This year
section_id: projects
weight: 40
section_class: "section--alt"
---

Each team's project — click through for goals, methods, and outcomes.
Want to add one? [Submit a project idea →](https://github.com/scripps-cbb/scripps-cbb.github.io/issues/new?template=project-idea.yml)

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
  <a class="project-card" href="https://github.com/scripps-cbb/scripps-cbb.github.io/issues/new?template=project-idea.yml">
    <span class="project-card__theme">Open call</span>
    <h3 class="card__title">Have a project idea?</h3>
    <p class="card__body">Pitch your own project — four required fields, takes a couple of minutes. Approved ideas land here as a card.</p>
    <span class="card__cta">Submit a project idea</span>
  </a>
</div>
