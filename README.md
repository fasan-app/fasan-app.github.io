# fasan-app.github.io

Wurzel der Fasan-Seiten. Hier liegt nur, was an der Wurzel der Adresse liegen muss:

- `.well-known/assetlinks.json`: Android App Links für Fasan Split (`app.fasan.split`). Erster Fingerabdruck: Release-Schlüssel
  (Secret `FASAN_KEYSTORE_B64` im Repo Fasan-Split), zweiter: öffentlicher Testschlüssel `ci/fasan-split-test.p12`, nur
  für den Übergang, später entfernen. Doku: developer.android.com/training/app-links/verify-android-applinks
- `.nojekyll`: sonst veröffentlicht GitHub Pages keine Ordner mit Punkt am Anfang.
- `index.html`: leitet auf die Web-App von Fasan Split weiter.

Die Web-App selbst baut das Repo Fasan-Split (`.github/workflows/web.yml`). Lizenz MPL-2.0.
