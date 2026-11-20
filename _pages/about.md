---
layout: single
permalink: /
title: "Computational Mechanics"
excerpt: "Rohit Raju Madke studies medical textiles, mechanical metamaterials and impact protection using nonlinear finite element and multiscale modelling."
author_profile: true
redirect_from:
  - /about/
  - /about.html
last_modified_at: "2026-11-20"
---

I am a postdoctoral researcher at the **Laboratory of Applied Biomechanics (LBA), Aix-Marseille University, France**, within the MICH Chair *Innovative Materials for the Human Body*. I develop computational models of textiles, composites and cellular materials for biomedical applications and impact protection.

<p>
  <a class="btn btn--primary" href="{{ '/publications/' | relative_url }}">Publications</a>
  <a class="btn btn--inverse" href="{{ '/cv/' | relative_url }}">CV</a>
  <a class="btn btn--inverse" href="#contact">Contact</a>
</p>

## Research

### Medical textiles

I develop yarn-scale finite element models of knitted medical textiles, accounting for large deformation and frictional contact. I compare the predicted mechanical response and pore deformation with experimental measurements, and connect yarn-scale behaviour with homogenised fabric models for pelvic organ prolapse repair.

### Helmet impact protection

I use LS-DYNA to investigate textile reinforcement in protective helmets under normal and oblique impacts. This work examines energy absorption and linear and angular head acceleration, with the aim of understanding how the reinforcement changes the protective response.

### Mechanical metamaterials and metacomposites

My doctoral research examined braided metacomposites, auxetic and dual-negative architectures, and ballistic-impact behaviour of multilayered body-armour concepts. My later postdoctoral work at the Indian Institute of Technology Roorkee included topology optimisation using LS-TaSC and the study of cellular materials for energy absorption.

### E-textiles and sensing

I contribute to mechanical and optical modelling studies of textiles incorporating fibre Bragg grating sensors. The work examines deformation, strain transfer and sensing requirements for protective and biomedical applications.

## Background

I received my PhD in **Civil Engineering, specialising in Structural Engineering**, from the **Indian Institute of Technology Roorkee** in 2022. Before joining Aix-Marseille University in September 2025, I held research appointments at the Indian Institute of Technology Roorkee (2024-2025) and San Diego State University, USA (2023-2024). These appointments covered architected materials and the static and fatigue behaviour of aerospace composite joints.

## Teaching and supervision

At the Indian Institute of Technology Roorkee, I supported teaching in finite element methods, structural dynamics and solid mechanics. At LBA, I supervise master's research and co-supervise doctoral work on strain measurement in protective helmets. [Teaching details]({{ '/teaching/' | relative_url }}).

## Methods and software

Nonlinear finite element analysis, multiscale modelling, homogenisation, contact, impact and material failure. My software experience includes **LS-DYNA, Abaqus, Ansys Mechanical, ACP, Autodyn, COMSOL and LS-TaSC**, supported by Python, MATLAB and Fortran UMAT/VUMAT development.

## Selected publications

{% comment %}Publication filenames follow YYYY-MM-DD-title.md.{% endcomment %}
{% assign selected_publications = site.publications | sort: 'path' | reverse %}
<ul>
{% for publication in selected_publications limit:3 %}
  {% assign publication_filename = publication.path | split: '/' | last %}
  <li>
    <a href="{{ publication.paperurl | escape }}">{{ publication.title | escape }}</a><br>
    <small><em>{{ publication.venue | escape }}</em>, {{ publication_filename | slice: 0, 4 }}.</small>
  </li>
{% endfor %}
</ul>

[View all publications]({{ '/publications/' | relative_url }}).

## Contact

Laboratory of Applied Biomechanics, Aix-Marseille University, Marseille, France.

[Email](mailto:{{ site.author.email }}) &nbsp; | &nbsp; [LinkedIn](https://www.linkedin.com/in/rohit-raju-madke-phd-a1aa4251/) &nbsp; | &nbsp; [Google Scholar](https://scholar.google.com/citations?user=QmkU4OgAAAAJ&hl=en)

*Last reviewed: {{ page.last_modified_at | date: '%B %Y' }}.*
