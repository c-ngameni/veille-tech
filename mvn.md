Construire un module particulier :
- `mvn clean package --projects <module> --also-make -DskipTests`

Exécuter les tests d'un paquetage :
- `mvn -Dtest=package.*Test test`
