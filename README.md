# Huawei-energy-managment
HACS package for Home Assistant to optimize your Huawei battery and solar panels. Control charging based on prices, battery state, and solar forecast to maximize self-consumption.

# Smart Home Power

A Home Assistant custom component for calculating house power consumption,
optionally excluding EV charging and including solar production.

## Installation

1. Copy the `custom_components/smart_home_power` folder to your Home Assistant `custom_components` directory.
2. Add `sensors.yaml` and `helpers.yaml` to your configuration.
3. Fill in your EV charger and solar sensors via the input_text helpers.

## Sensors

- `house_power_excl_ev`: Calculates house power in kW.
