---
layout: default
title: Meta Quest 3 with UR robots
parent: Robotics and XR projects
nav_order: 2
description: Operation and visualization of Universal Robots through Meta Quest 3.
permalink: /en/projects/quest-universal-robots/
---

# Universal Robots operation with Meta Quest 3

An immersive environment for visualizing, controlling, and analyzing UR3 and UR5 collaborative robots through Meta Quest 3.

![Universal Robots operation and visualization through Meta Quest 3](/assets/images/ur3_gv.png)

*UR3 digital twin.*

## Description

This project combines mixed reality, digital twins, and real-time communication to connect an application developed in Unity with Universal Robots and simulation environments.

Users interact with the system using Meta Quest 3 controllers or hand tracking.

## Objectives

- Virtually represent UR3 and UR5 robots.
- Synchronize virtual and physical robot motion.
- Send and receive information in real time.
- Explore intuitive teleoperation methods.
- Validate motions in simulation before execution.
- Develop training tools for non-expert users.

## Architecture

1. **Meta Quest 3:** immersive user interface.
2. **Unity:** visualization, interaction, and digital twin.
3. **Python:** message coordination and processing.
4. **RoboDK:** motion simulation and validation.
5. **Universal Robots:** collaborative robot execution.

<div style="text-align: center;">
  <img src="/assets/images/teleoperacion.png" alt="Universal Robots teleoperation architecture with Meta Quest 3" style="width: 100%; max-width: 650px; height: auto;">
  <p><em>Universal Robots teleoperation architecture using Meta Quest 3.</em></p>
</div>

General flow:

    Meta Quest 3
      ↔ Unity
      ↔ MQTT or UDP
      ↔ Python
      ↔ RoboDK
      ↔ UR3 or UR5 robot

## International implementations

- **Pontificia Universidad Javeriana, Colombia:** UR3 operation.
- **Białystok University of Technology, Poland:** UR5 operation with Meta Quest 3.

## Results

- Synchronization of the digital twin and robot.
- Bidirectional communication among Unity, Python, RoboDK, and Universal Robots.
- Controller and hand-tracking interaction.
- Motion validation in a virtual environment.
- Teleoperation demonstration across international institutions.
