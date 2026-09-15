# Cheng (Ricardo) 👋

**Hands-on Technical Leader · System Architecture · Embedded Systems · Control Systems**

I am especially interested in how complex systems are structured — how responsibilities, boundaries, interfaces, feedback, and evidence are arranged across engineering work, software, hardware, and physical systems.

My work spans hands-on implementation through system architecture, validation, and technical leadership. I move across layers when needed, from implementation details and real-world behavior back to the larger system and the assumptions that connect its parts.

> **The projects and technical work highlighted here are personal projects, historical work, or public open-source activities, and are independent of my current employer.**

## 🚀 Active Projects

These projects explore system architecture at different layers — from technical execution, software trust, semantic systems, and probabilistic modeling to computer architecture, machine control, sensing, motor drives, and physical power conversion.

### 🧭 [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework) · 2026

Explores how engineering work can be structured so that planning, decisions, risks, validation, and evidence remain connected throughout a project.

The framework is deliberately project-agnostic: it defines reusable principles, processes, and templates while project-specific architecture, requirements, evidence, decision records, and validation status remain in each project repository.

### 🧩 [Spec2Exec](https://github.com/cctsao1008/spec2exec) · 2026

Explores how authorized human intent can reach executable behavior without silent semantic invention or loss of traceability along the way.

The current prototype combines semantic-obligation discovery, authority gating, deterministic verification, artifact-bound evidence, and target realization. It demonstrates an authority-gated native RV32I path under QEMU with explicit per-boundary evidence, alongside bounded lifecycle Trust Graph validation; comparative assurance is the next research phase.

### 🧠 [LSMM](https://github.com/cctsao1008/lsmm.c) · 2026

Explores machine-native meaning and whether semantic organization can become a persistent, revisable, directly computable domain rather than remaining only a by-product of sequential token processing.

The research focuses on first-meaning formation, semantic judgment, consequential distinction, provenance, continuity, and legitimate semantic-regime development under an explicit constitutional kernel. The repository is currently private research.

### 🪧 [Conversation Blackboard](https://github.com/cctsao1008/conversation-blackboard) · 2026

Builds a persistent shared blackboard for independent AI conversations, agents, tools, and humans that need durable shared context without collapsing their identities, memories, or authority boundaries.

The architecture separates authentication, principal resolution, logical participant identity, authorization, semantic operations, and authoritative durable state. Multiple transports — including Web, programmatic APIs, MCP, and GitHub-authenticated paths — converge on the same runtime and authorization semantics.

### 📬 [Conversation Blackboard Gateway](https://github.com/cctsao1008/conversation-blackboard-gateway) · 2026

Provides a lightweight GitHub-facing mailbox for runtimes that can create GitHub Issues but cannot call Conversation Blackboard directly.

GitHub authenticates the submitting account while Blackboard remains responsible for participant ownership, authorization, provenance resolution, and durable persistence. The gateway deliberately acts as an adapter rather than a second identity or authority system.

### ☕ [Coffee Routine Model](https://github.com/cctsao1008/coffee-routine-model) · 2026

Explores how a recurring shared routine can be modeled probabilistically when observations are incomplete, interruptions happen, context accumulates, and uncertainty should remain visible.

The Coupled Shared Routine Dynamics Model (CSRDM) uses a stochastic hidden-state model and particle-filter inference while keeping a strict interpretation boundary: observable events are evidence about the routine, not direct measurements of private intention or human truth.

### 🎮 [Fami Pixel](https://github.com/cctsao1008/fami-pixel) · 2026

Builds a machine-learning and planning playground for Famicom / NES games, with Super Mario Bros. on Mesen CE as the first workload.

The emulator remains authoritative for machine state while Python and native adapters provide observation, deterministic frame stepping, controller input, forward-model rollouts, and planning experiments. The architecture supports vision-only, state-only, and hybrid observation paths without modifying the game ROM.

### 🕰️ [pi86-rp2350](https://github.com/cctsao1008/pi86-rp2350) · 2026

