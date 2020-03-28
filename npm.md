-  Installer les dépendances

`npm install`

- Installer et enregistrer une dépendance (mise à jour du champ **dependencies** de package.json)

`npm install <dependencie-name> --save`

- Installer et enregistrer une dépendance de développement (mise à jour du champ **devDependencies** de package.json)

`npm install <dependencie-name> --save-dev`

- Lancer le serveur NodeJS

`npm start`

`npm prune`

`npm run build`

- Récupérer le proxy

`npm config get proxy`

- Récupérer l'ensemble des configurations de NodeJS

`npm config ls -l`

- Vérifier la version d'Angular-cli

`ng --version`

- Générer un fichier avec l'extension *model*.ts

`ng generate class <file-name> --type=`*model*

- Générer un composant sans le fichier de test

`ng generate component <component-name> --no-spec`