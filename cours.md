### Dev web

Ceci est une commande :
``` shell
    mdkir test
```

Ceci est du code : 
```javascript
const test = 'Hello World';
```

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
On mets `i` et en dessous il y a écrit "INSERT" et on peut mettre notre message.


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
Untraked (non suivi) : quand le fichier vient d'être créer

Unmodified : le ficher est dans le git mais n'est pas modifié

Modified : le fichier est modifié

Staging area : zone dans lquelle je vais accumuler des fichiers nouvellement créés pour un commit 

Pour sortir de la phase staged : 
```
    git commit -m "first commit"
```
