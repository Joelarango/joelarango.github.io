---
layout: default
title: Yaskawa HC10 with HoloLens 2
parent: Robotics and XR projects
nav_order: 1
description: Mixed reality teleoperation and trajectory programming for a Yaskawa HC10 robot.
permalink: /en/projects/yaskawa-hololens/
---

# Yaskawa HC10 teleoperation with HoloLens 2

A mixed reality system for visualizing, controlling, and programming trajectories for a Yaskawa MOTOMAN HC10 collaborative robot.

Developed through collaboration between **Universidad Iberoamericana Mexico City** and **Linnaeus University, Sweden**.

## Description

A user manipulates a virtual target through Microsoft HoloLens 2. A digital twin of the robot calculates and reproduces the motion required to follow that target.

The application records trajectory points and sends them to a computer through MQTT for validation, simulation, and subsequent execution on the robot.

## Objectives

- Simplify robot programming through spatial interaction.
- Enable non-expert users to define trajectories.
- Visualize motion before physical execution.
- Detect positions outside the workspace.
- Record and replay trajectories.
- Connect HoloLens 2 to a computer through MQTT.

## System architecture

1. **HoloLens 2:** virtual target manipulation and digital-twin visualization.
2. **Unity:** interface, inverse kinematics, and trajectory recording.
3. **Python MQTT bridge:** trajectory reception, validation, and storage.
4. **RoboDK or physical robot:** motion simulation or execution.

Information flow:

    User
      → HoloLens 2
      → Unity and digital twin
      → MQTT
      → Python application
      → RoboDK or Yaskawa HC10

## Implemented features

- Spatial manipulation of the target with HoloLens 2.
- Target tracking through inverse kinematics.
- Visual indicators for reachability and proximity.
- Trajectory recording, playback, and transmission.
- Message validation and MQTT reception acknowledgement.
- RoboDK simulation before physical execution.

## International collaboration

The platform enabled motions intended for a Yaskawa HC10 in Sweden to be programmed from Mexico, previewed through a digital twin, and transferred for validation and execution.
