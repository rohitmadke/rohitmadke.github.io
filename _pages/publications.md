---
layout: archive
title: "Publications"
permalink: /publications/
excerpt: "Journal publications by Rohit Raju Madke in textile and composite mechanics, architected materials, impact and multiscale modelling."
author_profile: true
last_modified_at: "2026-11-20"
---

My publications concern textile and composite mechanics, architected materials, impact and multiscale modelling. Article links below lead to the publisher or DOI record.

{% if site.author.googlescholar and site.author.googlescholar != '' %}
<p>
  <a class="btn btn--primary" href="{{ site.author.googlescholar | escape }}">Google Scholar</a>
  <a class="btn btn--inverse" href="{{ '/conferences/' | relative_url }}">Conference contributions</a>
</p>
{% else %}
[Conference contributions]({{ '/conferences/' | relative_url }})
{% endif %}

## Journal articles

{% comment %}
Publication records are maintained in _publications, using YYYY-MM-DD-title.md
filenames. Each record should contain title, venue, citation and paperurl.
Render the citation once and use paperurl directly: older records may have
external URLs in permalink and no explicit publication date.
{% endcomment %}
{% assign journal_publications = site.publications | sort: 'path' | reverse %}

{% if journal_publications.size > 0 %}
<ol class="publication-list">
{% for publication in journal_publications %}
  <li>
    <p>
      {% if publication.citation and publication.citation != '' %}
        {{ publication.citation | escape | replace: 'R. R. Madke', '<strong>R. R. Madke</strong>' }}
      {% else %}
        <strong>{{ publication.title | escape }}</strong>{% if publication.venue %}. <em>{{ publication.venue | escape }}</em>{% endif %}{% if publication.year %}, {{ publication.year | escape }}{% endif %}.
      {% endif %}
      {% if publication.paperurl and publication.paperurl != '' %}
        <a href="{{ publication.paperurl | escape }}" aria-label="Read {{ publication.title | escape }}">Article / DOI</a>
      {% endif %}
    </p>
    {% if publication.excerpt and publication.excerpt != '' %}
    <details>
      <summary>Research summary</summary>
      <div>{{ publication.excerpt | markdownify }}</div>
    </details>
    {% endif %}
  </li>
{% endfor %}
</ol>
{% else %}
<p>Publication records are being updated.{% if site.author.googlescholar and site.author.googlescholar != '' %} See <a href="{{ site.author.googlescholar | escape }}">Google Scholar</a> for my publication record.{% endif %}</p>
{% endif %}

Conference papers, presentations and abstracts are listed on the [conference page]({{ '/conferences/' | relative_url }}).

*Last reviewed: {{ page.last_modified_at | date: '%B %Y' }}.*
