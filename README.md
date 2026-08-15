# Ricardo Tsao

**Senior Manager · Embedded Systems · Firmware · System Architecture · Control Systems · Robotics**

Hands-on engineering leader working across embedded software, firmware, hardware/software integration, control systems, real-time systems, and system-level validation.

My work and personal research span embedded Linux, MCU platforms, motor control, robotics, autonomous systems, low-level computer architecture, and specification-to-executable software engineering.

I am particularly interested in the boundaries between specification, architecture, implementation, verification, hardware behavior, and real-world measurement — the places where individually correct components can still fail as an integrated system.

## Current Focus

- Embedded systems and firmware architecture
- Embedded Linux and real-time Linux
- MCU-based system development
- Motor control and real-time control
- Control systems and robotics
- Hardware/software integration and bring-up
- System modeling, verification, debugging, and validation
- Specification-to-executable engineering
- Trust and evidence for AI-assisted software engineering

## Selected Projects

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

Historical open hardware and software multirotor flight-controller project built around STM32F405/STM32F407 and PX4-derived firmware.

The platform includes inertial and environmental sensing, actuator interfaces, data logging, navigation interfaces, and experiments with Raspberry Pi companion computing for OpenCV, ROS, MAVLink, vision, and optical-flow applications.

### [NTUT Rover](https://github.com/cctsao1008/ntut_rover)

Autonomous ground-vehicle experiment using Raspberry Pi, GPS waypoint navigation, motor control, filtering, and supporting MATLAB-based GPS analysis.

### [DEVC Motion Controller](https://github.com/cctsao1008/devc_motion_controller)

Modular mobile-robot motion-control framework covering forward/inverse kinematics, PID and fuzzy control paths, platform abstraction, simulation, and STM32-based firmware targets.

## Real-Time Linux Experiments

Ongoing exploration of Linux-based embedded and real-time systems, including:

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
`Linux` · `Embedded Linux` · `PREEMPT_RT` · `Buildroot` · `QEMU`

**Control / Robotics**  
`State Space` · `PID` · `LQR` · `State Estimation` · `Kalman Filtering` · `System Identification`

**Interfaces / Integration**  
`UART` · `SPI` · `I2C` · `CAN` · `USB` · `RS-485` · `MAVLink`

## Philosophy

> Build systems that are not only functional, but understandable, testable, verifiable, and explainable.
