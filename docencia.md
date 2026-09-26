---
layout: default
title: Docencia
nav_order: 5
description: Trayectoria docente, asignaturas y portafolios de estudiantes de Joel Arango Ramírez.
permalink: /docencia/
---

# Docencia

<div class="teaching-intro">
  <p>Mi enfoque docente combina fundamentos de ingeniería con aprendizaje basado en proyectos. Los estudiantes diseñan, construyen, programan, integran y documentan soluciones que conectan hardware, software, comunicaciones y tecnologías emergentes.</p>
</div>

## Asignaturas actuales

<div class="course-grid">
  <article class="course-card">
    <span>Asignatura actual</span>
    <h3>Sistemas Ciberfísicos</h3>
    <p>Integración de sistemas físicos y digitales mediante sensores, actuadores, sistemas embebidos, comunicaciones, software, plataformas web, IoT y control.</p>
  </article>
  <article class="course-card">
    <span>Asignatura actual</span>
    <h3>Tecnologías Emergentes</h3>
    <p>Exploración y aplicación de herramientas como realidad extendida, inteligencia artificial, sistemas conectados, simulación, interfaces interactivas y nuevas plataformas de desarrollo.</p>
  </article>
</div>

## Asignaturas impartidas anteriormente

<div class="course-grid">
  <article class="course-card">
    <span>Experiencia docente</span>
    <h3>Automatización</h3>
    <p>PLC, HMI, sensores, actuadores, comunicaciones industriales, control de procesos, robótica y desarrollo de prácticas orientadas a aplicaciones reales.</p>
  </article>
  <article class="course-card">
    <span>Experiencia docente</span>
    <h3>Prospectiva Tecnológica</h3>
    <p>Análisis de tendencias, escenarios futuros, impacto de tecnologías emergentes y evaluación de oportunidades para la innovación.</p>
  </article>
</div>

## Metodología de enseñanza

Mi participación incluye acompañamiento conceptual y trabajo técnico directo durante el desarrollo de los proyectos:

- Definición del problema y objetivos.
- Investigación y selección de tecnologías.
- Diseño de la arquitectura del sistema.
- Selección e integración de componentes electrónicos.
- Programación de microcontroladores, aplicaciones y comunicaciones.
- Integración de sensores, actuadores, motores, bases de datos y servicios web.
- Diagnóstico de fallas, pruebas y mejora iterativa.
- Documentación técnica, presentación y publicación de resultados.
- Creación de portafolios mediante GitHub Pages.

---

## Portafolios — Sistemas Ciberfísicos

Los siguientes sitios documentan proyectos desarrollados por estudiantes de la asignatura.

{% assign ciberfisicos = site.data.portafolios_alumnos.sistemas_ciberfisicos %}
{% if ciberfisicos and ciberfisicos.size > 0 %}
<div class="student-sites-grid">
{% for proyecto in ciberfisicos %}
  <article class="student-site-card">
    <span class="student-site-card__course">Sistemas Ciberfísicos</span>
    <h3>{{ proyecto.proyecto }}</h3>
    <p class="student-site-card__student">{{ proyecto.estudiante }}</p>
    <p>{{ proyecto.descripcion }}</p>
    <div class="student-site-actions">
      <a href="{{ proyecto.sitio }}" target="_blank" rel="noopener">Ver portafolio</a>
      {% if proyecto.repositorio %}
      <a href="{{ proyecto.repositorio }}" target="_blank" rel="noopener">Ver repositorio</a>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>
{% else %}
<p class="student-sites-empty">Los portafolios de esta asignatura se incorporarán conforme los estudiantes publiquen sus proyectos.</p>
{% endif %}

## Portafolios — Tecnologías Emergentes

Los siguientes sitios reúnen prácticas, prototipos y evidencias desarrolladas por estudiantes de la asignatura.

{% assign emergentes = site.data.portafolios_alumnos.tecnologias_emergentes %}
{% if emergentes and emergentes.size > 0 %}
<div class="student-sites-grid">
{% for proyecto in emergentes %}
  <article class="student-site-card">
    <span class="student-site-card__course">Tecnologías Emergentes</span>
    <h3>{{ proyecto.proyecto }}</h3>
    <p class="student-site-card__student">{{ proyecto.estudiante }}</p>
    <p>{{ proyecto.descripcion }}</p>
    <div class="student-site-actions">
      <a href="{{ proyecto.sitio }}" target="_blank" rel="noopener">Ver portafolio</a>
      {% if proyecto.repositorio %}
      <a href="{{ proyecto.repositorio }}" target="_blank" rel="noopener">Ver repositorio</a>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>
{% else %}
<p class="student-sites-empty">Los portafolios de esta asignatura se incorporarán conforme los estudiantes publiquen sus proyectos.</p>
{% endif %}

<details class="portfolio-data-help">
  <summary>Cómo agregar un nuevo portafolio</summary>
  <p>Los sitios se administran desde <code>_data/portafolios_alumnos.yml</code>. Solo es necesario agregar el nombre del estudiante, el título del proyecto, una descripción breve, la dirección de GitHub Pages y, opcionalmente, la dirección del repositorio.</p>
</details>

## Propósito formativo

El objetivo es que cada estudiante termine con una evidencia pública y organizada de su trabajo. Estos portafolios permiten mostrar el proceso de ingeniería, reconocer la autoría individual o del equipo y facilitar la continuidad de los proyectos en cursos posteriores.
