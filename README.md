# SA-MP Biker Delivery Event

A PAWN delivery event module for SA-MP biker factions.

The event spawns a Flatbed vehicle at a random location. Biker faction members must find it, take control of the vehicle, and deliver the cargo to their faction base before the event timer ends.

## Features

* Random Flatbed spawn points
* Support for multiple biker factions
* Map icon tracking for faction members
* Delivery checkpoints
* Event timer and cooldown system
* Event reminders
* Vehicle destruction handling
* Faction and player reward logic
* Test commands for development

## Requirements

* SA-MP server
* PAWN compiler
* Existing gamemode or filterscript
* Vehicle include: `a_vehicles`

## Installation

1. Download `biker_event.pwn`.
2. Add the file to your SA-MP server project.
3. Connect the event logic to your gamemode or filterscript.
4. Implement reward functions for your own server economy.
5. Compile the project.
6. Start or restart the server.

## Usage

The module starts the event automatically after cooldown.

Default event settings:

* Event duration: 30 minutes
* Event cooldown: 90 minutes + random delay
* Event vehicle: Flatbed
* Supported factions: 10 biker factions

## Development Commands

These commands are included for testing:

* `/makeleader` — set test faction
* `/start` — manually start event
* `/tpcar` — teleport to event vehicle
* `/tpbar` — teleport to faction delivery point

Remove or protect these commands before using the module on a live server.

## Notes

* Reward functions are placeholders and must be connected to your server systems.
* Some coordinates and faction names are server-specific.
* Check the code before using it on a production server.
