# Scores

Arrangements und Kompositionen mit MuseScore4 im .mscx Format, die mit git verwaltet werden.


## Initialisierung

In ein Verzeichnis deiner Wahl wechseln, in das du das Repo klonen möchtest.

```
git clone https://github.com/pilarcoordinates/Scores.git 
```

## Arbeitsablauf

1. Den aktuellen Stand des Repos ziehen: `git pull origin main` (bzw. den Stand eines Branch ziehen, an dem weiter gearbeitet werden soll `git pull origin [besagter_branch]`)
2. In das Verzeichnis des Notensatzes, der bearbeitet werden soll wechseln.
3. Branch für die Bearbeitung der neuen Aufgabe erstellen: ` git checkout -b [branch_name]" ` 
4. Die betreffende *dekomprimierte .mscx* Datei bearbeiten und speichern. *Wichtig:* .mscz Dateien werden nicht getrackt, da diese binär sind und keinen sinnvollen Diff ausgeben.
5. Änderungen hinzufügen z.B. mit `git add .`, damit sichergestellt wird, dass die beim Speichern der .mscx erstellen Metadaten beim Committen übernommen werden.
6. Mit `git status` überprüfen, ob alles korrekt erfasst wurde. Es wird benötigt:
	- .mscx Datei
	- score_style.mss
	- audiosettings.json
	- automation.json
	- viewsettings.json
	- das Verzeichnis META-INF/
	- das Verzeichnis Thumbnails/ 
7. Änderungen committen: `git commit -m "[commit_message]" `
8. Branch pushen: `git push origin [branch_name] `


