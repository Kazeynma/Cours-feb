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
permet  d'initialiser un depot GIT. Elle retourne :
```
Initialized empty Git repository in C:/Users/Mywin/BTS/.git/
```

Pour vérifier l'état de votre depot GIT utiliser la commande : 
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

Staging area : zone dans lquelle je vais accumuler des fichiers nouvellement créer pour un commit 

Pour sortir de la phase staged : 
```
    git commit -m "first commit"
```