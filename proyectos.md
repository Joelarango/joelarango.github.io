---
layout: default
title: Proyectos de robótica y XR
nav_order: 3
has_children: true
description: Proyectos de robótica, realidad extendida y gemelos digitales.
permalink: /proyectos/
---

# Proyectos de robótica y realidad extendida

Esta sección reúne proyectos relacionados con robótica colaborativa, realidad mixta, teleoperación, gemelos digitales e interacción humano-robot.

Cada proyecto documenta su objetivo, tecnologías utilizadas, arquitectura, desarrollo y resultados.

---

## Teleoperación de Yaskawa HC10 con HoloLens 2

Sistema de realidad mixta para controlar y programar trayectorias de un robot colaborativo Yaskawa MOTOMAN HC10.

La aplicación permite manipular un objetivo virtual, calcular el movimiento mediante cinemática inversa, registrar puntos de trayectoria y enviarlos mediante MQTT.

**Tecnologías principales:**

- Microsoft HoloLens 2.
- Unity y C#.
- OpenXR y MRTK.
- Yaskawa MOTOMAN HC10.
- MQTT y Python.
- RoboDK.

---

## Operación de robots Universal Robots con Meta Quest 3

Entorno inmersivo para visualizar, controlar y analizar el movimiento de robots UR3 y UR5 mediante Meta Quest 3.

El sistema conecta el entorno virtual con simuladores y robots mediante comunicación de red en tiempo real.

**Tecnologías principales:**

- Meta Quest 3.
- Unity y Meta XR SDK.
- Universal Robots UR3 y UR5.
- URScript.
- MQTT, UDP y Python.
- RoboDK.

---

## Gemelos digitales conectados

Desarrollo de representaciones virtuales de robots industriales capaces de recibir estados articulares, reproducir movimientos y enviar comandos.

Los gemelos digitales facilitan la simulación, validación y capacitación antes de operar el equipo físico.

**Componentes principales:**

- Modelos robóticos articulados.
- Sincronización de posiciones.
- Comunicación bidireccional.
- Registro de trayectorias.
- Visualización del estado del robot.
- Simulación previa a la ejecución real.

---

## Investigación en interacción humano-robot

Investigación orientada a utilizar realidad mixta e inteligencia artificial para apoyar a usuarios no expertos durante la operación y aprendizaje de robots colaborativos.

El objetivo es desarrollar sistemas más intuitivos, seguros y adaptables a las características de cada usuario.
