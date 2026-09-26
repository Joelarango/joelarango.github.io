---
layout: default
title: Teaching
nav_order: 5
description: Teaching experience, courses, and student portfolios of Joel Arango Ramírez.
permalink: /en/teaching/
---

# Teaching

<div class="teaching-intro">
  <p>My teaching approach combines engineering fundamentals with project-based learning. Students design, build, program, integrate, and document solutions connecting hardware, software, communications, and emerging technologies.</p>
</div>

## Current courses

<div class="course-grid">
  <article class="course-card">
    <span>Current course</span>
    <h3>Cyber-Physical Systems</h3>
    <p>Integration of physical and digital systems through sensors, actuators, embedded systems, communications, software, web platforms, IoT, and control.</p>
  </article>
  <article class="course-card">
    <span>Current course</span>
    <h3>Emerging Technologies</h3>
    <p>Exploration and application of extended reality, artificial intelligence, connected systems, simulation, interactive interfaces, and new development platforms.</p>
  </article>
</div>

## Previously taught courses

<div class="course-grid">
  <article class="course-card">
    <span>Teaching experience</span>
    <h3>Automation</h3>
    <p>PLCs, HMIs, sensors, actuators, industrial communications, process control, robotics, and practical work focused on real applications.</p>
  </article>
  <article class="course-card">
    <span>Teaching experience</span>
    <h3>Technology Foresight</h3>
    <p>Analysis of trends, future scenarios, the impact of emerging technologies, and assessment of innovation opportunities.</p>
  </article>
</div>

## Teaching methodology

My role includes conceptual guidance and direct technical work throughout project development:

- Problem and objective definition.
- Research and technology selection.
- System architecture design.
- Electronic component selection and integration.
- Programming of microcontrollers, applications, and communications.
- Integration of sensors, actuators, motors, databases, and web services.
- Technical documentation, presentation, and publication of results.
- Portfolio creation with GitHub Pages.

---

## Portfolios — Cyber-Physical Systems

The following sites document projects developed by students in this course.

{% assign ciberfisicos = site.data.portafolios_alumnos.sistemas_ciberfisicos %}
{% if ciberfisicos and ciberfisicos.size > 0 %}
<div class="student-sites-grid">
{% for proyecto in ciberfisicos %}
  <article class="student-site-card">
    <span class="student-site-card__course">Cyber-Physical Systems</span>
    <h3>{{ proyecto.proyecto }}</h3>
    <p class="student-site-card__student">{{ proyecto.estudiante }}</p>
    <p>{{ proyecto.descripcion }}</p>
    <div class="student-site-actions">
      <a href="{{ proyecto.sitio }}" target="_blank" rel="noopener">View portfolio</a>
      {% if proyecto.repositorio %}
      <a href="{{ proyecto.repositorio }}" target="_blank" rel="noopener">View repository</a>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>
{% else %}
<p class="student-sites-empty">Portfolios will be added as students publish their projects.</p>
{% endif %}

## Portfolios — Emerging Technologies

The following sites present assignments, prototypes, and evidence developed by students in this course.

{% assign emergentes = site.data.portafolios_alumnos.tecnologias_emergentes %}
{% if emergentes and emergentes.size > 0 %}
<div class="student-sites-grid">
{% for proyecto in emergentes %}
  <article class="student-site-card">
    <span class="student-site-card__course">Emerging Technologies</span>
    <h3>{{ proyecto.proyecto }}</h3>
    <p class="student-site-card__student">{{ proyecto.estudiante }}</p>
    <p>{{ proyecto.descripcion }}</p>
    <div class="student-site-actions">
      <a href="{{ proyecto.sitio }}" target="_blank" rel="noopener">View portfolio</a>
      {% if proyecto.repositorio %}
      <a href="{{ proyecto.repositorio }}" target="_blank" rel="noopener">View repository</a>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>
{% else %}
<p class="student-sites-empty">Portfolios will be added as students publish their projects.</p>
{% endif %}

<details class="portfolio-data-help">
  <summary>How to add a new portfolio</summary>
  <p>Sites are managed in <code>_data/portafolios_alumnos.yml</code>. Add the student's name, project title, a brief description, the GitHub Pages address, and optionally the repository address.</p>
</details>

## Educational purpose

The goal is for each student to finish with organized, public evidence of their work. These portfolios present the engineering process, acknowledge individual or team authorship, and facilitate project continuity in future courses.
