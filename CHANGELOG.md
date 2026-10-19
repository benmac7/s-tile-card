# Changelog

## 0.3.5 (beta)

- Showcase: the car graphic is smaller so it stays within the top half, below the stat pills and clear of the line, on the front and on the back of cars with no tracker.

## 0.3.4 (beta)

- **New car layout: 2 × 2 Showcase.**
  - **Front:** the top half shows the car graphic, or the car's own picture edge to edge (Tile type › Picture, or a Picture URL), like the media player's Detailed layout. Stat pills sit on top: where it is, the odometer, and today's driving (or the 12 V battery). The bottom half has the name, status, charge and range, the charge bar, pills and buttons.
  - **Back:** the map on top, with back, location and Charger buttons. Below it are the tyre pressures (low ones in rose), doors, boot, windows and locks, then the odometer, 12 V battery, software, inside temperature, range and today's driving.
  - **Cars with no location tracker:** the back shows the car instead of the map.

## 0.3.3 (beta)

- Car pictures now sit in a small-tile shape: a square with rounded corners and the tile shadow, the picture filling it edge to edge. This applies to single cars and car groups at every size.

## 0.3.2 (beta)

- **Car pictures.** Set Tile type to **Picture** to show the car's own image (an image entity on the car, such as BMW's Vehicle image, or a picture on its tracker) instead of the graphic, or paste a **Picture URL** (e.g. `/local/cars/rav4.png`). Car groups have **Use each car's own picture**; cars without one keep their graphic.
- Tested with both Toyota integrations: pytoyoda/ha_toyota and widewing/ha-toyota-na.
  - Plug-in hybrids show the battery, EV range and a Fuel pill.
  - "Charging status" text sensors now also show Plugged in.
  - The live location tracker is preferred over the parked location.
  - "Sound buzzer" works as the horn.
  - The spare tyre and "range with AC" are skipped.
- Car entity fields in the editor now have proper names.
- Car groups are called "Cars" when unnamed.

## 0.3.1 (beta)

Car tile tested against BYD, Tesla (Fleet / Teslemetry), Kia / Hyundai, Renault, Volvo, Polestar and a petrol car. The tile now finds:

- Tesla's "Charging" status sensor, so the tile shows charging, and the main Climate (not Cabin overheat protection) and the Location tracker (not Route).
- Kia and Hyundai's EV battery instead of the 12 V "Car Battery Level" (now shown as the 12 V battery), the AC charge limit (not V2L), and Estimated Charge Duration.
- Renault's Battery autonomy as range (not the charging time), Plug state, and the Hatch.
- Plugged in from a connection-status sensor (Volvo, Polestar, Renault); time to full from "charging time" and "remaining time" sensors.
- Climate on cars with no climate entity: a Climate switch (Kia, BYD "A/C on") or Start / Stop climatisation buttons (Renault, Volvo).
- BYD's Find car as the horn; flash no longer picks a "lights and horn" button.
- Polestar's read-only Charging Target Level, shown as a limit without the drag slider.
- Cars with no location tracker: pick the car's battery sensor as the entity.
- Fixes: no "driven NaN km" before history loads; the Charger button no longer shows on fuel cars; the boot isn't counted twice with the doors.
- New optional picks under Car entities: plug, time to full, climate switch, climate start and stop.

## 0.3.0 (beta)

- **New: car tile and car groups.** Location, battery or fuel and range, charging, cabin, locks, doors and tyres, and the car's buttons, in every size; backs with the battery through the day, a draggable charge limit, the week's driving and diagnostics. A Charger button opens your home charger when the car is home. Groups show each car; tap one for its detailed view.
- New graphics: SUV and pickup.
- Fan lights: the 1 × 1 back has a fan button beside the light's power and brightness.
- The Layout tab now says Category, Tile type and Layout.

## 0.2.0 (beta)

- **Every tile now flips**, and every size has a back: 1 × 1 buttons and a summary; 2 × 1 graphs and history; 2 × 2 Minimal buttons plus a graph or summary; 2 × 2 Basic and Detailed deeper graphs and timelines. Backs that already existed are unchanged.
- New backs use recorder history: hour-block timelines, the last 7 days, recent events (who locked a door, what played, when a scene ran, charging sessions, cleans and more).
- Tap now flips by default. Group tiles still do nothing when the card is tapped; their items have their own defaults: lights toggle, covers and locks toggle after asking, people flip to their map, sensors and graphs flip the card.
- EV charger start / stop shows on the 2 × 2 front whenever a charge switch or start button is found or picked.

## 0.1.1 (beta)

- Weather 2 × 2 Minimal and Basic can now flip to the five-day forecast, like Detailed: set Tap action › Flip.

## 0.1.0 (beta)

First public release.

- 31 tile types in 15 groups: lights, media, climate, sensors, weather, clock, timer, calendar, robot vacuums, people and trackers, covers, alarm panels and locks, scenes and scripts, graphs, plugs and EV chargers, sun and moon, and energy.
- Groups for lights, covers, locks, sensors, timers, people, plugs, scenes and scripts, and graphs, with per-item order, names, colours, show/hide names and states, and taps.
- 1 × 1, 2 × 1 and 2 × 2 sizes in Minimal, Basic and Detailed styles.
- A library of 90 graphics that follow each device's state.
- Flip tiles: power today, alarm history and keypad, vacuum map, climate modes and more.
- Energy from a pasted Power Flow Card Plus config first, then the Energy dashboard, then sensors you pick.
- A built-in light and dark palette, so tiles look right with any theme.
- A visual editor: choose a tile, layout and customise, with live previews.
