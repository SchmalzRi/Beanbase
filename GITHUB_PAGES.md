# GitHub Pages aktualisieren

1. Das ZIP entpacken.
2. **Den Inhalt des entpackten Ordners** in das Beanbase-Repository kopieren. `index.html` muss direkt im veröffentlichten Repository-Ordner liegen – nicht noch eine Ebene tiefer.
3. Bestehende Dateien vollständig ersetzen, committen und pushen.
4. In GitHub unter **Settings → Pages** prüfen, dass die richtige Branch und der richtige Ordner veröffentlicht werden.
5. Nach dem Deployment die Seite einmal normal neu laden. Eine installierte PWA vollständig schließen und erneut öffnen.
6. Unter **Einstellungen → Über Beanbase** muss **Version 0.1.6-alpha.7** stehen.

Der neue Service Worker löscht ältere Beanbase-Caches automatisch. Nur falls der Browser weiterhin eine alte Version zeigt, die installierte PWA einmal entfernen und die Seite erneut öffnen.
