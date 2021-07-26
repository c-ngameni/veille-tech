Constuire une image Docker :
- `docker build -t <name> <Dockerfile-directory>`

Lancer un conteneur :
- `docker run -p <external-port>:<internal-port> <image-name>`

Lancer un conteneur en arrière-plan :
- `docker run -d --name <container-name> -p <external-port>:<internal-port> <image-name>`

Vérifier les logs d'un conteneur :
- `docker logs <container-name>`

Ouvrir un terminal interactif dans un conteneur et exécuter un processus (bash par exemple) :
- `docker exec -it <container-name> <process-name>`
- `exit` pour sortir du terminal
- Ctrl + P + Q pour sortir d'un conteneur sans l'arrêter

Afficher la liste des conteneurs :
- `docker container ls`

Lancer un conteneur :
- `docker container start <container-name>`

Arrêter un conteneur :
`docker container stop <container-name>`

Supprimer un conteneur :
- `docker container rm <container-name>`
