# Enhanced Generic Thermostat

Combine heating and cooling into a single thermostat component for Home Assistant

## Installation

Open a terminal inside your custom_components folder type the following:

`git clone https://github.com/carlymarie/enhanced-generic-thermostat.git`

## Usage
Add the following to `configuration.yaml` and make changes if needed.
```yaml
climate:
    - platform: enhanced_generic_thermostat
      name: Thermostat
      target_sensor: sensor.temperature_average
      heater: switch.heating
      cooler: switch.cooling
      min_temp: 60
      max_temp: 85
      precision: 0.1
      cold_tolerance: 1
      hot_tolerance: 0
      min_cycle_duration:
          minutes: 8
      initial_hvac_mode: "heat"
      away_temp: 60
```
