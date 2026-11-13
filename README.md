# Zugwerk

Schachpartien verstehen: PGN einfügen, Züge nachspielen und mit Stockfish 19 Lite analysieren. Für Handy und Desktop.

## Funktionen
- Lokale Engine-Analyse mit Bewertungsbalken, Varianten und Zugbewertungen.
- Eigener Genauigkeitsindex und eine lokale Eröffnungsreferenz.
- Öffentliche Chess.com-Partien importieren und Endspiele über Lichess prüfen.
- Optionale KI-Erklärungen über ein vorhandenes lokales Ollama-Modell.

## Grenzen
Die Bewertungen sind eigene Regeln und nicht identisch mit Chess.com. Begrenzte Suchzeit kann Fehler übersehen. Online-Eröffnungsstatistiken sind noch nicht freigeschaltet. Ollama-Erklärungen können falsch sein; echte Modellqualität und iPhone/Safari sind noch nicht vollständig getestet.

## Datenschutz
PGN und Engine-Analyse bleiben auf dem Gerät. Online-Abfragen erfolgen nur per Klick: Dabei erhält Chess.com den eingegebenen Benutzernamen, Lichess die gewählte Stellung und ein verbundenes Ollama-Modell die ausgewählten Engine-Fakten. Kein Login und keine Analyse-Telemetrie.

## Starten
npm ci
npm run dev

Produktionsbuild: npm run build
Tests: npm test

## Lizenzen
App: GPL-3.0-or-later. Stockfish.js: GPLv3. chess.js: BSD-2-Clause. Eröffnungsdaten: CC0. Figuren von Colin M. L. Burnett: GPLv2 oder neuer. Twemoji-Grafiken: CC BY 4.0. Icons: Phosphor (MIT). Schrift: Nunito (SIL OFL 1.1). Lizenztexte, Quellen und passende Engine-Buildmaterialien sind enthalten. Keine Verbindung zu oder Empfehlung durch Chess.com oder Lichess.
