
# Home Assistant configuration - YamiFrankc

This is my configuration for Home Assistant. Its probably very basic. For automation I use a combination of
Node-Red and HA's own automation.


## System
My HA is running with Docker in an Ubuntu Server install, which is virtualized in Proxmox, running in a Dell R710.

## Hubs
I use Zigbee2MQTT to control all of my Zigbee devices, and I'm planning on getting a Vera plus to control
Z-Wave decives. I don't have any yet... but I know I will have at least a thermostat

## Switches

I use Sonoff basics flashed with Tasmota
