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


# Bewertung – Git & GitHub Nachschlagwerk

## 1. Begriffe

**Punkte: 1 / 3**

**Begründung:**
- Die wichtigsten Begriffe wie *Repository*, *Commit*, *Branch*, *Merge*, *Remote*, *Staging Area* und *Merge-Konflikt* sind erklärt.
- Der Begriff *Repository* ist nicht korrekt! Das Repository ist die "Datenbank mit den verschiedenen Versionen".
- Der Begriff "Working Directory" fehlt.
- Die Erklärungen sind knapp, aber häufig verständlich.
- Die Formatierung ist unstrukturiert.
- Es fehlen Hinweise auf häufige Fehler.
- Es fehlt jedoch ein einleitender Abschnitt („Was ist Git/GitHub?“), der den Gesamtzusammenhang für Einsteiger klarer machen würde.
- Eine anschauliche Analogie (z. B. „Schreibtisch“, „Cloud“) hätte die Begriffe greifbarer gemacht.

---

## 2. Lokale Git-Befehle

**Punkte: 1 / 3**

**Begründung:**
- Die wichtigsten Befehle sind alle vorhanden und korrekt beschrieben: `init`, `add`, `commit`, `status`, `log`, `diff`, `branch`, `checkout`, `merge`, `merge --abort`.
- Die Formatierung macht den Abschnitt quasi unleserlich.
- Es fehlen weitere Erläuterungen zu Merge-Konflikten oder den Zusätzen vn `git reset`.


---

## 3. Arbeit mit Remote-Repositories

**Punkte: 1.5 / 3**

**Begründung:**
- Die Auflistung der Remote-Befehle ist vollständig und korrekt: `clone`, `push`, `pull`, `remote add`, `fetch`, `checkout -b ... origin/...`.
- Die Formatierung macht den Abschnitt quasi unleserlich.
- Der Unterschied zwischen `fetch` und `pull` ist nur implizit erkennbar.

---

## 4. Zusammenarbeit über GitHub

### a) Branches und Commit-Verlauf

**Punkte: 1 / 3**

**Begründung:**
- Es wurden zwar zwei Feature-Branches erstellt (`Qais`, `davis`), was grundsätzlich eine sinnvolle Aufteilung erkennen lässt.
- Allerdings wurden diese Branches **nicht** zusammengeführt (kein `merge`, kein `pull request`) – jeder Branch steht isoliert.
- Der `master`-Branch enthält nur drei Commits: *Initial commit*, *add deadline*, *Git befehle* – danach wurde offensichtlich nicht weiter gemeinsam daran gearbeitet.
- Keine Konflikte, kein tatsächlicher Austausch (Zusammenführung) erkennbar.

### b) Commit-Nachrichten

**Begründung:**
- Die Commit-Messages sind sehr knapp und teils unspezifisch („Git befehle“ vs. „README: Abschnitt git status ergänzt“ wäre z. B. präziser).
- Positiv: Es wurde kein überflüssiger „Test“- oder „Final Version“-Commit gemacht.

### c) Frequenz & Verteilung

**Begründung:**
- Sehr wenige Commits (nur drei im `master`-Branch, je einer in den anderen Branches).
- Die Arbeit wurde wahrscheinlich eher in einem Schritt erstellt und hochgeladen, nicht iterativ über mehrere Tage hinweg.
- Kein erkennbarer Workflow mit Feature-Zweigen, Merge Requests oder Konfliktlösung.

---

## Gesamtbewertung

| Kriterium                        | Punkte (max. 3) |
|----------------------------------|-----------------|
| 1. Begriffe                      | 1               |
| 2. Lokale Git-Befehle            | 1               |
| 3. Arbeit mit Remote-Repositories| 1.5               |
| 4. Zusammenarbeit über GitHub    | 1             |
| **Gesamt**                       | **4.5 / 12**    |

--> **37,5% --> 5+ (3 NP.)**
