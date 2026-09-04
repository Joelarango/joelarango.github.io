---
layout: default
title: Meta Quest 3 con robots UR
parent: Proyectos de robótica y XR
nav_order: 2
description: Operación y visualización de robots Universal Robots mediante Meta Quest 3.
permalink: /proyectos/quest-universal-robots/
---

# Operación de robots Universal Robots con Meta Quest 3

Entorno inmersivo para visualizar, controlar y analizar robots colaborativos UR3 y UR5 mediante Meta Quest 3.

![Operación y visualización de robots Universal Robots mediante Meta Quest 3](/assets/images/ur3_gv.png)

*Gemelo digital UR3.*


## Descripción

Este proyecto integra realidad mixta, gemelos digitales y comunicación en tiempo real para conectar una aplicación desarrollada en Unity con robots Universal Robots y entornos de simulación.

El usuario puede interactuar con el sistema mediante los controladores o el seguimiento de manos de Meta Quest 3.

## Objetivos

- Representar virtualmente robots UR3 y UR5.
- Sincronizar el movimiento del robot virtual y el robot real.
- Enviar y recibir información en tiempo real.
- Explorar métodos intuitivos de teleoperación.
- Validar movimientos en simulación antes de ejecutarlos.
- Desarrollar herramientas de capacitación para usuarios no expertos.

## Arquitectura

El sistema conecta los siguientes componentes:

1. **Meta Quest 3:** interfaz inmersiva para el usuario.
2. **Unity:** visualización, interacción y gemelo digital.
3. **Python:** coordinación y procesamiento de mensajes.
4. **RoboDK:** simulación y validación de movimientos.
5. **Universal Robots:** ejecución en el robot colaborativo.

<div style="text-align: center;">
  <img
    src="/assets/images/teleoperacion.png"
    alt="Operación y visualización de robots Universal Robots mediante Meta Quest 3"
    style="width: 100%; max-width: 650px; height: auto;">

  <p><em>Teleoperación del Yaskawa HC10 mediante Microsoft HoloLens 2.</em></p>
</div>




Flujo general:

```text
Meta Quest 3
  ↔ Unity
  ↔ MQTT o UDP
  ↔ Python
  ↔ RoboDK
  ↔ Robot UR3 o UR5
