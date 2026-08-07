## 0.1.6 — UI Alpha 7 GitHub Pages Hotfix

- Fehlende PWA-Dateien (`manifest.webmanifest`, `sw.js`) wiederhergestellt.
- Eigenen Alpha-7-Cache ergänzt und alte Beanbase-Caches beim Aktivieren entfernt.
- Navigation auf Network-first umgestellt, damit neue GitHub-Pages-Builds nicht durch einen alten Offline-Cache verdeckt werden.
- Veraltete Versionsangaben in App und Begleitdateien korrigiert.
- Keine bestehenden Funktionen entfernt oder verändert.

## 0.1.6 — UI Alpha 7

- Entkalkungs-Countdown neu ausgerichtet: Jeder Zahlenwert steht jetzt direkt und zentriert über seiner Einheit (Wochen, Tage, Stunden).

# Beanbase 0.1.6 – UI Alpha 6

## Neu
- Das Kaffee-Setup startet bewusst nur mit **De'Longhi Vollautomat**.
- Weitere Maschinen lassen sich unter **Einstellungen → Kaffeemaschinen verwalten** ergänzen oder wieder entfernen.
- Neuer anklickbarer **Entkalkungs-Countdown** im Büro-Modul.
- Countdown-Anzeige im Schema **Wochen : Tage : Stunden**.
- Das Wartungsintervall ist frei einstellbar.
- Beim Zurücksetzen werden Name, Zeitpunkt und die zuvor verbleibende Zeit gespeichert.
- Der letzte versehentliche Reset kann rückgängig gemacht werden; die frühere Fälligkeit wird exakt wiederhergestellt.
- Kleine Wartungshistorie mit den letzten Vorgängen.

## Weiterhin lokal
Alle Wartungs- und Setupdaten bleiben in dieser Alpha im Browser und werden erst in der Connected Alpha mit Supabase geteilt.

## 0.1.6 UI Alpha 7 – GitHub Actions Deployment Hotfix

- GitHub-Pages-Workflow auf Node-24-kompatible Actions aktualisiert.
- Laufende Deployments werden nicht mehr durch neuere Workflow-Läufe abgebrochen.
- Deployment-Artefakt wird kontrolliert aus einem `_site`-Ordner erzeugt.
- Kritische PWA-Dateien werden vor dem Upload validiert.
- Keine Änderung an Beanbase-Funktionen oder lokalen Daten.
