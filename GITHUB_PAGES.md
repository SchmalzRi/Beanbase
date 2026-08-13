# GitHub Pages aktualisieren

## Wichtig: alten Workflow ersetzen

Der vorherige GitHub-Pages-Workflow verwendet veraltete Node-20-Actions. Dieses Paket enthält deshalb einen neuen Workflow unter:

`.github/workflows/static.yml`

1. Das ZIP entpacken.
2. Den **Inhalt** des entpackten Ordners in das Beanbase-Repository kopieren. `index.html` muss direkt im Repository-Stamm liegen.
3. In `.github/workflows/` den bisherigen Pages-Workflow löschen oder durch die enthaltene `static.yml` ersetzen. Es darf nur ein Beanbase-Pages-Workflow aktiv bleiben.
4. Alle Änderungen in **einem Commit** auf `main` oder `master` hochladen.
5. Unter **Settings → Pages → Build and deployment → Source** muss **GitHub Actions** ausgewählt sein.
6. Unter **Actions** den Lauf **Deploy Beanbase to GitHub Pages** öffnen. `build` und danach `deploy` müssen grün werden.
7. Anschließend die Webseite neu laden. Eine installierte PWA vollständig schließen und erneut öffnen.
8. Unter **Einstellungen → Über Beanbase** muss **Version 0.1.7-alpha.8** stehen.

## Was der Workflow korrigiert

- Node-24-kompatible Actions: `checkout@v6`, `configure-pages@v6`, `upload-pages-artifact@v5`, `deploy-pages@v5`
- `cancel-in-progress: false`, damit ein laufendes Deployment nicht durch einen weiteren Upload abgebrochen wird
- Sauberes `_site`-Artefakt mit `index.html` direkt auf oberster Ebene
- Explizite Prüfung der drei kritischen Dateien vor dem Deployment

Der Service Worker löscht ältere Beanbase-Caches automatisch. Nur falls der Browser weiterhin eine alte Version zeigt, die installierte PWA einmal entfernen und die Seite erneut öffnen.
