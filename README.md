# Git Shell Hausaufgabe

Dieses Repository enthält ein kleines Bash-Skript für einfache IT-Support-Aufgaben.

Das Skript begrüßt den Benutzer mit Namen und bietet ein Menü an. Über das Menü können Systeminformationen angezeigt, der Speicherplatz geprüft oder das Programm beendet werden.

## Geübte Git-Themen

- git add
- git commit
- git push
- git branch
- git checkout
- git merge
- git rebase

## Theoriefragen

### 1. Was ist ein Merge-Konflikt?

Ein Merge-Konflikt entsteht, wenn Git zwei Änderungen nicht automatisch zusammenführen kann. Das passiert häufig, wenn unterschiedliche Branches dieselben Zeilen einer Datei verändert haben.

### 2. Warum entsteht ein Merge-Konflikt meistens bei derselben Stelle?

Git weiß in diesem Fall nicht, welche Änderung behalten werden soll. Deshalb muss der Benutzer die gewünschte Lösung selbst auswählen oder beide Änderungen sinnvoll kombinieren.

### 3. Warum gab es in dieser Aufgabe keinen Merge-Konflikt?

Die Branches wurden in der vorgesehenen Reihenfolge erstellt und gemergt. Dadurch arbeitete jeder neue Branch auf dem aktuellen Stand von master, sodass keine widersprüchlichen Änderungen entstanden.

### 4. Was zeigt Git bei einem Merge-Konflikt an?

Git fügt Markierungen in die betroffene Datei ein. Diese Markierungen zeigen, welche Änderung aus welchem Branch stammt und welcher Bereich vom Konflikt betroffen ist.

### 5. Wie löst man einen Merge-Konflikt?

Zuerst öffnet man die betroffene Datei und entscheidet, welche Inhalte übernommen werden sollen. Danach entfernt man die Konfliktmarkierungen, speichert die Datei, testet sie und erstellt anschließend den Merge-Commit.

### 6. Warum soll man das Skript danach testen?

Beim Lösen eines Konflikts können versehentlich wichtige Zeilen gelöscht oder verändert werden. Ein Test zeigt, ob das Skript weiterhin korrekt funktioniert.

### 7. Was macht git merge?

git merge führt die Änderungen eines anderen Branches in den aktuell geöffneten Branch ein. Zum Beispiel können die Änderungen aus feature-menue in master übernommen werden.

### 8. Was macht git rebase?

git rebase setzt die eigenen Commits auf einen neueren Stand eines anderen Branches. Dadurch entsteht häufig eine geradere und übersichtlichere Historie.

### 9. Wichtigster Unterschied zwischen merge und rebase

merge bewahrt die ursprüngliche Entwicklung und erstellt häufig einen zusätzlichen Merge-Commit. rebase verändert die Reihenfolge beziehungsweise Grundlage der Commits und schreibt dadurch die Historie neu.

### 10. Warum zeigt merge besser, wann ein Branch zusammengeführt wurde?

Der Merge-Commit macht sichtbar, wann die Entwicklung eines Branches in den Hauptbranch übernommen wurde. Dadurch bleibt die ursprüngliche Branch-Struktur besser erkennbar.

### 11. Warum kann rebase sauberer aussehen?

Durch rebase werden die Commits häufig in eine gerade Reihenfolge gebracht. Die Historie enthält dadurch weniger zusätzliche Merge-Commits.

### 12. Warum muss man bei rebase mit geteilten Branches vorsichtig sein?

rebase verändert die Commit-Historie. Wenn andere Personen bereits auf dieser Historie arbeiten, können dadurch unterschiedliche Versionsstände und zusätzliche Probleme entstehen.

### 13. Wann würde man eher merge verwenden?

merge eignet sich besonders für gemeinsame Branches und für Situationen, in denen die ursprüngliche Entwicklungshistorie erhalten bleiben soll.

### 14. Wann könnte rebase sinnvoll sein?

rebase kann sinnvoll sein, wenn man auf einem eigenen, noch nicht veröffentlichten Branch arbeitet und die Historie vor dem Zusammenführen übersichtlicher machen möchte.