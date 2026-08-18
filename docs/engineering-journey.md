# Engineering Journey

This document expands the condensed background from the profile README and preserves
the technical context behind that progression.

Repositories are not listed here. The canonical index of public repositories is
[Historical Projects](historical-projects.md).

## 2005–2008 · Early Embedded Systems

My early work covered several different embedded domains:

- Quadcopter design, implementation, and flight-control work on an EM78569-based platform
- Mitsubishi PLC work for chemical-process control
- Sunplus-based interactive storybook systems
- Sunplus video / display processing experiments

One of the early quadcopter projects received **1st Place** in the 9th ELAN
Microcontroller Application and Artificial Intelligence Design Competition,
Microcontroller Application Project / Innovation Division. See
[2006 Quadcopter Project](early-quadcopter-2006.md) for project and provenance details.

These systems established a foundation in embedded implementation, control, timing, and
real-world I/O — and showed early on that system behavior rarely belongs to software or
hardware alone.

## 2008–2021 · Mobile Platforms, Flight Control, Robotics, and Automation

During this period my work expanded from device-level software and firmware into larger
embedded platforms, control systems, robotics, heterogeneous computing, and complete
physical-system integration.

As the systems grew, the engineering problem shifted from implementing individual
components toward understanding interfaces, integration behavior, and the assumptions
between subsystems.

### Mobile and Embedded Platforms

A major part of this period was Qualcomm-based mobile platforms: BSP and firmware
development, and embedded software integration across Windows Mobile, Android, and
related low-level stacks.

This built experience in large embedded software stacks, platform integration,
device-level debugging, communication interfaces, and the interaction between low-level
software and application-level system behavior.

### Flight Control, Motor Control, and Autonomous Systems

In parallel I worked on flight-control and autonomous-system technology using
STM32-class MCUs and related embedded platforms:

- STM32 flight controllers
- NuttX and PX4-derived systems
- BLDC electronic speed controllers
- Gimbal control
- Optical-flow sensing
- Integrated flight-controller and multi-ESC platforms
- IMU, barometer, magnetometer, and navigation-sensor integration

Source and board-porting work from this period is preserved in the
[flight control and autonomous systems](historical-projects.md#flight-control--autonomous-systems)
section of the archive.

### Robotics and Heterogeneous Systems

The work also expanded beyond MCU-only systems into heterogeneous architectures
combining embedded controllers with application processors:

- STM32 + Nvidia Tegra K1 heterogeneous flight-control architectures
- Drone computer-vision collaboration, focusing on embedded control and system integration
- SLAM-oriented autonomous ground-vehicle collaboration, focusing on vehicle control and motion integration
- Mixed-reality drone concepts
- TI-based embedded application-processor platforms
- Mecanum-wheel AGV motion control
- Four- and six-axis robot-arm integration, including UR3
- Instrument automation and multi-device equipment control

Related repositories are indexed under
[robotics and automation](historical-projects.md#robotics--automation).

### Embedded RTOS, Sensors, and Audio Experiments

Several older repositories preserve experiments in RTOS porting, sensor integration,
audio processing, and low-level embedded software — GPCE063 and GPCE2064 FreeRTOS work,
digital filter design translated to C, and an STM32 firmware build port. See
[RTOS and sensor experiments](historical-projects.md#embedded-rtos--sensor-experiments)
and [signal processing and firmware porting](historical-projects.md#signal-processing--firmware-porting).

## 2021–Present · System Integration, Architecture, and Technical Leadership

My work expanded from hands-on implementation, bring-up, and system debugging into
architecture, cross-domain integration, validation, technical decision-making, project
planning, and engineering execution across multiple projects and teams.

As the scope widened, the difficult questions moved toward architecture, technical
decisions, validation strategy, evidence, and how engineering work should be structured
and communicated.

The underlying approach did not change: understand the system at implementation level
when necessary, then connect those details back to architecture, interfaces, validation,
measurable evidence, and technical decisions.

### Recent Hands-On Work

More recent work has returned to low-level system architecture from a different
direction:

- Embedded Linux and Buildroot
- PREEMPT_RT and real-time Linux experiments
- USB gadget interfaces
- RP2350 and dual-core MCU architecture
- Physical processor interfacing and deterministic bus service
- Control-system implementation and verification

## Current Research

[Spec2Exec](https://github.com/cctsao1008/spec2exec) explores whether accepted
semantics, deterministic verification, executable generation, evidence, and provenance
can be connected into a more trustworthy software-development chain. In parallel, the
[Technical Management Framework](https://github.com/cctsao1008/technical-management-framework)
captures reusable practices for technical planning, governance, execution, validation,
evidence management, and AI-assisted collaboration across projects.

These directions are not separate from the earlier engineering work. They grew from
problems that recurred across embedded systems, control, integration, validation, and
technical execution: unclear assumptions, weak interfaces between specification and
implementation, incomplete evidence, and systems that appear correct locally but fail at
their boundaries.

[← Back to profile README](../README.md) · [Historical Projects →](historical-projects.md)
