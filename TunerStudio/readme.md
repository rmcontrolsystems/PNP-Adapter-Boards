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
| `VehicleSpeedMPH` | Displays the Vehicl Speed Sensor channel in MPH. |
| `VehicleSpeedMPH1` | Displays average wheel speed channel in MPH. |
| `FuelTempF` | Displays fuel temperature in °F. |
| `MAFlbsmin` | Displays measured mass airflow in pounds per minute (lb/min). |
| `MPG_Total` | Calculates cumulative average fuel economy in MPG using accumulated vehicle distance and calculated fuel consumption. |
| `AuxTemp1F` | Displays Auxiliary Temperature 1 in °F. This channel is commonly used for automatic transmission fluid temperature. |
| `coolantF` | Displays engine coolant temperature in °F. |
| `intakeF` | Displays intake air temperature in °F. |
| `MPG` | Calculates instantaneous fuel economy in MPG using vehicle speed, fuel flow, ethanol content, and fuel temperature. |

## Notes

The `custom.ini` file supplements the firmware-specific TunerStudio `.ini` file; it does not replace it.

Firmware-specific `.ini` files should always match the firmware version installed on the ECU.
