## 1. Set Env-Variables

- Die Umgebuzngsvariablen sind Teil der Session im Terminal/Powershell
- Im AWS Kontext nutzen wir die Env-Variablen, um unseren `AWS_ACCESS_KEY_ID` und `AWS_SECRET_ACCESS_KEY` zu setzen

### Linux

`export AWS_ACCESS_KEY_ID=`

`export AWS_SECRET_ACCESS_KEY=`

`export AWS_DEFAULT_REGION=us-east-1`

### Windows

`$env:AWS_ACCESS_KEY_ID=""`
`$env:AWS_SECRET_ACCESS_KEY=""`
`$env:AWS_DEFAULT_REGION="us-east-1"`

## Terraform state

### Workflow

![Basic Workflow](./images/tfstate_workflow.png)

### TF State Remote in Speicher ablegen

![](./images/tfstate_solution.png)

## Aufgabe Git Branches

1. `git pull` von main branch, um aktuelle Änderungen herunterzuladen
2. Neuen Branch erstellen `feature/003-update-infrastructure`
3. Infrastructure.md anlegen
4. `commit` auf Änderung
5. Branch publishen
6. Pull request über Github.com UI erstellen
7. Einen Kommentar bei einer Änderung hinterlassen
8. Über Github UI mergen
9. `git checkout main`
10. `git pull` ausführen

## Merge Konflikte beheben (einfach):

1. `git checkout main`
2. Datei auf main branch anlegen (Merge_Conflicts.md)
3. Datei mit `# Merge Conflicts` füllen
4. Speicher, comitten und auf main pushen
5. `git checkout -b dev-1-test`
6. Ändern der Überschrift zu `# Merge Konflikte beheben`
7. Commiten, Branch veröffentlichen und PR erstellen
8. wieder `git checkout main`
9. von hier aus `git checkout -b dev-2-test`
10. Ändern der Überschrift zu `# Arbeiten mit Merge Konflikten`
11. Commiten, Branch veröffentlichen und PR erstellen
12. 1. PR mergen
13. in UI den 2. PR überprüfen --> Merge Konflikte anzeigen
14. VS-Code öffnen
15. `git checkout main` && `git pull`
16. `git checkout dev-2-test`
17. `git merge main`
18. Müsst ihr merge Konflikte beheben, commiten, pushen
19. Auf github.com PR überprüfen, dass mergen möglich ist und letzendlich mergen

## Aufgabe für Git Vertiefung:

- [learngitbranching.js.org](https://learngitbranching.js.org/?locale=de_DE)
