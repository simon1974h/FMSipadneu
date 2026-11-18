# FMS für iPad

Liegenschaften und Begehung, Aufträge mit Abzeichnen, Wartung & Prüfungen, Anlagen, Leitern & Tritte mit Prüfprotokollen, Schlüssel, Termine, Berichte, Historie und PDF-Export. Läuft nach der Einrichtung vollständig offline. Die 33 Liegenschaften sind bereits angelegt.

## Auf GitHub Pages veröffentlichen

1. Auf github.com ein neues Repository anlegen, z. B. `fms` (Public).
2. „uploading an existing file“ → alle Dateien aus diesem Ordner hineinziehen → „Commit changes“.
3. Settings → Pages → Branch `main`, Ordner `/ (root)` → Save.
4. Nach 1–2 Minuten ist die App unter `https://DEINNAME.github.io/fms/` erreichbar.

Die Programmdateien sind unter dieser Adresse öffentlich abrufbar. Deine eingegebenen Daten nicht: Sie bleiben auf dem iPad.

## Aufs iPad holen

1. Die Adresse in **Safari** öffnen.
2. Teilen-Symbol (Quadrat mit Pfeil) → „Zum Home-Bildschirm“ → „Hinzufügen“.
3. Einmal vom Home-Bildschirm öffnen, solange Internet da ist. Danach läuft die App auch offline.

## Wichtig zu den Daten

- Die Daten liegen nur in der App auf diesem iPad.
- Regelmäßig unter „Liegenschaften“ → „Sicherung speichern“ → „In Dateien sichern“ → iCloud Drive. Wird die App vom Home-Bildschirm gelöscht, sind auch ihre Daten weg.
- Daten aus der Web-Version oder vom Windows-PC übernehmen: dort „Sicherung speichern“, auf dem iPad „Sicherung einlesen“ und die Datei wählen. Umgekehrt genauso.
- Fotos und Unterschriften (Finger oder Apple Pencil) werden in der App gespeichert und sind in der Sicherung enthalten.
- Berichte, Protokolle und PDFs öffnen das Teilen-Menü: drucken, per Mail senden oder in Dateien sichern.

- Die App erinnert auf der Übersicht, wenn die letzte Sicherung älter als 7 Tage ist.
- Zusätzlich legt sie täglich und vor jedem Einlesen einer Sicherung einen **Wiederherstellungspunkt** auf dem Gerät an (ohne Fotos, die letzten 10). Zu finden unter „Liegenschaften“ → „Wiederherstellungspunkte“. Er ersetzt keine Sicherung in iCloud Drive.

## Abgleich iPad ⇄ PC über iCloud Drive

Einmalig einrichten:
1. Am PC **iCloud für Windows** installieren und iCloud Drive einschalten.
2. In iCloud Drive einen Ordner `FMS` anlegen.
3. In der FMS-App am PC unter „Liegenschaften“ → **Datenordner wählen** → diesen Ordner `iCloud Drive\FMS` wählen.

Ab dann schreibt der PC die Datei `FMS-Abgleich.json` automatisch (nach Änderungen, beim Start und wenn das Fenster wieder aktiv wird) und übernimmt, was das iPad dort abgelegt hat.

Am iPad: Übersicht → **Abgleichen** (oder unter „Liegenschaften“ → „Mit iCloud abgleichen“):
1. **Datei wählen** → iCloud Drive › FMS › `FMS-Abgleich.json`. Neues vom PC wird übernommen.
2. **In iCloud Drive speichern** → „In Dateien sichern“ → iCloud Drive › FMS → vorhandene Datei **ersetzen**.

Es geht nichts verloren: Pro Eintrag gilt der zuletzt geänderte Stand. Tabellenzeilen und Prüfprotokolle derselben Liegenschaft werden von beiden Geräten zusammengeführt. Fotos und Unterschriften reisen mit. Das Speichern am iPad zählt gleichzeitig als Sicherung.

## QR-Etiketten

- Leitern/Tritte: Liegenschaft → „Leitern & Tritte“ → **QR-Etiketten** (alle) oder im Prüfbuch einer Leiter → **QR-Etikett**.
- Anlagen und Schlüssel: in der Liste → **QR-Etiketten**, oder im Eintrag → **QR-Etikett**.
- Format wählbar (62 × 29 mm Brother, 50 × 30 mm Niimbot/Phomemo u. a., eigene Größe). **PDF zum Drucken** für AirPrint-Drucker und den PC, **Als Bild** für Bluetooth-Etikettendrucker (Bild in der App des Druckers öffnen).
- **QR scannen** oben in der App: öffnet bei Leitern direkt das Prüfbuch, sonst den Eintrag. Wichtig: in der FMS-App scannen, nicht mit der Kamera-App (die würde Safari ohne deine Daten öffnen).

