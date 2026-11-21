---
# Existing filenames are retained for overwrite-safe installation.
# Use the date and event fields below rather than inferring dates from filenames.
title: Multiscale Mechanical Modelling of Medical Textile for Female Pelvic Organ Repair
collection: conferences
layout: archive
permalink: /conference/2026-medical-textile-mechanics/
authors:
- Rohit Raju Madke
- Amira Mziou
- Ayman Arwany
- Frédéric Turquier
year: 2026
date: '2026-07-19'
event_start_date: '2026-07-19'
event_end_date: '2026-07-24'
event_dates: 19–24 July 2026
conference: 17th World Congress on Computational Mechanics and 10th ECCOMAS Congress (WCCM–ECCOMAS 2026)
venue: Munich, Germany
contribution_type: Oral presentation
status: Oral presentation
presenter: Rohit Raju Madke
record_url: https://wccm-eccomas2026.org/
citation: R. R. Madke, A. Mziou, A. Arwany, and F. Turquier (2026). Multiscale Mechanical Modelling of Medical Textile
  for Female Pelvic Organ Repair. 17th World Congress on Computational Mechanics and 10th ECCOMAS Congress (WCCM–ECCOMAS
  2026), Munich, Germany, 19–24 July 2026. [Oral presentation].
summary: Oral presentation of research on the mechanical characterisation and multiscale modelling of knitted medical
  textiles for pelvic organ prolapse repair.
excerpt: Oral presentation. Oral presentation of research on the mechanical characterisation and multiscale modelling
  of knitted medical textiles for pelvic organ prolapse repair.
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
