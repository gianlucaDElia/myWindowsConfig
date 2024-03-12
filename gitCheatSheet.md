# Configurazione globale 

Imposta il nome che vuoi mostrare sulle tue commit:
```
$ git config --global user.name "[name]" 
```
Imposta l’email che vuoi mostrare sulle tue commit:
```
$ git config --global user.email "[email address]" 
```
 

# Creare un repository locale 

Crea un nuovo repository: 
```
$ git init 
```
 

# Effettuare modifiche 

Rivedi i cambiamenti al codice e prepara una commit: 
```
$ git status 
```
Inserire un file nell’area di staging: 
```
$ git add [file-name] 
```
inserire tutti i file nell’area di staging: 
```
$ git add . 
```
Salva gli snapshot dei file in maniera permanente nello storico: 
```
$ git commit -m"[descriptive message]" 
```
Elenca lo storico di versione per il branch corrente: 
```
$ git log 
```
 

# Modifiche di gruppo 

Elenca tutti i branch nel repository corrente: 
```
$ git branch 
```
Crea un nuovo branch: 
```
$ git branch [branch-name] 
```
Passa al branch specificato e aggiorna la directory corrente: 
```
$ git checkout [branch-name] 
```
Unisci lo storico del branch specificato con quello corrente: 
```
$ git merge [branch-name] 
```
Elimina il branch specificato: 
```
$ git branch -d [branch-name] 
```
 

# Tagging dei commits 

Elenca tutti i tag: 
```
$ git tag 
```
Crea un tag: 
```
$ git tag [name] [commit sha] 
```
Rimuove un tag: 
```
$ git tag -d [name] 
```
 

# Refactoring dei nomi di file 

Ricerca e rimuovi file dallo storico 
```
$ git rm [file] 
```
Rimuovi un file dalla directory e prepara l’eliminazione definitiva 
```
$ git rm --cached [file] 
```
Elimina il file dallo storico di versione ma mantieni il file locale 
```
$ git mv [file-original] [file-renamed] 
```
Modifica il nome del file in preparazione a una commit 

# Escludere file dallo storico 

Escludi file e percorsi temporanei 
```
*.log 

build/ 

temp-* 
```
 

Un file di testo chiamato .gitignore previene il versioning accidentale di file o directory secondo un pattern specificato. 

Elenca tutti i file ignorati in questo progetto: 
```
$ git ls-files --others --ignored --exclude-standard 
```
 

# Sincronizzare i cambiamenti 

Clonare un repository remoto: 
```
$ git clone [project url] 
```
Collegati a un URL remoto e ottieni lo storico dei cambiamenti 
```
$ git fetch [remote] 
```
Scarica lo storico dei cambiamenti dal repository remoto 
```
$ git merge [remote]/[branch] 
```
Unisci il branch remoto con quello locale 
```
$ git push [remote] [branch] 
```
Carica tutti i cambiamenti dal branch locale su GitHub 
```
$ git pull 
```
Scarica lo storico e unisci i cambiamenti 

 

# From local to bare repo 

Copy content of .git folder to the new location and than 
```
$ git config --bool core.bare true 
```
