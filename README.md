# Cheng (Ricardo)

**Hands-on Technical Leader · System Architecture · Embedded Systems · Control Systems**

I am especially interested in how complex systems are structured — how responsibilities, boundaries, interfaces, feedback, and evidence are arranged across engineering work, software, hardware, and physical systems.

My work spans hands-on implementation through system architecture, validation, and technical leadership. I move across layers when needed, from implementation details and real-world behavior back to the larger system and the assumptions that connect its parts.

> **The projects and technical work highlighted here are personal projects, historical work, or public open-source activities, and are independent of my current employer.**

## Active Projects

These projects explore system architecture at different layers — from technical execution and software trust to computer architecture, control systems, motor drives, and physical power conversion.

### [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework) · 2026

Explores how engineering work can be structured so that planning, decisions, risks, validation, and evidence remain connected throughout a project.

The framework is deliberately project-agnostic: it defines reusable principles, processes, and templates while project-specific architecture, requirements, evidence, decision records, and validation status remain in each project repository.

### [Spec2Exec](https://github.com/cctsao1008/spec2exec) · 2026

Explores how authorized human intent can reach executable behavior without silent semantic invention or loss of traceability along the way.

The current prototype combines semantic-obligation discovery, authority gating, deterministic verification, artifact-bound evidence, and target realization. It demonstrates an authority-gated native RV32I path under QEMU with explicit per-boundary evidence, alongside bounded lifecycle Trust Graph validation; comparative assurance is the next research phase.

### [Pi86-RP2350](https://github.com/cctsao1008/pi86-rp2350) · 2026

Explores how a modern RP2350 can act as a programmable chipset around a real NEC V30 while preserving the processor's original bus behavior.

The architecture keeps the hardest real-time bus path in PIO/DMA and moves higher-level supervision and services onto the Arm cores. The physical V30 has already executed a native BIOS diagnostic that prints `HELLO RP2350` at 0.300 MHz.

### [Rotary Inverted Pendulum](https://github.com/cctsao1008/inverted-pendulum) · 2026

Re-engineers an existing working rotary inverted pendulum into a measurable, testable, safety-gated, and progressively commissionable embedded control platform.

The architecture separates state estimation, control computation, and physical actuator authority, while keeping control logic platform-independent where practical for host-side testing before real motor output is enabled.

### [BLDC / PMSM Motor Control](https://github.com/cctsao1008/bldc-pmsm-motor-control) · 2026

Uses a vendor-validated three-phase inverter as a stable physical platform for developing and comparing BLDC and PMSM control strategies.

The architecture separates power hardware, sensing, timing, motor state, and control so sensorless six-step commutation and field-oriented control (FOC) can be developed against the same known-good hardware baseline.

### [Bidirectional Buck-Boost Control](https://github.com/cctsao1008/bidirectional-buckboost-control) · 2026

Uses a known-good four-switch bidirectional buck-boost converter as a physical plant for digital-control research.

The architecture separates measurement, plant modeling, sensing, control law, modulation, and hardware-specific PWM so different control methods can be compared under the same experimental protocol. Current work focuses on reference-system and physical-plant characterization.

## Background

- **2005–2008** — Early embedded systems and control. An EM78569-based quadcopter project received **1st Place** in the 9th ELAN Microcontroller Application and Artificial Intelligence Design Competition ([project and provenance](docs/early-quadcopter-2006.md)).
- **2008–2021** — Qualcomm mobile platforms and BSP work, STM32 flight control, BLDC motor control, Mecanum AGV motion control, robotics and automation, RTOS work, and heterogeneous embedded systems.
- **2021–Present** — System integration, architecture, validation, technical decision-making, and technical leadership across multiple projects and teams, with recent hands-on work in real-time Linux, RP2350, low-level architecture, and control-system implementation.
- **Current research** — Trustworthy software construction, evidence-oriented engineering, and specification-to-executable development.

[Full engineering journey →](docs/engineering-journey.md)

## Archive

Older public repositories covering flight control, robotics, RTOS experiments, signal processing, firmware ports, and automation are indexed in **[Historical Projects](docs/historical-projects.md)**, with original work, ports, derived work, and experiments labeled separately.

A representative historical project is [TMR-FC — Top Multi-Rotor Flight Controller](https://github.com/cctsao1008/tmr-flight-controller) (**2013**), an open hardware and software multirotor flight-controller platform built around STM32F405/STM32F407 with PX4-derived firmware.

## Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
