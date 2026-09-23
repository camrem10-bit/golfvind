# Golfvind PWA v1

Detta är en installerbar webbapp (PWA) för iPhone.

## Viktigt
För att "Lägg till på hemskärmen" och offline-funktionen ska fungera som en riktig PWA måste filerna ligga på en vanlig HTTPS-webbadress. Att bara öppna index.html direkt från appen Filer räcker inte för service worker/offline-läget.

## Innehåll
- index.html
- manifest.webmanifest
- sw.js
- appikoner 180, 192 och 512 px

## Installation på iPhone när sidan ligger online
1. Öppna Golfvind-adressen i Safari.
2. Tryck på Dela.
3. Välj "Lägg till på hemskärmen".
4. Tryck "Lägg till".
5. Golfvind visas som en egen appikon och öppnas utan Safaris vanliga gränssnitt.

## Funktioner
- Avstånd till flagga
- Vind 0–30 m/s
- Dragbar vindpil 0–359°
- Rak eller fade
- Rekommenderad klubba
- Carry och total längd
- Skillnad mot flaggan
- Uppskattad sidled
- Egna carry-längder sparas lokalt
- Offline-stöd efter första laddningen

## Vindriktning
- 0° = medvind
- 90° = vind från vänster
- 180° = motvind
- 270° = vind från höger
