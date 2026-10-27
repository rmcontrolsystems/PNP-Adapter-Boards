# RM Control Systems TunerStudio Files

This folder contains TunerStudio resources for RM Control Systems PNP standalone engine management systems, including custom dashboards, additional calculated channels, and firmware-specific ECU definition (.ini) files.

## Folder Contents

### Dashboards

The **Dashboards** folder contains custom TunerStudio dashboards and the `custom.ini` file used to add additional calculated and converted channels.

Resources include:

- **Imperial Dashboard** – Custom dashboard displaying vehicle and engine parameters using Imperial units.
- **Metric Dashboard** – Custom dashboard displaying vehicle and engine parameters using Metric units.
- **custom.ini** – Adds nine custom channels for vehicle speed, temperature, mass airflow, and fuel economy calculations.

Refer to the Dashboards folder for installation instructions and descriptions of the custom channels.

### INI Definition Files

The **INI Definition Files** folder contains firmware-specific TunerStudio ECU definition files.

These `.ini` files allow TunerStudio to communicate with the ECU and provide the appropriate configuration menus, settings, tables, and monitoring channels for the installed firmware.

**Always use the `.ini` definition file that corresponds to the firmware version installed on your ECU.**

Refer to the INI Definition Files folder for additional information and installation instructions.

## Important Notes

- Firmware-specific ECU definition files and `custom.ini` serve different purposes and are not interchangeable.
- The firmware definition file must be compatible with the installed ECU firmware.
- The `custom.ini` file supplements the firmware definition by adding additional custom channels.
- Some custom dashboards may require `custom.ini` to be installed for all gauges to function correctly.
