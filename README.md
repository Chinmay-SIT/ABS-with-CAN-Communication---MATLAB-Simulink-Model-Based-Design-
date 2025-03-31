# ABS-with-CAN-Communication in MATLAB-Simulink (Model-Based-Design)

## Project Overview

This project models an Anti-lock Braking System (ABS) with CAN communication in MATLAB Simulink using Model-Based Design (MBD) principles. The ABS prevents wheel lock-up during braking, improving vehicle control and safety. CAN communication enables real-time data exchange between the ABS and ECU.

### Features

1. ABS Model - Simulates wheel slip control and braking dynamics.
2. CAN Communication - Implements CAN-based message exchange between ABS and ECU.
3. Simulink Implementation - Fully modeled using Simulink blocks, including CAN Pack & Unpack.
4. Real-time Data Processing - Receives and processes wheel speed, vehicle speed, and stopping distance.
5. Model-Based Design (MBD) - Ensures structured development and automatic code generation.
6. Scalability - Can be extended for real hardware implementation.

## System Architecture

1. ABS Control Subsystem - Calculates slip ratio and applies braking force.
2. CAN Pack & Transmit - Converts ABS signals into CAN messages.
3. CAN Receive & Unpack - Receives messages and extracts signal data.
4. ECU Processing - Simulates real-time vehicle data processing.

## Setup & Simulation

### Prerequisites

MATLAB Simulink (R2022a or later recommended)

Simulink Real-Time & Vehicle Network Toolbox (for CAN simulation)

Embedded Coder (if generating C code for hardware)

Steps to Run

-Open ABS_MBD.slx in Simulink.

-Check the CAN Configuration Block settings (Baud rate, mode, etc.).

-Run the simulation and observe:

  1) Wheel Speed & Vehicle Speed outputs.

  2) Stopping Distance* computation.*

-CAN messages being sent and received.

-Adjust parameters as needed and re-run the simulation.

## Future Enhancements

 -Hardware-in-the-loop (HIL) Testing - Implement on actual ECUs.
 -Fault Injection Testing - Simulate CAN message loss and bit errors.
 -AI-based Optimization - Use machine learning for better braking control.
