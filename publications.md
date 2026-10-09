---
layout: default
title: Publications
permalink: /publications/
---

# Publications

## Peer-reviewed articles

<ul class="pub-list">
{% for p in site.data.publications.articles %}
  <li>{{ p.authors }} ({{ p.year }}). <span class="title">{{ p.title }}.</span> <span class="venue">{{ p.venue }}</span>{% if p.detail %}, {{ p.detail }}{% endif %}.{% if p.note %} <span class="meta">{{ p.note }}.</span>{% endif %}<span class="links">{% if p.doi %}<a href="https://doi.org/{{ p.doi }}">DOI</a>{% endif %}{% if p.url %}<a href="{{ p.url }}">PDF</a>{% endif %}</span></li>
{% endfor %}
</ul>

## Working papers

<ul class="pub-list">
{% for p in site.data.publications.working_papers %}
  <li>{{ p.authors }}{% if p.year %} ({{ p.year }}){% endif %}. <span class="title">{{ p.title }}.</span>{% if p.status %} <span class="meta">{{ p.status }} <span class="venue">{{ p.venue }}</span>.</span>{% endif %}{% if p.note %} <span class="meta">{{ p.note }}.</span>{% endif %}<span class="links">{% if p.url %}<a href="{{ p.url }}">PDF</a>{% endif %}</span></li>
{% endfor %}
</ul>

## Policy reports

<ul class="pub-list">
{% for p in site.data.publications.reports %}
  <li>{{ p.authors }} ({{ p.year }}). <span class="title">{{ p.title }}.</span> {{ p.venue }}.<span class="links">{% if p.url %}<a href="{{ p.url }}">PDF</a>{% endif %}</span></li>
{% endfor %}
</ul>

## Conference presentations

<ul class="pub-list">
{% for p in site.data.publications.presentations %}
  <li><span class="title">{{ p.title }}.</span> {{ p.venue }}, {{ p.detail }}.{% if p.note %} <span class="meta">With {{ p.note | remove: "with " }}.</span>{% endif %}</li>
{% endfor %}
</ul>
