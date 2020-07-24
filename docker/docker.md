Constuire une image Docker :
- docker build -t [name] [Dockerfile-directory]

Lancer un conteneur en arrière-plan :
- docker run -d --name [container-name] -p [external-port]:[internal-port] [image-name]

Vérifier les logs d'un conteneur:
- docker logs [container-name]

Ouvrir un terminal interactif dans un conteneur et exécuter un processus (bash par exemple)
- docker exec -it [container-name] [process-name]
- `exit` pour sortir du terminal
