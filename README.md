# Robot Goalkeeper — Embedded Control Portfolio

## Overview

This project is a real-time robotic goalkeeper system developed as a
Mechatronics Engineering graduation project.

The system combines camera-based trajectory estimation, STM32-based
motion control, motor-driver integration and mechanical actuation.

This repository presents the system architecture, engineering decisions,
verification methods and my individual contributions.

> Full source code, research files and unpublished technical implementations
> are maintained in private repositories.

## System Architecture

```text
Single Camera System
        |
        v
Raspberry Pi 5
Trajectory Estimation
        |
        | UART target command
        v
STM32G431KB
Real-Time Motion Control
        |
        | STEP / DIR
        v
CWD860 Motor Driver
        |
        v
NEMA 34 Stepper Motor
        |
        v
1:6 Belt-Pulley Mechanism
