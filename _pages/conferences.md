---
layout: archive
title: "Conference Contributions"
permalink: /conferences/
excerpt: "Conference papers, short communications, presentations, abstracts and accepted posters co-authored by Rohit Raju Madke."
author_profile: true
last_modified_at: "2026-11-21"
---

Conference papers, short communications, presentations, abstracts and accepted posters are listed by year. Each entry identifies the contribution type and provides links to the available publication or conference record.

<p>
  <a class="btn btn--primary" href="{{ '/publications/' | relative_url }}">Journal publications</a>
  <a class="btn btn--inverse" href="{{ '/talks/' | relative_url }}">Talks and workshops</a>
  <a class="btn btn--inverse" href="{{ '/cv/' | relative_url }}">CV</a>
</p>

{% if site.author.googlescholar and site.author.googlescholar != '' %}
<p>See also my <a href="{{ site.author.googlescholar | escape }}">Google Scholar profile</a>.</p>
{% endif %}

{% comment %}
Maintain entries in _conferences with year, date, citation, contribution_type
and summary fields. Only published work should have a paperurl; programmes and
conference records use record_url. The citation already includes the contribution
type. Sort by actual metadata dates, rather than legacy filename dates.
{% endcomment %}
{% assign ordered_contributions = site.conferences | sort: 'date' | reverse %}
{% assign conference_years = ordered_contributions | group_by: 'year' %}

{% if ordered_contributions.size > 0 %}
{% for year_group in conference_years %}
<h2>{{ year_group.name | default: 'Other contributions' | escape }}</h2>

<ol class="conference-list">
{% for contribution in year_group.items %}
  {% assign citation = contribution.citation | default: contribution.title | escape %}
  {% if contribution.contribution_type and contribution.contribution_type != '' %}
    {% assign escaped_type = contribution.contribution_type | escape %}
    {% capture type_label %}<strong>{{ escaped_type }}</strong>{% endcapture %}
    {% assign citation = citation | replace: escaped_type, type_label %}
  {% endif %}
  {% if citation contains 'R. R. Madke' %}
    {% assign citation = citation | replace: 'R. R. Madke', '<strong>R. R. Madke</strong>' %}
  {% elsif citation contains 'R. Madke' %}
    {% assign citation = citation | replace: 'R. Madke', '<strong>R. Madke</strong>' %}
  {% endif %}
  <li>
    <p>{{ citation }}</p>
    <p>
      <a href="{{ contribution.url | relative_url }}" aria-label="Details for {{ contribution.title | escape }}">Details</a>
      {% if contribution.paperurl and contribution.paperurl != '' %}
        &nbsp;&middot;&nbsp; <a href="{{ contribution.paperurl | escape }}" aria-label="Read publication: {{ contribution.title | escape }}">Read publication</a>
      {% endif %}
      {% if contribution.record_url and contribution.record_url != '' %}
        &nbsp;&middot;&nbsp; <a href="{{ contribution.record_url | escape }}" aria-label="Programme or record for {{ contribution.title | escape }}">Programme / record</a>
      {% endif %}
    </p>
    {% if contribution.summary and contribution.summary != '' %}
    <details>
      <summary>Research summary</summary>
      <p>{{ contribution.summary | escape }}</p>
    </details>
    {% endif %}
  </li>
{% endfor %}
</ol>
{% endfor %}
{% else %}
<p>Conference records are being updated. See my <a href="{{ '/cv/' | relative_url }}">CV</a> for selected contributions.</p>
{% endif %}

*Last reviewed: {{ page.last_modified_at | date: '%B %Y' }}.*
