# Board Documentation

This folder contains vehicle-specific documentation for RM Control Systems PNP Adapter Boards. Select the documentation that corresponds to your vehicle model and year, taking into account the emissions configuration (Federal or California) and transmission type (automatic or manual) where applicable. Verify that the adapter board revision number shown in the documentation matches the revision number stamped on your adapter board.

Each specification sheet includes ECU connector diagrams and detailed pin assignments for two categories:
1. **Additional Inputs/Outputs** – Available connections that can be used to add sensors, switches, outputs, and other functions.
2. **Factory Circuits** – Existing vehicle circuits connected to and controlled or monitored by the standalone engine management system.

## How to Use the Documentation

- **Page 1 – Open Pins / Additional I/O:** Identifies unused positions in the factory ECU connectors that can be populated to add additional inputs and outputs. The documentation identifies the factory ECU connector and pin, the available input or output function, and the corresponding TunerStudio channel.

- **Page 2 – Populated Pins / Factory Circuits:** Identifies the factory ECU circuits connected through the adapter board and the TunerStudio channels associated with them. This provides a reference for locating and configuring factory functions such as injectors, ignition coils, crank and cam signals, idle control, automatic transmission functions, vehicle speed signals, A/C circuits, and other factory inputs and outputs.
