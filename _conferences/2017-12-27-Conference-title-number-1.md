---
# Existing filenames are retained for overwrite-safe installation.
# Use the date and event fields below rather than inferring dates from filenames.
title: Numerical scheme for the prediction of elastic properties of textile composite
collection: conferences
layout: archive
permalink: /conference/2017-textile-composite-elastic-properties/
authors:
- Rohit Raju Madke
- Rajib Chowdhury
year: 2017
date: '2017-12-27'
event_start_date: '2017-12-27'
event_end_date: '2017-12-29'
event_dates: 27–29 December 2017
conference: International Conference on Composite Materials and Structures (ICCMS 2017)
venue: Indian Institute of Technology Hyderabad, India
contribution_type: Conference contribution
status: Conference contribution
record_url: https://imechanica.egr.uh.edu/sites/default/files/ICCMS_2017_final_brochure.pdf
citation: R. R. Madke and R. Chowdhury (2017). Numerical scheme for the prediction of elastic properties of textile
  composite. International Conference on Composite Materials and Structures (ICCMS 2017), Indian Institute of Technology
  Hyderabad, India, 27–29 December 2017. [Conference contribution].
summary: Representative-volume-element models of textile architectures are used to investigate effective elastic
  properties, combining TexGen geometry, finite element analysis and homogenisation approaches.
excerpt: Conference contribution. Representative-volume-element models of textile architectures are used to investigate
  effective elastic properties, combining TexGen geometry, finite element analysis and homogenisation approaches.
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
