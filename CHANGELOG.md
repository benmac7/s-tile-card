# Changelog

## 0.2.0 (beta)

Everything since 0.1.0, in one release.

### New tiles
- **Cars** (Category › Cars). One tile for the whole car: where it is, battery or fuel and range, charging, the cabin, locks, doors and tyres, and the buttons the car offers, in every size. Everything is found on the car's device and can be picked under Customise › Content › Car entities.
  - Tile types: car, SUV, pickup, or **Picture** (the car's own image, or a Picture URL), shown as a small rounded square.
  - **2 × 2 Showcase:** the car or its picture across the top with stat pills (location, odometer, today's driving), with charge, range, pills and buttons below. The back has the map on top, and tyres, doors, locks, odometer, 12 V battery and software below.
  - Backs: the battery through the day, a **draggable charge limit**, the week's driving and diagnostics (tyres, doors, boot, windows, odometer, 12 V battery, software, last charge).
  - **Plug-in hybrids:** the battery leads, and the fuel level and fuel range show as a second, thinner bar under it on every front (a line on the 1 × 1 Detailed).
  - Charge and fuel colours you can change (rose under 20 %, sand under 50 %, sage above by default), and extra pills for any sensor.
  - A **Charger** button opens your home charger's device page when the car is home. Pick the charger by its device or by any of its entities; otherwise it is found from your EV charger integration.
  - **Car groups** (2 × 1 and 2 × 2): each car with its charge and where it is. Tap a car for its detailed view.
  - Tested with BYD, Tesla (Fleet / Teslemetry), Kia / Hyundai, Toyota (ha_toyota and ha-toyota-na), Renault, Volvo and Polestar, plus petrol cars and plug-in hybrids.
- **Air** (Category › Air).
  - **Fans:** ceiling, pedestal and tower, with trails that show the speed. A light on the same device joins in with its own button and brightness.
  - **Air purifiers:** the air on a ring (green good, sand fair, rose poor), PM2.5 or AQI, filter life with a badge when it is due, fan levels, the modes and a child lock.
  - **Humidifiers:** the tank shows the water left and mist rises while it runs. Humidity is shown against the target, with a target slider and the modes.

### Every tile flips
- Every size has a back: 1 × 1 buttons and a summary; 2 × 1 graphs and history; 2 × 2 Minimal buttons plus a graph or summary; 2 × 2 Basic and Detailed deeper graphs and timelines.
- The new backs use recorder history: hour-block timelines, the last 7 days and recent events (who locked a door, what played, when a scene ran, charging sessions, cleans and more).
- Weather 2 × 2 Minimal and Basic flip to the five-day forecast.
- Tap flips by default, and new cards animate the flip. Group tiles do nothing when the card is tapped; their items have their own defaults: lights toggle, covers and locks toggle after asking, people flip to their map, sensors and graphs flip the card, and cars show that car.

### Better
- **The device decides the tile.** Picking a device looks at the whole device first: cars, EV chargers, vacuums, alarms, purifiers, fans and humidifiers are recognised before any single entity on them.
- **Maps:** a person or car without GPS (a router or Bluetooth tracker) shows in its zone with its picture.
- **Show the icon** works on every 1 × 1 Detailed tile and on the 2 × 2 tracker map tile.
- Fan lights: the 1 × 1 back has a fan button beside the light's power and brightness.
- EV charger start / stop shows on the 2 × 2 front whenever a charge switch or start button is found or picked.
- The Layout tab says Category, Tile type and Layout.
- The editor shows the entities you picked in their fields.

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
