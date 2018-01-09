# Glossaire GIT

## EFFECTUER DES CHANGEMENTS

```
$ git status
Liste tous les nouveaux fichiers et les fichiers modifiés à commiter

$ git add [fichier]
Ajoute un instantané du fichier, en préparation pour le suivi de version

$ git reset [fichier]
Enleve le fichier de l'index, mais conserve son contenu

$ git diff
Montre les modifications de fichier qui ne sont pas encore indexées

$ git diff --staged
Montre les différences de fichier entre la version indexée et la dernière
version

$ git commit -m "[message descriptif]"
Enregistre des instantanés de fichiers de façon permanente dans
l'historique des versions
```

## CONFIGURATION DES OUTILS

```
$ git config --global user.name "[nom]"
Définit le nom que vous voulez associer à toutes vos opérations de
commit

$ git config --global user.email "[adresse email]"
Définit l'email que vous voulez associer à toutes vos opérations de commit

$ git config --global color.ui auto
Active la colorisation de la sortie en ligne de commande
```

## GROUPER DES CHANGEMENTS

```
$ git branch
Liste toutes les branches locales dans le dépôt courant

$ git branch [nom-de-branche]
Crée une nouvelle branche

$ git checkout [nom-de-branche]
Bascule sur la branche spécifiée et met à jour le répertoire de travail

$ git merge [nom-de-branche]
Combine dans la branche courante l'historique de la branche spécifiée

$ git branch -d [nom-de-branche]
Supprime la branche spécifiée
```

## CRÉER DES DÉPÔTS

```
$ git init [nom-du-projet]
Crée un dépôt local à partir du nom spécifié

$ git clone [url]
Télécharge un projet et tout son historique de versions
Pas de git init lorsque git clone.
```

## ENREGISTRER DES FRAGMENTS

```
$ git stash
Enregistre de manière temporaire tous les fichiers sous suivi de version
qui ont été modifiés ("remiser son travail")

$ git stash list
Liste toutes les remises

$ git stash pop
Applique une remise et la supprime immédiatement

$ git stash drop
Supprime la remise la plus récente
```

## SYNCHRONISER LES CHANGEMENTS

```
$ git fetch [nom-de-depot]
Récupère tout l'historique du dépôt nommé

$ git merge [nom-de-depot]/[branche]
Fusionne la branche du dépôt dans la branche locale courante

$ git push [alias] [branche]
Envoie tous les commits de la branche locale vers GitHub

$ git pull
Récupère tout l'historique du dépôt nommé et incorpore les modifications
```

## REFAIRE DES COMMITS

```
$ git reset [commit]
Annule tous les commits après `[commit]`, en conservant les
modifications localement

$ git reset --hard [commit]
Supprime tout l'historique et les modifications effectuées après le
commit spécifié
```

## VÉRIFIER L'HISTORIQUE DES VERSIONS

```
$ git log
Montre l'historique des versions pour la branche courante

$ git log --follow [fichier]
Montre l'historique des versions, y compris les actions de renommage,
pour le fichier spécifié

$ git diff [premiere-branche]...[deuxieme-branche]
Montre les différences de contenu entre deux branches

$ git show [commit]
Montre les modifications de métadonnées et de contenu inclues dans
le commit spécifié
```

## CHANGEMENTS AU NIVEAU DES NOMS DE FICHIERS

```
$ git rm --cached [fichier]
Supprime le fichier du système de suivi de version mais le préserve
localement

$ git rm [fichier]
Supprime le fichier du répertoire de travail et met à jour l'index

$ git mv [fichier-nom] [fichier-nouveau-nom]
Renomme le fichier et prépare le changement pour un commit 
```