# vertriebskoepfe-website

Statische Website der Personalberatung Vertriebsköpfe — gleiche Bauweise wie
`leadsimply-website`: kein Framework, kein Build-Schritt, Unterseiten als Ordner
mit eigener `index.html`, damit die Adressen ohne `.html` auskommen.

## Struktur

```
index.html               Startseite
besetzungscheck/         → vertriebskoepfe.de/besetzungscheck
impressum/               → Vorlage, vor dem Livegang ausfüllen
datenschutz/             → Gerüst, vor dem Livegang ausfüllen und prüfen lassen
404.html                 Fehlerseite
favicon.svg              VK-Signet
og-image.png             Vorschaubild beim Teilen (1200 × 630)
CNAME                    vertriebskoepfe.de
robots.txt, sitemap.xml  für Suchmaschinen
.nojekyll                verhindert die Jekyll-Verarbeitung
.github/workflows/       optional: Übertragung auf den STRATO-Webspace
```

## Einrichtung

1. Repository `vertriebskoepfe-website` anlegen, öffentlich, wie bei leadsimply.
2. **Inhalt** dieses Ordners hochladen — nicht den Ordner selbst. `index.html`
   muss in der obersten Ebene liegen.
3. `Settings → Pages`: Source `Deploy from a branch`, Branch `main`, Ordner `/ (root)`.
4. `Custom domain` auf `vertriebskoepfe.de` setzen.
5. DNS bei STRATO: vier A-Einträge auf 185.199.108–111.153 für die nackte Domain,
   ein CNAME für `www` auf `stefanbruendl77.github.io`.
   **MX- und TXT-Einträge unangetastet lassen** — dort hängt die E-Mail.
6. Sobald GitHub grün meldet: `Enforce HTTPS` aktivieren.

## Pflichtliste vor dem Livegang

- [ ] `noindex` entfernen — steht im Kopfbereich von `index.html`,
      `besetzungscheck/index.html`, `impressum/index.html`, `datenschutz/index.html`
- [ ] Telefonnummer ersetzen: `tel:+49XXXXXXXXX` und der sichtbare Text `040 XXX XX XX`
- [ ] Kalenderlink hinterlegen
- [ ] Porträtfoto einsetzen (Platzhalterkasten im Abschnitt „Wer das macht")
- [ ] Impressum vollständig ausfüllen
- [ ] Datenschutzerklärung ausformulieren und prüfen lassen —
      inklusive Hosting-Abschnitt (GitHub in den USA oder STRATO in Deutschland)
- [ ] Belege-Abschnitt auf der Startseite füllen oder entfernen
- [ ] Auf dem Handy durchklicken, besonders den Besetzungscheck

## Änderungen

Direkt auf github.com bearbeiten oder lokal per Git. Jeder Commit auf `main`
veröffentlicht die neue Fassung; nach ein bis zwei Minuten ist sie online.

## Weitere Stellenanzeigen

Jede Stelle wird ein eigener Ordner mit `index.html`, zum Beispiel
`stellen/gebietsverkaufsleitung-nord/`. Vorlage folgt.
