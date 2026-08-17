# Cheng

**Technical Leader · Hands-on Embedded Systems Engineer · System Architecture · Control Systems**

I work on engineering problems that span software, embedded systems, system architecture, control, integration, timing, and real-world behavior.

My background includes embedded systems, real-time software, control systems, robotics, autonomous systems, system integration, and low-level computing.

Today, I remain hands-on while working increasingly at the architecture and technical-leadership level. I am especially interested in systems where correctness depends not only on individual components, but on how requirements, architecture, implementation, verification, measurement, and engineering decisions interact as a whole.

> **The projects and technical work highlighted here are personal projects, historical work, or public open-source activities, and are independent of my current employer.**

## Engineering Approach

I tend to look at engineering problems across layers — from requirements and architecture through implementation, integration, verification, and real-world behavior.

My approach is to understand the system deeply, make assumptions explicit, and connect technical decisions to measurable evidence.

## Current Focus

- System architecture and cross-domain integration
- Technical leadership and engineering execution
- Verification, validation, debugging, and evidence-based engineering
- Embedded and real-time systems
- Control systems and robotics
- Specification-to-executable engineering and trustworthy AI-assisted software development

## Selected Projects

These projects represent different parts of the same engineering path: system architecture, control, low-level implementation, verification, and technical execution.

### [Spec2Exec](https://github.com/cctsao1008/spec2exec)

**2026–Present · Active Research**  
**Specification-to-Executable Architecture**

Research prototype exploring how accepted semantics, deterministic verification, artifact-bound evidence, provenance, and executable generation can be connected into a trustworthy specification-to-executable chain.

The current prototype demonstrates a native RV32I path under QEMU with explicit per-boundary evidence. Semantic-authority gating and physical RP2350 / Hazard3 validation remain active research directions.

### [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework)

**2026–Present · Active Development**

A reusable, project-agnostic framework for technical planning, engineering governance, execution, validation, evidence management, knowledge capture, and AI-assisted collaboration.

The framework separates reusable management and execution practices from project-local technical truth, with explicit treatment of baselines and rebaselining, decision records, risk and assumption management, evidence chains, validation, retrospectives, and cross-project learning.

### [Rotary Inverted Pendulum](https://github.com/cctsao1008/inverted-pendulum)

**2026–Present · Active Development**

From-scratch embedded firmware and control software for a rotary inverted pendulum.

The project covers STM32F103 bring-up, sensing, encoder acquisition, motor characterization, state estimation, state-feedback control, fail-closed safety boundaries, telemetry, and host-side verification.

### [Pi86-RP2350](https://github.com/cctsao1008/pi86-rp2350)

**2026–Present · Active Development**

Porting the Pi86 concept to a Waveshare RP2350-PiZero while preserving the original Pi86 V20/V30 HAT and using a physical NEC V30 processor.

The architecture explores deterministic RP2350 firmware for V30 clocking and bus service using PIO/SIO, with planned PSRAM, MicroSD, DVI, and USB integration. The current phase is hardware bring-up.

### [TMR-FC — Top Multi-Rotor Flight Controller](https://github.com/cctsao1008/tmr-flight-controller)

**2013 · Historical Project**

Historical open hardware and software multirotor flight-controller platform built around STM32F405/STM32F407 and PX4-derived firmware.

The platform integrates inertial and environmental sensing, actuator interfaces, data logging, navigation interfaces, and Raspberry Pi companion-computer experiments for OpenCV, ROS, MAVLink, vision, and optical-flow applications.

## Engineering Journey

My engineering path has evolved from early embedded systems and control, through mobile platforms, flight control, robotics, heterogeneous systems, and system integration, toward architecture, technical leadership, verification, and evidence-based engineering.

- **2005–2008** — Early embedded systems and control, including an EM78569-based quadcopter project that received **1st Place** in the 9th ELAN Microcontroller Application and Artificial Intelligence Design Competition
- **2008–2021** — Mobile platforms, flight control, motor control, robotics, automation, RTOS work, and heterogeneous embedded systems
- **2021–Present** — System integration, architecture, validation, technical decision-making, and technical leadership across multiple projects and teams
- **Current** — Real-time Linux, low-level architecture, trustworthy software construction, evidence, and specification-to-executable research

[Read the detailed engineering journey →](docs/engineering-journey.md)  
[2006 quadcopter project and provenance →](docs/early-quadcopter-2006.md)  
[Historical projects index →](docs/historical-projects.md)

## Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
