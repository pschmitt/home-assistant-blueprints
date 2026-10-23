# Home Assistant Blueprint by pschmitt

## 🐝🛀 wasps in a bathtub

Automated bathroom lighting, using a motion sensor, a door sensor. It's a pure 
Home Assistant Wasps-in-a-box implementation.

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fpschmitt%2Fhome-assistant-blueprints%2Fblob%2Fmain%2Fwasps-in-a-bathtub.yaml)

## Shelly Detached Input

[shelly-detached-input.yaml](shelly-detached-input.yaml) handles a wall switch
paired with a Shelly relay and smart bulb. With watchdog v2, configure its
**Watchdog input event topic** so only presses owned by the Shelly's confirmed
smart mode reach HA. Native relay control handles fallback locally.

Read the [architecture and operations guide](https://github.com/pschmitt/homeassistant-smart-bulb-relay/blob/main/docs/shelly-watchdog.md)
for normal operation, outage/recovery behavior, mode diagnostics, configuration,
and the reasons for the heartbeat and input ownership rules.
