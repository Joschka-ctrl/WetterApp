# ☀️ Sonnenwetter – Die Wetter-App mit 100 % Sonnengarantie

Zeigt immer gutes Wetter. Immer. Regen: 0 %.

## Direkt nutzen (ohne Installation)
`index.html` im Browser öffnen – fertig.

## Als App aufs Handy (PWA)
1. Läuft bereits über GitHub Pages: **https://joschka-ctrl.github.io/WetterApp/** (
   oder jeden anderen Webserver mit https).
2. Die Seite auf dem Handy öffnen.
3. **Android (Chrome):** Menü ⋮ → „App installieren“ / „Zum Startbildschirm“.
   **iPhone (Safari):** Teilen-Symbol → „Zum Home-Bildschirm“.
Danach läuft sie wie eine echte App, auch offline.

## Als Desktop-Programm (Windows .exe / Mac .dmg / Linux AppImage)
Voraussetzung: Node.js (https://nodejs.org)

```bash
npm install
npm start          # zum Testen
npm run build:win  # erzeugt dist/Sonnenwetter Setup 2.0.0.exe + portable .exe
npm run build:mac  # dist/Sonnenwetter-2.0.0.dmg (nur auf einem Mac)
npm run build:linux
```

Die fertigen Installer liegen danach im Ordner `dist/`.

## Was neu ist (v2)
- Große „Heute“-Karte mit Regen 0 %, UV, Wind, Luftfeuchte, Sonnenstunden, Sonnenauf-/-untergang
- 7-Tage-Übersicht mit Nachttemperatur, Spruch des Tages und Markierung für „Heute“
- Gleicher Ort + gleicher Tag = gleiches Wetter (statt bei jedem Klick neu gewürfelt)
- Standort wird gespeichert, Enter-Taste funktioniert
- Responsive fürs Handy, installierbar als PWA, offline-fähig
- Electron-Wrapper für Desktop-Installer
