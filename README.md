# FCAE Auswertung – GitHub Pages

Statische Seite zur Auswertung von `log.txt`-Dateien der CPC-Effizienzmessung.
Läuft komplett im Browser (JavaScript), es wird nichts hochgeladen oder gespeichert.

## Veröffentlichen auf GitHub Pages

1. Neues (oder bestehendes) Repository auf GitHub anlegen.
2. `index.html` in das Repository-Root legen (per Weboberfläche hochladen oder committen/pushen).
3. Im Repo: **Settings → Pages**.
4. Unter „Build and deployment“ → Source: **Deploy from a branch** wählen.
5. Branch: `main` (oder `master`), Ordner: `/ (root)` → **Save**.
6. Nach ca. 1 Minute ist die Seite erreichbar unter:
   `https://<dein-github-nutzername>.github.io/<repo-name>/`

## Nutzung

1. `log.txt` per Drag&Drop auf die Fläche ziehen oder anklicken und auswählen.
2. Fluss des Referenzgeräts [LPM] sowie die k-Faktoren für DUT1–3 eingeben.
3. Auf „Berechnen“ klicken.
4. Tabelle mit den 5 Blockkonzentrationen (REF, DUT1, DUT2, DUT3) sowie Mittelwert erscheint.

## Anpassen

Die gesamte Logik (Parsing, Formeln, Darstellung) steckt in `index.html` –
keine Build-Tools, keine Abhängigkeiten außer zwei Google Fonts.
