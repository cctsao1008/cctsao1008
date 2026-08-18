# Cheng (Ricardo) Tsao

**Hands-on Technical Leader · Embedded Systems · System Architecture · Control Systems**

I work on systems where correctness depends on how software, embedded computing, control, timing, integration, and real-world behavior interact.

My work spans hands-on implementation through system architecture, validation, and technical leadership. Over time, the recurring engineering problem has shifted from making individual components work to understanding the boundaries between requirements, implementation, hardware, verification, measurement, and technical decisions.

> **The projects and technical work highlighted here are personal projects, historical work, or public open-source activities, and are independent of my current employer.**

## Active Projects

The following projects are active research and development efforts started in 2026.

### [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework)

A reusable, project-agnostic framework for technical planning, engineering governance, execution, validation, evidence management, knowledge capture, and AI-assisted collaboration. It separates reusable engineering practice from project-local technical truth, with explicit treatment of baselines, decision records, risks and assumptions, evidence chains, validation, retrospectives, and cross-project learning.

### [Spec2Exec](https://github.com/cctsao1008/spec2exec)

Research prototype exploring how accepted semantics, deterministic verification, artifact-bound evidence, provenance, and executable generation can be connected into a trustworthy specification-to-executable chain.

The current prototype demonstrates a native RV32I path under QEMU with explicit per-boundary evidence. Semantic-authority gating and physical RP2350 / Hazard3 validation remain active research directions.

### [Pi86-RP2350](https://github.com/cctsao1008/pi86-rp2350)

Porting the Pi86 concept to a Waveshare RP2350-PiZero while preserving the original Pi86 V20/V30 HAT and using a physical NEC V30 processor. The architecture explores deterministic RP2350 firmware for V30 clocking and bus service using PIO/SIO, with hardware bring-up and further system integration in progress.

### [Rotary Inverted Pendulum](https://github.com/cctsao1008/inverted-pendulum)

From-scratch embedded firmware and control software for a rotary inverted pendulum, covering STM32F103 bring-up, sensing, encoder acquisition, motor characterization, state estimation, state-feedback control, fail-closed safety boundaries, telemetry, and host-side verification.

### [BLDC / PMSM Motor Control](https://github.com/cctsao1008/bldc-pmsm-motor-control)

Physical motor-control platform for developing and comparing sensorless six-step commutation and field-oriented control (FOC), with emphasis on sensing, timing, estimation, current control, and measurement-driven validation. Current work focuses on hardware characterization, sensing validation, and establishing a known-good baseline before independent control development.

### [Bidirectional Buck-Boost Control](https://github.com/cctsao1008/bidirectional-buckboost-control)

Digital power-control research platform based on a four-switch bidirectional buck-boost converter, using measured hardware to study plant modeling, classical and state-space control, estimation, and reproducible controller comparison. Current work focuses on reference-system and physical-plant characterization.

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
