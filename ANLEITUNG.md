# Backup-Merger für JW Library – Anleitung

Die App ist eine Web-App: eine einzige Seite (`index.html`), die komplett im Browser läuft.
Deine Backups werden **nie hochgeladen** – alles wird lokal auf dem Gerät verarbeitet.

## Am PC (Windows) – sofort, ohne Installation

Doppelklick auf `index.html`. Die App öffnet sich im Browser und funktioniert auch ohne Internet.

## Auf iPhone und iPad installieren (einmalig, ca. 10 Minuten)

Apple erlaubt es nicht, eine Datei einfach so als App zu installieren. Die App muss deshalb einmal
auf eine Webseite gestellt werden. Danach legst du sie auf den Home-Bildschirm, und sie
funktioniert **offline**. Kostenlos geht das z. B. mit GitHub Pages:

1. Auf **github.com** ein kostenloses Konto anlegen und anmelden.
2. Oben rechts **„+“ → „New repository“**. Name z. B. `backup-merger`, **Public** auswählen, **„Create repository“**.
3. Auf der neuen Seite auf **„uploading an existing file“** klicken und **alle Dateien aus diesem Ordner**
   hineinziehen (`index.html`, `sw.js`, `manifest.webmanifest`, `icon-180.png`, `icon-192.png`, `icon-512.png`,
   `LICENSE-sql.js.txt`). Unten **„Commit changes“**.
4. **„Settings“ → „Pages“** (links). Bei *Source* „Deploy from a branch“, bei *Branch* **main** und **/(root)** wählen, **„Save“**.
5. Nach 1–2 Minuten steht oben die Adresse, z. B. `https://DEINNAME.github.io/backup-merger/`.
6. Diese Adresse auf dem iPhone/iPad in **Safari** öffnen → **Teilen-Symbol → „Zum Home-Bildschirm“**.
7. Die App einmal vom Home-Bildschirm aus öffnen, solange Internet da ist. Ab dann läuft sie auch offline.

Hinweis: Auf GitHub liegt dann nur das Programm, keine persönlichen Daten.

## Benutzung

1. In JW Library auf jedem Gerät ein Backup erstellen.
2. Die Backup-Dateien auf ein Gerät bringen (AirDrop, iCloud Drive …).
3. Backup-Merger öffnen → **„Dateien auswählen“** (auf dem iPhone „Durchsuchen“ bzw. „Dateien“ wählen) → beide Backups auswählen.
4. **„Vergleichen“**. Alles, was nur in einem Backup steht, wird automatisch übernommen.
   Bei Kollisionen tippst du auf die Version, die du behalten willst (bei Notizen und Lesezeichen geht auch „Beide behalten“).
5. **„Zusammenführen & Datei erstellen“** → **„Datei speichern“** oder **„Teilen / In ‚Dateien‘ sichern“**
   (auf dem iPhone ist „Teilen“ meist der zuverlässigere Weg).
6. Die neue Datei auf **allen** Geräten mit JW Library öffnen und wiederherstellen.

## Gut zu wissen

- Die Wiederherstellung in JW Library **ersetzt** alle Daten auf dem Gerät. Originale aufheben, bis du das Ergebnis geprüft hast.
- Ein Backup speichert keine Löschungen: Was auf einem Gerät gelöscht wurde, im anderen Backup aber noch existiert, kommt zurück.
- Mehr als zwei Backups gehen auch – sie werden Schritt für Schritt zusammengeführt.
- Große Videos in Playlists machen das Backup groß (z. B. eine 1,4-GB-Bildschirmaufnahme). Auf dem iPhone kann das Speichern
  sehr großer Dateien langsam sein; am PC klappt es am zuverlässigsten.
- Benötigt iOS 16.4 oder neuer bzw. einen aktuellen Browser.
- Getestet mit JW-Library-Backups im Datenbankformat „Schema 16“. Haben die Backups unterschiedliche Formate,
  bricht der Merger mit einem Hinweis ab. Bei einem neueren Format zeigt er eine Warnung – dann das Ergebnis besonders gut prüfen.
