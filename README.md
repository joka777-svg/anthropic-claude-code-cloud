# Kunden & Fahrtenbuch

Web-App für iPad und iPhone. Sie verwaltet Kunden, ein Fahrtenbuch und Dokumente wie Angebote, Rechnungen und Fotos. Sie funktioniert ohne Anmeldung und auch offline.

## Funktionen

- **Fahrtenbuch:** Datum, Start, Ziel, Kunde/Baustelle, Anlass, Kilometer und Art (geschäftlich, Arbeitsweg, privat).
  - km-Stände sind optional. Ab einem Anfangs-km-Stand rechnet die App sie automatisch weiter.
  - „Speichern + Rückfahrt“ trägt die Rückfahrt mit vertauschtem Start und Ziel vor.
  - Summen und Kilometerpauschale gibt es pro Monat oder Jahr.
  - Excel-Bericht für den Steuerberater mit den Blättern Übersicht, Fahrten und Kilometer je Kunde.
- **Kunden:** Adresse, Telefon, E-Mail, Baustellen, Maße/Aufmaß, Notizen und Termine. Dazu die Dokumente und alle Fahrten des Kunden.
- **Dokumente:** Dateien in jedem Format, mit Art, Nummer, Datum, Betrag und Status (offen, bezahlt …).
- **Import:** Excel (.xlsx/.xls), .ods, CSV/TSV/TXT, Markdown-Tabellen, JSON, vCard (.vcf) und Sicherungsdateien. Die Spalten werden automatisch zugeordnet.
- **Export:** CSV, Excel und eine Komplett-Sicherung als JSON. Die Dateien gehen über das Teilen-Menü (Dateien, AirDrop, Mail).

## Daten

Alle Daten liegen **nur auf dem Gerät**, im Speicher von Safari für diese App. Mach regelmäßig eine Sicherung unter „Import / Export“ → „Komplett-Sicherung“ und speichere sie in „Dateien“ → iCloud Drive. Die App erinnert dich alle 14 Tage daran.

## Auf das iPad bringen

1. In GitHub: **Settings → Pages → Source: „GitHub Actions“** einstellen.
2. Unter **Actions → „Web-App veröffentlichen“ → Run workflow** den Workflow starten.
3. Die angezeigte Adresse auf dem iPad in **Safari** öffnen.
4. **Teilen → „Zum Home-Bildschirm“** wählen.

## Entwicklung

Die App liegt in `www/`. Sie besteht aus reinem HTML, CSS und JavaScript und braucht keinen Build-Schritt. Zum Testen startest du einen lokalen Server: `python3 -m http.server -d www`.
