# Cheng

**Technical Leader · Hands-on Embedded Systems Engineer · System Architecture · Control Systems**

I work on engineering problems that cross the boundary between software, firmware, hardware, sensing, actuation, timing, and real-world system behavior.

My background spans embedded systems, MCU and application-processor platforms, RTOS and embedded Linux, flight control, motor control, robotics, autonomous systems, system integration, and low-level computer architecture.

Today, I remain hands-on while also working at the architecture and technical-leadership level. I am especially interested in systems where correctness depends not only on individual components, but on how specification, software, hardware, timing, verification, measurement, and engineering decisions interact as a whole.

> **The projects and technical work highlighted here are personal projects, historical work, or public open-source activities, and are independent of my current employer.**

## Current Focus

- Embedded systems and firmware architecture
- Embedded Linux and real-time Linux
- MCU-based system development
- Motor control and real-time control
- Control systems and robotics
- Hardware/software integration and bring-up
- System modeling, verification, debugging, and validation
- Low-level processor and bus interfacing
- Technical planning, engineering governance, validation, and evidence-based execution
- Specification-to-executable engineering
- Trust, evidence, and provenance for AI-assisted software engineering

## Selected Current Projects

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

### 2005–2008 · Early Embedded Systems

My early work covered several very different embedded domains:

- Quadcopter development and stability-control work on an EM78569 platform, including an award-winning student project
- Mitsubishi PLC work for chemical-process control
- Sunplus-based interactive storybook systems
- Sunplus video / display processing experiments

These projects established the foundation for working close to hardware, timing, peripherals, real-world I/O, and embedded-system constraints.

### 2008–2021 · Embedded Systems, Mobile Platforms, Robotics, and Automation

During this period, my work expanded from device-level software and firmware into larger embedded platforms, control systems, robotics, heterogeneous computing, and complete physical-system integration.

The work covered Qualcomm-based mobile platforms, STM32 flight-control systems, BLDC motor control, sensing, Mecanum-wheel AGV motion control, robotic-system integration, application-processor architectures, and instrument automation.

Across these projects, the recurring engineering problem was increasingly not just how to implement one component, but how multiple hardware and software subsystems should interact as a reliable system.

#### Mobile and Embedded Platforms

I spent a major part of this period working on Qualcomm-based mobile platforms, BSP and firmware development, and embedded software integration across Windows Mobile, Android, and related low-level software stacks.

This strengthened my experience in larger embedded software stacks, platform integration, device-level debugging, communication interfaces, and the interaction between low-level software and application-level system behavior.

#### Flight Control, Motor Control, and Autonomous Systems

In parallel, I worked extensively on flight-control and autonomous-system technology using STM32-class MCUs and related embedded platforms.

Representative areas include:

- STM32 flight controllers
- NuttX and PX4-derived systems
- BLDC electronic speed controllers
- Gimbal control
- Optical-flow sensing
- Integrated flight-controller and multi-ESC platforms
- IMU, barometer, magnetometer, and navigation-sensor integration

Some of the historical source and board-porting work from this period is preserved in:

