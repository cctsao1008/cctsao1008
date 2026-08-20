# Historical Projects

This is the canonical index of older public repositories and experiments. It keeps the profile README and the engineering journey focused on the larger engineering narrative rather than on platform inventories.

The projects are grouped by the kind of system problem they explored, not simply by processor, language, or toolchain. Read together, they show an evolution from RTOS and board-level work into flight-control systems, robotics, automation, heterogeneous system integration, and model-to-implementation workflows.

Descriptions deliberately distinguish original project work, platform and porting work, derived trees, and experiments. Everything listed here is preserved primarily as historical or reference material rather than as an actively maintained project; see the [profile README](../README.md) for current work.

## Flight Control & Autonomous Systems

### [TMR-FC — Top Multi-Rotor Flight Controller](https://github.com/cctsao1008/tmr-flight-controller)

**2013 · Historical Project**

An open hardware and software multirotor platform that combined an STM32 flight controller with onboard sensing, actuator interfaces, logging, navigation interfaces, and later Raspberry Pi companion-computer experiments.

The architecture used PX4-derived firmware and explored a split between a real-time STM32 flight-control layer and higher-level Raspberry Pi processing for OpenCV, ROS, MAVLink, vision, and optical-flow work.

### [TMR-FC NuttX](https://github.com/cctsao1008/tmrfc-nuttx)

**2013 · Historical Platform Work**

A NuttX RTOS source tree adapted for the TMR-FC STM32F405 platform, preserving the board-support and RTOS side of the broader flight-controller work.

The repository includes TMR-FC-specific board configuration, STM32F4 support, NSH/application configurations, and low-level porting context from the older NuttX toolchain model.

### [Bootloader](https://github.com/cctsao1008/Bootloader)

**2013 · Historical Derived Work**

A PX4-era STM32 bootloader tree adapted to include the TMR-FC flight-controller target.

The design separates common firmware-loading logic from MCU- and board-specific support, using USB CDC or USART for firmware transfer, flash programming, validation, and application handoff. It is preserved as derived bootloader and board-integration work rather than as an independently originated bootloader architecture.

### [NTUT Rover](https://github.com/cctsao1008/ntut_rover)

**2014 · Historical Project**

A small Raspberry Pi-based autonomous rover designed to run missions by following a list of recorded GPS waypoints.

The public repository currently has no top-level README, so this description is intentionally limited to the scope stated by the repository itself rather than inferring a deeper architecture that is not documented there.

## Robotics & Automation

### [Mecanum AGV Motion Control](https://github.com/cctsao1008/mecanum-agv-motion-control)

**2016 · Historical Project**

A motion-control subsystem for a physical Mecanum-wheel AGV, translating vehicle-level planar commands into coordinated wheel motion while keeping the mobile base usable as part of a larger robotic system.

The architecture separates vehicle-frame commands (`vx`, `vy`, `w0`), forward and inverse kinematics, feedback control, platform geometry, motor interfaces, host-side simulation, and embedded execution. This repository represents the AGV mobile-base control layer rather than the complete robot-arm or integrated robotic system.

### [Instrument Automation Control](https://github.com/cctsao1008/instrument-automation-control)

**2017 · Historical Project**

A legacy Windows C/C++ supervisory automation system for coordinating heterogeneous equipment, communication interfaces, scripts, scheduling, and data services within a multi-stage automated workflow.

Its architecture separates workflow and scripting from command/scheduling infrastructure, core orchestration, equipment-specific modules, motion and communication interfaces, and supporting services such as configuration, logging, messaging, and database access.

## Embedded RTOS & Sensor Experiments

### [GPCE063 FreeRTOS Storybook](https://github.com/cctsao1008/gpce063-freertos-storybook)

**2011 · Historical Project**

An interactive-audio embedded project on the Sunplus GPCE063 platform, combining FreeRTOS, audio playback, sensor access, file-system support, and board-level application behavior.

The repository also preserves low-level FreeRTOS porting work, including context-switch and interrupt integration, rather than only application code using an existing RTOS port.

### [GPCE063 FreeRTOS Motion Audio Demo](https://github.com/cctsao1008/gpce063-freertos-motion-audio-demo)

**2013 · Historical Experiment**

A motion-driven audio demo connecting BMA180 sensor input to application behavior under FreeRTOS, with software I2C, A1600 audio decoding, and Petit FAT storage support.

It preserves a complete sensing-to-application path — sensor input, I2C driver, RTOS task logic, and audio output — and shares significant historical code lineage with the GPCE063 storybook work.

### [GPCE2064 FreeRTOS Funny Car](https://github.com/cctsao1008/gpce2064-freertos-funny-car)

**2014 · Historical Project**

A GPCE2064 embedded application integrating FreeRTOS with audio playback, key scanning, LED updates, low-power behavior, and file-system support.

The codebase separates application behavior, RTOS services, BSP/drivers, and the physical GPCE2064 platform, while preserving the mixed C/assembly and vendor-toolchain environment of the original system.

## Signal Processing & Firmware Porting

### [C Digital Filter Lab](https://github.com/cctsao1008/c-digital-filter-lab)

**2016 · Historical Experiment**

A compact DSP workflow that starts with filter design and validation in Octave/MATLAB, then transfers the accepted coefficients and difference equations into an explicit C implementation.

The project is structured around a reference-model-to-implementation loop: inspect recorded sensor data, design and validate IIR/FIR filters numerically, implement them in C, and compare the resulting output against the numerical-tool reference.

### [TS100 GCC](https://github.com/cctsao1008/ts100-gcc)

**2017 · Historical Port / Build Work**

A GCC/Make-based STM32 firmware build for the TS100 soldering iron, preserving a small embedded system with temperature sensing, PID control, OLED UI, settings, watchdog handling, I2C, and accelerometer support.

The source identifies Ben V. Brown as the original application author; this repository is therefore positioned as historical GNU Arm toolchain, build, and firmware-port work rather than original authorship of the TS100 application firmware.

## Attribution Note

Some historical repositories contain substantial upstream, third-party, ported, or derived code. Where that applies — including PX4-, NuttX-, FreeRTOS-, and TS100-related trees — the descriptions above identify the local work as integration, porting, customization, derived work, or experimentation rather than claiming authorship of the upstream system.

The individual repositories remain the source of truth for their detailed architecture, implementation, build assumptions, and provenance.

[← Back to profile README](../README.md) · [Engineering Journey →](engineering-journey.md)
