---
title: "Partners & sponsors"
eyebrow: Partners
section_id: partners
weight: 60
section_class: "section--alt"
---

We're grateful for the support of the following institutes and
organizations.

<div class="partner-grid">
{% for p in site.data.partners %}
  <a class="partner" {% if p.url and p.url != "" %}href="{{ p.url }}"{% endif %} aria-label="{{ p.name }}">
    {% if p.logo and p.logo != "" %}
      <img src="{{ p.logo | prepend: '/assets/images/' | relative_url }}" alt="{{ p.name }}">
    {% else %}
      <span class="partner__placeholder">{{ p.name }}</span>
    {% endif %}
  </a>
{% endfor %}
</div>

Interested in sponsoring or partnering on the next hackathon? Get in touch
at [{{ site.event.contact_email }}](mailto:{{ site.event.contact_email }}).
