# Zigbee2mqtt Device Naming Convention

## Introduction
This document outlines the naming convention for Zigbee2mqtt devices. Following a structured naming convention facilitates easy identification and management of devices within the Zigbee network.

## Naming Format
The naming convention follows a specific format tailored to different types of devices:

### Media Players
For media players, the naming convention is as follows:

```
<location>(_<sublocation>)_<type>
```

- `<location>`: Location identifier where the media player is situated.
- `<sublocation>`: Optional sublocation within the main location.
- `<type>`: Type of media player, which can be either `tv` or `speaker`.

#### Examples:
- `lounge_tv`
- `kitchen_speaker`

### Sensors
Sensors adhere to the following naming convention:

```
<location>(_<sublocation>)_<type>
```

- `<location>`: Location identifier where the sensor is deployed.
- `<sublocation>`: Optional sublocation within the main location.
- `<type>`: Sensor type

#### Examples:
- `bedroom_climate`
- `tfhallway_motion`

### Radiator
Thermostatic Radiator Valves adhere to the following naming convention:

```
<location>_radiator
```

- `<location>`: Location identifier where the sensor is deployed.

#### Examples:
- `doffice_radiator`

### Lights
The naming convention for lights is structured as follows:

```
<location>(_<sublocation>(_<number>))_light
```

- `<location>`: Location identifier where the light is installed.
- `<sublocation>`: Optional sublocation within the main location.
- `<number>`: Optional number to distinguish between multiple lights in the same sublocation.

#### Examples:
- `ffbedroom_light`
- `kitchen_ceiling_1_light`

### Group Devices
Group devices, such as media player groups and light groups, follow the same naming convention as their individual counterparts. However, they are prefixed with `group_` and suffixed with `s`.

#### Examples:
- `group_livingroom_speakers`
- `group_kitchen_lights`

## Location Identifiers
Locations can be abbreviated as follows:
- `gf`: Ground Floor
- `ff`: First Floor
- `sf`: Second Floor (or Top Floor)
- `d`: Dillon's
- Specific room names or abbreviations (e.g., `hallway`, `kitchen`, `bedroom`, `bathroom`, `dining`, etc.)

## Conclusion
Consistently applying this naming convention ensures clarity and organization within the Zigbee2mqtt network. By following the prescribed format, users can easily identify and manage devices based on their locations and types.
