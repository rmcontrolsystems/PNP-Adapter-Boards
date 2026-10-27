# RM Control Systems TunerStudio Dashboards

This folder contains custom TunerStudio dashboards and the `custom.ini` file for RM Control Systems PNP standalone engine management systems. The dashboards provide a customized interface for monitoring engine and vehicle parameters, while `custom.ini` adds additional calculated and converted channels that can be used for dashboard gauges and data logging.

## Dashboard Files

Two dashboards are provided:

- **Main Dash Imperial Units.dash** – Displays engine and vehicle parameters using Imperial units, including MPH, °F, lb/min, and MPG where applicable.
- **Main Dash Metric Units.dash** – Displays engine and vehicle parameters using Metric units where applicable.

### Installing a Dashboard

1. Download the desired `.dash` file from this folder.
2. Open your TunerStudio project and connect to your ECU.
3. Navigate to **File → Load Dashboard** and select the downloaded `.dash` file.
4. Save the dashboard layout if prompted.

Some dashboard gauges rely on channels defined in `custom.ini`. Install this file using the instructions below to ensure all gauges function correctly.

## Installing custom.ini

The `custom.ini` file adds additional calculated and converted channels to TunerStudio. These channels supplement the ECU's firmware-specific definition file and do not replace it.

Download `custom.ini` from this folder and place it in the `projectCfg` folder for your TunerStudio project.

The typical Windows path is:

`Documents\TunerStudioProjects\[Project Name]\projectCfg`

For example:

`Documents\TunerStudioProjects\My 4Runner\projectCfg`

Copy `custom.ini` into the `projectCfg` folder, then restart or reopen the TunerStudio project.

**Note:** `[Project Name]` is the name of your individual TunerStudio project. Each project has its own `projectCfg` folder. If a `custom.ini` file already exists, back it up before replacing or modifying it.

## Custom Channels

The supplied `custom.ini` adds the following nine channels:

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

## Important Notes

- The `custom.ini` file supplements the firmware-specific TunerStudio ECU definition file; it does not replace it.
- Firmware-specific `.ini` files are located in the **INI Definition Files** folder and must match the firmware version installed on the ECU.
- Custom channels may depend on specific ECU firmware output channels. If a channel is unavailable or a gauge does not display correctly, verify that the installed firmware and ECU definition file support the required inputs.
- The MPG calculations are estimates based on ECU-reported parameters and may differ from actual fuel economy measured at the pump.