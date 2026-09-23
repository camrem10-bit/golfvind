# Golf Shot Calculator v5

Created by Camilla Remstedt, 2026.

## What is included

- iPhone layout based on the supplied Layout.pdf: Shot and compact recommendation side by side, followed by elevation, wind, full result, club table and settings.
- Custom supplied green golf logo beside the title; page background #707970 with white header and footer text.
- Carry or Total (including roll) for club selection; Meters or Yards for distances.
- Elevation to green: -30 to +30 metres (approximately -33 to +33 yards); straight shots only.
- GPS wind from Open-Meteo, locality name from BigDataCloud, and live shot direction from the iPhone compass.
- Small wind-source direction arrow between Current location and Refresh; it points towards the compass direction the wind comes from and disappears if wind is calm or unavailable.
- Manual wind speed and direction as a fallback; adjustable custom carry distances.
- Home Screen PWA with offline access to the interface and saved club distances.
- SF Pro Medium (500) for ordinary text and number fields on Apple devices; stronger weights remain for headings and controls. The smallest text is 9 CSS px (approximately 6.75 pt), above the requested 6 pt floor.
- Automatic reload after a new service worker takes over, plus a visible version number (5.9) and Check for updates button in Model.

## Use live wind on iPhone

Open from your HTTPS GitHub Pages link, tap **Use my location** and allow location access. The app sends your current GPS coordinates to Open-Meteo for wind and to BigDataCloud for the place name, such as Ystad, Sweden. If the place lookup fails, coordinates are shown and weather loading continues. Point the top of the phone at your target and tap **Enable live direction** if permission is requested. The heading, relative wind and club choice then update as you turn the phone while the app is open. You do not need to set a new direction for each shot. An old direction is never reused after reopening or resuming the app. Refresh obtains a fresh GPS fix and weather data. The current wind is 10 m weather-model data, so local conditions may differ. When wind or heading is unavailable, the result says **Calm estimate • live wind pending**. Select **Manual wind** to enter local conditions yourself. Compass accuracy may be affected by magnetic interference and local magnetic declination.

## Update your existing GitHub Pages repository

Unzip the archive and upload all eight files from its root to your existing repository, replacing matching names and adding logo-green.svg. Keep Settings → Pages set to the same branch and root. The URL stays the same. Load the page while online after the update to cache the new version, then reopen the Home Screen app if an older version appears.

The interface works offline after first load. GPS weather requires a connection; the compass requires a compatible sensor and browser permission. Preferences and club distances stay in the device's local browser storage.

To update an installed Home Screen app, upload all files, open the app while online, and use **Model → Check for updates** if it does not refresh automatically. Compare the version shown there with the hosted page in Safari. The app reloads when the new offline worker takes over. Home Screen icon or name changes may require removing the Home Screen icon and adding it again on iOS; the code and saved club distances normally update without reinstalling.
