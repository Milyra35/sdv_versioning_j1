# VERSIONING (Git, GitHub, GitLab)

- git init : créer un dépôt
- git add : préparer les fichiers pour le commit
- git commit -m 'message' : enregistrer les modifications
- git status : afficher l'état du depôt
- git log : afficher l'historique des commits
- git remote add origin URL_DU_DEPOT : Connecte avec ton dépôt local à GitHub
- git push : envoie les commits locaux vers GitHub
- git pull : récupère les dernières modifications de GitHub

# Branching

Les branches permettent de travailler sur des fonctionnalités indépendantes sans impaacter la branche principale.
- git branch : liste des branches
- git branch NOM_BRANCHE : créer une nouvelle branche
- git checkout NOM_BRANCHE : basculer sur une branche
- git merge NOM_BRANCHE : fusionner une branche dans la branche courante
- git branch -D NOM_BRANCHE : delete une branche

Merge crée un commit spécial qui fusionne deux branches, conservant l'historique entier.
Rebase réapplique les commits d'une branche par-dessus une autre, produisant un historique linéaire et plus propre.

# Branches et collaboration

- Brancher pour travailler sur une nouvelle fonctionnalité sans toucher au code principal
- Main : branche principale et stable
- Feature : créer une branche pour une nouveauté

# Fichier .gitignore

- Liste les fichiers et dossiers que Git doit ignorer, et donc idéalement éviter de commit des fichiers volumineux, sensibles ou temporaires.

# Parcourir et manipuler l'historique Git

- git log : affiche l'hsitorique clair et visuel des commits
- git reflog :remonte tous les mouvements de HEAD (utile pour retrouver des états perdus)
- git reset : replace le dépôt à un commit antérieur (!!destructif!!)
- git revert : crée un nouveau commit annulant un changement sans casser l'historique

# Sauvegarder / Restaurer / Appliquer

- git stash : met de côté temporairement les modifications non validées
- git stash list : affiche toutes les sauvegardes en attente
- git stash apply stash@{} : réapplique un stash spécifique sans le supprimer de la liste
- git stash pop : réapplique et supprime le dernier stash de la liste