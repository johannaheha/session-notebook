## 🌿 Branches bei GitHub / Git


Branches are a super important feature in Git and GitHub that allow you to work in parallel on different features, bug fixes, or experiments without disturbing the main branch (e.g., `main`).

--- 

### 👓 What is a branch?

* Branches enable parallel work on features, fixes, or experiments
* Keep main branch stable and clean
* Easy to merge changes when ready

---

### ⚡ Common Branch Workflows

* Feature Branch: A new branch for a new feature (e.g., `feature/login`).
* Bugfix Branch: Fix for a bug (e.g., `bugfix/header-crash`).
* Release Branch: Preparation for a release.
* Hotfix Branch: Urgent fix on production code.


## 🌿 Nützliche Git-Branchbefehle

| Emoji | Befehl                        | Bedeutung                                                                         |
| ----- | ----------------------------- | --------------------------------------------------------------------------------- |
| 🌿    | `git branch`                  | Listet deine lokalen Branches auf                                                 |
| 🌍    | `git branch -a`               | Listet alle Branches auf (lokal und remote)                                       |
| ➕🌿   | `git branch <branch-name>`    | Erstellt einen neuen Branch                                                       |
| 🔁    | `git switch <branch-name>`    | Wechselt zu einem bestehenden Branch                                              |
| ➕🔁   | `git switch -c <branch-name>` | Erstellt einen neuen Branch und wechselt direkt hin                               |
| 🚀🌿  | `git push -u origin <branch>` | Überträgt den Branch zum Remote-Repo und setzt Tracking                           |
| 🔁    | `git merge <branch-name>`     | Fügt Änderungen eines Branches in den aktuellen ein                               |
| 🗑️   | `git branch -d <branch-name>` | Löscht einen lokalen Branch                                                       |
| 🌍    | `git fetch`                   | Holt neue Branches und Änderungen vom Remote (ohne mergen)                        |
| 🔄🌍  | `git pull`                    | Holt und merged neue Änderungen vom Remote-Branch                                 |
| 🔄    | `git restore <Datei>`         | Macht Änderungen an Dateien im Arbeitsverzeichnis rückgängig (Datei zurücksetzen) |

---

### ℹ️ Hinweis zu `git switch`

* `git switch` ist der moderne Befehl nur zum Branch-Wechsel.
* `git switch <branch>` wechselt zu einem bestehenden Branch.
* `git switch -c <branch>` erstellt einen neuen Branch und wechselt direkt.
* Dadurch ist dein Workflow klarer als mit alten Befehlen.

### ℹ️ Hinweis zu `git restore`

* `git restore <Datei>` setzt Änderungen an einer Datei zurück, die noch nicht committet wurden.
* Ideal, wenn du z.B. versehentlich etwas geändert hast und zum letzten Commit zurück möchtest.
* Für mehr Kontrolle und Wiederherstellung gibt’s auch Optionen wie `--staged`.

---

## Beispiel Workflow

```bash
git checkout -b feature/login       # neuen Feature-Branch erstellen und wechseln
# Änderungen machen, Dateien adden und committen
git push -u origin feature/login    # Branch zum Remote hochladen
```

Auf GitHub erstellst du dann einen Pull Request von `feature/login` in `main`.

---

### Markdown Examples

| Element                         | Markdown Syntax                   |
| ------------------------------- | --------------------------------- |
| Level 1 headline                | `# Level 1 headline`              |
| Level 2 headline                | `## Level 2 headline`             |
| Level 5 headline                | `##### Level 5 headline`          |
| list item                       | `- list item`                     |
| [ ] done                        | `[ ] checkbox`                    |
| [x] done                        | `[x] checkbox`                    |
| **bold text**                   | `**bold text**`                   |
| _italicized text_               | `_italicized text_`               |
| [link](https://www.example.com) | `[link text](https://www.example.com)` |
| image                           | `![description of image](url to image)`           |
| block quote                     | `> block quote`                   |
| divider                         | `---`                             |
| `inline code block`             | `` `inline code block` ``         |
| `code block`                    | ` ``` code block ``` `            |

See this [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for
more Markdown Syntax.
