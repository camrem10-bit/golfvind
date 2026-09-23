# Golf Shot Calculator v5

Created by Camilla Remstedt, 2026.

## What is included

- iPhone layout based on the supplied Layout.pdf: Shot and compact recommendation side by side, followed by elevation, wind, full result, club table and settings.
- Custom supplied green golf logo beside the title; page background #707970 with white header and footer text.
- Carry or Total (including roll) for club selection; Meters or Yards for distances.
- Elevation to green: -30 to +30 metres (approximately -33 to +33 yards); straight shots only.
- GPS wind from Open-Meteo, locality name from BigDataCloud, and shot direction locked from the iPhone compass.
- Manual wind speed and direction as a fallback; adjustable custom carry distances.
- Home Screen PWA with offline access to the interface and saved club distances.

## Use live wind on iPhone

Open from your HTTPS GitHub Pages link, tap **Use my location** and allow location access. The app sends your current GPS coordinates to Open-Meteo for wind and to BigDataCloud for the place name, such as Ystad, Sweden. If the place lookup fails, coordinates are shown and weather loading continues. Point the top of the phone at your target, then tap **Set direction from phone** and grant orientation permission. Refresh obtains a fresh GPS fix and live wind; lock a new direction for each shot. The current wind is 10 m weather-model data, so local conditions may differ. When wind or heading is unavailable, the result says **Calm estimate • live wind pending**. Select **Manual wind** to enter local conditions yourself. Compass accuracy may be affected by magnetic interference and local magnetic declination.

## Update your existing GitHub Pages repository

Unzip the archive and upload all eight files from its root to your existing repository, replacing matching names and adding logo-green.svg. Keep Settings → Pages set to the same branch and root. The URL stays the same. Load the page while online after the update to cache the new version, then reopen the Home Screen app if an older version appears.

The interface works offline after first load. GPS weather requires a connection; the compass requires a compatible sensor and browser permission. Preferences and club distances stay in the device's local browser storage.