- [TMR-FC](https://github.com/cctsao1008/tmr-flight-controller) — **2013** · PX4-derived flight-controller platform and board-porting work
- [TMR-FC NuttX](https://github.com/cctsao1008/tmrfc-nuttx) — **2013** · NuttX-based platform work associated with TMR-FC
- [Bootloader](https://github.com/cctsao1008/Bootloader) — **2013** · Modified PX4 bootloader for TMR-FC

#### Robotics and Heterogeneous Systems

The work also expanded beyond MCU-only systems into heterogeneous architectures combining embedded controllers with application processors.

Projects and system-integration work included:

- STM32 + Nvidia Tegra K1 heterogeneous flight-control architectures
- Drone computer-vision collaboration, with primary responsibility for embedded control and system integration
- SLAM-oriented autonomous ground-vehicle collaboration, with primary responsibility for vehicle control and motion integration
- Mixed-reality drone concepts
- TI-based embedded application-processor platforms
- Mecanum-wheel AGV motion control
- Four- and six-axis robot-arm integration, including UR3
- Instrument automation and multi-device equipment control

Related repositories include:

- [NTUT Rover](https://github.com/cctsao1008/ntut_rover) — **2014** · Raspberry Pi-based autonomous rover following recorded GPS waypoints
- [Mecanum AGV Motion Control](https://github.com/cctsao1008/mecanum-agv-motion-control) — **2016** · vehicle-frame motion control, Mecanum-wheel kinematics, feedback control, and embedded execution for an AGV mobile base
- [Instrument Automation Control](https://github.com/cctsao1008/instrument-automation-control) — **2017** · modular instrument automation and equipment orchestration across device control, communication, scripting, scheduling, and data services

#### Historical Platform Context

Platforms and environments used during this period included Qualcomm MSM-series application processors, STM32 F1/F3/F4, Raspberry Pi, Generalplus GPCE, NXP and Nuvoton MCUs, Nvidia Tegra K1, and RTOS environments such as FreeRTOS, NuttX, uC/OS, RTX, and RT-Thread.

These platforms reflect the breadth of the engineering work from device-level firmware and RTOS-based systems to application processors, robotics, and heterogeneous embedded architectures.

### Embedded RTOS, Sensors, and Audio Experiments

Several older repositories preserve experiments in RTOS porting, sensor integration, audio processing, and low-level embedded software:

- [GPCE063 FreeRTOS Storybook](https://github.com/cctsao1008/gpce063-freertos-storybook) — **2011** · GPCE063, FreeRTOS, audio decoding, sensors, and file-system integration
- [GPCE063 FreeRTOS Motion Audio Demo](https://github.com/cctsao1008/gpce063-freertos-motion-audio-demo) — **2013** · FreeRTOS, BMA180, software I2C, A1600 audio, and Petit FAT
- [GPCE2064 FreeRTOS Funny Car](https://github.com/cctsao1008/gpce2064-freertos-funny-car) — **2014** · GPCE2064, FreeRTOS V8.0.0-era, audio, key scanning, LED control, sleep mode, and Petit FAT
- [C Digital Filter Lab](https://github.com/cctsao1008/c-digital-filter-lab) — **2016** · Octave/MATLAB filter design and validation, with resulting IIR/FIR coefficients translated into explicit C implementations
- [TS100 GCC](https://github.com/cctsao1008/ts100-gcc) — **2017** · historical GCC/Make-based STM32 firmware port/build work for the TS100 soldering iron

### 2021–Present · System Integration, Architecture, and Technical Leadership

My work has increasingly expanded from hands-on implementation, bring-up, and system debugging into architecture, cross-domain integration, validation, technical decision-making, project planning, and engineering execution across multiple projects and teams.

The underlying approach remains the same: understand the system at implementation level when necessary, then connect those details back to architecture, interfaces, validation, measurable evidence, and technical decisions.

### Recent Work · Real-Time Linux, RP2350, and Low-Level Architecture

More recent hands-on work has returned to low-level system architecture from a different direction:

- Embedded Linux and Buildroot
- PREEMPT_RT and real-time Linux experiments
- USB gadget interfaces
- RP2350 and dual-core MCU architecture
- Physical processor interfacing and deterministic bus service
- Control-system implementation and verification

### Current Research · Trustworthy Software Construction and Technical Execution

My current research direction is [Spec2Exec](https://github.com/cctsao1008/spec2exec), which explores whether accepted semantics, deterministic verification, executable generation, evidence, and provenance can be connected into a more trustworthy software-development chain.

In parallel, the [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework) captures reusable practices for technical planning, engineering governance, execution, validation, evidence management, and AI-assisted collaboration across projects.

Both directions grow from the same recurring engineering problem: a system can appear correct at the requirement, software, hardware, management, or test level individually and still fail at the boundaries between them.

## Real-Time Linux Experiments

Ongoing exploration of Linux-based embedded and real-time systems includes:

- PREEMPT_RT
- Embedded Linux
- Buildroot
- Kernel configuration and bring-up
- USB gadget interfaces
- Real-time measurement and control experiments

## Engineering Perspective

```text
Intent / Requirement
        ↓
Specification
        ↓
Architecture
        ↓
Planning / Governance
        ↓
Modeling
        ↓
Implementation
        ↓
Verification
        ↓
Hardware
        ↓
Measurement
        ↓
Evidence / Feedback
```

I am most interested in the gaps between these layers: ambiguous intent, hidden assumptions, timing effects, hardware/software mismatches, incomplete validation, weak evidence chains, and integration failures that are difficult to see when each layer is considered independently.

## Technologies

**Embedded / MCU**  
`STM32` · `GD32` · `RP2350` · `MSPM0` · `ARM Cortex-M`

**Software**  
`C` · `C++` · `Python` · `Bash` · `CMake` · `Git`

**Systems**  
`Linux` · `Embedded Linux` · `PREEMPT_RT` · `Buildroot` · `FreeRTOS` · `NuttX` · `QEMU`

**Control / Robotics**  
`State Space` · `PID` · `LQR` · `State Estimation` · `Kalman Filtering` · `System Identification`

**Engineering Execution**  
`Technical Planning` · `Engineering Governance` · `ADRs` · `Validation` · `Evidence Chains` · `Risk & Assumption Management`

**Interfaces / Integration**  
`UART` · `SPI` · `I2C` · `CAN` · `USB` · `RS-485` · `MAVLink`

## Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
