## Pourquoi Docker répond au pb ?
 * container : boîte qui peut faire tourner n'importe quoi
 * container : boîte qui peut être démarrée partout
 * isolation du container. Facilite la configuration réseau, disque, ...
 * automatisation : opération standards pour démarrer / stopper ... un container
 * Performances : peu d'overload
 * séparation des responsabilités : les devs s'occupent du code, les ops s'occupent de l'infra


## Intérêts pour les Dévs
 * on build une fois / on déploie n'importe où (dev/recette/prod)
 * pas de pbs de dépendances lors d'un déploiement
 * possibilité de prendre une snapshot d'un container pour le redémarrer ailleurs
 * pas de pbs de conflits entre les dépendances de 2 applications
 * on peut tout scripter pour automatiser le déploiement, les tests, etc...
 * réduit les pbs de compatibilité entre les différents environnements
 * pas de pbs de performances. permet de démarrer une application rapidement.
Note : on a déjà tous eu un pb reproduit uniquement en recette car l'environnement n'était pas configuré comme la dev.


## Intérêts pour les ops
 * 1 seule configuration pour démarrer n'importe quoi
 * plus de différence entre les environnements de dev/rec/prod.
 * Améliore le temps de mise en place des environnements
 * Plus performant qu'une VM mais règle la plupart des problèmes d'isolation


## Différence entre VM et Container
 * Pas de Guest OS à charger
 * bin et lib partagés.
![containers-vs-vms](data/comment/containers-vs-vms.png)
 * démarre rapidement
 * moins gourmand en resources


## Pourquoi une image Docker est légère
![why-are-containers-lightwight](data/comment/why-are-containers-lightwight.png)


## Fonctionnement général
![basics-of-docker-system](data/comment/basics-of-docker-system.png)


## Mise à jour d'une image
![changes-and-updates](data/comment/changes-and-updates.png)

# dans la vraie vie
 - schéma
 - images / registry / container / hub
