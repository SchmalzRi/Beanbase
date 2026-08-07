# Beanbase 0.1.6 – UI Alpha 7

Lokale, installierbare UI-Alpha für Beanbase.

Diese Ausgabe enthält den vollständigen Funktionsstand von **Beanbase 0.1.6 UI Alpha 7** sowie den GitHub-Pages-/PWA-Deployment-Hotfix. Der Entkalkungs-Countdown zeigt jeden Zahlenwert direkt und zentriert über seiner Einheit an.

## Datenstand

Die Daten werden lokal im Browser gespeichert. Profilbilder liegen in IndexedDB. Noch keine gemeinsame Supabase-Synchronisierung.

## Deployment-Hotfix

- Fehlende `manifest.webmanifest` und `sw.js` wiederhergestellt.
- Neuer Cache `beanbase-0.1.6-alpha.7` ersetzt ältere Beanbase-Caches.
- Navigation lädt zuerst die aktuelle GitHub-Pages-Version und nutzt den Cache nur offline.
- `.nojekyll` ergänzt, damit GitHub Pages alle Dateien unverändert ausliefert.

## GitHub Actions Deployment

Das Paket enthält `.github/workflows/static.yml` mit der aktuellen Node-24-kompatiblen GitHub-Pages-Action-Kette. Ein eventuell bereits vorhandener alter Pages-Workflow muss ersetzt werden, damit nicht mehrere Deployments parallel ausgelöst werden.
