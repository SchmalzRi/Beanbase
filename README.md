# Beanbase 0.1.7 – UI Alpha 8

Lokale, installierbare UI-Alpha für Beanbase.

Diese Ausgabe baut ausschließlich auf **Beanbase 0.1.6 UI Alpha 7** auf und erweitert den bestehenden Funktionsstand um zwei Büro-UX-Verbesserungen. Bestehende Funktionen und lokale Daten bleiben erhalten.

## Datenstand

Die Daten werden lokal im Browser gespeichert. Profilbilder liegen in IndexedDB. Noch keine gemeinsame Supabase-Synchronisierung.

## Deployment-Hotfix

- Fehlende `manifest.webmanifest` und `sw.js` wiederhergestellt.
- Neuer Cache `beanbase-0.1.7-alpha.8` ersetzt ältere Beanbase-Caches.
- Navigation lädt zuerst die aktuelle GitHub-Pages-Version und nutzt den Cache nur offline.
- `.nojekyll` ergänzt, damit GitHub Pages alle Dateien unverändert ausliefert.

## GitHub Actions Deployment

Das Paket enthält `.github/workflows/static.yml` mit der aktuellen Node-24-kompatiblen GitHub-Pages-Action-Kette. Ein eventuell bereits vorhandener alter Pages-Workflow muss ersetzt werden, damit nicht mehrere Deployments parallel ausgelöst werden.


## UI Alpha 8
- Zahlenfelder neben den Kaffee-Bewertungsslidern markieren ihren vorhandenen Wert beim Antippen/Anklicken automatisch; direkte Zahleneingabe ersetzt damit die Vorgabe statt sie anzuhängen.
- „Fehlt im Büro“-Einträge besitzen kein versehentlich antippbares × mehr. Die komplette Zeile öffnet stattdessen einen bewussten „Mitgebracht“-Dialog.
- Beim Abschließen eines fehlenden Artikels wird ein Name erfasst, der Artikel aus der Fehl-Liste entfernt und direkt unter „Mitgebracht von Kolleg:innen“ eingetragen.
- Namen vorhandener Kolleg:innen werden im Mitgebracht-Dialog als Vorschläge angeboten.
- GitHub Pages nutzt den direkten, `.nojekyll`-unabhängigen Deployment-Workflow.
