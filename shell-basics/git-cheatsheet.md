## 🧠 Nützliche Git-Befehle 

|       | Befehl                             | Bedeutung                                                     |
| ----- | ---------------------------------- | ------------------------------------------------------------- |
| 🆕    | `git init`                         | Erstellt ein neues, leeres Git-Repository im aktuellen Ordner |
| 📥    | `git clone URL`                    | Klont ein bestehendes GitHub-Repo auf deinen Rechner          |
| 🌐    | `git remote -v`                    | Zeigt die verbundenen Remote-Repositories (URLs) an           |
| ➕🌍   | `git remote add origin <SSH-Link>` | Fügt ein Remote-Repo namens `origin` hinzu (meist GitHub)     |
| 📋    | `git status`                       | Zeigt, welche Dateien geändert, gestaged oder untracked sind  |
| ➕     | `git add <Datei>`                  | Dateien für den nächsten Commit vormerken (stagen)            |
| 🔄    | `git restore <Datei>`              | Macht Änderungen an Dateien im Arbeitsverzeichnis rückgängig  |
| 💾    | `git commit -m "Nachricht"`        | Speichert die gestagten Änderungen als neuen Commit           |
| 🚀🚀  | `git push -u origin main`          | Überträgt den lokalen (neuen) Branch `main` zum Remote-Repo `origin`  |
| 🚀    | `git push`                         | Überträgt den akutellen Branch zum eingetragnen Remote-Repo                             |
| ⬇️🔄  | `git pull`                         | Holt neueste Änderungen vom Remote-Repo und merged sie        |
| 📜    | `git log`                          | Zeigt die Historie der Commits                                |
| 🔍    | `git diff`                         | Zeigt detailliert, was sich in den Dateien geändert hat       |

---

## 📁 Schritt 1: Lokales Git-Repository erstellen

### 1.1. Wechsle im Terminal in dein Projektverzeichnis:

```bash
cd /pfad/zu/deinem/projekt   🏃 cd--> change directory
```

Wenn du noch kein Verzeichnis hast:

```bash
mkdir mein-projekt  📁 mkdir --> make directory
cd mein-projekt       🏃
```

### 1.2. Initialisiere ein Git-Repository:

```bash
git init     🆕  init --> initialize
```

Jetzt ist dein Projektordner ein Git-Repository. Git kann ab jetzt Änderungen verfolgen.

---

## 📝 Schritt 2: Dateien hinzufügen und committen

### 2.1. Erstelle z. B. eine Datei:

```bash
echo "# Mein Projekt" > README.md
```
🧠 Merksatz:
echo ist wie „sagen“ im Terminal – es wiederholt, was du ihm gibst.

"# Mein Projekt" steht für eine Überschrift der Ebene 1 in Markdown.

">" Das ist ein Umleitungsoperator in der Shell. Er leitet die Ausgabe von echo nicht ins Terminal, sondern in eine Datei.

---

#### 🆚 Direkter Vergleich echo und touch:

| Funktion                 | `echo "# Mein Projekt" > README.md`        | `touch README.md`               |
| ------------------------ | ------------------------------------------ | ------------------------------------ |
| Erstellt Datei           | ✅ Ja                                       | ✅ Ja                                 |
| Schreibt Inhalt rein     | ✅ Ja (`# Mein Projekt`)                    | ❌ Nein                               |
| Bestehende Datei ändern  | ✅ Überschreibt den Inhalt                  | ✅ Ändert nur den Zeitstempel         |
| Standard-Endung          | `.md` → Markdown-Datei                     | keine `.md`, `.txt`, o. Ä.           |
| Typischer Anwendungsfall | README erzeugen mit Inhalt (z. B. für Git) | Leere Datei anlegen oder Zeitstempel |

---

## 🧠 Merksatz:

* `echo >` = **Datei mit Inhalt**
* `touch` = **leere Datei (oder nur Zeit aktualisieren)**

---

### 2.2. Füge alle Dateien zur Git-Überwachung hinzu:

```bash
git add .   ➕   (git add . --> alle Dateien)
```

Oder nur eine bestimmte Datei:

```bash
git add README.md   (git add "Datei A" --> Datei A)
```

### 2.3. Mache deinen ersten Commit:

```bash
git commit -m "Erster Commit"   💾   
```

---

## ☁️ Schritt 3: Repository auf GitHub erstellen

1. Gehe auf [https://github.com](https://github.com).
2. Klicke auf **"New repository"**.
3. Gib einen Namen ein, z. B. `mein-projekt`.
4. Wähle **"Public"** oder **"Private"**.
5. NICHT `README.md` hinzufügen (du hast lokal schon eins).
6. Klicke auf **"Create repository"**.

---

## 🔗 Schritt 4: GitHub-Repo verbinden und hochladen

Angenommen, dein GitHub-Repo heißt `mein-projekt` und dein Benutzername ist `deinname`.

### 4.1. Verbinde dein lokales Repo mit dem GitHub-Repo:

```bash
git remote add origin https://github.com/deinname/mein-projekt.git
```

### 4.2. Lade deine Änderungen hoch:

```bash
git push -u origin main
```

Jetzt ist dein Projekt auf GitHub online 🎉

---

### 🔁 Weitere Änderungen hochladen

Wenn du später weitere Änderungen machst:

```bash
# Änderungen prüfen
git status

# Änderungen hinzufügen
git add .

# Commit machen
git commit -m "Neue Änderungen"

# Hochladen
git push
```



