---
title: "Judges"
eyebrow: Judges
section_id: judges
weight: 55
---

The panel evaluating final project presentations on Monday.

<div class="people-grid">
{% for p in site.data.judges %}
  <div class="person">
    {% if p.role %}<p class="person__role">{{ p.role }}</p>{% endif %}
    <p class="person__name">
      {% if p.url and p.url != "" %}<a href="{{ p.url }}">{{ p.name }}</a>{% else %}{{ p.name }}{% endif %}
    </p>
    {% if p.affiliation %}<p class="person__affiliation">{{ p.affiliation }}</p>{% endif %}
  </div>
{% endfor %}
</div>
