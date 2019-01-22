# L'interface List<E>

**CopyOnWriteArrayList<E>** est une variante **thread-safe** de l'objet ArrayList.

- Avantage : Efficace en environnement multithread.

- Inconvénient : Très coûteux en temps et en mémoire.

# L'interface Set<E>
Une collection de type **Set** représente une structure qui ne supporte pas les valeurs dupliquées.

3 implémentations générales facilement utilisables de l'interface Set :
- TreeSet<E>
- HashSet<E>
- LinkedHashSet<E>

## L'objet HashSet<E>
Il utilise le principe de **table de hachage**.

Spécificités de stockage dans une table de hachage :
1. Les données sont gérées sous la forme **clé-valeur**.
2. Les données sont rangées dans un **bucket array**, en fonction de leur **code de hachage**, code retourné par la méthode `hashCode()`de chaque objet.

    Voilà pourquoi il est important de redéfinir la méthode `hashCode()` dans nos objets !

## L'objet LinkedHashSet<E>
Intermédiaire entre le HashSet<E> et le TreeSet<E>, il stocke les données sous la forme de table de hachage, mais gère aussi l'insertion de façon ordonnée.

- Avantage : Améliore les performances en lecture et écriture par rapport à HashSet<E>.