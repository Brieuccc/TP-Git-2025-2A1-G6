# Réflexion Git

## 1. Quelle est la structure actuelle du projet Git ?

Le projet est structuré autour de plusieurs branches : une branche principale `main`, et des branches personnelles pour chaque élève (`branch/deniz`, `branch/brieuc`, `branch/luka`). Chaque branche contient des fichiers spécifiques (comme `tp.md`, `detached.md`, etc.) et des commits reflétant les différentes phases du TP. Des merges ont été réalisés avec ou sans fast-forward, et une Pull Request a été fusionnée via Squash & Merge.

## 2. Quelle est la différence entre `git fetch` et `git pull` ?

`git fetch` récupère les dernières modifications du dépôt distant **sans les intégrer** dans la branche locale.  
`git pull` fait la même chose **mais en plus**, il **fusionne automatiquement** les changements dans la branche locale.  
Autrement dit, `git pull = git fetch + git merge`.

## 3. Quelle est la différence entre `git reset` et `git revert` ?

`git reset` annule des commits en **modifiant l’historique** (souvent utilisé en local).  
`git revert` crée un **nouveau commit** qui annule les effets d’un commit précédent **sans modifier l’historique**.  
`reset` est destructif, `revert` est sécurisé et recommandé pour les projets collaboratifs.

