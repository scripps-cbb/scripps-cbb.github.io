---
title: "Get in touch"
eyebrow: Contact
section_id: contact
weight: 80
section_class: "section--alt"
---

**The Slack workspace is the primary channel** for hackathon
communication. All instructions, updates, and announcements will be
posted there, and it's the fastest way to reach the organizers if you
hit any problems.

[**Join the CBB Hackathon Slack →**]({{ site.event.slack_url }})

You can also reach out to any of the organizers listed above directly.

<p style="margin-top: 2rem;">
  {% if site.event.cta_url %}
    <a class="btn btn--accent btn--lg btn--with-icon" href="{{ site.event.cta_url }}"><img class="luma-icon" src="{{ '/assets/images/luma-icon.png' | relative_url }}" alt="" aria-hidden="true"><span>{{ site.event.cta_label }}</span></a>
  {% endif %}
  {% if site.event.slack_url %}
    <a class="btn btn--accent btn--lg btn--with-icon" href="{{ site.event.slack_url }}">{% include slack-logo.svg %}<span>{{ site.event.slack_label }}</span></a>
  {% endif %}
</p>
