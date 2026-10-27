# TunerStudio INI Definition Files

This folder contains TunerStudio ECU definition (`.ini`) files for firmware versions supported by RM Control Systems PNP standalone engine management systems.

## What Is an INI Definition File?

TunerStudio uses an ECU definition file to interpret the settings, configuration parameters, tables, and real-time data provided by the ECU firmware.

The `.ini` file defines how TunerStudio communicates with and configures the ECU, including access to functions such as:

- Fuel injection and ignition configuration
- Fuel and ignition tuning tables
- Idle control
- Sensor calibration and configuration
- Automatic transmission control
- Additional inputs and outputs
- Real-time monitoring and data logging

Available functions depend on the installed firmware version and ECU hardware.

## Selecting the Correct INI File

**The `.ini` file must correspond to the firmware version installed on your ECU.**

Using an incompatible definition file may cause TunerStudio to display incorrect parameters, fail to communicate properly, or write incorrect configuration values to the ECU.

Before downloading, verify the firmware version installed on your ECU and select the corresponding `.ini` file from this folder.

## Installing the INI Definition File

For an existing TunerStudio project:

1. Download the `.ini` file corresponding to your installed ECU firmware.
2. Open your project in TunerStudio.
3. Navigate to **File → Project → Project Properties**.
4. Locate the **ECU Definition** section.
5. Select the option to use another ECU definition file and browse to the downloaded `.ini` file.
6. Save the project settings and reconnect to the ECU.

When creating a new TunerStudio project, select the appropriate `.ini` file during the project setup process if automatic ECU definition detection does not provide the correct version.

## Important Notes

- Always use the definition file corresponding to your installed firmware version.
- Updating the `.ini` file does **not** update the firmware installed on the ECU.
- Firmware updates may introduce new settings or change existing parameters. Use the corresponding definition file when updating firmware.
- Back up your existing TunerStudio project and tune (`.msq`) before changing firmware versions or ECU definitions.
- The `custom.ini` file located in the **Dashboards** folder is separate from the firmware-specific ECU definition file and provides additional custom channels.