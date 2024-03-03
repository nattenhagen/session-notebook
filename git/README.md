## Ein Projekt erstellen

_(inclusive Shell Befehle)_

mkdir neuer Ordner _"mein Projekt"_

touch neue Datei _"README.md index.html styles.css"_

cd steuern zu _"mein Projekt"_

code . öffnen _"mein Projekt"_

ihr öffnet VS-Code und öffnet die Datei (z.B. eine README.md)
diese Datei befüllt ihr mit etwas Text oder Code (z.B. _"mein Projekt"_)

git init git initialisieren

git add _"README.md"_

git commit -m "first commit"

git remote add origin git@github.com: username/reponame.git
(diesen Link findet ihr auf GitHub)

git push -u origin main

## Der alltägliche Workflow

(wenn das repo schon existiert und schon mit GitHub verknüpft ist)

```
git add .
```

alternativ: git add --all

wenn ihr nur spezifische Dateien commiten wollt: git add dateiname

git commit -m "a very good commit message"

git push

## Mit Branches arbeiten

git switch -c feature/feature-name

(ich wechsel den Branch und erstelle einen neuen -c = create - feature/feature name ist praktisch, wenn wir in "Ordnern" arbeiten, also einen Ordner nur um features zu bearbeiten oder bugs)

nächster Schritt --> schreibt den Code für das feature

git add .

git commit -m "Code für das Feature Branch"

git push -u origin feature/feature-name

nach erfolgreichem PR (Pull Request) + merge auf GitHub (Review Prozess!!!)

git switch main (jetzt bin ich wieder lokal, um weiterzuarbeiten nachdem alle Änderungen greviewt wurden und gemergt)

git pull

ein existierendes Repo auf GitHub lokal bearbeiten

git clone git@github.com:neuefische/hh-web-24-2.git

(lade dir ein Repository von Github runter und verbinde es direkt mit remote)

git switch -c "branchname" create a new branch and switch to it

git switch "branchname" --> switch branches

git branch --> list your branches
git branch -a --> list all branches (local and remote)

git branch -d "branchname" --> delete a branch
