# CAFM für iPad

Liegenschaften und Begehung, Aufträge mit Abzeichnen, Wartung & Prüfungen, Anlagen, Leitern & Tritte mit Prüfprotokollen, Schlüssel, Termine, Berichte, Historie und PDF-Export. Läuft nach der Einrichtung vollständig offline. Die 33 Liegenschaften sind bereits angelegt.

## Auf GitHub Pages veröffentlichen

1. Auf github.com ein neues Repository anlegen, z. B. `cafm` (Public).
2. „uploading an existing file“ → alle Dateien aus diesem Ordner hineinziehen → „Commit changes“.
3. Settings → Pages → Branch `main`, Ordner `/ (root)` → Save.
4. Nach 1–2 Minuten ist die App unter `https://DEINNAME.github.io/cafm/` erreichbar.

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

## Bedienung

- **Suchen** oben rechts (am PC auch Strg+K): findet Liegenschaften, Leitern/Tritte (z. B. Inventar-Nr.), Aufträge, Wartung, Anlagen, Schlüssel und Termine.
- iPad hochkant: Unter „Liegenschaften“ erst die Liste, nach Antippen das Blatt; „‹ Alle Liegenschaften“ führt zurück.

## Update

Neue Version hochladen (Dateien ersetzen, **alle** Dateien inkl. `pdf-lib.min.js`). Die App holt sich das Update beim nächsten Öffnen mit Internet. Die Daten bleiben erhalten. Beim ersten Start der neuen Version werden die Daten automatisch in den größeren Gerätespeicher (IndexedDB) übernommen.
