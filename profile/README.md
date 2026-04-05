# B-ROVERETTE

**B-ROVERETTE** is a modular ROS 2 Ackermann robotics platform for education, research, and autonomous systems development.

It is designed around a simple idea: build a solid core vehicle platform first, then layer higher-level autonomy, mapping, exploration, and learning systems on top of it without rewriting the foundation each time.

https://github.com/user-attachments/assets/8b9d1c06-a58a-40a6-a1f9-abc77dda6b2d

---

## What It Is

B-ROVERETTE is not just a single robot repo.

It is a growing robotics platform built around:

- a **core vehicle layer** for sensing, state, and motion interfaces
- a **navigation layer** for SLAM, localization, and Nav2
- an **exploration layer** for autonomous frontier-based exploration
- a **learning layer** for neural driving and data-driven experimentation

The goal is to make robotics work more reusable, modular, and realistic for both research and hands-on development.

---

## Why It Exists

A lot of small robotics projects stop at a demo.

B-ROVERETTE was built to be more useful than that.

It provides a practical base for:

- autonomous navigation
- SLAM and mapping
- perception and vision experiments
- controller-based teleoperation
- neural driving workflows
- modular system extensions

That makes it useful as both:

- a serious educational platform
- a repeatable research and experimentation platform

---

## Architecture

The platform is organized as a modular stack:

```text
Core Platform
  ├── Robot description
  ├── Sensor interfaces
  ├── cmd_vel / odom / scan / camera topics
  └── Basic runtime and hardware integration

Navigation Layer
  ├── SLAM Toolbox
  ├── AMCL
  ├── Nav2
  └── Teleoperation workflows

Exploration Layer
  ├── Frontier-based exploration
  ├── Autonomous map building
  └── End-to-end exploration bringup

Learning Layer
  ├── Data collection
  ├── Neural driving workflows
  ├── Multi-input model support
  └── DNN experimentation on top of the platform
```

This structure makes it easy to build on the same robot foundation while keeping subsystems cleanly separated.

---

## Repositories

### [`broverette-core`](https://github.com/broverette/broverette-core)
The base B-ROVERETTE robot platform.

Includes the foundational ROS 2 interfaces and hardware-facing functionality for the vehicle, including robot description, sensing, odometry, and motion-related topics.

### [`broverette-nav2`](https://github.com/broverette/broverette-nav2)
The autonomy and navigation stack.

Builds on the core platform to support:

- teleoperation
- SLAM
- map creation
- AMCL localization
- Nav2 path planning and navigation

### [`broverette-explorer`](https://github.com/broverette/broverette-explorer)
The autonomous exploration stack.

Combines the platform with exploration tooling to automatically build maps and explore unknown spaces with minimal configuration.

### [`broverette-oscar`](https://github.com/broverette/broverette-oscar)
The neural driving and learning extension.

Extends B-ROVERETTE with DNN-based workflows, data collection, multi-input model support, and controller-driven training/inference pipelines.

---

## Design Principles

- **Modular first**: higher-level capabilities build on top of a stable core
- **ROS 2 native**: designed around practical ROS 2 workflows
- **Research-friendly**: suitable for experimentation, evaluation, and publication-backed work
- **Hands-on**: grounded in real robot integration, not just simulation
- **Extendable**: easy to grow into new autonomy, perception, and learning modules

---

## Example Use Cases

- build and test a small autonomous Ackermann platform
- create maps with SLAM and run Nav2 navigation
- experiment with frontier-based autonomous exploration
- collect driving data with different controllers
- train and run neural driving models
- prototype perception and autonomy pipelines on a reusable robot base

---

## Publications

Selected work built around the platform includes:

- **B-ROVERETTE: Be RObotic Vehicle for Education and Research - Yet Another Scaled Robotics Vehicular Platform**
  - ICRA Workshop 2025

- **DriveNetBench: An Affordable and Configurable Single-Camera Benchmarking System for Autonomous Driving Networks**
  - IEEE EIT 2025

---

## Project Vision

B-ROVERETTE is meant to sit at the intersection of:

- robotics
- autonomy
- machine learning
- embedded systems
- practical platform engineering

The long-term goal is to make it easier to move from isolated robotics demos to a more complete, reusable robotics system that supports navigation, experimentation, benchmarking, and learning on the same platform.

---

## Get Involved

If you are interested in:

- ROS 2 robotics
- autonomous navigation
- SLAM and exploration
- neural driving
- modular robotics platforms

this project is intended to be a foundation you can build on.

---

## Name

The project is presented publicly as **B-ROVERETTE**.

For GitHub organization and repo naming, the simpler lowercase form `broverette` is typically used for handles and URLs.
