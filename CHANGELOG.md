# Changelog – JP PageBuilder

Alle Änderungen am JP PageBuilder (Joomla 5/6, Astroid Framework). Neueste Version oben.

## 0.23.24 – 2026-10-26

- **Cookie-Banner und Popups blockieren den Builder nicht mehr:** In der Builder-Vorschau werden Cookie-Banner und
  andere Overlays jedes Herstellers automatisch ausgeblendet. Auf der Website bleiben sie unverändert.
- Ursache: Die Vorschau entfernt aus Sicherheitsgründen alle Skripte der Seite. Banner ließen sich dort deshalb nicht
  wegklicken. Erkannt werden fixierte Ebenen, die nicht zum Layout gehören; bekannte Banner (reDim CookieHint,
  Astroid, Cookiebot, Complianz, Borlabs, Usercentrics, OneTrust, Klaro) entfernt schon der Server.

## 0.23.23 – 2026-10-25

- **Versions-Info automatisch veröffentlicht:** Der Hinweis „Neue Version …“ liest jetzt eine öffentliche Datei auf
  GitHub (joomlaplates-de/pagebuilder-updates). Sie wird bei jedem Release automatisch aktualisiert, ein Hochladen von
  Hand ist nicht mehr nötig.

## 0.23.22 – 2026-10-25

- **Hinweis auf neue Versionen:** Neben der Versionsnummer im Builder und auf der Startseite der Komponente erscheint
  ein grüner Hinweis „Neue Version …“ mit Link zum Kundenbereich. Die Prüfung läuft höchstens einmal am Tag.
- Der automatische Joomla-Update-Server ist entfernt (kostenpflichtige Erweiterung, Updates werden manuell
  installiert). Bereits eingetragene Update-Quellen werden beim Installieren gelöscht.
- Die Versions-Info (`jppagebuilder.xml`) enthält nur noch Version, Kurzbeschreibung und Link zum Kundenbereich.

## 0.23.21 – 2026-10-25

- **Builder bei „Website offline“:** Die Vorschau zeigt jetzt die echte Seite, auch wenn Joomla offline geschaltet ist.
  Freigegeben wird nur der signierte Vorschau-Abruf und nur für Benutzer mit dem Recht „Offline-Zugang“.
  Besucher sehen weiter die Offline-Seite.
- Fehlt das Recht, erscheint im Builder eine klare Meldung statt einer weißen Vorschau.

## 0.23.20 – 2026-10-25

- **Termine:** dezentere Farben. Nur der Aktions-Button nutzt die Primärfarbe. Datum, Symbole, Kalender-Einträge und
  die Ansichts-Schalter sind neutral, „Heute“ ist dunkel hervorgehoben.

## 0.23.19 – 2026-10-25

- **Termine:** neue Option „Ansicht für Besucher“. Mit „Besucher können wechseln“ gibt es im Frontend einen
  Umschalter Liste / Kacheln / Monat / Tag. Die gewählte Ansicht wird im Browser gemerkt.
- Neue **Tagesansicht** mit Vor/Zurück und „Heute“. Ein Klick auf einen Tag im Monatskalender öffnet diesen Tag.
- Für Handys optimierte Umschalt- und Tagesleiste.

## 0.23.18 – 2026-10-24

- **Update-Server:** Joomla findet neue Versionen automatisch
  (`https://pagebuilder.joomlaplates.net/updates/jppagebuilder.xml`).
- Der Build erzeugt die Update-XML mit Prüfsumme automatisch.

## 0.23.17

- Neue Vorlagen „Video (datenschutzfreundlich)“ und „Karte / Anfahrt“:
  - Video spielt YouTube über youtube-nocookie.com ab, Vimeo mit „Do not track“, oder eine eigene MP4/WebM-Datei.
  - Karte nutzt Google Maps oder OpenStreetMap, mit Adresskarte und Routen-Link.
- Externe Inhalte laden erst nach Klick. „Immer laden“ lässt sich je Anbieter einschalten und widerrufen.
- Neuer Feldtyp Videodatei.

## 0.23.16

- Neue Vorlage „Bild mit Karte (Slider)“:
  - großes Bild mit überlappender Textkarte, Kartenfarben frei wählbar;
  - Animation, Pfeile, Punkte, Wischen und Autoplay.
- Termine: „Vergangene Termine ausblenden“ gilt auch im Monatskalender.
- Neuer Feldtyp Farbe.

## 0.23.15

- Neue Vorlage „Termine“: Liste, Karten oder Monatskalender mit Datum, Uhrzeit, Ort, Art, Bild und Button.
- Vergangene Termine werden automatisch ausgeblendet.
- Neue Feldtypen Datum und Uhrzeit.

## 0.23.14

- Reiter „Astroid-Widgets“ im Einfügen-Dialog vorerst ausgeblendet. Vorhandene Widgets bleiben bearbeitbar.

## 0.23.12 – 0.23.13

- Korrekturen an der Oberfläche:
  - Hintergrundtyp „Ohne Hintergrund“;
  - Werkzeug- und Pfadleiste brechen nicht mehr um;
  - breitere Auswahlfelder;
  - Farbknopf im dunklen Modus sichtbar.

## 0.23.2

- Joomla-Module ohne gespeicherte Einstellungen lassen sich einfügen und duplizieren.
- Astroid-Layout-Module ohne Layoutdatei werden ausgeblendet.
- Verwerfen entfernt auch Sperrdateien gelöschter Module.

## 0.23.1

- Vorschau auf lokalen Servern (localhost, *.test, *.local, private IPs) wieder vollständig gestaltet.

## 0.23.0

- Neuer Reiter „Joomla-Module“: vorhandene Module als unabhängige Kopie nur für die aktuelle Seite einfügen.
- Duplizieren auch für Module ohne eigenen Textinhalt.

## 0.22.8

- Sicherheits- und Kompatibilitätsprüfung für Joomla 5 und 6:
  - abgesicherter Vorschau-Schlüssel;
  - robustere Fehlerbehandlung und schnellere Frontend-Ausgabe;
  - moderne Cache-API;
  - Installationsprüfung und Installation per Kommandozeile.
