# LTspice-LT1249-PFC-Boost-Converter
LTspice simulation of an Active PFC Boost Converter using LT1249, demonstrating high power factor AC-DC conversion with a regulated 385 V DC output.
LTspice Active PFC Boost Converter
AC-DC Power Factor Correction using LT1249 Controller

This repository contains a complete LTspice simulation of an Active Power Factor Correction (PFC) Boost Converter designed to convert AC mains voltage into a regulated high-voltage DC bus (~385 V) while maintaining high power factor and low harmonic distortion.

The design uses the LT1249 Average Current-Mode PFC Controller, a widely used integrated circuit for active PFC front-end stages in switch-mode power supplies.

This project demonstrates how an active PFC stage shapes input current to follow the AC input voltage waveform, resulting in efficient power transfer and compliance with harmonic standards.

Project Overview

Most modern power supplies (for computers, LED drivers, telecom equipment, etc.) require Power Factor Correction to reduce harmonic distortion and improve power efficiency when connected to the AC grid.

A Boost PFC Converter is commonly used as the front-end stage of such power supplies.

This project simulates that architecture using LTspice XVII, including:

AC input source
Full-bridge rectifier
Boost converter stage
LT1249 PFC controller
MOSFET switching device
Output energy storage capacitors
Feedback and compensation network

The converter takes AC mains input and produces a stable high-voltage DC bus suitable for downstream converters.

Key Features

• Active Power Factor Correction (PFC)

• Boost converter topology

• LT1249 average current-mode controller

• High output voltage regulation (~385 V DC)

• Near-unity power factor

• Low input current harmonic distortion

• Closed-loop voltage regulation

• Complete LTspice simulation environment

Electrical Specifications

•Input Voltage	120 VAC (165 V peak)

•Frequency	50 / 60 Hz

•Output Voltage	~385–400 V DC

•Switching Frequency	~100 kHz

•Inductor	750 µH

•Output Capacitance	66 µF

•Load	2 kΩ

•Controller	LT1249

•MOSFET	BSC240N12NS3

Simulation Results

The LTspice simulation verifies the correct operation of the Active PFC boost converter using the LT1249. The converter produces a regulated DC output of approximately 385–400 V with minimal ripple. The gate drive signal operates at high frequency (~100 kHz), ensuring proper switching of the MOSFET. The switch node waveform confirms typical boost converter behavior with efficient energy transfer.

The inductor current exhibits a triangular waveform with a sinusoidal envelope that closely follows the input voltage, indicating effective current shaping and near-unity power factor (≈0.98–0.99). 

FFT analysis shows that low-order harmonics are well suppressed, with dominant components around the switching frequency. Overall, the system demonstrates stable regulation, high power factor, and low harmonic distortion.
