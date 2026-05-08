---
title: "Organizing committee"
eyebrow: Organizers
section_id: organizers
weight: 50
---

The team running the hackathon. Reach the committee at
[{{ site.event.contact_email }}](mailto:{{ site.event.contact_email }}).

<div class="people-grid">
{% for p in site.data.organizers %}
  <div class="person">
    {% if p.role %}<p class="person__role">{{ p.role }}</p>{% endif %}
    <p class="person__name">
      {% if p.url and p.url != "" %}<a href="{{ p.url }}">{{ p.name }}</a>{% else %}{{ p.name }}{% endif %}
    </p>
    {% if p.affiliation %}<p class="person__affiliation">{{ p.affiliation }}</p>{% endif %}
  </div>
{% endfor %}
</div>
