# Engineering Journey

This document expands the condensed engineering journey from the profile README and preserves the technical context behind that progression.

## 2005–2008 · Early Embedded Systems

My early work covered several different embedded domains:

- Quadcopter design, implementation, and flight-control work on an EM78569-based platform
- Mitsubishi PLC work for chemical-process control
- Sunplus-based interactive storybook systems
- Sunplus video / display processing experiments

One of the early quadcopter projects received **1st Place** in the 9th ELAN Microcontroller Application and Artificial Intelligence Design Competition, Microcontroller Application Project / Innovation Division. See [2006 Quadcopter Project](early-quadcopter-2006.md) for project and provenance details.

These early systems established a foundation in embedded implementation, control, timing, and real-world I/O, while also showing that system behavior rarely belongs to software or hardware alone.

## 2008–2021 · Embedded Systems, Mobile Platforms, Robotics, and Automation

During this period, my work expanded from device-level software and firmware into larger embedded platforms, control systems, robotics, heterogeneous computing, and complete physical-system integration.

The work covered Qualcomm-based mobile platforms, STM32 flight-control systems, BLDC motor control, sensing, Mecanum-wheel AGV motion control, robotic-system integration, application-processor architectures, and instrument automation.

As the systems became more complex, the engineering challenge increasingly shifted from implementing individual components to understanding interfaces, integration behavior, and the assumptions between subsystems.

### Mobile and Embedded Platforms

I spent a major part of this period working on Qualcomm-based mobile platforms, BSP and firmware development, and embedded software integration across Windows Mobile, Android, and related low-level software stacks.

This strengthened my experience in larger embedded software stacks, platform integration, device-level debugging, communication interfaces, and the interaction between low-level software and application-level system behavior.

### Flight Control, Motor Control, and Autonomous Systems

In parallel, I worked extensively on flight-control and autonomous-system technology using STM32-class MCUs and related embedded platforms.

Representative areas included:

- STM32 flight controllers
- NuttX and PX4-derived systems
- BLDC electronic speed controllers
- Gimbal control
- Optical-flow sensing
- Integrated flight-controller and multi-ESC platforms
- IMU, barometer, magnetometer, and navigation-sensor integration

Some historical source and board-porting work from this period is preserved in:

- [TMR-FC](https://github.com/cctsao1008/tmr-flight-controller) — **2013** · PX4-derived flight-controller platform and board-porting work
- [TMR-FC NuttX](https://github.com/cctsao1008/tmrfc-nuttx) — **2013** · NuttX-based platform work associated with TMR-FC
- [Bootloader](https://github.com/cctsao1008/Bootloader) — **2013** · modified PX4 bootloader for TMR-FC

### Robotics and Heterogeneous Systems

The work also expanded beyond MCU-only systems into heterogeneous architectures combining embedded controllers with application processors.

Projects and system-integration work included:

- STM32 + Nvidia Tegra K1 heterogeneous flight-control architectures
- Drone computer-vision collaboration, focusing on embedded control and system integration
- SLAM-oriented autonomous ground-vehicle collaboration, focusing on vehicle control and motion integration
- Mixed-reality drone concepts
- TI-based embedded application-processor platforms
- Mecanum-wheel AGV motion control
- Four- and six-axis robot-arm integration, including UR3
- Instrument automation and multi-device equipment control

Related repositories include:

- [NTUT Rover](https://github.com/cctsao1008/ntut_rover) — **2014** · Raspberry Pi-based autonomous rover following recorded GPS waypoints
- [Mecanum AGV Motion Control](https://github.com/cctsao1008/mecanum-agv-motion-control) — **2016** · vehicle-frame motion control, Mecanum-wheel kinematics, feedback control, and embedded execution for an AGV mobile base
- [Instrument Automation Control](https://github.com/cctsao1008/instrument-automation-control) — **2017** · modular instrument automation and equipment orchestration across device control, communication, scripting, scheduling, and data services

### Historical Platform Context

The work during this period spanned mobile application processors, MCU-based control systems, RTOS platforms, robotics, and heterogeneous embedded architectures.

### Embedded RTOS, Sensors, and Audio Experiments

Several older repositories preserve experiments in RTOS porting, sensor integration, audio processing, and low-level embedded software:

- [GPCE063 FreeRTOS Storybook](https://github.com/cctsao1008/gpce063-freertos-storybook) — **2011** · GPCE063, FreeRTOS, audio decoding, sensors, and file-system integration
- [GPCE063 FreeRTOS Motion Audio Demo](https://github.com/cctsao1008/gpce063-freertos-motion-audio-demo) — **2013** · FreeRTOS, BMA180, software I2C, A1600 audio, and Petit FAT
- [GPCE2064 FreeRTOS Funny Car](https://github.com/cctsao1008/gpce2064-freertos-funny-car) — **2014** · GPCE2064, FreeRTOS V8.0.0-era, audio, key scanning, LED control, sleep mode, and Petit FAT
- [C Digital Filter Lab](https://github.com/cctsao1008/c-digital-filter-lab) — **2016** · Octave/MATLAB filter design and validation, with resulting IIR/FIR coefficients translated into explicit C implementations
- [TS100 GCC](https://github.com/cctsao1008/ts100-gcc) — **2017** · historical GCC/Make-based STM32 firmware port/build work for the TS100 soldering iron

## 2021–Present · System Integration, Architecture, and Technical Leadership

My work has increasingly expanded from hands-on implementation, bring-up, and system debugging into architecture, cross-domain integration, validation, technical decision-making, project planning, and engineering execution across multiple projects and teams.

As the scope expanded across projects and teams, the difficult questions increasingly moved toward architecture, technical decisions, validation strategy, evidence, and how engineering work should be structured and communicated.

The underlying approach remains the same: understand the system at implementation level when necessary, then connect those details back to architecture, interfaces, validation, measurable evidence, and technical decisions.

## Recent Work · Real-Time Linux, RP2350, and Low-Level Architecture

More recent hands-on work has returned to low-level system architecture from a different direction:

- Embedded Linux and Buildroot
- PREEMPT_RT and real-time Linux experiments
- USB gadget interfaces
- RP2350 and dual-core MCU architecture
- Physical processor interfacing and deterministic bus service
- Control-system implementation and verification

## Current Research · Trustworthy Software Construction and Technical Execution

My current research direction is [Spec2Exec](https://github.com/cctsao1008/spec2exec), which explores whether accepted semantics, deterministic verification, executable generation, evidence, and provenance can be connected into a more trustworthy software-development chain.

In parallel, the [Technical Management Framework](https://github.com/cctsao1008/technical-management-framework) captures reusable practices for technical planning, engineering governance, execution, validation, evidence management, and AI-assisted collaboration across projects.

These research directions are not separate from the earlier engineering work. They grew from recurring problems encountered across embedded systems, control, integration, validation, and technical execution: unclear assumptions, weak interfaces between specification and implementation, incomplete evidence, and systems that appear correct locally but fail at their boundaries.

[← Back to profile README](../README.md)
