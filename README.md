--------------------------------------------------------

=======================
GITHUB – BEGRIFFSERKLÄRUNG
=======================

• Repository (Repo)
Ein Projektordner, den Git verwaltet – lokal auf deinem PC oder online (z. B. auf GitHub).

• Working Tree (Arbeitsverzeichnis)
Der sichtbare Ordner mit deinen aktuellen Dateien – also das, woran du gerade arbeitest.

• Staging Area (Index)
Eine Zwischenablage für Änderungen, die du mit git add vorgemerkt hast – noch nicht endgültig übernommen.

• Remote
Ein Verweis auf ein entferntes Repository (z. B. auf GitHub).
Standardname ist meistens origin.

• Branch
Ein Entwicklungszweig, auf dem du unabhängig vom Hauptzweig arbeiten kannst.

=======================
 GIT BEFEHLE – GRUNDLAGEN
=======================

• git init
  Erstellt ein neues, leeres Git-Repository im aktuellen Ordner.

• git add <Datei> bzw. git add .
  Fügt Änderungen zur Staging Area hinzu – also zur Zwischenablage vor dem Commit.

• git commit -m "Nachricht"
  Speichert alle gestagten Änderungen dauerhaft im Repository mit einer erklärenden Nachricht.

• git status
  Zeigt den aktuellen Zustand des Arbeitsverzeichnisses: Was wurde geändert, was ist bereit für den Commit?

• git checkout <Branch/Commit>
  Wechselt zwischen Branches oder zu einem bestimmten Commit-Zustand.

• git branch <Name>
  Erstellt einen neuen Branch – eine separate Entwicklungslinie.

• git merge <Branch>
  Führt einen anderen Branch in den aktuellen zusammen – nützlich z. B. zum Zusammenführen von Features.

• git log
  Zeigt eine chronologische Liste aller bisherigen Commits mit Autor, Datum und Nachricht.

• git log --graph --all
  Zeigt die Commit-Historie als Baumstruktur – inklusive aller Branches.

• git rebase <Branch>
  Wendet Änderungen aus einem Branch auf einen neuen Ausgangspunkt an – für eine aufgeräumte Historie.

• git cherry-pick <Commit-Hash>
  Wendet einen bestimmten Commit gezielt auf den aktuellen Branch an.

• git reset --hard <Hash>
  Setzt den aktuellen Stand **komplett** zurück auf einen früheren Commit – Änderungen gehen **verloren**.

• git reset --mixed <Hash>
  Setzt zurück, behält aber die Änderungen im Arbeitsverzeichnis (nicht gestaged).

• git reset --soft <Hash>
  Setzt zurück, behält alles im Staging-Bereich – ideal, wenn du nur den letzten Commit ändern willst.

--------------------------------------------------------

=======================
 GITHUB BEFEHLE – REMOTE ARBEIT
=======================

• git clone <URL>
  Lädt ein bestehendes Repository von GitHub herunter und erstellt eine lokale Kopie.

• git push
  Überträgt deine lokalen Commits ins Remote-Repository auf GitHub.

• git fetch
  Holt neue Änderungen vom Remote-Repository – ohne sie direkt in deinen Code einzubauen.

• git pull
  Holt neue Änderungen und **führt sie direkt** in deinen aktuellen Branch ein (fetch + merge).

• git push --set-upstream origin <Branch>
  Verknüpft deinen lokalen Branch mit dem Remote-Branch und pusht die Änderungen – meist beim ersten Push nötig.

