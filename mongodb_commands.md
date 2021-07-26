Afficher les BDD :
- `show dbs`

Utiliser une BDD :
- `use` <database-name>

Afficher les collections :
- `show collections`

Afficher les documents d'une collection :
- `db.<collection-name>.find().toArray()`

Compter les documents d'une collection :
- `db.<collection-name>.count()`

Afficher le dernier document inséré :
- `db.<collection-name>.find().sort( { "_id": -1 } ).limit(1).toArray()`

Afficher les 2 derniers documents insérés :
- `db.<collection-name>.find().skip(db.<collection-name>.count() - 2).toArray()`

Exporter les données d'une collection :
- `mongoexport --collection=<collection-name> --db=<database-name> --pretty --out=<filename.extension>`

Supprimer un document :
- `db.<collection-name>.deleteOne(<filter>)`

Supprimer des documents :
- `db.<collection-name>.deleteMany(<filter>)`

Créer un index :
- `db.<collection-name>.ensureIndex(keys, options)`

Afficher la liste des index sur une collection :
- `db.<collection-name>.getIndexes()`

Supprimer un index :
- `db.<collection-name>.dropIndex(<index-name>)`
- `db.<collection-name>.dropIndexes(<index-name>)`
