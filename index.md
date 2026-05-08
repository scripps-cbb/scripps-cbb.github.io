---
layout: home
title: Home
description: "Computational biology & bioinformatics hackathon — bring a problem, leave with a prototype."
---

{% assign sections = site.sections | sort: 'weight' %}
{% for s in sections %}
<section class="section {{ s.section_class }}" id="{{ s.section_id }}">
  <div class="container">
    <div class="section__header">
      {% if s.eyebrow %}<p class="section__eyebrow">{{ s.eyebrow }}</p>{% endif %}
      <h2 class="section__title">{{ s.title }}</h2>
    </div>
    <div class="section__body prose">
      {{ s.content }}
    </div>
  </div>
</section>
{% endfor %}
