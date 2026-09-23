# Golf Shot Calculator v4

Created by Camilla Remstedt, 2026.

## New in v4
- GPS-based live wind using your iPhone location.
- Current 10 m wind speed and meteorological wind direction from Open-Meteo.
- Shot direction can be captured from the iPhone compass:
  point the top of the iPhone at the target and tap **Set direction from phone**.
- Live wind is converted into headwind/tailwind and left/right crosswind components relative to the shot.
- Manual wind mode remains available as a fallback.
- Elevation control from -10 m to +10 m.
- Carry / Including roll.
- Metres / Yards.
- Straight / Fade.
- Custom club carry distances stored locally.

## iPhone permissions
The first time you use live mode, iOS may ask for:
- Location access
- Motion & Orientation / compass access

These permissions are required for GPS wind and phone-heading shot direction.

## Weather source
Live wind is requested from Open-Meteo using:
- wind_speed_10m
- wind_direction_10m
- m/s wind units

Weather-model wind can differ from the wind experienced at the exact ball position because of trees, terrain, buildings and gusts.

## Update existing GitHub Pages
Upload/replace these files in the existing repository:
- index.html
- manifest.webmanifest
- sw.js
- icon-180.png
- icon-192.png
- icon-512.png
- README.md

Keep the same GitHub Pages settings and URL.
