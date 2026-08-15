# Ricardo Tsao

**Senior Manager · Hands-on Embedded Systems Engineer · Firmware · System Architecture · Control Systems**

I work on engineering problems that cross the boundary between software, firmware, hardware, sensing, actuation, timing, and real-world system behavior.

My background spans embedded systems, MCU and application-processor platforms, RTOS and embedded Linux, flight control, motor control, robotics, autonomous systems, system integration, and low-level computer architecture.

Today, I remain hands-on while also working at the architecture and technical-leadership level. I am especially interested in systems where correctness depends not only on individual components, but on how specification, software, hardware, timing, verification, and measurement interact as a whole.

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
- Specification-to-executable engineering
- Trust, evidence, and provenance for AI-assisted software engineering

## Selected Current Projects

### [Spec2Exec](https://github.com/cctsao1008/spec2exec)

**Specification-to-Executable Architecture**

Research prototype exploring how accepted semantics, deterministic verification, artifact-bound evidence, provenance, and executable generation can be connected into a trustworthy specification-to-executable chain.

The current prototype demonstrates a native RV32I path under QEMU with explicit per-boundary evidence. Semantic-authority gating and physical RP2350 / Hazard3 validation remain active research directions.

### [Rotary Inverted Pendulum](https://github.com/cctsao1008/inverted-pendulum)

From-scratch embedded firmware and control software for a rotary inverted pendulum.

The project covers STM32F103 bring-up, sensing, encoder acquisition, motor characterization, state estimation, state-feedback control, fail-closed safety boundaries, telemetry, and host-side verification.

### [Pi86-RP2350](https://github.com/cctsao1008/pi86-rp2350)

Porting the Pi86 concept to a Waveshare RP2350-PiZero while preserving the original Pi86 V20/V30 HAT and using a physical NEC V30 processor.

The architecture explores deterministic RP2350 firmware for V30 clocking and bus service using PIO/SIO, with planned PSRAM, MicroSD, DVI, and USB integration. The current phase is hardware bring-up.

### [TMR-FC — Top Multi-Rotor Flight Controller](https://github.com/cctsao1008/tmr-flight-controller)

Historical open hardware and software multirotor flight-controller platform built around STM32F405/STM32F407 and PX4-derived firmware.

The platform integrates inertial and environmental sensing, actuator interfaces, data logging, navigation interfaces, and Raspberry Pi companion-computer experiments for OpenCV, ROS, MAVLink, vision, and optical-flow applications.

## Engineering Journey

### 2005–2008 · Early Embedded Systems

My early work covered several very different embedded domains:

- Quadcopter development on an EM78569 platform
- Mitsubishi PLC work for chemical-process control
- Sunplus-based interactive storybook systems
- Sunplus video / display processing experiments

These projects established the foundation for working close to hardware, timing, peripherals, real-world I/O, and embedded-system constraints.

### 2008–2016 · Mobile and Embedded Platforms

I spent a major part of this period working on Qualcomm-based mobile platforms and embedded software integration.

This period strengthened my experience in larger embedded software stacks, platform integration, device-level debugging, communication interfaces, and the interaction between low-level software and application-level system behavior.

### 2010s · Flight Control, Motor Control, and Autonomous Systems

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

- [TMR-FC](https://github.com/cctsao1008/tmr-flight-controller)
- [TMR-FC NuttX](https://github.com/cctsao1008/tmrfc-nuttx)
- [Bootloader](https://github.com/cctsao1008/Bootloader)

### 2010s · Robotics and Heterogeneous Systems

The work expanded beyond MCU-only systems into heterogeneous architectures combining embedded controllers with application processors.

Projects and experiments included:

- STM32 + Nvidia Tegra K1 flight-controller architecture
- Computer-vision concepts for drones
- SLAM-oriented autonomous ground vehicles
- Mixed-reality drone concepts
- TI-based embedded application-processor platforms
- AGV systems
- Robot-arm integration
- Data-acquisition and equipment-control systems

Related repositories include:

- [NTUT Rover](https://github.com/cctsao1008/ntut_rover)
- [DEVC Motion Controller](https://github.com/cctsao1008/devc_motion_controller)
- [CTC Control](https://github.com/cctsao1008/ctc_control)

### Embedded RTOS, Sensors, and Audio Experiments

Several older repositories preserve experiments in RTOS porting, sensor integration, audio processing, and low-level embedded software:

- [GPCE063 FreeRTOS Storybook](https://github.com/cctsao1008/gpce063-freertos-storybook) — GPCE063, FreeRTOS, audio decoding, sensors, and file-system integration
- [GPCE063 FreeRTOS Motion Audio Demo](https://github.com/cctsao1008/gpce063-freertos-motion-audio-demo) — FreeRTOS, BMA180, software I2C, A1600 audio, and Petit FAT
- [GPCE2064 FreeRTOS Funny Car](https://github.com/cctsao1008/gpce2064-freertos-funny-car) — GPCE2064, FreeRTOS V8.0.0-era, audio, key scanning, LED control, sleep mode, and Petit FAT
- [Digital Filter](https://github.com/cctsao1008/digital-filter) — C implementation and Octave/MATLAB comparison of IIR/FIR digital filters
- [TS100 GCC](https://github.com/cctsao1008/ts100-gcc) — GCC/Make-based STM32 firmware build for the TS100 soldering iron

### Recent Work · Real-Time Linux, RP2350, and Low-Level Architecture

More recent work has returned to low-level system architecture from a different direction:

- Embedded Linux and Buildroot
- PREEMPT_RT and real-time Linux experiments
- USB gadget interfaces
- RP2350 and dual-core MCU architecture
- Physical processor interfacing and deterministic bus service
- Control-system implementation and verification

### Current Research · Trustworthy Software Construction

My current research direction is [Spec2Exec](https://github.com/cctsao1008/spec2exec), which explores whether accepted semantics, deterministic verification, executable generation, evidence, and provenance can be connected into a more trustworthy software-development chain.

This is a natural extension of a recurring engineering problem I have seen across embedded systems: a system can appear correct at the requirement, software, hardware, or test level individually and still fail at the boundaries between them.

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
Feedback
```

I am most interested in the gaps between these layers: ambiguous intent, hidden assumptions, timing effects, hardware/software mismatches, incomplete validation, and integration failures that are difficult to see when each layer is considered independently.

## Technologies

**Embedded / MCU**  
`STM32` · `GD32` · `RP2350` · `MSPM0` · `ARM Cortex-M`

**Software**  
`C` · `C++` · `Python` · `Bash` · `CMake` · `Git`

**Systems**  
`Linux` · `Embedded Linux` · `PREEMPT_RT` · `Buildroot` · `FreeRTOS` · `NuttX` · `QEMU`

**Control / Robotics**  
`State Space` · `PID` · `LQR` · `State Estimation` · `Kalman Filtering` · `System Identification`

**Interfaces / Integration**  
`UART` · `SPI` · `I2C` · `CAN` · `USB` · `RS-485` · `MAVLink`

## Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
