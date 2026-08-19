# fermasster0-rgb.github.io

Die Wurzel dieser GitHub-Pages-Domain. Sie liegt hier aus einem technischen
Grund, nicht als eigene Seite:

**Digital Asset Links** (`.well-known/assetlinks.json`) verknüpfen die Android-App
mit dieser Domain. Android prüft diese Datei ausschließlich in der Wurzel einer
Domain — ein Unterordner wie `/wild-spot/` reicht nicht. Ohne sie zeigt die App
eine Browser-Adressleiste und wirkt nicht wie eine App.

Die Startseite leitet deshalb einfach auf das eigentliche Projekt weiter:
https://fermasster0-rgb.github.io/wild-spot/

## Warum die Datei .nojekyll hier liegt

GitHub Pages schickt jede Seite durch Jekyll, und Jekyll überspringt alles, was
mit einem Punkt beginnt — also ausgerechnet `.well-known/`. Die Asset-Links-Datei
war dadurch nicht abrufbar (404), obwohl sie im Repo lag. Die leere Datei
`.nojekyll` schaltet Jekyll ab; seitdem wird der Ordner ausgeliefert.
