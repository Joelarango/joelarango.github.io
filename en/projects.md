---
layout: default
title: Robotics and XR projects
nav_order: 3
has_children: true
description: Robotics, extended reality, and digital twin projects.
permalink: /en/projects/
---

# Robotics and extended reality projects

This section presents projects in collaborative robotics, mixed reality, teleoperation, digital twins, and human–robot interaction. Each project documents its objective, technologies, architecture, development, and results.

---

## Yaskawa HC10 teleoperation with HoloLens 2

A mixed reality system for controlling and programming trajectories for a Yaskawa MOTOMAN HC10 collaborative robot.

The application lets a user manipulate a virtual target, calculate motion through inverse kinematics, record trajectory points, and transmit them using MQTT.

**Main technologies:**

- Microsoft HoloLens 2.
- Unity and C#.
- OpenXR and MRTK.
- Yaskawa MOTOMAN HC10.
- MQTT, Python, and RoboDK.

[View project and collaboration with Linnaeus University](yaskawa-hololens/){: .btn }

---

## Universal Robots operation with Meta Quest 3

An immersive environment for visualizing, controlling, and analyzing UR3 and UR5 robots using Meta Quest 3. The system connects the virtual environment to simulators and robots through real-time network communication.

**Main technologies:**

- Meta Quest 3.
- Unity and Meta XR SDK.
- Universal Robots UR3 and UR5.
- URScript.
- MQTT, UDP, Python, and RoboDK.

[View Universal Robots project](quest-universal-robots/){: .btn }

---

## International projects

### UR3 — Pontificia Universidad Javeriana, Colombia

Implementation and demonstration of a mixed reality platform to teleoperate a UR3 collaborative robot and make its operation more accessible to students and non-expert users.

[View project in Colombia](ur3-javeriana/){: .btn }

### UR5 — Białystok University of Technology, Poland

Teleoperation of a UR5 robot through Meta Quest 3, Unity, and a connected digital twin from an immersive interface.

[View project in Poland](ur5-bialystok/){: .btn }

---

## Connected digital twins

Development of virtual representations of industrial robots capable of receiving joint states, reproducing motions, and sending commands. Digital twins support simulation, validation, and training before operating physical equipment.

**Main components:**

- Articulated robotic models.
- Position synchronization.
- Bidirectional communication.
- Trajectory recording.
- Robot-state visualization.
- Simulation before physical execution.

## Human–robot interaction research

Research using mixed reality and artificial intelligence to support non-expert users while they operate and learn to use collaborative robots. The objective is to develop systems that are more intuitive, safe, and adaptable to each user.
