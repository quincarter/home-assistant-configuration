# HA Configuration

Hello There! I have been getting requests to expose my dashboards to the public for viewing. Well in this repo you will find my [raw-configuration](./raw-configuration.yaml) with a bunch of stuff ripped out of it for PII reasons.

## Quick Notes

The top 25% of the dashboard consists of very useful information for our household to show things that need to be acted on, or information about what is happening in the house (doors unlocked/opened, media playing, Vacuum running, Washer running, etc).

![top-part](./screenshots/top-of-dash.png)

Below that, Rooms become the basis of this dashboard. It gives a great virtual feel of being in the room itself. Each set of rooms is contained by a floor. 

![rooms](./screenshots/rooms.png)

I have grouped lights and switches using the `Helpers > Group > Light Group` with like `All Main Floor Lights` or `All Basement Lights`. Then Each room has a light group itself (very much like google/alexa handle area grouping - I tried to mimic that) so `Office Lights` would be a group of all the lights in the office. Or `Kitchen Lights` would be the 4 lights we have in the kitchen.

![living-room](./screenshots/living-room.png)

The horizontal flow at the bottom of the page is part of the [Bubble Card](./README.md#bubble-card) integration. Each room can potentially have a motion sensor attached to it so that the buttons will rearrange themselves when they are occupied.

## Live Demo

Click [here](https://photos.app.goo.gl/ARhj3e4pBj2PvSt68)(Google Photos Album) to see the Live Demo

## Integrations/Addons

### Addons

- [Zwave JS UI](https://github.com/zwave-js/zwave-js-ui)
  - All of my Switches are Zooz 800 switches
- [Zigbee2MQTT](https://www.zigbee2mqtt.io/)
  - I run all of my philips hue bulbs on my ZBT-1 stick through Zigbee2MQTT
- [Music Assistant Server](https://github.com/music-assistant/server)

### HACS Frontend Integrations

#### Mushroom

![Overview](https://user-images.githubusercontent.com/5878303/152332130-760cf616-5c40-4825-a482-bb8f1f0f5251.png)

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=piitaya&repository=lovelace-mushroom)

#### Bubble Card

![readme-images-bubble-card](https://github.com/Clooos/Bubble-Card/assets/36499953/c763bdad-ce71-46b0-aa9e-4ff0017072fe)

[![Open Bubble Card on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=clooos&repository=Bubble-Card&category=frontend)

#### Mini Media Player

![Preview Image](https://user-images.githubusercontent.com/457678/47517460-9282d600-d888-11e8-9705-cf9ec3698c3c.png)

[![Open Mini Media Player on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=kalkih&repository=mini-media-player&category=frontend)

#### Atomic Calendar Revive

| Event Mode                                                                                                                             | Calendar Mode                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="https://raw.githubusercontent.com/totaldebug/atomic-calendar-revive/master/.github/img/event-mode-example.png" width="300"/> | <img src="https://raw.githubusercontent.com/totaldebug/atomic-calendar-revive/master/.github/img/calendar-mode-allday.png" width="300"/> |
| <img src="https://raw.githubusercontent.com/totaldebug/atomic-calendar-revive/master/.github/img/event-mode-no-date.png" width="300"/> | <img src="https://raw.githubusercontent.com/totaldebug/atomic-calendar-revive/master/.github/img/calendar-mode-today.png" width="300"/>  |

[![Open Atomic Calendar Revive on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=totaldebug&repository=atomic-calendar-revive&category=frontend)

#### Timer Bar Card (not pictured in videos)

![timer bar card](./screenshots/timer-bar-card.png)

[![Open Bubble Card on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=rianadon&repository=timer-bar-card&category=frontend)

#### Universal Remote

![universal remote](./screenshots/universal-remote.png)
[![Open Universal Remote (Android TV Card) on Home assitant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?repository=android-tv-card&owner=Nerwyn&category=Plugin)

#### Time Picker Card

![time picker card](./screenshots/time-picker.png)
[![Open Time Picker Card on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?repository=lovelace-time-picker-card&owner=GeorgeSG&category=frontend)

#### Trash Card (Not Pictured in my videos)

![trash card](./screenshots/trash-card.png)

[![Open Trash Card on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?repository=hassio-trash-card&owner=idaho&category=frontend)

### HACS Integrations

#### WebRTC Camera

[![Open WebRTC Camera on Home Assistant Community Store (HACS).](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?repository=WebRTC&owner=AlexxIT&category=integration)

#### GE Home Appliances (Custom Source)

Entities card:

![Entities](https://raw.githubusercontent.com/simbaja/ha_components/master/img/appliance_entities.png)

Fridge Controls:

![Fridge controls](https://raw.githubusercontent.com/simbaja/ha_components/master/img/fridge_control.png)

Oven Controls:

![Fridge controls](https://raw.githubusercontent.com/simbaja/ha_components/master/img/oven_controls.png)

A/C Controls:

![A/C controls](https://raw.githubusercontent.com/simbaja/ha_components/master/img/ac_controls.png)

For installation - Please follow directions [here](https://hacs.xyz/docs/faq/custom_repositories/), and use https://github.com/simbaja/ha_gehome as the repository URL.

#### Keymaster (Not pictured in videos)

![keymaster](./screenshots/keymaster.png)

Please see their [wiki](https://github.com/FutureTense/keymaster/wiki) for setup instructions.

#### Google Keep Sync (for todo lists/shopping lists)

This is a direct integration with Home Assistant's built-in todos. Please read [all the docs](https://github.com/watkins-matt/home-assistant-google-keep-sync/blob/main/README.md) for setup instructions.

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=watkins-matt&repository=home-assistant-google-keep-sync&category=integration)
