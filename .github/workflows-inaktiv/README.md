# Inaktive Workflows

`deploy-strato.yml` liegt bewusst hier statt unter `.github/workflows/`.

**Warum:** In diesem Ordner führt GitHub den Workflow nicht aus. Solange die
Seite über GitHub Pages läuft, wäre der FTP-Upload zu STRATO doppelt — und
ohne hinterlegte Secrets würde er bei jedem Push als fehlgeschlagene Action
erscheinen.

**Aktivieren:** Datei nach `.github/workflows/` zurückschieben, dann die drei
Secrets im Repository hinterlegen (Settings → Secrets and variables → Actions):
`FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`.

Zum Verschieben braucht der verwendete GitHub-Token den Berechtigungsumfang
`workflow` — sonst lehnt GitHub den Push ab. Alternativ die Datei direkt über
die GitHub-Weboberfläche anlegen.

**Wichtig:** GitHub Pages und STRATO gleichzeitig zu betreiben ergibt keinen
Sinn — beide beanspruchen dieselbe Domain. Vor dem Aktivieren die `CNAME`-Datei
und die Pages-Einstellung entsprechend anpassen.
