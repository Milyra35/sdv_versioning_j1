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