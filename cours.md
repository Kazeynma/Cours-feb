# Dev web

Ceci est une commande :
``` shell
    mdkir test
```

Ceci est du code : 
```javascript
const test = 'Hello World';
```

## Git

La commande 
```
    git init 
```
permet  d'initialiser un depot GIT ou le repository (le dossier qui contient les données que l'on souhaite versionner) dans le répertoire courant. Cela se traduit par la présence d'un dossier cache `.git/`. Elle retourne :
```
Initialized empty Git repository in C:/Users/Mywin/BTS/.git/
```

Pour vérifier l'état de votre depot GIT ( ajout et l'édition d'un fichier ) utiliser la commande : 
```
    git status
```
Bien penser à se mettre à la racine du projet

Pour ajouter un fichier au suivi : 
```
    git add 
```
Il faut mettre à la suite le fichier qu'on veut ajouter. Si on veut tous ajouter on mets . ou *.

Commit : permet de sauvegarder un ou plusieurs fichiers
```
    git commit 
```
On mets `i` et en dessous il y a écrit "INSERT" et on peut mettre notre message. Une fois le message écrit, appuyer sur echap esuite `:q`


Pour configurer son git 
```
    git config
```
On aura la liste de tous les options possibles. Pour configurer le git pour qu'il soit connecté à notre github :
```
    git config --global user.name "Jonh Doe"
    git config --global user.email "jDoe@gmail.com"
```

Maintenant on va regarder l'historique des commits avec :
```
    git log
```
<image src='./assets/cycle_de_la_vie_fichier.png'>
Untraked (non suivi) : quand le fichier vient d'être créer

Unmodified : le ficher est dans le git mais n'est pas modifié

Modified : le fichier est modifié

Staging area : zone dans lquelle je vais accumuler des fichiers nouvellement créés pour un commit 

Pour sortir de la phase staged : 
```
    git commit -m "first commit"
```
Pour mettre notre dépot sur GitHub :

Clé ssh ? Principe : échanger les carte d'identité publique pour donner l'accès // permet d'identifier une machine 

Pour ajouter notre depot sur GitHub
```
    git remote add origin git@github.com:Kazeynma/Cours-feb.git

```

Pour voir où est-ce que notre depot est :
```
    git remote -v
```

Si jamais on se trompe et qu'on veut mettre url :
```
    git remote rm origin
```

Pour avoir des données qu'on ne veut pas mettre sur github car c'est secret, faire un fichier `.gitignore`
=> tous ce qu'on va lister (mettre le nom des fichiers que l'on veut masquer) va être ignorer du tracking GIT

# Commande bash

Création d’un dossier en cmd
Linux ou (git bash) :

- `ls` : pour voir les fichiers dans le dossier actuel
- ⇒ `mkdir nom_dossier` : créer un dossier (make a dir)
- ⇒ `cd nom_dossier` : pour aller dans le dossier
- ⇒ `code .` : permet d’aller sur vscode
- ⇒ `touch linux_commands.md`

Autres commandes :
- `pwd` : le chemin depuis la racine
- `~` : raccourci vers le dossier utilisateur
- `ls` : permet d’afficher les fichiers
    - `ls -la` : permet d’afficher les fichiers cachés / fichiers commençant par un .
- `rm -rf` : applique à tous les fichiers jusqu’au sous-dossier
- `cd` : répertoire utilisateur
- `cat` : permet d’afficher le contenu d’un fichier dans le terminal