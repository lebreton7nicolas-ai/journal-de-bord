# mémo Git

## 1. Configuration et démarrage
- `git init` : Initialiser un dépôt Git dans le dossier actuel.
- `git config --global user.name "Nom"` : Définir le nom d'utilisateur.
- > dans paramètres, modifier les variables d'environnements sytème; variables d'environnement; variable d'utilisateur : HOME %USERPROFILE% 
- `git config --global user.email "email@exemple.com"` : Définir e-mail.
-  `git config --list`: vérifier les config

## 2. Cycle de base (Modifications & Commits)
- `git status` : Vérifier l'état des fichiers (modifiés, suivis, prêts à être validés).
- `git add <fichier>` : Ajouter un fichier précis à la zone de transit (staging).
- `git add .` : Ajouter tous les fichiers modifiés.
- `git commit -m "Message clair"` : Enregistrer les modifications dans l'historique.
- `git log --oneline` : Afficher l'historique condensé des commits.

## 3. Gestion des branches
- `git branch` : Lister les branches locales.
- `git switch -c <nom-branche>` : Créer et basculer sur une nouvelle branche.
- `git switch <nom-branche>` : Changer de branche.
- `git merge <nom-branche>` : Fusionner une branche dans la branche actuelle.
- `git branch -d <nom-branche>` : Supprimer une branche déjà fusionnée.

## 4. Synchronisation avec un dépôt distant (GitHub / GitLab)
- `git remote -v` : Afficher les dépôts distants configurés.
- `git pull` : Récupérer et fusionner les dernières modifications distantes.
- `git push -u origin <nom-branche>` : Envoyer une branche locale pour la première fois.
- `git push` : Envoyer les nouveaux commits vers le dépôt distant.

## 5. Annuler ou corriger des erreurs
- `git restore <fichier>` : Annuler les modifications non enregistrées d'un fichier.
- `git restore --staged <fichier>` : Retirer un fichier de la zone de transit (sans perdre les modifs).
- `git commit --amend -m "Nouveau message"` : Modifier le dernier commit.
- `git revert <id-commit>` : Créer un nouveau commit qui annule proprement un ancien commit.