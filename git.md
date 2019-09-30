#### Dateien in die Staging Area einpflegen

```
git add .
```

#### Dateien aus der Staging Area entfernen

```
git reset [Datei_name]
```

#### Dateien in das local-repo einpflegen

```
git commit -m "[message]"
```

#### Dateien aus dem local-repo entfernen

```
git rm --cached file.txt
```

#### Dateien in das remote-repo einpflegen

```
git push origin master
```

#### Dateien aus dem remote-repo entfernen

Pull the changes from the server ```git rm``` on the local repo

### Status des Git-Working-Directories ansehen

```
git status
```

### Pretty Printing für Git-Logs

<https://stackoverflow.com/questions/1057564/pretty-git-branch-graphs>

 mit Verwendung von .gitconfig
``` $ nano ~/.gitconfig```
```
[alias]
lg1 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all
lg2 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all
lg = !"git lg1"
```
```git lg```/ ```git lg1```

### Zweige für eigene Features erstellen

````
git branch new-branch
````

### Branch wechseln

```
$ git checkout new-branch
Switched to branch 'new-branch'
```

In einem Zweig Daten ändern und anschließend im anderen Zweig Daten ändern und beide Änderungen commiten / pushen

### Branch mergen

merge the new-feature into the master branch
```
git checkout master
git merge new-branch
```


