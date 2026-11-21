---
# Existing filenames are retained for overwrite-safe installation.
# Use the date and event fields below rather than inferring dates from filenames.
title: Multi-objective optimization of a fabric reinforced composite
collection: conferences
layout: archive
permalink: /conference/2019-fabric-composite-optimization/
authors:
- Rohit Raju Madke
- Rajib Chowdhury
year: 2019
date: '2019-03-22'
event_start_date: '2019-03-22'
event_end_date: '2019-03-23'
event_dates: 22–23 March 2019
conference: 2nd National Conference on Multidisciplinary Design, Analysis and Optimization (NCMDAO-2)
venue: M. S. Ramaiah University of Applied Sciences, Bengaluru, India
contribution_type: Conference contribution
status: Conference contribution
record_url: https://ncmdao.github.io/webpage/2019.html
citation: R. R. Madke and R. Chowdhury (2019). Multi-objective optimization of a fabric reinforced composite. 2nd
  National Conference on Multidisciplinary Design, Analysis and Optimization (NCMDAO-2), M. S. Ramaiah University
  of Applied Sciences, Bengaluru, India, 22–23 March 2019. [Conference contribution].
summary: A multi-objective optimisation approach is considered for the lightweight design of fabric-reinforced composites
  using multiscale modelling.
excerpt: Conference contribution. A multi-objective optimisation approach is considered for the lightweight design
  of fabric-reinforced composites using multiscale modelling.
last_modified_at: '2026-11-21'
---

**Contribution:** {{ page.contribution_type }}

**Conference:** {{ page.conference }}

**Event dates:** {{ page.event_dates }}

**Venue:** {{ page.venue }}
{% if page.presentation_date %}

**Presentation date:** {{ page.presentation_date | date: '%-d %B %Y' }}
{% endif %}
{% if page.record_id %}

**Reference:** {{ page.record_id }}
{% endif %}

## Research summary

{{ page.summary }}

## Citation

{{ page.citation }}
{% if page.paperurl %}

[Read the paper / communication]({{ page.paperurl }})
{% endif %}
{% if page.record_url %}

[Programme / conference record]({{ page.record_url }})
{% endif %}
{% if page.event_url %}

[Conference information]({{ page.event_url }})
{% endif %}

[All conference contributions]({{ '/conferences/' | relative_url }}) &nbsp; | &nbsp; [Journal publications]({{ '/publications/' | relative_url }})
