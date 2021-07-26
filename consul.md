Lancer l'agent Consul :
- `consul agent -dev`

Charger une configuration :
- `consul kv import @<filename>`

Supprimer une clé :
- `consul kv delete <path-to-key>`

Supprimer les clés rattachées à un préfixe :
- `consul kv delete --recurse <prefix>`
