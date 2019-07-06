
# Home Assistant configuration - YamiFrankc

This is my configuration for Home Assistant. Its probably very basic. For automation I use a combination of Node-Red and HA's own automation; as of now.
But I'm planning to move everything to Node-Red.

## Custom Lovelace cards
|Card name| What for|
|-------| --------|
| Aftership Card| I use this card to neatly display the packages I am tracking |
|Compact Custom Header| Makes the header slim and cool|
|Button card| This makes Lovelace so prettier!|
|Mini Graph Card| I like how it looks|
| Mini media Player | Looks so much cooler than the default one|


## Screenshots

## Rough list and description of devices [ TODO: Do this right]

I have 3 Sonoff Basics flashed with Tasmota around the house. One of them is spliced  after the light switch for the bathroom. The other two are spliced in power strips to control a desk lamp and led strips in the pantry.

I have two Sonoff RF(flashed with Tasmota) in different parts of the house, that receive signals from RF door sensors for automation. And also RF buttons to control lights physically.

I have a LIFX Z led strip(actually, its 7 led strip in series, as a single light), that I'm using as the main source of white lightning in my room. Its not the best way, and I am looking for a better way to light up my room(I cant use normal light bulbs, because of my ceiling fan.)

I have a Zigbee2MQTT network, which uses Zigbee everything from here on is on that network:

Two Xiaomi Aqara motion sensors. To automatically turn on the light in the hallway and in the bathroom. I have a couple more but no idea of where to use them.

 Two Xiaomi Aqara temperature sensors. Mainly 'just to have them' , but I want to add them to automations in some way. One is in the bathroom and another one in my room.

4 Sylvania light bulbs. Scattered around the house, they only support dimming.

1 RGB light bulb in the porch. Its RGB so I can play with its colors along with the yard lights.

2 Sylvania RGB light strips. There are long RGB light that have many small leds in a string. I have them on the walkway that leads to my front door. These arent too reliable, as sometimes they wont respond. And its not because of bad signal strength because the RGB bulb is right by them, and it never fails.

A ceiling fan with the **Hamptom Bay Zigbee ceiling fan controller**, this fan is in my room and has an integrated LED light fixture that is very dim and has a warm color temperature. Its light makes me dizzy and its hard to see things in detail. That is why I added the led strips. -- ANYWAY: This device (the Hamptom Bay Zigbee controller) is really bad, for some reason it constanty disconnects from the Zigbee network, and sometimes takes a long time to respond to commands.
I do not recommend. Unfortunately there arent many options for Ceiling fan controllers.


## System
My HA is running with Docker in an Ubuntu Server install, which is virtualized in Proxmox, running in a Dell R710.

## Hubs
I use Zigbee2MQTT to control all of my Zigbee devices, and I'm planning on getting a Vera plus to control
Z-Wave decives. I don't have any yet... but I know I will have at least a thermostat

## Switches

I use Sonoff basics flashed with Tasmota
