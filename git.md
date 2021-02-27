- Cloner un dépôt en local

`git clone` *repository-url*

- Configurer le nom d'utilisateur et l'e-mail

`git config user.name <username>`

`git config user.email <email>`

- Créer une branche

`git branch` **branch-name**

- Se positionner sur une branche

`git checkout` __branch-name__

- Créer une branche, puis se positionner dessus

`git checkout -b <branch-name>`

- Se re-positionner sur la branche précédente

`git checkout @{-1}` | `git checkout -`

- Renommer une branche

`git branch -m <nouveau-nom*>`

- Fusionner 2 branches

`git merge <source-branch-name>`

- Fusionner 2 branches sans faire un commit de merge

`git rebase <branch-name>`

`git rebase --continue` *en cas de conflits*

`git push --force`

- Supprimer une branche

`git branch -d <branch-name>`

- Sauvegarder les modifications en cours sans faire de commit

`git stash`

- Récupérer les modifications sauvegardées

`git stash pop`
<p>
    <strong>NB :</strong> <strong>pop</strong> vide la réserve des modifications qui y sont stockées.
<p>

- Récupérer les modifications sauvegardées

`git stash apply`
<p>
    <strong>NB :</strong> Contrairement à pop, <strong>apply</strong> ne vide pas la réserve des modifications qui y sont stockées.
<p>

- Voir les modifications liées à une sauvegarde

`git stash show stash@{`*n*`}` où n est un entier naturel

- Récupérer un fichier spécificique d'une sauvegarde

`git checkout stash@{`*n*`}` *chemin-absolu-du-fichier*

- Ordonner

`git for-each-ref --sort=committerdate refs/heads/`

- Pusher une branche locale

`git push --set-upstream origin <branch-name>`

Appliquer sur une branche les modifications propres à un commit (sur une autre branche) :
- `git cherry-pick -n <commit-SHA>`

Retrouver l'auteur d'une modification :
- `git blame <filename>`

Ajouter un fichier à committer :
- `git add <filename>`

Retirer un fichier avant de committer :
- `git reset <filename>`

Définir la branche distante :
- `git branch --set-upstream-to=origin/<branch-name>`

Voir les répertoires distants :
- `git remote -v`

Voir les branches du répertoire distant :
- `git ls-remote`

Récupérer une branche distante :
- `git fetch origin <branch-name>`

Créer une branche à partir d'une branche distante :
- `git checkout --track origin/<branch-name>`

Comparer 2 branches :
- `git diff <branch-1> <branch-2>`

Voir les fichiers modifiés entre 2 commits :
- `git diff --stat <commit-SHA-1> <commit-SHA-2>`

Voir l'historique sur une ligne :
- `git log --oneline`

Voir l'historique de **tous** les changements :
- `git reflog`

# Le commit

# Le travail avec les branches

# L'historique

# L'affichage des différences
