Grundbegriffe

Repository: Ein Projektordner, der von Git verwaltet wird. Es kann lokal auf deinem Rechner oder als Remote-Version z. B. auf GitHub liegen.

Commit: Speichert einen bestimmten Stand deiner Dateien mit einer Nachricht.

Branch: Ein Entwicklungszweig für neue Features, der unabhängig vom Hauptzweig (z. B. main) verändert werden kann.

Merge: Verbindet zwei Branches zu einem gemeinsamen Stand.

Remote: Eine Online-Version deines Repositories (z. B. auf GitHub).

Staging Area: Zwischenspeicher für Dateien, bevor sie committet werden.

Merge-Konflikt: Tritt auf, wenn zwei Änderungen an derselben Stelle kollidieren und Git keine automatische Entscheidung treffen kann.

Lokale Git-Befehle

git init                       # Neues Git-Repository initialisieren
git status                     # Status der Dateien anzeigen
git add <datei>                # Datei zur Staging-Area hinzufügen
git add *                      # Alle Änderungen hinzufügen
git commit -m "Nachricht"      # Änderungen committen
git diff                       # Unterschiede anzeigen
git diff --staged              # Unterschiede zur Staging-Area anzeigen
git log                        # Commit-Historie anzeigen
git log --oneline              # Kurzform der Commit-Historie
git branch <name>              # Branch erstellen
git checkout <name>            # Zu einem Branch wechseln
git checkout -b <name>         # Branch erstellen und wechseln
git merge <branch>             # Branch in aktuellen Branch mergen
git merge --abort              # Merge-Konflikt-Vorgang abbrechen

GitHub & Remote-Repositories

git clone https://github.com/user/repo.git                 # Repository klonen
git remote add origin https://github.com/user/repo.git     # Remote hinzufügen
git remote -v                                              # Remote-Repositories anzeigen
git push                                                   # Push zum Remote-Repository
git push origin main                                       # Auf Branch 'main' pushen
git push --set-upstream origin <branch>                    # Remote-Branch erstellen und verknüpfen
git pull                                                   # Aktuellen Branch mit Remote abgleichen
git pull origin main                                       # Änderungen aus 'main' holen
git fetch origin                                           # Nur herunterladen, nicht mergen
git checkout -b localname origin/remotebranch              # Remote-Branch lokal auschecken