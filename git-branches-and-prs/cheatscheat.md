# Git Branches & Pull-requests

[Git Branches](../github-and-markdown/cheatsheet.md)

![Git Branches Grafik](./branches.png)


---

## 🔄 Was ist ein **Pull Request**?

Ein **Pull Request (PR)** ist eine **Anfrage**, Code von einem Branch (z. B. `feature/login`) in einen anderen Branch (z. B. `main`) **zu mergen** – **nachdem** du Änderungen gemacht hast.

**Typischer Ablauf:**

1. Du erstellst einen **Branch**.
2. Du arbeitest an neuen Features / Fixes.
3. Du **pushst** deinen Branch zu GitHub.
4. Du stellst einen **Pull Request**.
5. Andere prüfen deinen Code (Code Review).
6. Nach Freigabe wird er in den Hauptbranch **gemergt**.

---

## 📊 Veranschaulichung (grafisch)

Hier ist eine einfache visuelle Darstellung des Pull-Request-Flows:

```
main
 │
 ├── feature/login     ← Du arbeitest hier lokal
 │     ↓
 │   commit commit commit
 │     ↓
 │   Push to GitHub
 │     ↓
 └─> Pull Request → Code Review → Merge into main
```

---

## 💡 Warum Pull Requests?

| Vorteil           | Erklärung                                                       |
| ----------------- | --------------------------------------------------------------- |
| ✅ Code Review     | Andere Teammitglieder können den Code prüfen                    |
| 📝 Diskussion     | Kommentare, Vorschläge & Änderungswünsche direkt am Code        |
| 🧪 Tests & Checks | Automatische Checks können PRs testen (z. B. mit CI/CD)         |
| 📜 Dokumentation  | PRs zeigen, **was**, **warum** und **wie** etwas geändert wurde |
| 🔒 Sicherheit     | Änderungen kommen **nicht ungeprüft** in den Hauptzweig         |

---

## 🛠️ Häufige Pull-Request-Befehle (lokal)

| Befehl                             | Bedeutung                                    |
| ---------------------------------- | -------------------------------------------- |
| `git push -u origin feature/login` | Branch pushen, um PR auf GitHub zu erstellen |
| *(Rest passiert meist in GitHub)*  | GUI-gesteuert – mit Review, Merge etc.       |

---