Builds a Host-Managed Bare-Metal Physical Processor Runtime for real Intel 8086 and NEC V30 processors.

A modern Host loads and supervises native workloads, while the RP2350 owns clock, reset, memory, I/O, interrupts, storage, and the physical processor bus. The runtime has physically demonstrated automatic processor identification, native workload execution at 1 MHz, shared memory, persistent FAT storage, interactive control, and CRC-protected `.P86W` workload packages.

The physical processor executes the instructions. The RP2350 does not emulate it.

### 🌀 [Rotary Inverted Pendulum](https://github.com/cctsao1008/rotary-inverted-pendulum) · 2026

Re-engineers an existing working rotary inverted pendulum into a measurable, testable, safety-gated, and progressively commissionable embedded control platform.

The architecture separates state estimation, control computation, and physical actuator authority, while keeping control logic platform-independent where practical for host-side testing before real motor output is enabled.

### 🛞 [Single-Wheel Platform](https://github.com/cctsao1008/single-wheel-platform) · 2026

Builds a Rust `no_std` control and system-identification platform for a reaction-wheel-stabilized single-wheel robot.

The architecture deliberately separates physical evidence, estimated state, control intent, bounded actuator commands, runtime authorization, and electrical realization so that no layer gains more meaning or authority than the available evidence supports.

### 👀 [Bividi](https://github.com/cctsao1008/bividi) · 2026

Builds a stereo-inertial sensor-acquisition system that turns device-specific camera and IMU data into clean, synchronized observation streams.

The platform-independent core separates operating-system backends, device-family adapters, runtime capability discovery, timing and synchronization semantics, and normalized observations. The production camera path is native C++17/CMake, with OpenCV as an optional processing and engineering-view layer.

### ⚙️ [BLDC / PMSM Motor Control](https://github.com/cctsao1008/bldc-pmsm-motor-control) · 2026

Uses a vendor-validated three-phase inverter as a stable physical platform for developing and comparing BLDC and PMSM control strategies.

The architecture separates power hardware, sensing, timing, motor state, and control so sensorless six-step commutation and field-oriented control (FOC) can be developed against the same known-good hardware baseline.

### ⚡ [Bidirectional Buck-Boost Control](https://github.com/cctsao1008/bidirectional-buckboost-control) · 2026

Uses a known-good four-switch bidirectional buck-boost converter as a physical plant for digital-control research.

The architecture separates measurement, plant modeling, sensing, control law, modulation, and hardware-specific PWM so different control methods can be compared under the same experimental protocol. Current work focuses on reference-system and physical-plant characterization.

## 🛠️ Background

- **2005–2008** — Early embedded systems and control. An EM78569-based quadcopter project received **1st Place** in the 9th ELAN Microcontroller Application and Artificial Intelligence Design Competition ([project and provenance](docs/early-quadcopter-2006.md)).
- **2008–2021** — Qualcomm mobile platforms and BSP work, STM32 flight control, BLDC motor control, Mecanum AGV motion control, robotics and automation, RTOS work, and heterogeneous embedded systems.
- **2021–Present** — System integration, architecture, validation, technical decision-making, and technical leadership across multiple projects and teams, with recent hands-on work in real-time Linux, RP2350, low-level architecture, and control-system implementation.
- **Current research** — Machine-native meaning, trustworthy software construction, evidence-oriented engineering, and specification-to-executable development.

[Full engineering journey →](docs/engineering-journey.md)

## 📦 Archive

Older public repositories covering flight control, robotics, RTOS experiments, signal processing, firmware ports, and automation are indexed in **[Historical Projects](docs/historical-projects.md)**, with original work, ports, derived work, and experiments labeled separately.

A representative historical project is [TMR-FC — Top Multi-Rotor Flight Controller](https://github.com/cctsao1008/tmr-flight-controller) (**2013**), an open hardware and software multirotor flight-controller platform built around STM32F405/STM32F407 with PX4-derived firmware.

## ✨ Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
