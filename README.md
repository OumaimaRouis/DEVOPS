# DEVOPS

## PARTIE 1:
### Comment vérifier la configuration actuelle de Git sur votre machine, notamment le nom d’utilisateur et l’adresse e-mail ?
git config user.name
git config user.email

### Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installation de Git ?
git config user.email "nouvelle@email.com"

## PARTIE 2:
### Si vous avez oublié de créer un fichier README.md lors de l'initialisation du projet, comment pouvez-vous l'ajouter après coup et commiter les changements ?
git add README.md
git commit -m "Ajout du fichier README.md"
git push origin main

### Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la création du projet ?
git remote add origin git@github.com:votre-nom-utilisateur/mon-projet.git

## PARTIE 3:
### Comment annuler les modifications locales d'un fichier avant de les ajouter à l'index ?
git checkout -- index.html

### Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?
git status

## PARTIE 4:
### 4. Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?
git fetch --all

### Comment supprimer une branche locale après l'avoir fusionnée dans master ?
git branch -d ma-fonctionnalite

## PARTIE 5:
### Comment interrompre un rebase en cours si vous avez commis une erreur ?
git rebase --abort

### Comment lister les commits qui vont être rebasés avant de lancer un rebase ?
git rebase --interactive master

## PARTIE 6:
### Comment afficher la liste des branches actives et en cours de développement dans Gitflow ?
git flow feature list
git flow release list
git flow hotfix list

### Comment annuler une branche de correctif (hotfix) avant de la finaliser si vous constatez une erreur ?
git checkout master
git branch -D hotfix/mon-correctif
git push origin --delete hotfix/mon-correctif



