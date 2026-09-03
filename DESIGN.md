# Design-Leitplanken

Diese Datei ist bindend. Design-Skills (UI/UX, Vercel Guidelines und aehnliche)
duerfen als Handwerks-Checkliste dienen, nicht als Stilvorlage.

## Unveraenderlich

Farben, nur diese sechs:
  --navy #0D1A2E        Baender, Kopf, Fuss
  --paper #F6F8FB       Grundflaeche
  --card #FFFFFF        Karten
  --ink #14202F         Text, nie reines Schwarz
  --muted #5C6B7E       Nebentext, erst ab 16px
  --petrol #0E6F68      einziger Akzent
  --petrol-lite #5FD3C4 ausschliesslich auf Navy, nie auf Weiss
Signalfarben gruen/gelb/rot nur im Besetzungscheck.

Schriften: Source Serif 4 fuer Ueberschriften und Zahlen, Libre Franklin fuer
Text, Navigation und Buttons. Keine dritte Familie.

Bewegung: Einblendungen 350 ms, 14 px Versatz, Staffelung hoechstens 80 ms,
nur einmal. prefers-reduced-motion schaltet alles ab. Kein Parallax, kein
Pinning, kein Preloader.

Akzentregel 90 zu 10: Petrol nur auf Buttons, aktiven Links und Kennzahlen.
Hierarchie ueber Groesse und Weissraum, nicht ueber Farbe.

## Verboten

Farbverlaeufe, Glasmorphismus, weiche Schatten als Dekoration, ein zweiter
Akzentton, bunte Icon-Kacheln, Stockfotos, animierte Heroes, Rundungen ueber
8 px, Emoji als Gliederung.

## Erwuenscht

Kontrastpruefung nach WCAG AA, Tap-Ziele mindestens 44 px, sichtbare
Fokus-Zustaende, sauberes Abstandsraster, breite Inhalte mit eigenem
horizontalem Scrollbereich, schnelle Ladezeit ohne zusaetzliche Bibliotheken.

## Begruendung

Zielgruppe sind Geschaeftsfuehrer im Mittelstand, die 16.800 Euro an jemanden
zahlen, der solide wirkt. Die Seite ist bewusst gegen die Startup-Aesthetik der
Wettbewerber positioniert. Eine schoenere Seite, die weniger serioes wirkt,
ist ein Rueckschritt.
