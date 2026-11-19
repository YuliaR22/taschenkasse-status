# Zahlungsstatus-Abgleich

Dieses Repository hostet die statische Web-Ansicht für den selbstständigen Abgleich von Zahlungseingängen über GitHub Pages.

## Datenschutz & Funktionsweise (Zero-Knowledge)
* **Keine Klarnamen:** In diesem Repository und in der `status.json` werden zu keinem Zeitpunkt Namen oder personenbezogene Daten im Klartext gespeichert.
* **Lokale Prüfung:** Eingaben werden ausschließlich lokal im Browser des Endgeräts normalisiert, mit einem Salt kombiniert und per `SHA-256` gehasht.
* **Abgleich:** Der berechnete Hash wird lokal gegen die Liste in `status.json` geprüft. Es werden keine Eingaben an einen Server übertragen.

## Dateien
* `index.html` – Statische, mobile-optimierte Benutzeroberfläche für die Statusabfrage.
* `status.json` – Automatisch aktualisierte Datei mit Zeitstempel und gehashten Zahlungsstatus-Einträgen.
