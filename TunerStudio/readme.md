# RM Control Systems TunerStudio Files

This folder contains TunerStudio resources for RM Control Systems PNP standalone engine management systems, including custom dashboards and the `custom.ini` file used to add additional calculated and converted channels to TunerStudio.

## Installing custom.ini

Download the `custom.ini` file from this folder and place it in the `projectCfg` folder for your TunerStudio project.

The typical Windows path is:

`Documents\TunerStudioProjects\[Project Name]\projectCfg`

For example:

`Documents\TunerStudioProjects\My 4Runner\projectCfg`

Copy `custom.ini` into the `projectCfg` folder, then restart or reopen the TunerStudio project.

> **Note:** `[Project Name]` is the name of your individual TunerStudio project. Each project has its own `projectCfg` folder.

## Custom Channels

The supplied `custom.ini` adds the following channels:

| Channel | Description |
| --- | --- |
| `VehicleSpeedMPH` | Converts the primary vehicle speed channel from km/h to MPH. |
| `VehicleSpeedMPH1` | Converts the secondary vehicle speed channel from km/h to MPH. |
| `FuelTempF` | Converts fuel temperature from °C to °F. |
| `MAFlbsmin` | Converts measured mass airflow to pounds per minute (lb/min). |
| `MPG_Total` | Calculates cumulative average fuel economy in MPG using accumulated vehicle distance and calculated fuel consumption. |
| `AuxTemp1F` | Converts Auxiliary Temperature 1 from °C to °F. This channel is commonly used for automatic transmission fluid temperature. |
| `coolantF` | Converts engine coolant temperature from °C to °F. |
| `intakeF` | Converts intake air temperature from °C to °F. |
| `MPG` | Calculates instantaneous fuel economy in MPG using vehicle speed, fuel flow, ethanol content, and fuel temperature. |

## Dashboards

This folder also contains RM Control Systems TunerStudio dashboards in both Imperial and Metric units.

- `Main Dash Imperial Units.dash`
- `Main Dash Metric Units.dash`

The Imperial dashboard is intended for users who prefer MPH, °F, lb/min, and MPG-based channels. The Metric dashboard retains metric units where applicable.

## Notes

The `custom.ini` file supplements the firmware-specific TunerStudio `.ini` file; it does not replace it.

Firmware-specific `.ini` files should always match the firmware version installed on the ECU.