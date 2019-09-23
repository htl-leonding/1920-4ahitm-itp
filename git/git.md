# Git

VCS ... Version Contol System (Versionierungssystem)

## Probleme / Anforderungen

- Die Codebasis muss regelmäßig gesichert werden.
- Der Entwickler möchte Zugriff auf ältere Versionen seines Programms haben.
- Meistens werden Softwareprodukte in Teams erstellt; jedes Teammitglied braucht Zugriff auf den Sourcecode
- Teammmitglieder arbeiten oft gleichzeitig an den selben Sourcecode-Files. Sämtliche Änderungen müssen in die Codebasis eingepflegt werden.
- Separates Entwickeln von neuen Features, bis diese fehlerfrei sind und anschließendes Einfügen dieser neuen Funktionen in die Codebasis

## Alternativen

Sind ungenügend:

- regelmäßiges zippen der Codebasis und sichern
- zur Verfügung stellen der Codebasis auf einem File-Server und /oder auf der Dropbox (oder vergleichbare Dienste)

## Aufbau

- zentrale VCS zB Subversion
- dezentrale VCS zB Git

Provider: GitHub, Bitbucket, Gitlab


## Anwendungsfälle

### Erstellen eines Projekts

#### Leeres Projekt aus Git-Repo clonen


```
git remote add origin https://github.com/htl-leonding/my-project.git
git push -u origin master
```

#### Bereits bestehendes Projekt ins Git-Repo commiten

```
echo "# delete-me-please" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/htl-leonding/my-project.git
git push -u origin master
```

### Ein Projekt aus dem Repos downloaden (clonen)

### Neue und/oder geänderte Dateien ins das Repo einpflegen

#### Dateien in die Staging Area einpflegen

#### Dateien aus der Staging Area entfernen

#### Dateien in das local-repo einpflegen

#### Dateien aus dem local-repo entfernen

#### Dateien in das remote-repo einpflegen

#### Dateien aus dem remote-repo entfernen



### Status des Git-Working-Directories ansehen

```
git status
```

### Pretty Printing für Git-Logs

<https://stackoverflow.com/questions/1057564/pretty-git-branch-graphs>

ev. mit Verwendung von .gitconfig


### Zweige für eigene Features erstellen

### Branch wechseln

In einem Zweig Daten ändern und anschließend im anderen Zweig Daten ändern und beide Änderungen commiten / pushen

### Branch mergen

### Pull requests durchführen

- Jemand besitzt ein Repo
- Ein anderer cloned dieses Repo und möchte etwas im Original Repo ändern
- Er/Sie führt einen Pull Request durch

### Commits taggen

Szenario: Die einzelnen Releases (zB bei Auslieferung an den Kunden) sollen getagged werden

Begriff der Baseline

### Einen Release-Eintrag im Github erstellen (inkl. Doku)

### Verwerfen der lokalen Änderungen

Was bedeutet `stash`