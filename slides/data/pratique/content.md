## Ok... On rentre dans le vif du sujet !
![](data/pratique/pratique.gif)


## Définitions
* <!-- .element: class="fragment" -->**Image** - Ensemble d'un filesystem et de paramètres d'éxecution. N'a pas d'état et est immuable
* <!-- .element: class="fragment" -->**Container** - Instance d'une image
* <!-- .element: class="fragment" -->**Dockerfile** - Script pour créer une image
* <!-- .element: class="fragment" -->**Index** - Registre d'images Docker
* <!-- .element: class="fragment" -->**Push / Pull** - Commandes pour charger ou créer des images dans l'index
* <!-- .element: class="fragment" -->**Run** - Démarrer une image dans un nouveau container


## Fonctionnement général
![](data/comment/basics-of-docker-system.png)


## search
Permet de rechercher une image dans le docker hub
```sh
docker search postgres
```


## pull
Permet de télécharger une image depuis un repository
```sh
docker pull postgres:9.5.3
```


## images
Permet de lister les images présentes en local
```sh
docker images -a
```


## run
Permet de démarrer une image dans un container
```sh
docker run postgres:9.5.3
```
* <!-- .element: class="fragment" --> **-d** &mdash; mode daemon
* <!-- .element: class="fragment" --> **-t** &mdash; mode tty
* <!-- .element: class="fragment" --> **-i** &mdash; mode interactive
* <!-- .element: class="fragment" --> **-e** &mdash; variable d'environnement
* <!-- .element: class="fragment" --> **-v** &mdash; volume
* <!-- .element: class="fragment" --> **--name database** &mdash; nom du container
* <!-- .element: class="fragment" --> **--link database:database** &mdash; lien vers un autre container


## ps
Permet de lister les containers
```sh
docker ps -a


## inspect
Permet de récupérer des informations sur un container
```sh
docker inspect database
```


## exec
Permet d''executer une commande
```sh
docker exec -it database /bin/bash
```


## Docker File
Démo


## build
Permet de construire une image
```sh
docker build --build-arg HTTP_PROXY=http://proxy:80 -t alocquet/midi-tech-first:1.0 .
```
Note: On voit les images intermediaires.


## stop/start
Arrête/Démarre un container


# Docker trusted registry
 * Gérer une bibliothèque d'images
 * Serveur installé pour une entreprise
 * équivalent du repository maven

#Docker hub
 * Repository public
 * https://hub.docker.com/


# Upload d'une image
```sh
echo "http_proxy=http://****:8080" > ... TODO
docker build -t midi-tech-first:1.0 .
docker tag midi-tech-first:1.0 alocquet/midi-tech-first:1.0
docker push alocquet/midi-tech-first:1.0
```
