# Zugwerk

Schachpartien verstehen: PGN einfügen, Züge nachspielen und mit Stockfish 19 Lite analysieren. Für Handy und Desktop.

## Funktionen
- Lokale Engine-Analyse mit Bewertungsbalken, Varianten und Zugbewertungen.
- Eigener Genauigkeitsindex und eine lokale Eröffnungsreferenz.
- Öffentliche Chess.com-Partien importieren und Endspiele über Lichess prüfen.
- Optionale KI-Erklärungen über lokales Ollama oder die kostenlose Cloud-KI Pollinations, nach ausdrücklichem Einschalten ab 16. Überflug der engine-markierten Stellen, auf Wunsch alle Züge in Zehnerpaketen.

## Grenzen
Die Bewertungen sind eigene Regeln und nicht identisch mit Chess.com. Begrenzte Suchzeit kann Fehler übersehen. Online-Eröffnungsstatistiken sind noch nicht freigeschaltet. KI-Erklärungen können falsch, knapp oder holprig sein und sind nicht engine-geprüft. Maßgeblich bleibt Stockfish. Pollinations erlaubt aktuell eine Anfrage alle 30 Sekunden pro öffentlicher IP und garantiert keine Verfügbarkeit. iPhone/Safari sind noch nicht vollständig getestet.

## Datenschutz
Die Schachberechnung erfolgt auf deinem Gerät. Online-Abfragen erfolgen nur per Klick: Chess.com erhält beim Import den eingegebenen Benutzernamen, Lichess bei einer Abfrage die gewählte Stellung. Ein verbundenes Ollama-Modell erhält bei einer KI-Erklärung die ausgewählten Engine-Fakten.

Die Cloud-KI ist standardmäßig aus. Wenn du sie einschaltest, werden beim Klick auf "KI-Erklärung", "Überflug" oder "Alle Züge erklären" die jeweiligen Züge und Engine-Fakten an text.pollinations.ai gesendet: Zugnotation, Einstufung, Bewertung, empfohlener Zug, mögliche Fortsetzung und gegebenenfalls der Markierungsgrund. Pollinations sieht dabei auch deine IP-Adresse. Spielernamen und PGN-Kopfdaten werden nicht gesendet. Der Dienst ist ab 16; seine Datenschutzerklärung steht unter https://pollinations.ai/privacy. Zugwerk selbst erfordert keinen Login und sendet keine Analyse-Telemetrie.

## Starten
npm ci
npm run dev

Produktionsbuild: npm run build
Tests: npm test

## Lizenzen
App: GPL-3.0-or-later. Stockfish.js: GPLv3. chess.js: BSD-2-Clause. Eröffnungsdaten: CC0. Figuren von Colin M. L. Burnett: GPLv2 oder neuer. Twemoji-Grafiken: CC BY 4.0. Icons: Phosphor (MIT). Schrift: Nunito (SIL OFL 1.1). Lizenztexte, Quellen und passende Engine-Buildmaterialien sind enthalten. Keine Verbindung zu oder Empfehlung durch Chess.com oder Lichess.