## Störmeldungen per QR-Aushang

Kita-Personal, Gemeinde oder Gäste melden Defekte ohne App: QR-Code mit der Handy-Kamera scannen, kurz beschreiben, „E-Mail erstellen“ → die Mail geht an dich.

1. Liegenschaft öffnen → **Störmelde-QR** → E-Mail-Adresse für Meldungen und die Adresse der Web-App (z. B. `https://NAME.github.io/fms/`) eintragen, optional Räume (je Zeile ein Etikett).
2. Etiketten drucken und aushängen. Format ab 62 × 40 mm empfohlen, da der Code mehr Daten enthält.
3. Eingehende Meldung kopieren → **Aufträge → Aus E-Mail** → Liegenschaft, Raum, Dringlichkeit und Melder werden automatisch erkannt.

Voraussetzung: `melden.html` liegt mit auf GitHub Pages. Die E-Mail-Adresse steht im QR-Code – am besten eine Funktionsadresse verwenden.

## Verträge, Zähler, Fristen, Kosten

- **Verträge:** Wartungs-, Reinigungs- und Dienstleistungsverträge mit Laufzeit, automatischer Verlängerung und Kündigungsfrist. „Kündigen bis“ erscheint in Übersicht, Kalender und Fristen-Datei. Ist eine Frist verpasst, rechnet die App mit der verlängerten Laufzeit weiter.
- **Zähler:** Strom, Gas, Wasser, Wärme. Stände erfassen (auch per QR-Etikett am Zähler: scannen → Stand eintippen), Verbrauch je Jahr wird berechnet, Zählerwechsel wird berücksichtigt.
- **Fristen → Kalender** (Übersicht): alle Fristen der nächsten 13 Monate als Kalenderdatei mit Erinnerung (Prüfungen 14 Tage vorher). Auf dem iPad „In Kalender öffnen“, am PC in Outlook öffnen. Erneut importieren aktualisiert die Einträge.
- **Kostenübersicht** (Berichte): Auftrags- und Vertragskosten eines Jahres je Liegenschaft und Gewerk als PDF.

## Bedienung

- **Suchen** oben rechts (am PC auch Strg+K): findet Liegenschaften, Leitern/Tritte (z. B. Inventar-Nr.), Aufträge, Wartung, Anlagen, Schlüssel und Termine.
- **Merkliste:** Bei „Zuständig“, „Gemeldet von“, „Dienstleister“, „Firma“, Prüfer, Empfänger usw. erscheinen beim Antippen alle bisher verwendeten Personen und Firmen zur Auswahl. Mit × entfernst du einen Eintrag aus der Liste. Bei Terminen werden zur Firma die zuletzt verwendeten Kontaktdaten übernommen.
- iPad hochkant: Unter „Liegenschaften“ erst die Liste, nach Antippen das Blatt; „‹ Alle Liegenschaften“ führt zurück.

## Umstieg von „CAFM“ auf „FMS“ (iPad)

Der Name auf dem Home-Bildschirm wird beim Hinzufügen festgelegt und ändert sich durch ein Update nicht. Außerdem hat jede Web-App auf dem Home-Bildschirm ihren **eigenen** Speicher. Deshalb so vorgehen:

1. In der alten App (CAFM) **„Sicherung speichern“** → in iCloud Drive sichern.
2. Die neue Version hochladen (gleiches oder neues Repository) und in Safari öffnen → „Zum Home-Bildschirm“ → Name **FMS**.
3. In der neuen App **„Sicherung einlesen“** und die Datei aus Schritt 1 wählen.
4. Erst wenn alles da ist, das alte CAFM-Symbol vom Home-Bildschirm löschen.
## Update

Neue Version hochladen (Dateien ersetzen, **alle** Dateien inkl. `pdf-lib.min.js`, `qrcode.min.js`, `jsQR.min.js` und `melden.html`). Die App holt sich das Update beim nächsten Öffnen mit Internet. Die Daten bleiben erhalten. Beim ersten Start der neuen Version werden die Daten automatisch in den größeren Gerätespeicher (IndexedDB) übernommen.
