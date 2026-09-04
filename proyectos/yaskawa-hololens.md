---
layout: default
title: Yaskawa HC10 con HoloLens 2
parent: Proyectos de robótica y XR
nav_order: 1
description: Teleoperación y programación de trayectorias para un robot Yaskawa HC10 mediante realidad mixta.
permalink: /proyectos/yaskawa-hololens/
---

# Teleoperación de Yaskawa HC10 con HoloLens 2

Sistema de realidad mixta para visualizar, controlar y programar trayectorias de un robot colaborativo Yaskawa MOTOMAN HC10.

## Descripción

El proyecto permite que un usuario manipule un objetivo virtual desde Microsoft HoloLens 2. Un gemelo digital del robot calcula y reproduce el movimiento necesario para seguir ese objetivo.

La aplicación registra puntos de trayectoria y los envía a una computadora mediante MQTT para su validación, simulación y posterior ejecución en el robot.

## Objetivos

- Facilitar la programación del robot mediante interacción espacial.
- Permitir que usuarios no expertos definan trayectorias.
- Visualizar el movimiento antes de ejecutarlo en el robot físico.
- Detectar posiciones fuera del espacio de trabajo.
- Registrar y reproducir trayectorias.
- Comunicar HoloLens 2 con una computadora mediante MQTT.

## Arquitectura del sistema

El sistema está compuesto por cuatro elementos principales:

1. **HoloLens 2:** permite manipular el objetivo virtual y visualizar el gemelo digital.
2. **Unity:** ejecuta la interfaz, la cinemática inversa y el registro de trayectorias.
3. **Bridge MQTT en Python:** recibe, valida y almacena las trayectorias.
4. **RoboDK o robot físico:** simula o ejecuta el movimiento.

El flujo de información es:

```text
Usuario
  → HoloLens 2
  → Unity y gemelo digital
  → MQTT
  → Aplicación Python
  → RoboDK o Yaskawa HC10
