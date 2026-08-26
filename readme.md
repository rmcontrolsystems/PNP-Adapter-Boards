# RM Control Systems PNP Adapter Boards

This repository contains customer support files for **RM Control Systems Plug-and-Play ECU Adapter Boards**.

RM Control Systems adapter boards are designed to provide affordable, yet capable standalone engine management solutions without costing as much as a supercharger itself. The goal is to provide engine management solutions that integrate cleanly with the factory vehicle, minimize unnecessary wiring and installation complexity, and give enthusiasts the flexibility to build, modify, and tune their vehicles without the cost and complexity traditionally associated with standalone engine management.

## Features

RM Control Systems PNP Adapter Boards are standalone engine management systems that retain as much of the factory Toyota wiring and packaging as possible.

- **Factory ECU Case Installation** – The adapter board installs directly into the factory ECU enclosure, providing a clean, protected installation in the original ECU location. No standalone ECU hogging your glovebox! 

- **Plug-and-Play Factory Harness Connection** – The vehicle's original ECU wiring harness plugs directly into the adapter board. No expensive adapter harnesses required for installation!

- **Standalone Engine Management** – Provides an interface between the factory vehicle wiring and supported standalone ECU hardware, allowing full control of fueling, ignition, idle, and other engine functions.

- **Automatic Transmission Control** – Provides control of the A340E/F automatic transmission, including selectable shift maps, shift points, torque converter lockup, manual shift mode, etc.

- **Factory System Integration** – Adapter boards are designed to retain and interface with applicable factory vehicle systems rather than requiring the vehicle to be rewired around the standalone ECU. This includes compatibility with the shared negative leads that Toyota often uses in their crank/cam sensors that has proven problematic in other ECUs. There is no need to separate the negative crank/cam wires within the factory wiring harness like other ECUs often require.

- **Additional Inputs and Outputs** – Unused positions in the factory ECU connectors can be used for additional sensors, switches, and outputs. Please refer to each board's documentation file for pinouts for additional inputs/outputs.

- **Expandable Sensor Support** – Additional inputs can be used for upgrades such as manifold absolute pressure (MAP), flex-fuel, fuel pressure, oil pressure, wideband input, etc. Please refer to each board's documentation file for pinouts for additional inputs/outputs.

- **Expandable Output Support** – Available outputs can support additional functions such as fully sequential ignition (requires smart coils or 6-channel igniter), integrated 7th injector control, electronic throttle body (drive by wire), boost control, auxiliary relays, etc. Please refer to each board's documentation file for pinouts for additional inputs/outputs.

## Repository Contents

This repository contains resources including:

- **Board Documentation** – Pinouts, specifications, connector information, and other documentation specific to each adapter board. Page 1 is Open Pins / Additional I/O: Identifies unused positions in the factory ECU connectors that can be populated to add additional inputs and outputs. Page 2 is Populated Pins / Factory Circuits: Identifies the factory ECU circuits connected through the adapter board and the TunerStudio channels associated with them. This provides a reference for locating and configuring factory functions such as injectors, ignition coils, crank and cam signals, and other factory circuits.

In the future, this repository will contain:
- **Firmware** – Firmware releases for supported ECU hardware, including the corresponding TunerStudio `.ini` file when applicable
- **Base Tunes** – Starting calibration files for supported vehicle and engine combinations
- **TunerStudio** – Dashboards, custom channels, and other TunerStudio resources
- **Software & Drivers** – Utilities and drivers required for firmware installation or communication with supported hardware
- **Getting Started & Support Documentation** – Installation, initial setup, configuration, and troubleshooting information

Additional files and sections will be added as support for RM Control Systems products expands.

### Currently Supported Vehicles

Current vehicles include:

- **1996 4Runner / 1995–1997 Tacoma & T100**
- **1997–1998 4Runner / 1998–1999 Tacoma / 2000 Federal-Emissions Tacoma**
- **1999–2000 4Runner / 2000 California-Emissions Tacoma / 2001 Tacoma**

## Firmware and TunerStudio INI Files

Always use the **TunerStudio `.ini` file supplied with the corresponding firmware release**. Firmware and `.ini` files are version-specific and should be updated together.

## Base Tunes

Base tunes are intended only as **starting calibrations** for supported applications.

Engine configuration, injectors, fuel type, forced induction, sensors, vehicle modifications, and other differences can require substantial calibration changes. Verify all configuration settings for your specific vehicle before operating the engine.

## Important

### Tuning and Configuration Warning

Standalone engine management systems require proper installation, configuration, and calibration. Incorrect wiring, configuration, firmware, or engine calibration may cause improper vehicle operation and may result in damage to the engine, transmission, ECU, or other vehicle components.

Base tunes and configuration files provided by RM Control Systems are intended as starting points only. The user is responsible for verifying all settings and ensuring that the vehicle is properly calibrated for its specific engine, fuel system, sensors, modifications, and operating conditions before use.

### Competition / Off-Road Use and Emissions Compliance

RM Control Systems PNP Adapter Boards are intended for competition, racing, and other lawful off-road applications and are not intended to be used to bypass, defeat, disable, or render inoperative any emissions-control device or system.

These products are not intended for installation or use on emissions-controlled motor vehicles where such installation or use would violate applicable federal, state, or local law. The purchaser and installer are responsible for determining and maintaining compliance with all laws and regulations applicable to the vehicle and its use.