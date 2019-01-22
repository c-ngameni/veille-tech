- Cloner un dépôt dans un nouveau répertoire

`git clone` *nom-du-dossier*
- Créer une branche

`git branch` **nom-de-la-branche**
- Se positionner sur une branche

`git checkout` __nom-de-la-branche__
- Créer une branche, puis se positionner dessus

`git checkout -b <nom-de-la-branche>`
- Se re-positionner sur la branche précédente

`git checkout @{-1}` | `git checkout -`
- Renommer une branche

`git branch -m <nouveau-nom*>`
- Fusionner 2 branches

`git merge <nom-de-la-branche>`
- Fusionner 2 branches sans faire un commit de merge

`git rebase <nom-de-la-branche>`

`git rebase --continue` *en cas de conflits*

`git push --force`
- Supprimer une branche

`git branch -d <nom-de-la-branche>`
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

`git push --set-upstream origin <nom-de-la-branche>`
- Appliquer sur une branche les modifications propres à un commit (sur une autre branche)

`git cherry-pick -n`
- Retrouver l'auteur d'une modification

`git blame <nom-du-fichier.extension>`
- Ajouter un fichier à committer

`git add <nom-du-fichier>`
- Retirer un fichier avant de committer

`git reset <nom-du-fichier>`